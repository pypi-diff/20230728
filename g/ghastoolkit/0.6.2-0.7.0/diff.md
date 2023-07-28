# Comparing `tmp/ghastoolkit-0.6.2.tar.gz` & `tmp/ghastoolkit-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghastoolkit-0.6.2.tar", last modified: Wed Jul 26 18:27:31 2023, max compression
+gzip compressed data, was "ghastoolkit-0.7.0.tar", last modified: Fri Jul 28 14:57:47 2023, max compression
```

## Comparing `ghastoolkit-0.6.2.tar` & `ghastoolkit-0.7.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:27:31.575681 ghastoolkit-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-26 18:27:31.575681 ghastoolkit-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 18:27:31.575681 ghastoolkit-0.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:27:31.567680 ghastoolkit-0.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:27:31.567680 ghastoolkit-0.6.2/src/ghastoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:27:31.567680 ghastoolkit-0.6.2/src/ghastoolkit/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/codeql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/codeql/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/codeql/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/codeql/databases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:27:31.571680 ghastoolkit-0.6.2/src/ghastoolkit/codeql/dataextensions/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/codeql/dataextensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/codeql/dataextensions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/codeql/dataextensions/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/codeql/dataextensions/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:27:31.571680 ghastoolkit-0.6.2/src/ghastoolkit/codeql/packs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/codeql/packs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/codeql/packs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/codeql/packs/pack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/codeql/packs/packs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/codeql/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:27:31.571680 ghastoolkit-0.6.2/src/ghastoolkit/octokit/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/octokit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/octokit/advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/octokit/clearlydefined.py
--rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/octokit/codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/octokit/dependabot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/octokit/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/octokit/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:27:31.571680 ghastoolkit-0.6.2/src/ghastoolkit/octokit/graphql/
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/octokit/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12025 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/octokit/octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/octokit/secretscanning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:27:31.571680 ghastoolkit-0.6.2/src/ghastoolkit/secretscanning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/secretscanning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/secretscanning/secretalerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:27:31.571680 ghastoolkit-0.6.2/src/ghastoolkit/supplychain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/supplychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/supplychain/advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/supplychain/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/supplychain/dependencyalert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/supplychain/licensing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:27:31.567680 ghastoolkit-0.6.2/src/ghastoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-26 18:27:31.000000 ghastoolkit-0.6.2/src/ghastoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-26 18:27:31.000000 ghastoolkit-0.6.2/src/ghastoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:27:31.000000 ghastoolkit-0.6.2/src/ghastoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-26 18:27:31.000000 ghastoolkit-0.6.2/src/ghastoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 18:27:31.000000 ghastoolkit-0.6.2/src/ghastoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:27:31.575681 ghastoolkit-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/tests/test_advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/tests/test_clearlydefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/tests/test_codeql_dataext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/tests/test_codeql_packs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/tests/test_codeqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/tests/test_codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/tests/test_depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/tests/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/tests/test_octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/tests/test_secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:47.194078 ghastoolkit-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-28 14:57:47.194078 ghastoolkit-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 14:57:47.194078 ghastoolkit-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:47.186078 ghastoolkit-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:47.186078 ghastoolkit-0.7.0/src/ghastoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:47.190078 ghastoolkit-0.7.0/src/ghastoolkit/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/codeql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/codeql/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/codeql/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/codeql/databases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:47.190078 ghastoolkit-0.7.0/src/ghastoolkit/codeql/dataextensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/codeql/dataextensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/codeql/dataextensions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/codeql/dataextensions/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/codeql/dataextensions/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:47.190078 ghastoolkit-0.7.0/src/ghastoolkit/codeql/packs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/codeql/packs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/codeql/packs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/codeql/packs/pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/codeql/packs/packs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/codeql/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:47.190078 ghastoolkit-0.7.0/src/ghastoolkit/octokit/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/octokit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/octokit/advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/octokit/clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/octokit/codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/octokit/dependabot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/octokit/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/octokit/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:47.190078 ghastoolkit-0.7.0/src/ghastoolkit/octokit/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/octokit/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12025 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/octokit/octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/octokit/secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:47.190078 ghastoolkit-0.7.0/src/ghastoolkit/secretscanning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/secretscanning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/secretscanning/secretalerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:47.190078 ghastoolkit-0.7.0/src/ghastoolkit/supplychain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/supplychain/advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/supplychain/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/supplychain/dependencyalert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/supplychain/licensing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:47.190078 ghastoolkit-0.7.0/src/ghastoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-28 14:57:47.000000 ghastoolkit-0.7.0/src/ghastoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-28 14:57:47.000000 ghastoolkit-0.7.0/src/ghastoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 14:57:47.000000 ghastoolkit-0.7.0/src/ghastoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-28 14:57:47.000000 ghastoolkit-0.7.0/src/ghastoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 14:57:47.000000 ghastoolkit-0.7.0/src/ghastoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:47.194078 ghastoolkit-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/tests/test_advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/tests/test_clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/tests/test_codeql_dataext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/tests/test_codeql_packs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/tests/test_codeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/tests/test_codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/tests/test_depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/tests/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/tests/test_octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/tests/test_secretscanning.py
```

### Comparing `ghastoolkit-0.6.2/LICENSE` & `ghastoolkit-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.2/PKG-INFO` & `ghastoolkit-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.6.2
+Version: 0.7.0
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.6.2/README.md` & `ghastoolkit-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.2/pyproject.toml` & `ghastoolkit-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ghastoolkit"
-version = "0.6.2"
+version = "0.7.0"
 authors = [{ name = "GeekMasher" }]
 description = "GitHub Advanced Security Python Toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
