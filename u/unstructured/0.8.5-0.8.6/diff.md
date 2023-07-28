# Comparing `tmp/unstructured-0.8.5.tar.gz` & `tmp/unstructured-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured-0.8.5.tar", last modified: Thu Jul 27 18:38:13 2023, max compression
+gzip compressed data, was "unstructured-0.8.6.tar", last modified: Fri Jul 28 06:49:26 2023, max compression
```

## Comparing `unstructured-0.8.5.tar` & `unstructured-0.8.6.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.752186 unstructured-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-27 18:38:02.000000 unstructured-0.8.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 18:38:02.000000 unstructured-0.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20030 2023-07-27 18:38:13.752186 unstructured-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16273 2023-07-27 18:38:02.000000 unstructured-0.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.732186 unstructured-0.8.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/huggingface.in
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/ingest-azure.in
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/ingest-discord.in
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/ingest-dropbox.in
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/ingest-gcs.in
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/ingest-github.in
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/ingest-gitlab.in
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/ingest-google-drive.in
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/ingest-onedrive.in
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/ingest-outlook.in
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/ingest-reddit.in
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/ingest-s3.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/ingest-slack.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/ingest-wikipedia.in
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/local-inference.in
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-27 18:38:13.752186 unstructured-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-27 18:38:02.000000 unstructured-0.8.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.732186 unstructured-0.8.5/test_unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:02.000000 unstructured-0.8.5/test_unstructured/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.732186 unstructured-0.8.5/test_unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:02.000000 unstructured-0.8.5/test_unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-27 18:38:02.000000 unstructured-0.8.5/test_unstructured/nlp/mock_nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-27 18:38:02.000000 unstructured-0.8.5/test_unstructured/nlp/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-27 18:38:02.000000 unstructured-0.8.5/test_unstructured/nlp/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-27 18:38:02.000000 unstructured-0.8.5/test_unstructured/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.732186 unstructured-0.8.5/unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.732186 unstructured-0.8.5/unstructured/cleaners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/cleaners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/cleaners/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/cleaners/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/cleaners/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.736186 unstructured-0.8.5/unstructured/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/documents/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/documents/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/documents/email_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/documents/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/documents/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.736186 unstructured-0.8.5/unstructured/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/file_utils/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/file_utils/exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/file_utils/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    20781 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/file_utils/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/file_utils/google_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/file_utils/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.736186 unstructured-0.8.5/unstructured/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.740186 unstructured-0.8.5/unstructured/ingest/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/confluence.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/dropbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/onedrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/outlook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.740186 unstructured-0.8.5/unstructured/ingest/doc_processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/doc_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/doc_processor/generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33906 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.740186 unstructured-0.8.5/unstructured/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.744186 unstructured-0.8.5/unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/nlp/english-words.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/nlp/english_words.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/nlp/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/nlp/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/nlp/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.752186 unstructured-0.8.5/unstructured/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11739 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)    10584 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12408 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/md.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/odt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/org.py
--rw-r--r--   0 runner    (1001) docker     (123)    17533 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/ppt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/pptx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/rst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/text_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/tsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.752186 unstructured-0.8.5/unstructured/staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/staging/argilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/staging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/staging/baseplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/staging/datasaur.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/staging/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/staging/label_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/staging/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/staging/prodigy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/staging/weaviate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.732186 unstructured-0.8.5/unstructured.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20030 2023-07-27 18:38:13.000000 unstructured-0.8.5/unstructured.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-27 18:38:13.000000 unstructured-0.8.5/unstructured.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 18:38:13.000000 unstructured-0.8.5/unstructured.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-27 18:38:13.000000 unstructured-0.8.5/unstructured.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-27 18:38:13.000000 unstructured-0.8.5/unstructured.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-27 18:38:13.000000 unstructured-0.8.5/unstructured.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.686168 unstructured-0.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-28 06:49:14.000000 unstructured-0.8.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 06:49:14.000000 unstructured-0.8.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20030 2023-07-28 06:49:26.686168 unstructured-0.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16273 2023-07-28 06:49:14.000000 unstructured-0.8.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.662168 unstructured-0.8.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/huggingface.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/ingest-azure.in
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/ingest-discord.in
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/ingest-dropbox.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/ingest-gcs.in
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/ingest-github.in
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/ingest-gitlab.in
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/ingest-google-drive.in
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/ingest-onedrive.in
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/ingest-outlook.in
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/ingest-reddit.in
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/ingest-s3.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/ingest-slack.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/ingest-wikipedia.in
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/local-inference.in
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-28 06:49:26.690168 unstructured-0.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-28 06:49:14.000000 unstructured-0.8.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.662168 unstructured-0.8.6/test_unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:14.000000 unstructured-0.8.6/test_unstructured/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.662168 unstructured-0.8.6/test_unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:14.000000 unstructured-0.8.6/test_unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-28 06:49:14.000000 unstructured-0.8.6/test_unstructured/nlp/mock_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-28 06:49:14.000000 unstructured-0.8.6/test_unstructured/nlp/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-28 06:49:14.000000 unstructured-0.8.6/test_unstructured/nlp/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-28 06:49:14.000000 unstructured-0.8.6/test_unstructured/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.662168 unstructured-0.8.6/unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.666168 unstructured-0.8.6/unstructured/cleaners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/cleaners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/cleaners/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/cleaners/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/cleaners/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.666168 unstructured-0.8.6/unstructured/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/documents/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/documents/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/documents/email_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/documents/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/documents/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.666168 unstructured-0.8.6/unstructured/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/file_utils/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/file_utils/exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/file_utils/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20736 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/file_utils/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/file_utils/google_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/file_utils/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.670168 unstructured-0.8.6/unstructured/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.670168 unstructured-0.8.6/unstructured/ingest/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/confluence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/onedrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/outlook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.674168 unstructured-0.8.6/unstructured/ingest/doc_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/doc_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/doc_processor/generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33906 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.674168 unstructured-0.8.6/unstructured/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.682168 unstructured-0.8.6/unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/nlp/english-words.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/nlp/english_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/nlp/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/nlp/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/nlp/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.686168 unstructured-0.8.6/unstructured/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11739 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10544 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12408 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/odt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/org.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17533 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/text_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/tsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.686168 unstructured-0.8.6/unstructured/staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/staging/argilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/staging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/staging/baseplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/staging/datasaur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/staging/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/staging/label_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/staging/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/staging/prodigy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/staging/weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.666168 unstructured-0.8.6/unstructured.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20030 2023-07-28 06:49:26.000000 unstructured-0.8.6/unstructured.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-28 06:49:26.000000 unstructured-0.8.6/unstructured.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 06:49:26.000000 unstructured-0.8.6/unstructured.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 06:49:26.000000 unstructured-0.8.6/unstructured.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-28 06:49:26.000000 unstructured-0.8.6/unstructured.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 06:49:26.000000 unstructured-0.8.6/unstructured.egg-info/top_level.txt
```

### Comparing `unstructured-0.8.5/LICENSE.md` & `unstructured-0.8.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/MANIFEST.in` & `unstructured-0.8.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/PKG-INFO` & `unstructured-0.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.8.5
+Version: 0.8.6
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.8.5 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.8.6 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
```

### Comparing `unstructured-0.8.5/README.md` & `unstructured-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/setup.py` & `unstructured-0.8.6/setup.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/test_unstructured/nlp/mock_nltk.py` & `unstructured-0.8.6/test_unstructured/nlp/mock_nltk.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/test_unstructured/nlp/test_tokenize.py` & `unstructured-0.8.6/test_unstructured/nlp/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/test_unstructured/test_utils.py` & `unstructured-0.8.6/test_unstructured/test_utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/cleaners/core.py` & `unstructured-0.8.6/unstructured/cleaners/core.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/cleaners/extract.py` & `unstructured-0.8.6/unstructured/cleaners/extract.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/cleaners/translate.py` & `unstructured-0.8.6/unstructured/cleaners/translate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/documents/base.py` & `unstructured-0.8.6/unstructured/documents/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/documents/coordinates.py` & `unstructured-0.8.6/unstructured/documents/coordinates.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/documents/elements.py` & `unstructured-0.8.6/unstructured/documents/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/documents/email_elements.py` & `unstructured-0.8.6/unstructured/documents/email_elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/documents/html.py` & `unstructured-0.8.6/unstructured/documents/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/documents/xml.py` & `unstructured-0.8.6/unstructured/documents/xml.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Optional, Union
 
