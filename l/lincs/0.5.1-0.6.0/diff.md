# Comparing `tmp/lincs-0.5.1.tar.gz` & `tmp/lincs-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lincs-0.5.1.tar", last modified: Tue Jul 25 15:45:12 2023, max compression
+gzip compressed data, was "lincs-0.6.0.tar", last modified: Fri Jul 28 14:09:21 2023, max compression
```

## Comparing `lincs-0.5.1.tar` & `lincs-0.6.0.tar`

### file list

```diff
@@ -1,248 +1,332 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.037627 lincs-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-07-25 15:45:05.000000 lincs-0.5.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (122)     7652 2023-07-25 15:45:05.000000 lincs-0.5.1/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (122)      122 2023-07-25 15:45:05.000000 lincs-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5191 2023-07-25 15:45:12.037627 lincs-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4307 2023-07-25 15:45:05.000000 lincs-0.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.961627 lincs-0.5.1/lincs/
--rw-r--r--   0 runner    (1001) docker     (122)     1218 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      170 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    26193 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/command_line_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.965627 lincs-0.5.1/lincs/liblincs/
--rw-r--r--   0 runner    (1001) docker     (122)     5634 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/classification.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      369 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/classification.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    18418 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/generation.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/generation.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.969627 lincs-0.5.1/lincs/liblincs/io/
--rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/io/alternatives.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/io/alternatives.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     8247 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/io/model.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3158 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/io/model.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     4909 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/io/problem.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2038 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/io/problem.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/io/validation.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      583 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/io/validation.hpp
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/io.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      187 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/io.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.969627 lincs-0.5.1/lincs/liblincs/learning/
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/exception.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      477 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/exception.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.957627 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.969627 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/breed/
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/breed/reinitialize-least-accurate.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/breed/reinitialize-least-accurate.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.969627 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.969627 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic/
--rw-r--r--   0 runner    (1001) docker     (122)     1575 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic/desirability.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     9322 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-cpu.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    14371 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-gpu.cu
--rw-r--r--   0 runner    (1001) docker     (122)     1935 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-gpu.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.969627 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/
--rw-r--r--   0 runner    (1001) docker     (122)     4508 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1226 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.969627 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/
--rw-r--r--   0 runner    (1001) docker     (122)     4107 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/linear-program.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      838 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/linear-program.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.973627 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/
--rw-r--r--   0 runner    (1001) docker     (122)      901 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-iterations.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      913 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-seconds.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      211 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/at-accuracy.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      779 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/at-accuracy.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      295 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/composite.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      824 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/composite.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     7049 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4324 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     9825 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/ucncs-by-sat-by-coalitions.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      591 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/ucncs-by-sat-by-coalitions.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    11262 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1627 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    23065 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/liblincs_module.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      245 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/lincs.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.973627 lincs-0.5.1/lincs/liblincs/linear-programming/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/linear-programming/alglib.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2731 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/linear-programming/alglib.hpp
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/linear-programming/glop.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1817 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/linear-programming/glop.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/linear-programming/test.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      785 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/randomness-utils.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1736 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/randomness-utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.973627 lincs-0.5.1/lincs/liblincs/sat/
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/sat/eval-max-sat.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1665 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/sat/eval-max-sat.hpp
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/sat/minisat.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1341 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/sat/minisat.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2555 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/sat/test.cpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.977627 lincs-0.5.1/lincs/liblincs/vendored/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.005627 lincs-0.5.1/lincs/liblincs/vendored/alglib/
--rwxr-xr-x   0 runner    (1001) docker     (122)   615853 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/alglibinternal.cpp
--rwxr-xr-x   0 runner    (1001) docker     (122)    65139 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/alglibinternal.h
--rwxr-xr-x   0 runner    (1001) docker     (122)   322558 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/alglibmisc.cpp
--rwxr-xr-x   0 runner    (1001) docker     (122)    88614 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/alglibmisc.h
--rwxr-xr-x   0 runner    (1001) docker     (122)   493278 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/ap.cpp
--rwxr-xr-x   0 runner    (1001) docker     (122)   179632 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/ap.h
--rwxr-xr-x   0 runner    (1001) docker     (122)  1927587 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/dataanalysis.cpp
--rwxr-xr-x   0 runner    (1001) docker     (122)   438786 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/dataanalysis.h
--rwxr-xr-x   0 runner    (1001) docker     (122)    46242 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/diffequations.cpp
--rwxr-xr-x   0 runner    (1001) docker     (122)    10465 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/diffequations.h
--rwxr-xr-x   0 runner    (1001) docker     (122)   126902 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/fasttransforms.cpp
--rwxr-xr-x   0 runner    (1001) docker     (122)    27863 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/fasttransforms.h
--rwxr-xr-x   0 runner    (1001) docker     (122)   149125 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/integration.cpp
--rwxr-xr-x   0 runner    (1001) docker     (122)    33746 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/integration.h
--rwxr-xr-x   0 runner    (1001) docker     (122)  2674150 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/interpolation.cpp
--rwxr-xr-x   0 runner    (1001) docker     (122)   500164 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/interpolation.h
--rwxr-xr-x   0 runner    (1001) docker     (122)    76185 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/kernels_avx2.cpp
--rwxr-xr-x   0 runner    (1001) docker     (122)     7372 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/kernels_avx2.h
--rwxr-xr-x   0 runner    (1001) docker     (122)    39356 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/kernels_fma.cpp
--rwxr-xr-x   0 runner    (1001) docker     (122)     4704 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/kernels_fma.h
--rwxr-xr-x   0 runner    (1001) docker     (122)    23798 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/kernels_sse2.cpp
--rwxr-xr-x   0 runner    (1001) docker     (122)     4058 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/kernels_sse2.h
--rwxr-xr-x   0 runner    (1001) docker     (122)  2288262 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/linalg.cpp
--rwxr-xr-x   0 runner    (1001) docker     (122)   403192 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/linalg.h
--rwxr-xr-x   0 runner    (1001) docker     (122)  3545102 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/optimization.cpp
--rwxr-xr-x   0 runner    (1001) docker     (122)   608685 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/optimization.h
--rwxr-xr-x   0 runner    (1001) docker     (122)   752491 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/solvers.cpp
--rwxr-xr-x   0 runner    (1001) docker     (122)   198547 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/solvers.h
--rwxr-xr-x   0 runner    (1001) docker     (122)   339371 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/specialfunctions.cpp
--rwxr-xr-x   0 runner    (1001) docker     (122)    77195 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/specialfunctions.h
--rwxr-xr-x   0 runner    (1001) docker     (122)   612951 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/statistics.cpp
--rwxr-xr-x   0 runner    (1001) docker     (122)    56614 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/statistics.h
--rwxr-xr-x   0 runner    (1001) docker     (122)        4 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/stdafx.h
--rw-r--r--   0 runner    (1001) docker     (122)   321644 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/doctest.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.009627 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/
--rw-r--r--   0 runner    (1001) docker     (122)    30725 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/EvalMaxSAT.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.009627 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/MaLib/
--rw-r--r--   0 runner    (1001) docker     (122)     3857 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/MaLib/Chrono.h
--rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/MaLib/View.h
--rw-r--r--   0 runner    (1001) docker     (122)     3617 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/MaLib/communicationlist.h
--rw-r--r--   0 runner    (1001) docker     (122)     6040 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/MaLib/coutUtil.h
--rw-r--r--   0 runner    (1001) docker     (122)      437 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/MaLib/math.h
--rw-r--r--   0 runner    (1001) docker     (122)     8586 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/card_oe.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4176 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/card_oe.h
--rw-r--r--   0 runner    (1001) docker     (122)     7315 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/cardincremental.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5242 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/cardincremental.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.957627 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.013627 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/core/
--rw-r--r--   0 runner    (1001) docker     (122)     5770 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/core/BoundedQueue.h
--rw-r--r--   0 runner    (1001) docker     (122)     3208 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/core/Constants.h
--rw-r--r--   0 runner    (1001) docker     (122)     3293 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/core/Dimacs.h
--rw-r--r--   0 runner    (1001) docker     (122)    68578 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/core/Solver.cc
--rw-r--r--   0 runner    (1001) docker     (122)    35867 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/core/Solver.h
--rw-r--r--   0 runner    (1001) docker     (122)     4067 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/core/SolverStats.h
--rw-r--r--   0 runner    (1001) docker     (122)    20417 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/core/SolverTypes.h
--rw-r--r--   0 runner    (1001) docker     (122)    17254 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/core/lcm.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.017627 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/
--rw-r--r--   0 runner    (1001) docker     (122)     2814 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Alg.h
--rw-r--r--   0 runner    (1001) docker     (122)     4768 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Alloc.h
--rw-r--r--   0 runner    (1001) docker     (122)      166 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Clone.h
--rw-r--r--   0 runner    (1001) docker     (122)     4772 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Heap.h
--rw-r--r--   0 runner    (1001) docker     (122)     1825 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/IntTypes.h
--rw-r--r--   0 runner    (1001) docker     (122)     6949 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Map.h
--rw-r--r--   0 runner    (1001) docker     (122)     3162 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Queue.h
--rw-r--r--   0 runner    (1001) docker     (122)     3276 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Sort.h
--rw-r--r--   0 runner    (1001) docker     (122)     5992 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Vec.h
--rw-r--r--   0 runner    (1001) docker     (122)     7663 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/VecThreads.h
--rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/XAlloc.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.021627 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/
--rw-r--r--   0 runner    (1001) docker     (122)     9383 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/ClausesBuffer.cc
--rw-r--r--   0 runner    (1001) docker     (122)     5078 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/ClausesBuffer.h
--rw-r--r--   0 runner    (1001) docker     (122)    24142 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/MultiSolvers.cc
--rw-r--r--   0 runner    (1001) docker     (122)     8631 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/MultiSolvers.h
--rw-r--r--   0 runner    (1001) docker     (122)    20252 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/ParallelSolver.cc
--rw-r--r--   0 runner    (1001) docker     (122)     6800 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/ParallelSolver.h
--rw-r--r--   0 runner    (1001) docker     (122)     6558 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SharedCompanion.cc
--rw-r--r--   0 runner    (1001) docker     (122)     6099 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SharedCompanion.h
--rw-r--r--   0 runner    (1001) docker     (122)     3923 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SolverCompanion.cc
--rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SolverCompanion.h
--rw-r--r--   0 runner    (1001) docker     (122)     7213 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SolverConfiguration.cc
--rw-r--r--   0 runner    (1001) docker     (122)     3471 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SolverConfiguration.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.021627 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/simp/
--rw-r--r--   0 runner    (1001) docker     (122)    25949 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/simp/SimpSolver.cc
--rw-r--r--   0 runner    (1001) docker     (122)    11769 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/simp/SimpSolver.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.021627 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     3801 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/utils/Options.cc
--rw-r--r--   0 runner    (1001) docker     (122)    12150 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/utils/Options.h
--rw-r--r--   0 runner    (1001) docker     (122)     5376 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/utils/ParseUtils.h
--rw-r--r--   0 runner    (1001) docker     (122)     3135 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/utils/System.cc
--rw-r--r--   0 runner    (1001) docker     (122)     2707 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/utils/System.h
--rw-r--r--   0 runner    (1001) docker     (122)     1645 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/lazyvariable.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1201 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/lazyvariable.h
--rw-r--r--   0 runner    (1001) docker     (122)     8639 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/mcqd.h
--rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/monglucose41.h
--rw-r--r--   0 runner    (1001) docker     (122)      545 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/virtualcard.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/virtualcard.h
--rw-r--r--   0 runner    (1001) docker     (122)     3281 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/virtualmaxsat.h
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/virtualsat.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5039 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/virtualsat.h
--rw-r--r--   0 runner    (1001) docker     (122)    39756 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/lov-e.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    62179 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/magic_enum.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.961627 lincs-0.5.1/lincs/liblincs/vendored/minisat/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.025627 lincs-0.5.1/lincs/liblincs/vendored/minisat/core/
--rw-r--r--   0 runner    (1001) docker     (122)    34973 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/core/Solver.cc
--rw-r--r--   0 runner    (1001) docker     (122)    24022 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/core/Solver.h
--rw-r--r--   0 runner    (1001) docker     (122)    17280 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/core/SolverTypes.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.025627 lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/
--rw-r--r--   0 runner    (1001) docker     (122)     2839 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/Alg.h
--rw-r--r--   0 runner    (1001) docker     (122)     4379 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/Alloc.h
--rw-r--r--   0 runner    (1001) docker     (122)     5344 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/Heap.h
--rw-r--r--   0 runner    (1001) docker     (122)     4204 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/IntMap.h
--rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/IntTypes.h
--rw-r--r--   0 runner    (1001) docker     (122)     6682 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/Map.h
--rw-r--r--   0 runner    (1001) docker     (122)     3001 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/Queue.h
--rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/Rnd.h
--rw-r--r--   0 runner    (1001) docker     (122)     3276 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/Sort.h
--rw-r--r--   0 runner    (1001) docker     (122)     5588 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/Vec.h
--rw-r--r--   0 runner    (1001) docker     (122)     1924 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/XAlloc.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.029627 lincs-0.5.1/lincs/liblincs/vendored/minisat/simp/
--rw-r--r--   0 runner    (1001) docker     (122)    22244 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/simp/SimpSolver.cc
--rw-r--r--   0 runner    (1001) docker     (122)    10816 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/simp/SimpSolver.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.029627 lincs-0.5.1/lincs/liblincs/vendored/minisat/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     3816 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/utils/Options.cc
--rw-r--r--   0 runner    (1001) docker     (122)    12153 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/utils/Options.h
--rw-r--r--   0 runner    (1001) docker     (122)     4164 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/utils/ParseUtils.h
--rw-r--r--   0 runner    (1001) docker     (122)     5266 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/utils/System.cc
--rw-r--r--   0 runner    (1001) docker     (122)     3088 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/utils/System.h
--rw-r--r--   0 runner    (1001) docker     (122)    57901 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/rapidcsv.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.033627 lincs-0.5.1/lincs/liblincs/vendored/valijson/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.033627 lincs-0.5.1/lincs/liblincs/vendored/valijson/adapters/
--rw-r--r--   0 runner    (1001) docker     (122)     9433 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/adapters/std_string_adapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    19320 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/adapters/yaml_cpp_adapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      318 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/constraint_builder.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.033627 lincs-0.5.1/lincs/liblincs/vendored/valijson/constraints/
--rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/constraints/basic_constraint.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    34401 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/constraints/concrete_constraints.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/constraints/constraint.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     4649 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/constraints/constraint_visitor.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      856 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/exceptions.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.037627 lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/
--rw-r--r--   0 runner    (1001) docker     (122)    16614 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/adapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    25566 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/basic_adapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2355 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/custom_allocator.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      649 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/debug.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/frozen_value.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    10088 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/json_pointer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1694 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/json_reference.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      339 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/optional.hpp
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/optional_bundled.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1206 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/uri.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     6144 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/schema.hpp
--rw-r--r--   0 runner    (1001) docker     (122)   102841 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/schema_parser.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     8346 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/subschema.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.037627 lincs-0.5.1/lincs/liblincs/vendored/valijson/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/utils/file_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1378 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/utils/utf8_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2488 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/validation_results.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    68300 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/validation_visitor.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2250 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/validator.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    25311 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs_module_tests.py
--rw-r--r--   0 runner    (1001) docker     (122)     1184 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.965627 lincs-0.5.1/lincs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5191 2023-07-25 15:45:11.000000 lincs-0.5.1/lincs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10855 2023-07-25 15:45:11.000000 lincs-0.5.1/lincs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-25 15:45:11.000000 lincs-0.5.1/lincs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-25 15:45:11.000000 lincs-0.5.1/lincs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-07-25 15:45:11.000000 lincs-0.5.1/lincs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-25 15:45:11.000000 lincs-0.5.1/lincs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-25 15:45:05.000000 lincs-0.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-25 15:45:12.037627 lincs-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4706 2023-07-25 15:45:05.000000 lincs-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 14:09:21.235996 lincs-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-07-28 14:09:15.000000 lincs-0.6.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (122)     7652 2023-07-28 14:09:15.000000 lincs-0.6.0/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (122)      122 2023-07-28 14:09:15.000000 lincs-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5191 2023-07-28 14:09:21.235996 lincs-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4307 2023-07-28 14:09:15.000000 lincs-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 14:09:21.175995 lincs-0.6.0/lincs/
+-rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      170 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26182 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/command_line_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 14:09:21.175995 lincs-0.6.0/lincs/liblincs/
+-rw-r--r--   0 runner    (1001) docker     (122)     5634 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/classification.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      369 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/classification.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    18418 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/generation.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/generation.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 14:09:21.179995 lincs-0.6.0/lincs/liblincs/io/
+-rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/io/alternatives.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/io/alternatives.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8247 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/io/model.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3158 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/io/model.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4909 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/io/problem.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2038 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/io/problem.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/io/validation.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      583 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/io/validation.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/io.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      187 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/io.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 14:09:21.179995 lincs-0.6.0/lincs/liblincs/learning/
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/learning/exception.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      477 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/learning/exception.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 14:09:21.171995 lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 14:09:21.179995 lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/breed/
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/breed/reinitialize-least-accurate.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/breed/reinitialize-least-accurate.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 14:09:21.179995 lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 14:09:21.179995 lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic/
+-rw-r--r--   0 runner    (1001) docker     (122)     1575 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic/desirability.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9322 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-cpu.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    14371 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-gpu.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     1935 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-gpu.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 14:09:21.179995 lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/
+-rw-r--r--   0 runner    (1001) docker     (122)     4508 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1226 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 14:09:21.179995 lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/
+-rw-r--r--   0 runner    (1001) docker     (122)     4107 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/linear-program.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      838 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/linear-program.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 14:09:21.179995 lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/
+-rw-r--r--   0 runner    (1001) docker     (122)      901 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-iterations.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      913 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-seconds.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      211 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/at-accuracy.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      779 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/at-accuracy.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      295 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/composite.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/composite.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7049 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4324 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8810 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/learning/ucncs-by-sat-by-coalitions.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      593 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/learning/ucncs-by-sat-by-coalitions.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10536 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/learning/ucncs-by-sat-by-separation.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      593 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/learning/ucncs-by-sat-by-separation.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    12777 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/learning.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/learning.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    23056 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/liblincs_module.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      245 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/lincs.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 14:09:21.183995 lincs-0.6.0/lincs/liblincs/linear-programming/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/linear-programming/alglib.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2731 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/linear-programming/alglib.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/linear-programming/glop.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1817 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/linear-programming/glop.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/linear-programming/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      785 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/randomness-utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1736 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/randomness-utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 14:09:21.183995 lincs-0.6.0/lincs/liblincs/sat/
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/sat/eval-max-sat.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1670 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/sat/eval-max-sat.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/sat/minisat.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1341 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/sat/minisat.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2814 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/sat/test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 14:09:21.183995 lincs-0.6.0/lincs/liblincs/vendored/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 14:09:21.207996 lincs-0.6.0/lincs/liblincs/vendored/alglib/
+-rwxr-xr-x   0 runner    (1001) docker     (122)   615853 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/alglibinternal.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)    65139 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/alglibinternal.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)   322558 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/alglibmisc.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)    88614 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/alglibmisc.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)   493278 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/ap.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)   179632 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/ap.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)  1927587 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/dataanalysis.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)   438786 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/dataanalysis.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)    46242 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/diffequations.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10465 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/diffequations.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)   126902 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/fasttransforms.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)    27863 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/fasttransforms.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)   149125 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/integration.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)    33746 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/integration.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)  2674150 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/interpolation.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)   500164 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/interpolation.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)    76185 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/kernels_avx2.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7372 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/kernels_avx2.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)    39356 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/kernels_fma.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4704 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/kernels_fma.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)    23798 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/kernels_sse2.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4058 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/kernels_sse2.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)  2288262 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/linalg.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)   403192 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/linalg.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)  3545102 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/optimization.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)   608685 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/optimization.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)   752491 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/solvers.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)   198547 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/solvers.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)   339371 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/specialfunctions.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)    77195 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/specialfunctions.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)   612951 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/statistics.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)    56614 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/statistics.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)        4 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/alglib/stdafx.h
+-rw-r--r--   0 runner    (1001) docker     (122)   321644 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/doctest.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 14:09:21.207996 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/
+-rw-r--r--   0 runner    (1001) docker     (122)    55416 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/EvalMaxSAT.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 14:09:21.211995 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/MaLib/
+-rw-r--r--   0 runner    (1001) docker     (122)     4149 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/MaLib/Chrono.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/MaLib/View.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3433 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/MaLib/communicationlist.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6108 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/MaLib/coutUtil.h
+-rw-r--r--   0 runner    (1001) docker     (122)      437 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/MaLib/math.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4740 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/ParseUtils.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 14:09:21.227996 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/
+-rw-r--r--   0 runner    (1001) docker     (122)    25604 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/analyze.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/arena.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3628 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/arena.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6494 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/assume.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      779 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/averages.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      776 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/averages.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4207 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/backtrack.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4552 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/backward.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      456 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/bins.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/bins.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    22171 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/block.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      702 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/block.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    32258 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/cadical.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    36627 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/cadical.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4589 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/ccadical.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/ccadical.h
+-rw-r--r--   0 runner    (1001) docker     (122)    15910 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/checker.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5625 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/checker.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    13294 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/clause.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6936 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/clause.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    13934 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/collect.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    13886 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/compact.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    33283 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/condition.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2534 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/config.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      295 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/config.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/constrain.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      598 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/contract.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3948 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/contract.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    18900 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/cover.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1167 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/cover.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5136 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/decide.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    12205 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/decompose.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4154 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/deduplicate.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    31395 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/elim.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/elim.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3363 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/ema.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/ema.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6400 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/extend.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    18647 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/external.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    13200 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/external.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9153 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/file.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4755 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/file.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2706 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/flags.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2339 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/flags.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1752 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/format.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      888 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/format.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    14615 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/gates.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5517 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/heap.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7844 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/instantiate.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1289 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/instantiate.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    23025 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/internal.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    46902 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/internal.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1036 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/inttypes.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/ipasir.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1388 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/ipasir.h
+-rw-r--r--   0 runner    (1001) docker     (122)      744 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/level.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3254 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/limit.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2273 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/limit.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3470 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/logging.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2566 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/logging.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    13438 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/lookahead.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10326 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/lucky.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4555 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/message.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      985 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/message.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/minimize.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    96578 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/mobical.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      717 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/observer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      867 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/occs.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      784 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/occs.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10113 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/options.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    18179 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/options.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    11233 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/parse.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2539 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/parse.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      970 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/phases.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/phases.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    22375 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/probe.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2888 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/profile.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8255 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/profile.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5085 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/proof.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/proof.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    13080 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/propagate.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2482 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/queue.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1569 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/queue.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5291 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/radix.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5688 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/random.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2162 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/random.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3479 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/range.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2768 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/reap.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/reap.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7059 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/reduce.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/reluctant.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8110 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/rephase.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7951 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/report.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3711 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/resources.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/resources.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4409 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/restart.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7472 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/restore.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/score.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/score.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    13508 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/shrink.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2856 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/signal.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      524 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/signal.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1585 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/solution.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    38991 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/solver.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    24693 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/stats.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10368 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/stats.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    21919 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/subsume.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      731 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/terminal.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2813 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/terminal.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    12729 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/ternary.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2096 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/tracer.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      640 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/tracer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6326 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/transred.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3496 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/util.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3965 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/util.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      920 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/var.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      476 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/var.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2646 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/version.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      202 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/version.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    36971 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/vivify.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/vivify.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    20435 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/walk.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2345 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/watch.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1346 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/watch.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5020 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadicalinterface.h
+-rw-r--r--   0 runner    (1001) docker     (122)     8590 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/card_oe.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4194 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/card_oe.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4707 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cardincremental.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3946 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cardincremental.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1599 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/lazyvariable.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1445 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/lazyvariable.h
+-rw-r--r--   0 runner    (1001) docker     (122)     8639 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/mcqd.h
+-rw-r--r--   0 runner    (1001) docker     (122)      190 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/virtualcard.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      851 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/virtualcard.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4445 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/virtualmaxsat.h
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/virtualsat.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2043 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/virtualsat.h
+-rw-r--r--   0 runner    (1001) docker     (122)    39756 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/lov-e.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    62179 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/magic_enum.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 14:09:21.171995 lincs-0.6.0/lincs/liblincs/vendored/minisat/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 14:09:21.227996 lincs-0.6.0/lincs/liblincs/vendored/minisat/core/
+-rw-r--r--   0 runner    (1001) docker     (122)    34973 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/minisat/core/Solver.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    24022 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/minisat/core/Solver.h
+-rw-r--r--   0 runner    (1001) docker     (122)    17280 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/minisat/core/SolverTypes.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 14:09:21.231996 lincs-0.6.0/lincs/liblincs/vendored/minisat/mtl/
+-rw-r--r--   0 runner    (1001) docker     (122)     2839 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/minisat/mtl/Alg.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4379 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/minisat/mtl/Alloc.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5344 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/minisat/mtl/Heap.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4204 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/minisat/mtl/IntMap.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/minisat/mtl/IntTypes.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6682 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/minisat/mtl/Map.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3001 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/minisat/mtl/Queue.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/minisat/mtl/Rnd.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3276 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/minisat/mtl/Sort.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5588 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/minisat/mtl/Vec.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1924 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/minisat/mtl/XAlloc.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 14:09:21.231996 lincs-0.6.0/lincs/liblincs/vendored/minisat/simp/
+-rw-r--r--   0 runner    (1001) docker     (122)    22244 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/minisat/simp/SimpSolver.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    10816 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/minisat/simp/SimpSolver.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 14:09:21.231996 lincs-0.6.0/lincs/liblincs/vendored/minisat/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     3816 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/minisat/utils/Options.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    12153 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/minisat/utils/Options.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4164 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/minisat/utils/ParseUtils.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5266 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/minisat/utils/System.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     3088 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/minisat/utils/System.h
+-rw-r--r--   0 runner    (1001) docker     (122)    57901 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/rapidcsv.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 14:09:21.231996 lincs-0.6.0/lincs/liblincs/vendored/valijson/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 14:09:21.231996 lincs-0.6.0/lincs/liblincs/vendored/valijson/adapters/
+-rw-r--r--   0 runner    (1001) docker     (122)     9433 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/valijson/adapters/std_string_adapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    19320 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/valijson/adapters/yaml_cpp_adapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/valijson/constraint_builder.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 14:09:21.231996 lincs-0.6.0/lincs/liblincs/vendored/valijson/constraints/
+-rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/valijson/constraints/basic_constraint.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    34401 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/valijson/constraints/concrete_constraints.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/valijson/constraints/constraint.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4649 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/valijson/constraints/constraint_visitor.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      856 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/valijson/exceptions.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 14:09:21.235996 lincs-0.6.0/lincs/liblincs/vendored/valijson/internal/
+-rw-r--r--   0 runner    (1001) docker     (122)    16614 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/valijson/internal/adapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    25566 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/valijson/internal/basic_adapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2355 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/valijson/internal/custom_allocator.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      649 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/valijson/internal/debug.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/valijson/internal/frozen_value.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10088 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/valijson/internal/json_pointer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1694 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/valijson/internal/json_reference.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/valijson/internal/optional.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/valijson/internal/optional_bundled.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1206 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/valijson/internal/uri.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6144 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/valijson/schema.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)   102841 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/valijson/schema_parser.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8346 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/valijson/subschema.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 14:09:21.235996 lincs-0.6.0/lincs/liblincs/vendored/valijson/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/valijson/utils/file_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1378 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/valijson/utils/utf8_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2488 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/valijson/validation_results.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    68300 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/valijson/validation_visitor.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2250 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs/vendored/valijson/validator.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    25322 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/liblincs_module_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1184 2023-07-28 14:09:15.000000 lincs-0.6.0/lincs/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 14:09:21.175995 lincs-0.6.0/lincs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5191 2023-07-28 14:09:21.000000 lincs-0.6.0/lincs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    15573 2023-07-28 14:09:21.000000 lincs-0.6.0/lincs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-28 14:09:21.000000 lincs-0.6.0/lincs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-28 14:09:21.000000 lincs-0.6.0/lincs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-07-28 14:09:21.000000 lincs-0.6.0/lincs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-28 14:09:21.000000 lincs-0.6.0/lincs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-28 14:09:15.000000 lincs-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-28 14:09:21.235996 lincs-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4991 2023-07-28 14:09:15.000000 lincs-0.6.0/setup.py
```

### Comparing `lincs-0.5.1/COPYING` & `lincs-0.6.0/COPYING`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/COPYING.LESSER` & `lincs-0.6.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/PKG-INFO` & `lincs-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lincs
-Version: 0.5.1
+Version: 0.6.0
 Summary: Learn and Infer Non Compensatory Sortings
 Home-page: https://github.com/MICS-Lab/lincs
 Author: Vincent Jacques
 Author-email: vincent@vincent-jacques.net
 License: LGPLv3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
@@ -25,15 +25,15 @@
     - on GitHub (https://github.com/mics-lab/lincs/)
     - on PyPI after publication of the package (https://pypi.org/project/lincs/)
     - on GitHub Pages (https://mics-lab.github.io/lincs/)
     So when you change it, take care to check all those places.
 
 *lincs* (Learn and Infer Non Compensatory Sortings) is a collection of MCDA algorithms, usable as a C++ library, a Python (3.7+) package and a command-line utility.
 
-*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v0.5.1/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v0.5.1/COPYING.LESSER>`_.
+*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v0.6.0/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v0.6.0/COPYING.LESSER>`_.
 
 @todo (When we have a paper to actually cite) Add a note asking academics to kindly cite our work.
 
 *lincs* is available for install from the `Python package index <https://pypi.org/project/lincs/>`_.
 Its `documentation <http://mics-lab.github.io/lincs/>`_
 and its `source code <https://github.com/mics-lab/lincs/>`_ are on GitHub.
```

### Comparing `lincs-0.5.1/README.rst` & `lincs-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/__init__.py` & `lincs-0.6.0/lincs/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,10 +21,13 @@
     from liblincs import ImproveProfilesWithAccuracyHeuristicOnGpu
 except ImportError:
     pass
 from liblincs import ReinitializeLeastAccurate
 from liblincs import TerminateAtAccuracy, TerminateAfterSeconds, TerminateAfterIterations, TerminateWhenAny
 
 # Learning - SAT by coalitions
-from liblincs import LearnUcncsBySatByCoalitionsUsingMinisat, LearnUcncsBySatByCoalitionsUsingEvalmaxsat
+from liblincs import LearnUcncsBySatByCoalitionsUsingMinisat
+
+# Learning - SAT by separation
+from liblincs import LearnUcncsBySatBySeparationUsingMinisat
 
 # @todo Accept learning and training set as Pandas DataFrame?
```

### Comparing `lincs-0.5.1/lincs/command_line_interface.py` & `lincs-0.6.0/lincs/command_line_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -582,15 +582,15 @@
             ),
         ],
         "ucncs": [
             (
                 "approach",
                 dict(
                     help="The general approach to transform the learning problem into a satisfiability problem.",
-                    type=click.Choice(["sat-by-coalitions", "max-sat-by-coalitions"]),
+                    type=click.Choice(["sat-by-coalitions", "sat-by-separation"]),
                     default="sat-by-coalitions",
                     show_default=True,
                 ),
                 {},
             ),
         ],
     },
@@ -675,16 +675,16 @@
                 breeding_strategy,
                 termination_strategy,
                 observers,
             )
     elif model_type == "ucncs":
         if ucncs__approach == "sat-by-coalitions":
             learning = lincs.LearnUcncsBySatByCoalitionsUsingMinisat(problem, learning_set)
