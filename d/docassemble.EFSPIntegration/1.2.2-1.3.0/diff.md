# Comparing `tmp/docassemble.EFSPIntegration-1.2.2.tar.gz` & `tmp/docassemble.EFSPIntegration-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docassemble.EFSPIntegration-1.2.2.tar", last modified: Thu Jun  1 15:09:21 2023, max compression
+gzip compressed data, was "docassemble.EFSPIntegration-1.3.0.tar", last modified: Fri Jul 28 16:30:06 2023, max compression
```

## Comparing `docassemble.EFSPIntegration-1.2.2.tar` & `docassemble.EFSPIntegration-1.3.0.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 15:09:21.426988 docassemble.EFSPIntegration-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      812 2023-06-01 15:09:21.426988 docassemble.EFSPIntegration-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      668 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 15:09:21.418988 docassemble.EFSPIntegration-1.2.2/docassemble/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 15:09:21.422988 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    30386 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/conversions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 15:09:21.418988 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 15:09:21.422988 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/questions/
--rw-r--r--   0 runner    (1001) docker     (122)    40916 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/questions/admin_interview.yml
--rw-r--r--   0 runner    (1001) docker     (122)    26764 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/questions/any_filing_interview.yml
--rw-r--r--   0 runner    (1001) docker     (122)    20187 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/questions/case_search.yml
--rw-r--r--   0 runner    (1001) docker     (122)    32169 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/questions/efiling_integration.yml
--rw-r--r--   0 runner    (1001) docker     (122)     9637 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/questions/login_qs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1953 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/questions/minimal_interview.yml
--rw-r--r--   0 runner    (1001) docker     (122)    12606 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/questions/toga_payments.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/questions/toga_payments_interview.yml
--rw-r--r--   0 runner    (1001) docker     (122)     4393 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/questions/unauthenticated_actions.yml
--rw-r--r--   0 runner    (1001) docker     (122)      729 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/questions/unauthenticated_interview.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 15:09:21.422988 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/sources/
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/sources/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     7289 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/sources/admin_interview.feature
--rw-r--r--   0 runner    (1001) docker     (122)     8923 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/sources/any_filing_interview.feature
--rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/sources/example_upload.pdf
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/sources/unauthenticated_interview.feature
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 15:09:21.422988 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/static/
--rw-r--r--   0 runner    (1001) docker     (122)     3208 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/static/Ajax-loader.gif
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/static/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 15:09:21.422988 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/templates/README.md
--rw-r--r--   0 runner    (1001) docker     (122)    14390 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/efm_client.py
--rw-r--r--   0 runner    (1001) docker     (122)    15778 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/interview_logic.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    38477 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/py_efsp_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 15:09:21.426988 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18552 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/test/integration_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     7090 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/test/peoria_to_cr.json
--rw-r--r--   0 runner    (1001) docker     (122)   238595 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/test/temp2.json
--rw-r--r--   0 runner    (1001) docker     (122)     5698 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/test/test_conversions.py
--rw-r--r--   0 runner    (1001) docker     (122)    55792 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/test/vars.json
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/docassemble/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 15:09:21.422988 docassemble.EFSPIntegration-1.2.2/docassemble.EFSPIntegration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      812 2023-06-01 15:09:21.000000 docassemble.EFSPIntegration-1.2.2/docassemble.EFSPIntegration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2174 2023-06-01 15:09:21.000000 docassemble.EFSPIntegration-1.2.2/docassemble.EFSPIntegration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 15:09:21.000000 docassemble.EFSPIntegration-1.2.2/docassemble.EFSPIntegration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-01 15:09:21.000000 docassemble.EFSPIntegration-1.2.2/docassemble.EFSPIntegration.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 15:09:21.000000 docassemble.EFSPIntegration-1.2.2/docassemble.EFSPIntegration.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-01 15:09:21.000000 docassemble.EFSPIntegration-1.2.2/docassemble.EFSPIntegration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-01 15:09:21.000000 docassemble.EFSPIntegration-1.2.2/docassemble.EFSPIntegration.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-01 15:09:21.426988 docassemble.EFSPIntegration-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-06-01 15:09:10.000000 docassemble.EFSPIntegration-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 16:30:06.851148 docassemble.EFSPIntegration-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      812 2023-07-28 16:30:06.851148 docassemble.EFSPIntegration-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      668 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 16:30:06.843148 docassemble.EFSPIntegration-1.3.0/docassemble/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 16:30:06.847148 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35662 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 16:30:06.843148 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 16:30:06.847148 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/questions/
+-rw-r--r--   0 runner    (1001) docker     (122)    40822 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/questions/admin_interview.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    26752 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/questions/any_filing_interview.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    20201 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/questions/case_search.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    32550 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/questions/efiling_integration.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    10563 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/questions/login_qs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1953 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/questions/minimal_interview.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    12606 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/questions/toga_payments.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      966 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/questions/toga_payments_interview.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     4665 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/questions/unauthenticated_actions.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/questions/unauthenticated_interview.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 16:30:06.847148 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/sources/
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/sources/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     7289 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/sources/admin_interview.feature
+-rw-r--r--   0 runner    (1001) docker     (122)     8117 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/sources/any_filing_interview.feature
+-rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/sources/example_upload.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/sources/unauthenticated_interview.feature
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 16:30:06.851148 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/static/
+-rw-r--r--   0 runner    (1001) docker     (122)     3208 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/static/Ajax-loader.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/static/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 16:30:06.851148 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)    14390 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/efm_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16496 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/interview_logic.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)    38549 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/py_efsp_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 16:30:06.851148 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20832 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/test/integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    54217 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/test/opening_affidavit_adams.json
+-rw-r--r--   0 runner    (1001) docker     (122)     7090 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/test/peoria_to_cr.json
+-rw-r--r--   0 runner    (1001) docker     (122)   238595 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/test/temp2.json
+-rw-r--r--   0 runner    (1001) docker     (122)     5698 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/test/test_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    55792 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/test/vars.json
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/docassemble/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 16:30:06.843148 docassemble.EFSPIntegration-1.3.0/docassemble.EFSPIntegration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      812 2023-07-28 16:30:06.000000 docassemble.EFSPIntegration-1.3.0/docassemble.EFSPIntegration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2236 2023-07-28 16:30:06.000000 docassemble.EFSPIntegration-1.3.0/docassemble.EFSPIntegration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-28 16:30:06.000000 docassemble.EFSPIntegration-1.3.0/docassemble.EFSPIntegration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-28 16:30:06.000000 docassemble.EFSPIntegration-1.3.0/docassemble.EFSPIntegration.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-28 16:30:06.000000 docassemble.EFSPIntegration-1.3.0/docassemble.EFSPIntegration.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-28 16:30:06.000000 docassemble.EFSPIntegration-1.3.0/docassemble.EFSPIntegration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-28 16:30:06.000000 docassemble.EFSPIntegration-1.3.0/docassemble.EFSPIntegration.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-28 16:30:06.851148 docassemble.EFSPIntegration-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-07-28 16:29:57.000000 docassemble.EFSPIntegration-1.3.0/setup.py
```

### Comparing `docassemble.EFSPIntegration-1.2.2/LICENSE` & `docassemble.EFSPIntegration-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.2/PKG-INFO` & `docassemble.EFSPIntegration-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docassemble.EFSPIntegration
-Version: 1.2.2
+Version: 1.3.0
 Home-page: https://github.com/SuffolkLITLab/docassemble-EFSPIntegration
 Author: Bryce Willey
 Author-email: bwilley@suffolk.edu
 License: The MIT License (MIT)
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `docassemble.EFSPIntegration-1.2.2/README.md` & `docassemble.EFSPIntegration-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/conversions.py` & `docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/conversions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 """Functions that help convert the JSON-ized XML from the proxy server into usable information."""
 
 import re
+import tempfile
+import json
 from datetime import datetime, timezone
 from typing import List, Dict, Tuple, Any, Mapping, Callable, Optional, Union
 import docassemble.base.util
 from docassemble.base.util import (
     DADict,
     DAList,
     DAObject,
     DADateTime,
     as_datetime,
     validation_error,
     log,
     as_datetime,
+    user_info,
+    send_email,
 )
 from docassemble.AssemblyLine.al_general import ALIndividual, ALAddress
 from docassemble.base.functions import get_config
 from .efm_client import ApiResponse, ProxyConnection
 import importlib
 import dateutil.parser
 
@@ -35,19 +39,156 @@
     "_payment_type",
     "_payment_labels",
     "_payment_expiration",
     "filter_payment_accounts",
     "payment_account_labels",
     "filing_id_and_label",
     "get_tyler_roles",
+    "log_error_and_notify",
 ]
 
 TypeType = type(type(None))
 
 
+def error_notification(err, message=None, trace=None, referer=None, the_vars=None):
+    """Copied from docassemble.webapp.server.error_notification, since:
+    1) things from webapp.* are unstable
+    2) it breaks the unit tests and the mypy
+
+    Some slight modifications to work without server backends
+    """
+    recipient_email = get_config("error notification email", None)
+    if not recipient_email:
+        return
+    if (
+        err.__class__.__name__
+        in ["CSRFError", "ClientDisconnected", "MethodNotAllowed", "DANotFoundError"]
+        + ERROR_TYPES_NO_EMAIL
+    ):
+        return
+    email_recipients = []
+    if isinstance(recipient_email, list):
+        email_recipients.extend(recipient_email)
+    else:
+        email_recipients.append(recipient_email)
+    if message is None:
+        errmess = str(err)
+    else:
+        errmess = message
+    try:
+        email_address = user_info().email
+    except:
+        email_address = None
+    referer = None
+    if get_config("error notification variables", get_config("debug", True)):
+        if the_vars is None:
+            try:
+                the_vars = docassemble.base.functions.all_variables(
+                    include_internal=True
+                )
+            except:
+                pass
+    else:
+        the_vars = None
+    json_filename = None
+    if the_vars is not None and len(the_vars):
+        try:
+            with tempfile.NamedTemporaryFile(
+                mode="w",
+                prefix="datemp",
+                suffix=".json",
+                delete=False,
+                encoding="utf-8",
+            ) as fp:
+                fp.write(json.dumps(the_vars, sort_keys=True, indent=2))
+                json_filename = fp.name
+        except:
+            pass
+    interview_path = docassemble.base.functions.interview_path()
+    try:
+        try:
+            appname = get_config("appname", "docassemble")
+            html = (
+                "<html>\n  <body>\n    <p>There was an error in the "
+                + appname
+                + " application.</p>\n    <p>The error message was:</p>\n<pre>"
+                + err.__class__.__name__
+                + ": "
+                + str(errmess)
+                + "</pre>\n"
+            )
+            body = (
+                "There was an error in the "
+                + appname
+                + " application.\n\nThe error message was:\n\n"
+                + err.__class__.__name__
+                + ": "
+                + str(errmess)
+            )
+            if trace is not None:
+                body += "\n\n" + str(trace)
+                html += "<pre>" + str(trace) + "</pre>"
+            if referer is not None and referer != "None":
+                body += "\n\nThe referer URL was " + str(referer)
+                html += "<p>The referer URL was " + str(referer) + "</p>"
+            elif interview_path is not None:
+                body += "\n\nThe interview was " + str(interview_path)
+                html += "<p>The interview was " + str(interview_path) + "</p>"
+            if email_address is not None:
+                body += "\n\nThe user was " + str(email_address)
+                html += "<p>The user was " + str(email_address) + "</p>"
+            if trace is not None:
+                body += "\n\n" + str(trace)
+                html += "<pre>" + str(trace) + "</pre>"
+            if get_config("external hostname", None) is not None:
+                body += "\n\nThe external hostname was " + str(
+                    get_config("external hostname")
+                )
+                html += (
+                    "<p>The external hostname was "
+                    + str(get_config("external hostname"))
+                    + "</p>"
+                )
+            html += "\n  </body>\n</html>"
+            log(f"Trying to send error message {body}")
+            send_email(
+                subject=appname + " error: " + err.__class__.__name,
+                to=email_recipients,
+                body=body,
+                html=html,
+                attachments=[json_filename],
+            )
+        except Exception as zerr:
+            log(str(zerr))
+            body = "There was an error in the " + appname + " application."
+            html = (
+                "<html>\n  <body>\n    <p>There was an error in the "
+                + appname
+                + " application.</p>\n  </body>\n</html>"
+            )
+            log(f"Trying to send error message {body}")
+            send_email(
+                subject=appname + " error: " + err.__class__.__name__,
+                to=email_recipients,
+                body=body,
+                html=html,
+                attachments=[json_filename],
+            )
+    except:
+        pass
+
+
+def log_error_and_notify(context: str, resp: Optional[ApiResponse] = None):
+    """Similar to docassemble.webapp.server.error_notification, which will send an email to
+    the `error_notification_email` in the config."""
+    message = f"context: {context};; resp: {resp}"
+    log(f"EFSPIntegration ERROR: {message}")
+    error_notification(resp, message=message)
+
+
 def convert_court_to_id(trial_court) -> str:
     """Converts a court type to the specific id string expected by Tyler.
 
     A fairly ad-hoc function; it will check if the object has several attributes
     ("tyler_court_code", "tyler_code", or "name"), or if it's already a string, it
     tries to just make a lower case on the string. We strongly recommend that
     your court object use the "tyler_court_code" attribute though.
@@ -562,16 +703,17 @@
     if not roles:
         roles = {}
 
     # NOTE: case court can change from searched location (i.e. search in peoria can find cases
     # in peoriacr); using the original here, but can change it here if necessary
     full_case_details = proxy_conn.get_case(new_case.court_id, new_case.tracking_id)
     if not full_case_details.is_ok():
-        log(
-            f"couldn't get full details for {new_case.court_id}-{ new_case.tracking_id}: {full_case_details}"
+        log_error_and_notify(
+            f"couldn't get full details for {new_case.court_id}-{ new_case.tracking_id}",
+            full_case_details,
         )
     new_case.attorneys = DADict(
         new_case.instanceName + ".attorneys",
         object_type=ALIndividual,
         auto_gather=False,
     )
     new_case.party_to_attorneys = {}
@@ -719,15 +861,17 @@
     """Returns all payment accounts as choices, without filters."""
     if resp.data:
         return [
             {account.get("paymentAccountID"): _payment_labels(account)}
             for account in resp.data
         ]
     else:
-        log(f"payment_account_labels: {resp}")
+        log_error_and_notify(
+            "payment_account_labels couldn't build from failed response", resp
+        )
         return []
 
 
 def filing_id_and_label(case: Mapping, style: str = "FILING_ID") -> Dict[str, str]:
     """Converts a raw case information from [proxy_conn.get_filing_list()](py_efsp_client#get_filing_list)
     into a key-value pair, where the key is the filing id and the value is the user-facing label
     for that filing.
```

