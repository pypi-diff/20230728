# Comparing `tmp/read_structure_step-2023.7.27.tar.gz` & `tmp/read_structure_step-2023.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "read_structure_step-2023.7.27.tar", last modified: Thu Jul 27 22:49:58 2023, max compression
+gzip compressed data, was "read_structure_step-2023.7.6.tar", last modified: Thu Jul  6 20:21:36 2023, max compression
```

## Comparing `read_structure_step-2023.7.27.tar` & `read_structure_step-2023.7.6.tar`

### file list

```diff
@@ -1,129 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:49:58.826902 read_structure_step-2023.7.27/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-07-27 22:49:58.826902 read_structure_step-2023.7.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:49:58.810902 read_structure_step-2023.7.27/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:49:58.810902 read_structure_step-2023.7.27/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/docs/_static/SEAMM inverted.png
--rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:49:58.814902 read_structure_step-2023.7.27/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/docs/api/read_structure_step.formats.cif.rst
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/docs/api/read_structure_step.formats.mol2.rst
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/docs/api/read_structure_step.formats.mop.rst
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/docs/api/read_structure_step.formats.openbabel_io.rst
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/docs/api/read_structure_step.formats.rst
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/docs/api/read_structure_step.formats.sdf.rst
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/docs/api/read_structure_step.formats.smi.rst
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/docs/api/read_structure_step.formats.xyz.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9623 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:49:58.814902 read_structure_step-2023.7.27/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:49:58.814902 read_structure_step-2023.7.27/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)   434049 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/docs/getting_started/dialog.png
--rw-r--r--   0 runner    (1001) docker     (123)   121911 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/docs/getting_started/flowchart.png
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:49:58.814902 read_structure_step-2023.7.27/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:49:58.826902 read_structure_step-2023.7.27/read_structure_step/
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-27 22:49:58.826902 read_structure_step-2023.7.27/read_structure_step/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:49:58.818902 read_structure_step-2023.7.27/read_structure_step/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/data/references.bib
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:49:58.818902 read_structure_step-2023.7.27/read_structure_step/formats/
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/formats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:49:58.818902 read_structure_step-2023.7.27/read_structure_step/formats/cif/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/formats/cif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/formats/cif/cif.py
--rw-r--r--   0 runner    (1001) docker     (123)     8762 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/formats/cif/mmcif.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:49:58.818902 read_structure_step-2023.7.27/read_structure_step/formats/mol2/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/formats/mol2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/formats/mol2/mol2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:49:58.818902 read_structure_step-2023.7.27/read_structure_step/formats/mop/
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/formats/mop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/formats/mop/find_mopac.py
--rw-r--r--   0 runner    (1001) docker     (123)    22956 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/formats/mop/obabel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:49:58.822902 read_structure_step-2023.7.27/read_structure_step/formats/openbabel_io/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/formats/openbabel_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/formats/openbabel_io/checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/formats/openbabel_io/obabel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/formats/registries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:49:58.822902 read_structure_step-2023.7.27/read_structure_step/formats/sdf/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/formats/sdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15803 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/formats/sdf/sdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:49:58.822902 read_structure_step-2023.7.27/read_structure_step/formats/smi/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/formats/smi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/formats/smi/smi.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/formats/which.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:49:58.822902 read_structure_step-2023.7.27/read_structure_step/formats/xyz/
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/formats/xyz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19116 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/formats/xyz/xyz.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/read.py
--rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/read_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/read_structure_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/read_structure_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/tk_read_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/tk_write_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/write.py
--rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/write_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/write_structure_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/read_structure_step/write_structure_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:49:58.818902 read_structure_step-2023.7.27/read_structure_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-07-27 22:49:58.000000 read_structure_step-2023.7.27/read_structure_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-07-27 22:49:58.000000 read_structure_step-2023.7.27/read_structure_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 22:49:58.000000 read_structure_step-2023.7.27/read_structure_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-27 22:49:58.000000 read_structure_step-2023.7.27/read_structure_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 22:49:58.000000 read_structure_step-2023.7.27/read_structure_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 22:49:58.000000 read_structure_step-2023.7.27/read_structure_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 22:49:42.000000 read_structure_step-2023.7.27/read_structure_step.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-27 22:49:58.826902 read_structure_step-2023.7.27/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:49:58.822902 read_structure_step-2023.7.27/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/tests/build_filenames.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:49:58.826902 read_structure_step-2023.7.27/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/tests/data/3TR_model.json
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/tests/data/3TR_model.mol2
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/tests/data/3TR_model.pdb
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/tests/data/3TR_model.sdf
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/tests/data/3TR_model.sdf.bz2
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/tests/data/3TR_model.sdf.gz
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/tests/data/3TR_model.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/tests/data/3TR_model_MN.xyz
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/tests/data/Cr_ACETCR.mop
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/tests/data/Cu(II)4Br10(2-) (CIVNAW10).mop
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/tests/data/RM1 63 Europium, CCDC entry LAPJAN.mop
--rwxr-xr-x   0 runner    (1001) docker     (123)      658 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/tests/data/acetonitrile.mop
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/tests/data/lithium fluoride, trimer.mop
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/tests/data/methylidyne.mop
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/tests/data/potassium fluoride, dimer.mop
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/tests/data/spc
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/tests/data/spc.xyz
--rw-r--r--   0 runner    (1001) docker     (123)    13395 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/tests/data/tmQM_test.xyz.bz2
--rw-r--r--   0 runner    (1001) docker     (123)    16514 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/tests/data/tmQM_test.xyz.gz
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/tests/methylidyne.mop
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/tests/mopac_exists.py
--rw-r--r--   0 runner    (1001) docker     (123)     9538 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/tests/test_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/tests/test_read_structure_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-27 22:49:38.000000 read_structure_step-2023.7.27/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.616279 read_structure_step-2023.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-06 20:21:36.616279 read_structure_step-2023.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.600279 read_structure_step-2023.7.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.600279 read_structure_step-2023.7.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/_static/SEAMM inverted.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.604279 read_structure_step-2023.7.6/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/api/read_structure_step.formats.cif.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/api/read_structure_step.formats.mol2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/api/read_structure_step.formats.mop.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/api/read_structure_step.formats.openbabel_io.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/api/read_structure_step.formats.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/api/read_structure_step.formats.sdf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/api/read_structure_step.formats.smi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/api/read_structure_step.formats.xyz.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9623 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.604279 read_structure_step-2023.7.6/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.604279 read_structure_step-2023.7.6/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)   434049 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/getting_started/dialog.png
+-rw-r--r--   0 runner    (1001) docker     (123)   121911 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/getting_started/flowchart.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.604279 read_structure_step-2023.7.6/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.620279 read_structure_step-2023.7.6/read_structure_step/
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-06 20:21:36.620279 read_structure_step-2023.7.6/read_structure_step/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.608279 read_structure_step-2023.7.6/read_structure_step/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/data/references.bib
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.612279 read_structure_step-2023.7.6/read_structure_step/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.612279 read_structure_step-2023.7.6/read_structure_step/formats/cif/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/cif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/cif/cif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8762 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/cif/mmcif.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.612279 read_structure_step-2023.7.6/read_structure_step/formats/mol2/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/mol2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/mol2/mol2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.612279 read_structure_step-2023.7.6/read_structure_step/formats/mop/
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/mop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/mop/find_mopac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22956 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/mop/obabel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.612279 read_structure_step-2023.7.6/read_structure_step/formats/openbabel_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/openbabel_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/openbabel_io/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/openbabel_io/obabel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/registries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.612279 read_structure_step-2023.7.6/read_structure_step/formats/sdf/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/sdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15572 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/sdf/sdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.612279 read_structure_step-2023.7.6/read_structure_step/formats/smi/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/smi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/smi/smi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/which.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.612279 read_structure_step-2023.7.6/read_structure_step/formats/xyz/
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/xyz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/xyz/xyz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/read_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/read_structure_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/read_structure_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/tk_read_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/tk_write_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/write_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/write_structure_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/write_structure_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.608279 read_structure_step-2023.7.6/read_structure_step.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-06 20:21:36.000000 read_structure_step-2023.7.6/read_structure_step.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-06 20:21:36.000000 read_structure_step-2023.7.6/read_structure_step.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:21:36.000000 read_structure_step-2023.7.6/read_structure_step.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-06 20:21:36.000000 read_structure_step-2023.7.6/read_structure_step.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 20:21:36.000000 read_structure_step-2023.7.6/read_structure_step.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 20:21:36.000000 read_structure_step-2023.7.6/read_structure_step.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:21:21.000000 read_structure_step-2023.7.6/read_structure_step.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-06 20:21:36.620279 read_structure_step-2023.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.616279 read_structure_step-2023.7.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/build_filenames.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.616279 read_structure_step-2023.7.6/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/data/3TR_model.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/data/3TR_model.mol2
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/data/3TR_model.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/data/3TR_model.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/data/3TR_model.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/data/3TR_model_MN.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/data/Cr_ACETCR.mop
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/data/Cu(II)4Br10(2-) (CIVNAW10).mop
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/data/RM1 63 Europium, CCDC entry LAPJAN.mop
+-rwxr-xr-x   0 runner    (1001) docker     (123)      658 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/data/acetonitrile.mop
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/data/lithium fluoride, trimer.mop
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/data/methylidyne.mop
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/data/potassium fluoride, dimer.mop
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/data/spc
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/data/spc.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/methylidyne.mop
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/mopac_exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/test_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/test_read_structure_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/versioneer.py
```

### Comparing `read_structure_step-2023.7.27/CONTRIBUTING.rst` & `read_structure_step-2023.7.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/HISTORY.rst` & `read_structure_step-2023.7.6/HISTORY.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 =======
 History
 =======
 
