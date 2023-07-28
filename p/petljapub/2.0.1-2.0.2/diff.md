# Comparing `tmp/petljapub-2.0.1.tar.gz` & `tmp/petljapub-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petljapub-2.0.1.tar", last modified: Fri Jul 28 19:56:01 2023, max compression
+gzip compressed data, was "petljapub-2.0.2.tar", last modified: Fri Jul 28 20:16:01 2023, max compression
```

## Comparing `petljapub-2.0.1.tar` & `petljapub-2.0.2.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 19:56:01.521755 petljapub-2.0.1/
--rw-rw-r--   0 filip     (1000) filip     (1000)     1049 2021-08-26 07:51:10.000000 petljapub-2.0.1/LICENCE
--rw-rw-r--   0 filip     (1000) filip     (1000)    65748 2023-07-28 19:56:01.521755 petljapub-2.0.1/PKG-INFO
--rw-rw-r--   0 filip     (1000) filip     (1000)    65252 2023-02-02 09:47:42.000000 petljapub-2.0.1/README.md
--rw-rw-r--   0 filip     (1000) filip     (1000)      104 2021-08-26 07:42:20.000000 petljapub-2.0.1/pyproject.toml
--rw-rw-r--   0 filip     (1000) filip     (1000)       38 2023-07-28 19:56:01.521755 petljapub-2.0.1/setup.cfg
--rw-rw-r--   0 filip     (1000) filip     (1000)     1588 2023-07-28 19:55:57.000000 petljapub-2.0.1/setup.py
-drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 19:56:01.509754 petljapub-2.0.1/src/
-drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 19:56:01.517754 petljapub-2.0.1/src/petljapub/
--rw-rw-r--   0 filip     (1000) filip     (1000)        0 2021-08-26 08:36:06.000000 petljapub-2.0.1/src/petljapub/__init__.py
--rw-rw-r--   0 filip     (1000) filip     (1000)      355 2023-06-01 11:21:35.000000 petljapub-2.0.1/src/petljapub/code_parser.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     4180 2023-02-03 15:10:49.000000 petljapub-2.0.1/src/petljapub/compilation.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     1468 2023-01-20 21:26:43.000000 petljapub-2.0.1/src/petljapub/config.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     4163 2023-01-20 21:22:12.000000 petljapub-2.0.1/src/petljapub/configure_compilers.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     1967 2023-06-01 11:19:46.000000 petljapub-2.0.1/src/petljapub/cpp_parser.py
-drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 19:56:01.517754 petljapub-2.0.1/src/petljapub/data/
-drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 19:56:01.521755 petljapub-2.0.1/src/petljapub/data/_task_template/
-drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 19:56:01.521755 petljapub-2.0.1/src/petljapub/data/_task_template/en/
--rw-rw-r--   0 filip     (1000) filip     (1000)      163 2023-01-20 22:05:57.000000 petljapub-2.0.1/src/petljapub/data/_task_template/en/task-sol.md
--rw-rw-r--   0 filip     (1000) filip     (1000)      600 2023-01-20 21:46:16.000000 petljapub-2.0.1/src/petljapub/data/_task_template/en/task-st.md
-drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 19:56:01.521755 petljapub-2.0.1/src/petljapub/data/_task_template/sr-Cyrl/
--rw-rw-r--   0 filip     (1000) filip     (1000)      221 2023-01-20 22:05:18.000000 petljapub-2.0.1/src/petljapub/data/_task_template/sr-Cyrl/task-sol.md
--rw-rw-r--   0 filip     (1000) filip     (1000)      945 2023-01-20 21:48:04.000000 petljapub-2.0.1/src/petljapub/data/_task_template/sr-Cyrl/task-st.md
-drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 19:56:01.521755 petljapub-2.0.1/src/petljapub/data/_task_template/sr-Latn/
--rw-rw-r--   0 filip     (1000) filip     (1000)      157 2023-01-20 22:04:48.000000 petljapub-2.0.1/src/petljapub/data/_task_template/sr-Latn/task-sol.md
--rw-rw-r--   0 filip     (1000) filip     (1000)      654 2023-01-20 21:48:31.000000 petljapub-2.0.1/src/petljapub/data/_task_template/sr-Latn/task-st.md
--rw-rw-r--   0 filip     (1000) filip     (1000)      108 2022-05-26 09:03:06.000000 petljapub-2.0.1/src/petljapub/data/_task_template/task-tgen.cpp
--rw-rw-r--   0 filip     (1000) filip     (1000)       72 2021-08-26 09:05:12.000000 petljapub-2.0.1/src/petljapub/data/_task_template/task.cpp
--rw-rw-r--   0 filip     (1000) filip     (1000)       93 2021-08-26 09:05:12.000000 petljapub-2.0.1/src/petljapub/data/_task_template/task.cs
--rw-rw-r--   0 filip     (1000) filip     (1000)        8 2021-11-11 08:11:52.000000 petljapub-2.0.1/src/petljapub/data/_task_template/task.py
--rwxrwxr-x   0 filip     (1000) filip     (1000)     1008 2021-09-17 20:03:35.000000 petljapub-2.0.1/src/petljapub/data/compile-cs.sh
-drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 19:56:01.521755 petljapub-2.0.1/src/petljapub/data/html/
--rw-rw-r--   0 filip     (1000) filip     (1000)    18217 2023-02-05 17:07:03.000000 petljapub-2.0.1/src/petljapub/data/html/pandoc.css
-drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 19:56:01.521755 petljapub-2.0.1/src/petljapub/data/md/
--rw-rw-r--   0 filip     (1000) filip     (1000)      928 2023-01-17 12:19:40.000000 petljapub-2.0.1/src/petljapub/data/md/header.md
--rw-rw-r--   0 filip     (1000) filip     (1000)      170 2023-01-21 23:42:08.000000 petljapub-2.0.1/src/petljapub/data/template.yaml
-drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 19:56:01.521755 petljapub-2.0.1/src/petljapub/data/tex/
--rw-rw-r--   0 filip     (1000) filip     (1000)     8271 2023-01-19 15:30:58.000000 petljapub-2.0.1/src/petljapub/data/tex/default.latex
-drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 19:56:01.521755 petljapub-2.0.1/src/petljapub/data/tgen/
--rw-rw-r--   0 filip     (1000) filip     (1000)     2300 2021-08-26 11:04:47.000000 petljapub-2.0.1/src/petljapub/data/tgen/tgen-geom.hpp
--rw-rw-r--   0 filip     (1000) filip     (1000)    10168 2022-05-26 09:28:25.000000 petljapub-2.0.1/src/petljapub/data/tgen/tgen-graph.hpp
--rw-rw-r--   0 filip     (1000) filip     (1000)    12132 2022-10-22 08:05:12.000000 petljapub-2.0.1/src/petljapub/data/tgen/tgen.hpp
--rw-rw-r--   0 filip     (1000) filip     (1000)     1444 2022-02-24 21:25:45.000000 petljapub-2.0.1/src/petljapub/default_checker.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     4576 2022-12-13 00:25:03.000000 petljapub-2.0.1/src/petljapub/fix_latex.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     3584 2023-02-05 17:07:29.000000 petljapub-2.0.1/src/petljapub/javascript.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     1408 2022-03-10 10:38:08.000000 petljapub-2.0.1/src/petljapub/logger.py
--rw-rw-r--   0 filip     (1000) filip     (1000)      144 2022-10-16 07:28:50.000000 petljapub-2.0.1/src/petljapub/main.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     7069 2023-02-01 22:57:46.000000 petljapub-2.0.1/src/petljapub/markdown_magic_comments.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     7529 2023-01-12 12:29:21.000000 petljapub-2.0.1/src/petljapub/md_content_processor.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     5954 2023-05-19 15:10:00.000000 petljapub-2.0.1/src/petljapub/md_util.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     3171 2023-07-27 08:23:50.000000 petljapub-2.0.1/src/petljapub/messages.py
--rw-rw-r--   0 filip     (1000) filip     (1000)      888 2021-09-18 19:26:06.000000 petljapub-2.0.1/src/petljapub/plot_times.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     7109 2023-01-13 07:59:24.000000 petljapub-2.0.1/src/petljapub/publication_repository.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     1979 2023-01-07 22:31:37.000000 petljapub-2.0.1/src/petljapub/publication_visitor.py
--rw-rw-r--   0 filip     (1000) filip     (1000)    17276 2023-05-26 09:05:32.000000 petljapub-2.0.1/src/petljapub/publication_visitor_html.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     5522 2023-01-13 07:58:18.000000 petljapub-2.0.1/src/petljapub/publication_visitor_petlja.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     2404 2023-01-07 14:20:39.000000 petljapub-2.0.1/src/petljapub/publication_visitor_testing.py
--rw-rw-r--   0 filip     (1000) filip     (1000)    11733 2023-05-26 09:04:51.000000 petljapub-2.0.1/src/petljapub/publication_visitor_tex.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     1072 2023-02-03 20:21:18.000000 petljapub-2.0.1/src/petljapub/py_parser.py
--rw-rw-r--   0 filip     (1000) filip     (1000)    11205 2023-07-27 08:25:09.000000 petljapub-2.0.1/src/petljapub/serialization.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     3042 2021-08-26 15:29:54.000000 petljapub-2.0.1/src/petljapub/source_code_magic_comments.py
--rw-rw-r--   0 filip     (1000) filip     (1000)    46615 2023-05-26 09:01:06.000000 petljapub-2.0.1/src/petljapub/task.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     2752 2023-01-26 13:02:08.000000 petljapub-2.0.1/src/petljapub/task_repository.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     7519 2023-06-27 11:13:15.000000 petljapub-2.0.1/src/petljapub/task_visitor.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     4209 2023-01-22 00:14:26.000000 petljapub-2.0.1/src/petljapub/task_visitor_html.py
--rw-rw-r--   0 filip     (1000) filip     (1000)    31490 2023-03-02 11:37:38.000000 petljapub-2.0.1/src/petljapub/tasks.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     2893 2021-08-26 08:59:04.000000 petljapub-2.0.1/src/petljapub/translit.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     1005 2022-03-17 20:45:10.000000 petljapub-2.0.1/src/petljapub/util.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     9712 2023-01-21 07:52:28.000000 petljapub-2.0.1/src/petljapub/yaml_specification.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     7550 2021-09-25 18:42:07.000000 petljapub-2.0.1/src/petljapub/yaml_specification_visitor_runtime.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     2470 2021-09-19 22:45:26.000000 petljapub-2.0.1/src/petljapub/yaml_specification_visitor_stats.py
-drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 19:56:01.517754 petljapub-2.0.1/src/petljapub.egg-info/
--rw-rw-r--   0 filip     (1000) filip     (1000)    65748 2023-07-28 19:56:01.000000 petljapub-2.0.1/src/petljapub.egg-info/PKG-INFO
--rw-rw-r--   0 filip     (1000) filip     (1000)     2372 2023-07-28 19:56:01.000000 petljapub-2.0.1/src/petljapub.egg-info/SOURCES.txt
--rw-rw-r--   0 filip     (1000) filip     (1000)        1 2023-07-28 19:56:01.000000 petljapub-2.0.1/src/petljapub.egg-info/dependency_links.txt
--rw-rw-r--   0 filip     (1000) filip     (1000)       57 2023-07-28 19:56:01.000000 petljapub-2.0.1/src/petljapub.egg-info/entry_points.txt
--rw-rw-r--   0 filip     (1000) filip     (1000)      104 2023-07-28 19:56:01.000000 petljapub-2.0.1/src/petljapub.egg-info/requires.txt
--rw-rw-r--   0 filip     (1000) filip     (1000)       10 2023-07-28 19:56:01.000000 petljapub-2.0.1/src/petljapub.egg-info/top_level.txt
-drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 19:56:01.521755 petljapub-2.0.1/tests/
--rw-rw-r--   0 filip     (1000) filip     (1000)     5257 2023-01-22 14:22:00.000000 petljapub-2.0.1/tests/test_markdown_magic_comments.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     5075 2023-01-15 08:31:48.000000 petljapub-2.0.1/tests/test_md_content_processor.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     5947 2023-02-06 08:18:43.000000 petljapub-2.0.1/tests/test_md_util.py
--rw-rw-r--   0 filip     (1000) filip     (1000)      439 2023-01-21 20:08:18.000000 petljapub-2.0.1/tests/test_messages.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     3129 2023-02-06 08:14:26.000000 petljapub-2.0.1/tests/test_parsers.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     1937 2022-10-31 17:05:01.000000 petljapub-2.0.1/tests/test_publication_repository.py
--rw-rw-r--   0 filip     (1000) filip     (1000)     6991 2023-02-03 13:51:21.000000 petljapub-2.0.1/tests/test_task.py
+drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 20:16:01.843963 petljapub-2.0.2/
+-rw-rw-r--   0 filip     (1000) filip     (1000)     1049 2021-08-26 07:51:10.000000 petljapub-2.0.2/LICENCE
+-rw-rw-r--   0 filip     (1000) filip     (1000)    65748 2023-07-28 20:16:01.839963 petljapub-2.0.2/PKG-INFO
+-rw-rw-r--   0 filip     (1000) filip     (1000)    65252 2023-02-02 09:47:42.000000 petljapub-2.0.2/README.md
+-rw-rw-r--   0 filip     (1000) filip     (1000)      104 2021-08-26 07:42:20.000000 petljapub-2.0.2/pyproject.toml
+-rw-rw-r--   0 filip     (1000) filip     (1000)       38 2023-07-28 20:16:01.843963 petljapub-2.0.2/setup.cfg
+-rw-rw-r--   0 filip     (1000) filip     (1000)     1567 2023-07-28 20:15:55.000000 petljapub-2.0.2/setup.py
+drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 20:16:01.803963 petljapub-2.0.2/src/
+drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 20:16:01.827963 petljapub-2.0.2/src/petljapub/
+-rw-rw-r--   0 filip     (1000) filip     (1000)        0 2021-08-26 08:36:06.000000 petljapub-2.0.2/src/petljapub/__init__.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)      355 2023-06-01 11:21:35.000000 petljapub-2.0.2/src/petljapub/code_parser.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     4180 2023-02-03 15:10:49.000000 petljapub-2.0.2/src/petljapub/compilation.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     1468 2023-01-20 21:26:43.000000 petljapub-2.0.2/src/petljapub/config.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     4163 2023-01-20 21:22:12.000000 petljapub-2.0.2/src/petljapub/configure_compilers.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     1967 2023-06-01 11:19:46.000000 petljapub-2.0.2/src/petljapub/cpp_parser.py
+drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 20:16:01.831963 petljapub-2.0.2/src/petljapub/data/
+drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 20:16:01.831963 petljapub-2.0.2/src/petljapub/data/_task_template/
+drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 20:16:01.831963 petljapub-2.0.2/src/petljapub/data/_task_template/en/
+-rw-rw-r--   0 filip     (1000) filip     (1000)      163 2023-01-20 22:05:57.000000 petljapub-2.0.2/src/petljapub/data/_task_template/en/task-sol.md
+-rw-rw-r--   0 filip     (1000) filip     (1000)      600 2023-01-20 21:46:16.000000 petljapub-2.0.2/src/petljapub/data/_task_template/en/task-st.md
+drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 20:16:01.835963 petljapub-2.0.2/src/petljapub/data/_task_template/sr-Cyrl/
+-rw-rw-r--   0 filip     (1000) filip     (1000)      221 2023-01-20 22:05:18.000000 petljapub-2.0.2/src/petljapub/data/_task_template/sr-Cyrl/task-sol.md
+-rw-rw-r--   0 filip     (1000) filip     (1000)      945 2023-01-20 21:48:04.000000 petljapub-2.0.2/src/petljapub/data/_task_template/sr-Cyrl/task-st.md
+drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 20:16:01.835963 petljapub-2.0.2/src/petljapub/data/_task_template/sr-Latn/
+-rw-rw-r--   0 filip     (1000) filip     (1000)      157 2023-01-20 22:04:48.000000 petljapub-2.0.2/src/petljapub/data/_task_template/sr-Latn/task-sol.md
+-rw-rw-r--   0 filip     (1000) filip     (1000)      654 2023-01-20 21:48:31.000000 petljapub-2.0.2/src/petljapub/data/_task_template/sr-Latn/task-st.md
+-rw-rw-r--   0 filip     (1000) filip     (1000)      108 2022-05-26 09:03:06.000000 petljapub-2.0.2/src/petljapub/data/_task_template/task-tgen.cpp
+-rw-rw-r--   0 filip     (1000) filip     (1000)       72 2021-08-26 09:05:12.000000 petljapub-2.0.2/src/petljapub/data/_task_template/task.cpp
+-rw-rw-r--   0 filip     (1000) filip     (1000)       93 2021-08-26 09:05:12.000000 petljapub-2.0.2/src/petljapub/data/_task_template/task.cs
+-rw-rw-r--   0 filip     (1000) filip     (1000)        8 2021-11-11 08:11:52.000000 petljapub-2.0.2/src/petljapub/data/_task_template/task.py
+-rwxrwxr-x   0 filip     (1000) filip     (1000)     1008 2021-09-17 20:03:35.000000 petljapub-2.0.2/src/petljapub/data/compile-cs.sh
+drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 20:16:01.835963 petljapub-2.0.2/src/petljapub/data/html/
+-rw-rw-r--   0 filip     (1000) filip     (1000)    18217 2023-02-05 17:07:03.000000 petljapub-2.0.2/src/petljapub/data/html/pandoc.css
+drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 20:16:01.835963 petljapub-2.0.2/src/petljapub/data/md/
+-rw-rw-r--   0 filip     (1000) filip     (1000)      928 2023-01-17 12:19:40.000000 petljapub-2.0.2/src/petljapub/data/md/header.md
+-rw-rw-r--   0 filip     (1000) filip     (1000)      170 2023-01-21 23:42:08.000000 petljapub-2.0.2/src/petljapub/data/template.yaml
+drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 20:16:01.835963 petljapub-2.0.2/src/petljapub/data/tex/
+-rw-rw-r--   0 filip     (1000) filip     (1000)     8271 2023-01-19 15:30:58.000000 petljapub-2.0.2/src/petljapub/data/tex/default.latex
+drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 20:16:01.839963 petljapub-2.0.2/src/petljapub/data/tgen/
+-rw-rw-r--   0 filip     (1000) filip     (1000)     2300 2021-08-26 11:04:47.000000 petljapub-2.0.2/src/petljapub/data/tgen/tgen-geom.hpp
+-rw-rw-r--   0 filip     (1000) filip     (1000)    10168 2022-05-26 09:28:25.000000 petljapub-2.0.2/src/petljapub/data/tgen/tgen-graph.hpp
+-rw-rw-r--   0 filip     (1000) filip     (1000)    12132 2022-10-22 08:05:12.000000 petljapub-2.0.2/src/petljapub/data/tgen/tgen.hpp
+-rw-rw-r--   0 filip     (1000) filip     (1000)     1444 2022-02-24 21:25:45.000000 petljapub-2.0.2/src/petljapub/default_checker.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     4576 2022-12-13 00:25:03.000000 petljapub-2.0.2/src/petljapub/fix_latex.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     3584 2023-02-05 17:07:29.000000 petljapub-2.0.2/src/petljapub/javascript.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     1408 2022-03-10 10:38:08.000000 petljapub-2.0.2/src/petljapub/logger.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)      144 2022-10-16 07:28:50.000000 petljapub-2.0.2/src/petljapub/main.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     7069 2023-02-01 22:57:46.000000 petljapub-2.0.2/src/petljapub/markdown_magic_comments.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     7529 2023-01-12 12:29:21.000000 petljapub-2.0.2/src/petljapub/md_content_processor.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     5954 2023-05-19 15:10:00.000000 petljapub-2.0.2/src/petljapub/md_util.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     3171 2023-07-27 08:23:50.000000 petljapub-2.0.2/src/petljapub/messages.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)      888 2021-09-18 19:26:06.000000 petljapub-2.0.2/src/petljapub/plot_times.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     7109 2023-01-13 07:59:24.000000 petljapub-2.0.2/src/petljapub/publication_repository.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     1979 2023-01-07 22:31:37.000000 petljapub-2.0.2/src/petljapub/publication_visitor.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)    17276 2023-05-26 09:05:32.000000 petljapub-2.0.2/src/petljapub/publication_visitor_html.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     5522 2023-01-13 07:58:18.000000 petljapub-2.0.2/src/petljapub/publication_visitor_petlja.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     2404 2023-01-07 14:20:39.000000 petljapub-2.0.2/src/petljapub/publication_visitor_testing.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)    11733 2023-05-26 09:04:51.000000 petljapub-2.0.2/src/petljapub/publication_visitor_tex.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     1072 2023-02-03 20:21:18.000000 petljapub-2.0.2/src/petljapub/py_parser.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)    11205 2023-07-27 08:25:09.000000 petljapub-2.0.2/src/petljapub/serialization.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     3042 2021-08-26 15:29:54.000000 petljapub-2.0.2/src/petljapub/source_code_magic_comments.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)    46615 2023-05-26 09:01:06.000000 petljapub-2.0.2/src/petljapub/task.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     2752 2023-01-26 13:02:08.000000 petljapub-2.0.2/src/petljapub/task_repository.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     7519 2023-06-27 11:13:15.000000 petljapub-2.0.2/src/petljapub/task_visitor.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     4209 2023-01-22 00:14:26.000000 petljapub-2.0.2/src/petljapub/task_visitor_html.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)    31490 2023-03-02 11:37:38.000000 petljapub-2.0.2/src/petljapub/tasks.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     2893 2021-08-26 08:59:04.000000 petljapub-2.0.2/src/petljapub/translit.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     1005 2022-03-17 20:45:10.000000 petljapub-2.0.2/src/petljapub/util.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     9712 2023-01-21 07:52:28.000000 petljapub-2.0.2/src/petljapub/yaml_specification.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     7550 2021-09-25 18:42:07.000000 petljapub-2.0.2/src/petljapub/yaml_specification_visitor_runtime.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     2470 2021-09-19 22:45:26.000000 petljapub-2.0.2/src/petljapub/yaml_specification_visitor_stats.py
+drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 20:16:01.831963 petljapub-2.0.2/src/petljapub.egg-info/
+-rw-rw-r--   0 filip     (1000) filip     (1000)    65748 2023-07-28 20:16:01.000000 petljapub-2.0.2/src/petljapub.egg-info/PKG-INFO
+-rw-rw-r--   0 filip     (1000) filip     (1000)     2372 2023-07-28 20:16:01.000000 petljapub-2.0.2/src/petljapub.egg-info/SOURCES.txt
+-rw-rw-r--   0 filip     (1000) filip     (1000)        1 2023-07-28 20:16:01.000000 petljapub-2.0.2/src/petljapub.egg-info/dependency_links.txt
+-rw-rw-r--   0 filip     (1000) filip     (1000)       57 2023-07-28 20:16:01.000000 petljapub-2.0.2/src/petljapub.egg-info/entry_points.txt
+-rw-rw-r--   0 filip     (1000) filip     (1000)       86 2023-07-28 20:16:01.000000 petljapub-2.0.2/src/petljapub.egg-info/requires.txt
+-rw-rw-r--   0 filip     (1000) filip     (1000)       10 2023-07-28 20:16:01.000000 petljapub-2.0.2/src/petljapub.egg-info/top_level.txt
+drwxrwxr-x   0 filip     (1000) filip     (1000)        0 2023-07-28 20:16:01.839963 petljapub-2.0.2/tests/
+-rw-rw-r--   0 filip     (1000) filip     (1000)     5257 2023-01-22 14:22:00.000000 petljapub-2.0.2/tests/test_markdown_magic_comments.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     5075 2023-01-15 08:31:48.000000 petljapub-2.0.2/tests/test_md_content_processor.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     5947 2023-02-06 08:18:43.000000 petljapub-2.0.2/tests/test_md_util.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)      439 2023-01-21 20:08:18.000000 petljapub-2.0.2/tests/test_messages.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     3129 2023-02-06 08:14:26.000000 petljapub-2.0.2/tests/test_parsers.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     1937 2022-10-31 17:05:01.000000 petljapub-2.0.2/tests/test_publication_repository.py
+-rw-rw-r--   0 filip     (1000) filip     (1000)     6991 2023-02-03 13:51:21.000000 petljapub-2.0.2/tests/test_task.py
```

### Comparing `petljapub-2.0.1/LICENCE` & `petljapub-2.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/PKG-INFO` & `petljapub-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petljapub
-Version: 2.0.1
+Version: 2.0.2
 Summary: Petlja publishing system
 Home-page: https://github.com/pypa/petljapub
 Author: Filip Maric, Petlja
 Author-email: filip.maric@petlja.org
 Project-URL: Bug Tracker, https://github.com/pypa/petljapub/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `petljapub-2.0.1/README.md` & `petljapub-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/setup.py` & `petljapub-2.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="petljapub",
