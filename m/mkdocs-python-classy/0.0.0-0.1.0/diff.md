# Comparing `tmp/mkdocs-python-classy-0.0.0.tar.gz` & `tmp/mkdocs_python_classy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmp.QN6Ehpp1jy/mkdocs-python-classy-0.0.0.tar", last modified: Mon Apr 24 19:23:08 2023, max compression
+gzip compressed data, was "mkdocs_python_classy-0.1.0.tar", max compression
```

## Comparing `mkdocs-python-classy-0.0.0.tar` & `mkdocs_python_classy-0.1.0.tar`

### file list

```diff
@@ -1,3 +1,10 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:23:08.000000 mkdocs-python-classy-0.0.0/
--rw-r--r--   0 root         (0) root         (0)      241 2023-04-24 19:23:08.000000 mkdocs-python-classy-0.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      137 2023-04-24 19:23:08.000000 mkdocs-python-classy-0.0.0/setup.py
+-rw-r--r--   0        0        0      581 2023-07-28 03:22:49.953669 mkdocs_python_classy-0.1.0/LICENSE
+-rw-r--r--   0        0        0      302 2023-07-28 03:22:49.953669 mkdocs_python_classy-0.1.0/NOTICE
+-rw-r--r--   0        0        0     3997 2023-07-28 03:22:49.953669 mkdocs_python_classy-0.1.0/README.md
+-rw-r--r--   0        0        0     7950 2023-07-28 03:22:49.957669 mkdocs_python_classy-0.1.0/mkdocs_python_classy/__init__.py
+-rw-r--r--   0        0        0      288 2023-07-28 03:22:49.957669 mkdocs_python_classy-0.1.0/mkdocs_python_classy/constants.py
+-rw-r--r--   0        0        0       32 2023-07-28 03:22:49.957669 mkdocs_python_classy-0.1.0/mkdocs_python_classy/css/classy.css
+-rw-r--r--   0        0        0    13413 2023-07-28 03:22:49.957669 mkdocs_python_classy-0.1.0/mkdocs_python_classy/inspector.py
+-rw-r--r--   0        0        0     3598 2023-07-28 03:22:49.957669 mkdocs_python_classy-0.1.0/mkdocs_python_classy/utils.py
+-rw-r--r--   0        0        0     3203 2023-07-28 03:23:02.533755 mkdocs_python_classy-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4741 1970-01-01 00:00:00.000000 mkdocs_python_classy-0.1.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

