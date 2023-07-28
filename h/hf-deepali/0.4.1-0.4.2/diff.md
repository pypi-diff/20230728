# Comparing `tmp/hf-deepali-0.4.1.tar.gz` & `tmp/hf-deepali-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hf-deepali-0.4.1.tar", last modified: Thu Jul 20 22:36:42 2023, max compression
+gzip compressed data, was "hf-deepali-0.4.2.tar", last modified: Fri Jul 28 13:34:00 2023, max compression
```

## Comparing `hf-deepali-0.4.1.tar` & `hf-deepali-0.4.2.tar`

### file list

```diff
@@ -1,259 +1,261 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.336184 hf-deepali-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.296182 hf-deepali-0.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.300182 hf-deepali-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.300182 hf-deepali-0.4.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-07-20 22:36:42.336184 hf-deepali-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/TODO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.304183 hf-deepali-0.4.1/conda/
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/conda/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/conda/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   550833 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/conda/environment.conda-lock.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/conda/environment.devenv.yml
--rw-r--r--   0 runner    (1001) docker     (123)    53576 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/conda/environment.linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)    15553 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/conda/environment.linux-64.yml
--rw-r--r--   0 runner    (1001) docker     (123)    45592 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/conda/environment.osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)    13443 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/conda/environment.osx-64.yml
--rw-r--r--   0 runner    (1001) docker     (123)    48151 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/conda/environment.win-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)    14217 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/conda/environment.win-64.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.304183 hf-deepali-0.4.1/docker/
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docker/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (123)     1699 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docker/build
--rwxr-xr-x   0 runner    (1001) docker     (123)     7011 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docker/run
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.304183 hf-deepali-0.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/_citations.bib
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.304183 hf-deepali-0.4.1/docs/_images/
--rw-r--r--   0 runner    (1001) docker     (123)   390208 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/_images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/_toc.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.304183 hf-deepali-0.4.1/docs/basics/
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/basics/example-page.md
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/basics/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.296182 hf-deepali-0.4.1/docs/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.308183 hf-deepali-0.4.1/docs/reference/core/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/core/domain.md
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/core/flow.md
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/core/image.md
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/core/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/core/kernels.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.308183 hf-deepali-0.4.1/docs/reference/data/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/data/dataset.md
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/data/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/data/sampler.md
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/data/tensor.md
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/data/transforms.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.308183 hf-deepali-0.4.1/docs/reference/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/losses/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.308183 hf-deepali-0.4.1/docs/reference/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/modules/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.308183 hf-deepali-0.4.1/docs/reference/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/networks/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.308183 hf-deepali-0.4.1/docs/reference/spatial/
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/spatial/common.md
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/spatial/composite.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/spatial/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/spatial/transformer.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.308183 hf-deepali-0.4.1/docs/reference/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/utils/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.308183 hf-deepali-0.4.1/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/tutorials/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/tutorials/example-myst-notebook.md
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/tutorials/example-notebook.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    45126 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/tutorials/pairwise-registration-intro.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.308183 hf-deepali-0.4.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.312183 hf-deepali-0.4.1/examples/ffd/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/ffd/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/ffd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/ffd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/ffd/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/ffd/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/ffd/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/ffd/optim.py
--rw-r--r--   0 runner    (1001) docker     (123)    32029 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/ffd/pairwise.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/ffd/params.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/ffd/register.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.312183 hf-deepali-0.4.1/examples/istn/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/istn/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/istn/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.312183 hf-deepali-0.4.1/examples/istn/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/istn/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/istn/models/itn.py
--rw-r--r--   0 runner    (1001) docker     (123)    23150 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/istn/models/stn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/istn/params.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/istn/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    27820 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/istn/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/pyrightconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 22:36:42.336184 hf-deepali-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.296182 hf-deepali-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.296182 hf-deepali-0.4.1/src/deepali/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.316183 hf-deepali-0.4.1/src/deepali/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19990 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/_kornia.py
--rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/affine.py
--rw-r--r--   0 runner    (1001) docker     (123)    17034 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    23034 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/bspline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24560 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/cube.py
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/environ.py
--rw-r--r--   0 runner    (1001) docker     (123)    20232 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    74082 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    78487 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)    19580 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    16779 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/nnutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/pathlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/pointset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/psutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/tempfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.320183 hf-deepali-0.4.1/src/deepali/data/
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/data/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    19033 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    24776 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/data/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    62290 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/data/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/data/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/data/prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/data/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/data/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/data/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.320183 hf-deepali-0.4.1/src/deepali/data/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/data/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16685 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/data/transforms/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/data/transforms/item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.320183 hf-deepali-0.4.1/src/deepali/losses/
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/losses/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/losses/bspline.py
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/losses/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    66499 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/losses/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/losses/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/losses/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/losses/pointset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.320183 hf-deepali-0.4.1/src/deepali/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/modules/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/modules/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/modules/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/modules/lambd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/modules/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/modules/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    14656 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/modules/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/modules/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.324183 hf-deepali-0.4.1/src/deepali/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.324183 hf-deepali-0.4.1/src/deepali/networks/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15316 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/blocks/residual.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/blocks/skip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.324183 hf-deepali-0.4.1/src/deepali/networks/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/layers/acti.py
--rw-r--r--   0 runner    (1001) docker     (123)    15589 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/layers/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/layers/join.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/layers/lambd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/layers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/layers/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/layers/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    18771 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/layers/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)    19788 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    42916 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.324183 hf-deepali-0.4.1/src/deepali/spatial/
--rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/spatial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22608 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/spatial/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/spatial/bspline.py
--rw-r--r--   0 runner    (1001) docker     (123)    14042 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/spatial/composite.py
--rw-r--r--   0 runner    (1001) docker     (123)    16560 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/spatial/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/spatial/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    29233 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/spatial/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    12619 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/spatial/nonrigid.py
--rw-r--r--   0 runner    (1001) docker     (123)    17031 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/spatial/parametric.py
--rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/spatial/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.328184 hf-deepali-0.4.1/src/deepali/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.328184 hf-deepali-0.4.1/src/deepali/utils/aws/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.328184 hf-deepali-0.4.1/src/deepali/utils/aws/s3/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/aws/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21866 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/aws/s3/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/aws/s3/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/aws/s3/object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.328184 hf-deepali-0.4.1/src/deepali/utils/ignite/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/ignite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13571 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/ignite/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.328184 hf-deepali-0.4.1/src/deepali/utils/ignite/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/ignite/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/ignite/metrics/average_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/ignite/metrics/binary_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/ignite/metrics/multilabel_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/ignite/output_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/ignite/score_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.328184 hf-deepali-0.4.1/src/deepali/utils/imageio/
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/imageio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/imageio/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/imageio/nifti.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/imageio/sitk.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/ipython.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.332184 hf-deepali-0.4.1/src/deepali/utils/simpleitk/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/simpleitk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13664 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/simpleitk/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/simpleitk/imageio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/simpleitk/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/simpleitk/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/simpleitk/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.332184 hf-deepali-0.4.1/src/deepali/utils/vtk/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/vtk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/vtk/idlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/vtk/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/vtk/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/vtk/polydataio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/vtk/simpleitk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.332184 hf-deepali-0.4.1/src/hf_deepali.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-07-20 22:36:42.000000 hf-deepali-0.4.1/src/hf_deepali.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-07-20 22:36:42.000000 hf-deepali-0.4.1/src/hf_deepali.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 22:36:42.000000 hf-deepali-0.4.1/src/hf_deepali.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-20 22:36:42.000000 hf-deepali-0.4.1/src/hf_deepali.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 22:36:42.000000 hf-deepali-0.4.1/src/hf_deepali.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.332184 hf-deepali-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/tests/_test_core_bspline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/tests/test_core_bspline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/tests/test_core_cube.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/tests/test_core_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/tests/test_core_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/tests/test_core_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/tests/test_core_tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/tests/test_data_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    23869 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/tests/test_data_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/tests/test_network_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/tests/test_network_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/tests/test_network_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/tests/test_network_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/tests/test_utils_imageio_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.897742 hf-deepali-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.853740 hf-deepali-0.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.857740 hf-deepali-0.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.861740 hf-deepali-0.4.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-07-28 13:34:00.897742 hf-deepali-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10421 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/TODO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.861740 hf-deepali-0.4.2/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/conda/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/conda/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   550833 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/conda/environment.conda-lock.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/conda/environment.devenv.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    53576 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/conda/environment.linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    15553 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/conda/environment.linux-64.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    45592 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/conda/environment.osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    13443 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/conda/environment.osx-64.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    48151 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/conda/environment.win-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    14217 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/conda/environment.win-64.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.861740 hf-deepali-0.4.2/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docker/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1699 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docker/build
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7011 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docker/run
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.865740 hf-deepali-0.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/_citations.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.865740 hf-deepali-0.4.2/docs/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)   390208 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/_images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/_toc.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.865740 hf-deepali-0.4.2/docs/basics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/basics/example-page.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/basics/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.853740 hf-deepali-0.4.2/docs/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.865740 hf-deepali-0.4.2/docs/reference/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/core/domain.md
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/core/flow.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/core/image.md
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/core/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/core/kernels.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.865740 hf-deepali-0.4.2/docs/reference/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/data/dataset.md
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/data/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/data/sampler.md
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/data/tensor.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/data/transforms.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.865740 hf-deepali-0.4.2/docs/reference/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/losses/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.865740 hf-deepali-0.4.2/docs/reference/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/modules/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.865740 hf-deepali-0.4.2/docs/reference/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/networks/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.869741 hf-deepali-0.4.2/docs/reference/spatial/
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/spatial/common.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/spatial/composite.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/spatial/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/spatial/transformer.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.869741 hf-deepali-0.4.2/docs/reference/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/utils/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.869741 hf-deepali-0.4.2/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/tutorials/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/tutorials/example-myst-notebook.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/tutorials/example-notebook.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    45126 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/tutorials/pairwise-registration-intro.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.869741 hf-deepali-0.4.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.869741 hf-deepali-0.4.2/examples/ffd/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/ffd/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/ffd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/ffd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/ffd/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/ffd/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/ffd/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/ffd/optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32029 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/ffd/pairwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/ffd/params.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/ffd/register.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.873741 hf-deepali-0.4.2/examples/istn/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/istn/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/istn/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.873741 hf-deepali-0.4.2/examples/istn/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/istn/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/istn/models/itn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23150 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/istn/models/stn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/istn/params.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/istn/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    27820 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/istn/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 13:34:00.897742 hf-deepali-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.857740 hf-deepali-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.857740 hf-deepali-0.4.2/src/deepali/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.877741 hf-deepali-0.4.2/src/deepali/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19990 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/_kornia.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17034 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23034 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/bspline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24560 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20207 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74082 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79771 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19580 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16779 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/nnutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/pointset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/psutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/tempfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.881741 hf-deepali-0.4.2/src/deepali/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/data/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19033 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24776 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/data/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62290 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/data/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/data/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/data/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/data/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/data/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/data/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.881741 hf-deepali-0.4.2/src/deepali/data/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/data/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16685 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/data/transforms/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/data/transforms/item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.881741 hf-deepali-0.4.2/src/deepali/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/losses/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/losses/bspline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/losses/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68167 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/losses/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/losses/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/losses/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/losses/pointset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.881741 hf-deepali-0.4.2/src/deepali/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/modules/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/modules/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/modules/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/modules/lambd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/modules/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/modules/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14656 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/modules/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/modules/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.885742 hf-deepali-0.4.2/src/deepali/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.885742 hf-deepali-0.4.2/src/deepali/networks/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15316 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/blocks/residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/blocks/skip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.885742 hf-deepali-0.4.2/src/deepali/networks/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/layers/acti.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15589 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/layers/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/layers/join.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/layers/lambd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/layers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/layers/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/layers/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18771 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/layers/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19788 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42916 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.889742 hf-deepali-0.4.2/src/deepali/spatial/
+-rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/spatial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22608 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/spatial/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/spatial/bspline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14042 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/spatial/composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16560 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/spatial/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/spatial/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29233 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/spatial/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12619 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/spatial/nonrigid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17031 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/spatial/parametric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/spatial/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.889742 hf-deepali-0.4.2/src/deepali/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.889742 hf-deepali-0.4.2/src/deepali/utils/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.889742 hf-deepali-0.4.2/src/deepali/utils/aws/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/aws/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21866 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/aws/s3/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/aws/s3/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/aws/s3/object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.889742 hf-deepali-0.4.2/src/deepali/utils/ignite/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/ignite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13571 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/ignite/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.893742 hf-deepali-0.4.2/src/deepali/utils/ignite/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/ignite/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/ignite/metrics/average_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/ignite/metrics/binary_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/ignite/metrics/multilabel_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/ignite/output_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/ignite/score_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.893742 hf-deepali-0.4.2/src/deepali/utils/imageio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/imageio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/imageio/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/imageio/nifti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/imageio/sitk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/ipython.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.893742 hf-deepali-0.4.2/src/deepali/utils/simpleitk/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/simpleitk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13664 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/simpleitk/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/simpleitk/imageio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/simpleitk/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/simpleitk/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/simpleitk/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.893742 hf-deepali-0.4.2/src/deepali/utils/vtk/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/vtk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/vtk/idlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/vtk/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/vtk/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/vtk/polydataio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/vtk/simpleitk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.893742 hf-deepali-0.4.2/src/hf_deepali.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-07-28 13:34:00.000000 hf-deepali-0.4.2/src/hf_deepali.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-07-28 13:34:00.000000 hf-deepali-0.4.2/src/hf_deepali.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:34:00.000000 hf-deepali-0.4.2/src/hf_deepali.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-28 13:34:00.000000 hf-deepali-0.4.2/src/hf_deepali.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-28 13:34:00.000000 hf-deepali-0.4.2/src/hf_deepali.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.897742 hf-deepali-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/_test_core_bspline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/test_core_bspline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/test_core_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/test_core_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/test_core_image_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/test_core_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/test_core_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/test_core_tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/test_data_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23869 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/test_data_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/test_network_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/test_network_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/test_network_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/test_network_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/test_spatial_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/test_utils_imageio_meta.py
```

### Comparing `hf-deepali-0.4.1/.github/workflows/docs.yml` & `hf-deepali-0.4.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/.github/workflows/release.yml` & `hf-deepali-0.4.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/.github/workflows/tests.yml` & `hf-deepali-0.4.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/.gitignore` & `hf-deepali-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/.vscode/extensions.json` & `hf-deepali-0.4.2/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/.vscode/launch.json` & `hf-deepali-0.4.2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/.vscode/settings.json` & `hf-deepali-0.4.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/CITATION.cff` & `hf-deepali-0.4.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/CODE_OF_CONDUCT.md` & `hf-deepali-0.4.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/LICENSE` & `hf-deepali-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/PKG-INFO` & `hf-deepali-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hf-deepali
-Version: 0.4.1
+Version: 0.4.2
 Summary: Image, point set, and surface registration library for PyTorch.
 Maintainer-email: Andreas Schuh <andreas.schuh@imperial.ac.uk>
 License: Apache-2.0
 Project-URL: Homepage, https://biomedia.github.io/deepali
 Project-URL: Repository, https://github.com/BioMedIA/deepali.git
 Project-URL: Bug Tracker, https://github.com/BioMedIA/deepali/issues
 Keywords: medical-imaging,image-registration,spatial-transformer-networks