-2023.7.27 -- Support for .gz and .bz2 files, and multi-structure .xyz files
-  * Handle .gz and .bz2 files for .sdf and .xyz extensions.
-  * Handle multi-structure XYZ files with a blank line between records.
-    
 2023.7.6 -- Bugfixes
   * Fixed output of number of structures written to SDF files, which was off by 1.
   * Cleaned up the output for the write-structure step
     
 2023.1.30 -- Fixed issue#43, duplicate systems or configuration created
 
   * Reading a single structure from e.g. a .sdf file created a second system or
```

### Comparing `read_structure_step-2023.7.27/LICENSE` & `read_structure_step-2023.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/PKG-INFO` & `read_structure_step-2023.7.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: read_structure_step
-Version: 2023.7.27
+Version: 2023.7.6
 Summary: A SEAMM plug-in to read common formats in computational chemistry
 Home-page: https://github.com/molssi-seamm/read_structure_step
 Author: Eliseo Marin-R-Rimoldi
 Author-email: meliseo@vt.edu
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,Open Babel,molecules,atomistic,files
 Platform: Linux
@@ -101,18 +101,14 @@
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
 
-2023.7.27 -- Support for .gz and .bz2 files, and multi-structure .xyz files
-  * Handle .gz and .bz2 files for .sdf and .xyz extensions.
-  * Handle multi-structure XYZ files with a blank line between records.
-    
 2023.7.6 -- Bugfixes
   * Fixed output of number of structures written to SDF files, which was off by 1.
   * Cleaned up the output for the write-structure step
     
 2023.1.30 -- Fixed issue#43, duplicate systems or configuration created
 
   * Reading a single structure from e.g. a .sdf file created a second system or
