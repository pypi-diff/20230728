# Comparing `tmp/sparglim-0.1.0rc6.tar.gz` & `tmp/sparglim-0.1.1.tar.gz`

## Comparing `sparglim-0.1.0rc6.tar` & `sparglim-0.1.1.tar`

### file list

```diff
@@ -1,70 +1,73 @@
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/.dockerignore
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/.editorconfig
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/RELEASE.md
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/config.md
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/.github/workflows/lint.yml
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/.github/workflows/publish.yml
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/docker/Dockerfile.jupyterlab-sparglim
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/docker/Dockerfile.sparglim-server
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/jupyter-sparglim-on-k8s/README.md
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/jupyter-sparglim-on-k8s/k8s/deployment.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/jupyter-sparglim-on-k8s/k8s/headless-service.yaml
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/jupyter-sparglim-on-k8s/k8s/lab-service.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/jupyter-sparglim-sc/README.md
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/jupyter-sparglim-sc/k8s/jupyter-sparglim/deployment.yaml
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/jupyter-sparglim-sc/k8s/jupyter-sparglim/lab-service.yaml
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/jupyter-sparglim-sc/k8s/sparglim-server/connect-server-service.yaml
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/jupyter-sparglim-sc/k8s/sparglim-server/deployment.yaml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/jupyter-sparglim-sc/k8s/sparglim-server/headless-service.yaml
--rwxr-xr-x   0        0        0      236 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/scripts/reload.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/sparglim-server/README.md
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/sparglim-server/k8s/connect-server-service.yaml
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/sparglim-server/k8s/deployment.yaml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/sparglim-server/k8s/headless-service.yaml
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/docker/Dockerfile.jupyterlab-sparglim
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/docker/Dockerfile.sparglim-server
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/examples/jupyter-sparglim-on-k8s/README.md
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/examples/jupyter-sparglim-on-k8s/k8s/deployment.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/examples/jupyter-sparglim-on-k8s/k8s/headless-service.yaml
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/examples/jupyter-sparglim-on-k8s/k8s/lab-service.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/examples/jupyter-sparglim-sc/README.md
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/examples/jupyter-sparglim-sc/k8s/jupyter-sparglim/deployment.yaml
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/examples/jupyter-sparglim-sc/k8s/jupyter-sparglim/lab-service.yaml
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/examples/jupyter-sparglim-sc/k8s/sparglim-server/connect-server-service.yaml
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/examples/jupyter-sparglim-sc/k8s/sparglim-server/deployment.yaml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/examples/jupyter-sparglim-sc/k8s/sparglim-server/headless-service.yaml
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/examples/sparglim-server/README.md
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/examples/sparglim-server/k8s/connect-server-service.yaml
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/examples/sparglim-server/k8s/deployment.yaml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/examples/sparglim-server/k8s/headless-service.yaml
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/sparglim/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/sparglim/exceptions.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/sparglim/log.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/sparglim/py.typed
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/sparglim/utils.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/sparglim/config/__init__.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/sparglim/config/builder.py
--rw-r--r--   0        0        0    11568 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/sparglim/config/configer.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/sparglim/config/k8s.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/sparglim/server/__init__.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/sparglim/server/cli.py
--rw-r--r--   0        0        0     8921 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/sparglim/server/daemon.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/sparglim/server/tailer.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/sparglim/sql/__init__.py
--rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/sparglim/sql/magic.py
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/tests/conftest.py
--rw-r--r--   0        0        0     9525 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/tests/test_builder.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/tests/test_daemon.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/tests/test_magic.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/tests/example/people.json
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/tests/mock/sbin/entrypoint.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/tests/mock/sbin/mock_spark_server.py
--rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/tests/mock/sbin/start-connect-server.sh
--rw-r--r--   0        0        0    10147 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/.gitignore
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/LICENSE
--rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/README.md
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/pyproject.toml
--rw-r--r--   0        0        0     6204 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/PKG-INFO
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 sparglim-0.1.1/.dockerignore
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 sparglim-0.1.1/.editorconfig
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 sparglim-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 sparglim-0.1.1/RELEASE.md
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 sparglim-0.1.1/config-template.md
+-rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 sparglim-0.1.1/config.md
+-rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 sparglim-0.1.1/generate-config.sh
+-rwxr-xr-x   0        0        0     1828 2020-02-02 00:00:00.000000 sparglim-0.1.1/generate_config_docs.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 sparglim-0.1.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 sparglim-0.1.1/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 sparglim-0.1.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 sparglim-0.1.1/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/docker/Dockerfile.jupyterlab-sparglim
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/docker/Dockerfile.sparglim-server
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/jupyter-sparglim-on-k8s/README.md
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/jupyter-sparglim-on-k8s/k8s/deployment.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/jupyter-sparglim-on-k8s/k8s/headless-service.yaml
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/jupyter-sparglim-on-k8s/k8s/lab-service.yaml
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/jupyter-sparglim-sc/README.md
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/jupyter-sparglim-sc/k8s/jupyter-sparglim/deployment.yaml
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/jupyter-sparglim-sc/k8s/jupyter-sparglim/lab-service.yaml
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/jupyter-sparglim-sc/k8s/sparglim-server/connect-server-service.yaml
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/jupyter-sparglim-sc/k8s/sparglim-server/deployment.yaml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/jupyter-sparglim-sc/k8s/sparglim-server/headless-service.yaml
+-rwxr-xr-x   0        0        0      236 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/scripts/reload.sh
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/sparglim-server/README.md
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/sparglim-server/k8s/connect-server-service.yaml
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/sparglim-server/k8s/deployment.yaml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/sparglim-server/k8s/headless-service.yaml
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 sparglim-0.1.1/docker/Dockerfile.jupyterlab-sparglim
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 sparglim-0.1.1/docker/Dockerfile.sparglim-server
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 sparglim-0.1.1/examples/jupyter-sparglim-on-k8s/README.md
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 sparglim-0.1.1/examples/jupyter-sparglim-on-k8s/k8s/deployment.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sparglim-0.1.1/examples/jupyter-sparglim-on-k8s/k8s/headless-service.yaml
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 sparglim-0.1.1/examples/jupyter-sparglim-on-k8s/k8s/lab-service.yaml
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 sparglim-0.1.1/examples/jupyter-sparglim-sc/README.md
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 sparglim-0.1.1/examples/jupyter-sparglim-sc/k8s/jupyter-sparglim/deployment.yaml
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 sparglim-0.1.1/examples/jupyter-sparglim-sc/k8s/jupyter-sparglim/lab-service.yaml
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.1/examples/jupyter-sparglim-sc/k8s/sparglim-server/connect-server-service.yaml
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 sparglim-0.1.1/examples/jupyter-sparglim-sc/k8s/sparglim-server/deployment.yaml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.1/examples/jupyter-sparglim-sc/k8s/sparglim-server/headless-service.yaml
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 sparglim-0.1.1/examples/sparglim-server/README.md
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.1/examples/sparglim-server/k8s/connect-server-service.yaml
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 sparglim-0.1.1/examples/sparglim-server/k8s/deployment.yaml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.1/examples/sparglim-server/k8s/headless-service.yaml
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 sparglim-0.1.1/sparglim/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 sparglim-0.1.1/sparglim/exceptions.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 sparglim-0.1.1/sparglim/log.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.1/sparglim/py.typed
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 sparglim-0.1.1/sparglim/utils.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 sparglim-0.1.1/sparglim/config/__init__.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 sparglim-0.1.1/sparglim/config/builder.py
+-rw-r--r--   0        0        0    11844 2020-02-02 00:00:00.000000 sparglim-0.1.1/sparglim/config/configer.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 sparglim-0.1.1/sparglim/config/k8s.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 sparglim-0.1.1/sparglim/server/__init__.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 sparglim-0.1.1/sparglim/server/cli.py
+-rw-r--r--   0        0        0     8921 2020-02-02 00:00:00.000000 sparglim-0.1.1/sparglim/server/daemon.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 sparglim-0.1.1/sparglim/server/tailer.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 sparglim-0.1.1/sparglim/sql/__init__.py
+-rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 sparglim-0.1.1/sparglim/sql/magic.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 sparglim-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0     9525 2020-02-02 00:00:00.000000 sparglim-0.1.1/tests/test_builder.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 sparglim-0.1.1/tests/test_daemon.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 sparglim-0.1.1/tests/test_magic.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 sparglim-0.1.1/tests/example/people.json
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 sparglim-0.1.1/tests/mock/sbin/entrypoint.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 sparglim-0.1.1/tests/mock/sbin/mock_spark_server.py
+-rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 sparglim-0.1.1/tests/mock/sbin/start-connect-server.sh
+-rw-r--r--   0        0        0    10147 2020-02-02 00:00:00.000000 sparglim-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 sparglim-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 sparglim-0.1.1/README.md
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 sparglim-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 sparglim-0.1.1/PKG-INFO
```