-from lxml import etree, html
+from lxml import etree
 
 from unstructured.documents.base import Document, Page
 from unstructured.file_utils.encoding import read_txt_file
 from unstructured.logger import logger
 from unstructured.partition.text import (
     element_from_text,
     partition_text,
@@ -65,15 +65,14 @@
         # The correct output is returned once you add the initial return.
         is_html_parser = isinstance(self.parser, etree.HTMLParser)
         if content and not content.startswith("\n") and is_html_parser:
             content = "\n" + content
         if self.document_tree is None:
             try:
                 document_tree = etree.fromstring(content, self.parser)
-                print("document_tree", document_tree)
                 if document_tree is None:
                     raise ValueError("document_tree is None")
 
             # NOTE(robinson) - The following ValueError occurs with unicode strings. In that
             # case, we call back to encoding the string and passing in bytes.
             #     ValueError: Unicode strings with encoding declaration are not supported.
             #     Please use  bytes input or XML fragments without declaration.
@@ -89,20 +88,14 @@
                     for element in partition_text(text=element.text, paragraph_grouper=False):
                         text_content.append(element.text)
 
                     for text in text_content:
                         element = etree.Element("span")
                         element.text = str(element_from_text(text=text))
                         document_tree.append(element)
-            if "</a>" in content:
-                tree = html.fromstring(content)
-                links = list(tree.iterlinks())
-                print("here", links)
-                for el in document_tree:
-                    print(el)
 
             if self.stylesheet:
                 if isinstance(self.parser, etree.HTMLParser):
                     logger.warning(
                         "You are using the HTML parser with an XSLT stylesheet. "
                         "Stylesheets are more commonly parsed with the "
                         "XMLParser. If your HTML does not display properly, try "
@@ -111,15 +104,14 @@
                     )
                 xslt = etree.parse(self.stylesheet)
                 transform = etree.XSLT(xslt)
                 document_tree = transform(document_tree)
 
             self.document_tree = document_tree
 
-        print("self.document_tree", self.document_tree)
         return self.document_tree
 
     @classmethod
     def from_string(
         cls,
         text: str,
         parser: VALID_PARSERS = None,
@@ -138,10 +130,8 @@
         filename,
         parser: VALID_PARSERS = None,
         stylesheet: Optional[str] = None,
         encoding: Optional[str] = None,
         **kwargs,
     ):
         _, content = read_txt_file(filename=filename, encoding=encoding)
-        print("_____", _)
-        print("content", content)
         return cls.from_string(content, parser=parser, stylesheet=stylesheet, **kwargs)
```

### Comparing `unstructured-0.8.5/unstructured/file_utils/encoding.py` & `unstructured-0.8.6/unstructured/file_utils/encoding.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/file_utils/exploration.py` & `unstructured-0.8.6/unstructured/file_utils/exploration.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/file_utils/file_conversion.py` & `unstructured-0.8.6/unstructured/file_utils/file_conversion.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/file_utils/filetype.py` & `unstructured-0.8.6/unstructured/file_utils/filetype.py`

 * *Files 1% similar despite different names*

```diff
@@ -558,15 +558,14 @@
                     if el.metadata.coordinates
                     else float("inf"),
                     el.id,
                 ),
             )
         if include_page_breaks and i < num_pages - 1:
             page_elements.append(PageBreak(text=""))