```

### Comparing `read_structure_step-2023.7.27/README.rst` & `read_structure_step-2023.7.6/README.rst`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/docs/Makefile` & `read_structure_step-2023.7.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/docs/_static/SEAMM inverted.png` & `read_structure_step-2023.7.6/docs/_static/SEAMM inverted.png`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/docs/_static/SEAMM logo.png` & `read_structure_step-2023.7.6/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/docs/_static/molssi_main_logo.png` & `read_structure_step-2023.7.6/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/docs/_static/molssi_main_logo_inverted_white.png` & `read_structure_step-2023.7.6/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/docs/_static/molssi_square.png` & `read_structure_step-2023.7.6/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/docs/_static/nsf.png` & `read_structure_step-2023.7.6/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/docs/api/read_structure_step.formats.cif.rst` & `read_structure_step-2023.7.6/docs/api/read_structure_step.formats.cif.rst`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/docs/api/read_structure_step.formats.mop.rst` & `read_structure_step-2023.7.6/docs/api/read_structure_step.formats.mop.rst`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/docs/api/read_structure_step.formats.openbabel_io.rst` & `read_structure_step-2023.7.6/docs/api/read_structure_step.formats.openbabel_io.rst`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/docs/api/read_structure_step.formats.rst` & `read_structure_step-2023.7.6/docs/api/read_structure_step.formats.rst`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/docs/conf.py` & `read_structure_step-2023.7.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/docs/developer_guide/installation.rst` & `read_structure_step-2023.7.6/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/docs/getting_started/dialog.png` & `read_structure_step-2023.7.6/docs/getting_started/dialog.png`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/docs/getting_started/flowchart.png` & `read_structure_step-2023.7.6/docs/getting_started/flowchart.png`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/docs/getting_started/index.rst` & `read_structure_step-2023.7.6/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/docs/index.rst` & `read_structure_step-2023.7.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/docs/make.bat` & `read_structure_step-2023.7.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/read_structure_step/__init__.py` & `read_structure_step-2023.7.6/read_structure_step/__init__.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/read_structure_step/data/references.bib` & `read_structure_step-2023.7.6/read_structure_step/data/references.bib`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/read_structure_step/errors.py` & `read_structure_step-2023.7.6/read_structure_step/errors.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/read_structure_step/formats/__init__.py` & `read_structure_step-2023.7.6/read_structure_step/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/read_structure_step/formats/cif/cif.py` & `read_structure_step-2023.7.6/read_structure_step/formats/cif/cif.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/read_structure_step/formats/cif/mmcif.py` & `read_structure_step-2023.7.6/read_structure_step/formats/cif/mmcif.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/read_structure_step/formats/mol2/mol2.py` & `read_structure_step-2023.7.6/read_structure_step/formats/mol2/mol2.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/read_structure_step/formats/mop/__init__.py` & `read_structure_step-2023.7.6/read_structure_step/formats/mop/__init__.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/read_structure_step/formats/mop/find_mopac.py` & `read_structure_step-2023.7.6/read_structure_step/formats/mop/find_mopac.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/read_structure_step/formats/mop/obabel.py` & `read_structure_step-2023.7.6/read_structure_step/formats/mop/obabel.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/read_structure_step/formats/openbabel_io/checkers.py` & `read_structure_step-2023.7.6/read_structure_step/formats/openbabel_io/checkers.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/read_structure_step/formats/openbabel_io/obabel.py` & `read_structure_step-2023.7.6/read_structure_step/formats/openbabel_io/obabel.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/read_structure_step/formats/registries.py` & `read_structure_step-2023.7.6/read_structure_step/formats/registries.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/read_structure_step/formats/sdf/sdf.py` & `read_structure_step-2023.7.6/read_structure_step/formats/sdf/sdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 Implementation of the reader for SDF files using OpenBabel
 """
 
-import bz2
 import gzip
 from pathlib import Path
 import shutil
 import string
 import subprocess
 import time
 
@@ -130,23 +129,18 @@
 
     if isinstance(path, str):
         path = Path(path)
 
     path.expanduser().resolve()
 
     # Get the information for progress output, if requested.
+    compress = path.suffix == ".gz"
     if printer is not None:
         n_structures = 0
-        with (
-            gzip.open(path, mode="rt")
-            if path.suffix == ".gz"
-            else bz2.open(path, mode="rt")
-            if path.suffix == ".bz2"
-            else open(path, "r")
-        ) as fd:
+        with gzip.open(path, mode="rt") if compress else open(path, "r") as fd:
             for line in fd:
                 if line[0:4] == "$$$$":
                     n_structures += 1
         printer("")
         printer(f"    The SDF file contains {n_structures} structures.")
         last_percent = 0
         t0 = time.time()
@@ -156,21 +150,15 @@
     obConversion.SetInAndOutFormats("sdf", "smi")
 
     configurations = []
     structure_no = 1
     n_errors = 0
     obMol = openbabel.OBMol()
     text = ""
-    with (
-        gzip.open(path, mode="rt")
-        if path.suffix == ".gz"
-        else bz2.open(path, mode="rt")
-        if path.suffix == ".bz2"
-        else open(path, "r")
-    ) as fd:
+    with gzip.open(path, mode="rt") if compress else open(path, "r") as fd:
         for line in fd:
             text += line
 
             if line[0:4] != "$$$$":
                 continue
 
             obConversion.ReadString(obMol, text)
```

