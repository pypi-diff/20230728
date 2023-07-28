# Comparing `tmp/petljapub-2.0.0.tar.gz` & `tmp/petljapub-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petljapub-2.0.0.tar", last modified: Thu Feb  2 09:53:50 2023, max compression
+gzip compressed data, was "petljapub-2.0.1.tar", last modified: Fri Jul 28 19:56:01 2023, max compression
```

## Comparing `petljapub-2.0.0.tar` & `petljapub-2.0.1.tar`

### file list

```diff
@@ -1,78 +1,86 @@
-drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-02-02 09:53:50.261561 petljapub-2.0.0/
--rw-rw-r--   0 filip     (1000) filip     (1000)     1049 2021-08-26 07:51:10.000000 petljapub-2.0.0/LICENCE
--rw-rw-r--   0 filip     (1000) filip     (1000)    65748 2023-02-02 09:53:50.261561 petljapub-2.0.0/PKG-INFO
--rw-rw-r--   0 filip     (1000) filip     (1000)    65252 2023-02-02 09:47:42.000000 petljapub-2.0.0/README.md
--rw-rw-r--   0 filip     (1000) filip     (1000)      104 2021-08-26 07:42:20.000000 petljapub-2.0.0/pyproject.toml
--rw-rw-r--   0 filip     (1000) filip     (1000)       38 2023-02-02 09:53:50.261561 petljapub-2.0.0/setup.cfg
--rw-rw-r--   0 filip     (1000) filip     (1000)     1550 2023-02-02 09:53:40.000000 petljapub-2.0.0/setup.py
-drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-02-02 09:53:50.249560 petljapub-2.0.0/src/
-drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-02-02 09:53:50.257560 petljapub-2.0.0/src/petljapub/
--rw-rw-r--   0 filip     (1000) filip     (1000)        0 2021-08-26 08:36:06.000000 petljapub-2.0.0/src/petljapub/__init__.py
--rw-rw-r--   0 filip     (1000) filip     (1000)      340 2023-01-11 09:36:30.000000 petljapub-2.0.0/src/petljapub/code_parser.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     4169 2022-04-18 16:59:55.000000 petljapub-2.0.0/src/petljapub/compilation.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     1468 2023-01-20 21:26:43.000000 petljapub-2.0.0/src/petljapub/config.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     4163 2023-01-20 21:22:12.000000 petljapub-2.0.0/src/petljapub/configure_compilers.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     1003 2023-01-09 08:48:42.000000 petljapub-2.0.0/src/petljapub/cpp_parser.py
-drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-02-02 09:53:50.257560 petljapub-2.0.0/src/petljapub/data/
-drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-02-02 09:53:50.261561 petljapub-2.0.0/src/petljapub/data/_task_template/
-drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-02-02 09:53:50.261561 petljapub-2.0.0/src/petljapub/data/_task_template/en/
--rw-rw-r--   0 filip     (1000) filip     (1000)      163 2023-01-20 22:05:57.000000 petljapub-2.0.0/src/petljapub/data/_task_template/en/task-sol.md
--rw-rw-r--   0 filip     (1000) filip     (1000)      600 2023-01-20 21:46:16.000000 petljapub-2.0.0/src/petljapub/data/_task_template/en/task-st.md
-drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-02-02 09:53:50.261561 petljapub-2.0.0/src/petljapub/data/_task_template/sr-Cyrl/
--rw-rw-r--   0 filip     (1000) filip     (1000)      221 2023-01-20 22:05:18.000000 petljapub-2.0.0/src/petljapub/data/_task_template/sr-Cyrl/task-sol.md
--rw-rw-r--   0 filip     (1000) filip     (1000)      945 2023-01-20 21:48:04.000000 petljapub-2.0.0/src/petljapub/data/_task_template/sr-Cyrl/task-st.md
-drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-02-02 09:53:50.261561 petljapub-2.0.0/src/petljapub/data/_task_template/sr-Latn/
--rw-rw-r--   0 filip     (1000) filip     (1000)      157 2023-01-20 22:04:48.000000 petljapub-2.0.0/src/petljapub/data/_task_template/sr-Latn/task-sol.md
--rw-rw-r--   0 filip     (1000) filip     (1000)      654 2023-01-20 21:48:31.000000 petljapub-2.0.0/src/petljapub/data/_task_template/sr-Latn/task-st.md
--rw-rw-r--   0 filip     (1000) filip     (1000)      108 2022-05-26 09:03:06.000000 petljapub-2.0.0/src/petljapub/data/_task_template/task-tgen.cpp
--rw-rw-r--   0 filip     (1000) filip     (1000)       72 2021-08-26 09:05:12.000000 petljapub-2.0.0/src/petljapub/data/_task_template/task.cpp
--rw-rw-r--   0 filip     (1000) filip     (1000)       93 2021-08-26 09:05:12.000000 petljapub-2.0.0/src/petljapub/data/_task_template/task.cs
--rw-rw-r--   0 filip     (1000) filip     (1000)        8 2021-11-11 08:11:52.000000 petljapub-2.0.0/src/petljapub/data/_task_template/task.py
--rwxrwxr-x   0 filip     (1000) filip     (1000)     1008 2021-09-17 20:03:35.000000 petljapub-2.0.0/src/petljapub/data/compile-cs.sh
-drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-02-02 09:53:50.261561 petljapub-2.0.0/src/petljapub/data/html/
--rw-rw-r--   0 filip     (1000) filip     (1000)    17623 2023-01-22 15:08:36.000000 petljapub-2.0.0/src/petljapub/data/html/pandoc.css
-drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-02-02 09:53:50.261561 petljapub-2.0.0/src/petljapub/data/md/
--rw-rw-r--   0 filip     (1000) filip     (1000)      928 2023-01-17 12:19:40.000000 petljapub-2.0.0/src/petljapub/data/md/header.md
--rw-rw-r--   0 filip     (1000) filip     (1000)      170 2023-01-21 23:42:08.000000 petljapub-2.0.0/src/petljapub/data/template.yaml
-drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-02-02 09:53:50.261561 petljapub-2.0.0/src/petljapub/data/tex/
--rw-rw-r--   0 filip     (1000) filip     (1000)     8271 2023-01-19 15:30:58.000000 petljapub-2.0.0/src/petljapub/data/tex/default.latex
-drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-02-02 09:53:50.261561 petljapub-2.0.0/src/petljapub/data/tgen/
--rw-rw-r--   0 filip     (1000) filip     (1000)     2300 2021-08-26 11:04:47.000000 petljapub-2.0.0/src/petljapub/data/tgen/tgen-geom.hpp
--rw-rw-r--   0 filip     (1000) filip     (1000)    10168 2022-05-26 09:28:25.000000 petljapub-2.0.0/src/petljapub/data/tgen/tgen-graph.hpp
--rw-rw-r--   0 filip     (1000) filip     (1000)    12132 2022-10-22 08:05:12.000000 petljapub-2.0.0/src/petljapub/data/tgen/tgen.hpp
--rw-rw-r--   0 filip     (1000) filip     (1000)     1444 2022-02-24 21:25:45.000000 petljapub-2.0.0/src/petljapub/default_checker.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     4576 2022-12-13 00:25:03.000000 petljapub-2.0.0/src/petljapub/fix_latex.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     2913 2023-02-01 22:50:40.000000 petljapub-2.0.0/src/petljapub/javascript.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     1408 2022-03-10 10:38:08.000000 petljapub-2.0.0/src/petljapub/logger.py
--rw-rw-r--   0 filip     (1000) filip     (1000)      144 2022-10-16 07:28:50.000000 petljapub-2.0.0/src/petljapub/main.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     7069 2023-02-01 22:57:46.000000 petljapub-2.0.0/src/petljapub/markdown_magic_comments.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     7529 2023-01-12 12:29:21.000000 petljapub-2.0.0/src/petljapub/md_content_processor.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     5936 2023-02-01 23:15:13.000000 petljapub-2.0.0/src/petljapub/md_util.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     3038 2023-02-01 23:25:02.000000 petljapub-2.0.0/src/petljapub/messages.py
--rw-rw-r--   0 filip     (1000) filip     (1000)      888 2021-09-18 19:26:06.000000 petljapub-2.0.0/src/petljapub/plot_times.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     7109 2023-01-13 07:59:24.000000 petljapub-2.0.0/src/petljapub/publication_repository.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     1979 2023-01-07 22:31:37.000000 petljapub-2.0.0/src/petljapub/publication_visitor.py
--rw-rw-r--   0 filip     (1000) filip     (1000)    16707 2023-02-01 22:41:37.000000 petljapub-2.0.0/src/petljapub/publication_visitor_html.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     5522 2023-01-13 07:58:18.000000 petljapub-2.0.0/src/petljapub/publication_visitor_petlja.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     2404 2023-01-07 14:20:39.000000 petljapub-2.0.0/src/petljapub/publication_visitor_testing.py
--rw-rw-r--   0 filip     (1000) filip     (1000)    11487 2023-02-01 23:30:07.000000 petljapub-2.0.0/src/petljapub/publication_visitor_tex.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     1014 2023-01-09 09:21:18.000000 petljapub-2.0.0/src/petljapub/py_parser.py
--rw-rw-r--   0 filip     (1000) filip     (1000)    11093 2023-01-21 21:34:57.000000 petljapub-2.0.0/src/petljapub/serialization.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     3042 2021-08-26 15:29:54.000000 petljapub-2.0.0/src/petljapub/source_code_magic_comments.py
--rw-rw-r--   0 filip     (1000) filip     (1000)    46385 2023-02-02 09:41:43.000000 petljapub-2.0.0/src/petljapub/task.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     2752 2023-01-26 13:02:08.000000 petljapub-2.0.0/src/petljapub/task_repository.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     7028 2023-01-11 09:19:13.000000 petljapub-2.0.0/src/petljapub/task_visitor.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     4209 2023-01-22 00:14:26.000000 petljapub-2.0.0/src/petljapub/task_visitor_html.py
--rw-rw-r--   0 filip     (1000) filip     (1000)    31459 2023-02-02 09:37:56.000000 petljapub-2.0.0/src/petljapub/tasks.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     2893 2021-08-26 08:59:04.000000 petljapub-2.0.0/src/petljapub/translit.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     1005 2022-03-17 20:45:10.000000 petljapub-2.0.0/src/petljapub/util.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     9712 2023-01-21 07:52:28.000000 petljapub-2.0.0/src/petljapub/yaml_specification.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     7550 2021-09-25 18:42:07.000000 petljapub-2.0.0/src/petljapub/yaml_specification_visitor_runtime.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     2470 2021-09-19 22:45:26.000000 petljapub-2.0.0/src/petljapub/yaml_specification_visitor_stats.py
-drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-02-02 09:53:50.257560 petljapub-2.0.0/src/petljapub.egg-info/
--rw-rw-r--   0 filip     (1000) filip     (1000)    65748 2023-02-02 09:53:50.000000 petljapub-2.0.0/src/petljapub.egg-info/PKG-INFO
--rw-rw-r--   0 filip     (1000) filip     (1000)     2176 2023-02-02 09:53:50.000000 petljapub-2.0.0/src/petljapub.egg-info/SOURCES.txt
--rw-rw-r--   0 filip     (1000) filip     (1000)        1 2023-02-02 09:53:50.000000 petljapub-2.0.0/src/petljapub.egg-info/dependency_links.txt
--rw-rw-r--   0 filip     (1000) filip     (1000)       57 2023-02-02 09:53:50.000000 petljapub-2.0.0/src/petljapub.egg-info/entry_points.txt
--rw-rw-r--   0 filip     (1000) filip     (1000)       73 2023-02-02 09:53:50.000000 petljapub-2.0.0/src/petljapub.egg-info/requires.txt
--rw-rw-r--   0 filip     (1000) filip     (1000)       10 2023-02-02 09:53:50.000000 petljapub-2.0.0/src/petljapub.egg-info/top_level.txt
+drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 19:56:01.521755 petljapub-2.0.1/
+-rw-rw-r--   0 filip     (1000) filip     (1000)     1049 2021-08-26 07:51:10.000000 petljapub-2.0.1/LICENCE
+-rw-rw-r--   0 filip     (1000) filip     (1000)    65748 2023-07-28 19:56:01.521755 petljapub-2.0.1/PKG-INFO
+-rw-rw-r--   0 filip     (1000) filip     (1000)    65252 2023-02-02 09:47:42.000000 petljapub-2.0.1/README.md
+-rw-rw-r--   0 filip     (1000) filip     (1000)      104 2021-08-26 07:42:20.000000 petljapub-2.0.1/pyproject.toml
+-rw-rw-r--   0 filip     (1000) filip     (1000)       38 2023-07-28 19:56:01.521755 petljapub-2.0.1/setup.cfg
+-rw-rw-r--   0 filip     (1000) filip     (1000)     1588 2023-07-28 19:55:57.000000 petljapub-2.0.1/setup.py
+drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 19:56:01.509754 petljapub-2.0.1/src/
+drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 19:56:01.517754 petljapub-2.0.1/src/petljapub/
+-rw-rw-r--   0 filip     (1000) filip     (1000)        0 2021-08-26 08:36:06.000000 petljapub-2.0.1/src/petljapub/__init__.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)      355 2023-06-01 11:21:35.000000 petljapub-2.0.1/src/petljapub/code_parser.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     4180 2023-02-03 15:10:49.000000 petljapub-2.0.1/src/petljapub/compilation.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     1468 2023-01-20 21:26:43.000000 petljapub-2.0.1/src/petljapub/config.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     4163 2023-01-20 21:22:12.000000 petljapub-2.0.1/src/petljapub/configure_compilers.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     1967 2023-06-01 11:19:46.000000 petljapub-2.0.1/src/petljapub/cpp_parser.py
+drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 19:56:01.517754 petljapub-2.0.1/src/petljapub/data/
+drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 19:56:01.521755 petljapub-2.0.1/src/petljapub/data/_task_template/
+drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 19:56:01.521755 petljapub-2.0.1/src/petljapub/data/_task_template/en/
+-rw-rw-r--   0 filip     (1000) filip     (1000)      163 2023-01-20 22:05:57.000000 petljapub-2.0.1/src/petljapub/data/_task_template/en/task-sol.md
+-rw-rw-r--   0 filip     (1000) filip     (1000)      600 2023-01-20 21:46:16.000000 petljapub-2.0.1/src/petljapub/data/_task_template/en/task-st.md
+drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 19:56:01.521755 petljapub-2.0.1/src/petljapub/data/_task_template/sr-Cyrl/
+-rw-rw-r--   0 filip     (1000) filip     (1000)      221 2023-01-20 22:05:18.000000 petljapub-2.0.1/src/petljapub/data/_task_template/sr-Cyrl/task-sol.md
+-rw-rw-r--   0 filip     (1000) filip     (1000)      945 2023-01-20 21:48:04.000000 petljapub-2.0.1/src/petljapub/data/_task_template/sr-Cyrl/task-st.md
+drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 19:56:01.521755 petljapub-2.0.1/src/petljapub/data/_task_template/sr-Latn/
+-rw-rw-r--   0 filip     (1000) filip     (1000)      157 2023-01-20 22:04:48.000000 petljapub-2.0.1/src/petljapub/data/_task_template/sr-Latn/task-sol.md
+-rw-rw-r--   0 filip     (1000) filip     (1000)      654 2023-01-20 21:48:31.000000 petljapub-2.0.1/src/petljapub/data/_task_template/sr-Latn/task-st.md
+-rw-rw-r--   0 filip     (1000) filip     (1000)      108 2022-05-26 09:03:06.000000 petljapub-2.0.1/src/petljapub/data/_task_template/task-tgen.cpp
+-rw-rw-r--   0 filip     (1000) filip     (1000)       72 2021-08-26 09:05:12.000000 petljapub-2.0.1/src/petljapub/data/_task_template/task.cpp
+-rw-rw-r--   0 filip     (1000) filip     (1000)       93 2021-08-26 09:05:12.000000 petljapub-2.0.1/src/petljapub/data/_task_template/task.cs
+-rw-rw-r--   0 filip     (1000) filip     (1000)        8 2021-11-11 08:11:52.000000 petljapub-2.0.1/src/petljapub/data/_task_template/task.py
+-rwxrwxr-x   0 filip     (1000) filip     (1000)     1008 2021-09-17 20:03:35.000000 petljapub-2.0.1/src/petljapub/data/compile-cs.sh
+drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 19:56:01.521755 petljapub-2.0.1/src/petljapub/data/html/
+-rw-rw-r--   0 filip     (1000) filip     (1000)    18217 2023-02-05 17:07:03.000000 petljapub-2.0.1/src/petljapub/data/html/pandoc.css
+drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 19:56:01.521755 petljapub-2.0.1/src/petljapub/data/md/
+-rw-rw-r--   0 filip     (1000) filip     (1000)      928 2023-01-17 12:19:40.000000 petljapub-2.0.1/src/petljapub/data/md/header.md
+-rw-rw-r--   0 filip     (1000) filip     (1000)      170 2023-01-21 23:42:08.000000 petljapub-2.0.1/src/petljapub/data/template.yaml
+drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 19:56:01.521755 petljapub-2.0.1/src/petljapub/data/tex/
+-rw-rw-r--   0 filip     (1000) filip     (1000)     8271 2023-01-19 15:30:58.000000 petljapub-2.0.1/src/petljapub/data/tex/default.latex
+drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 19:56:01.521755 petljapub-2.0.1/src/petljapub/data/tgen/
+-rw-rw-r--   0 filip     (1000) filip     (1000)     2300 2021-08-26 11:04:47.000000 petljapub-2.0.1/src/petljapub/data/tgen/tgen-geom.hpp
+-rw-rw-r--   0 filip     (1000) filip     (1000)    10168 2022-05-26 09:28:25.000000 petljapub-2.0.1/src/petljapub/data/tgen/tgen-graph.hpp
+-rw-rw-r--   0 filip     (1000) filip     (1000)    12132 2022-10-22 08:05:12.000000 petljapub-2.0.1/src/petljapub/data/tgen/tgen.hpp
+-rw-rw-r--   0 filip     (1000) filip     (1000)     1444 2022-02-24 21:25:45.000000 petljapub-2.0.1/src/petljapub/default_checker.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     4576 2022-12-13 00:25:03.000000 petljapub-2.0.1/src/petljapub/fix_latex.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     3584 2023-02-05 17:07:29.000000 petljapub-2.0.1/src/petljapub/javascript.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     1408 2022-03-10 10:38:08.000000 petljapub-2.0.1/src/petljapub/logger.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)      144 2022-10-16 07:28:50.000000 petljapub-2.0.1/src/petljapub/main.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     7069 2023-02-01 22:57:46.000000 petljapub-2.0.1/src/petljapub/markdown_magic_comments.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     7529 2023-01-12 12:29:21.000000 petljapub-2.0.1/src/petljapub/md_content_processor.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     5954 2023-05-19 15:10:00.000000 petljapub-2.0.1/src/petljapub/md_util.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     3171 2023-07-27 08:23:50.000000 petljapub-2.0.1/src/petljapub/messages.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)      888 2021-09-18 19:26:06.000000 petljapub-2.0.1/src/petljapub/plot_times.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     7109 2023-01-13 07:59:24.000000 petljapub-2.0.1/src/petljapub/publication_repository.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     1979 2023-01-07 22:31:37.000000 petljapub-2.0.1/src/petljapub/publication_visitor.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)    17276 2023-05-26 09:05:32.000000 petljapub-2.0.1/src/petljapub/publication_visitor_html.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     5522 2023-01-13 07:58:18.000000 petljapub-2.0.1/src/petljapub/publication_visitor_petlja.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     2404 2023-01-07 14:20:39.000000 petljapub-2.0.1/src/petljapub/publication_visitor_testing.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)    11733 2023-05-26 09:04:51.000000 petljapub-2.0.1/src/petljapub/publication_visitor_tex.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     1072 2023-02-03 20:21:18.000000 petljapub-2.0.1/src/petljapub/py_parser.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)    11205 2023-07-27 08:25:09.000000 petljapub-2.0.1/src/petljapub/serialization.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     3042 2021-08-26 15:29:54.000000 petljapub-2.0.1/src/petljapub/source_code_magic_comments.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)    46615 2023-05-26 09:01:06.000000 petljapub-2.0.1/src/petljapub/task.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     2752 2023-01-26 13:02:08.000000 petljapub-2.0.1/src/petljapub/task_repository.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     7519 2023-06-27 11:13:15.000000 petljapub-2.0.1/src/petljapub/task_visitor.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     4209 2023-01-22 00:14:26.000000 petljapub-2.0.1/src/petljapub/task_visitor_html.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)    31490 2023-03-02 11:37:38.000000 petljapub-2.0.1/src/petljapub/tasks.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     2893 2021-08-26 08:59:04.000000 petljapub-2.0.1/src/petljapub/translit.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     1005 2022-03-17 20:45:10.000000 petljapub-2.0.1/src/petljapub/util.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     9712 2023-01-21 07:52:28.000000 petljapub-2.0.1/src/petljapub/yaml_specification.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     7550 2021-09-25 18:42:07.000000 petljapub-2.0.1/src/petljapub/yaml_specification_visitor_runtime.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     2470 2021-09-19 22:45:26.000000 petljapub-2.0.1/src/petljapub/yaml_specification_visitor_stats.py
+drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 19:56:01.517754 petljapub-2.0.1/src/petljapub.egg-info/
+-rw-rw-r--   0 filip     (1000) filip     (1000)    65748 2023-07-28 19:56:01.000000 petljapub-2.0.1/src/petljapub.egg-info/PKG-INFO
+-rw-rw-r--   0 filip     (1000) filip     (1000)     2372 2023-07-28 19:56:01.000000 petljapub-2.0.1/src/petljapub.egg-info/SOURCES.txt
+-rw-rw-r--   0 filip     (1000) filip     (1000)        1 2023-07-28 19:56:01.000000 petljapub-2.0.1/src/petljapub.egg-info/dependency_links.txt
+-rw-rw-r--   0 filip     (1000) filip     (1000)       57 2023-07-28 19:56:01.000000 petljapub-2.0.1/src/petljapub.egg-info/entry_points.txt
+-rw-rw-r--   0 filip     (1000) filip     (1000)      104 2023-07-28 19:56:01.000000 petljapub-2.0.1/src/petljapub.egg-info/requires.txt
+-rw-rw-r--   0 filip     (1000) filip     (1000)       10 2023-07-28 19:56:01.000000 petljapub-2.0.1/src/petljapub.egg-info/top_level.txt
+drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 19:56:01.521755 petljapub-2.0.1/tests/
+-rw-rw-r--   0 filip     (1000) filip     (1000)     5257 2023-01-22 14:22:00.000000 petljapub-2.0.1/tests/test_markdown_magic_comments.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     5075 2023-01-15 08:31:48.000000 petljapub-2.0.1/tests/test_md_content_processor.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     5947 2023-02-06 08:18:43.000000 petljapub-2.0.1/tests/test_md_util.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)      439 2023-01-21 20:08:18.000000 petljapub-2.0.1/tests/test_messages.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     3129 2023-02-06 08:14:26.000000 petljapub-2.0.1/tests/test_parsers.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     1937 2022-10-31 17:05:01.000000 petljapub-2.0.1/tests/test_publication_repository.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     6991 2023-02-03 13:51:21.000000 petljapub-2.0.1/tests/test_task.py
```

### Comparing `petljapub-2.0.0/LICENCE` & `petljapub-2.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.0/PKG-INFO` & `petljapub-2.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: petljapub
-Version: 2.0.0
-Summary: Petlja publishing system
-Home-page: https://github.com/pypa/petljapub
-Author: Filip Maric, Petlja
-Author-email: filip.maric@petlja.org
-Project-URL: Bug Tracker, https://github.com/pypa/petljapub/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
 # PetljaPub - систем за дигиталне публикације из програмирања
 
 Систем *PetljaPub* служи за креирање збирки задатака, уџбеника и
 других едукативних материјала за учење програмирања. Решења задатака
 се могу писати на различитим програмским језицима и омогућено је
 њихово превођење, покретање и аутоматско тестирање пре укључивања у
 публикацију (збирку или уџбеник). Публикације се граде укључивањем
