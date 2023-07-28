# Comparing `tmp/Brian2GeNN-1.6.tar.gz` & `tmp/Brian2GeNN-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Brian2GeNN-1.6.tar", last modified: Wed Jan 13 15:33:37 2021, max compression
+gzip compressed data, was "Brian2GeNN-1.7.0.tar", last modified: Fri Jul 28 13:16:05 2023, max compression
```

## Comparing `Brian2GeNN-1.6.tar` & `Brian2GeNN-1.7.0.tar`

### file list

```diff
@@ -1,71 +1,77 @@
-drwxr-xr-x   0 marcel    (1001) marcel    (1001)        0 2021-01-13 15:33:37.000000 Brian2GeNN-1.6/
-drwxr-xr-x   0 marcel    (1001) marcel    (1001)        0 2021-01-13 15:33:37.000000 Brian2GeNN-1.6/Brian2GeNN.egg-info/
--rw-r--r--   0 marcel    (1001) marcel    (1001)     2000 2021-01-13 15:33:36.000000 Brian2GeNN-1.6/Brian2GeNN.egg-info/PKG-INFO
--rw-r--r--   0 marcel    (1001) marcel    (1001)     1850 2021-01-13 15:33:36.000000 Brian2GeNN-1.6/Brian2GeNN.egg-info/SOURCES.txt
--rw-r--r--   0 marcel    (1001) marcel    (1001)        1 2021-01-13 15:33:36.000000 Brian2GeNN-1.6/Brian2GeNN.egg-info/dependency_links.txt
--rw-r--r--   0 marcel    (1001) marcel    (1001)       83 2021-01-13 15:33:36.000000 Brian2GeNN-1.6/Brian2GeNN.egg-info/requires.txt
--rw-r--r--   0 marcel    (1001) marcel    (1001)       11 2021-01-13 15:33:36.000000 Brian2GeNN-1.6/Brian2GeNN.egg-info/top_level.txt
--rw-r--r--   0 marcel    (1001) marcel    (1001)      348 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/CITATION.md
--rw-r--r--   0 marcel    (1001) marcel    (1001)    18025 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/LICENSE
--rw-r--r--   0 marcel    (1001) marcel    (1001)      116 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/MANIFEST.in
--rw-r--r--   0 marcel    (1001) marcel    (1001)     2000 2021-01-13 15:33:37.000000 Brian2GeNN-1.6/PKG-INFO
--rw-r--r--   0 marcel    (1001) marcel    (1001)      843 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/README.md
-drwxr-xr-x   0 marcel    (1001) marcel    (1001)        0 2021-01-13 15:33:37.000000 Brian2GeNN-1.6/brian2genn/
--rw-r--r--   0 marcel    (1001) marcel    (1001)     2190 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/__init__.py
-drwxr-xr-x   0 marcel    (1001) marcel    (1001)        0 2021-01-13 15:33:37.000000 Brian2GeNN-1.6/brian2genn/b2glib/
--rw-r--r--   0 marcel    (1001) marcel    (1001)     4753 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/b2glib/convert_synapses.h
--rw-r--r--   0 marcel    (1001) marcel    (1001)     2478 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/binomial.py
--rw-r--r--   0 marcel    (1001) marcel    (1001)     2101 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/codeobject.py
--rw-r--r--   0 marcel    (1001) marcel    (1001)     1039 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/correctness_testing.py
--rw-r--r--   0 marcel    (1001) marcel    (1001)    93816 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/device.py
--rw-r--r--   0 marcel    (1001) marcel    (1001)    16978 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/genn_generator.py
--rw-r--r--   0 marcel    (1001) marcel    (1001)     4936 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/insyn.py
--rw-r--r--   0 marcel    (1001) marcel    (1001)    10036 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/preferences.py
-drwxr-xr-x   0 marcel    (1001) marcel    (1001)        0 2021-01-13 15:33:37.000000 Brian2GeNN-1.6/brian2genn/sphinxext/
--rw-r--r--   0 marcel    (1001) marcel    (1001)       80 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/sphinxext/__init__.py
--rw-r--r--   0 marcel    (1001) marcel    (1001)    10215 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/sphinxext/briandoc.py
--rw-r--r--   0 marcel    (1001) marcel    (1001)    16011 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/sphinxext/docscrape.py
--rw-r--r--   0 marcel    (1001) marcel    (1001)     8638 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/sphinxext/docscrape_sphinx.py
--rw-r--r--   0 marcel    (1001) marcel    (1001)     2684 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/sphinxext/examplefinder.py
--rw-r--r--   0 marcel    (1001) marcel    (1001)     5695 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/sphinxext/generate_examples.py
--rw-r--r--   0 marcel    (1001) marcel    (1001)     9702 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/sphinxext/generate_reference.py
-drwxr-xr-x   0 marcel    (1001) marcel    (1001)        0 2021-01-13 15:33:37.000000 Brian2GeNN-1.6/brian2genn/templates/
--rw-r--r--   0 marcel    (1001) marcel    (1001)      580 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/templates/Makefile
--rw-r--r--   0 marcel    (1001) marcel    (1001)    12820 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/templates/engine.cpp
--rw-r--r--   0 marcel    (1001) marcel    (1001)     8900 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/templates/main.cpp
--rw-r--r--   0 marcel    (1001) marcel    (1001)     1725 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/templates/max_row_length_array.cpp
--rw-r--r--   0 marcel    (1001) marcel    (1001)     6686 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/templates/max_row_length_generator.cpp
--rw-r--r--   0 marcel    (1001) marcel    (1001)     9466 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/templates/model.cpp
--rw-r--r--   0 marcel    (1001) marcel    (1001)      328 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/templates/network.cpp
--rw-r--r--   0 marcel    (1001) marcel    (1001)      675 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/templates/neuron_code.cpp
--rw-r--r--   0 marcel    (1001) marcel    (1001)     3136 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/templates/project_vcxproj
--rw-r--r--   0 marcel    (1001) marcel    (1001)      980 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/templates/ratemonitor.cpp
--rw-r--r--   0 marcel    (1001) marcel    (1001)      173 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/templates/reset.cpp
--rw-r--r--   0 marcel    (1001) marcel    (1001)     1167 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/templates/spikegenerator.cpp
--rw-r--r--   0 marcel    (1001) marcel    (1001)     1618 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/templates/spikemonitor.cpp
--rw-r--r--   0 marcel    (1001) marcel    (1001)     1210 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/templates/statemonitor.cpp
--rw-r--r--   0 marcel    (1001) marcel    (1001)      204 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/templates/stateupdate.cpp
--rw-r--r--   0 marcel    (1001) marcel    (1001)      204 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/templates/synapses.cpp
--rw-r--r--   0 marcel    (1001) marcel    (1001)      981 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/templates/template_notes.txt
--rw-r--r--   0 marcel    (1001) marcel    (1001)      260 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/brian2genn/templates/threshold.cpp
-drwxr-xr-x   0 marcel    (1001) marcel    (1001)        0 2021-01-13 15:33:37.000000 Brian2GeNN-1.6/docs_sphinx/
--rw-r--r--   0 marcel    (1001) marcel    (1001)    10654 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/docs_sphinx/conf.py
--rw-r--r--   0 marcel    (1001) marcel    (1001)      428 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/docs_sphinx/index.rst
-drwxr-xr-x   0 marcel    (1001) marcel    (1001)        0 2021-01-13 15:33:37.000000 Brian2GeNN-1.6/docs_sphinx/introduction/
--rw-r--r--   0 marcel    (1001) marcel    (1001)     5534 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/docs_sphinx/introduction/exclusions.rst
--rw-r--r--   0 marcel    (1001) marcel    (1001)     3330 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/docs_sphinx/introduction/index.rst
--rw-r--r--   0 marcel    (1001) marcel    (1001)     3449 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/docs_sphinx/introduction/preferences.rst
-drwxr-xr-x   0 marcel    (1001) marcel    (1001)        0 2021-01-13 15:33:37.000000 Brian2GeNN-1.6/docs_sphinx/technical/
--rw-r--r--   0 marcel    (1001) marcel    (1001)     4158 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/docs_sphinx/technical/how_it_works.rst
-drwxr-xr-x   0 marcel    (1001) marcel    (1001)        0 2021-01-13 15:33:37.000000 Brian2GeNN-1.6/examples/
--rw-r--r--   0 marcel    (1001) marcel    (1001)      403 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/examples/insyn_translation.py
--rw-r--r--   0 marcel    (1001) marcel    (1001)      338 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/examples/shortEx.py
--rw-r--r--   0 marcel    (1001) marcel    (1001)      248 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/examples/simple_example.py
--rw-r--r--   0 marcel    (1001) marcel    (1001)      550 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/examples/simple_example_HH.py
--rw-r--r--   0 marcel    (1001) marcel    (1001)      662 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/examples/simple_example_HH_CPP.py
--rw-r--r--   0 marcel    (1001) marcel    (1001)      978 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/examples/simple_example_synapses.py
--rw-r--r--   0 marcel    (1001) marcel    (1001)      471 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/examples/simple_example_with_synapses.py
--rw-r--r--   0 marcel    (1001) marcel    (1001)      414 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/examples/simple_spikesource.py
--rw-r--r--   0 marcel    (1001) marcel    (1001)      733 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/examples/testSummedVars.py
--rw-r--r--   0 marcel    (1001) marcel    (1001)       38 2021-01-13 15:33:37.000000 Brian2GeNN-1.6/setup.cfg
--rw-r--r--   0 marcel    (1001) marcel    (1001)     3005 2021-01-13 15:33:22.000000 Brian2GeNN-1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:16:05.930124 Brian2GeNN-1.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:16:05.922124 Brian2GeNN-1.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:16:05.922124 Brian2GeNN-1.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/.github/workflows/test_latest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/.github/workflows/testsuite.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:16:05.922124 Brian2GeNN-1.7.0/Brian2GeNN.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-28 13:16:05.000000 Brian2GeNN-1.7.0/Brian2GeNN.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-28 13:16:05.000000 Brian2GeNN-1.7.0/Brian2GeNN.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:16:05.000000 Brian2GeNN-1.7.0/Brian2GeNN.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:16:05.000000 Brian2GeNN-1.7.0/Brian2GeNN.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-28 13:16:05.000000 Brian2GeNN-1.7.0/Brian2GeNN.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 13:16:05.000000 Brian2GeNN-1.7.0/Brian2GeNN.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/CITATION.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18025 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-28 13:16:05.930124 Brian2GeNN-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:16:05.922124 Brian2GeNN-1.7.0/brian2genn/
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-28 13:16:05.000000 Brian2GeNN-1.7.0/brian2genn/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:16:05.926124 Brian2GeNN-1.7.0/brian2genn/b2glib/
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/b2glib/convert_synapses.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/binomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/codeobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/correctness_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99143 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16881 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/genn_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/insyn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/preferences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:16:05.926124 Brian2GeNN-1.7.0/brian2genn/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/sphinxext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/sphinxext/briandoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15967 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/sphinxext/docscrape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/sphinxext/docscrape_sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9505 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/sphinxext/generate_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:16:05.926124 Brian2GeNN-1.7.0/brian2genn/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/templates/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    14864 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/templates/engine.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/templates/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/templates/max_row_length_array.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/templates/max_row_length_generator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/templates/model.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/templates/network.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/templates/neuron_code.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/templates/project_vcxproj
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/templates/ratemonitor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/templates/reset.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/templates/spikegenerator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/templates/spikemonitor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/templates/statemonitor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/templates/stateupdate.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/templates/synapses.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/templates/template_notes.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/brian2genn/templates/threshold.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:16:05.926124 Brian2GeNN-1.7.0/docs_sphinx/
+-rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/docs_sphinx/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/docs_sphinx/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:16:05.926124 Brian2GeNN-1.7.0/docs_sphinx/introduction/
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/docs_sphinx/introduction/exclusions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/docs_sphinx/introduction/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/docs_sphinx/introduction/preferences.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:16:05.926124 Brian2GeNN-1.7.0/docs_sphinx/technical/
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/docs_sphinx/technical/how_it_works.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:16:05.926124 Brian2GeNN-1.7.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/examples/insyn_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/examples/shortEx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/examples/simple_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/examples/simple_example_HH.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/examples/simple_example_HH_CPP.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/examples/simple_example_synapses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/examples/simple_example_with_synapses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/examples/simple_spikesource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/examples/testSummedVars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-28 13:15:56.000000 Brian2GeNN-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 13:16:05.930124 Brian2GeNN-1.7.0/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Brian2GeNN-1.6/Brian2GeNN.egg-info/PKG-INFO` & `Brian2GeNN-1.7.0/Brian2GeNN.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 Metadata-Version: 2.1
 Name: Brian2GeNN
-Version: 1.6
+Version: 1.7.0
 Summary: An interface to use the GeNN framework as a device in Brian 2
-Home-page: http://github.com/brian-team/brian2genn
 Author: Thomas Nowotny, Marcel Stimberg, Dan Goodman