### Comparing `read_structure_step-2023.7.27/read_structure_step/formats/smi/smi.py` & `read_structure_step-2023.7.6/read_structure_step/formats/smi/smi.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/read_structure_step/formats/xyz/__init__.py` & `read_structure_step-2023.7.6/read_structure_step/formats/xyz/__init__.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/read_structure_step/formats/xyz/xyz.py` & `read_structure_step-2023.7.6/read_structure_step/formats/xyz/xyz.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """
 Implementation of the reader for XYZ files using OpenBabel
 """
 
-import bz2
-import gzip
 import logging
 import os
 from pathlib import Path
 import shutil
 import string
 import subprocess
 import sys
@@ -117,86 +115,38 @@
     indices="1:end",
     subsequent_as_configurations=False,
     system_name="Canonical SMILES",
     configuration_name="sequential",
     printer=None,
     references=None,
     bibliography=None,
+    save_data=True,
     **kwargs,
 ):
     """Read an XYZ input file.
 
     Parameters
     ----------
     file_name : str or Path
         The path to the file, as either a string or Path.
 
     configuration : molsystem.Configuration
         The configuration to put the imported structure into.
 
-    extension : str, optional, default: None
-        The extension, including initial dot, defining the format.
-
-    add_hydrogens : bool = True
-        Whether to add any missing hydrogen atoms.
-
-    system_db : System_DB = None
-        The system database, used if multiple structures in the file.
-
-    system : System = None
-        The system to use if adding subsequent structures as configurations.
-
-    indices : str = "1:end"
-        The generalized indices (slices, SMARTS, etc.) to select structures
-        from a file containing multiple structures.
-
-    subsequent_as_configurations : bool = False
-        Normally and subsequent structures are loaded into new systems; however,
-        if this option is True, they will be added as configurations.
-
-    system_name : str = "from file"
-        The name for systems. Can be directives like "SMILES" or
-        "Canonical SMILES". If None, no name is given.
-
-    configuration_name : str = "sequential"
-        The name for configurations. Can be directives like "SMILES" or
-        "Canonical SMILES". If None, no name is given.
-
-    printer : Logger or Printer
-        A function that prints to the appropriate place, used for progress.
-
-    references : ReferenceHandler = None
-        The reference handler object or None
-
-    bibliography : dict
-        The bibliography as a dictionary.
-
-    Returns
-    -------
-    [Configuration]
-        The list of configurations created.
-
-
     We'll use OpenBabel to read the file; however, OpenBabel is somewhat limited, so
     we'll first preprocess the file to extract extra data and also to fit it to the
     format that OpenBabel can handle.
 
     A "standard" .xyz file the following structure:
 
         #. The number of atoms on the first line
         #. A comment on the second, often the structure name
         #. symbol, x, y, z
         #. ...
 
-    Some XYZ files, for instance those from tmQM encode data in the comment line::
-
-        CSD_code = WIXKOE | q = 0 | S = 0 | Stoichiometry = C47H65LaN2O | MND = 7
-
-    We'll try to handle this type of comment.
-
     The Minnesota Solvation database uses a slightly modified form:
 
         #. A comment, often the structure name and provenance
         #. A blank line (maybe the number of atoms, but seems to be blank)
         #. <charge> <multiplicity>
         #. symbol, x, y, z
         #. ...
@@ -210,275 +160,159 @@
     global OpenBabel_version
 
     # Get the text in the file
     if isinstance(file_name, str):
         path = Path(file_name)
     else:
         path = file_name
-    path = path.expanduser().resolve()
-
-    print(f"In xyz.py, path = {path}")
+    path.expanduser().resolve()
+    lines = path.read_text().splitlines()
 
