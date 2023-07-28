# Comparing `tmp/optuna-distributed-0.6.0.tar.gz` & `tmp/optuna-distributed-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optuna-distributed-0.6.0.tar", last modified: Wed Jul 26 11:33:13 2023, max compression
+gzip compressed data, was "optuna-distributed-0.6.1.tar", last modified: Fri Jul 28 11:29:04 2023, max compression
```

## Comparing `optuna-distributed-0.6.0.tar` & `optuna-distributed-0.6.1.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:33:13.113499 optuna-distributed-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:33:13.101499 optuna-distributed-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:33:13.105499 optuna-distributed-0.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/.github/ISSUE_TEMPLATE/general-question.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:33:13.105499 optuna-distributed-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/.github/workflows/format.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-26 11:33:13.117499 optuna-distributed-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:33:13.109499 optuna-distributed-0.6.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/examples/disable_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/examples/quadratic_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/examples/simple_pruning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/examples/simple_storages.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/examples/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:33:13.109499 optuna-distributed-0.6.0/optuna_distributed/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/eventloop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:33:13.109499 optuna-distributed-0.6.0/optuna_distributed/ipc/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/ipc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/ipc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/ipc/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/ipc/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:33:13.113499 optuna-distributed-0.6.0/optuna_distributed/managers/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/managers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/managers/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/managers/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:33:13.113499 optuna-distributed-0.6.0/optuna_distributed/messages/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/messages/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/messages/completed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/messages/failed.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/messages/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/messages/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/messages/pruned.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/messages/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/messages/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/messages/setattr.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/messages/shouldprune.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/messages/suggest.py
--rw-r--r--   0 runner    (1001) docker     (123)    14733 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/study.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)    10796 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:33:13.109499 optuna-distributed-0.6.0/optuna_distributed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-26 11:33:13.000000 optuna-distributed-0.6.0/optuna_distributed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-26 11:33:13.000000 optuna-distributed-0.6.0/optuna_distributed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:33:13.000000 optuna-distributed-0.6.0/optuna_distributed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-26 11:33:13.000000 optuna-distributed-0.6.0/optuna_distributed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-26 11:33:13.000000 optuna-distributed-0.6.0/optuna_distributed.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-26 11:33:13.117499 optuna-distributed-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:33:13.113499 optuna-distributed-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/tests/test_eventloop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/tests/test_ipc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/tests/test_managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/tests/test_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/tests/test_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:29:04.616310 optuna-distributed-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:29:04.600310 optuna-distributed-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:29:04.604310 optuna-distributed-0.6.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/.github/ISSUE_TEMPLATE/general-question.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:29:04.604310 optuna-distributed-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/.github/workflows/format.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-28 11:29:04.616310 optuna-distributed-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:29:04.608310 optuna-distributed-0.6.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/examples/disable_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/examples/quadratic_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/examples/simple_pruning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/examples/simple_storages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/examples/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:29:04.608310 optuna-distributed-0.6.1/optuna_distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/eventloop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:29:04.608310 optuna-distributed-0.6.1/optuna_distributed/ipc/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/ipc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/ipc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/ipc/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/ipc/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:29:04.612310 optuna-distributed-0.6.1/optuna_distributed/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/managers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/managers/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/managers/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:29:04.612310 optuna-distributed-0.6.1/optuna_distributed/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/messages/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/messages/completed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/messages/failed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/messages/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/messages/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/messages/pruned.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/messages/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/messages/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/messages/setattr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/messages/shouldprune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/messages/suggest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14733 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/study.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10796 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:29:04.608310 optuna-distributed-0.6.1/optuna_distributed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-28 11:29:04.000000 optuna-distributed-0.6.1/optuna_distributed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-28 11:29:04.000000 optuna-distributed-0.6.1/optuna_distributed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 11:29:04.000000 optuna-distributed-0.6.1/optuna_distributed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-28 11:29:04.000000 optuna-distributed-0.6.1/optuna_distributed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 11:29:04.000000 optuna-distributed-0.6.1/optuna_distributed.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-28 11:29:04.616310 optuna-distributed-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:29:04.616310 optuna-distributed-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/tests/test_eventloop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/tests/test_ipc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/tests/test_managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/tests/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/tests/test_trial.py
```

### Comparing `optuna-distributed-0.6.0/.github/ISSUE_TEMPLATE/feature_request.md` & `optuna-distributed-0.6.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/.github/workflows/format.yaml` & `optuna-distributed-0.6.1/.github/workflows/format.yaml`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/.github/workflows/release.yaml` & `optuna-distributed-0.6.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/.github/workflows/test.yaml` & `optuna-distributed-0.6.1/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/.gitignore` & `optuna-distributed-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/LICENSE` & `optuna-distributed-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/PKG-INFO` & `optuna-distributed-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optuna-distributed
-Version: 0.6.0
+Version: 0.6.1
 Summary: Distributed hyperparameter optimization made easy
 Author-email: Adrian Zuber <xadrianzetx@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/xadrianzetx/optuna-distributed
 Project-URL: Bug Tracker, https://github.com/xadrianzetx/optuna-distributed/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `optuna-distributed-0.6.0/README.md` & `optuna-distributed-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/examples/disable_logging.py` & `optuna-distributed-0.6.1/examples/disable_logging.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/examples/quadratic_simple.py` & `optuna-distributed-0.6.1/examples/quadratic_simple.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/examples/simple_pruning.py` & `optuna-distributed-0.6.1/examples/simple_pruning.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/examples/simple_storages.py` & `optuna-distributed-0.6.1/examples/simple_storages.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/examples/visualization.py` & `optuna-distributed-0.6.1/examples/visualization.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/optuna_distributed/config.py` & `optuna-distributed-0.6.1/optuna_distributed/config.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/optuna_distributed/eventloop.py` & `optuna-distributed-0.6.1/optuna_distributed/eventloop.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/optuna_distributed/ipc/base.py` & `optuna-distributed-0.6.1/optuna_distributed/ipc/base.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/optuna_distributed/ipc/pipe.py` & `optuna-distributed-0.6.1/optuna_distributed/ipc/pipe.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/optuna_distributed/ipc/queue.py` & `optuna-distributed-0.6.1/optuna_distributed/ipc/queue.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/optuna_distributed/managers/__init__.py` & `optuna-distributed-0.6.1/optuna_distributed/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/optuna_distributed/managers/base.py` & `optuna-distributed-0.6.1/optuna_distributed/managers/base.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/optuna_distributed/managers/distributed.py` & `optuna-distributed-0.6.1/optuna_distributed/managers/distributed.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/optuna_distributed/managers/local.py` & `optuna-distributed-0.6.1/optuna_distributed/managers/local.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/optuna_distributed/messages/__init__.py` & `optuna-distributed-0.6.1/optuna_distributed/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/optuna_distributed/messages/base.py` & `optuna-distributed-0.6.1/optuna_distributed/messages/base.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/optuna_distributed/messages/completed.py` & `optuna-distributed-0.6.1/optuna_distributed/messages/completed.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/optuna_distributed/messages/failed.py` & `optuna-distributed-0.6.1/optuna_distributed/messages/failed.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/optuna_distributed/messages/heartbeat.py` & `optuna-distributed-0.6.1/optuna_distributed/messages/heartbeat.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/optuna_distributed/messages/property.py` & `optuna-distributed-0.6.1/optuna_distributed/messages/property.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/optuna_distributed/messages/pruned.py` & `optuna-distributed-0.6.1/optuna_distributed/messages/pruned.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/optuna_distributed/messages/report.py` & `optuna-distributed-0.6.1/optuna_distributed/messages/report.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/optuna_distributed/messages/response.py` & `optuna-distributed-0.6.1/optuna_distributed/messages/response.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/optuna_distributed/messages/setattr.py` & `optuna-distributed-0.6.1/optuna_distributed/messages/setattr.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/optuna_distributed/messages/shouldprune.py` & `optuna-distributed-0.6.1/optuna_distributed/messages/shouldprune.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/optuna_distributed/messages/suggest.py` & `optuna-distributed-0.6.1/optuna_distributed/messages/suggest.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/optuna_distributed/study.py` & `optuna-distributed-0.6.1/optuna_distributed/study.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/optuna_distributed/terminal.py` & `optuna-distributed-0.6.1/optuna_distributed/terminal.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/optuna_distributed/trial.py` & `optuna-distributed-0.6.1/optuna_distributed/trial.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/optuna_distributed.egg-info/PKG-INFO` & `optuna-distributed-0.6.1/optuna_distributed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optuna-distributed