### Comparing `docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/questions/admin_interview.yml` & `docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/questions/admin_interview.yml`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,16 @@
   - case_search.yml
   - toga_payments.yml
   - docassemble.AssemblyLine:al_package.yml
 ---
 features:
   question back button: True
   navigation back button: False
+  custom datatypes to load:
+    - ALVisiblePassword
 ---
 default screen parts:
   back button label: |
     Back
 ---
 metadata:
   title: |
@@ -1289,27 +1291,21 @@
 ---
 event: show_error_event
 question: |
   Error
 subquestion: |
   ${ error_message }
 ---
-id: which-jurisdiction
-question: |
-  Which jurisdiction?
-fields:
-  - no label: jurisdiction_id
-    choices:
-      - Illinois: 'illinois'
-      - Massachusetts: 'massachusetts'
-      - Texas: 'texas'
----
-code: |
-  if 'jurisdiction_id' in url_args:
-    jurisdiction_id = url_args['jurisdiction_id']
+variable name: jurisdiction_names
+data:
+  illinois: Illinois
+  massachusetts: Massachusetts
+  texas: Texas
+  california: California
+  indiana: Indiana
 ---
 code: |
   case_category_options, case_category_map = choices_and_map(proxy_conn.get_case_categories(court_id, fileable_only=False, timing=None).data)
 ---
 comment: |
   Overrides login_qs: all jurisdictions allowed here are Tyler
 depends on:
