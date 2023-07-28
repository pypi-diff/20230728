# Comparing `tmp/circleci_webhook_manager-0.0.2.tar.gz` & `tmp/circleci_webhook_manager-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circleci_webhook_manager-0.0.2.tar", max compression
+gzip compressed data, was "circleci_webhook_manager-0.0.3.tar", max compression
```

## Comparing `circleci_webhook_manager-0.0.2.tar` & `circleci_webhook_manager-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1068 2023-07-24 00:56:37.287820 circleci_webhook_manager-0.0.2/LICENSE
--rw-r--r--   0        0        0     1870 2023-07-24 00:56:37.287820 circleci_webhook_manager-0.0.2/README.md
--rw-r--r--   0        0        0     5138 2023-07-24 00:56:37.287820 circleci_webhook_manager-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      194 2023-07-24 00:56:37.287820 circleci_webhook_manager-0.0.2/webhook_manager/__init__.py
--rw-r--r--   0        0        0      149 2023-07-24 00:56:37.287820 circleci_webhook_manager-0.0.2/webhook_manager/__main__.py
--rw-r--r--   0        0        0      966 2023-07-24 00:56:37.287820 circleci_webhook_manager-0.0.2/webhook_manager/cli.py
--rw-r--r--   0        0        0     2634 1970-01-01 00:00:00.000000 circleci_webhook_manager-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-28 05:38:38.122822 circleci_webhook_manager-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1870 2023-07-28 05:38:38.122822 circleci_webhook_manager-0.0.3/README.md
+-rw-r--r--   0        0        0     5174 2023-07-28 05:38:38.122822 circleci_webhook_manager-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      194 2023-07-28 05:38:38.122822 circleci_webhook_manager-0.0.3/webhook_manager/__init__.py
+-rw-r--r--   0        0        0      149 2023-07-28 05:38:38.122822 circleci_webhook_manager-0.0.3/webhook_manager/__main__.py
+-rw-r--r--   0        0        0      966 2023-07-28 05:38:38.122822 circleci_webhook_manager-0.0.3/webhook_manager/cli.py
+-rw-r--r--   0        0        0     3562 2023-07-28 05:38:38.122822 circleci_webhook_manager-0.0.3/webhook_manager/client.py
+-rw-r--r--   0        0        0     2827 2023-07-28 05:38:38.122822 circleci_webhook_manager-0.0.3/webhook_manager/models.py
+-rw-r--r--   0        0        0     2674 1970-01-01 00:00:00.000000 circleci_webhook_manager-0.0.3/PKG-INFO
```

### Comparing `circleci_webhook_manager-0.0.2/LICENSE` & `circleci_webhook_manager-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `circleci_webhook_manager-0.0.2/README.md` & `circleci_webhook_manager-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `circleci_webhook_manager-0.0.2/pyproject.toml` & `circleci_webhook_manager-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "circleci-webhook-manager"
-version = "0.0.2"
+version = "0.0.3"
 description = "This project aims to provide a simple way to manage bulk (selective or organization-wide) CircleCI webhooks."
 authors = ["Mark Beacom <m@beacom.dev>"]
 readme = "README.md"
 packages = [{include = "webhook_manager"}]
 license = "MIT"
 keywords = ["cli", "circleci", "webhook", "manager", "webhook", "organization"]
 classifiers = [
@@ -155,19 +155,21 @@
 # requires poethepoet outside of poetry.
 install = "poetry install"
 build = "poetry build"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 typer = {extras = ["all"], version = "^0.9.0"}
+httpx = "^0.24.1"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
 coverage = "^7.2.7"
+respx = "^0.20.2"
 
 [tool.poetry.group.dev.dependencies]
 isort = {extras = ["toml"], version = "^5.12.0"}
 black = "^23.7.0"
 mypy = "^1.4.1"
 debugpy = "^1.6.7"
 ruff = "^0.0.280"
```

### Comparing `circleci_webhook_manager-0.0.2/webhook_manager/cli.py` & `circleci_webhook_manager-0.0.3/webhook_manager/cli.py`

 * *Files identical despite different names*

### Comparing `circleci_webhook_manager-0.0.2/PKG-INFO` & `circleci_webhook_manager-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: circleci-webhook-manager
-Version: 0.0.2
+Version: 0.0.3
 Summary: This project aims to provide a simple way to manage bulk (selective or organization-wide) CircleCI webhooks.
 License: MIT
 Keywords: cli,circleci,webhook,manager,webhook,organization
 Author: Mark Beacom
 Author-email: m@beacom.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # circleci-webhook-manager
 
 [![Validation Workflow](https://github.com/mbeacom/circleci-webhook-manager/actions/workflows/validate.yaml/badge.svg?branch=main&event=push)](https://github.com/mbeacom/circleci-webhook-manager/actions/workflows/validate.yaml)
 [![Pre-Commit Checks Workflow](https://github.com/mbeacom/circleci-webhook-manager/actions/workflows/pre-commit.yaml/badge.svg?branch=main&event=push)](https://github.com/mbeacom/circleci-webhook-manager/actions/workflows/pre-commit.yaml)
```