-Version: 0.6.0
+Version: 0.6.1
 Summary: Distributed hyperparameter optimization made easy
 Author-email: Adrian Zuber <xadrianzetx@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/xadrianzetx/optuna-distributed
 Project-URL: Bug Tracker, https://github.com/xadrianzetx/optuna-distributed/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `optuna-distributed-0.6.0/optuna_distributed.egg-info/SOURCES.txt` & `optuna-distributed-0.6.1/optuna_distributed.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 examples/quadratic_simple.py
 examples/simple_pruning.py
 examples/simple_storages.py
 examples/visualization.py
 optuna_distributed/__init__.py
 optuna_distributed/config.py
 optuna_distributed/eventloop.py
+optuna_distributed/py.typed
 optuna_distributed/study.py
 optuna_distributed/terminal.py
 optuna_distributed/trial.py
 optuna_distributed.egg-info/PKG-INFO
 optuna_distributed.egg-info/SOURCES.txt
 optuna_distributed.egg-info/dependency_links.txt
 optuna_distributed.egg-info/requires.txt
```

### Comparing `optuna-distributed-0.6.0/pyproject.toml` & `optuna-distributed-0.6.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,17 @@
 [project.urls]
 "Source" = "https://github.com/xadrianzetx/optuna-distributed"
 "Bug Tracker" = "https://github.com/xadrianzetx/optuna-distributed/issues"
 
 [tool.setuptools]
 packages = ["optuna_distributed"]
 
+[tool.setuptools.package-data]
+optuna_distributed = ["py.typed"]
+
 [tool.setuptools.dynamic]
 version = { attr = "optuna_distributed.__version__" }
 readme = { file = "README.md" }
 
 [tool.black]
 line-length = 99
 target-version = ["py310"]
```

### Comparing `optuna-distributed-0.6.0/tests/test_eventloop.py` & `optuna-distributed-0.6.1/tests/test_eventloop.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/tests/test_ipc.py` & `optuna-distributed-0.6.1/tests/test_ipc.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/tests/test_managers.py` & `optuna-distributed-0.6.1/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/tests/test_messages.py` & `optuna-distributed-0.6.1/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.0/tests/test_trial.py` & `optuna-distributed-0.6.1/tests/test_trial.py`

 * *Files identical despite different names*