-Author-email: t.nowotny@sussex.ac.uk
-License: UNKNOWN
-Description: 
-        Brian2GeNN is an interface between Brian 2 and GeNN. Brian2 is a simulator for spiking neural networks available on a variety of platforms. It is the successor of Brian1 and shares its approach of being highly flexible and easily extensible. It is based on a code generation framework that allows to execute simulations using other programming languages and/or on different
-        devices. 
-        
-        GeNN (GPU enhanced Neuronal Networksm, https://github.com/genn-team/genn) is a framework that uses code generation methods to allow using GPU accelerators without in-depth knowledge of the CUDA programming interface.
-        
-        Brian2Genn provides an interface to use GeNN as a backend device in Brian2. This allows users to run their Brian 2 scripts on NVIDIA GPU accelerators without any further necessary programming.
-        
-        We currently consider this software to be in the beta status, please report
-        issues to the github issue tracker (https://github.com/brian-team/brian2genn/issues).
-        
-        Documentation for Brian2GeNN can be found at http://brian2genn.readthedocs.org
-        
-Platform: UNKNOWN
+Project-URL: Documentation, https://brian2genn.readthedocs.io/
+Project-URL: Source, https://github.com/brian-team/brian2genn
+Project-URL: Tracker, https://github.com/brian-team/brian2genn/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Intended Audience :: Science/Research
-Provides: brian2genn
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: test
 Provides-Extra: docs
+License-File: LICENSE
+
+Brian2GeNN
+==========
+Brian2GeNN is an interface between Brian 2 and GeNN. Brian2 is a simulator for spiking neural networks available on a variety of platforms. It is the successor of Brian1 and shares its approach of being highly flexible and easily extensible. It is based on a code generation framework that allows to execute simulations using other programming languages and/or on different
+devices. 
+
+GeNN (GPU enhanced Neuronal Networks, https://github.com/genn-team/genn) is a framework that uses code generation methods to allow using GPU accelerators without in-depth knowledge of the CUDA programming interface.
+
+Brian2Genn provides an interface to use GeNN as a backend device in Brian2. This allows users to run their Brian 2 scripts on NVIDIA GPU accelerators without any further necessary programming.
+
+We currently consider this software to be in the beta status, please report
+issues to the github issue tracker (https://github.com/brian-team/brian2genn/issues).
+
+Documentation for Brian2GeNN can be found at http://brian2genn.readthedocs.org
+
+[![PyPI package](https://img.shields.io/pypi/v/Brian2GeNN.svg)](https://pypi.python.org/pypi/Brian2GeNN)
+[![Documentation Status](https://readthedocs.org/projects/brian2genn/badge/?version=stable)](https://brian2genn.readthedocs.io/en/stable/?badge=stable)
+[![Build Status](https://github.com/brian-team/brian2genn/actions/workflows/testsuite.yml/badge.svg)](https://github.com/brian-team/brian2genn/actions/workflows/testsuite.yml)
+
+If you use BrianGeNN for your published research, we kindly ask you to cite our article:  
+Marcel Stimberg, Dan F. M. Goodman, and Thomas Nowotny. “Brian2GeNN: Accelerating Spiking Neural Network Simulations with Graphics Hardware.” Sci Rep 10 (January 2020): 410. [doi: 10.1038/s41598-019-54957-7](https://doi.org/10.1038/s41598-019-54957-7).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Brian2GeNN-1.6/Brian2GeNN.egg-info/SOURCES.txt` & `Brian2GeNN-1.7.0/Brian2GeNN.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,36 @@
+.readthedocs.yaml
 CITATION.md
 LICENSE
 MANIFEST.in
 README.md
-setup.py
+pyproject.toml
+.github/workflows/publish_to_pypi.yml
+.github/workflows/test_latest.yml
+.github/workflows/testsuite.yml
 Brian2GeNN.egg-info/PKG-INFO
 Brian2GeNN.egg-info/SOURCES.txt
 Brian2GeNN.egg-info/dependency_links.txt
+Brian2GeNN.egg-info/not-zip-safe
 Brian2GeNN.egg-info/requires.txt
 Brian2GeNN.egg-info/top_level.txt
 brian2genn/__init__.py
+brian2genn/_version.py
 brian2genn/binomial.py
 brian2genn/codeobject.py
 brian2genn/correctness_testing.py
 brian2genn/device.py
 brian2genn/genn_generator.py
 brian2genn/insyn.py
 brian2genn/preferences.py
 brian2genn/b2glib/convert_synapses.h
 brian2genn/sphinxext/__init__.py
 brian2genn/sphinxext/briandoc.py
 brian2genn/sphinxext/docscrape.py
 brian2genn/sphinxext/docscrape_sphinx.py
-brian2genn/sphinxext/examplefinder.py
-brian2genn/sphinxext/generate_examples.py
 brian2genn/sphinxext/generate_reference.py
 brian2genn/templates/Makefile
 brian2genn/templates/engine.cpp
 brian2genn/templates/main.cpp
 brian2genn/templates/max_row_length_array.cpp
 brian2genn/templates/max_row_length_generator.cpp
 brian2genn/templates/model.cpp
```

### Comparing `Brian2GeNN-1.6/LICENSE` & `Brian2GeNN-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Brian2GeNN-1.6/PKG-INFO` & `Brian2GeNN-1.7.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 Metadata-Version: 2.1
 Name: Brian2GeNN
-Version: 1.6
+Version: 1.7.0
 Summary: An interface to use the GeNN framework as a device in Brian 2
-Home-page: http://github.com/brian-team/brian2genn
 Author: Thomas Nowotny, Marcel Stimberg, Dan Goodman
-Author-email: t.nowotny@sussex.ac.uk
-License: UNKNOWN
-Description: 
-        Brian2GeNN is an interface between Brian 2 and GeNN. Brian2 is a simulator for spiking neural networks available on a variety of platforms. It is the successor of Brian1 and shares its approach of being highly flexible and easily extensible. It is based on a code generation framework that allows to execute simulations using other programming languages and/or on different
-        devices. 
-        
-        GeNN (GPU enhanced Neuronal Networksm, https://github.com/genn-team/genn) is a framework that uses code generation methods to allow using GPU accelerators without in-depth knowledge of the CUDA programming interface.
-        
-        Brian2Genn provides an interface to use GeNN as a backend device in Brian2. This allows users to run their Brian 2 scripts on NVIDIA GPU accelerators without any further necessary programming.
-        
-        We currently consider this software to be in the beta status, please report
-        issues to the github issue tracker (https://github.com/brian-team/brian2genn/issues).
-        
-        Documentation for Brian2GeNN can be found at http://brian2genn.readthedocs.org
-        
-Platform: UNKNOWN
+Project-URL: Documentation, https://brian2genn.readthedocs.io/
+Project-URL: Source, https://github.com/brian-team/brian2genn
+Project-URL: Tracker, https://github.com/brian-team/brian2genn/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Intended Audience :: Science/Research
-Provides: brian2genn
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: test
 Provides-Extra: docs
+License-File: LICENSE
+
+Brian2GeNN
+==========
+Brian2GeNN is an interface between Brian 2 and GeNN. Brian2 is a simulator for spiking neural networks available on a variety of platforms. It is the successor of Brian1 and shares its approach of being highly flexible and easily extensible. It is based on a code generation framework that allows to execute simulations using other programming languages and/or on different
+devices. 
+
+GeNN (GPU enhanced Neuronal Networks, https://github.com/genn-team/genn) is a framework that uses code generation methods to allow using GPU accelerators without in-depth knowledge of the CUDA programming interface.
+
+Brian2Genn provides an interface to use GeNN as a backend device in Brian2. This allows users to run their Brian 2 scripts on NVIDIA GPU accelerators without any further necessary programming.
+
+We currently consider this software to be in the beta status, please report
+issues to the github issue tracker (https://github.com/brian-team/brian2genn/issues).
+
+Documentation for Brian2GeNN can be found at http://brian2genn.readthedocs.org
+
+[![PyPI package](https://img.shields.io/pypi/v/Brian2GeNN.svg)](https://pypi.python.org/pypi/Brian2GeNN)
+[![Documentation Status](https://readthedocs.org/projects/brian2genn/badge/?version=stable)](https://brian2genn.readthedocs.io/en/stable/?badge=stable)
+[![Build Status](https://github.com/brian-team/brian2genn/actions/workflows/testsuite.yml/badge.svg)](https://github.com/brian-team/brian2genn/actions/workflows/testsuite.yml)
+
+If you use BrianGeNN for your published research, we kindly ask you to cite our article:  
+Marcel Stimberg, Dan F. M. Goodman, and Thomas Nowotny. “Brian2GeNN: Accelerating Spiking Neural Network Simulations with Graphics Hardware.” Sci Rep 10 (January 2020): 410. [doi: 10.1038/s41598-019-54957-7](https://doi.org/10.1038/s41598-019-54957-7).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Brian2GeNN-1.6/brian2genn/__init__.py` & `Brian2GeNN-1.7.0/brian2genn/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,27 +4,35 @@
 from brian2genn.codeobject import GeNNCodeObject
 from brian2genn.device import genn_device
 # Register preferences and the binomial implementation:
 import brian2genn.preferences
 import brian2genn.binomial
 
 
-from pkg_resources import get_distribution, DistributionNotFound
 try:
-    __version__ = get_distribution(__name__).version
-except DistributionNotFound:
-    # Apparently we are running directly from a git clone, let
-    # setuptools_scm fetch the version from git
+    from ._version import __version__, __version_tuple__
+except ImportError:
     try:
         from setuptools_scm import get_version
-        __version__ = get_version(relative_to=os.path.dirname(__file__))
+
+        __version__ = get_version(
+            root="..",
+            relative_to=__file__,
+            version_scheme="post-release",
+            local_scheme="no-local-version",
+        )
+        __version_tuple__ = tuple(int(x) if x.isdigit() else x
+                                  for x in __version__.split("."))
     except ImportError:
-        warnings.warn('Cannot determine brian2genn version (running directly '
-                      'from source code and no setuptools_scm package '
-                      'available).')
+        warnings.warn(
+            "Cannot determine Brian version, running from source and "
+            "setuptools_scm is not installed."
+        )
+        __version__ = "unknown"
+        __version_tuple__ = (0, 0, 0)
 
 
 def example_run(debug=False, **build_options):
     '''
     Run a simple example simulation that test whether the Brian2/Brian2GeNN/GeNN
     pipeline is working correctly.
```

### Comparing `Brian2GeNN-1.6/brian2genn/b2glib/convert_synapses.h` & `Brian2GeNN-1.7.0/brian2genn/b2glib/convert_synapses.h`

 * *Files identical despite different names*

### Comparing `Brian2GeNN-1.6/brian2genn/binomial.py` & `Brian2GeNN-1.7.0/brian2genn/binomial.py`

 * *Files identical despite different names*

### Comparing `Brian2GeNN-1.6/brian2genn/codeobject.py` & `Brian2GeNN-1.7.0/brian2genn/codeobject.py`

 * *Files identical despite different names*

### Comparing `Brian2GeNN-1.6/brian2genn/correctness_testing.py` & `Brian2GeNN-1.7.0/brian2genn/correctness_testing.py`

 * *Files identical despite different names*

### Comparing `Brian2GeNN-1.6/brian2genn/device.py` & `Brian2GeNN-1.7.0/brian2genn/device.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 import re
 import shutil
 import sys
 
 from pkg_resources import parse_version
 from subprocess import call, check_call, CalledProcessError
 import inspect
-from builtins import map, range
 from collections import defaultdict
-from six import iteritems, iterkeys, itervalues
 import tempfile
 import itertools
 import numpy
 import numbers
 from collections import Counter
 
 from brian2.codegen.cpp_prefs import get_msvc_env
@@ -28,15 +26,15 @@
 from brian2.units import second
 from brian2.codegen.generators.cpp_generator import (c_data_type,
                                                      CPPCodeGenerator)
 from brian2.codegen.templates import MultiTemplate
 from brian2.core.clocks import defaultclock
 from brian2.core.variables import *
 from brian2.core.functions import Function
-from brian2.core.network import Network
+from brian2.core.network import _get_all_objects
 from brian2.devices.device import all_devices
 from brian2.devices.cpp_standalone.device import CPPStandaloneDevice
 from brian2.parsing.rendering import CPPNodeRenderer
 from brian2.synapses.synapses import Synapses, SynapticPathway
 from brian2.monitors.spikemonitor import SpikeMonitor
 from brian2.monitors.ratemonitor import PopulationRateMonitor
 from brian2.monitors.statemonitor import StateMonitor
@@ -77,15 +75,15 @@
 
 
 def freeze(code, ns):
     '''
     Support function for substituting constant values.
     '''
     # this is a bit of a hack, it should be passed to the template somehow
-    for k, v in iteritems(ns):
+    for k, v in ns.items():
 
         if (isinstance(v, Variable) and
                 v.scalar and v.constant and v.read_only):
             try:
                 v = v.get_value()
             except NotImplementedError:
                 continue
@@ -140,15 +138,15 @@
 
 
 def extract_source_variables(variables, varname, smvariables):
     '''Support function to extract the "atomic" variables used in a variable
     that is of instance `Subexpression`.
     '''
     identifiers = get_identifiers(variables[varname].expr)
-    for vnm, var in iteritems(variables):
+    for vnm, var in variables.items():
         if vnm in identifiers:
             if var in defaultclock.variables.values():
                 raise NotImplementedError('Recording an expression that depends on '
                                           'the time t or the timestep dt is '
                                           'currently not supported in Brian2GeNN')
             elif isinstance(var, ArrayVariable):
                 smvariables.append(vnm)
@@ -156,30 +154,30 @@
                 smvariables = extract_source_variables(variables, vnm,
                                                        smvariables)
     return smvariables
 
 def find_executable(executable):
     """Tries to find 'executable' in the path
 
-    Modified version of distutils.spawn.find_executable as 
-    this has stupid rules for extensions on Windows. 
+    Modified version of distutils.spawn.find_executable as
+    this has stupid rules for extensions on Windows.
     Returns the complete filename or None if not found.
     """
     path = os.environ.get('PATH', os.defpath)
 
     paths = path.split(os.pathsep)
 
     for p in paths:
         f = os.path.join(p, executable)
         if os.path.isfile(f):
             # the file exists, we have a shot at spawn working
             return f
     return None
 
-class DelayedCodeObject(object):
+class DelayedCodeObject:
     '''
     Dummy class used for delaying the CodeObject creation of stateupdater,
     thresholder, and resetter of a NeuronGroup (which will all be merged into a
     single code object).
     '''
     def __init__(self, owner, name, abstract_code, variables, variable_indices,
                  override_conditional_write):
@@ -193,17 +191,17 @@
     def before_run(self):
         pass
 
     def after_run(self):
         pass
 
 
-class neuronModel(object):
+class neuronModel:
     '''
-    Class that contains all relevant information of a neuron model. 
+    Class that contains all relevant information of a neuron model.
     '''
 
     def __init__(self):
         self.name = ''
         self.clock = None
         self.N = 0
         self.variables = []
@@ -215,25 +213,25 @@
         self.pvalue = []
         self.code_lines = []
         self.thresh_cond_lines = []
         self.reset_code_lines = []
         self.support_code_lines = []
 
 
-class spikegeneratorModel(object):
+class spikegeneratorModel:
     '''
     Class that contains all relevant information of a spike generator group.
     '''
     def __init__(self):
         self.name = ''
         self.codeobject_name = ''
         self.N = 0
 
 
-class synapseModel(object):
+class synapseModel:
     '''
     Class that contains all relevant information about a synapse model.
     '''
     def __init__(self):
         self.name = ''
         self.srcname = ''
         self.srcN = 0
@@ -253,65 +251,66 @@
         # and post-synaptic pathway and "dynamics" for the synaptic dynamics
         self.main_code_lines = defaultdict(str)
         self.support_code_lines = defaultdict(str)
         self.connectivity = ''
         self.delay = 0
         self.summed_variables= None
 
-class spikeMonitorModel(object):
+class spikeMonitorModel:
     '''
     Class the contains all relevant information about a spike monitor.
     '''
     def __init__(self):
         self.name = ''
         self.codeobject_name = ''
         self.neuronGroup = ''
         self.notSpikeGeneratorGroup = True
 
 
-class rateMonitorModel(object):
+class rateMonitorModel:
     '''
     CLass that contains all relevant information about a rate monitor.
     '''
     def __init__(self):
         self.name = ''
         self.codeobject_name = ''
         self.neuronGroup = ''
         self.notSpikeGeneratorGroup = True
 
 
-class stateMonitorModel(object):
+class stateMonitorModel:
     '''
     Class that contains all relvant information about a state monitor.
     '''
     def __init__(self):
         self.name = ''
         self.codeobject_name = ''
         self.order = 0
         self.monitored = ''
         self.src = None
         self.isSynaptic = False
         self.variables = []
         self.srcN = 0
         self.trgN = 0
         self.when = ''
+        self.step = 1
         self.connectivity = ''
 
 
 # ------------------------------------------------------------------------------
 # Start of GeNNDevice
 # ------------------------------------------------------------------------------
 
 class GeNNDevice(CPPStandaloneDevice):
     '''
     The main "genn" device. This does most of the translation work from Brian 2
     generated code to functional GeNN code, assisted by the "GeNN language".
     '''
     def __init__(self):
-        super(GeNNDevice, self).__init__()
+        super().__init__()
         # Remember whether we have already passed the "run" statement
         self.run_statement_used = False
         self.network_schedule = ['start', 'synapses', 'groups', 'thresholds',
                                  'resets', 'end']
         self.neuron_models = []
         self.spikegenerator_models = []
         self.synapse_models = []
@@ -322,76 +321,80 @@
         self.delays = {}
         self.spike_monitor_models = []
         self.rate_monitor_models = []
         self.state_monitor_models = []
         self.run_regularly_read_write = {}
         self.run_duration = None
         self.net = None
+        self.net_objects = set()
         self.simple_code_objects = {}
         self.report_func = ''
         self.src_counts= dict()
         self.trg_counts= dict()
         #: Set of all source and header files (to be included in runner)
         self.source_files = set()
         self.header_files = set()
 
         self.connectivityDict = dict()
         self.groupDict = dict()
 
         # Overwrite the code slots defined in standard C++ standalone
         self.code_lines = {'before_start': [],
                            'after_start': [],
-                           'before_run': [],
-                           'after_run': [],
+                           'before_network_run': [],
+                           'after_network_run': [],
                            'before_end': [],
                            'after_end': []}
 
+        #: Use GeNN's kernel timings?
+        self.kernel_timings = False
+
     def insert_code(self, slot, code):
         '''
         Insert custom C++ code directly into ``main.cpp``. The available slots
         are:
 
         ``before_start`` / ``after_start``
             Before/after allocating memory for the arrays and loading arrays from
             disk.
-        ``before_run`` / ``after_run``
+        ``before_network_run`` / ``after_network_run``
             Before/after calling GeNN's ``run`` function.
         ``before_end`` / ``after_end``
             Before/after writing results to disk and deallocating memory.
 
         Parameters
         ----------
         slot : str
             The name of the slot where the code will be placed (see above for
             list of available slots).
         code : str
             The C++ code that should be inserted.
         '''
         # Only overwritten so that we can have custom documentation
-        super(GeNNDevice, self).insert_code(slot, code)
+        super().insert_code(slot, code)
 
     def activate(self, build_on_run=True, **kwargs):
         new_prefs = {'codegen.generators.cpp.restrict_keyword': '__restrict',
                      'codegen.loop_invariant_optimisations': False,
                      'core.network.default_schedule': ['start', 'synapses',
                                                        'groups', 'thresholds',
                                                        'resets', 'end']}
         changed = []
-        for new_pref, new_value in iteritems(new_prefs):
+        for new_pref, new_value in new_prefs.items():
             if prefs[new_pref] != new_value:
                 changed.append(new_pref)
                 prefs[new_pref] = new_value
 
         if changed:
             logger.info('The following preferences have been changed for '
                         'Brian2GeNN, reset them manually if you use a '
                         'different device later in the same script: '
                         '{}'.format(', '.join(changed)), once=True)
             prefs._backup()
-        super(GeNNDevice, self).activate(build_on_run, **kwargs)
+        super().activate(build_on_run, **kwargs)
 
     def code_object_class(self, codeobj_class=None, *args, **kwds):
         if codeobj_class is None:
             codeobj_class = GeNNUserCodeObject
         return codeobj_class
 
     def code_object(self, owner, name, abstract_code, variables, template_name,
@@ -402,23 +405,24 @@
         arrays for `GeNNCodeObjects` and `GeNNUserCodeObjects`.
         '''
         if '_run_regularly_' in name:
             variables['N'] = owner.variables['N']
             # Add an extra code object that executes the scalar code of
             # the run_regularly operation (will be directly called from
             # engine.cpp)
-            codeobj = super(GeNNDevice, self).code_object(owner, name,
-                                                          abstract_code,
-                                                          variables,
-                                                          'stateupdate',
-                                                          variable_indices,
-                                                          codeobj_class=CPPStandaloneCodeObject,
-                                                          template_kwds=template_kwds,
-                                                          override_conditional_write=override_conditional_write,
-                                                          )
+            codeobj = super().code_object(owner, name,
+                                          abstract_code,
+                                          variables,
+                                          'stateupdate',
+                                          variable_indices,
+                                          codeobj_class=CPPStandaloneCodeObject,
+                                          template_kwds=template_kwds,
+                                          override_conditional_write=override_conditional_write,
+                                          )
+
             # FIXME: The following is redundant with what is done during
             # the code object creation above. At the moment, the code
             # object does not allow us to access the information we
             # need (variables that are read/written by the run_regularly
             # code), though.
             generator = CPPCodeGenerator(variables,
                                          variable_indices, owner=owner,
@@ -459,66 +463,66 @@
                 if (isinstance(var, ArrayVariable) and
                     not var.read_only):
                     self.array_cache[var] = None
             self.simple_code_objects[name] = codeobj
 
         elif template_name in ['reset', 'synapses', 'stateupdate', 'threshold']:
             codeobj_class = GeNNCodeObject
-            codeobj = super(GeNNDevice, self).code_object(owner, name,
-                                                          abstract_code,
-                                                          variables,
-                                                          template_name,
-                                                          variable_indices,
-                                                          codeobj_class=codeobj_class,
-                                                          template_kwds=template_kwds,
-                                                          override_conditional_write=override_conditional_write,
+            codeobj = super().code_object(owner, name,
+                                          abstract_code,
+                                          variables,
+                                          template_name,
+                                          variable_indices,
+                                          codeobj_class=codeobj_class,
+                                          template_kwds=template_kwds,
+                                          override_conditional_write=override_conditional_write,
                                                           )
             self.simple_code_objects[codeobj.name] = codeobj
         else:
             codeobj_class = GeNNUserCodeObject
             if ('_synapses_create_generator_' in name) or ('_synapses_create_array_' in name):
-                # Here we process max_row_length for synapses 
+                # Here we process max_row_length for synapses
                 # the strategy is to do a dry run of connection generationin in the model definition
                 # function that has the same random numbers and just counts synaptic connections
                 # rather than generating them for real
                 generator= '_synapses_create_generator_' in name
                 mrl_name= '%s_max_row_length' % owner.name
                 i= 1
                 while mrl_name in self.max_row_length_code_objects:
                     mrl_name= '%s_max_row_length_%d' % (owner.name, i)
                     i= i+1
                 if generator:
                     mrl_template_name= 'max_row_length_generator'
                 else:
                     mrl_template_name='max_row_length_array'
-                codeobj = super(GeNNDevice, self).code_object(owner, mrl_name,
-                                                              abstract_code,
-                                                              variables,
-                                                              mrl_template_name,
-                                                              variable_indices,
-                                                              codeobj_class=codeobj_class,
-                                                              template_kwds=template_kwds,
-                                                              override_conditional_write=override_conditional_write,
+                codeobj = super().code_object(owner, mrl_name,
+                                              abstract_code,
+                                              variables,
+                                              mrl_template_name,
+                                              variable_indices,
+                                              codeobj_class=codeobj_class,
+                                              template_kwds=template_kwds,
+                                              override_conditional_write=override_conditional_write,
                 )
                 #self.code_objects['%s_max_row_length' % owner.name] = codeobj
                 self.code_objects.pop(mrl_name, None)   # remove this from the normal list of code objects
                 self.max_row_length_code_objects[mrl_name]= codeobj # add to this dict instead
                 self.max_row_length_synapses.add(owner.name)
                 self.max_row_length_include.append('#include "code_objects/%s.cpp"' % codeobj.name)
                 self.max_row_length_run_calls.append('_run_%s();' % mrl_name)
 
-            codeobj = super(GeNNDevice, self).code_object(owner, name,
-                                                          abstract_code,
-                                                          variables,
-                                                          template_name,
-                                                          variable_indices,
-                                                          codeobj_class=codeobj_class,
-                                                          template_kwds=template_kwds,
-                                                          override_conditional_write=override_conditional_write,
-                                                          )
+            codeobj = super().code_object(owner, name,
+                                          abstract_code,
+                                          variables,
+                                          template_name,
+                                          variable_indices,
+                                          codeobj_class=codeobj_class,
+                                          template_kwds=template_kwds,
+                                          override_conditional_write=override_conditional_write,
+                                          )
             # FIXME: is this actually necessary or is it already added by the super?
             self.code_objects[codeobj.name] = codeobj
         return codeobj
 
     # The following two methods are only overwritten to catch assignments to the
     # delay variable -- GeNN does not support heterogeneous delays
     def fill_with_array(self, var, arr):
@@ -542,26 +546,26 @@
             if arr == -numpy.inf:
                 logger.warn('Initializing the lastspike variable with -10000s '
                             'instead of -inf to copy the behaviour of Brian 2 '
                             'for versions >= 2.2 -- upgrade Brian 2 to remove '
                             'this warning',
                             name_suffix='lastspike_inf', once=True)
                 arr = numpy.array(-1e4)
-        super(GeNNDevice, self).fill_with_array(var, arr)
+        super().fill_with_array(var, arr)
 
     def variableview_set_with_index_array(self, variableview, item,
                                           value, check_units):
         var = variableview.variable
         if isinstance(var.owner, Synapses) and var.name == 'delay':
             raise NotImplementedError('GeNN does not support assigning to the '
                                       'delay variable -- set the delay for all '
                                       'synapses (heterogeneous delays are not '
                                       'supported) as an argument to the '
                                       'Synapses initializer.')
-        super(GeNNDevice, self).variableview_set_with_index_array(variableview,
+        super().variableview_set_with_index_array(variableview,
                                                                   item,
                                                                   value,
                                                                   check_units)
 
     def variableview_set_with_expression(self, variableview, item, code, run_namespace, check_units=True):
         var = variableview.variable
         if isinstance(var.owner, Synapses) and var.name == 'delay':
@@ -685,15 +689,15 @@
             elif func == 'seed':
                 raise NotImplementedError('Setting a seed is currently '
                                           'not supported')
             else:
                 raise TypeError("Unknown main queue function type " + func)
 
         # generate the finalisations
-        for codeobj in itervalues(self.code_objects):
+        for codeobj in self.code_objects.values():
             if hasattr(codeobj.code, 'main_finalise'):
                 main_lines.append(codeobj.code.main_finalise)
         return main_lines
 
     def fix_random_generators(self, model, code):
         '''
         Translates cpp_standalone style random number generator calls into
@@ -735,64 +739,51 @@
         structures using the static (not code-generated) b2glib library
         functions. This means that the GeNN specific cod only has to be
         concerned about executing the correct model and feeding back results
         into the appropriate cpp_standalone data structures.
         '''
 
         print('building genn executable ...')
-        
+
         if directory is None:  # used during testing
             directory = tempfile.mkdtemp()
 
         # Start building the project
         self.project_dir = directory
         ensure_directory(directory)
         for d in ['code_objects', 'results', 'static_arrays']:
             ensure_directory(os.path.join(directory, d))
 
         writer = CPPWriter(directory)
 
         logger.debug(
             "Writing GeNN project to directory " + os.path.normpath(directory))
 
-        # FIXME: This is only needed to keep Brian2GeNN compatible with Brian2 2.0.1 and earlier
-        if isinstance(self.arange_arrays, dict):
-            arange_arrays = sorted([(var, start)
-                                    for var, start in
-                                    iteritems(self.arange_arrays)],
-                                   key=lambda var_start: var_start[0].name)
-        else:
-            arange_arrays = self.arange_arrays
+        arange_arrays = self.arange_arrays
 
         # write the static arrays
-        for code_object in itervalues(self.code_objects):
-            for var in itervalues(code_object.variables):
+        for code_object in self.code_objects.values():
+            for var in code_object.variables.values():
                 if isinstance(var, Function):
                     self._insert_func_namespace(var, code_object,
                                                 self.static_arrays)
 
         logger.debug("static arrays: " + str(sorted(self.static_arrays.keys())))
         static_array_specs = []
         for name, arr in sorted(self.static_arrays.items()):
             arr.tofile(os.path.join(directory, 'static_arrays', name))
             static_array_specs.append(
                 (name, c_data_type(arr.dtype), arr.size, name))
 
-        try:
-            # Brian versions > 2.2.2.1 do not save the "contained objects" in
-            # net.objects anymore
-            from brian2.core.network import _get_all_objects
-            net_objects = _get_all_objects(self.net.objects)
-        except ImportError:
-            net_objects = self.net.objects
+        net_objects = self.net_objects
 
         main_lines = self.make_main_lines()
 
         # assemble the model descriptions:
-        objects = dict((obj.name, obj) for obj in net_objects)
+        objects = {obj.name: obj for obj in net_objects}
         neuron_groups = [obj for obj in net_objects if
                          isinstance(obj, NeuronGroup)]
         poisson_groups = [obj for obj in net_objects if
                           isinstance(obj, PoissonGroup)]
         spikegenerator_groups = [obj for obj in net_objects if
                                  isinstance(obj, SpikeGeneratorGroup)]
 
@@ -841,17 +832,17 @@
 
         # Turn anonymous namespaces into named namespaces to avoid
         # issues when cpp files are included
         for code_object in itertools.chain(self.code_objects.values(),
                                            self.max_row_length_code_objects.values()):
             cpp_code = getattr(code_object.code, 'cpp_file', code_object.code)
             if 'namespace {' in cpp_code:
-                cpp_code = cpp_code.replace('namespace {', 'namespace {} {{'.format(code_object.name))
+                cpp_code = cpp_code.replace('namespace {', f'namespace {code_object.name} {{')
                 cpp_code = cpp_code.replace('using namespace brian;',
-                                            'using namespace brian;\nusing namespace {};'.format(code_object.name))
+                                            f'using namespace brian;\nusing namespace {code_object.name};')
                 if hasattr(code_object.code, 'cpp_file'):
                     code_object.code.cpp_file = cpp_code
             else:
                 code_object.code = cpp_code
         # Write files from templates
         # Create an empty network.h file, this allows us to use Brian2's
         # objects.cpp template unchanged
@@ -902,17 +893,17 @@
                                         'details.').format(cmd=ex.cmd,
                                                            returncode=ex.returncode)
                                        )
 
     def generate_code_objects(self, writer):
         # Generate data for non-constant values
         code_object_defs = defaultdict(list)
-        for codeobj in itervalues(self.code_objects):
+        for codeobj in self.code_objects.values():
             lines = []
-            for k, v in iteritems(codeobj.variables):
+            for k, v in codeobj.variables.items():
                 if isinstance(v, ArrayVariable):
                     try:
                         if isinstance(v, DynamicArrayVariable):
                             if get_var_ndim(v) == 1:
                                 dyn_array_name = self.dynamic_arrays[v]
                                 array_name = self.arrays[v]
                                 line = '{c_type}* const {array_name} = &{dyn_array_name}[0];'
@@ -921,24 +912,24 @@
                                                    dyn_array_name=dyn_array_name)
                                 lines.append(line)
                                 line = 'const int _num{k} = {dyn_array_name}.size();'
                                 line = line.format(k=k,
                                                    dyn_array_name=dyn_array_name)
                                 lines.append(line)
                         else:
-                            lines.append('const int _num%s = %s;' % (k, v.size))
+                            lines.append(f'const int _num{k} = {v.size};')
                     except TypeError:
                         pass
             for line in lines:
                 # Sometimes an array is referred to by to different keys in our
                 # dictionary -- make sure to never add a line twice
                 if not line in code_object_defs[codeobj.name]:
                     code_object_defs[codeobj.name].append(line)
         # Generate the code objects
-        for codeobj in itervalues(self.code_objects):
+        for codeobj in self.code_objects.values():
             ns = codeobj.variables
             # TODO: fix these freeze/CONSTANTS hacks somehow - they work but not elegant.
             if ((codeobj.template_name not in ['stateupdate', 'threshold',
                                                'reset', 'synapses']) or
                     ('_run_regularly_' in codeobj.name)):
                 if isinstance(codeobj.code, MultiTemplate):
                     code = freeze(codeobj.code.cpp_file, ns)
@@ -953,16 +944,16 @@
                                  codeobj.code.h_file)
                     self.header_files.add(
                         'code_objects/' + codeobj.name + '.h')
 
     def generate_max_row_length_code_objects(self, writer):
         # Generate data for non-constant values
         code_object_defs = defaultdict(set)
-        for codeobj in itervalues(self.max_row_length_code_objects):
-            for k, v in iteritems(codeobj.variables):
+        for codeobj in self.max_row_length_code_objects.values():
+            for k, v in codeobj.variables.items():
                 if isinstance(v, ArrayVariable):
                     try:
                         if isinstance(v, DynamicArrayVariable):
                             if get_var_ndim(v) == 1:
                                 dyn_array_name = self.dynamic_arrays[v]
                                 array_name = self.arrays[v]
                                 # do the const stuff
@@ -977,39 +968,39 @@
                                 code_object_defs[codeobj.name].add(line)
                         else:
                             array_name = self.arrays[v]
                             line = '{c_type} {array_name}[{size}];'
                             line = line.format(c_type=c_data_type(v.dtype),
                                                array_name=array_name,
                                                size=v.size)
-                            code_object_defs[codeobj.name].add('const int _num%s = %s;' % (k, v.size))
+                            code_object_defs[codeobj.name].add(f'const int _num{k} = {v.size};')
                     except TypeError:
                         pass
-    
-        for codeobj in itervalues(self.max_row_length_code_objects):
+
+        for codeobj in self.max_row_length_code_objects.values():
             ns = codeobj.variables
             # TODO: fix these freeze/CONSTANTS hacks somehow - they work but not elegant.
             code = freeze(codeobj.code, ns)
             code = code.replace('%CONSTANTS%', '\n'.join(
                         code_object_defs[codeobj.name]))
             writer.write('code_objects/' + codeobj.name + '.cpp', code)
 
-              
-            
+
+
     def run(self, directory, use_GPU, with_output):
         gpu_arg = "1" if use_GPU else "0"
         if gpu_arg == "1":
             where = 'on GPU'
         else:
             where = 'on CPU'
         print('executing genn binary %s ...' % where)
 
         pref_vars = prefs['devices.cpp_standalone.run_environment_variables']
-        for key, value in itertools.chain(iteritems(pref_vars),
-                                          iteritems(self.run_environment_variables)):
+        for key, value in itertools.chain(pref_vars.items(),
+                                          self.run_environment_variables.items()):
             if key in os.environ and os.environ[key] != value:
                 logger.info('Overwriting environment variable '
                             '"{key}"'.format(key=key),
                             name_suffix='overwritten_env_var', once=True)
             os.environ[key] = value
 
         with std_silent(with_output):
@@ -1018,16 +1009,16 @@
                     self.run_duration)
                 check_call(cmd, cwd=directory)
             else:
                 # print ["./main", "test", str(self.run_duration), gpu_arg]
                 check_call(["./main", "test", str(self.run_duration)],
                            cwd=directory)
         self.has_been_run = True
-        last_run_info = open(
-            os.path.join(directory, 'results/last_run_info.txt'), 'r').read()
+        with open(os.path.join(directory, 'results/last_run_info.txt')) as f:
+            last_run_info = f.read()
         self._last_run_time, self._last_run_completed_fraction = map(float,
                                                                      last_run_info.split())
 
         # The following is a verbatim copy of the respective code in
         # CPPStandaloneDevice.run. In the long run, we can hopefully implement
         # this on the device-independent level, see #761 and discussion in
         # #750.
@@ -1061,33 +1052,33 @@
             logger.debug('Using GeNN path from environment variable: '
                          '"{}"'.format(genn_path))
         else:
             # Find genn-buildmodel
             genn_bin = (find_executable("genn-buildmodel.bat")
                         if os.sys.platform == 'win32'
                         else find_executable("genn-buildmodel.sh"))
-            
+
             if genn_bin is None:
                 raise RuntimeError('Add GeNN\'s bin directory to the path '
                                    'or set the devices.genn.path preference.')
 
             # Remove genn-buildmodel from path, navigate up a directory and normalize
             genn_path = os.path.normpath(os.path.join(os.path.dirname(genn_bin), ".."))
             logger.debug('Using GeNN path determined from path: '
                          '"{}"'.format(genn_path))
-        
+
         # Check for GeNN compatibility
         genn_version = None
         version_file = os.path.join(genn_path, 'version.txt')
         if os.path.exists(version_file):
             try:
-                with open(version_file, 'r') as f:
+                with open(version_file) as f:
                     genn_version = parse_version(f.read().strip())
                     logger.debug('GeNN version: %s' % genn_version)
-            except (OSError, IOError) as ex:
+            except OSError as ex:
                 logger.debug('Getting version from %s/version.txt '
                              'failed: %s' % (genn_path, str(ex)))
 
         if genn_version is None or not genn_version >= parse_version('4.2.1'):
             raise RuntimeError('Brian2GeNN requires GeNN 4.2.1 or later. '
                                'Please upgrade your GeNN version.')
 
@@ -1100,65 +1091,65 @@
                              '"{}"'.format(cuda_path))
             elif 'CUDA_PATH' in env:
                 cuda_path = env['CUDA_PATH']
                 logger.debug('Using CUDA path from environment variable: '
                              '"{}"'.format(cuda_path))
             else:
                 raise RuntimeError('Set the CUDA_PATH environment variable or '
-                                   'the devices.genn.cuda_path preference.')
+                                   'the devices.genn.cuda_backend.cuda_path preference.')
 
         with std_silent(debug):
             if os.sys.platform == 'win32':
                 # Make sure that all environment variables are upper case
-                env = {k.upper() : v for k, v in iteritems(env)}
-                
+                env = {k.upper() : v for k, v in env.items()}
+
                 # If there is vcvars command to call, start cmd with that
                 cmd = ''
                 msvc_env, vcvars_cmd = get_msvc_env()
                 if vcvars_cmd:
                     cmd += vcvars_cmd + ' && '
-                # Otherwise, update environment, again ensuring 
+                # Otherwise, update environment, again ensuring
                 # that all variables are upper case
                 else:
-                    env.update({k.upper() : v for k, v in iteritems(msvc_env)})
+                    env.update({k.upper() : v for k, v in msvc_env.items()})
 
                 # Add start of call to genn-buildmodel
                 buildmodel_cmd = os.path.join(genn_path, 'bin',
                                               'genn-buildmodel.bat')
                 cmd += buildmodel_cmd + ' -s'
-                
+
                 # If we're not using CPU, add CPU option
                 if not use_GPU:
                     cmd += ' -c'
-                    
+
                 # Add include directories
                 # **NOTE** on windows semicolons are used to seperate multiple include paths
                 # **HACK** argument list syntax to check_call doesn't support quoting arguments to batch
                 # files so we have to build argument string manually(https://bugs.python.org/issue23862)
                 wdir = os.getcwd()
-                cmd += ' -i "%s;%s;%s"' % (wdir, os.path.join(wdir, directory),
+                cmd += ' -i "{};{};{}"'.format(wdir, os.path.join(wdir, directory),
                                            os.path.join(wdir, directory, 'brianlib','randomkit'))
                 cmd += ' magicnetwork_model.cpp'
-                
+
                 # Add call to build generated code
                 cmd += ' && msbuild /m /verbosity:minimal /p:Configuration=Release "' + os.path.join(wdir, directory, 'magicnetwork_model_CODE', 'runner.vcxproj') + '"'
-                
+
                 # Add call to build executable
                 cmd += ' && msbuild /m /verbosity:minimal /p:Configuration=Release "' + os.path.join(wdir, directory, 'project.vcxproj') + '"'
-                
+
                 # Run combined command
-                # **NOTE** because vcvars MODIFIED environment, 
+                # **NOTE** because vcvars MODIFIED environment,
                 # making seperate check_calls doesn't work
                 check_call(cmd, cwd=directory, env=env)
             else:
                 if prefs['codegen.cpp.extra_link_args']:
                     # declare the link flags as an environment variable so that GeNN's
                     # generateALL can pick it up
                     env['LDFLAGS'] = ' '.join(prefs['codegen.cpp.extra_link_args'])
-                
+
                 buildmodel_cmd = os.path.join(genn_path, 'bin', 'genn-buildmodel.sh')
                 args = [buildmodel_cmd]
                 if not use_GPU:
                     args += ['-c']
                 wdir= os.getcwd()
                 inc_path= wdir;
                 inc_path+= ':'+os.path.join(wdir, directory)
@@ -1180,42 +1171,41 @@
             model.shared_variabletypes.append(c_data_type(variable.dtype))
         else:
             model.variables.append(varname)
             model.variabletypes.append(c_data_type(variable.dtype))
             model.variablescope[varname] = 'brian'
 
     def add_array_variables(self, model, owner):
-        for varname, variable in iteritems(owner.variables):
+        for varname, variable in owner.variables.items():
             if varname in ['_spikespace', 't', 'dt']:
                 pass
             elif getattr(variable.owner, 'name', None) != owner.name:
                 pass
             elif isinstance(variable, ArrayVariable):
                 self.add_array_variable(model, varname, variable)
 
     def process_poisson_groups(self, objects, poisson_groups):
         for obj in poisson_groups:
             # throw error if events other than spikes are used
-            event_keys = list(iterkeys(obj.events))
-            if (len(event_keys) > 1 
+            event_keys = list(obj.events.keys())
+            if (len(event_keys) > 1
                 or (len(event_keys) == 1 and event_keys[0] != 'spike')):
                 raise NotImplementedError(
                     'Brian2GeNN does not support events that are not spikes')
 
             # Extract the variables
             neuron_model = neuronModel()
             neuron_model.name = obj.name
             neuron_model.clock = obj.clock
             neuron_model.N = obj.N
             self.add_array_variables(neuron_model, obj)
             support_lines = []
-            suffix = '_thresholder';
-            lines = neuron_model.thresh_cond_lines;
-            codeobj = objects[obj.name + suffix].codeobj
-            for k, v in iteritems(codeobj.variables):
+            codeobj = obj.thresholder['spike'].codeobj
+            lines = neuron_model.thresh_cond_lines
+            for k, v in codeobj.variables.items():
                 if k != 'dt' and isinstance(v, Constant):
                     if k not in neuron_model.parameters:
                         self.add_parameter(neuron_model, k, v)
                 code = codeobj.code.cpp_file
 
             code = self.fix_random_generators(neuron_model, code)
             code = decorate(code, neuron_model.variables,
@@ -1227,15 +1217,15 @@
             neuron_model.support_code_lines = support_lines
             self.neuron_models.append(neuron_model)
             self.groupDict[neuron_model.name] = neuron_model
 
     def process_neuron_groups(self, neuron_groups, objects):
         for obj in neuron_groups:
             # throw error if events other than spikes are used
-            event_keys = list(iterkeys(obj.events))
+            event_keys = list(obj.events.keys())
             if len(event_keys) > 1 or (len(event_keys) == 1 and event_keys[0] != 'spike'):
                 raise NotImplementedError(
                     'Brian2GeNN does not support events that are not spikes')
             # Extract the variables
             neuron_model = neuronModel()
             neuron_model.name = obj.name
             neuron_model.clock = obj.clock
@@ -1258,81 +1248,94 @@
             # functions.
             combined_abstract_code = {'stateupdate': [], 'reset': [],
                                       'subexpression_update': [],
                                       'poisson_input': []}
             combined_variables = {}
             combined_variable_indices = defaultdict(lambda: '_idx')
             combined_override_conditional_write = set()
-            thresholder_codeobj = getattr(objects.get(obj.name + '_thresholder', None), 'codeobj', None)
-            if thresholder_codeobj is not None:
-                neuron_model.thresh_cond_lines = '_cond'
-            else:
-                neuron_model.thresh_cond_lines = '0'
+            has_thresholder = False
 
-            for suffix, code_slot in [('_stateupdater', 'stateupdate'),
-                                      ('_thresholder', 'stateupdate'),
-                                      ('_resetter', 'reset'),
-                                      ('_subexpression_update', 'subexpression_update')]:
-                full_name = obj.name + suffix
-                if full_name in objects and objects[full_name].codeobj is not None:
-                    codeobj = objects[full_name].codeobj
-                    combined_abstract_code[code_slot] += [codeobj.abstract_code[None]]
+            stateupdater_name = None
+            slot_mapping = {StateUpdater: 'stateupdate',
+                            Thresholder: 'stateupdate',
+                            Resetter: 'reset',
+                            SubexpressionUpdater: 'subexpression_update'}
+            for klass, code_slot in slot_mapping.items():
+                codeobj = None
+                for contained_obj in obj.contained_objects:
+                    if isinstance(contained_obj, klass):
+                        codeobj = contained_obj.codeobj
+                        if klass is StateUpdater:
+                            stateupdater_name = contained_obj.name
+                        break
+                if codeobj is not None:
+                    combined_abstract_code[code_slot] += [
+                        codeobj.abstract_code[None]]
                     combined_variables.update(codeobj.variables)
                     combined_variable_indices.update(codeobj.variable_indices)
                     # The resetter includes "not_refractory" as an override_conditional_write
                     # variable, meaning that it removes the write-protection based on that
                     # variable that would otherwise apply to "unless refractory" variables,
                     # e.g. the membrane potential. This is not strictly necessary, it will just
                     # introduce an unnecessary check, because a neuron that spiked is by
                     # definition not in its refractory period. However, if we included it as
                     # a override_conditional_write variable for the whole code object here,
                     # this would apply also to the state updater, and therefore
                     # remove the write-protection from "unless refractory" variables in the
                     # state update code.
-                    if suffix != '_resetter':
-                        combined_override_conditional_write.update(codeobj.override_conditional_write)
+                    if klass is not Resetter:
+                        combined_override_conditional_write.update(
+                            codeobj.override_conditional_write)
+                    if klass is Thresholder:
+                        has_thresholder = True
+
+            if has_thresholder:
+                neuron_model.thresh_cond_lines = '_cond'
+            else:
+                neuron_model.thresh_cond_lines = '0'
 
             if obj._refractory is not False:
                 combined_abstract_code['reset'] += ['lastspike = t',
                                                     'not_refractory = False']
 
             # Find PoissonInputs targetting this NeuronGroup
-            poisson_inputs = [o for o in itervalues(objects)
+            poisson_inputs = [o for o in objects.values()
                               if isinstance(o, PoissonInput) and
                                  o.group.name == obj.name]
 
             for poisson_input in poisson_inputs:
                 if poisson_input.when != 'synapses':
                     raise NotImplementedError('Brian2GeNN does not support '
                                               'changing the scheduling slot '
                                               'of PoissonInput objects.')
                 codeobj = poisson_input.codeobj
                 combined_abstract_code['poisson_input'] += [codeobj.abstract_code[None]]
                 combined_variables.update(codeobj.variables)
                 combined_variable_indices.update(codeobj.variable_indices)
 
-            for code_block in iterkeys(combined_abstract_code):
+            for code_block in combined_abstract_code.keys():
                 combined_abstract_code[code_block] = '\n'.join(combined_abstract_code[code_block])
 
-            if any(len(ac) for ac in itervalues(combined_abstract_code)):
-                codeobj = super(GeNNDevice, self).code_object(obj, obj.name + '_stateupdater',
+            if any(len(ac) for ac in combined_abstract_code.values()):
+                assert stateupdater_name, 'No StateUpdater found in object.'
+                codeobj = super().code_object(obj, stateupdater_name,
                                                               combined_abstract_code,
                                                               combined_variables.copy(),
                                                               'neuron_code',
                                                               combined_variable_indices,
                                                               codeobj_class=GeNNCodeObject,
                                                               override_conditional_write=combined_override_conditional_write,
                                                               )
 
                 # Remove the code object from the code_objects dictionary, we
                 # take care of it manually and do not want it to be generated as
                 # part of `generate_code_objects`.
                 del self.code_objects[codeobj.name]
 
-                for k, v in iteritems(codeobj.variables):
+                for k, v in codeobj.variables.items():
                     if k != 'dt' and isinstance(v, Constant):
                         if k not in neuron_model.parameters:
                             self.add_parameter(neuron_model, k, v)
 
                 update_code = codeobj.code.stateupdate_code
                 reset_code = codeobj.code.reset_code
                 for code, lines in [(update_code, neuron_model.code_lines),
@@ -1355,14 +1358,18 @@
             spikegenerator_model.N = obj.N
             self.spikegenerator_models.append(spikegenerator_model)
 
     def process_synapses(self, synapse_groups, objects):
         for obj in synapse_groups:
             synapse_model = synapseModel()
             synapse_model.name = obj.name
+            if isinstance(obj.source, Synapses) or isinstance(obj.target, Synapses):
+                raise NotImplementedError('Brian2GeNN does not support '
+                                          'Synapses objects as source or '
+                                          'target of Synapses objects.')
             if isinstance(obj.source, Subgroup):
                 synapse_model.srcname = obj.source.source.name
                 synapse_model.srcN = obj.source.source.variables['N'].get_value()
             else:
                 synapse_model.srcname = obj.source.name
                 synapse_model.srcN = obj.source.variables['N'].get_value()
             if isinstance(obj.target, Subgroup):
@@ -1451,40 +1458,43 @@
                     addVar = summed_variable_updater.abstract_code.replace('_synaptic_var = ', '').replace('\n', '').replace(' ', '')
                     codeobj = summed_variable_updater.codeobj
                     code_generator = GeNNCodeGenerator(codeobj.variables, codeobj.variable_indices, codeobj.owner, None,
                                                        GeNNCodeObject, codeobj.name, None)
                     addVar = code_generator.translate_expression(addVar)
                     kwds = code_generator.determine_keywords()
                     identifiers = get_identifiers(addVar)
-                    for k, v in iteritems(codeobj.variables):
+                    for k, v in codeobj.variables.items():
                         if k in ['_spikespace', 't', 'dt'] or k not in identifiers:
                             pass
                         else:
                             if '_pre' not in k and '_post' not in k:
                                 if isinstance(v, Constant):
                                     if k not in synapse_model.parameters:
                                         self.add_parameter(synapse_model, k, v)
                                 elif isinstance(v, ArrayVariable):
                                     if k not in synapse_model.variables:
                                         self.add_array_variable(synapse_model, k, v)
                             addVar= addVar.replace(k,'$('+k+')')
-                    code= '\\n\\\n $(addToInSyn,'+addVar+');\\n'                    
+                    code= '\\n\\\n $(addToInSyn,'+addVar+');\\n'
                     synapse_model.main_code_lines['dynamics'] += code
-                    synapse_model.support_code_lines['dynamics'] += stringify('\n'.join(kwds['support_code_lines']))
+                    #quick and dirty test to avoid adding the same support code twice
+                    support_code = stringify('\n'.join(kwds['support_code_lines']))
+                    if support_code not in synapse_model.support_code_lines['dynamics']:
+                        synapse_model.support_code_lines['dynamics'] += support_code
                 else:
                     synapse_model.postSyntoCurrent = '0'
             self.synapse_models.append(synapse_model)
             self.groupDict[synapse_model.name] = synapse_model
 
     def collect_synapses_variables(self, synapse_model, pathway, codeobj):
         identifiers = set()
-        for code in itervalues(codeobj.code):
+        for code in codeobj.code.values():
             identifiers |= get_identifiers(code)
         indices = codeobj.variable_indices
-        for k, v in iteritems(codeobj.variables):
+        for k, v in codeobj.variables.items():
             if k in ['_spikespace', 't', 'dt'] or k not in identifiers:
                 pass
             elif isinstance(v, Constant):
                 if k not in synapse_model.parameters:
                     self.add_parameter(synapse_model, k, v)
             elif isinstance(v, ArrayVariable):
                 if indices[k] == '_idx':
@@ -1492,15 +1502,15 @@
                         self.add_array_variable(synapse_model, k, v)
                 elif indices[k] == '0':
                     if k not in synapse_model.shared_variables:
                         self.add_array_variable(synapse_model, k, v)
                 else:
                     index = indices[k]
                     if (pathway in ['pre', 'post'] and
-                                index == '_{}synaptic_idx'.format(pathway)):
+                                index == f'_{pathway}synaptic_idx'):
                         raise NotImplementedError('brian2genn does not support '
                                                   'references to {pathway}-'
                                                   'synaptic variables in '
                                                   'on_{pathway} '
                                                   'statements.'.format(
                             pathway=pathway))
                     if k not in synapse_model.external_variables:
@@ -1586,39 +1596,106 @@
             if sm.when not in ['start', 'end']:
                 logger.warn("State monitor {!s} has 'when' property '{!s}'"
                             "which is not supported in GeNN, defaulting to"
                             "'end'.".format(sm.name, sm.when))
                 sm.when = 'end'
             if isinstance(src, Synapses):
                 sm.isSynaptic = True
-                sm.srcN = src.source.variables['N'].get_value()
-                sm.trgN = src.target.variables['N'].get_value()
+                neuron_src = src.source
+                # in brian2genn, we need the size of the entire pre-synaptic neuron population, not a sub-group size
+                if isinstance(neuron_src, Subgroup):
+                    neuron_src = neuron_src.source
+                sm.srcN = neuron_src.variables['N'].get_value()
+                neuron_trg = src.target
+                # in brian2genn, we need the size of the entire post-synaptic neuron population, not a sub-group size
+                if isinstance(neuron_trg, Subgroup):
+                    neuron_trg = neuron_trg.source
+                sm.trgN = neuron_trg.variables['N'].get_value()
                 sm.connectivity = self.connectivityDict[src.name]
             else:
                 sm.isSynaptic = False
                 sm.N = src.variables['N'].get_value()
             for varname in obj.record_variables:
-                if src.variables[varname] in itervalues(defaultclock.variables):
+                if src.variables[varname] in defaultclock.variables.values():
                     raise NotImplementedError('Recording the time t or the '
                                               'timestep dt is currently not '
                                               'supported in Brian2GeNN')
                 if isinstance(src.variables[varname], Subexpression):
                     extract_source_variables(src.variables, varname,
                                              sm.variables)
                 elif isinstance(src.variables[varname], Constant):
                     logger.warn(
                         "variable '%s' is a constant - not monitoring" % varname)
                 elif varname not in self.groupDict[sm.monitored].variables:
-                    logger.warn(
-                        "variable '%s' is unused - not monitoring" % varname)
+                    # Check that the variable is also not updated by any run_regularly operation
+                    run_regularly_objects = {o.name: o for o in self.net_objects
+                                             if '_run_regularly' in o.name}
+                    updated = False
+                    for codeobj_name, read_write in self.run_regularly_read_write.items():
+                        if (
+                                varname in read_write['write'] and
+                                run_regularly_objects[codeobj_name].owner.name == sm.monitored
+                        ):
+                            updated = True
+                            break
+
+                    if updated:
+                        sm.variables.append(varname)
+                    else:
+                        raise NotImplementedError("variable '%s' is unused - cannot monitor it" % varname)
                 else:
                     sm.variables.append(varname)
+            if obj.clock.name != 'defaultclock':
+                obj_dt = obj.clock.dt_
+                source_dt = src.dt_[:]
+                if obj_dt < source_dt:
+                    raise NotImplementedError(
+                        'Brian2GeNN does not support StateMonitors '
+                        'with a dt smaller than the dt of the '
+                        'monitored object')
+                dt_mismatch = abs(((obj_dt + source_dt / 2) % source_dt) - source_dt / 2)
+                if dt_mismatch > 1e-4 * source_dt:
+                    raise NotImplementedError(
+                        'Brian2GeNN does not support StateMonitors '
+                        'with a dt that is not a multiple of the dt of the '
+                        'monitored object.')
+                sm.step = int(obj_dt / source_dt + 0.5)
 
             self.state_monitor_models.append(sm)
 
+    def consolidate_pull_operations(self, run_regularly_operations):
+        models_start = defaultdict(list)
+        models_end = defaultdict(list)
+        for sm in self.state_monitor_models:
+            if sm.when == 'start':
+                for varname in sm.variables:
+                    # Do not pull variables that are only updated in run_regularly
+                    if varname in self.groupDict[sm.monitored].variables:
+                        models_start[f'{varname}{sm.monitored}'].append(sm.step)
+            else:
+                for varname in sm.variables:
+                    if varname in self.groupDict[sm.monitored].variables:
+                        models_end[f'{varname}{sm.monitored}'].append(sm.step)
+        for op in run_regularly_operations:
+            for varname in op['read']:
+                if varname not in ['t', 'dt']:
+                    owner_name = op['owner'].variables[varname].owner.name
+                    models_start[f'{varname}{owner_name}'].append(op['step'])
+        # Shortcut: If a state is pulled on every turn, no need to list all steps
+        models_start = {key: [1] if 1 in val else sorted(set(val))
+                        for key, val in models_start.items()}
+        models_end = {key: [1] if 1 in val else sorted(set(val))
+                      for key, val in models_end.items()}
+        # Shortcut: If start or end pulls on every turn, pulling on start is enough.
+        for key, val in models_start.items():
+            if (key in models_end) and (val[0] == 1 or models_end[key][0] == 1):
+                models_end.pop(key)
+                models_start[key] = [1]
+        return models_start, models_end
+
     def generate_model_source(self, writer, main_lines, use_GPU):
         synapses_classes_tmp = CPPStandaloneCodeObject.templater.synapses_classes(None, None)
         writer.write('synapses_classes.*', synapses_classes_tmp)
         default_dtype = prefs.core.default_float_dtype
         if default_dtype == numpy.float32:
             precision = 'GENN_FLOAT'
         elif default_dtype == numpy.float64:
@@ -1627,44 +1704,46 @@
             raise NotImplementedError("GeNN does not support default dtype "
                                       "'{}'".format(default_dtype.__name__))
         dry_main_lines= []
         for line in main_lines:
             if ('_synapses_create_' not in line) and ('monitor' not in line):
                 dry_main_lines.append(line)
         codeobj_inc= []
-        for codeobj in itervalues(self.code_objects):
+        for codeobj in self.code_objects.values():
             if ('group_variable' in codeobj.name):
                 codeobj_inc.append('#include "code_objects/'+codeobj.name+'.cpp"')
         model_tmp = GeNNCodeObject.templater.model(None, None,
                                                    use_GPU=use_GPU,
                                                    code_lines=self.code_lines,
                                                    neuron_models=self.neuron_models,
                                                    spikegenerator_models=self.spikegenerator_models,
                                                    synapse_models=self.synapse_models,
                                                    main_lines=dry_main_lines,
                                                    max_row_length_include= self.max_row_length_include,
                                                    max_row_length_run_calls=self.max_row_length_run_calls,
                                                    max_row_length_synapses=self.max_row_length_synapses,
                                                    codeobj_inc=codeobj_inc,
                                                    dtDef=self.dtDef,
+                                                   profiled=self.kernel_timings,
                                                    prefs=prefs,
-                                                   precision=precision
+                                                   precision=precision,
+                                                   header_files=prefs['codegen.cpp.headers']
                                                    )
         writer.write('magicnetwork_model.cpp', model_tmp)
 
     def generate_main_source(self, writer, main_lines):
         header_files = sorted(self.header_files) + prefs['codegen.cpp.headers']
         runner_tmp = GeNNCodeObject.templater.main(None, None,
                                                    code_lines=self.code_lines,
                                                    neuron_models=self.neuron_models,
                                                    synapse_models=self.synapse_models,
                                                    main_lines=main_lines,
                                                    header_files=header_files,
                                                    source_files=sorted(self.source_files),
-                                                   prefs=prefs,
+                                                   profiled=self.kernel_timings,
                                                    )
         writer.write('main.*', runner_tmp)
 
     def generate_engine_source(self, writer, objects):
         maximum_run_time = self._maximum_run_time
         if maximum_run_time is not None:
             maximum_run_time = float(maximum_run_time)
@@ -1717,47 +1796,52 @@
                                              for run_reg in run_regularly_operations] +
                                             [(sm.order, sm.name, True, sm)
                                              for sm in self.state_monitor_models]
                                             )
         run_reg_state_monitor_operations = [(is_state_mon, obj)
                                             for _, _, is_state_mon, obj
                                             in sorted(run_reg_state_monitor_operations)]
+        vars_to_pull_for_start, vars_to_pull_for_end = self.consolidate_pull_operations(run_regularly_operations)
         engine_tmp = GeNNCodeObject.templater.engine(None, None,
                                                      neuron_models=self.neuron_models,
                                                      spikegenerator_models=self.spikegenerator_models,
                                                      synapse_models=self.synapse_models,
                                                      spike_monitor_models=self.spike_monitor_models,
                                                      rate_monitor_models=self.rate_monitor_models,
                                                      state_monitor_models=self.state_monitor_models,
                                                      run_regularly_operations=run_regularly_operations,
                                                      maximum_run_time=maximum_run_time,
-                                                     run_reg_state_monitor_operations=run_reg_state_monitor_operations
+                                                     run_reg_state_monitor_operations=run_reg_state_monitor_operations,
+                                                     vars_to_pull_for_start=vars_to_pull_for_start,
+                                                     vars_to_pull_for_end=vars_to_pull_for_end,
+                                                     groupDict=self.groupDict
                                                      )
         writer.write('engine.*', engine_tmp)
 
     def generate_makefile(self, directory, use_GPU):
         if os.sys.platform == 'win32':
             project_tmp = GeNNCodeObject.templater.project_vcxproj(None, None,
                                                                    source_files=self.source_files)
-            open(os.path.join(directory, 'project.vcxproj'), 'w').write(
-                project_tmp)
+            with open(os.path.join(directory, 'project.vcxproj'), 'w') as f:
+                f.write(project_tmp)
         else:
             compile_args_gcc = get_gcc_compile_args()
             linker_flags = ' '.join(prefs.codegen.cpp.extra_link_args)
             makefile_tmp = GeNNCodeObject.templater.Makefile(None, None,
                                                              source_files=self.source_files,
                                                              compiler_flags=compile_args_gcc,
                                                              linker_flags=linker_flags)
-            open(os.path.join(directory, 'Makefile'), 'w').write(makefile_tmp)
+            with open(os.path.join(directory, 'Makefile'), 'w') as f:
+                f.write(makefile_tmp)
 
     def generate_objects_source(self, arange_arrays, net, static_array_specs,
                                 synapses, writer):
         # ------------------------------------------------------------------------------
         # create the objects.cpp and objects.h code
-        the_objects = list(itervalues(self.code_objects))
+        the_objects = list(self.code_objects.values())
         arr_tmp = GeNNUserCodeObject.templater.objects(
             None, None,
             array_specs=self.arrays,
             dynamic_array_specs=self.dynamic_arrays,
             dynamic_array_2d_specs=self.dynamic_arrays_2d,
             zero_arrays=self.zero_arrays,
             arange_arrays=arange_arrays,
@@ -1771,65 +1855,102 @@
         )
         writer.write('objects.*', arr_tmp)
         self.header_files.add('objects.h')
         self.source_files.add('objects.cpp')
 
     def copy_source_files(self, writer, directory):
         # Copies brianlib, spikequeue and randomkit
-        super(GeNNDevice, self).copy_source_files(writer, directory)
+        super().copy_source_files(writer, directory)
 
         # Copy the b2glib directory
         b2glib_dir = os.path.join(
             os.path.split(inspect.getsourcefile(GeNNCodeObject))[0],
             'b2glib')
         b2glib_files = copy_directory(b2glib_dir,
                                       os.path.join(directory, 'b2glib'))
         for file in b2glib_files:
             if file.lower().endswith('.cpp'):
                 self.source_files.add('b2glib/' + file)
             elif file.lower().endswith('.h'):
                 self.header_files.add('b2glib/' + file)
 
     def network_run(self, net, duration, report=None, report_period=10 * second,
-                    namespace=None, profile=False, level=0, **kwds):
-        if profile is True:
-            raise NotImplementedError('Brian2GeNN does not yet support '
-                                      'detailed profiling.')
-
+                    namespace=None, profile=None, level=0, **kwds):
+        self.kernel_timings = profile
+        # Allow setting `profile` in the `set_device` call (used e.g. in brian2cuda
+        # SpeedTest configurations)
+        if profile is None:
+            self.kernel_timings = self.build_options.pop("profile", None)
+            # If not set, check the deprecated preference
+            if profile is None and prefs.devices.genn.kernel_timing:
+                logger.warn("The preference 'devices.genn.kernel_timing' is "
+                            "deprecated, please set profile=True instead")
+                self.kernel_timings = True
         if kwds:
             logger.warn(('Unsupported keyword argument(s) provided for run: '
-                         + '%s') % ', '.join(iterkeys(kwds)))
+                         + '%s') % ', '.join(kwds.keys()))
 
         if self.run_duration is not None:
             raise NotImplementedError(
                 'Only a single run statement is supported for the genn device.')
         self.run_duration = float(duration)
         for obj in net.objects:
-            if obj.clock.name != 'defaultclock' and not (obj.__class__ == CodeRunner):
+            if (obj.clock.name != 'defaultclock') and (obj.__class__ not in (CodeRunner, StateMonitor)):
                 raise NotImplementedError(
                     'Multiple clocks are not supported for the genn device')
 
         for obj in net.objects:
             if hasattr(obj, '_linked_variables'):
                 if len(obj._linked_variables) > 0:
                     raise NotImplementedError(
                         'The genn device does not support linked variables')
 
         print('running brian code generation ...')
 
         self.net = net
+        # We need to store all objects, since MagicNetwork.after_run will clear
+        # Network.objects to avoid memory leaks
+        self.net_objects = _get_all_objects(self.net.objects)
+        super().network_run(net=net, duration=duration,
+                            report=report,
+                            report_period=report_period,
+                            namespace=namespace,
+                            level=level + 1,
+                            profile=False)
 
-        super(GeNNDevice, self).network_run(net=net, duration=duration,
-                                            report=report,
-                                            report_period=report_period,
-                                            namespace=namespace,
-                                            level=level + 1)
         self.run_statement_used = True
 
 
+    def network_get_profiling_info(self, net):
+        fname = os.path.join(self.project_dir, 'test_output', 'test.time')
+        if not self.kernel_timings:
+            raise ValueError("No profiling info collected (need to set "
+                             "profile = True ?)")
+        net._profiling_info = []
+        keys = ['neuronUpdateTime',
+                'presynapticUpdateTime',
+                'postsynapticUpdateTime',
+                'synapseDynamicsTime',
+                'initTime',
+                'initSparseTime']
+        with open(fname) as f:
+            # times are appended as new line in each run
+            last_line = f.read().splitlines()[-1]
+        times = last_line.split()
+        n_time = len(times)
+        n_key = len(keys)
+        assert n_time == n_key, (
+            f'{n_time} != {n_key} \ntimes: {times}\nkeys: {keys}'
+        )
+        for key, time in zip(keys, times):
+            net._profiling_info.append((key, float(time)*second))
+        return sorted(net._profiling_info, key=lambda item: item[1],
+                      reverse=True)
+
+
 # ------------------------------------------------------------------------------
 # End of GeNNDevice
 # ------------------------------------------------------------------------------
 
 genn_device = GeNNDevice()
 
 all_devices['genn'] = genn_device
```

### Comparing `Brian2GeNN-1.6/brian2genn/genn_generator.py` & `Brian2GeNN-1.7.0/brian2genn/genn_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 '''
 The code generator for the "genn" language. This is mostly C++ with some specific
 decorators (mainly "__host__ __device__") to allow operation in a CUDA context.
 '''
-
-from six import iteritems
 from brian2.utils.stringtools import (deindent, stripped_deindented_lines,
                                       word_substitute)
 from brian2.utils.logger import get_logger
 from brian2.parsing.rendering import CPPNodeRenderer
 from brian2.core.functions import Function, DEFAULT_FUNCTIONS
 from brian2.core.preferences import prefs
 from brian2.core.variables import ArrayVariable
@@ -100,15 +98,15 @@
 
     class_name = 'genn'
 
     universal_support_code = (_hightype_support_code + _mod_support_code +
                               _floordiv_support_code + _pow_support_code)
 
     def __init__(self, *args, **kwds):
-        super(GeNNCodeGenerator, self).__init__(*args, **kwds)
+        super().__init__(*args, **kwds)
         self.c_data_type = c_data_type
 
     @property
     def restrict(self):
         return prefs['codegen.generators.cpp.restrict_keyword'] + ' '
 
     @property
@@ -122,15 +120,15 @@
         device = get_device()
         if access_data:
             return '_ptr' + device.get_array_name(var)
         else:
             return device.get_array_name(var, access_data=False)
 
     def translate_expression(self, expr):
-        for varname, var in iteritems(self.variables):
+        for varname, var in self.variables.items():
             if isinstance(var, Function):
                 try:
                     impl_name = var.implementations[self.codeobj_class].name
                 except KeyError:
                     raise NotImplementedError('Function {} is not available '
                                               'for use with '
                                               'GeNN.'.format(getattr(var, 'name',
@@ -175,17 +173,17 @@
 
     def translate_to_write_arrays(self, statements):
         return []
 
     def translate_one_statement_sequence(self, statements, scalar=False):
         if len(statements) and self.template_name=='synapses':
             _, _, _, conditional_write_vars = self.arrays_helper(statements)
-            vars_pre = [k for k, v in iteritems(self.variable_indices) if v=='_presynaptic_idx']
-            vars_syn = [k for k, v in iteritems(self.variable_indices) if v=='_idx']
-            vars_post = [k for k, v in iteritems(self.variable_indices) if v=='_postsynaptic_idx']
+            vars_pre = [k for k, v in self.variable_indices.items() if v=='_presynaptic_idx']
+            vars_syn = [k for k, v in self.variable_indices.items() if v=='_idx']
+            vars_post = [k for k, v in self.variable_indices.items() if v=='_postsynaptic_idx']
             if '_pre_codeobject' in self.name:
                 post_write_var, statements = check_pre_code(self, statements,
                                                 vars_pre, vars_syn, vars_post,
                                                 conditional_write_vars)
                 if (post_write_var != None):
                     self.owner._genn_post_write_var = post_write_var
         lines = []
@@ -209,48 +207,48 @@
         support_code = []
         hash_defines = []
         pointers = []
         user_functions = [(varname, variable)]
         funccode = impl.get_code(self.owner)
         if isinstance(funccode, str):
             # Rename references to any dependencies if necessary
-            for dep_name, dep in iteritems(impl.dependencies):
+            for dep_name, dep in impl.dependencies.items():
                 dep_impl = dep.implementations[self.codeobj_class]
                 dep_impl_name = dep_impl.name
                 if dep_impl_name is None:
                     dep_impl_name = dep.pyfunc.__name__
                 if dep_name != dep_impl_name:
                     funccode = word_substitute(funccode,
                                                {dep_name: dep_impl_name})
             funccode = {'support_code': funccode}
         if funccode is not None:
             # To make namespace variables available to functions, we
             # create global variables and assign to them in the main
             # code
             func_namespace = impl.get_namespace(self.owner) or {}
-            for ns_key, ns_value in iteritems(func_namespace):
+            for ns_key, ns_value in func_namespace.items():
                 if hasattr(ns_value, 'dtype'):
                     if ns_value.shape == ():
-                        raise NotImplementedError((
+                        raise NotImplementedError(
                         'Directly replace scalar values in the function '
-                        'instead of providing them via the namespace'))
+                        'instead of providing them via the namespace')
                     type_str = c_data_type(ns_value.dtype) + '*'
                 else:  # e.g. a function
                     type_str = 'py::object'
-                support_code.append('static {0} _namespace{1};'.format(type_str,
+                support_code.append('static {} _namespace{};'.format(type_str,
                                                                        ns_key))
-                pointers.append('_namespace{0} = {1};'.format(ns_key, ns_key))
+                pointers.append(f'_namespace{ns_key} = {ns_key};')
             support_code.append(deindent(funccode.get('support_code', '')))
             hash_defines.append(deindent(funccode.get('hashdefine_code', '')))
 
         dep_hash_defines = []
         dep_pointers = []
         dep_support_code = []
         if impl.dependencies is not None:
-            for dep_name, dep in iteritems(impl.dependencies):
+            for dep_name, dep in impl.dependencies.items():
                 if dep_name not in self.variables:  # do not add a dependency twice
                     self.variables[dep_name] = dep
                     dep_impl = dep.implementations[self.codeobj_class]
                     if dep_name != dep_impl.name:
                         self.func_name_replacements[dep_name] = dep_impl.name
                     hd, ps, sc, uf = self._add_user_function(dep_name, dep)
                     dep_hash_defines.extend(hd)
@@ -271,35 +269,35 @@
         # same array. E.g. in gapjunction code, v_pre and v_post refer to the
         # same array if a group is connected to itself
         handled_pointers = set()
         template_kwds = {}
         # Again, do the import here to avoid a circular dependency.
         from brian2.devices.device import get_device
         device = get_device()
-        for varname, var in iteritems(self.variables):
+        for varname, var in self.variables.items():
             if isinstance(var, ArrayVariable):
                 # This is the "true" array name, not the restricted pointer.
                 array_name = device.get_array_name(var)
                 pointer_name = self.get_array_name(var)
                 if pointer_name in handled_pointers:
                     continue
                 if get_var_ndim(var, 1) > 1:
                     continue  # multidimensional (dynamic) arrays have to be treated differently
-                line = '{0}* {1} {2} = {3};'.format(self.c_data_type(var.dtype),
+                line = '{}* {} {} = {};'.format(self.c_data_type(var.dtype),
                                                     self.restrict,
                                                     pointer_name,
                                                     array_name)
                 pointers.append(line)
                 handled_pointers.add(pointer_name)
 
         # set up the functions
         user_functions = []
         support_code = []
         hash_defines = []
-        for varname, variable in list(iteritems(self.variables)):
+        for varname, variable in list(self.variables.items()):
             if isinstance(variable, Function):
                 hd, ps, sc, uf = self._add_user_function(varname, variable)
                 user_functions.extend(uf)
                 support_code.extend(sc)
                 pointers.extend(ps)
                 hash_defines.extend(hd)
```

### Comparing `Brian2GeNN-1.6/brian2genn/insyn.py` & `Brian2GeNN-1.7.0/brian2genn/insyn.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             if stmt.inplace:
                 if stmt.op!='+=':
                     raise NotImplementedError("GeNN only supports the += in place operation on postsynaptic variables.")
                 accumulation_expr = stmt.expr
                 # "write-protect" a variable during refractoriness to match Brian's semantics
                 if stmt.var in conditional_write_vars:
                     assert conditional_write_vars[stmt.var] == 'not_refractory'
-                    accumulation_expr = 'int(not_refractory_post) * ({})'.format(accumulation_expr)
+                    accumulation_expr = f'int(not_refractory_post) * ({accumulation_expr})'
             else:
                 # TODO: we could support expressions like v = v + expr, but this requires some additional work
                 # namely, for an expression like v = expr we need to check if (expr-v) when simplified reduces to
                 # an expression that only has postsynaptic variables using sympy
                 raise NotImplementedError("GeNN only supports in-place modification of postsynaptic variables")
             new_stmt = Statement('addtoinSyn', '=', '_hidden_weightmatrix*('+accumulation_expr+')',
                                  comment=stmt.comment, dtype=stmt.dtype)
```

### Comparing `Brian2GeNN-1.6/brian2genn/preferences.py` & `Brian2GeNN-1.7.0/brian2genn/preferences.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 '''
 Preferences that relate to the brian2genn interface.
 '''
 import os
 
 from brian2.core.preferences import *
 
-class DeprecatedValidator(object):
+class DeprecatedValidator:
     '''
     'Validator' for deprecated preferences
     
     Used as a validator for preferences that have been (rudely) deprecated
     '''
     def __init__(self, message):
         self.message = message
@@ -90,15 +90,16 @@
     ),
     path=BrianPreference(
         docs='''The path to the GeNN installation (if not set, the version of GeNN in the path will be used instead)''',
         default=None,
         validator=lambda value: value is None or os.path.isdir(value)
     ),
     kernel_timing=BrianPreference(
-        docs='''This preference determines whether GeNN should record kernel runtimes; note that this can affect performance.''',
+        docs='''This preference determines whether GeNN should record kernel runtimes; note that this can affect performance.
+        This preference is deprecated, use profile=True in the set_device or run call instead.''',
         default=False,
     )
 )
 
 prefs.register_preferences(
     'devices.genn.cuda_backend',
     'Preferences that relate to the CUDA backend for the brian2genn interface',
```

### Comparing `Brian2GeNN-1.6/brian2genn/sphinxext/briandoc.py` & `Brian2GeNN-1.7.0/brian2genn/sphinxext/briandoc.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,267 +12,268 @@
 - Convert See Also section to a See also entry.
 - Renumber references.
 - Extract the signature from the docstring, if it can't be determined otherwise.
 
 .. [1] https://github.com/numpy/numpy/blob/master/doc/HOWTO_DOCUMENT.rst.txt
 
 """
-import re
-import pydoc
 import inspect
-from docutils import statemachine
-from docutils.parsers.rst import directives, Directive
-from six import iteritems
+import pydoc
+import re
 
-import sphinx
+from docutils import nodes, statemachine
+from docutils.parsers.rst import Directive, directives
+from docutils.statemachine import ViewList
+from sphinx.domains.c import CDomain
+from sphinx.domains.python import PythonDomain, PyXRefRole
 from sphinx.roles import XRefRole
-from sphinx.domains.python import PyXRefRole
-if sphinx.__version__ < '1.0.1':
-    raise RuntimeError("Sphinx 1.0.1 or newer is required")
 
 import brian2genn
 from brian2.core.preferences import prefs
-import brian2genn
-from .docscrape_sphinx import get_doc_object, SphinxDocString
+
+from .docscrape_sphinx import SphinxDocString, get_doc_object
 
 
 class BrianPrefsDirective(Directive):
-    '''
+    """
     A sphinx 'Directive' for automatically generated documentation of Brian preferences.
-    
+
     The directive takes an optional argument, the basename of the preferences
     to document. In addition, you can specify a `nolinks` option which means
     that no target links for the references are added. Do this if you document
     preferences in more then one place.
-    
+
     Examples
     --------
-    
+
     Document one category of preferences and generate links::
-    
+
         .. document_brian_prefs:: core
-    
+
     Document all preferences without generating links::
-    
+
         .. document_brian_prefs::
            :nolinks:
-    '''
+    """
+
     required_arguments = 0
     optional_arguments = 1
     final_argument_whitespace = True
-    option_spec = {'nolinks': directives.flag}
+    option_spec = {"nolinks": directives.flag, "as_file": directives.flag}
     has_content = False
 
     def run(self):
         # The section that should be documented
         if len(self.arguments):
             section = self.arguments[0]
         else:
             section = None
-        link_targets = not ('nolinks' in self.options)
-        rawtext = prefs.get_documentation(section, link_targets)
-        include_lines = statemachine.string2lines(rawtext,
-                                                  convert_whitespace=True)
-        self.state_machine.insert_input(include_lines, 'Brian preferences')
-        return []
+        if "as_file" in self.options:
+            rawtext = prefs.as_file
+            return [nodes.literal_block(text=rawtext)]
+        else:
+            rawtext = prefs.get_documentation(section, "nolinks" not in self.options)
+            include_lines = statemachine.string2lines(rawtext, convert_whitespace=True)
+            self.state_machine.insert_input(include_lines, "Brian preferences")
+            return []
 
 
-def brianobj_role(role, rawtext, text, lineno, inliner, options={}, content=[]):
-    '''
+def brianobj_role(role, rawtext, text, lineno, inliner, options=None, content=None):
+    """
     A Sphinx role, used as a wrapper for the default `py:obj` role, allowing
     us to use the simple backtick syntax for brian classes/functions without
     having to qualify the package for classes/functions that are available after
     a `from brian2 import *`, e.g `NeuronGroup`.
     Also allows to directly link to preference names using the same syntax.
-    '''
+    """
+    if options is None:
+        options = {}
+    if content is None:
+        content = []
     if text in prefs:
-        linktext = text.replace('_', '-').replace('.', '-')
-        text = '%s <brian-pref-%s>' % (text, linktext)
+        linktext = text.replace("_", "-").replace(".", "-")
+        text = f"{text} <brian-pref-{linktext}>"
         # Use sphinx's cross-reference role
         xref = XRefRole(warn_dangling=True)
-        return xref('std:ref', rawtext, text, lineno, inliner, options, content)
+        return xref("std:ref", rawtext, text, lineno, inliner, options, content)
     else:
-        if text and (not '~' in text):
+        if text and ("~" not in text):
             try:
                 # A simple class or function name
-                if not '.' in text:
-                    module = __import__('brian2genn', fromlist=[str(text)])
+                if "." not in text:
+                    module = __import__("brian2genn", fromlist=[str(text)])
                     imported = getattr(module, str(text), None)
-                    if hasattr(imported, '__module__'):
-                        text = '~' + imported.__module__ + '.' + text
+                    if getattr(imported, "__module__", None):
+                        text = f"~{imported.__module__}.{text}"
                         if inspect.isfunction(imported):
-                            text += '()'
+                            text += "()"
                 # Possibly a method/classmethod/attribute name
-                elif len(text.split('.')) == 2:
-                    classname, attrname = text.split('.')
+                elif len(text.split(".")) == 2:
+                    classname, attrname = text.split(".")
                     # Remove trailing parentheses (will be readded for display)
-                    if attrname.endswith('()'):
+                    if attrname.endswith("()"):
                         attrname = attrname[:-2]
-                    module = __import__('brian2genn', fromlist=[str(classname)])
+                    module = __import__("brian2genn", fromlist=[str(classname)])
                     imported = getattr(module, str(classname), None)
-                    if hasattr(imported, '__module__'):
+                    if hasattr(imported, "__module__"):
                         # Add trailing parentheses only for methods not for
                         # attributes
-                        if inspect.ismethod(getattr(imported,
-                                                    str(attrname),
-                                                    None)):
-                            parentheses = '()'
+                        if inspect.ismethod(getattr(imported, str(attrname), None)):
+                            parentheses = "()"
                         else:
-                            parentheses = ''
+                            parentheses = ""
 
-                        text = ('{classname}.{attrname}{parentheses} '
-                                '<{modname}.{classname}.{attrname}>').format(classname=classname,
-                                                                             attrname=attrname,
-                                                                             modname=imported.__module__,
-                                                                             parentheses=parentheses)
+                        text = (
+                            f"{classname}.{attrname}{parentheses} "
+                            f"<{imported.__module__}.{classname}.{attrname}>"
+                        )
 
             except ImportError:
                 pass
-        role = 'py:obj'
+        role = "py:obj"
         py_role = PyXRefRole()
         return py_role(role, rawtext, text, lineno, inliner, options, content)
 
 
-def mangle_docstrings(app, what, name, obj, options, lines,
-                      reference_offset=[0]):
+def mangle_docstrings(app, what, name, obj, options, lines, reference_offset=None):
+    if reference_offset is None:
+        reference_offset = [0]
     cfg = dict()
-    if what == 'module':
+    if what == "module":
         # Strip top title
-        title_re = re.compile(r'^\s*[#*=]{4,}\n[a-z0-9 -]+\n[#*=]{4,}\s*',
-                              re.I | re.S)
-        lines[:] = title_re.sub('', "\n".join(lines)).split("\n")
-        exported_members = getattr(obj, '__all__', None)
+        title_re = re.compile(r"^\s*[#*=]{4,}\n[a-z0-9 -]+\n[#*=]{4,}\s*", re.I | re.S)
+        lines[:] = title_re.sub("", "\n".join(lines)).split("\n")
+        exported_members = getattr(obj, "__all__", None)
         if exported_members:
-            lines.append('*Exported members:* ')
+            lines.append("*Exported members:* ")
             # do not print more than 25 members
-            lines.append(', '.join(['`%s`' % member for
-                                    member in exported_members[:25]]))
+            lines.append(", ".join([f"`{member}`" for member in exported_members[:25]]))
             if len(exported_members) > 25:
-                lines.append('... (%d more members)' % (len(exported_members) - 25))
+                lines.append(f"... ({int(len(exported_members) - 25)} more members)")
 
-            lines.append('')
+            lines.append("")
     else:
-        doc = get_doc_object(obj, what, "\n".join(lines), name=name,
-                             config=cfg)
+        doc = get_doc_object(obj, what, "\n".join(lines), name=name, config=cfg)
         lines[:] = str(doc).split("\n")
 
     # replace reference numbers so that there are no duplicates
     references = []
     for line in lines:
         line = line.strip()
-        m = re.match(r'^.. \[([a-z0-9_.-])\]', line, re.I)
+        m = re.match(r"^.. \[([a-z0-9_.-])\]", line, re.I)
         if m:
             references.append(m.group(1))
 
     # start renaming from the longest string, to avoid overwriting parts
-    references.sort(key=lambda x:-len(x))
+    references.sort(key=lambda x: -len(x))
     if references:
-        for i, line in enumerate(lines):
+        for i in range(len(lines)):
             for r in references:
-                if re.match(r'^\d+$', r):
-                    new_r = "R%d" % (reference_offset[0] + int(r))
+                if re.match(r"^\d+$", r):
+                    new_r = f"R{int(reference_offset[0] + int(r))}"
                 else:
-                    new_r = "%s%d" % (r, reference_offset[0])
-                lines[i] = lines[i].replace('[%s]_' % r,
-                                            '[%s]_' % new_r)
-                lines[i] = lines[i].replace('.. [%s]' % r,
-                                            '.. [%s]' % new_r)
+                    new_r = f"{r}{int(reference_offset[0])}"
+                lines[i] = lines[i].replace(f"[{r}]_", f"[{new_r}]_")
+                lines[i] = lines[i].replace(f".. [{r}]", f".. [{new_r}]")
 
     reference_offset[0] += len(references)
 
 
 def mangle_signature(app, what, name, obj, options, sig, retann):
     # Do not try to inspect classes that don't define `__init__`
-    if (inspect.isclass(obj) and
-        (not hasattr(obj, '__init__') or
-        'initializes x; see ' in pydoc.getdoc(obj.__init__))):
-        return '', ''
+    if inspect.isclass(obj) and (
+        not hasattr(obj, "__init__")
+        or "initializes x; see " in pydoc.getdoc(obj.__init__)
+    ):
+        return "", ""
 
-    if not (callable(obj) or hasattr(obj, '__argspec_is_invalid_')):
+    if not (callable(obj) or hasattr(obj, "__argspec_is_invalid_")):
         return
-    if not hasattr(obj, '__doc__'):
+    if not hasattr(obj, "__doc__"):
         return
 
     doc = SphinxDocString(pydoc.getdoc(obj))
-    if doc['Signature']:
-        sig = re.sub("^[^(]*", "", doc['Signature'])
-        return sig, ''
+    if doc["Signature"]:
+        sig = re.sub("^[^(]*", "", doc["Signature"])
+        return sig, ""
+
 
 def setup(app, get_doc_object_=get_doc_object):
     global get_doc_object
     get_doc_object = get_doc_object_
 
-    app.connect('autodoc-process-docstring', mangle_docstrings)
-    app.connect('autodoc-process-signature', mangle_signature)
+    app.connect("autodoc-process-docstring", mangle_docstrings)
+    app.connect("autodoc-process-signature", mangle_signature)
 
     # Extra mangling domains
     app.add_domain(NumpyPythonDomain)
     app.add_domain(NumpyCDomain)
 
-    directives.register_directive('document_brian_prefs', BrianPrefsDirective)
+    directives.register_directive("document_brian_prefs", BrianPrefsDirective)
 
     # provide the brianobj role with a link to the Python domain
-    app.add_role('brianobj', brianobj_role)
+    app.add_role("brianobj", brianobj_role)
+
 
-#------------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 # Docstring-mangling domains
-#------------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 
-from docutils.statemachine import ViewList
-from sphinx.domains.c import CDomain
-from sphinx.domains.python import PythonDomain
 
-class ManglingDomainBase(object):
+class ManglingDomainBase:
     directive_mangling_map = {}
 
     def __init__(self, *a, **kw):
-        super(ManglingDomainBase, self).__init__(*a, **kw)
+        super().__init__(*a, **kw)
         self.wrap_mangling_directives()
 
     def wrap_mangling_directives(self):
-        for name, objtype in iteritems(self.directive_mangling_map):
+        for name, objtype in self.directive_mangling_map.items():
             self.directives[name] = wrap_mangling_directive(
-                self.directives[name], objtype)
+                self.directives[name], objtype
+            )
+
 
 class NumpyPythonDomain(ManglingDomainBase, PythonDomain):
-    name = 'np'
+    name = "np"
     directive_mangling_map = {
-        'function': 'function',
-        'class': 'class',
-        'exception': 'class',
-        'method': 'function',
-        'classmethod': 'function',
-        'staticmethod': 'function',
-        'attribute': 'attribute',
+        "function": "function",
+        "class": "class",
+        "exception": "class",
+        "method": "function",
+        "classmethod": "function",
+        "staticmethod": "function",
+        "attribute": "attribute",
     }
 
+
 class NumpyCDomain(ManglingDomainBase, CDomain):
-    name = 'np-c'
+    name = "np-c"
     directive_mangling_map = {
-        'function': 'function',
-        'member': 'attribute',
-        'macro': 'function',
-        'type': 'class',
-        'var': 'object',
+        "function": "function",
+        "member": "attribute",
+        "macro": "function",
+        "type": "class",
+        "var": "object",
     }
 
+
 def wrap_mangling_directive(base_directive, objtype):
     class directive(base_directive):
         def run(self):
             env = self.state.document.settings.env
 
             name = None
             if self.arguments:
-                m = re.match(r'^(.*\s+)?(.*?)(\(.*)?', self.arguments[0])
+                m = re.match(r"^(.*\s+)?(.*?)(\(.*)?", self.arguments[0])
                 name = m.group(2).strip()
 
             if not name:
                 name = self.arguments[0]
 
             lines = list(self.content)
             mangle_docstrings(env.app, objtype, name, None, None, lines)
             self.content = ViewList(lines, self.content.parent)
 
             return base_directive.run(self)
 
     return directive
-
```

### Comparing `Brian2GeNN-1.6/brian2genn/sphinxext/docscrape.py` & `Brian2GeNN-1.7.0/brian2genn/sphinxext/docscrape.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,199 +1,206 @@
 """Extract reference documentation from the NumPy source tree.
 
 """
 
+
 import inspect
-import textwrap
-import re
 import pydoc
-from six import iteritems, iterkeys
+import re
+import textwrap
 from warnings import warn
 
 from sphinx.pycode import ModuleAnalyzer
 
-class Reader(object):
-    """A line-based string reader.
 
-    """
+class Reader:
+    """A line-based string reader."""
+
     def __init__(self, data):
         """
         Parameters
         ----------
         data : str
            String with lines separated by '\n'.
 
         """
         if isinstance(data, list):
             self._str = data
         else:
-            self._str = data.split('\n') # store string as list of lines
+            self._str = data.split("\n")  # store string as list of lines
 
         self.reset()
 
     def __getitem__(self, n):
         return self._str[n]
 
     def reset(self):
-        self._l = 0 # current line nr
+        self._l = 0  # current line nr
 
     def read(self):
         if not self.eof():
             out = self[self._l]
             self._l += 1
             return out
         else:
-            return ''
+            return ""
 
     def seek_next_non_empty_line(self):
-        for l in self[self._l:]:
-            if l.strip():
+        for line in self[self._l :]:
+            if line.strip():
                 break
             else:
                 self._l += 1
 
     def eof(self):
         return self._l >= len(self._str)
 
     def read_to_condition(self, condition_func):
         start = self._l
         for line in self[start:]:
             if condition_func(line):
-                return self[start:self._l]
+                return self[start : self._l]
             self._l += 1
             if self.eof():
-                return self[start:self._l+1]
+                return self[start : self._l + 1]
         return []
 
     def read_to_next_empty_line(self):
         self.seek_next_non_empty_line()
+
         def is_empty(line):
             return not line.strip()
+
         return self.read_to_condition(is_empty)
 
     def read_to_next_unindented_line(self):
         def is_unindented(line):
-            return (line.strip() and (len(line.lstrip()) == len(line)))
+            return line.strip() and (len(line.lstrip()) == len(line))
+
         return self.read_to_condition(is_unindented)
 
     def peek(self, n=0):
         if self._l + n < len(self._str):
             return self[self._l + n]
         else:
-            return ''
+            return ""
 
     def is_empty(self):
-        return not ''.join(self._str).strip()
+        return not "".join(self._str).strip()
 
 
-class NumpyDocString(object):
-    def __init__(self, docstring, config={}):
-        docstring = textwrap.dedent(docstring).split('\n')
+class NumpyDocString:
+    def __init__(self, docstring, config=None):
+        docstring = textwrap.dedent(docstring).split("\n")
 
         self._doc = Reader(docstring)
         self._parsed_data = {
-            'Signature': '',
-            'Summary': [''],
-            'Extended Summary': [],
-            'Parameters': [],
-            'Returns': [],
-            'Raises': [],
-            'Warns': [],
-            'Other Parameters': [],
-            'Attributes': [],
-            'Methods': [],
-            'See Also': [],
-            'Notes': [],
-            'Warnings': [],
-            'References': '',
-            'Examples': '',
-            'index': {}
-            }
+            "Signature": "",
+            "Summary": [""],
+            "Extended Summary": [],
+            "Parameters": [],
+            "Returns": [],
+            "Raises": [],
+            "Warns": [],
+            "Other Parameters": [],
+            "Attributes": [],
+            "Methods": [],
+            "See Also": [],
+            "Notes": [],
+            "Warnings": [],
+            "References": "",
+            "Examples": "",
+            "index": {},
+        }
 
         self._parse()
 
     def __getitem__(self, key):
         return self._parsed_data[key]
 
     def __setitem__(self, key, val):
         if key not in self._parsed_data:
-            warn("Unknown section %s" % key)
+            warn(f"Unknown section {key}")
         else:
             self._parsed_data[key] = val
 
     def _is_at_section(self):
         self._doc.seek_next_non_empty_line()
 
         if self._doc.eof():
             return False
 
         l1 = self._doc.peek().strip()  # e.g. Parameters
 
-        if l1.startswith('.. index::'):
+        if l1.startswith(".. index::"):
             return True
 
-        l2 = self._doc.peek(1).strip() #    ---------- or ==========
-        return l2.startswith('-'*len(l1)) or l2.startswith('='*len(l1))
+        l2 = self._doc.peek(1).strip()  # ---------- or ==========
+        return l2.startswith("-" * len(l1)) or l2.startswith("=" * len(l1))
 
     def _strip(self, doc):
-        i = 0
-        j = 0
+        start = stop = 0
         for i, line in enumerate(doc):
             if line.strip():
+                start = i
                 break
 
-        for j, line in enumerate(doc[::-1]):
+        for i, line in enumerate(doc[::-1]):
             if line.strip():
+                stop = i
                 break
 
-        return doc[i:len(doc)-j]
+        return doc[start:-stop]
 
     def _read_to_next_section(self):
         section = self._doc.read_to_next_empty_line()
 
         while not self._is_at_section() and not self._doc.eof():
-            if not self._doc.peek(-1).strip(): # previous line was empty
-                section += ['']
+            if not self._doc.peek(-1).strip():  # previous line was empty
+                section += [""]
 
             section += self._doc.read_to_next_empty_line()
 
         return section
 
     def _read_sections(self):
         while not self._doc.eof():
             data = self._read_to_next_section()
             name = data[0].strip()
 
-            if name.startswith('..'): # index section
+            if name.startswith(".."):  # index section
                 yield name, data[1:]
             elif len(data) < 2:
                 yield StopIteration
             else:
                 yield name, self._strip(data[2:])
 
     def _parse_param_list(self, content):
         r = Reader(content)
         params = []
         while not r.eof():
             header = r.read().strip()
-            if ' : ' in header:
-                arg_name, arg_type = header.split(' : ')[:2]
+            if " : " in header:
+                arg_name, arg_type = header.split(" : ")[:2]
             else:
-                arg_name, arg_type = header, ''
+                arg_name, arg_type = header, ""
 
             desc = r.read_to_next_unindented_line()
             desc = dedent_lines(desc)
 
             params.append((arg_name, arg_type, desc))
 
         return params
 
+    _name_rgx = re.compile(
+        r"^\s*(:(?P<role>\w+):`(?P<name>[a-zA-Z0-9_.-]+)`|"
+        r" (?P<name2>[a-zA-Z0-9_.-]+))\s*",
+        re.X,
+    )
 
-    _name_rgx = re.compile(r"^\s*(:(?P<role>\w+):`(?P<name>[a-zA-Z0-9_.-]+)`|"
-                           r" (?P<name2>[a-zA-Z0-9_.-]+))\s*", re.X)
     def _parse_see_also(self, content):
         """
         func_name : Descriptive text
             continued text
         another_func_name : Descriptive text
         func_name1, func_name2, :meth:`func_name`, func_name3
 
@@ -205,15 +212,15 @@
             m = self._name_rgx.match(text)
             if m:
                 g = m.groups()
                 if g[1] is None:
                     return g[3], None
                 else:
                     return g[2], g[1]
-            raise ValueError("%s is not a item name" % text)
+            raise ValueError(f"{text} is not a item name")
 
         def push_item(name, rest):
             if not name:
                 return
             name, role = parse_item_name(name)
             items.append((name, list(rest), role))
             del rest[:]
@@ -222,25 +229,25 @@
         rest = []
 
         for line in content:
             if not line.strip():
                 continue
 
             m = self._name_rgx.match(line)
-            if m and line[m.end():].strip().startswith(':'):
+            if m and line[m.end() :].strip().startswith(":"):
                 push_item(current_func, rest)
-                current_func, line = line[:m.end()], line[m.end():]
-                rest = [line.split(':', 1)[1].strip()]
+                current_func, line = line[: m.end()], line[m.end() :]
+                rest = [line.split(":", 1)[1].strip()]
                 if not rest[0]:
                     rest = []
-            elif not line.startswith(' '):
+            elif not line.startswith(" "):
                 push_item(current_func, rest)
                 current_func = None
-                if ',' in line:
-                    for func in line.split(','):
+                if "," in line:
+                    for func in line.split(","):
                         if func.strip():
                             push_item(func, [])
                 elif line.strip():
                     current_func = line
             elif current_func is not None:
                 rest.append(line.strip())
         push_item(current_func, rest)
@@ -248,271 +255,293 @@
 
     def _parse_index(self, section, content):
         """
         .. index: default
            :refguide: something, else, and more
 
         """
+
         def strip_each_in(lst):
             return [s.strip() for s in lst]
 
         out = {}
-        section = section.split('::')
+        section = section.split("::")
         if len(section) > 1:
-            out['default'] = strip_each_in(section[1].split(','))[0]
+            out["default"] = strip_each_in(section[1].split(","))[0]
         for line in content:
-            line = line.split(':')
+            line = line.split(":")
             if len(line) > 2:
-                out[line[1]] = strip_each_in(line[2].split(','))
+                out[line[1]] = strip_each_in(line[2].split(","))
         return out
 
     def _parse_summary(self):
         """Grab signature (if given) and summary"""
         if self._is_at_section():
             return
 
         summary = self._doc.read_to_next_empty_line()
         summary_str = " ".join([s.strip() for s in summary]).strip()
-        if re.compile('^([\w., ]+=)?\s*[\w\.]+\(.*\)$').match(summary_str):
-            self['Signature'] = summary_str
+        if re.compile(r"^([\w., ]+=)?\s*[\w.]+\(.*\)$").match(summary_str):
+            self["Signature"] = summary_str
             if not self._is_at_section():
-                self['Summary'] = self._doc.read_to_next_empty_line()
+                self["Summary"] = self._doc.read_to_next_empty_line()
         else:
-            self['Summary'] = summary
+            self["Summary"] = summary
 
         if not self._is_at_section():
-            self['Extended Summary'] = self._read_to_next_section()
+            self["Extended Summary"] = self._read_to_next_section()
 
     def _parse(self):
         self._doc.reset()
         self._parse_summary()
 
-        for (section, content) in self._read_sections():
-            if not section.startswith('..'):
-                section = ' '.join([s.capitalize() for s in section.split(' ')])
-            if section in ('Parameters', 'Returns', 'Raises', 'Warns',
-                           'Other Parameters', 'Attributes', 'Methods'):
+        for section, content in self._read_sections():
+            if not section.startswith(".."):
+                section = " ".join([s.capitalize() for s in section.split(" ")])
+            if section in (
+                "Parameters",
+                "Returns",
+                "Raises",
+                "Warns",
+                "Other Parameters",
+                "Attributes",
+                "Methods",
+            ):
                 self[section] = self._parse_param_list(content)
-            elif section.startswith('.. index::'):
-                self['index'] = self._parse_index(section, content)
-            elif section == 'See Also':
-                self['See Also'] = self._parse_see_also(content)
+            elif section.startswith(".. index::"):
+                self["index"] = self._parse_index(section, content)
+            elif section == "See Also":
+                self["See Also"] = self._parse_see_also(content)
             else:
                 self[section] = content
 
     # string conversion routines
 
-    def _str_header(self, name, symbol='-'):
-        return [name, len(name)*symbol]
+    def _str_header(self, name, symbol="-"):
+        return [name, len(name) * symbol]
 
     def _str_indent(self, doc, indent=4):
         out = []
         for line in doc:
-            out += [' '*indent + line]
+            out += [" " * indent + line]
         return out
 
     def _str_signature(self):
-        if self['Signature']:
-            return [self['Signature'].replace('*','\*')] + ['']
+        if self["Signature"]:
+            return [self["Signature"].replace("*", r"\*")] + [""]
         else:
-            return ['']
+            return [""]
 
     def _str_summary(self):
-        if self['Summary']:
-            return self['Summary'] + ['']
+        if self["Summary"]:
+            return self["Summary"] + [""]
         else:
             return []
 
     def _str_extended_summary(self):
-        if self['Extended Summary']:
-            return self['Extended Summary'] + ['']
+        if self["Extended Summary"]:
+            return self["Extended Summary"] + [""]
         else:
             return []
 
     def _str_param_list(self, name):
         out = []
         if self[name]:
             out += self._str_header(name)
-            for param,param_type,desc in self[name]:
-                out += ['%s : %s' % (param, param_type)]
+            for param, param_type, desc in self[name]:
+                out += [f"{param} : {param_type}"]
                 out += self._str_indent(desc)
-            out += ['']
+            out += [""]
         return out
 
     def _str_section(self, name):
         out = []
         if self[name]:
             out += self._str_header(name)
             out += self[name]
-            out += ['']
+            out += [""]
         return out
 
     def _str_see_also(self, func_role):
-        if not self['See Also']:
+        if not self["See Also"]:
             return []
         out = []
         out += self._str_header("See Also")
         last_had_desc = True
-        for func, desc, role in self['See Also']:
+        for func, desc, role in self["See Also"]:
             if role:
-                link = ':%s:`%s`' % (role, func)
+                link = f":{role}:`{func}`"
             elif func_role:
-                link = ':%s:`%s`' % (func_role, func)
+                link = f":{func_role}:`{func}`"
             else:
-                link = "`%s`_" % func
+                link = f"`{func}`_"
             if desc or last_had_desc:
-                out += ['']
+                out += [""]
                 out += [link]
             else:
-                out[-1] += ", %s" % link
+                out[-1] += f", {link}"
             if desc:
-                out += self._str_indent([' '.join(desc)])
+                out += self._str_indent([" ".join(desc)])
                 last_had_desc = True
             else:
                 last_had_desc = False
-        out += ['']
+        out += [""]
         return out
 
     def _str_index(self):
-        idx = self['index']
+        idx = self["index"]
         out = []
-        out += ['.. index:: %s' % idx.get('default','')]
-        for section, references in iteritems(idx):
-            if section == 'default':
+        out += [f".. index:: {idx.get('default', '')}"]
+        for section, references in idx.items():
+            if section == "default":
                 continue
-            out += ['   :%s: %s' % (section, ', '.join(references))]
+            out += [f"   :{section}: {', '.join(references)}"]
         return out
 
-    def __str__(self, func_role=''):
+    def __str__(self, func_role=""):
         out = []
         out += self._str_signature()
         out += self._str_summary()
         out += self._str_extended_summary()
-        for param_list in ('Parameters', 'Returns', 'Other Parameters',
-                           'Raises', 'Warns'):
+        for param_list in (
+            "Parameters",
+            "Returns",
+            "Other Parameters",
+            "Raises",
+            "Warns",
+        ):
             out += self._str_param_list(param_list)
-        out += self._str_section('Warnings')
+        out += self._str_section("Warnings")
         out += self._str_see_also(func_role)
-        for s in ('Notes', 'References', 'Examples'):
+        for s in ("Notes", "References", "Examples"):
             out += self._str_section(s)
-        for param_list in ('Attributes', 'Methods'):
+        for param_list in ("Attributes", "Methods"):
             out += self._str_param_list(param_list)
         out += self._str_index()
-        return '\n'.join(out)
+        return "\n".join(out)
 
 
 def indent(str, indent=4):
-    indent_str = ' '*indent
+    indent_str = " " * indent
     if str is None:
         return indent_str
-    lines = str.split('\n')
-    return '\n'.join(indent_str + l for l in lines)
+    lines = str.split("\n")
+    return "\n".join(indent_str + line for line in lines)
+
 
 def dedent_lines(lines):
     """Deindent a list of lines maximally"""
     return textwrap.dedent("\n".join(lines)).split("\n")
 
-def header(text, style='-'):
-    return text + '\n' + style*len(text) + '\n'
+
+def header(text, style="-"):
+    return f"{text}\n{style * len(text)}\n"
 
 
 class FunctionDoc(NumpyDocString):
-    def __init__(self, func, role='func', doc=None, config={}):
+    def __init__(self, func, role="func", doc=None, config=None):
         self._f = func
-        self._role = role # e.g. "func" or "meth"
+        self._role = role  # e.g. "func" or "meth"
 
         if doc is None:
             if func is None:
                 raise ValueError("No function or docstring given")
-            doc = inspect.getdoc(func) or ''
+            doc = inspect.getdoc(func) or ""
         NumpyDocString.__init__(self, doc)
 
-        if not self['Signature'] and func is not None:
+        if not self["Signature"] and func is not None:
             func, func_name = self.get_func()
             try:
                 # try to read signature
-                argspec = inspect.getargspec(func)
-                argspec = inspect.formatargspec(*argspec)
-                argspec = argspec.replace('*','\*')
-                signature = '%s%s' % (func_name, argspec)
-            except TypeError:
-                signature = '%s()' % func_name
-            self['Signature'] = signature
+                argspec = str(inspect.signature(func))
+                argspec = argspec.replace("*", r"\*")
+                signature = f"{func_name}{argspec}"
+            except (TypeError, ValueError):
+                signature = f"{func_name}()"
+            self["Signature"] = signature
 
     def get_func(self):
-        func_name = getattr(self._f, '__name__', self.__class__.__name__)
+        func_name = getattr(self._f, "__name__", self.__class__.__name__)
         if inspect.isclass(self._f):
-            func = getattr(self._f, '__call__', self._f.__init__)
+            if callable(self._f):
+                func = self._f.__call__
+            else:
+                func = self._f.__init__
         else:
             func = self._f
         return func, func_name
 
     def __str__(self):
-        out = ''
+        out = ""
 
         _, func_name = self.get_func()
 
-        roles = {'func': 'function',
-                 'meth': 'method'}
+        roles = {"func": "function", "meth": "method"}
 
         if self._role:
             if self._role not in roles:
-                print("Warning: invalid role %s" % self._role)
-            out += '.. %s:: %s\n    \n\n' % (roles.get(self._role,''),
-                                             func_name)
+                print(f"Warning: invalid role {self._role}")
+            out += f".. {roles.get(self._role, '')}:: {func_name}\n    \n\n"
 
-        out += super(FunctionDoc, self).__str__(func_role=self._role)
+        out += super().__str__(func_role=self._role)
         return out
 
 
 class ClassDoc(NumpyDocString):
+    extra_public_methods = ["__call__"]
 
-    extra_public_methods = ['__call__']
-
-    def __init__(self, cls, doc=None, modulename='', func_doc=FunctionDoc,
-                 config={}):
+    def __init__(self, cls, doc=None, modulename="", func_doc=FunctionDoc, config=None):
         if not inspect.isclass(cls) and cls is not None:
-            raise ValueError("Expected a class or None, but got %r" % cls)
+            raise ValueError(f"Expected a class or None, but got {cls!r}")
         self._cls = cls
 
-        if modulename and not modulename.endswith('.'):
-            modulename += '.'
+        if modulename and not modulename.endswith("."):
+            modulename += "."
         self._mod = modulename
 
         if doc is None:
             if cls is None:
                 raise ValueError("No class or documentation string given")
             doc = pydoc.getdoc(cls)
 
         NumpyDocString.__init__(self, doc)
 
-        if not self['Methods']:
-            self['Methods'] = [(name, '', '')
-                               for name in sorted(self.methods)]
-        if not self['Attributes']:
-            self['Attributes'] = [(name, '', '')
-                                  for name in sorted(self.properties)]
+        if not self["Methods"]:
+            self["Methods"] = [(name, "", "") for name in sorted(self.methods)]
+        if not self["Attributes"]:
+            self["Attributes"] = [(name, "", "") for name in sorted(self.properties)]
 
     @property
     def methods(self):
         if self._cls is None:
-            return [] 
-        methods = [name for name, func in iteritems(getattr(self._cls, '__dict__'))
-                   if ((not name.startswith('_')
-                        or name in self.extra_public_methods)
-                       and ((callable(func) and not isinstance(func, type)) or
-                            inspect.ismethoddescriptor(func)))]
+            return []
+        methods = [
+            name
+            for name, func in self._cls.__dict__.items()
+            if (
+                (not name.startswith("_") or name in self.extra_public_methods)
+                and (
+                    (callable(func) and not isinstance(func, type))
+                    or inspect.ismethoddescriptor(func)
+                )
+            )
+        ]
         return methods
 
     @property
     def properties(self):
         if self._cls is None:
             return []
         analyzer = ModuleAnalyzer.for_module(self._cls.__module__)
-        instance_members = set([attr_name for (class_name, attr_name) in
-                                iterkeys(analyzer.find_attr_docs())
-                                if class_name == self._cls.__name__])
-        class_members = set([name for name, func in iteritems(getattr(self._cls, '__dict__'))
-                             if not name.startswith('_') and (func is None or
-                                                              inspect.isdatadescriptor(func))])
+        instance_members = {
+            attr_name
+            for (class_name, attr_name) in analyzer.find_attr_docs().keys()
+            if class_name == self._cls.__name__
+        }
+        class_members = {
+            name
+            for name, func in self._cls.__dict__.items()
+            if not name.startswith("_")
+            and (func is None or inspect.isdatadescriptor(func))
+        }
 
         return instance_members | class_members
```

### Comparing `Brian2GeNN-1.6/brian2genn/sphinxext/docscrape_sphinx.py` & `Brian2GeNN-1.7.0/brian2genn/sphinxext/docscrape_sphinx.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,259 +1,278 @@
-import re, inspect, textwrap, pydoc
-import sphinx
+import inspect
+import pydoc
+import re
+import textwrap
+
 from sphinx.pycode import ModuleAnalyzer
-from six import iteritems
-from .docscrape import NumpyDocString, FunctionDoc, ClassDoc
+
+from .docscrape import ClassDoc, FunctionDoc, NumpyDocString
+
 
 class SphinxDocString(NumpyDocString):
-    def __init__(self, docstring, config={}):
+    def __init__(self, docstring, config=None):
+        if config is None:
+            config = {}
         NumpyDocString.__init__(self, docstring, config=config)
 
     # string conversion routines
     @staticmethod
-    def _str_header(name, symbol='`'):
-        return ['.. rubric:: ' + name, '']
+    def _str_header(name, symbol="`"):
+        return [f".. rubric:: {name}", ""]
 
     @staticmethod
     def _str_field_list(name):
-        return [':' + name + ':']
+        return [f":{name}:"]
 
     @staticmethod
     def _str_indent(doc, indent=4):
         out = []
         for line in doc:
-            out += [' '*indent + line]
+            out += [" " * indent + line]
         return out
 
     def _str_summary(self):
-        return self['Summary'] + ['']
+        return self["Summary"] + [""]
 
     def _str_extended_summary(self):
-        return self['Extended Summary'] + ['']
+        return self["Extended Summary"] + [""]
 
     def _str_param_list(self, name):
         out = []
         if self[name]:
             out += self._str_field_list(name)
-            out += ['']
+            out += [""]
             for param, param_type, desc in self[name]:
-                out += self._str_indent(['**%s** : %s' % (param.strip(),
-                                                          param_type)])
-                out += ['']
+                out += self._str_indent([f"**{param.strip()}** : {param_type}"])
+                out += [""]
                 out += self._str_indent(desc, 8)
-                out += ['']
+                out += [""]
 
         return out
 
     @property
     def _obj(self):
-        if hasattr(self, '_cls'):
+        if hasattr(self, "_cls"):
             return self._cls
-        elif hasattr(self, '_f'):
+        elif hasattr(self, "_f"):
             return self._f
         return None
 
     def _str_member_list(self):
         """
         Generate a member listing, autosummary:: table .
 
         """
         out = []
 
-        
-        
-        for name in ['Attributes', 'Methods']:
+        for name in ["Attributes", "Methods"]:
             if not self[name]:
                 continue
-            
-            out += ['.. rubric:: %s' % name, '']
-            prefix = getattr(self, '_name', '')
+
+            out += [f".. rubric:: {name}", ""]
+            prefix = getattr(self, "_name", "")
 
             if prefix:
-                prefix = '%s.' % prefix
+                prefix = f"{prefix}."
 
             autosum = []
             for param, _, desc in self[name]:
                 param = param.strip()
                 if self._obj:
                     # Fake the attribute as a class property, but do not touch
                     # methods
-                    if (hasattr(self._obj, '__module__') and not 
-                        (hasattr(self._obj, param) and callable(getattr(self._obj, param)))):
-
+                    if hasattr(self._obj, "__module__") and not (
+                        hasattr(self._obj, param)
+                        and callable(getattr(self._obj, param))
+                    ):
                         # Do not override directly provided docstrings
-                        if not len(''.join(desc).strip()):
+                        if not len("".join(desc).strip()):
                             analyzer = ModuleAnalyzer.for_module(self._obj.__module__)
-                            desc = analyzer.find_attr_docs().get((self._obj.__name__, param), '')
-                            
+                            desc = analyzer.find_attr_docs().get(
+                                (self._obj.__name__, param), ""
+                            )
+
                         # Only fake a property if we got a docstring
-                        if len(''.join(desc).strip()):
-                            setattr(self._obj, param, property(lambda self: None,
-                                                               doc='\n'.join(desc)))
+                        if len("".join(desc).strip()):
+                            setattr(
+                                self._obj,
+                                param,
+                                property(lambda self: None, doc="\n".join(desc)),
+                            )
 
                 if len(prefix):
-                    autosum += ["   ~%s%s" % (prefix, param)]
+                    autosum += [f"   ~{prefix}{param}"]
                 else:
-                    autosum += ["   %s" % param]
+                    autosum += [f"   {param}"]
 
             if autosum:
-                out += ['.. autosummary::', '']
+                out += [".. autosummary::", ""]
                 out += autosum
-            
-            out += ['']
+
+            out += [""]
         return out
 
     def _str_member_docs(self, name):
         """
         Generate the full member autodocs
 
         """
         out = []
 
         if self[name]:
-            prefix = getattr(self, '_name', '')
+            prefix = getattr(self, "_name", "")
 
             if prefix:
-                prefix += '.'
+                prefix += "."
 
             for param, _, _ in self[name]:
-                if name == 'Methods':
-                    out += ['.. automethod:: %s%s' % (prefix, param)]
-                elif name == 'Attributes':
-                    out += ['.. autoattribute:: %s%s' % (prefix, param)]
-            
-            out += ['']
+                if name == "Methods":
+                    out += [f".. automethod:: {prefix}{param}"]
+                elif name == "Attributes":
+                    out += [f".. autoattribute:: {prefix}{param}"]
+
+            out += [""]
         return out
 
     def _str_section(self, name):
         out = []
         if self[name]:
             out += self._str_header(name)
-            out += ['']
+            out += [""]
             content = textwrap.dedent("\n".join(self[name])).split("\n")
             out += content
-            out += ['']
+            out += [""]
         return out
 
     def _str_see_also(self, func_role):
         out = []
-        if self['See Also']:
-            see_also = super(SphinxDocString, self)._str_see_also(func_role)
-            out = ['.. seealso::', '']
+        if self["See Also"]:
+            see_also = super()._str_see_also(func_role)
+            out = [".. seealso::", ""]
             out += self._str_indent(see_also[2:])
         return out
 
     def _str_raises(self, name, func_role):
         if not self[name]:
             return []
         out = []
         out += self._str_header(name)
         for func, _, desc in self[name]:
-            out += [":exc:`%s`" % func]
+            out += [f":exc:`{func}`"]
             if desc:
-                out += self._str_indent([' '.join(desc)])
-        out += ['']
-        return out        
+                out += self._str_indent([" ".join(desc)])
+        out += [""]
+        return out
 
     def _str_warnings(self):
         out = []
-        if self['Warnings']:
-            out = ['.. warning::', '']
-            out += self._str_indent(self['Warnings'])
+        if self["Warnings"]:
+            out = [".. warning::", ""]
+            out += self._str_indent(self["Warnings"])
         return out
 
     def _str_index(self):
-        idx = self['index']
+        idx = self["index"]
         out = []
         if len(idx) == 0:
             return out
 
-        out += ['.. index:: %s' % idx.get('default','')]
-        for section, references in iteritems(idx):
-            if section == 'default':
+        out += [f".. index:: {idx.get('default', '')}"]
+        for section, references in idx.items():
+            if section == "default":
                 continue
-            elif section == 'refguide':
-                out += ['   single: %s' % (', '.join(references))]
+            elif section == "refguide":
+                out += [f"   single: {', '.join(references)}"]
             else:
-                out += ['   %s: %s' % (section, ','.join(references))]
+                out += [f"   {section}: {','.join(references)}"]
         return out
 
     def _str_references(self):
         out = []
-        if self['References']:
-            out += self._str_header('References')
-            if isinstance(self['References'], str):
-                self['References'] = [self['References']]
-            out.extend(self['References'])
-            out += ['']
+        if self["References"]:
+            out += self._str_header("References")
+            if isinstance(self["References"], str):
+                self["References"] = [self["References"]]
+            out.extend(self["References"])
+            out += [""]
             # Latex collects all references to a separate bibliography,
             # so we need to insert links to it
-            if sphinx.__version__ >= "0.6":
-                out += ['.. only:: latex','']
-            else:
-                out += ['.. latexonly::','']
+            out += [".. only:: latex", ""]
             items = []
-            for line in self['References']:
-                m = re.match(r'.. \[([a-z0-9._-]+)\]', line, re.I)
+            for line in self["References"]:
+                m = re.match(r".. \[([a-z0-9._-]+)\]", line, re.I)
                 if m:
                     items.append(m.group(1))
-            out += ['   ' + ", ".join(["[%s]_" % item for item in items]), '']
+            out += [f"   {', '.join([f'[{item}]_' for item in items])}", ""]
         return out
 
     def _str_examples(self):
-        return self._str_section('Examples')
+        return self._str_section("Examples")
 
     def __str__(self, indent=0, func_role="brianobj"):
         out = []
-        out += self._str_index() + ['']
+        out += self._str_index() + [""]
         out += self._str_summary()
         out += self._str_extended_summary()
-        for param_list in ('Parameters', 'Returns', 'Other Parameters'):
+        for param_list in ("Parameters", "Returns", "Other Parameters"):
             out += self._str_param_list(param_list)
-        for param_list in ('Raises', 'Warns'):
+        for param_list in ("Raises", "Warns"):
             out += self._str_raises(param_list, func_role)
         out += self._str_warnings()
         out += self._str_see_also(func_role)
-        out += self._str_section('Notes')
+        out += self._str_section("Notes")
         out += self._str_references()
         out += self._str_examples()
         out += self._str_member_list()
-        if self['Attributes'] + self['Methods']:
-            out += ['.. rubric:: Details', '']
-            for param_list in ('Attributes', 'Methods'):
+        if self["Attributes"] + self["Methods"]:
+            out += [".. rubric:: Details", ""]
+            for param_list in ("Attributes", "Methods"):
                 out += self._str_member_docs(param_list)
         out = self._str_indent(out, indent)
-        return '\n'.join(out)
+        return "\n".join(out)
+
 
 class SphinxFunctionDoc(SphinxDocString, FunctionDoc):
-    def __init__(self, obj, doc=None, config={}):
+    def __init__(self, obj, doc=None, config=None):
+        if config is None:
+            config = {}
         FunctionDoc.__init__(self, obj, doc=doc, config=config)
 
+
 class SphinxClassDoc(SphinxDocString, ClassDoc):
-    def __init__(self, obj, doc=None, func_doc=None, name=None, config={}):
+    def __init__(self, obj, doc=None, func_doc=None, name=None, config=None):
+        if config is None:
+            config = {}
         self.name = name
         ClassDoc.__init__(self, obj, doc=doc, func_doc=None, config=config)
 
+
 class SphinxObjDoc(SphinxDocString):
-    def __init__(self, obj, doc=None, config={}):
+    def __init__(self, obj, doc=None, config=None):
+        if config is None:
+            config = {}
         self._f = obj
         SphinxDocString.__init__(self, doc, config=config)
 
-def get_doc_object(obj, what=None, doc=None, name=None, config={}):
+
+def get_doc_object(obj, what=None, doc=None, name=None, config=None):
+    if config is None:
+        config = {}
     if what is None:
         if inspect.isclass(obj):
-            what = 'class'
+            what = "class"
         elif inspect.ismodule(obj):
-            what = 'module'
+            what = "module"
         elif callable(obj):
-            what = 'function'
+            what = "function"
         else:
-            what = 'object'
-    if what == 'class':
-        return SphinxClassDoc(obj, func_doc=SphinxFunctionDoc, doc=doc,
-                              name=name, config=config)
-    elif what in ('function', 'method'):
+            what = "object"
+    if what == "class":
+        return SphinxClassDoc(
+            obj, func_doc=SphinxFunctionDoc, doc=doc, name=name, config=config
+        )
+    elif what in ("function", "method"):
         return SphinxFunctionDoc(obj, doc=doc, config=config)
     else:
         if doc is None:
             doc = pydoc.getdoc(obj)
         return SphinxObjDoc(obj, doc, config=config)
```

### Comparing `Brian2GeNN-1.6/brian2genn/sphinxext/generate_reference.py` & `Brian2GeNN-1.7.0/brian2genn/sphinxext/generate_reference.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,191 +1,188 @@
-# -*- coding: utf-8 -*-
 """
     Automatically generate Brian's reference documentation.
-    
+
     Based on sphinx-apidoc, published under a BSD license: http://sphinx-doc.org/
 """
+
+
 import inspect
-import sys
 import os
+import sys
 from os import path
 
-from .examplefinder import auto_find_examples
-
-INITPY = '__init__.py'
+INITPY = "__init__.py"
 
-OPTIONS = ['show-inheritance']
+OPTIONS = ["show-inheritance"]
 
 
 def makename(package, module):
     """Join package and module with a dot."""
     # Both package and module can be None/empty.
     if package:
         name = package
         if module:
-            name += '.' + module
+            name += f".{module}"
     else:
         name = module
     return name
 
 
 def write_file(name, text, destdir, suffix):
     """Write the output file for module/package <name>."""
-    fname = path.join(destdir, '%s.%s' % (name, suffix))
-    print('Creating file %s.' % fname)
-    f = open(fname, 'w')
+    fname = path.join(destdir, f"{name}.{suffix}")
+    print(f"Creating file {fname}.")
+    f = open(fname, "w")
     try:
         f.write(text)
     finally:
         f.close()
 
 
 def format_heading(level, text):
     """Create a heading of <level> [1, 2 or 3 supported]."""
-    underlining = ['=', '-', '~', ][level-1] * len(text)
-    return '%s\n%s\n\n' % (text, underlining)
+    underlining = ["=", "-", "~"][level - 1] * len(text)
+    return f"{text}\n{underlining}\n\n"
 
 
-def format_directive(module, destdir, package=None, basename='brian2genn'):
+def format_directive(module, destdir, package=None, basename="brian2genn"):
     """Create the automodule directive and add the options."""
-    directive = '.. automodule:: %s\n' % makename(package, module)
+    directive = f".. automodule:: {makename(package, module)}\n"
     for option in OPTIONS:
-        directive += '    :%s:\n' % option
-    directive += '\n'
+        directive += f"    :{option}:\n"
+    directive += "\n"
     # document all the classes in the modules
-    full_name = basename + '.' + module
-    print('processing ' + full_name)
-    try:
-        __import__(full_name)
-    except:
-        return directive
+    full_name = f"{basename}.{module}"
+    __import__(full_name)
     mod = sys.modules[full_name]
     dir_members = dir(mod)
     classes = []
     functions = []
     variables = []
     for member in dir_members:
         _temp = __import__(full_name, {}, {}, [member], 0)
         member_obj = getattr(_temp, member)
-        member_module = getattr(member_obj, '__module__', None)
+        member_module = getattr(member_obj, "__module__", None)
         # only document members that where defined in this module
-        if member_module == full_name and not member.startswith('_'):
+        if member_module == full_name and not member.startswith("_"):
             if inspect.isclass(member_obj):
                 classes.append((member, member_obj))
             elif inspect.isfunction(member_obj):
                 functions.append((member, member_obj))
             else:
                 variables.append((member, member_obj))
-                    
+
     if classes:
-        directive += '**Classes**\n\n'
+        directive += "**Classes**\n\n"
         for member, member_obj in classes:
-            directive += '.. autosummary:: %s\n' % (member)
-            directive += '    :toctree:\n\n'
+            directive += f".. autosummary:: {member}\n"
+            directive += "    :toctree:\n\n"
             create_member_file(full_name, member, member_obj, destdir)
     if functions:
-        directive += '**Functions**\n\n'
+        directive += "**Functions**\n\n"
         for member, member_obj in functions:
-            directive += '.. autosummary:: %s\n' % (member)
-            directive += '    :toctree:\n\n'
+            directive += f".. autosummary:: {member}\n"
+            directive += "    :toctree:\n\n"
             create_member_file(full_name, member, member_obj, destdir)
     if variables:
-        directive += '**Objects**\n\n'
+        directive += "**Objects**\n\n"
         for member, member_obj in variables:
-            directive += '.. autosummary:: %s\n' % (member)
-            directive += '    :toctree:\n\n'
+            directive += f".. autosummary:: {member}\n"
+            directive += "    :toctree:\n\n"
             create_member_file(full_name, member, member_obj, destdir)
-                
+
     return directive
 
 
 def find_shortest_import(module_name, obj_name):
-    parts = module_name.split('.')
+    parts = module_name.split(".")
     for idx in range(1, len(parts) + 1):
         try:
-            result = __import__('.'.join(parts[:idx]), globals(), {},
-                                fromlist=[str(obj_name)], level=0)
+            result = __import__(
+                ".".join(parts[:idx]), globals(), {}, fromlist=[str(obj_name)], level=0
+            )
             result_obj = getattr(result, obj_name, None)
-            if result_obj is not None and getattr(result_obj,
-                                                  '__module__',
-                                                  None) == module_name:
+            if (
+                result_obj is not None
+                and getattr(result_obj, "__module__", None) == module_name
+            ):
                 # import seems to have worked
-                return '.'.join(parts[:idx])
+                return ".".join(parts[:idx])
         except ImportError:
             pass
-    raise AssertionError("Couldn't import " + module_name + '.' + obj_name)
+    raise AssertionError(f"Couldn't import {module_name}.{obj_name}")
 
 
-def create_member_file(module_name, member, member_obj, destdir, suffix='rst'):
+def create_member_file(module_name, member, member_obj, destdir, suffix="rst"):
     """Build the text of the file and write the file."""
-    
-    text = '.. currentmodule:: ' + module_name + '\n\n'
+
+    text = f".. currentmodule:: {module_name}\n\n"
 
     shortest_import = find_shortest_import(module_name, member)
-    import_text = '(*Shortest import*: ``from {} import {})``\n\n'.format(shortest_import,
-                                                                          member)
+    import_text = f"(*Shortest import*: ``from {shortest_import} import {member})``\n\n"
     if inspect.isclass(member_obj):
-        text += format_heading(1, '%s class' % member)
+        text += format_heading(1, f"{member} class")
         text += import_text
-        text += '.. autoclass:: %s\n\n' % member
-        text += auto_find_examples(member_obj, headersymbol='-')
+        text += f".. autoclass:: {member}\n\n"
     elif inspect.isfunction(member_obj):
-        text += format_heading(1, '%s function' % member)
+        text += format_heading(1, f"{member} function")
         text += import_text
-        text += '.. autofunction:: %s\n\n' % member
+        text += f".. autofunction:: {member}\n\n"
     else:
-        text += format_heading(1, '%s object' % member)
+        text += format_heading(1, f"{member} object")
         text += import_text
-        text += '.. autodata:: %s\n' % member
+        text += f".. autodata:: {member}\n"
 
     write_file(makename(module_name, member), text, destdir, suffix)
 
 
-def create_package_file(root, master_package, subroot, py_files, subs,
-                        destdir, excludes, suffix='rst'):
+def create_package_file(
+    root, master_package, subroot, py_files, subs, destdir, excludes, suffix="rst"
+):
     """Build the text of the file and write the file."""
     package = path.split(root)[-1]
-    text = format_heading(1, '%s package' % package)
+    text = format_heading(1, f"{package} package")
     # add each module in the package
     for py_file in py_files:
         if shall_skip(path.join(root, py_file)):
             continue
         is_package = py_file == INITPY
         py_file = path.splitext(py_file)[0]
         py_path = makename(subroot, py_file)
         # we don't want an additional header for the package,
         if not is_package:
-            heading = ':mod:`%s` module' % py_file
+            heading = f":mod:`{py_file}` module"
             text += format_heading(2, heading)
-        text += format_directive(is_package and subroot or py_path, destdir,
-                                 master_package)
-        text += '\n'
+        text += format_directive(
+            is_package and subroot or py_path, destdir, master_package
+        )
+        text += "\n"
 
     # build a list of directories that are packages (contain an INITPY file)
     subs = [sub for sub in subs if path.isfile(path.join(root, sub, INITPY))]
     # if there are some package directories, add a TOC for theses subpackages
     if subs:
-        text += format_heading(2, 'Subpackages')
-        text += '.. toctree::\n'
-        text += '    :maxdepth: 2\n\n'
+        text += format_heading(2, "Subpackages")
+        text += ".. toctree::\n"
+        text += "    :maxdepth: 2\n\n"
         for sub in subs:
             if not is_excluded(os.path.join(root, sub), excludes):
-                text += '    %s.%s\n' % (makename(master_package, subroot), sub)
-        text += '\n'
+                text += f"    {makename(master_package, subroot)}.{sub}\n"
+        text += "\n"
 
     write_file(makename(master_package, subroot), text, destdir, suffix)
 
 
 def shall_skip(module):
     """Check if we want to skip this module."""
     # skip it if there is nothing (or just \n or \r\n) in the file
     return path.getsize(module) <= 2
 
 
-def recurse_tree(rootpath, excludes, destdir):
+def recurse_tree(rootpath, exclude_dirs, exclude_files, destdir):
     """
     Look for every file in the directory tree and create the corresponding
     ReST files.
     """
     # use absolute path for root, as relative paths like '../../foo' cause
     # 'if "/." in root ...' to filter out *all* modules otherwise
     rootpath = path.normpath(path.abspath(rootpath))
@@ -194,41 +191,54 @@
         root_package = rootpath.split(path.sep)[-1]
     else:
         # otherwise, the base is a directory with packages
         root_package = None
 
     toplevels = []
     for root, subs, files in os.walk(rootpath):
-        if is_excluded(root, excludes):
+        if is_excluded(root, exclude_dirs):
             del subs[:]
             continue
         # document only Python module files
-        py_files = sorted([f for f in files if path.splitext(f)[1] == '.py'])
+        py_files = sorted(
+            [
+                f
+                for f in files
+                if (path.splitext(f)[1] == ".py" and f not in exclude_files)
+            ]
+        )
         is_pkg = INITPY in py_files
         if is_pkg:
             py_files.remove(INITPY)
             py_files.insert(0, INITPY)
         elif root != rootpath:
             # only accept non-package at toplevel
             del subs[:]
             continue
         # remove hidden ('.') and private ('_') directories
-        subs[:] = sorted(sub for sub in subs if sub[0] not in ['.', '_'])
+        subs[:] = sorted(sub for sub in subs if sub[0] not in [".", "_"])
 
         if is_pkg:
             # we are in a package with something to document
-            if subs or len(py_files) > 1 or not \
-                shall_skip(path.join(root, INITPY)):
-                subpackage = root[len(rootpath):].lstrip(path.sep).\
-                    replace(path.sep, '.')
-                create_package_file(root, root_package, subpackage,
-                                    py_files, subs, destdir, excludes)
+            if subs or len(py_files) > 1 or not shall_skip(path.join(root, INITPY)):
+                subpackage = (
+                    root[len(rootpath) :].lstrip(path.sep).replace(path.sep, ".")
+                )
+                create_package_file(
+                    root,
+                    root_package,
+                    subpackage,
+                    py_files,
+                    subs,
+                    destdir,
+                    exclude_dirs,
+                )
                 toplevels.append(makename(root_package, subpackage))
         else:
-            raise AssertionError('Expected it to be a package')
+            raise AssertionError("Expected it to be a package")
 
     return toplevels
 
 
 def normalize_excludes(rootpath, excludes):
     """
     Normalize the excluded directory list:
@@ -256,14 +266,13 @@
         root += sep
     for exclude in excludes:
         if root.startswith(exclude):
             return True
     return False
 
 
-def main(rootpath, excludes, destdir):
+def main(rootpath, exclude_dirs, exclude_files, destdir):
     if not os.path.exists(destdir):
         os.makedirs(destdir)
 
-    excludes = normalize_excludes(rootpath, excludes)
-    modules = recurse_tree(rootpath, excludes, destdir)
-
+    exclude_dirs = normalize_excludes(rootpath, exclude_dirs)
+    recurse_tree(rootpath, exclude_dirs, exclude_files, destdir)
```

### Comparing `Brian2GeNN-1.6/brian2genn/templates/Makefile` & `Brian2GeNN-1.7.0/brian2genn/templates/Makefile`

 * *Files identical despite different names*

### Comparing `Brian2GeNN-1.6/brian2genn/templates/engine.cpp` & `Brian2GeNN-1.7.0/brian2genn/templates/engine.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -21,22 +21,22 @@
 
 double Network::_last_run_time = 0.0;
 double Network::_last_run_completed_fraction = 0.0;
 
 class engine
 {
  public:
-  // end of data fields 
+  // end of data fields
 
   engine();
   ~engine();
-  void free_device_mem(); 
+  void free_device_mem();
   void run(double);
-  void getStateFromGPU(); 
-  void getSpikesFromGPU(); 
+  void getStateFromGPU();
+  void getSpikesFromGPU();
 };
 
 #endif
 {% endmacro %}
 
 
 {% macro cpp_file() %}
@@ -71,251 +71,293 @@
 //--------------------------------------------------------------------------
 /*! \brief Method for simulating the model for a given period of time
  */
 //--------------------------------------------------------------------------
 
 void engine::run(double duration)  //!< Duration of time to run the model for
 {
-  std::clock_t start, current; 
+  std::clock_t start, current;
   const double t_start = t;
 
   start = std::clock();
   int riT= (int) (duration/DT+1e-2);
   double elapsed_realtime;
 
   for (int i= 0; i < riT; i++) {
-      // The StateMonitor and run_regularly operations are ordered by their "order" value
-      {% for is_state_monitor, obj in run_reg_state_monitor_operations %}
-      {% if is_state_monitor %}
-      {% if obj.when == 'start' %}
-      {% for var in obj.variables %}
-      {% if obj.isSynaptic %}
-      {% if obj.connectivity == 'DENSE' %}
-      convert_dense_matrix_2_dynamic_arrays({{var}}{{obj.monitored}},
-                                            {{obj.srcN}}, {{obj.trgN}},
-                                            brian::_dynamic_array_{{obj.monitored}}__synaptic_pre,
-                                            brian::_dynamic_array_{{obj.monitored}}__synaptic_post,
-                                            brian::_dynamic_array_{{obj.monitored}}_{{var}});
-      {% else %}
-      convert_sparse_synapses_2_dynamic_arrays(rowLength{{obj.monitored}},
-					       ind{{obj.monitored}},
-					       maxRowLength{{obj.monitored}},
-                                               {{var}}{{obj.monitored}},
-                                               {{obj.srcN}}, {{obj.trgN}},
-                                               brian::_dynamic_array_{{obj.monitored}}__synaptic_pre,
-                                               brian::_dynamic_array_{{obj.monitored}}__synaptic_post,
-                                               brian::_dynamic_array_{{obj.monitored}}_{{var}},
-                                               b2g::FULL_MONTY);
-      {% endif %}
-      {% else %}
-      {% if obj.src.variables[var].scalar %}
-      *brian::_array_{{obj.monitored}}_{{var}} = {{var}}{{obj.monitored}};
-      {% else %}
-      std::copy_n({{var}}{{obj.monitored}}, {{obj.N}}, brian::_array_{{obj.monitored}}_{{var}});
-      {% endif %}
-      {% endif %}
-      {% endfor %}
+    // The StateMonitor and run_regularly operations are ordered by their "order" value
+        {% for is_state_monitor, obj in run_reg_state_monitor_operations %}
+    if (i % {{obj['step']}} == 0)
+    {
+          {% if is_state_monitor %}
+      // Execute state monitor operation: {{obj['name']}}
+            {% if obj.when == 'start' %}
+              {% for var in obj.variables %}
+                {# No need to convert/copy for variables only changed on the host #}
+                {% if var + obj.monitored in vars_to_pull_for_start %}
+                  {% if obj.isSynaptic %}
+                    {% if obj.connectivity == 'DENSE' %}
+        convert_dense_matrix_2_dynamic_arrays({{var}}{{obj.monitored}},
+                                              {{obj.srcN}}, {{obj.trgN}},
+                                              brian::_dynamic_array_{{obj.monitored}}__synaptic_pre,
+                                              brian::_dynamic_array_{{obj.monitored}}__synaptic_post,
+                                              brian::_dynamic_array_{{obj.monitored}}_{{var}});
+                    {% else %}
+        convert_sparse_synapses_2_dynamic_arrays(rowLength{{obj.monitored}},
+                                                ind{{obj.monitored}},
+                                                maxRowLength{{obj.monitored}},
+                                                {{var}}{{obj.monitored}},
+                                                {{obj.srcN}}, {{obj.trgN}},
+                                                brian::_dynamic_array_{{obj.monitored}}__synaptic_pre,
+                                                brian::_dynamic_array_{{obj.monitored}}__synaptic_post,
+                                                brian::_dynamic_array_{{obj.monitored}}_{{var}},
+                                                b2g::FULL_MONTY);
+                    {% endif %}
+                  {% else %}
+                    {% if obj.src.variables[var].scalar %}
+        *brian::_array_{{obj.monitored}}_{{var}} = {{var}}{{obj.monitored}};
+                    {% else %}
+        std::copy_n({{var}}{{obj.monitored}}, {{obj.N}}, brian::_array_{{obj.monitored}}_{{var}});
+                    {% endif %}
+                  {% endif %}
+                {% endif %}
+              {% endfor %}
       _run_{{obj.codeobject_name}}();
-      {% endif %}
-      {% else %}
-      if (i % {{obj['step']}} == 0)
-      {
-          // Execute run_regularly operation: {{obj['name']}}
-          {% for var in obj['read'] %}
-        {% if var == 't' %}
-        std::copy_n(&t, 1, brian::_array_{{obj['owner'].clock.name}}_t);
-        {% elif var == 'dt' %}
-        {# nothing to do #}
-        {% else %}
-          {% if obj['isSynaptic'] %}
-          {% if obj['connectivity'] == 'DENSE' %}
-          convert_dense_matrix_2_dynamic_arrays({{var}}{{obj['owner'].name}},
-                                                {{obj['srcN']}}, {{obj['trgN']}},
-                                                brian::_dynamic_array_{{obj['owner'].name}}__synaptic_pre,
-                                                brian::_dynamic_array_{{obj['owner'].name}}__synaptic_post,
-                                                brian::_dynamic_array_{{obj['owner'].name}}_{{var}});
-          {% else %}
-          convert_sparse_synapses_2_dynamic_arrays(rowLength{{obj['owner'].name}},
-		                                   ind{{obj['owner'].name}},
-						   maxRowLength{{obj['owner'].name}},
-		                                   {{var}}{{obj['owner'].name}},
-                                                   {{obj['srcN']}}, {{obj['trgN']}},
-                                                   brian::_dynamic_array_{{obj['owner'].name}}__synaptic_pre,
-                                                   brian::_dynamic_array_{{obj['owner'].name}}__synaptic_post,
-                                                   brian::_dynamic_array_{{obj['owner'].name}}_{{var}}, b2g::FULL_MONTY);
-          {% endif %}
+            {% endif %}
           {% else %}
-	  {% if obj['owner'].variables[var].scalar %}
-	  *brian::_array_{{obj['owner'].name}}_{{var}} = {{var}}{{obj['owner'].name}};
-	  {% else %}
-           std::copy_n({{var}}{{obj['owner'].name}}, {{obj['owner'].variables[var].size}},
-                       brian::_array_{{obj['owner'].name}}_{{var}});
-	   {% endif %}
-          {% endif %}
-        {% endif %}
-        {% endfor %}
+      // Execute run_regularly operation: {{obj['name']}}
+            {% for var in obj['read'] %}
+              {% if var == 't' %}
+      std::copy_n(&t, 1, brian::_array_{{obj['owner'].clock.name}}_t);
+              {% elif var == 'dt' %}
+                {# nothing to do #}
+              {% else %}
+                {% if obj['isSynaptic'] %}
+                  {% if obj['connectivity'] == 'DENSE' %}
+      convert_dense_matrix_2_dynamic_arrays({{var}}{{obj['owner'].name}},
+                                            {{obj['srcN']}}, {{obj['trgN']}},
+                                            brian::_dynamic_array_{{obj['owner'].name}}__synaptic_pre,
+                                            brian::_dynamic_array_{{obj['owner'].name}}__synaptic_post,
+                                            brian::_dynamic_array_{{obj['owner'].name}}_{{var}});
+                  {% else %}
+      convert_sparse_synapses_2_dynamic_arrays(rowLength{{obj['owner'].name}},
+                                               ind{{obj['owner'].name}},
+                                               maxRowLength{{obj['owner'].name}},
+                                               {{var}}{{obj['owner'].name}},
+                                               {{obj['srcN']}}, {{obj['trgN']}},
+                                               brian::_dynamic_array_{{obj['owner'].name}}__synaptic_pre,
+                                               brian::_dynamic_array_{{obj['owner'].name}}__synaptic_post,
+                                               brian::_dynamic_array_{{obj['owner'].name}}_{{var}}, b2g::FULL_MONTY);
+                  {% endif %}
+                {% else %}
+                  {% if obj['owner'].variables[var].scalar %}
+      *brian::_array_{{obj['owner'].name}}_{{var}} = {{var}}{{obj['owner'].name}};
+                  {% else %}
+      std::copy_n({{var}}{{obj['owner'].name}}, {{obj['owner'].variables[var].size}},
+      brian::_array_{{obj['owner'].name}}_{{var}});
+                  {% endif %}
+                {% endif %}
+              {% endif %}
+            {% endfor %}
 
-          _run_{{obj['codeobj'].name}}();
+      _run_{{obj['codeobj'].name}}();
 
-           {% for var in obj['write'] %}
-           {% if obj['isSynaptic'] %}
-           {% if obj['connectivity'] == 'DENSE' %}
-           convert_dynamic_arrays_2_dense_matrix(brian::_dynamic_array_{{obj['owner'].name}}__synaptic_pre,
-                                                 brian::_dynamic_array_{{obj['owner'].name}}__synaptic_post,
-                                                 brian::_dynamic_array_{{obj['owner'].name}}_{{var}},
-                                                 {{var}}{{obj['owner'].name}},
-                                                 {{obj['srcN']}}, {{obj['trgN']}});
-           {% else %}
-           convert_dynamic_arrays_2_sparse_synapses(brian::_dynamic_array_{{obj['owner'].name}}_{{var}},
-						    sparseSynapseIndices{{obj['owner'].name}},
-                                                    {{var}}{{obj['owner'].name}},
-                                                    {{obj['srcN']}}, {{obj['trgN']}});
-           {% endif %}
-           {% else %}
-	   {% if obj['owner'].variables[var].scalar %}
-	   {{var}}{{obj['owner'].name}} = *brian::_array_{{obj['owner'].name}}_{{var}};
-	   {% else %}
-           std::copy_n(brian::_array_{{obj['owner'].name}}_{{var}}, {{obj['owner'].variables[var].size}}, {{var}}{{obj['owner'].name}});
-	   {% endif %}
-           {% endif %}
+            {% for var in obj['write'] %}
+              {% if obj['isSynaptic'] %}
+                {% if obj['connectivity'] == 'DENSE' %}
+      convert_dynamic_arrays_2_dense_matrix(brian::_dynamic_array_{{obj['owner'].name}}__synaptic_pre,
+                                            brian::_dynamic_array_{{obj['owner'].name}}__synaptic_post,
+                                            brian::_dynamic_array_{{obj['owner'].name}}_{{var}},
+                                            {{var}}{{obj['owner'].name}},
+                                            {{obj['srcN']}}, {{obj['trgN']}});
+                {% else %}
+      convert_dynamic_arrays_2_sparse_synapses(brian::_dynamic_array_{{obj['owner'].name}}_{{var}},
+                                               sparseSynapseIndices{{obj['owner'].name}},
+                                               {{var}}{{obj['owner'].name}},
+                                               {{obj['srcN']}}, {{obj['trgN']}});
+                {% endif %}
+              {% else %}
+                {% if obj['owner'].variables[var].scalar %}
+      {{var}}{{obj['owner'].name}} = *brian::_array_{{obj['owner'].name}}_{{var}};
+                {% else %}
+      std::copy_n(brian::_array_{{obj['owner'].name}}_{{var}}, {{obj['owner'].variables[var].size}}, {{var}}{{obj['owner'].name}});
+                {% endif %}
+              {% endif %}
+            {% endfor %}
+          {% endif %}
+    }
         {% endfor %}
-      }
-      {% endif %}
-      {% endfor %}
-      {% set states_pushed = [] %}
-      {% for run_reg in run_regularly_operations %}
-      if (i % {{run_reg['step']}} == 0)  // only push state if we executed the operation
-      {
+        {% set states_pushed = [] %}
+        {% for run_reg in run_regularly_operations %}
+    if (i % {{run_reg['step']}} == 0)  // only push state if we executed the operation
+    {
           {% for var in run_reg['write'] %}
-              {% if not run_reg['owner'].variables[var].owner.name in states_pushed %}
-              push{{run_reg['owner'].variables[var].owner.name}}StateToDevice();
-              {% if states_pushed.append(run_reg['owner'].variables[var].owner.name) %}{% endif %}
+            {# Don't push variables that are not used on the device #}
+            {% if var in groupDict[run_reg['owner'].name].variables %}
+              {% if not run_reg['owner'].variables[var] in states_pushed %}
+                {% set var_owner = run_reg['owner'].variables[var].owner %}
+                {% if var_owner.__class__.__name__ == 'Synapses' %}
+                  {% set push_name = var + var_owner.name%}
+                {% else %}
+                  {% set push_name = 'Current' + var + var_owner.name %}
+                {% endif %}
+                push{{push_name}}ToDevice();
+                {% if states_pushed.append(run_reg['owner'].variables[var]) %}{% endif %}
               {% endif %}
+            {% endif %}
           {% endfor %}
-      }
-      {% endfor %}
-      stepTime();
-      // The stepTimeGPU function already updated everything for the next time step
-      iT--;
-      t = iT*DT;
-      {% for spkGen in spikegenerator_models %}
-      _run_{{spkGen.codeobject_name}}();
-      push{{spkGen.name}}SpikesToDevice();
-      {% endfor %}
-      {% set spikes_pulled = [] %}
-      {% for spkMon in spike_monitor_models %}
-      {% if (spkMon.notSpikeGeneratorGroup) %}
-      {% if not spkMon.neuronGroup in spikes_pulled %}
-      pull{{spkMon.neuronGroup}}CurrentSpikesFromDevice();
-      {% if spikes_pulled.append(spkMon.neuronGroup) %}{% endif %}
-      {% endif %}
-      {% endif %}
-      {% endfor %}
-      {% for rateMon in rate_monitor_models %}
-      {% if (rateMon.notSpikeGeneratorGroup) %}
-      {% if not rateMon.neuronGroup in spikes_pulled %}
-      pull{{rateMon.neuronGroup}}CurrentSpikesFromDevice();
-      {% if spikes_pulled.append(rateMon.neuronGroup) %}{% endif %}
-      {% endif %}
-      {% endif %}
-      {% endfor %}
-      {% set states_pulled = [] %}
-      {% for sm in state_monitor_models %}
-      {% if not sm.monitored in states_pulled %}
-      pull{{sm.monitored}}StateFromDevice();
-      {% if states_pulled.append(sm.monitored) %}{% endif %}
-      {% endif %}
-      {% endfor %}
-      {% for run_reg in run_regularly_operations %}
-        if ((i + 1) % {{run_reg['step']}} == 0)  // only pull state if next time step executes operation
-        {
-            {% for var in run_reg['read'] %}
-            {% if not var in ['t', 'dt'] %}
-            {% if not run_reg['owner'].variables[var].owner.name in states_pulled %}
-            pull{{run_reg['owner'].variables[var].owner.name}}StateFromDevice();
-            {% if states_pulled.append(run_reg['owner'].variables[var].owner.name) %}{% endif %}
+    }
+        {% endfor %}
+    stepTime();
+    // The stepTimeGPU function already updated everything for the next time step
+    iT--;
+    t = iT*DT;
+        {% for spkGen in spikegenerator_models %}
+    _run_{{spkGen.codeobject_name}}();
+    push{{spkGen.name}}SpikesToDevice();
+        {% endfor %}
+        {% set spikes_pulled = [] %}
+        {% for spkMon in spike_monitor_models %}
+          {% if (spkMon.notSpikeGeneratorGroup) %}
+            {% if not spkMon.neuronGroup in spikes_pulled %}
+    pull{{spkMon.neuronGroup}}CurrentSpikesFromDevice();
+              {% if spikes_pulled.append(spkMon.neuronGroup) %}
+              {% endif %}
             {% endif %}
+          {% endif %}
+        {% endfor %}
+        {% for rateMon in rate_monitor_models %}
+          {% if (rateMon.notSpikeGeneratorGroup) %}
+            {% if not rateMon.neuronGroup in spikes_pulled %}
+    pull{{rateMon.neuronGroup}}CurrentSpikesFromDevice();
+              {% if spikes_pulled.append(rateMon.neuronGroup) %}
+              {% endif %}
             {% endif %}
+          {% endif %}
+        {% endfor %}
+        {% for key, steps in vars_to_pull_for_start.items() %}
+          {% if steps[0] == 1 %}
+    pull{{key}}FromDevice();
+          {% else %}
+    if (
+            {%- for step in steps %}
+              {% if loop.index > 1 %} || {% endif -%}
+      ((i+1) % {{step}} == 0)
+            {%- endfor -%}
+    ) {
+      pull{{key}}FromDevice();
+    }
+          {% endif %}
+        {% endfor %}
+        {% for key, steps in vars_to_pull_for_end.items() %}
+          {% if steps[0] == 1 %}
+    pull{{key}}FromDevice();
+          {% else %}
+    if (
+            {%- for step in steps %}
+              {% if loop.index > 1 %} || {% endif -%}
+      ((i+1) % {{step}} == 0)
+            {%- endfor -%}
+    ) {
+      pull{{key}}FromDevice();
+    }
+          {% endif %}
+        {% endfor %}
+    // report state
+        {% for sm in state_monitor_models %}
+          {% if sm.when != 'start' %}
+    if (i % {{sm['step']}} == 0)
+    {
+      // Execute state monitor operation: {{sm['name']}}
+            {% for var in sm.variables %}
+              {# No need to convert/copy for variables only changed on the host #}
+              {% if var + sm.monitored in vars_to_pull_for_end %}
+                {% if sm.isSynaptic %}
+                  {% if sm.connectivity == 'DENSE' %}
+        convert_dense_matrix_2_dynamic_arrays({{var}}{{sm.monitored}},
+                                              {{sm.srcN}}, {{sm.trgN}},
+                                              brian::_dynamic_array_{{sm.monitored}}__synaptic_pre,
+                                              brian::_dynamic_array_{{sm.monitored}}__synaptic_post,
+                                              brian::_dynamic_array_{{sm.monitored}}_{{var}});
+                  {% else %}
+        convert_sparse_synapses_2_dynamic_arrays(rowLength{{sm.monitored}},
+                                                ind{{sm.monitored}},
+                                                maxRowLength{{sm.monitored}},
+                                                {{var}}{{sm.monitored}},
+                                                {{sm.srcN}}, {{sm.trgN}},
+                                                brian::_dynamic_array_{{sm.monitored}}__synaptic_pre,
+                                                brian::_dynamic_array_{{sm.monitored}}__synaptic_post,
+                                                brian::_dynamic_array_{{sm.monitored}}_{{var}},
+                                                b2g::FULL_MONTY);
+                  {% endif %}
+                {% else %}
+                  {% if sm.src.variables[var].scalar %}
+        *brian::_array_{{sm.monitored}}_{{var}} = {{var}}{{sm.monitored}};
+                  {% else %}
+        std::copy_n({{var}}{{sm.monitored}}, {{sm.N}}, brian::_array_{{sm.monitored}}_{{var}});
+                  {% endif %}
+                {% endif %}
+              {% endif %}
             {% endfor %}
-        }
-      {% endfor %}
-      // report state 
-      {% for sm in state_monitor_models %}
-      {% if sm.when != 'start' %}
-      {% for var in sm.variables %}
-      {% if sm.isSynaptic %}
-      {% if sm.connectivity == 'DENSE' %}
-      convert_dense_matrix_2_dynamic_arrays({{var}}{{sm.monitored}}, {{sm.srcN}}, {{sm.trgN}},brian::_dynamic_array_{{sm.monitored}}__synaptic_pre, brian::_dynamic_array_{{sm.monitored}}__synaptic_post, brian::_dynamic_array_{{sm.monitored}}_{{var}});
-      {% else %}
-      convert_sparse_synapses_2_dynamic_arrays(rowLength{{sm.monitored}}, ind{{sm.monitored}}, maxRowLength{{sm.monitored}}, {{var}}{{sm.monitored}}, {{sm.srcN}}, {{sm.trgN}}, brian::_dynamic_array_{{sm.monitored}}__synaptic_pre, brian::_dynamic_array_{{sm.monitored}}__synaptic_post, brian::_dynamic_array_{{sm.monitored}}_{{var}}, b2g::FULL_MONTY);
-      {% endif %}
-      {% else %}
-      {% if sm.src.variables[var].scalar %}
-      *brian::_array_{{sm.monitored}}_{{var}} = {{var}}{{sm.monitored}};
-      {% else %}
-      std::copy_n({{var}}{{sm.monitored}}, {{sm.N}}, brian::_array_{{sm.monitored}}_{{var}});
-      {% endif %}
-      {% endif %}
-      {% endfor %}
       _run_{{sm.codeobject_name}}();
-      {% endif %}
-      {% endfor %}
-      // report spikes
-      {% for spkMon in spike_monitor_models %}
-      _run_{{spkMon.codeobject_name}}();
-      {% endfor %}
-      {% for rateMon in rate_monitor_models %}
-      _run_{{rateMon.codeobject_name}}();
-      {% endfor %}
-      // Bring the time step back to the value for the next loop iteration
-      iT++;
-      t = iT*DT;
-      {% if maximum_run_time is not none %}
-      current= std::clock();
-      elapsed_realtime= (double) (current - start)/CLOCKS_PER_SEC;
-      if (elapsed_realtime > {{maximum_run_time}}) {
-        break;
-      }
-      {% endif %}
-  }  
-  {% if maximum_run_time is none %}
+    }
+          {% endif %}
+        {% endfor %}
+    // report spikes
+        {% for spkMon in spike_monitor_models %}
+    _run_{{spkMon.codeobject_name}}();
+        {% endfor %}
+        {% for rateMon in rate_monitor_models %}
+    _run_{{rateMon.codeobject_name}}();
+        {% endfor %}
+    // Bring the time step back to the value for the next loop iteration
+    iT++;
+    t = iT*DT;
+        {% if maximum_run_time is not none %}
+    current= std::clock();
+    elapsed_realtime= (double) (current - start)/CLOCKS_PER_SEC;
+    if (elapsed_realtime > {{maximum_run_time}}) {
+      break;
+    }
+        {% endif %}
+  }
+        {% if maximum_run_time is none %}
   current= std::clock();
   elapsed_realtime= (double) (current - start)/CLOCKS_PER_SEC;
-  {% endif %}
+        {% endif %}
   Network::_last_run_time = elapsed_realtime;
   if (duration > 0.0)
   {
-      Network::_last_run_completed_fraction = (t-t_start)/duration;
+    Network::_last_run_completed_fraction = (t-t_start)/duration;
   } else {
-      Network::_last_run_completed_fraction = 1.0;
+    Network::_last_run_completed_fraction = 1.0;
   }
 }
 
 //--------------------------------------------------------------------------
 /*! \brief Method for copying all variables of the last time step from the GPU
- 
+
   This is a simple wrapper for the convenience function copyStateFromDevice() which is provided by GeNN.
 */
 //--------------------------------------------------------------------------
 
 void engine::getStateFromGPU()
 {
   copyStateFromDevice();
 }
 
 //--------------------------------------------------------------------------
 /*! \brief Method for copying all spikes of the last time step from the GPU
- 
+
   This is a simple wrapper for the convenience function copySpikesFromDevice() which is provided by GeNN.
 */
 //--------------------------------------------------------------------------
 
 void engine::getSpikesFromGPU()
 {
   copyCurrentSpikesFromDevice();
 }
 
 
 
-#endif	
+#endif
 
 {% endmacro %}
```

### Comparing `Brian2GeNN-1.6/brian2genn/templates/main.cpp` & `Brian2GeNN-1.7.0/brian2genn/templates/main.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -33,18 +33,19 @@
     return 1;
   }
   double totalTime= atof(argv[2]);
   string OutDir = std::string(argv[1]) +"_output";
   string cmd= std::string("mkdir ") +OutDir;
   system(cmd.c_str());
   string name;
+  {% if profiled %}
   name= OutDir+ "/"+ argv[1] + ".time";
   FILE *timef= fopen(name.c_str(),"a");
-
-  fprintf(stderr, "# DT %f \n", DT);
+  {% endif %}
+  fprintf(stderr, "# DT %g \n", DT);
   fprintf(stderr, "# totalTime %f \n", totalTime);
 
   {{'\n'.join(code_lines['before_start'])|autoindent}}
 
   //-----------------------------------------------------------------
   // build the neuronal circuitery (calls initialize and allocateMem)
   engine eng;
@@ -125,22 +126,23 @@
   
   //------------------------------------------------------------------
   // output general parameters to output file and start the simulation
   fprintf(stderr, "# We are running with fixed time step %f \n", DT);
 
   t= 0.;
   void *devPtr;
-  {{'\n'.join(code_lines['before_run'])|autoindent}}
+  {{'\n'.join(code_lines['before_network_run'])|autoindent}}
   eng.run(totalTime); // run for the full duration
-  {{'\n'.join(code_lines['after_run'])|autoindent}}
+  {{'\n'.join(code_lines['after_network_run'])|autoindent}}
   cerr << t << " done ..." << endl;
-  {% if prefs['devices.genn.kernel_timing'] %}
+  {% if profiled %}
   {% for kt in ('neuronUpdateTime', 'presynapticUpdateTime', 'postsynapticUpdateTime', 'synapseDynamicsTime', 'initTime', 'initSparseTime') %}
   fprintf(timef,"%f ", {{kt}});
   {% endfor %}
+  fprintf(timef,"\n");
   {% endif %} 
 
   // get the final results from the GPU 
   eng.getStateFromGPU();
   eng.getSpikesFromGPU();
 
   // translate GeNN arrays back to synaptic arrays
```

### Comparing `Brian2GeNN-1.6/brian2genn/templates/max_row_length_array.cpp` & `Brian2GeNN-1.7.0/brian2genn/templates/max_row_length_array.cpp`

 * *Files identical despite different names*

### Comparing `Brian2GeNN-1.6/brian2genn/templates/model.cpp` & `Brian2GeNN-1.7.0/brian2genn/templates/model.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,23 @@
 
 #include <stdint.h>
 #include "modelSpec.h"
 #include "brianlib/randomkit/randomkit.cc"
 
 #include "objects.h"
 #include "objects.cpp"
+
+{% for header in header_files %}
+{% if header.startswith('"') or header.startswith('<') %}
+#include {{header}}
+{% else %}
+#include "{{header}}"
+{% endif %}
+{% endfor %}
+
 // We need these to compile objects.cpp, but they are only used in _write_arrays which we never call.
 double Network::_last_run_time = 0.0;
 double Network::_last_run_completed_fraction = 0.0;
 
 {% for inc in codeobj_inc %}
 {{inc}}
 {% endfor %}
@@ -209,15 +218,15 @@
     {{ dtDef }}
 
     model.setName("magicnetwork_model");
     model.setPrecision({{precision}});
     {% if precision == 'GENN_FLOAT' %}
     model.setTimePrecision(TimePrecision::DOUBLE);
     {% endif %}
-    {% if prefs['devices.genn.kernel_timing'] %}
+    {% if profiled %}
     model.setTiming(true);
     {% endif %}
     {% for neuron_model in neuron_models %}
     model.addNeuronPopulation<{{neuron_model.name}}NEURON>("{{neuron_model.name}}", {{neuron_model.N}}, {{neuron_model.name}}_p, {{neuron_model.name}}_ini);
     {% endfor %}
     {% for spikeGen_model in spikegenerator_models %}
     model.addNeuronPopulation<NeuronModels::SpikeSource>("{{spikeGen_model.name}}", {{spikeGen_model.N}}, {}, {});
```

### Comparing `Brian2GeNN-1.6/brian2genn/templates/neuron_code.cpp` & `Brian2GeNN-1.7.0/brian2genn/templates/neuron_code.cpp`

 * *Files identical despite different names*

### Comparing `Brian2GeNN-1.6/brian2genn/templates/project_vcxproj` & `Brian2GeNN-1.7.0/brian2genn/templates/project_vcxproj`

 * *Files identical despite different names*

### Comparing `Brian2GeNN-1.6/brian2genn/templates/ratemonitor.cpp` & `Brian2GeNN-1.7.0/brian2genn/templates/ratemonitor.cpp`

 * *Files identical despite different names*

### Comparing `Brian2GeNN-1.6/brian2genn/templates/spikegenerator.cpp` & `Brian2GeNN-1.7.0/brian2genn/templates/spikegenerator.cpp`

 * *Files identical despite different names*

### Comparing `Brian2GeNN-1.6/brian2genn/templates/spikemonitor.cpp` & `Brian2GeNN-1.7.0/brian2genn/templates/spikemonitor.cpp`

 * *Files identical despite different names*

### Comparing `Brian2GeNN-1.6/brian2genn/templates/statemonitor.cpp` & `Brian2GeNN-1.7.0/brian2genn/templates/statemonitor.cpp`

 * *Files identical despite different names*

### Comparing `Brian2GeNN-1.6/brian2genn/templates/template_notes.txt` & `Brian2GeNN-1.7.0/brian2genn/templates/template_notes.txt`

 * *Files identical despite different names*

### Comparing `Brian2GeNN-1.6/docs_sphinx/conf.py` & `Brian2GeNN-1.7.0/docs_sphinx/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,74 +17,61 @@
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 sys.path.insert(0, os.path.abspath('..'))
 
 
-# Mock the scipy module
-class Mock(object):
-    def __init__(self, *args, **kwargs):
-        pass
-
-    def __call__(self, *args, **kwargs):
-        return Mock()
-
-    @classmethod
-    def __getattr__(cls, name):
-        if name in ('__file__', '__path__'):
-            return '/dev/null'
-        elif name[0] == name[0].upper():
-            mockType = type(name, (), {})
-            mockType.__module__ = __name__
-            return mockType
-        else:
-            return Mock()
-
-MOCK_MODULES = ['scipy', 'brian2genn', 'brian', 'brian.hears',   # mock Brian1 for the bridge
-                'Cython', 'Cython.Compiler', 'Cython.Build']
-for mod_name in MOCK_MODULES:
-    sys.modules[mod_name] = Mock()
-
-# Store the examples and tutorials directory in an environment variable,
-# used by the "example finder" that is called as part of the autoclass documentation
-#os.environ['BRIAN2_DOCS_EXAMPLE_DIR'] = root_dir = os.path.abspath('../examples')
-#os.environ['BRIAN2_DOCS_TUTORIALS_DIR'] = root_dir = os.path.abspath('../tutorials')
-
-#if 'BRIAN2GENN_DOCS_QUICK_REBUILD' not in os.environ:
-    # -- Automatically generate the reference documentation -----------------------
-    #import brian2genn.sphinxext.generate_reference as generate_reference
-    # first generate the reference documentation
-    target_dir = './reference'
-    if os.path.exists(target_dir):
-        shutil.rmtree(target_dir)
-    os.makedirs(target_dir)
-    abs_root = os.path.abspath('../brian2genn')
-    generate_reference.main(abs_root, ['tests', 'sphinxext'], target_dir)
-    
-    # -- Automatically generate the examples documentation -------------------------
-#    import brian2.sphinxext.generate_examples as generate_examples
-#    target_dir = './examples'
-#    root_dir = os.path.abspath('../examples')
-#    generate_examples.main(root_dir, target_dir)
+# # Mock the scipy module
+# class Mock(object):
+#     def __init__(self, *args, **kwargs):
+#         pass
+#
+#     def __call__(self, *args, **kwargs):
+#         return Mock()
+#
+#     @classmethod
+#     def __getattr__(cls, name):
+#         if name in ('__file__', '__path__'):
+#             return '/dev/null'
+#         elif name[0] == name[0].upper():
+#             mockType = type(name, (), {})
+#             mockType.__module__ = __name__
+#             return mockType
+#         else:
+#             return Mock()
+#
+# MOCK_MODULES = ['scipy', 'brian2genn', 'brian', 'brian.hears',   # mock Brian1 for the bridge
+#                 'Cython', 'Cython.Compiler', 'Cython.Build']
+# for mod_name in MOCK_MODULES:
+#     sys.modules[mod_name] = Mock()
+
+target_dir = './reference'
+if os.path.exists(target_dir):
+    shutil.rmtree(target_dir)
+os.makedirs(target_dir)
+abs_root = os.path.abspath('../brian2genn')
+generate_reference.main(abs_root, exclude_dirs=['tests', 'sphinxext'],
+                        exclude_files=[], destdir=target_dir)
+
 
 # -- General configuration -----------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 needs_sphinx = '1.0.1'
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = ['sphinx.ext.autodoc', 'sphinx.ext.doctest',
               'sphinx.ext.intersphinx', 'sphinx.ext.todo',
               'sphinx.ext.coverage', 'sphinx.ext.mathjax',
               'sphinx.ext.viewcode',
               'brian2genn.sphinxext.briandoc',
               'sphinx.ext.autosummary',
-#              'sphinxcontrib.issuetracker'
+              'sphinxcontrib.issuetracker'
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix of source filenames.
 source_suffix = '.rst'
@@ -99,18 +86,18 @@
 project = 'Brian2GeNN'
 copyright = '2012-, Brian2GeNN authors'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
-# The short X.Y version.
-version = '1.5'
-# The full version, including alpha/beta/rc tags.
-release = '1.5'
+from importlib.metadata import version
+release = version('brian2genn')
+# only major/minor
+version = '.'.join(release.split('.')[:2])
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
@@ -140,27 +127,14 @@
 pygments_style = 'sphinx'
 
 # A list of ignored prefixes for module index sorting.
 modindex_common_prefix = ['brian2genn.']
 
 
 # -- Options for HTML output ---------------------------------------------------
-
-# on_rtd is whether we are on readthedocs.org, this line of code grabbed from docs.readthedocs.org
-on_rtd = os.environ.get('READTHEDOCS', None) == 'True'
-
-if not on_rtd:
-    # ReadTheDocs theme
-    try:
-        import sphinx_rtd_theme
-        html_theme = "sphinx_rtd_theme"
-        html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]
-    except ImportError:
-        pass  # use the default theme
-
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #html_theme_options = {}
 
 
 # The name for this set of Sphinx documents.  If None, it defaults to
@@ -305,15 +279,16 @@
 
 
 intersphinx_mapping = {
     'http://docs.python.org/': None,
     'http://docs.scipy.org/doc/numpy': None,
     'http://docs.scipy.org/doc/scipy/reference': None,
     'http://docs.sympy.org/dev/': None,
-    'https://nose.readthedocs.org/en/latest/': None
+    'https://nose.readthedocs.org/en/latest/': None,
+    'https://brian2.readthedocs.org/en/stable/': None,
 }
 
 autodoc_default_flags = ['show-inheritance']
 
 # Configure linking to github
 issuetracker = 'github'
 issuetracker_project = 'brian-team/brian2genn'
```

### Comparing `Brian2GeNN-1.6/docs_sphinx/introduction/exclusions.rst` & `Brian2GeNN-1.7.0/docs_sphinx/introduction/exclusions.rst`

 * *Files identical despite different names*

### Comparing `Brian2GeNN-1.6/docs_sphinx/introduction/index.rst` & `Brian2GeNN-1.7.0/docs_sphinx/introduction/index.rst`

 * *Files identical despite different names*

### Comparing `Brian2GeNN-1.6/docs_sphinx/introduction/preferences.rst` & `Brian2GeNN-1.7.0/docs_sphinx/introduction/preferences.rst`

 * *Files identical despite different names*

### Comparing `Brian2GeNN-1.6/docs_sphinx/technical/how_it_works.rst` & `Brian2GeNN-1.7.0/docs_sphinx/technical/how_it_works.rst`

 * *Files identical despite different names*

### Comparing `Brian2GeNN-1.6/examples/simple_example_HH.py` & `Brian2GeNN-1.7.0/examples/simple_example_HH.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,14 +10,14 @@
 gK= 36
 EK= -72
 gl= 0.3
 El= -50
 C= 1
 eqs = '''
 dV/dt= (m**3*h*gNa*(ENa-V)+n**4*gK*(EK-V)+gl*(El-V)+Iin)/C/ms : 1
-dm/dt= ((3.5+0.1*V)/(1-exp(-3.5-0.1*V))*(1-m)-4*exp(-(V+60)/18)*m)/ms : 1
-dh/dt= (0.07*exp(-V/20-3)*(1-h)-1/(exp(-3-0.1*V)+1)*h)/ms : 1
-dn/dt= ((-0.5-0.01*V)/(exp(-5-0.1*V)-1)*(1-n)-0.125*exp(-(V+60)/80)*n)/ms : 1
+dm/dt= ((3.5+0.1*V)/(1-exp(-3.5-0.1*V))*(1.0-m)-4.0*exp(-(V+60.0)/18.0)*m)/ms : 1
+dh/dt= (0.07*exp(-V/20.0-3.0)*(1.0-h)-1.0/(exp(-3.0-0.1*V)+1.0)*h)/ms : 1
+dn/dt= ((-0.5-0.01*V)/(exp(-5.0-0.1*V)-1)*(1.0-n)-0.125*exp(-(V+60.0)/80.0)*n)/ms : 1
 '''
 G = NeuronGroup(N, eqs, threshold='V> 0', reset='', method='exponential_euler')
 
 run(500*ms)
```

### Comparing `Brian2GeNN-1.6/examples/simple_example_HH_CPP.py` & `Brian2GeNN-1.7.0/examples/simple_example_HH_CPP.py`

 * *Files identical despite different names*

### Comparing `Brian2GeNN-1.6/examples/simple_example_synapses.py` & `Brian2GeNN-1.7.0/examples/simple_example_synapses.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,38 +11,38 @@
 Iin : 1
 '''
 G = NeuronGroup(N, eqs, threshold='V>1', reset='V=0', name='PN')
 G.V = rand()
 G2 = NeuronGroup(N, eqs, threshold='V>1', reset='V=0', name='LN')
 G2.V = 2 * rand()
 
-alpha = 20 * ms
-beta = 30 * ms
+alpha = 20/ms
+beta = 30/ms
 S = Synapses(G, G2,
              model='''
             ds/dt= alpha*(1-s) - beta*s: 1
             g: 1
             ''',
              pre='Iin_post+= g',
              name='ex_syns')
 
-alpha2 = 40 * ms
-beta2 = 60 * ms
+alpha2 = 40/ms
+beta2 = 60/ms
 p_post = 1
 p_pre = 30
 S2 = Synapses(G2, G,
               model='''
              ds/dt= alpha2*(1-s) - beta2*s: 1
              g: 1
              ''',
               pre='Iin_post+= g*p_pre',
               post='''
              g*= p_post-0.9;
              ''',
               name='inh_syns')
 
 S.connect(i=1, j=5)
-S.connect(i=[1, 2], j=[1, 2])
+S2.connect(i=[1, 2], j=[1, 2])
 
 S.g = 'rand()'
 
 run(100*ms)
```

### Comparing `Brian2GeNN-1.6/examples/testSummedVars.py` & `Brian2GeNN-1.7.0/examples/testSummedVars.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from brian2 import *
 import brian2genn
 
-set_device('genn', directory='testSummedVars', use_GPU=False)
+set_device('genn', directory='testSummedVars')
 # set_device('cpp_standalone')
 
 neurons = NeuronGroup(1, """dv/dt = (g-v)/(10*ms) : 1
                             g : 1""", method='exact', threshold='v > 0.1', reset='v= 0')
 neurons.g = 0.2
-H = NeuronGroup(10, 'V:1', threshold='V > 0.5')
+H = NeuronGroup(10, 'V:1', threshold='V > 0.5', reset='')
 
 S = Synapses(neurons, H, '''
-               dg_syn/dt = -g_syn/(100*ms) : 1 (event-driven)
+                dg_syn/dt = -g_syn/(100*ms) : 1 (clock-driven)
                 V_post = g_syn : 1 (summed)''', on_pre='g_syn= g_syn+1')
 S.connect(True)
 mon = StateMonitor(S, variables=True, record=range(10))
 mon2 = StateMonitor(neurons, variables=True, record=True)
 mon3 = StateMonitor(H, variables=True, record=True)
 run(101 * ms)
```