-    # Get the information for progress output, if requested.
-    n_structures = 0
-    last_line = 0
-    with (
-        gzip.open(path, mode="rt")
-        if path.suffix == ".gz"
-        else bz2.open(path, mode="rt")
-        if path.suffix == ".bz2"
-        else open(path, "r")
-    ) as fd:
-        for line in fd:
-            last_line += 1
-            if line.strip() == "":
-                n_structures += 1
-    # may not have blank line at end
-    if line.strip() != "":
-        n_structures += 1
-    if printer is not None:
-        printer("")
-        printer(f"    The XYZ file contains {n_structures} structures.")
-        last_percent = 0
-        t0 = time.time()
-        last_t = t0
-
-    obConversion = openbabel.OBConversion()
-    obConversion.SetInFormat("xyz")
-
-    configurations = []
-    structure_no = 0
-    n_errors = 0
-    obMol = openbabel.OBMol()
-
-    total_lines = 0
-    with (
-        gzip.open(path, mode="rt")
-        if path.suffix == ".gz"
-        else bz2.open(path, mode="rt")
-        if path.suffix == ".bz2"
-        else open(path, "r")
-    ) as fd:
-        print(f"{fd=}")
-        lines = []
-        line_no = 0
-        for line in fd:
-            # lines have \n at end. It is not stripped as is more normal.
-            total_lines += 1
-            line_no += 1
-            lines.append(line)
-            if total_lines == last_line or line_no > 3 and line.strip() == "":
-                # End of block, so examine the first lines and see which format
-                file_type = "unknown"
-                n_lines = len(lines)
-                print(f"Found block of {n_lines} lines")
-                line1 = lines[0].strip()
-                fields1 = line1.split()
-                n_fields1 = len(fields1)
-
-                if n_lines <= 1:
-                    line2 = None
-                    fields2 = []
-                    n_fields2 = 0
+    # Examine the first lines and see what the format might be
+    file_type = "unknown"
+    n_lines = len(lines)
+    line1 = lines[0].strip()
+    fields1 = line1.split()
+    n_fields1 = len(fields1)
+
+    if n_lines <= 1:
+        line2 = None
+        fields2 = []
+        n_fields2 = 0
+    else:
+        line2 = lines[1].strip()
+        fields2 = line2.split()
+        n_fields2 = len(fields2)
+
+    if n_lines <= 2:
+        line3 = None
+        fields3 = []
+        n_fields3 = 0
+    else:
+        line3 = lines[2].strip()
+        fields3 = line3.split()
+        n_fields3 = len(fields3)
+
+    # Check for "standard" file
+    if n_fields1 == 1:
+        try:
+            n_atoms = int(fields1[0])
+        except Exception:
+            pass
+        else:
+            # Might be traditional file. Check 3rd line for atom
+            if n_fields3 == 4:
+                file_type = "standard"
+    elif n_fields1 == 0:
+        # Might be standard file without atom count.
+        if n_fields3 == 4:
+            file_type = "standard"
+            n_atoms = 0
+            for line in lines[2:]:
+                n_fields = len(line.split())
+                if n_fields == 0:
+                    break
                 else:
-                    line2 = lines[1].strip()
-                    fields2 = line2.split()
-                    n_fields2 = len(fields2)
-
-                if n_lines <= 2:
-                    line3 = None
-                    fields3 = []
-                    n_fields3 = 0
+                    n_atoms += 1
+            # Put the count in line 1
+            lines[0] = str(n_atoms)
+
+    # And Minnesota variant with three headers.
+    if n_lines > 3 and n_fields3 == 2:
+        try:
+            charge = int(fields3[0])
+            multiplicity = int(fields3[1])
+        except Exception:
+            pass
+        else:
+            file_type = "Minnesota"
+            if n_fields2 != 0:
+                logger.warning(
+                    f"Minnesota style XYZ file, 2nd line is not blank:\n\t{lines[1]}"
+                )
+            # Count atoms
+            n_atoms = 0
+            for line in lines[3:]:
+                n_fields = len(line.split())
+                if n_fields == 0:
+                    break
                 else:
