# Comparing `tmp/read_structure_step-2023.7.28.tar.gz` & `tmp/read_structure_step-2023.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "read_structure_step-2023.7.28.tar", last modified: Fri Jul 28 10:37:45 2023, max compression
+gzip compressed data, was "read_structure_step-2023.7.6.tar", last modified: Thu Jul  6 20:21:36 2023, max compression
```

## Comparing `read_structure_step-2023.7.28.tar` & `read_structure_step-2023.7.6.tar`

### file list

```diff
@@ -1,129 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:37:45.674717 read_structure_step-2023.7.28/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-07-28 10:37:45.674717 read_structure_step-2023.7.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:37:45.650718 read_structure_step-2023.7.28/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:37:45.654718 read_structure_step-2023.7.28/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/docs/_static/SEAMM inverted.png
--rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:37:45.658717 read_structure_step-2023.7.28/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/docs/api/read_structure_step.formats.cif.rst
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/docs/api/read_structure_step.formats.mol2.rst
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/docs/api/read_structure_step.formats.mop.rst
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/docs/api/read_structure_step.formats.openbabel_io.rst
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/docs/api/read_structure_step.formats.rst
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/docs/api/read_structure_step.formats.sdf.rst
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/docs/api/read_structure_step.formats.smi.rst
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/docs/api/read_structure_step.formats.xyz.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9623 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:37:45.658717 read_structure_step-2023.7.28/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:37:45.658717 read_structure_step-2023.7.28/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)   434049 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/docs/getting_started/dialog.png
--rw-r--r--   0 runner    (1001) docker     (123)   121911 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/docs/getting_started/flowchart.png
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:37:45.662717 read_structure_step-2023.7.28/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:37:45.674717 read_structure_step-2023.7.28/read_structure_step/
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-28 10:37:45.674717 read_structure_step-2023.7.28/read_structure_step/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:37:45.666717 read_structure_step-2023.7.28/read_structure_step/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/data/references.bib
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:37:45.670717 read_structure_step-2023.7.28/read_structure_step/formats/
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/formats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:37:45.670717 read_structure_step-2023.7.28/read_structure_step/formats/cif/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/formats/cif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/formats/cif/cif.py
--rw-r--r--   0 runner    (1001) docker     (123)     8762 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/formats/cif/mmcif.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:37:45.670717 read_structure_step-2023.7.28/read_structure_step/formats/mol2/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/formats/mol2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/formats/mol2/mol2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:37:45.670717 read_structure_step-2023.7.28/read_structure_step/formats/mop/
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/formats/mop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/formats/mop/find_mopac.py
--rw-r--r--   0 runner    (1001) docker     (123)    22956 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/formats/mop/obabel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:37:45.670717 read_structure_step-2023.7.28/read_structure_step/formats/openbabel_io/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/formats/openbabel_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/formats/openbabel_io/checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/formats/openbabel_io/obabel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/formats/registries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:37:45.670717 read_structure_step-2023.7.28/read_structure_step/formats/sdf/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/formats/sdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16229 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/formats/sdf/sdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:37:45.670717 read_structure_step-2023.7.28/read_structure_step/formats/smi/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/formats/smi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/formats/smi/smi.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/formats/which.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:37:45.670717 read_structure_step-2023.7.28/read_structure_step/formats/xyz/
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/formats/xyz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19372 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/formats/xyz/xyz.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/read.py
--rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/read_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/read_structure_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/read_structure_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/tk_read_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/tk_write_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/write.py
--rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/write_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/write_structure_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/read_structure_step/write_structure_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:37:45.666717 read_structure_step-2023.7.28/read_structure_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-07-28 10:37:45.000000 read_structure_step-2023.7.28/read_structure_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-07-28 10:37:45.000000 read_structure_step-2023.7.28/read_structure_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:37:45.000000 read_structure_step-2023.7.28/read_structure_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-28 10:37:45.000000 read_structure_step-2023.7.28/read_structure_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 10:37:45.000000 read_structure_step-2023.7.28/read_structure_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 10:37:45.000000 read_structure_step-2023.7.28/read_structure_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:37:33.000000 read_structure_step-2023.7.28/read_structure_step.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-28 10:37:45.674717 read_structure_step-2023.7.28/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:37:45.670717 read_structure_step-2023.7.28/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/tests/build_filenames.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:37:45.674717 read_structure_step-2023.7.28/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/tests/data/3TR_model.json
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/tests/data/3TR_model.mol2
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/tests/data/3TR_model.pdb
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/tests/data/3TR_model.sdf
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/tests/data/3TR_model.sdf.bz2
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/tests/data/3TR_model.sdf.gz
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/tests/data/3TR_model.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/tests/data/3TR_model_MN.xyz
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/tests/data/Cr_ACETCR.mop
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/tests/data/Cu(II)4Br10(2-) (CIVNAW10).mop
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/tests/data/RM1 63 Europium, CCDC entry LAPJAN.mop
--rwxr-xr-x   0 runner    (1001) docker     (123)      658 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/tests/data/acetonitrile.mop
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/tests/data/lithium fluoride, trimer.mop
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/tests/data/methylidyne.mop
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/tests/data/potassium fluoride, dimer.mop
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/tests/data/spc
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/tests/data/spc.xyz
--rw-r--r--   0 runner    (1001) docker     (123)    13395 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/tests/data/tmQM_test.xyz.bz2
--rw-r--r--   0 runner    (1001) docker     (123)    16514 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/tests/data/tmQM_test.xyz.gz
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/tests/methylidyne.mop
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/tests/mopac_exists.py
--rw-r--r--   0 runner    (1001) docker     (123)     9538 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/tests/test_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/tests/test_read_structure_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-28 10:37:29.000000 read_structure_step-2023.7.28/versioneer.py
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