```

### Comparing `petljapub-2.0.0/README.md` & `petljapub-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: petljapub
+Version: 2.0.1
+Summary: Petlja publishing system
+Home-page: https://github.com/pypa/petljapub
+Author: Filip Maric, Petlja
+Author-email: filip.maric@petlja.org
+Project-URL: Bug Tracker, https://github.com/pypa/petljapub/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENCE
+
 # PetljaPub - систем за дигиталне публикације из програмирања
 
 Систем *PetljaPub* служи за креирање збирки задатака, уџбеника и
 других едукативних материјала за учење програмирања. Решења задатака
 се могу писати на различитим програмским језицима и омогућено је
 њихово превођење, покретање и аутоматско тестирање пре укључивања у
 публикацију (збирку или уџбеник). Публикације се граде укључивањем
```

### Comparing `petljapub-2.0.0/setup.py` & `petljapub-2.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="petljapub",
-    version="2.0.0",
+    version="2.0.1",
     author="Filip Maric, Petlja",
     author_email="filip.maric@petlja.org",
     description="Petlja publishing system",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/petljapub",
     project_urls={
@@ -19,15 +19,15 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.7",
-    install_requires=['invoke', 'pyyaml', 'pypandoc', 'pandoc-xnos', 'pandoc-fignos', 'appdirs', 'matplotlib>=3.4'],
+    install_requires=['invoke', 'pyyaml', 'pypandoc', 'pandoc-xnos', 'pandoc-fignos',  'pandoc-eqnos', 'pandoc-theoremnos', 'appdirs', 'matplotlib>=3.4'],
     entry_points={
         'console_scripts': ['petljapub = petljapub.main:program.run']
     },
     package_data={"petljapub": ["data/_task_template/*",
                                 "data/_task_template/en/*",
                                 "data/_task_template/sr-Cyrl/*",
                                 "data/_task_template/sr-Latn/*",
```

### Comparing `petljapub-2.0.0/src/petljapub/compilation.py` & `petljapub-2.0.1/src/petljapub/compilation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os, sys
+import os, sys, traceback
 import subprocess
 from petljapub.config import read_config
 from . import logger
 
 # we expect that all custom compilation scripts reside in the data directory of petljapub
 
 base_dir = os.path.dirname(os.path.abspath(__file__))
```

### Comparing `petljapub-2.0.0/src/petljapub/config.py` & `petljapub-2.0.1/src/petljapub/config.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.0/src/petljapub/configure_compilers.py` & `petljapub-2.0.1/src/petljapub/configure_compilers.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.0/src/petljapub/cpp_parser.py` & `petljapub-2.0.1/src/petljapub/py_parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 import re
 
 def is_fun_declaration(line, fun_id):
-    type_re = r"[a-z*&]+"
     id_re = r"[a-z_][a-z0-9_]*"
-    param_re = r"({}\s+{})*".format(type_re, id_re)
-    declaration_re = r"{}\s+{}(\(\)|\({}(\s*,\s*{})*\))\s*{{?".format(type_re, fun_id, param_re, param_re)
+    declaration_re = r"\s*def\s+{}\s*(\(\s*\)|\(\s*{}\s*(,\s*{})*\s*\))\s*:\s*".format(id_re, id_re, id_re)
     return bool(re.match(declaration_re, line, re.IGNORECASE))    
+    
 
-def extract_fun(cpp, fun_id):
+# FIXME: works only for function declarations in one line
+def extract_fun(py, fun_id):
+
+    def empty(s):
+        return s.strip() == ""
+
+    def count_spaces(s):
+        return len(s) - len(s.lstrip())
+    
     in_declaration = False
     result = []
-    for line in cpp.split("\n"):
+    for line in py.split("\n"):
         if is_fun_declaration(line, fun_id):
             in_declaration = True
+            leading_spaces = count_spaces(line)
             result.append(line)
-            num_braces = line.count("{")
         else:
             if in_declaration:
-                result.append(line)
-                for c in line:
-                    if c == "{":
-                        num_braces += 1
-                    elif c == "}":
-                        num_braces -= 1
-                if num_braces == 0:
+                if not empty(line) and count_spaces(line) <= leading_spaces:
                     in_declaration = False
+                    while empty(result[-1]):
+                        result.pop()
                     return "\n".join(result)
+                else:
+                    result.append(line)
     return ""
-
```

### Comparing `petljapub-2.0.0/src/petljapub/data/_task_template/en/task-st.md` & `petljapub-2.0.1/src/petljapub/data/_task_template/en/task-st.md`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.0/src/petljapub/data/_task_template/sr-Cyrl/task-st.md` & `petljapub-2.0.1/src/petljapub/data/_task_template/sr-Cyrl/task-st.md`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.0/src/petljapub/data/_task_template/sr-Latn/task-st.md` & `petljapub-2.0.1/src/petljapub/data/_task_template/sr-Latn/task-st.md`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.0/src/petljapub/data/compile-cs.sh` & `petljapub-2.0.1/src/petljapub/data/compile-cs.sh`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.0/src/petljapub/data/html/pandoc.css` & `petljapub-2.0.1/src/petljapub/data/html/pandoc.css`

 * *Files 3% similar despite different names*

```diff
@@ -974,8 +974,44 @@
 }
 
 div.abc p {
     margin: 0px
 }
 
 
+.popupbg {
+    margin: 0px;
+    width: 100%;
+    height: 100%;
+    position: fixed;
+    top: 0px;
+    left: 0px;
+    background-color: rgba(0, 0, 0, 0.6);
+    z-index: 1000;
+    visibility: hidden;
+}
+
+.popupclose{
+    text-align: right;
+    font-size: 20px;
+    background-color: white;
+    margin-top: 30px;
+    margin-left: 50px;
+    margin-right: 50px;
+    margin-bottom: 0px;
+    border: 1px solid white;
+}
+
+.popupclose p {
+    margin: 0
+}
+
+.popup {
+    background-color: white;
+    z-index: 1001;
+    margin-top: 0px;
+    margin-left: 50px;
+    margin-right: 50px;
+    height: 85%;
+}
+    
 </style>
```

### Comparing `petljapub-2.0.0/src/petljapub/data/md/header.md` & `petljapub-2.0.1/src/petljapub/data/md/header.md`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.0/src/petljapub/data/tex/default.latex` & `petljapub-2.0.1/src/petljapub/data/tex/default.latex`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.0/src/petljapub/data/tgen/tgen-geom.hpp` & `petljapub-2.0.1/src/petljapub/data/tgen/tgen-geom.hpp`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.0/src/petljapub/data/tgen/tgen-graph.hpp` & `petljapub-2.0.1/src/petljapub/data/tgen/tgen-graph.hpp`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.0/src/petljapub/data/tgen/tgen.hpp` & `petljapub-2.0.1/src/petljapub/data/tgen/tgen.hpp`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.0/src/petljapub/default_checker.py` & `petljapub-2.0.1/src/petljapub/default_checker.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.0/src/petljapub/fix_latex.py` & `petljapub-2.0.1/src/petljapub/fix_latex.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.0/src/petljapub/javascript.py` & `petljapub-2.0.1/src/petljapub/javascript.py`

 * *Files 25% similar despite different names*

```diff
@@ -69,7 +69,30 @@
 def iframe(file_name, title="", height=500):
     if title == None:
         title = ""
     if height == None:
         height = 500
     return "<iframe src='{}' title='{}' style='width: 100%; height: {}px' frameBorder='0'></iframe>".format(file_name, title, height)
 
+
+def popup(button, content, popup_id=0):
+    code = """\n\n<button id='showPopup{}'>{}</button>
+
+<div id='popup{}' class='popupbg'>
+<div class='popupclose'>
+<span id='closePopup{}'>✖</span>
+</div>
+<div class='popup'>
+{}
+</div>
+</div>
+
+<script>
+document.getElementById('showPopup{}').addEventListener("click", function() {{
+  document.getElementById("popup{}").style.visibility="visible";
+}});
+document.getElementById('closePopup{}').addEventListener("click", function() {{
+ document.getElementById("popup{}").style.visibility="hidden";
+}});
+</script>"""
+    
+    return code.format(popup_id, button, popup_id, popup_id, content, popup_id, popup_id, popup_id, popup_id)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -15,8 +15,12 @@
 {}
 {}
 [Unknown INPUT type]
  """ return div.format(question_id, spec["question"], "\n".join(options), msg
 ("CHECK"), question_id, question_id, question_id, question_id, question_id,
 spec["correct"]) def iframe(file_name, title="", height=500): if title == None:
 title = "" if height == None: height = 500 return "".format(file_name, title,
-height)
+height) def popup(button, content, popup_id=0): code = """\n\n{}
+â
+{}
+""" return code.format(popup_id, button, popup_id, popup_id, content, popup_id,
+popup_id, popup_id, popup_id)
```

### Comparing `petljapub-2.0.0/src/petljapub/logger.py` & `petljapub-2.0.1/src/petljapub/logger.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.0/src/petljapub/markdown_magic_comments.py` & `petljapub-2.0.1/src/petljapub/markdown_magic_comments.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.0/src/petljapub/md_content_processor.py` & `petljapub-2.0.1/src/petljapub/md_content_processor.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.0/src/petljapub/md_util.py` & `petljapub-2.0.1/src/petljapub/md_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,17 +156,17 @@
     # fix latex $ signs in accordance with Pandoc Markdown dialect
     @staticmethod
     def fix_latex_dollars(md):
         # replace $$ by $ for inline maths
         md = re.sub(r"\$\$", "$", md)
         # put $$ around displayed maths
         # single displayed line
-        md = re.sub(r"\n\n[ \t]*\$(.+)\$[ \t]*(\n\n|\n\Z|\Z)", r"\n\n$$\1$$\n\n", md)
+        md = re.sub(r"\n\n\s*\$(.+)\$([ \t]*{.+})?\s*(\n\n|\n\Z|\Z)", r"\n\n$$\1$$\2\n\n", md)
         # multiple displayed lines
-        md = re.sub(r"\n\n[ \t]*\$([^$]+)\$[ \t]*(\n\n|\n\Z|\Z)", r"\n\n$$\1$$\n\n", md)
+        md = re.sub(r"\n\n\s*\$([^$]+)\$([ \t]*{.+})?\s*(\n\n|\n\Z|\Z)", r"\n\n$$\1$$\2\n\n", md)
         return md
 
     # fix indentation of itemized lists in accordance with Pandoc
     # Markdown dialect
     @staticmethod
     def fix_itemize(md):
         return re.sub(r"^-(?!(\d|\n|[-]))", "  -", md)
```

### Comparing `petljapub-2.0.0/src/petljapub/messages.py` & `petljapub-2.0.1/src/petljapub/messages.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,17 @@
     "TRY_TO_SOLVE"  : "Try to solve the task using techniques described in this section.",
     "LOOKUP_TASK"   : "Show the task statement.",
     "ADDITIONAL_SOLUTIONS" : "See different solutions of this task.",
     "ADDITIONAL_SOLUTIONS_EXIST" : "This task has multiple solutions.",
     "FIGURE" : "Figure",
     "CHECK": "Check",
     "QUESTION": "Question",
-    "ANSWERS": "Answers"
+    "ANSWERS": "Answers",
+    "SHOW_APPLET": "Show applet",
+    "TABLE": "Table"
 }
 
 srCyrl = {
     "TASK"         : "Задатак",
     "TASKS"        : "Задаци",
     "STATEMENT"    : "Поставка",
     "SOLUTION"     : "Решење",
@@ -41,15 +43,17 @@
     "TRY_TO_SOLVE"  : "Покушај да задатак урадиш коришћењем техника које се излажу у овом поглављу.",
     "LOOKUP_TASK"   : "Види текст задатка.",
     "ADDITIONAL_SOLUTIONS" : "Види другачија решења овог задатка.",
     "ADDITIONAL_SOLUTIONS_EXIST" : "Овај задатак има и другачија решења у делу збирке који следи.",
     "FIGURE" : "Слика",
     "CHECK": "Провери",
     "QUESTION": "Питање",
-    "ANSWERS": "Одговори"
+    "ANSWERS": "Одговори",
+    "SHOW_APPLET": "Прикажи аплет",
+    "TABLE": "Табела"
 }
 
 srLatn = {key : cyr_to_lat(value) for key, value in srCyrl.items()}
 
 languages = {
     "en" : en,
     "sr" : srLatn,
```

### Comparing `petljapub-2.0.0/src/petljapub/plot_times.py` & `petljapub-2.0.1/src/petljapub/plot_times.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.0/src/petljapub/publication_repository.py` & `petljapub-2.0.1/src/petljapub/publication_repository.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.0/src/petljapub/publication_visitor.py` & `petljapub-2.0.1/src/petljapub/publication_visitor.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.0/src/petljapub/publication_visitor_html.py` & `petljapub-2.0.1/src/petljapub/publication_visitor_html.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,16 @@
             
         # remember parameters
         self._join_langs = join_langs
         self._standalone = standalone
 
         # javascript language switcher id
         self._switcher_id = 0
+        # javascript popup id
+        self._popup_id = 0
 
         # tasks are not inline by default
         self._inline_task = False
 
         # dictionary that maps section paths to section titles (read from index.md files)
         self._section_titles = {}
 
@@ -123,15 +125,15 @@
 
         # process included tasks
         def include_task(task_spec_lines):
             self._inline_task = True
             task_spec = yaml.safe_load("\n".join(task_spec_lines))
             task_result = self.task(section_path, level, task_spec["id"], task_spec)
             self._inline_task = False
-            return task_result
+            return task_result if task_result != None else ""
         md = markdown_magic_comments.replace_magic_comment_directives(md, "task", include_task)
 
         # process multichoice (abc) questions
         def process_abc(abc_spec_lines):
             abc_spec = yaml.safe_load("\n".join(abc_spec_lines))
             process_abc.question_id += 1
             return javascript.abc_question(abc_spec, process_abc.question_id)
@@ -159,17 +161,23 @@
                     copy(javascript_spec["extra"])
                 else:
                     for file_name in javascript_spec["extra"]:
                         copy(file_name)
 
             height = int(javascript_spec["height"]) if "height" in javascript_spec else None
             title = javascript_spec["title"] if "title" in javascript_spec else ""
-            return javascript.iframe(javascript_spec["src"], title=title, height=height)
+            iframe = javascript.iframe(javascript_spec["src"], title=title, height=height)
+            if "popup" in javascript_spec:
+                self._popup_id += 1
+                return javascript.popup(msg("SHOW_APPLET"), iframe, self._popup_id)
+            else:
+                return iframe
+            
         md = markdown_magic_comments.replace_magic_comment_directives(md, "javascript", process_javascript)
-        
+
         return title, md
 
     def create_toc(self, section_path, md_files, subsections, tasks):
         md = ""
 
         def link_target(path):
             target_path = self._md_serializer.path(path)
@@ -249,15 +257,22 @@
             self._st_md += md_util.italic(msg("REPEATED_TASK")) + "\n\n"
             
         # append the statement content, read from the task repository
         self._st_md += task.statement() + "\n\n"
         # process obtained md
         self._st_md = self._md_processor.process(self.task_output_dir(task.id()), task.st_path(), self._st_md)
 
-    def task_io(self, task):
+    def task_io(self, task, description=True, examples=True):
+        # read input-output specification
+        if description and examples:
+            md = task.io()
+        elif description:
+            md = task.io_description()
+        elif examples:
+            md = task.io_examples()
         # append it to the statement md
         self._st_md += task.io()
         # process obtained md
         self._st_md = self._md_processor.process(self.task_output_dir(task.id()), task.st_path(), self._st_md)        
 
     def task_end_st(self, task):
         # append the link to the solution
```

### Comparing `petljapub-2.0.0/src/petljapub/publication_visitor_petlja.py` & `petljapub-2.0.1/src/petljapub/publication_visitor_petlja.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.0/src/petljapub/publication_visitor_testing.py` & `petljapub-2.0.1/src/petljapub/publication_visitor_testing.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.0/src/petljapub/publication_visitor_tex.py` & `petljapub-2.0.1/src/petljapub/publication_visitor_tex.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         # process the content
         md = self.process(section_path, md_file_path, md, level, self._langs, unnumbered=unnumbered)
 
         # process included tasks
         def include_task(task_spec_lines):
             task_spec = yaml.safe_load("\n".join(task_spec_lines))
             task_result = self.task(section_path, level + 1, task_spec["id"], task_spec)
-            return task_result
+            return task_result if task_result != None else ""
         self._inline_task = True
         md = markdown_magic_comments.replace_magic_comment_directives(md, "task", include_task)
         self._inline_task = False
 
 
         # process multichoice (abc) questions
         def process_abc(abc_spec_lines):
@@ -165,30 +165,35 @@
                                       md_util.link(msg("LOOKUP_TASK"), "#" + task.id()),
                                       md_util.italic(msg("TRY_TO_SOLVE")))
 
         # append content to the resulting string
         self._task_md += md + "\n\n"
 
 
-    def task_io(self, task):
+    def task_io(self, task, description=True, examples=True):
         # inner headings are collapsed to save space
         def format_inner_headings(text):
             # collapse inner headings
             text = md_util.remove_headings(text, 2, "**")
             text = md_util.remove_headings(text, 3, "*")
             # remove blank lines behind inner headings so that they
             # are printed in the same line with the rest of the text (to save space)
             for m in (msg("INPUT"), msg("OUTPUT")):
                 text = md_util.keep_with_next(text, md_util.bold(m))
             return text
         
         current_occurrence = self._extra_info["current_occurrence"]
         if current_occurrence == 1:
-            # read full input-output description
-            md = task.io()
+            # read input-output specification
+            if description and examples:
+                md = task.io()
+            elif description:
+                md = task.io_description()
+            elif examples:
+                md = task.io_examples()
             # format inner headings
             md = format_inner_headings(md)
             # process the content
             md = self.process(self._extra_info["section_path"], task.st_path(), md, self._extra_info["level"], self._langs)
 
             # append content to the resulting string
             self._task_md += md + "\n\n"
```

### Comparing `petljapub-2.0.0/src/petljapub/serialization.py` & `petljapub-2.0.1/src/petljapub/serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,15 +211,15 @@
         html = re.sub(r"<pre>\s*<code>(((?!<code).)*)</code>\s*</pre>", r"<pre><div class='verbatim-text'>\1</div></pre>", html, 0, re.DOTALL)
         return html
 
     # conversion of Markdown to HTML (via pypandoc)
     def md_to_html(self, md, title):
         if not check_pandoc():
             return "Pandoc is not properly configured"
-        
+
         # for mathematical formulae and cross referencing filter (pandoc-xnos)
         extra_args = ['--eol=lf', '--mathjax=https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-MML-AM_CHTML', '--filter=pandoc-xnos']
         # generate standalone HTML files (with HTML header and footer)
         if self._standalone:
             extra_args.append('--standalone')
         # apply the given stylesheet
         if self._css:
@@ -227,14 +227,16 @@
             extra_args.append(self._css)
         # set language
         if self._babel:
             extra_args.append('-V')
             extra_args.append('lang=' + self._babel)
             extra_args.append('-M')
             extra_args.append('fignos-caption-name=' + msg("FIGURE", self._babel))
+            extra_args.append('-M')
+            extra_args.append('tablenos-caption-name=' + msg("TABLE", self._babel))
         # set title
         if title:
             extra_args.append('-M')
             extra_args.append('pagetitle=' + title)
             
         # do the conversion
         logger.info("convert md to html", extra_args, verbosity=5)
```

### Comparing `petljapub-2.0.0/src/petljapub/source_code_magic_comments.py` & `petljapub-2.0.1/src/petljapub/source_code_magic_comments.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.0/src/petljapub/task.py` & `petljapub-2.0.1/src/petljapub/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,19 +240,28 @@
         return parser.output_description()
 
     # examples of input and output
     def examples(self, strip_md_verbatim=False):
         parser = StParser(self.st_content())
         return parser.examples(strip_md_verbatim)
 
-    # complete IO description
+    # complete IO specification (description + examples)
     def io(self):
+        return self.io_description() + self.io_examples()
+        
+    # IO description
+    def io_description(self):
         md = ""
         md += md_util.heading(msg("INPUT_DESC"), 2) + "\n\n" + self.input_description() + "\n\n"
         md += md_util.heading(msg("OUTPUT_DESC"), 2) + "\n\n" + self.output_description() + "\n\n"
+        return md
+
+    # IO examples
+    def io_examples(self):
+        md = ""
         examples = self.examples()
         for i, example in enumerate(examples):
             example_num = " " + str(i+1) if len(examples) > 1 else ""
             md += md_util.heading(msg("EXAMPLE"), 2) + example_num + "\n\n"
             md += md_util.heading(msg("INPUT"), 3) + "\n\n" + example["input"] + "\n\n"
             md += md_util.heading(msg("OUTPUT"), 3) + "\n\n" +example["output"] + "\n\n"
             if example["explanation"]:
@@ -309,15 +318,15 @@
         testcases = os.path.join(self.crafted_testcases_dir() , "*.in")
         return sorted(glob.glob(testcases))
     
     # return the number of crafted testcases
     def number_of_crafted_testcases(self):
         return len(self.crafted_testcases())
 
-    #the list of all testcase paths
+    # the list of all testcase paths
     def all_testcases(self):
         return self.example_testcases() + self.generated_testcases() + self.crafted_testcases()
     
 
     # generate yaml description of testcases
     def scoring_yaml(self, subtask=False):
         ex = self.number_of_example_testcases()
@@ -623,15 +632,15 @@
             return
 
         with open(tgen_src) as tgen:
             content = tgen.read()
             if re.search(r"void gen_test\([^)]*\)\s*{\s*}", content):
                 logger.warn(tgen_src + " - gen_test function is empty - generating testcases skipped")
                 return
-        
+            
         if not compile_cpp(tgen_src, tgen_exe):
             logger.error("compiling test generator failed")
             return False
 
         # compile the main solution used to generate outputs
         if not self.compile("ex0", "cpp", force=True):
             logger.error("compiling main solution failed")
```

### Comparing `petljapub-2.0.0/src/petljapub/task_repository.py` & `petljapub-2.0.1/src/petljapub/task_repository.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.0/src/petljapub/task_visitor.py` & `petljapub-2.0.1/src/petljapub/task_visitor.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,40 +24,47 @@
         # a hook called when the processing of the task is started
         # (the hook is defined by subclasses)
         self.task_start(task)
         
         # determine what components to print - if it is not specified
         # in the task specification, everything is processed
         print_spec = task_spec.get("print", "full")
-        self._what_to_print = {
-            "full": ["statement", "io", "solution", "source"],
-            "solution": ["statement", "io", "solution"],
-            "statement": ["statement", "io"],
-            "code": ["source"],
-            "exclude": []
-        }[print_spec]
+        if type(print_spec) == list:
+            self._what_to_print = print_spec
+        else:
+            self._what_to_print = {
+                "full": ["statement", "io-description", "io-examples", "solution", "source"],
+                "solution": ["statement", "io-description", "io-examples", "solution"],
+                "statement": ["statement", "io-description", "io-examples"],
+                "code": ["source"],
+                "exclude": []
+            }[print_spec]
 
         # do not print input output specification if requested by the user
         if task_spec.get("no-io", False):
             if "io" in self._what_to_print:
-                self._what_to_print.remove("io") 
+                self._what_to_print.remove("io-description") 
+                self._what_to_print.remove("io-examples") 
 
         # print the task title (if not requested otherwise)
         if not task_spec.get("no-title", False):
             self.task_title(task)
 
         # if the task statement should be processed
         if "statement" in self._what_to_print:
             # the hook (defined in subclasses) is called
             self.task_st(task)
 
         # if taks input-output description and examples should be processed
-        if "io" in self._what_to_print:
+        if "io-description" in self._what_to_print or "io-examples" in self._what_to_print:
             # the hook (defined in subclasses) is called
-            self.task_io(task)
+            self.task_io(task,
+                         description="io-description" in self._what_to_print,
+                         examples="io-examples" in self._what_to_print)
+            
 
         # finish processing the statement
         if "statement" in self._what_to_print:
             self.task_end_st(task)
     
         # if task solutions should be processed
         if "solution" in self._what_to_print:
```

### Comparing `petljapub-2.0.0/src/petljapub/task_visitor_html.py` & `petljapub-2.0.1/src/petljapub/task_visitor_html.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.0/src/petljapub/tasks.py` & `petljapub-2.0.1/src/petljapub/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,32 +285,32 @@
         task.prepare_crafted_testcases(crafted_dir)
     
     zip_file = os.path.join(task.build_dir(), "testcases.zip")
     writer = ZipWriter(zip_file)
     writer.open()
 
     i = 1
-    for testcase_in in (task.example_testcases() + task.crafted_testcases() + task.generated_testcases()):
+    for testcase_in in (task.example_testcases() + task.generated_testcases() + task.crafted_testcases()):
         logger.info(testcase_in)
         writer.copy_file(testcase_in, "{:02d}.in".format(i))
         testcase_out = testcase_in[0:-2] + "out"
         logger.info(testcase_out)
         writer.copy_file(testcase_out, "{:02d}.out".format(i))
         i += 1
     writer.close()
     logger.info("Testcases stored in", zip_file)
 
 @task
-def tz(ctx):
+def tz(ctx, crafted_dir=None):
     """
     Generate zip with all testcases for the current task (shortcut for 'petljapub tests-zip')
 
     """
 
-    tests_zip(ctx)
+    tests_zip(ctx, crafted_dir)
     
 @task
 def compile_checker(ctx):
     """
     Compile custom checker (if exists)
     """
     if not ensure_task_dir():
```

### Comparing `petljapub-2.0.0/src/petljapub/translit.py` & `petljapub-2.0.1/src/petljapub/translit.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.0/src/petljapub/util.py` & `petljapub-2.0.1/src/petljapub/util.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.0/src/petljapub/yaml_specification.py` & `petljapub-2.0.1/src/petljapub/yaml_specification.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.0/src/petljapub/yaml_specification_visitor_runtime.py` & `petljapub-2.0.1/src/petljapub/yaml_specification_visitor_runtime.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.0/src/petljapub/yaml_specification_visitor_stats.py` & `petljapub-2.0.1/src/petljapub/yaml_specification_visitor_stats.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.0/src/petljapub.egg-info/PKG-INFO` & `petljapub-2.0.1/src/petljapub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petljapub
-Version: 2.0.0
+Version: 2.0.1
 Summary: Petlja publishing system
 Home-page: https://github.com/pypa/petljapub
 Author: Filip Maric, Petlja
 Author-email: filip.maric@petlja.org
 Project-URL: Bug Tracker, https://github.com/pypa/petljapub/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

