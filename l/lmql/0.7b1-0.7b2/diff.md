# Comparing `tmp/lmql-0.7b1.tar.gz` & `tmp/lmql-0.7b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmql-0.7b1.tar", last modified: Tue Jul 25 15:21:24 2023, max compression
+gzip compressed data, was "lmql-0.7b2.tar", last modified: Fri Jul 28 19:02:16 2023, max compression
```

## Comparing `lmql-0.7b1.tar` & `lmql-0.7b2.tar`

### file list

```diff
@@ -1,350 +1,358 @@
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.281753 lmql-0.7b1/
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.237754 lmql-0.7b1/.github/
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.241754 lmql-0.7b1/.github/workflows/
--rw-r--r--   0 docker    (1000) docker    (1000)     2590 2023-07-14 15:52:52.000000 lmql-0.7b1/.github/workflows/lmql-ci.yml
--rw-r--r--   0 docker    (1000) docker    (1000)     1543 2023-07-14 11:33:53.000000 lmql-0.7b1/.github/workflows/lmql-tests.yml
--rw-r--r--   0 docker    (1000) docker    (1000)     2372 2023-07-25 13:45:45.000000 lmql-0.7b1/.github/workflows/lmql-web.yml
--rw-r--r--   0 docker    (1000) docker    (1000)     2743 2023-07-14 11:31:18.000000 lmql-0.7b1/.gitignore
--rw-r--r--   0 docker    (1000) docker    (1000)    23151 2023-07-14 11:31:18.000000 lmql-0.7b1/LICENSE
--rw-r--r--   0 docker    (1000) docker    (1000)      140 2023-07-14 11:31:18.000000 lmql-0.7b1/MANIFEST.in
--rw-r--r--   0 docker    (1000) docker    (1000)     9896 2023-07-25 15:21:24.281753 lmql-0.7b1/PKG-INFO
--rw-r--r--   0 docker    (1000) docker    (1000)     9448 2023-07-14 15:36:31.000000 lmql-0.7b1/README.md
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.241754 lmql-0.7b1/docs/
--rw-r--r--   0 docker    (1000) docker    (1000)      638 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/Makefile
--rw-r--r--   0 docker    (1000) docker    (1000)      444 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/RELEASE.md
--rw-r--r--   0 docker    (1000) docker    (1000)      799 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/make.bat
--rw-r--r--   0 docker    (1000) docker    (1000)       81 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/requirements.txt
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.245754 lmql-0.7b1/docs/source/
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.245754 lmql-0.7b1/docs/source/_ext/
--rw-r--r--   0 docker    (1000) docker    (1000)     5728 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/_ext/lmql_snippets.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.237754 lmql-0.7b1/docs/source/_static/
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.245754 lmql-0.7b1/docs/source/_static/css/
--rw-r--r--   0 docker    (1000) docker    (1000)     6010 2023-07-14 15:36:31.000000 lmql-0.7b1/docs/source/_static/css/lmql-docs.css
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.245754 lmql-0.7b1/docs/source/_static/images/
--rw-r--r--   0 docker    (1000) docker    (1000)     3675 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/_static/images/lmql.svg
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.245754 lmql-0.7b1/docs/source/_static/js/
--rw-r--r--   0 docker    (1000) docker    (1000)     2087 2023-07-14 15:36:31.000000 lmql-0.7b1/docs/source/_static/js/lmql-playground.js
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.245754 lmql-0.7b1/docs/source/_templates/
--rw-r--r--   0 docker    (1000) docker    (1000)      292 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/_templates/layout.html
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.245754 lmql-0.7b1/docs/source/blog/
--rw-r--r--   0 docker    (1000) docker    (1000)     4591 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/blog/release-0.0.5.md
--rw-r--r--   0 docker    (1000) docker    (1000)     1444 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/blog/release-0.0.6.1.md
--rw-r--r--   0 docker    (1000) docker    (1000)     2068 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/blog/release-0.0.6.3.md
--rw-r--r--   0 docker    (1000) docker    (1000)     3221 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/blog/release-0.0.6.4.md
--rw-r--r--   0 docker    (1000) docker    (1000)     5872 2023-07-20 09:50:34.000000 lmql-0.7b1/docs/source/blog/release-0.0.6.5.md
--rw-r--r--   0 docker    (1000) docker    (1000)     1445 2023-07-25 13:45:45.000000 lmql-0.7b1/docs/source/blog/release-0.0.6.6.md
--rw-r--r--   0 docker    (1000) docker    (1000)     8976 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/blog/release-0.0.6.md
--rw-r--r--   0 docker    (1000) docker    (1000)     1167 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/conf.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1293 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/dev-setup.md
--rw-r--r--   0 docker    (1000) docker    (1000)     2333 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/docker-setup.md
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.245754 lmql-0.7b1/docs/source/images/
--rw-r--r--   0 docker    (1000) docker    (1000)   125712 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/images/inference.svg
--rw-r--r--   0 docker    (1000) docker    (1000)     2823 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/index.rst
--rw-r--r--   0 docker    (1000) docker    (1000)     2563 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/installation.md
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.245754 lmql-0.7b1/docs/source/language/
--rw-r--r--   0 docker    (1000) docker    (1000)     2313 2023-07-14 15:36:31.000000 lmql-0.7b1/docs/source/language/azure.md
--rw-r--r--   0 docker    (1000) docker    (1000)     7435 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/language/constraints.md
--rw-r--r--   0 docker    (1000) docker    (1000)     5365 2023-07-14 15:36:31.000000 lmql-0.7b1/docs/source/language/decoders.md
--rw-r--r--   0 docker    (1000) docker    (1000)     7850 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/language/functions.md
--rw-r--r--   0 docker    (1000) docker    (1000)     3967 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/language/hf.md
--rw-r--r--   0 docker    (1000) docker    (1000)     2027 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/language/llama.cpp.md
--rw-r--r--   0 docker    (1000) docker    (1000)     2896 2023-07-14 15:36:31.000000 lmql-0.7b1/docs/source/language/models.md
--rw-r--r--   0 docker    (1000) docker    (1000)     5710 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/language/openai.md
--rw-r--r--   0 docker    (1000) docker    (1000)     8292 2023-07-14 15:36:31.000000 lmql-0.7b1/docs/source/language/overview.md
--rw-r--r--   0 docker    (1000) docker    (1000)     6032 2023-07-20 09:50:34.000000 lmql-0.7b1/docs/source/language/scripted_prompts.md
--rw-r--r--   0 docker    (1000) docker    (1000)     3675 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/lmql.svg
--rw-r--r--   0 docker    (1000) docker    (1000)    28444 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/logo.png
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.245754 lmql-0.7b1/docs/source/pending/
--rw-r--r--   0 docker    (1000) docker    (1000)     3550 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/pending/release-next.md
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.249754 lmql-0.7b1/docs/source/python/
--rw-r--r--   0 docker    (1000) docker    (1000)       11 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/python/.gitignore
--rw-r--r--   0 docker    (1000) docker    (1000)     4924 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/python/comparison.md
--rw-r--r--   0 docker    (1000) docker    (1000)    11193 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/python/langchain.ipynb
--rw-r--r--   0 docker    (1000) docker    (1000)     1157 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/python/lc.py
--rw-r--r--   0 docker    (1000) docker    (1000)     6681 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/python/llama_index.ipynb
--rw-r--r--   0 docker    (1000) docker    (1000)    75148 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/python/lmql.txt
--rw-r--r--   0 docker    (1000) docker    (1000)     7458 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/python/output.ipynb
--rw-r--r--   0 docker    (1000) docker    (1000)     9592 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/python/pandas.ipynb
--rw-r--r--   0 docker    (1000) docker    (1000)    13317 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/python/python.ipynb
--rw-r--r--   0 docker    (1000) docker    (1000)     4806 2023-07-14 15:36:31.000000 lmql-0.7b1/docs/source/quickstart.md
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.249754 lmql-0.7b1/docs/source/releases/
--rw-r--r--   0 docker    (1000) docker    (1000)     2263 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/releases/misc-snippets.md
--rw-r--r--   0 docker    (1000) docker    (1000)      321 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/source/releases/release-0.0.5.md
--rw-r--r--   0 docker    (1000) docker    (1000)      257 2023-07-14 11:31:18.000000 lmql-0.7b1/docs/todo.md
--rw-r--r--   0 docker    (1000) docker    (1000)      137 2023-07-14 11:31:18.000000 lmql-0.7b1/pyproject.toml
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.249754 lmql-0.7b1/scripts/
--rw-r--r--   0 docker    (1000) docker    (1000)      577 2023-07-14 11:31:18.000000 lmql-0.7b1/scripts/Dockerfile
--rw-r--r--   0 docker    (1000) docker    (1000)      295 2023-07-14 11:31:18.000000 lmql-0.7b1/scripts/activate-dev.sh
--rw-r--r--   0 docker    (1000) docker    (1000)      357 2023-07-25 13:45:45.000000 lmql-0.7b1/scripts/changelog.sh
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.249754 lmql-0.7b1/scripts/conda/
--rw-r--r--   0 docker    (1000) docker    (1000)      198 2023-07-14 11:31:18.000000 lmql-0.7b1/scripts/conda/requirements-no-gpu.yml
--rw-r--r--   0 docker    (1000) docker    (1000)      332 2023-07-14 11:31:18.000000 lmql-0.7b1/scripts/conda/requirements.yml
--rw-r--r--   0 docker    (1000) docker    (1000)      638 2023-07-14 11:31:18.000000 lmql-0.7b1/scripts/pypi-release.sh
--rw-r--r--   0 docker    (1000) docker    (1000)     3897 2023-07-14 11:31:18.000000 lmql-0.7b1/scripts/serve-all.py
--rw-r--r--   0 docker    (1000) docker    (1000)      854 2023-07-14 11:31:18.000000 lmql-0.7b1/scripts/wheel.sh
--rw-r--r--   0 docker    (1000) docker    (1000)      866 2023-07-25 15:21:24.281753 lmql-0.7b1/setup.cfg
--rw-r--r--   0 docker    (1000) docker    (1000)       37 2023-07-14 11:31:18.000000 lmql-0.7b1/setup.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.249754 lmql-0.7b1/src/
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.249754 lmql-0.7b1/src/lmql/
--rw-r--r--   0 docker    (1000) docker    (1000)        6 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/.gitignore
--rw-r--r--   0 docker    (1000) docker    (1000)     8078 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/__init__.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.249754 lmql-0.7b1/src/lmql/algorithms/
--rw-r--r--   0 docker    (1000) docker    (1000)       45 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/algorithms/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2763 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/algorithms/cache.py
--rw-r--r--   0 docker    (1000) docker    (1000)      942 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/algorithms/functools.py
--rwxr-xr-x   0 docker    (1000) docker    (1000)     8644 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/cli.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1577 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/demo.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1531 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/http.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.253754 lmql-0.7b1/src/lmql/language/
--rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/language/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)    32080 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/language/compiler.py
--rw-r--r--   0 docker    (1000) docker    (1000)    11442 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/language/fragment_parser.py
--rw-r--r--   0 docker    (1000) docker    (1000)     4700 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/language/qstrings.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1804 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/language/validator.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.253754 lmql-0.7b1/src/lmql/lib/
--rw-r--r--   0 docker    (1000) docker    (1000)      143 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/lib/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)    12764 2023-07-25 15:16:34.000000 lmql-0.7b1/src/lmql/lib/actions.py
--rw-r--r--   0 docker    (1000) docker    (1000)    61974 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/lib/algebra222.csv
--rw-r--r--   0 docker    (1000) docker    (1000)     5225 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/lib/data.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.253754 lmql-0.7b1/src/lmql/lib/prompts/
--rw-r--r--   0 docker    (1000) docker    (1000)     1682 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/lib/prompts/inline_code copy.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1625 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/lib/prompts/inline_code.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1450 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/lib/prompts/inline_use.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1694 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/lib/prompts/inline_use_kevin.py
--rw-r--r--   0 docker    (1000) docker    (1000)     5900 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/lib/prompts/wiki_prompt.py
--rw-r--r--   0 docker    (1000) docker    (1000)     7473 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/lib/types.py
--rw-r--r--   0 docker    (1000) docker    (1000)      942 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/lib/value.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.253754 lmql-0.7b1/src/lmql/models/
--rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/models/__init__.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.253754 lmql-0.7b1/src/lmql/models/lmtp/
--rw-r--r--   0 docker    (1000) docker    (1000)     6156 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/models/lmtp/README.md
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.253754 lmql-0.7b1/src/lmql/models/lmtp/backends/
--rw-r--r--   0 docker    (1000) docker    (1000)      493 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/models/lmtp/backends/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)      694 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/models/lmtp/backends/__main__.py
--rw-r--r--   0 docker    (1000) docker    (1000)     4362 2023-07-25 10:16:53.000000 lmql-0.7b1/src/lmql/models/lmtp/backends/llama_cpp_model.py
--rw-r--r--   0 docker    (1000) docker    (1000)     4689 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/models/lmtp/backends/lmtp_model.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2002 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/models/lmtp/backends/random_model.py
--rw-r--r--   0 docker    (1000) docker    (1000)     4327 2023-07-20 09:50:34.000000 lmql-0.7b1/src/lmql/models/lmtp/backends/transformers_model.py
--rw-r--r--   0 docker    (1000) docker    (1000)       42 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/models/lmtp/errors.py
--rw-r--r--   0 docker    (1000) docker    (1000)     4669 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/models/lmtp/lmtp_async.py
--rw-r--r--   0 docker    (1000) docker    (1000)     5645 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/models/lmtp/lmtp_client.py
--rw-r--r--   0 docker    (1000) docker    (1000)    20210 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/models/lmtp/lmtp_dcmodel.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2283 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/models/lmtp/lmtp_inference_server.py
--rw-r--r--   0 docker    (1000) docker    (1000)     5606 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/models/lmtp/lmtp_multiprocessing.py
--rw-r--r--   0 docker    (1000) docker    (1000)      298 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/models/lmtp/lmtp_programmatic_serve_example.py
--rw-r--r--   0 docker    (1000) docker    (1000)    15201 2023-07-25 10:16:53.000000 lmql-0.7b1/src/lmql/models/lmtp/lmtp_scheduler.py
--rw-r--r--   0 docker    (1000) docker    (1000)     6381 2023-07-20 09:50:34.000000 lmql-0.7b1/src/lmql/models/lmtp/lmtp_serve.py
--rw-r--r--   0 docker    (1000) docker    (1000)     3562 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/models/lmtp/lmtp_threading.py
--rw-r--r--   0 docker    (1000) docker    (1000)      634 2023-07-14 15:36:31.000000 lmql-0.7b1/src/lmql/models/lmtp/utils.py
--rw-r--r--   0 docker    (1000) docker    (1000)     3396 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/models/model.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.257754 lmql-0.7b1/src/lmql/ops/
--rw-r--r--   0 docker    (1000) docker    (1000)       93 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ops/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1656 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/ops/booleans.py
--rw-r--r--   0 docker    (1000) docker    (1000)     8088 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/ops/follow_map.py
--rw-r--r--   0 docker    (1000) docker    (1000)     4377 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/ops/inline_call.py
--rw-r--r--   0 docker    (1000) docker    (1000)     8362 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/ops/node.py
--rw-r--r--   0 docker    (1000) docker    (1000)    37311 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/ops/ops.py
--rw-r--r--   0 docker    (1000) docker    (1000)     8370 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/ops/regex.py
--rw-r--r--   0 docker    (1000) docker    (1000)    21352 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/ops/token_set.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.257754 lmql-0.7b1/src/lmql/output/
--rw-r--r--   0 docker    (1000) docker    (1000)       57 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/output/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2334 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/output/http.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1889 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/output/sse.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2282 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/output/ws.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.257754 lmql-0.7b1/src/lmql/runtime/
--rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/__init__.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.257754 lmql-0.7b1/src/lmql/runtime/bopenai/
--rw-r--r--   0 docker    (1000) docker    (1000)     2236 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/bopenai/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)    29922 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/runtime/bopenai/batched_openai.py
--rw-r--r--   0 docker    (1000) docker    (1000)    21823 2023-07-25 10:16:53.000000 lmql-0.7b1/src/lmql/runtime/bopenai/openai_api.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2096 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/caching.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.261754 lmql-0.7b1/src/lmql/runtime/dclib/
--rw-r--r--   0 docker    (1000) docker    (1000)      494 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/dclib/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)    18839 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/dclib/dclib_array.py
--rw-r--r--   0 docker    (1000) docker    (1000)    26386 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/runtime/dclib/dclib_cache.py
--rw-r--r--   0 docker    (1000) docker    (1000)      592 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/dclib/dclib_global.py
--rw-r--r--   0 docker    (1000) docker    (1000)     4970 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/dclib/dclib_model.py
--rw-r--r--   0 docker    (1000) docker    (1000)     9585 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/runtime/dclib/dclib_rewrite.py
--rw-r--r--   0 docker    (1000) docker    (1000)    33321 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/runtime/dclib/dclib_seq.py
--rw-r--r--   0 docker    (1000) docker    (1000)    22268 2023-07-25 13:45:45.000000 lmql-0.7b1/src/lmql/runtime/dclib/decoders.py
--rw-r--r--   0 docker    (1000) docker    (1000)    52685 2023-07-25 15:16:34.000000 lmql-0.7b1/src/lmql/runtime/interpreter.py
--rw-r--r--   0 docker    (1000) docker    (1000)      250 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/interrupt.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1231 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/langchain.py
--rw-r--r--   0 docker    (1000) docker    (1000)    11319 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/runtime/lmql_runtime.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1940 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/loop.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1245 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/maiohttp.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1726 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/masks.py
--rw-r--r--   0 docker    (1000) docker    (1000)     3145 2023-07-25 10:16:53.000000 lmql-0.7b1/src/lmql/runtime/model_registry.py
--rw-r--r--   0 docker    (1000) docker    (1000)     5965 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/runtime/multi_head_interpretation.py
--rw-r--r--   0 docker    (1000) docker    (1000)    45053 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/runtime/openai_integration.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2179 2023-07-20 09:50:34.000000 lmql-0.7b1/src/lmql/runtime/openai_secret.py
--rw-r--r--   0 docker    (1000) docker    (1000)     4038 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/runtime/output_writer.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.261754 lmql-0.7b1/src/lmql/runtime/postprocessing/
--rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/postprocessing/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)     3543 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/postprocessing/conditional_prob.py
--rw-r--r--   0 docker    (1000) docker    (1000)      152 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/postprocessing/group_by.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2298 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/runtime/program_state.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1317 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/stats.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2220 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/token_distribution.py
--rw-r--r--   0 docker    (1000) docker    (1000)    12577 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/runtime/tokenizer.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.261754 lmql-0.7b1/src/lmql/runtime/tokenizers/
--rw-r--r--   0 docker    (1000) docker    (1000)     4509 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/tokenizers/hf_tokenizer.py
--rw-r--r--   0 docker    (1000) docker    (1000)     3427 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/tokenizers/pure_python_tokenizer.py
--rw-r--r--   0 docker    (1000) docker    (1000)     3207 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/runtime/tokenizers/tiktoken_tokenizer.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.261754 lmql-0.7b1/src/lmql/tests/
--rw-r--r--   0 docker    (1000) docker    (1000)      319 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/README.md
--rw-r--r--   0 docker    (1000) docker    (1000)     1018 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/tests/all.py
--rw-r--r--   0 docker    (1000) docker    (1000)     5916 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/tests/expr_test_utils.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1314 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/fin_and.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.265753 lmql-0.7b1/src/lmql/tests/outdated/
--rw-r--r--   0 docker    (1000) docker    (1000)     1611 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/outdated/mask_product_test.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2789 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/outdated/monotonicity.py
--rw-r--r--   0 docker    (1000) docker    (1000)      546 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/outdated/one_of_tests.py
--rw-r--r--   0 docker    (1000) docker    (1000)      758 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/outdated/sentences_op.py
--rw-r--r--   0 docker    (1000) docker    (1000)      984 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/outdated/starts_with_op_test.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1236 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/outdated/stops_at.py
--rw-r--r--   0 docker    (1000) docker    (1000)      537 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/outdated/str_in_str_tests.py
--rw-r--r--   0 docker    (1000) docker    (1000)     4738 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/outdated/test_multi_head.py
--rw-r--r--   0 docker    (1000) docker    (1000)     3036 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/outdated/token_set_test.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.265753 lmql-0.7b1/src/lmql/tests/queryargs/
--rw-r--r--   0 docker    (1000) docker    (1000)     4489 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/queryargs/test_args.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2072 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/queryargs/test_args_query_str.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1095 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/queryargs/test_args_run.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1066 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/queryargs/test_sync.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1092 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/queryargs/test_var_errors.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.265753 lmql-0.7b1/src/lmql/tests/system/
--rw-r--r--   0 docker    (1000) docker    (1000)     3402 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/system/basic_use_cases.py
--rw-r--r--   0 docker    (1000) docker    (1000)      842 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/tail_token_set.py
--rw-r--r--   0 docker    (1000) docker    (1000)      788 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/test_back2back_caching.py
--rw-r--r--   0 docker    (1000) docker    (1000)      335 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/test_beam_in.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2775 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/test_eq.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1756 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/test_escaping.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2370 2023-07-25 10:16:53.000000 lmql-0.7b1/src/lmql/tests/test_f.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1033 2023-07-25 10:16:53.000000 lmql-0.7b1/src/lmql/tests/test_local_model_python.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1444 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/test_minimal_syntax.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1139 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/test_multibyte_characters.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1171 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/test_multibyte_local_models.py
--rw-r--r--   0 docker    (1000) docker    (1000)      457 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/test_orop.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2931 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/test_qstrings.py
--rw-r--r--   0 docker    (1000) docker    (1000)      479 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/test_query_args.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2639 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/test_sample_queries.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1703 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/test_scoping.py
--rw-r--r--   0 docker    (1000) docker    (1000)     3647 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/test_stopping.py
--rw-r--r--   0 docker    (1000) docker    (1000)      707 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/tests/tiktoken_tsets.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.265753 lmql-0.7b1/src/lmql/ui/
--rw-r--r--   0 docker    (1000) docker    (1000)       27 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/.gitignore
--rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/__init__.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.265753 lmql-0.7b1/src/lmql/ui/chat/
--rw-r--r--   0 docker    (1000) docker    (1000)     6267 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/ui/chat/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)      335 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/ui/chat/__main__.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.265753 lmql-0.7b1/src/lmql/ui/chat/assets/
--rw-r--r--   0 docker    (1000) docker    (1000)     1665 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/ui/chat/assets/code.svg
--rw-r--r--   0 docker    (1000) docker    (1000)     7015 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/ui/chat/assets/index.css
--rw-r--r--   0 docker    (1000) docker    (1000)     8687 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/ui/chat/assets/index.html
--rw-r--r--   0 docker    (1000) docker    (1000)     8689 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/ui/chat/assets/lmql-monaco.js
--rw-r--r--   0 docker    (1000) docker    (1000)     3675 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/ui/chat/assets/lmql.svg
--rw-r--r--   0 docker    (1000) docker    (1000)      551 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/ui/chat/assets/send.svg
--rw-r--r--   0 docker    (1000) docker    (1000)     7853 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/ui/chat/assets/studio.css
--rw-r--r--   0 docker    (1000) docker    (1000)    13744 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/ui/chat/assets/studio.html
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.265753 lmql-0.7b1/src/lmql/ui/live/
--rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/live/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)     6747 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/live/live.js
--rw-r--r--   0 docker    (1000) docker    (1000)     3475 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/live/live.py
--rw-r--r--   0 docker    (1000) docker    (1000)     3885 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/live/livelib.py
--rw-r--r--   0 docker    (1000) docker    (1000)      349 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/live/package.json
--rw-r--r--   0 docker    (1000) docker    (1000)    33701 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/live/yarn.lock
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.269753 lmql-0.7b1/src/lmql/ui/playground/
--rw-r--r--   0 docker    (1000) docker    (1000)       31 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/.dockerignore
--rw-r--r--   0 docker    (1000) docker    (1000)       34 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/.env
--rw-r--r--   0 docker    (1000) docker    (1000)      310 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/.gitignore
--rw-r--r--   0 docker    (1000) docker    (1000)      354 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/Dockerfile
--rw-r--r--   0 docker    (1000) docker    (1000)     3359 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/README.md
--rw-r--r--   0 docker    (1000) docker    (1000)     1327 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/package.json
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.269753 lmql-0.7b1/src/lmql/ui/playground/public/
--rw-r--r--   0 docker    (1000) docker    (1000)       90 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/_headers
--rw-r--r--   0 docker    (1000) docker    (1000)     3870 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/favicon.ico
--rw-r--r--   0 docker    (1000) docker    (1000)     1678 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/index.html
--rw-r--r--   0 docker    (1000) docker    (1000)     2817 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/lmql.svg
--rw-r--r--   0 docker    (1000) docker    (1000)      306 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/manifest.json
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.273753 lmql-0.7b1/src/lmql/ui/playground/public/precomputed/
--rw-r--r--   0 docker    (1000) docker    (1000)  1227728 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/precomputed/calc.json
--rw-r--r--   0 docker    (1000) docker    (1000)   295285 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/precomputed/chat.json
--rw-r--r--   0 docker    (1000) docker    (1000)   160131 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/precomputed/cot.json
--rw-r--r--   0 docker    (1000) docker    (1000)    13974 2023-07-25 15:16:34.000000 lmql-0.7b1/src/lmql/ui/playground/public/precomputed/date-regex.json
--rw-r--r--   0 docker    (1000) docker    (1000)    81768 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/precomputed/distribution.json
--rw-r--r--   0 docker    (1000) docker    (1000)    22895 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/precomputed/hello.json
--rw-r--r--   0 docker    (1000) docker    (1000)    89531 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/precomputed/joke.json
--rw-r--r--   0 docker    (1000) docker    (1000)   484450 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/ui/playground/public/precomputed/json-robust.json
--rw-r--r--   0 docker    (1000) docker    (1000)   265372 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/precomputed/json-template.json
--rw-r--r--   0 docker    (1000) docker    (1000)  1710847 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/precomputed/kv.json
--rw-r--r--   0 docker    (1000) docker    (1000)    52748 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/precomputed/list.json
--rw-r--r--   0 docker    (1000) docker    (1000)   628184 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/precomputed/meta.json
--rw-r--r--   0 docker    (1000) docker    (1000)   264768 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/precomputed/translation.json
--rw-r--r--   0 docker    (1000) docker    (1000)   215050 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/precomputed/wiki.json
--rw-r--r--   0 docker    (1000) docker    (1000)       67 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/robots.txt
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.273753 lmql-0.7b1/src/lmql/ui/playground/public/snippets/
--rw-r--r--   0 docker    (1000) docker    (1000)   381736 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/snippets/dynamic-cfg.json
--rw-r--r--   0 docker    (1000) docker    (1000)   184008 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/public/snippets/json-parsing.json
--rw-r--r--   0 docker    (1000) docker    (1000)       62 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/ref.py
--rw-r--r--   0 docker    (1000) docker    (1000)       80 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/run-in-docker.sh
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.277753 lmql-0.7b1/src/lmql/ui/playground/src/
--rw-r--r--   0 docker    (1000) docker    (1000)    76544 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/ui/playground/src/App.jsx
--rw-r--r--   0 docker    (1000) docker    (1000)      246 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/App.test.js
--rw-r--r--   0 docker    (1000) docker    (1000)    29983 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/CodeScreenshot.jsx
--rw-r--r--   0 docker    (1000) docker    (1000)      961 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/ui/playground/src/Configuration.js
--rw-r--r--   0 docker    (1000) docker    (1000)     1174 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/DataListView.js
--rw-r--r--   0 docker    (1000) docker    (1000)    21726 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/ui/playground/src/DecoderGraph.js
--rw-r--r--   0 docker    (1000) docker    (1000)      329 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/DecodingTree.js
--rw-r--r--   0 docker    (1000) docker    (1000)       89 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/Embed.jsx
--rw-r--r--   0 docker    (1000) docker    (1000)    12240 2023-07-25 15:16:34.000000 lmql-0.7b1/src/lmql/ui/playground/src/Explore.jsx
--rw-r--r--   0 docker    (1000) docker    (1000)      675 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/SharedState.js
--rw-r--r--   0 docker    (1000) docker    (1000)     4819 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/State.js
--rw-r--r--   0 docker    (1000) docker    (1000)     5871 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/ValidationGraph.jsx
--rw-r--r--   0 docker    (1000) docker    (1000)     9360 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/browser_process.js
--rw-r--r--   0 docker    (1000) docker    (1000)     1163 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/build_info.js
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.277753 lmql-0.7b1/src/lmql/ui/playground/src/editor/
--rw-r--r--   0 docker    (1000) docker    (1000)     9032 2023-07-25 13:45:46.000000 lmql-0.7b1/src/lmql/ui/playground/src/editor/lmql-monaco-language.js
--rw-r--r--   0 docker    (1000) docker    (1000)     4758 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/editor/theme.json
--rw-r--r--   0 docker    (1000) docker    (1000)      889 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/explore.svg
--rw-r--r--   0 docker    (1000) docker    (1000)     1345 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/graph-layout.css
--rw-r--r--   0 docker    (1000) docker    (1000)     1698 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/index.css
--rw-r--r--   0 docker    (1000) docker    (1000)      489 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/index.js
--rw-r--r--   0 docker    (1000) docker    (1000)     2632 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/logo.svg
--rw-r--r--   0 docker    (1000) docker    (1000)    12203 2023-07-25 15:16:34.000000 lmql-0.7b1/src/lmql/ui/playground/src/queries.js
--rw-r--r--   0 docker    (1000) docker    (1000)     5990 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/remote_process.js
--rw-r--r--   0 docker    (1000) docker    (1000)      362 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/reportWebVitals.js
--rw-r--r--   0 docker    (1000) docker    (1000)     9520 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/screenshot.css
--rw-r--r--   0 docker    (1000) docker    (1000)      241 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/setupTests.js
--rw-r--r--   0 docker    (1000) docker    (1000)     3466 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/spinner.svg
--rw-r--r--   0 docker    (1000) docker    (1000)     3200 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/src/tagged-model-result.js
--rw-r--r--   0 docker    (1000) docker    (1000)   449905 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/playground/yarn.lock
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.281753 lmql-0.7b1/src/lmql/ui/vscode/
--rw-r--r--   0 docker    (1000) docker    (1000)       76 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/vscode/.gitattributes
--rw-r--r--   0 docker    (1000) docker    (1000)       19 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/vscode/.gitignore
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.281753 lmql-0.7b1/src/lmql/ui/vscode/.vscode/
--rw-r--r--   0 docker    (1000) docker    (1000)      540 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/vscode/.vscode/launch.json
--rw-r--r--   0 docker    (1000) docker    (1000)       66 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/vscode/.vscodeignore
--rw-r--r--   0 docker    (1000) docker    (1000)    23151 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/vscode/LICENSE
--rw-r--r--   0 docker    (1000) docker    (1000)      357 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/vscode/README.md
--rw-r--r--   0 docker    (1000) docker    (1000)      959 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/vscode/language-configuration.json
--rw-r--r--   0 docker    (1000) docker    (1000)    11532 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/vscode/lmql-vscode.png
--rw-r--r--   0 docker    (1000) docker    (1000)     1214 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/vscode/package.json
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.281753 lmql-0.7b1/src/lmql/ui/vscode/syntaxes/
--rw-r--r--   0 docker    (1000) docker    (1000)      518 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/vscode/syntaxes/lmql.qstring.json
--rw-r--r--   0 docker    (1000) docker    (1000)      642 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json
--rw-r--r--   0 docker    (1000) docker    (1000)      853 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/ui/vscode/syntaxes/pylmql.json
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.281753 lmql-0.7b1/src/lmql/utils/
--rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/utils/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2402 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/utils/docstring_parser.py
--rw-r--r--   0 docker    (1000) docker    (1000)     4933 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/utils/graph.py
--rw-r--r--   0 docker    (1000) docker    (1000)     2715 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql/utils/nputil.py
--rw-r--r--   0 docker    (1000) docker    (1000)      112 2023-07-25 15:21:16.000000 lmql-0.7b1/src/lmql/version.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-25 15:21:24.249754 lmql-0.7b1/src/lmql.egg-info/
--rw-r--r--   0 docker    (1000) docker    (1000)     9896 2023-07-25 15:21:24.000000 lmql-0.7b1/src/lmql.egg-info/PKG-INFO
--rw-r--r--   0 docker    (1000) docker    (1000)    10123 2023-07-25 15:21:24.000000 lmql-0.7b1/src/lmql.egg-info/SOURCES.txt
--rw-r--r--   0 docker    (1000) docker    (1000)        1 2023-07-25 15:21:24.000000 lmql-0.7b1/src/lmql.egg-info/dependency_links.txt
--rw-r--r--   0 docker    (1000) docker    (1000)       39 2023-07-25 15:21:24.000000 lmql-0.7b1/src/lmql.egg-info/entry_points.txt
--rw-r--r--   0 docker    (1000) docker    (1000)       95 2023-07-25 15:21:24.000000 lmql-0.7b1/src/lmql.egg-info/requires.txt
--rw-r--r--   0 docker    (1000) docker    (1000)        5 2023-07-25 15:21:24.000000 lmql-0.7b1/src/lmql.egg-info/top_level.txt
--rw-r--r--   0 docker    (1000) docker    (1000)   115785 2023-07-14 11:31:18.000000 lmql-0.7b1/src/lmql.svg
--rw-r--r--   0 docker    (1000) docker    (1000)       86 2023-07-14 11:31:18.000000 lmql-0.7b1/yarn.lock
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.107395 lmql-0.7b2/
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.047396 lmql-0.7b2/.github/
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.055396 lmql-0.7b2/.github/workflows/
+-rw-r--r--   0 docker    (1000) docker    (1000)     2590 2023-07-14 15:52:52.000000 lmql-0.7b2/.github/workflows/lmql-ci.yml
+-rw-r--r--   0 docker    (1000) docker    (1000)     1543 2023-07-14 11:33:53.000000 lmql-0.7b2/.github/workflows/lmql-tests.yml
+-rw-r--r--   0 docker    (1000) docker    (1000)     2372 2023-07-25 13:45:45.000000 lmql-0.7b2/.github/workflows/lmql-web.yml
+-rw-r--r--   0 docker    (1000) docker    (1000)     2743 2023-07-14 11:31:18.000000 lmql-0.7b2/.gitignore
+-rw-r--r--   0 docker    (1000) docker    (1000)      578 2023-07-28 18:57:38.000000 lmql-0.7b2/.readthedocs.yaml
+-rw-r--r--   0 docker    (1000) docker    (1000)    23151 2023-07-14 11:31:18.000000 lmql-0.7b2/LICENSE
+-rw-r--r--   0 docker    (1000) docker    (1000)      140 2023-07-14 11:31:18.000000 lmql-0.7b2/MANIFEST.in
+-rw-r--r--   0 docker    (1000) docker    (1000)     9896 2023-07-28 19:02:16.107395 lmql-0.7b2/PKG-INFO
+-rw-r--r--   0 docker    (1000) docker    (1000)     9448 2023-07-14 15:36:31.000000 lmql-0.7b2/README.md
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.055396 lmql-0.7b2/docs/
+-rw-r--r--   0 docker    (1000) docker    (1000)      638 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/Makefile
+-rw-r--r--   0 docker    (1000) docker    (1000)      444 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/RELEASE.md
+-rw-r--r--   0 docker    (1000) docker    (1000)      799 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/make.bat
+-rw-r--r--   0 docker    (1000) docker    (1000)       89 2023-07-28 18:57:38.000000 lmql-0.7b2/docs/requirements.txt
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.055396 lmql-0.7b2/docs/source/
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.055396 lmql-0.7b2/docs/source/_ext/
+-rw-r--r--   0 docker    (1000) docker    (1000)     5728 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/source/_ext/lmql_snippets.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.055396 lmql-0.7b2/docs/source/_static/
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.055396 lmql-0.7b2/docs/source/_static/css/
+-rw-r--r--   0 docker    (1000) docker    (1000)     6756 2023-07-28 18:57:38.000000 lmql-0.7b2/docs/source/_static/css/lmql-docs.css
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.055396 lmql-0.7b2/docs/source/_static/images/
+-rw-r--r--   0 docker    (1000) docker    (1000)     3675 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/source/_static/images/lmql.svg
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.055396 lmql-0.7b2/docs/source/_static/js/
+-rw-r--r--   0 docker    (1000) docker    (1000)     2087 2023-07-14 15:36:31.000000 lmql-0.7b2/docs/source/_static/js/lmql-playground.js
+-rw-r--r--   0 docker    (1000) docker    (1000)    12144 2023-07-28 18:57:38.000000 lmql-0.7b2/docs/source/_static/logo-light.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)     5074 2023-07-28 18:57:38.000000 lmql-0.7b2/docs/source/_static/logo.png
+-rw-r--r--   0 docker    (1000) docker    (1000)    12154 2023-07-28 18:57:38.000000 lmql-0.7b2/docs/source/_static/logo.svg
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.055396 lmql-0.7b2/docs/source/_templates/
+-rw-r--r--   0 docker    (1000) docker    (1000)      292 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/source/_templates/layout.html
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.059396 lmql-0.7b2/docs/source/blog/
+-rw-r--r--   0 docker    (1000) docker    (1000)     4591 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/source/blog/release-0.0.5.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     1444 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/source/blog/release-0.0.6.1.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     2068 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/source/blog/release-0.0.6.3.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     3221 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/source/blog/release-0.0.6.4.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     5872 2023-07-20 09:50:34.000000 lmql-0.7b2/docs/source/blog/release-0.0.6.5.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     1445 2023-07-25 13:45:45.000000 lmql-0.7b2/docs/source/blog/release-0.0.6.6.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     8976 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/source/blog/release-0.0.6.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     1721 2023-07-28 18:57:38.000000 lmql-0.7b2/docs/source/conf.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1293 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/source/dev-setup.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     2333 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/source/docker-setup.md
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.059396 lmql-0.7b2/docs/source/images/
+-rw-r--r--   0 docker    (1000) docker    (1000)   125712 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/source/images/inference.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)     2771 2023-07-28 18:57:38.000000 lmql-0.7b2/docs/source/index.rst
+-rw-r--r--   0 docker    (1000) docker    (1000)     2563 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/source/installation.md
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.059396 lmql-0.7b2/docs/source/language/
+-rw-r--r--   0 docker    (1000) docker    (1000)     2313 2023-07-14 15:36:31.000000 lmql-0.7b2/docs/source/language/azure.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     4366 2023-07-28 18:57:38.000000 lmql-0.7b2/docs/source/language/constraints.md
+-rw-r--r--   0 docker    (1000) docker    (1000)    12627 2023-07-28 18:57:38.000000 lmql-0.7b2/docs/source/language/custom-constraints.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     5368 2023-07-28 18:57:38.000000 lmql-0.7b2/docs/source/language/decoders.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     7850 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/source/language/functions.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     3967 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/source/language/hf.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     2027 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/source/language/llama.cpp.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     3173 2023-07-28 18:57:38.000000 lmql-0.7b2/docs/source/language/models.rst
+-rw-r--r--   0 docker    (1000) docker    (1000)     5710 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/source/language/openai.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     8292 2023-07-14 15:36:31.000000 lmql-0.7b2/docs/source/language/overview.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     6032 2023-07-20 09:50:34.000000 lmql-0.7b2/docs/source/language/scripted_prompts.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     3675 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/source/lmql.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)    28444 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/source/logo.png
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.059396 lmql-0.7b2/docs/source/pending/
+-rw-r--r--   0 docker    (1000) docker    (1000)     3550 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/source/pending/release-next.md
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.059396 lmql-0.7b2/docs/source/python/
+-rw-r--r--   0 docker    (1000) docker    (1000)       11 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/source/python/.gitignore
+-rw-r--r--   0 docker    (1000) docker    (1000)     4924 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/source/python/comparison.md
+-rw-r--r--   0 docker    (1000) docker    (1000)    11193 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/source/python/langchain.ipynb
+-rw-r--r--   0 docker    (1000) docker    (1000)     1157 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/source/python/lc.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     6681 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/source/python/llama_index.ipynb
+-rw-r--r--   0 docker    (1000) docker    (1000)    75148 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/source/python/lmql.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)     7458 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/source/python/output.ipynb
+-rw-r--r--   0 docker    (1000) docker    (1000)     9592 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/source/python/pandas.ipynb
+-rw-r--r--   0 docker    (1000) docker    (1000)    13317 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/source/python/python.ipynb
+-rw-r--r--   0 docker    (1000) docker    (1000)     4807 2023-07-28 18:57:38.000000 lmql-0.7b2/docs/source/quickstart.md
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.063396 lmql-0.7b2/docs/source/releases/
+-rw-r--r--   0 docker    (1000) docker    (1000)     2263 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/source/releases/misc-snippets.md
+-rw-r--r--   0 docker    (1000) docker    (1000)      321 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/source/releases/release-0.0.5.md
+-rw-r--r--   0 docker    (1000) docker    (1000)      257 2023-07-14 11:31:18.000000 lmql-0.7b2/docs/todo.md
+-rw-r--r--   0 docker    (1000) docker    (1000)      137 2023-07-14 11:31:18.000000 lmql-0.7b2/pyproject.toml
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.063396 lmql-0.7b2/scripts/
+-rw-r--r--   0 docker    (1000) docker    (1000)      577 2023-07-14 11:31:18.000000 lmql-0.7b2/scripts/Dockerfile
+-rw-r--r--   0 docker    (1000) docker    (1000)      295 2023-07-14 11:31:18.000000 lmql-0.7b2/scripts/activate-dev.sh
+-rw-r--r--   0 docker    (1000) docker    (1000)      357 2023-07-25 13:45:45.000000 lmql-0.7b2/scripts/changelog.sh
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.063396 lmql-0.7b2/scripts/conda/
+-rw-r--r--   0 docker    (1000) docker    (1000)      198 2023-07-14 11:31:18.000000 lmql-0.7b2/scripts/conda/requirements-no-gpu.yml
+-rw-r--r--   0 docker    (1000) docker    (1000)      332 2023-07-14 11:31:18.000000 lmql-0.7b2/scripts/conda/requirements.yml
+-rw-r--r--   0 docker    (1000) docker    (1000)      638 2023-07-14 11:31:18.000000 lmql-0.7b2/scripts/pypi-release.sh
+-rw-r--r--   0 docker    (1000) docker    (1000)     4156 2023-07-28 18:57:38.000000 lmql-0.7b2/scripts/serve-all.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      854 2023-07-14 11:31:18.000000 lmql-0.7b2/scripts/wheel.sh
+-rw-r--r--   0 docker    (1000) docker    (1000)      866 2023-07-28 19:02:16.107395 lmql-0.7b2/setup.cfg
+-rw-r--r--   0 docker    (1000) docker    (1000)       37 2023-07-14 11:31:18.000000 lmql-0.7b2/setup.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.063396 lmql-0.7b2/src/
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.063396 lmql-0.7b2/src/lmql/
+-rw-r--r--   0 docker    (1000) docker    (1000)        6 2023-07-25 13:45:45.000000 lmql-0.7b2/src/lmql/.gitignore
+-rw-r--r--   0 docker    (1000) docker    (1000)     8078 2023-07-25 13:45:45.000000 lmql-0.7b2/src/lmql/__init__.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.063396 lmql-0.7b2/src/lmql/algorithms/
+-rw-r--r--   0 docker    (1000) docker    (1000)       45 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/algorithms/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2763 2023-07-25 13:45:45.000000 lmql-0.7b2/src/lmql/algorithms/cache.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      942 2023-07-25 13:45:45.000000 lmql-0.7b2/src/lmql/algorithms/functools.py
+-rwxr-xr-x   0 docker    (1000) docker    (1000)     8644 2023-07-25 13:45:45.000000 lmql-0.7b2/src/lmql/cli.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1577 2023-07-25 13:45:45.000000 lmql-0.7b2/src/lmql/demo.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1531 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/http.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.067396 lmql-0.7b2/src/lmql/language/
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/language/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    32350 2023-07-28 18:57:38.000000 lmql-0.7b2/src/lmql/language/compiler.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    11442 2023-07-25 13:45:45.000000 lmql-0.7b2/src/lmql/language/fragment_parser.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4700 2023-07-25 13:45:45.000000 lmql-0.7b2/src/lmql/language/qstrings.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1804 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/language/validator.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.067396 lmql-0.7b2/src/lmql/lib/
+-rw-r--r--   0 docker    (1000) docker    (1000)      143 2023-07-25 13:45:45.000000 lmql-0.7b2/src/lmql/lib/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    12327 2023-07-28 18:57:38.000000 lmql-0.7b2/src/lmql/lib/actions.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    61974 2023-07-25 13:45:45.000000 lmql-0.7b2/src/lmql/lib/algebra222.csv
+-rw-r--r--   0 docker    (1000) docker    (1000)     5225 2023-07-25 13:45:45.000000 lmql-0.7b2/src/lmql/lib/data.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.067396 lmql-0.7b2/src/lmql/lib/prompts/
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-28 18:57:38.000000 lmql-0.7b2/src/lmql/lib/prompts/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1682 2023-07-25 13:45:45.000000 lmql-0.7b2/src/lmql/lib/prompts/inline_code copy.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1625 2023-07-25 13:45:45.000000 lmql-0.7b2/src/lmql/lib/prompts/inline_code.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1450 2023-07-25 13:45:45.000000 lmql-0.7b2/src/lmql/lib/prompts/inline_use.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1694 2023-07-25 13:45:45.000000 lmql-0.7b2/src/lmql/lib/prompts/inline_use_kevin.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     5900 2023-07-25 13:45:45.000000 lmql-0.7b2/src/lmql/lib/prompts/wiki_prompt.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     7473 2023-07-25 13:45:45.000000 lmql-0.7b2/src/lmql/lib/types.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      942 2023-07-25 13:45:45.000000 lmql-0.7b2/src/lmql/lib/value.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.067396 lmql-0.7b2/src/lmql/models/
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/models/__init__.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.071396 lmql-0.7b2/src/lmql/models/lmtp/
+-rw-r--r--   0 docker    (1000) docker    (1000)     6156 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/models/lmtp/README.md
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-28 18:57:38.000000 lmql-0.7b2/src/lmql/models/lmtp/__init__.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.071396 lmql-0.7b2/src/lmql/models/lmtp/backends/
+-rw-r--r--   0 docker    (1000) docker    (1000)      493 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/models/lmtp/backends/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      694 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/models/lmtp/backends/__main__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4302 2023-07-28 18:57:38.000000 lmql-0.7b2/src/lmql/models/lmtp/backends/llama_cpp_model.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4689 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/models/lmtp/backends/lmtp_model.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2002 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/models/lmtp/backends/random_model.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4327 2023-07-20 09:50:34.000000 lmql-0.7b2/src/lmql/models/lmtp/backends/transformers_model.py
+-rw-r--r--   0 docker    (1000) docker    (1000)       42 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/models/lmtp/errors.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4669 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/models/lmtp/lmtp_async.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     5645 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/models/lmtp/lmtp_client.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    20210 2023-07-25 13:45:45.000000 lmql-0.7b2/src/lmql/models/lmtp/lmtp_dcmodel.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2283 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/models/lmtp/lmtp_inference_server.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     5606 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/models/lmtp/lmtp_multiprocessing.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      298 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/models/lmtp/lmtp_programmatic_serve_example.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    15201 2023-07-25 10:16:53.000000 lmql-0.7b2/src/lmql/models/lmtp/lmtp_scheduler.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     6381 2023-07-20 09:50:34.000000 lmql-0.7b2/src/lmql/models/lmtp/lmtp_serve.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3562 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/models/lmtp/lmtp_threading.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      634 2023-07-14 15:36:31.000000 lmql-0.7b2/src/lmql/models/lmtp/utils.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3396 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/models/model.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.071396 lmql-0.7b2/src/lmql/ops/
+-rw-r--r--   0 docker    (1000) docker    (1000)       93 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ops/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1656 2023-07-25 13:45:45.000000 lmql-0.7b2/src/lmql/ops/booleans.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     8088 2023-07-25 13:45:45.000000 lmql-0.7b2/src/lmql/ops/follow_map.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4689 2023-07-28 18:57:38.000000 lmql-0.7b2/src/lmql/ops/inline_call.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     8362 2023-07-25 13:45:45.000000 lmql-0.7b2/src/lmql/ops/node.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    37311 2023-07-25 13:45:45.000000 lmql-0.7b2/src/lmql/ops/ops.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     8370 2023-07-25 13:45:45.000000 lmql-0.7b2/src/lmql/ops/regex.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    21352 2023-07-25 13:45:45.000000 lmql-0.7b2/src/lmql/ops/token_set.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.071396 lmql-0.7b2/src/lmql/output/
+-rw-r--r--   0 docker    (1000) docker    (1000)       57 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/output/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2334 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/output/http.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1889 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/output/sse.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2282 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/output/ws.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.075396 lmql-0.7b2/src/lmql/runtime/
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/runtime/__init__.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.075396 lmql-0.7b2/src/lmql/runtime/bopenai/
+-rw-r--r--   0 docker    (1000) docker    (1000)     2236 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/runtime/bopenai/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    29922 2023-07-25 13:45:45.000000 lmql-0.7b2/src/lmql/runtime/bopenai/batched_openai.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    21823 2023-07-25 10:16:53.000000 lmql-0.7b2/src/lmql/runtime/bopenai/openai_api.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2096 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/runtime/caching.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.075396 lmql-0.7b2/src/lmql/runtime/dclib/
+-rw-r--r--   0 docker    (1000) docker    (1000)      494 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/runtime/dclib/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    18839 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/runtime/dclib/dclib_array.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    26386 2023-07-25 13:45:45.000000 lmql-0.7b2/src/lmql/runtime/dclib/dclib_cache.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      592 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/runtime/dclib/dclib_global.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4970 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/runtime/dclib/dclib_model.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     9585 2023-07-25 13:45:45.000000 lmql-0.7b2/src/lmql/runtime/dclib/dclib_rewrite.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    33321 2023-07-25 13:45:45.000000 lmql-0.7b2/src/lmql/runtime/dclib/dclib_seq.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    22268 2023-07-25 13:45:45.000000 lmql-0.7b2/src/lmql/runtime/dclib/decoders.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    52693 2023-07-28 18:57:38.000000 lmql-0.7b2/src/lmql/runtime/interpreter.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      250 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/runtime/interrupt.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1231 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/runtime/langchain.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    11319 2023-07-25 13:45:46.000000 lmql-0.7b2/src/lmql/runtime/lmql_runtime.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1940 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/runtime/loop.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1245 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/runtime/maiohttp.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1726 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/runtime/masks.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3145 2023-07-25 10:16:53.000000 lmql-0.7b2/src/lmql/runtime/model_registry.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     5965 2023-07-25 13:45:46.000000 lmql-0.7b2/src/lmql/runtime/multi_head_interpretation.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    45053 2023-07-25 13:45:46.000000 lmql-0.7b2/src/lmql/runtime/openai_integration.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2179 2023-07-20 09:50:34.000000 lmql-0.7b2/src/lmql/runtime/openai_secret.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4038 2023-07-25 13:45:46.000000 lmql-0.7b2/src/lmql/runtime/output_writer.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.075396 lmql-0.7b2/src/lmql/runtime/postprocessing/
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/runtime/postprocessing/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3543 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/runtime/postprocessing/conditional_prob.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      152 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/runtime/postprocessing/group_by.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2298 2023-07-25 13:45:46.000000 lmql-0.7b2/src/lmql/runtime/program_state.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1317 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/runtime/stats.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2220 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/runtime/token_distribution.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    12577 2023-07-25 13:45:46.000000 lmql-0.7b2/src/lmql/runtime/tokenizer.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.075396 lmql-0.7b2/src/lmql/runtime/tokenizers/
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-28 18:57:38.000000 lmql-0.7b2/src/lmql/runtime/tokenizers/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4509 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/runtime/tokenizers/hf_tokenizer.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3427 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/runtime/tokenizers/pure_python_tokenizer.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3207 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/runtime/tokenizers/tiktoken_tokenizer.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.079396 lmql-0.7b2/src/lmql/tests/
+-rw-r--r--   0 docker    (1000) docker    (1000)      319 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/README.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     1018 2023-07-25 13:45:46.000000 lmql-0.7b2/src/lmql/tests/all.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     5916 2023-07-25 13:45:46.000000 lmql-0.7b2/src/lmql/tests/expr_test_utils.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1314 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/fin_and.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.079396 lmql-0.7b2/src/lmql/tests/outdated/
+-rw-r--r--   0 docker    (1000) docker    (1000)     1611 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/outdated/mask_product_test.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2789 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/outdated/monotonicity.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      546 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/outdated/one_of_tests.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      758 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/outdated/sentences_op.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      984 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/outdated/starts_with_op_test.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1236 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/outdated/stops_at.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      537 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/outdated/str_in_str_tests.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4738 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/outdated/test_multi_head.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3036 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/outdated/token_set_test.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.079396 lmql-0.7b2/src/lmql/tests/queryargs/
+-rw-r--r--   0 docker    (1000) docker    (1000)     4489 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/queryargs/test_args.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2072 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/queryargs/test_args_query_str.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1095 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/queryargs/test_args_run.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1066 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/queryargs/test_sync.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1092 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/queryargs/test_var_errors.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.079396 lmql-0.7b2/src/lmql/tests/system/
+-rw-r--r--   0 docker    (1000) docker    (1000)     3402 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/system/basic_use_cases.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      842 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/tail_token_set.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      788 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/test_back2back_caching.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      335 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/test_beam_in.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2775 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/test_eq.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1756 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/test_escaping.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2370 2023-07-25 10:16:53.000000 lmql-0.7b2/src/lmql/tests/test_f.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1033 2023-07-25 10:16:53.000000 lmql-0.7b2/src/lmql/tests/test_local_model_python.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1444 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/test_minimal_syntax.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1139 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/test_multibyte_characters.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1171 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/test_multibyte_local_models.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      457 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/test_orop.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2931 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/test_qstrings.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      479 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/test_query_args.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2639 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/test_sample_queries.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1703 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/test_scoping.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3647 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/test_stopping.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      707 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/tests/tiktoken_tsets.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.079396 lmql-0.7b2/src/lmql/ui/
+-rw-r--r--   0 docker    (1000) docker    (1000)       27 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/.gitignore
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/__init__.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.079396 lmql-0.7b2/src/lmql/ui/chat/
+-rw-r--r--   0 docker    (1000) docker    (1000)     6267 2023-07-25 13:45:46.000000 lmql-0.7b2/src/lmql/ui/chat/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      335 2023-07-25 13:45:46.000000 lmql-0.7b2/src/lmql/ui/chat/__main__.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.083395 lmql-0.7b2/src/lmql/ui/chat/assets/
+-rw-r--r--   0 docker    (1000) docker    (1000)     1665 2023-07-25 13:45:46.000000 lmql-0.7b2/src/lmql/ui/chat/assets/code.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)     7015 2023-07-25 13:45:46.000000 lmql-0.7b2/src/lmql/ui/chat/assets/index.css
+-rw-r--r--   0 docker    (1000) docker    (1000)     8691 2023-07-28 18:57:38.000000 lmql-0.7b2/src/lmql/ui/chat/assets/index.html
+-rw-r--r--   0 docker    (1000) docker    (1000)     8689 2023-07-25 13:45:46.000000 lmql-0.7b2/src/lmql/ui/chat/assets/lmql-monaco.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     3675 2023-07-25 13:45:46.000000 lmql-0.7b2/src/lmql/ui/chat/assets/lmql.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)      551 2023-07-25 13:45:46.000000 lmql-0.7b2/src/lmql/ui/chat/assets/send.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)     7853 2023-07-25 13:45:46.000000 lmql-0.7b2/src/lmql/ui/chat/assets/studio.css
+-rw-r--r--   0 docker    (1000) docker    (1000)    13765 2023-07-28 18:57:38.000000 lmql-0.7b2/src/lmql/ui/chat/assets/studio.html
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.083395 lmql-0.7b2/src/lmql/ui/live/
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/live/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     6747 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/live/live.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     3475 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/live/live.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3885 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/live/livelib.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      349 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/live/package.json
+-rw-r--r--   0 docker    (1000) docker    (1000)    33701 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/live/yarn.lock
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.083395 lmql-0.7b2/src/lmql/ui/playground/
+-rw-r--r--   0 docker    (1000) docker    (1000)       31 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/.dockerignore
+-rw-r--r--   0 docker    (1000) docker    (1000)       34 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/.env
+-rw-r--r--   0 docker    (1000) docker    (1000)      310 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/.gitignore
+-rw-r--r--   0 docker    (1000) docker    (1000)      354 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/Dockerfile
+-rw-r--r--   0 docker    (1000) docker    (1000)     3359 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/README.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     1327 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/package.json
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.083395 lmql-0.7b2/src/lmql/ui/playground/public/
+-rw-r--r--   0 docker    (1000) docker    (1000)       90 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/public/_headers
+-rw-r--r--   0 docker    (1000) docker    (1000)     3870 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/public/favicon.ico
+-rw-r--r--   0 docker    (1000) docker    (1000)     1678 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/public/index.html
+-rw-r--r--   0 docker    (1000) docker    (1000)     2817 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/public/lmql.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)      306 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/public/manifest.json
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.099395 lmql-0.7b2/src/lmql/ui/playground/public/precomputed/
+-rw-r--r--   0 docker    (1000) docker    (1000)  1227728 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/public/precomputed/calc.json
+-rw-r--r--   0 docker    (1000) docker    (1000)   295285 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/public/precomputed/chat.json
+-rw-r--r--   0 docker    (1000) docker    (1000)   160131 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/public/precomputed/cot.json
+-rw-r--r--   0 docker    (1000) docker    (1000)    13974 2023-07-25 15:16:34.000000 lmql-0.7b2/src/lmql/ui/playground/public/precomputed/date-regex.json
+-rw-r--r--   0 docker    (1000) docker    (1000)    81768 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/public/precomputed/distribution.json
+-rw-r--r--   0 docker    (1000) docker    (1000)    22895 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/public/precomputed/hello.json
+-rw-r--r--   0 docker    (1000) docker    (1000)    89531 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/public/precomputed/joke.json
+-rw-r--r--   0 docker    (1000) docker    (1000)   484450 2023-07-25 13:45:46.000000 lmql-0.7b2/src/lmql/ui/playground/public/precomputed/json-robust.json
+-rw-r--r--   0 docker    (1000) docker    (1000)   265372 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/public/precomputed/json-template.json
+-rw-r--r--   0 docker    (1000) docker    (1000)  1710847 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/public/precomputed/kv.json
+-rw-r--r--   0 docker    (1000) docker    (1000)    52748 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/public/precomputed/list.json
+-rw-r--r--   0 docker    (1000) docker    (1000)   628184 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/public/precomputed/meta.json
+-rw-r--r--   0 docker    (1000) docker    (1000)   264768 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/public/precomputed/translation.json
+-rw-r--r--   0 docker    (1000) docker    (1000)   215050 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/public/precomputed/wiki.json
+-rw-r--r--   0 docker    (1000) docker    (1000)       67 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/public/robots.txt
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.099395 lmql-0.7b2/src/lmql/ui/playground/public/snippets/
+-rw-r--r--   0 docker    (1000) docker    (1000)   381736 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/public/snippets/dynamic-cfg.json
+-rw-r--r--   0 docker    (1000) docker    (1000)   184008 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/public/snippets/json-parsing.json
+-rw-r--r--   0 docker    (1000) docker    (1000)       62 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/ref.py
+-rw-r--r--   0 docker    (1000) docker    (1000)       80 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/run-in-docker.sh
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.103395 lmql-0.7b2/src/lmql/ui/playground/src/
+-rw-r--r--   0 docker    (1000) docker    (1000)    76707 2023-07-28 18:57:38.000000 lmql-0.7b2/src/lmql/ui/playground/src/App.jsx
+-rw-r--r--   0 docker    (1000) docker    (1000)      246 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/src/App.test.js
+-rw-r--r--   0 docker    (1000) docker    (1000)    29983 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/src/CodeScreenshot.jsx
+-rw-r--r--   0 docker    (1000) docker    (1000)      961 2023-07-25 13:45:46.000000 lmql-0.7b2/src/lmql/ui/playground/src/Configuration.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     1174 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/src/DataListView.js
+-rw-r--r--   0 docker    (1000) docker    (1000)    21726 2023-07-25 13:45:46.000000 lmql-0.7b2/src/lmql/ui/playground/src/DecoderGraph.js
+-rw-r--r--   0 docker    (1000) docker    (1000)      329 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/src/DecodingTree.js
+-rw-r--r--   0 docker    (1000) docker    (1000)       89 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/src/Embed.jsx
+-rw-r--r--   0 docker    (1000) docker    (1000)    13042 2023-07-28 18:57:38.000000 lmql-0.7b2/src/lmql/ui/playground/src/Explore.jsx
+-rw-r--r--   0 docker    (1000) docker    (1000)      675 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/src/SharedState.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     4819 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/src/State.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     5871 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/src/ValidationGraph.jsx
+-rw-r--r--   0 docker    (1000) docker    (1000)     9360 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/src/browser_process.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     1163 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/src/build_info.js
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.103395 lmql-0.7b2/src/lmql/ui/playground/src/editor/
+-rw-r--r--   0 docker    (1000) docker    (1000)     9032 2023-07-25 13:45:46.000000 lmql-0.7b2/src/lmql/ui/playground/src/editor/lmql-monaco-language.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     4758 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/src/editor/theme.json
+-rw-r--r--   0 docker    (1000) docker    (1000)      889 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/src/explore.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)     1345 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/src/graph-layout.css
+-rw-r--r--   0 docker    (1000) docker    (1000)     1924 2023-07-28 18:57:38.000000 lmql-0.7b2/src/lmql/ui/playground/src/index.css
+-rw-r--r--   0 docker    (1000) docker    (1000)      489 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/src/index.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     2632 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/src/logo.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)    12209 2023-07-28 18:57:38.000000 lmql-0.7b2/src/lmql/ui/playground/src/queries.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     5990 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/src/remote_process.js
+-rw-r--r--   0 docker    (1000) docker    (1000)      362 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/src/reportWebVitals.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     9520 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/src/screenshot.css
+-rw-r--r--   0 docker    (1000) docker    (1000)      241 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/src/setupTests.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     3466 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/src/spinner.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)     3200 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/src/tagged-model-result.js
+-rw-r--r--   0 docker    (1000) docker    (1000)   449905 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/playground/yarn.lock
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.103395 lmql-0.7b2/src/lmql/ui/vscode/
+-rw-r--r--   0 docker    (1000) docker    (1000)       76 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/vscode/.gitattributes
+-rw-r--r--   0 docker    (1000) docker    (1000)       19 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/vscode/.gitignore
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.103395 lmql-0.7b2/src/lmql/ui/vscode/.vscode/
+-rw-r--r--   0 docker    (1000) docker    (1000)      540 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/vscode/.vscode/launch.json
+-rw-r--r--   0 docker    (1000) docker    (1000)       66 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/vscode/.vscodeignore
+-rw-r--r--   0 docker    (1000) docker    (1000)    23151 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/vscode/LICENSE
+-rw-r--r--   0 docker    (1000) docker    (1000)      357 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/vscode/README.md
+-rw-r--r--   0 docker    (1000) docker    (1000)      959 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/vscode/language-configuration.json
+-rw-r--r--   0 docker    (1000) docker    (1000)    11532 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/vscode/lmql-vscode.png
+-rw-r--r--   0 docker    (1000) docker    (1000)     1214 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/vscode/package.json
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.103395 lmql-0.7b2/src/lmql/ui/vscode/syntaxes/
+-rw-r--r--   0 docker    (1000) docker    (1000)      518 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/vscode/syntaxes/lmql.qstring.json
+-rw-r--r--   0 docker    (1000) docker    (1000)      642 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json
+-rw-r--r--   0 docker    (1000) docker    (1000)      853 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/ui/vscode/syntaxes/pylmql.json
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.107395 lmql-0.7b2/src/lmql/utils/
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/utils/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2402 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/utils/docstring_parser.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4933 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/utils/graph.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2715 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql/utils/nputil.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      112 2023-07-28 19:02:08.000000 lmql-0.7b2/src/lmql/version.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-28 19:02:16.063396 lmql-0.7b2/src/lmql.egg-info/
+-rw-r--r--   0 docker    (1000) docker    (1000)     9896 2023-07-28 19:02:15.000000 lmql-0.7b2/src/lmql.egg-info/PKG-INFO
+-rw-r--r--   0 docker    (1000) docker    (1000)    10384 2023-07-28 19:02:16.000000 lmql-0.7b2/src/lmql.egg-info/SOURCES.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)        1 2023-07-28 19:02:15.000000 lmql-0.7b2/src/lmql.egg-info/dependency_links.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)       39 2023-07-28 19:02:15.000000 lmql-0.7b2/src/lmql.egg-info/entry_points.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)       95 2023-07-28 19:02:15.000000 lmql-0.7b2/src/lmql.egg-info/requires.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)        5 2023-07-28 19:02:15.000000 lmql-0.7b2/src/lmql.egg-info/top_level.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)   115785 2023-07-14 11:31:18.000000 lmql-0.7b2/src/lmql.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)       86 2023-07-14 11:31:18.000000 lmql-0.7b2/yarn.lock
```

### Comparing `lmql-0.7b1/.github/workflows/lmql-ci.yml` & `lmql-0.7b2/.github/workflows/lmql-ci.yml`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/.github/workflows/lmql-tests.yml` & `lmql-0.7b2/.github/workflows/lmql-tests.yml`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/.github/workflows/lmql-web.yml` & `lmql-0.7b2/.github/workflows/lmql-web.yml`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/.gitignore` & `lmql-0.7b2/.gitignore`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/LICENSE` & `lmql-0.7b2/LICENSE`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/PKG-INFO` & `lmql-0.7b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmql
-Version: 0.7b1
+Version: 0.7b2
 Summary: A query language for language models.
 Home-page: https://lmql.ai
 Author: Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 Author-email: hello@lmql.ai
 Project-URL: Docs, https://docs.lmql.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lmql Version: 0.7b1 Summary: A query language for
+Metadata-Version: 2.1 Name: lmql Version: 0.7b2 Summary: A query language for
 language models. Home-page: https://lmql.ai Author: Luca Beurer-Kellner, Marc
 Fischer, Martin Vechev Author-email: hello@lmql.ai Project-URL: Docs, https://
 docs.lmql.ai Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.10 Description-Content-
 Type: text/markdown Provides-Extra: hf License-File: LICENSE
                                     [Logo]
                                 **** LMQL ****
```

