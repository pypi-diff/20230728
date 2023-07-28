# Comparing `tmp/adafruit-circuitpython-minimqtt-7.4.0.tar.gz` & `tmp/adafruit-circuitpython-minimqtt-7.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-minimqtt-7.4.0.tar", last modified: Sat Jul  8 14:23:05 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-minimqtt-7.4.1.tar", last modified: Fri Jul 28 04:54:42 2023, max compression
```

## Comparing `adafruit-circuitpython-minimqtt-7.4.0.tar` & `adafruit-circuitpython-minimqtt-7.4.1.tar`

### file list

```diff
@@ -1,76 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.248154 adafruit-circuitpython-minimqtt-7.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.232154 adafruit-circuitpython-minimqtt-7.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.236154 adafruit-circuitpython-minimqtt-7.4.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.236154 adafruit-circuitpython-minimqtt-7.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.236154 adafruit-circuitpython-minimqtt-7.4.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/LICENSES/EPL-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-08 14:23:05.248154 adafruit-circuitpython-minimqtt-7.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.240154 adafruit-circuitpython-minimqtt-7.4.0/adafruit_circuitpython_minimqtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-08 14:23:05.000000 adafruit-circuitpython-minimqtt-7.4.0/adafruit_circuitpython_minimqtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-08 14:23:05.000000 adafruit-circuitpython-minimqtt-7.4.0/adafruit_circuitpython_minimqtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 14:23:05.000000 adafruit-circuitpython-minimqtt-7.4.0/adafruit_circuitpython_minimqtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-08 14:23:05.000000 adafruit-circuitpython-minimqtt-7.4.0/adafruit_circuitpython_minimqtt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-08 14:23:05.000000 adafruit-circuitpython-minimqtt-7.4.0/adafruit_circuitpython_minimqtt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.240154 adafruit-circuitpython-minimqtt-7.4.0/adafruit_minimqtt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/adafruit_minimqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45757 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/adafruit_minimqtt/adafruit_minimqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/adafruit_minimqtt/matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.240154 adafruit-circuitpython-minimqtt-7.4.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.244154 adafruit-circuitpython-minimqtt-7.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.244154 adafruit-circuitpython-minimqtt-7.4.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.244154 adafruit-circuitpython-minimqtt-7.4.0/examples/cellular/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3034 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/cellular/minimqtt_adafruitio_cellular.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/cellular/minimqtt_simpletest_cellular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.244154 adafruit-circuitpython-minimqtt-7.4.0/examples/cpython/
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/cpython/minimqtt_adafruitio_cpython.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/cpython/minimqtt_simpletest_cpython.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.248154 adafruit-circuitpython-minimqtt-7.4.0/examples/esp32spi/
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/esp32spi/minimqtt_adafruitio_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/esp32spi/minimqtt_certificate_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/esp32spi/minimqtt_pub_sub_blocking_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/esp32spi/minimqtt_pub_sub_blocking_topic_callbacks_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/esp32spi/minimqtt_pub_sub_nonblocking_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/esp32spi/minimqtt_pub_sub_pyportal_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/esp32spi/minimqtt_simpletest_esp32spi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.248154 adafruit-circuitpython-minimqtt-7.4.0/examples/ethernet/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2608 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/ethernet/minimqtt_adafruitio_eth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/ethernet/minimqtt_simpletest_eth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/minimqtt_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.248154 adafruit-circuitpython-minimqtt-7.4.0/examples/native_networking/
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/native_networking/minimqtt_adafruitio_native_networking.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/native_networking/minimqtt_pub_sub_blocking_native_networking.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/native_networking/minimqtt_pub_sub_blocking_topic_callbacks_native_networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 14:23:05.248154 adafruit-circuitpython-minimqtt-7.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.248154 adafruit-circuitpython-minimqtt-7.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/tests/backoff_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/tests/test_port_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:54:42.649945 adafruit-circuitpython-minimqtt-7.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:54:42.633945 adafruit-circuitpython-minimqtt-7.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:54:42.637945 adafruit-circuitpython-minimqtt-7.4.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-28 04:54:23.000000 adafruit-circuitpython-minimqtt-7.4.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:54:42.641945 adafruit-circuitpython-minimqtt-7.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-28 04:54:23.000000 adafruit-circuitpython-minimqtt-7.4.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-28 04:54:23.000000 adafruit-circuitpython-minimqtt-7.4.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-28 04:54:23.000000 adafruit-circuitpython-minimqtt-7.4.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-28 04:54:23.000000 adafruit-circuitpython-minimqtt-7.4.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-28 04:54:23.000000 adafruit-circuitpython-minimqtt-7.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-28 04:54:23.000000 adafruit-circuitpython-minimqtt-7.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-28 04:54:23.000000 adafruit-circuitpython-minimqtt-7.4.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-28 04:54:23.000000 adafruit-circuitpython-minimqtt-7.4.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-07-28 04:54:23.000000 adafruit-circuitpython-minimqtt-7.4.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-28 04:54:23.000000 adafruit-circuitpython-minimqtt-7.4.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:54:42.641945 adafruit-circuitpython-minimqtt-7.4.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-07-28 04:54:23.000000 adafruit-circuitpython-minimqtt-7.4.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-07-28 04:54:23.000000 adafruit-circuitpython-minimqtt-7.4.1/LICENSES/EPL-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-28 04:54:23.000000 adafruit-circuitpython-minimqtt-7.4.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-28 04:54:23.000000 adafruit-circuitpython-minimqtt-7.4.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-28 04:54:42.649945 adafruit-circuitpython-minimqtt-7.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-07-28 04:54:23.000000 adafruit-circuitpython-minimqtt-7.4.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-28 04:54:23.000000 adafruit-circuitpython-minimqtt-7.4.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:54:42.641945 adafruit-circuitpython-minimqtt-7.4.1/adafruit_circuitpython_minimqtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-28 04:54:42.000000 adafruit-circuitpython-minimqtt-7.4.1/adafruit_circuitpython_minimqtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-28 04:54:42.000000 adafruit-circuitpython-minimqtt-7.4.1/adafruit_circuitpython_minimqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 04:54:42.000000 adafruit-circuitpython-minimqtt-7.4.1/adafruit_circuitpython_minimqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 04:54:42.000000 adafruit-circuitpython-minimqtt-7.4.1/adafruit_circuitpython_minimqtt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 04:54:42.000000 adafruit-circuitpython-minimqtt-7.4.1/adafruit_circuitpython_minimqtt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:54:42.641945 adafruit-circuitpython-minimqtt-7.4.1/adafruit_minimqtt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 04:54:34.000000 adafruit-circuitpython-minimqtt-7.4.1/adafruit_minimqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45757 2023-07-28 04:54:34.000000 adafruit-circuitpython-minimqtt-7.4.1/adafruit_minimqtt/adafruit_minimqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-28 04:54:34.000000 adafruit-circuitpython-minimqtt-7.4.1/adafruit_minimqtt/matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:54:42.641945 adafruit-circuitpython-minimqtt-7.4.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:54:42.645945 adafruit-circuitpython-minimqtt-7.4.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-28 04:54:23.000000 adafruit-circuitpython-minimqtt-7.4.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-28 04:54:23.000000 adafruit-circuitpython-minimqtt-7.4.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-28 04:54:23.000000 adafruit-circuitpython-minimqtt-7.4.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-28 04:54:23.000000 adafruit-circuitpython-minimqtt-7.4.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-07-28 04:54:23.000000 adafruit-circuitpython-minimqtt-7.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-28 04:54:23.000000 adafruit-circuitpython-minimqtt-7.4.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-28 04:54:23.000000 adafruit-circuitpython-minimqtt-7.4.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-28 04:54:23.000000 adafruit-circuitpython-minimqtt-7.4.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-28 04:54:23.000000 adafruit-circuitpython-minimqtt-7.4.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-28 04:54:23.000000 adafruit-circuitpython-minimqtt-7.4.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:54:42.645945 adafruit-circuitpython-minimqtt-7.4.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:54:42.645945 adafruit-circuitpython-minimqtt-7.4.1/examples/cellular/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3034 2023-07-28 04:54:34.000000 adafruit-circuitpython-minimqtt-7.4.1/examples/cellular/minimqtt_adafruitio_cellular.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-28 04:54:34.000000 adafruit-circuitpython-minimqtt-7.4.1/examples/cellular/minimqtt_simpletest_cellular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:54:42.645945 adafruit-circuitpython-minimqtt-7.4.1/examples/cpython/
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-28 04:54:34.000000 adafruit-circuitpython-minimqtt-7.4.1/examples/cpython/minimqtt_adafruitio_cpython.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-28 04:54:34.000000 adafruit-circuitpython-minimqtt-7.4.1/examples/cpython/minimqtt_simpletest_cpython.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:54:42.645945 adafruit-circuitpython-minimqtt-7.4.1/examples/esp32spi/
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-28 04:54:34.000000 adafruit-circuitpython-minimqtt-7.4.1/examples/esp32spi/minimqtt_adafruitio_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-07-28 04:54:34.000000 adafruit-circuitpython-minimqtt-7.4.1/examples/esp32spi/minimqtt_certificate_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-28 04:54:34.000000 adafruit-circuitpython-minimqtt-7.4.1/examples/esp32spi/minimqtt_pub_sub_blocking_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-28 04:54:34.000000 adafruit-circuitpython-minimqtt-7.4.1/examples/esp32spi/minimqtt_pub_sub_blocking_topic_callbacks_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-28 04:54:34.000000 adafruit-circuitpython-minimqtt-7.4.1/examples/esp32spi/minimqtt_pub_sub_nonblocking_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-28 04:54:34.000000 adafruit-circuitpython-minimqtt-7.4.1/examples/esp32spi/minimqtt_pub_sub_pyportal_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-07-28 04:54:34.000000 adafruit-circuitpython-minimqtt-7.4.1/examples/esp32spi/minimqtt_simpletest_esp32spi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:54:42.645945 adafruit-circuitpython-minimqtt-7.4.1/examples/ethernet/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2608 2023-07-28 04:54:34.000000 adafruit-circuitpython-minimqtt-7.4.1/examples/ethernet/minimqtt_adafruitio_eth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-28 04:54:34.000000 adafruit-circuitpython-minimqtt-7.4.1/examples/ethernet/minimqtt_simpletest_eth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-28 04:54:34.000000 adafruit-circuitpython-minimqtt-7.4.1/examples/minimqtt_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:54:42.645945 adafruit-circuitpython-minimqtt-7.4.1/examples/native_networking/
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-28 04:54:34.000000 adafruit-circuitpython-minimqtt-7.4.1/examples/native_networking/minimqtt_adafruitio_native_networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-28 04:54:34.000000 adafruit-circuitpython-minimqtt-7.4.1/examples/native_networking/minimqtt_pub_sub_blocking_native_networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-28 04:54:34.000000 adafruit-circuitpython-minimqtt-7.4.1/examples/native_networking/minimqtt_pub_sub_blocking_topic_callbacks_native_networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-28 04:54:23.000000 adafruit-circuitpython-minimqtt-7.4.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-28 04:54:34.000000 adafruit-circuitpython-minimqtt-7.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-28 04:54:23.000000 adafruit-circuitpython-minimqtt-7.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 04:54:42.649945 adafruit-circuitpython-minimqtt-7.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:54:42.649945 adafruit-circuitpython-minimqtt-7.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-28 04:54:34.000000 adafruit-circuitpython-minimqtt-7.4.1/tests/backoff_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-28 04:54:34.000000 adafruit-circuitpython-minimqtt-7.4.1/tests/test_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-07-28 04:54:34.000000 adafruit-circuitpython-minimqtt-7.4.1/tests/test_port_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-28 04:54:23.000000 adafruit-circuitpython-minimqtt-7.4.1/tox.ini
```

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-minimqtt-7.4.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/.gitignore` & `adafruit-circuitpython-minimqtt-7.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/.pre-commit-config.yaml` & `adafruit-circuitpython-minimqtt-7.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/.pylintrc` & `adafruit-circuitpython-minimqtt-7.4.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-minimqtt-7.4.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/LICENSE` & `adafruit-circuitpython-minimqtt-7.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-minimqtt-7.4.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/LICENSES/EPL-1.0.txt` & `adafruit-circuitpython-minimqtt-7.4.1/LICENSES/EPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/LICENSES/MIT.txt` & `adafruit-circuitpython-minimqtt-7.4.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-minimqtt-7.4.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/PKG-INFO` & `adafruit-circuitpython-minimqtt-7.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-minimqtt
-Version: 7.4.0
+Version: 7.4.1
 Summary: MQTT client library for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MiniMQTT
 Keywords: adafruit,blinka,circuitpython,micropython,minimqtt,mqtt,,client,,socket
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/README.rst` & `adafruit-circuitpython-minimqtt-7.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/adafruit_circuitpython_minimqtt.egg-info/PKG-INFO` & `adafruit-circuitpython-minimqtt-7.4.1/adafruit_circuitpython_minimqtt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-minimqtt
-Version: 7.4.0
+Version: 7.4.1
 Summary: MQTT client library for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MiniMQTT
 Keywords: adafruit,blinka,circuitpython,micropython,minimqtt,mqtt,,client,,socket
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/adafruit_circuitpython_minimqtt.egg-info/SOURCES.txt` & `adafruit-circuitpython-minimqtt-7.4.1/adafruit_circuitpython_minimqtt.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -51,8 +51,9 @@
 examples/esp32spi/minimqtt_simpletest_esp32spi.py
 examples/ethernet/minimqtt_adafruitio_eth.py
 examples/ethernet/minimqtt_simpletest_eth.py
 examples/native_networking/minimqtt_adafruitio_native_networking.py
 examples/native_networking/minimqtt_pub_sub_blocking_native_networking.py
 examples/native_networking/minimqtt_pub_sub_blocking_topic_callbacks_native_networking.py
 tests/backoff_test.py
+tests/test_loop.py
 tests/test_port_ssl.py
```

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/adafruit_minimqtt/adafruit_minimqtt.py` & `adafruit-circuitpython-minimqtt-7.4.1/adafruit_minimqtt/adafruit_minimqtt.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 except ImportError:
     pass
 
 from micropython import const
 
 from .matcher import MQTTMatcher
 