### Comparing `read_structure_step-2023.7.28/CONTRIBUTING.rst` & `read_structure_step-2023.7.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/HISTORY.rst` & `read_structure_step-2023.7.6/HISTORY.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,11 @@
 =======
 History
 =======
 
-2023.7.28 -- Implemented ranges for reading XYZ and SDF files.
-
-2023.7.27.1 -- Removed debug printing.
-
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

### Comparing `read_structure_step-2023.7.28/LICENSE` & `read_structure_step-2023.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/PKG-INFO` & `read_structure_step-2023.7.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: read_structure_step
-Version: 2023.7.28
+Version: 2023.7.6
 Summary: A SEAMM plug-in to read common formats in computational chemistry
 Home-page: https://github.com/molssi-seamm/read_structure_step
 Author: Eliseo Marin-R-Rimoldi
 Author-email: meliseo@vt.edu
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,Open Babel,molecules,atomistic,files
 Platform: Linux
@@ -101,22 +101,14 @@
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
 
-2023.7.28 -- Implemented ranges for reading XYZ and SDF files.
-
-2023.7.27.1 -- Removed debug printing.
-
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

### Comparing `read_structure_step-2023.7.28/README.rst` & `read_structure_step-2023.7.6/README.rst`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/docs/Makefile` & `read_structure_step-2023.7.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/docs/_static/SEAMM inverted.png` & `read_structure_step-2023.7.6/docs/_static/SEAMM inverted.png`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/docs/_static/SEAMM logo.png` & `read_structure_step-2023.7.6/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/docs/_static/molssi_main_logo.png` & `read_structure_step-2023.7.6/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/docs/_static/molssi_main_logo_inverted_white.png` & `read_structure_step-2023.7.6/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/docs/_static/molssi_square.png` & `read_structure_step-2023.7.6/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/docs/_static/nsf.png` & `read_structure_step-2023.7.6/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/docs/api/read_structure_step.formats.cif.rst` & `read_structure_step-2023.7.6/docs/api/read_structure_step.formats.cif.rst`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/docs/api/read_structure_step.formats.mop.rst` & `read_structure_step-2023.7.6/docs/api/read_structure_step.formats.mop.rst`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/docs/api/read_structure_step.formats.openbabel_io.rst` & `read_structure_step-2023.7.6/docs/api/read_structure_step.formats.openbabel_io.rst`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/docs/api/read_structure_step.formats.rst` & `read_structure_step-2023.7.6/docs/api/read_structure_step.formats.rst`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/docs/conf.py` & `read_structure_step-2023.7.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/docs/developer_guide/installation.rst` & `read_structure_step-2023.7.6/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/docs/getting_started/dialog.png` & `read_structure_step-2023.7.6/docs/getting_started/dialog.png`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/docs/getting_started/flowchart.png` & `read_structure_step-2023.7.6/docs/getting_started/flowchart.png`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/docs/getting_started/index.rst` & `read_structure_step-2023.7.6/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/docs/index.rst` & `read_structure_step-2023.7.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/docs/make.bat` & `read_structure_step-2023.7.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/read_structure_step/__init__.py` & `read_structure_step-2023.7.6/read_structure_step/__init__.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/read_structure_step/data/references.bib` & `read_structure_step-2023.7.6/read_structure_step/data/references.bib`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/read_structure_step/errors.py` & `read_structure_step-2023.7.6/read_structure_step/errors.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/read_structure_step/formats/__init__.py` & `read_structure_step-2023.7.6/read_structure_step/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/read_structure_step/formats/cif/cif.py` & `read_structure_step-2023.7.6/read_structure_step/formats/cif/cif.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/read_structure_step/formats/cif/mmcif.py` & `read_structure_step-2023.7.6/read_structure_step/formats/cif/mmcif.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/read_structure_step/formats/mol2/mol2.py` & `read_structure_step-2023.7.6/read_structure_step/formats/mol2/mol2.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/read_structure_step/formats/mop/__init__.py` & `read_structure_step-2023.7.6/read_structure_step/formats/mop/__init__.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/read_structure_step/formats/mop/find_mopac.py` & `read_structure_step-2023.7.6/read_structure_step/formats/mop/find_mopac.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/read_structure_step/formats/mop/obabel.py` & `read_structure_step-2023.7.6/read_structure_step/formats/mop/obabel.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/read_structure_step/formats/openbabel_io/checkers.py` & `read_structure_step-2023.7.6/read_structure_step/formats/openbabel_io/checkers.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/read_structure_step/formats/openbabel_io/obabel.py` & `read_structure_step-2023.7.6/read_structure_step/formats/openbabel_io/obabel.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/read_structure_step/formats/registries.py` & `read_structure_step-2023.7.6/read_structure_step/formats/registries.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/read_structure_step/formats/sdf/sdf.py` & `read_structure_step-2023.7.6/read_structure_step/formats/sdf/sdf.py`

 * *Files 5% similar despite different names*

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
 