```

### Comparing `docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/questions/any_filing_interview.yml` & `docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/questions/any_filing_interview.yml`

 * *Files 1% similar despite different names*

```diff
@@ -9,23 +9,21 @@
   - efiling_integration.yml
   - docassemble.AssemblyLine:al_package.yml
   - case_search.yml
 ---
 code: |
   user_wants_efile = True # This interview is always for e-filing
 ---
-id: which-jurisdiction
-question: |
-  Which jurisdiction?
-fields:
-  - no label: jurisdiction_id
-    choices:
-      - Illinois: 'illinois'
-      - Massachusetts: 'massachusetts'
-      - Texas: 'texas'
+variable name: jurisdiction_names
+data:
+  illinois: Illinois
+  massachusetts: Massachusetts
+  texas: Texas
+  california: California
+  indiana: Indiana
 ---
 objects:
   - case_search: EFCaseSearch.using(court_id=court_id)
   - lower_court_case: DAObject
 ---
 code: |
   efile_case_category_filters = []
@@ -538,15 +536,15 @@
 id: your name
 sets:
     - users[0].name.first
 question:  |
   What is your name?
 fields:
   - code: |
-      users[0].name_fields(person_or_business='unknown' if not users[0].is_form_filler else 'ALIndividual', show_suffix=False)
+      users[0].name_fields(person_or_business='ALIndividual' if hasattr(users[0], 'is_form_filler') and users[0].is_form_filler else 'unknown', show_suffix=False)
 ---
 sets:
   - users[i].name.first
   - users[i].name.last
 id: other users names
 question: |
   What is the name of the ${ ordinal(i) } person who is part of the case with you?
```

### Comparing `docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/questions/case_search.yml` & `docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/questions/case_search.yml`

 * *Files 0% similar despite different names*

```diff
@@ -243,15 +243,15 @@
 generic object: EFCaseSearch
 code: |
   x.party_type_map = all_party_type_map
 ---
 id: docket id
 generic object: EFCaseSearch
 question: |
-  ${ str(x.docket_lookup_choice) }
+  What is your ${ str(x.docket_lookup_choice) }?
 subquestion: |
   ${ collapse_template(x.case_number_format_template) }
 
 fields:
   - ${ str(x.docket_lookup_choice) }: x.docket_number_from_user
 ---
 id: ask non-indexed docket number
```

### Comparing `docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/questions/efiling_integration.yml` & `docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/questions/efiling_integration.yml`

 * *Files 2% similar despite different names*

```diff
@@ -218,23 +218,24 @@
 ---
 if: can_check_efile
 need:
   - efile_author_mode
 id: ready_to_efile
 code: |
   # Ask for the clerk comments, they'll go in the lead filing doc comments
+  ready_to_efile_user_hook
   check_resp
   remaining_to_check = check_resp.data
   log('check_resp: ' + str(check_resp))
   if not check_resp.is_ok():
     ready_to_efile = False
     if efile_author_mode:
       show_remaining
     else:
-      log(f'Something went wrong: {check_resp.error_msg}')
+      log_error_and_notify('Check response failed', check_resp)
   elif not remaining_to_check.get("required_vars") and not remaining_to_check.get("wrong_vars"):
     ready_to_efile = True
   else:
     if efile_author_mode:
       show_remaining
       follow_up_setup
       for key in follow_up_vars.keys():
@@ -245,20 +246,24 @@
       log(f"Couldn't efile, remaining_to_check: {remaining_to_check}")
       fallback_user_choice
   globals().pop('check_resp', None)
 
   if not ready_to_efile:
     show_no_efile
 ---
+code: |
+  ready_to_efile_user_hook = True
+---
 id: actually efile
 depends on:
   - can_check_efile
   - user_wants_efile
 if: can_check_efile and user_wants_efile and ready_to_efile
 code: |
+  tyler_payment_id
   efile_user_reviewed
   if not efile_author_mode:
     prevent_going_back()
   efile_resp
   show_efile_resp
   # TODO(brycew): This is a bit hacky. Should have a proxy call for enabled features
   if efile_resp.is_ok() and proxy_conn.default_jurisdiction != 'louisiana' and submitted_court_reserve_resp.is_ok():
@@ -495,15 +500,15 @@
   - x.optional_services_filters
 code: |
   x.optional_services.clear()
   for opt_srv_default, opt_srv_filter in zip(x.optional_services_defaults, x.optional_services_filters):
     opt_srv_options, opt_srv_code = filter_codes(x.optional_service_options, opt_srv_filter, opt_srv_default)
     if opt_srv_code is None:
       # We shouldn't automatically add things, but should pay attention to:
-      log(f"Can't find optional service for {x.filing_code} at {court_id}, {opt_srv_filter}")
+      log(f"Can't find optional service for {x.filing_type} at {court_id}, {opt_srv_filter}, these options: {x.optional_service_options}")
     else:
       new_opt_srv = x.optional_services.appendObject()
       new_opt_srv.code = opt_srv_code
   x.added_necessary_opt_services = True
 ---
 generic object: DAObject
 code: |
@@ -601,19 +606,25 @@
 if: len(x.document_type_options) == 1
 code: |
   x.document_type = x.document_type_options[0][0]
 ---
 generic object: DAObject
 code: |
   x.document_type_filters = []
+---
+generic object: DAObject
+code: |
   x.document_type_default = None
 ---
 generic object: DAObject
 code: |
   x.filing_type_filters = []
+---
+generic object: DAObject
+code: |
   x.filing_type_default = None
 ---
 generic object: DAObject
 code: |
   x.filing_component_filters = []
   x.filing_component_default = None
 ---
@@ -781,24 +792,27 @@
 ---
 code: |
   service_contact_options = parse_service_contacts(proxy_conn.get_service_contact_list().data)
 ---
 code: |
   admin_interview = "docassemble.EFSPIntegration:admin_interview.yml"
 ---
+code: |
+  toga_interview = "docassemble.EFSPIntegration:toga_payments_interview.yml"
+---
 ############ Payments Stuff ############
 reconsider:
   - tyler_payment_account_options
 id: payment account
 question: |
   Payment Account
 subquestion: |
   Select an existing account below, or add a payment account
   using the 
-  [Admin Interface](${ interview_url(i=admin_interview, reset=1, jurisdiction_id=jurisdiction_id) }){:target="_blank"}
+  [payments screen](${ interview_url(i=toga_interview, reset=1, jurisdiction_id=jurisdiction_id) }){:target="_blank"}
   
   Refresh this page when you have finished adding the account.
 fields:
   - Payment Account: tyler_payment_id
     datatype: dropdown
     code: |
       tyler_payment_account_options