### Comparing `sparglim-0.1.0rc6/.pre-commit-config.yaml` & `sparglim-0.1.1/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,17 @@
 repos:
+  # FIXME: This is slow and unreliable.
+  - repo: local
+    hooks:
+      - id: generate-config
+        name: Generate config
+        entry: ./generate-config.sh
+        language: system
+        verbose: true
+
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: end-of-file-fixer
       - id: check-case-conflict
       - id: check-executables-have-shebangs
       - id: requirements-txt-fixer
```

### Comparing `sparglim-0.1.0rc6/RELEASE.md` & `sparglim-0.1.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc6/.github/workflows/publish.yml` & `sparglim-0.1.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc6/.github/workflows/python-package.yml` & `sparglim-0.1.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc6/dev/docker/Dockerfile.jupyterlab-sparglim` & `sparglim-0.1.1/dev/docker/Dockerfile.jupyterlab-sparglim`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc6/dev/jupyter-sparglim-on-k8s/k8s/deployment.yaml` & `sparglim-0.1.1/dev/jupyter-sparglim-on-k8s/k8s/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc6/dev/jupyter-sparglim-sc/k8s/jupyter-sparglim/deployment.yaml` & `sparglim-0.1.1/dev/jupyter-sparglim-sc/k8s/jupyter-sparglim/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc6/dev/jupyter-sparglim-sc/k8s/sparglim-server/deployment.yaml` & `sparglim-0.1.1/dev/jupyter-sparglim-sc/k8s/sparglim-server/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc6/dev/sparglim-server/k8s/deployment.yaml` & `sparglim-0.1.1/dev/sparglim-server/k8s/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc6/examples/jupyter-sparglim-on-k8s/k8s/deployment.yaml` & `sparglim-0.1.1/examples/jupyter-sparglim-on-k8s/k8s/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc6/examples/jupyter-sparglim-sc/k8s/jupyter-sparglim/deployment.yaml` & `sparglim-0.1.1/examples/jupyter-sparglim-sc/k8s/jupyter-sparglim/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc6/examples/jupyter-sparglim-sc/k8s/sparglim-server/deployment.yaml` & `sparglim-0.1.1/examples/jupyter-sparglim-sc/k8s/sparglim-server/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc6/examples/sparglim-server/k8s/deployment.yaml` & `sparglim-0.1.1/examples/sparglim-server/k8s/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc6/sparglim/utils.py` & `sparglim-0.1.1/sparglim/utils.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc6/sparglim/config/builder.py` & `sparglim-0.1.1/sparglim/config/builder.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc6/sparglim/config/configer.py` & `sparglim-0.1.1/sparglim/config/configer.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,22 +121,21 @@
         "spark.executor.resource.gpu.amount": ("SPARGLIM_K8S_GPU_AMOUNT", None),
         "spark.rapids.sql.enabled": ("SPARGLIM_RAPIDS_SQL_ENABLED", None)
         # TODO: Mount config
         #       Given that it is highly customizable
         #       Not sure when it will be supported
         #       Welcome PR or discussion here!
     }
+    default_config_mapper = {
+        **_basic,
+        **_s3,
+        **_kerberos,
+    }
 
     def __init__(self) -> None:
-        self.default_config_mapper: ConfigEnvMapper = {
-            **self._basic,
-            **self._s3,
-            **self._kerberos,
-        }
-
         self._config: Config
         self.initialize()
 
     def initialize(self) -> None:
         self._config: Config = Config(self._config_from_env(self.default_config_mapper))
         logger.debug(f"Initialized config: {self._config}")
 
@@ -187,14 +186,25 @@
             {
                 **self._config_from_env(self._s3),
                 **custom_config,
             }
         )
         return self
 
+    def config_kerberos(self, custom_config: Optional[Dict[str, Any]] = None) -> SparkEnvConfiger:
+        if not custom_config:
+            custom_config = dict()
+        self.config(
+            {
+                **self._config_from_env(self._kerberos),
+                **custom_config,
+            }
+        )
+        return self
+
     def config_local(self, custom_config: Optional[Dict[str, Any]] = None) -> SparkEnvConfiger:
         logger.info(f"Config master: local mode")
         if not custom_config:
             custom_config = dict()
         self.config(
             {
                 **self._config_from_env(self._local),
```

