# Comparing `tmp/emc-pypi-2023.8.1.tar.gz` & `tmp/emc-pypi-2023.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emc-pypi-2023.8.1.tar", last modified: Thu Jul 27 21:29:00 2023, max compression
+gzip compressed data, was "emc-pypi-2023.8.2.tar", last modified: Thu Jul 27 22:28:46 2023, max compression
```

## Comparing `emc-pypi-2023.8.1.tar` & `emc-pypi-2023.8.2.tar`

### file list

```diff
@@ -1,377 +1,377 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.455956 emc-pypi-2023.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-27 21:29:00.455956 emc-pypi-2023.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.391955 emc-pypi-2023.8.1/emc_pypi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-27 21:29:00.000000 emc-pypi-2023.8.1/emc_pypi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-07-27 21:29:00.000000 emc-pypi-2023.8.1/emc_pypi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 21:29:00.000000 emc-pypi-2023.8.1/emc_pypi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 21:29:00.000000 emc-pypi-2023.8.1/emc_pypi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 21:29:00.000000 emc-pypi-2023.8.1/emc_pypi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.391955 emc-pypi-2023.8.1/pyemc/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.391955 emc-pypi-2023.8.1/pyemc/emc/
--rw-r--r--   0 runner    (1001) docker     (123)    47987 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/HISTORY
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/README
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.407955 emc-pypi-2023.8.1/pyemc/emc/bin/
--rw-r--r--   0 runner    (1001) docker     (123)  8243072 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/bin/emc_linux_x86_64
--rwxr-xr-x   0 runner    (1001) docker     (123)  5771456 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/bin/emc_macos
--rwxr-xr-x   0 runner    (1001) docker     (123)  5436928 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/bin/emc_win32.exe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.415955 emc-pypi-2023.8.1/pyemc/emc/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   919858 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/docs/emc.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.383955 emc-pypi-2023.8.1/pyemc/emc/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.387955 emc-pypi-2023.8.1/pyemc/emc/examples/setup/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.387955 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.415955 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/bulk/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/bulk/chemistry.esh
--rwxr-xr-x   0 runner    (1001) docker     (123)     2442 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/bulk/setup.esh
--rwxr-xr-x   0 runner    (1001) docker     (123)      652 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/bulk/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.387955 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.415955 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/charmm/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/charmm/chemistry.esh
--rwxr-xr-x   0 runner    (1001) docker     (123)      634 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/charmm/setup.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     2339 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/charmm/solution.esh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.415955 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/dpd/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/dpd/name.esh
--rwxr-xr-x   0 runner    (1001) docker     (123)      811 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/dpd/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.415955 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/generate/
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/generate/build.emc
--rwxr-xr-x   0 runner    (1001) docker     (123)     1347 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/generate/field.esh
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/generate/field.in
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/generate/field.prm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.415955 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/lj/
--rwxr-xr-x   0 runner    (1001) docker     (123)      468 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/lj/field.esh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.383955 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/opls/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.419955 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/opls/aa/
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/opls/aa/build.emc
--rw-r--r--   0 runner    (1001) docker     (123)   161701 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.data
--rw-r--r--   0 runner    (1001) docker     (123)    46813 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.emc.gz
--rwxr-xr-x   0 runner    (1001) docker     (123)     2341 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.esh
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.in
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.params
--rw-r--r--   0 runner    (1001) docker     (123)    16723 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.pdb.gz
--rw-r--r--   0 runner    (1001) docker     (123)     9520 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.psf.gz
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.vmd
--rwxr-xr-x   0 runner    (1001) docker     (123)      636 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/opls/aa/setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/opls/aa/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.419955 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/opls/ua/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2341 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/opls/ua/name.esh
--rwxr-xr-x   0 runner    (1001) docker     (123)      636 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/opls/ua/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.419955 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/opls/water/
--rwxr-xr-x   0 runner    (1001) docker     (123)      487 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/opls/water/water.esh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.419955 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/pcff/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2335 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/pcff/name.esh
--rwxr-xr-x   0 runner    (1001) docker     (123)      630 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/pcff/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.419955 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/trappe/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2339 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/trappe/name.esh
--rwxr-xr-x   0 runner    (1001) docker     (123)      634 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/trappe/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.419955 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/user/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1857 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/user/polymer.esh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.419955 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/multiphase/
--rwxr-xr-x   0 runner    (1001) docker     (123)      335 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/multiphase/multiphase.esh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.387955 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.419955 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/alternate/
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/alternate/build.emc
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/alternate/dpd.in
--rwxr-xr-x   0 runner    (1001) docker     (123)      413 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/alternate/polymer.esh
--rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/alternate/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.419955 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/biphase/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1357 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/biphase/polymer.esh
--rwxr-xr-x   0 runner    (1001) docker     (123)      779 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/biphase/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.419955 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/block/
--rwxr-xr-x   0 runner    (1001) docker     (123)      372 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/block/polymer.esh
--rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/block/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.419955 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/copolymer/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1534 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/copolymer/polymer.esh
--rwxr-xr-x   0 runner    (1001) docker     (123)      754 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/copolymer/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.419955 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/dendrimer/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1404 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/dendrimer/polymer.esh
--rwxr-xr-x   0 runner    (1001) docker     (123)      763 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/dendrimer/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.423956 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/homopolymer/
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/homopolymer/build.emc
--rwxr-xr-x   0 runner    (1001) docker     (123)     1450 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/homopolymer/polymer.esh
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/homopolymer/polymer.in
--rwxr-xr-x   0 runner    (1001) docker     (123)      768 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/homopolymer/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.423956 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/random/
--rwxr-xr-x   0 runner    (1001) docker     (123)      373 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/random/polymer.esh
--rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/random/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.423956 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/random_block/
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/random_block/block.in
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/random_block/block.prm
--rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/random_block/build.emc
--rwxr-xr-x   0 runner    (1001) docker     (123)      564 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/random_block/polymer.esh
--rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/random_block/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.423956 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/record/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1344 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/record/cat.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      697 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/record/exec.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      481 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/record/fullerene.esh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.423956 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/surface/
--rwxr-xr-x   0 runner    (1001) docker     (123)      140 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/surface/lammps.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      321 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/surface/lmp2pdb.emc
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/surface/setup.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      699 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/surface/surface.esh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.387955 emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.423956 emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/field/
--rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/field/README
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.387955 emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/field/chemistry/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.387955 emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/field/chemistry/field/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.423956 emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/field/chemistry/field/stage/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/field/chemistry/field/stage/lj.prm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.423956 emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/field/chemistry/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1768 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/field/chemistry/scripts/lj.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.387955 emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/field/chemistry/stages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.423956 emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/field/chemistry/stages/lj/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1483 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/field/chemistry/stages/lj/stage.esh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.423956 emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/field/setup/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1722 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/field/setup/lj.esh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.423956 emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/green-kubo/
--rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/green-kubo/viscosity.esh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.423956 emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/nemd/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1130 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/nemd/shear.esh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.423956 emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/t_glass/
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/t_glass/README
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.423956 emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/t_glass/setup/
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/t_glass/setup/2023072600.esh
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/t_glass/setup/2023072601.esh
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/t_glass/setup/2023072610.esh
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/t_glass/setup/2023072611.esh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.387955 emc-pypi-2023.8.1/pyemc/emc/field/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.387955 emc-pypi-2023.8.1/pyemc/emc/field/born/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.427955 emc-pypi-2023.8.1/pyemc/emc/field/born/2016/
--rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/born/2016/convert.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/born/2016/guillot.define
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/born/2016/guillot.prm
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/born/2016/guillot.top
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/born/2016/matsui.define
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/born/2016/matsui.prm
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/born/2016/matsui.top
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.427955 emc-pypi-2023.8.1/pyemc/emc/field/cff/
--rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/cff/al2o3.frc
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/cff/al2o3_templates.dat
--rw-r--r--   0 runner    (1001) docker     (123)    10526 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/cff/c3s.frc
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/cff/c3s_templates.dat
--rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/cff/caso4.frc
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/cff/caso4_templates.dat
--rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/cff/sio2.frc
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/cff/sio2_templates.dat
--rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/cff/template.frc
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/cff/template_templates.dat
--rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/cff/zno.frc
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/cff/zno_templates.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.387955 emc-pypi-2023.8.1/pyemc/emc/field/charmm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.431956 emc-pypi-2023.8.1/pyemc/emc/field/charmm/c36a/
--rw-r--r--   0 runner    (1001) docker     (123)    70528 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/charmm/c36a/carb.prm
--rw-r--r--   0 runner    (1001) docker     (123)     9810 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/charmm/c36a/carb.top
--rw-r--r--   0 runner    (1001) docker     (123)   260876 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/charmm/c36a/cgenff.prm
--rw-r--r--   0 runner    (1001) docker     (123)    51267 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/charmm/c36a/cgenff.top
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/charmm/c36a/ethers.prm
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/charmm/c36a/ethers.top
--rw-r--r--   0 runner    (1001) docker     (123)    25799 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/charmm/c36a/lipid.prm
--rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/charmm/c36a/lipid.top
--rw-r--r--   0 runner    (1001) docker     (123)    61430 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/charmm/c36a/na.prm
--rw-r--r--   0 runner    (1001) docker     (123)    44046 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/charmm/c36a/na.top
--rw-r--r--   0 runner    (1001) docker     (123)    76928 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/charmm/c36a/prot.prm
--rw-r--r--   0 runner    (1001) docker     (123)    10373 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/charmm/c36a/prot.top
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/charmm/c36a/water_ions.prm
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/charmm/c36a/water_ions.top
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.431956 emc-pypi-2023.8.1/pyemc/emc/field/dpd/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/dpd/general.prm
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/dpd/srp.prm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.431956 emc-pypi-2023.8.1/pyemc/emc/field/gauss/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/gauss/general.prm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.387955 emc-pypi-2023.8.1/pyemc/emc/field/martini/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.431956 emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/aminoacids.prm
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/cholesterol.prm
--rw-r--r--   0 runner    (1001) docker     (123)    13507 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/convert.out
--rwxr-xr-x   0 runner    (1001) docker     (123)      384 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/convert.sh
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/file.prm
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/ions.prm
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/lipids.prm
--rw-r--r--   0 runner    (1001) docker     (123)    49816 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/martini.prm
--rw-r--r--   0 runner    (1001) docker     (123)    13899 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/other.prm
--rw-r--r--   0 runner    (1001) docker     (123)    14807 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/polymers.prm
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/solvents.prm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.435956 emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/src/aminoacids.itp
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/src/cholesterol.itp
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/src/ions.itp
--rw-r--r--   0 runner    (1001) docker     (123)    28941 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/src/lipids.itp
--rw-r--r--   0 runner    (1001) docker     (123)    45704 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/src/martini.itp
--rw-r--r--   0 runner    (1001) docker     (123)    34302 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/src/other.itp
--rw-r--r--   0 runner    (1001) docker     (123)    13976 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/src/other.prm
--rw-r--r--   0 runner    (1001) docker     (123)   162621 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/src/polymers.itp
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/src/solvents.itp
--rw-r--r--   0 runner    (1001) docker     (123)    19001 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/src/sugars.itp
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/src/surfactants.itp
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/src/xemium.itp
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/sugars.prm
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/surfactants.prm
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/xemium.prm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.387955 emc-pypi-2023.8.1/pyemc/emc/field/opls/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.435956 emc-pypi-2023.8.1/pyemc/emc/field/opls/2012/
--rwxr-xr-x   0 runner    (1001) docker     (123)      102 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/opls/2012/convert.sh
--rw-r--r--   0 runner    (1001) docker     (123)    26118 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/opls/2012/opls-aa.define
--rw-r--r--   0 runner    (1001) docker     (123)    35717 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/opls/2012/opls-aa.prm
--rw-r--r--   0 runner    (1001) docker     (123)    30668 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/opls/2012/opls-aa.top
--rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/opls/2012/opls-ua.define
--rw-r--r--   0 runner    (1001) docker     (123)    29216 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/opls/2012/opls-ua.prm
--rw-r--r--   0 runner    (1001) docker     (123)    13150 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/opls/2012/opls-ua.top
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.435956 emc-pypi-2023.8.1/pyemc/emc/field/opls/2012/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/opls/2012/src/add.txt
--rw-r--r--   0 runner    (1001) docker     (123)   265526 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/opls/2012/src/oplsaa.par
--rw-r--r--   0 runner    (1001) docker     (123)    63470 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/opls/2012/src/oplsaa.sb
--rw-r--r--   0 runner    (1001) docker     (123)    58915 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/opls/2012/src/reoplsff.zip
--rwxr-xr-x   0 runner    (1001) docker     (123)      115 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/opls/2012/src/trim.pl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.435956 emc-pypi-2023.8.1/pyemc/emc/field/pcff/
--rw-r--r--   0 runner    (1001) docker     (123)   340414 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/pcff/pcff.frc
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/pcff/pcff.rlb
--rw-r--r--   0 runner    (1001) docker     (123)    39285 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/pcff/pcff_templates.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.439956 emc-pypi-2023.8.1/pyemc/emc/field/pcff_ore/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/pcff_ore/._pcff_ore.frc
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/pcff_ore/._pcff_ore_templates.dat
--rwxr-xr-x   0 runner    (1001) docker     (123)   403462 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/pcff_ore/pcff_ore.frc
--rwxr-xr-x   0 runner    (1001) docker     (123)    39216 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/pcff_ore/pcff_ore_templates.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.439956 emc-pypi-2023.8.1/pyemc/emc/field/polystyrene/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/polystyrene/README
--rw-r--r--   0 runner    (1001) docker     (123)    15648 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/polystyrene/smoothed_e-e.m
--rw-r--r--   0 runner    (1001) docker     (123)    15912 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/polystyrene/smoothed_m-e.m
--rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/polystyrene/smoothed_m-m.m
--rw-r--r--   0 runner    (1001) docker     (123)    15939 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/polystyrene/smoothed_m-r.m
--rw-r--r--   0 runner    (1001) docker     (123)    15662 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/polystyrene/smoothed_r-e.m
--rw-r--r--   0 runner    (1001) docker     (123)    15666 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/polystyrene/smoothed_r-r.m
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.387955 emc-pypi-2023.8.1/pyemc/emc/field/sdk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.439956 emc-pypi-2023.8.1/pyemc/emc/field/sdk/v1.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/sdk/v1.0/convert.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/sdk/v1.0/sdk.define
--rw-r--r--   0 runner    (1001) docker     (123)    16542 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/sdk/v1.0/sdk.prm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.439956 emc-pypi-2023.8.1/pyemc/emc/field/sdk/v1.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/sdk/v1.0/src/angle.dat
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/sdk/v1.0/src/bond.dat
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/sdk/v1.0/src/convert.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/sdk/v1.0/src/mass.dat
--rw-r--r--   0 runner    (1001) docker     (123)    11061 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/sdk/v1.0/src/pair.dat
--rw-r--r--   0 runner    (1001) docker     (123)    79940 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/sdk/v1.0/src/sdk.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/sdk/v1.0/src/torsion.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.387955 emc-pypi-2023.8.1/pyemc/emc/field/trappe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.443956 emc-pypi-2023.8.1/pyemc/emc/field/trappe/2014/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/trappe/2014/convert.emc
--rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/trappe/2014/convert.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      347 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/trappe/2014/e2k.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1444 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/trappe/2014/list.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3449 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/trappe/2014/torsions.pl
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/trappe/2014/torsions.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/trappe/2014/trappe-eh.define
--rw-r--r--   0 runner    (1001) docker     (123)    21631 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/trappe/2014/trappe-ua.define
--rw-r--r--   0 runner    (1001) docker     (123)    16562 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/trappe/2014/trappe-ua.define.old
--rw-r--r--   0 runner    (1001) docker     (123)   128013 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/trappe/2014/trappe-ua.field
--rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/trappe/2014/trappe-ua.prm
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/field/trappe/2014/trappe-ua.top
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.443956 emc-pypi-2023.8.1/pyemc/emc/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/modules/changes.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.451956 emc-pypi-2023.8.1/pyemc/emc/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.451956 emc-pypi-2023.8.1/pyemc/emc/scripts/analyze/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5852 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/analyze/cavity.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     3371 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/analyze/files.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     3276 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/analyze/harvest.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     3746 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/analyze/last.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     2984 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/analyze/project.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.451956 emc-pypi-2023.8.1/pyemc/emc/scripts/analyze/sample/
--rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/analyze/sample/bond.emc
--rwxr-xr-x   0 runner    (1001) docker     (123)      818 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/analyze/sample/cavity.emc
--rwxr-xr-x   0 runner    (1001) docker     (123)      581 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/analyze/sample/distance.emc
--rwxr-xr-x   0 runner    (1001) docker     (123)      641 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/analyze/sample/gr.emc
--rwxr-xr-x   0 runner    (1001) docker     (123)      622 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/analyze/sample/gyration.emc
--rwxr-xr-x   0 runner    (1001) docker     (123)     4272 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/analyze/script.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     8532 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/average.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1101 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/avg_error.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2340 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/change.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      992 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/change_header.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)    41097 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/charmm2lammps.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      479 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/clean_restart.pl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.451956 emc-pypi-2023.8.1/pyemc/emc/scripts/coding/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4139 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/coding/cpmod.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1255 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/coding/cpmoddir.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      670 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/coding/emc_comments.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2143 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/coding/emc_parse_oper.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)     4247 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/coding/header.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      881 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/coding/hold.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      443 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/coding/scrape.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1715 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/emc.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      312 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/emc2emc.emc
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/emc2energy.emc
--rwxr-xr-x   0 runner    (1001) docker     (123)      386 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/emc2insight.emc
--rwxr-xr-x   0 runner    (1001) docker     (123)      452 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/emc2lammps.emc
--rwxr-xr-x   0 runner    (1001) docker     (123)      550 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/emc2pdb.emc
--rwxr-xr-x   0 runner    (1001) docker     (123)      689 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/emc2volume.emc
--rwxr-xr-x   0 runner    (1001) docker     (123)      306 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/emc2xyz.emc
--rwxr-xr-x   0 runner    (1001) docker     (123)     5434 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/emc_align.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      613 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/emc_clean.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     5093 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/emc_error.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)    19538 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/emc_field.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)    18675 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/emc_generate.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)    32713 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/emc_martini.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)    35299 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/emc_opls.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)    29396 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/emc_sdk.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)   369774 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/emc_setup.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2871 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/emc_template.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)    20155 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/emc_trappe.pl
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/hold.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)    39906 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/insight2lammps.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      381 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/lammps2emc.emc
--rwxr-xr-x   0 runner    (1001) docker     (123)      488 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/lammps2lammps.emc
--rwxr-xr-x   0 runner    (1001) docker     (123)      825 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/lammps2pdb.emc
--rwxr-xr-x   0 runner    (1001) docker     (123)     4282 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/last.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.451956 emc-pypi-2023.8.1/pyemc/emc/scripts/modules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.451956 emc-pypi-2023.8.1/pyemc/emc/scripts/modules/Charmm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/modules/Charmm/Core
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/modules/Charmm/Global.pm
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/modules/Charmm.pm
--rw-r--r--   0 runner    (1001) docker     (123)    27706 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/modules/EMCField.pm
--rwxr-xr-x   0 runner    (1001) docker     (123)    18057 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/myjobs.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)    10303 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/openff.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      252 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/pack.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      312 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/pdb.emc
--rwxr-xr-x   0 runner    (1001) docker     (123)    17277 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/pdb_extract.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)     4116 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/prm_compare.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      999 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/prm_duplicate.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2591 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/prm_extract.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     8495 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/prm_list_types.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)     7094 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/prm_reduce.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      679 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/prm_reduce.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     5748 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/prm_search.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1575 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/psf_charge.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)     4929 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/replace.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)    18135 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/run.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      610 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/run_analyze.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     6648 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/run_host.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     3025 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/run_restart.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1744 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/run_stat.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/template.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      756 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/traject2pdb.emc
--rwxr-xr-x   0 runner    (1001) docker     (123)     3525 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/trj_reduce.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1105 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/try.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     4118 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/view_record.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     4632 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/view_vmd.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      274 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/scripts/xyz.emc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.455956 emc-pypi-2023.8.1/pyemc/emc/templates/
--rwxr-xr-x   0 runner    (1001) docker     (123)      347 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/templates/chemistry.esh
--rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/templates/cluster.esh
--rwxr-xr-x   0 runner    (1001) docker     (123)      837 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/templates/environment.esh
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/templates/field.define
--rwxr-xr-x   0 runner    (1001) docker     (123)      862 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/templates/field.esh
--rwxr-xr-x   0 runner    (1001) docker     (123)      395 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/templates/import.esh
--rwxr-xr-x   0 runner    (1001) docker     (123)      496 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/templates/polymer.esh
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/templates/restart.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.455956 emc-pypi-2023.8.1/pyemc/emc/vmd/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/vmd/README
--rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/vmd/license.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:29:00.455956 emc-pypi-2023.8.1/pyemc/emc/vmd/packages/
--rw-r--r--   0 runner    (1001) docker     (123)   299843 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/vmd/packages/gui.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    14504 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/vmd/packages/options.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/vmd/packages/textview.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/emc/vmd/packages.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/pyemc/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 21:29:00.455956 emc-pypi-2023.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-27 21:28:46.000000 emc-pypi-2023.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.984664 emc-pypi-2023.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-27 22:28:46.984664 emc-pypi-2023.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.896664 emc-pypi-2023.8.2/emc_pypi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-27 22:28:46.000000 emc-pypi-2023.8.2/emc_pypi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-07-27 22:28:46.000000 emc-pypi-2023.8.2/emc_pypi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 22:28:46.000000 emc-pypi-2023.8.2/emc_pypi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 22:28:46.000000 emc-pypi-2023.8.2/emc_pypi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 22:28:46.000000 emc-pypi-2023.8.2/emc_pypi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.896664 emc-pypi-2023.8.2/pyemc/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.896664 emc-pypi-2023.8.2/pyemc/emc/
+-rw-r--r--   0 runner    (1001) docker     (123)    47987 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/HISTORY
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/README
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.916664 emc-pypi-2023.8.2/pyemc/emc/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)  8243072 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/bin/emc_linux_x86_64
+-rwxr-xr-x   0 runner    (1001) docker     (123)  5771456 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/bin/emc_macos
+-rwxr-xr-x   0 runner    (1001) docker     (123)  5436928 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/bin/emc_win32.exe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.920664 emc-pypi-2023.8.2/pyemc/emc/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   919858 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/docs/emc.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.884663 emc-pypi-2023.8.2/pyemc/emc/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.888664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.888664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.924664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/bulk/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/bulk/chemistry.esh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2442 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/bulk/setup.esh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      652 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/bulk/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.888664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.924664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/charmm/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/charmm/chemistry.esh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      634 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/charmm/setup.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2339 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/charmm/solution.esh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.924664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/dpd/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/dpd/name.esh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      811 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/dpd/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.924664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/generate/build.emc
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1347 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/generate/field.esh
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/generate/field.in
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/generate/field.prm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.924664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/lj/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      468 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/lj/field.esh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.884663 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/opls/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.928664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/opls/aa/
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/opls/aa/build.emc
+-rw-r--r--   0 runner    (1001) docker     (123)   161701 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.data
+-rw-r--r--   0 runner    (1001) docker     (123)    46813 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.emc.gz
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2341 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.esh
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.params
+-rw-r--r--   0 runner    (1001) docker     (123)    16723 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.pdb.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     9520 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.psf.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.vmd
+-rwxr-xr-x   0 runner    (1001) docker     (123)      636 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/opls/aa/setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/opls/aa/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.928664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/opls/ua/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2341 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/opls/ua/name.esh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      636 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/opls/ua/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.928664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/opls/water/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      487 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/opls/water/water.esh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.928664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/pcff/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2335 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/pcff/name.esh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      630 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/pcff/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.932664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/trappe/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2339 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/trappe/name.esh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      634 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/trappe/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.932664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/user/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1857 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/user/polymer.esh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.932664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/multiphase/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      335 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/multiphase/multiphase.esh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.888664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.932664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/alternate/
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/alternate/build.emc
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/alternate/dpd.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)      413 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/alternate/polymer.esh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/alternate/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.932664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/biphase/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1357 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/biphase/polymer.esh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      779 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/biphase/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.932664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/block/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      372 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/block/polymer.esh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/block/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.932664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/copolymer/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1534 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/copolymer/polymer.esh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      754 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/copolymer/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.932664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/dendrimer/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1404 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/dendrimer/polymer.esh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      763 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/dendrimer/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.936664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/homopolymer/
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/homopolymer/build.emc
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1450 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/homopolymer/polymer.esh
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/homopolymer/polymer.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)      768 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/homopolymer/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.936664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/random/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      373 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/random/polymer.esh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/random/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.936664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/random_block/
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/random_block/block.in
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/random_block/block.prm
+-rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/random_block/build.emc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      564 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/random_block/polymer.esh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/random_block/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.936664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/record/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1344 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/record/cat.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      697 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/record/exec.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      481 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/record/fullerene.esh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.940664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/surface/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      140 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/surface/lammps.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      321 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/surface/lmp2pdb.emc
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/surface/setup.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      699 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/surface/surface.esh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.888664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.940664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/field/
+-rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/field/README
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.888664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/field/chemistry/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.888664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/field/chemistry/field/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.940664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/field/chemistry/field/stage/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/field/chemistry/field/stage/lj.prm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.940664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/field/chemistry/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1768 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/field/chemistry/scripts/lj.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.888664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/field/chemistry/stages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.940664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/field/chemistry/stages/lj/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1483 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/field/chemistry/stages/lj/stage.esh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.940664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/field/setup/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1722 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/field/setup/lj.esh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.940664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/green-kubo/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/green-kubo/viscosity.esh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.940664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/nemd/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1130 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/nemd/shear.esh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.940664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/t_glass/
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/t_glass/README
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.940664 emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/t_glass/setup/
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/t_glass/setup/2023072600.esh
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/t_glass/setup/2023072601.esh
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/t_glass/setup/2023072610.esh
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/t_glass/setup/2023072611.esh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.892664 emc-pypi-2023.8.2/pyemc/emc/field/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.888664 emc-pypi-2023.8.2/pyemc/emc/field/born/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.944664 emc-pypi-2023.8.2/pyemc/emc/field/born/2016/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/born/2016/convert.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/born/2016/guillot.define
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/born/2016/guillot.prm
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/born/2016/guillot.top
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/born/2016/matsui.define
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/born/2016/matsui.prm
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/born/2016/matsui.top
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.944664 emc-pypi-2023.8.2/pyemc/emc/field/cff/
+-rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/cff/al2o3.frc
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/cff/al2o3_templates.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    10526 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/cff/c3s.frc
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/cff/c3s_templates.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/cff/caso4.frc
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/cff/caso4_templates.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/cff/sio2.frc
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/cff/sio2_templates.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/cff/template.frc
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/cff/template_templates.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/cff/zno.frc
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/cff/zno_templates.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.888664 emc-pypi-2023.8.2/pyemc/emc/field/charmm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.948664 emc-pypi-2023.8.2/pyemc/emc/field/charmm/c36a/
+-rw-r--r--   0 runner    (1001) docker     (123)    70528 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/charmm/c36a/carb.prm
+-rw-r--r--   0 runner    (1001) docker     (123)     9810 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/charmm/c36a/carb.top
+-rw-r--r--   0 runner    (1001) docker     (123)   260876 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/charmm/c36a/cgenff.prm
+-rw-r--r--   0 runner    (1001) docker     (123)    51267 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/charmm/c36a/cgenff.top
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/charmm/c36a/ethers.prm
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/charmm/c36a/ethers.top
+-rw-r--r--   0 runner    (1001) docker     (123)    25799 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/charmm/c36a/lipid.prm
+-rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/charmm/c36a/lipid.top
+-rw-r--r--   0 runner    (1001) docker     (123)    61430 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/charmm/c36a/na.prm
+-rw-r--r--   0 runner    (1001) docker     (123)    44046 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/charmm/c36a/na.top
+-rw-r--r--   0 runner    (1001) docker     (123)    76928 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/charmm/c36a/prot.prm
+-rw-r--r--   0 runner    (1001) docker     (123)    10373 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/charmm/c36a/prot.top
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/charmm/c36a/water_ions.prm
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/charmm/c36a/water_ions.top
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.948664 emc-pypi-2023.8.2/pyemc/emc/field/dpd/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/dpd/general.prm
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/dpd/srp.prm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.948664 emc-pypi-2023.8.2/pyemc/emc/field/gauss/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/gauss/general.prm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.888664 emc-pypi-2023.8.2/pyemc/emc/field/martini/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.952664 emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/aminoacids.prm
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/cholesterol.prm
+-rw-r--r--   0 runner    (1001) docker     (123)    13507 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/convert.out
+-rwxr-xr-x   0 runner    (1001) docker     (123)      384 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/convert.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/file.prm
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/ions.prm
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/lipids.prm
+-rw-r--r--   0 runner    (1001) docker     (123)    49816 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/martini.prm
+-rw-r--r--   0 runner    (1001) docker     (123)    13899 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/other.prm
+-rw-r--r--   0 runner    (1001) docker     (123)    14807 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/polymers.prm
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/solvents.prm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.956664 emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/src/aminoacids.itp
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/src/cholesterol.itp
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/src/ions.itp
+-rw-r--r--   0 runner    (1001) docker     (123)    28941 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/src/lipids.itp
+-rw-r--r--   0 runner    (1001) docker     (123)    45704 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/src/martini.itp
+-rw-r--r--   0 runner    (1001) docker     (123)    34302 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/src/other.itp
+-rw-r--r--   0 runner    (1001) docker     (123)    13976 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/src/other.prm
+-rw-r--r--   0 runner    (1001) docker     (123)   162621 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/src/polymers.itp
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/src/solvents.itp
+-rw-r--r--   0 runner    (1001) docker     (123)    19001 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/src/sugars.itp
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/src/surfactants.itp
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/src/xemium.itp
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/sugars.prm
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/surfactants.prm
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/xemium.prm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.892664 emc-pypi-2023.8.2/pyemc/emc/field/opls/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.960664 emc-pypi-2023.8.2/pyemc/emc/field/opls/2012/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      102 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/opls/2012/convert.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    26118 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/opls/2012/opls-aa.define
+-rw-r--r--   0 runner    (1001) docker     (123)    35717 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/opls/2012/opls-aa.prm
+-rw-r--r--   0 runner    (1001) docker     (123)    30668 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/opls/2012/opls-aa.top
+-rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/opls/2012/opls-ua.define
+-rw-r--r--   0 runner    (1001) docker     (123)    29216 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/opls/2012/opls-ua.prm
+-rw-r--r--   0 runner    (1001) docker     (123)    13150 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/opls/2012/opls-ua.top
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.960664 emc-pypi-2023.8.2/pyemc/emc/field/opls/2012/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/opls/2012/src/add.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   265526 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/opls/2012/src/oplsaa.par
+-rw-r--r--   0 runner    (1001) docker     (123)    63470 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/opls/2012/src/oplsaa.sb
+-rw-r--r--   0 runner    (1001) docker     (123)    58915 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/opls/2012/src/reoplsff.zip
+-rwxr-xr-x   0 runner    (1001) docker     (123)      115 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/opls/2012/src/trim.pl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.960664 emc-pypi-2023.8.2/pyemc/emc/field/pcff/
+-rw-r--r--   0 runner    (1001) docker     (123)   340414 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/pcff/pcff.frc
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/pcff/pcff.rlb
+-rw-r--r--   0 runner    (1001) docker     (123)    39285 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/pcff/pcff_templates.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.964664 emc-pypi-2023.8.2/pyemc/emc/field/pcff_ore/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/pcff_ore/._pcff_ore.frc
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/pcff_ore/._pcff_ore_templates.dat
+-rwxr-xr-x   0 runner    (1001) docker     (123)   403462 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/pcff_ore/pcff_ore.frc
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39216 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/pcff_ore/pcff_ore_templates.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.964664 emc-pypi-2023.8.2/pyemc/emc/field/polystyrene/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/polystyrene/README
+-rw-r--r--   0 runner    (1001) docker     (123)    15648 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/polystyrene/smoothed_e-e.m
+-rw-r--r--   0 runner    (1001) docker     (123)    15912 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/polystyrene/smoothed_m-e.m
+-rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/polystyrene/smoothed_m-m.m
+-rw-r--r--   0 runner    (1001) docker     (123)    15939 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/polystyrene/smoothed_m-r.m
+-rw-r--r--   0 runner    (1001) docker     (123)    15662 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/polystyrene/smoothed_r-e.m
+-rw-r--r--   0 runner    (1001) docker     (123)    15666 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/polystyrene/smoothed_r-r.m
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.892664 emc-pypi-2023.8.2/pyemc/emc/field/sdk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.964664 emc-pypi-2023.8.2/pyemc/emc/field/sdk/v1.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/sdk/v1.0/convert.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/sdk/v1.0/sdk.define
+-rw-r--r--   0 runner    (1001) docker     (123)    16542 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/sdk/v1.0/sdk.prm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.968664 emc-pypi-2023.8.2/pyemc/emc/field/sdk/v1.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/sdk/v1.0/src/angle.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/sdk/v1.0/src/bond.dat
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/sdk/v1.0/src/convert.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/sdk/v1.0/src/mass.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    11061 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/sdk/v1.0/src/pair.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    79940 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/sdk/v1.0/src/sdk.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/sdk/v1.0/src/torsion.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.892664 emc-pypi-2023.8.2/pyemc/emc/field/trappe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.968664 emc-pypi-2023.8.2/pyemc/emc/field/trappe/2014/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/trappe/2014/convert.emc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/trappe/2014/convert.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      347 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/trappe/2014/e2k.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1444 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/trappe/2014/list.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3449 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/trappe/2014/torsions.pl
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/trappe/2014/torsions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/trappe/2014/trappe-eh.define
+-rw-r--r--   0 runner    (1001) docker     (123)    21631 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/trappe/2014/trappe-ua.define
+-rw-r--r--   0 runner    (1001) docker     (123)    16562 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/trappe/2014/trappe-ua.define.old
+-rw-r--r--   0 runner    (1001) docker     (123)   128013 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/trappe/2014/trappe-ua.field
+-rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/trappe/2014/trappe-ua.prm
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/field/trappe/2014/trappe-ua.top
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.968664 emc-pypi-2023.8.2/pyemc/emc/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/modules/changes.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.976664 emc-pypi-2023.8.2/pyemc/emc/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.980664 emc-pypi-2023.8.2/pyemc/emc/scripts/analyze/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5852 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/analyze/cavity.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3371 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/analyze/files.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3276 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/analyze/harvest.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3746 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/analyze/last.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2984 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/analyze/project.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.980664 emc-pypi-2023.8.2/pyemc/emc/scripts/analyze/sample/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/analyze/sample/bond.emc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      818 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/analyze/sample/cavity.emc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      581 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/analyze/sample/distance.emc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      641 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/analyze/sample/gr.emc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      622 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/analyze/sample/gyration.emc
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4272 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/analyze/script.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8532 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/average.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1101 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/avg_error.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2340 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/change.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      992 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/change_header.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)    41097 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/charmm2lammps.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      479 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/clean_restart.pl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.980664 emc-pypi-2023.8.2/pyemc/emc/scripts/coding/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4139 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/coding/cpmod.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1255 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/coding/cpmoddir.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      670 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/coding/emc_comments.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2143 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/coding/emc_parse_oper.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4247 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/coding/header.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      881 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/coding/hold.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      443 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/coding/scrape.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1715 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/emc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      312 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/emc2emc.emc
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/emc2energy.emc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      386 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/emc2insight.emc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      452 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/emc2lammps.emc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      550 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/emc2pdb.emc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      689 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/emc2volume.emc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      306 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/emc2xyz.emc
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5434 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/emc_align.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      613 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/emc_clean.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5093 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/emc_error.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19538 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/emc_field.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18675 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/emc_generate.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32713 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/emc_martini.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35299 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/emc_opls.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29396 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/emc_sdk.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)   369774 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/emc_setup.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2871 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/emc_template.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20155 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/emc_trappe.pl
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/hold.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39906 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/insight2lammps.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      381 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/lammps2emc.emc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      488 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/lammps2lammps.emc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      825 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/lammps2pdb.emc
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4282 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/last.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.980664 emc-pypi-2023.8.2/pyemc/emc/scripts/modules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.980664 emc-pypi-2023.8.2/pyemc/emc/scripts/modules/Charmm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/modules/Charmm/Core
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/modules/Charmm/Global.pm
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/modules/Charmm.pm
+-rw-r--r--   0 runner    (1001) docker     (123)    27706 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/modules/EMCField.pm
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18057 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/myjobs.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10303 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/openff.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      252 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/pack.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      312 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/pdb.emc
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17277 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/pdb_extract.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4116 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/prm_compare.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      999 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/prm_duplicate.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2591 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/prm_extract.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8495 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/prm_list_types.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7094 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/prm_reduce.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      679 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/prm_reduce.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5748 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/prm_search.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1575 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/psf_charge.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4929 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/replace.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18135 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/run.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      610 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/run_analyze.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6648 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/run_host.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3025 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/run_restart.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1744 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/run_stat.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/template.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      756 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/traject2pdb.emc
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3525 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/trj_reduce.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1105 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/try.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4118 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/view_record.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4632 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/view_vmd.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      274 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/scripts/xyz.emc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.980664 emc-pypi-2023.8.2/pyemc/emc/templates/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      347 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/templates/chemistry.esh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/templates/cluster.esh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      837 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/templates/environment.esh
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/templates/field.define
+-rwxr-xr-x   0 runner    (1001) docker     (123)      862 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/templates/field.esh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      395 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/templates/import.esh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      496 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/templates/polymer.esh
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/templates/restart.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.980664 emc-pypi-2023.8.2/pyemc/emc/vmd/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/vmd/README
+-rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/vmd/license.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:28:46.984664 emc-pypi-2023.8.2/pyemc/emc/vmd/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)   299843 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/vmd/packages/gui.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    14504 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/vmd/packages/options.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/vmd/packages/textview.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/emc/vmd/packages.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/pyemc/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 22:28:46.984664 emc-pypi-2023.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-27 22:28:31.000000 emc-pypi-2023.8.2/setup.py
```

### Comparing `emc-pypi-2023.8.1/LICENSE` & `emc-pypi-2023.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/PKG-INFO` & `emc-pypi-2023.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emc-pypi
-Version: 2023.8.1
+Version: 2023.8.2
 Summary: Python interface for the Enhanced Monte Carlo (EMC) package
 Home-page: https://github.com/kevinshen56714/emc-pypi
 Author: Kuan-Hsuan (Kevin) Shen
 Author-email: kevinshen56714@gmail.com
 License: UNKNOWN
 Description: # Enhanced Monte Carlo (EMC) Python Interface