@@ -809,18 +823,18 @@
 code: |
   allowable_card_types = full_court_info.get('allowablecardtypes', [])
   res = proxy_conn.get_payment_account_list().data
   if res:
     tyler_payment_account_options = filter_payment_accounts(res, allowable_card_types)
   else:
     tyler_payment_account_options = []
-
-  res = proxy_conn.get_global_payment_account_list().data
-  if res:
-    tyler_payment_account_options.extend(filter_payment_accounts(res, allowable_card_types))
+  # For now, don't show global options for payment accounts.
+  #res = proxy_conn.get_global_payment_account_list().data
+  #if res:
+  #  tyler_payment_account_options.extend(filter_payment_accounts(res, allowable_card_types))
 ---
 ################################
 ## Fees
 id: review_fees_screen
 question: |
   Review filing fees
 subquestion: |
@@ -856,15 +870,15 @@
   - fees_resp
 code: |
   has_fees = fee_total(fees_resp) and fee_total(fees_resp) > 0
 ---
 code: |
   fees_resp = proxy_conn.calculate_filing_fees(court_id, al_court_bundle)
   if not fees_resp.is_ok():
-    log(f'fees not ok! {fees_resp}')
+    log_error_and_notify('Fees not ok', fees_resp)
 ---
 depends on:
   - fees_resp
 table: fees_table
 rows: |
   [fee for fee in fees_resp.data.get('allowanceCharge',[]) if fee.get('chargeIndicator',{}).get('value')]
 columns:
```

### Comparing `docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/questions/login_qs.yml` & `docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/questions/login_qs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -52,17 +52,19 @@
   tyler_login = True
 ---
 need:
   - proxy_conn
   - da_store
 code: |
     tyler_header_name = f"TYLER-TOKEN-{jurisdiction_id.upper()}"
+    tyler_id_name = f"TYLER-ID-{jurisdiction_id}"
     try:
       if da_store.defined("EFSP-" + tyler_header_name):
         proxy_conn.proxy_client.headers[tyler_header_name] = da_store.get("EFSP-" + tyler_header_name)
+        proxy_conn.proxy_client.headers[tyler_id_name] = da_store.get("EFSP-" + tyler_id_name)
         tyler_user = proxy_conn.get_user()
         if tyler_user.is_ok():
           my_username = tyler_user.data.get('email')
           if continue_stored_login:
             log(word("You are now connected to your e-filing account") + f" ({my_username})", "primary")
             logged_in_user_is_admin, logged_in_user_is_global_admin = get_tyler_roles(proxy_conn, None, tyler_user)
             tyler_login = True
@@ -285,18 +287,14 @@
   You will *not* be able to e-file this document
 subquestion: |
   Unfortunately, you cannot e-file this document at ${ trial_court } through this program.
 
   However, you can still continue and download a completed form at the end.
 continue button field: show_no_efile
 ---
-depends on:
-  - court_id
-  - available_efile_courts
-only sets: efile_setup
 code: |
   efile_setup = court_id in available_efile_courts
 ---
 id: check efile possibility
 sets:
   - can_check_efile
 code: |
@@ -306,8 +304,36 @@
   else:
     show_no_efile
     can_check_efile = False
 ---
 only sets: full_court_info
 code: |
   full_court_info = get_full_court_info(proxy_conn, court_id)
----
+---
+id: which-jurisdiction
+question: |
+  Which jurisdiction are you filing in?
+fields:
+  - no label: jurisdiction_id
+    code: |
+      [{k: v} for k, v in jurisdiction_names.items() if k in jurisdiction_choices]
+---
+variable name: jurisdiction_names
+data:
+  illinois: Illinois
+  massachusetts: Massachusetts
+  texas: Texas
+  california: California
+  indiana: Indiana
+  louisiana: Louisiana
+---
+imports:
+  - requests
+---
+code: |
+  if 'jurisdiction_id' in url_args:
+    jurisdiction_id = url_args['jurisdiction_id']
+  try:
+    jurisdiction_choices = set(requests.get(get_config("efile proxy", {}).get("url", "") + "/jurisdictions").json().keys())
+  except (requests.exceptions.MissingSchema, requests.exceptions.ConnectionError, requests.exceptions.JSONDecodeError) as ex:
+    log(f"Couldn't connect with the efile proxy server! {ex}")
+    jurisdiction_id = ""
```

### Comparing `docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/questions/minimal_interview.yml` & `docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/questions/minimal_interview.yml`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/questions/toga_payments.yml` & `docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/questions/toga_payments.yml`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/questions/toga_payments_interview.yml` & `docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/questions/toga_payments_interview.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 include:
   - login_qs.yml
   - toga_payments.yml
 ---
-id: which-jurisdiction
-question: |
-  Which jurisdiction are you filing in?
-fields:
-  - no label: jurisdiction_id
-    choices:
-      - Illinois: 'illinois'
-      - Massachusetts: 'massachusetts'
-      - Texas: 'texas'
----
-code: |
-  if 'jurisdiction_id' in url_args:
-    jurisdiction_id = url_args['jurisdiction_id']
+variable name: jurisdiction_names
+data:
+  illinois: Illinois
+  massachusetts: Massachusetts
+  texas: Texas
+  california: California
+  indiana: Indiana
 ---
 need:
   - tyler_login
 event: payment_main_screen
 id: Payment Main screen
 question: |
   Payment methods for ${ my_username }
```

### Comparing `docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/questions/unauthenticated_actions.yml` & `docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/questions/unauthenticated_actions.yml`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 ---
 modules:
   - .efm_client
   - .conversions
 ---
 include:
   - docassemble.ALToolbox:phone-number-validation.yml
+  - docassemble.AssemblyLine:assembly_line.yml
 ---
 objects:
   person_to_reg: ALIndividual
 ---
 variable name: account_action_list
 data: !!omap
   - register: "Register"
@@ -37,23 +38,28 @@
   account_action_recompute = {
     "register": ["register_introduction", "person_to_reg", "register", "register_status"],
     "reset_user_password": ["reset_user_password", "show_reset_resp"],
     "self_resend_activation": ["self_resend_activation", "show_resend_resp"]
   }
 ---
 code: |
-  proxy_conn = ProxyConnection(credentials_code_block='tyler_login', default_jurisdiction=jurisdiction_id)
+  proxy_conn = ProxyConnection(credentials_code_block='', default_jurisdiction=jurisdiction_id)
 ---
+code: |
+  can_connect_to_proxy = proxy_conn.get_server_name().is_ok()
+---
+if: can_connect_to_proxy
 id: unauth-intro
 question: |
   This website will help you register as an e-filing user in ${ jurisdiction_id.title() }
 subquestion: |
   You will need to provide your email and create a password.
 continue button field: register_introduction
 ---
+if: can_connect_to_proxy
 id: unauth-register-done
 question: |
   % if register_resp.is_ok():
   Successfully registered
   % else:
   Something went wrong when we tried to register your account
   % endif
@@ -107,15 +113,15 @@
       ---
   - Email address: person_to_reg.email
     datatype: email
     required: True
   - Phone number: person_to_reg.phone_number
     datatype: al_international_phone
   - note: |
-      ${ password_rules.data.get("validationmessage") }
+      ${ password_rules.get("validationmessage") }
   - Password: new_password
     datatype: ALVisiblePassword
     validate: proxy_conn.is_valid_password
   - note: |
       ---
   - Firm name: person_to_reg.firm_name
     show if:
@@ -124,15 +130,19 @@
   - code: person_to_reg.name_fields()
   - note: |
       ---
   - code: |
       person_to_reg.address_fields()
 ---
 code: |
-  password_rules = proxy_conn.get_password_rules()
+  password_rules_resp = proxy_conn.get_password_rules()
+  if password_rules_resp.is_ok():
+    password_rules = password_rules_resp.data
+  else:
+    password_rules = {}
 ---
 code: |
   resent_activation_resp = proxy_conn.self_resend_activation_email(unauthed_user_email)
   del unauthed_user_email
   self_resend_activation = True
 ---
 code: |
```

