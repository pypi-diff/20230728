# Comparing `tmp/sphinx-asdf-0.2.0.tar.gz` & `tmp/sphinx-asdf-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-asdf-0.2.0.tar", last modified: Wed Jul  5 19:25:00 2023, max compression
+gzip compressed data, was "sphinx-asdf-0.2.1.tar", last modified: Fri Jul 28 16:15:43 2023, max compression
```

## Comparing `sphinx-asdf-0.2.0.tar` & `sphinx-asdf-0.2.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.216387 sphinx-asdf-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.208387 sphinx-asdf-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.212387 sphinx-asdf-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/.github/workflows/sphinx_asdf_ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-05 19:25:00.216387 sphinx-asdf-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/bandit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-05 19:25:00.220387 sphinx-asdf-0.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       81 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.212387 sphinx-asdf-0.2.0/sphinx_asdf/
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/sphinx_asdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-05 19:25:00.000000 sphinx-asdf-0.2.0/sphinx_asdf/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/sphinx_asdf/asdf2rst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/sphinx_asdf/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/sphinx_asdf/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    16494 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/sphinx_asdf/directives.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/sphinx_asdf/md2rst.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/sphinx_asdf/nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.216387 sphinx-asdf-0.2.0/sphinx_asdf/static/
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/sphinx_asdf/static/logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/sphinx_asdf/static/logo.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    16762 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/sphinx_asdf/static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/sphinx_asdf/static/sphinx_asdf.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/sphinx_asdf/static/sphinx_asdf.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.216387 sphinx-asdf-0.2.0/sphinx_asdf/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/sphinx_asdf/templates/schema.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.216387 sphinx-asdf-0.2.0/sphinx_asdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-05 19:25:00.000000 sphinx-asdf-0.2.0/sphinx_asdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-05 19:25:00.000000 sphinx-asdf-0.2.0/sphinx_asdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 19:25:00.000000 sphinx-asdf-0.2.0/sphinx_asdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-05 19:25:00.000000 sphinx-asdf-0.2.0/sphinx_asdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 19:25:00.000000 sphinx-asdf-0.2.0/sphinx_asdf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.216387 sphinx-asdf-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.212387 sphinx-asdf-0.2.0/tests/roots/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.216387 sphinx-asdf-0.2.0/tests/roots/test-basic-generation/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/roots/test-basic-generation/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/roots/test-basic-generation/contents.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.216387 sphinx-asdf-0.2.0/tests/roots/test-basic-generation/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/roots/test-basic-generation/schemas/bar.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.216387 sphinx-asdf-0.2.0/tests/roots/test-basic-generation/schemas/core/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/roots/test-basic-generation/schemas/core/baz.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/roots/test-basic-generation/schemas/foo.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.216387 sphinx-asdf-0.2.0/tests/roots/test-global-config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.208387 sphinx-asdf-0.2.0/tests/roots/test-global-config/a/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.208387 sphinx-asdf-0.2.0/tests/roots/test-global-config/a/b/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.208387 sphinx-asdf-0.2.0/tests/roots/test-global-config/a/b/c/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.216387 sphinx-asdf-0.2.0/tests/roots/test-global-config/a/b/c/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/roots/test-global-config/a/b/c/schemas/bar.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.216387 sphinx-asdf-0.2.0/tests/roots/test-global-config/a/b/c/schemas/core/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/roots/test-global-config/a/b/c/schemas/core/baz.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/roots/test-global-config/a/b/c/schemas/foo.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/roots/test-global-config/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/roots/test-global-config/contents.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.216387 sphinx-asdf-0.2.0/tests/roots/test-global-prefix/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/roots/test-global-prefix/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/roots/test-global-prefix/contents.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.212387 sphinx-asdf-0.2.0/tests/roots/test-global-prefix/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.212387 sphinx-asdf-0.2.0/tests/roots/test-global-prefix/schemas/a/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.212387 sphinx-asdf-0.2.0/tests/roots/test-global-prefix/schemas/a/b/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.216387 sphinx-asdf-0.2.0/tests/roots/test-global-prefix/schemas/a/b/c/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/roots/test-global-prefix/schemas/a/b/c/bar.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.216387 sphinx-asdf-0.2.0/tests/roots/test-global-prefix/schemas/a/b/c/core/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/roots/test-global-prefix/schemas/a/b/c/core/baz.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/roots/test-global-prefix/schemas/a/b/c/foo.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/test_sphinx_asdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:15:43.292274 sphinx-asdf-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:15:43.284274 sphinx-asdf-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:15:43.288274 sphinx-asdf-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/.github/workflows/sphinx_asdf_ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-28 16:15:43.292274 sphinx-asdf-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/bandit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-28 16:15:43.296274 sphinx-asdf-0.2.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       81 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:15:43.288274 sphinx-asdf-0.2.1/sphinx_asdf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/sphinx_asdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-28 16:15:43.000000 sphinx-asdf-0.2.1/sphinx_asdf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/sphinx_asdf/asdf2rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/sphinx_asdf/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/sphinx_asdf/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16494 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/sphinx_asdf/directives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/sphinx_asdf/md2rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/sphinx_asdf/nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:15:43.292274 sphinx-asdf-0.2.1/sphinx_asdf/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/sphinx_asdf/static/logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/sphinx_asdf/static/logo.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    16762 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/sphinx_asdf/static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/sphinx_asdf/static/sphinx_asdf.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/sphinx_asdf/static/sphinx_asdf.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:15:43.292274 sphinx-asdf-0.2.1/sphinx_asdf/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/sphinx_asdf/templates/schema.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:15:43.292274 sphinx-asdf-0.2.1/sphinx_asdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-28 16:15:43.000000 sphinx-asdf-0.2.1/sphinx_asdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-28 16:15:43.000000 sphinx-asdf-0.2.1/sphinx_asdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 16:15:43.000000 sphinx-asdf-0.2.1/sphinx_asdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-28 16:15:43.000000 sphinx-asdf-0.2.1/sphinx_asdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 16:15:43.000000 sphinx-asdf-0.2.1/sphinx_asdf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:15:43.292274 sphinx-asdf-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/tests/coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:15:43.288274 sphinx-asdf-0.2.1/tests/roots/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:15:43.292274 sphinx-asdf-0.2.1/tests/roots/test-basic-generation/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/tests/roots/test-basic-generation/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/tests/roots/test-basic-generation/contents.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:15:43.292274 sphinx-asdf-0.2.1/tests/roots/test-basic-generation/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/tests/roots/test-basic-generation/schemas/bar.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:15:43.292274 sphinx-asdf-0.2.1/tests/roots/test-basic-generation/schemas/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/tests/roots/test-basic-generation/schemas/core/baz.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/tests/roots/test-basic-generation/schemas/foo.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:15:43.292274 sphinx-asdf-0.2.1/tests/roots/test-global-config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:15:43.288274 sphinx-asdf-0.2.1/tests/roots/test-global-config/a/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:15:43.288274 sphinx-asdf-0.2.1/tests/roots/test-global-config/a/b/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:15:43.288274 sphinx-asdf-0.2.1/tests/roots/test-global-config/a/b/c/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:15:43.292274 sphinx-asdf-0.2.1/tests/roots/test-global-config/a/b/c/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/tests/roots/test-global-config/a/b/c/schemas/bar.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:15:43.292274 sphinx-asdf-0.2.1/tests/roots/test-global-config/a/b/c/schemas/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/tests/roots/test-global-config/a/b/c/schemas/core/baz.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/tests/roots/test-global-config/a/b/c/schemas/foo.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/tests/roots/test-global-config/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/tests/roots/test-global-config/contents.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:15:43.292274 sphinx-asdf-0.2.1/tests/roots/test-global-prefix/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/tests/roots/test-global-prefix/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/tests/roots/test-global-prefix/contents.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:15:43.288274 sphinx-asdf-0.2.1/tests/roots/test-global-prefix/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:15:43.288274 sphinx-asdf-0.2.1/tests/roots/test-global-prefix/schemas/a/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:15:43.288274 sphinx-asdf-0.2.1/tests/roots/test-global-prefix/schemas/a/b/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:15:43.292274 sphinx-asdf-0.2.1/tests/roots/test-global-prefix/schemas/a/b/c/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/tests/roots/test-global-prefix/schemas/a/b/c/bar.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:15:43.292274 sphinx-asdf-0.2.1/tests/roots/test-global-prefix/schemas/a/b/c/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/tests/roots/test-global-prefix/schemas/a/b/c/core/baz.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/tests/roots/test-global-prefix/schemas/a/b/c/foo.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/tests/test_sphinx_asdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-28 16:15:30.000000 sphinx-asdf-0.2.1/tox.ini
```

### Comparing `sphinx-asdf-0.2.0/.github/workflows/publish-to-pypi.yml` & `sphinx-asdf-0.2.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `sphinx-asdf-0.2.0/.github/workflows/sphinx_asdf_ci.yml` & `sphinx-asdf-0.2.1/.github/workflows/sphinx_asdf_ci.yml`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 jobs:
   tox_pytest:
     name: ${{ matrix.name }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         include:
+          - name: Python 3.11 Tests
+            python-version: "3.11"
+            os: ubuntu-latest
+            toxenv: py311
+
           - name: Python 3.10 Tests
             python-version: "3.10"
             os: ubuntu-latest
             toxenv: py310
 
           - name: Python 3.9, with Code Coverage
             python-version: "3.9"
@@ -77,14 +82,39 @@
             toxenv: asdf-wcs-schemas
 
           - name: ASDF-astropy Document Build
             python-version: "3.9"
             os: ubuntu-latest
             toxenv: asdf-astropy
 
+          - name: rad Document Build
+            python-version: "3.9"
+            os: ubuntu-latest
+            toxenv: rad
+
+          - name: roman_datamodels Document Build
+            python-version: "3.11"
+            os: ubuntu-latest
+            toxenv: roman_datamodels
+
+          - name: romancal Document Build
+            python-version: "3.11"
+            os: ubuntu-latest
+            toxenv: romancal
+
+          - name: stdatamodels Document Build
+            python-version: "3.10"
+            os: ubuntu-latest
+            toxenv: stdatamodels
+
+          - name: jwst Document Build
+            python-version: "3.11"
+            os: ubuntu-latest
+            toxenv: jwst
+
     steps:
       - name: Checkout code
         uses: actions/checkout@v2
         with:
           fetch-depth: 0
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
```

### Comparing `sphinx-asdf-0.2.0/.pre-commit-config.yaml` & `sphinx-asdf-0.2.1/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -8,26 +8,26 @@
   - id: check-yaml
     args: ["--unsafe"]
   - id: debug-statements
   - id: end-of-file-fixer
   - id: trailing-whitespace
 
 - repo: https://github.com/asottile/pyupgrade
-  rev: v3.8.0
+  rev: v3.9.0
   hooks:
     - id: pyupgrade
       args: ["--py38-plus"]
 
 - repo: https://github.com/pycqa/isort
   rev: 5.12.0
   hooks:
     - id: isort
 
 - repo: https://github.com/psf/black
-  rev: 23.3.0
+  rev: 23.7.0
   hooks:
     - id: black
 
 - repo: https://github.com/PyCQA/flake8
   rev: 6.0.0
   hooks:
     - id: flake8
```

### Comparing `sphinx-asdf-0.2.0/CONTRIBUTING.md` & `sphinx-asdf-0.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sphinx-asdf-0.2.0/LICENSE` & `sphinx-asdf-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-asdf-0.2.0/PKG-INFO` & `sphinx-asdf-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-asdf
-Version: 0.2.0
+Version: 0.2.1
 Summary: Sphinx plugin for generating documentation from ASDF schemas
 Home-page: https://github.com/spacetelescope/sphinx-asdf
 Author: The ASDF Developers
 License: BSD-3-Clause
 Provides: sphinx_asdf
 Requires-Python: >=3.9
 Provides-Extra: tests
```

### Comparing `sphinx-asdf-0.2.0/README.rst` & `sphinx-asdf-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx-asdf-0.2.0/setup.cfg` & `sphinx-asdf-0.2.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 include_package_data = True
 setup_requires = setuptools_scm
 install_requires = 
 	asdf
 	astropy>=5.0.4
 	docutils
 	mistune>=3
+	packaging
 	sphinx
 	sphinx-astropy
 	sphinx_bootstrap_theme
 	sphinx-rtd-theme
 	toml
 
 [options.extras_require]
```

### Comparing `sphinx-asdf-0.2.0/sphinx_asdf/__init__.py` & `sphinx-asdf-0.2.1/sphinx_asdf/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-asdf-0.2.0/sphinx_asdf/asdf2rst.py` & `sphinx-asdf-0.2.1/sphinx_asdf/asdf2rst.py`

 * *Files identical despite different names*

### Comparing `sphinx-asdf-0.2.0/sphinx_asdf/conf.py` & `sphinx-asdf-0.2.1/sphinx_asdf/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx-asdf-0.2.0/sphinx_asdf/connections.py` & `sphinx-asdf-0.2.1/sphinx_asdf/connections.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,54 @@
 import logging
 import os
 import posixpath
 import warnings
 
+import docutils
+import packaging.version
 import sphinx.builders
 from docutils import nodes
 from sphinx.util import rst
 from sphinx.util.docutils import sphinx_domains
 from sphinx.util.fileutil import copy_asset
 
 from .directives import schema_def
 from .nodes import schema_doc
 
 TEMPLATE_PATH = os.path.join(os.path.dirname(__file__), "templates")
 
+# docutils 0.19.0 fixed a bug in traverse/findall
+# https://sourceforge.net/p/docutils/bugs/448/
+# however sphinx-rtd-theme currently pins docutils to <0.19
+# docutils has since deprecated traverse so for packages that don't
+# use sphinx-rtd-theme (and will fetch 0.19.0) using findall will
+# avoid the deprecation warnings
+if packaging.version.parse(docutils.__version__) >= packaging.version.parse("0.19.0"):
+
+    def traverse(doctree, *args, **kwargs):
+        return doctree.findall(*args, **kwargs)
+
+else:
+
+    def traverse(doctree, *args, **kwargs):
+        return doctree.traverse(*args, **kwargs)
+
 
 def find_autoasdf_directives(env, filename):
     if filename.endswith(".md"):
         return []
 
     docname = env.path2doc(filename)
     env.prepare_settings(docname)
     with sphinx_domains(env), rst.default_role(docname, env.config.default_role):
         builder = sphinx.builders.text.TextBuilder(env.app, env)
         builder.read_doc(docname)
         doctree = env.get_and_resolve_doctree(docname, builder)
 
-    return doctree.findall(schema_def)
+    return traverse(doctree, schema_def)
 
 
 def find_autoschema_references(app, genfiles):
     # We set this environment variable to indicate that the AsdfSchemas
     # directive should be parsed as a simple list of schema references
     # rather than as the toctree that will be generated when the documentation
     # is actually built.
@@ -101,30 +119,30 @@
     dist = get_distribution("sphinx_asdf")
     config.html_context["sphinx_asdf_version"] = dist.version
 
 
 def handle_page_context(app, pagename, templatename, ctx, doctree):
     # Use custom template when rendering pages containing schema documentation.
     # This allows us to selectively include bootstrap
-    if doctree is not None and doctree.findall(schema_doc):
+    if doctree is not None and traverse(doctree, schema_doc):
         return os.path.join(TEMPLATE_PATH, "schema.html")
 
 
 def normalize_name(name):
     for char in [".", "_", "/"]:
         name = name.replace(char, "-")
     return name
 
 
 def add_labels_to_nodes(app, document):
     labels = app.env.domaindata["std"]["labels"]
     anonlabels = app.env.domaindata["std"]["anonlabels"]
     basepath = os.path.join("generated", app.env.config.asdf_schema_standard_prefix)
 
-    for node in document.findall():
+    for node in traverse(document):
         if isinstance(node, str) or not (isinstance(node, nodes.Node) and node["ids"]):
             continue
 
         labelid = node["ids"][0]
         docname = app.env.docname
         basename = os.path.relpath(docname, basepath)
```

### Comparing `sphinx-asdf-0.2.0/sphinx_asdf/directives.py` & `sphinx-asdf-0.2.1/sphinx_asdf/directives.py`

 * *Files identical despite different names*

### Comparing `sphinx-asdf-0.2.0/sphinx_asdf/md2rst.py` & `sphinx-asdf-0.2.1/sphinx_asdf/md2rst.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,10 +37,10 @@
 def md2rst(content):
     renderer = RSTRenderer()
     renderer.register("inline_math", inline_math_to_rst)
     renderer.register("block_math", block_math_to_rst)
     converter = mistune.create_markdown(renderer=renderer)
     INLINE_MATH_PATTERN = r"\$\$?(?!\s)(?P<math_text>.+?)(?!\s)(?<!\\)\$\$?"
     converter.inline.register("inline_math", INLINE_MATH_PATTERN, parse_inline_math, before="link")
-    BLOCK_MATH_PATTERN = r"(?s)\$\$(?P<math_text>.*?)\$\$"
+    BLOCK_MATH_PATTERN = r"\$\$(?P<math_text>[\w\W]*?)\$\$"
     converter.block.register("block_math", BLOCK_MATH_PATTERN, parse_block_math, before="list")
     return converter(content)
```

### Comparing `sphinx-asdf-0.2.0/sphinx_asdf/nodes.py` & `sphinx-asdf-0.2.1/sphinx_asdf/nodes.py`

 * *Files identical despite different names*

### Comparing `sphinx-asdf-0.2.0/sphinx_asdf/static/logo.ico` & `sphinx-asdf-0.2.1/sphinx_asdf/static/logo.ico`

 * *Files identical despite different names*

### Comparing `sphinx-asdf-0.2.0/sphinx_asdf/static/logo.pdf` & `sphinx-asdf-0.2.1/sphinx_asdf/static/logo.pdf`

 * *Files identical despite different names*

### Comparing `sphinx-asdf-0.2.0/sphinx_asdf/static/logo.png` & `sphinx-asdf-0.2.1/sphinx_asdf/static/logo.png`

 * *Files identical despite different names*

### Comparing `sphinx-asdf-0.2.0/sphinx_asdf/static/sphinx_asdf.css` & `sphinx-asdf-0.2.1/sphinx_asdf/static/sphinx_asdf.css`

 * *Files identical despite different names*

### Comparing `sphinx-asdf-0.2.0/sphinx_asdf/templates/schema.html` & `sphinx-asdf-0.2.1/sphinx_asdf/templates/schema.html`

 * *Files identical despite different names*

### Comparing `sphinx-asdf-0.2.0/sphinx_asdf.egg-info/PKG-INFO` & `sphinx-asdf-0.2.1/sphinx_asdf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-asdf
-Version: 0.2.0
+Version: 0.2.1
 Summary: Sphinx plugin for generating documentation from ASDF schemas
 Home-page: https://github.com/spacetelescope/sphinx-asdf
 Author: The ASDF Developers
 License: BSD-3-Clause
 Provides: sphinx_asdf
 Requires-Python: >=3.9
 Provides-Extra: tests
```

### Comparing `sphinx-asdf-0.2.0/sphinx_asdf.egg-info/SOURCES.txt` & `sphinx-asdf-0.2.1/sphinx_asdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sphinx-asdf-0.2.0/tests/coveragerc` & `sphinx-asdf-0.2.1/tests/coveragerc`

 * *Files identical despite different names*

### Comparing `sphinx-asdf-0.2.0/tests/test_sphinx_asdf.py` & `sphinx-asdf-0.2.1/tests/test_sphinx_asdf.py`

 * *Files identical despite different names*