```

### Comparing `emc-pypi-2023.8.1/README.md` & `emc-pypi-2023.8.2/README.md`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/emc_pypi.egg-info/PKG-INFO` & `emc-pypi-2023.8.2/emc_pypi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emc-pypi
-Version: 2023.8.1
+Version: 2023.8.2
 Summary: Python interface for the Enhanced Monte Carlo (EMC) package
 Home-page: https://github.com/kevinshen56714/emc-pypi
 Author: Kuan-Hsuan (Kevin) Shen
 Author-email: kevinshen56714@gmail.com
 License: UNKNOWN
 Description: # Enhanced Monte Carlo (EMC) Python Interface
```

### Comparing `emc-pypi-2023.8.1/emc_pypi.egg-info/SOURCES.txt` & `emc-pypi-2023.8.2/emc_pypi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/HISTORY` & `emc-pypi-2023.8.2/pyemc/emc/HISTORY`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/LICENSE` & `emc-pypi-2023.8.2/pyemc/emc/LICENSE`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/README` & `emc-pypi-2023.8.2/pyemc/emc/README`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/bin/emc_linux_x86_64` & `emc-pypi-2023.8.2/pyemc/emc/bin/emc_linux_x86_64`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/bin/emc_macos` & `emc-pypi-2023.8.2/pyemc/emc/bin/emc_macos`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/bin/emc_win32.exe` & `emc-pypi-2023.8.2/pyemc/emc/bin/emc_win32.exe`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/docs/emc.pdf` & `emc-pypi-2023.8.2/pyemc/emc/docs/emc.pdf`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/bulk/setup.esh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/bulk/setup.esh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/bulk/setup.sh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/bulk/setup.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/charmm/setup.sh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/charmm/setup.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/charmm/solution.esh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/charmm/solution.esh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/dpd/name.esh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/dpd/name.esh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/dpd/setup.sh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/dpd/setup.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/generate/build.emc` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/generate/build.emc`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/generate/field.esh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/generate/field.esh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/generate/field.in` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/generate/field.in`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/generate/field.prm` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/generate/field.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/opls/aa/build.emc` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/opls/aa/build.emc`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.data` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.data`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.emc.gz` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.emc.gz`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.esh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.esh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.in` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.in`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.params` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.params`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.pdb.gz` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.pdb.gz`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.psf.gz` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.psf.gz`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.vmd` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/opls/aa/name.vmd`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/opls/aa/setup.sh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/opls/aa/setup.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/opls/ua/name.esh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/opls/ua/name.esh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/opls/ua/setup.sh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/opls/ua/setup.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/pcff/name.esh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/pcff/name.esh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/pcff/setup.sh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/pcff/setup.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/trappe/name.esh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/trappe/name.esh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/trappe/setup.sh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/trappe/setup.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/field/user/polymer.esh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/field/user/polymer.esh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/alternate/build.emc` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/alternate/build.emc`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/alternate/dpd.in` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/alternate/dpd.in`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/biphase/polymer.esh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/biphase/polymer.esh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/biphase/setup.sh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/biphase/setup.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/copolymer/polymer.esh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/copolymer/polymer.esh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/copolymer/setup.sh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/copolymer/setup.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/dendrimer/polymer.esh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/dendrimer/polymer.esh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/dendrimer/setup.sh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/dendrimer/setup.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/homopolymer/build.emc` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/homopolymer/build.emc`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/homopolymer/polymer.esh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/homopolymer/polymer.esh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/homopolymer/polymer.in` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/homopolymer/polymer.in`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/homopolymer/setup.sh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/homopolymer/setup.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/random_block/block.in` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/random_block/block.in`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/random_block/block.prm` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/random_block/block.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/random_block/build.emc` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/random_block/build.emc`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/polymer/random_block/polymer.esh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/polymer/random_block/polymer.esh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/record/cat.sh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/record/cat.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/record/exec.sh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/record/exec.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/chemistry/surface/surface.esh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/chemistry/surface/surface.esh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/field/README` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/field/README`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/field/chemistry/field/stage/lj.prm` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/field/chemistry/field/stage/lj.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/field/chemistry/scripts/lj.sh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/field/chemistry/scripts/lj.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/field/chemistry/stages/lj/stage.esh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/field/chemistry/stages/lj/stage.esh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/field/setup/lj.esh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/field/setup/lj.esh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/green-kubo/viscosity.esh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/green-kubo/viscosity.esh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/nemd/shear.esh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/nemd/shear.esh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/t_glass/README` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/t_glass/README`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/t_glass/setup/2023072600.esh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/t_glass/setup/2023072600.esh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/t_glass/setup/2023072601.esh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/t_glass/setup/2023072601.esh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/t_glass/setup/2023072610.esh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/t_glass/setup/2023072610.esh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/examples/setup/environment/t_glass/setup/2023072611.esh` & `emc-pypi-2023.8.2/pyemc/emc/examples/setup/environment/t_glass/setup/2023072611.esh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/born/2016/guillot.define` & `emc-pypi-2023.8.2/pyemc/emc/field/born/2016/guillot.define`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/born/2016/guillot.prm` & `emc-pypi-2023.8.2/pyemc/emc/field/born/2016/guillot.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/born/2016/guillot.top` & `emc-pypi-2023.8.2/pyemc/emc/field/born/2016/guillot.top`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/born/2016/matsui.define` & `emc-pypi-2023.8.2/pyemc/emc/field/born/2016/matsui.define`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/born/2016/matsui.prm` & `emc-pypi-2023.8.2/pyemc/emc/field/born/2016/matsui.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/cff/al2o3.frc` & `emc-pypi-2023.8.2/pyemc/emc/field/cff/al2o3.frc`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/cff/al2o3_templates.dat` & `emc-pypi-2023.8.2/pyemc/emc/field/cff/al2o3_templates.dat`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/cff/c3s.frc` & `emc-pypi-2023.8.2/pyemc/emc/field/cff/c3s.frc`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/cff/c3s_templates.dat` & `emc-pypi-2023.8.2/pyemc/emc/field/cff/c3s_templates.dat`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/cff/caso4.frc` & `emc-pypi-2023.8.2/pyemc/emc/field/cff/caso4.frc`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/cff/caso4_templates.dat` & `emc-pypi-2023.8.2/pyemc/emc/field/cff/caso4_templates.dat`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/cff/sio2.frc` & `emc-pypi-2023.8.2/pyemc/emc/field/cff/sio2.frc`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/cff/sio2_templates.dat` & `emc-pypi-2023.8.2/pyemc/emc/field/cff/sio2_templates.dat`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/cff/template.frc` & `emc-pypi-2023.8.2/pyemc/emc/field/cff/template.frc`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/cff/template_templates.dat` & `emc-pypi-2023.8.2/pyemc/emc/field/cff/template_templates.dat`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/cff/zno.frc` & `emc-pypi-2023.8.2/pyemc/emc/field/cff/zno.frc`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/cff/zno_templates.dat` & `emc-pypi-2023.8.2/pyemc/emc/field/cff/zno_templates.dat`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/charmm/c36a/carb.prm` & `emc-pypi-2023.8.2/pyemc/emc/field/charmm/c36a/carb.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/charmm/c36a/carb.top` & `emc-pypi-2023.8.2/pyemc/emc/field/charmm/c36a/carb.top`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/charmm/c36a/cgenff.prm` & `emc-pypi-2023.8.2/pyemc/emc/field/charmm/c36a/cgenff.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/charmm/c36a/cgenff.top` & `emc-pypi-2023.8.2/pyemc/emc/field/charmm/c36a/cgenff.top`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/charmm/c36a/ethers.prm` & `emc-pypi-2023.8.2/pyemc/emc/field/charmm/c36a/ethers.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/charmm/c36a/ethers.top` & `emc-pypi-2023.8.2/pyemc/emc/field/charmm/c36a/ethers.top`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/charmm/c36a/lipid.prm` & `emc-pypi-2023.8.2/pyemc/emc/field/charmm/c36a/lipid.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/charmm/c36a/lipid.top` & `emc-pypi-2023.8.2/pyemc/emc/field/charmm/c36a/lipid.top`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/charmm/c36a/na.prm` & `emc-pypi-2023.8.2/pyemc/emc/field/charmm/c36a/na.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/charmm/c36a/na.top` & `emc-pypi-2023.8.2/pyemc/emc/field/charmm/c36a/na.top`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/charmm/c36a/prot.prm` & `emc-pypi-2023.8.2/pyemc/emc/field/charmm/c36a/prot.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/charmm/c36a/prot.top` & `emc-pypi-2023.8.2/pyemc/emc/field/charmm/c36a/prot.top`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/charmm/c36a/water_ions.prm` & `emc-pypi-2023.8.2/pyemc/emc/field/charmm/c36a/water_ions.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/charmm/c36a/water_ions.top` & `emc-pypi-2023.8.2/pyemc/emc/field/charmm/c36a/water_ions.top`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/dpd/general.prm` & `emc-pypi-2023.8.2/pyemc/emc/field/dpd/general.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/dpd/srp.prm` & `emc-pypi-2023.8.2/pyemc/emc/field/dpd/srp.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/gauss/general.prm` & `emc-pypi-2023.8.2/pyemc/emc/field/gauss/general.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/aminoacids.prm` & `emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/aminoacids.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/cholesterol.prm` & `emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/cholesterol.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/convert.out` & `emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/convert.out`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/ions.prm` & `emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/ions.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/lipids.prm` & `emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/lipids.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/martini.prm` & `emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/martini.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/other.prm` & `emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/other.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/polymers.prm` & `emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/polymers.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/solvents.prm` & `emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/solvents.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/src/aminoacids.itp` & `emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/src/aminoacids.itp`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/src/cholesterol.itp` & `emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/src/cholesterol.itp`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/src/ions.itp` & `emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/src/ions.itp`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/src/lipids.itp` & `emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/src/lipids.itp`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/src/martini.itp` & `emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/src/martini.itp`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/src/other.itp` & `emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/src/other.itp`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/src/other.prm` & `emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/src/other.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/src/polymers.itp` & `emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/src/polymers.itp`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/src/solvents.itp` & `emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/src/solvents.itp`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/src/sugars.itp` & `emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/src/sugars.itp`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/src/surfactants.itp` & `emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/src/surfactants.itp`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/src/xemium.itp` & `emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/src/xemium.itp`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/sugars.prm` & `emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/sugars.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/surfactants.prm` & `emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/surfactants.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/martini/v2.0/xemium.prm` & `emc-pypi-2023.8.2/pyemc/emc/field/martini/v2.0/xemium.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/opls/2012/opls-aa.define` & `emc-pypi-2023.8.2/pyemc/emc/field/opls/2012/opls-aa.define`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/opls/2012/opls-aa.prm` & `emc-pypi-2023.8.2/pyemc/emc/field/opls/2012/opls-aa.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/opls/2012/opls-aa.top` & `emc-pypi-2023.8.2/pyemc/emc/field/opls/2012/opls-aa.top`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/opls/2012/opls-ua.define` & `emc-pypi-2023.8.2/pyemc/emc/field/opls/2012/opls-ua.define`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/opls/2012/opls-ua.prm` & `emc-pypi-2023.8.2/pyemc/emc/field/opls/2012/opls-ua.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/opls/2012/opls-ua.top` & `emc-pypi-2023.8.2/pyemc/emc/field/opls/2012/opls-ua.top`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/opls/2012/src/add.txt` & `emc-pypi-2023.8.2/pyemc/emc/field/opls/2012/src/add.txt`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/opls/2012/src/oplsaa.par` & `emc-pypi-2023.8.2/pyemc/emc/field/opls/2012/src/oplsaa.par`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/opls/2012/src/oplsaa.sb` & `emc-pypi-2023.8.2/pyemc/emc/field/opls/2012/src/oplsaa.sb`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/opls/2012/src/reoplsff.zip` & `emc-pypi-2023.8.2/pyemc/emc/field/opls/2012/src/reoplsff.zip`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/pcff/pcff.frc` & `emc-pypi-2023.8.2/pyemc/emc/field/pcff/pcff.frc`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/pcff/pcff_templates.dat` & `emc-pypi-2023.8.2/pyemc/emc/field/pcff/pcff_templates.dat`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/pcff_ore/pcff_ore.frc` & `emc-pypi-2023.8.2/pyemc/emc/field/pcff_ore/pcff_ore.frc`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/pcff_ore/pcff_ore_templates.dat` & `emc-pypi-2023.8.2/pyemc/emc/field/pcff_ore/pcff_ore_templates.dat`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/polystyrene/smoothed_e-e.m` & `emc-pypi-2023.8.2/pyemc/emc/field/polystyrene/smoothed_e-e.m`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/polystyrene/smoothed_m-e.m` & `emc-pypi-2023.8.2/pyemc/emc/field/polystyrene/smoothed_m-e.m`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/polystyrene/smoothed_m-m.m` & `emc-pypi-2023.8.2/pyemc/emc/field/polystyrene/smoothed_m-m.m`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/polystyrene/smoothed_m-r.m` & `emc-pypi-2023.8.2/pyemc/emc/field/polystyrene/smoothed_m-r.m`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/polystyrene/smoothed_r-e.m` & `emc-pypi-2023.8.2/pyemc/emc/field/polystyrene/smoothed_r-e.m`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/polystyrene/smoothed_r-r.m` & `emc-pypi-2023.8.2/pyemc/emc/field/polystyrene/smoothed_r-r.m`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/sdk/v1.0/sdk.define` & `emc-pypi-2023.8.2/pyemc/emc/field/sdk/v1.0/sdk.define`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/sdk/v1.0/sdk.prm` & `emc-pypi-2023.8.2/pyemc/emc/field/sdk/v1.0/sdk.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/sdk/v1.0/src/angle.dat` & `emc-pypi-2023.8.2/pyemc/emc/field/sdk/v1.0/src/angle.dat`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/sdk/v1.0/src/bond.dat` & `emc-pypi-2023.8.2/pyemc/emc/field/sdk/v1.0/src/bond.dat`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/sdk/v1.0/src/mass.dat` & `emc-pypi-2023.8.2/pyemc/emc/field/sdk/v1.0/src/mass.dat`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/sdk/v1.0/src/pair.dat` & `emc-pypi-2023.8.2/pyemc/emc/field/sdk/v1.0/src/pair.dat`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/sdk/v1.0/src/sdk.xlsx` & `emc-pypi-2023.8.2/pyemc/emc/field/sdk/v1.0/src/sdk.xlsx`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/trappe/2014/list.pl` & `emc-pypi-2023.8.2/pyemc/emc/field/trappe/2014/list.pl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/trappe/2014/torsions.pl` & `emc-pypi-2023.8.2/pyemc/emc/field/trappe/2014/torsions.pl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/trappe/2014/torsions.txt` & `emc-pypi-2023.8.2/pyemc/emc/field/trappe/2014/torsions.txt`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/trappe/2014/trappe-eh.define` & `emc-pypi-2023.8.2/pyemc/emc/field/trappe/2014/trappe-eh.define`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/trappe/2014/trappe-ua.define` & `emc-pypi-2023.8.2/pyemc/emc/field/trappe/2014/trappe-ua.define`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/trappe/2014/trappe-ua.define.old` & `emc-pypi-2023.8.2/pyemc/emc/field/trappe/2014/trappe-ua.define.old`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/trappe/2014/trappe-ua.field` & `emc-pypi-2023.8.2/pyemc/emc/field/trappe/2014/trappe-ua.field`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/trappe/2014/trappe-ua.prm` & `emc-pypi-2023.8.2/pyemc/emc/field/trappe/2014/trappe-ua.prm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/field/trappe/2014/trappe-ua.top` & `emc-pypi-2023.8.2/pyemc/emc/field/trappe/2014/trappe-ua.top`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/modules/changes.txt` & `emc-pypi-2023.8.2/pyemc/emc/modules/changes.txt`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/analyze/cavity.sh` & `emc-pypi-2023.8.2/pyemc/emc/scripts/analyze/cavity.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/analyze/files.sh` & `emc-pypi-2023.8.2/pyemc/emc/scripts/analyze/files.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/analyze/harvest.sh` & `emc-pypi-2023.8.2/pyemc/emc/scripts/analyze/harvest.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/analyze/last.sh` & `emc-pypi-2023.8.2/pyemc/emc/scripts/analyze/last.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/analyze/project.sh` & `emc-pypi-2023.8.2/pyemc/emc/scripts/analyze/project.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/analyze/sample/bond.emc` & `emc-pypi-2023.8.2/pyemc/emc/scripts/analyze/sample/bond.emc`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/analyze/sample/cavity.emc` & `emc-pypi-2023.8.2/pyemc/emc/scripts/analyze/sample/cavity.emc`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/analyze/sample/distance.emc` & `emc-pypi-2023.8.2/pyemc/emc/scripts/analyze/sample/distance.emc`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/analyze/sample/gr.emc` & `emc-pypi-2023.8.2/pyemc/emc/scripts/analyze/sample/gr.emc`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/analyze/sample/gyration.emc` & `emc-pypi-2023.8.2/pyemc/emc/scripts/analyze/sample/gyration.emc`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/analyze/script.sh` & `emc-pypi-2023.8.2/pyemc/emc/scripts/analyze/script.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/average.pl` & `emc-pypi-2023.8.2/pyemc/emc/scripts/average.pl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/avg_error.pl` & `emc-pypi-2023.8.2/pyemc/emc/scripts/avg_error.pl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/change.sh` & `emc-pypi-2023.8.2/pyemc/emc/scripts/change.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/change_header.pl` & `emc-pypi-2023.8.2/pyemc/emc/scripts/change_header.pl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/charmm2lammps.pl` & `emc-pypi-2023.8.2/pyemc/emc/scripts/charmm2lammps.pl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/coding/cpmod.pl` & `emc-pypi-2023.8.2/pyemc/emc/scripts/coding/cpmod.pl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/coding/cpmoddir.sh` & `emc-pypi-2023.8.2/pyemc/emc/scripts/coding/cpmoddir.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/coding/emc_comments.pl` & `emc-pypi-2023.8.2/pyemc/emc/scripts/coding/emc_comments.pl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/coding/emc_parse_oper.pl` & `emc-pypi-2023.8.2/pyemc/emc/scripts/coding/emc_parse_oper.pl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/coding/header.pl` & `emc-pypi-2023.8.2/pyemc/emc/scripts/coding/header.pl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/coding/hold.sh` & `emc-pypi-2023.8.2/pyemc/emc/scripts/coding/hold.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/emc.sh` & `emc-pypi-2023.8.2/pyemc/emc/scripts/emc.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/emc2pdb.emc` & `emc-pypi-2023.8.2/pyemc/emc/scripts/emc2pdb.emc`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/emc2volume.emc` & `emc-pypi-2023.8.2/pyemc/emc/scripts/emc2volume.emc`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/emc_align.pl` & `emc-pypi-2023.8.2/pyemc/emc/scripts/emc_align.pl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/emc_clean.sh` & `emc-pypi-2023.8.2/pyemc/emc/scripts/emc_clean.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/emc_error.sh` & `emc-pypi-2023.8.2/pyemc/emc/scripts/emc_error.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/emc_field.pl` & `emc-pypi-2023.8.2/pyemc/emc/scripts/emc_field.pl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/emc_generate.pl` & `emc-pypi-2023.8.2/pyemc/emc/scripts/emc_generate.pl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/emc_martini.pl` & `emc-pypi-2023.8.2/pyemc/emc/scripts/emc_martini.pl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/emc_opls.pl` & `emc-pypi-2023.8.2/pyemc/emc/scripts/emc_opls.pl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/emc_sdk.pl` & `emc-pypi-2023.8.2/pyemc/emc/scripts/emc_sdk.pl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/emc_setup.pl` & `emc-pypi-2023.8.2/pyemc/emc/scripts/emc_setup.pl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/emc_template.sh` & `emc-pypi-2023.8.2/pyemc/emc/scripts/emc_template.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/emc_trappe.pl` & `emc-pypi-2023.8.2/pyemc/emc/scripts/emc_trappe.pl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/hold.sh` & `emc-pypi-2023.8.2/pyemc/emc/scripts/hold.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/insight2lammps.pl` & `emc-pypi-2023.8.2/pyemc/emc/scripts/insight2lammps.pl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/lammps2pdb.emc` & `emc-pypi-2023.8.2/pyemc/emc/scripts/lammps2pdb.emc`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/last.sh` & `emc-pypi-2023.8.2/pyemc/emc/scripts/last.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/modules/Charmm/Global.pm` & `emc-pypi-2023.8.2/pyemc/emc/scripts/modules/Charmm/Global.pm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/modules/Charmm.pm` & `emc-pypi-2023.8.2/pyemc/emc/scripts/modules/Charmm.pm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/modules/EMCField.pm` & `emc-pypi-2023.8.2/pyemc/emc/scripts/modules/EMCField.pm`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/myjobs.pl` & `emc-pypi-2023.8.2/pyemc/emc/scripts/myjobs.pl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/openff.pl` & `emc-pypi-2023.8.2/pyemc/emc/scripts/openff.pl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/pdb_extract.pl` & `emc-pypi-2023.8.2/pyemc/emc/scripts/pdb_extract.pl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/prm_compare.pl` & `emc-pypi-2023.8.2/pyemc/emc/scripts/prm_compare.pl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/prm_duplicate.pl` & `emc-pypi-2023.8.2/pyemc/emc/scripts/prm_duplicate.pl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/prm_extract.sh` & `emc-pypi-2023.8.2/pyemc/emc/scripts/prm_extract.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/prm_list_types.pl` & `emc-pypi-2023.8.2/pyemc/emc/scripts/prm_list_types.pl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/prm_reduce.pl` & `emc-pypi-2023.8.2/pyemc/emc/scripts/prm_reduce.pl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/prm_reduce.sh` & `emc-pypi-2023.8.2/pyemc/emc/scripts/prm_reduce.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/prm_search.pl` & `emc-pypi-2023.8.2/pyemc/emc/scripts/prm_search.pl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/psf_charge.pl` & `emc-pypi-2023.8.2/pyemc/emc/scripts/psf_charge.pl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/replace.pl` & `emc-pypi-2023.8.2/pyemc/emc/scripts/replace.pl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/run.sh` & `emc-pypi-2023.8.2/pyemc/emc/scripts/run.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/run_analyze.sh` & `emc-pypi-2023.8.2/pyemc/emc/scripts/run_analyze.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/run_host.sh` & `emc-pypi-2023.8.2/pyemc/emc/scripts/run_host.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/run_restart.sh` & `emc-pypi-2023.8.2/pyemc/emc/scripts/run_restart.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/run_stat.sh` & `emc-pypi-2023.8.2/pyemc/emc/scripts/run_stat.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/template.pl` & `emc-pypi-2023.8.2/pyemc/emc/scripts/template.pl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/traject2pdb.emc` & `emc-pypi-2023.8.2/pyemc/emc/scripts/traject2pdb.emc`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/trj_reduce.sh` & `emc-pypi-2023.8.2/pyemc/emc/scripts/trj_reduce.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/try.sh` & `emc-pypi-2023.8.2/pyemc/emc/scripts/try.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/view_record.sh` & `emc-pypi-2023.8.2/pyemc/emc/scripts/view_record.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/scripts/view_vmd.sh` & `emc-pypi-2023.8.2/pyemc/emc/scripts/view_vmd.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/templates/environment.esh` & `emc-pypi-2023.8.2/pyemc/emc/templates/environment.esh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/templates/field.define` & `emc-pypi-2023.8.2/pyemc/emc/templates/field.define`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/templates/field.esh` & `emc-pypi-2023.8.2/pyemc/emc/templates/field.esh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/templates/restart.sh` & `emc-pypi-2023.8.2/pyemc/emc/templates/restart.sh`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/vmd/README` & `emc-pypi-2023.8.2/pyemc/emc/vmd/README`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/vmd/license.txt` & `emc-pypi-2023.8.2/pyemc/emc/vmd/license.txt`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/vmd/packages/gui.tcl` & `emc-pypi-2023.8.2/pyemc/emc/vmd/packages/gui.tcl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/vmd/packages/options.dat` & `emc-pypi-2023.8.2/pyemc/emc/vmd/packages/options.dat`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/emc/vmd/packages/textview.tcl` & `emc-pypi-2023.8.2/pyemc/emc/vmd/packages/textview.tcl`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/pyemc/runner.py` & `emc-pypi-2023.8.2/pyemc/runner.py`

 * *Files identical despite different names*

### Comparing `emc-pypi-2023.8.1/setup.py` & `emc-pypi-2023.8.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     return paths
 
 
 extra_files = package_files('pyemc/emc')
 
 setup(
     name='emc-pypi',
-    version='2023.8.1',
+    version='2023.8.2',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     description='Python interface for the Enhanced Monte Carlo (EMC) package',
     keywords=['EMC', 'Molecular Dynamics', 'LAMMPS', 'SMILES', 'Simulation'],
     url='https://github.com/kevinshen56714/emc-pypi',
     author='Kuan-Hsuan (Kevin) Shen',
     author_email='kevinshen56714@gmail.com',
```