### Comparing `lmql-0.7b1/README.md` & `lmql-0.7b2/README.md`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/Makefile` & `lmql-0.7b2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/make.bat` & `lmql-0.7b2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/_ext/lmql_snippets.py` & `lmql-0.7b2/docs/source/_ext/lmql_snippets.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/_static/css/lmql-docs.css` & `lmql-0.7b2/docs/source/_static/css/lmql-docs.css`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 .highlight.lmql {
-    border: 1pt solid rgb(212, 212, 212);
     position: relative;
-}
-
-html[data-theme="dark"] .highlight.lmql {
-    border: 1pt solid rgb(110, 109, 109);
+    border-radius: 2pt;
 }
 
 .highlight.lmql iframe {
     background-color: var(--pst-color-background);
 }
 
 .highlight.lmql pre {
@@ -38,15 +34,15 @@
 
     text-align: right;
     font-size: 0.8em;
     font-weight: regular;
     padding: 0;
     position: absolute;
     top: 5pt;
-    right: 5pt;
+    right: 8pt;
     color: var(--pst-color-link);
 }
 
 .highlight.lmql button:hover {
     cursor: pointer;
     text-decoration: underline;
 }
@@ -103,21 +99,21 @@
     font-size: 10pt;
     font-weight: bold;
     font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
     cursor: pointer;
     color:rgba(0, 0, 0, 0.957)
 }
 