```

### Comparing `ghastoolkit-0.6.2/src/ghastoolkit/__init__.py` & `ghastoolkit-0.7.0/src/ghastoolkit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """GitHub Advanced Security Toolkit."""
 __name__ = "ghastoolkit"
 __title__ = "GHAS Toolkit"
 
-__version__ = "0.6.2"
+__version__ = "0.7.0"
 
 __description__ = "GitHub Advanced Security Python Toolkit"
 __summary__ = """\
 GitHub Advanced Security Python Toolkit
 """
 
 __url__ = "https://github.com/GeekMasher/ghastoolkit"
```

### Comparing `ghastoolkit-0.6.2/src/ghastoolkit/__main__.py` & `ghastoolkit-0.7.0/src/ghastoolkit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.2/src/ghastoolkit/codeql/databases.py` & `ghastoolkit-0.7.0/src/ghastoolkit/codeql/databases.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from datetime import datetime
+from logging import log
 import os
 import shutil
 import zipfile
 import tempfile
 from typing import *
 from dataclasses import dataclass
 
@@ -80,14 +81,19 @@
         return False
 
     def exists(self) -> bool:
         """Checks if the CodeQL Database exists"""
         return False if not self.path else os.path.exists(self.path)
 
     @property
+    def root(self) -> str:
+        """Get the standard root location."""
+        return __CODEQL_DATABASE_PATHS__[0]
+
+    @property
     def default_pack(self) -> str:
         """Gets the default query pack for language"""
         return f"codeql/{self.language}-queries"
 
     def getSuite(self, name: str) -> str:
         """Gets suite based on default pack"""
         return f"{self.default_pack}:codeql-suites/{self.language}-{name}.qls"
@@ -134,15 +140,15 @@
         else:
             result = f"{self.name}"
 
         return result
 
     @staticmethod
     def loadFromYml(path: str) -> "CodeQLDatabase":