@@ -130,85 +129,55 @@
 
     if isinstance(path, str):
         path = Path(path)
 
     path.expanduser().resolve()
 
     # Get the information for progress output, if requested.
-    n_structures = 0
-    with (
-        gzip.open(path, mode="rt")
-        if path.suffix == ".gz"
-        else bz2.open(path, mode="rt")
-        if path.suffix == ".bz2"
-        else open(path, "r")
-    ) as fd:
-        for line in fd:
-            if line[0:4] == "$$$$":
-                n_structures += 1
+    compress = path.suffix == ".gz"
     if printer is not None:
+        n_structures = 0
+        with gzip.open(path, mode="rt") if compress else open(path, "r") as fd:
+            for line in fd:
+                if line[0:4] == "$$$$":
+                    n_structures += 1
         printer("")
         printer(f"    The SDF file contains {n_structures} structures.")
         last_percent = 0
         t0 = time.time()
         last_t = t0
 
-    # Get the indices to pick
-    tmp = indices.replace("end", str(n_structures + 1))
-    tmp = tmp.split(":")
-    start = int(tmp[0])
-    if len(tmp) == 3:
-        step = int(tmp[2])
-    else:
-        step = 1
-    if len(tmp) == 2:
-        stop = int(tmp[1])
-    else:
-        stop = start + 1
-    indices = list(range(start, stop, step))
-
     obConversion = openbabel.OBConversion()
     obConversion.SetInAndOutFormats("sdf", "smi")
 
     configurations = []
-    structure_no = 0
+    structure_no = 1
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
 
-            structure_no += 1
-            if structure_no >= stop:
-                break
-            if structure_no not in indices:
-                continue
-
             obConversion.ReadString(obMol, text)
 
             if add_hydrogens:
                 obMol.AddHydrogens()
 
             if structure_no > 1:
                 if subsequent_as_configurations:
                     configuration = system.create_configuration()
                 else:
                     system = system_db.create_system()
                     configuration = system.create_configuration()
 
+            structure_no += 1
             try:
                 configuration.from_OBMol(obMol)
             except Exception as e:
                 n_errors += 1
                 printer("")
                 printer(f"    Error handling entry {structure_no} in the SDF file:")
                 printer("        " + str(e))
```

### Comparing `read_structure_step-2023.7.28/read_structure_step/formats/smi/smi.py` & `read_structure_step-2023.7.6/read_structure_step/formats/smi/smi.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/read_structure_step/formats/xyz/__init__.py` & `read_structure_step-2023.7.6/read_structure_step/formats/xyz/__init__.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/read_structure_step/read.py` & `read_structure_step-2023.7.6/read_structure_step/read.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 def read(
     file_name,
     configuration,
     extension=None,
     add_hydrogens=False,
     system_db=None,
     system=None,
-    indices="1:end",
+    indices=None,
     subsequent_as_configurations=False,
     system_name=None,
     configuration_name=None,
     printer=None,
     references=None,
     bibliography=None,
 ):