### Comparing `docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/sources/admin_interview.feature` & `docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/sources/admin_interview.feature`

 * *Files 0% similar despite different names*

```diff
@@ -6,40 +6,40 @@
   [x] Contains some additional example Steps. They use fake values and are commented out with a "#" so they won't run.
 
   These tests are made to work with the ALKiln testing framework, an automated testing framework made under the Document Assembly Line Project.
 
   @ai1 @admin_interview @taps @admin @attorneys
   Scenario: admin_interview.yml Admin login
     Given I start the interview at "admin_interview.yml"
-    And the maximum seconds for each Step in this Scenario is 15
+    And the maximum seconds for each Step in this Scenario is 30
     And I set the variable "jurisdiction_id" to "illinois"
     And I tap to continue
     And I set the variable "my_username" to secret "TYLER_EMAIL"
     And I set the variable "my_password" to secret "TYLER_PASSWORD"
     And I tap to continue
     And I tap the "Tests-Attorneys-tab" tab 
     And I tap the "#create_attorney" element
     Then I should see the phrase "Comment: Tyler validates the bar number" 
   
   @ai2 @admin_interview @taps @prose @service_contacts
   Scenario: admin_interview.yml Pro Se login 
     Given I start the interview at "admin_interview.yml"
-    And the maximum seconds for each Step in this Scenario is 20
+    And the maximum seconds for each Step in this Scenario is 40
     And I set the variable "jurisdiction_id" to "illinois"
     And I tap to continue
     And I set the variable "my_username" to secret "PROSE_EMAIL"
     And I set the variable "my_password" to secret "PROSE_PASSWORD"
     And I tap to continue
     And I tap the "Tests-Service_contacts-tab" tab 
     Then I tap the "#attach_service_contact" element
 
   @ai3 @admin_interview @taps @firm @accessibility
   Scenario: admin_interview.yml Get Firm
     Given I start the interview at "admin_interview.yml"
-    And the maximum seconds for each Step in this Scenario is 20
+    And the maximum seconds for each Step in this Scenario is 40
     And I check all pages for accessibility issues
     And I set the variable "jurisdiction_id" to "illinois"
     And I tap to continue
     And I set the variable "my_username" to secret "TYLER_EMAIL"
     And I set the variable "my_password" to secret "TYLER_PASSWORD"
     And I tap to continue
     And I tap the "Tests-Firm-tab" tab
@@ -49,15 +49,15 @@
     And I tap the "Tests-Firm-tab" tab
     And I tap the "#get_firm" element and wait 5 seconds
     Then I should see the phrase "Suffolk LIT Lab"
 
   @ai4 @admin_interview @taps @accessibility
   Scenario: admin_interview.yml is accessible
     Given I start the interview at "admin_interview.yml"
-    And the maximum seconds for each Step in this Scenario is 50
+    And the maximum seconds for each Step in this Scenario is 70
     And I check all pages for accessibility issues
     And I set the variable "jurisdiction_id" to "illinois"
     And I tap to continue
     And I set the variable "my_username" to secret "TYLER_EMAIL"
     And I set the variable "my_password" to secret "TYLER_PASSWORD"
     And I tap to continue
     And I tap the "Tests-Firm-tab" tab
@@ -71,15 +71,15 @@
     And I tap the "#get_court" element
     And I set the variable "trial_court" to "cook:dr5"
     And I tap to continue
 
   @ai5 @admin_interview @taps @admin @courts
   Scenario: admin_interview.yml See court information
     Given I start the interview at "admin_interview.yml"
-    And the maximum seconds for each Step in this Scenario is 20
+    And the maximum seconds for each Step in this Scenario is 40
     And I set the variable "jurisdiction_id" to "illinois"
     And I tap to continue
     And I set the variable "my_username" to secret "TYLER_EMAIL"
     And I set the variable "my_password" to secret "TYLER_PASSWORD"
     And I tap to continue
     And I tap the "Tests-Filings-tab" tab
     And I tap the "#get_courts" element and wait 3 seconds
@@ -91,15 +91,15 @@
     And I set the variable "trial_court" to "cook:dr5" 
     And I tap to continue
     Then I should see the phrase "name: Cook County - Domestic Relations - District 5 - Bridgeview"
 
   @ai6 @admin_interview @attach
   Scenario: multiple-times through attach
     Given I start the interview at "admin_interview.yml"
-    And the maximum seconds for each Step in this Scenario is 40
+    And the maximum seconds for each Step in this Scenario is 60
     And I set the variable "jurisdiction_id" to "illinois"
     And I tap to continue
     And I set the variable "my_username" to secret "TYLER_EMAIL"
     And I set the variable "my_password" to secret "TYLER_PASSWORD"
     And I tap to continue
     And I tap the "Tests-Service_contacts-tab" tab 
     And I tap the "#attach_service_contact" element
@@ -133,15 +133,15 @@
     And I set the variable "case_party_id" to "87bfa962-ce95-43c7-8370-021828672a38"
     And I tap to continue
     And I see the phrase "All ok! (204)"
 
   @ai7 @admin_interview @attach @prose
   Scenario: earlyish stop attach when no service contacts
     Given I start the interview at "admin_interview.yml"
-    And the maximum seconds for each Step in this Scenario is 40
+    And the maximum seconds for each Step in this Scenario is 60
     And I set the variable "jurisdiction_id" to "illinois"
     And I tap to continue
     And I set the variable "my_username" to secret "PROSE_EMAIL"
     And I set the variable "my_password" to secret "PROSE_PASSWORD"
     And I tap to continue
     And I tap the "Tests-Service_contacts-tab" tab 
     And I tap the "#attach_service_contact" element
```

### Comparing `docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/sources/any_filing_interview.feature` & `docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/sources/any_filing_interview.feature`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 @interviews_start
 Feature: Make any type of filing
 
   Runs the `any_filing_interview.yml` to completion a few different ways
 
+  # This one errors because of description’: “Court Peoria County doesn’t allow service on subsequent filings
+
+
   @any_filing_interview @af1
   Scenario: any_filing_interview goes to end
     Given I start the interview at "any_filing_interview.yml"
     And the maximum seconds for each Step in this Scenario is 50
     And I set the variable "jurisdiction_id" to "illinois"
     And I tap to continue
     And I tap to continue
     And I set the variable "my_username" to secret "TYLER_EMAIL"
     And I set the variable "my_password" to secret "TYLER_PASSWORD"
     And I tap to continue
-    And I get to the question id "service contact" with this data:
+    And I get to the question id "ready to efile" with this data:
       | var | value | trigger |
       | trial_court | peoria | |
       | filing_interview_initial_or_existing | existing_case | |
       | x.do_what_choice | docket_lookup | case_search.do_what_choice |
       | x.docket_number_from_user | 87-SC-01549 | case_search.docket_number_from_user |
       | x.self_in_case | is_filing | case_search.self_in_case |
       | x.self_partip_choice | case_search.found_case.participants[0] | case_search.self_in_case |
@@ -33,21 +36,15 @@
       | x.filing_description | example description | |
       | x.exhibits[0].pages | example_upload.pdf | |
       | x.document_type | 7688 | lead_doc.document_description |
       | x.user_chosen_filing_component | 332 | lead_doc.user_chosen_filing_component |
       | x[i].pages.target_number | 1 | lead_doc.exhibits[0].pages.there_is_another |
       | x.existing_parties_payment_dict['87bfa962-ce95-43c7-8370-021828672a38'] | True | lead_doc.existing_parties_payment_dict |
       | contacts_to_attach.there_are_any | False | |
