# Comparing `tmp/NeuralPlayground-0.0.2.tar.gz` & `tmp/NeuralPlayground-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeuralPlayground-0.0.2.tar", last modified: Fri Jul 21 13:09:28 2023, max compression
+gzip compressed data, was "NeuralPlayground-0.0.3.tar", last modified: Fri Jul 28 12:56:09 2023, max compression
```

## Comparing `NeuralPlayground-0.0.2.tar` & `NeuralPlayground-0.0.3.tar`

### file list

```diff
@@ -1,60 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:09:28.793414 NeuralPlayground-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-21 13:09:19.000000 NeuralPlayground-0.0.2/.all-contributorsrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:09:28.789414 NeuralPlayground-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:09:28.789414 NeuralPlayground-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-21 13:09:19.000000 NeuralPlayground-0.0.2/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-21 13:09:19.000000 NeuralPlayground-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-21 13:09:19.000000 NeuralPlayground-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-21 13:09:19.000000 NeuralPlayground-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-21 13:09:19.000000 NeuralPlayground-0.0.2/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:09:28.789414 NeuralPlayground-0.0.2/NeuralPlayground.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-07-21 13:09:28.000000 NeuralPlayground-0.0.2/NeuralPlayground.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-21 13:09:28.000000 NeuralPlayground-0.0.2/NeuralPlayground.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 13:09:28.000000 NeuralPlayground-0.0.2/NeuralPlayground.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-21 13:09:28.000000 NeuralPlayground-0.0.2/NeuralPlayground.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-21 13:09:28.000000 NeuralPlayground-0.0.2/NeuralPlayground.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-07-21 13:09:28.793414 NeuralPlayground-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12373 2023-07-21 13:09:19.000000 NeuralPlayground-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:09:28.789414 NeuralPlayground-0.0.2/documents/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-21 13:09:19.000000 NeuralPlayground-0.0.2/documents/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-21 13:09:19.000000 NeuralPlayground-0.0.2/documents/citation.cff
--rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-07-21 13:09:19.000000 NeuralPlayground-0.0.2/documents/code_of_conduct.md
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-21 13:09:19.000000 NeuralPlayground-0.0.2/documents/contributors.md
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-07-21 13:09:19.000000 NeuralPlayground-0.0.2/documents/licence.md
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-21 13:09:19.000000 NeuralPlayground-0.0.2/documents/road_map.md
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-21 13:09:19.000000 NeuralPlayground-0.0.2/documents/style_guide.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:09:28.789414 NeuralPlayground-0.0.2/neuralplayground/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:09:28.793414 NeuralPlayground-0.0.2/neuralplayground/agents/
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/agents/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8167 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/agents/agent_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    16662 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/agents/stachenfeld_2018.py
--rw-r--r--   0 runner    (1001) docker     (123)    17934 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/agents/weber_2018.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:09:28.793414 NeuralPlayground-0.0.2/neuralplayground/arenas/
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/arenas/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/arenas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/arenas/arena_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/arenas/connected_rooms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/arenas/hafting_2008.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/arenas/sargolini_2006.py
--rw-r--r--   0 runner    (1001) docker     (123)    14509 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/arenas/simple2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/arenas/wernle_2018.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:09:28.793414 NeuralPlayground-0.0.2/neuralplayground/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/experiments/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/experiments/experiment_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    22676 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/experiments/hafting_2008_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/experiments/sargolini_2006_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    25566 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/experiments/wernle_2018_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11834 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 13:09:28.793414 NeuralPlayground-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:09:28.793414 NeuralPlayground-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/tests/agent_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/tests/arena_exp_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:09.784187 NeuralPlayground-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/.all-contributorsrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:09.772187 NeuralPlayground-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:09.776187 NeuralPlayground-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:09.776187 NeuralPlayground-0.0.3/NeuralPlayground.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14553 2023-07-28 12:56:09.000000 NeuralPlayground-0.0.3/NeuralPlayground.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-28 12:56:09.000000 NeuralPlayground-0.0.3/NeuralPlayground.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 12:56:09.000000 NeuralPlayground-0.0.3/NeuralPlayground.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-28 12:56:09.000000 NeuralPlayground-0.0.3/NeuralPlayground.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 12:56:09.000000 NeuralPlayground-0.0.3/NeuralPlayground.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14553 2023-07-28 12:56:09.784187 NeuralPlayground-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13343 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:09.776187 NeuralPlayground-0.0.3/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/documents/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/documents/citation.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/documents/code_of_conduct.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/documents/contributors.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/documents/licence.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/documents/road_map.md
+-rw-r--r--   0 runner    (1001) docker     (123)    20407 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/documents/style_guide.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:09.776187 NeuralPlayground-0.0.3/neuralplayground/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:09.776187 NeuralPlayground-0.0.3/neuralplayground/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/agents/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/agents/agent_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17483 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/agents/stachenfeld_2018.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19519 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/agents/weber_2018.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22858 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/agents/whittington_2020.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:09.780187 NeuralPlayground-0.0.3/neuralplayground/agents/whittington_2020_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)    20991 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/agents/whittington_2020_extras/whittington_2020_analyse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66462 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/agents/whittington_2020_extras/whittington_2020_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/agents/whittington_2020_extras/whittington_2020_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/agents/whittington_2020_extras/whittington_2020_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:09.780187 NeuralPlayground-0.0.3/neuralplayground/arenas/
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/arenas/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/arenas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/arenas/arena_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/arenas/batch_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/arenas/connected_rooms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15728 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/arenas/discritized_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9980 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/arenas/hafting_2008.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/arenas/sargolini_2006.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13424 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/arenas/simple2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/arenas/wernle_2018.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:09.780187 NeuralPlayground-0.0.3/neuralplayground/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/backend/default_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/backend/simulation_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/backend/training_loops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:09.780187 NeuralPlayground-0.0.3/neuralplayground/comparison/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/comparison/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22109 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/comparison/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:09.780187 NeuralPlayground-0.0.3/neuralplayground/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/config/default_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/config/load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/config/main_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/config/plot_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:09.780187 NeuralPlayground-0.0.3/neuralplayground/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/experiments/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/experiments/experiment_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20311 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/experiments/hafting_2008_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9539 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/experiments/sargolini_2006_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23539 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/experiments/wernle_2018_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:09.780187 NeuralPlayground-0.0.3/neuralplayground/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/plotting/plot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 12:56:09.784187 NeuralPlayground-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:09.780187 NeuralPlayground-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/tests/agent_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/tests/arena_exp_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/tox.ini
```

### Comparing `NeuralPlayground-0.0.2/.all-contributorsrc` & `NeuralPlayground-0.0.3/.all-contributorsrc`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9907407407407408%*

 * *Differences: {"'contributors'": "{insert: [(7, OrderedDict([('login', 'rhayman'), ('name', 'rhayman'), "*

 * *                   "('avatar_url', 'https://avatars.githubusercontent.com/u/5619644?v=4'), "*

 * *                   "('profile', 'https://github.com/rhayman'), ('contributions', ['code'])])), (8, "*

 * *                   "OrderedDict([('login', 'JarvisDevon'), ('name', 'Devon Jarvis'), "*

 * *                   "('avatar_url', 'https://avatars.githubusercontent.com/u/30460455?v=4'), "*

 * *                   "('profile', 'https://gith […]*

```diff
@@ -71,14 +71,33 @@
             "contributions": [
                 "maintenance",
                 "infra"
             ],
             "login": "adamltyson",
             "name": "Adam Tyson",
             "profile": "http://adamltyson.com"
+        },
+        {
+            "avatar_url": "https://avatars.githubusercontent.com/u/5619644?v=4",
+            "contributions": [
+                "code"
+            ],
+            "login": "rhayman",
+            "name": "rhayman",
+            "profile": "https://github.com/rhayman"
+        },
+        {
+            "avatar_url": "https://avatars.githubusercontent.com/u/30460455?v=4",
+            "contributions": [
+                "doc",
+                "code"
+            ],
+            "login": "JarvisDevon",
+            "name": "Devon Jarvis",
+            "profile": "https://github.com/JarvisDevon"
         }
     ],
     "contributorsPerLine": 7,
     "files": [
         "README.md"
     ],
     "imageSize": 100,
```

### Comparing `NeuralPlayground-0.0.2/.github/workflows/test_and_deploy.yml` & `NeuralPlayground-0.0.3/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.2/.gitignore` & `NeuralPlayground-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.2/.pre-commit-config.yaml` & `NeuralPlayground-0.0.3/.pre-commit-config.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -8,15 +8,16 @@
           - id: check-merge-conflict
           - id: check-toml
           - id: end-of-file-fixer
           - id: mixed-line-ending
             args: [--fix=lf]
           - id: requirements-txt-fixer
           - id: trailing-whitespace
+            exclude: 'README.md'
     - repo: https://github.com/charliermarsh/ruff-pre-commit
-      rev: v0.0.265
+      rev: v0.0.280
       hooks:
         - id: ruff
     - repo: https://github.com/psf/black
-      rev: 23.3.0
+      rev: 23.7.0
       hooks:
           - id: black
```

### Comparing `NeuralPlayground-0.0.2/LICENSE` & `NeuralPlayground-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.2/NeuralPlayground.egg-info/PKG-INFO` & `NeuralPlayground-0.0.3/NeuralPlayground.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuralPlayground
-Version: 0.0.2
+Version: 0.0.3
 Summary: The standardised environment for the hippocampus and entorhinal cortex models
 Author: Clementine Domine
 Author-email: Rodrigo Carrasco-Davis <rodrigo.carrasco.davis@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/ClementineDomine/NeuralPlayground
 Project-URL: Bug tracker, https://github.com/ClementineDomine/NeuralPlayground/issues
 Project-URL: Documentation, https://github.com/ClementineDomine/NeuralPlayground