-        elif ucncs__approach == "max-sat-by-coalitions":
-            learning = lincs.LearnUcncsBySatByCoalitionsUsingEvalmaxsat(problem, learning_set)
+        elif ucncs__approach == "sat-by-separation":
+            learning = lincs.LearnUcncsBySatBySeparationUsingMinisat(problem, learning_set)
 
     model = learning.perform()
     model.dump(problem, output_model)
 
 
 @main.command(
     help="""
```

### Comparing `lincs-0.5.1/lincs/liblincs/classification.cpp` & `lincs-0.6.0/lincs/liblincs/classification.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/generation.cpp` & `lincs-0.6.0/lincs/liblincs/generation.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/generation.hpp` & `lincs-0.6.0/lincs/liblincs/generation.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/io/alternatives.cpp` & `lincs-0.6.0/lincs/liblincs/io/alternatives.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/io/alternatives.hpp` & `lincs-0.6.0/lincs/liblincs/io/alternatives.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/io/model.cpp` & `lincs-0.6.0/lincs/liblincs/io/model.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/io/model.hpp` & `lincs-0.6.0/lincs/liblincs/io/model.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/io/problem.cpp` & `lincs-0.6.0/lincs/liblincs/io/problem.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/io/problem.hpp` & `lincs-0.6.0/lincs/liblincs/io/problem.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/io/validation.cpp` & `lincs-0.6.0/lincs/liblincs/io/validation.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/io/validation.hpp` & `lincs-0.6.0/lincs/liblincs/io/validation.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/breed/reinitialize-least-accurate.hpp` & `lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/breed/reinitialize-least-accurate.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic/desirability.hpp` & `lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic/desirability.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-cpu.cpp` & `lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-cpu.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-cpu.hpp` & `lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-cpu.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-gpu.cu` & `lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-gpu.cu`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-gpu.hpp` & `lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-gpu.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp` & `lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp` & `lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/linear-program.cpp` & `lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/linear-program.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/linear-program.hpp` & `lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/linear-program.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-iterations.hpp` & `lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-iterations.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-seconds.hpp` & `lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-seconds.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/at-accuracy.hpp` & `lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/at-accuracy.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/composite.hpp` & `lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/composite.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed.cpp` & `lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed.hpp` & `lincs-0.6.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/learning/ucncs-by-sat-by-coalitions.cpp` & `lincs-0.6.0/lincs/liblincs/learning/ucncs-by-sat-by-coalitions.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -3,47 +3,24 @@
 #include "ucncs-by-sat-by-coalitions.hpp"
 
 #include <algorithm>
 #include <map>
 #include <type_traits>
 
 #include "exception.hpp"
-// @todo Let these two be included in alphabetical order
-// Currently, swapping them results in the following error:
-// could not convert ‘Glucose::lbool(2)’ from ‘Glucose::lbool’ to ‘Minisat::lbool’
 #include "../sat/minisat.hpp"
-#include "../sat/eval-max-sat.hpp"
 
 
 namespace lincs {
 
 template<typename SatProblem>
-std::enable_if_t<!std::is_same_v<typename SatProblem::weight_type, void>>
-add_possibly_weighted_clause(
-  SatProblem& sat,
-  const std::vector<typename SatProblem::variable_type>& clause,
-  const typename SatProblem::weight_type weight
-) {
-  sat.add_weighted_clause(clause, weight);
-}
-
-template<typename SatProblem>
-std::enable_if_t<std::is_same_v<typename SatProblem::weight_type, void>>
-add_possibly_weighted_clause(
-  SatProblem& sat,
-  const std::vector<typename SatProblem::variable_type>& clause,
-  const int
-) {
-  sat.add_clause(clause);
-}
-
-template<typename SatProblem>
-Model SatCoalitionUcncsLearning<SatProblem>::perform() {
+Model SatCoalitionsUcncsLearning<SatProblem>::perform() {
   const unsigned criteria_count = problem.criteria.size();
   const unsigned categories_count = problem.categories.size();
+  const unsigned boundaries_count = categories_count - 1;
 
   std::vector<std::vector<float>> unique_values(criteria_count);
   for (auto alternative : learning_set.alternatives) {
     for (unsigned i = 0; i != criteria_count; ++i) {
       unique_values[i].push_back(alternative.profile[i]);
     }
   }
@@ -54,18 +31,18 @@
 
   SatProblem sat;
 
   // x[i][h][k]: value k is above profile h on criterion i
   std::vector<std::vector<std::vector<typename SatProblem::variable_type>>> x(criteria_count);
   for (unsigned criterion_index = 0; criterion_index != criteria_count; ++criterion_index) {
     x[criterion_index].resize(categories_count);
-    for (unsigned category_index = 0; category_index != categories_count - 1; ++category_index) {
-      x[criterion_index][category_index].resize(unique_values[criterion_index].size());
+    for (unsigned boundary_index = 0; boundary_index != boundaries_count; ++boundary_index) {
+      x[criterion_index][boundary_index].resize(unique_values[criterion_index].size());
       for (unsigned value_index = 0; value_index != unique_values[criterion_index].size(); ++value_index) {
-        x[criterion_index][category_index][value_index] = sat.create_variable();
+        x[criterion_index][boundary_index][value_index] = sat.create_variable();
       }
     }
   }
 
   // A subsets b of criteria (i.e. a coalition) is represented
   // as a bitset where bit i is set if and only if criteria i is in b.
   // y[b]: coalition b is sufficient
@@ -79,30 +56,28 @@
 
   // Note: "A => B" <=> "-A or B"
 
   // Ascending scales: values are ordered according to index k
   // so if a value is above profile h, then values above it are above profile h too
   // so x[i][h][k] => x[i][h][k + 1]
   for (unsigned criterion_index = 0; criterion_index != criteria_count; ++criterion_index) {
-    for (unsigned category_index = 0; category_index != categories_count - 1; ++category_index) {
+    for (unsigned boundary_index = 0; boundary_index != boundaries_count; ++boundary_index) {
       for (unsigned value_index = 0; value_index != unique_values[criterion_index].size() - 1; ++value_index) {
-        sat.add_clause({-x[criterion_index][category_index][value_index], x[criterion_index][category_index][value_index + 1]});
+        sat.add_clause({-x[criterion_index][boundary_index][value_index], x[criterion_index][boundary_index][value_index + 1]});
       }
     }
   }
 
   // Hierarchy of profiles: profiles are ordered according to index h
   // so if a value is above a profile h, then it is above lower profiles too
-  // so x[i][h][k] => x[i][hp][k] for hp < h
+  // so x[i][h][k] => x[i][h - 1][k]
   for (unsigned criterion_index = 0; criterion_index != criteria_count; ++criterion_index) {
     for (unsigned value_index = 0; value_index != unique_values[criterion_index].size(); ++value_index) {
-      for (unsigned category_index_a = 0; category_index_a != categories_count - 1; ++category_index_a) {
-        for (unsigned category_index_b = 0; category_index_b != category_index_a; ++category_index_b) {
-          sat.add_clause({-x[criterion_index][category_index_a][value_index], x[criterion_index][category_index_b][value_index]});
-        }
+      for (unsigned boundary_index_a = 1; boundary_index_a != boundaries_count; ++boundary_index_a) {
+        sat.add_clause({-x[criterion_index][boundary_index_a][value_index], x[criterion_index][boundary_index_a - 1][value_index]});
       }
     }
   }
 
   // Coalitions strength: coalitions are an upset
   // so if coalition b is sufficient and b is included in bp, then bp is sufficient too
   // so y[b] => y[bp] for b included in bp
@@ -133,15 +108,15 @@
           assert(criterion_index < x.size());
           assert(category_index < x[criterion_index].size());
           assert(value_index < x[criterion_index][category_index].size());
           clause.push_back(-x[criterion_index][category_index][value_index]);
         }
       }
       clause.push_back(-y[subset]);
-      add_possibly_weighted_clause(sat, clause, 1);
+      sat.add_clause(clause);
     }
   }
 
   // Alternatives outrank the boundary below them
   for (auto alternative : learning_set.alternatives) {
     const unsigned category_index = *alternative.category_index;
     if (category_index == 0) {
@@ -159,73 +134,73 @@
           assert(category_index - 1 < x[criterion_index].size());
           assert(value_index < x[criterion_index][category_index - 1].size());
           clause.push_back(x[criterion_index][category_index - 1][value_index]);
         }
       }
       unsigned subset_complement = ~subset & (subsets_count - 1);
       clause.push_back(y[subset_complement]);
-      add_possibly_weighted_clause(sat, clause, 1);
+      sat.add_clause(clause);
     }
   }
 
   std::optional<std::vector<bool>> solution = sat.solve();
 
   if (!solution) {
     throw LearningFailureException();
   }
 
+  std::vector<std::vector<unsigned>> roots;
+  for (unsigned subset_a = 0; subset_a != subsets_count; ++subset_a) {
+    if ((*solution)[y[subset_a]]) {
+      bool is_root = true;
+      // @todo Optimize this search for actual roots; it may be something like a transitive reduction
+      for (unsigned subset_b = 0; subset_b != subsets_count; ++subset_b) {
+        if ((*solution)[y[subset_b]]) {
+          if ((subset_a & subset_b) == subset_b && subset_a != subset_b) {
+            is_root = false;
+            break;
+          }
+        }
+      }
+      if (is_root) {
+        roots.emplace_back();
+        for (unsigned criterion_index = 0; criterion_index != criteria_count; ++criterion_index) {
+          if (subset_a & (1 << criterion_index)) {
+            roots.back().push_back(criterion_index);
+          }
+        }
+      }
+    }
+  }
+
   std::vector<Model::Boundary> boundaries;
-  for (unsigned category_index = 0; category_index != categories_count - 1; ++category_index) {
+  boundaries.reserve(boundaries_count);
+  for (unsigned boundary_index = 0; boundary_index != boundaries_count; ++boundary_index) {
     std::vector<float> profile(criteria_count);
     for (unsigned criterion_index = 0; criterion_index != criteria_count; ++criterion_index) {
       bool found = false;
       // @todo Replace next loop with a binary search
       for (unsigned value_index = 0; value_index != unique_values[criterion_index].size(); ++value_index) {
-        if ((*solution)[x[criterion_index][category_index][value_index]]) {
+        if ((*solution)[x[criterion_index][boundary_index][value_index]]) {
           if (value_index == 0) {
             profile[criterion_index] = unique_values[criterion_index][value_index];
           } else {
             profile[criterion_index] = (unique_values[criterion_index][value_index - 1] + unique_values[criterion_index][value_index]) / 2;
           }
           found = true;
           break;
         }
       }
       if (!found) {
         profile[criterion_index] = 1;  // @todo Use the max value for the criterion
       }
     }
 
-    std::vector<std::vector<unsigned>> roots;
-    for (unsigned subset_a = 0; subset_a != subsets_count; ++subset_a) {
-      if ((*solution)[y[subset_a]]) {
-        bool is_root = true;
-        // @todo Optimize this search for actual roots; it may be something like a transitive reduction
-        for (unsigned subset_b = 0; subset_b != subsets_count; ++subset_b) {
-          if ((*solution)[y[subset_b]]) {
-            if ((subset_a & subset_b) == subset_b && subset_a != subset_b) {
-              is_root = false;
-              break;
-            }
-          }
-        }
-        if (is_root) {
-          roots.emplace_back();
-          for (unsigned criterion_index = 0; criterion_index != criteria_count; ++criterion_index) {
-            if (subset_a & (1 << criterion_index)) {
-              roots.back().push_back(criterion_index);
-            }
-          }
-        }
-      }
-    }
-
     boundaries.emplace_back(profile, SufficientCoalitions{SufficientCoalitions::roots, criteria_count, roots});
   }
 
   return Model{problem, boundaries};
 }
 
-template class SatCoalitionUcncsLearning<EvalmaxsatSatProblem>;
-template class SatCoalitionUcncsLearning<MinisatSatProblem>;
+template class SatCoalitionsUcncsLearning<MinisatSatProblem>;
 
 }  // namespace lincs
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `lincs-0.5.1/lincs/liblincs/learning/ucncs-by-sat-by-coalitions.hpp` & `lincs-0.6.0/lincs/liblincs/learning/ucncs-by-sat-by-separation.hpp`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 // Copyright 2023 Vincent Jacques
 
-#ifndef LINCS__LEARNING__UCNCS_BY_SAT_BY_COALITIONS_HPP
-#define LINCS__LEARNING__UCNCS_BY_SAT_BY_COALITIONS_HPP
+#ifndef LINCS__LEARNING__UCNCS_BY_SAT_BY_SEPARATION_HPP
+#define LINCS__LEARNING__UCNCS_BY_SAT_BY_SEPARATION_HPP
 
 #include "../io.hpp"
 
 
 namespace lincs {
 
 template<typename SatProblem>
-class SatCoalitionUcncsLearning {
+class SatSeparationUcncsLearning {
  public:
-  SatCoalitionUcncsLearning(const Problem& problem_, const Alternatives& learning_set_) : problem(problem_), learning_set(learning_set_) {}
+  SatSeparationUcncsLearning(const Problem& problem_, const Alternatives& learning_set_) : problem(problem_), learning_set(learning_set_) {}
 
  public:
   Model perform();
 
  private:
   const Problem& problem;
   const Alternatives& learning_set;
 };
 
 }  // namespace lincs
 
-#endif  // LINCS__LEARNING__UCNCS_BY_SAT_BY_COALITIONS_HPP
+#endif  // LINCS__LEARNING__UCNCS_BY_SAT_BY_SEPARATION_HPP
```

### Comparing `lincs-0.5.1/lincs/liblincs/learning.cpp` & `lincs-0.6.0/lincs/liblincs/learning.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -14,54 +14,85 @@
 bool env_is_true(const char* name) {
   const char* value = std::getenv(name);
   return value && std::string(value) == "true";
 }
 
 const bool forbid_gpu = env_is_true("LINCS_DEV_FORBID_GPU");
 const bool skip_long = env_is_true("LINCS_DEV_SKIP_LONG");
+const bool coverage = env_is_true("LINCS_DEV_COVERAGE");
+const unsigned default_seeds_count = coverage ? 1 : (skip_long ? 10 : 100);
 
 template<typename T>
 void check_exact_learning(const lincs::Problem& problem, unsigned seed) {
+  CAPTURE(problem.criteria.size());
+  CAPTURE(problem.categories.size());
   CAPTURE(seed);
 
   lincs::Model model = lincs::generate_mrsort_classification_model(problem, seed);
   lincs::Alternatives learning_set = lincs::generate_classified_alternatives(problem, model, 200, seed);
 
   T learning(problem, learning_set);
 
   lincs::Model learned_model = learning.perform();
 
   CHECK(lincs::classify_alternatives(problem, learned_model, &learning_set).changed == 0);
 }
 
 template<typename T>
-void check_exact_learning(const unsigned criteria_count, const unsigned categories_count, bool is_wpb) {
-  CAPTURE(criteria_count);
-  CAPTURE(categories_count);
-
+void check_exact_learning(
+  const unsigned criteria_count,
+  const unsigned categories_count,
+  std::set<unsigned> bad_seeds = {},
+  const unsigned seeds_count = default_seeds_count
+) {
   lincs::Problem problem = lincs::generate_classification_problem(criteria_count, categories_count, 41);
 
-  const unsigned max_seed = skip_long ? 10 : 100;
-
-  for (unsigned seed = 0; seed != max_seed; ++seed) {
-    // This set of parameters can't reach 100% accuracy with WPB approach
-    if (is_wpb && criteria_count == 4 && categories_count == 3 && seed == 59) {
+  for (unsigned seed = 0; seed != seeds_count; ++seed) {
+    if (bad_seeds.find(seed) != bad_seeds.end()) {
       CHECK_THROWS_AS(check_exact_learning<T>(problem, seed), lincs::LearningFailureException);
     } else {
       check_exact_learning<T>(problem, seed);
     }
   }
 }
 
 template<typename T>
-void check_exact_learning(bool is_wpb = false) {
-  check_exact_learning<T>(1, 2, is_wpb);
-  check_exact_learning<T>(3, 2, is_wpb);
-  check_exact_learning<T>(1, 3, is_wpb);
-  check_exact_learning<T>(4, 3, is_wpb);
+void check_non_exact_learning(const lincs::Problem& problem, unsigned seed) {
+  CAPTURE(problem.criteria.size());
+  CAPTURE(problem.categories.size());
+  CAPTURE(seed);
+
+  lincs::Model model = lincs::generate_mrsort_classification_model(problem, seed);
+  lincs::Alternatives learning_set = lincs::generate_classified_alternatives(problem, model, 200, seed);
+  lincs::misclassify_alternatives(problem, &learning_set, 10, seed);
+
+  T learning(problem, learning_set);
+
+  lincs::Model learned_model = learning.perform();
+
+  // The original model would classify with .changed == 10, so the best model must have .changed <= 10
+  CHECK(lincs::classify_alternatives(problem, learned_model, &learning_set).changed <= 10);
+}
+
+template<typename T>
+void check_non_exact_learning(
+  const unsigned criteria_count,
+  const unsigned categories_count,
+  std::set<unsigned> bad_seeds = {},
+  const unsigned seeds_count = default_seeds_count
+) {
+  lincs::Problem problem = lincs::generate_classification_problem(criteria_count, categories_count, 41);
+
+  for (unsigned seed = 0; seed != seeds_count; ++seed) {
+    if (bad_seeds.find(seed) != bad_seeds.end()) {
+      CHECK_THROWS_AS(check_non_exact_learning<T>(problem, seed), lincs::LearningFailureException);
+    } else {
+      check_non_exact_learning<T>(problem, seed);
+    }
+  }
 }
 
 }  // namespace
 
 namespace lincs {
 
 TEST_CASE("Basic MR-Sort learning") {
@@ -95,15 +126,19 @@
     OptimizeWeightsUsingGlop weights_optimization_strategy;
     ImproveProfilesWithAccuracyHeuristicOnCpu profiles_improvement_strategy;
     ReinitializeLeastAccurate breeding_strategy;
     TerminateAtAccuracy termination_strategy;
     LearnMrsortByWeightsProfilesBreed learning;
   };
 
-  check_exact_learning<Wrapper>(true);
+  check_exact_learning<Wrapper>(1, 2);
+  check_exact_learning<Wrapper>(3, 2);
+  check_exact_learning<Wrapper>(7, 2, {78});
+  check_exact_learning<Wrapper>(1, 3);
+  check_exact_learning<Wrapper>(4, 3, {59});
 }
 
 TEST_CASE("No termination strategy MR-Sort learning") {
   struct NeverTerminate : LearnMrsortByWeightsProfilesBreed::TerminationStrategy {
     bool terminate() override { return false; }
   };
 
@@ -137,15 +172,19 @@
     OptimizeWeightsUsingGlop weights_optimization_strategy;
     ImproveProfilesWithAccuracyHeuristicOnCpu profiles_improvement_strategy;
     ReinitializeLeastAccurate breeding_strategy;
     NeverTerminate termination_strategy;
     LearnMrsortByWeightsProfilesBreed learning;
   };
 
-  check_exact_learning<Wrapper>(true);
+  check_exact_learning<Wrapper>(1, 2);
+  check_exact_learning<Wrapper>(3, 2);
+  check_exact_learning<Wrapper>(7, 2, {78});
+  check_exact_learning<Wrapper>(1, 3);
+  check_exact_learning<Wrapper>(4, 3, {59});
 }
 
 TEST_CASE("Alglib MR-Sort learning") {
   class Wrapper {
    public:
     Wrapper(const Problem& problem, const Alternatives& learning_set) :
       learning_data(LearnMrsortByWeightsProfilesBreed::LearningData::make(
@@ -175,15 +214,19 @@
     OptimizeWeightsUsingAlglib weights_optimization_strategy;
     ImproveProfilesWithAccuracyHeuristicOnCpu profiles_improvement_strategy;
     ReinitializeLeastAccurate breeding_strategy;
     TerminateAtAccuracy termination_strategy;
     LearnMrsortByWeightsProfilesBreed learning;
   };
 
-  check_exact_learning<Wrapper>(true);
+  check_exact_learning<Wrapper>(1, 2);
+  check_exact_learning<Wrapper>(3, 2);
+  check_exact_learning<Wrapper>(7, 2);  // @todo Investigate why seed 78 succeeds with Alglib but not with Glop
+  check_exact_learning<Wrapper>(1, 3);
+  check_exact_learning<Wrapper>(4, 3, {59});
 }
 
 #ifdef LINCS_HAS_NVCC
 
 TEST_CASE("GPU MR-Sort learning" * doctest::skip(forbid_gpu)) {
   class Wrapper {
    public:
@@ -215,56 +258,53 @@
     OptimizeWeightsUsingGlop weights_optimization_strategy;
     ImproveProfilesWithAccuracyHeuristicOnGpu profiles_improvement_strategy;
     ReinitializeLeastAccurate breeding_strategy;
     TerminateAtAccuracy termination_strategy;
     LearnMrsortByWeightsProfilesBreed learning;
   };
 
-  check_exact_learning<Wrapper>(true);
+  check_exact_learning<Wrapper>(1, 2);
+  check_exact_learning<Wrapper>(3, 2);
+  check_exact_learning<Wrapper>(7, 2, {78});
+  check_exact_learning<Wrapper>(1, 3);
+  check_exact_learning<Wrapper>(4, 3, {59});
 }
 
 #endif  // LINCS_HAS_NVCC
 
 TEST_CASE("SAT by coalitions using Minisat learning") {
-  check_exact_learning<LearnUcncsBySatByCoalitionsUsingMinisat>();
+  check_exact_learning<LearnUcncsBySatByCoalitionsUsingMinisat>(1, 2);
+  check_exact_learning<LearnUcncsBySatByCoalitionsUsingMinisat>(3, 2);
+  check_exact_learning<LearnUcncsBySatByCoalitionsUsingMinisat>(7, 2);
+  check_exact_learning<LearnUcncsBySatByCoalitionsUsingMinisat>(1, 3);
+  check_exact_learning<LearnUcncsBySatByCoalitionsUsingMinisat>(4, 3);
+  check_exact_learning<LearnUcncsBySatByCoalitionsUsingMinisat>(3, 5);
 }
 
-TEST_CASE("SAT by coalitions using EvalMaxSAT learning") {
-  check_exact_learning<LearnUcncsBySatByCoalitionsUsingEvalmaxsat>();
-}
-
-TEST_CASE("Non-exact learning - SAT by coalitions") {
-  const Problem problem = generate_classification_problem(3, 2, 41);
-  const Model model = generate_mrsort_classification_model(problem, 44);
-  Alternatives learning_set = generate_classified_alternatives(problem, model, 100, 44);
-  misclassify_alternatives(problem, &learning_set, 10, 44);
-
-  CHECK_THROWS_AS(
-    LearnUcncsBySatByCoalitionsUsingMinisat(problem, learning_set).perform(),
-    LearningFailureException
-  );
-
-  LearnUcncsBySatByCoalitionsUsingEvalmaxsat learning(problem, learning_set);
-  Model learned_model = learning.perform();
-
-  CHECK(classify_alternatives(problem, learned_model, &learning_set).changed == 10);
+TEST_CASE("SAT by separation using Minisat learning") {
+  check_exact_learning<LearnUcncsBySatBySeparationUsingMinisat>(1, 2);
+  check_exact_learning<LearnUcncsBySatBySeparationUsingMinisat>(3, 2);
+  check_exact_learning<LearnUcncsBySatBySeparationUsingMinisat>(7, 2);
+  check_exact_learning<LearnUcncsBySatBySeparationUsingMinisat>(1, 3);
+  check_exact_learning<LearnUcncsBySatBySeparationUsingMinisat>(4, 3);
+  check_exact_learning<LearnUcncsBySatBySeparationUsingMinisat>(3, 5);
 }
 
 TEST_CASE("Non-exact learning - MR-Sort") {
   class Wrapper {
    public:
-    Wrapper(const Problem& problem, const Alternatives& learning_set, const unsigned target_accuracy) :
+    Wrapper(const Problem& problem, const Alternatives& learning_set) :
       learning_data(LearnMrsortByWeightsProfilesBreed::LearningData::make(
         problem, learning_set, LearnMrsortByWeightsProfilesBreed::default_models_count, 44
       )),
       profiles_initialization_strategy(learning_data),
       weights_optimization_strategy(learning_data),
       profiles_improvement_strategy(learning_data),
       breeding_strategy(learning_data, profiles_initialization_strategy, LearnMrsortByWeightsProfilesBreed::default_models_count / 2),
-      termination_strategy(learning_data, target_accuracy),
+      termination_strategy(learning_data, 190),
       learning(
         learning_data,
         profiles_initialization_strategy,
         weights_optimization_strategy,
         profiles_improvement_strategy,
         breeding_strategy,
         termination_strategy
@@ -280,24 +320,14 @@
     OptimizeWeightsUsingGlop weights_optimization_strategy;
     ImproveProfilesWithAccuracyHeuristicOnCpu profiles_improvement_strategy;
     ReinitializeLeastAccurate breeding_strategy;
     TerminateAtAccuracy termination_strategy;
     LearnMrsortByWeightsProfilesBreed learning;
   };
 
-  const Problem problem = generate_classification_problem(3, 2, 41);
-  const Model model = generate_mrsort_classification_model(problem, 44);
-  Alternatives learning_set = generate_classified_alternatives(problem, model, 100, 44);
-  misclassify_alternatives(problem, &learning_set, 10, 44);
-
-  CHECK_THROWS_AS(
-    Wrapper(problem, learning_set, 100).perform(),
-    LearningFailureException
-  );
-
-  Wrapper learning(problem, learning_set, 90);
-  Model learned_model = learning.perform();
-
-  CHECK(classify_alternatives(problem, learned_model, &learning_set).changed == 10);
+  check_non_exact_learning<Wrapper>(1, 2);
+  check_non_exact_learning<Wrapper>(3, 2, {21});
+  check_non_exact_learning<Wrapper>(1, 3);
+  check_non_exact_learning<Wrapper>(4, 3, {86, 97});
 }
 
 }  // namespace lincs
```

### Comparing `lincs-0.5.1/lincs/liblincs/learning.hpp` & `lincs-0.6.0/lincs/liblincs/learning.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 // Copyright 2023 Vincent Jacques
 
 #ifndef LINCS__LEARNING_HPP
 #define LINCS__LEARNING_HPP
 
-#include "learning/ucncs-by-sat-by-coalitions.hpp"
 #include "learning/mrsort-by-weights-profiles-breed.hpp"
+#include "learning/mrsort-by-weights-profiles-breed/breed/reinitialize-least-accurate.hpp"
 #include "learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-cpu.hpp"
 #include "learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-gpu.hpp"
 #include "learning/mrsort-by-weights-profiles-breed/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp"
 #include "learning/mrsort-by-weights-profiles-breed/optimize-weights/linear-program.hpp"
-#include "learning/mrsort-by-weights-profiles-breed/breed/reinitialize-least-accurate.hpp"
-#include "learning/mrsort-by-weights-profiles-breed/terminate/at-accuracy.hpp"
-#include "learning/mrsort-by-weights-profiles-breed/terminate/composite.hpp"
 #include "learning/mrsort-by-weights-profiles-breed/terminate/after-iterations.hpp"
 #include "learning/mrsort-by-weights-profiles-breed/terminate/after-seconds.hpp"
+#include "learning/mrsort-by-weights-profiles-breed/terminate/at-accuracy.hpp"
+#include "learning/mrsort-by-weights-profiles-breed/terminate/composite.hpp"
+#include "learning/ucncs-by-sat-by-coalitions.hpp"
+#include "learning/ucncs-by-sat-by-separation.hpp"
 #include "linear-programming/alglib.hpp"
 #include "linear-programming/glop.hpp"
 #include "sat/minisat.hpp"
-#include "sat/eval-max-sat.hpp"
 
 namespace lincs {
   typedef OptimizeWeightsUsingLinearProgram<AlglibLinearProgram> OptimizeWeightsUsingAlglib;
   typedef OptimizeWeightsUsingLinearProgram<GlopLinearProgram> OptimizeWeightsUsingGlop;
-  typedef SatCoalitionUcncsLearning<EvalmaxsatSatProblem> LearnUcncsBySatByCoalitionsUsingEvalmaxsat;
-  typedef SatCoalitionUcncsLearning<MinisatSatProblem> LearnUcncsBySatByCoalitionsUsingMinisat;
+  typedef SatCoalitionsUcncsLearning<MinisatSatProblem> LearnUcncsBySatByCoalitionsUsingMinisat;
+  typedef SatSeparationUcncsLearning<MinisatSatProblem> LearnUcncsBySatBySeparationUsingMinisat;
 }  // namespace lincs
 
 #endif  // LINCS__LEARNING_HPP
```

### Comparing `lincs-0.5.1/lincs/liblincs/liblincs_module.cpp` & `lincs-0.6.0/lincs/liblincs/liblincs_module.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -530,11 +530,11 @@
   ;
 
 
   bp::class_<lincs::LearnUcncsBySatByCoalitionsUsingMinisat>("LearnUcncsBySatByCoalitionsUsingMinisat", bp::init<const lincs::Problem&, const lincs::Alternatives&>())
     .def("perform", &lincs::LearnUcncsBySatByCoalitionsUsingMinisat::perform)
   ;
 
-  bp::class_<lincs::LearnUcncsBySatByCoalitionsUsingEvalmaxsat>("LearnUcncsBySatByCoalitionsUsingEvalmaxsat", bp::init<const lincs::Problem&, const lincs::Alternatives&>())
-    .def("perform", &lincs::LearnUcncsBySatByCoalitionsUsingEvalmaxsat::perform)
+  bp::class_<lincs::LearnUcncsBySatBySeparationUsingMinisat>("LearnUcncsBySatBySeparationUsingMinisat", bp::init<const lincs::Problem&, const lincs::Alternatives&>())
+    .def("perform", &lincs::LearnUcncsBySatBySeparationUsingMinisat::perform)
   ;
 }
```

### Comparing `lincs-0.5.1/lincs/liblincs/linear-programming/alglib.hpp` & `lincs-0.6.0/lincs/liblincs/linear-programming/alglib.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/linear-programming/glop.hpp` & `lincs-0.6.0/lincs/liblincs/linear-programming/glop.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/linear-programming/test.cpp` & `lincs-0.6.0/lincs/liblincs/linear-programming/test.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/randomness-utils.cpp` & `lincs-0.6.0/lincs/liblincs/randomness-utils.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/randomness-utils.hpp` & `lincs-0.6.0/lincs/liblincs/randomness-utils.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/sat/eval-max-sat.hpp` & `lincs-0.6.0/lincs/liblincs/sat/eval-max-sat.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
   void mark_all_variables_created() {}
 
  public:
   void add_clause(std::vector<variable_type> clause) {
     solver.addClause(clause);
   }
 
-  typedef int weight_type;
+  typedef unsigned weight_type;
   void add_weighted_clause(std::vector<variable_type> clause, weight_type weight) {
     solver.addWeightedClause(clause, weight);
   }
 
   std::optional<std::vector<bool>> solve() {
     if (solver.solve()) {
       std::vector<bool> solution(variables.back() + 1);
```

### Comparing `lincs-0.5.1/lincs/liblincs/sat/minisat.hpp` & `lincs-0.6.0/lincs/liblincs/sat/minisat.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/sat/test.cpp` & `lincs-0.6.0/lincs/liblincs/sat/test.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -77,14 +77,33 @@
   if ((*solution)[x1] || (*solution)[x2]) ++score;
   if ((*solution)[x3]) ++score;
   if ((*solution)[x1] || !(*solution)[x3]) ++score;
   if ((*solution)[x2] || !(*solution)[x3]) ++score;
   CHECK(score == 3);
 }
 
+// Some SAT solvers:
+// - minisat
+// - glucose
+// - cadical
+// - lingeling
+// - cryptominisat
+// - picosat
+// - riss
+// - kissat
+// - minisatp
+
+// Some max-SAT solvers:
+// - EvalMaxSAT
+// - open-wbo
+// - maxhs
+// - cryptominisat
+// - maxwalksat
+// - maxsatz
+
 TEST_CASE("Minisat SAT problem") {
   test_sat_problem<lincs::MinisatSatProblem>();
 }
 
 TEST_CASE("EvalMaxSAT SAT problem") {
   test_sat_problem<lincs::EvalmaxsatSatProblem>();
 }
```

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/alglibinternal.cpp` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/alglibinternal.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/alglibinternal.h` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/alglibinternal.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/alglibmisc.cpp` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/alglibmisc.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/alglibmisc.h` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/alglibmisc.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/ap.cpp` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/ap.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/ap.h` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/ap.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/dataanalysis.cpp` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/dataanalysis.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/dataanalysis.h` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/dataanalysis.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/diffequations.cpp` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/diffequations.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/diffequations.h` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/diffequations.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/fasttransforms.cpp` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/fasttransforms.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/fasttransforms.h` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/fasttransforms.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/integration.cpp` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/integration.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/integration.h` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/integration.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/interpolation.cpp` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/interpolation.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/interpolation.h` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/interpolation.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/kernels_avx2.cpp` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/kernels_avx2.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/kernels_avx2.h` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/kernels_avx2.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/kernels_fma.cpp` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/kernels_fma.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/kernels_fma.h` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/kernels_fma.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/kernels_sse2.cpp` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/kernels_sse2.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/kernels_sse2.h` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/kernels_sse2.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/linalg.cpp` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/linalg.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/linalg.h` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/linalg.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/optimization.cpp` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/optimization.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/optimization.h` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/optimization.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/solvers.cpp` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/solvers.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/solvers.h` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/solvers.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/specialfunctions.cpp` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/specialfunctions.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/specialfunctions.h` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/specialfunctions.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/statistics.cpp` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/statistics.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/alglib/statistics.h` & `lincs-0.6.0/lincs/liblincs/vendored/alglib/statistics.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/doctest.h` & `lincs-0.6.0/lincs/liblincs/vendored/doctest.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/MaLib/Chrono.h` & `lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/MaLib/Chrono.h`

 * *Files 9% similar despite different names*

```diff
@@ -111,24 +111,30 @@
                 {
                     return _dureeSec;
                 }
             }
 
             void print()
             {
+                #if false
                 double val = tac();
-
                 if(_name.size())
                     std::cout << _name << ": ";
                 if(val < 1000.0)
                     std::cout << val << " µs" << std::endl;
                 else if(val < 1000000.0)
                     std::cout << val/1000.0 << " ms" << std::endl;
                 else
                     std::cout << val/1000000.0 << " sec" << std::endl;
+                #endif
+                //static double total; total+=val/1000000.0; std::cout<<"Total : "<<total<<" s"<<std::endl; // TODO: Remove this line
+            }
+
+            void afficherQuandDetruit(bool val) {
+                _afficherQuandDetruit = val;
             }
 
         private :
 
 
         std::string _name;
         struct timeval depart, fin;
```

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/MaLib/View.h` & `lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/MaLib/View.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/MaLib/communicationlist.h` & `lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/MaLib/communicationlist.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,88 +1,113 @@
 #ifndef COMMUNICATIONLIST_LQSF093AEJL__H
-#define COMMUNICATIONLIST_LQSF093AEJL___H
+#define COMMUNICATIONLIST_LQSF093AEJL__H
 
 #include <list>
 #include <vector>
 #include <thread>
 #include <mutex>
 #include <condition_variable>
 #include <optional>
 #include <cassert>
 #include <iostream>
 
 
 namespace MaLib {
 
+
+
 template <class T>
 class CommunicationList {
     std::mutex _mutex;
-
-    std::condition_variable _cv_pop;
+    std::condition_variable _cv_push;
     std::condition_variable _cv_wait;
-    bool newWaintingProcess = false;
-    bool _closed = false;
-    unsigned int numberWaiting=0;
 
     std::list<T> data;
+    unsigned int numberWaiting=0;
 
+    bool _closed = false;
 public:
 
     CommunicationList() {
 
     }
 
-    unsigned int getNumberWaiting() {
-        std::lock_guard<std::mutex> lock(_mutex);
-        return numberWaiting;
+    unsigned int size() {
+        std::scoped_lock<std::mutex> lock(_mutex);
+        return data.size();
     }
 
     void clear() {
-        std::lock_guard<std::mutex> lock(_mutex);
+        std::scoped_lock<std::mutex> lock(_mutex);
         assert(numberWaiting == 0);
         _closed = false;
-        newWaintingProcess = false;
+        //newWaintingProcess = false;
         numberWaiting=0;
         data.clear();
     }
 
+    /*
+     * No more elements will be added.
+     * Processes waiting in pop() will be unlocked.
+     */
+    void close() {
+        {
+            std::scoped_lock<std::mutex> lock(_mutex);
+            _closed = true;
+        }
+        _cv_push.notify_all();
+    }
+
     void push(const T& element) {
         {
-            std::lock_guard<std::mutex> lock(_mutex);
+            std::scoped_lock<std::mutex> lock(_mutex);
             assert(!_closed);
             data.push_back(element);
         }
-        _cv_pop.notify_one();
+        _cv_push.notify_one();
     }
 
     template <class T2>
     void pushAll(const T2 &elements) {
         {
-            std::lock_guard<std::mutex> lock(_mutex);
+            std::scoped_lock<std::mutex> lock(_mutex);
             assert(!_closed);
             data.insert(data.end(), elements.begin(), elements.end());
         }
-        _cv_pop.notify_all();
+        _cv_push.notify_all();
+    }
+
+    const std::list<T> & getWithoutRemove_unsafe() {
+        return data;
+    }
+
+
+    unsigned int getNumberWaiting() {
+        std::lock_guard<std::mutex> lock(_mutex);
+        return numberWaiting;
     }
 
+
     /*
      * Blocks until a new element is added or the method close() is called.
      * return nothing if the CommunicationList is empty and closed.
      */
     std::optional<T> pop() {
         std::unique_lock<std::mutex> lock(_mutex);
+
         if((data.size() == 0) && (_closed == false)) {
             ++numberWaiting;
-            newWaintingProcess = true;
+            //newWaintingProcess = true;
             _cv_wait.notify_all();
 
-            _cv_pop.wait(lock, [&]{
+            _cv_push.wait(lock, [&]{
                 return (data.size() || _closed);
             });
 
+            assert(data.size() || _closed);
             assert(numberWaiting > 0);
             --numberWaiting;
         }
 
         if(data.size()) {
             auto result = data.front();
             data.pop_front();
@@ -90,55 +115,32 @@
         }
         assert(_closed);
 
         return {};
     }
 
     /*
-     * No more elements will be added.
-     * Processes waiting in pop() will be unlocked.
-     */
-    void close() {
-        {
-            std::lock_guard<std::mutex> lock(_mutex);
-            _closed = true;
-        }
-        _cv_pop.notify_all();
-    }
-
-    unsigned int size() {
-        std::lock_guard<std::mutex> lock(_mutex);
-        return data.size();
-    }
-
-    /*
      * Wait until at least $n$ processes are wainting in pop().
-     * If aware = true, then the function return the new number of processes wainting each time that new process becomes waiting in pop().
      */
-    unsigned int wait(unsigned int n, bool aware = false) {
-
+    unsigned int areWaiting(unsigned int n) {
         std::unique_lock<std::mutex> lock(_mutex);
         assert(!_closed);
 
+
         if( std::max(0, static_cast<int>(numberWaiting) - static_cast<int>(data.size()) ) >= n ) {
-            return std::max(0, static_cast<int>(numberWaiting) - static_cast<int>(data.size()) );
+            return static_cast<int>(numberWaiting) - static_cast<int>(data.size());
         }
 
-        if(aware) {
-            _cv_wait.wait(lock, [&]{
-                return newWaintingProcess;
-            });
-        } else {
-            _cv_wait.wait(lock, [&]{
-                return std::max(0, static_cast<int>(numberWaiting) - static_cast<int>(data.size())) >= static_cast<int>(n);
-            });
-        }
-        newWaintingProcess = false;
-        return std::max(0, static_cast<int>(numberWaiting) - static_cast<int>(data.size()) );
+        _cv_wait.wait(lock, [&]{
+            return std::max(0, static_cast<int>(numberWaiting) - static_cast<int>(data.size())) >= n;
+        });
+
+        assert( std::max(0, static_cast<int>(numberWaiting) - static_cast<int>(data.size())) >= n );
+        return static_cast<int>(numberWaiting) - static_cast<int>(data.size());
     }
 
 };
 
 }
 
+#endif // COMMUNICATIONLIST_LQSF093AEJL__H
 
-#endif // COMMUNICATIONLIST_LQSF093AEJL___H
```

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/MaLib/coutUtil.h` & `lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/MaLib/coutUtil.h`

 * *Files 3% similar despite different names*

```diff
@@ -266,25 +266,33 @@
 template <typename...T>
 std::tuple<T...> operator + (std::tuple<T...> lhs, const std::tuple<T...>& rhs)
 {
    return lhs += rhs;
 }
 
 namespace {
-//MaLib::Chrono MonPrint_Chrono;
+#ifdef NDEBUG
+
+#else
+//    MaLib::Chrono MonPrint_Chrono;
+#endif
 }
 template<typename ...T>
 void MonPrint(const T&... args) {
+#ifdef NDEBUG
+
+#else
 /*
     static std::mutex forPrint;
     {
         std::lock_guard lock(forPrint);
-        std::cout << MonPrint_Chrono.tacSec() << ": " << toString(args...) << std::endl;
+        std::cout << "c " << MonPrint_Chrono.tacSec() << ": " << toString(args...) << std::endl;
     }
 */
+#endif
 }
 
 
 }
 
 
 #endif
```

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/card_oe.cpp` & `lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/card_oe.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
             }
         }
     }
 
     // y[i−2] & x[i+1] => x''[i]    <===>   -y[i−2]  V  -x[i+1]  V  x''[i]
     {
         // Cas particulier quand i={0,1}
-        //addClause(-x[1], X(0)); inutile car x[0] => X(0)
+        //addUnitClause(-x[1], X(0)); inutile car x[0] => X(0)
         if(x.size() > 2) {
             if(X(1)) {
                 //std::cout << "x[2] => X(1)" << std::endl;
                 X(1)->addImpliquant({x[2]});
             }
             int max = std::min(static_cast<int>(x.size()-1), static_cast<int>(y.size()+2));
             for(int i=2; i<max; i++) {
```

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/card_oe.h` & `lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/card_oe.h`

 * *Files 2% similar despite different names*

```diff
@@ -17,23 +17,23 @@
 class Card_Lazy_OE : public VirtualCard {
     std::vector< std::shared_ptr<LazyVariable> > coutingVar;
 
     std::vector<int> clause;
 
 public:
 
-    virtual int atMost(unsigned int k) {
+    virtual int atMost(unsigned int k) override {
         if(k >= coutingVar.size()) {
             return 0;
         }
 
         return -coutingVar[k]->get();
     }
 
-    virtual std::vector<int> getClause() {
+    virtual std::vector<int> getClause() override {
         return clause;
     }
 
     Card_Lazy_OE(VirtualSAT * solver, const std::vector< int >& clause, std::optional<unsigned int> k = {})
         : VirtualCard (solver, clause), clause(clause) {
 
         k = k.value_or(clause.size()) + 1;
```

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/core/Dimacs.h` & `lincs-0.6.0/lincs/liblincs/vendored/minisat/mtl/Alg.h`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/****************************************************************************************[Dimacs.h]
+/*******************************************************************************************[Alg.h]
 Copyright (c) 2003-2006, Niklas Een, Niklas Sorensson
 Copyright (c) 2007-2010, Niklas Sorensson
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software without restriction,
 including without limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is
@@ -14,76 +14,71 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT
 NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT
 OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 **************************************************************************************************/
 
-#ifndef Glucose_Dimacs_h
-#define Glucose_Dimacs_h
+#ifndef Minisat_Alg_h
+#define Minisat_Alg_h
 
-#include <stdio.h>
+#include "Vec.h"
 
-#include "../utils/ParseUtils.h"
-#include "SolverTypes.h"
+namespace Minisat {
 
-namespace Glucose {
+//=================================================================================================
+// Useful functions on vector-like types:
 
 //=================================================================================================
-// DIMACS Parser:
+// Removing and searching for elements:
+//
 
-template<class B, class Solver>
-static void readClause(B& in, Solver& S, vec<Lit>& lits) {
-    int     parsed_lit, var;
-    lits.clear();
-    for (;;){
-        parsed_lit = parseInt(in);
-        if (parsed_lit == 0) break;
-        var = abs(parsed_lit)-1;
-        while (var >= S.nVars()) S.newVar();
-        lits.push( (parsed_lit > 0) ? mkLit(var) : ~mkLit(var) );
-    }
+template<class V, class T>
+static inline void remove(V& ts, const T& t)
+{
+    int j = 0;
+    for (; j < (int)ts.size() && ts[j] != t; j++);
+    assert(j < (int)ts.size());
+    for (; j < (int)ts.size()-1; j++) ts[j] = ts[j+1];
+    ts.pop();
 }
 
-template<class B, class Solver>
-static void parse_DIMACS_main(B& in, Solver& S) {
-    vec<Lit> lits;
-    int vars    = 0;
-    int clauses = 0;
-    int cnt     = 0;
-    for (;;){
-        skipWhitespace(in);
-        if (*in == EOF) break;
-        else if (*in == 'p'){
-            if (eagerMatch(in, "p cnf")){
-                vars    = parseInt(in);
-                clauses = parseInt(in);
-                // SATRACE'06 hack
-                // if (clauses > 4000000)
-                //     S.eliminate(true);
-            }else{
-                printf("PARSE ERROR! Unexpected char: %c\n", *in), exit(3);
-            }
-        } else if (*in == 'c' || *in == 'p')
-            skipLine(in);
-        else{
-            cnt++;
-            readClause(in, S, lits);
-            S.addClause_(lits); }
-    }
-    if (vars != S.nVars())
-        fprintf(stderr, "WARNING! DIMACS header mismatch: wrong number of variables.\n");
-    if (cnt  != clauses)
-        fprintf(stderr, "WARNING! DIMACS header mismatch: wrong number of clauses.\n");
+
+template<class V, class T>
+static inline bool find(V& ts, const T& t)
+{
+    int j = 0;
+    for (; j < (int)ts.size() && ts[j] != t; j++);
+    return j < (int)ts.size();
 }
 
-// Inserts problem into solver.
+
+//=================================================================================================
+// Copying vectors with support for nested vector types:
 //
-template<class Solver>
-static void parse_DIMACS(gzFile input_stream, Solver& S) {
-    StreamBuffer in(input_stream);
-    parse_DIMACS_main(in, S); }
+
+// Base case:
+template<class T>
+static inline void copy(const T& from, T& to)
+{
+    to = from;
+}
+
+// Recursive case:
+template<class T>
+static inline void copy(const vec<T>& from, vec<T>& to, bool append = false)
+{
+    if (!append)
+        to.clear();
+    for (int i = 0; i < from.size(); i++){
+        to.push();
+        copy(from[i], to.last());
+    }
+}
+
+template<class T>
+static inline void append(const vec<T>& from, vec<T>& to){ copy(from, to, true); }
 
 //=================================================================================================
 }
 
 #endif
```

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/core/Solver.h` & `lincs-0.6.0/lincs/liblincs/vendored/minisat/core/Solver.h`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,8 @@
-/***************************************************************************************[Solver.h]
- Glucose -- Copyright (c) 2009-2014, Gilles Audemard, Laurent Simon
-                                CRIL - Univ. Artois, France
-                                LRI  - Univ. Paris Sud, France (2009-2013)
-                                Labri - Univ. Bordeaux, France
-
- Syrup (Glucose Parallel) -- Copyright (c) 2013-2014, Gilles Audemard, Laurent Simon
-                                CRIL - Univ. Artois, France
-                                Labri - Univ. Bordeaux, France
-
-Glucose sources are based on MiniSat (see below MiniSat copyrights). Permissions and copyrights of
-Glucose (sources until 2013, Glucose 3.0, single core) are exactly the same as Minisat on which it 
-is based on. (see below).
-
-Glucose-Syrup sources are based on another copyright. Permissions and copyrights for the parallel
-version of Glucose-Syrup (the "Software") are granted, free of charge, to deal with the Software
-without restriction, including the rights to use, copy, modify, merge, publish, distribute,
-sublicence, and/or sell copies of the Software, and to permit persons to whom the Software is 
-furnished to do so, subject to the following conditions:
-
-- The above and below copyrights notices and this permission notice shall be included in all
-copies or substantial portions of the Software;
-- The parallel version of Glucose (all files modified since Glucose 3.0 releases, 2013) cannot
-be used in any competitive event (sat competitions/evaluations) without the express permission of 
-the authors (Gilles Audemard / Laurent Simon). This is also the case for any competitive event
-using Glucose Parallel as an embedded SAT engine (single core or not).
-
-
---------------- Original Minisat Copyrights
-
+/****************************************************************************************[Solver.h]
 Copyright (c) 2003-2006, Niklas Een, Niklas Sorensson
 Copyright (c) 2007-2010, Niklas Sorensson
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software without restriction,
 including without limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is
@@ -41,225 +12,101 @@
 substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT
 NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT
 OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
- **************************************************************************************************/
+**************************************************************************************************/
 
-#ifndef Glucose_Solver_h
-#define Glucose_Solver_h
+#ifndef Minisat_Solver_h
+#define Minisat_Solver_h
 
+#include "../mtl/Vec.h"
 #include "../mtl/Heap.h"
 #include "../mtl/Alg.h"
+#include "../mtl/IntMap.h"
 #include "../utils/Options.h"
 #include "SolverTypes.h"
-#include "BoundedQueue.h"
-#include "Constants.h"
-#include "../mtl/Clone.h"
-#include "SolverStats.h"
-
-
-namespace Glucose {
-// Core stats 
-
-enum CoreStats {
-  sumResSeen,
-  sumRes,
-  sumTrail,
-  nbPromoted,
-  originalClausesSeen,
-  sumDecisionLevels,
-  nbPermanentLearnts,
-  nbRemovedClauses,
-  nbRemovedUnaryWatchedClauses,
-  nbReducedClauses,
-  nbDL2,
-  nbBin,
-  nbUn,
-  nbReduceDB,
-  rnd_decisions,
-  nbstopsrestarts,
-  nbstopsrestartssame,
-  lastblockatrestart,
-  dec_vars,
-  clauses_literals,
-  learnts_literals,
-  max_literals,
-  tot_literals,
-  noDecisionConflict,
-  lcmtested,
-    lcmreduced,
-    sumSizes
-} ;
 
-#define coreStatsSize 27
-//=================================================================================================
-// Solver -- the main class:
 
-class Solver : public Clone {
+namespace Minisat {
 
-    friend class SolverConfiguration;
+//=================================================================================================
+// Solver -- the main class:
 
+class Solver {
 public:
 
     // Constructor/Destructor:
     //
     Solver();
-    Solver(const  Solver &s);
-
     virtual ~Solver();
 
-    /**
-     * Clone function
-     */
-    virtual Clone* clone() const {
-        return  new Solver(*this);
-    }
-
     // Problem specification:
     //
-    virtual Var     newVar    (bool polarity = true, bool dvar = true); // Add a new variable with parameters specifying variable mode.
-
-
-
-    void resetActivity(Var var) {
-        activity[var] = std::numeric_limits<double>::lowest();
-	order_heap.update(var);
-    }
+    Var     newVar    (lbool upol = l_Undef, bool dvar = true); // Add a new variable with parameters specifying variable mode.
+    void    releaseVar(Lit l);                                  // Make literal true and promise to never refer to variable again.
 
-    bool START_LOG = false;
-    void placeInTop(Var var) {
-        if(!order_heap.inHeap(var)) {
-            order_heap.insert(var);
-        }
-
-        activity[var] = activity[order_heap[0]]+1;
-        order_heap.update(var);
-        START_LOG=true;
-    }
-
-    double getActivity(Var var) {
-        return activity[var]/var_inc;
-    }
-
-    void addActivity(Var var, double nbInc) {
-        varBumpActivity(var, nbInc*var_inc);
-    }
-
-
-    bool    addClause (const vec<Lit>& ps);                     // Add a clause to the solver.
+    bool    addClause (const vec<Lit>& ps);                     // Add a clause to the solver. 
     bool    addEmptyClause();                                   // Add the empty clause, making the solver contradictory.
-    bool    addClause (Lit p);                                  // Add a unit clause to the solver.
-    bool    addClause (Lit p, Lit q);                           // Add a binary clause to the solver.
-    bool    addClause (Lit p, Lit q, Lit r);                    // Add a ternary clause to the solver.
-    virtual bool    addClause_(      vec<Lit>& ps);                     // Add a clause to the solver without making superflous internal copy. Will
+    bool    addClause (Lit p);                                  // Add a unit clause to the solver. 
+    bool    addClause (Lit p, Lit q);                           // Add a binary clause to the solver. 
+    bool    addClause (Lit p, Lit q, Lit r);                    // Add a ternary clause to the solver. 
+    bool    addClause (Lit p, Lit q, Lit r, Lit s);             // Add a quaternary clause to the solver. 
+    bool    addClause_(      vec<Lit>& ps);                     // Add a clause to the solver without making superflous internal copy. Will
                                                                 // change the passed vector 'ps'.
+
     // Solving:
     //
     bool    simplify     ();                        // Removes already satisfied clauses.
     bool    solve        (const vec<Lit>& assumps); // Search for a model that respects a given set of assumptions.
     lbool   solveLimited (const vec<Lit>& assumps); // Search for a model that respects a given set of assumptions (With resource constraints).
     bool    solve        ();                        // Search without assumptions.
     bool    solve        (Lit p);                   // Search for a model that respects a single assumption.
     bool    solve        (Lit p, Lit q);            // Search for a model that respects two assumptions.
     bool    solve        (Lit p, Lit q, Lit r);     // Search for a model that respects three assumptions.
     bool    okay         () const;                  // FALSE means solver is in a conflicting state
 
+    bool    implies      (const vec<Lit>& assumps, vec<Lit>& out);
 
-    // From pysat
-    bool prop_check(const vec<Lit>& assumps, vec<Lit>& prop, int psaving)
-    {
-        prop.clear();
+    // Iterate over clauses and top-level assignments:
+    ClauseIterator clausesBegin() const;
+    ClauseIterator clausesEnd()   const;
+    TrailIterator  trailBegin()   const;
+    TrailIterator  trailEnd  ()   const;
 
-        if (!ok)
-            return false;
-
-        bool    st = true;
-        int  level = decisionLevel();
-        CRef confl = CRef_Undef;
-
-        // dealing with phase saving
-        int psaving_copy = phase_saving;
-        phase_saving = psaving;
-
-        // propagate each assumption at a new decision level
-        for (int i = 0; st && confl == CRef_Undef && i < assumps.size(); ++i) {
-            Lit p = assumps[i];
-
-            if (value(p) == l_False)
-                st = false;
-            else if (value(p) != l_True) {
-                newDecisionLevel ();
-                uncheckedEnqueue(p);
-                confl = propagate();
-            }
-        }
-
-        // copying the result
-        if (decisionLevel() > level) {
-            for (int c = trail_lim[level]; c < trail.size(); ++c)
-                prop.push(trail[c]);
-
-            // if there is a conflict, pushing
-            // the conflicting literal as well
-            // here we may choose a wrong literal
-            // in Glucose if the clause is binary!
-            if (confl != CRef_Undef)
-                prop.push(ca[confl][0]);
-
-            // backtracking
-            cancelUntil(level);
-        }
-
-        // restoring phase saving
-        phase_saving = psaving_copy;
-
-        return st && confl == CRef_Undef;
-    }
-
-       // Convenience versions of 'toDimacs()':
     void    toDimacs     (FILE* f, const vec<Lit>& assumps);            // Write CNF to file in DIMACS-format.
     void    toDimacs     (const char *file, const vec<Lit>& assumps);
     void    toDimacs     (FILE* f, Clause& c, vec<Var>& map, Var& max);
+
+    // Convenience versions of 'toDimacs()':
     void    toDimacs     (const char* file);
     void    toDimacs     (const char* file, Lit p);
     void    toDimacs     (const char* file, Lit p, Lit q);
     void    toDimacs     (const char* file, Lit p, Lit q, Lit r);
-
-    // Display clauses and literals
-    void printLit(Lit l);
-    void printClause(CRef c);
-    void printInitialClause(CRef c);
-
+    
     // Variable mode:
-    //
-    void    setPolarity    (Var v, bool b); // Declare which polarity the decision heuristic should use for a variable. Requires mode 'polarity_user'.
-    void    setDecisionVar (Var v, bool b); // Declare if a variable should be eligible for selection in the decision heuristic.
+    // 
+    void    setPolarity    (Var v, lbool b); // Declare which polarity the decision heuristic should use for a variable. Requires mode 'polarity_user'.
+    void    setDecisionVar (Var v, bool b);  // Declare if a variable should be eligible for selection in the decision heuristic.
 
     // Read state:
     //
     lbool   value      (Var x) const;       // The current value of a variable.
     lbool   value      (Lit p) const;       // The current value of a literal.
     lbool   modelValue (Var x) const;       // The value of a variable in the last model. The last call to solve must have been satisfiable.
     lbool   modelValue (Lit p) const;       // The value of a literal in the last model. The last call to solve must have been satisfiable.
     int     nAssigns   ()      const;       // The current number of assigned literals.
     int     nClauses   ()      const;       // The current number of original clauses.
     int     nLearnts   ()      const;       // The current number of learnt clauses.
     int     nVars      ()      const;       // The current number of variables.
-    int     nFreeVars  ()      ;
+    int     nFreeVars  ()      const;
+    void    printStats ()      const;       // Print some current statistics to standard output.
 
-    inline char valuePhase(Var v) {return polarity[v];}
-
-    // Incremental mode
-    void setIncrementalMode();
-    void initNbInitialVars(int nb);
-    void printIncrementalStats();
-    bool isIncremental();
     // Resource contraints:
     //
     void    setConfBudget(int64_t x);
     void    setPropBudget(int64_t x);
     void    budgetOff();
     void    interrupt();          // Trigger a (potentially asynchronous) interruption of the solver.
     void    clearInterrupt();     // Clear interrupt indicator flag.
@@ -269,319 +116,188 @@
     virtual void garbageCollect();
     void    checkGarbage(double gf);
     void    checkGarbage();
 
     // Extra results: (read-only member variable)
     //
     vec<lbool> model;             // If problem is satisfiable, this vector contains the model (if any).
-    vec<Lit>   conflict;          // If problem is unsatisfiable (possibly under assumptions),
+    LSet       conflict;          // If problem is unsatisfiable (possibly under assumptions),
                                   // this vector represent the final conflict clause expressed in the assumptions.
 
     // Mode of operation:
     //
     int       verbosity;
-    int       verbEveryConflicts;
-    int       showModel;
-
-    // Constants For restarts
-    double    K;
-    double    R;
-    double    sizeLBDQueue;
-    double    sizeTrailQueue;
-
-    // Constants for reduce DB
-    int          firstReduceDB;
-    int          incReduceDB;
-    int          specialIncReduceDB;
-    unsigned int lbLBDFrozenClause;
-    bool         chanseokStrategy;
-    int          coLBDBound; // Keep all learnts with lbd<=coLBDBound
-    // Constant for reducing clause
-    int          lbSizeMinimizingClause;
-    unsigned int lbLBDMinimizingClause;
-    bool useLCM; // See ijcai17 (Chu Min Li paper, related to vivif).
-    bool LCMUpdateLBD; // Updates the LBD when shrinking/replacing a clause with the vivification
-
-    // Constant for heuristic
     double    var_decay;
-    double    max_var_decay;
     double    clause_decay;
     double    random_var_freq;
     double    random_seed;
+    bool      luby_restart;
     int       ccmin_mode;         // Controls conflict clause minimization (0=none, 1=basic, 2=deep).
     int       phase_saving;       // Controls the level of phase saving (0=none, 1=limited, 2=full).
     bool      rnd_pol;            // Use random polarities for branching heuristics.
     bool      rnd_init_act;       // Initialize variable activities with a small random value.
-    bool      randomizeFirstDescent; // the first decisions (until first cnflict) are made randomly
-                                     // Useful for syrup!
-
-    // Constant for Memory managment
     double    garbage_frac;       // The fraction of wasted memory allowed before a garbage collection is triggered.
+    int       min_learnts_lim;    // Minimum number to set the learnts limit to.
 
-    // Certified UNSAT ( Thanks to Marijn Heule
-    // New in 2016 : proof in DRAT format, possibility to use binary output
-    FILE*               certifiedOutput;
-    bool                certifiedUNSAT;
-    bool                vbyte;
-
-    void write_char (unsigned char c);
-    void write_lit (int n);
-    template <typename T> void addToDrat(T & lits, bool add);
-
-    // Panic mode.
-    // Save memory
-    uint32_t panicModeLastRemoved, panicModeLastRemovedShared;
-
-    bool useUnaryWatched;            // Enable unary watched literals
-    bool promoteOneWatchedClause;    // One watched clauses are promotted to two watched clauses if found empty
-
-    // Functions useful for multithread solving
-    // Useless in the sequential case
-    // Overide in ParallelSolver
-    virtual void parallelImportClauseDuringConflictAnalysis(Clause &c,CRef confl);
-    virtual bool parallelImportClauses(); // true if the empty clause was received
-    virtual void parallelImportUnaryClauses();
-    virtual void parallelExportUnaryClause(Lit p);
-    virtual void parallelExportClauseDuringSearch(Clause &c);
-    virtual bool parallelJobIsFinished();
-    virtual bool panicModeIsEnabled();
-
+    int       restart_first;      // The initial restart limit.                                                                (default 100)
+    double    restart_inc;        // The factor with which the restart limit is multiplied in each restart.                    (default 1.5)
+    double    learntsize_factor;  // The intitial limit for learnt clauses is a factor of the original clauses.                (default 1 / 3)
+    double    learntsize_inc;     // The limit for learnt clauses is multiplied with this factor each restart.                 (default 1.1)
 
-    double luby(double y, int x);
+    int       learntsize_adjust_start_confl;
+    double    learntsize_adjust_inc;
 
-    // Statistics
-    vec<uint64_t> stats;
-
-    // Important stats completely related to search. Keep here
-    uint64_t solves,starts,decisions,propagations,conflicts,conflictsRestarts;
+    // Statistics: (read-only member variable)
+    //
+    uint64_t solves, starts, decisions, rnd_decisions, propagations, conflicts;
+    uint64_t dec_vars, num_clauses, num_learnts, clauses_literals, learnts_literals, max_literals, tot_literals;
 
 protected:
 
-    long curRestart;
-
-    // Alpha variables
-    bool glureduce;
-    uint32_t restart_inc;
-    bool  luby_restart;
-    bool adaptStrategies;
-    uint32_t luby_restart_factor;
-    bool randomize_on_restarts, fixed_randomize_on_restarts, newDescent;
-    uint32_t randomDescentAssignments;
-    bool forceUnsatOnNewDescent;
     // Helper structures:
     //
     struct VarData { CRef reason; int level; };
     static inline VarData mkVarData(CRef cr, int l){ VarData d = {cr, l}; return d; }
 
     struct Watcher {
         CRef cref;
         Lit  blocker;
         Watcher(CRef cr, Lit p) : cref(cr), blocker(p) {}
         bool operator==(const Watcher& w) const { return cref == w.cref; }
         bool operator!=(const Watcher& w) const { return cref != w.cref; }
-/*        Watcher &operator=(Watcher w) {
-            this->cref = w.cref;
-            this->blocker = w.blocker;
-            return *this;
-        }
-*/
     };
 
     struct WatcherDeleted
     {
         const ClauseAllocator& ca;
         WatcherDeleted(const ClauseAllocator& _ca) : ca(_ca) {}
         bool operator()(const Watcher& w) const { return ca[w.cref].mark() == 1; }
     };
 
     struct VarOrderLt {
-        const vec<double>&  activity;
+        const IntMap<Var, double>&  activity;
         bool operator () (Var x, Var y) const { return activity[x] > activity[y]; }
-        VarOrderLt(const vec<double>&  act) : activity(act) { }
+        VarOrderLt(const IntMap<Var, double>&  act) : activity(act) { }
     };
 
+    struct ShrinkStackElem {
+        uint32_t i;
+        Lit      l;
+        ShrinkStackElem(uint32_t _i, Lit _l) : i(_i), l(_l){}
+    };
 
     // Solver state:
     //
-    int                lastIndexRed;
-    bool                ok;               // If FALSE, the constraints are already unsatisfiable. No part of the solver state may be used!
-    double              cla_inc;          // Amount to bump next clause with.
-    vec<double>         activity;         // A heuristic measurement of the activity of a variable.
-    double              var_inc;          // Amount to bump next variable with.
-    OccLists<Lit, vec<Watcher>, WatcherDeleted>
-                        watches;          // 'watches[lit]' is a list of constraints watching 'lit' (will go there if literal becomes true).
-    OccLists<Lit, vec<Watcher>, WatcherDeleted>
-                        watchesBin;          // 'watches[lit]' is a list of constraints watching 'lit' (will go there if literal becomes true).
-    OccLists<Lit, vec<Watcher>, WatcherDeleted>
-                        unaryWatches;       //  Unary watch scheme (clauses are seen when they become empty
     vec<CRef>           clauses;          // List of problem clauses.
     vec<CRef>           learnts;          // List of learnt clauses.
-    vec<CRef>           permanentLearnts; // The list of learnts clauses kept permanently
-    vec<CRef>           permanentLearntsReduced; // The list of learnts clauses kept permanently that have been reduced by LCM
-    vec<CRef>           unaryWatchedClauses;  // List of imported clauses (after the purgatory) // TODO put inside ParallelSolver
-    vec<CRef>           mostActiveClauses; // Used to keep most active clauses (instead of removing them)
-
-    vec<lbool>          assigns;          // The current assignments.
-    vec<char>           polarity;         // The preferred polarity of each variable.
-    vec<char>           forceUNSAT;
-    void                bumpForceUNSAT(Lit q); // Handles the forces
-
-    vec<char>           decision;         // Declares if a variable is eligible for selection in the decision heuristic.
     vec<Lit>            trail;            // Assignment stack; stores all assigments made in the order they were made.
-    vec<int>            nbpos;
     vec<int>            trail_lim;        // Separator indices for different decision levels in 'trail'.
-    vec<VarData>        vardata;          // Stores reason and level for each variable.
+    vec<Lit>            assumptions;      // Current set of assumptions provided to solve by the user.
+
+    VMap<double>        activity;         // A heuristic measurement of the activity of a variable.
+    VMap<lbool>         assigns;          // The current assignments.
+    VMap<char>          polarity;         // The preferred polarity of each variable.
+    VMap<lbool>         user_pol;         // The users preferred polarity of each variable.
+    VMap<char>          decision;         // Declares if a variable is eligible for selection in the decision heuristic.
+    VMap<VarData>       vardata;          // Stores reason and level for each variable.
+    OccLists<Lit, vec<Watcher>, WatcherDeleted, MkIndexLit>
+                        watches;          // 'watches[lit]' is a list of constraints watching 'lit' (will go there if literal becomes true).
+
+    Heap<Var,VarOrderLt>order_heap;       // A priority queue of variables ordered with respect to the variable activity.
+
+    bool                ok;               // If FALSE, the constraints are already unsatisfiable. No part of the solver state may be used!
+    double              cla_inc;          // Amount to bump next clause with.
+    double              var_inc;          // Amount to bump next variable with.
     int                 qhead;            // Head of queue (as index into the trail -- no more explicit propagation queue in MiniSat).
     int                 simpDB_assigns;   // Number of top-level assignments since last execution of 'simplify()'.
     int64_t             simpDB_props;     // Remaining number of propagations that must be made before next execution of 'simplify()'.
-    vec<Lit>            assumptions;      // Current set of assumptions provided to solve by the user.
-    Heap<VarOrderLt>    order_heap;       // A priority queue of variables ordered with respect to the variable activity.
     double              progress_estimate;// Set by 'search()'.
     bool                remove_satisfied; // Indicates whether possibly inefficient linear scan for satisfied clauses should be performed in 'simplify'.
-    vec<unsigned int>   permDiff;           // permDiff[var] contains the current conflict number... Used to count the number of  LBD
-
-
-    // UPDATEVARACTIVITY trick (see competition'09 companion paper)
-    vec<Lit> lastDecisionLevel;
-
+    Var                 next_var;         // Next variable to be created.
     ClauseAllocator     ca;
 
-    int nbclausesbeforereduce;            // To know when it is time to reduce clause database
-
-    // Used for restart strategies
-    bqueue<unsigned int> trailQueue,lbdQueue; // Bounded queues for restarts.
-    float sumLBD; // used to compute the global average of LBD. Restarts...
-    int sumAssumptions;
-    CRef lastLearntClause;
-
+    vec<Var>            released_vars;
+    vec<Var>            free_vars;
 
     // Temporaries (to reduce allocation overhead). Each variable is prefixed by the method in which it is
     // used, exept 'seen' wich is used in several places.
     //
-    vec<char>           seen;
-    vec<Lit>            analyze_stack;
+    VMap<char>          seen;
+    vec<ShrinkStackElem>analyze_stack;
     vec<Lit>            analyze_toclear;
     vec<Lit>            add_tmp;
-    unsigned int  MYFLAG;
 
-    // Initial reduceDB strategy
     double              max_learnts;
     double              learntsize_adjust_confl;
     int                 learntsize_adjust_cnt;
 
     // Resource contraints:
     //
     int64_t             conflict_budget;    // -1 means no budget.
     int64_t             propagation_budget; // -1 means no budget.
     bool                asynch_interrupt;
 
-    // Variables added for incremental mode
-    int incremental; // Use incremental SAT Solver
-    int nbVarsInitialFormula; // nb VAR in formula without assumptions (incremental SAT)
-    double totalTime4Sat,totalTime4Unsat;
-    int nbSatCalls,nbUnsatCalls;
-    vec<int> assumptionPositions,initialPositions;
-
-
     // Main internal methods:
     //
     void     insertVarOrder   (Var x);                                                 // Insert a variable in the decision order priority queue.
     Lit      pickBranchLit    ();                                                      // Return the next decision variable.
     void     newDecisionLevel ();                                                      // Begins a new decision level.
     void     uncheckedEnqueue (Lit p, CRef from = CRef_Undef);                         // Enqueue a literal. Assumes value of literal is undefined.
     bool     enqueue          (Lit p, CRef from = CRef_Undef);                         // Test if fact 'p' contradicts current state, enqueue otherwise.
     CRef     propagate        ();                                                      // Perform unit propagation. Returns possibly conflicting clause.
-    CRef     propagateUnaryWatches(Lit p);                                                  // Perform propagation on unary watches of p, can find only conflicts
     void     cancelUntil      (int level);                                             // Backtrack until a certain level.
-    void     analyze          (CRef confl, vec<Lit>& out_learnt, vec<Lit> & selectors, int& out_btlevel,unsigned int &nblevels,unsigned int &szWithoutSelectors);    // (bt = backtrack)
-    void     analyzeFinal     (Lit p, vec<Lit>& out_conflict);                         // COULD THIS BE IMPLEMENTED BY THE ORDINARIY "analyze" BY SOME REASONABLE GENERALIZATION?
-    bool     litRedundant     (Lit p, uint32_t abstract_levels);                       // (helper method for 'analyze()')
+    void     analyze          (CRef confl, vec<Lit>& out_learnt, int& out_btlevel);    // (bt = backtrack)
+    void     analyzeFinal     (Lit p, LSet& out_conflict);                             // COULD THIS BE IMPLEMENTED BY THE ORDINARIY "analyze" BY SOME REASONABLE GENERALIZATION?
+    bool     litRedundant     (Lit p);                                                 // (helper method for 'analyze()')
     lbool    search           (int nof_conflicts);                                     // Search for a given number of conflicts.
-    virtual lbool    solve_           (bool do_simp = true, bool turn_off_simp = false);                                                      // Main solve method (assumptions given in 'assumptions').
-    virtual void     reduceDB         ();                                              // Reduce the set of learnt clauses.
+    lbool    solve_           ();                                                      // Main solve method (assumptions given in 'assumptions').
+    void     reduceDB         ();                                                      // Reduce the set of learnt clauses.
     void     removeSatisfied  (vec<CRef>& cs);                                         // Shrink 'cs' to contain only non-satisfied clauses.
     void     rebuildOrderHeap ();
 
-    void     adaptSolver();                                                            // Adapt solver strategies
-
     // Maintaining Variable/Clause activity:
     //
     void     varDecayActivity ();                      // Decay all variables with the specified factor. Implemented by increasing the 'bump' value instead.
     void     varBumpActivity  (Var v, double inc);     // Increase a variable with the current 'bump' value.
     void     varBumpActivity  (Var v);                 // Increase a variable with the current 'bump' value.
     void     claDecayActivity ();                      // Decay all clauses with the specified factor. Implemented by increasing the 'bump' value instead.
     void     claBumpActivity  (Clause& c);             // Increase a clause with the current 'bump' value.
 
     // Operations on clauses:
     //
     void     attachClause     (CRef cr);               // Attach a clause to watcher lists.
     void     detachClause     (CRef cr, bool strict = false); // Detach a clause to watcher lists.
-    void     detachClausePurgatory(CRef cr, bool strict = false);
-    void     attachClausePurgatory(CRef cr);
-    void     removeClause     (CRef cr, bool inPurgatory = false);               // Detach and free a clause.
+    void     removeClause     (CRef cr);               // Detach and free a clause.
+    bool     isRemoved        (CRef cr) const;         // Test if a clause has been removed.
     bool     locked           (const Clause& c) const; // Returns TRUE if a clause is a reason for some implication in the current state.
     bool     satisfied        (const Clause& c) const; // Returns TRUE if a clause is satisfied in the current state.
 
-    template <typename T> unsigned int computeLBD(const T & lits,int end=-1);
-    void minimisationWithBinaryResolution(vec<Lit> &out_learnt);
-
-    virtual void     relocAll         (ClauseAllocator& to);
-
     // Misc:
     //
     int      decisionLevel    ()      const; // Gives the current decisionlevel.
     uint32_t abstractLevel    (Var x) const; // Used to represent an abstraction of sets of decision levels.
     CRef     reason           (Var x) const;
     int      level            (Var x) const;
     double   progressEstimate ()      const; // DELETE THIS ?? IT'S NOT VERY USEFUL ...
     bool     withinBudget     ()      const;
-    inline bool isSelector(Var v) {return (incremental && v>nbVarsInitialFormula);}
+    void     relocAll         (ClauseAllocator& to);
 
     // Static helpers:
     //
 
     // Returns a random float 0 <= x < 1. Seed must never be 0.
     static inline double drand(double& seed) {
         seed *= 1389796;
         int q = (int)(seed / 2147483647);
         seed -= (double)q * 2147483647;
         return seed / 2147483647; }
 
     // Returns a random integer 0 <= x < size. Seed must never be 0.
     static inline int irand(double& seed, int size) {
         return (int)(drand(seed) * size); }
-
-
-    // simplify
-    //
-public:
-    bool	simplifyAll();
-    void	simplifyLearnt(Clause& c);
-    int		trailRecord;
-    void	litsEnqueue(int cutP, Clause& c);
-    void	cancelUntilTrailRecord();
-    void	simpleUncheckEnqueue(Lit p, CRef from = CRef_Undef);
-    CRef    simplePropagate();
-    CRef    simplePropagateUnaryWatches(Lit p);
-
-    vec<Lit> simp_learnt_clause;
-    vec<CRef> simp_reason_clause;
-    void	simpleAnalyze(CRef confl, vec<Lit>& out_learnt, vec<CRef>& reason_clause, bool True_confl);
-    // sort learnt clause literal by litValue
-
-    // in redundant
-    bool removed(CRef cr);
-    int performLCM;
-
-    //// test
-    vec<int> valueDup;
-    void compareValue();
-    void wholeCompareValue();
-
-
 };
 
 
 //=================================================================================================
 // Implementation of inline methods:
 
 inline CRef Solver::reason(Var x) const { return vardata[x].reason; }
@@ -619,42 +335,37 @@
 // NOTE: enqueue does not set the ok flag! (only public methods do)
 inline bool     Solver::enqueue         (Lit p, CRef from)      { return value(p) != l_Undef ? value(p) != l_False : (uncheckedEnqueue(p, from), true); }
 inline bool     Solver::addClause       (const vec<Lit>& ps)    { ps.copyTo(add_tmp); return addClause_(add_tmp); }
 inline bool     Solver::addEmptyClause  ()                      { add_tmp.clear(); return addClause_(add_tmp); }
 inline bool     Solver::addClause       (Lit p)                 { add_tmp.clear(); add_tmp.push(p); return addClause_(add_tmp); }
 inline bool     Solver::addClause       (Lit p, Lit q)          { add_tmp.clear(); add_tmp.push(p); add_tmp.push(q); return addClause_(add_tmp); }
 inline bool     Solver::addClause       (Lit p, Lit q, Lit r)   { add_tmp.clear(); add_tmp.push(p); add_tmp.push(q); add_tmp.push(r); return addClause_(add_tmp); }
- inline bool     Solver::locked          (const Clause& c) const {
-   if(c.size()>2)
-     return value(c[0]) == l_True && reason(var(c[0])) != CRef_Undef && ca.lea(reason(var(c[0]))) == &c;
-   return
-     (value(c[0]) == l_True && reason(var(c[0])) != CRef_Undef && ca.lea(reason(var(c[0]))) == &c)
-     ||
-     (value(c[1]) == l_True && reason(var(c[1])) != CRef_Undef && ca.lea(reason(var(c[1]))) == &c);
- }
+inline bool     Solver::addClause       (Lit p, Lit q, Lit r, Lit s){ add_tmp.clear(); add_tmp.push(p); add_tmp.push(q); add_tmp.push(r); add_tmp.push(s); return addClause_(add_tmp); }
+
+inline bool     Solver::isRemoved       (CRef cr)         const { return ca[cr].mark() == 1; }
+inline bool     Solver::locked          (const Clause& c) const { return value(c[0]) == l_True && reason(var(c[0])) != CRef_Undef && ca.lea(reason(var(c[0]))) == &c; }
 inline void     Solver::newDecisionLevel()                      { trail_lim.push(trail.size()); }
 
 inline int      Solver::decisionLevel ()      const   { return trail_lim.size(); }
 inline uint32_t Solver::abstractLevel (Var x) const   { return 1 << (level(x) & 31); }
 inline lbool    Solver::value         (Var x) const   { return assigns[x]; }
 inline lbool    Solver::value         (Lit p) const   { return assigns[var(p)] ^ sign(p); }
 inline lbool    Solver::modelValue    (Var x) const   { return model[x]; }
 inline lbool    Solver::modelValue    (Lit p) const   { return model[var(p)] ^ sign(p); }
 inline int      Solver::nAssigns      ()      const   { return trail.size(); }
-inline int      Solver::nClauses      ()      const   { return clauses.size(); }
-inline int      Solver::nLearnts      ()      const   { return learnts.size(); }
-inline int      Solver::nVars         ()      const   { return vardata.size(); }
-inline int      Solver::nFreeVars     ()         {
-    int a = stats[dec_vars];
-    return (int)(a) - (trail_lim.size() == 0 ? trail.size() : trail_lim[0]); }
-inline void     Solver::setPolarity   (Var v, bool b) { polarity[v] = b; }
-inline void     Solver::setDecisionVar(Var v, bool b)
-{
-    if      ( b && !decision[v]) stats[dec_vars]++;
-    else if (!b &&  decision[v]) stats[dec_vars]--;
+inline int      Solver::nClauses      ()      const   { return num_clauses; }
+inline int      Solver::nLearnts      ()      const   { return num_learnts; }
+inline int      Solver::nVars         ()      const   { return next_var; }
+// TODO: nFreeVars() is not quite correct, try to calculate right instead of adapting it like below:
+inline int      Solver::nFreeVars     ()      const   { return (int)dec_vars - (trail_lim.size() == 0 ? trail.size() : trail_lim[0]); }
+inline void     Solver::setPolarity   (Var v, lbool b){ user_pol[v] = b; }
+inline void     Solver::setDecisionVar(Var v, bool b) 
+{ 
+    if      ( b && !decision[v]) dec_vars++;
+    else if (!b &&  decision[v]) dec_vars--;
 
     decision[v] = b;
     insertVarOrder(v);
 }
 inline void     Solver::setConfBudget(int64_t x){ conflict_budget    = conflicts    + x; }
 inline void     Solver::setPropBudget(int64_t x){ propagation_budget = propagations + x; }
 inline void     Solver::interrupt(){ asynch_interrupt = true; }
@@ -672,154 +383,27 @@
 inline bool     Solver::solve         (Lit p)               { budgetOff(); assumptions.clear(); assumptions.push(p); return solve_() == l_True; }
 inline bool     Solver::solve         (Lit p, Lit q)        { budgetOff(); assumptions.clear(); assumptions.push(p); assumptions.push(q); return solve_() == l_True; }
 inline bool     Solver::solve         (Lit p, Lit q, Lit r) { budgetOff(); assumptions.clear(); assumptions.push(p); assumptions.push(q); assumptions.push(r); return solve_() == l_True; }
 inline bool     Solver::solve         (const vec<Lit>& assumps){ budgetOff(); assumps.copyTo(assumptions); return solve_() == l_True; }
 inline lbool    Solver::solveLimited  (const vec<Lit>& assumps){ assumps.copyTo(assumptions); return solve_(); }
 inline bool     Solver::okay          ()      const   { return ok; }
 
+inline ClauseIterator Solver::clausesBegin() const { return ClauseIterator(ca, &clauses[0]); }
+inline ClauseIterator Solver::clausesEnd  () const { return ClauseIterator(ca, &clauses[clauses.size()]); }
+inline TrailIterator  Solver::trailBegin  () const { return TrailIterator(&trail[0]); }
+inline TrailIterator  Solver::trailEnd    () const { 
+    return TrailIterator(&trail[decisionLevel() == 0 ? trail.size() : trail_lim[0]]); }
+
 inline void     Solver::toDimacs     (const char* file){ vec<Lit> as; toDimacs(file, as); }
 inline void     Solver::toDimacs     (const char* file, Lit p){ vec<Lit> as; as.push(p); toDimacs(file, as); }
 inline void     Solver::toDimacs     (const char* file, Lit p, Lit q){ vec<Lit> as; as.push(p); as.push(q); toDimacs(file, as); }
 inline void     Solver::toDimacs     (const char* file, Lit p, Lit q, Lit r){ vec<Lit> as; as.push(p); as.push(q); as.push(r); toDimacs(file, as); }
 
 
-/************************************************************
- * Compute LBD functions
- *************************************************************/
-
-template <typename T>inline unsigned int Solver::computeLBD(const T &lits, int end) {
-    int nblevels = 0;
-    MYFLAG++;
-#ifdef INCREMENTAL
-    if(incremental) { // ----------------- INCREMENTAL MODE
-      if(end==-1) end = lits.size();
-      int nbDone = 0;
-      for(int i=0;i<lits.size();i++) {
-        if(nbDone>=end) break;
-        if(isSelector(var(lits[i]))) continue;
-        nbDone++;
-        int l = level(var(lits[i]));
-        if (permDiff[l] != MYFLAG) {
-      permDiff[l] = MYFLAG;
-      nblevels++;
-        }
-      }
-    } else { // -------- DEFAULT MODE. NOT A LOT OF DIFFERENCES... BUT EASIER TO READ
-#endif
-    for(int i = 0; i < lits.size(); i++) {
-        int l = level(var(lits[i]));
-        if(permDiff[l] != MYFLAG) {
-            permDiff[l] = MYFLAG;
-            nblevels++;
-        }
-    }
-#ifdef INCREMENTAL
-    }
-#endif
-    return nblevels;
-}
-
-
-
 //=================================================================================================
 // Debug etc:
 
 
-inline void Solver::printLit(Lit l)
-{
-    printf("%s%d:%c", sign(l) ? "-" : "", var(l)+1, value(l) == l_True ? '1' : (value(l) == l_False ? '0' : 'X'));
-}
-
-
-inline void Solver::printClause(CRef cr)
-{
-  Clause &c = ca[cr];
-    for (int i = 0; i < c.size(); i++){
-        printLit(c[i]);
-        printf(" ");
-    }
-}
-
-inline void Solver::printInitialClause(CRef cr)
-{
-  Clause &c = ca[cr];
-    for (int i = 0; i < c.size(); i++){
-      if(!isSelector(var(c[i]))) {
-	printLit(c[i]);
-        printf(" ");
-      }
-    }
-}
-
-template <typename T>inline void Solver::addToDrat(T &lits, bool add) {
-    if(vbyte) {
-        if(add)
-            write_char('a');
-        else
-            write_char('d');
-        for(int i = 0; i < lits.size(); i++)
-            write_lit(2 * (var(lits[i]) + 1) + sign(lits[i]));
-        write_lit(0);
-    }
-    else {
-        if(!add)
-            fprintf(certifiedOutput, "d ");
-
-        for(int i = 0; i < lits.size(); i++)
-            fprintf(certifiedOutput, "%i ", (var(lits[i]) + 1) * (-2 * sign(lits[i]) + 1));
-        fprintf(certifiedOutput, "0\n");
-    }
-}
-
-
-
 //=================================================================================================
-struct reduceDBAct_lt {
-    ClauseAllocator& ca;
-
-    reduceDBAct_lt(ClauseAllocator& ca_) : ca(ca_) {
-    }
-
-    bool operator()(CRef x, CRef y) {
-
-        // Main criteria... Like in MiniSat we keep all binary clauses
-        if (ca[x].size() > 2 && ca[y].size() == 2) return 1;
-
-        if (ca[y].size() > 2 && ca[x].size() == 2) return 0;
-        if (ca[x].size() == 2 && ca[y].size() == 2) return 0;
-
-        return ca[x].activity() < ca[y].activity();
-    }
-};
-
-struct reduceDB_lt {
-    ClauseAllocator& ca;
-
-    reduceDB_lt(ClauseAllocator& ca_) : ca(ca_) {
-    }
-
-    bool operator()(CRef x, CRef y) {
-
-        // Main criteria... Like in MiniSat we keep all binary clauses
-        if (ca[x].size() > 2 && ca[y].size() == 2) return 1;
-
-        if (ca[y].size() > 2 && ca[x].size() == 2) return 0;
-        if (ca[x].size() == 2 && ca[y].size() == 2) return 0;
-
-        // Second one  based on literal block distance
-        if (ca[x].lbd() > ca[y].lbd()) return 1;
-        if (ca[x].lbd() < ca[y].lbd()) return 0;
-
-
-        // Finally we can use old activity or size, we choose the last one
-        return ca[x].activity() < ca[y].activity();
-        //return x->size() < y->size();
-
-        //return ca[x].size() > 2 && (ca[y].size() == 2 || ca[x].activity() < ca[y].activity()); }
-    }
-};
-
-
 }
 
-
 #endif
```

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Alloc.h` & `lincs-0.6.0/lincs/liblincs/vendored/minisat/mtl/Alloc.h`

 * *Files 14% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT
 OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 **************************************************************************************************/
 
 
-#ifndef Glucose_Alloc_h
-#define Glucose_Alloc_h
+#ifndef Minisat_Alloc_h
+#define Minisat_Alloc_h
 
 #include "XAlloc.h"
 #include "Vec.h"
 
-namespace Glucose {
+namespace Minisat {
 
 //=================================================================================================
 // Simple Region-based memory allocator:
 
 template<class T>
 class RegionAllocator
 {
@@ -39,92 +39,82 @@
 
     void capacity(uint32_t min_cap);
 
  public:
     // TODO: make this a class for better type-checking?
     typedef uint32_t Ref;
     enum { Ref_Undef = UINT32_MAX };
-    enum { Unit_Size = sizeof(uint32_t) };
+    enum { Unit_Size = sizeof(T) };
 
     explicit RegionAllocator(uint32_t start_cap = 1024*1024) : memory(NULL), sz(0), cap(0), wasted_(0){ capacity(start_cap); }
     ~RegionAllocator()
     {
         if (memory != NULL)
             ::free(memory);
     }
 
 
     uint32_t size      () const      { return sz; }
-    uint32_t getCap    () const      { return cap;}
     uint32_t wasted    () const      { return wasted_; }
 
     Ref      alloc     (int size); 
     void     free      (int size)    { wasted_ += size; }
 
     // Deref, Load Effective Address (LEA), Inverse of LEA (AEL):
-    T&       operator[](Ref r)       { assert(r >= 0 && r < sz); return memory[r]; }
-    const T& operator[](Ref r) const { assert(r >= 0 && r < sz); return memory[r]; }
+    T&       operator[](Ref r)       { assert(r < sz); return memory[r]; }
+    const T& operator[](Ref r) const { assert(r < sz); return memory[r]; }
 
-    T*       lea       (Ref r)       { assert(r >= 0 && r < sz); return &memory[r]; }
-    const T* lea       (Ref r) const { assert(r >= 0 && r < sz); return &memory[r]; }
+    T*       lea       (Ref r)       { assert(r < sz); return &memory[r]; }
+    const T* lea       (Ref r) const { assert(r < sz); return &memory[r]; }
     Ref      ael       (const T* t)  { assert((void*)t >= (void*)&memory[0] && (void*)t < (void*)&memory[sz-1]);
         return  (Ref)(t - &memory[0]); }
 
     void     moveTo(RegionAllocator& to) {
         if (to.memory != NULL) ::free(to.memory);
         to.memory = memory;
         to.sz = sz;
         to.cap = cap;
         to.wasted_ = wasted_;
 
         memory = NULL;
         sz = cap = wasted_ = 0;
     }
 
-    void copyTo(RegionAllocator& to) const {
-     //   if (to.memory != NULL) ::free(to.memory);
-        to.memory = (T*)xrealloc(to.memory, sizeof(T)*cap);
-        memcpy(to.memory,memory,sizeof(T)*cap);        
-        to.sz = sz;
-        to.cap = cap;
-        to.wasted_ = wasted_;
-    }
-
-
 
 };
 
 template<class T>
 void RegionAllocator<T>::capacity(uint32_t min_cap)
 {
     if (cap >= min_cap) return;
+
     uint32_t prev_cap = cap;
     while (cap < min_cap){
         // NOTE: Multiply by a factor (13/8) without causing overflow, then add 2 and make the
         // result even by clearing the least significant bit. The resulting sequence of capacities
         // is carefully chosen to hit a maximum capacity that is close to the '2^32-1' limit when
         // using 'uint32_t' as indices so that as much as possible of this space can be used.
         uint32_t delta = ((cap >> 1) + (cap >> 3) + 2) & ~1;
         cap += delta;
 
         if (cap <= prev_cap)
             throw OutOfMemoryException();
     }
-    //printf(" .. (%p) cap = %u\n", this, cap);
+    // printf(" .. (%p) cap = %u\n", this, cap);
 
     assert(cap > 0);
     memory = (T*)xrealloc(memory, sizeof(T)*cap);
 }
 
 
 template<class T>
 typename RegionAllocator<T>::Ref
 RegionAllocator<T>::alloc(int size)
 { 
-    //printf("ALLOC called (this = %p, size = %d)\n", this, size); fflush(stdout);
+    // printf("ALLOC called (this = %p, size = %d)\n", this, size); fflush(stdout);
     assert(size > 0);
     capacity(sz + size);
 
     uint32_t prev_sz = sz;
     sz += size;
     
     // Handle overflow:
```

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Heap.h` & `lincs-0.6.0/lincs/liblincs/vendored/minisat/mtl/Heap.h`

 * *Files 15% similar despite different names*

```diff
@@ -14,43 +14,41 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT
 NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT
 OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 **************************************************************************************************/
 
-#ifndef Glucose_Heap_h
-#define Glucose_Heap_h
+#ifndef Minisat_Heap_h
+#define Minisat_Heap_h
 
 #include "Vec.h"
+#include "IntMap.h"
 
-#include <iostream>
-
-namespace Glucose {
+namespace Minisat {
 
 //=================================================================================================
 // A heap implementation with support for decrease/increase key.
 
 
-template<class Comp>
+template<class K, class Comp, class MkIndex = MkIndexDefault<K> >
 class Heap {
-    Comp     lt;       // The heap is a minimum-heap with respect to this comparator
-    vec<int> heap;     // Heap of integers
-    vec<int> indices;  // Each integers position (index) in the Heap
+    vec<K>                heap;     // Heap of Keys
+    IntMap<K,int,MkIndex> indices;  // Each Key's position (index) in the Heap
+    Comp                  lt;       // The heap is a minimum-heap with respect to this comparator
 
     // Index "traversal" functions
     static inline int left  (int i) { return i*2+1; }
     static inline int right (int i) { return (i+1)*2; }
     static inline int parent(int i) { return (i-1) >> 1; }
 
 
-
     void percolateUp(int i)
     {
-        int x  = heap[i];
+        K   x  = heap[i];
         int p  = parent(i);
         
         while (i != 0 && lt(x, heap[p])){
             heap[i]          = heap[p];
             indices[heap[p]] = i;
             i                = p;
             p                = parent(p);
@@ -58,94 +56,112 @@
         heap   [i] = x;
         indices[x] = i;
     }
 
 
     void percolateDown(int i)
     {
-        int x = heap[i];
+        K x = heap[i];
         while (left(i) < heap.size()){
             int child = right(i) < heap.size() && lt(heap[right(i)], heap[left(i)]) ? right(i) : left(i);
             if (!lt(heap[child], x)) break;
             heap[i]          = heap[child];
             indices[heap[i]] = i;
             i                = child;
         }
         heap   [i] = x;
         indices[x] = i;
     }
 
 
   public:
-    Heap(const Comp& c) : lt(c) { }
+    Heap(const Comp& c, MkIndex _index = MkIndex()) : indices(_index), lt(c) {}
 
     int  size      ()          const { return heap.size(); }
     bool empty     ()          const { return heap.size() == 0; }
-    bool inHeap    (int n)     const { return n < indices.size() && indices[n] >= 0; }
+    bool inHeap    (K k)       const { return indices.has(k) && indices[k] >= 0; }
     int  operator[](int index) const { assert(index < heap.size()); return heap[index]; }
 
+    void decrease  (K k) { assert(inHeap(k)); percolateUp  (indices[k]); }
+    void increase  (K k) { assert(inHeap(k)); percolateDown(indices[k]); }
 
-    void decrease  (int n) { assert(inHeap(n)); percolateUp  (indices[n]); }
-    void increase  (int n) { assert(inHeap(n)); percolateDown(indices[n]); }
-
-    void copyTo(Heap& copy) const {heap.copyTo(copy.heap);indices.copyTo(copy.indices);}
 
     // Safe variant of insert/decrease/increase:
-    void update(int n)
+    void update(K k)
     {
-        if (!inHeap(n))
-            insert(n);
+        if (!inHeap(k))
+            insert(k);
         else {
-            percolateUp(indices[n]);
-            percolateDown(indices[n]); }
+            percolateUp(indices[k]);
+            percolateDown(indices[k]); }
     }
 
 
-    void insert(int n)
+    void insert(K k)
     {
-        indices.growTo(n+1, -1);
-        assert(!inHeap(n));
+        indices.reserve(k, -1);
+        assert(!inHeap(k));
+
+        indices[k] = heap.size();
+        heap.push(k);
+        percolateUp(indices[k]);
+    }
+
+
+    void remove(K k)
+    {
+        assert(inHeap(k));
+
+        int k_pos  = indices[k];
+        indices[k] = -1;
 
-        indices[n] = heap.size();
-        heap.push(n);
-        percolateUp(indices[n]); 
+        if (k_pos < heap.size()-1){
+            heap[k_pos]          = heap.last();
+            indices[heap[k_pos]] = k_pos;
+            heap.pop();
+            percolateDown(k_pos);
+        }else
+            heap.pop();
     }
 
 
-    int  removeMin()
+    K removeMin()
     {
-        int x            = heap[0];
+        K x              = heap[0];
         heap[0]          = heap.last();
         indices[heap[0]] = 0;
         indices[x]       = -1;
         heap.pop();
         if (heap.size() > 1) percolateDown(0);
         return x; 
     }
 
 
     // Rebuild the heap from scratch, using the elements in 'ns':
-    void build(vec<int>& ns) {
+    void build(const vec<K>& ns) {
         for (int i = 0; i < heap.size(); i++)
             indices[heap[i]] = -1;
         heap.clear();
 
         for (int i = 0; i < ns.size(); i++){
+            // TODO: this should probably call reserve instead of relying on it being reserved already.
+            assert(indices.has(ns[i]));
             indices[ns[i]] = i;
             heap.push(ns[i]); }
 
         for (int i = heap.size() / 2 - 1; i >= 0; i--)
             percolateDown(i);
     }
 
-    void clear(bool dealloc = false) 
+    void clear(bool dispose = false) 
     { 
+        // TODO: shouldn't the 'indices' map also be dispose-cleared?
         for (int i = 0; i < heap.size(); i++)
             indices[heap[i]] = -1;
-        heap.clear(dealloc); 
+        heap.clear(dispose); 
     }
 };
 
 
 //=================================================================================================
 }
```

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/IntTypes.h` & `lincs-0.6.0/lincs/liblincs/vendored/minisat/mtl/IntTypes.h`

 * *Files 14% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT
 NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT
 OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 **************************************************************************************************/
 
-#ifndef Glucose_IntTypes_h
-#define Glucose_IntTypes_h
+#ifndef Minisat_IntTypes_h
+#define Minisat_IntTypes_h
 
 #ifdef __sun
     // Not sure if there are newer versions that support C99 headers. The
     // needed features are implemented in the headers below though:
 
 #   include <sys/int_types.h>
 #   include <sys/int_fmtio.h>
@@ -33,14 +33,10 @@
 #   include <stdint.h>
 #   include <inttypes.h>
 
 #endif
 
 #include <limits.h>
 
-#ifndef PRIu64
-#define PRIu64 "lu"
-#define PRIi64 "ld"
-#endif
 //=================================================================================================
 
 #endif
```

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Map.h` & `lincs-0.6.0/lincs/liblincs/vendored/minisat/mtl/Map.h`

 * *Files 8% similar despite different names*

```diff
@@ -13,30 +13,26 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT
 NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT
 OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 **************************************************************************************************/
 
-#ifndef Glucose_Map_h
-#define Glucose_Map_h
+#ifndef Minisat_Map_h
+#define Minisat_Map_h
 
 #include "IntTypes.h"
 #include "Vec.h"
-#include <string>
-#include <unordered_map>
 
-namespace Glucose {
+namespace Minisat {
 
 //=================================================================================================
 // Default hash/equals functions
 //
 
-static inline uint32_t hash(std::string x) {std::hash<std::string> hasher;return hasher(x); }
-
 template<class K> struct Hash  { uint32_t operator()(const K& k)               const { return hash(k);  } };
 template<class K> struct Equal { bool     operator()(const K& k1, const K& k2) const { return k1 == k2; } };
 
 template<class K> struct DeepHash  { uint32_t operator()(const K* k)               const { return hash(*k);  } };
 template<class K> struct DeepEqual { bool     operator()(const K* k1, const K* k2) const { return *k1 == *k2; } };
 
 static inline uint32_t hash(uint32_t x){ return x; }
@@ -66,16 +62,16 @@
     E          equals;
 
     vec<Pair>* table;
     int        cap;
     int        size;
 
     // Don't allow copying (error prone):
-    Map<K,D,H,E>&  operator = (Map<K,D,H,E>& other) { assert(0); }
-                   Map        (Map<K,D,H,E>& other) { assert(0); }
+    Map<K,D,H,E>&  operator = (Map<K,D,H,E>& other);
+                   Map        (Map<K,D,H,E>& other);
 
     bool    checkCap(int new_size) const { return new_size > cap; }
 
     int32_t index  (const K& k) const { return hash(k) % cap; }
     void   _insert (const K& k, const D& d) { 
         vec<Pair>& ps = table[index(k)];
         ps.push(); ps.last().key = k; ps.last().data = d; }
@@ -112,30 +108,27 @@
     {
         assert(size != 0);
         const D*         res = NULL;
         const vec<Pair>& ps  = table[index(k)];
         for (int i = 0; i < ps.size(); i++)
             if (equals(ps[i].key, k))
                 res = &ps[i].data;
-//        if(res==NULL) printf("%s\n",k.c_str());
         assert(res != NULL);
         return *res;
     }
 
     // PRECONDITION: the key must already exist in the map.
     D& operator [] (const K& k)
     {
         assert(size != 0);
         D*         res = NULL;
         vec<Pair>& ps  = table[index(k)];
         for (int i = 0; i < ps.size(); i++)
             if (equals(ps[i].key, k))
                 res = &ps[i].data;
-//        if(res==NULL) printf("%s\n",k.c_str());
-
         assert(res != NULL);
         return *res;
     }
 
     // PRECONDITION: the key must *NOT* exist in the map.
     void insert (const K& k, const D& d) { if (checkCap(size+1)) rehash(); _insert(k, d); size++; }
     bool peek   (const K& k, D& d) const {
```

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Queue.h` & `lincs-0.6.0/lincs/liblincs/vendored/minisat/mtl/Queue.h`

 * *Files 10% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT
 NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT
 OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 **************************************************************************************************/
 
-#ifndef Glucose_Queue_h
-#define Glucose_Queue_h
+#ifndef Minisat_Queue_h
+#define Minisat_Queue_h
 
 #include "Vec.h"
 
-namespace Glucose {
+namespace Minisat {
 
 //=================================================================================================
 
 template<class T>
 class Queue {
     vec<T>  buf;
     int     first;
@@ -37,30 +37,19 @@
     typedef T Key;
 
     Queue() : buf(1), first(0), end(0) {}
 
     void clear (bool dealloc = false) { buf.clear(dealloc); buf.growTo(1); first = end = 0; }
     int  size  () const { return (end >= first) ? end - first : end - first + buf.size(); }
 
-    
-    
     const T& operator [] (int index) const  { assert(index >= 0); assert(index < size()); return buf[(first + index) % buf.size()]; }
     T&       operator [] (int index)        { assert(index >= 0); assert(index < size()); return buf[(first + index) % buf.size()]; }
 
     T    peek  () const { assert(first != end); return buf[first]; }
     void pop   () { assert(first != end); first++; if (first == buf.size()) first = 0; }
-    
-    
-    void copyTo(Queue<T>& copy) const {
-        copy.first = first;
-        copy.end = end;
-        buf.memCopyTo(copy.buf);
-    }
-    
-    
     void insert(T elem) {   // INVARIANT: buf[end] is always unused
         buf[end++] = elem;
         if (end == buf.size()) end = 0;
         if (first == end){  // Resize:
             vec<T>  tmp((buf.size()*3 + 1) >> 1);
             //**/printf("queue alloc: %d elems (%.1f MB)\n", tmp.size(), tmp.size() * sizeof(T) / 1000000.0);
             int     i = 0;
```

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Sort.h` & `lincs-0.6.0/lincs/liblincs/vendored/minisat/mtl/Sort.h`

 * *Files 6% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT
 NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT
 OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 **************************************************************************************************/
 
-#ifndef Glucose_Sort_h
-#define Glucose_Sort_h
+#ifndef Minisat_Sort_h
+#define Minisat_Sort_h
 
 #include "Vec.h"
 
 //=================================================================================================
 // Some sorting algorithms for vec's
 
 
-namespace Glucose {
+namespace Minisat {
 
 template<class T>
 struct LessThan_default {
     bool operator () (T x, T y) { return x < y; }
 };
```

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Vec.h` & `lincs-0.6.0/lincs/liblincs/vendored/minisat/mtl/Vec.h`

 * *Files 20% similar despite different names*

```diff
@@ -14,139 +14,121 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT
 NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT
 OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 **************************************************************************************************/
 
-#ifndef Glucose_Vec_h
-#define Glucose_Vec_h
+#ifndef Minisat_Vec_h
+#define Minisat_Vec_h
 
 #include <assert.h>
+#include <limits>
 #include <new>
 
 #include "IntTypes.h"
 #include "XAlloc.h"
-#include <string.h>
 
-namespace Glucose {
+namespace Minisat {
 
 //=================================================================================================
 // Automatically resizable arrays
 //
 // NOTE! Don't use this vector on datatypes that cannot be re-located in memory (with realloc)
 
-template<class T>
+template<class T, class _Size = int>
 class vec {
-    T*  data;
-    int sz;
-    int cap;
+public:
+    typedef _Size Size;
+private:
+    T*   data;
+    Size sz;
+    Size cap;
 
     // Don't allow copying (error prone):
-    vec<T>&  operator = (vec<T>& other) { assert(0); return *this; }
-             vec        (vec<T>& other) { assert(0); }
-             
-    // Helpers for calculating next capacity:
-    static inline int  imax   (int x, int y) { int mask = (y-x) >> (sizeof(int)*8-1); return (x&mask) + (y&(~mask)); }
-    //static inline void nextCap(int& cap){ cap += ((cap >> 1) + 2) & ~1; }
-    static inline void nextCap(int& cap){ cap += ((cap >> 1) + 2) & ~1; }
+    vec<T>&  operator=(vec<T>& other);
+             vec      (vec<T>& other);
+
+    static inline Size max(Size x, Size y){ return (x > y) ? x : y; }
 
 public:
     // Constructors:
-    vec()                       : data(NULL) , sz(0)   , cap(0)    { }
-    explicit vec(int size)      : data(NULL) , sz(0)   , cap(0)    { growTo(size); }
-    vec(int size, const T& pad) : data(NULL) , sz(0)   , cap(0)    { growTo(size, pad); }
-   ~vec()                                                          { clear(true); }
+    vec()                        : data(NULL), sz(0), cap(0)    { }
+    explicit vec(Size size)      : data(NULL), sz(0), cap(0)    { growTo(size); }
+    vec(Size size, const T& pad) : data(NULL), sz(0), cap(0)    { growTo(size, pad); }
+   ~vec()                                                       { clear(true); }
 
     // Pointer to first element:
     operator T*       (void)           { return data; }
 
     // Size operations:
-    int      size     (void) const     { return sz; }
-    void     shrink   (int nelems)     { assert(nelems <= sz); for (int i = 0; i < nelems; i++) sz--, data[sz].~T(); }
-    void     shrink_  (int nelems)     { assert(nelems <= sz); sz -= nelems; }
-    int      capacity (void) const     { return cap; }
-    void     capacity (int min_cap);
-    void     growTo   (int size);
-    void     growTo   (int size, const T& pad);
+    Size     size     (void) const   { return sz; }
+    void     shrink   (Size nelems)  { assert(nelems <= sz); for (Size i = 0; i < nelems; i++) sz--, data[sz].~T(); }
+    void     shrink_  (Size nelems)  { assert(nelems <= sz); sz -= nelems; }
+    int      capacity (void) const   { return cap; }
+    void     capacity (Size min_cap);
+    void     growTo   (Size size);
+    void     growTo   (Size size, const T& pad);
     void     clear    (bool dealloc = false);
 
     // Stack interface:
     void     push  (void)              { if (sz == cap) capacity(sz+1); new (&data[sz]) T(); sz++; }
-    void     push  (const T& elem)     { if (sz == cap) capacity(sz+1); data[sz++] = elem; }
+    //void     push  (const T& elem)     { if (sz == cap) capacity(sz+1); data[sz++] = elem; }
+    void     push  (const T& elem)     { if (sz == cap) capacity(sz+1); new (&data[sz++]) T(elem); }
     void     push_ (const T& elem)     { assert(sz < cap); data[sz++] = elem; }
     void     pop   (void)              { assert(sz > 0); sz--, data[sz].~T(); }
-    
-    void     remove(const T &elem) {
-        int tmp;
-        for(tmp = 0;tmp<sz;tmp++) {
-            if(data[tmp]==elem) 
-                break;
-        }
-        if(tmp<sz) {
-            assert(data[tmp] == elem);
-            data[tmp] = data[sz-1];
-            sz = sz - 1;
-        }
-        
-    }
-    
     // NOTE: it seems possible that overflow can happen in the 'sz+1' expression of 'push()', but
     // in fact it can not since it requires that 'cap' is equal to INT_MAX. This in turn can not
     // happen given the way capacities are calculated (below). Essentially, all capacities are
     // even, but INT_MAX is odd.
 
     const T& last  (void) const        { return data[sz-1]; }
     T&       last  (void)              { return data[sz-1]; }
 
     // Vector interface:
-    const T& operator [] (int index) const { return data[index]; }
-    T&       operator [] (int index)       { return data[index]; }
+    const T& operator [] (Size index) const { return data[index]; }
+    T&       operator [] (Size index)       { return data[index]; }
 
     // Duplicatation (preferred instead):
-    void copyTo(vec<T>& copy) const { copy.clear(); copy.growTo(sz); for (int i = 0; i < sz; i++) copy[i] = data[i]; }
+    void copyTo(vec<T>& copy) const { copy.clear(); copy.growTo(sz); for (Size i = 0; i < sz; i++) copy[i] = data[i]; }
     void moveTo(vec<T>& dest) { dest.clear(true); dest.data = data; dest.sz = sz; dest.cap = cap; data = NULL; sz = 0; cap = 0; }
-    void memCopyTo(vec<T>& copy) const{
-        copy.capacity(cap);
-        copy.sz = sz;
-        memcpy(copy.data,data,sizeof(T)*cap);
-    }
-
 };
 
 
-template<class T>
-void vec<T>::capacity(int min_cap) {
+template<class T, class _Size>
+void vec<T,_Size>::capacity(Size min_cap) {
     if (cap >= min_cap) return;
-    int add = imax((min_cap - cap + 1) & ~1, ((cap >> 1) + 2) & ~1);   // NOTE: grow by approximately 3/2
-    if (add > INT_MAX - cap || (((data = (T*)::realloc(data, (cap += add) * sizeof(T))) == NULL) && errno == ENOMEM))
+    Size add = max((min_cap - cap + 1) & ~1, ((cap >> 1) + 2) & ~1);   // NOTE: grow by approximately 3/2
+    const Size size_max = std::numeric_limits<Size>::max();
+    if ( ((size_max <= std::numeric_limits<int>::max()) && (add > size_max - cap))
+    ||   (((data = (T*)::realloc(data, (cap += add) * sizeof(T))) == NULL) && errno == ENOMEM) )
         throw OutOfMemoryException();
  }
 
 
-template<class T>
-void vec<T>::growTo(int size, const T& pad) {
+template<class T, class _Size>
+void vec<T,_Size>::growTo(Size size, const T& pad) {
     if (sz >= size) return;
     capacity(size);
-    for (int i = sz; i < size; i++) data[i] = pad;
+    for (Size i = sz; i < size; i++) data[i] = pad;
     sz = size; }
 
 
-template<class T>
-void vec<T>::growTo(int size) {
+template<class T, class _Size>
+void vec<T,_Size>::growTo(Size size) {
     if (sz >= size) return;
     capacity(size);
-    for (int i = sz; i < size; i++) new (&data[i]) T();
+    for (Size i = sz; i < size; i++) new (&data[i]) T();
     sz = size; }
 
 
-template<class T>
-void vec<T>::clear(bool dealloc) {
+template<class T, class _Size>
+void vec<T,_Size>::clear(bool dealloc) {
     if (data != NULL){
-        for (int i = 0; i < sz; i++) data[i].~T();
+        for (Size i = 0; i < sz; i++) data[i].~T();
         sz = 0;
         if (dealloc) free(data), data = NULL, cap = 0; } }
 
 //=================================================================================================
 }
 
 #endif
```

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/XAlloc.h` & `lincs-0.6.0/lincs/liblincs/vendored/minisat/mtl/XAlloc.h`

 * *Files 7% similar despite different names*

```diff
@@ -14,34 +14,32 @@
 NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT
 OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 **************************************************************************************************/
 
 
-#ifndef Glucose_XAlloc_h
-#define Glucose_XAlloc_h
+#ifndef Minisat_XAlloc_h
+#define Minisat_XAlloc_h
 
 #include <errno.h>
 #include <stdlib.h>
-#include <stdio.h>
 
-namespace Glucose {
+namespace Minisat {
 
 //=================================================================================================
 // Simple layer on top of malloc/realloc to catch out-of-memory situtaions and provide some typing:
 
 class OutOfMemoryException{};
 static inline void* xrealloc(void *ptr, size_t size)
 {
     void* mem = realloc(ptr, size);
     if (mem == NULL && errno == ENOMEM){
         throw OutOfMemoryException();
-    }else {
+    }else
         return mem;
-	}
 }
 
 //=================================================================================================
 }
 
 #endif
```

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SolverConfiguration.h` & `lincs-0.6.0/lincs/liblincs/vendored/minisat/utils/System.h`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,8 @@
-/***************************************************************************************[SolverConfiguration.h]
- Glucose -- Copyright (c) 2009-2014, Gilles Audemard, Laurent Simon
-                                CRIL - Univ. Artois, France
-                                LRI  - Univ. Paris Sud, France (2009-2013)
-                                Labri - Univ. Bordeaux, France
-
- Syrup (Glucose Parallel) -- Copyright (c) 2013-2014, Gilles Audemard, Laurent Simon
-                                CRIL - Univ. Artois, France
-                                Labri - Univ. Bordeaux, France
-
-Glucose sources are based on MiniSat (see below MiniSat copyrights). Permissions and copyrights of
-Glucose (sources until 2013, Glucose 3.0, single core) are exactly the same as Minisat on which it 
-is based on. (see below).
-
-Glucose-Syrup sources are based on another copyright. Permissions and copyrights for the parallel
-version of Glucose-Syrup (the "Software") are granted, free of charge, to deal with the Software
-without restriction, including the rights to use, copy, modify, merge, publish, distribute,
-sublicence, and/or sell copies of the Software, and to permit persons to whom the Software is 
-furnished to do so, subject to the following conditions:
-
-- The above and below copyrights notices and this permission notice shall be included in all
-copies or substantial portions of the Software;
-- The parallel version of Glucose (all files modified since Glucose 3.0 releases, 2013) cannot
-be used in any competitive event (sat competitions/evaluations) without the express permission of 
-the authors (Gilles Audemard / Laurent Simon). This is also the case for any competitive event
-using Glucose Parallel as an embedded SAT engine (single core or not).
-
-
---------------- Original Minisat Copyrights
-
+/****************************************************************************************[System.h]
 Copyright (c) 2003-2006, Niklas Een, Niklas Sorensson
 Copyright (c) 2007-2010, Niklas Sorensson
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software without restriction,
 including without limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is
@@ -41,33 +12,61 @@
 substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT
 NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT
 OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
- **************************************************************************************************/
+**************************************************************************************************/
+
+#ifndef Minisat_System_h
+#define Minisat_System_h
+
+#if defined(__linux__)
+#include <fpu_control.h>
+#endif
 
+#include "../mtl/IntTypes.h"
 
-#ifndef SolverConfiguration_h
-#define SolverConfiguration_h
+//-------------------------------------------------------------------------------------------------
 
+namespace Minisat {
 
+static inline double cpuTime(void); // CPU-time in seconds.
 
-namespace Glucose {
+extern double memUsed();            // Memory in mega bytes (returns 0 for unsupported architectures).
+extern double memUsedPeak(bool strictlyPeak = false); // Peak-memory in mega bytes (returns 0 for unsupported architectures).
 
-class MultiSolvers;
+extern void   setX86FPUPrecision(); // Make sure double's are represented with the same precision
+                                    // in memory and registers.
 
-class SolverConfiguration {
+extern void   limitMemory(uint64_t max_mem_mb); // Set a limit on total memory usage. The exact
+                                                // semantics varies depending on architecture.
 
-public : 
-    static void configure(MultiSolvers *ms, int nbsolvers);
+extern void   limitTime(uint32_t max_cpu_time); // Set a limit on maximum CPU time. The exact
+                                                // semantics varies depending on architecture.
 
-    // Special configurations
-    static void configureSAT14(MultiSolvers *ms, int nbsolvers);
-    void configureSAT15Adapt(MultiSolvers *ms, int nbsolvers);
-    void configureSAT15Default(MultiSolvers *ms, int nbsolvers);
-    
-};
+extern void   sigTerm(void handler(int));      // Set up handling of available termination signals.
 
 }
+
+//-------------------------------------------------------------------------------------------------
+// Implementation of inline functions:
+
+#if defined(_MSC_VER) || defined(__MINGW32__)
+#include <time.h>
+
+static inline double Minisat::cpuTime(void) { return (double)clock() / CLOCKS_PER_SEC; }
+
+#else
+#include <sys/time.h>
+#include <sys/resource.h>
+#include <unistd.h>
+
+static inline double Minisat::cpuTime(void) {
+    struct rusage ru;
+    getrusage(RUSAGE_SELF, &ru);
+    return (double)ru.ru_utime.tv_sec + (double)ru.ru_utime.tv_usec / 1000000; }
+
+#endif
+
 #endif
```

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/simp/SimpSolver.cc` & `lincs-0.6.0/lincs/liblincs/vendored/minisat/simp/SimpSolver.cc`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,9 @@
-/***************************************************************************************[SimpSolver.cc]
- Glucose -- Copyright (c) 2009-2014, Gilles Audemard, Laurent Simon
-                                CRIL - Univ. Artois, France
-                                LRI  - Univ. Paris Sud, France (2009-2013)
-                                Labri - Univ. Bordeaux, France
-
- Syrup (Glucose Parallel) -- Copyright (c) 2013-2014, Gilles Audemard, Laurent Simon
-                                CRIL - Univ. Artois, France
-                                Labri - Univ. Bordeaux, France
-
-Glucose sources are based on MiniSat (see below MiniSat copyrights). Permissions and copyrights of
-Glucose (sources until 2013, Glucose 3.0, single core) are exactly the same as Minisat on which it
-is based on. (see below).
-
-Glucose-Syrup sources are based on another copyright. Permissions and copyrights for the parallel
-version of Glucose-Syrup (the "Software") are granted, free of charge, to deal with the Software
-without restriction, including the rights to use, copy, modify, merge, publish, distribute,
-sublicence, and/or sell copies of the Software, and to permit persons to whom the Software is 
-furnished to do so, subject to the following conditions:
-
-- The above and below copyrights notices and this permission notice shall be included in all
-copies or substantial portions of the Software;
-- The parallel version of Glucose (all files modified since Glucose 3.0 releases, 2013) cannot
-be used in any competitive event (sat competitions/evaluations) without the express permission of 
-the authors (Gilles Audemard / Laurent Simon). This is also the case for any competitive event
-using Glucose Parallel as an embedded SAT engine (single core or not).
-
-
---------------- Original Minisat Copyrights
-
-Copyright (c) 2003-2006, Niklas Een, Niklas Sorensson
+/***********************************************************************************[SimpSolver.cc]
+Copyright (c) 2006,      Niklas Een, Niklas Sorensson
 Copyright (c) 2007-2010, Niklas Sorensson
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software without restriction,
 including without limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -41,21 +12,21 @@
 substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT
 NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT
 OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
- **************************************************************************************************/
+**************************************************************************************************/
 
 #include "../mtl/Sort.h"
 #include "SimpSolver.h"
 #include "../utils/System.h"
 
-using namespace Glucose;
+using namespace Minisat;
 
 //=================================================================================================
 // Options:
 
 
 static const char* _cat = "SIMP";
 
@@ -69,27 +40,27 @@
 
 
 //=================================================================================================
 // Constructor/Destructor:
 
 
 SimpSolver::SimpSolver() :
-   Solver()
-  , grow               (opt_grow)
+    grow               (opt_grow)
   , clause_lim         (opt_clause_lim)
   , subsumption_lim    (opt_subsumption_lim)
   , simp_garbage_frac  (opt_simp_garbage_frac)
   , use_asymm          (opt_use_asymm)
   , use_rcheck         (opt_use_rcheck)
   , use_elim           (opt_use_elim)
+  , extend_model       (true)
   , merges             (0)
   , asymm_lits         (0)
   , eliminated_vars    (0)
-  , use_simplification (true)
   , elimorder          (1)
+  , use_simplification (true)
   , occurs             (ClauseDeleted(ca))
   , elim_heap          (ElimLt(n_occ))
   , bwdsub_assigns     (0)
   , n_touched          (0)
 {
     vec<Lit> dummy(1,lit_Undef);
     ca.extra_clause_field = true; // NOTE: must happen before allocating the dummy clause below.
@@ -99,78 +70,48 @@
 
 
 SimpSolver::~SimpSolver()
 {
 }
 
 
+Var SimpSolver::newVar(lbool upol, bool dvar) {
+    Var v = Solver::newVar(upol, dvar);
 
-SimpSolver::SimpSolver(const SimpSolver &s) : Solver(s)
-  , grow               (s.grow)
-  , clause_lim         (s.clause_lim)
-  , subsumption_lim    (s.subsumption_lim)
-  , simp_garbage_frac  (s.simp_garbage_frac)
-  , use_asymm          (s.use_asymm)
-  , use_rcheck         (s.use_rcheck)
-  , use_elim           (s.use_elim)
-  , merges             (s.merges)
-  , asymm_lits         (s.asymm_lits)
-  , eliminated_vars    (s.eliminated_vars)
-  , use_simplification (s.use_simplification)
-  , elimorder          (s.elimorder)
-  , occurs             (ClauseDeleted(ca))
-  , elim_heap          (ElimLt(n_occ))
-  , bwdsub_assigns     (s.bwdsub_assigns)
-  , n_touched          (s.n_touched)
-{
-    // TODO: Copy dummy... what is it???
-    vec<Lit> dummy(1,lit_Undef);
-    ca.extra_clause_field = true; // NOTE: must happen before allocating the dummy clause below.
-    bwdsub_tmpunit        = ca.alloc(dummy);
-    remove_satisfied      = false;
-    //End TODO  
-    
-
-    s.elimclauses.memCopyTo(elimclauses);
-    s.touched.memCopyTo(touched);
-    s.occurs.copyTo(occurs);
-    s.n_occ.memCopyTo(n_occ);
-    s.elim_heap.copyTo(elim_heap);
-    s.subsumption_queue.copyTo(subsumption_queue);
-    s.frozen.memCopyTo(frozen);
-    s.eliminated.memCopyTo(eliminated);
-
-    use_simplification = s.use_simplification;
-    bwdsub_assigns = s.bwdsub_assigns;
-    n_touched = s.n_touched;
-    bwdsub_tmpunit = s.bwdsub_tmpunit;
-    qhead = s.qhead;
-    ok = s.ok;
-}
-
-
-
-Var SimpSolver::newVar(bool sign, bool dvar) {
-    Var v = Solver::newVar(sign, dvar);
-    frozen    .push((char)false);
-    eliminated.push((char)false);
+    frozen    .insert(v, (char)false);
+    eliminated.insert(v, (char)false);
 
     if (use_simplification){
-        n_occ     .push(0);
-        n_occ     .push(0);
-        occurs    .init(v);
-        touched   .push(0);
+        n_occ     .insert( mkLit(v), 0);
+        n_occ     .insert(~mkLit(v), 0);
+        occurs    .init  (v);
+        touched   .insert(v, 0);
         elim_heap .insert(v);
     }
     return v; }
 
+
+void SimpSolver::releaseVar(Lit l)
+{
+    assert(!isEliminated(var(l)));
+    if (!use_simplification && var(l) >= max_simp_var)
+        // Note: Guarantees that no references to this variable is
+        // left in model extension datastructure. Could be improved!
+        Solver::releaseVar(l);
+    else
+        // Otherwise, don't allow variable to be reused.
+        Solver::addClause(l);
+}
+
+
 lbool SimpSolver::solve_(bool do_simp, bool turn_off_simp)
 {
     vec<Var> extra_frozen;
     lbool    result = l_True;
+
     do_simp &= use_simplification;
 
     if (do_simp){
         // Assumptions must be temporarily frozen to run variable elimination:
         for (int i = 0; i < assumptions.size(); i++){
             Var v = var(assumptions[i]);
 
@@ -187,122 +128,101 @@
     }
 
     if (result == l_True)
         result = Solver::solve_();
     else if (verbosity >= 1)
         printf("===============================================================================\n");
 
-    if (result == l_True)
+    if (result == l_True && extend_model)
         extendModel();
 
     if (do_simp)
         // Unfreeze the assumptions that were frozen:
         for (int i = 0; i < extra_frozen.size(); i++)
             setFrozen(extra_frozen[i], false);
 
-
     return result;
 }
 
 
 
 bool SimpSolver::addClause_(vec<Lit>& ps)
 {
 #ifndef NDEBUG
     for (int i = 0; i < ps.size(); i++)
         assert(!isEliminated(var(ps[i])));
 #endif
+
     int nclauses = clauses.size();
 
     if (use_rcheck && implied(ps))
         return true;
 
     if (!Solver::addClause_(ps))
         return false;
 
-    if(!parsing && certifiedUNSAT)
-        addToDrat(ps, true);
-
     if (use_simplification && clauses.size() == nclauses + 1){
         CRef          cr = clauses.last();
         const Clause& c  = ca[cr];
 
         // NOTE: the clause is added to the queue immediately and then
         // again during 'gatherTouchedClauses()'. If nothing happens
         // in between, it will only be checked once. Otherwise, it may
         // be checked twice unnecessarily. This is an unfortunate
         // consequence of how backward subsumption is used to mimic
         // forward subsumption.
         subsumption_queue.insert(cr);
         for (int i = 0; i < c.size(); i++){
             occurs[var(c[i])].push(cr);
-            n_occ[toInt(c[i])]++;
+            n_occ[c[i]]++;
             touched[var(c[i])] = 1;
             n_touched++;
             if (elim_heap.inHeap(var(c[i])))
                 elim_heap.increase(var(c[i]));
         }
     }
 
     return true;
 }
 
 
-
-void SimpSolver::removeClause(CRef cr,bool inPurgatory)
+void SimpSolver::removeClause(CRef cr)
 {
     const Clause& c = ca[cr];
 
     if (use_simplification)
         for (int i = 0; i < c.size(); i++){
-            n_occ[toInt(c[i])]--;
+            n_occ[c[i]]--;
             updateElimHeap(var(c[i]));
             occurs.smudge(var(c[i]));
         }
 
-    Solver::removeClause(cr,inPurgatory);
+    Solver::removeClause(cr);
 }
 
 
 bool SimpSolver::strengthenClause(CRef cr, Lit l)
 {
     Clause& c = ca[cr];
     assert(decisionLevel() == 0);
     assert(use_simplification);
 
     // FIX: this is too inefficient but would be nice to have (properly implemented)
     // if (!find(subsumption_queue, &c))
     subsumption_queue.insert(cr);
 
-    if (certifiedUNSAT) {
-        if (vbyte) {
-            write_char('a');
-            for (int i = 0; i < c.size(); i++)
-                if (c[i] != l) write_lit(2*(var(c[i])+1) + sign(c[i]));
-            write_lit(0);
-        }
-        else {
-            for (int i = 0; i < c.size(); i++)
-                if (c[i] != l) fprintf(certifiedOutput, "%i " , (var(c[i]) + 1) * (-2 * sign(c[i]) + 1) );
-            fprintf(certifiedOutput, "0\n");
-        }
-    }
-
     if (c.size() == 2){
         removeClause(cr);
         c.strengthen(l);
     }else{
-        if (certifiedUNSAT)
-            addToDrat(c, false);
-
         detachClause(cr, true);
         c.strengthen(l);
         attachClause(cr);
         remove(occurs[var(l)], cr);
-        n_occ[toInt(l)]--;
+        n_occ[l]--;
         updateElimHeap(var(l));
     }
 
     return c.size() == 1 ? enqueue(c[0]) && propagate() == CRef_Undef : true;
 }
 
 
@@ -315,19 +235,20 @@
     bool  ps_smallest = _ps.size() < _qs.size();
     const Clause& ps  =  ps_smallest ? _qs : _ps;
     const Clause& qs  =  ps_smallest ? _ps : _qs;
 
     for (int i = 0; i < qs.size(); i++){
         if (var(qs[i]) != v){
             for (int j = 0; j < ps.size(); j++)
-                if (var(ps[j]) == var(qs[i]))
+                if (var(ps[j]) == var(qs[i])){
                     if (ps[j] == ~qs[i])
                         return false;
                     else
                         goto next;
+                }
             out_clause.push(qs[i]);
         }
         next:;
     }
 
     for (int i = 0; i < ps.size(); i++)
         if (var(ps[i]) != v)
@@ -349,19 +270,20 @@
     const Lit*  __qs  = (const Lit*)qs;
 
     size = ps.size()-1;
 
     for (int i = 0; i < qs.size(); i++){
         if (var(__qs[i]) != v){
             for (int j = 0; j < ps.size(); j++)
-                if (var(__ps[j]) == var(__qs[i]))
+                if (var(__ps[j]) == var(__qs[i])){
                     if (__ps[j] == ~__qs[i])
                         return false;
                     else
                         goto next;
+                }
             size++;
         }
         next:;
     }
 
     return true;
 }
@@ -372,15 +294,15 @@
     if (n_touched == 0) return;
 
     int i,j;
     for (i = j = 0; i < subsumption_queue.size(); i++)
         if (ca[subsumption_queue[i]].mark() == 0)
             ca[subsumption_queue[i]].mark(2);
 
-    for (i = 0; i < touched.size(); i++)
+    for (i = 0; i < nVars(); i++)
         if (touched[i]){
             const vec<CRef>& cs = occurs.lookup(i);
             for (j = 0; j < cs.size(); j++)
                 if (ca[cs[j]].mark() == 0){
                     subsumption_queue.insert(cs[j]);
                     ca[cs[j]].mark(2);
                 }
@@ -399,15 +321,15 @@
 {
     assert(decisionLevel() == 0);
 
     trail_lim.push(trail.size());
     for (int i = 0; i < c.size(); i++)
         if (value(c[i]) == l_True){
             cancelUntil(0);
-            return false;
+            return true;
         }else if (value(c[i]) != l_False){
             assert(value(c[i]) == l_Undef);
             uncheckedEnqueue(~c[i]);
         }
 
     bool result = propagate() != CRef_Undef;
     cancelUntil(0);
@@ -581,43 +503,42 @@
 
     for (int i = 0; i < pos.size(); i++)
         for (int j = 0; j < neg.size(); j++)
             if (merge(ca[pos[i]], ca[neg[j]], v, clause_size) && 
                 (++cnt > cls.size() + grow || (clause_lim != -1 && clause_size > clause_lim)))
                 return true;
 
-    // Delete and store old clauses
+    // Delete and store old clauses:
     eliminated[v] = true;
     setDecisionVar(v, false);
     eliminated_vars++;
 
     if (pos.size() > neg.size()){
         for (int i = 0; i < neg.size(); i++)
             mkElimClause(elimclauses, v, ca[neg[i]]);
         mkElimClause(elimclauses, mkLit(v));
     }else{
         for (int i = 0; i < pos.size(); i++)
             mkElimClause(elimclauses, v, ca[pos[i]]);
         mkElimClause(elimclauses, ~mkLit(v));
     }
 
+    for (int i = 0; i < cls.size(); i++)
+        removeClause(cls[i]); 
 
     // Produce clauses in cross product:
     vec<Lit>& resolvent = add_tmp;
     for (int i = 0; i < pos.size(); i++)
         for (int j = 0; j < neg.size(); j++)
             if (merge(ca[pos[i]], ca[neg[j]], v, resolvent) && !addClause_(resolvent))
                 return false;
 
-    for (int i = 0; i < cls.size(); i++)
-        removeClause(cls[i]);
-
     // Free occurs list for this variable:
     occurs[v].clear(true);
-
+    
     // Free watchers lists for this variable, if possible:
     if (watches[ mkLit(v)].size() == 0) watches[ mkLit(v)].clear(true);
     if (watches[~mkLit(v)].size() == 0) watches[~mkLit(v)].clear(true);
 
     return backwardSubsumptionCheck();
 }
 
@@ -640,64 +561,51 @@
 
         subst_clause.clear();
         for (int j = 0; j < c.size(); j++){
             Lit p = c[j];
             subst_clause.push(var(p) == v ? x ^ sign(p) : p);
         }
 
- 
+        removeClause(cls[i]);
+
         if (!addClause_(subst_clause))
             return ok = false;
-
-       removeClause(cls[i]);
- 
-   }
+    }
 
     return true;
 }
 
 
 void SimpSolver::extendModel()
 {
     int i, j;
     Lit x;
 
-    if(model.size()==0) model.growTo(nVars());
-
     for (i = elimclauses.size()-1; i > 0; i -= j){
         for (j = elimclauses[i--]; j > 1; j--, i--)
             if (modelValue(toLit(elimclauses[i])) != l_False)
                 goto next;
 
         x = toLit(elimclauses[i]);
         model[var(x)] = lbool(!sign(x));
     next:;
     }
 }
 
 
 bool SimpSolver::eliminate(bool turn_off_elim)
 {
-    if (!simplify()) {
-        ok = false;
+    if (!simplify())
         return false;
-    }
     else if (!use_simplification)
         return true;
 
     // Main simplification loop:
     //
-
-    int toPerform = clauses.size()<=4800000;
-    
-    if(!toPerform) {
-      printf("c Too many clauses... No preprocessing\n");
-    }
-
-    while (toPerform && (n_touched > 0 || bwdsub_assigns < trail.size() || elim_heap.size() > 0)){
+    while (n_touched > 0 || bwdsub_assigns < trail.size() || elim_heap.size() > 0){
 
         gatherTouchedClauses();
         // printf("  ## (time = %6.2f s) BWD-SUB: queue = %d, trail = %d\n", cpuTime(), subsumption_queue.size(), trail.size() - bwdsub_assigns);
         if ((subsumption_queue.size() > 0 || bwdsub_assigns < trail.size()) && 
             !backwardSubsumptionCheck(true)){
             ok = false; goto cleanup; }
 
@@ -747,80 +655,70 @@
         n_occ    .clear(true);
         elim_heap.clear(true);
         subsumption_queue.clear(true);
 
         use_simplification    = false;
         remove_satisfied      = true;
         ca.extra_clause_field = false;
+        max_simp_var          = nVars();
 
         // Force full cleanup (this is safe and desirable since it only happens once):
         rebuildOrderHeap();
         garbageCollect();
     }else{
         // Cheaper cleanup:
-        cleanUpClauses(); // TODO: can we make 'cleanUpClauses()' not be linear in the problem size somehow?
         checkGarbage();
     }
 
-    if (verbosity >= 0 && elimclauses.size() > 0)
-        printf("c |  Eliminated clauses:     %10.2f Mb                                                                |\n", 
+    if (verbosity >= 1 && elimclauses.size() > 0)
+        printf("|  Eliminated clauses:     %10.2f Mb                                      |\n", 
                double(elimclauses.size() * sizeof(uint32_t)) / (1024*1024));
 
-               
     return ok;
-
-    
-}
-
-
-void SimpSolver::cleanUpClauses()
-{
-    occurs.cleanAll();
-    int i,j;
-    for (i = j = 0; i < clauses.size(); i++)
-        if (ca[clauses[i]].mark() == 0)
-            clauses[j++] = clauses[i];
-    clauses.shrink(i - j);
 }
 
 
 //=================================================================================================
 // Garbage Collection methods:
 
 
 void SimpSolver::relocAll(ClauseAllocator& to)
 {
     if (!use_simplification) return;
 
     // All occurs lists:
     //
     for (int i = 0; i < nVars(); i++){
+        occurs.clean(i);
         vec<CRef>& cs = occurs[i];
         for (int j = 0; j < cs.size(); j++)
             ca.reloc(cs[j], to);
     }
 
     // Subsumption queue:
     //
-    for (int i = 0; i < subsumption_queue.size(); i++)
-        ca.reloc(subsumption_queue[i], to);
-
+    for (int i = subsumption_queue.size(); i > 0; i--){
+        CRef cr = subsumption_queue.peek(); subsumption_queue.pop();
+        if (ca[cr].mark()) continue;
+        ca.reloc(cr, to);
+        subsumption_queue.insert(cr);
+    }
+        
     // Temporary clause:
     //
     ca.reloc(bwdsub_tmpunit, to);
 }
 
 
 void SimpSolver::garbageCollect()
 {
     // Initialize the next region to a size corresponding to the estimated utilization degree. This
     // is not precise but should avoid some unnecessary reallocations for the new region:
     ClauseAllocator to(ca.size() - ca.wasted()); 
 
-    cleanUpClauses();
     to.extra_clause_field = ca.extra_clause_field; // NOTE: this is important to keep (or lose) the extra fields.
     relocAll(to);
     Solver::relocAll(to);
     if (verbosity >= 2)
         printf("|  Garbage collection:   %12d bytes => %12d bytes             |\n", 
                ca.size()*ClauseAllocator::Unit_Size, to.size()*ClauseAllocator::Unit_Size);
     to.moveTo(ca);
```

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/simp/SimpSolver.h` & `lincs-0.6.0/lincs/liblincs/vendored/minisat/simp/SimpSolver.h`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,9 @@
-/***************************************************************************************[SimpSolver.h]
- Glucose -- Copyright (c) 2009-2014, Gilles Audemard, Laurent Simon
-                                CRIL - Univ. Artois, France
-                                LRI  - Univ. Paris Sud, France (2009-2013)
-                                Labri - Univ. Bordeaux, France
-
- Syrup (Glucose Parallel) -- Copyright (c) 2013-2014, Gilles Audemard, Laurent Simon
-                                CRIL - Univ. Artois, France
-                                Labri - Univ. Bordeaux, France
-
-Glucose sources are based on MiniSat (see below MiniSat copyrights). Permissions and copyrights of
-Glucose (sources until 2013, Glucose 3.0, single core) are exactly the same as Minisat on which it 
-is based on. (see below).
-
-Glucose-Syrup sources are based on another copyright. Permissions and copyrights for the parallel
-version of Glucose-Syrup (the "Software") are granted, free of charge, to deal with the Software
-without restriction, including the rights to use, copy, modify, merge, publish, distribute,
-sublicence, and/or sell copies of the Software, and to permit persons to whom the Software is 
-furnished to do so, subject to the following conditions:
-
-- The above and below copyrights notices and this permission notice shall be included in all
-copies or substantial portions of the Software;
-- The parallel version of Glucose (all files modified since Glucose 3.0 releases, 2013) cannot
-be used in any competitive event (sat competitions/evaluations) without the express permission of 
-the authors (Gilles Audemard / Laurent Simon). This is also the case for any competitive event
-using Glucose Parallel as an embedded SAT engine (single core or not).
-
-
---------------- Original Minisat Copyrights
-
-Copyright (c) 2003-2006, Niklas Een, Niklas Sorensson
+/************************************************************************************[SimpSolver.h]
+Copyright (c) 2006,      Niklas Een, Niklas Sorensson
 Copyright (c) 2007-2010, Niklas Sorensson
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software without restriction,
 including without limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -41,62 +12,58 @@
 substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT
 NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT
 OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
- **************************************************************************************************/
+**************************************************************************************************/
 
-#ifndef Glucose_SimpSolver_h
-#define Glucose_SimpSolver_h
+#ifndef Minisat_SimpSolver_h
+#define Minisat_SimpSolver_h
 
 #include "../mtl/Queue.h"
 #include "../core/Solver.h"
-#include "../mtl/Clone.h"
 
-namespace Glucose {
+
+namespace Minisat {
 
 //=================================================================================================
 
 
 class SimpSolver : public Solver {
  public:
     // Constructor/Destructor:
     //
     SimpSolver();
     ~SimpSolver();
-    
-    SimpSolver(const  SimpSolver &s);
-    
-
-    /**
-     * Clone function
-    */
-    virtual Clone* clone() const {
-        return  new SimpSolver(*this);
-    }   
 
-    
     // Problem specification:
     //
-    virtual Var     newVar    (bool polarity = true, bool dvar = true); // Add a new variable with parameters specifying variable mode.
+    Var     newVar    (lbool upol = l_Undef, bool dvar = true);
+    void    releaseVar(Lit l);
     bool    addClause (const vec<Lit>& ps);
     bool    addEmptyClause();                // Add the empty clause to the solver.
     bool    addClause (Lit p);               // Add a unit clause to the solver.
     bool    addClause (Lit p, Lit q);        // Add a binary clause to the solver.
     bool    addClause (Lit p, Lit q, Lit r); // Add a ternary clause to the solver.
-    virtual bool    addClause_(      vec<Lit>& ps);
+    bool    addClause (Lit p, Lit q, Lit r, Lit s); // Add a quaternary clause to the solver. 
+    bool    addClause_(      vec<Lit>& ps);
     bool    substitute(Var v, Lit x);  // Replace all occurences of v with x (may cause a contradiction).
 
     // Variable mode:
     // 
     void    setFrozen (Var v, bool b); // If a variable is frozen it will not be eliminated.
     bool    isEliminated(Var v) const;
 
+    // Alternative freeze interface (may replace 'setFrozen()'):
+    void    freezeVar (Var v);         // Freeze one variable so it will not be eliminated.
+    void    thaw      ();              // Thaw all frozen variables.
+
+
     // Solving:
     //
     bool    solve       (const vec<Lit>& assumps, bool do_simp = true, bool turn_off_simp = false);
     lbool   solveLimited(const vec<Lit>& assumps, bool do_simp = true, bool turn_off_simp = false);
     bool    solve       (                     bool do_simp = true, bool turn_off_simp = false);
     bool    solve       (Lit p       ,        bool do_simp = true, bool turn_off_simp = false);       
     bool    solve       (Lit p, Lit q,        bool do_simp = true, bool turn_off_simp = false);
@@ -116,42 +83,42 @@
     void    toDimacs  (const char* file, Lit p);
     void    toDimacs  (const char* file, Lit p, Lit q);
     void    toDimacs  (const char* file, Lit p, Lit q, Lit r);
 #endif
 
     // Mode of operation:
     //
-    int     parsing;
     int     grow;              // Allow a variable elimination step to grow by a number of clauses (default to zero).
     int     clause_lim;        // Variables are not eliminated if it produces a resolvent with a length above this limit.
                                // -1 means no limit.
     int     subsumption_lim;   // Do not check if subsumption against a clause larger than this. -1 means no limit.
     double  simp_garbage_frac; // A different limit for when to issue a GC during simplification (Also see 'garbage_frac').
 
     bool    use_asymm;         // Shrink clauses by asymmetric branching.
     bool    use_rcheck;        // Check if a clause is already implied. Prett costly, and subsumes subsumptions :)
     bool    use_elim;          // Perform variable elimination.
+    bool    extend_model;      // Flag to indicate whether the user needs to look at the full model.
+
     // Statistics:
     //
     int     merges;
     int     asymm_lits;
     int     eliminated_vars;
-    bool                use_simplification;
 
  protected:
 
     // Helper structures:
     //
     struct ElimLt {
-        const vec<int>& n_occ;
-        explicit ElimLt(const vec<int>& no) : n_occ(no) {}
+        const LMap<int>& n_occ;
+        explicit ElimLt(const LMap<int>& no) : n_occ(no) {}
 
         // TODO: are 64-bit operations here noticably bad on 32-bit platforms? Could use a saturating
         // 32-bit implementation instead then, but this will have to do for now.
-        uint64_t cost  (Var x)        const { return (uint64_t)n_occ[toInt(mkLit(x))] * (uint64_t)n_occ[toInt(~mkLit(x))]; }
+        uint64_t cost  (Var x)        const { return (uint64_t)n_occ[mkLit(x)] * (uint64_t)n_occ[~mkLit(x)]; }
         bool operator()(Var x, Var y) const { return cost(x) < cost(y); }
         
         // TODO: investigate this order alternative more.
         // bool operator()(Var x, Var y) const { 
         //     int c_x = cost(x);
         //     int c_y = cost(y);
         //     return c_x < c_y || c_x == c_y && x < y; }
@@ -161,48 +128,50 @@
         const ClauseAllocator& ca;
         explicit ClauseDeleted(const ClauseAllocator& _ca) : ca(_ca) {}
         bool operator()(const CRef& cr) const { return ca[cr].mark() == 1; } };
 
     // Solver state:
     //
     int                 elimorder;
+    bool                use_simplification;
+    Var                 max_simp_var;        // Max variable at the point simplification was turned off.
     vec<uint32_t>       elimclauses;
-    vec<char>           touched;
+    VMap<char>          touched;
     OccLists<Var, vec<CRef>, ClauseDeleted>
                         occurs;
-    vec<int>            n_occ;
-    Heap<ElimLt>        elim_heap;
+    LMap<int>           n_occ;
+    Heap<Var,ElimLt>    elim_heap;
     Queue<CRef>         subsumption_queue;
-    vec<char>           frozen;
-    vec<char>           eliminated;
+    VMap<char>          frozen;
+    vec<Var>            frozen_vars;
+    VMap<char>          eliminated;
     int                 bwdsub_assigns;
     int                 n_touched;
 
     // Temporaries:
     //
     CRef                bwdsub_tmpunit;
 
     // Main internal methods:
     //
-    virtual lbool         solve_                   (bool do_simp = true, bool turn_off_simp = false);
+    lbool         solve_                   (bool do_simp = true, bool turn_off_simp = false);
     bool          asymm                    (Var v, CRef cr);
     bool          asymmVar                 (Var v);
     void          updateElimHeap           (Var v);
     void          gatherTouchedClauses     ();
     bool          merge                    (const Clause& _ps, const Clause& _qs, Var v, vec<Lit>& out_clause);
     bool          merge                    (const Clause& _ps, const Clause& _qs, Var v, int& size);
     bool          backwardSubsumptionCheck (bool verbose = false);
     bool          eliminateVar             (Var v);
     void          extendModel              ();
 
-    void          removeClause             (CRef cr,bool inPurgatory=false);
+    void          removeClause             (CRef cr);
     bool          strengthenClause         (CRef cr, Lit l);
-    void          cleanUpClauses           ();
     bool          implied                  (const vec<Lit>& c);
-    virtual void          relocAll                 (ClauseAllocator& to);
+    void          relocAll                 (ClauseAllocator& to);
 };
 
 
 //=================================================================================================
 // Implementation of inline methods:
 
 
@@ -215,16 +184,32 @@
 
 
 inline bool SimpSolver::addClause    (const vec<Lit>& ps)    { ps.copyTo(add_tmp); return addClause_(add_tmp); }
 inline bool SimpSolver::addEmptyClause()                     { add_tmp.clear(); return addClause_(add_tmp); }
 inline bool SimpSolver::addClause    (Lit p)                 { add_tmp.clear(); add_tmp.push(p); return addClause_(add_tmp); }
 inline bool SimpSolver::addClause    (Lit p, Lit q)          { add_tmp.clear(); add_tmp.push(p); add_tmp.push(q); return addClause_(add_tmp); }
 inline bool SimpSolver::addClause    (Lit p, Lit q, Lit r)   { add_tmp.clear(); add_tmp.push(p); add_tmp.push(q); add_tmp.push(r); return addClause_(add_tmp); }
+inline bool SimpSolver::addClause    (Lit p, Lit q, Lit r, Lit s){ add_tmp.clear(); add_tmp.push(p); add_tmp.push(q); add_tmp.push(r); add_tmp.push(s); return addClause_(add_tmp); }
 inline void SimpSolver::setFrozen    (Var v, bool b) { frozen[v] = (char)b; if (use_simplification && !b) { updateElimHeap(v); } }
 
+inline void SimpSolver::freezeVar(Var v){
+    if (!frozen[v]){
+        frozen[v] = 1;
+        frozen_vars.push(v); 
+    } }
+
+inline void SimpSolver::thaw(){
+    for (int i = 0; i < frozen_vars.size(); i++){
+        Var v = frozen_vars[i];
+        frozen[v] = 0;
+        if (use_simplification)
+            updateElimHeap(v);
+    }
+    frozen_vars.clear(); }
+
 inline bool SimpSolver::solve        (                     bool do_simp, bool turn_off_simp)  { budgetOff(); assumptions.clear(); return solve_(do_simp, turn_off_simp) == l_True; }
 inline bool SimpSolver::solve        (Lit p       ,        bool do_simp, bool turn_off_simp)  { budgetOff(); assumptions.clear(); assumptions.push(p); return solve_(do_simp, turn_off_simp) == l_True; }
 inline bool SimpSolver::solve        (Lit p, Lit q,        bool do_simp, bool turn_off_simp)  { budgetOff(); assumptions.clear(); assumptions.push(p); assumptions.push(q); return solve_(do_simp, turn_off_simp) == l_True; }
 inline bool SimpSolver::solve        (Lit p, Lit q, Lit r, bool do_simp, bool turn_off_simp)  { budgetOff(); assumptions.clear(); assumptions.push(p); assumptions.push(q); assumptions.push(r); return solve_(do_simp, turn_off_simp) == l_True; }
 inline bool SimpSolver::solve        (const vec<Lit>& assumps, bool do_simp, bool turn_off_simp){ 
     budgetOff(); assumps.copyTo(assumptions); return solve_(do_simp, turn_off_simp) == l_True; }
```

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/utils/Options.cc` & `lincs-0.6.0/lincs/liblincs/vendored/minisat/utils/Options.cc`

 * *Files 6% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 **************************************************************************************************/
 
 #include "../mtl/Sort.h"
 #include "Options.h"
 #include "ParseUtils.h"
 
-using namespace Glucose;
+using namespace Minisat;
 
-void Glucose::parseOptions(int& argc, char** argv, bool strict)
+void Minisat::parseOptions(int& argc, char** argv, bool strict)
 {
     int i, j;
     for (i = j = 1; i < argc; i++){
         const char* str = argv[i];
         if (match(str, "--") && match(str, Option::getHelpPrefixString()) && match(str, "help")){
             if (*str == '\0')
                 printUsageAndExit(argc, argv);
@@ -38,35 +38,36 @@
         
             for (int k = 0; !parsed_ok && k < Option::getOptionList().size(); k++){
                 parsed_ok = Option::getOptionList()[k]->parse(argv[i]);
 
                 // fprintf(stderr, "checking %d: %s against flag <%s> (%s)\n", i, argv[i], Option::getOptionList()[k]->name, parsed_ok ? "ok" : "skip");
             }
 
-            if (!parsed_ok)
+            if (!parsed_ok){
                 if (strict && match(argv[i], "-"))
                     fprintf(stderr, "ERROR! Unknown flag \"%s\". Use '--%shelp' for help.\n", argv[i], Option::getHelpPrefixString()), exit(1);
                 else
                     argv[j++] = argv[i];
+            }
         }
     }
 
     argc -= (i - j);
 }
 
 
-void Glucose::setUsageHelp      (const char* str){ Option::getUsageString() = str; }
-void Glucose::setHelpPrefixStr  (const char* str){ Option::getHelpPrefixString() = str; }
-void Glucose::printUsageAndExit (int argc, char** argv, bool verbose)
+void Minisat::setUsageHelp      (const char* str){ Option::getUsageString() = str; }
+void Minisat::setHelpPrefixStr  (const char* str){ Option::getHelpPrefixString() = str; }
+void Minisat::printUsageAndExit (int /*argc*/, char** argv, bool verbose)
 {
     const char* usage = Option::getUsageString();
     if (usage != NULL)
         fprintf(stderr, usage, argv[0]);
 
-        sort(Option::getOptionList(), Option::OptionLt());
+    sort(Option::getOptionList(), Option::OptionLt());
 
     const char* prev_cat  = NULL;
     const char* prev_type = NULL;
 
     for (int i = 0; i < Option::getOptionList().size(); i++){
         const char* cat  = Option::getOptionList()[i]->category;
         const char* type = Option::getOptionList()[i]->type_name;
```

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/utils/Options.h` & `lincs-0.6.0/lincs/liblincs/vendored/minisat/utils/Options.h`

 * *Files 1% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT
 NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT
 OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 **************************************************************************************************/
 
-#ifndef Glucose_Options_h
-#define Glucose_Options_h
+#ifndef Minisat_Options_h
+#define Minisat_Options_h
 
 #include <stdlib.h>
 #include <stdio.h>
 #include <math.h>
 #include <string.h>
 
 #include "../mtl/IntTypes.h"
 #include "../mtl/Vec.h"
 #include "ParseUtils.h"
 
-namespace Glucose {
+namespace Minisat {
 
 //==================================================================================================
 // Top-level option parse/help functions:
 
 
 extern void parseOptions     (int& argc, char** argv, bool strict = false);
 extern void printUsageAndExit(int  argc, char** argv, bool verbose = false);
@@ -56,15 +56,15 @@
     static vec<Option*>& getOptionList () { static vec<Option*> options; return options; }
     static const char*&  getUsageString() { static const char* usage_str; return usage_str; }
     static const char*&  getHelpPrefixString() { static const char* help_prefix_str = ""; return help_prefix_str; }
 
     struct OptionLt {
         bool operator()(const Option* x, const Option* y) {
             int test1 = strcmp(x->category, y->category);
-            return test1 < 0 || test1 == 0 && strcmp(x->type_name, y->type_name) < 0;
+            return test1 < 0 || (test1 == 0 && strcmp(x->type_name, y->type_name) < 0);
         }
     };
 
     Option(const char* name_, 
            const char* desc_,
            const char* cate_,
            const char* type_) : 
@@ -286,15 +286,15 @@
 
         fprintf(stderr, " .. ");
         if (range.end == INT64_MAX)
             fprintf(stderr, "imax");
         else
             fprintf(stderr, "%4" PRIi64, range.end);
 
-        fprintf(stderr, "] (default: %" PRIi64")\n", value);
+        fprintf(stderr, "] (default: %" PRIi64 ")\n", value);
         if (verbose){
             fprintf(stderr, "\n        %s\n", description);
             fprintf(stderr, "\n");
         }
     }
 };
 #endif
```

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/utils/ParseUtils.h` & `lincs-0.6.0/lincs/liblincs/vendored/minisat/utils/ParseUtils.h`

 * *Files 22% similar despite different names*

```diff
@@ -14,44 +14,50 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT
 NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT
 OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 **************************************************************************************************/
 
-#ifndef Glucose_ParseUtils_h
-#define Glucose_ParseUtils_h
+#ifndef Minisat_ParseUtils_h
+#define Minisat_ParseUtils_h
 
 #include <stdlib.h>
 #include <stdio.h>
-#include <cmath>
 
 #include <zlib.h>
 
-namespace Glucose {
+#include "../mtl/XAlloc.h"
+
+namespace Minisat {
 
 //-------------------------------------------------------------------------------------------------
 // A simple buffered character stream class:
 
-static const int buffer_size = 1048576;
 
 
 class StreamBuffer {
-    gzFile        in;
-    unsigned char buf[buffer_size];
-    int           pos;
-    int           size;
+    gzFile         in;
+    unsigned char* buf;
+    int            pos;
+    int            size;
+
+    enum { buffer_size = 64*1024 };
 
     void assureLookahead() {
         if (pos >= size) {
             pos  = 0;
-            size = gzread(in, buf, sizeof(buf)); } }
+            size = gzread(in, buf, buffer_size); } }
 
 public:
-    explicit StreamBuffer(gzFile i) : in(i), pos(0), size(0) { assureLookahead(); }
+    explicit StreamBuffer(gzFile i) : in(i), pos(0), size(0){
+        buf = (unsigned char*)xrealloc(NULL, buffer_size);
+        assureLookahead();
+    }
+    ~StreamBuffer() { free(buf); }
 
     int  operator *  () const { return (pos >= size) ? EOF : buf[pos]; }
     void operator ++ ()       { pos++; assureLookahead(); }
     int  position    () const { return pos; }
 };
 
 
@@ -75,67 +81,25 @@
 template<class B>
 static void skipLine(B& in) {
     for (;;){
         if (isEof(in)) return;
         if (*in == '\n') { ++in; return; }
         ++in; } }
 
-template<class B>
-static double parseDouble(B& in) { // only in the form X.XXXXXe-XX
-    bool    neg= false;
-	double accu = 0.0;
-	double currentExponent = 1;
-	int exponent;
-	
-    skipWhitespace(in);
-    if(*in == EOF) return 0;
-    if      (*in == '-') neg = true, ++in;
-    else if (*in == '+') ++in;
-    if (*in < '1' || *in > '9') printf("PARSE ERROR! Unexpected char: %c\n", *in), exit(3);
-	accu = (double)(*in - '0');
-	++in;
-	if (*in != '.') printf("PARSE ERROR! Unexpected char: %c\n", *in),exit(3);
-	++in; // skip dot
-	currentExponent = 0.1;
-    while (*in >= '0' && *in <= '9')
-        accu = accu + currentExponent * ((double)(*in - '0')),
-		currentExponent /= 10,
-        ++in;
-	if (*in != 'e') printf("PARSE ERROR! Unexpected char: %c\n", *in),exit(3);
-	++in; // skip dot
-	exponent = parseInt(in); // read exponent
-        accu *= std::pow(10,exponent);
-	return neg ? -accu:accu;
-}
-
 
 template<class B>
 static int parseInt(B& in) {
     int     val = 0;
     bool    neg = false;
     skipWhitespace(in);
     if      (*in == '-') neg = true, ++in;
     else if (*in == '+') ++in;
     if (*in < '0' || *in > '9') fprintf(stderr, "PARSE ERROR! Unexpected char: %c\n", *in), exit(3);
     while (*in >= '0' && *in <= '9')
         val = val*10 + (*in - '0'),
-        ++in;
-    return neg ? -val : val; }
-
-
-template<class B>
-static int64_t parseInt64(B& in) {
-    int64_t     val = 0;
-    bool    neg = false;
-    skipWhitespace(in);
-    if      (*in == '-') neg = true, ++in;
-    else if (*in == '+') ++in;
-    if (*in < '0' || *in > '9') fprintf(stderr, "PARSE ERROR! Unexpected char: %c\n", *in), exit(3);
-    while (*in >= '0' && *in <= '9')
-        val = val*10 + (*in - '0'),
         ++in;
     return neg ? -val : val; }
 
 
 // String matching: in case of a match the input iterator will be advanced the corresponding
 // number of characters.
 template<class B>
```

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/mcqd.h` & `lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/mcqd.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/virtualcard.h` & `lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/virtualcard.h`

 * *Files 21% similar despite different names*

```diff
@@ -11,35 +11,29 @@
 
 
 protected:
     VirtualSAT *solver;
     unsigned int nbLit;
     unsigned int bound;
 
-    unsigned int newVar();
-    void addClause(const std::vector<int> & clause);
-
-    bool getValue(int lit);
-    void setDecisionVar(unsigned int var, bool value);
-
 public:
 
     VirtualCard(VirtualSAT *solver, const std::vector<int> &clause, unsigned int bound=0)
         : solver(solver), nbLit(static_cast<unsigned int>(clause.size())), bound(bound) {
 
     }
 
+    virtual std::vector<int> getClause() = 0;
+
     virtual ~VirtualCard();
 
     virtual int operator <= (unsigned int k) {
         return atMost(k);
     }
 
-    //virtual std::vector<int> getClause() {assert(!"TODO");}
-
     virtual unsigned int size() const {
         return nbLit;
     }
 
     virtual void print(std::ostream& os) const {
         os << "VirtualCard(size: "<<nbLit<<", bound: " << bound << ")";
     }
```

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/lov-e.hpp` & `lincs-0.6.0/lincs/liblincs/vendored/lov-e.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/magic_enum.hpp` & `lincs-0.6.0/lincs/liblincs/vendored/magic_enum.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/minisat/core/Solver.cc` & `lincs-0.6.0/lincs/liblincs/vendored/minisat/core/Solver.cc`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/minisat/core/SolverTypes.h` & `lincs-0.6.0/lincs/liblincs/vendored/minisat/core/SolverTypes.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/Alg.h` & `lincs-0.6.0/lincs/liblincs/vendored/minisat/mtl/Rnd.h`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-/*******************************************************************************************[Alg.h]
-Copyright (c) 2003-2006, Niklas Een, Niklas Sorensson
-Copyright (c) 2007-2010, Niklas Sorensson
-
+/*******************************************************************************************[Rnd.h]
+Copyright (c) 2012, Niklas Sorensson
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software without restriction,
 including without limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or
@@ -14,71 +12,56 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT
 NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT
 OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 **************************************************************************************************/
 
-#ifndef Minisat_Alg_h
-#define Minisat_Alg_h
+#ifndef Minisat_Rnd_h
+#define Minisat_Rnd_h
 
-#include "Vec.h"
+#include "minisat/mtl/Vec.h"
 
 namespace Minisat {
 
-//=================================================================================================
-// Useful functions on vector-like types:
-
-//=================================================================================================
-// Removing and searching for elements:
-//
-
-template<class V, class T>
-static inline void remove(V& ts, const T& t)
+// Generate a random double:
+static inline double drand(double& seed)
 {
-    int j = 0;
-    for (; j < (int)ts.size() && ts[j] != t; j++);
-    assert(j < (int)ts.size());
-    for (; j < (int)ts.size()-1; j++) ts[j] = ts[j+1];
-    ts.pop();
+    seed *= 1389796;
+    int q = (int)(seed / 2147483647);
+    seed -= (double)q * 2147483647;
+    return seed / 2147483647;
 }
 
 
-template<class V, class T>
-static inline bool find(V& ts, const T& t)
-{
-    int j = 0;
-    for (; j < (int)ts.size() && ts[j] != t; j++);
-    return j < (int)ts.size();
-}
+// Generate a random integer:
+static inline int irand(double& seed, int size) { return (int)(drand(seed) * size); }
 
 
-//=================================================================================================
-// Copying vectors with support for nested vector types:
-//
-
-// Base case:
+// Randomly shuffle the contents of a vector:
 template<class T>
-static inline void copy(const T& from, T& to)
+static void randomShuffle(double& seed, vec<T>& xs)
 {
-    to = from;
+    for (int i = 0; i < xs.size(); i++){
+        int pick = i + irand(seed, xs.size() - i);
+        T tmp = xs[i];
+        xs[i] = xs[pick];
+        xs[pick] = tmp;
+    }
 }
 
-// Recursive case:
+// Randomly shuffle a vector of a vector (ugly)
 template<class T>
-static inline void copy(const vec<T>& from, vec<T>& to, bool append = false)
+static void randomShuffle(double& seed, vec<vec<T> >& xs)
 {
-    if (!append)
-        to.clear();
-    for (int i = 0; i < from.size(); i++){
-        to.push();
-        copy(from[i], to.last());
+    for (int i = 0; i < xs.size(); i++){
+        int pick = i + irand(seed, xs.size() - i);
+        vec<T> tmp; xs[i].moveTo(tmp);
+        xs[pick].moveTo(xs[i]);
+        tmp.moveTo(xs[pick]);
     }
 }
 
-template<class T>
-static inline void append(const vec<T>& from, vec<T>& to){ copy(from, to, true); }
 
 //=================================================================================================
-}
-
+} // namespace Minisat
 #endif
```

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/IntMap.h` & `lincs-0.6.0/lincs/liblincs/vendored/minisat/mtl/IntMap.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/minisat/simp/SimpSolver.cc` & `lincs-0.6.0/lincs/liblincs/vendored/eval-max-sat/cadical/subsume.cpp`

 * *Files 27% similar despite different names*

```diff
@@ -1,725 +1,612 @@
-/***********************************************************************************[SimpSolver.cc]
-Copyright (c) 2006,      Niklas Een, Niklas Sorensson
-Copyright (c) 2007-2010, Niklas Sorensson
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
-associated documentation files (the "Software"), to deal in the Software without restriction,
-including without limitation the rights to use, copy, modify, merge, publish, distribute,
-sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or
-substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT
-NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
-NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
-DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT
-OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-**************************************************************************************************/
-
-#include "../mtl/Sort.h"
-#include "SimpSolver.h"
-#include "../utils/System.h"
-
-using namespace Minisat;
-
-//=================================================================================================
-// Options:
-
-
-static const char* _cat = "SIMP";
-
-static BoolOption   opt_use_asymm        (_cat, "asymm",        "Shrink clauses by asymmetric branching.", false);
-static BoolOption   opt_use_rcheck       (_cat, "rcheck",       "Check if a clause is already implied. (costly)", false);
-static BoolOption   opt_use_elim         (_cat, "elim",         "Perform variable elimination.", true);
-static IntOption    opt_grow             (_cat, "grow",         "Allow a variable elimination step to grow by a number of clauses.", 0);
-static IntOption    opt_clause_lim       (_cat, "cl-lim",       "Variables are not eliminated if it produces a resolvent with a length above this limit. -1 means no limit", 20,   IntRange(-1, INT32_MAX));
-static IntOption    opt_subsumption_lim  (_cat, "sub-lim",      "Do not check if subsumption against a clause larger than this. -1 means no limit.", 1000, IntRange(-1, INT32_MAX));
-static DoubleOption opt_simp_garbage_frac(_cat, "simp-gc-frac", "The fraction of wasted memory allowed before a garbage collection is triggered during simplification.",  0.5, DoubleRange(0, false, HUGE_VAL, false));
-
-
-//=================================================================================================
-// Constructor/Destructor:
-
-
-SimpSolver::SimpSolver() :
-    grow               (opt_grow)
-  , clause_lim         (opt_clause_lim)
-  , subsumption_lim    (opt_subsumption_lim)
-  , simp_garbage_frac  (opt_simp_garbage_frac)
-  , use_asymm          (opt_use_asymm)
-  , use_rcheck         (opt_use_rcheck)
-  , use_elim           (opt_use_elim)
-  , extend_model       (true)
-  , merges             (0)
-  , asymm_lits         (0)
-  , eliminated_vars    (0)
-  , elimorder          (1)
-  , use_simplification (true)
-  , occurs             (ClauseDeleted(ca))
-  , elim_heap          (ElimLt(n_occ))
-  , bwdsub_assigns     (0)
-  , n_touched          (0)
-{
-    vec<Lit> dummy(1,lit_Undef);
-    ca.extra_clause_field = true; // NOTE: must happen before allocating the dummy clause below.
-    bwdsub_tmpunit        = ca.alloc(dummy);
-    remove_satisfied      = false;
-}
-
-
-SimpSolver::~SimpSolver()
-{
-}
-
-
-Var SimpSolver::newVar(lbool upol, bool dvar) {
-    Var v = Solver::newVar(upol, dvar);
-
-    frozen    .insert(v, (char)false);
-    eliminated.insert(v, (char)false);
-
-    if (use_simplification){
-        n_occ     .insert( mkLit(v), 0);
-        n_occ     .insert(~mkLit(v), 0);
-        occurs    .init  (v);
-        touched   .insert(v, 0);
-        elim_heap .insert(v);
-    }
-    return v; }
-
-
-void SimpSolver::releaseVar(Lit l)
-{
-    assert(!isEliminated(var(l)));
-    if (!use_simplification && var(l) >= max_simp_var)
-        // Note: Guarantees that no references to this variable is
-        // left in model extension datastructure. Could be improved!
-        Solver::releaseVar(l);
-    else
-        // Otherwise, don't allow variable to be reused.
-        Solver::addClause(l);
-}
-
-
-lbool SimpSolver::solve_(bool do_simp, bool turn_off_simp)
-{
-    vec<Var> extra_frozen;
-    lbool    result = l_True;
-
-    do_simp &= use_simplification;
+#include "internal.hpp"
 
-    if (do_simp){
-        // Assumptions must be temporarily frozen to run variable elimination:
-        for (int i = 0; i < assumptions.size(); i++){
-            Var v = var(assumptions[i]);
-
-            // If an assumption has been eliminated, remember it.
-            assert(!isEliminated(v));
-
-            if (!frozen[v]){
-                // Freeze and store.
-                setFrozen(v, true);
-                extra_frozen.push(v);
-            } }
+namespace CaDiCaL {
 
-        result = lbool(eliminate(turn_off_simp));
-    }
+/*------------------------------------------------------------------------*/
 
-    if (result == l_True)
-        result = Solver::solve_();
-    else if (verbosity >= 1)
-        printf("===============================================================================\n");
-
-    if (result == l_True && extend_model)
-        extendModel();
-
-    if (do_simp)
-        // Unfreeze the assumptions that were frozen:
-        for (int i = 0; i < extra_frozen.size(); i++)
-            setFrozen(extra_frozen[i], false);
-
-    return result;
-}
+// This file implements a global forward subsumption algorithm, which is run
+// frequently during search.  It works both on original (irredundant)
+// clauses and on 'sticky' learned clauses which are likely to be kept.
+// This is abstracted away in the 'likely_to_be_kept_clause' function, which
+// implicitly relies on 'opts.reducetier1lgue' (glucose level of clauses
+// which are not reduced) as well as dynamically determined size and glucose
+// level ('lim.keptglue' and 'lim.keptsize') of clauses kept in 'reduce'.
+//
+// Note, that 'forward' means that the clause from which the subsumption
+// check is started is checked for being subsumed by other (smaller or equal
+// size) clauses.  Since 'vivification' is an extended version of subsume,
+// more powerful, but also slower, we schedule 'vivify' right after
+// 'subsume', which in contrast to 'subsume' is not run until to completion.
+//
+// This implementation is inspired by Bayardo's SDM'11 analysis of our
+// subsumption algorithm in our SATeLite preprocessor in the context of
+// finding extremal sets in data mining and his suggested improvements.
+
+// Our original subsumption algorithm in 'Quantor' and 'SATeLite' (and in
+// MiniSAT and descendants) is based on backward subsumption.  It uses the
+// observation that only the occurrence list of one literal of a clause has
+// to be traversed in order to find all potential clauses which are subsumed
+// by the candidate.  Thus the literal with the smallest number of
+// occurrences is used.  However, that scheme requires to connect all
+// literals of surviving clauses, while forward algorithms only need to
+// connect one literal. On the other hand forward checking requires to
+// traverse the occurrence lists of all literals of the candidate clause to
+// find subsuming clauses.  During connecting the single literal (similar to
+// the one-watch scheme by Lintao Zhang) one can connect a literal with a
+// minimal number of occurrence so far, which implicitly also reduces future
+// occurrence list traversal time.
+
+// Also the actual subsumption check is cheaper since during backward
+// checking the short subsuming candidate clause is marked and all the
+// literals in the larger subsume candidate clauses have to be traversed,
+// while for our forward approach the long subsumed candidate clause is only
+// marked once, while the literals of the shorter subsuming clauses have to
+// be checked.  We also use a fixed special more cache friendly data
+// structure for binary clauses, to avoid traversing them directly.
+
+// In our forward scheme it is still possible to skip occurrence lists of
+// literals which were not added since the last subsumption round, since
+// only those can contain subsuming candidates.  Actually, clauses which
+// contain at least one literal, which was not added since the last
+// subsumption round do not have to be connected at all, even though they
+// might still be subsumed them self.
+
+// Bayardo suggests to sort the literals in clauses and perform some kind of
+// partial merge-sort, while we mark literals, but do sort literals during
+// connecting a clause w.r.t. the number of occurrences, in order to find
+// literals which do not occur in the subsumed candidate fast with high
+// probability (less occurring literals have a higher chance).
+
+bool Internal::subsuming () {
+
+  if (!opts.subsume && !opts.vivify) return false;
+  if (!preprocessing && !opts.inprocessing) return false;
+  if (preprocessing) assert (lim.preprocessing);
+
+  // Only perform global subsumption checking immediately after a clause
+  // reduction happened where the overall allocated memory is small and we
+  // got a limit on the number of kept clause in terms of size and glue.
+  //
+  if (opts.reduce &&
+      stats.conflicts != last.reduce.conflicts) return false;
+
+  if (stats.conflicts < lim.subsume) return false;
+
+  return true;
+}
+
+// This is the actual subsumption and strengthening check.  We assume that
+// all the literals of the candidate clause to be subsumed or strengthened
+// are marked, so we only have to check that all the literals of the
+// argument clause 'subsuming', which is checked for subsuming the candidate
+// clause 'subsumed', has all its literals marked (in the correct phase).
+// If exactly one is in the opposite phase we can still strengthen the
+// candidate clause by this single literal which occurs in opposite phase.
+//
+// The result is INT_MIN if all literals are marked and thus the candidate
+// clause can be subsumed.  It is zero if neither subsumption nor
+// strengthening is possible.  Otherwise the candidate clause can be
+// strengthened and as a result the negation of the literal which can be
+// removed is returned.
 
-
-
-bool SimpSolver::addClause_(vec<Lit>& ps)
+inline int Internal::subsume_check (Clause * subsuming, Clause * subsumed)
 {
-#ifndef NDEBUG
-    for (int i = 0; i < ps.size(); i++)
-        assert(!isEliminated(var(ps[i])));
+#ifdef NDEBUG
+  (void) subsumed;
 #endif
+  // Only use 'subsumed' for these following assertion checks.  Otherwise we
+  // only require that 'subsumed' has all its literals marked.
+  //
+  assert (!subsumed->garbage);
+  assert (!subsuming->garbage);
+  assert (subsuming != subsumed);
+  assert (subsuming->size <= subsumed->size);
+
+  stats.subchecks++;
+  if (subsuming->size == 2) stats.subchecks2++;
+
+  int flipped = 0, prev = 0;
+  bool failed = false;
+  const auto eoc = subsuming->end ();
+  for (auto i = subsuming->begin (); !failed && i != eoc; i++) {
+    int lit = *i;
+    *i = prev;
+    prev = lit;
+    const int tmp = marked (lit);
+    if (!tmp) failed = true;
+    else if (tmp > 0) continue;
+    else if (flipped) failed = true;
+    else flipped = lit;
+  }
+  assert (prev);
+  assert (!subsuming->literals[0]);
+  subsuming->literals[0] = prev;
+  if (failed) return 0;
+
+  if (!flipped) return INT_MIN;                   // subsumed!!
+  else if (!opts.subsumestr) return 0;
+  else return flipped;                            // strengthen!!
+}
+
+/*------------------------------------------------------------------------*/
+
+// Candidate clause 'subsumed' is subsumed by 'subsuming'.
+
+inline void
+Internal::subsume_clause (Clause * subsuming, Clause * subsumed) {
+  stats.subsumed++;
+  assert (subsuming->size <= subsumed->size);
+  LOG (subsumed, "subsumed");
+  if (subsumed->redundant) stats.subred++; else stats.subirr++;
+  mark_garbage (subsumed);
+  if (subsumed->redundant || !subsuming->redundant) return;
+  LOG ("turning redundant subsuming clause into irredundant clause");
+  subsuming->redundant = false;
+  stats.current.irredundant++;
+  stats.added.irredundant++;
+  stats.irrbytes += subsuming->bytes ();
+  assert (stats.current.redundant > 0);
+  stats.current.redundant--;
+  assert (stats.added.redundant > 0);
+  stats.added.redundant--;
+  // ... and keep 'stats.added.total'.
+}
+
+/*------------------------------------------------------------------------*/
+
+// Candidate clause 'c' is strengthened by removing 'lit'.
+
+void Internal::strengthen_clause (Clause * c, int lit) {
+  stats.strengthened++;
+  assert (c->size > 2);
+  LOG (c, "removing %d in", lit);
+  if (proof) proof->strengthen_clause (c, lit);
+  if (!c->redundant) mark_removed (lit);
+  auto new_end = remove (c->begin (), c->end (), lit);
+  assert (new_end + 1 == c->end ()), (void) new_end;
+  (void) shrink_clause (c, c->size - 1);
+  c->used = true;
+  LOG (c, "strengthened");
+  external->check_shrunken_clause (c);
+}
+
+/*------------------------------------------------------------------------*/
+
+// Find clauses connected in the occurrence lists 'occs' which subsume the
+// candidate clause 'c' given as first argument.  If this is the case the
+// clause is subsumed and the result is positive.   If the clause was
+// strengthened the result is negative.  Otherwise the candidate clause
+// can not be subsumed nor strengthened and zero is returned.
+
+inline int
+Internal::try_to_subsume_clause (Clause * c, vector<Clause *> & shrunken) {
+
+  stats.subtried++;
+  assert (!level);
+  LOG (c, "trying to subsume");
+
+  mark (c);     // signed!
+
+  Clause dummy; // Communicate binary subsuming clause.
+
+  Clause * d = 0;
+  int flipped = 0;
+
+  for (const auto & lit : *c) {
+
+    // Only clauses which have a variable which has recently been added are
+    // checked for being subsumed.  The idea is that all these newly added
+    // clauses are candidates for subsubming the clause.  Then we also only
+    // need to check occurrences of these variables.  The occurrence lists
+    // of other literal do not have to be checked.
+    //
+    if (!flags (lit).subsume) continue;
 
-    int nclauses = clauses.size();
-
-    if (use_rcheck && implied(ps))
-        return true;
-
-    if (!Solver::addClause_(ps))
-        return false;
-
-    if (use_simplification && clauses.size() == nclauses + 1){
-        CRef          cr = clauses.last();
-        const Clause& c  = ca[cr];
-
-        // NOTE: the clause is added to the queue immediately and then
-        // again during 'gatherTouchedClauses()'. If nothing happens
-        // in between, it will only be checked once. Otherwise, it may
-        // be checked twice unnecessarily. This is an unfortunate
-        // consequence of how backward subsumption is used to mimic
-        // forward subsumption.
-        subsumption_queue.insert(cr);
-        for (int i = 0; i < c.size(); i++){
-            occurs[var(c[i])].push(cr);
-            n_occ[c[i]]++;
-            touched[var(c[i])] = 1;
-            n_touched++;
-            if (elim_heap.inHeap(var(c[i])))
-                elim_heap.increase(var(c[i]));
-        }
-    }
-
-    return true;
-}
-
-
-void SimpSolver::removeClause(CRef cr)
-{
-    const Clause& c = ca[cr];
-
-    if (use_simplification)
-        for (int i = 0; i < c.size(); i++){
-            n_occ[c[i]]--;
-            updateElimHeap(var(c[i]));
-            occurs.smudge(var(c[i]));
-        }
-
-    Solver::removeClause(cr);
-}
-
-
-bool SimpSolver::strengthenClause(CRef cr, Lit l)
-{
-    Clause& c = ca[cr];
-    assert(decisionLevel() == 0);
-    assert(use_simplification);
-
-    // FIX: this is too inefficient but would be nice to have (properly implemented)
-    // if (!find(subsumption_queue, &c))
-    subsumption_queue.insert(cr);
-
-    if (c.size() == 2){
-        removeClause(cr);
-        c.strengthen(l);
-    }else{
-        detachClause(cr, true);
-        c.strengthen(l);
-        attachClause(cr);
-        remove(occurs[var(l)], cr);
-        n_occ[l]--;
-        updateElimHeap(var(l));
-    }
-
-    return c.size() == 1 ? enqueue(c[0]) && propagate() == CRef_Undef : true;
-}
-
-
-// Returns FALSE if clause is always satisfied ('out_clause' should not be used).
-bool SimpSolver::merge(const Clause& _ps, const Clause& _qs, Var v, vec<Lit>& out_clause)
-{
-    merges++;
-    out_clause.clear();
-
-    bool  ps_smallest = _ps.size() < _qs.size();
-    const Clause& ps  =  ps_smallest ? _qs : _ps;
-    const Clause& qs  =  ps_smallest ? _ps : _qs;
-
-    for (int i = 0; i < qs.size(); i++){
-        if (var(qs[i]) != v){
-            for (int j = 0; j < ps.size(); j++)
-                if (var(ps[j]) == var(qs[i])){
-                    if (ps[j] == ~qs[i])
-                        return false;
-                    else
-                        goto next;
-                }
-            out_clause.push(qs[i]);
-        }
-        next:;
-    }
-
-    for (int i = 0; i < ps.size(); i++)
-        if (var(ps[i]) != v)
-            out_clause.push(ps[i]);
-
-    return true;
-}
-
-
-// Returns FALSE if clause is always satisfied.
-bool SimpSolver::merge(const Clause& _ps, const Clause& _qs, Var v, int& size)
-{
-    merges++;
+    for (int sign = -1; !d && sign <= 1; sign += 2) {
 
-    bool  ps_smallest = _ps.size() < _qs.size();
-    const Clause& ps  =  ps_smallest ? _qs : _ps;
-    const Clause& qs  =  ps_smallest ? _ps : _qs;
-    const Lit*  __ps  = (const Lit*)ps;
-    const Lit*  __qs  = (const Lit*)qs;
-
-    size = ps.size()-1;
-
-    for (int i = 0; i < qs.size(); i++){
-        if (var(__qs[i]) != v){
-            for (int j = 0; j < ps.size(); j++)
-                if (var(__ps[j]) == var(__qs[i])){
-                    if (__ps[j] == ~__qs[i])
-                        return false;
-                    else
-                        goto next;
-                }
-            size++;
+      // First we check against all binary clauses.  The other literals of
+      // all binary clauses of 'sign*lit' are stored in one consecutive
+      // array, which is way faster than storing clause pointers and
+      // dereferencing them.  Since this binary clause array is also not
+      // shrunken, we also can bail out earlier if subsumption or
+      // strengthening is determined.  In both cases the (self-)subsuming
+      // clause is stored in 'd', which makes it nonzero and forces
+      // aborting both the outer and inner loop.  If the binary clause can
+      // strengthen the candidate clause 'c' (through self-subsuming
+      // resolution), then 'filled' is set to the literal which can be
+      // removed in 'c', otherwise to 'INT_MIN' which is a non-valid
+      // literal.
+      //
+      for (const auto & other : bins (sign*lit) ) {
+        const int tmp = marked (other);
+        if (!tmp) continue;
+        if (tmp < 0 && sign < 0) continue;
+        if (tmp < 0) {
+          if (sign < 0) continue;               // tautological resolvent
+          dummy.literals[0] = lit;
+          dummy.literals[1] = other;
+          flipped = other;
+        } else {
+          dummy.literals[0] = sign*lit;
+          dummy.literals[1] = other;
+          flipped = (sign < 0) ? -lit : INT_MIN;
         }
-        next:;
+        dummy.redundant = false;
+        dummy.size = 2;
+        d = &dummy;
+        break;
+      }
+
+      if (d) break;
+
+      // In this second loop we check for larger than binary clauses to
+      // subsume or strengthen the candidate clause.   This is more costly,
+      // and needs a call to 'subsume_check'.  Otherwise the same contract
+      // as above for communicating 'subsumption' or 'strengthening' to the
+      // code after the loop is used.
+      //
+      const Occs & os = occs (sign * lit);
+      for (const auto & e : os) {
+        assert (!e->garbage);                   // sanity check
+        if (e->garbage) continue;               // defensive: not needed
+        flipped = subsume_check (e, c);
+        if (!flipped) continue;
+        d = e;                                  // leave also outer loop
+        break;
+      }
+    }
+
+    if (d) break;
+  }
+
+  unmark (c);
+
+  if (flipped == INT_MIN) {
+    LOG (d, "subsuming");
+    subsume_clause (d, c);
+    return 1;
+  }
+
+  if (flipped) {
+    LOG (d, "strengthening");
+    strengthen_clause (c, -flipped);
+    assert (likely_to_be_kept_clause (c));
+    shrunken.push_back (c);
+    return -1;
+  }
+
+  return 0;
+}
+
+/*------------------------------------------------------------------------*/
+
+// Sorting the scheduled clauses is way faster if we compute and save the
+// clause size in the schedule to avoid pointer access to clauses during
+// sorting.  This slightly increases the schedule size though.
+
+struct ClauseSize {
+  size_t size;
+  Clause * clause;
+  ClauseSize (int s, Clause * c) : size (s), clause (c) { }
+  ClauseSize () { }
+};
+
+struct smaller_clause_size_rank {
+  typedef size_t Type;
+  Type operator () (const ClauseSize & a) { return a.size; }
+};
+
+/*------------------------------------------------------------------------*/
+
+struct subsume_less_noccs {
+  Internal * internal;
+  subsume_less_noccs (Internal * i) : internal (i) { }
+  bool operator () (int a, int b) {
+    const signed char u = internal->val (a), v = internal->val (b);
+    if (!u && v) return true;
+    if (u && !v) return false;
+    const int64_t m = internal->noccs (a), n = internal ->noccs (b);
+    if (m < n) return true;
+    if (m > n) return false;
+    return abs (a) < abs (b);
+  }
+};
+
+/*------------------------------------------------------------------------*/
+
+// Usually called from 'subsume' below if 'subsuming' triggered it.  Then
+// the idea is to subsume both redundant and irredundant clauses. It is also
+// called in the elimination loop in 'elim' in which case we focus on
+// irredundant clauses only to help bounded variable elimination.  The
+// function returns true of an irredundant clause was removed or
+// strengthened, which might then in the second usage scenario trigger new
+// variable eliminations.
+
+bool Internal::subsume_round () {
+
+  if (!opts.subsume) return false;
+  if (unsat) return false;
+  if (terminated_asynchronously ()) return false;
+  if (!stats.current.redundant && !stats.current.irredundant) return false;
+
+  START_SIMPLIFIER (subsume, SUBSUME);
+  stats.subsumerounds++;
+
+  int64_t check_limit;
+  if (opts.subsumelimited) {
+    int64_t delta = stats.propagations.search;
+    delta *= 1e-3 * opts.subsumereleff;
+    if (delta < opts.subsumemineff) delta = opts.subsumemineff;
+    if (delta > opts.subsumemaxeff) delta = opts.subsumemaxeff;
+    delta = max (delta, (int64_t) 2l * active ());
+
+    PHASE ("subsume-round", stats.subsumerounds,
+      "limit of %" PRId64 " subsumption checks", delta);
+
+    check_limit = stats.subchecks + delta;
+  } else {
+    PHASE ("subsume-round", stats.subsumerounds,
+      "unlimited subsumption checks");
+    check_limit = LONG_MAX;
+  }
+
+  int old_marked_candidate_variables_for_elimination = stats.mark.elim;
+
+  assert (!level);
+
+  // Allocate schedule and occurrence lists.
+  //
+  vector<ClauseSize> schedule;
+  init_noccs ();
+
+  // Determine candidate clauses and sort them by size.
+  //
+  int64_t left_over_from_last_subsumption_round = 0;
+
+  for (auto c : clauses) {
+
+    if (c->garbage) continue;
+    if (c->size > opts.subsumeclslim) continue;
+    if (!likely_to_be_kept_clause (c)) continue;
+
+    bool fixed = false;
+    int subsume = 0;
+    for (const auto & lit : *c)
+      if (val (lit)) fixed = true;
+      else if (flags (lit).subsume) subsume++;
+
+    // If the clause contains a root level assigned (fixed) literal we will
+    // not work on it.  This simplifies the code substantially since we do
+    // not have to care about assignments at all.  Strengthening becomes
+    // much simpler too.
+    //
+    if (fixed) {
+      LOG (c, "skipping (fixed literal)");
+      continue;
     }
 
-    return true;
-}
-
-
-void SimpSolver::gatherTouchedClauses()
-{
-    if (n_touched == 0) return;
-
-    int i,j;
-    for (i = j = 0; i < subsumption_queue.size(); i++)
-        if (ca[subsumption_queue[i]].mark() == 0)
-            ca[subsumption_queue[i]].mark(2);
-
-    for (i = 0; i < nVars(); i++)
-        if (touched[i]){
-            const vec<CRef>& cs = occurs.lookup(i);
-            for (j = 0; j < cs.size(); j++)
-                if (ca[cs[j]].mark() == 0){
-                    subsumption_queue.insert(cs[j]);
-                    ca[cs[j]].mark(2);
-                }
-            touched[i] = 0;
-        }
-
-    for (i = 0; i < subsumption_queue.size(); i++)
-        if (ca[subsumption_queue[i]].mark() == 2)
-            ca[subsumption_queue[i]].mark(0);
-
-    n_touched = 0;
-}
-
-
-bool SimpSolver::implied(const vec<Lit>& c)
-{
-    assert(decisionLevel() == 0);
-
-    trail_lim.push(trail.size());
-    for (int i = 0; i < c.size(); i++)
-        if (value(c[i]) == l_True){
-            cancelUntil(0);
-            return true;
-        }else if (value(c[i]) != l_False){
-            assert(value(c[i]) == l_Undef);
-            uncheckedEnqueue(~c[i]);
-        }
-
-    bool result = propagate() != CRef_Undef;
-    cancelUntil(0);
-    return result;
-}
-
+    // Further, if less than two variables in the clause were added since
+    // the last subsumption round, the clause is ignored too.
+    //
+    if (subsume < 2) {
+      LOG (c, "skipping (only %d added literals)", subsume);
+      continue;
+    }
+
+    if (c->subsume) left_over_from_last_subsumption_round++;
+    schedule.push_back (ClauseSize (c->size, c));
+    for (const auto & lit : *c)
+      noccs (lit)++;
+  }
+  shrink_vector (schedule);
+
+  // Smaller clauses are checked and connected first.
+  //
+  rsort (schedule.begin (), schedule.end (), smaller_clause_size_rank ());
+
+  if (!left_over_from_last_subsumption_round)
+    for (auto cs : schedule)
+      if (cs.clause->size > 2)
+        cs.clause->subsume = true;
+
+#ifndef QUIET
+  int64_t scheduled = schedule.size ();
+  int64_t total = stats.current.irredundant + stats.current.redundant;
+  PHASE ("subsume-round", stats.subsumerounds,
+    "scheduled %" PRId64 " clauses %.0f%% out of %" PRId64 " clauses",
+    scheduled, percent (scheduled, total), total);
+#endif
 
-// Backward subsumption + backward subsumption resolution
-bool SimpSolver::backwardSubsumptionCheck(bool verbose)
-{
-    int cnt = 0;
-    int subsumed = 0;
-    int deleted_literals = 0;
-    assert(decisionLevel() == 0);
-
-    while (subsumption_queue.size() > 0 || bwdsub_assigns < trail.size()){
-
-        // Empty subsumption queue and return immediately on user-interrupt:
-        if (asynch_interrupt){
-            subsumption_queue.clear();
-            bwdsub_assigns = trail.size();
-            break; }
-
-        // Check top-level assignments by creating a dummy clause and placing it in the queue:
-        if (subsumption_queue.size() == 0 && bwdsub_assigns < trail.size()){
-            Lit l = trail[bwdsub_assigns++];
-            ca[bwdsub_tmpunit][0] = l;
-            ca[bwdsub_tmpunit].calcAbstraction();
-            subsumption_queue.insert(bwdsub_tmpunit); }
-
-        CRef    cr = subsumption_queue.peek(); subsumption_queue.pop();
-        Clause& c  = ca[cr];
-
-        if (c.mark()) continue;
-
-        if (verbose && verbosity >= 2 && cnt++ % 1000 == 0)
-            printf("subsumption left: %10d (%10d subsumed, %10d deleted literals)\r", subsumption_queue.size(), subsumed, deleted_literals);
-
-        assert(c.size() > 1 || value(c[0]) == l_True);    // Unit-clauses should have been propagated before this point.
-
-        // Find best variable to scan:
-        Var best = var(c[0]);
-        for (int i = 1; i < c.size(); i++)
-            if (occurs[var(c[i])].size() < occurs[best].size())
-                best = var(c[i]);
-
-        // Search all candidates:
-        vec<CRef>& _cs = occurs.lookup(best);
-        CRef*       cs = (CRef*)_cs;
-
-        for (int j = 0; j < _cs.size(); j++)
-            if (c.mark())
-                break;
-            else if (!ca[cs[j]].mark() &&  cs[j] != cr && (subsumption_lim == -1 || ca[cs[j]].size() < subsumption_lim)){
-                Lit l = c.subsumes(ca[cs[j]]);
-
-                if (l == lit_Undef)
-                    subsumed++, removeClause(cs[j]);
-                else if (l != lit_Error){
-                    deleted_literals++;
-
-                    if (!strengthenClause(cs[j], ~l))
-                        return false;
-
-                    // Did current candidate get deleted from cs? Then check candidate at index j again:
-                    if (var(l) == best)
-                        j--;
-                }
-            }
+  // Now go over the scheduled clauses in the order of increasing size and
+  // try to forward subsume and strengthen them. Forward subsumption tries
+  // to find smaller or same size clauses which subsume or might strengthen
+  // the candidate.  After the candidate has been processed connect one
+  // of its literals (with smallest number of occurrences at this point) in
+  // a one-watched scheme.
+
+  int64_t subsumed = 0, strengthened = 0, checked = 0;
+
+  vector<Clause *> shrunken;
+  init_occs ();
+  init_bins ();
+
+  for (const auto & s : schedule) {
+
+    if (terminated_asynchronously ()) break;
+    if (stats.subchecks >= check_limit) break;
+
+    Clause * c = s.clause;
+    assert (!c->garbage);
+
+    checked++;
+
+    // First try to subsume or strengthen this candidate clause.  For binary
+    // clauses this could be done much faster by hashing and is costly due
+    // to a usually large number of binary clauses.  There is further the
+    // issue, that strengthening binary clauses (through double
+    // self-subsuming resolution) would produce units, which needs much more
+    // care. In the same (lazy) spirit we also ignore clauses with fixed
+    // literals (false or true).
+    //
+    if (c->size > 2 && c->subsume) {
+      c->subsume = false;
+      const int tmp = try_to_subsume_clause (c, shrunken);
+      if (tmp > 0) { subsumed++; continue; }
+      if (tmp < 0) strengthened++;
     }
 
-    return true;
-}
-
-
-bool SimpSolver::asymm(Var v, CRef cr)
-{
-    Clause& c = ca[cr];
-    assert(decisionLevel() == 0);
-
-    if (c.mark() || satisfied(c)) return true;
-
-    trail_lim.push(trail.size());
-    Lit l = lit_Undef;
-    for (int i = 0; i < c.size(); i++)
-        if (var(c[i]) != v && value(c[i]) != l_False)
-            uncheckedEnqueue(~c[i]);
-        else
-            l = c[i];
-
-    if (propagate() != CRef_Undef){
-        cancelUntil(0);
-        asymm_lits++;
-        if (!strengthenClause(cr, l))
-            return false;
-    }else
-        cancelUntil(0);
-
-    return true;
-}
-
-
-bool SimpSolver::asymmVar(Var v)
-{
-    assert(use_simplification);
-
-    const vec<CRef>& cls = occurs.lookup(v);
-
-    if (value(v) != l_Undef || cls.size() == 0)
-        return true;
-
-    for (int i = 0; i < cls.size(); i++)
-        if (!asymm(v, cls[i]))
-            return false;
-
-    return backwardSubsumptionCheck();
-}
-
-
-static void mkElimClause(vec<uint32_t>& elimclauses, Lit x)
-{
-    elimclauses.push(toInt(x));
-    elimclauses.push(1);
-}
-
-
-static void mkElimClause(vec<uint32_t>& elimclauses, Var v, Clause& c)
-{
-    int first = elimclauses.size();
-    int v_pos = -1;
+    // If not subsumed connect smallest occurring literal, where occurring
+    // means the number of times it was used to connect (as a one-watch) a
+    // previous smaller or equal sized clause.  This minimizes the length of
+    // the occurrence lists traversed during 'try_to_subsume_clause'. Also
+    // note that this number is usually way smaller than the number of
+    // occurrences computed before and stored in 'noccs'.
+    //
+    int minlit = 0;
+    int64_t minoccs = 0;
+    size_t minsize = 0;
+    bool subsume = true;
+    bool binary = (c->size == 2 && !c->redundant);
+
+    for (const auto & lit : *c) {
+
+      if (!flags (lit).subsume) subsume = false;
+      const size_t size = binary ? bins (lit).size () : occs (lit).size ();
+      if (minlit && minsize <= size) continue;
+      const int64_t tmp = noccs (lit);
+      if (minlit && minsize == size && tmp <= minoccs) continue;
+      minlit = lit, minsize = size, minoccs = tmp;
+    }
+
+    // If there is a variable in a clause different from is not 'subsume'
+    // (has been added since the last subsumption round), then this clause
+    // can not serve to strengthen or subsume another clause, since all
+    // shrunken or added clauses mark all their variables as 'subsume'.
+    //
+    if (!subsume) continue;
 
-    // Copy clause to elimclauses-vector. Remember position where the
-    // variable 'v' occurs:
-    for (int i = 0; i < c.size(); i++){
-        elimclauses.push(toInt(c[i]));
-        if (var(c[i]) == v)
-            v_pos = i + first;
-    }
-    assert(v_pos != -1);
+    if (!binary) {
 
-    // Swap the first literal with the 'v' literal, so that the literal
-    // containing 'v' will occur first in the clause:
-    uint32_t tmp = elimclauses[v_pos];
-    elimclauses[v_pos] = elimclauses[first];
-    elimclauses[first] = tmp;
+      // If smallest occurring literal occurs too often do not connect.
+      //
+      if (minsize > (size_t) opts.subsumeocclim) continue;
 
-    // Store the length of the clause last:
-    elimclauses.push(c.size());
-}
+      LOG (c, "watching %d with %zd current and total %" PRId64 " occurrences",
+        minlit, minsize, minoccs);
 
+      occs (minlit).push_back (c);
 
+      // This sorting should give faster failures for assumption checks
+      // since the less occurring variables are put first in a clause and
+      // thus will make it more likely to be found as witness for a clause
+      // not to be subsuming.  One could in principle (see also the
+      // discussion on 'subsumption' in our 'Splatz' solver) replace marking
+      // by a kind of merge sort, as also suggested by Bayardo.  It would
+      // avoid 'marked' calls and thus might be slightly faster but could
+      // not take benefit of this sorting optimization.
+      //
+      sort (c->begin (), c->end (), subsume_less_noccs (this));
 
-bool SimpSolver::eliminateVar(Var v)
-{
-    assert(!frozen[v]);
-    assert(!isEliminated(v));
-    assert(value(v) == l_Undef);
+    } else {
 
-    // Split the occurrences into positive and negative:
-    //
-    const vec<CRef>& cls = occurs.lookup(v);
-    vec<CRef>        pos, neg;
-    for (int i = 0; i < cls.size(); i++)
-        (find(ca[cls[i]], mkLit(v)) ? pos : neg).push(cls[i]);
+      // If smallest occurring literal occurs too often do not connect.
+      //
+      if (minsize > (size_t) opts.subsumebinlim) continue;
 
-    // Check wether the increase in number of clauses stays within the allowed ('grow'). Moreover, no
-    // clause must exceed the limit on the maximal clause size (if it is set):
-    //
-    int cnt         = 0;
-    int clause_size = 0;
+      LOG (c,
+        "watching %d with %zd current binary and total %" PRId64 " occurrences",
+        minlit, minsize, minoccs);
 
-    for (int i = 0; i < pos.size(); i++)
-        for (int j = 0; j < neg.size(); j++)
-            if (merge(ca[pos[i]], ca[neg[j]], v, clause_size) && 
-                (++cnt > cls.size() + grow || (clause_lim != -1 && clause_size > clause_lim)))
-                return true;
-
-    // Delete and store old clauses:
-    eliminated[v] = true;
-    setDecisionVar(v, false);
-    eliminated_vars++;
-
-    if (pos.size() > neg.size()){
-        for (int i = 0; i < neg.size(); i++)
-            mkElimClause(elimclauses, v, ca[neg[i]]);
-        mkElimClause(elimclauses, mkLit(v));
-    }else{
-        for (int i = 0; i < pos.size(); i++)
-            mkElimClause(elimclauses, v, ca[pos[i]]);
-        mkElimClause(elimclauses, ~mkLit(v));
+      const int minlit_pos = (c->literals[1] == minlit);
+      const int other = c->literals[!minlit_pos];
+      bins (minlit).push_back (other);
     }
+  }
 
-    for (int i = 0; i < cls.size(); i++)
-        removeClause(cls[i]); 
+  PHASE ("subsume-round", stats.subsumerounds,
+    "subsumed %" PRId64 " and strengthened %" PRId64
+    " out of %" PRId64 " clauses %.0f%%",
+    subsumed, strengthened, scheduled,
+    percent (subsumed + strengthened, scheduled));
 
-    // Produce clauses in cross product:
-    vec<Lit>& resolvent = add_tmp;
-    for (int i = 0; i < pos.size(); i++)
-        for (int j = 0; j < neg.size(); j++)
-            if (merge(ca[pos[i]], ca[neg[j]], v, resolvent) && !addClause_(resolvent))
-                return false;
-
-    // Free occurs list for this variable:
-    occurs[v].clear(true);
-    
-    // Free watchers lists for this variable, if possible:
-    if (watches[ mkLit(v)].size() == 0) watches[ mkLit(v)].clear(true);
-    if (watches[~mkLit(v)].size() == 0) watches[~mkLit(v)].clear(true);
+  const int64_t remain = schedule.size () - checked;
+  const bool completed = !remain;
 
-    return backwardSubsumptionCheck();
-}
+  if (completed)
+    PHASE ("subsume-round", stats.subsumerounds,
+      "checked all %" PRId64 " scheduled clauses", checked);
+  else
+    PHASE ("subsume-round", stats.subsumerounds,
+      "checked %" PRId64 " clauses %.0f%% of scheduled (%" PRId64 " remain)",
+      checked, percent (checked, scheduled), remain);
 
+  // Release occurrence lists and schedule.
+  //
+  erase_vector (schedule);
+  reset_noccs ();
+  reset_occs ();
+  reset_bins ();
 
-bool SimpSolver::substitute(Var v, Lit x)
-{
-    assert(!frozen[v]);
-    assert(!isEliminated(v));
-    assert(value(v) == l_Undef);
-
-    if (!ok) return false;
-
-    eliminated[v] = true;
-    setDecisionVar(v, false);
-    const vec<CRef>& cls = occurs.lookup(v);
-    
-    vec<Lit>& subst_clause = add_tmp;
-    for (int i = 0; i < cls.size(); i++){
-        Clause& c = ca[cls[i]];
-
-        subst_clause.clear();
-        for (int j = 0; j < c.size(); j++){
-            Lit p = c[j];
-            subst_clause.push(var(p) == v ? x ^ sign(p) : p);
-        }
-
-        removeClause(cls[i]);
-
-        if (!addClause_(subst_clause))
-            return ok = false;
-    }
+  // Reset all old 'added' flags and mark variables in shrunken
+  // clauses as 'added' for the next subsumption round.
+  //
+  if (completed)
+    reset_subsume_bits ();
 
-    return true;
-}
+  for (const auto & c : shrunken)
+    mark_added (c);
+  erase_vector (shrunken);
 
+  report ('s', !opts.reportall && !(subsumed + strengthened));
 
-void SimpSolver::extendModel()
-{
-    int i, j;
-    Lit x;
+  STOP_SIMPLIFIER (subsume, SUBSUME);
 
-    for (i = elimclauses.size()-1; i > 0; i -= j){
-        for (j = elimclauses[i--]; j > 1; j--, i--)
-            if (modelValue(toLit(elimclauses[i])) != l_False)
-                goto next;
-
-        x = toLit(elimclauses[i]);
-        model[var(x)] = lbool(!sign(x));
-    next:;
-    }
+  return old_marked_candidate_variables_for_elimination < stats.mark.elim;
 }
 
+/*------------------------------------------------------------------------*/
 
-bool SimpSolver::eliminate(bool turn_off_elim)
-{
-    if (!simplify())
-        return false;
-    else if (!use_simplification)
-        return true;
+void Internal::subsume (bool update_limits) {
 
-    // Main simplification loop:
-    //
-    while (n_touched > 0 || bwdsub_assigns < trail.size() || elim_heap.size() > 0){
+  stats.subsumephases++;
 
-        gatherTouchedClauses();
-        // printf("  ## (time = %6.2f s) BWD-SUB: queue = %d, trail = %d\n", cpuTime(), subsumption_queue.size(), trail.size() - bwdsub_assigns);
-        if ((subsumption_queue.size() > 0 || bwdsub_assigns < trail.size()) && 
-            !backwardSubsumptionCheck(true)){
-            ok = false; goto cleanup; }
-
-        // Empty elim_heap and return immediately on user-interrupt:
-        if (asynch_interrupt){
-            assert(bwdsub_assigns == trail.size());
-            assert(subsumption_queue.size() == 0);
-            assert(n_touched == 0);
-            elim_heap.clear();
-            goto cleanup; }
-
-        // printf("  ## (time = %6.2f s) ELIM: vars = %d\n", cpuTime(), elim_heap.size());
-        for (int cnt = 0; !elim_heap.empty(); cnt++){
-            Var elim = elim_heap.removeMin();
-            
-            if (asynch_interrupt) break;
-
-            if (isEliminated(elim) || value(elim) != l_Undef) continue;
-
-            if (verbosity >= 2 && cnt % 100 == 0)
-                printf("elimination left: %10d\r", elim_heap.size());
-
-            if (use_asymm){
-                // Temporarily freeze variable. Otherwise, it would immediately end up on the queue again:
-                bool was_frozen = frozen[elim];
-                frozen[elim] = true;
-                if (!asymmVar(elim)){
-                    ok = false; goto cleanup; }
-                frozen[elim] = was_frozen; }
-
-            // At this point, the variable may have been set by assymetric branching, so check it
-            // again. Also, don't eliminate frozen variables:
-            if (use_elim && value(elim) == l_Undef && !frozen[elim] && !eliminateVar(elim)){
-                ok = false; goto cleanup; }
+  if (!stats.current.redundant && !stats.current.irredundant)
+    goto UPDATE_LIMITS;
 
-            checkGarbage(simp_garbage_frac);
-        }
+  if (unsat) return;
 
-        assert(subsumption_queue.size() == 0);
-    }
- cleanup:
+  backtrack ();
+  if (!propagate ()) {
+    learn_empty_clause ();
+    return;
+  }
 
-    // If no more simplification is needed, free all simplification-related data structures:
-    if (turn_off_elim){
-        touched  .clear(true);
-        occurs   .clear(true);
-        n_occ    .clear(true);
-        elim_heap.clear(true);
-        subsumption_queue.clear(true);
-
-        use_simplification    = false;
-        remove_satisfied      = true;
-        ca.extra_clause_field = false;
-        max_simp_var          = nVars();
-
-        // Force full cleanup (this is safe and desirable since it only happens once):
-        rebuildOrderHeap();
-        garbageCollect();
-    }else{
-        // Cheaper cleanup:
-        checkGarbage();
+  if (opts.subsume) {
+    reset_watches ();
+    subsume_round ();
+    init_watches ();
+    connect_watches ();
+    if (!unsat && !propagate ()) {
+      LOG ("propagation after subsume rounds results in inconsistency");
+      learn_empty_clause ();
     }
+  }
 
-    if (verbosity >= 1 && elimclauses.size() > 0)
-        printf("|  Eliminated clauses:     %10.2f Mb                                      |\n", 
-               double(elimclauses.size() * sizeof(uint32_t)) / (1024*1024));
-
-    return ok;
-}
-
-
-//=================================================================================================
-// Garbage Collection methods:
+  // Schedule 'vivification' in 'subsume' as well as 'transitive reduction'.
+  //
+  if (opts.vivify) vivify ();
+  if (opts.transred) transred ();
 
+UPDATE_LIMITS:
 
-void SimpSolver::relocAll(ClauseAllocator& to)
-{
-    if (!use_simplification) return;
+  if (!update_limits) return;
 
-    // All occurs lists:
-    //
-    for (int i = 0; i < nVars(); i++){
-        occurs.clean(i);
-        vec<CRef>& cs = occurs[i];
-        for (int j = 0; j < cs.size(); j++)
-            ca.reloc(cs[j], to);
-    }
+  int64_t delta = scale (opts.subsumeint * (stats.subsumephases + 1));
+  lim.subsume = stats.conflicts + delta;
 
-    // Subsumption queue:
-    //
-    for (int i = subsumption_queue.size(); i > 0; i--){
-        CRef cr = subsumption_queue.peek(); subsumption_queue.pop();
-        if (ca[cr].mark()) continue;
-        ca.reloc(cr, to);
-        subsumption_queue.insert(cr);
-    }
-        
-    // Temporary clause:
-    //
-    ca.reloc(bwdsub_tmpunit, to);
+  PHASE ("subsume-phase", stats.subsumephases,
+    "new subsume limit %" PRId64 " after %" PRId64 " conflicts",
+    lim.subsume, delta);
 }
 
-
-void SimpSolver::garbageCollect()
-{
-    // Initialize the next region to a size corresponding to the estimated utilization degree. This
-    // is not precise but should avoid some unnecessary reallocations for the new region:
-    ClauseAllocator to(ca.size() - ca.wasted()); 
-
-    to.extra_clause_field = ca.extra_clause_field; // NOTE: this is important to keep (or lose) the extra fields.
-    relocAll(to);
-    Solver::relocAll(to);
-    if (verbosity >= 2)
-        printf("|  Garbage collection:   %12d bytes => %12d bytes             |\n", 
-               ca.size()*ClauseAllocator::Unit_Size, to.size()*ClauseAllocator::Unit_Size);
-    to.moveTo(ca);
 }
```

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/minisat/utils/System.cc` & `lincs-0.6.0/lincs/liblincs/vendored/minisat/utils/System.cc`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/rapidcsv.h` & `lincs-0.6.0/lincs/liblincs/vendored/rapidcsv.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/valijson/adapters/std_string_adapter.hpp` & `lincs-0.6.0/lincs/liblincs/vendored/valijson/adapters/std_string_adapter.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/valijson/adapters/yaml_cpp_adapter.hpp` & `lincs-0.6.0/lincs/liblincs/vendored/valijson/adapters/yaml_cpp_adapter.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/valijson/constraints/basic_constraint.hpp` & `lincs-0.6.0/lincs/liblincs/vendored/valijson/constraints/basic_constraint.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/valijson/constraints/concrete_constraints.hpp` & `lincs-0.6.0/lincs/liblincs/vendored/valijson/constraints/concrete_constraints.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/valijson/constraints/constraint.hpp` & `lincs-0.6.0/lincs/liblincs/vendored/valijson/constraints/constraint.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/valijson/constraints/constraint_visitor.hpp` & `lincs-0.6.0/lincs/liblincs/vendored/valijson/constraints/constraint_visitor.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/valijson/exceptions.hpp` & `lincs-0.6.0/lincs/liblincs/vendored/valijson/exceptions.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/adapter.hpp` & `lincs-0.6.0/lincs/liblincs/vendored/valijson/internal/adapter.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/basic_adapter.hpp` & `lincs-0.6.0/lincs/liblincs/vendored/valijson/internal/basic_adapter.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/custom_allocator.hpp` & `lincs-0.6.0/lincs/liblincs/vendored/valijson/internal/custom_allocator.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/debug.hpp` & `lincs-0.6.0/lincs/liblincs/vendored/valijson/internal/debug.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/frozen_value.hpp` & `lincs-0.6.0/lincs/liblincs/vendored/valijson/internal/frozen_value.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/json_pointer.hpp` & `lincs-0.6.0/lincs/liblincs/vendored/valijson/internal/json_pointer.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/json_reference.hpp` & `lincs-0.6.0/lincs/liblincs/vendored/valijson/internal/json_reference.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/uri.hpp` & `lincs-0.6.0/lincs/liblincs/vendored/valijson/internal/uri.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/valijson/schema.hpp` & `lincs-0.6.0/lincs/liblincs/vendored/valijson/schema.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/valijson/schema_parser.hpp` & `lincs-0.6.0/lincs/liblincs/vendored/valijson/schema_parser.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/valijson/subschema.hpp` & `lincs-0.6.0/lincs/liblincs/vendored/valijson/subschema.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/valijson/utils/file_utils.hpp` & `lincs-0.6.0/lincs/liblincs/vendored/valijson/utils/file_utils.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/valijson/utils/utf8_utils.hpp` & `lincs-0.6.0/lincs/liblincs/vendored/valijson/utils/utf8_utils.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/valijson/validation_results.hpp` & `lincs-0.6.0/lincs/liblincs/vendored/valijson/validation_results.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/valijson/validation_visitor.hpp` & `lincs-0.6.0/lincs/liblincs/vendored/valijson/validation_visitor.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs/vendored/valijson/validator.hpp` & `lincs-0.6.0/lincs/liblincs/vendored/valijson/validator.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs/liblincs_module_tests.py` & `lincs-0.6.0/lincs/liblincs_module_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,15 +285,15 @@
         class MyTerminationStrategy(LearnMrsortByWeightsProfilesBreed.TerminationStrategy):
             def __init__(self):
                 super().__init__()
                 self.called_count = 0
 
             def terminate(self):
                 self.called_count += 1
-                return False
+                return self.called_count == 6
 
         learning_data = LearnMrsortByWeightsProfilesBreed.LearningData.make(problem, learning_set, 9, 44)
         profiles_initialization_strategy = InitializeProfilesForProbabilisticMaximalDiscriminationPowerPerCriterion(learning_data)
         weights_optimization_strategy = OptimizeWeightsUsingGlop(learning_data)
         profiles_improvement_strategy = ImproveProfilesWithAccuracyHeuristicOnCpu(learning_data)
         breeding_strategy = ReinitializeLeastAccurate(learning_data, profiles_initialization_strategy, 4)
         my_termination_strategy = MyTerminationStrategy()
@@ -303,16 +303,16 @@
             profiles_initialization_strategy,
             weights_optimization_strategy,
             profiles_improvement_strategy,
             breeding_strategy,
             termination_strategy,
         ).perform()
 
-        self.assertEqual(my_termination_strategy.called_count, 7)
-        self.assertEqual(classify_alternatives(problem, learned_model, learning_set).changed, 0)
+        self.assertEqual(my_termination_strategy.called_count, 6)
+        self.assertEqual(classify_alternatives(problem, learned_model, learning_set).changed, 1)
 
     def test_python_strategies(self):
         problem = generate_classification_problem(5, 3, 41)
         model = generate_mrsort_classification_model(problem, 42)
         learning_set = generate_classified_alternatives(problem, model, 200, 43)
 
         class MyProfileInitializationStrategy(LearnMrsortByWeightsProfilesBreed.ProfilesInitializationStrategy):
@@ -499,22 +499,22 @@
         self.assertEqual(result.unchanged, 200)
 
         testing_set = generate_classified_alternatives(problem, model, 1000, 44)
         result = classify_alternatives(problem, learned_model, testing_set)
         self.assertEqual(result.changed, 21)
         self.assertEqual(result.unchanged, 979)
 
-    def test_sat_by_coalitions_using_evalmaxsat_learning(self):
-        problem = generate_classification_problem(5, 3, 41)
+    def test_sat_by_separation_using_minisat_learning(self):
+        problem = generate_classification_problem(5, 2, 41)
         model = generate_mrsort_classification_model(problem, 42)
         learning_set = generate_classified_alternatives(problem, model, 200, 43)
 
-        learned_model = LearnUcncsBySatByCoalitionsUsingEvalmaxsat(problem, learning_set).perform()
+        learned_model = LearnUcncsBySatBySeparationUsingMinisat(problem, learning_set).perform()
 
         result = classify_alternatives(problem, learned_model, learning_set)
         self.assertEqual(result.changed, 0)
         self.assertEqual(result.unchanged, 200)
 
         testing_set = generate_classified_alternatives(problem, model, 1000, 44)
         result = classify_alternatives(problem, learned_model, testing_set)
-        self.assertEqual(result.changed, 29)
-        self.assertEqual(result.unchanged, 971)
+        self.assertEqual(result.changed, 24)
+        self.assertEqual(result.unchanged, 976)
```

### Comparing `lincs-0.5.1/lincs/visualization.py` & `lincs-0.6.0/lincs/visualization.py`

 * *Files identical despite different names*

### Comparing `lincs-0.5.1/lincs.egg-info/PKG-INFO` & `lincs-0.6.0/lincs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lincs
-Version: 0.5.1
+Version: 0.6.0
 Summary: Learn and Infer Non Compensatory Sortings
 Home-page: https://github.com/MICS-Lab/lincs
 Author: Vincent Jacques
 Author-email: vincent@vincent-jacques.net
 License: LGPLv3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
@@ -25,15 +25,15 @@
     - on GitHub (https://github.com/mics-lab/lincs/)
     - on PyPI after publication of the package (https://pypi.org/project/lincs/)
     - on GitHub Pages (https://mics-lab.github.io/lincs/)
     So when you change it, take care to check all those places.
 
 *lincs* (Learn and Infer Non Compensatory Sortings) is a collection of MCDA algorithms, usable as a C++ library, a Python (3.7+) package and a command-line utility.
 
-*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v0.5.1/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v0.5.1/COPYING.LESSER>`_.
+*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v0.6.0/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v0.6.0/COPYING.LESSER>`_.
 
 @todo (When we have a paper to actually cite) Add a note asking academics to kindly cite our work.
 
 *lincs* is available for install from the `Python package index <https://pypi.org/project/lincs/>`_.
 Its `documentation <http://mics-lab.github.io/lincs/>`_
 and its `source code <https://github.com/mics-lab/lincs/>`_ are on GitHub.
```

### Comparing `lincs-0.5.1/setup.py` & `lincs-0.6.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,29 +5,35 @@
 import os
 import shutil
 import sys
 import setuptools
 import setuptools.command.build_ext
 
 
-version = "0.5.1"
+version = "0.6.0"
 
 with open("README.rst") as f:
     long_description = f.read()
 for file in ["COPYING", "COPYING.LESSER"]:
     long_description = long_description.replace(f" <{file}>`_", f" <https://github.com/MICS-Lab/lincs/blob/v{version}/{file}>`_")
 for lang in ["yaml", "shell", "text", "diff"]:
     long_description = long_description.replace(f".. highlight:: {lang}", "")
 
 with open("requirements.txt") as f:
     install_requires = f.readlines()
 
 
 has_nvcc = os.environ.get("LINCS_DEV_FORBID_NVCC", "false") != "true" and shutil.which("nvcc") is not None
 
+coverage_compile_args = []
+coverage_link_args = []
+if os.environ.get("LINCS_DEV_COVERAGE", "false") == "true":
+    coverage_compile_args = ["--coverage", "-O0"]
+    coverage_link_args = ["--coverage"]
+
 # Method for building an extension with CUDA code extracted from https://stackoverflow.com/a/13300714/905845
 # @todo Consider using scikit-build:
 # it should make it easier to compile CUDA code using nvcc and to run C++ unit tests during build.
 # Note that pybind11 comes with an example of building using scikit-build.
 # (see also https://www.benjack.io/hybrid-python/c-packages-revisited/)
 def customize_compiler_for_nvcc(self):
     self.src_extensions.append(".cu")
@@ -35,18 +41,18 @@
     default_compiler_so = self.compiler_so
     default_compile = self._compile
 
     def _compile(obj, src, ext, cc_args, extra_postargs, pp_opts):
         if os.path.splitext(src)[1] == ".cu":
             self.set_executable("compiler_so", "nvcc")
             postargs = extra_postargs["nvcc"]
+        elif "/vendored/" in src:
+            postargs = extra_postargs["gcc"] + ["-w", "-DQUIET", "-DNBUILD"]
         else:
-            postargs = extra_postargs["gcc"]
-        if "/vendored/" in src:
-            postargs = postargs + ["-w"]
+            postargs = extra_postargs["gcc"] + coverage_compile_args
 
         default_compile(obj, src, ext, cc_args, postargs, pp_opts)
         self.compiler_so = default_compiler_so
 
     self._compile = _compile
 
 
@@ -88,15 +94,15 @@
     library_dirs=["/usr/local/cuda-12.1/targets/x86_64-linux/lib"],
     # Non-standard: the dict is accessed in `customize_compiler_for_nvcc`
     # to get the standard form for `extra_compile_args`
     extra_compile_args={
         "gcc": ["-std=c++17", "-Werror=switch"] + omp_compile_args,
         "nvcc": ["-std=c++17", "-Xcompiler", "-fopenmp,-fPIC,-Werror=switch"],
     },
-    extra_link_args=omp_link_args,
+    extra_link_args=omp_link_args + coverage_link_args,
 )
 
 setuptools.setup(
     name="lincs",
     version=version,
     description="Learn and Infer Non Compensatory Sortings",
     license="LGPLv3",
```