-        print("page_element", page_elements)
         elements.extend(page_elements)
 
     return elements
 
 
 def _get_page_image_metadata(
     page: PageLayout,
```

### Comparing `unstructured-0.8.5/unstructured/file_utils/metadata.py` & `unstructured-0.8.6/unstructured/file_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/ingest/connector/azure.py` & `unstructured-0.8.6/unstructured/ingest/connector/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/ingest/connector/biomed.py` & `unstructured-0.8.6/unstructured/ingest/connector/biomed.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/ingest/connector/confluence.py` & `unstructured-0.8.6/unstructured/ingest/connector/confluence.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/ingest/connector/discord.py` & `unstructured-0.8.6/unstructured/ingest/connector/discord.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/ingest/connector/dropbox.py` & `unstructured-0.8.6/unstructured/ingest/connector/dropbox.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/ingest/connector/elasticsearch.py` & `unstructured-0.8.6/unstructured/ingest/connector/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/ingest/connector/fsspec.py` & `unstructured-0.8.6/unstructured/ingest/connector/fsspec.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/ingest/connector/gcs.py` & `unstructured-0.8.6/unstructured/ingest/connector/gcs.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/ingest/connector/git.py` & `unstructured-0.8.6/unstructured/ingest/connector/git.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/ingest/connector/github.py` & `unstructured-0.8.6/unstructured/ingest/connector/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/ingest/connector/gitlab.py` & `unstructured-0.8.6/unstructured/ingest/connector/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/ingest/connector/google_drive.py` & `unstructured-0.8.6/unstructured/ingest/connector/google_drive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/ingest/connector/local.py` & `unstructured-0.8.6/unstructured/ingest/connector/local.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/ingest/connector/onedrive.py` & `unstructured-0.8.6/unstructured/ingest/connector/onedrive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/ingest/connector/outlook.py` & `unstructured-0.8.6/unstructured/ingest/connector/outlook.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/ingest/connector/reddit.py` & `unstructured-0.8.6/unstructured/ingest/connector/reddit.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/ingest/connector/s3.py` & `unstructured-0.8.6/unstructured/ingest/connector/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/ingest/connector/slack.py` & `unstructured-0.8.6/unstructured/ingest/connector/slack.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/ingest/connector/wikipedia.py` & `unstructured-0.8.6/unstructured/ingest/connector/wikipedia.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/ingest/doc_processor/generalized.py` & `unstructured-0.8.6/unstructured/ingest/doc_processor/generalized.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/ingest/interfaces.py` & `unstructured-0.8.6/unstructured/ingest/interfaces.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/ingest/main.py` & `unstructured-0.8.6/unstructured/ingest/main.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/nlp/english-words.txt` & `unstructured-0.8.6/unstructured/nlp/english-words.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/nlp/english_words.py` & `unstructured-0.8.6/unstructured/nlp/english_words.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/nlp/patterns.py` & `unstructured-0.8.6/unstructured/nlp/patterns.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/nlp/tokenize.py` & `unstructured-0.8.6/unstructured/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/partition/__init__.py` & `unstructured-0.8.6/unstructured/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/partition/api.py` & `unstructured-0.8.6/unstructured/partition/api.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/partition/auto.py` & `unstructured-0.8.6/unstructured/partition/auto.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/partition/common.py` & `unstructured-0.8.6/unstructured/partition/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,14 @@
         layout_dict = layout_element
 
     text = layout_dict.get("text")
     # Both `coordinates` and `coordinate_system` must be present
     # in order to add coordinates metadata to the element.
     coordinates = layout_dict.get("coordinates")
     element_type = layout_dict.get("type")
-    print("element_type", element_type)
     if element_type == "List":
         return layout_list_to_list_items(
             text,
             coordinates=coordinates,
             coordinate_system=coordinate_system,
         )
     elif element_type in TYPE_TO_TEXT_ELEMENT_MAP:
```

### Comparing `unstructured-0.8.5/unstructured/partition/csv.py` & `unstructured-0.8.6/unstructured/partition/csv.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/partition/doc.py` & `unstructured-0.8.6/unstructured/partition/doc.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/partition/docx.py` & `unstructured-0.8.6/unstructured/partition/docx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/partition/email.py` & `unstructured-0.8.6/unstructured/partition/email.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/partition/epub.py` & `unstructured-0.8.6/unstructured/partition/epub.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/partition/html.py` & `unstructured-0.8.6/unstructured/partition/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/partition/image.py` & `unstructured-0.8.6/unstructured/partition/image.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/partition/json.py` & `unstructured-0.8.6/unstructured/partition/json.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/partition/md.py` & `unstructured-0.8.6/unstructured/partition/md.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/partition/msg.py` & `unstructured-0.8.6/unstructured/partition/msg.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/partition/odt.py` & `unstructured-0.8.6/unstructured/partition/odt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/partition/org.py` & `unstructured-0.8.6/unstructured/partition/org.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/partition/pdf.py` & `unstructured-0.8.6/unstructured/partition/pdf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/partition/ppt.py` & `unstructured-0.8.6/unstructured/partition/ppt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/partition/pptx.py` & `unstructured-0.8.6/unstructured/partition/pptx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/partition/rst.py` & `unstructured-0.8.6/unstructured/partition/rst.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/partition/rtf.py` & `unstructured-0.8.6/unstructured/partition/rtf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/partition/strategies.py` & `unstructured-0.8.6/unstructured/partition/strategies.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/partition/text.py` & `unstructured-0.8.6/unstructured/partition/text.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/partition/text_type.py` & `unstructured-0.8.6/unstructured/partition/text_type.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/partition/tsv.py` & `unstructured-0.8.6/unstructured/partition/tsv.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/partition/xlsx.py` & `unstructured-0.8.6/unstructured/partition/xlsx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/partition/xml.py` & `unstructured-0.8.6/unstructured/partition/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/staging/argilla.py` & `unstructured-0.8.6/unstructured/staging/argilla.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/staging/base.py` & `unstructured-0.8.6/unstructured/staging/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/staging/baseplate.py` & `unstructured-0.8.6/unstructured/staging/baseplate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/staging/datasaur.py` & `unstructured-0.8.6/unstructured/staging/datasaur.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/staging/huggingface.py` & `unstructured-0.8.6/unstructured/staging/huggingface.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/staging/label_box.py` & `unstructured-0.8.6/unstructured/staging/label_box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/staging/label_studio.py` & `unstructured-0.8.6/unstructured/staging/label_studio.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/staging/prodigy.py` & `unstructured-0.8.6/unstructured/staging/prodigy.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/staging/weaviate.py` & `unstructured-0.8.6/unstructured/staging/weaviate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured/utils.py` & `unstructured-0.8.6/unstructured/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured.egg-info/PKG-INFO` & `unstructured-0.8.6/unstructured.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.8.5
+Version: 0.8.6
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.8.5 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.8.6 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
```

### Comparing `unstructured-0.8.5/unstructured.egg-info/SOURCES.txt` & `unstructured-0.8.6/unstructured.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.5/unstructured.egg-info/requires.txt` & `unstructured-0.8.6/unstructured.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -56,20 +56,20 @@
 transformers
 
 [local-inference]
 unstructured-inference==0.5.7
 
 [onedrive]
 msal
-Office365-REST-Python-Client
+Office365-REST-Python-Client==2.4.2
 cryptography==41.0.2
 
 [outlook]
 msal
-Office365-REST-Python-Client
+Office365-REST-Python-Client==2.4.2
 cryptography==41.0.2
 
 [reddit]
 praw
 
 [s3]
 s3fs
```