-      | service_contacts.there_are_any | True | |
-    And I set the var "service_contacts[i].contact_id" to "4fc26680-6b9a-42bd-8934-c67aaee7c97f"
-    And I set the var "service_contacts[i].service_type" to "-580"
-    And I set the var "service_contacts[i].attach_service_contact_to_party" to "True"
-    And I set the var "service_contacts[i].party_association" to "87bfa962-ce95-43c7-8370-021828672a38"
-    And I tap to continue
-    And I get to the question id "ready to efile" with this data:
+      | service_contacts.there_are_any | False | |
       | var | value | trigger |
       | service_contacts.target_number | 1 | service_contacts.there_is_another |
       | x.filing_action | efile_and_serve | lead_doc.filing_action |
       | x.optional_services.there_are_any | False | lead_doc.optional_services.there_are_any |
       | al_court_bundle.target_number | 1 | |
       | tyler_payment_id | 3edbc236-14e1-4850-b101-50c1da073e30 | |
       | review_fees_screen['agrees_to_pay_fees'] | True | |
@@ -59,15 +56,15 @@
     And the maximum seconds for each Step in this Scenario is 100
     And I set the variable "jurisdiction_id" to "illinois"
     And I tap to continue
     And I tap to continue
     And I set the variable "my_username" to secret "PROSE_EMAIL"
     And I set the variable "my_password" to secret "PROSE_PASSWORD"
     And I tap to continue
-    And I get to the question id "service contact" with this data:
+    And I get to the question id "ready to efile" with this data:
       | var | value | trigger |
       | trial_court | peoria | |
       | filing_interview_initial_or_existing | existing_case | |
       | x.do_what_choice | docket_lookup | case_search.do_what_choice |
       | x.docket_number_from_user | 87-SC-01549 | case_search.docket_number_from_user |
       | x.self_in_case | is_self | case_search.self_in_case |
       | x.self_partip_choice | case_search.found_case.participants[0] | case_search.self_in_case |
@@ -83,22 +80,15 @@
       | x.filing_type | 145495 | |
       | x.filing_description | example description | |
       | x.exhibits[0].pages | example_upload.pdf | |
       | x.document_type | 7688 | lead_doc.document_type |
       | x.user_chosen_filing_component | 332 | lead_doc.user_chosen_filing_component |
       | x[i].pages.target_number | 1 | lead_doc.exhibits[0].pages.there_is_another |
       | x.existing_parties_payment_dict['87bfa962-ce95-43c7-8370-021828672a38'] | True | lead_doc.existing_parties_payment_dict |
-      | service_contacts.there_are_any | True | |
-    And I set the var "service_contacts[i].contact_id" to "4fc26680-6b9a-42bd-8934-c67aaee7c97f"
-    And I set the var "service_contacts[i].service_type" to "-580"
-    And I set the var "service_contacts[i].attach_service_contact_to_party" to "True"
-    And I set the var "service_contacts[i].party_association" to "87bfa962-ce95-43c7-8370-021828672a38"
-    And I tap to continue
-    And I get to the question id "ready to efile" with this data:
-      | var | value | trigger |
+      | service_contacts.there_are_any | False | |
       | service_contacts.target_number | 1 | service_contacts.there_is_another |
       | x.filing_action | efile_and_serve | lead_doc.filing_action |
       | x.optional_services.there_are_any | False | lead_doc.optional_services.there_are_any |
       | al_court_bundle.target_number | 1 | |
       | tyler_payment_id | e9cd74e2-ee91-4706-a25c-cac6865013c8 | |
       | review_fees_screen['agrees_to_pay_fees'] | True | |
     Then I see the phrase "Below is your Lead Filing Doc"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/sources/example_upload.pdf` & `docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/sources/example_upload.pdf`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/data/static/Ajax-loader.gif` & `docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/data/static/Ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/efm_client.py` & `docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/efm_client.py`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/interview_logic.py` & `docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/interview_logic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,32 @@
 """
 A group of methods that were code blocks in various parts of the EFSP
 package, but for better python tooling support, were moved here.
 """
 
-from typing import Any, Callable, Dict, List, Tuple, Optional, Iterable, Union
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    Tuple,
+    Optional,
+    Iterable,
+    Union,
+    TypedDict,
+)
 from datetime import datetime
 
 from docassemble.base.util import CustomDataType, DAObject, DAList, log, word
-from .conversions import parse_case_info, fetch_case_info, chain_xml
+from .conversions import (
+    parse_case_info,
+    fetch_case_info,
+    chain_xml,
+    log_error_and_notify,
+)
 from docassemble.AssemblyLine.al_general import ALPeopleList, ALIndividual
 
 
 class EFCaseSearch(DAObject):
     """A data-class that has holds all of the information and state for a single case search"""
 
     court_id: str
@@ -108,18 +123,40 @@
                 if field.get("field", "").endswith(".state"):
                     field["default"] = firm_info.data["address"].get("state")
                 if field.get("field", "").endswith(".zip"):
                     field["default"] = firm_info.data["address"].get("zipCode")
     return address_fields
 
 
+FieldEntry = TypedDict(
+    "FieldEntry",
+    {
+        "label": str,
+        "field": str,
+        "datatype": str,
+        "rows": int,
+        "help": str,
+        "show if": Union[str, Dict[str, str]],
+        "hide if": str,
+        "input type": str,
+        "default": str,
+        "code": str,
+        "address autocomplete": bool,
+        "choices": Union[List[str], Dict[str, str]],
+        "required": bool,
+    },
+    total=False,
+)
+Fields = List[FieldEntry]
+
+
 def contact_fields_with_defaults(
     proxy_conn, person: ALIndividual, is_admin: bool, can_check_efile: bool
 ):