```

### Comparing `read_structure_step-2023.7.28/read_structure_step/read_structure.py` & `read_structure_step-2023.7.6/read_structure_step/read_structure.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/read_structure_step/read_structure_parameters.py` & `read_structure_step-2023.7.6/read_structure_step/read_structure_parameters.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/read_structure_step/read_structure_step.py` & `read_structure_step-2023.7.6/read_structure_step/read_structure_step.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/read_structure_step/tk_read_structure.py` & `read_structure_step-2023.7.6/read_structure_step/tk_read_structure.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/read_structure_step/tk_write_structure.py` & `read_structure_step-2023.7.6/read_structure_step/tk_write_structure.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/read_structure_step/utils.py` & `read_structure_step-2023.7.6/read_structure_step/utils.py`

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

### Comparing `read_structure_step-2023.7.28/read_structure_step/write.py` & `read_structure_step-2023.7.6/read_structure_step/write.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/read_structure_step/write_structure.py` & `read_structure_step-2023.7.6/read_structure_step/write_structure.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/read_structure_step/write_structure_parameters.py` & `read_structure_step-2023.7.6/read_structure_step/write_structure_parameters.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/read_structure_step/write_structure_step.py` & `read_structure_step-2023.7.6/read_structure_step/write_structure_step.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/read_structure_step.egg-info/PKG-INFO` & `read_structure_step-2023.7.6/read_structure_step.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: read-structure-step
-Version: 2023.7.28
+Version: 2023.7.6
 Summary: A SEAMM plug-in to read common formats in computational chemistry
 Home-page: https://github.com/molssi-seamm/read_structure_step
 Author: Eliseo Marin-R-Rimoldi
 Author-email: meliseo@vt.edu
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,Open Babel,molecules,atomistic,files
 Platform: Linux
@@ -101,22 +101,14 @@
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
 
-2023.7.28 -- Implemented ranges for reading XYZ and SDF files.
-
-2023.7.27.1 -- Removed debug printing.
-
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

### Comparing `read_structure_step-2023.7.28/read_structure_step.egg-info/SOURCES.txt` & `read_structure_step-2023.7.6/read_structure_step.egg-info/SOURCES.txt`

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

### Comparing `read_structure_step-2023.7.28/setup.py` & `read_structure_step-2023.7.6/setup.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/tests/build_filenames.py` & `read_structure_step-2023.7.6/tests/build_filenames.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/tests/data/3TR_model.json` & `read_structure_step-2023.7.6/tests/data/3TR_model.json`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/tests/data/3TR_model.mol2` & `read_structure_step-2023.7.6/tests/data/3TR_model.mol2`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/tests/data/3TR_model.pdb` & `read_structure_step-2023.7.6/tests/data/3TR_model.pdb`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/tests/data/3TR_model.sdf` & `read_structure_step-2023.7.6/tests/data/3TR_model.sdf`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/tests/data/Cr_ACETCR.mop` & `read_structure_step-2023.7.6/tests/data/Cr_ACETCR.mop`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/tests/data/Cu(II)4Br10(2-) (CIVNAW10).mop` & `read_structure_step-2023.7.6/tests/data/Cu(II)4Br10(2-) (CIVNAW10).mop`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/tests/data/RM1 63 Europium, CCDC entry LAPJAN.mop` & `read_structure_step-2023.7.6/tests/data/RM1 63 Europium, CCDC entry LAPJAN.mop`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/tests/data/acetonitrile.mop` & `read_structure_step-2023.7.6/tests/data/acetonitrile.mop`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/tests/data/lithium fluoride, trimer.mop` & `read_structure_step-2023.7.6/tests/data/lithium fluoride, trimer.mop`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/tests/test_formats.py` & `read_structure_step-2023.7.6/tests/test_formats.py`

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

### Comparing `read_structure_step-2023.7.28/tests/test_read_structure_step.py` & `read_structure_step-2023.7.6/tests/test_read_structure_step.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/tests/test_utils.py` & `read_structure_step-2023.7.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.7.28/versioneer.py` & `read_structure_step-2023.7.6/versioneer.py`

 * *Files identical despite different names*