@@ -24,15 +24,15 @@
 Provides-Extra: utils
 Provides-Extra: tests
 License-File: LICENSE
 
 # deepali
 
 <!-- ![downloads](https://img.shields.io/pypi/dm/hf-deepali) -->
-![pypi](https://img.shields.io/pypi/v/hf-deepali)
+[![pypi](https://img.shields.io/pypi/v/hf-deepali)](https://pypi.org/project/hf-deepali/)
 ![python](https://img.shields.io/pypi/pyversions/hf-deepali)
 [![docs](https://github.com/BioMedIA/deepali/actions/workflows/docs.yml/badge.svg)](https://github.com/BioMedIA/deepali/actions/workflows/docs.yml)
 [![tests](https://github.com/BioMedIA/deepali/actions/workflows/tests.yml/badge.svg)](https://github.com/BioMedIA/deepali/actions/workflows/tests.yml)
 [![release](https://github.com/BioMedIA/deepali/actions/workflows/release.yml/badge.svg)](https://github.com/BioMedIA/deepali/actions/workflows/release.yml)
 [![doi](https://zenodo.org/badge/DOI/10.5281/zenodo.8170161.svg)](https://doi.org/10.5281/zenodo.8170161)
 
 An [open source](https://github.com/BioMedIA/deepali/tree/main/LICENSE) research library for image, point set, and surface registration in [PyTorch], which is developed and maintained by the [HeartFlow-Imperial College London] research lab at the [Biomedical Image Analysis Group].
```

### Comparing `hf-deepali-0.4.1/README.md` & `hf-deepali-0.4.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # deepali
 
 <!-- ![downloads](https://img.shields.io/pypi/dm/hf-deepali) -->
-![pypi](https://img.shields.io/pypi/v/hf-deepali)
+[![pypi](https://img.shields.io/pypi/v/hf-deepali)](https://pypi.org/project/hf-deepali/)
 ![python](https://img.shields.io/pypi/pyversions/hf-deepali)
 [![docs](https://github.com/BioMedIA/deepali/actions/workflows/docs.yml/badge.svg)](https://github.com/BioMedIA/deepali/actions/workflows/docs.yml)
 [![tests](https://github.com/BioMedIA/deepali/actions/workflows/tests.yml/badge.svg)](https://github.com/BioMedIA/deepali/actions/workflows/tests.yml)
 [![release](https://github.com/BioMedIA/deepali/actions/workflows/release.yml/badge.svg)](https://github.com/BioMedIA/deepali/actions/workflows/release.yml)
 [![doi](https://zenodo.org/badge/DOI/10.5281/zenodo.8170161.svg)](https://doi.org/10.5281/zenodo.8170161)
 
 An [open source](https://github.com/BioMedIA/deepali/tree/main/LICENSE) research library for image, point set, and surface registration in [PyTorch], which is developed and maintained by the [HeartFlow-Imperial College London] research lab at the [Biomedical Image Analysis Group].
```

### Comparing `hf-deepali-0.4.1/TODO` & `hf-deepali-0.4.2/TODO`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/conda/Makefile` & `hf-deepali-0.4.2/conda/Makefile`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/conda/README.md` & `hf-deepali-0.4.2/conda/README.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/conda/environment.conda-lock.yml` & `hf-deepali-0.4.2/conda/environment.conda-lock.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/conda/environment.devenv.yml` & `hf-deepali-0.4.2/conda/environment.devenv.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/conda/environment.linux-64.lock` & `hf-deepali-0.4.2/conda/environment.linux-64.lock`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/conda/environment.linux-64.yml` & `hf-deepali-0.4.2/conda/environment.linux-64.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/conda/environment.osx-64.lock` & `hf-deepali-0.4.2/conda/environment.osx-64.lock`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/conda/environment.osx-64.yml` & `hf-deepali-0.4.2/conda/environment.osx-64.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/conda/environment.win-64.lock` & `hf-deepali-0.4.2/conda/environment.win-64.lock`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/conda/environment.win-64.yml` & `hf-deepali-0.4.2/conda/environment.win-64.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/docker/Dockerfile` & `hf-deepali-0.4.2/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/docker/build` & `hf-deepali-0.4.2/docker/build`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/docker/run` & `hf-deepali-0.4.2/docker/run`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/docs/_citations.bib` & `hf-deepali-0.4.2/docs/_citations.bib`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/docs/_config.yml` & `hf-deepali-0.4.2/docs/_config.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/docs/_images/logo.png` & `hf-deepali-0.4.2/docs/_images/logo.png`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/docs/_toc.yml` & `hf-deepali-0.4.2/docs/_toc.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/docs/basics/example-page.md` & `hf-deepali-0.4.2/docs/basics/example-page.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/docs/basics/installation.md` & `hf-deepali-0.4.2/docs/basics/installation.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/docs/index.md` & `hf-deepali-0.4.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/docs/reference/core/flow.md` & `hf-deepali-0.4.2/docs/reference/core/flow.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/docs/reference/core/image.md` & `hf-deepali-0.4.2/docs/reference/core/image.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/docs/reference/data/transforms.md` & `hf-deepali-0.4.2/docs/reference/data/transforms.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/docs/reference/spatial/common.md` & `hf-deepali-0.4.2/docs/reference/spatial/common.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/docs/reference/spatial/composite.md` & `hf-deepali-0.4.2/docs/reference/spatial/composite.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/docs/reference/utils/index.md` & `hf-deepali-0.4.2/docs/reference/utils/index.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/docs/tutorials/example-myst-notebook.md` & `hf-deepali-0.4.2/docs/tutorials/example-myst-notebook.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/docs/tutorials/example-notebook.ipynb` & `hf-deepali-0.4.2/docs/tutorials/example-notebook.ipynb`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/docs/tutorials/pairwise-registration-intro.ipynb` & `hf-deepali-0.4.2/docs/tutorials/pairwise-registration-intro.ipynb`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/examples/ffd/README.md` & `hf-deepali-0.4.2/examples/ffd/README.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/examples/ffd/engine.py` & `hf-deepali-0.4.2/examples/ffd/engine.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/examples/ffd/hooks.py` & `hf-deepali-0.4.2/examples/ffd/hooks.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/examples/ffd/losses.py` & `hf-deepali-0.4.2/examples/ffd/losses.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/examples/ffd/optim.py` & `hf-deepali-0.4.2/examples/ffd/optim.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/examples/ffd/pairwise.py` & `hf-deepali-0.4.2/examples/ffd/pairwise.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/examples/ffd/params.yaml` & `hf-deepali-0.4.2/examples/ffd/params.yaml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/examples/ffd/register.py` & `hf-deepali-0.4.2/examples/ffd/register.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/examples/istn/models/__init__.py` & `hf-deepali-0.4.2/examples/istn/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/examples/istn/models/itn.py` & `hf-deepali-0.4.2/examples/istn/models/itn.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/examples/istn/models/stn.py` & `hf-deepali-0.4.2/examples/istn/models/stn.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/examples/istn/params.yaml` & `hf-deepali-0.4.2/examples/istn/params.yaml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/examples/istn/train.py` & `hf-deepali-0.4.2/examples/istn/train.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/pyproject.toml` & `hf-deepali-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/core/__init__.py` & `hf-deepali-0.4.2/src/deepali/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/core/_kornia.py` & `hf-deepali-0.4.2/src/deepali/core/_kornia.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/core/affine.py` & `hf-deepali-0.4.2/src/deepali/core/affine.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/core/argparse.py` & `hf-deepali-0.4.2/src/deepali/core/argparse.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/core/bspline.py` & `hf-deepali-0.4.2/src/deepali/core/bspline.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/core/collections.py` & `hf-deepali-0.4.2/src/deepali/core/collections.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/core/config.py` & `hf-deepali-0.4.2/src/deepali/core/config.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/core/cube.py` & `hf-deepali-0.4.2/src/deepali/core/cube.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/core/enum.py` & `hf-deepali-0.4.2/src/deepali/core/enum.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/core/environ.py` & `hf-deepali-0.4.2/src/deepali/core/environ.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/core/flow.py` & `hf-deepali-0.4.2/src/deepali/core/flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -425,15 +425,14 @@
     assert data.device == grid.device
     return grid_sample(data, grid, mode=mode, padding=padding, align_corners=align_corners)
 
 
 def zeros_flow(
     size: Optional[Union[int, Size, Grid]] = None,
     shape: Optional[Shape] = None,
-    num: int = 1,
-    named: bool = False,
+    num: Optional[int] = None,
     dtype: Optional[DType] = None,
     device: Optional[Device] = None,
 ) -> Tensor:
     r"""Create batch of flow fields filled with zeros for given image batch size or grid."""
     size = _image_size("zeros_flow", size, shape)
-    return zeros_image(size, num=num, channels=len(size), named=named, dtype=dtype, device=device)
+    return zeros_image(size, num=num, channels=len(size), dtype=dtype, device=device)
```

### Comparing `hf-deepali-0.4.1/src/deepali/core/functional.py` & `hf-deepali-0.4.2/src/deepali/core/functional.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/core/grid.py` & `hf-deepali-0.4.2/src/deepali/core/grid.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/core/image.py` & `hf-deepali-0.4.2/src/deepali/core/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -1696,115 +1696,132 @@
 ) -> Tensor:
     r"""Synthetic image of a circle.
 
     Args:
         size: Spatial size in the order ``(X, Y)``.
         shape: Spatial size in the order ``(Y, X)``.
         num: Number ``N`` of images in batch.
+            If zero, return a single unbatched image tensor.
         center: Coordinates of center pixel in the order ``(x, y)``.
         radius: Radius of circle in pixel units.
         sigma: Standard deviation of isotropic Gaussian blurring kernel in pixel units.
         x_max: Maximum ``x`` pixel index at which to clamp image to zero.
             This can be used to create partial circles such as a half circle.
         dtype: Data type of output tensor. Use ``torch.uint8`` if ``None``.
             When the output data type is a floating point type, the output tensor
             values are in the interval ``[0, 1]``. Otherwise, the output values are
             in the interval ``[0, 255]``.
         device: Device on which to create image tensor.
 
     Returns:
-        Image tensor of shape ``(N, 1, Y, X)``.
+        Image tensor of shape ``(N, 1, Y, X)`` or ``(1, Y, X)`` (``num=0``).
 
     """
     size = _image_size("circle_image", size, shape, ndim=2)
     if center is None:
         center = tuple(((n - 1) / 2 for n in size))
     center = tuple(float(x) for x in center)
     grid = Grid(size=size)
     if radius is None:
         radius = max(0, (min(center) - 1) - math.ceil(2 * sigma))
     _dtype = torch.float32
     _device = torch.device("cpu")
     c = as_tensor(center, dtype=_dtype, device=_device)
     x = grid.coords(normalize=False, dtype=_dtype, device=_device)
-    x = x.reshape(num or 1, 1, *x.shape) - c
+    x = x.reshape(1, 1, *grid.shape, grid.ndim).sub_(c)
     data = torch.norm(x, dim=-1) <= radius
-    if x_max:
+    if x_max is not None:
         x_threshold = as_tensor(x_max, dtype=_dtype, device=_device)
         if x_threshold.ndim == 0:
             data &= x[..., 0] <= x_threshold
         else:
             data &= (x <= x_threshold).all(dim=-1)
     data = data.type(_dtype)
     if sigma > 0:
         kernel = gaussian1d(sigma, dtype=data.dtype, device=_device)
         data = conv(data, kernel / kernel.sum())
     if dtype is None:
         dtype = torch.uint8
     if not dtype.is_floating_point:
-        data = 255 * data / data.max()
-    return data.to(dtype=dtype, device=device)
+        data = data.mul_(255).div_(data.max())
+    data = data.to(dtype=dtype, device=device)
+    if num is not None:
+        if num == 0:
+            data = data.squeeze_(0)
+        elif num > 1:
+            data = data.expand(num, *data.shape[1:])
+    return data
 
 
 def cshape_image(
     size: Optional[Union[int, Size, Grid]] = None,
     shape: Optional[Shape] = None,
     num: Optional[int] = None,
     center: Optional[Sequence[float]] = None,
     radius: Optional[float] = None,
     width: Optional[float] = None,
     sigma: float = 0,
-    x_max: Union[float, Sequence[float]] = 5,
+    x_max: Optional[Union[float, Sequence[float]]] = None,
     dtype: Optional[DType] = None,
     device: Optional[Device] = None,
 ) -> Tensor:
     r"""Synthetic C-shaped image.
 
     Args:
         size: Spatial size in the order ``(X, Y)``.
         shape: Spatial size in the order ``(Y, X)``.
         num: Number ``N`` of images in batch.
+            If zero, return a single unbatched image tensor.
         center: Coordinates of center pixel in the order ``(y, x)``.
         radius: Radius of circle in pixel units.
+        width: Difference between outer and inner circle radius.
+            A default width of ``radius // 2`` is used if ``None``.
         sigma: Standard deviation of isotropic Gaussian blurring kernel in pixel units.
-        x_max: Maximum ``x`` pixel index at which to clamp image to zero.
-            This can be used to create partial circles such as a half circle.
+        x_max: Maximum ``x`` pixel index at which to clamp image to zero. This is used to create
+            partial circles with an opening for the "C" shape to the right. If ``None``, a default
+            value equal to 75% of the inner circle radius is chosen.
         dtype: Data type of output tensor. Use ``torch.uint8`` if ``None``.
             When the output data type is a floating point type, the output tensor
             values are in the interval ``[0, 1]``. Otherwise, the output values are
             in the interval ``[0, 255]``.
         device: Device on which to create image tensor.
 
     Returns:
-        Image tensor of shape ``(N, 1, Y, X)``.
+        Image tensor of shape ``(N, 1, Y, X)`` or ``(1, Y, X)`` (``num=0``).
 
     """
     size = _image_size("cshape_image", size, shape, ndim=2)
     if dtype is None:
         dtype = torch.uint8
     if radius is None:
         center = tuple(float(x) for x in center)
         radius = max(0, (min(center) - 1) - math.ceil(2 * sigma))
     if width is None:
         width = radius // 2
-    outer = circle_image(size, center=center, radius=radius, x_max=x_max, sigma=0)
-    inner = circle_image(size, center=center, radius=radius - width, sigma=0)
-    image = (outer - inner).type(torch.float32)
+    if x_max is None:
+        x_max = 0.75 * (radius - width)
+    outer = circle_image(size, num=1, x_max=x_max, sigma=0, center=center, radius=radius)
+    inner = circle_image(size, num=1, x_max=x_max, sigma=0, center=center, radius=radius - width)
+    image = outer.type(torch.float32).sub(inner)
     if sigma > 0:
         kernel = gaussian1d(sigma, dtype=torch.float32, device=image.device)
         image = conv(image, kernel)
         if dtype.is_floating_point:
             image /= image.max()
             image.clamp_(min=0, max=1)
         else:
             image *= 255 / image.max()
             image.clamp_(min=0, max=255)
-    if num and num > 1:
-        image = image.expand((1,) + image.shape[1:])
-    return image.to(dtype=dtype, device=device)
+    image = image.to(dtype=dtype, device=device)
+    if num is not None:
+        if num == 0:
+            image = image.squeeze_(0)
+        elif num > 1:
+            image = image.expand((1,) + image.shape[1:])
+    return image
 
 
 def empty_image(
     size: Optional[Union[int, Size, Grid]] = None,
     shape: Optional[Shape] = None,
     num: Optional[int] = None,
     channels: Optional[int] = None,
@@ -1813,25 +1830,29 @@
 ) -> Tensor:
     """Create new batch of uninitalized image data.
 
     Args:
         size: Spatial size in the order ``(X, ...)``.
         shape: Spatial size in the order ``(..., X)``.
         num: Number of images in batch.
+            If zero, return a single unbatched image tensor.
         channels: Number of channels per image.
         dtype: Data type of image tensor.
         device: Device on which to store image data.
 
     Returns:
-        Uninitialized image batch tensor.
+        Image tensor of shape ``(N, 1, ..., X)`` or ``(1, ..., X)`` (``num=0``).
 
     """
     size = _image_size("empty_image", size, shape)
     shape = (num or 1, channels or 1) + tuple(reversed(size))
-    return torch.empty(shape, dtype=dtype, device=device)
+    data = torch.empty(shape, dtype=dtype, device=device)
+    if num == 0:
+        data = data.squeeze_(0)
+    return data
 
 
 def grid_image(
     size: Optional[Union[int, Size, Grid]] = None,
     shape: Optional[Shape] = None,
     num: Optional[int] = None,
     stride: Optional[Union[int, Sequence[int]]] = None,
@@ -1842,24 +1863,25 @@
     """Create batch of regularly spaced grid images.
 
     Args:
         size: Spatial size in the order ``(X, ...)``.
         shape: Spatial size in the order ``(..., X)``.
         num: Number of images in batch. When ``shape`` is not a ``Grid``, must
             match the size of the first dimension in ``shape`` if not ``None``.
+            If zero, return a single unbatched image tensor.
         stride: Spacing between grid lines. To draw in-plane grid lines on a
             D-dimensional image where ``D>2``, specify a sequence of two stride
             values, where the first stride applies to the last tensor dimension,
             which corresponds to the first spatial grid dimension.
         inverted: Whether to draw grid lines in black (0) over white (1) background.
         dtype: Data type of image tensor.
         device: Device on which to store image data.
 
     Returns:
-        Image tensor of shape ``(N, 1, ..., X)``. The default number of channels is 1.
+        Image tensor of shape ``(N, 1, ..., X)`` or ``(1, ..., X)`` (``num=0``).
 
     """
     size = _image_size("grid_image", size, shape)
     data = empty_image(size, num=1, channels=1, dtype=dtype, device=device)
     data.fill_(1 if inverted else 0)
     if stride is None:
         stride = 4
@@ -1870,15 +1892,20 @@
             "grid_image() 'stride' length must not be greater than number of spatial dimensions"
         )
     start = data.ndim - len(stride)
     for dim, step in zip(range(start, data.ndim), reversed(stride)):
         n = data.shape[dim]
         index = torch.arange((n % step) // 2, n, step, dtype=torch.int64, device=data.device)
         data.index_fill_(dim, index, 0 if inverted else 1)
-    return data.expand(num or 1, *data.shape[1:])
+    if num is not None:
+        if num == 0:
+            data = data.squeeze_(0)
+        elif num > 1:
+            data = data.expand((1,) + data.shape[1:])
+    return data
 
 
 def ones_image(
     size: Optional[Union[int, Size, Grid]] = None,
     shape: Optional[Shape] = None,
     num: Optional[int] = None,
     channels: Optional[int] = None,
@@ -1892,15 +1919,15 @@
         shape: Spatial size in the order ``(..., X)``.
         num: Number of images in batch.
         channels: Number of channels per image.
         dtype: Data type of image tensor.
         device: Device on which to store image data.
 
     Returns:
-        Image batch tensor filled with ones.
+        Image tensor of shape ``(N, 1, ..., X)`` or ``(1, ..., X)`` (``num=0``) filled with ones.
 
     """
     size = _image_size("ones_image", size, shape)
     data = empty_image(size, num=num, channels=channels, dtype=dtype, device=device)
     return data.fill_(1)
 
 
@@ -1919,13 +1946,13 @@
         shape: Spatial size in the order ``(..., X)``.
         num: Number of images in batch.
         channels: Number of channels per image.
         dtype: Data type of image tensor.
         device: Device on which to store image data.
 
     Returns:
-        Image batch tensor filled with zeros.
+        Image tensor of shape ``(N, 1, ..., X)`` or ``(1, ..., X)`` (``num=0``) filled with zeros.
 
     """
     size = _image_size("zeros_image", size, shape)
     data = empty_image(size, num=num, channels=channels, dtype=dtype, device=device)
     return data.fill_(0)
```

### Comparing `hf-deepali-0.4.1/src/deepali/core/itertools.py` & `hf-deepali-0.4.2/src/deepali/core/itertools.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/core/kernels.py` & `hf-deepali-0.4.2/src/deepali/core/kernels.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/core/linalg.py` & `hf-deepali-0.4.2/src/deepali/core/linalg.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/core/logging.py` & `hf-deepali-0.4.2/src/deepali/core/logging.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/core/math.py` & `hf-deepali-0.4.2/src/deepali/core/math.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/core/nnutils.py` & `hf-deepali-0.4.2/src/deepali/core/nnutils.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/core/pathlib.py` & `hf-deepali-0.4.2/src/deepali/core/pathlib.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/core/pointset.py` & `hf-deepali-0.4.2/src/deepali/core/pointset.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/core/psutil.py` & `hf-deepali-0.4.2/src/deepali/core/psutil.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/core/random.py` & `hf-deepali-0.4.2/src/deepali/core/random.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/core/tempfile.py` & `hf-deepali-0.4.2/src/deepali/core/tempfile.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/core/tensor.py` & `hf-deepali-0.4.2/src/deepali/core/tensor.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/core/typing.py` & `hf-deepali-0.4.2/src/deepali/core/typing.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/data/__init__.py` & `hf-deepali-0.4.2/src/deepali/data/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/data/collate.py` & `hf-deepali-0.4.2/src/deepali/data/collate.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/data/dataset.py` & `hf-deepali-0.4.2/src/deepali/data/dataset.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/data/flow.py` & `hf-deepali-0.4.2/src/deepali/data/flow.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/data/image.py` & `hf-deepali-0.4.2/src/deepali/data/image.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/data/partition.py` & `hf-deepali-0.4.2/src/deepali/data/partition.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/data/prepare.py` & `hf-deepali-0.4.2/src/deepali/data/prepare.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/data/sample.py` & `hf-deepali-0.4.2/src/deepali/data/sample.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/data/sampler.py` & `hf-deepali-0.4.2/src/deepali/data/sampler.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/data/tensor.py` & `hf-deepali-0.4.2/src/deepali/data/tensor.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/data/transforms/__init__.py` & `hf-deepali-0.4.2/src/deepali/data/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/data/transforms/image.py` & `hf-deepali-0.4.2/src/deepali/data/transforms/image.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/data/transforms/item.py` & `hf-deepali-0.4.2/src/deepali/data/transforms/item.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/losses/__init__.py` & `hf-deepali-0.4.2/src/deepali/losses/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 from .flow import Diffusion
 from .flow import Divergence
 from .flow import Elasticity
 from .flow import TotalVariation, TV
 
 from .image import PatchwiseImageLoss, PatchLoss
 from .image import Dice, DSC
+from .image import NCC
 from .image import LCC, LNCC
 from .image import SLCC, WLCC
 from .image import MI, NMI
 from .image import MAE, L1ImageLoss
 from .image import HuberImageLoss
 from .image import SmoothL1ImageLoss
 from .image import MSE, L2ImageLoss
@@ -95,14 +96,15 @@
     "LandmarkPointDistance",
     "LPD",
     "LCC",
     "LNCC",
     "MAE",
     "MI",
     "MSE",
+    "NCC",
     "NMI",
     "SLCC",
     "SmoothL1ImageLoss",
     "Sparsity",
     "SSD",
     "TotalVariation",
     "TV",
```

### Comparing `hf-deepali-0.4.1/src/deepali/losses/base.py` & `hf-deepali-0.4.2/src/deepali/losses/base.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/losses/flow.py` & `hf-deepali-0.4.2/src/deepali/losses/flow.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/losses/functional.py` & `hf-deepali-0.4.2/src/deepali/losses/functional.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     "label_smoothing",
     "dice_score",
     "dice_loss",
     "kld_loss",
     "lcc_loss",
     "mae_loss",
     "mse_loss",
+    "ncc_loss",
     "ssd_loss",
     "mi_loss",
     "grad_loss",
     "bending_loss",
     "bending_energy",
     "be_loss",
     "bspline_bending_loss",
@@ -524,14 +525,63 @@
     """
     loss = mean.square().add_(logvar.exp()).sub_(1).sub_(logvar)
     loss = reduce_loss(loss, reduction)
     loss = loss.mul_(0.5)
     return loss
 
 
+def ncc_loss(
+    source: Tensor,
+    target: Tensor,
+    mask: Optional[Tensor] = None,
+    epsilon: float = 1e-15,
+    reduction: str = "mean",
+) -> Tensor:
+    r"""Normalized cross correlation.
+
+    Args:
+        source: Source image sampled on ``target`` grid.
+        target: Target image with same shape as ``source``.
+        mask: Multiplicative mask tensor with same shape as ``source``.
+        epsilon: Small constant added to denominator to avoid division by zero.
+        reduction: Whether to compute "mean" or "sum" of normalized cross correlation
+            of image pairs in batch. If "none", a 1-dimensional tensor is returned
+            with length equal the batch size.
+
+    Returns:
+        Negative squared normalized cross correlation plus one.
+
+    """
+
+    if not isinstance(source, Tensor):
+        raise TypeError("ncc_loss() 'source' must be tensor")
+    if not isinstance(target, Tensor):
+        raise TypeError("ncc_loss() 'target' must be tensor")
+    if source.shape != target.shape:
+        raise ValueError("ncc_loss() 'source' must have same shape as 'target'")
+
+    source = source.reshape(source.shape[0], -1).float()
+    target = target.reshape(source.shape[0], -1).float()
+
+    source_mean = source.mean(dim=1, keepdim=True)
+    target_mean = target.mean(dim=1, keepdim=True)
+
+    x = source.sub(source_mean)
+    y = target.sub(target_mean)
+
+    a = x.mul(y).sum(dim=1)
+    b = x.square().sum(dim=1)
+    c = y.square().sum(dim=1)
+
+    loss = a.square_().div_(b.mul_(c).add_(epsilon)).neg_().add_(1)
+    loss = masked_loss(loss, mask, "ncc_loss")
+    loss = reduce_loss(loss, reduction, mask)
+    return loss
+
+
 def lcc_loss(
     source: Tensor,
     target: Tensor,
     mask: Optional[Tensor] = None,
     kernel_size: ScalarOrTuple[int] = 7,
     epsilon: float = 1e-15,
     reduction: str = "mean",
```

### Comparing `hf-deepali-0.4.1/src/deepali/losses/image.py` & `hf-deepali-0.4.2/src/deepali/losses/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,34 @@
     def extra_repr(self) -> str:
         return f"epsilon={self.epsilon:.2e}"
 
 
 DSC = Dice
 
 
+class NCC(PairwiseImageLoss):
+    r"""Normalized cross correlation."""
+
+    def __init__(self, epsilon: float = 1e-15) -> None:
+        super().__init__()
+        self.epsilon = epsilon
+
+    def forward(self, source: Tensor, target: Tensor, mask: Optional[Tensor] = None) -> Tensor:
+        r"""Evaluate image dissimilarity loss."""
+        return L.ncc_loss(
+            source,
+            target,
+            mask=mask,
+            epsilon=self.epsilon,
+        )
+
+    def extra_repr(self) -> str:
+        return f"epsilon={self.epsilon:.2e}"
+
+
 class LCC(PairwiseImageLoss):
     r"""Local normalized cross correlation."""
 
     def __init__(self, kernel_size: ScalarOrTuple[int] = 7, epsilon: float = 1e-15) -> None:
         super().__init__()
         self.kernel_size = kernel_size
         self.epsilon = epsilon
```

### Comparing `hf-deepali-0.4.1/src/deepali/losses/params.py` & `hf-deepali-0.4.2/src/deepali/losses/params.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/losses/pointset.py` & `hf-deepali-0.4.2/src/deepali/losses/pointset.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/modules/__init__.py` & `hf-deepali-0.4.2/src/deepali/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/modules/basic.py` & `hf-deepali-0.4.2/src/deepali/modules/basic.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/modules/flow.py` & `hf-deepali-0.4.2/src/deepali/modules/flow.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/modules/image.py` & `hf-deepali-0.4.2/src/deepali/modules/image.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/modules/lambd.py` & `hf-deepali-0.4.2/src/deepali/modules/lambd.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/modules/mixins.py` & `hf-deepali-0.4.2/src/deepali/modules/mixins.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/modules/output.py` & `hf-deepali-0.4.2/src/deepali/modules/output.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/modules/sample.py` & `hf-deepali-0.4.2/src/deepali/modules/sample.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/modules/utilities.py` & `hf-deepali-0.4.2/src/deepali/modules/utilities.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/networks/__init__.py` & `hf-deepali-0.4.2/src/deepali/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/networks/blocks/residual.py` & `hf-deepali-0.4.2/src/deepali/networks/blocks/residual.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/networks/blocks/skip.py` & `hf-deepali-0.4.2/src/deepali/networks/blocks/skip.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/networks/layers/__init__.py` & `hf-deepali-0.4.2/src/deepali/networks/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/networks/layers/acti.py` & `hf-deepali-0.4.2/src/deepali/networks/layers/acti.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/networks/layers/conv.py` & `hf-deepali-0.4.2/src/deepali/networks/layers/conv.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/networks/layers/join.py` & `hf-deepali-0.4.2/src/deepali/networks/layers/join.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/networks/layers/linear.py` & `hf-deepali-0.4.2/src/deepali/networks/layers/linear.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/networks/layers/norm.py` & `hf-deepali-0.4.2/src/deepali/networks/layers/norm.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/networks/layers/pool.py` & `hf-deepali-0.4.2/src/deepali/networks/layers/pool.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/networks/layers/upsample.py` & `hf-deepali-0.4.2/src/deepali/networks/layers/upsample.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/networks/resnet.py` & `hf-deepali-0.4.2/src/deepali/networks/resnet.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/networks/unet.py` & `hf-deepali-0.4.2/src/deepali/networks/unet.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/networks/utils.py` & `hf-deepali-0.4.2/src/deepali/networks/utils.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/spatial/__init__.py` & `hf-deepali-0.4.2/src/deepali/spatial/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/spatial/base.py` & `hf-deepali-0.4.2/src/deepali/spatial/base.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/spatial/bspline.py` & `hf-deepali-0.4.2/src/deepali/spatial/bspline.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/spatial/composite.py` & `hf-deepali-0.4.2/src/deepali/spatial/composite.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/spatial/generic.py` & `hf-deepali-0.4.2/src/deepali/spatial/generic.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/spatial/linear.py` & `hf-deepali-0.4.2/src/deepali/spatial/linear.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/spatial/nonrigid.py` & `hf-deepali-0.4.2/src/deepali/spatial/nonrigid.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/spatial/parametric.py` & `hf-deepali-0.4.2/src/deepali/spatial/parametric.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/spatial/transformer.py` & `hf-deepali-0.4.2/src/deepali/spatial/transformer.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 and maps these to new spatial locations, to a given input data tensor.
 
 """
 
 from __future__ import annotations
 
 from copy import copy as shallow_copy
-from typing import Dict, Optional, Tuple, TypeVar, Union, cast, overload
+from typing import Dict, Optional, Tuple, TypeVar, Union, overload
 
 from torch import Tensor
 from torch.nn import Module
 
 from deepali.core.enum import PaddingMode, Sampling
 from deepali.core.grid import Axes, Grid
 from deepali.core.typing import Scalar
@@ -120,16 +120,23 @@
         align_centers: bool = False,
         flip_coords: bool = False,
     ) -> None:
         r"""Initialize spatial image transformer.
 
         Args:
             transform: Spatial coordinate transformation which is applied to ``target`` grid points.
-            target: Sampling grid of output images. If ``None``, use ``transform.grid()``.
-            source: Sampling grid of input images. If ``None``, use ``target``.
+            target: Sampling grid of output images. Use ``transform.grid()`` if ``None``.
+            source: Sampling grid of input images. The attributes of this sampling grid are used
+                to map the transformed normalized coordinates defined with respect to ``transform.grid()``
+                to normalized coordinates with respect to the moving ``source`` image grid. These
+                normalized coordinates are used to sample the image tensor passed to the forward
+                method of the image transformer. If ``None``, it is assumed that the sampling grid
+                of the moving source image is identical to the ``target`` image grid. In order to
+                avoid having to re-normalize coordinates between image domains, the ``source`` grid
+                domain should be the same as the ``transform.grid()`` (cf. :meth:`Grid.same_domain_as`).
             sampling: Image interpolation mode.
             padding: Image extrapolation mode or scalar out-of-domain value.
             align_centers: Whether to implicitly align the ``target`` and ``source`` centers.
                 If ``True``, only the affine component of the target to source transformation
                 is applied after the spatial grid ``transform``. If ``False``, also the
                 translation of grid center points is considered.
             flip_coords: Whether spatial transformation applies to flipped grid point coordinates
@@ -141,39 +148,37 @@
             target = transform.grid()
         if source is None:
             source = target
         if not isinstance(target, Grid):
             raise TypeError(f"{type(self).__name__}() 'target' must be of type Grid")
         if not isinstance(source, Grid):
             raise TypeError(f"{type(self).__name__}() 'source' must be of type Grid")
-        if not transform.grid().same_domain_as(target):
-            raise ValueError(
-                f"{type(self).__name__}() 'target' and 'transform' grid must define the same domain"
-            )
         device = transform.device
         sampler = SampleImage(
-            target=target,
+            target=transform.grid(),
             source=source,
             sampling=sampling,
             padding=padding,
             align_centers=align_centers,
         )
         self._sample = sampler.to(device)
-        grid_coords = target.coords(flip=flip_coords, device=device).unsqueeze(0)
-        self.register_buffer("grid_coords", grid_coords, persistent=False)
-        self.flip_coords = bool(flip_coords)
+        self._target_grid = target
+        self._flip_coords = bool(flip_coords)
+        x = target.coords(align_corners=transform.align_corners(), flip=flip_coords, device=device)
+        x = target.transform_points(x, axes=transform.axes(), to_grid=transform.grid())
+        self.register_buffer("grid_coords", x.unsqueeze(0), persistent=False)
 
     @property
     def sample(self) -> SampleImage:
         r"""Source image sampler."""
         return self._sample
 
     def target_grid(self) -> Grid:
         r"""Sampling grid of output images."""
-        return self._sample.target_grid()
+        return self._target_grid
 
     def source_grid(self) -> Grid:
         r"""Sampling grid of input images."""
         return self._sample.source_grid()
 
     def align_centers(self) -> bool:
         r"""Whether grid center points are implicitly aligned."""
@@ -196,17 +201,17 @@
 
     def forward(
         self,
         data: Union[Tensor, Dict[str, Union[Tensor, Grid]]],
         mask: Optional[Tensor] = None,
     ) -> Union[Tensor, Tuple[Tensor, Tensor], Dict[str, Union[Tensor, Grid]]]:
         r"""Sample batch of images at spatially transformed target grid points."""
-        grid: Tensor = cast(Tensor, self.grid_coords)
+        grid: Tensor = self.grid_coords
         grid = self._transform(grid, grid=True)
-        if self.flip_coords:
+        if self._flip_coords:
             grid = grid.flip((-1,))
         return self._sample(grid, data, mask)
 
 
 class PointSetTransformer(SpatialTransformer):
     r"""Spatially transform a set of points.
```

### Comparing `hf-deepali-0.4.1/src/deepali/utils/aws/s3/client.py` & `hf-deepali-0.4.2/src/deepali/utils/aws/s3/client.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/utils/aws/s3/config.py` & `hf-deepali-0.4.2/src/deepali/utils/aws/s3/config.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/utils/aws/s3/object.py` & `hf-deepali-0.4.2/src/deepali/utils/aws/s3/object.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/utils/ignite/handlers.py` & `hf-deepali-0.4.2/src/deepali/utils/ignite/handlers.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/utils/ignite/metrics/average_loss.py` & `hf-deepali-0.4.2/src/deepali/utils/ignite/metrics/average_loss.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/utils/ignite/metrics/binary_classification.py` & `hf-deepali-0.4.2/src/deepali/utils/ignite/metrics/binary_classification.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/utils/ignite/metrics/multilabel_classification.py` & `hf-deepali-0.4.2/src/deepali/utils/ignite/metrics/multilabel_classification.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/utils/ignite/output_transforms.py` & `hf-deepali-0.4.2/src/deepali/utils/ignite/output_transforms.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/utils/ignite/score_functions.py` & `hf-deepali-0.4.2/src/deepali/utils/ignite/score_functions.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/utils/imageio/__init__.py` & `hf-deepali-0.4.2/src/deepali/utils/imageio/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/utils/imageio/meta.py` & `hf-deepali-0.4.2/src/deepali/utils/imageio/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         data, meta = read_meta_image_from_fileobj(arg)
     else:
         raise TypeError("read_meta_image() 'arg' must be path, bytes, or io.BufferedReader")
     if meta.get("ElementNumberOfChannels", 1) == 1:
         data = np.expand_dims(data, 0)
     else:
         data = np.squeeze(np.swapaxes(np.expand_dims(data, 0), 0, -1), -1)
-    size = meta.get("DimSize", data.shape[:0:-1])
+    size = tuple(meta.get("DimSize", data.shape[:0:-1]))
     assert size[::-1] == data.shape[1:]
     origin = meta.get("Position", meta.get("Origin", meta.get("Offset")))
     matrix = meta.get("Rotation", meta.get("Orientation", meta.get("TransformMatrix")))
     spacing = meta.get("ElementSpacing")
     grid = Grid(
         size=size,
         origin=origin,
@@ -288,14 +288,15 @@
                 read = 0
         data.write(f.read(read))
         buffer = data.getbuffer()
 
     image = np.frombuffer(buffer, dtype=meta["ElementType"]).reshape(shape)
     if meta.get("BinaryDataByteOrderMSB") or meta.get("ElementByteOrderMSB"):
         image.byteswap(inplace=True)
+    image = image.copy()
 
     # remove unused metadata
     meta["ElementDataFile"] = None
     meta = {x: y for x, y in meta.items() if y is not None}
 
     return image, meta
```

### Comparing `hf-deepali-0.4.1/src/deepali/utils/imageio/nifti.py` & `hf-deepali-0.4.2/src/deepali/utils/imageio/nifti.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/utils/imageio/sitk.py` & `hf-deepali-0.4.2/src/deepali/utils/imageio/sitk.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/utils/simpleitk/grid.py` & `hf-deepali-0.4.2/src/deepali/utils/simpleitk/grid.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/utils/simpleitk/imageio.py` & `hf-deepali-0.4.2/src/deepali/utils/simpleitk/imageio.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/utils/simpleitk/numpy.py` & `hf-deepali-0.4.2/src/deepali/utils/simpleitk/numpy.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/utils/simpleitk/sample.py` & `hf-deepali-0.4.2/src/deepali/utils/simpleitk/sample.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/utils/simpleitk/torch.py` & `hf-deepali-0.4.2/src/deepali/utils/simpleitk/torch.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/utils/storage.py` & `hf-deepali-0.4.2/src/deepali/utils/storage.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/utils/tensorboard.py` & `hf-deepali-0.4.2/src/deepali/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/utils/vtk/idlist.py` & `hf-deepali-0.4.2/src/deepali/utils/vtk/idlist.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/utils/vtk/image.py` & `hf-deepali-0.4.2/src/deepali/utils/vtk/image.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/utils/vtk/numpy.py` & `hf-deepali-0.4.2/src/deepali/utils/vtk/numpy.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/utils/vtk/polydataio.py` & `hf-deepali-0.4.2/src/deepali/utils/vtk/polydataio.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/deepali/utils/vtk/simpleitk.py` & `hf-deepali-0.4.2/src/deepali/utils/vtk/simpleitk.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/src/hf_deepali.egg-info/PKG-INFO` & `hf-deepali-0.4.2/src/hf_deepali.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hf-deepali
-Version: 0.4.1
+Version: 0.4.2
 Summary: Image, point set, and surface registration library for PyTorch.
 Maintainer-email: Andreas Schuh <andreas.schuh@imperial.ac.uk>
 License: Apache-2.0
 Project-URL: Homepage, https://biomedia.github.io/deepali
 Project-URL: Repository, https://github.com/BioMedIA/deepali.git
 Project-URL: Bug Tracker, https://github.com/BioMedIA/deepali/issues
 Keywords: medical-imaging,image-registration,spatial-transformer-networks
@@ -24,15 +24,15 @@
 Provides-Extra: utils
 Provides-Extra: tests
 License-File: LICENSE
 
 # deepali
 
 <!-- ![downloads](https://img.shields.io/pypi/dm/hf-deepali) -->
-![pypi](https://img.shields.io/pypi/v/hf-deepali)
+[![pypi](https://img.shields.io/pypi/v/hf-deepali)](https://pypi.org/project/hf-deepali/)
 ![python](https://img.shields.io/pypi/pyversions/hf-deepali)
 [![docs](https://github.com/BioMedIA/deepali/actions/workflows/docs.yml/badge.svg)](https://github.com/BioMedIA/deepali/actions/workflows/docs.yml)
 [![tests](https://github.com/BioMedIA/deepali/actions/workflows/tests.yml/badge.svg)](https://github.com/BioMedIA/deepali/actions/workflows/tests.yml)
 [![release](https://github.com/BioMedIA/deepali/actions/workflows/release.yml/badge.svg)](https://github.com/BioMedIA/deepali/actions/workflows/release.yml)
 [![doi](https://zenodo.org/badge/DOI/10.5281/zenodo.8170161.svg)](https://doi.org/10.5281/zenodo.8170161)
 
 An [open source](https://github.com/BioMedIA/deepali/tree/main/LICENSE) research library for image, point set, and surface registration in [PyTorch], which is developed and maintained by the [HeartFlow-Imperial College London] research lab at the [Biomedical Image Analysis Group].
```

### Comparing `hf-deepali-0.4.1/src/hf_deepali.egg-info/SOURCES.txt` & `hf-deepali-0.4.2/src/hf_deepali.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -198,17 +198,19 @@
 src/hf_deepali.egg-info/requires.txt
 src/hf_deepali.egg-info/top_level.txt
 tests/__init__.py
 tests/_test_core_bspline.py
 tests/test_core_bspline.py
 tests/test_core_cube.py
 tests/test_core_grid.py
+tests/test_core_image_create.py
 tests/test_core_image_utils.py
 tests/test_core_random.py
 tests/test_core_tensor_utils.py
 tests/test_data_flow.py
 tests/test_data_image.py
 tests/test_network_blocks.py
 tests/test_network_layers.py
 tests/test_network_resnet.py
 tests/test_network_unet.py
+tests/test_spatial_transformer.py
 tests/test_utils_imageio_meta.py
```

### Comparing `hf-deepali-0.4.1/tests/_test_core_bspline.py` & `hf-deepali-0.4.2/tests/_test_core_bspline.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/tests/test_core_bspline.py` & `hf-deepali-0.4.2/tests/test_core_bspline.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/tests/test_core_cube.py` & `hf-deepali-0.4.2/tests/test_core_cube.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/tests/test_core_grid.py` & `hf-deepali-0.4.2/tests/test_core_grid.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/tests/test_core_image_utils.py` & `hf-deepali-0.4.2/tests/test_core_image_utils.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/tests/test_core_random.py` & `hf-deepali-0.4.2/tests/test_core_random.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/tests/test_core_tensor_utils.py` & `hf-deepali-0.4.2/tests/test_core_tensor_utils.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/tests/test_data_flow.py` & `hf-deepali-0.4.2/tests/test_data_flow.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/tests/test_data_image.py` & `hf-deepali-0.4.2/tests/test_data_image.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/tests/test_network_blocks.py` & `hf-deepali-0.4.2/tests/test_network_blocks.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/tests/test_network_layers.py` & `hf-deepali-0.4.2/tests/test_network_layers.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/tests/test_network_unet.py` & `hf-deepali-0.4.2/tests/test_network_unet.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.1/tests/test_utils_imageio_meta.py` & `hf-deepali-0.4.2/tests/test_utils_imageio_meta.py`

 * *Files identical despite different names*