-    contact_fields = [
+    contact_fields: List[FieldEntry] = [
         {
             "label": word("Mobile number"),
             "field": person.attr_name("mobile_number"),
             "required": False,
         },
         {
             "label": word("Other phone number"),
@@ -200,15 +237,17 @@
                 proxy_conn, new_case, entry, court_id, fetch=should_fetch, roles=roles
             )
             # Allows users to control what cases are shown as options
             if not filter_fn(new_case):
                 found_cases.pop()
             log(f"done with {idx} in search_case_by_name, {new_case.as_serializable()}")
     else:
-        log(f"get_cases_response: {get_cases_response}")
+        log_error_and_notify(
+            "get_cases_response failed when searching for case", get_cases_response
+        )
         found_cases.resp_ok = False
     found_cases.gathered = True
     return cms_connection_issue, found_cases
 
 
 def shift_case_select_window(
     proxy_conn,
@@ -271,15 +310,17 @@
 
 def get_full_court_info(proxy_conn, court_id: str) -> Dict:
     """Gets all of the information about the court from the id"""
     full_court_resp = proxy_conn.get_court(court_id)
     if full_court_resp.is_ok():
         return full_court_resp.data
     else:
-        log(f"Couldn't get full court info for {court_id}: {full_court_resp}")
+        log_error_and_notify(
+            f"Couldn't get full court info for {court_id}", full_court_resp
+        )
         return {}
 
 
 def _scale_byte_units(value: Union[str, int], unit: str) -> int:
     """Idk if these are right, but there's no examples out there.
     Niem suggests they might not matter:
     https://docs.oasis-open.org/legalxml-courtfiling/ecf/v5.0/csprd03/model/class137602.html
@@ -419,12 +460,12 @@
     """Gets the list of efilable courts, if it can"""
     resp = proxy_conn.authenticate_user()  # use default config keys
     if resp.response_code == 200:
         court_list = proxy_conn.get_court_list()
         if court_list.is_ok():
             return sorted(court_list.data or [])
         else:
-            log(f"Couldn't get courts from proxy server? {court_list}")
+            log_error_and_notify("Couldn't get courts from proxy server?", court_list)
             return []
     else:
-        log(f"Couldn't login to the proxy server!: {resp}")
+        log_error_and_notify("Couldn't login to the proxy server", resp)
         return []
```

### Comparing `docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/py_efsp_client.py` & `docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/py_efsp_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 The base python client used to communicate with the E-file proxy server.
 
 Doesn't include anything from docassemble, and can be used without having it installed.
 """
 
 import re
 import logging
-import isodate
 import requests
 from requests import Response
 from datetime import datetime
 from typing import Optional, Union, List, Dict
 import http.client as http_client
 from copy import deepcopy
 
@@ -230,18 +229,20 @@
         send = lambda: self.proxy_client.post(
             self.full_url("adminusers/users"), json=reg_obj
         )
         return self._call_proxy(send)
 
     def get_password_rules(self) -> ApiResponse:
         """
-        Password rules are stored in the global court, id 1.
+        Password rules are stored in the global court, id 0.
+
+        TODO: They're in other courts too, including 1. Could they ever be different?
         """
         send = lambda: self.proxy_client.get(
-            self.full_url("codes/courts/1/datafields/GlobalPassword")
+            self.full_url("codes/courts/0/datafields/GlobalPassword")
         )
         return self._call_proxy(send)
 
     def is_valid_password(self, password: str) -> Optional[bool]:
         results = self.get_password_rules()
         if results.data:
             password_regex = results.data.get("regularexpression", ".*")
```

### Comparing `docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/test/integration_test.py` & `docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/test/integration_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/env python3
 
-from ..py_efsp_client import EfspConnection, ApiResponse
+import os
+import json
 import sys
 import subprocess
-import json
-import os
+from docassemble.EFSPIntegration.py_efsp_client import EfspConnection, ApiResponse
 from pathlib import Path
 from datetime import datetime, timedelta
 
 
 def get_proxy_server_ip():
     # Figure out the ip addr of the service, assuming it's running through
     # Docker compose
@@ -48,63 +48,100 @@
         "country": "US",
     }
     per["phoneNumber"] = "1234567890"
     return per
 
 
 class TestClass:
-    def __init__(self, proxy_conn, verbose: bool = True):
+    def __init__(
+        self, proxy_conn, verbose: bool = True, user_email=None, user_password=None
+    ):
         self.proxy_conn = proxy_conn
         self.verbose = verbose
+        self.user_email = user_email
+        self.user_password = user_password
 
     def basic_assert(self, resp: ApiResponse):
-        if self.verbose:
+        if self.verbose or not resp.is_ok():
             print(resp)
         assert resp.is_ok()
         return resp
 
     def test_authenticate(self):
         print("\n\n### Authenticate ###\n\n")
         empty_resp = self.proxy_conn.authenticate_user()
         self.basic_assert(empty_resp)
         assert len(empty_resp.data["tokens"]) == 0
         resp = self.proxy_conn.authenticate_user(
-            tyler_email=os.getenv("bryce_user_email"),
-            tyler_password=os.getenv("bryce_user_password"),
+            tyler_email=self.user_email, tyler_password=self.user_password
         )
         self.basic_assert(resp)
 
     def test_hateos(self):
         print("\n\n### Hateos ###\n\n")
         base_url = self.proxy_conn.base_url
         base_send = lambda: self.proxy_conn.proxy_client.get(base_url)
         next_level_urls = self.basic_assert(self.proxy_conn._call_proxy(base_send)).data
-        for url in next_level_urls.values():
+        all_urls = [url for url in next_level_urls.values()]
+        visited_urls = set()
+        while len(all_urls) > 0:
+            url = all_urls.pop(0)
+            if url in visited_urls:
+                continue
+            else:
+                visited_urls.add(url)
             if "authenticate" in url:
                 continue
+            if "logs" in url:
+                continue
+            if "{" in url or "}" in url:
+                continue
+            # TODO(brycew): scheduling is broken, /service-contacts/public isn't RESTful
+            if (
+                "scheduling" in url
+                or "service-contacts/public" in url
+                or (
+                    (
+                        "adminusers" in url
+                        or "firmattorneyservice" in url
+                        or "payments" in url
+                    )
+                    and "illinois" not in url
+                )
+            ):
+                continue
+            print(f"visiting {url}")
             send = lambda: self.proxy_conn.proxy_client.get(url)
-            self.basic_assert(self.proxy_conn._call_proxy(send))
+            resp = self.basic_assert(self.proxy_conn._call_proxy(send)).data
+            if isinstance(resp, dict):
+                for url in resp.values():
+                    if isinstance(url, str) and url.startswith("http"):
+                        all_urls.append(url)
+                    elif (
+                        isinstance(url, dict)
+                        and ("method" in url and url["method"] == "GET")
+                        and "url" in url
+                    ):
+                        all_urls.append(url["url"])
 
     def test_self_user(self):
         print("\n\n### Self user ###\n\n")
         myself = self.basic_assert(self.proxy_conn.get_user())
         assert myself.data["middleName"] == "Steven"
         nm = self.basic_assert(
             self.proxy_conn.update_user(myself.data["userID"], middle_name="Stephen")
         )
         bad_spelling = self.basic_assert(self.proxy_conn.get_user())
         assert bad_spelling.data["middleName"] == "Stephen"
-        self.basic_assert(
-            self.proxy_conn.update_user(myself.data["userID"], middle_name="Steven")
-        )
+        self.basic_assert(self.proxy_conn.self_update_user(middle_name="Steven"))
 
         # Password stuff
-        current_password = os.getenv("bryce_user_password")
+        current_password = self.user_password
         new_password = "12345678AbcDe!"
-        email = os.getenv("bryce_user_email")
+        email = self.user_email
         changed_password = self.basic_assert(
             self.proxy_conn.self_change_password(current_password, new_password)
         )
         self.basic_assert(
             self.proxy_conn.authenticate_user(
                 tyler_email=email, tyler_password=new_password
             )
@@ -387,45 +424,44 @@
         assert full_new_attorney.data["middleName"] == "Lobert"
 
         deleted_maybe = self.proxy_conn.remove_attorney(new_attorney_id)
         assert deleted_maybe.response_code == 200
 
     def test_filings(self):
         print("\n\n### Filings ###\n\n")
+        court = "adams"
         filing_list = self.basic_assert(
             self.proxy_conn.get_filing_list(
-                "illinois",
-                "adams",
+                court,
                 start_date=datetime.today() - timedelta(days=3),
                 before_date=datetime.today(),
             )
         )
-        policy = self.basic_assert(self.proxy_conn.get_policy("illinois", "adams"))
+        policy = self.basic_assert(self.proxy_conn.get_policy(court))
 
         cdir = Path(__file__).resolve().parent
-        # TODO(brycew): needs a more up to date JSON from any filing interiview
-        all_vars_str = (
-            cdir.joinpath("initial_cook_filing_vars_shorter.json").open("r").read()
-        )
+        with open(cdir.joinpath("opening_affidavit_adams.json"), "r") as f:
+            all_vars_str = f.read()
         base_url = self.proxy_conn.base_url
-        court = "cook:cvd1"
         fees_send = lambda: self.proxy_conn.proxy_client.post(
             base_url
-            + f"filingreview/jurisdictions/illinois/courts/{court}/filing/fees",
+            + f"jurisdictions/illinois/filingreview/courts/{court}/filing/fees",
             data=all_vars_str,
         )
         fees_resp = self.basic_assert(self.proxy_conn._call_proxy(fees_send))
         check_send = lambda: self.proxy_conn.proxy_client.get(
             base_url
-            + f"filingreview/jurisdictions/illinois/courts/{court}/filing/check",
+            + f"jurisdictions/illinois/filingreview/courts/{court}/filing/check",
             data=all_vars_str,
         )
         checked_resp = self.basic_assert(self.proxy_conn._call_proxy(check_send))
+        return
+        # IDK if I want to make a new filing each time, even if we cancel it
         file_send = lambda: self.proxy_conn.proxy_client.post(
-            base_url + f"filingreview/jurisdictions/illinois/courts/{court}/filings",
+            base_url + f"jurisdictions/illinois/filingreview/courts/{court}/filings",
             data=all_vars_str,
         )
         filing_resp = self.basic_assert(self.proxy_conn._call_proxy(file_send))
 
         for filing_id in filing_resp.data:
             status_resp = self.basic_assert(
                 self.proxy_conn.get_filing_status(court, filing_id)
@@ -436,55 +472,76 @@
             cancel_resp = self.basic_assert(
                 self.proxy_conn.cancel_filing_status(court, filing_id)
             )
 
     def test_codes(self):
         print("\n\n### Codes ###\n\n")
         self.basic_assert(self.proxy_conn.get_court_list())
-        self.basic_assert(self.proxy_conn.get_case_categories("adams"))
+        self.basic_assert(self.proxy_conn.get_court("adams"))
+        self.basic_assert(self.proxy_conn.get_datafield("adams", "GlobalPassword"))
+        self.basic_assert(self.proxy_conn.get_disclaimers("adams"))
+        categories = self.basic_assert(
+            self.proxy_conn.get_case_categories("adams")
+        ).data
+        for idx, cat in enumerate(categories):
+            if idx > 5:
+                continue
+            self.basic_assert(self.proxy_conn.get_case_types("adams", cat["code"]))
 
     def test_logs(self):
         print("\n\n### Test Logs ###\n\n")
         server_id = self.basic_assert(self.proxy_conn.get_server_id()).data
         all_logs = self.basic_assert(self.proxy_conn.get_logs())
         for l in all_logs.data:
             assert l.split("|")[1].strip() == server_id
 
 
-def main(args):
-    base_url = get_proxy_server_ip()
-    api_key = os.getenv("PROXY_API_KEY")
+def main(*, base_url, api_key, user_email=None, user_password=None):
+    if not base_url:
+        base_url = get_proxy_server_ip()
     if not api_key:
         print("You need to have the PROXY_API_KEY env var set; not running tests")
-        return
+        return 1
+    if not user_email:
+        user_email = os.getenv("bryce_user_email")
+    if not user_password:
+        user_password = os.getenv("bryce_user_password")
     bad_proxy = EfspConnection(
         url=base_url, api_key="IntenionallyWrongKey", default_jurisdiction="illinois"
     )
     intentional_bad_resp = bad_proxy.authenticate_user()
     if intentional_bad_resp.response_code != 403:
         print(intentional_bad_resp)
     assert intentional_bad_resp.response_code == 403
+    bad_proxy.proxy_client.close()
     proxy_conn = EfspConnection(
         url=base_url, api_key=api_key, default_jurisdiction="illinois"
     )
-    proxy_conn.set_verbose_logging(True)
-    tc = TestClass(proxy_conn, verbose=True)
+    proxy_conn.set_verbose_logging(False)
+    tc = TestClass(
+        proxy_conn, verbose=False, user_email=user_email, user_password=user_password
+    )
     tc.test_authenticate()
     tc.test_hateos()
     tc.test_self_user()
     tc.test_firm()
     tc.test_service_contacts()
     tc.test_get_courts()
     tc.test_payment_accounts()
     tc.test_attorneys()
     tc.test_court_record()
     tc.test_users()
     tc.test_codes()
     tc.test_logs()
     # TODO(brycew): needs a more up to date JSON from any filing interiview
-    # tc.test_filings()
+    tc.test_filings()
+    print("Done!")
     # TODO(brycew): Tyler issue, have to wait on them
     # tc.test_global_payment_accounts()
+    proxy_conn.proxy_client.close()
 
 
 if __name__ == "__main__":
-    main(sys.argv)
+    main(
+        base_url=sys.argv[1] if len(sys.argv) > 1 else None,
+        api_key=os.getenv("PROXY_API_KEY"),
+    )
```

### Comparing `docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/test/peoria_to_cr.json` & `docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/test/peoria_to_cr.json`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/test/temp2.json` & `docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/test/temp2.json`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/test/test_conversions.py` & `docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/test/test_conversions.py`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.2/docassemble/EFSPIntegration/test/vars.json` & `docassemble.EFSPIntegration-1.3.0/docassemble/EFSPIntegration/test/vars.json`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.2/docassemble.EFSPIntegration.egg-info/PKG-INFO` & `docassemble.EFSPIntegration-1.3.0/docassemble.EFSPIntegration.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docassemble.EFSPIntegration
-Version: 1.2.2
+Version: 1.3.0
 Home-page: https://github.com/SuffolkLITLab/docassemble-EFSPIntegration
 Author: Bryce Willey
 Author-email: bwilley@suffolk.edu
 License: The MIT License (MIT)
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `docassemble.EFSPIntegration-1.2.2/docassemble.EFSPIntegration.egg-info/SOURCES.txt` & `docassemble.EFSPIntegration-1.3.0/docassemble.EFSPIntegration.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,11 +35,12 @@
 docassemble/EFSPIntegration/data/sources/example_upload.pdf
 docassemble/EFSPIntegration/data/sources/unauthenticated_interview.feature
 docassemble/EFSPIntegration/data/static/Ajax-loader.gif
 docassemble/EFSPIntegration/data/static/README.md
 docassemble/EFSPIntegration/data/templates/README.md
 docassemble/EFSPIntegration/test/__init__.py
 docassemble/EFSPIntegration/test/integration_test.py
+docassemble/EFSPIntegration/test/opening_affidavit_adams.json
 docassemble/EFSPIntegration/test/peoria_to_cr.json
 docassemble/EFSPIntegration/test/temp2.json
 docassemble/EFSPIntegration/test/test_conversions.py
 docassemble/EFSPIntegration/test/vars.json
```

### Comparing `docassemble.EFSPIntegration-1.2.2/setup.py` & `docassemble.EFSPIntegration-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                         break
                 if bad_name:
                     continue
                 out.setdefault(package, []).append(prefix+name)
     return out
 
 setup(name='docassemble.EFSPIntegration',
-      version='1.2.2',
+      version='1.3.0',
       description=(''),
       long_description='# docassemble-EFSPIntegration\r\n\r\nA docassemble extension that talks to [a proxy e-filing server](https://github.com/SuffolkLITLab/EfileProxyServer/) easily within a docassemble interview.\r\n\r\nMain interviews of import:\r\n\r\n* any_filing_interview.yml: allows you to make any type of filing, initial or subsequent\r\n* admin_interview.yml: lets you handle admin / user functionality, outside of the context of cases and filings\r\n\r\nIn progress!\r\n\r\n## Authors\r\n\r\nQuinten Steenhuis (qsteenhuis@suffolk.edu)\r\nBryce Willey (bwilley@suffolk.edu)\r\n',
       long_description_content_type='text/markdown',
       author='Bryce Willey',
       author_email='bwilley@suffolk.edu',
       license='The MIT License (MIT)',
       url='https://github.com/SuffolkLITLab/docassemble-EFSPIntegration',
```