-                    line3 = lines[2].strip()
-                    fields3 = line3.split()
-                    n_fields3 = len(fields3)
-
-                # Check for "standard" file
-                if n_fields1 == 1:
-                    try:
-                        n_atoms = int(fields1[0])
-                    except Exception:
-                        pass
-                    else:
-                        # Might be traditional file. Check 3rd line for atom
-                        if n_fields3 == 4:
-                            file_type = "standard"
-                elif n_fields1 == 0:
-                    # Might be standard file without atom count.
-                    if n_fields3 == 4:
-                        file_type = "standard"
-                        n_atoms = 0
-                        for line in lines[2:]:
-                            n_fields = len(line.split())
-                            if n_fields == 0:
-                                break
-                            else:
-                                n_atoms += 1
-                        # Put the count in line 1
-                        lines[0] = str(n_atoms)
-
-                # And Minnesota variant with three headers.
-                if n_lines > 3 and n_fields3 == 2:
-                    try:
-                        charge = int(fields3[0])
-                        multiplicity = int(fields3[1])
-                    except Exception:
-                        pass
-                    else:
-                        file_type = "Minnesota"
-                        if n_fields2 != 0:
-                            logger.warning(
-                                "Minnesota style XYZ file, 2nd line is not blank:"
-                                f"\n\t{lines[1]}"
-                            )
-                        # Count atoms
-                        n_atoms = 0
-                        for line in lines[3:]:
-                            n_fields = len(line.split())
-                            if n_fields == 0:
-                                break
-                            else:
-                                n_atoms += 1
-                        # Move comment to 2nd line
-                        lines[1] = lines[0]
-                        # Put the count in line 1
-                        lines[0] = str(n_atoms) + "\n"
-                        # Remove 3rd line with charge and multiplicity
-                        del lines[2]
-
-                # Reassemble an input file.
-                input_data = "".join(lines)
-
-                print("Input data")
-                print(input_data)
-                print("---------")
-
-                logger.info(f"Input data:\n\n{input_data}\n")
-
-                title = lines[1].strip()
-
-                lines = []
-                line_no = 0
-
-                # Now try to convert using OpenBabel
-                out = OutputGrabber(sys.stderr)
-                with out:
-                    success = obConversion.ReadString(obMol, input_data)
-                    if not success:
-                        raise RuntimeError("obConversion failed")
-
-                    if add_hydrogens:
-                        obMol.AddHydrogens()
-
-                    structure_no += 1
-                    if structure_no > 1:
-                        if subsequent_as_configurations:
-                            configuration = system.create_configuration()
-                        else:
-                            system = system_db.create_system()
-                            configuration = system.create_configuration()
-
-                    configuration.from_OBMol(obMol)
-                    configurations.append(configuration)
-
-                # Check any stderr information from obabel.
-                if out.capturedtext != "":
-                    tmp = out.capturedtext
-                    if (
-                        "Failed to kekulize aromatic bonds in OBMol::PerceiveBondOrders"
-                        not in tmp
-                    ):
-                        logger.warning(f"{structure_no}: {tmp}")
-
-                if file_type == "Minnesota":
-                    # Record the charge, and the spin state
-                    configuration.charge = charge
-                    configuration.spin_multiplicity = multiplicity
-
-                    logger.info(f"{charge=} {multiplicity=}")
-                elif "|" in title:
-                    for tmp in title.split("|"):
-                        if "=" in tmp:
-                            key, val = tmp.split(maxsplit=1)
-                            key = key.strip()
-                            val = val.strip()
-                            if key == "q":
-                                try:
-                                    configuration.charge = float(val)
-                                except Exception:
-                                    pass
-                            elif key == "S":
-                                try:
-                                    configuration.spin_multiplicity = int(val)
-                                except Exception:
-                                    pass
-                            elif key == "CSD_code":
-                                title = val
-
-                # Set the system name
-                if system_name is not None and system_name != "":
-                    lower_name = system_name.lower()
-                    if "from file" in lower_name:
-                        system.name = str(path)
-                    elif lower_name == "title":
-                        if len(title) > 0:
-                            system.name = title
-                        else:
-                            system.name = str(path)
-                    elif "canonical smiles" in lower_name:
-                        system.name = configuration.canonical_smiles
-                    elif "smiles" in lower_name:
-                        system.name = configuration.smiles
-                    else:
-                        system.name = system_name
-
-                # And the configuration name
-                if configuration_name is not None and configuration_name != "":
-                    lower_name = configuration_name.lower()
-                    if "from file" in lower_name:
-                        configuration.name = obMol.GetTitle()
-                    elif lower_name == "title":
-                        if len(title) > 0:
-                            configuration.name = title
-                        else:
-                            configuration.name = str(path)
-                    elif "canonical smiles" in lower_name:
-                        configuration.name = configuration.canonical_smiles
-                    elif "smiles" in lower_name:
-                        configuration.name = configuration.smiles
-                    elif lower_name == "sequential":
-                        configuration.name = str(structure_no)
-                    else:
-                        configuration.name = configuration_name
-
-                if printer:
-                    percent = int(100 * structure_no / n_structures)
-                    if percent > last_percent:
-                        t1 = time.time()
-                        if t1 - last_t >= 60:
-                            t = int(t1 - t0)
-                            rate = structure_no / (t1 - t0)
-                            t_left = int((n_structures - structure_no) / rate)
-                            printer(
-                                f"\t{structure_no:6} ({percent}%) structures read in "
-                                f"{t} seconds. About {t_left} seconds remaining."
-                            )
-                            last_t = t1
-                            last_percent = percent
-
-    if printer:
-        t1 = time.time()
-        rate = structure_no / (t1 - t0)
-        printer(
-            f"    Read {structure_no - n_errors - 1} structures in {t1 - t0:.1f} "
-            f"seconds = {rate:.2f} per second"
-        )
-        if n_errors > 0:
-            printer(f"    {n_errors} structures could not be read due to errors.")
+                    n_atoms += 1
+            # Move comment to 2nd line
+            lines[1] = lines[0]
+            # Put the count in line 1
+            lines[0] = str(n_atoms)
+            # Remove 3rd line with charge and multiplicity
+            del lines[2]
+
+    # Reassemble an input file.
+    input_data = "\n".join(lines)
+    logger.info(f"Input data:\n\n{input_data}\n")
+
+    title = lines[1].strip()
+
+    # Now try to convert using OpenBabel
+    out = OutputGrabber(sys.stderr)
+    with out:
+        obConversion = openbabel.OBConversion()
+        obConversion.SetInFormat("xyz")
+        obMol = openbabel.OBMol()
+
+        success = obConversion.ReadString(obMol, input_data)
+        if not success:
+            raise RuntimeError("obConversion failed")
+
+        if add_hydrogens:
+            obMol.AddHydrogens()
+
+        configuration.from_OBMol(obMol)
+
+    # Check any stderr information from obabel.
+    if out.capturedtext != "":
+        tmp = out.capturedtext
+        if "Failed to kekulize aromatic bonds in OBMol::PerceiveBondOrders" not in tmp:
+            logger.warning(tmp)
+
+    if file_type == "Minnesota":
+        # Record the charge, and the spin state
+        configuration.charge = charge
+        configuration.spin_multiplicity = multiplicity
+
+        logger.info(f"{charge=} {multiplicity=}")
+
+    # Set the system name
+    if system_name is not None and system_name != "":
+        lower_name = system_name.lower()
+        if "from file" in lower_name:
+            system.name = str(path)
+        elif lower_name == "title":
+            if len(title) > 0:
+                system.name = title
+            else:
+                system.name = str(path)
+        elif "canonical smiles" in lower_name:
+            system.name = configuration.canonical_smiles
+        elif "smiles" in lower_name:
+            system.name = configuration.smiles
+        else:
+            system.name = system_name
+
+    # And the configuration name
+    if configuration_name is not None and configuration_name != "":
+        lower_name = configuration_name.lower()
+        if "from file" in lower_name:
+            configuration.name = obMol.GetTitle()
+        elif "canonical smiles" in lower_name:
+            configuration.name = configuration.canonical_smiles
+        elif "smiles" in lower_name:
+            configuration.name = configuration.smiles
+        elif lower_name == "sequential":
+            configuration.name = "1"
+        else:
+            configuration.name = configuration_name
 
     if references:
         # Add the citations for Open Babel
         references.cite(
             raw=bibliography["openbabel"],
             alias="openbabel_jcinf",
             module="read_structure_step",
@@ -530,8 +364,8 @@
                     module="read_structure_step",
                     level=1,
                     note="The principle citation for the Open Babel executables.",
                 )
             except Exception:
                 pass
 