-__version__ = "7.4.0"
+__version__ = "7.4.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MiniMQTT.git"
 
 # Client-specific variables
 MQTT_MSG_MAX_SZ = const(268435455)
 MQTT_MSG_SZ_LIM = const(10000000)
 MQTT_TOPIC_LENGTH_LIMIT = const(65535)
 MQTT_TCP_PORT = const(1883)
```

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/adafruit_minimqtt/matcher.py` & `adafruit-circuitpython-minimqtt-7.4.1/adafruit_minimqtt/matcher.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/docs/_static/favicon.ico` & `adafruit-circuitpython-minimqtt-7.4.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/docs/conf.py` & `adafruit-circuitpython-minimqtt-7.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/docs/index.rst` & `adafruit-circuitpython-minimqtt-7.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/examples/cellular/minimqtt_adafruitio_cellular.py` & `adafruit-circuitpython-minimqtt-7.4.1/examples/cellular/minimqtt_adafruitio_cellular.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/examples/cellular/minimqtt_simpletest_cellular.py` & `adafruit-circuitpython-minimqtt-7.4.1/examples/cellular/minimqtt_simpletest_cellular.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/examples/cpython/minimqtt_adafruitio_cpython.py` & `adafruit-circuitpython-minimqtt-7.4.1/examples/cpython/minimqtt_adafruitio_cpython.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/examples/cpython/minimqtt_simpletest_cpython.py` & `adafruit-circuitpython-minimqtt-7.4.1/examples/cpython/minimqtt_simpletest_cpython.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/examples/esp32spi/minimqtt_adafruitio_esp32spi.py` & `adafruit-circuitpython-minimqtt-7.4.1/examples/esp32spi/minimqtt_adafruitio_esp32spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/examples/esp32spi/minimqtt_certificate_esp32spi.py` & `adafruit-circuitpython-minimqtt-7.4.1/examples/esp32spi/minimqtt_certificate_esp32spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/examples/esp32spi/minimqtt_pub_sub_blocking_esp32spi.py` & `adafruit-circuitpython-minimqtt-7.4.1/examples/esp32spi/minimqtt_pub_sub_blocking_esp32spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/examples/esp32spi/minimqtt_pub_sub_blocking_topic_callbacks_esp32spi.py` & `adafruit-circuitpython-minimqtt-7.4.1/examples/esp32spi/minimqtt_pub_sub_blocking_topic_callbacks_esp32spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/examples/esp32spi/minimqtt_pub_sub_nonblocking_esp32spi.py` & `adafruit-circuitpython-minimqtt-7.4.1/examples/esp32spi/minimqtt_pub_sub_nonblocking_esp32spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/examples/esp32spi/minimqtt_pub_sub_pyportal_esp32spi.py` & `adafruit-circuitpython-minimqtt-7.4.1/examples/esp32spi/minimqtt_pub_sub_pyportal_esp32spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/examples/esp32spi/minimqtt_simpletest_esp32spi.py` & `adafruit-circuitpython-minimqtt-7.4.1/examples/esp32spi/minimqtt_simpletest_esp32spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/examples/ethernet/minimqtt_adafruitio_eth.py` & `adafruit-circuitpython-minimqtt-7.4.1/examples/ethernet/minimqtt_adafruitio_eth.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/examples/ethernet/minimqtt_simpletest_eth.py` & `adafruit-circuitpython-minimqtt-7.4.1/examples/ethernet/minimqtt_simpletest_eth.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/examples/minimqtt_simpletest.py` & `adafruit-circuitpython-minimqtt-7.4.1/examples/minimqtt_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/examples/native_networking/minimqtt_adafruitio_native_networking.py` & `adafruit-circuitpython-minimqtt-7.4.1/examples/native_networking/minimqtt_adafruitio_native_networking.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/examples/native_networking/minimqtt_pub_sub_blocking_native_networking.py` & `adafruit-circuitpython-minimqtt-7.4.1/examples/native_networking/minimqtt_pub_sub_blocking_native_networking.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/examples/native_networking/minimqtt_pub_sub_blocking_topic_callbacks_native_networking.py` & `adafruit-circuitpython-minimqtt-7.4.1/examples/native_networking/minimqtt_pub_sub_blocking_topic_callbacks_native_networking.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/pyproject.toml` & `adafruit-circuitpython-minimqtt-7.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-minimqtt"
 description = "MQTT client library for CircuitPython"
-version = "7.4.0"
+version = "7.4.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_MiniMQTT"}
 keywords = [
     "adafruit",
```

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/tests/backoff_test.py` & `adafruit-circuitpython-minimqtt-7.4.1/tests/backoff_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.4.0/tests/test_port_ssl.py` & `adafruit-circuitpython-minimqtt-7.4.1/tests/test_port_ssl.py`

 * *Files identical despite different names*

