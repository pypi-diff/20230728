# Comparing `tmp/linopy-0.2.2.tar.gz` & `tmp/linopy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linopy-0.2.2.tar", last modified: Wed Jun 28 14:01:38 2023, max compression
+gzip compressed data, was "linopy-0.2.3.tar", last modified: Fri Jul 28 09:49:04 2023, max compression
```

## Comparing `linopy-0.2.2.tar` & `linopy-0.2.3.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:01:38.903917 linopy-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)   180224 2023-06-28 14:01:29.000000 linopy-0.2.2/.coverage
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-28 14:01:29.000000 linopy-0.2.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:01:38.883917 linopy-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:01:38.887917 linopy-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-28 14:01:29.000000 linopy-0.2.2/.github/workflows/CI.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-28 14:01:29.000000 linopy-0.2.2/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-28 14:01:29.000000 linopy-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-28 14:01:29.000000 linopy-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-28 14:01:29.000000 linopy-0.2.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-28 14:01:29.000000 linopy-0.2.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-28 14:01:29.000000 linopy-0.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-28 14:01:38.903917 linopy-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-28 14:01:29.000000 linopy-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:01:38.887917 linopy-0.2.2/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/Snakefile
--rw-r--r--   0 runner    (1001) docker     (123)    21144 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/benchmark-absolute.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   188981 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/benchmark-absolute.png
--rw-r--r--   0 runner    (1001) docker     (123)    20512 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/benchmark-overhead.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   179946 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/benchmark-overhead.png
--rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/benchmark_resource-absolute.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   149975 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/benchmark_resource-absolute.png
--rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/benchmark_resource-overhead.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   132957 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/benchmark_resource-overhead.png
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/environment.fixed.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:01:38.887917 linopy-0.2.2/benchmark/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/notebooks/plot-benchmarks.py.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:01:38.891918 linopy-0.2.2/benchmark/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1450 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/benchmark_cvxpy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1537 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/benchmark_gurobipy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1541 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/benchmark_jump.jl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1458 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/benchmark_linopy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2007 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/benchmark_ortools.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1796 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/benchmark_pulp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2043 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/benchmark_pyomo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:01:38.891918 linopy-0.2.2/benchmark/scripts/benchmarks-pypsa-eur/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/benchmarks-pypsa-eur/benchmark-linopy.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/benchmarks-pypsa-eur/benchmark-pyomo.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/benchmarks-pypsa-eur/benchmark-pypsa-linopf.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/benchmarks-pypsa-eur/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/benchmarks-pypsa-eur/plot-benchmarks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      469 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1050 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/concat-benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:01:38.891918 linopy-0.2.2/benchmark/scripts/leftovers/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/leftovers/benchmark-linopy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:01:38.895918 linopy-0.2.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:01:38.895918 linopy-0.2.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-linopy.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pyomo.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pypsa-linopf.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/plot-benchmarks.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-linopy-pypsa-eur.dat
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-linopy.py
--rw-r--r--   0 runner    (1001) docker     (123)   103087 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pyomo-pypsa-eur.dat
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pyomo.py
--rw-r--r--   0 runner    (1001) docker     (123)    26681 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur-with-pypsa.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    18332 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-linopf.py
--rw-r--r--   0 runner    (1001) docker     (123)   381819 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa_linopf-pypsa-eur.dat
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/plot-benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/leftovers/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1392 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/merge-benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/plot-benchmarks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/run-cvxpy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/run-gurobipy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      399 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/run-linopy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      290 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/run-ortools.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      287 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/run-pulp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      399 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/run-pyomo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-06-28 14:01:29.000000 linopy-0.2.2/benchmark/scripts/write-lp-file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:01:38.899917 linopy-0.2.2/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-28 14:01:29.000000 linopy-0.2.2/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:01:38.899917 linopy-0.2.2/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-28 14:01:29.000000 linopy-0.2.2/doc/_static/theme_overrides.css
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-28 14:01:29.000000 linopy-0.2.2/doc/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)    57997 2023-06-28 14:01:29.000000 linopy-0.2.2/doc/benchmark.png
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-28 14:01:29.000000 linopy-0.2.2/doc/benchmark.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-28 14:01:29.000000 linopy-0.2.2/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-06-28 14:01:29.000000 linopy-0.2.2/doc/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-28 14:01:29.000000 linopy-0.2.2/doc/create-a-model-with-coordinates.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-28 14:01:29.000000 linopy-0.2.2/doc/create-a-model.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-28 14:01:29.000000 linopy-0.2.2/doc/creating-constraints.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-28 14:01:29.000000 linopy-0.2.2/doc/creating-expressions.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-28 14:01:29.000000 linopy-0.2.2/doc/creating-variables.nblink
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-06-28 14:01:29.000000 linopy-0.2.2/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-28 14:01:29.000000 linopy-0.2.2/doc/infeasible-model.nblink
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-06-28 14:01:29.000000 linopy-0.2.2/doc/logo.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    49959 2023-06-28 14:01:29.000000 linopy-0.2.2/doc/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-28 14:01:29.000000 linopy-0.2.2/doc/logo.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-28 14:01:29.000000 linopy-0.2.2/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-28 14:01:29.000000 linopy-0.2.2/doc/manipulating-models.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-28 14:01:29.000000 linopy-0.2.2/doc/migrating-from-pyomo.nblink
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-28 14:01:29.000000 linopy-0.2.2/doc/prerequisites.rst
--rw-r--r--   0 runner    (1001) docker     (123)    20317 2023-06-28 14:01:29.000000 linopy-0.2.2/doc/release_notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 14:01:29.000000 linopy-0.2.2/doc/solve-on-remote.nblink
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-28 14:01:29.000000 linopy-0.2.2/doc/syntax.rst
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-28 14:01:29.000000 linopy-0.2.2/doc/testing-framework.nblink
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-28 14:01:29.000000 linopy-0.2.2/doc/user-guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:01:38.899917 linopy-0.2.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-06-28 14:01:29.000000 linopy-0.2.2/examples/create-a-model-with-coordinates.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-06-28 14:01:29.000000 linopy-0.2.2/examples/create-a-model.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-06-28 14:01:29.000000 linopy-0.2.2/examples/creating-constraints.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-06-28 14:01:29.000000 linopy-0.2.2/examples/creating-expressions.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    16957 2023-06-28 14:01:29.000000 linopy-0.2.2/examples/creating-variables.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-28 14:01:29.000000 linopy-0.2.2/examples/infeasible-model.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-06-28 14:01:29.000000 linopy-0.2.2/examples/manipulating-models.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-28 14:01:29.000000 linopy-0.2.2/examples/migrating-from-pyomo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    26407 2023-06-28 14:01:29.000000 linopy-0.2.2/examples/solve-on-remote.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-28 14:01:29.000000 linopy-0.2.2/examples/testing-framework.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:01:38.899917 linopy-0.2.2/linopy/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-28 14:01:29.000000 linopy-0.2.2/linopy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12779 2023-06-28 14:01:29.000000 linopy-0.2.2/linopy/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-28 14:01:29.000000 linopy-0.2.2/linopy/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-28 14:01:29.000000 linopy-0.2.2/linopy/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    30484 2023-06-28 14:01:29.000000 linopy-0.2.2/linopy/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)    47260 2023-06-28 14:01:29.000000 linopy-0.2.2/linopy/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-06-28 14:01:29.000000 linopy-0.2.2/linopy/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-06-28 14:01:29.000000 linopy-0.2.2/linopy/matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)    38430 2023-06-28 14:01:29.000000 linopy-0.2.2/linopy/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-28 14:01:29.000000 linopy-0.2.2/linopy/monkey_patch_xarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-06-28 14:01:29.000000 linopy-0.2.2/linopy/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    20119 2023-06-28 14:01:29.000000 linopy-0.2.2/linopy/solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-28 14:01:29.000000 linopy-0.2.2/linopy/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    35634 2023-06-28 14:01:29.000000 linopy-0.2.2/linopy/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-28 14:01:38.000000 linopy-0.2.2/linopy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:01:38.903917 linopy-0.2.2/linopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-28 14:01:38.000000 linopy-0.2.2/linopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-06-28 14:01:38.000000 linopy-0.2.2/linopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 14:01:38.000000 linopy-0.2.2/linopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-28 14:01:38.000000 linopy-0.2.2/linopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-28 14:01:38.000000 linopy-0.2.2/linopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-28 14:01:29.000000 linopy-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 14:01:38.903917 linopy-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-28 14:01:29.000000 linopy-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:01:38.903917 linopy-0.2.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-06-28 14:01:29.000000 linopy-0.2.2/test/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-06-28 14:01:29.000000 linopy-0.2.2/test/test_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-28 14:01:29.000000 linopy-0.2.2/test/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-28 14:01:29.000000 linopy-0.2.2/test/test_inconsistency_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-28 14:01:29.000000 linopy-0.2.2/test/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    17392 2023-06-28 14:01:29.000000 linopy-0.2.2/test/test_linear_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-28 14:01:29.000000 linopy-0.2.2/test/test_matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-28 14:01:29.000000 linopy-0.2.2/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15195 2023-06-28 14:01:29.000000 linopy-0.2.2/test/test_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-28 14:01:29.000000 linopy-0.2.2/test/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-06-28 14:01:29.000000 linopy-0.2.2/test/test_quadratic_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-06-28 14:01:29.000000 linopy-0.2.2/test/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-28 14:01:29.000000 linopy-0.2.2/test/test_scalar_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-28 14:01:29.000000 linopy-0.2.2/test/test_scalar_linear_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-06-28 14:01:29.000000 linopy-0.2.2/test/test_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-06-28 14:01:29.000000 linopy-0.2.2/test/test_variable_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-28 14:01:29.000000 linopy-0.2.2/test/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:49:04.923808 linopy-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)   180224 2023-07-28 09:48:55.000000 linopy-0.2.3/.coverage
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 09:48:55.000000 linopy-0.2.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:49:04.903808 linopy-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:49:04.907808 linopy-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-28 09:48:55.000000 linopy-0.2.3/.github/workflows/CI.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-28 09:48:55.000000 linopy-0.2.3/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-28 09:48:55.000000 linopy-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-28 09:48:55.000000 linopy-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-28 09:48:55.000000 linopy-0.2.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-28 09:48:55.000000 linopy-0.2.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-28 09:48:55.000000 linopy-0.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-07-28 09:49:04.923808 linopy-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-28 09:48:55.000000 linopy-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:49:04.911809 linopy-0.2.3/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (123)    21144 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/benchmark-absolute.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   188981 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/benchmark-absolute.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20512 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/benchmark-overhead.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   179946 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/benchmark-overhead.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/benchmark_resource-absolute.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   149975 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/benchmark_resource-absolute.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/benchmark_resource-overhead.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   132957 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/benchmark_resource-overhead.png
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/environment.fixed.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:49:04.911809 linopy-0.2.3/benchmark/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/notebooks/plot-benchmarks.py.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:49:04.911809 linopy-0.2.3/benchmark/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1450 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/benchmark_cvxpy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1537 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/benchmark_gurobipy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1541 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/benchmark_jump.jl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1458 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/benchmark_linopy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2007 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/benchmark_ortools.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1796 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/benchmark_pulp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2043 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/benchmark_pyomo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:49:04.911809 linopy-0.2.3/benchmark/scripts/benchmarks-pypsa-eur/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/benchmarks-pypsa-eur/benchmark-linopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/benchmarks-pypsa-eur/benchmark-pyomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/benchmarks-pypsa-eur/benchmark-pypsa-linopf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/benchmarks-pypsa-eur/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/benchmarks-pypsa-eur/plot-benchmarks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      469 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1050 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/concat-benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:49:04.911809 linopy-0.2.3/benchmark/scripts/leftovers/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/leftovers/benchmark-linopy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:49:04.915809 linopy-0.2.3/benchmark/scripts/leftovers/benchmarks-pypsa-eur/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:49:04.915809 linopy-0.2.3/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-linopy.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pyomo.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pypsa-linopf.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/plot-benchmarks.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-linopy-pypsa-eur.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-linopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103087 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pyomo-pypsa-eur.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pyomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26681 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur-with-pypsa.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    18332 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-linopf.py
+-rw-r--r--   0 runner    (1001) docker     (123)   381819 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa_linopf-pypsa-eur.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/leftovers/benchmarks-pypsa-eur/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/leftovers/benchmarks-pypsa-eur/plot-benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/leftovers/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1392 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/merge-benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/plot-benchmarks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/run-cvxpy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/run-gurobipy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      399 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/run-linopy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      290 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/run-ortools.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      287 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/run-pulp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      399 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/run-pyomo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-07-28 09:48:55.000000 linopy-0.2.3/benchmark/scripts/write-lp-file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:49:04.919808 linopy-0.2.3/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-28 09:48:55.000000 linopy-0.2.3/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:49:04.919808 linopy-0.2.3/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-28 09:48:55.000000 linopy-0.2.3/doc/_static/theme_overrides.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-28 09:48:55.000000 linopy-0.2.3/doc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    57997 2023-07-28 09:48:55.000000 linopy-0.2.3/doc/benchmark.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-28 09:48:55.000000 linopy-0.2.3/doc/benchmark.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-28 09:48:55.000000 linopy-0.2.3/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-28 09:48:55.000000 linopy-0.2.3/doc/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 09:48:55.000000 linopy-0.2.3/doc/create-a-model-with-coordinates.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-28 09:48:55.000000 linopy-0.2.3/doc/create-a-model.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-28 09:48:55.000000 linopy-0.2.3/doc/creating-constraints.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-28 09:48:55.000000 linopy-0.2.3/doc/creating-expressions.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-28 09:48:55.000000 linopy-0.2.3/doc/creating-variables.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-28 09:48:55.000000 linopy-0.2.3/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-28 09:48:55.000000 linopy-0.2.3/doc/infeasible-model.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-07-28 09:48:55.000000 linopy-0.2.3/doc/logo.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    49959 2023-07-28 09:48:55.000000 linopy-0.2.3/doc/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-28 09:48:55.000000 linopy-0.2.3/doc/logo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-28 09:48:55.000000 linopy-0.2.3/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-28 09:48:55.000000 linopy-0.2.3/doc/manipulating-models.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-28 09:48:55.000000 linopy-0.2.3/doc/migrating-from-pyomo.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-28 09:48:55.000000 linopy-0.2.3/doc/prerequisites.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    20635 2023-07-28 09:48:55.000000 linopy-0.2.3/doc/release_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 09:48:55.000000 linopy-0.2.3/doc/solve-on-remote.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-28 09:48:55.000000 linopy-0.2.3/doc/syntax.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-28 09:48:55.000000 linopy-0.2.3/doc/testing-framework.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-28 09:48:55.000000 linopy-0.2.3/doc/user-guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:49:04.919808 linopy-0.2.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-07-28 09:48:55.000000 linopy-0.2.3/examples/create-a-model-with-coordinates.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-07-28 09:48:55.000000 linopy-0.2.3/examples/create-a-model.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-07-28 09:48:55.000000 linopy-0.2.3/examples/creating-constraints.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-07-28 09:48:55.000000 linopy-0.2.3/examples/creating-expressions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    16957 2023-07-28 09:48:55.000000 linopy-0.2.3/examples/creating-variables.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-28 09:48:55.000000 linopy-0.2.3/examples/infeasible-model.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-07-28 09:48:55.000000 linopy-0.2.3/examples/manipulating-models.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-28 09:48:55.000000 linopy-0.2.3/examples/migrating-from-pyomo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    26407 2023-07-28 09:48:55.000000 linopy-0.2.3/examples/solve-on-remote.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-28 09:48:55.000000 linopy-0.2.3/examples/testing-framework.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:49:04.923808 linopy-0.2.3/linopy/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-28 09:48:55.000000 linopy-0.2.3/linopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12779 2023-07-28 09:48:55.000000 linopy-0.2.3/linopy/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-28 09:48:55.000000 linopy-0.2.3/linopy/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-28 09:48:55.000000 linopy-0.2.3/linopy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30484 2023-07-28 09:48:55.000000 linopy-0.2.3/linopy/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49457 2023-07-28 09:48:55.000000 linopy-0.2.3/linopy/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-07-28 09:48:55.000000 linopy-0.2.3/linopy/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-28 09:48:55.000000 linopy-0.2.3/linopy/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38423 2023-07-28 09:48:55.000000 linopy-0.2.3/linopy/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-28 09:48:55.000000 linopy-0.2.3/linopy/monkey_patch_xarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-07-28 09:48:55.000000 linopy-0.2.3/linopy/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20119 2023-07-28 09:48:55.000000 linopy-0.2.3/linopy/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-28 09:48:55.000000 linopy-0.2.3/linopy/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37311 2023-07-28 09:48:55.000000 linopy-0.2.3/linopy/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-28 09:49:04.000000 linopy-0.2.3/linopy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:49:04.923808 linopy-0.2.3/linopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-07-28 09:49:04.000000 linopy-0.2.3/linopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-07-28 09:49:04.000000 linopy-0.2.3/linopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 09:49:04.000000 linopy-0.2.3/linopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-28 09:49:04.000000 linopy-0.2.3/linopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 09:49:04.000000 linopy-0.2.3/linopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-28 09:48:55.000000 linopy-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 09:49:04.923808 linopy-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-28 09:48:55.000000 linopy-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:49:04.923808 linopy-0.2.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-07-28 09:48:55.000000 linopy-0.2.3/test/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-07-28 09:48:55.000000 linopy-0.2.3/test/test_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-28 09:48:55.000000 linopy-0.2.3/test/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-28 09:48:55.000000 linopy-0.2.3/test/test_inconsistency_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-28 09:48:55.000000 linopy-0.2.3/test/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18190 2023-07-28 09:48:55.000000 linopy-0.2.3/test/test_linear_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-28 09:48:55.000000 linopy-0.2.3/test/test_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-28 09:48:55.000000 linopy-0.2.3/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15195 2023-07-28 09:48:55.000000 linopy-0.2.3/test/test_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-28 09:48:55.000000 linopy-0.2.3/test/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-07-28 09:48:55.000000 linopy-0.2.3/test/test_quadratic_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-07-28 09:48:55.000000 linopy-0.2.3/test/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-28 09:48:55.000000 linopy-0.2.3/test/test_scalar_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-28 09:48:55.000000 linopy-0.2.3/test/test_scalar_linear_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-07-28 09:48:55.000000 linopy-0.2.3/test/test_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-07-28 09:48:55.000000 linopy-0.2.3/test/test_variable_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-28 09:48:55.000000 linopy-0.2.3/test/test_variables.py
```

### Comparing `linopy-0.2.2/.coverage` & `linopy-0.2.3/.coverage`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/.github/workflows/CI.yaml` & `linopy-0.2.3/.github/workflows/CI.yaml`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/.github/workflows/deploy.yml` & `linopy-0.2.3/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/.pre-commit-config.yaml` & `linopy-0.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/LICENSE.txt` & `linopy-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/PKG-INFO` & `linopy-0.2.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linopy
-Version: 0.2.2
+Version: 0.2.3
 Summary: Linear optimization with N-D labeled arrays in Python
 Home-page: https://github.com/PyPSA/linopy
 Author: Fabian Hofmann
 Author-email: hofmann@fias.uni-frankfurt.de
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -65,15 +65,38 @@
 * [HiGHS](https://www.maths.ed.ac.uk/hall/HiGHS/)
 * [Gurobi](https://www.gurobi.com/)
 * [Xpress](https://www.fico.com/en/products/fico-xpress-solver)
 * [Cplex](https://www.ibm.com/de-de/analytics/cplex-optimizer)
 
 Note that these do have to be installed by the user separately.
 
+## Citing Linopy
 
-# License
+If you use Linopy in your research, please cite the following paper:
+
+- Hofmann, F., (2023). Linopy: Linear optimization with n-dimensional labeled variables.
+Journal of Open Source Software, 8(84), 4823, [https://doi.org/10.21105/joss.04823](https://doi.org/10.21105/joss.04823)
+
+A BibTeX entry for LaTeX users is
+
+```latex
+@article{Hofmann2023,
+    doi = {10.21105/joss.04823},
+    url = {https://doi.org/10.21105/joss.04823},
+    year = {2023}, publisher = {The Open Journal},
+    volume = {8},
+    number = {84},
+    pages = {4823},
+    author = {Fabian Hofmann},
+    title = {Linopy: Linear optimization with n-dimensional labeled variables},
+    journal = {Journal of Open Source Software}
+}
+```
+
+
+## License
 
 Copyright 2021 Fabian Hofmann
 
 
 
 This package is published under MIT license. See [LICENSE.txt](LICENSE.txt) for details.
```

### Comparing `linopy-0.2.2/README.md` & `linopy-0.2.3/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -44,15 +44,38 @@
 * [HiGHS](https://www.maths.ed.ac.uk/hall/HiGHS/)
 * [Gurobi](https://www.gurobi.com/)
 * [Xpress](https://www.fico.com/en/products/fico-xpress-solver)
 * [Cplex](https://www.ibm.com/de-de/analytics/cplex-optimizer)
 
 Note that these do have to be installed by the user separately.
 
+## Citing Linopy
 
-# License
+If you use Linopy in your research, please cite the following paper:
+
+- Hofmann, F., (2023). Linopy: Linear optimization with n-dimensional labeled variables.
+Journal of Open Source Software, 8(84), 4823, [https://doi.org/10.21105/joss.04823](https://doi.org/10.21105/joss.04823)
+
+A BibTeX entry for LaTeX users is
+
+```latex
+@article{Hofmann2023,
+    doi = {10.21105/joss.04823},
+    url = {https://doi.org/10.21105/joss.04823},
+    year = {2023}, publisher = {The Open Journal},
+    volume = {8},
+    number = {84},
+    pages = {4823},
+    author = {Fabian Hofmann},
+    title = {Linopy: Linear optimization with n-dimensional labeled variables},
+    journal = {Journal of Open Source Software}
+}
+```
+
+
+## License
 
 Copyright 2021 Fabian Hofmann
 
 
 
 This package is published under MIT license. See [LICENSE.txt](LICENSE.txt) for details.
```

### Comparing `linopy-0.2.2/benchmark/README.md` & `linopy-0.2.3/benchmark/README.md`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/Snakefile` & `linopy-0.2.3/benchmark/Snakefile`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/benchmark-absolute.pdf` & `linopy-0.2.3/benchmark/benchmark-absolute.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/benchmark-absolute.png` & `linopy-0.2.3/benchmark/benchmark-absolute.png`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/benchmark-overhead.pdf` & `linopy-0.2.3/benchmark/benchmark-overhead.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/benchmark-overhead.png` & `linopy-0.2.3/benchmark/benchmark-overhead.png`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/benchmark_resource-absolute.pdf` & `linopy-0.2.3/benchmark/benchmark_resource-absolute.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/benchmark_resource-absolute.png` & `linopy-0.2.3/benchmark/benchmark_resource-absolute.png`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/benchmark_resource-overhead.pdf` & `linopy-0.2.3/benchmark/benchmark_resource-overhead.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/benchmark_resource-overhead.png` & `linopy-0.2.3/benchmark/benchmark_resource-overhead.png`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/environment.fixed.yaml` & `linopy-0.2.3/benchmark/environment.fixed.yaml`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/notebooks/plot-benchmarks.py.ipynb` & `linopy-0.2.3/benchmark/notebooks/plot-benchmarks.py.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/scripts/benchmark_cvxpy.py` & `linopy-0.2.3/benchmark/scripts/benchmark_cvxpy.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/scripts/benchmark_gurobipy.py` & `linopy-0.2.3/benchmark/scripts/benchmark_gurobipy.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/scripts/benchmark_jump.jl` & `linopy-0.2.3/benchmark/scripts/benchmark_jump.jl`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/scripts/benchmark_linopy.py` & `linopy-0.2.3/benchmark/scripts/benchmark_linopy.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/scripts/benchmark_ortools.py` & `linopy-0.2.3/benchmark/scripts/benchmark_ortools.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/scripts/benchmark_pulp.py` & `linopy-0.2.3/benchmark/scripts/benchmark_pulp.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/scripts/benchmark_pyomo.py` & `linopy-0.2.3/benchmark/scripts/benchmark_pyomo.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/scripts/benchmarks-pypsa-eur/plot-benchmarks.py` & `linopy-0.2.3/benchmark/scripts/benchmarks-pypsa-eur/plot-benchmarks.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/scripts/concat-benchmarks.py` & `linopy-0.2.3/benchmark/scripts/concat-benchmarks.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/scripts/leftovers/benchmark-linopy.py` & `linopy-0.2.3/benchmark/scripts/leftovers/benchmark-linopy.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-linopy.cpython-310.pyc` & `linopy-0.2.3/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-linopy.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pyomo.cpython-310.pyc` & `linopy-0.2.3/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pyomo.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pypsa-linopf.cpython-310.pyc` & `linopy-0.2.3/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pypsa-linopf.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/plot-benchmarks.cpython-310.pyc` & `linopy-0.2.3/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/plot-benchmarks.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-linopy-pypsa-eur.dat` & `linopy-0.2.3/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-linopy-pypsa-eur.dat`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pyomo-pypsa-eur.dat` & `linopy-0.2.3/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pyomo-pypsa-eur.dat`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur-with-pypsa.pdf` & `linopy-0.2.3/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur-with-pypsa.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur.pdf` & `linopy-0.2.3/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa_linopf-pypsa-eur.dat` & `linopy-0.2.3/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa_linopf-pypsa-eur.dat`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/plot-benchmarks.py` & `linopy-0.2.3/benchmark/scripts/leftovers/benchmarks-pypsa-eur/plot-benchmarks.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/scripts/leftovers/common.py` & `linopy-0.2.3/benchmark/scripts/leftovers/common.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/scripts/merge-benchmarks.py` & `linopy-0.2.3/benchmark/scripts/merge-benchmarks.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/scripts/plot-benchmarks.py` & `linopy-0.2.3/benchmark/scripts/plot-benchmarks.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/benchmark/scripts/write-lp-file.py` & `linopy-0.2.3/benchmark/scripts/write-lp-file.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/doc/Makefile` & `linopy-0.2.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/doc/_static/theme_overrides.css` & `linopy-0.2.3/doc/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/doc/api.rst` & `linopy-0.2.3/doc/api.rst`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/doc/benchmark.png` & `linopy-0.2.3/doc/benchmark.png`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/doc/benchmark.rst` & `linopy-0.2.3/doc/benchmark.rst`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/doc/conf.py` & `linopy-0.2.3/doc/conf.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/doc/contributing.rst` & `linopy-0.2.3/doc/contributing.rst`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/doc/logo.pdf` & `linopy-0.2.3/doc/logo.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/doc/logo.png` & `linopy-0.2.3/doc/logo.png`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/doc/logo.py` & `linopy-0.2.3/doc/logo.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/doc/make.bat` & `linopy-0.2.3/doc/make.bat`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/doc/prerequisites.rst` & `linopy-0.2.3/doc/prerequisites.rst`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/doc/release_notes.rst` & `linopy-0.2.3/doc/release_notes.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 Release Notes
 =============
 
 .. Upcoming Release
 .. ----------------
 
+
+Version 0.2.1
+-------------
+
+**Bugfixes**
+
+* When multiplying a `LinearExpression` with a constant value, the constant in the `LinearExpression` was not updated. This is fixed now.
+
+**New Features**
+
+* The `Variable` and the `LinearExpression` have a new method `cumsum`, which allows to compute the cumulative sum.
+
 Version 0.2.1
 -------------
 
 
 * The documentation was revised and extended.
 * A new function `print_labels` was added to the `Variables` and `Constraints` class. This function allows to print the variables/constraints from a list of labels.
 * A new function `compute_infeasibilities` and `print_infeasibilities` was added to the `Model` class. This function allows to compute the infeasibilities of an infeasible model and print them out. The function only supports the `gurobi` solver so far.
```

### Comparing `linopy-0.2.2/doc/syntax.rst` & `linopy-0.2.3/doc/syntax.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Syntax comparison
 =================
 
 In order to compare the syntax between different API's, let's initialize the following problem in the different API's:
 
 .. math::
 
-    & \min \;\; \sum_{i,j} 2 x_{i,j} \; y_{i,j} \\
+    & \min \;\; \sum_{i,j} 2 x_{i,j} + \; y_{i,j} \\
     s.t. & \\
     & x_{i,j} - y_{i,j} \; \ge \; i \qquad \forall \; i,j \in \{1,...,N\} \\
     & x_{i,j} + y_{i,j} \; \ge \; 0 \qquad \forall \; i,j \in \{1,...,N\}
```

### Comparing `linopy-0.2.2/doc/user-guide.rst` & `linopy-0.2.3/doc/user-guide.rst`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/examples/create-a-model-with-coordinates.ipynb` & `linopy-0.2.3/examples/create-a-model-with-coordinates.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/examples/create-a-model.ipynb` & `linopy-0.2.3/examples/create-a-model.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/examples/creating-constraints.ipynb` & `linopy-0.2.3/examples/creating-constraints.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/examples/creating-expressions.ipynb` & `linopy-0.2.3/examples/creating-expressions.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/examples/creating-variables.ipynb` & `linopy-0.2.3/examples/creating-variables.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/examples/infeasible-model.ipynb` & `linopy-0.2.3/examples/infeasible-model.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/examples/manipulating-models.ipynb` & `linopy-0.2.3/examples/manipulating-models.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/examples/migrating-from-pyomo.ipynb` & `linopy-0.2.3/examples/migrating-from-pyomo.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/examples/solve-on-remote.ipynb` & `linopy-0.2.3/examples/solve-on-remote.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/examples/testing-framework.ipynb` & `linopy-0.2.3/examples/testing-framework.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/linopy/__init__.py` & `linopy-0.2.3/linopy/__init__.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/linopy/common.py` & `linopy-0.2.3/linopy/common.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/linopy/config.py` & `linopy-0.2.3/linopy/config.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/linopy/constants.py` & `linopy-0.2.3/linopy/constants.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/linopy/constraints.py` & `linopy-0.2.3/linopy/constraints.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/linopy/expressions.py` & `linopy-0.2.3/linopy/expressions.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,26 +7,27 @@
 """
 
 import functools
 import logging
 import warnings
 from dataclasses import dataclass, field
 from itertools import product, zip_longest
-from typing import Any, Mapping, Union
+from typing import Any, Mapping, Optional, Union
 
 import numpy as np
 import pandas as pd
 import xarray as xr
 import xarray.core.groupby
 import xarray.core.rolling
 from deprecation import deprecated
 from numpy import arange, array, nan
 from scipy.sparse import csc_matrix
 from xarray import DataArray, Dataset
 from xarray.core.dataarray import DataArrayCoordinates
+from xarray.core.types import Dims
 
 from linopy import constraints, expressions, variables
 from linopy.common import (
     LocIndexer,
     as_dataarray,
     check_common_keys_values,
     fill_missing_coords,
@@ -428,19 +429,19 @@
         if type(other) is LinearExpression:
             if other.nterm > 1:
                 raise TypeError("Multiplication of multiple terms is not supported.")
             ds = other.data[["coeffs", "vars"]].sel(_term=0).broadcast_like(self.data)
             ds = ds.assign(const=other.const)
             return merge(self, ds, dim=FACTOR_DIM, cls=QuadraticExpression)
         else:
-            coeffs = self.coeffs * as_dataarray(
-                other, coords=self.coords, dims=self.coord_dims
-            )
+            multiplyer = as_dataarray(other, coords=self.coords, dims=self.coord_dims)
+            coeffs = self.coeffs * multiplyer
             assert set(coeffs.shape) == set(self.coeffs.shape)
-            return self.assign(coeffs=coeffs)
+            const = self.const * multiplyer
+            return self.assign(coeffs=coeffs, const=const)
 
     def __rmul__(self, other):
         """
         Right-multiply the expr by a factor.
         """
         return self.__mul__(other)
 
@@ -582,14 +583,62 @@
         res = self.__class__(self._sum(self, dims=dims), self.model)
 
         if drop_zeros:
             res = res.densify_terms()
 
         return res
 
+    def cumsum(
+        self,
+        dim: Dims = None,
+        *,
+        skipna: Optional[bool] = None,
+        keep_attrs: Optional[bool] = None,
+        **kwargs: Any,
+    ) -> "LinearExpression":
+        """
+        Cumulated sum along a given axis.
+
+        Docstring and arguments are borrowed from `xarray.Dataset.cumsum`
+
+        Parameters
+        ----------
+        dim : str, Iterable of Hashable, "..." or None, default: None
+            Name of dimension[s] along which to apply ``cumsum``. For e.g. ``dim="x"``
+            or ``dim=["x", "y"]``. If "..." or None, will reduce over all dimensions.
+        skipna : bool or None, optional
+            If True, skip missing values (as marked by NaN). By default, only
+            skips missing values for float dtypes; other dtypes either do not
+            have a sentinel missing value (int) or ``skipna=True`` has not been
+            implemented (object, datetime64 or timedelta64).
+        keep_attrs : bool or None, optional
+            If True, ``attrs`` will be copied from the original
+            object to the new one.  If False, the new object will be
+            returned without attributes.
+        **kwargs : Any
+            Additional keyword arguments passed on to the appropriate array
+            function for calculating ``cumsum`` on this object's data.
+            These could include dask-specific kwargs like ``split_every``.
+
+        Returns
+        -------
+        linopy.expression.LinearExpression
+        """
+        # Along every dimensions, we want to perform cumsum along, get the size of the
+        # dimension to pass that to self.rolling.
+        if not dim:
+            # If user did not specify a dimension to sum over, use all relevant
+            # dimensions
+            dim = self.coord_dims
+        if isinstance(dim, str):
+            # Make sure, single mentioned dimensions is handled correctly.
+            dim = [dim]
+        dim_dict = {dim_name: self.data.dims[dim_name] for dim_name in dim}
+        return self.rolling(dim=dim_dict).sum(keep_attrs=keep_attrs, skipna=skipna)
+
     @classmethod
     def from_tuples(cls, *tuples, model=None, chunk=None):
         """
         Create a linear expression by using tuples of coefficients and
         variables.
 
         The function internally checks that all variables in the tuples belong to the same
```

### Comparing `linopy-0.2.2/linopy/io.py` & `linopy-0.2.3/linopy/io.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/linopy/matrices.py` & `linopy-0.2.3/linopy/matrices.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/linopy/model.py` & `linopy-0.2.3/linopy/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1007,15 +1007,15 @@
 
         if len(available_solvers) == 0:
             raise RuntimeError("No solver installed.")
 
         if solver_name is None:
             solver_name = available_solvers[0]
 
-        logger.info(f" Solve linear problem using {solver_name.title()} solver")
+        logger.info(f" Solve problem using {solver_name.title()} solver")
         assert solver_name in available_solvers, f"Solver {solver_name} not installed"
 
         # reset result
         self.reset_solution()
 
         if log_fn is not None:
             logger.info(f"Solver logs written to `{log_fn}`.")
```

### Comparing `linopy-0.2.2/linopy/monkey_patch_xarray.py` & `linopy-0.2.3/linopy/monkey_patch_xarray.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/linopy/remote.py` & `linopy-0.2.3/linopy/remote.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/linopy/solvers.py` & `linopy-0.2.3/linopy/solvers.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/linopy/testing.py` & `linopy-0.2.3/linopy/testing.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/linopy/variables.py` & `linopy-0.2.3/linopy/variables.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 This module contains variable related definitions of the package.
 """
 
 import functools
 import logging
 from collections.abc import Iterable
 from dataclasses import dataclass, field
-from typing import Any, Dict, Mapping, Sequence, Union
+from typing import Any, Dict, Mapping, Optional, Sequence, Union
 from warnings import warn
 
 import dask
 import numpy as np
 import pandas as pd
 from deprecation import deprecated
 from numpy import floating, inf, issubdtype
 from xarray import DataArray, Dataset, align, broadcast, zeros_like
+from xarray.core.types import Dims
 
 import linopy.expressions as expressions
 from linopy.common import (
     LocIndexer,
     as_dataarray,
     fill_missing_coords,
     forward_as_properties,
@@ -411,14 +412,54 @@
         -------
         linopy.expression.LinearExpressionRolling
         """
         return self.to_linexpr().rolling(
             dim=dim, min_periods=min_periods, center=center, **window_kwargs
         )
 
+    def cumsum(
+        self,
+        dim: Dims = None,
+        *,
+        skipna: Optional[bool] = None,
+        keep_attrs: Optional[bool] = None,
+        **kwargs: Any,
+    ) -> "expressions.LinearExpression":
+        """
+        Cumulated sum along a given axis.
+
+        Docstring and arguments are borrowed from `xarray.Dataset.cumsum`
+
+        Parameters
+        ----------
+        dim : str, Iterable of Hashable, "..." or None, default: None
+            Name of dimension[s] along which to apply ``cumsum``. For e.g. ``dim="x"``
+            or ``dim=["x", "y"]``. If "..." or None, will reduce over all dimensions.
+        skipna : bool or None, optional
+            If True, skip missing values (as marked by NaN). By default, only
+            skips missing values for float dtypes; other dtypes either do not
+            have a sentinel missing value (int) or ``skipna=True`` has not been
+            implemented (object, datetime64 or timedelta64).
+        keep_attrs : bool or None, optional
+            If True, ``attrs`` will be copied from the original
+            object to the new one.  If False, the new object will be
+            returned without attributes.
+        **kwargs : Any
+            Additional keyword arguments passed on to the appropriate array
+            function for calculating ``cumsum`` on this object's data.
+            These could include dask-specific kwargs like ``split_every``.
+
+        Returns
+        -------
+        linopy.expression.LinearExpression
+        """
+        return self.to_linexpr().cumsum(
+            dim=dim, skipna=skipna, keep_attrs=keep_attrs, **kwargs
+        )
+
     @property
     def name(self):
         """
         Return the name of the variable.
         """
         return self.attrs["name"]
```

### Comparing `linopy-0.2.2/linopy.egg-info/PKG-INFO` & `linopy-0.2.3/linopy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linopy
-Version: 0.2.2
+Version: 0.2.3
 Summary: Linear optimization with N-D labeled arrays in Python
 Home-page: https://github.com/PyPSA/linopy
 Author: Fabian Hofmann
 Author-email: hofmann@fias.uni-frankfurt.de
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -65,15 +65,38 @@
 * [HiGHS](https://www.maths.ed.ac.uk/hall/HiGHS/)
 * [Gurobi](https://www.gurobi.com/)
 * [Xpress](https://www.fico.com/en/products/fico-xpress-solver)
 * [Cplex](https://www.ibm.com/de-de/analytics/cplex-optimizer)
 
 Note that these do have to be installed by the user separately.
 
+## Citing Linopy
 
-# License
+If you use Linopy in your research, please cite the following paper:
+
+- Hofmann, F., (2023). Linopy: Linear optimization with n-dimensional labeled variables.
+Journal of Open Source Software, 8(84), 4823, [https://doi.org/10.21105/joss.04823](https://doi.org/10.21105/joss.04823)
+
+A BibTeX entry for LaTeX users is
+
+```latex
+@article{Hofmann2023,
+    doi = {10.21105/joss.04823},
+    url = {https://doi.org/10.21105/joss.04823},
+    year = {2023}, publisher = {The Open Journal},
+    volume = {8},
+    number = {84},
+    pages = {4823},
+    author = {Fabian Hofmann},
+    title = {Linopy: Linear optimization with n-dimensional labeled variables},
+    journal = {Journal of Open Source Software}
+}
+```
+
+
+## License
 
 Copyright 2021 Fabian Hofmann
 
 
 
 This package is published under MIT license. See [LICENSE.txt](LICENSE.txt) for details.
```

### Comparing `linopy-0.2.2/linopy.egg-info/SOURCES.txt` & `linopy-0.2.3/linopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/setup.py` & `linopy-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/test/test_common.py` & `linopy-0.2.3/test/test_common.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/test/test_constraint.py` & `linopy-0.2.3/test/test_constraint.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/test/test_constraints.py` & `linopy-0.2.3/test/test_constraints.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/test/test_inconsistency_checks.py` & `linopy-0.2.3/test/test_inconsistency_checks.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/test/test_io.py` & `linopy-0.2.3/test/test_io.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/test/test_linear_expression.py` & `linopy-0.2.3/test/test_linear_expression.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,14 +178,21 @@
 
     expr = -x - 8 * y - 10
     assert isinstance(expr, LinearExpression)
     assert (expr.const == -10).all()
     assert expr.nterm == 2
 
 
+def test_linear_expression_with_constant_multiplication(m, x, y):
+    expr = x + 1
+    expr = expr * 10
+    assert isinstance(expr, LinearExpression)
+    assert (expr.const == 10).all()
+
+
 def test_linear_expression_multi_indexed(u):
     expr = 3 * u + 1 * u
     assert isinstance(expr, LinearExpression)
 
 
 def test_linear_expression_with_errors(m, x):
     with pytest.raises(TypeError):
@@ -442,14 +449,22 @@
     expr = 1 * v
     groups = pd.Series([1] * 10 + [2] * 10, index=v.indexes["dim_2"])
     groups.name = "dim_2"
     with pytest.raises(ValueError):
         grouped = expr.groupby(groups).sum()
 
 
+def test_linear_expression_groupby_with_series_false(v):
+    expr = 1 * v
+    groups = pd.Series([1] * 10 + [2] * 10, index=v.indexes["dim_2"])
+    groups.name = "dim_2"
+    with pytest.raises(ValueError):
+        grouped = expr.groupby(groups).sum()
+
+
 def test_linear_expression_groupby_with_dataframe(v):
     expr = 1 * v
     groups = pd.DataFrame(
         {"a": [1] * 10 + [2] * 10, "b": list(range(4)) * 5}, index=v.indexes["dim_2"]
     )
     grouped = expr.groupby(xr.DataArray(groups)).sum()
     index = pd.MultiIndex.from_frame(groups)
@@ -599,7 +614,20 @@
     renamed = expr.rename({"dim_0": "dim_5"})
     assert set(renamed.dims) == {"dim_1", "dim_5", TERM_DIM}
     assert renamed.nterm == 3
 
     renamed = expr.rename({"dim_0": "dim_1", "dim_1": "dim_2"})
     assert set(renamed.dims) == {"dim_1", "dim_2", TERM_DIM}
     assert renamed.nterm == 3
+
+
+@pytest.mark.parametrize("multiple", [1.0, 0.5, 2.0, 0.0])
+def test_cumsum(m, multiple):
+    # Test cumsum on variable x
+    var = m.variables["x"]
+    cumsum = (multiple * var).cumsum()
+    cumsum.nterm == 2
+
+    # Test cumsum on sum of variables
+    var = m.variables["x"] + m.variables["y"]
+    cumsum = (multiple * var).cumsum()
+    cumsum.nterm == 2
```

### Comparing `linopy-0.2.2/test/test_matrices.py` & `linopy-0.2.3/test/test_matrices.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/test/test_model.py` & `linopy-0.2.3/test/test_model.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/test/test_optimization.py` & `linopy-0.2.3/test/test_optimization.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/test/test_options.py` & `linopy-0.2.3/test/test_options.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/test/test_quadratic_expression.py` & `linopy-0.2.3/test/test_quadratic_expression.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/test/test_repr.py` & `linopy-0.2.3/test/test_repr.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/test/test_scalar_constraint.py` & `linopy-0.2.3/test/test_scalar_constraint.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/test/test_scalar_linear_expression.py` & `linopy-0.2.3/test/test_scalar_linear_expression.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/test/test_variable.py` & `linopy-0.2.3/test/test_variable.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/test/test_variable_assignment.py` & `linopy-0.2.3/test/test_variable_assignment.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2.2/test/test_variables.py` & `linopy-0.2.3/test/test_variables.py`

 * *Files identical despite different names*