-    return configurations
+    return [configuration]
```

### Comparing `read_structure_step-2023.7.27/read_structure_step/read.py` & `read_structure_step-2023.7.6/read_structure_step/read.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/read_structure_step/read_structure.py` & `read_structure_step-2023.7.6/read_structure_step/read_structure.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/read_structure_step/read_structure_parameters.py` & `read_structure_step-2023.7.6/read_structure_step/read_structure_parameters.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/read_structure_step/read_structure_step.py` & `read_structure_step-2023.7.6/read_structure_step/read_structure_step.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/read_structure_step/tk_read_structure.py` & `read_structure_step-2023.7.6/read_structure_step/tk_read_structure.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/read_structure_step/tk_write_structure.py` & `read_structure_step-2023.7.6/read_structure_step/tk_write_structure.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/read_structure_step/utils.py` & `read_structure_step-2023.7.6/read_structure_step/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-from pathlib import Path
+import os
 from . import formats
 import re
 
 
 def guess_extension(file_name, use_file_name=False):
     """
     Returns the file format. It can either use the file name extension or
     guess based on signatures found in the file.
 
-    Correctly handles .gz and .bz2 files.
-
     Parameters
     ----------
     file_name: str
         Name of the file
 
     use_file_name: bool, optional, default: False
         If set to True, uses the file name extension to identify the
@@ -22,21 +20,16 @@
     Returns
     -------
     extension: str
         The file format.
     """
 
     if use_file_name is True:
-        path = Path(file_name)
-        suffixes = path.suffixes
-        ext = ""
-        if len(suffixes) > 0:
-            ext = suffixes[-1]
-            if ext in (".gz", ".bz2") and len(suffixes) > 1:
-                ext = suffixes[-2]
+        (root, ext) = os.path.splitext(file_name)
+
         if ext == "":
             return None
 
         return ext.lower()
 
     available_extensions = formats.registries.REGISTERED_FORMAT_CHECKERS.keys()
```

### Comparing `read_structure_step-2023.7.27/read_structure_step/write.py` & `read_structure_step-2023.7.6/read_structure_step/write.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/read_structure_step/write_structure.py` & `read_structure_step-2023.7.6/read_structure_step/write_structure.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/read_structure_step/write_structure_parameters.py` & `read_structure_step-2023.7.6/read_structure_step/write_structure_parameters.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/read_structure_step/write_structure_step.py` & `read_structure_step-2023.7.6/read_structure_step/write_structure_step.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/read_structure_step.egg-info/PKG-INFO` & `read_structure_step-2023.7.6/read_structure_step.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: read-structure-step
-Version: 2023.7.27
+Version: 2023.7.6
 Summary: A SEAMM plug-in to read common formats in computational chemistry
 Home-page: https://github.com/molssi-seamm/read_structure_step
 Author: Eliseo Marin-R-Rimoldi
 Author-email: meliseo@vt.edu
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,Open Babel,molecules,atomistic,files
 Platform: Linux
@@ -101,18 +101,14 @@
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
 