@@ -20,20 +20,21 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# NeuralPlayground: The  standardised environment for the hippocampus and entorhinal cortex models.
-<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-7-orange.svg?style=flat-square)](#contributors-)
-<!-- ALL-CONTRIBUTORS-BADGE:END -->
 
+# NeuralPlayground: The  standardised environment for the hippocampus and entorhinal cortex models. 
+### (Developing visualization and comparison board)
 
+<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
+[![All Contributors](https://img.shields.io/badge/all_contributors-9-orange.svg?style=flat-square)](#contributors-)
+<!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 * [1 Introduction](#1-Introduction)
 * [2 Installation ](#2-Installation)
 * [3 The Project](#3-Project)
 * [4 How to Contribute](#4-I-want-to-Contribute)
 * [5 Cite ](#5-Cite)
 * [6 Licence](#6-License)
@@ -93,15 +94,16 @@
 git clone https://github.com/SainsburyWellcomeCentre/NeuralPlayground/
 cd NeuralPlayground
 pip install -e '.[dev]'
 ```
 
 ## 3. Project
 
-Try our package! We are gathering opinions to focus our efforts on improving aspects of the code or adding new features, so if you tell us what you would like to have, we might just implement it ;) Please refer to the [Roadmap](https://github.com/ClementineDomine/NeuralPlayground/blob/main/documents/road_map.md) to understand the state of the project and get an idea of the direction it is going in. This open-source software was built to be collaborative and lasting. We hope that the framework will be simple enough to be adopted by a great number of neuroscientists, eventually guiding the path to the computational understanding of the HEC mechanisms. We follow reproducible, inclusive, and collaborative project design guidelines. All relevant documents can be found in [Documents](https://github.com/ClementineDomine/NeuralPlayground/blob/main/documents/).
+Try our package! We are gathering opinions to focus our efforts on improving aspects of the code or adding new features, so if you tell us what you would like to have, we might just implement it 😊.
+Please refer to the [Roadmap](https://github.com/ClementineDomine/NeuralPlayground/blob/main/documents/road_map.md) to understand the state of the project and get an idea of the direction it is going in. This open-source software was built to be collaborative and lasting. We hope that the framework will be simple enough to be adopted by a great number of neuroscientists, eventually guiding the path to the computational understanding of the HEC mechanisms. We follow reproducible, inclusive, and collaborative project design guidelines. All relevant documents can be found in [Documents](https://github.com/ClementineDomine/NeuralPlayground/blob/main/documents/).
 
 #### How to run a single module
 
 Each module can be used separately to easily explore and analyze experimental data and better understand any implemented model. Additionally, different Arenas can be initialised with artificial architectures or with data from real-life experiments. We provide examples of module instantiation in the detailed jupyter notebooks found in [Examples_experiment](https://github.com/ClementineDomine/NeuralPlayground/tree/main/examples/experimental_examples), [Examples_arena](https://github.com/ClementineDomine/NeuralPlayground/tree/main/examples/arena_examples) and [Examples_agents](https://github.com/ClementineDomine/NeuralPlayground/tree/main/examples/agent_examples).
 
 #### How to run interactions between modules
 
@@ -158,17 +160,21 @@
   <tbody>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/ClementineDomine"><img src="https://avatars.githubusercontent.com/u/18595111?v=4?s=100" width="100px;" alt="Clementine Domine"/><br /><sub><b>Clementine Domine</b></sub></a><br /><a href="#design-ClementineDomine" title="Design">🎨</a> <a href="#mentoring-ClementineDomine" title="Mentoring">🧑‍🏫</a> <a href="https://github.com/SainsburyWellcomeCentre/NeuralPlayground/commits?author=ClementineDomine" title="Code">💻</a> <a href="#data-ClementineDomine" title="Data">🔣</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/rodrigcd"><img src="https://avatars.githubusercontent.com/u/22643681?v=4?s=100" width="100px;" alt="rodrigcd"/><br /><sub><b>rodrigcd</b></sub></a><br /><a href="#design-rodrigcd" title="Design">🎨</a> <a href="#mentoring-rodrigcd" title="Mentoring">🧑‍🏫</a> <a href="https://github.com/SainsburyWellcomeCentre/NeuralPlayground/commits?author=rodrigcd" title="Code">💻</a> <a href="#data-rodrigcd" title="Data">🔣</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/LukeHollingsworth"><img src="https://avatars.githubusercontent.com/u/93782020?v=4?s=100" width="100px;" alt="Luke Hollingsworth"/><br /><sub><b>Luke Hollingsworth</b></sub></a><br /><a href="https://github.com/SainsburyWellcomeCentre/NeuralPlayground/commits?author=LukeHollingsworth" title="Documentation">📖</a> <a href="https://github.com/SainsburyWellcomeCentre/NeuralPlayground/commits?author=LukeHollingsworth" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://saxelab.org"><img src="https://avatars.githubusercontent.com/u/4165949?v=4?s=100" width="100px;" alt="Andrew Saxe"/><br /><sub><b>Andrew Saxe</b></sub></a><br /><a href="#mentoring-asaxe" title="Mentoring">🧑‍🏫</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/DrCaswellBarry"><img src="https://avatars.githubusercontent.com/u/17472149?v=4?s=100" width="100px;" alt="DrCaswellBarry"/><br /><sub><b>DrCaswellBarry</b></sub></a><br /><a href="#mentoring-DrCaswellBarry" title="Mentoring">🧑‍🏫</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="http://nikosirmpilatze.com"><img src="https://avatars.githubusercontent.com/u/20923448?v=4?s=100" width="100px;" alt="Niko Sirmpilatze"/><br /><sub><b>Niko Sirmpilatze</b></sub></a><br /><a href="#infra-niksirbi" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-niksirbi" title="Maintenance">🚧</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://nikosirmpilatze.com"><img src="https://avatars.githubusercontent.com/u/20923448?v=4?s=100" width="100px;" alt="Niko Sirmpilatze"/><br /><sub><b>Niko Sirmpilatze</b></sub></a><br /><a href="#infra-niksirbi" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-niksirbi" title="Maintenance">🚧</a> <a href="#tool-niksirbi" title="Tools">🔧</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://adamltyson.com"><img src="https://avatars.githubusercontent.com/u/13147259?v=4?s=100" width="100px;" alt="Adam Tyson"/><br /><sub><b>Adam Tyson</b></sub></a><br /><a href="#maintenance-adamltyson" title="Maintenance">🚧</a> <a href="#infra-adamltyson" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
     </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/rhayman"><img src="https://avatars.githubusercontent.com/u/5619644?v=4?s=100" width="100px;" alt="rhayman"/><br /><sub><b>rhayman</b></sub></a><br /><a href="https://github.com/SainsburyWellcomeCentre/NeuralPlayground/commits?author=rhayman" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/JarvisDevon"><img src="https://avatars.githubusercontent.com/u/30460455?v=4?s=100" width="100px;" alt="Devon Jarvis"/><br /><sub><b>Devon Jarvis</b></sub></a><br /><a href="https://github.com/SainsburyWellcomeCentre/NeuralPlayground/commits?author=JarvisDevon" title="Documentation">📖</a> <a href="https://github.com/SainsburyWellcomeCentre/NeuralPlayground/commits?author=JarvisDevon" title="Code">💻</a></td>
+    </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

### Comparing `NeuralPlayground-0.0.2/PKG-INFO` & `NeuralPlayground-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuralPlayground
-Version: 0.0.2
+Version: 0.0.3
 Summary: The standardised environment for the hippocampus and entorhinal cortex models
 Author: Clementine Domine
 Author-email: Rodrigo Carrasco-Davis <rodrigo.carrasco.davis@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/ClementineDomine/NeuralPlayground
 Project-URL: Bug tracker, https://github.com/ClementineDomine/NeuralPlayground/issues
 Project-URL: Documentation, https://github.com/ClementineDomine/NeuralPlayground
@@ -20,20 +20,21 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# NeuralPlayground: The  standardised environment for the hippocampus and entorhinal cortex models.
-<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-7-orange.svg?style=flat-square)](#contributors-)
-<!-- ALL-CONTRIBUTORS-BADGE:END -->
 
+# NeuralPlayground: The  standardised environment for the hippocampus and entorhinal cortex models. 
+### (Developing visualization and comparison board)
 
+<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
+[![All Contributors](https://img.shields.io/badge/all_contributors-9-orange.svg?style=flat-square)](#contributors-)
+<!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 * [1 Introduction](#1-Introduction)
 * [2 Installation ](#2-Installation)
 * [3 The Project](#3-Project)
 * [4 How to Contribute](#4-I-want-to-Contribute)
 * [5 Cite ](#5-Cite)
 * [6 Licence](#6-License)
@@ -93,15 +94,16 @@
 git clone https://github.com/SainsburyWellcomeCentre/NeuralPlayground/
 cd NeuralPlayground
 pip install -e '.[dev]'
 ```
 
 ## 3. Project
 
-Try our package! We are gathering opinions to focus our efforts on improving aspects of the code or adding new features, so if you tell us what you would like to have, we might just implement it ;) Please refer to the [Roadmap](https://github.com/ClementineDomine/NeuralPlayground/blob/main/documents/road_map.md) to understand the state of the project and get an idea of the direction it is going in. This open-source software was built to be collaborative and lasting. We hope that the framework will be simple enough to be adopted by a great number of neuroscientists, eventually guiding the path to the computational understanding of the HEC mechanisms. We follow reproducible, inclusive, and collaborative project design guidelines. All relevant documents can be found in [Documents](https://github.com/ClementineDomine/NeuralPlayground/blob/main/documents/).
+Try our package! We are gathering opinions to focus our efforts on improving aspects of the code or adding new features, so if you tell us what you would like to have, we might just implement it 😊.
+Please refer to the [Roadmap](https://github.com/ClementineDomine/NeuralPlayground/blob/main/documents/road_map.md) to understand the state of the project and get an idea of the direction it is going in. This open-source software was built to be collaborative and lasting. We hope that the framework will be simple enough to be adopted by a great number of neuroscientists, eventually guiding the path to the computational understanding of the HEC mechanisms. We follow reproducible, inclusive, and collaborative project design guidelines. All relevant documents can be found in [Documents](https://github.com/ClementineDomine/NeuralPlayground/blob/main/documents/).
 
 #### How to run a single module
 
 Each module can be used separately to easily explore and analyze experimental data and better understand any implemented model. Additionally, different Arenas can be initialised with artificial architectures or with data from real-life experiments. We provide examples of module instantiation in the detailed jupyter notebooks found in [Examples_experiment](https://github.com/ClementineDomine/NeuralPlayground/tree/main/examples/experimental_examples), [Examples_arena](https://github.com/ClementineDomine/NeuralPlayground/tree/main/examples/arena_examples) and [Examples_agents](https://github.com/ClementineDomine/NeuralPlayground/tree/main/examples/agent_examples).
 
 #### How to run interactions between modules
 
@@ -158,17 +160,21 @@
   <tbody>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/ClementineDomine"><img src="https://avatars.githubusercontent.com/u/18595111?v=4?s=100" width="100px;" alt="Clementine Domine"/><br /><sub><b>Clementine Domine</b></sub></a><br /><a href="#design-ClementineDomine" title="Design">🎨</a> <a href="#mentoring-ClementineDomine" title="Mentoring">🧑‍🏫</a> <a href="https://github.com/SainsburyWellcomeCentre/NeuralPlayground/commits?author=ClementineDomine" title="Code">💻</a> <a href="#data-ClementineDomine" title="Data">🔣</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/rodrigcd"><img src="https://avatars.githubusercontent.com/u/22643681?v=4?s=100" width="100px;" alt="rodrigcd"/><br /><sub><b>rodrigcd</b></sub></a><br /><a href="#design-rodrigcd" title="Design">🎨</a> <a href="#mentoring-rodrigcd" title="Mentoring">🧑‍🏫</a> <a href="https://github.com/SainsburyWellcomeCentre/NeuralPlayground/commits?author=rodrigcd" title="Code">💻</a> <a href="#data-rodrigcd" title="Data">🔣</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/LukeHollingsworth"><img src="https://avatars.githubusercontent.com/u/93782020?v=4?s=100" width="100px;" alt="Luke Hollingsworth"/><br /><sub><b>Luke Hollingsworth</b></sub></a><br /><a href="https://github.com/SainsburyWellcomeCentre/NeuralPlayground/commits?author=LukeHollingsworth" title="Documentation">📖</a> <a href="https://github.com/SainsburyWellcomeCentre/NeuralPlayground/commits?author=LukeHollingsworth" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://saxelab.org"><img src="https://avatars.githubusercontent.com/u/4165949?v=4?s=100" width="100px;" alt="Andrew Saxe"/><br /><sub><b>Andrew Saxe</b></sub></a><br /><a href="#mentoring-asaxe" title="Mentoring">🧑‍🏫</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/DrCaswellBarry"><img src="https://avatars.githubusercontent.com/u/17472149?v=4?s=100" width="100px;" alt="DrCaswellBarry"/><br /><sub><b>DrCaswellBarry</b></sub></a><br /><a href="#mentoring-DrCaswellBarry" title="Mentoring">🧑‍🏫</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="http://nikosirmpilatze.com"><img src="https://avatars.githubusercontent.com/u/20923448?v=4?s=100" width="100px;" alt="Niko Sirmpilatze"/><br /><sub><b>Niko Sirmpilatze</b></sub></a><br /><a href="#infra-niksirbi" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-niksirbi" title="Maintenance">🚧</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://nikosirmpilatze.com"><img src="https://avatars.githubusercontent.com/u/20923448?v=4?s=100" width="100px;" alt="Niko Sirmpilatze"/><br /><sub><b>Niko Sirmpilatze</b></sub></a><br /><a href="#infra-niksirbi" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-niksirbi" title="Maintenance">🚧</a> <a href="#tool-niksirbi" title="Tools">🔧</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://adamltyson.com"><img src="https://avatars.githubusercontent.com/u/13147259?v=4?s=100" width="100px;" alt="Adam Tyson"/><br /><sub><b>Adam Tyson</b></sub></a><br /><a href="#maintenance-adamltyson" title="Maintenance">🚧</a> <a href="#infra-adamltyson" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
     </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/rhayman"><img src="https://avatars.githubusercontent.com/u/5619644?v=4?s=100" width="100px;" alt="rhayman"/><br /><sub><b>rhayman</b></sub></a><br /><a href="https://github.com/SainsburyWellcomeCentre/NeuralPlayground/commits?author=rhayman" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/JarvisDevon"><img src="https://avatars.githubusercontent.com/u/30460455?v=4?s=100" width="100px;" alt="Devon Jarvis"/><br /><sub><b>Devon Jarvis</b></sub></a><br /><a href="https://github.com/SainsburyWellcomeCentre/NeuralPlayground/commits?author=JarvisDevon" title="Documentation">📖</a> <a href="https://github.com/SainsburyWellcomeCentre/NeuralPlayground/commits?author=JarvisDevon" title="Code">💻</a></td>
+    </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

### Comparing `NeuralPlayground-0.0.2/README.md` & `NeuralPlayground-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-# NeuralPlayground: The  standardised environment for the hippocampus and entorhinal cortex models.
-<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-7-orange.svg?style=flat-square)](#contributors-)
-<!-- ALL-CONTRIBUTORS-BADGE:END -->
 
+# NeuralPlayground: The  standardised environment for the hippocampus and entorhinal cortex models. 
+### (Developing visualization and comparison board)
 
+<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
+[![All Contributors](https://img.shields.io/badge/all_contributors-9-orange.svg?style=flat-square)](#contributors-)
+<!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 * [1 Introduction](#1-Introduction)
 * [2 Installation ](#2-Installation)
 * [3 The Project](#3-Project)
 * [4 How to Contribute](#4-I-want-to-Contribute)
 * [5 Cite ](#5-Cite)
 * [6 Licence](#6-License)
@@ -67,15 +68,16 @@
 git clone https://github.com/SainsburyWellcomeCentre/NeuralPlayground/
 cd NeuralPlayground
 pip install -e '.[dev]'
 ```
 
 ## 3. Project
 
-Try our package! We are gathering opinions to focus our efforts on improving aspects of the code or adding new features, so if you tell us what you would like to have, we might just implement it ;) Please refer to the [Roadmap](https://github.com/ClementineDomine/NeuralPlayground/blob/main/documents/road_map.md) to understand the state of the project and get an idea of the direction it is going in. This open-source software was built to be collaborative and lasting. We hope that the framework will be simple enough to be adopted by a great number of neuroscientists, eventually guiding the path to the computational understanding of the HEC mechanisms. We follow reproducible, inclusive, and collaborative project design guidelines. All relevant documents can be found in [Documents](https://github.com/ClementineDomine/NeuralPlayground/blob/main/documents/).
+Try our package! We are gathering opinions to focus our efforts on improving aspects of the code or adding new features, so if you tell us what you would like to have, we might just implement it 😊.
+Please refer to the [Roadmap](https://github.com/ClementineDomine/NeuralPlayground/blob/main/documents/road_map.md) to understand the state of the project and get an idea of the direction it is going in. This open-source software was built to be collaborative and lasting. We hope that the framework will be simple enough to be adopted by a great number of neuroscientists, eventually guiding the path to the computational understanding of the HEC mechanisms. We follow reproducible, inclusive, and collaborative project design guidelines. All relevant documents can be found in [Documents](https://github.com/ClementineDomine/NeuralPlayground/blob/main/documents/).
 
 #### How to run a single module
 
 Each module can be used separately to easily explore and analyze experimental data and better understand any implemented model. Additionally, different Arenas can be initialised with artificial architectures or with data from real-life experiments. We provide examples of module instantiation in the detailed jupyter notebooks found in [Examples_experiment](https://github.com/ClementineDomine/NeuralPlayground/tree/main/examples/experimental_examples), [Examples_arena](https://github.com/ClementineDomine/NeuralPlayground/tree/main/examples/arena_examples) and [Examples_agents](https://github.com/ClementineDomine/NeuralPlayground/tree/main/examples/agent_examples).
 
 #### How to run interactions between modules
 
@@ -132,17 +134,21 @@
   <tbody>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/ClementineDomine"><img src="https://avatars.githubusercontent.com/u/18595111?v=4?s=100" width="100px;" alt="Clementine Domine"/><br /><sub><b>Clementine Domine</b></sub></a><br /><a href="#design-ClementineDomine" title="Design">🎨</a> <a href="#mentoring-ClementineDomine" title="Mentoring">🧑‍🏫</a> <a href="https://github.com/SainsburyWellcomeCentre/NeuralPlayground/commits?author=ClementineDomine" title="Code">💻</a> <a href="#data-ClementineDomine" title="Data">🔣</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/rodrigcd"><img src="https://avatars.githubusercontent.com/u/22643681?v=4?s=100" width="100px;" alt="rodrigcd"/><br /><sub><b>rodrigcd</b></sub></a><br /><a href="#design-rodrigcd" title="Design">🎨</a> <a href="#mentoring-rodrigcd" title="Mentoring">🧑‍🏫</a> <a href="https://github.com/SainsburyWellcomeCentre/NeuralPlayground/commits?author=rodrigcd" title="Code">💻</a> <a href="#data-rodrigcd" title="Data">🔣</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/LukeHollingsworth"><img src="https://avatars.githubusercontent.com/u/93782020?v=4?s=100" width="100px;" alt="Luke Hollingsworth"/><br /><sub><b>Luke Hollingsworth</b></sub></a><br /><a href="https://github.com/SainsburyWellcomeCentre/NeuralPlayground/commits?author=LukeHollingsworth" title="Documentation">📖</a> <a href="https://github.com/SainsburyWellcomeCentre/NeuralPlayground/commits?author=LukeHollingsworth" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://saxelab.org"><img src="https://avatars.githubusercontent.com/u/4165949?v=4?s=100" width="100px;" alt="Andrew Saxe"/><br /><sub><b>Andrew Saxe</b></sub></a><br /><a href="#mentoring-asaxe" title="Mentoring">🧑‍🏫</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/DrCaswellBarry"><img src="https://avatars.githubusercontent.com/u/17472149?v=4?s=100" width="100px;" alt="DrCaswellBarry"/><br /><sub><b>DrCaswellBarry</b></sub></a><br /><a href="#mentoring-DrCaswellBarry" title="Mentoring">🧑‍🏫</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="http://nikosirmpilatze.com"><img src="https://avatars.githubusercontent.com/u/20923448?v=4?s=100" width="100px;" alt="Niko Sirmpilatze"/><br /><sub><b>Niko Sirmpilatze</b></sub></a><br /><a href="#infra-niksirbi" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-niksirbi" title="Maintenance">🚧</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://nikosirmpilatze.com"><img src="https://avatars.githubusercontent.com/u/20923448?v=4?s=100" width="100px;" alt="Niko Sirmpilatze"/><br /><sub><b>Niko Sirmpilatze</b></sub></a><br /><a href="#infra-niksirbi" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-niksirbi" title="Maintenance">🚧</a> <a href="#tool-niksirbi" title="Tools">🔧</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://adamltyson.com"><img src="https://avatars.githubusercontent.com/u/13147259?v=4?s=100" width="100px;" alt="Adam Tyson"/><br /><sub><b>Adam Tyson</b></sub></a><br /><a href="#maintenance-adamltyson" title="Maintenance">🚧</a> <a href="#infra-adamltyson" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
     </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/rhayman"><img src="https://avatars.githubusercontent.com/u/5619644?v=4?s=100" width="100px;" alt="rhayman"/><br /><sub><b>rhayman</b></sub></a><br /><a href="https://github.com/SainsburyWellcomeCentre/NeuralPlayground/commits?author=rhayman" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/JarvisDevon"><img src="https://avatars.githubusercontent.com/u/30460455?v=4?s=100" width="100px;" alt="Devon Jarvis"/><br /><sub><b>Devon Jarvis</b></sub></a><br /><a href="https://github.com/SainsburyWellcomeCentre/NeuralPlayground/commits?author=JarvisDevon" title="Documentation">📖</a> <a href="https://github.com/SainsburyWellcomeCentre/NeuralPlayground/commits?author=JarvisDevon" title="Code">💻</a></td>
+    </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

#### html2text {}

```diff
@@ -1,39 +1,40 @@
-# NeuralPlayground: The standardised environment for the hippocampus and
-entorhinal cortex models.  [![All Contributors](https://img.shields.io/badge/
-all_contributors-7-orange.svg?style=flat-square)](#contributors-)  * [1
-Introduction](#1-Introduction) * [2 Installation ](#2-Installation) * [3 The
-Project](#3-Project) * [4 How to Contribute](#4-I-want-to-Contribute) * [5 Cite
-](#5-Cite) * [6 Licence](#6-License) ## 1. Introduction The abstract
-representation of space has been extensively studied in the hippocampus and
-entorhinal cortex in part due to the easy monitoring of the task and neural
-recording. A growing variety of theoretical models have been proposed to
-capture the rich neural and behavioral phenomena associated with these
-circuits. However, objective comparison of these theories against each other
-and against empirical data is difficult. Although the significance of virtuous
-interaction between experiments and theory is widely recognized, the tools
-available to facilitate comparison are limited. Some important challenge to
-standardized coparaison are the 1. Lack availability and accessibility of data
-in a standardized, labeled format. 2. Lack of standard or easy ways for models
-to interact with the task. 3. Lack of standard or easy ways to compare model
-output with empirical data. To address this gap, we present an open-source
-standardised software framework - NeuralPlayground - to enable adjudication
-between the hippocampus and entorhinal cortex models. This Python software
-package offers a reproducible way to compare models against a centralised
-library of published experimental results, including neural recordings and
-animal behavior. The framework currently contains implementations of three
-Agents, as well as three Experiments providing simple interfaces to publicly
-available neural and behavioral data. It also contains a customizable 2-
-dimensional Arena (continuous and discrete) able to produce common experimental
-environments in which the agents can move in and interact with. We note that
-each module can also be used separately, allowing flexible access to
-influential models and data sets. We currently rely on visual comparison of a
-hand-selected number of outputs of the model with neural recordings as shown in
-[github.com/NeuralPlayground/examples/comparison](https://github.com/
-ClementineDomine/NeuralPlayground/blob/main/examples/comparison_board_examples/
+ # NeuralPlayground: The standardised environment for the hippocampus and
+entorhinal cortex models. ### (Developing visualization and comparison board)
+[![All Contributors](https://img.shields.io/badge/all_contributors-9-
+orange.svg?style=flat-square)](#contributors-)  * [1 Introduction](#1-
+Introduction) * [2 Installation ](#2-Installation) * [3 The Project](#3-
+Project) * [4 How to Contribute](#4-I-want-to-Contribute) * [5 Cite ](#5-Cite)
+* [6 Licence](#6-License) ## 1. Introduction The abstract representation of
+space has been extensively studied in the hippocampus and entorhinal cortex in
+part due to the easy monitoring of the task and neural recording. A growing
+variety of theoretical models have been proposed to capture the rich neural and
+behavioral phenomena associated with these circuits. However, objective
+comparison of these theories against each other and against empirical data is
+difficult. Although the significance of virtuous interaction between
+experiments and theory is widely recognized, the tools available to facilitate
+comparison are limited. Some important challenge to standardized coparaison are
+the 1. Lack availability and accessibility of data in a standardized, labeled
+format. 2. Lack of standard or easy ways for models to interact with the task.
+3. Lack of standard or easy ways to compare model output with empirical data.
+To address this gap, we present an open-source standardised software framework
+- NeuralPlayground - to enable adjudication between the hippocampus and
+entorhinal cortex models. This Python software package offers a reproducible
+way to compare models against a centralised library of published experimental
+results, including neural recordings and animal behavior. The framework
+currently contains implementations of three Agents, as well as three
+Experiments providing simple interfaces to publicly available neural and
+behavioral data. It also contains a customizable 2-dimensional Arena
+(continuous and discrete) able to produce common experimental environments in
+which the agents can move in and interact with. We note that each module can
+also be used separately, allowing flexible access to influential models and
+data sets. We currently rely on visual comparison of a hand-selected number of
+outputs of the model with neural recordings as shown in [github.com/
+NeuralPlayground/examples/comparison](https://github.com/ClementineDomine/
+NeuralPlayground/blob/main/examples/comparison_board_examples/
 comparison_board.ipynb). In the future, a set of quantitative measures and
 qualitative measures will be added for systematic comparisonsk from any Agent,
 Arena, Experiments.We want to restate that this wonât constitute an objective
 judgment of the quality of an Agent to replicate the brain mechanism. Instead,
 this only allows an objective and complete comparison to the current evidence
 in the field, as is typically done in publications. Altogether, we hope our
 framework, available at [github.com/NeuralPlayground](https://github.com/
@@ -51,15 +52,15 @@
 NeuralPlayground==0.0.1 ``` ### Install for development If you want to
 contribute to the project, get the latest development version from GitHub, and
 install it in editable mode, including the "dev" dependencies: ```bash git
 clone https://github.com/SainsburyWellcomeCentre/NeuralPlayground/ cd
 NeuralPlayground pip install -e '.[dev]' ``` ## 3. Project Try our package! We
 are gathering opinions to focus our efforts on improving aspects of the code or
 adding new features, so if you tell us what you would like to have, we might
-just implement it ;) Please refer to the [Roadmap](https://github.com/
+just implement it ð. Please refer to the [Roadmap](https://github.com/
 ClementineDomine/NeuralPlayground/blob/main/documents/road_map.md) to
 understand the state of the project and get an idea of the direction it is
 going in. This open-source software was built to be collaborative and lasting.
 We hope that the framework will be simple enough to be adopted by a great
 number of neuroscientists, eventually guiding the path to the computational
 understanding of the HEC mechanisms. We follow reproducible, inclusive, and
 collaborative project design guidelines. All relevant documents can be found in
@@ -107,15 +108,18 @@
 the modules for further details on how to contribute to them. ## 5. Cite See
 [Citation](https://github.com/ClementineDomine/NeuralPlayground/blob/main/
 documents/citation.cff) for the correct citation of this framework. ## 6.
 License More details about the license can be found at [Licence](https://
 github.com/ClementineDomine/NeuralPlayground/blob/main/documents/lisence.md).
 ## Contributors â¨ Thanks goes to these wonderful people ([emoji key](https://
 allcontributors.org/docs/en/emoji-key)):
-               [Clementine_Domine]                                   [rodrigcd]                           [Luke           [Andrew_Saxe]         [DrCaswellBarry]          [Niko         [Adam_Tyson]
-                Clementine_Domine                                     rodrigcd                       Hollingsworth]        Andrew_Saxe           DrCaswellBarry       Sirmpilatze]       Adam_Tyson
-           ð¨ ð§âð« ð�           ð¨ ð§âð« ð�      Luke             ð§âð     ð§âðNiko_Sirmpilatze      ð§ ð
-                                                                                                      Hollingsworth                                                     ð ð§
+               [Clementine_Domine]                                   [rodrigcd]                           [Luke           [Andrew_Saxe]         [DrCaswellBarry]        [Niko_Sirmpilatze]       [Adam_Tyson]
+                Clementine_Domine                                     rodrigcd                       Hollingsworth]        Andrew_Saxe           DrCaswellBarry          Niko_Sirmpilatze         Adam_Tyson
+           ð¨ ð§âð« ð�           ð¨ ð§âð« ð�      Luke             ð§âð     ð§âð      ð ð§ ð�    ð§ ð
+                                                                                                      Hollingsworth
                                                                                                         ð ð»
+                             [rhayman]                                   [Devon_Jarvis]
+                              rhayman                                     Devon_Jarvis
+                               ð»                                     ð ð»
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind are
 welcome!
```

### Comparing `NeuralPlayground-0.0.2/documents/citation.cff` & `NeuralPlayground-0.0.3/documents/citation.cff`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.2/documents/code_of_conduct.md` & `NeuralPlayground-0.0.3/documents/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.2/documents/contributors.md` & `NeuralPlayground-0.0.3/documents/contributors.md`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.2/documents/licence.md` & `NeuralPlayground-0.0.3/documents/licence.md`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.2/documents/road_map.md` & `NeuralPlayground-0.0.3/documents/road_map.md`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.2/neuralplayground/agents/README.md` & `NeuralPlayground-0.0.3/neuralplayground/agents/README.md`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.2/neuralplayground/agents/agent_core.py` & `NeuralPlayground-0.0.3/neuralplayground/agents/agent_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,18 +41,14 @@
         self.obs_history = []
         self.global_steps = 0
 
     def reset(self):
         """Erase all memory from the model, initialize all relevant parameters and build from scratch"""
         pass
 
-    def neural_response(self):
-        """Function that returns some representation that will be compared against real experimental data"""
-        pass
-
     def act(self, obs, policy_func=None):
         """
         The base model executes a random action from a normal distribution
         Parameters
         ----------
         obs
             Observation from the environment class needed to choose the right action
@@ -60,18 +56,18 @@
             Arbitrary function that represents a custom policy that receives and observation and gives an action
         Returns
         -------
         action: float
             action value which in this case is random number draw from a Gaussian
         """
         self.obs_history.append(obs)
-        # if len(self.obs_history) >= 1000:  # reset every 1000
-        self.obs_history = [
-            obs,
-        ]
+        if len(self.obs_history) >= 1000:  # reset every 1000
+            self.obs_history = [
+                obs,
+            ]
         if policy_func is not None:
             return policy_func(obs)
         action = np.random.normal(scale=self.agent_step_size, size=(2,))
         return action
 
     def update(self):
         pass
@@ -80,33 +76,40 @@
         """Save current state and information in general to re-instantiate the environment
 
         Parameters
         ----------
         save_path: str
             Path to save the agent
         """
-        pickle.dump(self.__dict__, open(os.path.join(save_path), "wb"), pickle.HIGHEST_PROTOCOL)
+        # pickle.dump(self.__dict__, open(os.path.join(save_path), "wb"), pickle.HIGHEST_PROTOCOL)
+        pickle.dump(self, open(os.path.join(save_path), "wb"), pickle.HIGHEST_PROTOCOL)
 
     def restore_agent(self, save_path: str):
         """Restore saved environment
 
         Parameters
         ----------
         save_path: str
             Path to retrieve the agent
         """
-        self.__dict__ = pd.read_pickle(save_path)
+        # self.__dict__ = pd.read_pickle(save_path)
+        # TODO: for some reason, ruff has a problem with this: self = pd.read_pickle(save_path)
+        pd.read_pickle(save_path)
 
     def __eq__(self, other):
         diff = DeepDiff(self.__dict__, other.__dict__)
         if len(diff) == 0:
             return True
         else:
             return False
 
+    def get_ratemap_matrix(self):
+        """Function that returns some representation that will be compared against real experimental data"""
+        pass
+
 
 class RandomAgent(AgentCore):
     """Simple agent with random trajectories"""
 
     def __init__(self, step_size: float = 1.0):
         """Initialization
```

### Comparing `NeuralPlayground-0.0.2/neuralplayground/agents/stachenfeld_2018.py` & `NeuralPlayground-0.0.3/neuralplayground/agents/stachenfeld_2018.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,20 +3,24 @@
 The hippocampus as a predictive map
 https://doi.org/10.1101/097170;
 
 This implementation can interact with environments from the package as shown in the examples jupyter notebook.
 Check examples/Stachenfeld_2018_example.ipynb
 """
 
+import random
 import sys
+from typing import Union
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 
+from neuralplayground.plotting.plot_utils import make_plot_rate_map
+
 from .agent_core import AgentCore
 
 sys.path.append("../")
 
 
 class Stachenfeld2018(AgentCore):
     """
@@ -110,45 +114,44 @@
         super().__init__(model_name, **mod_kwargs)
         self.metadata = {"mod_kwargs": mod_kwargs}
         self.obs_history = []  # Initialize observation history to update weights later
         self.grad_history = []
         self.gamma = mod_kwargs["discount"]
         self.threshold = mod_kwargs["threshold"]
         self.learning_rate = mod_kwargs["lr_td"]
-        self.t_episode = mod_kwargs["t_episode"]
-        self.n_episode = mod_kwargs["n_episode"]
         self.room_width = mod_kwargs["room_width"]
         self.room_depth = mod_kwargs["room_depth"]
         self.state_density = mod_kwargs["state_density"]
         twoD = mod_kwargs["twoD"]
         self.inital_obs_variable = None
 
         self.reset()
         # Variables for the SR-agent state space
-        self.resolution_d = int(self.state_density * self.room_depth)
-        self.resolution_w = int(self.state_density * self.room_width)
-        self.x_array = np.linspace(-self.room_width / 2, self.room_width / 2, num=self.resolution_d)
-        self.y_array = np.linspace(self.room_depth / 2, -self.room_depth / 2, num=self.resolution_w)
+        self.resolution_depth = int(self.state_density * self.room_depth)
+        self.resolution_width = int(self.state_density * self.room_width)
+        self.x_array = np.linspace(-self.room_width / 2, self.room_width / 2, num=self.resolution_width)
+        self.y_array = np.linspace(self.room_depth / 2, -self.room_depth / 2, num=self.resolution_depth)
         self.mesh = np.array(np.meshgrid(self.x_array, self.y_array))
         self.xy_combinations = self.mesh.T.reshape(-1, 2)
-        self.w = int(self.room_width * self.state_density)
-        self.l = int(self.room_depth * self.state_density)
-        self.n_state = int(self.l * self.w)
+        self.width = int(self.room_width * self.state_density)
+        self.depth = int(self.room_depth * self.state_density)
+        self.n_state = int(self.depth * self.width)
         self.obs_history = []
         if twoD:
             self.create_transmat(self.state_density, "2D_env")
 
     def reset(self):
         """
         Initialize the successor matrices, normalized transition matrix and observation variables (history and initialisation)
         """
 
         self.srmat = []
         self.srmat_sum = []
         self.srmat_ground = []
+        self.srmat_full_td = []
         self.transmat_norm = []
         self.inital_obs_variable = None
         self.obs_history = []  # Reset observation history
 
     def obs_to_state(self, pos: np.ndarray):
         """
         Converts the agent's position in the environment to the agent's position in the SR-agent state space.
@@ -161,15 +164,15 @@
         Returns
         -------
         curr_state: int
             integer corresponding to the position in the SR-agent state space
 
 
         """
-        np.arange(self.n_state).reshape(self.l, self.w)
+        np.arange(self.n_state).reshape(self.depth, self.width)
 
         diff = self.xy_combinations - pos[np.newaxis, ...]
         dist = np.sum(diff**2, axis=1)
         index = np.argmin(dist)
         curr_state = index
         return curr_state
 
@@ -236,30 +239,30 @@
             transmat_norm: array (n_state,n_state)
                 Normalised transition matrix
 
         """
 
         if name_env == "2D_env":
             adjmat_triu = np.zeros((self.n_state, self.n_state))
-            node_layout = np.arange(self.n_state).reshape(self.l, self.w)
-            np.linspace(0, np.min([self.l / self.w, 1]), num=self.l)
-            np.linspace(0, np.min([self.w / self.l, 1]), num=self.w)
+            node_layout = np.arange(self.n_state).reshape(self.depth, self.width)
+            np.linspace(0, np.min([self.depth / self.width, 1]), num=self.depth)
+            np.linspace(0, np.min([self.width / self.depth, 1]), num=self.width)
             self.xy = []
 
-            for i in range(self.l):
-                for j in range(self.w):
+            for i in range(self.depth):
+                for j in range(self.width):
                     s = node_layout[i, j]
                     neighbours = []
                     if i - 1 >= 0:
                         neighbours.append(node_layout[i - 1, j])
-                    if i + 1 < self.l:
+                    if i + 1 < self.depth:
                         neighbours.append(node_layout[i + 1, j])
                     if j - 1 >= 0:
                         neighbours.append(node_layout[i, j - 1])
-                    if j + 1 < self.w:
+                    if j + 1 < self.width:
                         neighbours.append(node_layout[i, j + 1])
                     adjmat_triu[s, neighbours] = 1
 
             transmat = adjmat_triu + adjmat_triu.T
             transmat = np.array(transmat, dtype=np.float64)
             row_sums = np.sum(transmat, axis=1)
             row_sums[row_sums == 0] = 1
@@ -270,17 +273,17 @@
 
         if plotting_variable is True:
             f, ax = plt.subplots(1, 1, figsize=(14, 5))
             ax.imshow(self.transmat_norm, interpolation="nearest", cmap="jet")
 
         return self.transmat_norm
 
-    def update_successor_rep(self):
+    def successor_rep_solution(self):
         """
-        Compute the successor representation matrix using geometric sums.
+        Compute closed form solution of successor representation matrix using geometric sums.
 
         Returns:
         -------
             srmat_ground: (n_state, n_state) numpy array,
                 Successor representation matrix
         """
         transmat_type = np.array(self.transmat_norm, dtype=np.float64)
@@ -325,104 +328,112 @@
         self.n_state = self.transmat_norm.shape[0]
         a = np.array(self.curr_state)
         x = a.flatten()
         b = np.eye(self.n_state)[x, : self.n_state]
         L = b.reshape(a.shape + (self.n_state,))
         curr_state_vec = L
 
-        update_val = curr_state_vec + self.gamma * self.srmat[:, next_state] - self.srmat[:, self.curr_state]
-        self.srmat[:, self.curr_state] = self.srmat[:, self.curr_state] + self.learning_rate * update_val
+        td_error = curr_state_vec + self.gamma * self.srmat[:, next_state] - self.srmat[:, self.curr_state]
+        self.srmat[:, self.curr_state] = self.srmat[:, self.curr_state] + self.learning_rate * td_error
 
-        self.grad_history.append(np.sqrt(np.sum(update_val**2)))
+        self.grad_history.append(np.sqrt(np.sum(td_error**2)))
         self.curr_state = next_state
 
-        return self.srmat
+        return {"state_td_error": td_error}
 
-    def update_successor_rep_td_full(self):
+    def update_successor_rep_td_full(self, n_episode: int = 100, t_episode: int = 100):
         """
         Compute the successor representation matrix using TD learning
 
         Returns:
         ----------
             srmat_full: (n_state, n_state)
                 successor representation matrix
 
         """
         random_state = np.random.RandomState(1234)
-
         t_elapsed = 0
         srmat0 = np.eye(self.n_state)
         srmat_full = srmat0.copy()
-        for i in range(self.n_episode):
+        for i in range(n_episode):
             curr_state = random_state.randint(self.n_state)
-            for j in range(self.t_episode):
+            for j in range(t_episode):
                 a = np.array([curr_state])
                 x = a.flatten()
                 b = np.eye(self.n_state)[x, : self.n_state]
                 L = b.reshape(a.shape + (self.n_state,))
-
                 curr_state_vec = L
                 random_state.multinomial(1, self.transmat_norm[curr_state, :])
                 next_state = np.where(random_state.multinomial(1, self.transmat_norm[curr_state, :]))[0][0]
 
                 srmat_full[:, curr_state] = srmat_full[:, curr_state] + self.learning_rate * (
                     curr_state_vec + self.gamma * srmat_full[:, next_state] - srmat_full[:, curr_state]
                 )
                 curr_state = next_state
                 t_elapsed += 1
+                self.srmat_full_td = srmat_full
+        return self.srmat_full_td
 
-        return srmat_full
+    def get_rate_map_matrix(
+        self,
+        sr_matrix=None,
+        eigen_vector: int = 10,
+    ):
+        if sr_matrix is None:
+            sr_matrix = self.successor_rep_solution()
+        evals, evecs = np.linalg.eig(sr_matrix)
+        r_out_im = evecs[:, eigen_vector].reshape((self.resolution_width, self.resolution_depth)).real
+        return r_out_im
 
-    def plot_transition(self, matrix: np.ndarray, save_path: str = None, ax: mpl.axes.Axes = None):
+    def plot_transition(self, save_path: str = None, ax: mpl.axes.Axes = None):
         """
         Plot the input matrix and compare it to the transition matrix from the rectangular
         environment states space (rectangular- transmat).
         (If a new state space type is added please update this function)
         Parameters
         ----------
         matrix: array
             The matrix that will be plotted
         save_path: string
             Path to save the plot
         """
-        evals, evecs = np.linalg.eig(matrix)
+        T = self.get_T_from_M(self.srmat)
         if ax is None:
             f, ax = plt.subplots(1, 2, figsize=(14, 5))
-            ax[0].imshow(self.transmat_norm, cmap="jet")
-            ax[1].imshow(matrix, cmap="jet")
+            make_plot_rate_map(self.transmat_norm, ax[0], "Transition matrix", "states", "states", "State occupency")
+            make_plot_rate_map(T, ax[1], "Transition calculated from SR matrix", "states", "states", "State occupency")
         if save_path is not None:
             plt.savefig(save_path, bbox_inches="tight")
             plt.close("all")
         return ax
 
-    def plot_eigen(self, matrix: np.ndarray, save_path: str, eigen=(0, 1), ax: mpl.axes.Axes = None):
-        """ "
-        Plot the matrix and the 4 largest modes of its eigen-decomposition
-
-        Parameters
-        ----------
-        matrix: array
-            The matrix that will be plotted
-        eigen:  np.ndarray
-            Which eigenvectors you would like to plot
-        save_path: string
-            Path to save the plot
-        """
-
-        evals, evecs = np.linalg.eig(matrix)
-
-        if ax is None:
-            f, ax = plt.subplots(1, len(eigen), figsize=(4 * len(eigen), 5))
-            if len(eigen) == 1:
-                evecs_0 = evecs[:, eigen[0]].reshape(self.l, self.w).real
-                im = ax.imshow(evecs_0, cmap="jet")
-                plt.colorbar(im, ax=ax)
-            else:
-                for i, eig in enumerate(eigen):
-                    evecs_0 = evecs[:, eig].reshape(self.l, self.w).real
-                    im = ax[i].imshow(evecs_0, cmap="jet")
-                plt.colorbar(im, ax=ax[i])
+    def plot_rate_map(
+        self,
+        sr_matrix=None,
+        eigen_vectors: Union[int, list, tuple] = None,
+        ax: mpl.axes.Axes = None,
+        save_path: str = None,
+    ):
+        if eigen_vectors is None:
+            eigen_vectors = random.randint(5, 19)
+
+        if isinstance(eigen_vectors, int):
+            rate_map_mat = self.get_rate_map_matrix(sr_matrix, eigen_vector=eigen_vectors)
+
+            if ax is None:
+                f, ax = plt.subplots(1, 1, figsize=(4, 5))
+            make_plot_rate_map(rate_map_mat, ax, "Rate map: Eig" + str(eigen_vectors), "width", "depth", "Firing rate")
+        else:
+            if ax is None:
+                f, ax = plt.subplots(1, len(eigen_vectors), figsize=(4 * len(eigen_vectors), 5))
+            if isinstance(ax, mpl.axes.Axes):
+                ax = [
+                    ax,
+                ]
+            for i, eig in enumerate(eigen_vectors):
+                rate_map_mat = self.get_rate_map_matrix(sr_matrix, eigen_vector=eig)
+                make_plot_rate_map(rate_map_mat, ax[i], "Rate map: " + "Eig" + str(eig), "width", "depth", "Firing rate")
         if save_path is None:
             pass
         else:
             plt.savefig(save_path, bbox_inches="tight")
-        return ax
+            return ax
```

### Comparing `NeuralPlayground-0.0.2/neuralplayground/agents/weber_2018.py` & `NeuralPlayground-0.0.3/neuralplayground/agents/weber_2018.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 from scipy.stats import multivariate_normal
 from tqdm import tqdm
 
+from neuralplayground.plotting.plot_utils import make_plot_rate_map
+
 from .agent_core import AgentCore
 
 
 class Weber2018(AgentCore):
     """
     Implementation for Weber and Sprekeler 2018
     Learning place cells, grid cells and invariances with excitatory and inhibitory plasticity
@@ -138,14 +140,18 @@
 
         self.sigma_exc = mod_kwargs["sigma_exc"]
         self.sigma_inh = mod_kwargs["sigma_inh"]
         if "resolution" in mod_kwargs.keys():
             self.resolution = mod_kwargs["resolution"]
         else:
             self.resolution = 50
+        if "disable_tqdm" in mod_kwargs.keys():
+            self.disable_tqdm = mod_kwargs["disable_tqdm"]
+        else:
+            self.disable_tqdm = False
 
         self.room_width, self.room_depth = (
             mod_kwargs["room_width"],
             mod_kwargs["room_depth"],
         )
         self.ro = mod_kwargs["ro"]
         self.obs_history = []  # Initialize observation history to update weights later
@@ -214,15 +220,15 @@
         cell_list: numpy ndarray
             n_curves x (self.resolution**2) with tuning curves for each neuron and each pixel in the 2D array
         """
         width_limit = self.room_width / 2.0
         depth_limit = self.room_depth / 2.0
         cell_list = []  # This will become a numpy array with the tuning curves in 2D (images)
         function_list = []  # List with parameters of each gaussian in the tuning curve
-        for i in tqdm(range(n_curves)):
+        for i in tqdm(range(n_curves), disable=self.disable_tqdm):
             gauss_list = []
             cell_i = 0
             for j in range(Nf):
                 # The +0.2 in the following is to avoid border effects
                 mean1 = np.random.uniform(-width_limit * (1 + 0.2), width_limit * (1 + 0.2))  # Sample means
                 mean2 = np.random.uniform(-depth_limit * (1 + 0.2), depth_limit * (1 + 0.2))
                 room_scale = np.max(np.array([self.room_width, self.room_width]))
@@ -326,14 +332,15 @@
         self.wi = self.wi + delta_wi
 
         if exc_normalization:
             self.we = self.init_we_sum / np.sqrt(np.sum(self.we**2)) * self.we
 
         self.we = np.clip(self.we, a_min=0, a_max=np.amax(self.we))  # Negative weights to zero
         self.wi = np.clip(self.wi, a_min=0, a_max=np.amax(self.wi))
+        return {"delta_we": delta_we, "delta_wi": delta_wi}
 
     def full_average_update(self, exc_normalization: bool = True):
         """
         Update weights using hebbian plasticity according to equation 2 for excitatory weights
         and equation 3 for inhibitory weights for all available positions in the grid
 
         Parameters
@@ -369,15 +376,53 @@
             True if excitatory weights are normalized after each update
         """
         random_permutation = np.arange(self.xy_combinations.shape[0])
         xy_array = self.xy_combinations[random_permutation, :]  # All points (x, y) in the grid
         for i in range(self.xy_combinations.shape[0]):
             self.update(exc_normalization=exc_normalization, pos=xy_array[i, :])
 
-    def plot_rates(self, save_path: str = None, ax: mpl.axes.Axes = None):
+    def get_rate_map_matrix(
+        self,
+    ):
+        """
+        Get the ratemap matrix of the network
+
+        Returns
+        -------
+        ratemap_matrix : ndarray
+            (self.resolution_width, self.resolution_depth) with the ratemap matrix
+        """
+        r_out_im = self.get_full_output_rate()
+        r_out_im = r_out_im.reshape((self.resolution_width, self.resolution_depth))
+        return r_out_im
+
+    def plot_rate_map(self, save_path: str = None, ax: mpl.axes.Axes = None):
+        """
+        Plot current rates and an example of inhibitory and excitatory neuron
+
+        Parameters
+        ----------
+        save_path : str
+            Path to save the figure. Default None, it doesn't save the figure
+        ax : ndarray of matplotlib.axis
+            (3,) with 3 axis to make plots from matplotlib, if None it will create an entire figure
+        """
+        if ax is None:
+            f, ax = plt.subplots()
+        r_out_im = self.get_full_output_rate()
+        r_out_im = r_out_im.reshape((self.resolution_width, self.resolution_depth))
+        make_plot_rate_map(r_out_im.T, ax, "Out rate", "width", "depth", "Firing rate")
+
+        if save_path is not None:
+            plt.savefig(save_path, bbox_inches="tight")
+            plt.close("all")
+        else:
+            return ax
+
+    def plot_all_rates(self, save_path: str = None, ax: mpl.axes.Axes = None):
         """
         Plot current rates and an example of inhibitory and excitatory neuron
 
         Parameters
         ----------
         save_path : str
             Path to save the figure. Default None, it doesn't save the figure
@@ -385,28 +430,22 @@
             (3,) with 3 axis to make plots from matplotlib, if None it will create an entire figure
         """
         if ax is None:
             f, ax = plt.subplots(1, 3, figsize=(14, 5))
 
         r_out_im = self.get_full_output_rate()
         r_out_im = r_out_im.reshape((self.resolution_width, self.resolution_depth))
-
         exc_im = self.exc_cell_list[np.random.choice(np.arange(self.exc_cell_list.shape[0])), ...].reshape(
             (self.resolution_width, self.resolution_depth)
         )
         inh_im = self.inh_cell_list[np.random.choice(np.arange(self.inh_cell_list.shape[0])), ...].reshape(
             (self.resolution_width, self.resolution_depth)
         )
-
-        ax[0].imshow(exc_im.T, cmap="Reds")
-        ax[0].set_title("Exc rates", fontsize=14)
-        ax[1].imshow(inh_im.T, cmap="Blues")
-        ax[1].set_title("Inh rates", fontsize=14)
-        im = ax[2].imshow(r_out_im.T, cmap="jet")
-        ax[2].set_title("Out rate", fontsize=14)
-        plt.colorbar(im, ax=ax[2])
+        make_plot_rate_map(exc_im.T, ax[0], "Exc rates", "width", "depth", "Firing rate")
+        make_plot_rate_map(inh_im.T, ax[1], "Inh rates", "width", "depth", "Firing rate")
+        make_plot_rate_map(r_out_im.T, ax[2], "Out rate", "width", "depth", "Firing rate")
 
         if save_path is not None:
             plt.savefig(save_path, bbox_inches="tight")
             plt.close("all")
         else:
             return ax
```

### Comparing `NeuralPlayground-0.0.2/neuralplayground/arenas/README.md` & `NeuralPlayground-0.0.3/neuralplayground/arenas/README.md`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.2/neuralplayground/arenas/arena_core.py` & `NeuralPlayground-0.0.3/neuralplayground/arenas/arena_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,25 +139,28 @@
         """Save current variables of the object to re-instantiate the environment later
 
         Parameters
         ----------
         save_path: str
             Path to save the environment
         """
-        pickle.dump(self.__dict__, open(os.path.join(save_path), "wb"), pickle.HIGHEST_PROTOCOL)
+        # pickle.dump(self.__dict__, open(os.path.join(save_path), "wb"), pickle.HIGHEST_PROTOCOL)
+        pickle.dump(self, open(os.path.join(save_path), "wb"), pickle.HIGHEST_PROTOCOL)
 
     def restore_environment(self, save_path: str):
         """Restore environment saved using save_environment method
 
         Parameters
         ----------
         save_path: str
             Path to retrieve the environment
         """
-        self.__dict__ = pd.read_pickle(save_path)
+        # self.__dict__ = pd.read_pickle(save_path)
+        # TODO: for some reason, ruff has a problem with this: self = pd.read_pickle(save_path)
+        pd.read_pickle(save_path)
 
     def __eq__(self, other):
         """Check if two environments are equal by comparing all of its attributes
 
         Parameters:
         ----------
         other: Environment
```

### Comparing `NeuralPlayground-0.0.2/neuralplayground/arenas/connected_rooms.py` & `NeuralPlayground-0.0.3/neuralplayground/arenas/connected_rooms.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.2/neuralplayground/arenas/hafting_2008.py` & `NeuralPlayground-0.0.3/neuralplayground/arenas/hafting_2008.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,15 @@
         self.experiment = experiment_class(
             data_path=self.data_path,
             experiment_name=self.environment_name,
             verbose=verbose,
             recording_index=recording_index,
         )
         self.arena_limits = self.experiment.arena_limits
+        self.recording_list = self.experiment.recording_list
         self.arena_x_limits, self.arena_y_limits = (
             self.arena_limits[0, :],
             self.arena_limits[1, :],
         )
         env_kwargs["arena_x_limits"] = self.arena_x_limits
         env_kwargs["arena_y_limits"] = self.arena_y_limits
         env_kwargs["agent_step_size"] = 1.0
@@ -147,26 +148,37 @@
 
         Returns
         -------
         recording_list: Pandas dataframe
             List of available experiment, columns with rat_id, recording session and recorded variables
         """
         self.experiment.show_data(full_dataframe=full_dataframe)
+        return self.experiment.show_data(full_dataframe=full_dataframe)
 
     def plot_recording_tetr(
         self,
         recording_index: Union[int, tuple, list] = None,
         save_path: Union[str, tuple, list] = None,
         ax: Union[mpl.axes.Axes, tuple, list] = None,
         tetrode_id: Union[str, tuple, list] = None,
         bin_size: float = 2.0,
     ):
         """Check plot_recording_tetrode method from neuralplayground.experiments.Hafting2008Data"""
         return self.experiment.plot_recording_tetr(recording_index, save_path, ax, tetrode_id, bin_size)
 
+    def recording_tetr(
+        self,
+        recording_index: Union[int, tuple, list] = None,
+        save_path: Union[str, tuple, list] = None,
+        tetrode_id: Union[str, tuple, list] = None,
+        bin_size: float = 2.0,
+    ):
+        """Check plot_recording_tetrode method from neuralplayground.experiments.Hafting2008Data"""
+        return self.experiment.recording_tetr(recording_index, save_path, tetrode_id, bin_size)
+
     def plot_recorded_trajectory(
         self,
         recording_index: Union[int, tuple, list] = None,
         save_path: Union[str, tuple, list] = None,
         ax: Union[mpl.axes.Axes, tuple, list] = None,
         plot_every: int = 20,
     ):
```

### Comparing `NeuralPlayground-0.0.2/neuralplayground/arenas/sargolini_2006.py` & `NeuralPlayground-0.0.3/neuralplayground/arenas/sargolini_2006.py`

 * *Files 5% similar despite different names*

```diff
@@ -110,10 +110,7 @@
             self.reset()
 
     def show_data(self, full_dataframe: bool = False):
         print("no dataframe with sessions, just pre-processed positions of all trajectories")
 
     def plot_recording_tetr(self, **kwargs):
         print("No tetrode data available")
-
-    def plot_recorded_trajectory(self, **kwargs):
-        NotImplemented
```

### Comparing `NeuralPlayground-0.0.2/neuralplayground/arenas/simple2d.py` & `NeuralPlayground-0.0.3/neuralplayground/arenas/simple2d.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import cv2
-import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 from gymnasium.spaces import Box
 from matplotlib.backends.backend_agg import FigureCanvasAgg as FigureCanvas
 
 from neuralplayground.arenas.arena_core import Environment
+from neuralplayground.plotting.plot_utils import make_plot_trajectories
 from neuralplayground.utils import check_crossing_wall
 
 
 class Simple2D(Environment):
     """
     Methods (Some in addition to Environment class)
     ----------
@@ -281,71 +281,41 @@
         Returns
         -------
         ax: mpl.axes._subplots.AxesSubplot (matplotlib axis from subplots)
             Modified axis where the trajectory is plotted
         f: matplotlib.figure
             if return_figure parameters is True
         """
-
         # Use or not saved history
         if history_data is None:
             history_data = self.history
 
         # Generate Figure
         if ax is None:
             f, ax = plt.subplots(1, 1, figsize=(8, 6))
 
-        # Draw walls
-        for wall in self.default_walls:
-            ax.plot(wall[:, 0], wall[:, 1], "C3", lw=3)
-
-        # Draw custom walls
-        for wall in self.custom_walls:
-            ax.plot(wall[:, 0], wall[:, 1], "C0", lw=3)
-
-        # Making the trajectory plot roughly square to show structure of the arena better
-        lower_lim, upper_lim = np.amin(self.arena_limits), np.amax(self.arena_limits)
-        ax.set_xlim([lower_lim, upper_lim])
-        ax.set_ylim([lower_lim, upper_lim])
-
         # Make plot of positions
         if len(history_data) != 0:
             state_history = [s["state"] for s in history_data]
-            next_state_history = [s["next_state"] for s in history_data]
-            state_history[0]
-            next_state_history[-1]
+            x = []
+            y = []
+            for i, s in enumerate(state_history):
+                # if i % plot_every == 0:
+                #     if i + plot_every >= len(state_history):
+                #         break
+                x.append(s[0])
+                y.append(s[1])
+            ax = make_plot_trajectories(self.arena_limits, np.asarray(x), np.asarray(y), ax, plot_every)
 
-            cmap = mpl.cm.get_cmap("plasma")
-            norm = plt.Normalize(0, len(state_history))
+        for wall in self.default_walls:
+            ax.plot(wall[:, 0], wall[:, 1], "C3", lw=3)
 
-            aux_x = []
-            aux_y = []
-            for i, s in enumerate(state_history):
-                if i % plot_every == 0:
-                    if i + plot_every >= len(state_history):
-                        break
-                    x_ = [s[0], state_history[i + plot_every][0]]
-                    y_ = [s[1], state_history[i + plot_every][1]]
-                    aux_x.append(s[0])
-                    aux_y.append(s[1])
-                    sc = ax.plot(x_, y_, "-", color=cmap(norm(i)), alpha=0.6)
-
-            sc = ax.scatter(
-                aux_x,
-                aux_y,
-                c=np.arange(len(aux_x)),
-                vmin=0,
-                vmax=len(aux_x),
-                cmap="plasma",
-                alpha=0.6,
-                s=0.5,
-            )
-            cbar = plt.colorbar(sc, ax=ax, ticks=[0, len(state_history)])
-            cbar.ax.set_ylabel("N steps", rotation=270, fontsize=16)
-            cbar.ax.set_yticklabels([0, len(state_history)], fontsize=16)
+            # Draw custom walls
+        for wall in self.custom_walls:
+            ax.plot(wall[:, 0], wall[:, 1], "C0", lw=3)
 
         if save_path is not None:
             plt.savefig(save_path, bbox_inches="tight")
 
         if return_figure:
             return ax, f
         else:
```

### Comparing `NeuralPlayground-0.0.2/neuralplayground/arenas/wernle_2018.py` & `NeuralPlayground-0.0.3/neuralplayground/arenas/wernle_2018.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.2/neuralplayground/datasets.py` & `NeuralPlayground-0.0.3/neuralplayground/datasets.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.2/neuralplayground/experiments/README.md` & `NeuralPlayground-0.0.3/neuralplayground/experiments/README.md`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.2/neuralplayground/experiments/hafting_2008_data.py` & `NeuralPlayground-0.0.3/neuralplayground/experiments/hafting_2008_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import numpy as np
 import pandas as pd
 import scipy.io as sio
 from IPython.display import display
 
 from neuralplayground.datasets import fetch_data_path
 from neuralplayground.utils import clean_data, get_2D_ratemap
+from neuralplayground.plotting.plot_utils import make_plot_trajectories , make_plot_rate_map
+
 
 from .experiment_core import Experiment
 
 
 class Hafting2008Data(Experiment):
     """Data class for Hafting et al. 2008. https://www.nature.com/articles/nature06957
     The data can be obtained from https://archive.norstore.no/pages/public/datasetDetail.jsf?id=C43035A4-5CC5-44F2-B207-126922523FD9
@@ -75,14 +77,15 @@
 
     def _load_data(self):
         """Parse data according to specific data format
         if you are a user check the notebook examples"""
         self.best_recording_index = 4  # Nice session recording as default
         # Arena limits from the experimental setting, first row x limits, second row y limits, in cm
         self.arena_limits = np.array([[-200, 200], [-20, 20]])
+
         data_path_list = glob.glob(self.data_path + "*.mat")
         mice_ids = np.unique([dp.split("/")[-1][:5] for dp in data_path_list])
         # Initialize data dictionary, later handled by this object itself (so don't worry about this)
         self.data_per_animal = {}
         for m_id in mice_ids:
             m_paths_list = glob.glob(self.data_path + m_id + "*.mat")
             sessions = np.unique([dp.split("/")[-1].split("-")[1][:8] for dp in m_paths_list]).astype(str)
@@ -261,25 +264,27 @@
         tetrode_data = session_data[tetrode_id]
         test_spikes = tetrode_data["ts"][:,]
         test_spikes = test_spikes[:, 0]
         time_array = time_array[:, 0]
 
         return time_array, test_spikes, x, y
 
+
     def plot_recording_tetr(
         self,
         recording_index: Union[int, tuple, list] = None,
         save_path: Union[str, tuple, list] = None,
         ax: Union[mpl.axes.Axes, tuple, list] = None,
         tetrode_id: Union[str, tuple, list] = None,
         bin_size: float = 2.0,
     ):
         """Plot tetrode ratemap from spike data for a given recording index or a list of recording index.
         If given a list or tuple as argument, all arguments must be list, tuple, or None.
 
+
         Parameters
         ----------
         recording_index: int, tuple of ints, list of ints
             recording index to plot spike ratemap, if list or tuple, it will recursively call this function
             to make a plot per recording index. If this argument is list or tuple, the rest of variables must
             be list or tuple with their respective types, or keep the default None value.
         save_path: str, list of str, tuple of str
@@ -324,83 +329,30 @@
                 ind_axis = self.plot_recording_tetr(ind, save_path=save_path_i, ax=ax_i, tetrode_id=tetrode_id_i)
                 axis_list.append(ind_axis)
             return axis_list
 
         # Generate axis in case ax is None
         if ax is None:
             f, ax = plt.subplots(1, 1, figsize=(10, 8))
-
-        # Recall recorded data
+        # Compute ratemap matrices from data
         session_data, rev_vars, rat_info = self.get_recording_data(recording_index)
         if tetrode_id is None:
             tetrode_id = self._find_tetrode(rev_vars)
 
-        arena_width = self.arena_limits[0, 1] - self.arena_limits[0, 0]
-        arena_depth = self.arena_limits[1, 1] - self.arena_limits[1, 0]
-
-        # Recall spike data
-        time_array, test_spikes, x, y = self.get_tetrode_data(session_data, tetrode_id)
 
-        # Compute ratemap matrices from data
-        h, binx, biny = get_2D_ratemap(
-            time_array,
-            test_spikes,
-            x,
-            y,
-            x_size=int(arena_width / bin_size),
-            y_size=int(arena_depth / bin_size),
-            filter_result=True,
-        )
+        h, binx, biny = self.recording_tetr(recording_index, save_path, tetrode_id, bin_size)
 
         # Use auxiliary function to make the plot
-        self._make_tetrode_plot(h, ax, tetrode_id, save_path)
-        # Return ratemap values, x bin limits and y bin limits
-        return h, binx, biny
-
-    def _make_tetrode_plot(self, h, ax, title, save_path):
-        """plot function with formating of ratemap plot
-
-        Parameters
-        ----------
-        h: ndarray (nybins, nxbins)
-            Number of spikes falling on each bin through the recorded session, nybins number of bins in y axis,
-            nxbins number of bins in x axis
-        ax: mpl.axes._subplots.AxesSubplot (matplotlib axis from subplots)
-            axis from subplot from matplotlib where the ratemap will be plotted.
-        title: str
-            plot title, tetrode id by default when called
-        save_path: str, list of str, tuple of str
-            saving path of the generated figure, if None, no figure is saved
-
-        Returns
-        -------
-        ax: mpl.axes._subplots.AxesSubplot (matplotlib axis from subplots)
-            Modified axis where ratemap is plotted
-        """
-
-        # Formating ratemap plot
-        sc = ax.imshow(h, cmap="jet")
-        cbar = plt.colorbar(sc, ax=ax, ticks=[np.min(h), np.max(h)], orientation="horizontal")
-        cbar.ax.set_xlabel("Firing rate", fontsize=12)
-        cbar.ax.set_xticklabels([np.round(np.min(h)), np.round(np.max(h))], fontsize=12)
-        ax.set_title(title)
-
-        ax.set_ylabel("width", fontsize=16)
-        ax.set_xlabel("depth", fontsize=16)
-        ax.grid(False)
-
-        ax.set_xticks([])
-        ax.set_yticks([])
-
-        # Save if save_path is not None
+        ax = make_plot_rate_map(h, ax, 'rat: '+str(rat_info['rat_id'])+' sess: '+str(rat_info['sess'])+' tetrode: '+tetrode_id,"width","depth","Firing rate")
         if save_path is None:
-            return ax
+            return h, binx, biny
         else:
             plt.savefig(save_path, bbox_inches="tight")
-            return ax
+            # Return ratemap values, x bin limits and y bin limits
+            return h, binx, biny
 
     def plot_trajectory(
         self,
         recording_index: Union[int, tuple, list] = None,
         save_path: Union[str, tuple, list] = None,
         ax: Union[mpl.axes.Axes, tuple, list] = None,
         plot_every: int = 20,
@@ -452,106 +404,66 @@
             f, ax = plt.subplots(1, 1, figsize=(8, 6))
 
         session_data, rev_vars, rat_info = self.get_recording_data(recording_index)
         tetrode_id = self._find_tetrode(rev_vars)
 
         time_array, test_spikes, x, y = self.get_tetrode_data(session_data, tetrode_id)
         # Helper function to format the trajectory plot
-        self._make_trajectory_plot(x, y, ax, plot_every)
+
+        ax = make_plot_trajectories(self.arena_limits, x, y, ax, plot_every)
+
         # Save if save_path is not None
         if save_path is None:
             pass
         else:
             plt.savefig(save_path, bbox_inches="tight")
         return x, y, time_array
 
-    def _make_trajectory_plot(self, x, y, ax, plot_every, fontsize=24):
-        """
+
+    def recording_tetr(self, recording_index: Union[int, tuple, list] = None,
+                            save_path: Union[str, tuple, list] = None,
+                            tetrode_id: Union[str, tuple, list] = None,
+                            bin_size: float = 2.0):
+        """ tetrode ratemap from spike data for a given recording index or a list of recording index.
+        If given a list or tuple as argument, all arguments must be list, tuple, or None.
 
         Parameters
         ----------
-        x: ndarray (n_samples,)
-            x position throughout recording of the given session
-        y: ndarray (n_samples,)
-            y position throughout recording of the given session
-        ax: mpl.axes._subplots.AxesSubplot (matplotlib axis from subplots)
-            axis from subplot from matplotlib where the ratemap will be plotted.
-        plot_every: int
-            time steps skipped to make the plot to reduce cluttering
-        fontsize: int
-            fontsize of labels in the plot
+        recording_index: int, tuple of ints, list of ints
+            recording index to plot spike ratemap, if list or tuple, it will recursively call this function
+            to make a plot per recording index. If this argument is list or tuple, the rest of variables must
+            be list or tuple with their respective types, or keep the default None value.
+        save_path: str, list of str, tuple of str
+            saving path of the generated figure, if None, no figure is saved
+        tetrode_id: str, list of str, or tuple of str
+            tetrode id in the corresponding session
+        bin_size: float
+            bin size to discretize space when computing ratemap
 
         Returns
         -------
-        ax: mpl.axes._subplots.AxesSubplot (matplotlib axis from subplots)
-            Modified axis where the trajectory is plotted
+        h: ndarray (nybins, nxbins)
+            Number of spikes falling on each bin through the recorded session, nybins number of bins in y axis,
+            nxbins number of bins in x axis
+        binx: ndarray (nxbins +1,)
+            bin limits of the ratemap on the x axis
+        biny: ndarray (nybins +1,)
+            bin limits of the ratemap on the y axis
+        (when using list pr tuple as argument, this function return a list or tuple of the variables listed above)
         """
 
-        # Plotting borders of the arena
-        ax.plot(
-            [self.arena_limits[0, 0], self.arena_limits[0, 0]],
-            [self.arena_limits[1, 0], self.arena_limits[1, 1]],
-            "C3",
-            lw=3,
-        )
-        ax.plot(
-            [self.arena_limits[0, 1], self.arena_limits[0, 1]],
-            [self.arena_limits[1, 0], self.arena_limits[1, 1]],
-            "C3",
-            lw=3,
-        )
-        ax.plot(
-            [self.arena_limits[0, 0], self.arena_limits[0, 1]],
-            [self.arena_limits[1, 1], self.arena_limits[1, 1]],
-            "C3",
-            lw=3,
-        )
-        ax.plot(
-            [self.arena_limits[0, 0], self.arena_limits[0, 1]],
-            [self.arena_limits[1, 0], self.arena_limits[1, 0]],
-            "C3",
-            lw=3,
-        )
+        # Recursive call of this function in case of list or tuple
+        session_data, rev_vars, rat_info = self.get_recording_data(recording_index)
+        if tetrode_id is None:
+            tetrode_id = self._find_tetrode(rev_vars)
 
-        # Setting colormap of trajectory
-        cmap = mpl.cm.get_cmap("plasma")
-        norm = plt.Normalize(0, np.size(x))
-
-        aux_x = []
-        aux_y = []
-        for i in range(len(x)):
-            if i % plot_every == 0:
-                if i + plot_every >= len(x):
-                    break
-                x_ = [x[i], x[i + plot_every]]
-                y_ = [y[i], y[i + plot_every]]
-                aux_x.append(x[i])
-                aux_y.append(y[i])
-                sc = ax.plot(x_, y_, "-", color=cmap(norm(i)), alpha=0.6)
-
-        # Setting plot labels
-        ax.set_xlabel("width", fontsize=fontsize)
-        ax.set_ylabel("depth", fontsize=fontsize)
-        ax.set_title("position", fontsize=fontsize)
-        ax.grid(False)
-
-        cmap = mpl.cm.get_cmap("plasma")
-        norm = plt.Normalize(0, np.size(x))
-        sc = ax.scatter(
-            aux_x,
-            aux_y,
-            c=np.arange(len(aux_x)),
-            vmin=0,
-            vmax=len(x),
-            cmap="plasma",
-            alpha=0.6,
-            s=0.1,
-        )
+        arena_width = self.arena_limits[0, 1] - self.arena_limits[0, 0]
+        arena_depth = self.arena_limits[1, 1] - self.arena_limits[1, 0]
 
-        # Setting colorbar to show number of sampled (time steps) recorded
-        cbar = plt.colorbar(sc, ax=ax, ticks=[0, len(x)])
-        cbar.ax.tick_params(labelsize=fontsize)
-        cbar.ax.set_ylabel("N steps", rotation=270, fontsize=fontsize)
-        cbar.ax.set_yticklabels([0, len(x)], fontsize=fontsize)
-        ax.set_xlim([np.amin([x.min(), y.min()]) - 1.0, np.amax([x.max(), y.max()]) + 1.0])
-        ax.set_ylim([np.amin([x.min(), y.min()]) - 1.0, np.amax([x.max(), y.max()]) + 1.0])
-        return ax
+        # Recall spike data
+        time_array, test_spikes, x, y = self.get_tetrode_data(session_data, tetrode_id)
+
+        # Compute ratemap matrices from data
+        h, binx, biny = get_2D_ratemap(time_array, test_spikes, x, y, x_size=int(arena_width / bin_size),
+                                       y_size=int(arena_depth / bin_size), filter_result=True)
+
+        return h, binx, biny
```

### Comparing `NeuralPlayground-0.0.2/neuralplayground/experiments/sargolini_2006_data.py` & `NeuralPlayground-0.0.3/neuralplayground/experiments/sargolini_2006_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         experiment_name: str
             string to identify object in case of multiple instances
         data_path: str
             if None, fetch the data from the NeuralPlayground data repository,
             else load data from given path
         """
         self.experiment_name = experiment_name
+        self.recording_list = []
         if data_path is None:
             # Set data_path to the data directory within the package
             self.data_path = fetch_data_path("sargolini_2006")
         else:
             self.data_path = data_path
         # Sort the data in data_path
         (
@@ -133,16 +134,16 @@
 
     def _load_data(self):
         """Parse data according to specific data format
         if you are a user check the notebook examples"""
         self.best_recording_index = 0  # Nice session recording as default
         # Arena limits from the experimental setting, first row x limits, second row y limits, in cm
         self.arena_limits = np.array([[-50.0, 50.0], [-50.0, 50.0]])
-        data_path_list = glob.glob(self.data_path + "*.mat")
-        mice_ids = np.unique([dp.split("/")[-1][:5] for dp in data_path_list])
+        data_path_list = glob.glob(os.path.join(self.data_path, "*.mat"))
+        mice_ids = np.unique([os.path.basename(dp)[:5] for dp in data_path_list])
         # Initialize data dictionary, later handled by this object itself (so don't worry about this)
         self.data_per_animal = {}
         for m_id in mice_ids:
             m_paths_list = glob.glob(self.data_path + m_id + "*.mat")
             sessions = np.unique([dp.split("/")[-1].split("-")[1][:8] for dp in m_paths_list]).astype(str)
             self.data_per_animal[m_id] = {}
             for sess in sessions:
```

### Comparing `NeuralPlayground-0.0.2/neuralplayground/experiments/wernle_2018_data.py` & `NeuralPlayground-0.0.3/neuralplayground/experiments/wernle_2018_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import pandas as pd
 import scipy.io as sio
 
 import neuralplayground
 from neuralplayground.datasets import fetch_data_path
 from neuralplayground.experiments.hafting_2008_data import Hafting2008Data
 from neuralplayground.utils import get_2D_ratemap
+from neuralplayground.plotting.plot_utils import make_plot_trajectories , make_plot_rate_map
 
 
 class Wernle2018Data(Hafting2008Data):
     """Data class for https://www.nature.com/articles/s41593-017-0036-6
     The data can be obtained from https://doi.org/10.11582/2017.00023
     """
 
@@ -100,14 +101,15 @@
             Position of rats after merging rooms
             (19 x 1) where each element is a (T, 4) recording where T are the total number of samples in time
             at a 50Hz frequency, and column 1 is the time in seconds, column 2 is x_position, column 3 is y_position,
             column 4 is speed index (1 if speed is above 5cm/s)
         """
 
         # Load ratemaps
+        self.best_recording_index = 100  # Nice session recording as default
         self.inner_path = "nn_Data+Code/data/"
         self.ratemap = sio.loadmat(os.path.join(self.data_path, self.inner_path, "Figures_1_2_3/ratemaps.mat"))
         self.ratemap = self.ratemap["ratemaps"]
 
         # The following is the recording progression of grid cell patterns for 19 different cells
         # over 10 different rats
 
@@ -254,14 +256,16 @@
                                 identifiers,
                             ]
                         )
 
             return data_list
 
         else:
+            if recording_index is None:
+                recording_index = self.best_recording_index
             session_info = self.recording_list.iloc[recording_index]
             if type(session_info["recorded_vars"]) is list:
                 sess_index = session_info["session"]
                 identifiers = {"sess_index": sess_index}
                 if session_info["before_merge"]:
                     sess_data = {
                         "time": self.pos_A_B[sess_index, 0][:, 0],
@@ -329,14 +333,17 @@
         binx: ndarray (nxbins +1,)
             bin limits of the ratemap on the x axis
         biny: ndarray (nybins +1,)
             bin limits of the ratemap on the y axis
         (when using list pr tuple as argument, this function return a list or tuple of the variables listed above)
         """
         # Recursive call of this function in case of list or tuple
+        if recording_index is None:
+            recording_index = self.best_recording_index
+
         if type(recording_index) is list or type(recording_index) is tuple:
             axis_list = []
             for i, ind in enumerate(recording_index):
                 # Checking if rest of variables are default or list values
                 if save_path is not None:
                     save_path_i = save_path[i]
                 else:
@@ -354,14 +361,40 @@
             return axis_list
 
         # Generate axis in case ax is None
         if ax is None:
             f, ax = plt.subplots(1, 1, figsize=(10, 8))
 
         # Recall recorded data
+
+        h, binx, biny = self.recording_tetr()
+
+        # Adding merging status to plot title
+
+        merged = self.recording_list.iloc[recording_index]["before_merge"]
+        merged_mssg = "merged" if not merged else "before_merge"
+
+        sess_index = self.recording_list.iloc[recording_index]["session"]
+        # Use auxiliary function to make the plot
+        ax=make_plot_rate_map(h, ax, "sess_index_" + str(sess_index) + "_" + merged_mssg,"width","depth","Firing rate")
+        # Save if save_path is not None
+        if save_path is None:
+            pass
+        else:
+            plt.savefig(save_path, bbox_inches="tight")
+        # Return ratemap values, x bin limits and y bin limits
+        return ax
+
+    def recording_tetr(self, recording_index: Union[int, tuple, list] = None,
+                            save_path: Union[str, tuple, list] = None,
+                            tetrode_id: Union[str, tuple, list] = None,
+                            bin_size: float = 2.0):
+
+
+        # Recall recorded data
         session_data, rev_vars, rat_info = self.get_recording_data(recording_index)
 
         arena_width = self.arena_limits[0, 1] - self.arena_limits[0, 0]
         arena_depth = self.arena_limits[1, 1] - self.arena_limits[1, 0]
 
         # Check of the session has spikes to compute ratemap
         # Plot pre-computed ratemap otherwise
@@ -378,38 +411,25 @@
                 test_spikes,
                 x,
                 y,
                 x_size=int(arena_width / bin_size),
                 y_size=int(arena_depth / bin_size),
                 filter_result=True,
             )
-
         elif type(rev_vars) is list and "spikes" not in rev_vars:
             warnings.warn("No spike data pre merging")
             return
         else:
             h = session_data["ratemap"]
             binx = np.linspace(self.arena_limits[0, 0], self.arena_limits[0, 1], num=h.shape[1])
             biny = np.linspace(self.arena_limits[1, 0], self.arena_limits[1, 1], num=h.shape[0])
 
-        # Adding merging status to plot title
-        merged = self.recording_list.iloc[recording_index]["before_merge"]
-        merged_mssg = "merged" if not merged else "before_merge"
-
-        sess_index = self.recording_list.iloc[recording_index]["session"]
-        # Use auxiliary function to make the plot
-        self._make_tetrode_plot(h, ax, "sess_index_" + str(sess_index) + "_" + merged_mssg, save_path)
-        # Save if save_path is not None
-        if save_path is None:
-            pass
-        else:
-            plt.savefig(save_path, bbox_inches="tight")
-        # Return ratemap values, x bin limits and y bin limits
         return h, binx, biny
 
+
     def plot_trajectory(
         self,
         recording_index: Union[int, tuple, list] = None,
         save_path: Union[str, tuple, list] = None,
         ax: Union[mpl.axes.Axes, tuple, list] = None,
         plot_every: int = 20,
     ):
@@ -435,14 +455,17 @@
             x position throughout recording of the given session
         y: ndarray (n_samples,)
             y position throughout recording of the given session
         time_array: ndarray (n_samples,)
             array with the timestamps in seconds per position of the given session
 
         """
+        if recording_index is None:
+            recording_index = self.best_recording_index
+
         if type(recording_index) is list or type(recording_index) is tuple:
             axis_list = []
             for i, ind in enumerate(recording_index):
                 # Checking if rest of variables are default or list values
                 if save_path is not None:
                     save_path_i = save_path[i]
                 else:
@@ -471,15 +494,16 @@
                 session_data["posy"],
             )
         else:
             warnings.warn("This index does not have position data")
             return
 
         # Helper function to format the trajectory plot
-        ax = self._make_trajectory_plot(x, y, ax, plot_every)
+
+        ax =  make_plot_trajectories(self.arena_limits, x, y, ax, plot_every)
         if save_path is None:
             pass
         else:
             plt.savefig(save_path, bbox_inches="tight")
         return x, y, time_array
 
     def plot_merging_comparison(self, session_index: Union[int, list, tuple]):
@@ -505,97 +529,23 @@
             session_index = [
                 session_index,
             ]
         f, ax = plt.subplots(n_cells, 2, figsize=(8, 5 * n_cells))
         ratemaps_before = []
         ratemaps_after = []
         for i in range(n_cells):
-            ax[i, 0].imshow(self.ratemap[session_index[i], 0], cmap="jet")
-            ax[i, 1].imshow(self.ratemap[session_index[i], 1], cmap="jet")
+            make_plot_rate_map(self.ratemap[session_index[i], 0],  ax[i, 0], "Before merging", "width", "depth","Firing rate")
+            make_plot_rate_map(self.ratemap[session_index[i], 1], ax[i, 1], "After merging", "width", "depth", "Firing rate")
             ratemaps_before.append(self.ratemap[session_index[i], 0])
             ratemaps_after.append(self.ratemap[session_index[i], 1])
             ax[i, 0].axhline(y=50, color="white")
             ax[i, 1].axhline(y=50, color="white", linestyle="--")
-        ax[0, 0].set_title("Before merging")
-        ax[0, 1].set_title("After merging")
         return ratemaps_before, ratemaps_after, ax
 
-    def plot_development(
-        self,
-        n_cells: int = 3,
-        time_interval: Union[tuple, list] = (1.0, 2.0),
-        merged: bool = False,
-        plot_every: int = 10,
-    ):
-        """Prototype function for evolution of ratemaps through time
-
-        Parameters
-        ----------
-        n_cells: int
-            Number of cells to plot, from 0 to 19
-        time_interval: 2D-tuple or list with floats
-            Time inverval from experiment, if merged true, then time inverval after merging
-        merged: bool
-            If True, make plot for data after merging
-        plot_every: int
-            time steps skipped to make the plot to reduce cluttering
 
-        Returns
-        -------
-        ax: mpl.axes._subplots.AxesSubplot (matplotlib axis from subplots)
-            Modified axis where the trajectory is plotted
-        """
-        if merged:
-            pos = self.pos_AB[:n_cells, 0]
-        else:
-            pos = self.pos_A_B[:n_cells, 0]
-
-        f, ax = plt.subplots(1, n_cells, figsize=(4 * n_cells, 3))
-        for cell in range(n_cells):
-            pos_i = pos[cell]
-            init_sample = int(pos_i.shape[0] * (time_interval[0] * 60.0) / (np.amax(pos_i[:, 0])))
-            finish_sample = int(pos_i.shape[0] * (time_interval[1] * 60.0) / (np.amax(pos_i[:, 0])))
-            finish_sample - init_sample
-            cmap = mpl.cm.get_cmap("plasma")
-            norm = plt.Normalize(init_sample, finish_sample)
-            aux_x, aux_y = [], []
-            prev_x, prev_y = pos_i[init_sample, 1], pos_i[finish_sample, 2]
-            for sample_i in range(init_sample, finish_sample, plot_every):
-                x, y = pos_i[sample_i, 1], pos_i[sample_i, 2]
-                aux_x.append(x)
-                aux_y.append(y)
-                ax[cell].plot(
-                    (prev_x, x),
-                    (prev_y, y),
-                    "-",
-                    color=cmap(norm(sample_i)),
-                    alpha=0.4,
-                    lw=0.5,
-                )
-                prev_x = x
-                prev_y = y
-            ax[cell].set_ylim((-100, 100))
-            ax[cell].set_xlim((-100, 100))
-            sc = ax[cell].scatter(
-                aux_x,
-                aux_y,
-                c=np.arange(init_sample, finish_sample, plot_every),
-                vmin=init_sample,
-                vmax=finish_sample,
-                cmap="plasma",
-                alpha=0.4,
-                s=2,
-            )
-            ax[cell].axhline(y=0, color="black")
-            ticks = np.linspace(init_sample, finish_sample, num=10)
-            tickslabels = np.round(np.linspace(init_sample / 50 / 60, finish_sample / 50 / 60, num=10), 1)
-            cbar = plt.colorbar(sc, ax=ax[cell], ticks=ticks)
-            cbar.ax.set_yticklabels(tickslabels, fontsize=8)
-            cbar.ax.set_ylabel("Time [min]", rotation=270, labelpad=12)
-        return ax
 
     def get_recorded_session(self, recording_index=None):
         # Not used, override to avoid issues
         return [None, None, None]
 
 
 if __name__ == "__main__":
```

### Comparing `NeuralPlayground-0.0.2/neuralplayground/utils.py` & `NeuralPlayground-0.0.3/neuralplayground/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+import json
+import os
+from datetime import datetime
+
 import numpy as np
 from scipy.interpolate import interp1d
 from scipy.ndimage import gaussian_filter
 
 
 def check_crossing_wall(
     pre_state: np.ndarray,
@@ -328,7 +332,31 @@
         nan_indexes = np.isnan(self.ratemap)
         aux_ratemap = np.copy(self.ratemap)
         aux_ratemap[nan_indexes] = 0
         filtered_ratemap = gaussian_filter(aux_ratemap, 3.5)
         self.nan = np.nan
         filtered_ratemap[nan_indexes] = self.nan
         return filtered_ratemap
+
+
+def check_dir(path):
+    if not os.path.isdir(path):
+        os.makedirs(path)
+
+
+def get_date_time():
+    # datetime object containing current date and time
+    now = datetime.now()
+    dt_string = now.strftime("%d-%m-%Y_%H-%M-%S-%f")[:-3]
+    now = str(dt_string)
+    return now
+
+
+def dict_to_json(dict, path):
+    with open(path, "w") as outfile:
+        json.dump(dict, outfile)
+
+
+def load_json(path):
+    with open(path, "r") as infile:
+        dict = json.load(infile)
+    return dict
```

### Comparing `NeuralPlayground-0.0.2/pyproject.toml` & `NeuralPlayground-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
   "tqdm",
   "jupyter",
   "ipython",
   "matplotlib",
   "deepdiff",
   "opencv-python",
   "gymnasium",
+  "scikit-image",
   "pooch",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ClementineDomine/NeuralPlayground"
 "Bug tracker" = "https://github.com/ClementineDomine/NeuralPlayground/issues"
 "Documentation" = "https://github.com/ClementineDomine/NeuralPlayground"
```

### Comparing `NeuralPlayground-0.0.2/tests/README.md` & `NeuralPlayground-0.0.3/tests/README.md`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.2/tests/agent_test.py` & `NeuralPlayground-0.0.3/tests/agent_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             agent,
         ]
 
     def test_init_model(self, init_model):
         assert isinstance(init_model[0], Weber2018)
 
     def test_plot_rates(self, init_model):
-        init_model[0].plot_rates()
+        init_model[0].plot_rate_map()
 
     def test_agent_interaction(self, init_model, get_environment):
         env = get_environment[0]
         total_iters = 0
         n_steps = 1
         obs, state = env.reset()
         obs = obs[:2]
@@ -137,18 +137,18 @@
             obs = obs[:2]
             total_iters += 1
 
     def test_init_model(self, init_model):
         assert isinstance(init_model[0], Stachenfeld2018)
 
     def test_plot_sr_ground_truth(self, init_model):
-        sr = init_model[0].update_successor_rep()  # Choose your type of Update
-        init_model[0].plot_eigen(sr, eigen=(0,), save_path=None)
-        init_model[0].plot_eigen(sr, eigen=(0, 1), save_path=None)
+        sr = init_model[0].successor_rep_solution()  # Choose your type of Update
+        init_model[0].plot_rate_map(sr, eigen_vectors=(0,), save_path=None)
+        init_model[0].plot_rate_map(sr, eigen_vectors=(0, 1), save_path=None)
 
     def test_plot_sr_td(self, init_model):
         sr_td = init_model[0].update_successor_rep_td_full()  # Choose your type of Update
-        init_model[0].plot_eigen(sr_td, eigen=(0,), save_path=None)
+        init_model[0].plot_rate_map(sr_td, eigen_vectors=(0,), save_path=None)
 
     def test_plot_sr_sum(self, init_model):
         sr_sum = init_model[0].successor_rep_sum()
-        init_model[0].plot_eigen(sr_sum, eigen=(0,), save_path=None)
+        init_model[0].plot_rate_map(sr_sum, eigen_vectors=(0,), save_path=None)
```

### Comparing `NeuralPlayground-0.0.2/tests/arena_exp_test.py` & `NeuralPlayground-0.0.3/tests/arena_exp_test.py`

 * *Files identical despite different names*