-html[data-theme="dark"] .getting-started>a {
+html.dark .getting-started>a {
     background-color: rgb(57, 57, 57) !important;
     border-color: rgb(75, 75, 75);
     color: rgb(215, 215, 215);
 }
 
-html[data-theme="dark"] .getting-started>a.primary {
+html.dark .getting-started>a.primary {
     background-color: rgb(66, 64, 174) !important;
 }
 
 .getting-started>a:hover {
     background-color: rgb(233, 228, 228);
 }
 
@@ -188,48 +184,50 @@
     text-align: center;
     color: grey;
 }
 
 .highlight-model-output {
     position: relative;
     padding-left: 5pt;
-    top: -5pt;
+    top: -10pt;
     padding-right: 5pt;
     z-index: -1;
     font-size: 0.9em;
     font-family: monospace;
 }
 
-html[data-theme="dark"] .highlight-model-output::before {
+html.dark .highlight-model-output::before {
     color: rgb(143, 143, 143);
 }
 
-html[data-theme="dark"] .highlight-model-output {
+html.dark .highlight-model-output {
     background: transparent;
 }
 
-.highlight-model-output .highlight, html[data-theme="dark"] .highlight-model-output .highlight {
+.highlight-model-output .highlight, html.dark .highlight-model-output .highlight {
     display: block;
     white-space: break-spaces !important;
 }
 
 
 .highlight-model-output .highlight {
-    background-color: #fbfbfb !important;
-    border: 0.5pt solid grey;
+    /* background-color: #fbfbfb !important; */
+    /* background-color: #f7f6f9; */
+    border: 1.5pt solid black;
+    border-radius: 2pt;
     position: relative;
     /* top: -12pt; */
-    border-color: rgb(223, 219, 219);
+    border-color: rgb(241, 240, 240);
     white-space: break-spaces !important;
     padding: 10pt;
     padding-top: 20pt;
 }
 
-html[data-theme="dark"] .highlight-model-output .highlight {
-    background-color: rgb(30, 30, 30) !important;
+html.dark .highlight-model-output .highlight {
+    /* background-color: #2c283b8b !important; */
     border-color: rgb(68, 68, 68) !important;
 }
 
 .variable {
     display: inline; 
     padding: 0.5pt;
 }
@@ -285,8 +283,54 @@
 }
 
 .dataframe th {
     width: 120pt !important;
 }
 .dataframe th:first-child {
     width: auto !important;
+}
+
+.globaltoc li a {
+    display: block;
+    padding: 4pt 0pt;
+}
+
+.globaltoc li {
+    padding: 4pt;
+    padding-bottom: 0;
+    padding-top: 0;
+    margin: 0;
+    margin-bottom: 1pt;
+    transition: background-color 0.1s ease-in-out;
+    padding-left: 6pt;
+    padding-right: 6pt;
+}
+
+.globaltoc li.toctree-l2, .globaltoc>ul>li>ul {
+    border-width: 0pt;
+}
+
+.globaltoc li:hover, .globaltoc li.current {
+    background-color: rgb(245, 245, 245);
+    border-radius: 2pt;
+}
+
+html.dark .globaltoc li:hover, html.dark .globaltoc li.current {
+    background-color: rgb(57, 57, 57);
+}
+
+p>code.literal {
+    background-color: #F3F1FA;
+    border-radius: 2pt;
+    padding: 2pt;
+    font-size: 0.9em;
+    color: rgb(0, 0, 0);
+}
+
+html.dark p>code.literal {
+    background-color: #2c283b;
+    color: rgb(215, 215, 215);
+}
+
+.sy-head-nav .link i.external-link {
+    display: none;
 }
```

### Comparing `lmql-0.7b1/docs/source/_static/images/lmql.svg` & `lmql-0.7b2/docs/source/_static/images/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/_static/js/lmql-playground.js` & `lmql-0.7b2/docs/source/_static/js/lmql-playground.js`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/blog/release-0.0.5.md` & `lmql-0.7b2/docs/source/blog/release-0.0.5.md`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/blog/release-0.0.6.1.md` & `lmql-0.7b2/docs/source/blog/release-0.0.6.1.md`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/blog/release-0.0.6.3.md` & `lmql-0.7b2/docs/source/blog/release-0.0.6.3.md`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/blog/release-0.0.6.4.md` & `lmql-0.7b2/docs/source/blog/release-0.0.6.4.md`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/blog/release-0.0.6.5.md` & `lmql-0.7b2/docs/source/blog/release-0.0.6.5.md`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/blog/release-0.0.6.6.md` & `lmql-0.7b2/docs/source/blog/release-0.0.6.6.md`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/blog/release-0.0.6.md` & `lmql-0.7b2/docs/source/blog/release-0.0.6.md`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/dev-setup.md` & `lmql-0.7b2/docs/source/dev-setup.md`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/docker-setup.md` & `lmql-0.7b2/docs/source/docker-setup.md`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/images/inference.svg` & `lmql-0.7b2/docs/source/images/inference.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/index.rst` & `lmql-0.7b2/docs/source/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -59,25 +59,24 @@
 --------
 
 .. toctree::
   :maxdepth: 1
 
   quickstart
   installation
-  ⚡️ Playground IDE <https://lmql.ai/playground>
 
 .. toctree::
-   :maxdepth: 1
+   :maxdepth: 2
    :caption: 📖 LMQL Language 
    
    language/overview.md
    language/scripted_prompts.md
    language/constraints.md
    language/decoders.md
-   language/models.md
+   language/models.rst
    language/functions.md
 
 .. toctree::
     :maxdepth: 1
     :caption: 🔗 Python Integration
     
     python/python.ipynb
```

#### html2text {}

```diff
@@ -14,19 +14,17 @@
 Playground_IDE ð_Getting_Started_Guide ð¼ï¸_Examples_Gallery
 ***** Run Locally *****
 pip install lmql
 To run LMQL locally, read the Installation_Instructions section of the
 documentation.
 ***** Community *****
 ð¬_Discord_Server ð¥_Twitter âï¸_E-Mail
-Contents -------- .. toctree:: :maxdepth: 1 quickstart installation â¡ï¸
-Playground IDE
-lmql.ai/playground> .. toctree:: :maxdepth: 1 :caption: ð LMQL Language
-language/overview.md language/scripted_prompts.md language/constraints.md
-language/decoders.md language/models.md language/functions.md .. toctree:: :
-maxdepth: 1 :caption: ð Python Integration python/python.ipynb python/
-langchain.ipynb python/llama_index.ipynb python/pandas.ipynb python/output.md
-python/comparison.md .. toctree:: :maxdepth: 1 :caption: ð¬ Contribute dev-
-setup docker-setup Discord
+Contents -------- .. toctree:: :maxdepth: 1 quickstart installation ..
+toctree:: :maxdepth: 2 :caption: ð LMQL Language language/overview.md
+language/scripted_prompts.md language/constraints.md language/decoders.md
+language/models.rst language/functions.md .. toctree:: :maxdepth: 1 :caption:
+ð Python Integration python/python.ipynb python/langchain.ipynb python/
+llama_index.ipynb python/pandas.ipynb python/output.md python/comparison.md ..
+toctree:: :maxdepth: 1 :caption: ð¬ Contribute dev-setup docker-setup Discord
 discord.gg/7eJP4fcyNT> GitHub Issues
 github.com/eth-sri/lmql/issues> E-Mail
 lmql.ai>
```

### Comparing `lmql-0.7b1/docs/source/installation.md` & `lmql-0.7b2/docs/source/installation.md`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/language/azure.md` & `lmql-0.7b2/docs/source/language/azure.md`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/language/decoders.md` & `lmql-0.7b2/docs/source/language/decoders.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Decoders
 
 LMQL support various decoding algorithms, which are used to generate text from the token distribution of a language model. The decoding algorithm in use, is specified right at the beginning of a query, e.g. `argmax`. Here, we provide a brief overview of the currently supported decoders.
 
 LMQL also includes a library for array-based decoding `dclib`, which can be used to implement custom decoders. More information on this, will be provided in the future. The implementation of the available decoding procedures is located in `src/lmql/runtime/dclib/decoders.py` of the LMQL repository.
 
-In general, all LMQL decoding algorithms are model-agnostic and can be used with any LMQL-supported inference backend. For more information on the supported inference backends, see the [Models](./models.md) chapter.
+In general, all LMQL decoding algorithms are model-agnostic and can be used with any LMQL-supported inference backend. For more information on the supported inference backends, see the [Models](./models.rst) chapter.
 
 ## Specifying The Decoding Algorithm
 
 Depending on the context, LMQL offers two ways to specify the decoding algorithm to use. 
 
 **Queries with Decoding Clause**: The first option is to simply specify the decoding algorithm and its parameters as part of the query itself. This can be particularly useful, if your choice of decoder is relevant and should be part of your program.
 
@@ -34,15 +34,15 @@
     A:[PUNCHLINE]""" where STOPS_AT(JOKE, "?") and  STOPS_AT(PUNCHLINE, "\n")
     '''
 
 tell_a_joke() # uses the decoder specified in @lmql.query(...)
 tell_a_joke(decoder="beam", n=2) # uses a beam search decoder with n=2
 ```
 
-This is only possible when using LMQL from a Python program. For more information on this, also see the chapter on how to specify the [model to use for decoding](models.md).
+This is only possible when using LMQL from a Python program. For more information on this, also see the chapter on how to specify the [model to use for decoding](models.rst).
 ## Supported Decoding Algorithms
 
 In general, the very first keyword of an LMQL query, specifies the decoding algorithm to use. For this, the following decoder keywords are available:
 
 ### `argmax`
 
 The `argmax` decoder is the simplest decoder available in LMQL. It greedily selects the most likely token at each step of the decoding process. It has no additional parameters. Since `argmax` decoding is deterministic, one can only generate a single sequence at a time.
@@ -78,8 +78,8 @@
 Among other things, this view allows you to track the decoding process, active hypotheses and interpreter state, including the current evaluation result of the `where` clause. For an example, consider the [translation example](https://lmql.ai/playground/#translation) as included in the Playground IDE (make sure to enable `Advanced Mode`).
 
 
 ## Other Decoding Parameters
 
 * `max_len: int` - The maximum length of the generated sequence. If not specified, the default value of `max_len` is `512`. Note if the maximum length is reached, the LMQL runtime will throw an error if the query has not yet come to a valid result, according to the provided `where` clause.
 
-* `openai_chunksize: int` - The chunksize parameter for OpenAI's `Completion` API. If not specified, the default value of `openai_chunksize` is `32`. See also the description of this parameter in the [Models](./models.md#configuring-speculative-openai-api-use) chapter.
+* `openai_chunksize: int` - The chunksize parameter for OpenAI's `Completion` API. If not specified, the default value of `openai_chunksize` is `32`. See also the description of this parameter in the [Models](./models.rst#configuring-speculative-openai-api-use) chapter.
```

### Comparing `lmql-0.7b1/docs/source/language/functions.md` & `lmql-0.7b2/docs/source/language/functions.md`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/language/hf.md` & `lmql-0.7b2/docs/source/language/hf.md`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/language/llama.cpp.md` & `lmql-0.7b2/docs/source/language/llama.cpp.md`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/language/models.md` & `lmql-0.7b2/docs/source/language/models.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,72 @@
-# Models
+Models
+===================================
 
 LMQL is a high-level, front-end language for text generation. This means that LMQL is not specific to any particular text generation model. Instead, we support a wide range of text generation models on the backend, including [OpenAI models](https://platform.openai.com/docs/models), as well as self-hosted models via [🤗 Transformers](https://huggingface.co/transformers).
 
 Due to the modular design of LMQL, it is easy to add support for new models and backends. If you would like to propose or add support for a new model API or inference engine, please reach out to us via our [Community Discord](https://discord.com/invite/7eJP4fcyNT) or via [hello@lmql.ai](mailto:hello@lmql.ai).
 
-## Specifying The Model
+Specifying The Model
+--------------------
 
 LMQL offers two ways to specify the model that is used as underlying LLM:
 
 **Queries with `from` Clause**: The first option is to simply specify the model as part of the query itself. For this, you can use the `from` in combination with the indented syntax. This can be particularly useful, if your choice of model is intentional and should be part of your program.
 
-```{lmql}
-
-name::specify-decoder
-argmax
-    "This is a query with a specified decoder: [RESPONSE]
-from
-    "openai/text-ada-001"
-```
+.. lmql:: 
+    name::specify-model
+    argmax
+        "This is a query with a specified decoder: [RESPONSE]
+    from
+        "openai/text-ada-001"
 
 **Specifying the Model Externally**: The second option is to specify the model and its parameters externally, i.e. separately from the actual program code:
 
-```python
-import lmql
 
-# uses 'chatgpt' by default
-@lmql.query(model="chatgpt")
-def tell_a_joke():
-    '''lmql
-    """A list of good dad jokes. A indicates the punchline
-    Q: How does a penguin build its house?
-    A: Igloos it together.
-    Q: Which knight invented King Arthur's Round Table?
-    A: Sir Cumference.
-    Q:[JOKE]
-    A:[PUNCHLINE]""" where STOPS_AT(JOKE, "?") and  STOPS_AT(PUNCHLINE, "\n")
-    '''
+.. code-block:: python
+
+    import lmql
 
-tell_a_joke() # uses chatgpt
+    # uses 'chatgpt' by default
+    @lmql.query(model="chatgpt")
+    def tell_a_joke():
+        '''lmql
+        """A list of good dad jokes. A indicates the punchline
+        Q: How does a penguin build its house?
+        A: Igloos it together.
+        Q: Which knight invented King Arthur's Round Table?
+        A: Sir Cumference.
+        Q:[JOKE]
+        A:[PUNCHLINE]""" where STOPS_AT(JOKE, "?") and  STOPS_AT(PUNCHLINE, "\n")
+        '''
 
-tell_a_joke(model="openai/text-davinci-003") # uses text-davinci-003
+    tell_a_joke() # uses chatgpt
 
-```
+    tell_a_joke(model="openai/text-davinci-003") # uses text-davinci-003
 
 This is only possible when using LMQL from a Python program. When running in the playground, you can alternatively use the model dropdown available in the top right of the program editor:
 
-<center>
-    <img src="https://github.com/eth-sri/lmql/assets/17903049/5ba2ffdd-e64d-465c-85be-5d9dc2ab6c14" width="70%" alt="Screenshot of the model dropdown in the playground" />
-</center>
-
-## Available Model Backends
-
-```{toctree}
-:maxdepth: 1
-
-openai.md
-azure.md
-hf.md
-llama.cpp.md
-```
+.. raw html  
+.. figure:: https://github.com/eth-sri/lmql/assets/17903049/5ba2ffdd-e64d-465c-85be-5d9dc2ab6c14
+    :align: center
+    :width: 70%
+    :alt: Screenshot of the model dropdown in the playground
+
+    Screenshot of the model dropdown in the playground
 
-## Using Multiple Models
+Using Multiple Models
+---------------------
 
 LMQL currently supports the use of only one model per query. If you want to mix multiple models, the advised way is to use multiple queries that are executed in sequence. The main obstacles in supporting this, is the fact that different models produce differently scaled token probabilities, which means an end-to-end decoding process would be difficult to implement. 
 
-However, we are actively exploring ways to [support this in the future](https://github.com/eth-sri/lmql/issues/82).
+However, we are actively exploring ways to [support this in the future](https://github.com/eth-sri/lmql/issues/82).
+
+Available Model Backends
+------------------------
+
+.. toctree::
+    :maxdepth: 1
+    
+    ./openai.md
+    ./azure.md
+    ./hf.md
+    ./llama.cpp.md
```

### Comparing `lmql-0.7b1/docs/source/language/openai.md` & `lmql-0.7b2/docs/source/language/openai.md`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/language/overview.md` & `lmql-0.7b2/docs/source/language/overview.md`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/language/scripted_prompts.md` & `lmql-0.7b2/docs/source/language/scripted_prompts.md`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/lmql.svg` & `lmql-0.7b2/docs/source/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/logo.png` & `lmql-0.7b2/docs/source/logo.png`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/pending/release-next.md` & `lmql-0.7b2/docs/source/pending/release-next.md`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/python/comparison.md` & `lmql-0.7b2/docs/source/python/comparison.md`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/python/langchain.ipynb` & `lmql-0.7b2/docs/source/python/langchain.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/python/lc.py` & `lmql-0.7b2/docs/source/python/lc.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/python/llama_index.ipynb` & `lmql-0.7b2/docs/source/python/llama_index.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/python/lmql.txt` & `lmql-0.7b2/docs/source/python/lmql.txt`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/python/output.ipynb` & `lmql-0.7b2/docs/source/python/output.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/python/pandas.ipynb` & `lmql-0.7b2/docs/source/python/pandas.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/python/python.ipynb` & `lmql-0.7b2/docs/source/python/python.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/docs/source/quickstart.md` & `lmql-0.7b2/docs/source/quickstart.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,13 +53,13 @@
 
 **Prompt Program**: The main body of the program specifies the prompt. As before, we use prompt statements here, however, now we also make use of control-flow and branching behavior.
     
 On each LLM call, the concatenation of all prompt statements so far, form the prompt used to generate a value for the currently active template variable like `RESPONSE`. This means the LLM is always aware of the full prompt context so far, when generating a value for a template variable.
     
 After a prompt statement has been executed, the contained template variables are automatically exposed to the surrounding program context. This allows you to react to model output and incorporate the results in your program logic. To learn more about this form of interactive prompting, please see [Scripted Prompting](./language/scripted_prompts.md).
 
-**Model Clause** `from "openai/text-ada-001"`: In this extended version we now specify a specific model to use for text generation. LMQL supports [OpenAI models](https://platform.openai.com/docs/models), like GPT-3.5 variants, ChatGPT, and GPT-4, but also self-hosted models, e.g. via [🤗 Transformers](https://huggingface.co/transformers). For more details, please see [Models](./language/models.md). By default, LMQL relies on `openai/text-davinci-003`, if not specified otherwise.
+**Model Clause** `from "openai/text-ada-001"`: In this extended version we now specify a specific model to use for text generation. LMQL supports [OpenAI models](https://platform.openai.com/docs/models), like GPT-3.5 variants, ChatGPT, and GPT-4, but also self-hosted models, e.g. via [🤗 Transformers](https://huggingface.co/transformers). For more details, please see [Models](./language/models.rst). By default, LMQL relies on `openai/text-davinci-003`, if not specified otherwise.
 ## 3. Enjoy
 
 These basic steps should get you started with LMQL. If you need more inspiration before writing your own queries, you can explore the examples included with the [Playground IDE](https://lmql.ai/playground) or showcased on the [LMQL Website](https://lmql.ai/).
 
 If you have any questions and or requests for documentation, please feel free to reach out to us via our [Community Discord](https://discord.com/invite/7eJP4fcyNT), [GitHub Issues](https://github.com/eth-sri/lmql/issues), or [Twitter](https://twitter.com/lmqllang).
```

### Comparing `lmql-0.7b1/docs/source/releases/misc-snippets.md` & `lmql-0.7b2/docs/source/releases/misc-snippets.md`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/scripts/Dockerfile` & `lmql-0.7b2/scripts/Dockerfile`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/scripts/pypi-release.sh` & `lmql-0.7b2/scripts/pypi-release.sh`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/scripts/serve-all.py` & `lmql-0.7b2/scripts/serve-all.py`

 * *Files 9% similar despite different names*

```diff
@@ -57,14 +57,18 @@
 processes.append(autobuild_blog_p)
 
 # autobuild web/
 # onchange "index.template.html" "**/*.js" "**/*.css" "**/*.md" -e "./index.html" -- node generate.js
 autobuild_web_p = subprocess.Popen(["onchange", "index.template.html", "**/*.js", "**/*.css", "**/*.md", "-e", "./index.html", "--", "node", "generate.js"], cwd="web")
 processes.append(autobuild_web_p)
 
+# autobuild web/actions
+auto_build_actions_p = subprocess.Popen(["onchange", "**/*.js", "**/*.css", "**/*.md", "**/*.html", "**/*.pd", "**/*.json", "-e", "./index.html", "--", "node", "generate.js"], cwd="web/actions")
+processes.append(auto_build_actions_p)
+
 while True:
     try:
         print(summary)
         # listen for keyboard input
         command = input("Enter command (q to quit, bb to build browser playground, docs-clean to clean build docs, web-clean to clean build web-deploy): ")
         if command == "q":
             raise KeyboardInterrupt
```

### Comparing `lmql-0.7b1/scripts/wheel.sh` & `lmql-0.7b2/scripts/wheel.sh`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/setup.cfg` & `lmql-0.7b2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lmql
-version = 0.7b1
+version = 0.7b2
 author = Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 author_email = hello@lmql.ai
 description = A query language for language models.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://lmql.ai
 project_urls =
```

### Comparing `lmql-0.7b1/src/lmql/__init__.py` & `lmql-0.7b2/src/lmql/__init__.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/algorithms/cache.py` & `lmql-0.7b2/src/lmql/algorithms/cache.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/algorithms/functools.py` & `lmql-0.7b2/src/lmql/algorithms/functools.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/cli.py` & `lmql-0.7b2/src/lmql/cli.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/demo.py` & `lmql-0.7b2/src/lmql/demo.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/http.py` & `lmql-0.7b2/src/lmql/http.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/language/compiler.py` & `lmql-0.7b2/src/lmql/language/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,36 +114,41 @@
 
         # collect defined vars in prompt
         for p in query.prompt: 
             self.visit(p)
 
         # also collect variable reads from where clause
         if query.where is not None:
-            FreeVarCollector(self.free_vars, exclude_criteria=[self.exclude_identifier]).visit(query.where)
+            self.visit_where(query.where)
         if query.from_ast is not None:
             FreeVarCollector(self.free_vars, exclude_criteria=[self.exclude_identifier]).visit(query.from_ast)
         if query.decode is not None:
             FreeVarCollector(self.free_vars, exclude_criteria=[self.exclude_identifier]).visit(query.decode)
         if query.distribution is not None:
             FreeVarCollector(self.free_vars, exclude_criteria=[self.exclude_identifier]).visit(query.distribution.values)
 
         # remove all defined and prologue vars from free vars
         self.free_vars = self.free_vars - self.defined_vars - self.prologue_vars - self.defined_constraints
 
         query.scope = self
 
+    def visit_where(self, node):
+        FreeVarCollector(self.free_vars, exclude_criteria=[self.exclude_identifier]).visit(node)
+
     def visit_Expr(self, expr):
         if type(expr.value) is ast.Constant:
             self.scope_Constant(expr.value)
         else:
             super().generic_visit(expr)
 
     def visit_BoolOp(self, node: ast.BoolOp) -> Any:
         if is_query_string_with_constraints(node):
             self.scope_Constant(node.values[0])
+            for constraint in node.values[1:]:
+                self.visit_where(constraint)
         else:
             super().generic_visit(node)
 
     def scope_Constant(self, node):
         if type(node.value) is not str: return super().visit_Constant(node)
         qstring = node.value
 
@@ -515,15 +520,17 @@
                 return f"{constraint_ref}([{args_list}])"
             if is_allowed_builtin_python_call(expr.func):
                 return self.default_transform_node(expr, snf).strip()
             
             assert type(expr.func) is ast.Name, "In LMQL constraint expressions, only function calls to direct function references are allowed: {}".format(astunparse.unparse(expr))
             tfunc = ast.unparse(expr.func)
             targs = [self.transform_node(a, snf) for a in expr.args]
-            targs_list = ", ".join(targs)
+            kwargs = [f"('__kw:{e.arg}', {self.transform_node(e.value, snf)})" for e in expr.keywords]
+            targs_list = ", ".join(targs + kwargs)
+
             return f"{OPS_NAMESPACE}.CallOp([{tfunc}, [{targs_list}]], locals(), globals())"
         elif type(expr) is ast.List:
             return self.default_transform_node(expr, snf).strip()
 
         print(f"compiler warning: expressions of type {type(expr)} are not explicitly supported: '{astunparse.unparse(expr).strip()}'")
         return snf.add(self.default_transform_node(expr, snf))
```

### Comparing `lmql-0.7b1/src/lmql/language/fragment_parser.py` & `lmql-0.7b2/src/lmql/language/fragment_parser.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/language/qstrings.py` & `lmql-0.7b2/src/lmql/language/qstrings.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/language/validator.py` & `lmql-0.7b2/src/lmql/language/validator.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/lib/actions.py` & `lmql-0.7b2/src/lmql/lib/actions.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,94 +70,84 @@
 DELIMITER = "<<"
 DELIMITER_END = ">>"
 
 
 @lmql.query
 async def fct_call(fcts):
     '''lmql
-    incontext
-        action_fcts = {str(f.__name__): make_fct(f) for f in fcts}
-        "[CALL]"
-        truncated = CALL
-        if not CALL.endswith("|") and not CALL.endswith(DELIMITER_END):
+    action_fcts = {str(f.__name__): make_fct(f) for f in fcts}
+    "[CALL]" where STOPS_AT(CALL, "|") and STOPS_AT(CALL, DELIMITER_END)
+
+    truncated = CALL
+    if not CALL.endswith("|") and not CALL.endswith(DELIMITER_END):
+        return CALL
+    else:    
+        if CALL.endswith(DELIMITER_END):
+            CALL = CALL[:-len(DELIMITER_END)]
+        else:
+            CALL = CALL[:-len("|")]
+        
+        if "(" not in CALL:
             return CALL
-        else:    
-            if CALL.endswith(DELIMITER_END):
-                CALL = CALL[:-len(DELIMITER_END)]
-            else:
-                CALL = CALL[:-len("|")]
-            
-            if "(" not in CALL:
-                return CALL
-            
-            action, args = CALL.split("(", 1)
-            action = action.strip()
-            if action not in action_fcts.keys():
-                print("unknown action", [action], list(action_fcts.keys()))
-                " Unknown action: {action} {DELIMITER_END}"
-                result = ""
+        
+        action, args = CALL.split("(", 1)
+        action = action.strip()
+        if action not in action_fcts.keys():
+            print("unknown action", [action], list(action_fcts.keys()))
+            " Unknown action: {action} {DELIMITER_END}"
+            result = ""
+            return "(error)"
+        else:
+            try:
+                result = await action_fcts[action].call("(" + args.strip())
+                return DELIMITER + str(CALL) + "| " + str(result)
+            except Exception:
+                result = "Error."
                 return "(error)"
-            else:
-                try:
-                    result = await action_fcts[action].call("(" + args.strip())
-                    return DELIMITER + str(CALL) + "| " + str(result)
-                except Exception:
-                    result = "Error."
-                    return "(error)"
-    where
-        STOPS_AT(CALL, "|") and STOPS_AT(CALL, DELIMITER_END)
     '''
 
 
 @lmql.query
 async def inline_segment(fcts):
     '''lmql
-    incontext
-        "[SEGMENT]"
-        if not SEGMENT.endswith(DELIMITER):
-            return SEGMENT
-        else:
-            "[CALL]"
-            result = CALL.split("|", 1)[1]
-            return SEGMENT[:-len(DELIMITER)] + CALL + DELIMITER_END
-    where
-        STOPS_AT(SEGMENT, DELIMITER) and fct_call(CALL, fcts)
+    "[SEGMENT]" where STOPS_AT(SEGMENT, DELIMITER)
+    if not SEGMENT.endswith(DELIMITER):
+        return SEGMENT
+    else:
+        "[CALL]" where fct_call(CALL, fcts) and len(TOKENS(CALL)) > 0
+        result = CALL.split("|", 1)[1]
+        return SEGMENT[:-len(DELIMITER)] + CALL + DELIMITER_END
     '''
 
 @lmql.query
-async def inline_use(fcts):
+async def inline_use(fcts, instruct=True):
     '''lmql
-    incontext
-        action_fcts = {str(f.__name__): make_fct(f) for f in fcts}
-        first_tool_name = list(action_fcts.keys())[0] if len(action_fcts) > 0 else "tool"
+    action_fcts = {str(f.__name__): make_fct(f) for f in fcts}
+    first_tool_name = list(action_fcts.keys())[0] if len(action_fcts) > 0 else "tool"
 
-        # add instruction prompt if no few-shot prompt was already used
-        if not INLINE_USE_PROMPT in context.prompt:
-            """
-            \n\n{:system} Instructions: In your reasoning, you can use the following tools:"""
-            
-            for fct in action_fcts.values():
-                "\n   - {fct.name}: {fct.description} Usage: {DELIMITER}{fct.example} | {fct.example_result}{DELIMITER_END}"
-            '   Example Use: ... this means they had <<calc("5-2") | 3 >> 3 apples left...\n'
-            "   You can also use the tools multiple times in one reasoning step.\n\n"
-            "Reasoning with Tools: {:assistant}"
-        else:
-            "\n\nInline Tool Use:\n\n"
+    # add instruction prompt if no few-shot prompt was already used
+    if instruct and not INLINE_USE_PROMPT in context.prompt:
+        """
+        \n\nInstructions: In your reasoning, you can use the following tools:"""
         
-        # decode segment-by-segment, handling action calls along the way
-        truncated = ""
-        while True: 
-            "[SEGMENT]"
-            if not SEGMENT.endswith(DELIMITER_END):
-                " " # seems to be needed for now
-                return truncated + SEGMENT
-            truncated += SEGMENT
-        return truncated
-    where
-        inline_segment(SEGMENT, fcts)
+        for fct in action_fcts.values():
+            "\n   - {fct.name}: {fct.description} Usage: {DELIMITER}{fct.example} | {fct.example_result}{DELIMITER_END}"
+        '   Example Use: ... this means they had <<calc("5-2") | 3 >> 3 apples left...\n'
+        "   You can also use the tools multiple times in one reasoning step.\n\n"
+        "Reasoning with Tools:\n\n"
+    
+    # decode segment-by-segment, handling action calls along the way
+    truncated = ""
+    while True: 
+        "[SEGMENT]" where inline_segment(SEGMENT, fcts)
+        if not SEGMENT.endswith(DELIMITER_END):
+            " " # seems to be needed for now
+            return truncated + SEGMENT
+        truncated += SEGMENT
+    return truncated
     '''
 inline_use.demonstrations = INLINE_USE_PROMPT
 
 def dedent(code):
     common_indent = None
     for line in code.split("\n"):
         if line.strip() == "":
@@ -312,17 +302,17 @@
     except Exception as e:
         if "unmatched" in str(e) or "never closed" in str(e) or "unterminated" in str(e):
             acc = last_line
             return "", acc
         return "", None
 
 @lmql.query
-async def reAct(fcts):
+async def reAct(fcts, instruct=True):
     '''lmql
-    incontext
+    if instruct:
         """
         Instructions: In your reasoning adhere to the following structure:
 
             Thought: <your conclusions>
             
             If required you can also use the following actions:
                 Action: tool(<ARG>)
@@ -330,49 +320,47 @@
         
             Available Tools:
         """
         action_fcts = {str(f.__name__): make_fct(f) for f in fcts}
         
         for fct in action_fcts.values():
             "   - {fct.name}: {fct.description}. Usage: {fct.example}. Observation: {fct.example_result}\n"
-        
+    
         "Now you can start reasoning.\n"
-            
-        offset = len(context.prompt)
         
-        while True:
-            "[SEGMENT]"
+    offset = len(context.prompt)
+    
+    while True:
+        "[SEGMENT]" where STOPS_AT(SEGMENT, "Action:")
 
-            if not SEGMENT.endswith("Action:"):
-                break
+        if not SEGMENT.endswith("Action:"):
+            break
+        else:
+            "[CALL]" where STOPS_AT(CALL, "\n")
+            
+            if not CALL.endswith("\n") or not "(" in CALL:
+                continue
             else:
-                "[CALL]"
-                
-                if not CALL.endswith("\n") or not "(" in CALL:
-                    continue
+                "Observation:"
+                action, args = CALL.split("(", 1)
+                action = action.strip()
+                if action not in action_fcts.keys():
+                    print("unknown action", [action], list(action_fcts.keys()))
+                    " Unknown action: {action}\n"
+                    result = ""
                 else:
-                    "Observation:"
-                    action, args = CALL.split("(", 1)
-                    action = action.strip()
-                    if action not in action_fcts.keys():
-                        print("unknown action", [action], list(action_fcts.keys()))
-                        " Unknown action: {action}\n"
-                        result = ""
-                    else:
-                        try:
-                            result = await action_fcts[action].call("(" + args)
-                            if type(result) is float:
-                                result = round(result, 2)
-                            " {result}\n"
-                        except Exception:
-                            " Error. Try differently.\n"
-        
-        return "\n" + context.prompt[offset:]
-    where
-        STOPS_AT(SEGMENT, "Action:") and STOPS_AT(CALL, "\n")
+                    try:
+                        result = await action_fcts[action].call("(" + args)
+                        if type(result) is float:
+                            result = round(result, 2)
+                        " {result}\n"
+                    except Exception:
+                        " Error. Try differently.\n"
+    
+    return "\n" + context.prompt[offset:]
     '''
 
 
 if __name__ == "__main__":
     code = ' eggs_per_day = 16\n    eggs_eaten = 3\n    eggs_baked = 4933828\n    egg_price = 2\n   \n   money_made = (eggs_per_day - eggs_eaten - eggs_baked) * egg_price #|'
     print(dedent(code))
     print(exec(dedent(code)))
```

### Comparing `lmql-0.7b1/src/lmql/lib/algebra222.csv` & `lmql-0.7b2/src/lmql/lib/algebra222.csv`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/lib/data.py` & `lmql-0.7b2/src/lmql/lib/data.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/lib/prompts/inline_code copy.py` & `lmql-0.7b2/src/lmql/lib/prompts/inline_code copy.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/lib/prompts/inline_code.py` & `lmql-0.7b2/src/lmql/lib/prompts/inline_code.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/lib/prompts/inline_use.py` & `lmql-0.7b2/src/lmql/lib/prompts/inline_use.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/lib/prompts/inline_use_kevin.py` & `lmql-0.7b2/src/lmql/lib/prompts/inline_use_kevin.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/lib/prompts/wiki_prompt.py` & `lmql-0.7b2/src/lmql/lib/prompts/wiki_prompt.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/lib/types.py` & `lmql-0.7b2/src/lmql/lib/types.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/lib/value.py` & `lmql-0.7b2/src/lmql/lib/value.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/models/lmtp/README.md` & `lmql-0.7b2/src/lmql/models/lmtp/README.md`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/models/lmtp/backends/__main__.py` & `lmql-0.7b2/src/lmql/models/lmtp/backends/__main__.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/models/lmtp/backends/llama_cpp_model.py` & `lmql-0.7b2/src/lmql/models/lmtp/backends/llama_cpp_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,17 +36,17 @@
                 else:
                     break
             if longest_prefix > 0:
                 tokens = tokens[longest_prefix:]
                 self.llm.n_tokens = longest_prefix
 
         self.llm.eval(tokens)
-        scores = np.array([self.llm.scores[j][i] for j,i in enumerate(input_ids[0])])
-        scores = nputil.log_softmax(scores, axis=-1)
-        # print("llama_cpp_model: score() took", time.time() - s, "seconds", file=sys.stderr)
+        logits = np.array(self.llm.scores)
+        logits = nputil.log_softmax(logits, axis=-1)
+        scores = np.array([logits[j][i] for j,i in enumerate(input_ids[0])])
 
         return scores.reshape(1, -1)
     
     def generate(self, input_ids, attention_mask, 
                  temperature: float, max_new_tokens: int, 
                  bias_tensor, streamer: TokenStreamer) -> LMTPModelResult:
         token_scores = []
```

### Comparing `lmql-0.7b1/src/lmql/models/lmtp/backends/lmtp_model.py` & `lmql-0.7b2/src/lmql/models/lmtp/backends/lmtp_model.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/models/lmtp/backends/random_model.py` & `lmql-0.7b2/src/lmql/models/lmtp/backends/random_model.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/models/lmtp/backends/transformers_model.py` & `lmql-0.7b2/src/lmql/models/lmtp/backends/transformers_model.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/models/lmtp/lmtp_async.py` & `lmql-0.7b2/src/lmql/models/lmtp/lmtp_async.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/models/lmtp/lmtp_client.py` & `lmql-0.7b2/src/lmql/models/lmtp/lmtp_client.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/models/lmtp/lmtp_dcmodel.py` & `lmql-0.7b2/src/lmql/models/lmtp/lmtp_dcmodel.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/models/lmtp/lmtp_inference_server.py` & `lmql-0.7b2/src/lmql/models/lmtp/lmtp_inference_server.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/models/lmtp/lmtp_multiprocessing.py` & `lmql-0.7b2/src/lmql/models/lmtp/lmtp_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/models/lmtp/lmtp_scheduler.py` & `lmql-0.7b2/src/lmql/models/lmtp/lmtp_scheduler.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/models/lmtp/lmtp_serve.py` & `lmql-0.7b2/src/lmql/models/lmtp/lmtp_serve.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/models/lmtp/lmtp_threading.py` & `lmql-0.7b2/src/lmql/models/lmtp/lmtp_threading.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/models/lmtp/utils.py` & `lmql-0.7b2/src/lmql/models/lmtp/utils.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/models/model.py` & `lmql-0.7b2/src/lmql/models/model.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ops/booleans.py` & `lmql-0.7b2/src/lmql/ops/booleans.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ops/follow_map.py` & `lmql-0.7b2/src/lmql/ops/follow_map.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ops/inline_call.py` & `lmql-0.7b2/src/lmql/ops/inline_call.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,15 +53,21 @@
             # print(f"internal warning: InlineCallOp could not find subinterpreter forward() result in context ProgramState: " + str(context.subinterpreter_results))
             return None
         return context.subinterpreter_results[si]
     
     def subinterpreter(self, runtime, prompt, args = None):
         query_kwargs = None
         if args is not None:
-            query_kwargs, _ = self.query_fct.make_kwargs(*args[1:])
+            args = args[1:]
+            def is_kwarg(a):
+                return type(a) is tuple and len(a) == 2 and type(a[0]) is str and a[0].startswith("__kw:")
+            kwargs = {k[0][len("__kw:"):]: k[1] for k in args if is_kwarg(k)}
+            args = [a for a in args if not is_kwarg(a)]
+
+            query_kwargs, _ = self.query_fct.make_kwargs(*args, **kwargs)
             self.query_kwargs = query_kwargs
         else:
             if self.query_kwargs is None:
                 return None
             query_kwargs = self.query_kwargs
 
         return runtime.subinterpreter(id(self), prompt, self.query_fct, query_kwargs)
@@ -85,15 +91,15 @@
         _, args, context = operands
         runtime = context.runtime
         # instructs postprocessing logic to use subinterpreters results as postprocessing results
         si = self.subinterpreter(runtime, context.prompt, args)
         return si
     
     def postprocess_order(self, other, operands, other_inputs, **kwargs):
-        return 0 # other constraints cannot be compared
+        return "before" # other constraints cannot be compared
 
     @staticmethod
     def collect(op: Node):
         if isinstance(op, InlineCallOp):
             return [op]
         elif isinstance(op, AndOp) or isinstance(op, OrOp) or isinstance(op, NotOp):
             return [o for p in op.predecessors for o in InlineCallOp.collect(p)]
```

### Comparing `lmql-0.7b1/src/lmql/ops/node.py` & `lmql-0.7b2/src/lmql/ops/node.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ops/ops.py` & `lmql-0.7b2/src/lmql/ops/ops.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ops/regex.py` & `lmql-0.7b2/src/lmql/ops/regex.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ops/token_set.py` & `lmql-0.7b2/src/lmql/ops/token_set.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/output/http.py` & `lmql-0.7b2/src/lmql/output/http.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/output/sse.py` & `lmql-0.7b2/src/lmql/output/sse.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/output/ws.py` & `lmql-0.7b2/src/lmql/output/ws.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/runtime/bopenai/__init__.py` & `lmql-0.7b2/src/lmql/runtime/bopenai/__init__.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/runtime/bopenai/batched_openai.py` & `lmql-0.7b2/src/lmql/runtime/bopenai/batched_openai.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/runtime/bopenai/openai_api.py` & `lmql-0.7b2/src/lmql/runtime/bopenai/openai_api.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/runtime/caching.py` & `lmql-0.7b2/src/lmql/runtime/caching.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/runtime/dclib/dclib_array.py` & `lmql-0.7b2/src/lmql/runtime/dclib/dclib_array.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/runtime/dclib/dclib_cache.py` & `lmql-0.7b2/src/lmql/runtime/dclib/dclib_cache.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/runtime/dclib/dclib_global.py` & `lmql-0.7b2/src/lmql/runtime/dclib/dclib_global.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/runtime/dclib/dclib_model.py` & `lmql-0.7b2/src/lmql/runtime/dclib/dclib_model.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/runtime/dclib/dclib_rewrite.py` & `lmql-0.7b2/src/lmql/runtime/dclib/dclib_rewrite.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/runtime/dclib/dclib_seq.py` & `lmql-0.7b2/src/lmql/runtime/dclib/dclib_seq.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/runtime/dclib/decoders.py` & `lmql-0.7b2/src/lmql/runtime/dclib/decoders.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/runtime/interpreter.py` & `lmql-0.7b2/src/lmql/runtime/interpreter.py`

 * *Files 0% similar despite different names*

```diff
@@ -410,15 +410,15 @@
             query_head=query_head,
             program_state=program_state
         )
 
     def process_query_string(self, s: str):
         if not ("turbo" in self.model_identifier or "gpt-4" in self.model_identifier):
             # replace all r"<lmql:(.*?)\/>" tags with ((\1))
-            s = re.sub(r"<lmql:(.*?)\/>", "", s)
+            s = re.sub(r"<lmql:(.*?)\/>", r"((\1)):", s)
         s = unescape_qstring(s)
         return s
 
     def interpreter_state_user_data(self, state: PromptState):
         return {self.user_data_key: state}
 
     def interpreter_state_from_user_data(self, seq, noroot=False):
```

### Comparing `lmql-0.7b1/src/lmql/runtime/langchain.py` & `lmql-0.7b2/src/lmql/runtime/langchain.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/runtime/lmql_runtime.py` & `lmql-0.7b2/src/lmql/runtime/lmql_runtime.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/runtime/loop.py` & `lmql-0.7b2/src/lmql/runtime/loop.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/runtime/maiohttp.py` & `lmql-0.7b2/src/lmql/runtime/maiohttp.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/runtime/masks.py` & `lmql-0.7b2/src/lmql/runtime/masks.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/runtime/model_registry.py` & `lmql-0.7b2/src/lmql/runtime/model_registry.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/runtime/multi_head_interpretation.py` & `lmql-0.7b2/src/lmql/runtime/multi_head_interpretation.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/runtime/openai_integration.py` & `lmql-0.7b2/src/lmql/runtime/openai_integration.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/runtime/openai_secret.py` & `lmql-0.7b2/src/lmql/runtime/openai_secret.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/runtime/output_writer.py` & `lmql-0.7b2/src/lmql/runtime/output_writer.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/runtime/postprocessing/conditional_prob.py` & `lmql-0.7b2/src/lmql/runtime/postprocessing/conditional_prob.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/runtime/program_state.py` & `lmql-0.7b2/src/lmql/runtime/program_state.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/runtime/stats.py` & `lmql-0.7b2/src/lmql/runtime/stats.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/runtime/token_distribution.py` & `lmql-0.7b2/src/lmql/runtime/token_distribution.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/runtime/tokenizer.py` & `lmql-0.7b2/src/lmql/runtime/tokenizer.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/runtime/tokenizers/hf_tokenizer.py` & `lmql-0.7b2/src/lmql/runtime/tokenizers/hf_tokenizer.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/runtime/tokenizers/pure_python_tokenizer.py` & `lmql-0.7b2/src/lmql/runtime/tokenizers/pure_python_tokenizer.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/runtime/tokenizers/tiktoken_tokenizer.py` & `lmql-0.7b2/src/lmql/runtime/tokenizers/tiktoken_tokenizer.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/all.py` & `lmql-0.7b2/src/lmql/tests/all.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/expr_test_utils.py` & `lmql-0.7b2/src/lmql/tests/expr_test_utils.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/fin_and.py` & `lmql-0.7b2/src/lmql/tests/fin_and.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/outdated/mask_product_test.py` & `lmql-0.7b2/src/lmql/tests/outdated/mask_product_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/outdated/monotonicity.py` & `lmql-0.7b2/src/lmql/tests/outdated/monotonicity.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/outdated/one_of_tests.py` & `lmql-0.7b2/src/lmql/tests/outdated/one_of_tests.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/outdated/sentences_op.py` & `lmql-0.7b2/src/lmql/tests/outdated/sentences_op.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/outdated/starts_with_op_test.py` & `lmql-0.7b2/src/lmql/tests/outdated/starts_with_op_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/outdated/stops_at.py` & `lmql-0.7b2/src/lmql/tests/outdated/stops_at.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/outdated/str_in_str_tests.py` & `lmql-0.7b2/src/lmql/tests/outdated/str_in_str_tests.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/outdated/test_multi_head.py` & `lmql-0.7b2/src/lmql/tests/outdated/test_multi_head.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/outdated/token_set_test.py` & `lmql-0.7b2/src/lmql/tests/outdated/token_set_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/queryargs/test_args.py` & `lmql-0.7b2/src/lmql/tests/queryargs/test_args.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/queryargs/test_args_query_str.py` & `lmql-0.7b2/src/lmql/tests/queryargs/test_args_query_str.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/queryargs/test_args_run.py` & `lmql-0.7b2/src/lmql/tests/queryargs/test_args_run.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/queryargs/test_sync.py` & `lmql-0.7b2/src/lmql/tests/queryargs/test_sync.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/queryargs/test_var_errors.py` & `lmql-0.7b2/src/lmql/tests/queryargs/test_var_errors.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/system/basic_use_cases.py` & `lmql-0.7b2/src/lmql/tests/system/basic_use_cases.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/tail_token_set.py` & `lmql-0.7b2/src/lmql/tests/tail_token_set.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/test_back2back_caching.py` & `lmql-0.7b2/src/lmql/tests/test_back2back_caching.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/test_eq.py` & `lmql-0.7b2/src/lmql/tests/test_eq.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/test_escaping.py` & `lmql-0.7b2/src/lmql/tests/test_escaping.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/test_f.py` & `lmql-0.7b2/src/lmql/tests/test_f.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/test_local_model_python.py` & `lmql-0.7b2/src/lmql/tests/test_local_model_python.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/test_minimal_syntax.py` & `lmql-0.7b2/src/lmql/tests/test_minimal_syntax.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/test_multibyte_characters.py` & `lmql-0.7b2/src/lmql/tests/test_multibyte_characters.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/test_multibyte_local_models.py` & `lmql-0.7b2/src/lmql/tests/test_multibyte_local_models.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/test_qstrings.py` & `lmql-0.7b2/src/lmql/tests/test_qstrings.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/test_sample_queries.py` & `lmql-0.7b2/src/lmql/tests/test_sample_queries.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/test_scoping.py` & `lmql-0.7b2/src/lmql/tests/test_scoping.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/test_stopping.py` & `lmql-0.7b2/src/lmql/tests/test_stopping.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/tests/tiktoken_tsets.py` & `lmql-0.7b2/src/lmql/tests/tiktoken_tsets.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/chat/__init__.py` & `lmql-0.7b2/src/lmql/ui/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/chat/assets/code.svg` & `lmql-0.7b2/src/lmql/ui/chat/assets/code.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/chat/assets/index.css` & `lmql-0.7b2/src/lmql/ui/chat/assets/index.css`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/chat/assets/index.html` & `lmql-0.7b2/src/lmql/ui/chat/assets/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -202,15 +202,15 @@
     }
     </script>
 </head>
 <body>
     <div class="content side-view">
         <div class="front side">
         <div class="toolbar">
-            <span class="icon">🤖</span>
+            <img src="chat_assets/lmql.svg" />
             <h1>LMQL Chat</h1>
             <h2 id="connection-status"></h2>
             <button onclick="document.querySelector('.content').classList.toggle('side-view')">
                 <img src="chat_assets/code.svg"/>
             </button>
         </div>
         <div class="chat"></div>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
 
 
-ð¤
+[chat_assets/lmql.svg]
 ****** LMQL Chat ******
  [chat_assets/code.svg]
   [chat_assets/send.svg]
 ****** Internal Trace ******
```

### Comparing `lmql-0.7b1/src/lmql/ui/chat/assets/lmql-monaco.js` & `lmql-0.7b2/src/lmql/ui/chat/assets/lmql-monaco.js`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/chat/assets/lmql.svg` & `lmql-0.7b2/src/lmql/ui/chat/assets/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/chat/assets/send.svg` & `lmql-0.7b2/src/lmql/ui/chat/assets/send.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/chat/assets/studio.css` & `lmql-0.7b2/src/lmql/ui/chat/assets/studio.css`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/chat/assets/studio.html` & `lmql-0.7b2/src/lmql/ui/chat/assets/studio.html`

 * *Files 0% similar despite different names*

```diff
@@ -147,14 +147,15 @@
                     // escape all << and >>
                     prompt = prompt.replace(/<</g, '&lt;&lt;');
                     prompt = prompt.replace(/>>/g, '&gt;&gt;');
                     
                     document.getElementById("raw-prompt").innerHTML = prompt;
 
                     let value = object.variables["ANSWER"].trim();
+                    
                     // escape all << and >>
                     value = value.replace(/<</g, '&lt;&lt;');
                     value = value.replace(/>>/g, '&gt;&gt;');
 
                     addResponse(value, 'assistant', "response-" + id);
                 } else if (payload.type == "error") {
                     addError(payload.message);
```

### Comparing `lmql-0.7b1/src/lmql/ui/live/live.js` & `lmql-0.7b2/src/lmql/ui/live/live.js`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/live/live.py` & `lmql-0.7b2/src/lmql/ui/live/live.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/live/livelib.py` & `lmql-0.7b2/src/lmql/ui/live/livelib.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/live/yarn.lock` & `lmql-0.7b2/src/lmql/ui/live/yarn.lock`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/README.md` & `lmql-0.7b2/src/lmql/ui/playground/README.md`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/package.json` & `lmql-0.7b2/src/lmql/ui/playground/package.json`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/public/favicon.ico` & `lmql-0.7b2/src/lmql/ui/playground/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/public/index.html` & `lmql-0.7b2/src/lmql/ui/playground/public/index.html`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/public/lmql.svg` & `lmql-0.7b2/src/lmql/ui/playground/public/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/public/precomputed/calc.json` & `lmql-0.7b2/src/lmql/ui/playground/public/precomputed/calc.json`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/public/precomputed/chat.json` & `lmql-0.7b2/src/lmql/ui/playground/public/precomputed/chat.json`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/public/precomputed/cot.json` & `lmql-0.7b2/src/lmql/ui/playground/public/precomputed/cot.json`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/public/precomputed/date-regex.json` & `lmql-0.7b2/src/lmql/ui/playground/public/precomputed/date-regex.json`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/public/precomputed/distribution.json` & `lmql-0.7b2/src/lmql/ui/playground/public/precomputed/distribution.json`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/public/precomputed/hello.json` & `lmql-0.7b2/src/lmql/ui/playground/public/precomputed/hello.json`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/public/precomputed/joke.json` & `lmql-0.7b2/src/lmql/ui/playground/public/precomputed/joke.json`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/public/precomputed/json-robust.json` & `lmql-0.7b2/src/lmql/ui/playground/public/precomputed/json-robust.json`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/public/precomputed/json-template.json` & `lmql-0.7b2/src/lmql/ui/playground/public/precomputed/json-template.json`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/public/precomputed/kv.json` & `lmql-0.7b2/src/lmql/ui/playground/public/precomputed/kv.json`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/public/precomputed/list.json` & `lmql-0.7b2/src/lmql/ui/playground/public/precomputed/list.json`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/public/precomputed/meta.json` & `lmql-0.7b2/src/lmql/ui/playground/public/precomputed/meta.json`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/public/precomputed/translation.json` & `lmql-0.7b2/src/lmql/ui/playground/public/precomputed/translation.json`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/public/precomputed/wiki.json` & `lmql-0.7b2/src/lmql/ui/playground/public/precomputed/wiki.json`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/public/snippets/dynamic-cfg.json` & `lmql-0.7b2/src/lmql/ui/playground/public/snippets/dynamic-cfg.json`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/public/snippets/json-parsing.json` & `lmql-0.7b2/src/lmql/ui/playground/public/snippets/json-parsing.json`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/src/App.jsx` & `lmql-0.7b2/src/lmql/ui/playground/src/App.jsx`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import styled from 'styled-components';
 import Editor from "@monaco-editor/react";
 import React, { useEffect, useRef, useState } from "react";
 import { registerLmqlLanguage } from "./editor/lmql-monaco-language";
 import { BsSquare, BsFillExclamationSquareFill, BsBoxArrowUpRight, BsArrowRightCircle, BsFillCameraFill, BsCheckSquare, BsSendFill, 
   BsFileArrowDownFill, BsKeyFill, BsTerminal, BsFileCode, BsGithub, BsCardList, BsFullscreen, BsXCircle, BsFillChatLeftTextFill, 
-  BsGear, BsGridFill, BsPlus } from 'react-icons/bs';
+  BsGear, BsGridFill, BsPlus, BsBook } from 'react-icons/bs';
 import { DecoderGraph } from './DecoderGraph';
 import { BUILD_INFO } from './build_info';
 import exploreIcon from "./explore.svg"
 import { ExploreState, Explore, PromptPopup, Dialog } from './Explore'
 import { CodeScreenshot } from "./CodeScreenshot";
 import { errorState, persistedState, trackingState, displayState} from "./State"
 import { configuration, LMQLProcess, isLocalMode} from './Configuration';
@@ -2871,14 +2871,17 @@
               <BsKeyFill/> OpenAI Credentials
               </li>}
               {configuration.DEV_MODE && <li onClick={() => this.onExportState()}><BsFileArrowDownFill/> Export State</li>}
               {configuration.DEV_MODE && <li onClick={() => this.onCodeScreenshot()}><BsFillCameraFill/> Code Screenshot</li>}
               <li>
                 <a href="https://github.com/eth-sri/lmql" disabled target="_blank" rel="noreferrer"><BsGithub/>LMQL on Github</a>
               </li>
+              <li>
+                <a href="https://docs.lmql.ai" disabled target="_blank" rel="noreferrer"><BsBook/>Documentation</a>
+              </li>
               <span>
                 LMQL {this.state.buildInfo.commit} 
                 {(configuration.BROWSER_MODE && !isLocalMode()) && <> In-Browser</>}
                 {isLocalMode() && <> Self-Hosted</>}
                 {this.state.buildInfo.date != "-" ? <>
                   <br/>
                   Build on {this.state.buildInfo.date}
```

### Comparing `lmql-0.7b1/src/lmql/ui/playground/src/CodeScreenshot.jsx` & `lmql-0.7b2/src/lmql/ui/playground/src/CodeScreenshot.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/src/Configuration.js` & `lmql-0.7b2/src/lmql/ui/playground/src/Configuration.js`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/src/DataListView.js` & `lmql-0.7b2/src/lmql/ui/playground/src/DataListView.js`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/src/DecoderGraph.js` & `lmql-0.7b2/src/lmql/ui/playground/src/DecoderGraph.js`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/src/Explore.jsx` & `lmql-0.7b2/src/lmql/ui/playground/src/Explore.jsx`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import React, { useEffect, useState } from "react";
 import styled from "styled-components";
 import {queries} from "./queries";
 import { displayState, persistedState, trackingState } from "./State";
 import {configuration} from "./Configuration"
 
+import { BUILD_INFO } from './build_info';
+import { isLocalMode} from './Configuration';
+
 export const PromptPopup = styled.div`
   position: absolute;
   top: 0;
   left: 0;
   width: 100vw;
   height: 100vh;
   background-color: #000000c2;
@@ -82,56 +85,61 @@
     left: 2pt;
   }
 `
 
 const ExploreDialog = styled(Dialog)`
   width: 800pt;
   height: 700pt;
-  max-height: 100vh;
-  max-width: 100vh;
+  max-height: calc(100vh - 40pt);
+  max-width: 100vw;
   overflow-y: auto;
 
   /* invisible scroll bar */
   ::-webkit-scrollbar {
     width: 0px;
     background: transparent;
   }
 
   position: relative;
   padding: 0pt;
   
 
-  @media (max-width: 550pt) {
+  @media (max-width: 800pt) {
+    border-radius: 0 !important;
+    width: 100vw !important;
+    height: 100vh !important;
+    max-height: 100vh !important;
+    max-width: 100vw !important;
+  }
+  
+
+  @media (max-width: 450pt) {
     width: calc(100vw - 20pt);
     height: calc(100vh - 20pt);
     max-height: 100vh;
     max-width: 100vw;
     overflow-y: auto;
     position: relative;
     padding: 10pt;
     padding-bottom: 80pt;
     padding-left: 0;
     margin: 0;
-    border-radius: 0;
 
     div.tile {
       display: block !important;
+      height: 40pt;
       width: 100% !important;
-      border: 1pt solid transparent;
 
       &:hover {
         transform: none !important;
         border: 1pt solid #ababab;
       }
     }
   }
 
-  /* very light white to grey grdient */
-  background: linear-gradient(180deg, #ffffff 0%, #e4e2e2 100%);
-
   >div {
     padding: 5pt 20pt;
     position: relative;
   }
 
   >div .sidenote a {
     padding-left: 2pt;
@@ -141,15 +149,17 @@
     position: absolute;
     top: 15pt;
     right: 15pt;
     font-size: 8pt;
   }
 
   div.highlight {
-    background-color: #dedef8;
+    background-color: #f5f5f5;
+    margin: 5pt;
+    border-radius: 4pt;
   }
 
   >div>div {
     display: flex;
     flex-direction: row;
     flex-wrap: wrap;
   }
@@ -157,14 +167,16 @@
   p {
     text-align: justify;
   }
 
   h1 {
     margin: 0;
     padding: 20pt;
+    font-weight: bold;
+    padding-bottom: 10pt;
   }
 
   h1 img {
     width: 20pt;
     height: 20pt;
     margin-right: 8pt;
     position: relative;
@@ -176,15 +188,15 @@
   }
 
   h3 {
     font-size: 12pt;
     color: #373737;
     margin: 0;
     z-index: 999;
-    font-weight: 500;
+    font-weight: 700;
   }
 
   .close {
     position: absolute;
     top: 10pt;
     right: 10pt;
     width: 30pt;
@@ -195,36 +207,37 @@
     cursor: pointer;
   }
 `
 
 const Tile = styled.div.attrs({
   className: "tile"
 })`
-  background-color: #f5f5f5;
+  background-color: white;
   border-radius: 4pt;
   padding: 10pt;
   margin: 10pt;
   margin-left: 0pt;
   margin-top: 0pt;
   cursor: pointer;
-  transition: 0.1s;
+  transition: 0.05s ease-in-out transform;
   height: 80pt;
   width: 100pt;
-  border: 0.5pt solid #ababab;
+  border: 1pt solid #d4d4d4;
   opacity: 0.9;
   position: relative;
   display: flex;
   flex-direction: column;
   
   align-items: flex-start;
   justify-content: flex-start;
 
   :hover {
     transform: scale(1.05);
     opacity: 1.0;
+    border: 1pt solid #9b9a9a;
   }
 
   h3 {
     color: #212121;
   }
 
   code {
@@ -248,15 +261,15 @@
     background-color: #e2e0e1;
     padding: 2pt;
     z-index: 9;
   }
 `
 
 export const ExploreState = {
-    visible: false,
+    visible: window.location.hash === "#explore",
     setVisibility: (s) => {
         ExploreState.visible = s;
         ExploreState.listeners.forEach((l) => l(s));
     },
     listeners: []
 }
 
@@ -307,69 +320,14 @@
     left: 0;
     right: 0;
     height: 20pt;
     /* background: linear-gradient(180deg, transparent 0%, #f5f5f561 100%); */
   }
 `
 
-const TypingContainer = styled.span`
-  .cursor {
-    animation: blink 2s linear infinite;
-    transform: scale(2.2);
-    transform-origin: top middle;
-    font-size: 25pt;
-    height: 15pt;
-    background-color: #313131;
-    width: 1pt;
-    position: relative;
-    left: 6pt;
-    content: " ";
-    overflow: hidden;
-    display: inline-block;
-  }
-
-  @keyframes blink {
-    0% {
-      opacity: 0;
-    }
-    50% {
-      opacity: 1;
-    }
-    100% {
-      opacity: 0;
-    }
-  }
-`
-
-
-function TypedText(props) {
-  const text = props.text;
-  const speed = 50;
-  let [index, setIndex] = useState(window.textWasTyped ? text.length : 0);
-  let [isTyping, setIsTyping] = useState(!window.textWasTyped);
-
-  useEffect(() => {
-    if (!isTyping) return;
-    
-    if (index < text.length) {
-      setTimeout(() => {
-        setIndex(index + 1);
-      }, speed);
-    } else {
-      setIsTyping(false);
-      window.textWasTyped = true;
-    }
-  })
-
-  return <TypingContainer>
-    {text.substring(0, index)}
-    <span className="cursor"></span>
-  </TypingContainer>
-}
-
 function BasicHighlighted(props) {
   const s = props.code;
 
   const keywords = ["argmax", "where", "from", "and", "or", "not", "sample", "beam_search"];
   // split into words (also split on ()\t\n)
   const words = s.split(/(\s+|[()\t])/g);
   const result = words.map((w,i) => {
@@ -383,23 +341,68 @@
   </CodeContainer>
 }
 
 const Description = styled.p`
   font-size: 14pt;
   color: #696969;
   padding: 0pt 20pt;
+  font-weight: 500;
+  margin-top: 0pt;
+`
+
+const LinkBox = styled.div`
+  display: flex;
+  flex-direction: row;
+
+  a.button {
+    display: block;
+    border: 1pt solid #6b77ff;
+    padding: 5pt;
+    margin-top: 15pt;
+    margin-right: 5pt;
+    border-radius: 2pt;
+    color: #6b77ff;
+
+    font-size: 10pt;
+  }
+
+  a.button:first-child {
+    color: white;
+    background-color: #6b77ff;
+
+    &:hover {
+      background-color: #8e98ea;
+      text-decoration: none;
+    }
+  }
 `
 
 const CiteBox = styled.code`
   display: block;
-  background-color: #dbdbdb;
+  background-color: #f5f5f5;
   padding: 4pt;
   border-radius: 4pt;
 `
 
+const PoweredBy = styled.div`
+  font-size: 8pt;
+  color: #696969;
+  text-align: center;
+  margin: auto;
+
+  display: flex;
+  justify-content: center;
+  align-items: center;
+  padding: 10pt;
+
+  >div:nth-child(2) {
+    margin-left: 5pt;
+  }
+`
+
 let didLoadAnchor = false;
 
 const PreviewQueries = {
   queries: [],
   listeners: []
 }
 
@@ -479,54 +482,68 @@
       }
     }, [])
 
 
     if (!visible) return null;
 
     let description = <>
-    This playground allows you to explore LMQL's capabilities. To get started, choose one of the example queries below.
+    LMQL is a query language for large language models. Explore the examples below to get started.
+    <LinkBox>
+      <a className="button" target="_blank" rel="noreferrer" href="https://docs.lmql.ai">Documentation</a>
+      <a className="button" target="_blank" rel="noreferrer" href="https://lmql.ai">Overview</a>
+    </LinkBox>
     </>
 
     if (configuration.NEXT_MODE) {
       description = <>This is the preview channel of LMQL. It contains the latest features, but may be unstable. If you are looking for the stable version, please visit <a href="https://lmql.ai/playground">the stable Playground IDE</a>.</>
     }
 
     return <PromptPopup>
         <div className="click-handler" onClick={() => ExploreState.setVisibility(false)}/>
         <ExploreDialog>
           <h1 key="welcome">
             <img src="/lmql.svg" alt="LMQL Logo"/>  
-            <TypedText text="Welcome To LMQL" speed={20}/>
+            Welcome To LMQL
           </h1>
           <Description>{description}</Description>
           <span className="close" onClick={() => ExploreState.setVisibility(false)}>
             &times;
           </span>
           {exploreQueries.map(c => 
             <div className={c.highlight ? "highlight" : ""} key={c.category + "-container"}>
             <h2 key={c.category}>{c.category}</h2>
             {c.highlight && <span class="sidenote">
-              <a href="https://github.com/eth-sri/lmql/issues" target="_blank" rel="noreferrer"> Report Issues</a>
+              <a href="https://github.com/eth-sri/lmql/issues" target="_blank" rel="noreferrer" title="Please report any issue you find with Preview features to help us improve LMQL."> Report Issues</a>
             </span>}
             <div key={c.category + "-div"}>
             {c.queries.map((q,i) => <Tile key={c.category + "-" + i} onClick={() => onClickTile(q)}>
               {/* {q.state && <div className="badge">PRECOMPUTED</div>} */}
               <BasicHighlighted code={q.code}/>
               <h3>{q.name}</h3>
               <p>{q.description}</p>
             </Tile>)}
             </div>
             </div>
           )}
           {!configuration.NEXT_MODE && <>
           <div>
-          <h2 key="read-paper">Read the Paper</h2>
+          <h2 key="read-paper">Read More</h2>
           <CiteBox key="cite">
           Beurer-Kellner, Luca, Marc Fischer, and Martin Vechev. "Prompting Is Programming: A Query Language For Large Language Models." 
           <a target="_blank" rel="noreferrer" href="https://arxiv.org/pdf/2212.06094">arXiv preprint arXiv:2212.06094</a> (2022).
           </CiteBox>
           <br/>
+          <PoweredBy>
+            <div>LMQL {BUILD_INFO.info().commit}</div>
+            <div>
+            {(configuration.BROWSER_MODE && !isLocalMode()) && <span> In-Browser, Made with ❤️ + <a href="https://pyodide.org" target="_blank" rel="noreferrer">Pyodide</a> + <a href="https://webassembly.org/" target="_blank" rel="noreferrer">WebAssembly</a></span>}
+              {BUILD_INFO.info().date != "-" ? <>
+                <br/>
+                Build on {BUILD_INFO.info().date}
+              </> : null}
+            </div>
+          </PoweredBy>
           </div>
           </>}
         </ExploreDialog>
     </PromptPopup>
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lmql-0.7b1/src/lmql/ui/playground/src/SharedState.js` & `lmql-0.7b2/src/lmql/ui/playground/src/SharedState.js`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/src/State.js` & `lmql-0.7b2/src/lmql/ui/playground/src/State.js`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/src/ValidationGraph.jsx` & `lmql-0.7b2/src/lmql/ui/playground/src/ValidationGraph.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/src/browser_process.js` & `lmql-0.7b2/src/lmql/ui/playground/src/browser_process.js`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/src/build_info.js` & `lmql-0.7b2/src/lmql/ui/playground/src/build_info.js`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/src/editor/lmql-monaco-language.js` & `lmql-0.7b2/src/lmql/ui/playground/src/editor/lmql-monaco-language.js`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/src/editor/theme.json` & `lmql-0.7b2/src/lmql/ui/playground/src/editor/theme.json`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/src/explore.svg` & `lmql-0.7b2/src/lmql/ui/playground/src/explore.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/src/graph-layout.css` & `lmql-0.7b2/src/lmql/ui/playground/src/graph-layout.css`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/src/index.css` & `lmql-0.7b2/src/lmql/ui/playground/src/index.css`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 body {
   margin: 0;
-  font-family: 'Open Sans', sans-serif;
+  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto,
+    'Helvetica Neue', Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji',
+    'Segoe UI Symbol';
   -webkit-font-smoothing: antialiased;
   -moz-osx-font-smoothing: grayscale;
   padding: 0pt;
   overflow: hidden;
   display: flex;
   flex-direction: column;
   align-items: stretch;
@@ -91,14 +93,23 @@
 
 @media (max-width: 40em) {
   .hidden-on-small {
     display: none;
   }
 }
 
+a {
+  color: #6b77ff;
+  text-decoration: none;
+}
+
+a:hover {
+  text-decoration: underline;
+}
+
 /* 
 #root {
   margin: 100pt;
 }
 
 #sidepanel {
   background-color: white;
```

### Comparing `lmql-0.7b1/src/lmql/ui/playground/src/logo.svg` & `lmql-0.7b2/src/lmql/ui/playground/src/logo.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/src/queries.js` & `lmql-0.7b2/src/lmql/ui/playground/src/queries.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -122,15 +122,15 @@
                 name: "🔤 Regex Constraints",
                 description: "Specify constraints using regex.",
                 code: `"It's the last day of June so today is [RESPONSE]" where REGEX(RESPONSE, r"[0-9]{2}/[0-9]{2}")`,
                 state: 'precomputed/date-regex.json'
             }, {
                 // hello world
                 name: "❤️ Sentiment Constraints",
-                description: "Affect sentiment with in-context prompting.",
+                description: "Affect sentiment with in-context instructions.",
                 code: `@lmql.query(cache="mood.tokens", model="chatgpt")
 async def mood_description(m: str):
     '''lmql
     print("Generating mood for", m)
     """Provide a one sentence instruction that prompts a model to write text that 
     is written in a {m} tone, addressing some previously provided question.\\n"""
     "[SUMMARY]\\n"
@@ -159,15 +159,15 @@
     mood(RESPONSE, "loving like a partner")
           
 `,
                 state: ''
             }, {
                 // hello world
                 name: "📝 Write A Poem",
-                description: "Insert dynamic instructions with incontext.",
+                description: "Insert dynamic instructions during generation.",
                 code: `@lmql.query
 async def rhyme():
     '''
     """
     Above is the beginning of the poem. Generate the next verse that rhymes with the last line and has the same number of syllables.
     [VERSE]
     """ where stops_before(VERSE, "\\n")
```

### Comparing `lmql-0.7b1/src/lmql/ui/playground/src/remote_process.js` & `lmql-0.7b2/src/lmql/ui/playground/src/remote_process.js`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/src/screenshot.css` & `lmql-0.7b2/src/lmql/ui/playground/src/screenshot.css`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/src/spinner.svg` & `lmql-0.7b2/src/lmql/ui/playground/src/spinner.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/src/tagged-model-result.js` & `lmql-0.7b2/src/lmql/ui/playground/src/tagged-model-result.js`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/playground/yarn.lock` & `lmql-0.7b2/src/lmql/ui/playground/yarn.lock`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/vscode/.vscode/launch.json` & `lmql-0.7b2/src/lmql/ui/vscode/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/vscode/LICENSE` & `lmql-0.7b2/src/lmql/ui/vscode/LICENSE`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/vscode/language-configuration.json` & `lmql-0.7b2/src/lmql/ui/vscode/language-configuration.json`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/vscode/lmql-vscode.png` & `lmql-0.7b2/src/lmql/ui/vscode/lmql-vscode.png`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/vscode/package.json` & `lmql-0.7b2/src/lmql/ui/vscode/package.json`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/vscode/syntaxes/lmql.qstring.json` & `lmql-0.7b2/src/lmql/ui/vscode/syntaxes/lmql.qstring.json`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json` & `lmql-0.7b2/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/ui/vscode/syntaxes/pylmql.json` & `lmql-0.7b2/src/lmql/ui/vscode/syntaxes/pylmql.json`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/utils/docstring_parser.py` & `lmql-0.7b2/src/lmql/utils/docstring_parser.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/utils/graph.py` & `lmql-0.7b2/src/lmql/utils/graph.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql/utils/nputil.py` & `lmql-0.7b2/src/lmql/utils/nputil.py`

 * *Files identical despite different names*

### Comparing `lmql-0.7b1/src/lmql.egg-info/PKG-INFO` & `lmql-0.7b2/src/lmql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmql
-Version: 0.7b1
+Version: 0.7b2
 Summary: A query language for language models.
 Home-page: https://lmql.ai
 Author: Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 Author-email: hello@lmql.ai
 Project-URL: Docs, https://docs.lmql.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lmql Version: 0.7b1 Summary: A query language for
+Metadata-Version: 2.1 Name: lmql Version: 0.7b2 Summary: A query language for
 language models. Home-page: https://lmql.ai Author: Luca Beurer-Kellner, Marc
 Fischer, Martin Vechev Author-email: hello@lmql.ai Project-URL: Docs, https://
 docs.lmql.ai Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.10 Description-Content-
 Type: text/markdown Provides-Extra: hf License-File: LICENSE
                                     [Logo]
                                 **** LMQL ****
```

### Comparing `lmql-0.7b1/src/lmql.egg-info/SOURCES.txt` & `lmql-0.7b2/src/lmql.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .gitignore
+.readthedocs.yaml
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 yarn.lock
@@ -19,33 +20,37 @@
 docs/source/docker-setup.md
 docs/source/index.rst
 docs/source/installation.md
 docs/source/lmql.svg
 docs/source/logo.png
 docs/source/quickstart.md
 docs/source/_ext/lmql_snippets.py
+docs/source/_static/logo-light.svg
+docs/source/_static/logo.png
+docs/source/_static/logo.svg
 docs/source/_static/css/lmql-docs.css
 docs/source/_static/images/lmql.svg
 docs/source/_static/js/lmql-playground.js
 docs/source/_templates/layout.html
 docs/source/blog/release-0.0.5.md
 docs/source/blog/release-0.0.6.1.md
 docs/source/blog/release-0.0.6.3.md
 docs/source/blog/release-0.0.6.4.md
 docs/source/blog/release-0.0.6.5.md
 docs/source/blog/release-0.0.6.6.md
 docs/source/blog/release-0.0.6.md
 docs/source/images/inference.svg
 docs/source/language/azure.md
 docs/source/language/constraints.md
+docs/source/language/custom-constraints.md
 docs/source/language/decoders.md
 docs/source/language/functions.md
 docs/source/language/hf.md
 docs/source/language/llama.cpp.md
-docs/source/language/models.md
+docs/source/language/models.rst
 docs/source/language/openai.md
 docs/source/language/overview.md
 docs/source/language/scripted_prompts.md
 docs/source/pending/release-next.md
 docs/source/python/.gitignore
 docs/source/python/comparison.md
 docs/source/python/langchain.ipynb
@@ -88,22 +93,24 @@
 src/lmql/language/validator.py
 src/lmql/lib/__init__.py
 src/lmql/lib/actions.py
 src/lmql/lib/algebra222.csv
 src/lmql/lib/data.py
 src/lmql/lib/types.py
 src/lmql/lib/value.py
+src/lmql/lib/prompts/__init__.py
 src/lmql/lib/prompts/inline_code copy.py
 src/lmql/lib/prompts/inline_code.py
 src/lmql/lib/prompts/inline_use.py
 src/lmql/lib/prompts/inline_use_kevin.py
 src/lmql/lib/prompts/wiki_prompt.py
 src/lmql/models/__init__.py
 src/lmql/models/model.py
 src/lmql/models/lmtp/README.md
+src/lmql/models/lmtp/__init__.py
 src/lmql/models/lmtp/errors.py
 src/lmql/models/lmtp/lmtp_async.py
 src/lmql/models/lmtp/lmtp_client.py
 src/lmql/models/lmtp/lmtp_dcmodel.py
 src/lmql/models/lmtp/lmtp_inference_server.py
 src/lmql/models/lmtp/lmtp_multiprocessing.py
 src/lmql/models/lmtp/lmtp_programmatic_serve_example.py
@@ -157,14 +164,15 @@
 src/lmql/runtime/dclib/dclib_model.py
 src/lmql/runtime/dclib/dclib_rewrite.py
 src/lmql/runtime/dclib/dclib_seq.py
 src/lmql/runtime/dclib/decoders.py
 src/lmql/runtime/postprocessing/__init__.py
 src/lmql/runtime/postprocessing/conditional_prob.py
 src/lmql/runtime/postprocessing/group_by.py
+src/lmql/runtime/tokenizers/__init__.py
 src/lmql/runtime/tokenizers/hf_tokenizer.py
 src/lmql/runtime/tokenizers/pure_python_tokenizer.py
 src/lmql/runtime/tokenizers/tiktoken_tokenizer.py
 src/lmql/tests/README.md
 src/lmql/tests/all.py
 src/lmql/tests/expr_test_utils.py
 src/lmql/tests/fin_and.py
```

### Comparing `lmql-0.7b1/src/lmql.svg` & `lmql-0.7b2/src/lmql.svg`

 * *Files identical despite different names*