-2023.7.27 -- Support for .gz and .bz2 files, and multi-structure .xyz files
-  * Handle .gz and .bz2 files for .sdf and .xyz extensions.
-  * Handle multi-structure XYZ files with a blank line between records.
-    
 2023.7.6 -- Bugfixes
   * Fixed output of number of structures written to SDF files, which was off by 1.
   * Cleaned up the output for the write-structure step
     
 2023.1.30 -- Fixed issue#43, duplicate systems or configuration created
 
   * Reading a single structure from e.g. a .sdf file created a second system or
```

### Comparing `read_structure_step-2023.7.27/read_structure_step.egg-info/SOURCES.txt` & `read_structure_step-2023.7.6/read_structure_step.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -87,22 +87,18 @@
 tests/test_formats.py
 tests/test_read_structure_step.py
 tests/test_utils.py
 tests/data/3TR_model.json
 tests/data/3TR_model.mol2
 tests/data/3TR_model.pdb
 tests/data/3TR_model.sdf
-tests/data/3TR_model.sdf.bz2
-tests/data/3TR_model.sdf.gz
 tests/data/3TR_model.xyz
 tests/data/3TR_model_MN.xyz
 tests/data/Cr_ACETCR.mop
 tests/data/Cu(II)4Br10(2-) (CIVNAW10).mop
 tests/data/RM1 63 Europium, CCDC entry LAPJAN.mop
 tests/data/acetonitrile.mop
 tests/data/lithium fluoride, trimer.mop
 tests/data/methylidyne.mop
 tests/data/potassium fluoride, dimer.mop
 tests/data/spc
-tests/data/spc.xyz
-tests/data/tmQM_test.xyz.bz2
-tests/data/tmQM_test.xyz.gz
+tests/data/spc.xyz
```

### Comparing `read_structure_step-2023.7.27/setup.py` & `read_structure_step-2023.7.6/setup.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/tests/build_filenames.py` & `read_structure_step-2023.7.6/tests/build_filenames.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/tests/data/3TR_model.json` & `read_structure_step-2023.7.6/tests/data/3TR_model.json`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/tests/data/3TR_model.mol2` & `read_structure_step-2023.7.6/tests/data/3TR_model.mol2`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/tests/data/3TR_model.pdb` & `read_structure_step-2023.7.6/tests/data/3TR_model.pdb`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/tests/data/3TR_model.sdf` & `read_structure_step-2023.7.6/tests/data/3TR_model.sdf`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/tests/data/Cr_ACETCR.mop` & `read_structure_step-2023.7.6/tests/data/Cr_ACETCR.mop`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/tests/data/Cu(II)4Br10(2-) (CIVNAW10).mop` & `read_structure_step-2023.7.6/tests/data/Cu(II)4Br10(2-) (CIVNAW10).mop`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/tests/data/RM1 63 Europium, CCDC entry LAPJAN.mop` & `read_structure_step-2023.7.6/tests/data/RM1 63 Europium, CCDC entry LAPJAN.mop`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/tests/data/acetonitrile.mop` & `read_structure_step-2023.7.6/tests/data/acetonitrile.mop`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/tests/data/lithium fluoride, trimer.mop` & `read_structure_step-2023.7.6/tests/data/lithium fluoride, trimer.mop`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/tests/test_formats.py` & `read_structure_step-2023.7.6/tests/test_formats.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 1  2  5          1
 2  2  4          1
 3  1  2          1
 4  1  6          3
 5  2  3          1"""
 
 
-@pytest.fixture()
+@pytest.fixture(scope="module")
 def configuration():
     """Create a system db, system and configuration."""
     db = SystemDB(filename="file:seamm_db?mode=memory&cache=shared")
     system = db.create_system(name="default")
     configuration = system.create_configuration(name="default")
 
     yield configuration
@@ -62,16 +62,14 @@
     "structure",
     [
         "3TR_model.mol2",
         "3TR_model.xyz",
         "3TR_model_MN.xyz",
         "3TR_model.pdb",
         "3TR_model.sdf",
-        "3TR_model.sdf.gz",
-        "3TR_model.sdf.bz2",
     ],
 )
 def test_format(configuration, structure):
     file_name = build_filenames.build_data_filename(structure)
     read_structure_step.read(file_name, configuration)
 
     assert configuration.n_atoms == 10
@@ -368,29 +366,7 @@
         print(configuration.atoms.symbols)
     smiles = configuration.canonical_smiles
     if smiles != check_smiles:
         print(smiles)
 
     assert configuration.atoms.symbols == check_symbols
     assert smiles == check_smiles
-
-
-@pytest.mark.parametrize(
-    "structure",
-    [
-        "tmQM_test.xyz.gz",
-        "tmQM_test.xyz.bz2",
-    ],
-)
-def test_compressed(configuration, structure):
-    file_name = build_filenames.build_data_filename(structure)
-    system = configuration.system
-    system_db = system.system_db
-    read_structure_step.read(
-        file_name,
-        configuration,
-        system_db=system_db,
-        system=system,
-        subsequent_as_configurations=False,
-    )
-
-    assert system_db.n_systems == 7
```

### Comparing `read_structure_step-2023.7.27/tests/test_read_structure_step.py` & `read_structure_step-2023.7.6/tests/test_read_structure_step.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/tests/test_utils.py` & `read_structure_step-2023.7.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.27/versioneer.py` & `read_structure_step-2023.7.6/versioneer.py`

 * *Files identical despite different names*

