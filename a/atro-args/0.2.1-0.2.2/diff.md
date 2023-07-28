# Comparing `tmp/atro_args-0.2.1.tar.gz` & `tmp/atro_args-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atro_args-0.2.1.tar", max compression
+gzip compressed data, was "atro_args-0.2.2.tar", max compression
```

## Comparing `atro_args-0.2.1.tar` & `atro_args-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0        0 2023-06-17 12:33:58.233092 atro_args-0.2.1/README.md
--rw-r--r--   0        0        0       89 2023-07-23 14:15:04.213219 atro_args-0.2.1/atro_args/__init__.py
--rw-r--r--   0        0        0      314 2023-07-23 19:54:45.502758 atro_args-0.2.1/atro_args/arg.py
--rw-r--r--   0        0        0      147 2023-07-23 14:11:53.169286 atro_args-0.2.1/atro_args/arg_type.py
--rw-r--r--   0        0        0     5677 2023-07-23 19:54:13.448770 atro_args-0.2.1/atro_args/input_args.py
--rw-r--r--   0        0        0      407 2023-07-23 19:54:58.126350 atro_args-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      349 1970-01-01 00:00:00.000000 atro_args-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      963 2023-07-28 15:55:58.438531 atro_args-0.2.2/README.md
+-rw-r--r--   0        0        0       89 2023-07-28 15:55:58.438531 atro_args-0.2.2/atro_args/__init__.py
+-rw-r--r--   0        0        0     1688 2023-07-28 15:55:58.438531 atro_args-0.2.2/atro_args/arg.py
+-rw-r--r--   0        0        0      333 2023-07-28 15:55:58.438531 atro_args-0.2.2/atro_args/arg_source.py
+-rw-r--r--   0        0        0     1254 2023-07-28 15:55:58.438531 atro_args-0.2.2/atro_args/helpers.py
+-rw-r--r--   0        0        0     8192 2023-07-28 15:55:58.438531 atro_args-0.2.2/atro_args/input_args.py
+-rw-r--r--   0        0        0      407 2023-07-28 18:14:24.886698 atro_args-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1312 1970-01-01 00:00:00.000000 atro_args-0.2.2/PKG-INFO
```