-    version="2.0.1",
+    version="2.0.2",
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
-    install_requires=['invoke', 'pyyaml', 'pypandoc', 'pandoc-xnos', 'pandoc-fignos',  'pandoc-eqnos', 'pandoc-theoremnos', 'appdirs', 'matplotlib>=3.4'],
+    install_requires=['invoke', 'pyyaml', 'pypandoc', 'pandoc-xnos', 'pandoc-fignos',  'pandoc-eqnos', 'appdirs', 'matplotlib>=3.4'],
     entry_points={
         'console_scripts': ['petljapub = petljapub.main:program.run']
     },
     package_data={"petljapub": ["data/_task_template/*",
                                 "data/_task_template/en/*",
                                 "data/_task_template/sr-Cyrl/*",
                                 "data/_task_template/sr-Latn/*",
```

### Comparing `petljapub-2.0.1/src/petljapub/compilation.py` & `petljapub-2.0.2/src/petljapub/compilation.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/config.py` & `petljapub-2.0.2/src/petljapub/config.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/configure_compilers.py` & `petljapub-2.0.2/src/petljapub/configure_compilers.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/cpp_parser.py` & `petljapub-2.0.2/src/petljapub/cpp_parser.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/data/_task_template/en/task-st.md` & `petljapub-2.0.2/src/petljapub/data/_task_template/en/task-st.md`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/data/_task_template/sr-Cyrl/task-st.md` & `petljapub-2.0.2/src/petljapub/data/_task_template/sr-Cyrl/task-st.md`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/data/_task_template/sr-Latn/task-st.md` & `petljapub-2.0.2/src/petljapub/data/_task_template/sr-Latn/task-st.md`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/data/compile-cs.sh` & `petljapub-2.0.2/src/petljapub/data/compile-cs.sh`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/data/html/pandoc.css` & `petljapub-2.0.2/src/petljapub/data/html/pandoc.css`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/data/md/header.md` & `petljapub-2.0.2/src/petljapub/data/md/header.md`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/data/tex/default.latex` & `petljapub-2.0.2/src/petljapub/data/tex/default.latex`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/data/tgen/tgen-geom.hpp` & `petljapub-2.0.2/src/petljapub/data/tgen/tgen-geom.hpp`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/data/tgen/tgen-graph.hpp` & `petljapub-2.0.2/src/petljapub/data/tgen/tgen-graph.hpp`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/data/tgen/tgen.hpp` & `petljapub-2.0.2/src/petljapub/data/tgen/tgen.hpp`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/default_checker.py` & `petljapub-2.0.2/src/petljapub/default_checker.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/fix_latex.py` & `petljapub-2.0.2/src/petljapub/fix_latex.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/javascript.py` & `petljapub-2.0.2/src/petljapub/javascript.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/logger.py` & `petljapub-2.0.2/src/petljapub/logger.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/markdown_magic_comments.py` & `petljapub-2.0.2/src/petljapub/markdown_magic_comments.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/md_content_processor.py` & `petljapub-2.0.2/src/petljapub/md_content_processor.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/md_util.py` & `petljapub-2.0.2/src/petljapub/md_util.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/messages.py` & `petljapub-2.0.2/src/petljapub/messages.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/plot_times.py` & `petljapub-2.0.2/src/petljapub/plot_times.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/publication_repository.py` & `petljapub-2.0.2/src/petljapub/publication_repository.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/publication_visitor.py` & `petljapub-2.0.2/src/petljapub/publication_visitor.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/publication_visitor_html.py` & `petljapub-2.0.2/src/petljapub/publication_visitor_html.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/publication_visitor_petlja.py` & `petljapub-2.0.2/src/petljapub/publication_visitor_petlja.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/publication_visitor_testing.py` & `petljapub-2.0.2/src/petljapub/publication_visitor_testing.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/publication_visitor_tex.py` & `petljapub-2.0.2/src/petljapub/publication_visitor_tex.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/py_parser.py` & `petljapub-2.0.2/src/petljapub/py_parser.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/serialization.py` & `petljapub-2.0.2/src/petljapub/serialization.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/source_code_magic_comments.py` & `petljapub-2.0.2/src/petljapub/source_code_magic_comments.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/task.py` & `petljapub-2.0.2/src/petljapub/task.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/task_repository.py` & `petljapub-2.0.2/src/petljapub/task_repository.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/task_visitor.py` & `petljapub-2.0.2/src/petljapub/task_visitor.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/task_visitor_html.py` & `petljapub-2.0.2/src/petljapub/task_visitor_html.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/tasks.py` & `petljapub-2.0.2/src/petljapub/tasks.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/translit.py` & `petljapub-2.0.2/src/petljapub/translit.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/util.py` & `petljapub-2.0.2/src/petljapub/util.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/yaml_specification.py` & `petljapub-2.0.2/src/petljapub/yaml_specification.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/yaml_specification_visitor_runtime.py` & `petljapub-2.0.2/src/petljapub/yaml_specification_visitor_runtime.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub/yaml_specification_visitor_stats.py` & `petljapub-2.0.2/src/petljapub/yaml_specification_visitor_stats.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/src/petljapub.egg-info/PKG-INFO` & `petljapub-2.0.2/src/petljapub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petljapub
-Version: 2.0.1
+Version: 2.0.2
 Summary: Petlja publishing system
 Home-page: https://github.com/pypa/petljapub
 Author: Filip Maric, Petlja
 Author-email: filip.maric@petlja.org
 Project-URL: Bug Tracker, https://github.com/pypa/petljapub/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `petljapub-2.0.1/src/petljapub.egg-info/SOURCES.txt` & `petljapub-2.0.2/src/petljapub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/tests/test_markdown_magic_comments.py` & `petljapub-2.0.2/tests/test_markdown_magic_comments.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/tests/test_md_content_processor.py` & `petljapub-2.0.2/tests/test_md_content_processor.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/tests/test_md_util.py` & `petljapub-2.0.2/tests/test_md_util.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/tests/test_parsers.py` & `petljapub-2.0.2/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/tests/test_publication_repository.py` & `petljapub-2.0.2/tests/test_publication_repository.py`

 * *Files identical despite different names*

### Comparing `petljapub-2.0.1/tests/test_task.py` & `petljapub-2.0.2/tests/test_task.py`

 * *Files identical despite different names*