-        """Load from YAML / YML file
+        """Load from YAML / YML file.
 
         **Example:**
         >>> db = CodeQLDatabase.loadFromYml("codeql-db")
 
         """
         if not os.path.exists(path):
             raise Exception("CodeQL Database YML does not exist")
@@ -154,15 +160,15 @@
         db.loadDatabaseYml(path)
         if db.language == "":
             logger.error(f"CodeQLDatabase Language not set from YML")
             raise Exception(f"Unable to load DB correctly")
         return db
 
     def loadDatabaseYml(self, path: str):
-        """Load content from YML file"""
+        """Load content from YML file."""
         if not os.path.exists(path):
             raise Exception("CodeQL Database YML does not exist")
         if not path.endswith(".yml"):
             raise Exception("File is not a YML file")
 
         with open(path, "r") as handle:
             data = safe_load(handle)
@@ -175,17 +181,19 @@
         creation_time = data.get("creationMetadata", {}).get("creationTime")
         if isinstance(creation_time, datetime):
             self.created = creation_time
         else:
             creation_time, _ = creation_time.split(".", 1)
             self.created = datetime.fromisoformat(creation_time)
 
-    def downloadDatabase(self, output: Optional[str], use_cache: bool = True) -> str:
-        """Download CodeQL Database"""
-        output = output or self.path or self.path_download
+    def downloadDatabase(
+        self, output: Optional[str] = None, use_cache: bool = True
+    ) -> str:
+        """Download CodeQL Database."""
+        output = output or self.path or self.root
         if not output:
             raise Exception(f"CodeQL Database path not set")
 
         if not self.language or not self.repository:
             raise Exception(
                 f"Database download requires a repository and language to be set"
             )
@@ -196,122 +204,127 @@
         if not url:
             raise Exception(f"Remote Database does not exist for `{self.language}`")
 
         if not os.path.exists(output):
             logger.debug(f"Creating path: {output}")
             os.makedirs(output)
 
-        output_zip = os.path.join(output, self.database_folder + ".tar.gz")
-        output_db = os.path.join(output, self.database_folder)
+        output_zip = os.path.join(
+            tempfile.gettempdir(), self.database_folder + ".tar.gz"
+        )
+        output_db = os.path.join(tempfile.gettempdir(), self.database_folder)
 
         # Deleting cached files
         if not use_cache:
             logger.info(f"Deleting cached files...")
             if os.path.exists(output_db):
                 shutil.rmtree(output_db)
 
             if os.path.exists(output_zip):
                 os.remove(output_zip)
 
         if not os.path.exists(output_zip):
-            logger.info("Downloading CodeQL Database from GitHub")
+            logger.debug("Downloading CodeQL Database from GitHub")
 
             headers = {
                 "Accept": "application/zip",
                 "Authorization": f"token {GitHub.token}",
             }
 
             with request("get", url, headers=headers) as resp:
                 with open(output_zip, "wb") as f:
                     for chunk in resp.iter_content(chunk_size=1024):
                         if chunk:
                             f.write(chunk)
 
         else:
-            logger.info("Database archive is present on system, skipping download...")
+            logger.debug("Database archive is present on system, skipping download...")
 
-        logger.info(f"Extracting archive data :: {output_zip}")
+        logger.debug(f"Extracting archive data :: {output_zip}")
 
         # SECURITY: Do we trust this DB?
         with zipfile.ZipFile(output_zip) as zf:
             zf.extractall(output_db)
 
-        logger.info(f" >>> {output_db}")
+        logger.debug(f" >>> {output_db}")
         codeql_lang_path = os.path.join(output_db, self.language)
 
         if os.path.exists(codeql_lang_path):
-            return codeql_lang_path
+            logger.debug(f"Moving Database...")
 
-        for codeql_dir in os.listdir(output_db):
-            codeql_dir = os.path.join(output_db, codeql_dir)
-            if os.path.isdir(codeql_dir):
-                return codeql_dir
+            if os.path.exists(output):
+                logger.debug(f"Removing old DB :: {output}")
+                shutil.rmtree(output)
+
+            shutil.move(codeql_lang_path, output)
+            self.path = output
+            return output
 
         raise Exception(f"Database downloaded but not DB files...")
 
 
 class CodeQLDatabases(list[CodeQLDatabase]):
+    """List of CodeQL Databases."""
+
     def loadDefault(self):
-        """Load Databases from standard locations"""
+        """Load Databases from standard locations."""
         for location in __CODEQL_DATABASE_PATHS__:
             if not os.path.exists(location):
                 continue
             self.findDatabases(location)
 
     @staticmethod
     def loadLocalDatabase() -> "CodeQLDatabases":
-        """Load all Local Databases"""
+        """Load all Local Databases."""
         db = CodeQLDatabases()
         db.loadDefault()
         return db
 
     def getRemoteDatabases(self, repository: Repository):
-        """Find all remote databases and return a list of them"""
+        """Find all remote databases and return a list of them."""
         cs = CodeScanning(repository)
         databases = cs.getCodeQLDatabases()
         for db in databases:
             lang = db.get("language")
             if not lang:
                 raise Exception(f"CodeQL remote language is not set")
             self.append(
-                CodeQLDatabase(
-                    f"{repository.repo}-{lang}", language=lang, repository=repository
-                )
+                CodeQLDatabase(repository.repo, language=lang, repository=repository)
             )
 
     @staticmethod
     def loadRemoteDatabases(repository: Repository) -> "CodeQLDatabases":
-        """Use API to find all the databases and return a list of them"""
+        """Use API to find all the databases and return a list of them."""
         dbs = CodeQLDatabases()
         dbs.getRemoteDatabases(repository)
         return dbs
 
     def findDatabases(self, path: str):
-        """Find databases based on a path (recursive)"""
+        """Find databases based on a path (recursive)."""
         if not os.path.exists(path):
             raise Exception(f"Path does not exist: {path}")
 
         for root, _, files in os.walk(path):
             for file in files:
                 if file == "codeql-database.yml":
                     path = os.path.join(root, file)
                     self.append(CodeQLDatabase.loadFromYml(path))
 
     def get(self, name: str) -> Optional[CodeQLDatabase]:
-        """Get a database by name"""
+        """Get a database by name."""
         for db in self:
             if db.name == name:
                 return db
         return
 
     def getLanguages(self, language: str) -> "CodeQLDatabases":
-        """Get a list of databases by language"""
+        """Get a list of databases by language."""
         dbs = CodeQLDatabases()
         for db in dbs:
             if db.language == language:
                 dbs.append(db)
         return dbs
 
     def downloadDatabases(self):
-        """Download all databases from GitHub"""
+        """Download all databases from GitHub."""
         for db in self:
             db.downloadDatabase(None)
```

### Comparing `ghastoolkit-0.6.2/src/ghastoolkit/codeql/dataextensions/__main__.py` & `ghastoolkit-0.7.0/src/ghastoolkit/codeql/dataextensions/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.2/src/ghastoolkit/codeql/dataextensions/ext.py` & `ghastoolkit-0.7.0/src/ghastoolkit/codeql/dataextensions/ext.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.2/src/ghastoolkit/codeql/dataextensions/models.py` & `ghastoolkit-0.7.0/src/ghastoolkit/codeql/dataextensions/models.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.2/src/ghastoolkit/codeql/packs/__main__.py` & `ghastoolkit-0.7.0/src/ghastoolkit/codeql/packs/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.2/src/ghastoolkit/codeql/packs/pack.py` & `ghastoolkit-0.7.0/src/ghastoolkit/codeql/packs/pack.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """CodeQL Packs."""
 
 import os
 import json
 import glob
 import logging
 from typing import Any, List, Optional
-from collections import OrderedDict
 from semantic_version import Version
 import yaml
 
 from ghastoolkit.codeql.cli import CodeQL
 
 
 logger = logging.getLogger("ghastoolkit.codeql.packs")
@@ -28,28 +27,30 @@
         name: Optional[str] = None,
         version: Optional[str] = None,
         cli: Optional[CodeQL] = None,
     ) -> None:
         """Initialise CodeQL Pack."""
         self.cli = cli or CodeQL()
 
-        self.path = path
+        self.path = path  # dir
         self.library: bool = library or False
         self.name: str = name or ""
         self.version: str = version or "0.0.0"
         self.dependencies: List["CodeQLPack"] = []
         self.default_suite: Optional[str] = None
 
         if path:
             # if its a file
             if os.path.isfile(path) and path.endswith("qlpack.yml"):
                 path = os.path.realpath(os.path.dirname(path))
 
             self.path = os.path.realpath(os.path.expanduser(path))
-            self.load()
+
+            if os.path.exists(self.qlpack):
+                self.load()
 
         logger.debug(f"Finished loading Pack :: {self}")
 
     @property
     def qlpack(self) -> str:
         """QL Pack Location."""
         if self.path:
@@ -59,28 +60,44 @@
     def validate(self) -> bool:
         """Validate and check if the path is a valid CodeQL Pack."""
         return os.path.exists(self.qlpack)
 
     def load(self):
         """Load QLPack file."""
         if not os.path.exists(self.qlpack):
+            logger.warning(f"Pack Path :: {self.path}")
             raise Exception(f"Failed to find qlpack file")
 
         logger.debug(f"Loading Pack from path :: {self.path}")
         with open(self.qlpack, "r") as handle:
             data = yaml.safe_load(handle)
 
         self.library = bool(data.get("library"))
         self.name = data.get("name", "")
         self.version = data.get("version", "")
         self.default_suite = data.get("defaultSuiteFile")
 
         for name, version in data.get("dependencies", {}).items():
             self.dependencies.append(CodeQLPack(name=name, version=version))
 
+    @staticmethod
+    def findByQuery(query_path: str) -> Optional["CodeQLPack"]:
+        """Find Pack by query path."""
+        stack = query_path.split("/")
+        if query_path.startswith("/"):
+            stack.insert(0, "/")
+
+        while len(stack) != 0:
+            path = os.path.join(*stack, "qlpack.yml")
+            if os.path.exists(path):
+                return CodeQLPack(path)
+
+            stack.pop(-1)
+        return
+
     def run(self, *args, display: bool = False) -> Optional[str]:
         """Run Pack command."""
         return self.cli.runCommand("pack", *args, display=display)
 
     def create(self) -> str:
         """Create / Compile a CodeQL Pack."""
         logger.debug(f"Creating CodeQL Pack :: {self.name}")
```

### Comparing `ghastoolkit-0.6.2/src/ghastoolkit/codeql/packs/packs.py` & `ghastoolkit-0.7.0/src/ghastoolkit/codeql/packs/packs.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.2/src/ghastoolkit/codeql/results.py` & `ghastoolkit-0.7.0/src/ghastoolkit/codeql/results.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.2/src/ghastoolkit/octokit/advisories.py` & `ghastoolkit-0.7.0/src/ghastoolkit/octokit/advisories.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.2/src/ghastoolkit/octokit/clearlydefined.py` & `ghastoolkit-0.7.0/src/ghastoolkit/octokit/clearlydefined.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.2/src/ghastoolkit/octokit/codescanning.py` & `ghastoolkit-0.7.0/src/ghastoolkit/octokit/codescanning.py`

 * *Files 3% similar despite different names*

```diff
@@ -292,7 +292,21 @@
 
     def getLatestPackVersion(self, pack_name: str) -> dict:
         """Get the current remote CodeQL pack version."""
         versions = self.getPackVersions(pack_name)
         if len(versions) != 0:
             return versions[0]
         return {}
+
+    def downloadExtractorPack(self, repository_name: str, output: str) -> Optional[str]:
+        """Download Extractor Packs from GitHub Releases."""
+        owner, repo = repository_name.split("/", 1)
+
+        latest_release = self.rest.get(
+            f"/repos/{owner}/{repo}/releases/latest",
+        )
+        if not isinstance(latest_release, dict):
+            return
+        version = latest_release.get("tag_name", "0.0.0")
+        logger.debug(f"Latest Releases :: {version}")
+
+        # for asset in latest_release.get("assets", []):
```

### Comparing `ghastoolkit-0.6.2/src/ghastoolkit/octokit/dependabot.py` & `ghastoolkit-0.7.0/src/ghastoolkit/octokit/dependabot.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Dependabot API."""
 import logging
 from typing import Optional
 
 from ghastoolkit.octokit.github import GitHub, Repository