### Comparing `sparglim-0.1.0rc6/sparglim/config/k8s.py` & `sparglim-0.1.1/sparglim/config/k8s.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc6/sparglim/server/cli.py` & `sparglim-0.1.1/sparglim/server/cli.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc6/sparglim/server/daemon.py` & `sparglim-0.1.1/sparglim/server/daemon.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc6/sparglim/server/tailer.py` & `sparglim-0.1.1/sparglim/server/tailer.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc6/sparglim/sql/magic.py` & `sparglim-0.1.1/sparglim/sql/magic.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc6/tests/conftest.py` & `sparglim-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc6/tests/test_builder.py` & `sparglim-0.1.1/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc6/tests/test_daemon.py` & `sparglim-0.1.1/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc6/tests/test_magic.py` & `sparglim-0.1.1/tests/test_magic.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc6/tests/mock/sbin/entrypoint.py` & `sparglim-0.1.1/tests/mock/sbin/entrypoint.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc6/tests/mock/sbin/mock_spark_server.py` & `sparglim-0.1.1/tests/mock/sbin/mock_spark_server.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc6/.gitignore` & `sparglim-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc6/LICENSE` & `sparglim-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc6/README.md` & `sparglim-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 ![](https://img.shields.io/github/license/wh1isper/sparglim)
 ![](https://img.shields.io/github/v/release/wh1isper/sparglim?logo=github)
 ![](https://img.shields.io/github/v/release/wh1isper/sparglim?include_prereleases&label=pre-release&logo=github)
 ![](https://img.shields.io/pypi/dm/sparglim)
 ![](https://img.shields.io/github/last-commit/wh1isper/sparglim)
 ![](https://img.shields.io/pypi/pyversions/sparglim)
 
-# Sparglim
+# Sparglim ✨
 
 Sparglim is aimed at providing a clean solution for PySpark applications in cloud-native scenarios (On K8S、Connect Server etc.).
 
+**This is a fledgling project, looking forward to any PRs, Feature Requests and Discussions!**
+
+🌟✨⭐ Start to support!
+
 ## Quick Start
 
 Run Jupyterlab with `sparglim` docker image:
 
 ```bash
 docker run \
 -it \
@@ -52,15 +56,15 @@
 
 ## User cases
 
 ### PySpark App
 
 To config Spark on k8s for Data explorations, see [examples/jupyter-sparglim-on-k8s](./examples/jupyter-sparglim-on-k8s)
 
-To config Spark for ELT Application/Service, see [pyspark-sampling](https://github.com/Wh1isper/pyspark-sampling/)
+*TODO: To config Spark for ELT Application/Service, see [pyspark-sampling](https://github.com/Wh1isper/pyspark-sampling/)*
 
 ### Spark Connect Server on K8S
 
 To daemon Spark Connect Server on K8S, see [examples/sparglim-server](./examples/sparglim-server)
 
 To daemon Spark Connect Server on K8S and Connect it in JupyterLab , see [examples/jupyter-sparglim-sc](./examples/jupyter-sparglim-sc)
```

### Comparing `sparglim-0.1.0rc6/pyproject.toml` & `sparglim-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sparglim"
 description = "sparglim"
-keywords = ["sparglim"]
+keywords = ["sparglim", "pyspark", "magic", "ipython", "spark"]
 requires-python = ">=3.8"
 dependencies = ["loguru", "click", "findspark", "psutil", "kubernetes"]
 dynamic = ["version"]
 classifiers = [
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
```

### Comparing `sparglim-0.1.0rc6/PKG-INFO` & `sparglim-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sparglim
-Version: 0.1.0rc6
+Version: 0.1.1
 Summary: sparglim
 Project-URL: Source, https://github.com/wh1isper/sparglim
 Author-email: wh1isper <9573586@qq.com>
 License: BSD license
 License-File: LICENSE
-Keywords: sparglim
+Keywords: ipython,magic,pyspark,sparglim,spark
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Requires-Dist: click
@@ -39,18 +39,22 @@
 ![](https://img.shields.io/github/license/wh1isper/sparglim)
 ![](https://img.shields.io/github/v/release/wh1isper/sparglim?logo=github)
 ![](https://img.shields.io/github/v/release/wh1isper/sparglim?include_prereleases&label=pre-release&logo=github)
 ![](https://img.shields.io/pypi/dm/sparglim)
 ![](https://img.shields.io/github/last-commit/wh1isper/sparglim)
 ![](https://img.shields.io/pypi/pyversions/sparglim)
 
-# Sparglim
+# Sparglim ✨
 
 Sparglim is aimed at providing a clean solution for PySpark applications in cloud-native scenarios (On K8S、Connect Server etc.).
 
+**This is a fledgling project, looking forward to any PRs, Feature Requests and Discussions!**
+
+🌟✨⭐ Start to support!
+
 ## Quick Start
 
 Run Jupyterlab with `sparglim` docker image:
 
 ```bash
 docker run \
 -it \
@@ -90,15 +94,15 @@
 
 ## User cases
 
 ### PySpark App
 
 To config Spark on k8s for Data explorations, see [examples/jupyter-sparglim-on-k8s](./examples/jupyter-sparglim-on-k8s)
 
-To config Spark for ELT Application/Service, see [pyspark-sampling](https://github.com/Wh1isper/pyspark-sampling/)
+*TODO: To config Spark for ELT Application/Service, see [pyspark-sampling](https://github.com/Wh1isper/pyspark-sampling/)*
 
 ### Spark Connect Server on K8S
 
 To daemon Spark Connect Server on K8S, see [examples/sparglim-server](./examples/sparglim-server)
 
 To daemon Spark Connect Server on K8S and Connect it in JupyterLab , see [examples/jupyter-sparglim-sc](./examples/jupyter-sparglim-sc)
```