-from ghastoolkit.octokit.octokit import GraphQLRequest
+from ghastoolkit.octokit.octokit import GraphQLRequest, RestRequest
 from ghastoolkit.supplychain.advisories import Advisory
 from ghastoolkit.supplychain.dependencyalert import DependencyAlert
 
 
 logger = logging.getLogger("ghastoolkit.octokit.dependabot")
 
 
@@ -15,14 +15,37 @@
     """Dependabot API instance."""
 
     def __init__(self, repository: Optional[Repository] = None) -> None:
         """Initialise Dependabot API class."""
         self.repository = repository or GitHub.repository
         self.graphql = GraphQLRequest(repository)
 
+        self.rest = RestRequest(repository)
+
+    def isEnabled(self) -> bool:
+        """Is Dependabot enabled."""
+        try:
+            self.graphql.query(
+                "GetDependencyStatus",
+                options={"owner": self.repository.owner, "repo": self.repository.repo},
+            )
+            return True
+        except:
+            logger.debug(f"Failed to get alert count")
+        return False
+
+    def isSecurityUpdatesEnabled(self) -> bool:
+        """Is Security Updates for Dependabot enabled."""
+        result = self.rest.get("get/repos/{owner}/{repo}")
+        if not isinstance(result, dict):
+            raise Exception(f"Unable to get repository info")
+        saa = result.get("source", {}).get("security_and_analysis", {})
+        status = saa.get("dependabot_security_updates", {}).get("status", "disabled")
+        return status == "enabled"
+
     def getAlerts(self) -> list[DependencyAlert]:
         """Get All Dependabot alerts from GraphQL API using the `GetDependencyAlerts` query."""
         results = []
 
         while True:
             data = self.graphql.query(
                 "GetDependencyAlerts",
```

### Comparing `ghastoolkit-0.6.2/src/ghastoolkit/octokit/dependencygraph.py` & `ghastoolkit-0.7.0/src/ghastoolkit/octokit/dependencygraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.2/src/ghastoolkit/octokit/github.py` & `ghastoolkit-0.7.0/src/ghastoolkit/octokit/github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.2/src/ghastoolkit/octokit/octokit.py` & `ghastoolkit-0.7.0/src/ghastoolkit/octokit/octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.2/src/ghastoolkit/octokit/secretscanning.py` & `ghastoolkit-0.7.0/src/ghastoolkit/octokit/secretscanning.py`

 * *Files 9% similar despite different names*

```diff
@@ -58,35 +58,47 @@
             raise Exception("SecretScanning requires Repository to be set")
 
         self.rest = RestRequest(self.repository)
 
         self.state = None
 
     def isEnabled(self) -> bool:
-        """Check to see if Secret Scanning is enabled or not."""
+        """Check to see if Secret Scanning is enabled or not via the repository status.
+
+        https://docs.github.com/en/rest/repos/repos?apiVersion=2022-11-28#get-a-repository
+        """
         if not self.state:
             self.state = self.getStatus()
-        # if advanced_security is disabled, secret scanning will be
-        adsec = self.state.get("advanced_security", {}).get("status", "disabled")
-        return self.state.get("secret_scanning", {}).get("status", adsec) == "enabled"
+        if self.state.get("visibility") == "public":
+            logger.debug("All public repositories have secret scanning enabled")
+            return True
+        return (
+            self.state.get("security_and_analysis", {})
+            .get("secret_scanning", {})
+            .get("status", "disabled")
+            == "enabled"
+        )
 
     def isPushProtectionEnabled(self) -> bool:
         """Check if Push Protection is enabled."""
         if not self.state:
             self.state = self.getStatus()
-        status = self.state.get("secret_scanning_push_protection", {}).get(
-            "status", "disabled"
+
+        status = (
+            self.state.get("security_and_analysis", {})
+            .get("secret_scanning_push_protection", {})
+            .get("status", "disabled")
         )
         return status == "enabled"
 
     def getStatus(self) -> dict:
         """Get Status of GitHub Advanced Security."""
-        result = self.rest.get("get/repos/{owner}/{repo}")
+        result = self.rest.get("/repos/{owner}/{repo}")
         if isinstance(result, dict):
-            return result.get("source", {}).get("security_and_analysis", {})
+            return result
         raise Exception("Failed to get the current state of secret scanning")
 
     def getOrganizationAlerts(self, state: Optional[str] = None) -> list[dict]:
         """Get Organization Alerts.
 
         https://docs.github.com/en/rest/secret-scanning#list-secret-scanning-alerts-for-an-organization
         """
```

### Comparing `ghastoolkit-0.6.2/src/ghastoolkit/secretscanning/secretalerts.py` & `ghastoolkit-0.7.0/src/ghastoolkit/secretscanning/secretalerts.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.2/src/ghastoolkit/supplychain/advisories.py` & `ghastoolkit-0.7.0/src/ghastoolkit/supplychain/advisories.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.2/src/ghastoolkit/supplychain/dependencies.py` & `ghastoolkit-0.7.0/src/ghastoolkit/supplychain/dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.2/src/ghastoolkit/supplychain/dependencyalert.py` & `ghastoolkit-0.7.0/src/ghastoolkit/supplychain/dependencyalert.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.2/src/ghastoolkit/supplychain/licensing.py` & `ghastoolkit-0.7.0/src/ghastoolkit/supplychain/licensing.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.2/src/ghastoolkit.egg-info/PKG-INFO` & `ghastoolkit-0.7.0/src/ghastoolkit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.6.2
+Version: 0.7.0
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.6.2/src/ghastoolkit.egg-info/SOURCES.txt` & `ghastoolkit-0.7.0/src/ghastoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.2/tests/test_advisories.py` & `ghastoolkit-0.7.0/tests/test_advisories.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.2/tests/test_codeql_dataext.py` & `ghastoolkit-0.7.0/tests/test_codeql_dataext.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.2/tests/test_codeql_packs.py` & `ghastoolkit-0.7.0/tests/test_codeql_packs.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.2/tests/test_codeqldb.py` & `ghastoolkit-0.7.0/tests/test_codeqldb.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.2/tests/test_codescanning.py` & `ghastoolkit-0.7.0/tests/test_codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.2/tests/test_default.py` & `ghastoolkit-0.7.0/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.2/tests/test_dependencies.py` & `ghastoolkit-0.7.0/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.2/tests/test_depgraph.py` & `ghastoolkit-0.7.0/tests/test_depgraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.2/tests/test_github.py` & `ghastoolkit-0.7.0/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.2/tests/test_licenses.py` & `ghastoolkit-0.7.0/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.2/tests/test_octokit.py` & `ghastoolkit-0.7.0/tests/test_octokit.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,23 +30,23 @@
         item = loadOctoItem(Example, {"number": 5})
 
         self.assertTrue(isinstance(item, Example))
         self.assertTrue(is_dataclass(item))
 
         self.assertEqual(item.number, 5)
 
+
 class TestOctokitGraphQL(unittest.TestCase):
     def setUp(self) -> None:
         GitHub.init(repository="GeekMasher/ghastoolkit@main")
         return super().setUp()
 
     def test_loading_defaults(self):
         gql = GraphQLRequest()
-        # load 2 default queries
-        self.assertEqual(len(gql.queries.keys()), 2)
+        # load 3 default queries
+        self.assertEqual(len(gql.queries.keys()), 3)
 
         query1 = gql.queries.get("GetDependencyAlerts")
         self.assertIsNotNone(query1)
-        
+
         query2 = gql.queries.get("GetDependencyInfo")
         self.assertIsNotNone(query2)
-
```

### Comparing `ghastoolkit-0.6.2/tests/test_secretscanning.py` & `ghastoolkit-0.7.0/tests/test_secretscanning.py`

 * *Files identical despite different names*

