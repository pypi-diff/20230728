# Comparing `tmp/unstructured-0.8.6.tar.gz` & `tmp/unstructured-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured-0.8.6.tar", last modified: Fri Jul 28 06:49:26 2023, max compression
+gzip compressed data, was "unstructured-0.8.7.tar", last modified: Fri Jul 28 16:42:16 2023, max compression
```

## Comparing `unstructured-0.8.6.tar` & `unstructured-0.8.7.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.686168 unstructured-0.8.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-28 06:49:14.000000 unstructured-0.8.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 06:49:14.000000 unstructured-0.8.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20030 2023-07-28 06:49:26.686168 unstructured-0.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16273 2023-07-28 06:49:14.000000 unstructured-0.8.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.662168 unstructured-0.8.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/huggingface.in
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/ingest-azure.in
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/ingest-discord.in
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/ingest-dropbox.in
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/ingest-gcs.in
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/ingest-github.in
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/ingest-gitlab.in
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/ingest-google-drive.in
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/ingest-onedrive.in
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/ingest-outlook.in
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/ingest-reddit.in
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/ingest-s3.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/ingest-slack.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/ingest-wikipedia.in
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-28 06:49:14.000000 unstructured-0.8.6/requirements/local-inference.in
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-28 06:49:26.690168 unstructured-0.8.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-28 06:49:14.000000 unstructured-0.8.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.662168 unstructured-0.8.6/test_unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:14.000000 unstructured-0.8.6/test_unstructured/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.662168 unstructured-0.8.6/test_unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:14.000000 unstructured-0.8.6/test_unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-28 06:49:14.000000 unstructured-0.8.6/test_unstructured/nlp/mock_nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-28 06:49:14.000000 unstructured-0.8.6/test_unstructured/nlp/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-28 06:49:14.000000 unstructured-0.8.6/test_unstructured/nlp/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-28 06:49:14.000000 unstructured-0.8.6/test_unstructured/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.662168 unstructured-0.8.6/unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.666168 unstructured-0.8.6/unstructured/cleaners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/cleaners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/cleaners/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/cleaners/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/cleaners/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.666168 unstructured-0.8.6/unstructured/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/documents/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/documents/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/documents/email_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/documents/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/documents/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.666168 unstructured-0.8.6/unstructured/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/file_utils/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/file_utils/exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/file_utils/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    20736 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/file_utils/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/file_utils/google_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/file_utils/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.670168 unstructured-0.8.6/unstructured/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.670168 unstructured-0.8.6/unstructured/ingest/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/confluence.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/dropbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/onedrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/outlook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/connector/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.674168 unstructured-0.8.6/unstructured/ingest/doc_processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/doc_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/doc_processor/generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33906 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/ingest/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.674168 unstructured-0.8.6/unstructured/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.682168 unstructured-0.8.6/unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/nlp/english-words.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/nlp/english_words.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/nlp/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/nlp/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/nlp/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.686168 unstructured-0.8.6/unstructured/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11739 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)    10544 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12408 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/md.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/odt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/org.py
--rw-r--r--   0 runner    (1001) docker     (123)    17533 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/ppt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/pptx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/rst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/text_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/tsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/partition/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.686168 unstructured-0.8.6/unstructured/staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/staging/argilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/staging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/staging/baseplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/staging/datasaur.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/staging/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/staging/label_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/staging/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/staging/prodigy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/staging/weaviate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-28 06:49:14.000000 unstructured-0.8.6/unstructured/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:49:26.666168 unstructured-0.8.6/unstructured.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20030 2023-07-28 06:49:26.000000 unstructured-0.8.6/unstructured.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-28 06:49:26.000000 unstructured-0.8.6/unstructured.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 06:49:26.000000 unstructured-0.8.6/unstructured.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 06:49:26.000000 unstructured-0.8.6/unstructured.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-28 06:49:26.000000 unstructured-0.8.6/unstructured.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 06:49:26.000000 unstructured-0.8.6/unstructured.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.215083 unstructured-0.8.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-28 16:42:06.000000 unstructured-0.8.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 16:42:06.000000 unstructured-0.8.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20030 2023-07-28 16:42:16.215083 unstructured-0.8.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16273 2023-07-28 16:42:06.000000 unstructured-0.8.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.203083 unstructured-0.8.7/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/huggingface.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/ingest-azure.in
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/ingest-discord.in
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/ingest-dropbox.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/ingest-gcs.in
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/ingest-github.in
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/ingest-gitlab.in
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/ingest-google-drive.in
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/ingest-onedrive.in
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/ingest-outlook.in
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/ingest-reddit.in
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/ingest-s3.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/ingest-slack.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/ingest-wikipedia.in
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/local-inference.in
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-28 16:42:16.215083 unstructured-0.8.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-28 16:42:06.000000 unstructured-0.8.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.203083 unstructured-0.8.7/test_unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:06.000000 unstructured-0.8.7/test_unstructured/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.203083 unstructured-0.8.7/test_unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:06.000000 unstructured-0.8.7/test_unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-28 16:42:06.000000 unstructured-0.8.7/test_unstructured/nlp/mock_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-28 16:42:06.000000 unstructured-0.8.7/test_unstructured/nlp/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-28 16:42:06.000000 unstructured-0.8.7/test_unstructured/nlp/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-28 16:42:06.000000 unstructured-0.8.7/test_unstructured/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.203083 unstructured-0.8.7/unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.203083 unstructured-0.8.7/unstructured/cleaners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/cleaners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/cleaners/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/cleaners/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/cleaners/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.203083 unstructured-0.8.7/unstructured/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/documents/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/documents/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/documents/email_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/documents/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/documents/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.203083 unstructured-0.8.7/unstructured/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/file_utils/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/file_utils/exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/file_utils/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20736 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/file_utils/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/file_utils/google_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/file_utils/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.203083 unstructured-0.8.7/unstructured/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.207083 unstructured-0.8.7/unstructured/ingest/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/confluence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/onedrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/outlook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.207083 unstructured-0.8.7/unstructured/ingest/doc_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/doc_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/doc_processor/generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33906 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.207083 unstructured-0.8.7/unstructured/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.211083 unstructured-0.8.7/unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/nlp/english-words.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/nlp/english_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/nlp/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/nlp/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/nlp/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.215083 unstructured-0.8.7/unstructured/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11739 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10544 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12408 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/odt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/org.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17533 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/text_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/tsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.215083 unstructured-0.8.7/unstructured/staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/staging/argilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/staging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/staging/baseplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/staging/datasaur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/staging/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/staging/label_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/staging/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/staging/prodigy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/staging/weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.203083 unstructured-0.8.7/unstructured.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20030 2023-07-28 16:42:15.000000 unstructured-0.8.7/unstructured.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-28 16:42:16.000000 unstructured-0.8.7/unstructured.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 16:42:15.000000 unstructured-0.8.7/unstructured.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 16:42:15.000000 unstructured-0.8.7/unstructured.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-28 16:42:15.000000 unstructured-0.8.7/unstructured.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 16:42:15.000000 unstructured-0.8.7/unstructured.egg-info/top_level.txt
```

### Comparing `unstructured-0.8.6/LICENSE.md` & `unstructured-0.8.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/MANIFEST.in` & `unstructured-0.8.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/PKG-INFO` & `unstructured-0.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.8.6
+Version: 0.8.7
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
-Metadata-Version: 2.1 Name: unstructured Version: 0.8.6 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.8.7 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
```

### Comparing `unstructured-0.8.6/README.md` & `unstructured-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/setup.py` & `unstructured-0.8.7/setup.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/test_unstructured/nlp/mock_nltk.py` & `unstructured-0.8.7/test_unstructured/nlp/mock_nltk.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/test_unstructured/nlp/test_tokenize.py` & `unstructured-0.8.7/test_unstructured/nlp/test_tokenize.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,7 +64,14 @@
 def test_pos_tag_caches(monkeypatch):
     monkeypatch.setattr(tokenize, "_word_tokenize", mock_word_tokenize)
     monkeypatch.setattr(tokenize, "_pos_tag", mock_pos_tag)
     tokenize.pos_tag.cache_clear()
     assert tokenize.pos_tag.cache_info().currsize == 0
     tokenize.pos_tag("Greetings! I am from outer space.")
     assert tokenize.pos_tag.cache_info().currsize == 1
+
+
+def test_tokenizers_functions_run():
+    sentence = "I am a big brown bear. What are you?"
+    tokenize.sent_tokenize(sentence)
+    tokenize.word_tokenize(sentence)
+    tokenize.pos_tag(sentence)
```

### Comparing `unstructured-0.8.6/test_unstructured/test_utils.py` & `unstructured-0.8.7/test_unstructured/test_utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/cleaners/core.py` & `unstructured-0.8.7/unstructured/cleaners/core.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/cleaners/extract.py` & `unstructured-0.8.7/unstructured/cleaners/extract.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/cleaners/translate.py` & `unstructured-0.8.7/unstructured/cleaners/translate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/documents/base.py` & `unstructured-0.8.7/unstructured/documents/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/documents/coordinates.py` & `unstructured-0.8.7/unstructured/documents/coordinates.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/documents/elements.py` & `unstructured-0.8.7/unstructured/documents/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/documents/email_elements.py` & `unstructured-0.8.7/unstructured/documents/email_elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/documents/html.py` & `unstructured-0.8.7/unstructured/documents/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/documents/xml.py` & `unstructured-0.8.7/unstructured/documents/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/file_utils/encoding.py` & `unstructured-0.8.7/unstructured/file_utils/encoding.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/file_utils/exploration.py` & `unstructured-0.8.7/unstructured/file_utils/exploration.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/file_utils/file_conversion.py` & `unstructured-0.8.7/unstructured/file_utils/file_conversion.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/file_utils/filetype.py` & `unstructured-0.8.7/unstructured/file_utils/filetype.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/file_utils/metadata.py` & `unstructured-0.8.7/unstructured/file_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/ingest/connector/azure.py` & `unstructured-0.8.7/unstructured/ingest/connector/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/ingest/connector/biomed.py` & `unstructured-0.8.7/unstructured/ingest/connector/biomed.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/ingest/connector/confluence.py` & `unstructured-0.8.7/unstructured/ingest/connector/confluence.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/ingest/connector/discord.py` & `unstructured-0.8.7/unstructured/ingest/connector/discord.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/ingest/connector/dropbox.py` & `unstructured-0.8.7/unstructured/ingest/connector/dropbox.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/ingest/connector/elasticsearch.py` & `unstructured-0.8.7/unstructured/ingest/connector/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/ingest/connector/fsspec.py` & `unstructured-0.8.7/unstructured/ingest/connector/fsspec.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/ingest/connector/gcs.py` & `unstructured-0.8.7/unstructured/ingest/connector/gcs.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/ingest/connector/git.py` & `unstructured-0.8.7/unstructured/ingest/connector/git.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/ingest/connector/github.py` & `unstructured-0.8.7/unstructured/ingest/connector/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/ingest/connector/gitlab.py` & `unstructured-0.8.7/unstructured/ingest/connector/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/ingest/connector/google_drive.py` & `unstructured-0.8.7/unstructured/ingest/connector/google_drive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/ingest/connector/local.py` & `unstructured-0.8.7/unstructured/ingest/connector/local.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/ingest/connector/onedrive.py` & `unstructured-0.8.7/unstructured/ingest/connector/onedrive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/ingest/connector/outlook.py` & `unstructured-0.8.7/unstructured/ingest/connector/outlook.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/ingest/connector/reddit.py` & `unstructured-0.8.7/unstructured/ingest/connector/reddit.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/ingest/connector/s3.py` & `unstructured-0.8.7/unstructured/ingest/connector/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/ingest/connector/slack.py` & `unstructured-0.8.7/unstructured/ingest/connector/slack.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/ingest/connector/wikipedia.py` & `unstructured-0.8.7/unstructured/ingest/connector/wikipedia.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/ingest/doc_processor/generalized.py` & `unstructured-0.8.7/unstructured/ingest/doc_processor/generalized.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/ingest/interfaces.py` & `unstructured-0.8.7/unstructured/ingest/interfaces.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/ingest/main.py` & `unstructured-0.8.7/unstructured/ingest/main.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/nlp/english-words.txt` & `unstructured-0.8.7/unstructured/nlp/english-words.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/nlp/english_words.py` & `unstructured-0.8.7/unstructured/nlp/english_words.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/nlp/patterns.py` & `unstructured-0.8.7/unstructured/nlp/patterns.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/nlp/tokenize.py` & `unstructured-0.8.7/unstructured/nlp/tokenize.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,30 +22,33 @@
     except LookupError:
         nltk.download(package_name)
 
 
 @lru_cache(maxsize=CACHE_MAX_SIZE)
 def sent_tokenize(text: str) -> List[str]:
     """A wrapper around the NLTK sentence tokenizer with LRU caching enabled."""
-    _download_nltk_package_if_not_present("tokenizers", "punkt")
+    _download_nltk_package_if_not_present(package_category="tokenizers", package_name="punkt")
     return _sent_tokenize(text)
 
 
 @lru_cache(maxsize=CACHE_MAX_SIZE)
 def word_tokenize(text: str) -> List[str]:
     """A wrapper around the NLTK word tokenizer with LRU caching enabled."""
-    _download_nltk_package_if_not_present("tokenizers", "punkt")
+    _download_nltk_package_if_not_present(package_category="tokenizers", package_name="punkt")
     return _word_tokenize(text)
 
 
 @lru_cache(maxsize=CACHE_MAX_SIZE)
 def pos_tag(text: str) -> List[Tuple[str, str]]:
     """A wrapper around the NLTK POS tagger with LRU caching enabled."""
-    _download_nltk_package_if_not_present("tokenizers", "punkt")
-    _download_nltk_package_if_not_present("taggers", "averaged_perceptron_tagger")
+    _download_nltk_package_if_not_present(package_category="tokenizers", package_name="punkt")
+    _download_nltk_package_if_not_present(
+        package_category="taggers",
+        package_name="averaged_perceptron_tagger",
+    )
     # NOTE(robinson) - Splitting into sentences before tokenizing. The helps with
     # situations like "ITEM 1A. PROPERTIES" where "PROPERTIES" can be mistaken
     # for a verb because it looks like it's in verb form an "ITEM 1A." looks like the subject.
     sentences = _sent_tokenize(text)
     parts_of_speech = []
     for sentence in sentences:
         tokens = _word_tokenize(sentence)
```

### Comparing `unstructured-0.8.6/unstructured/partition/__init__.py` & `unstructured-0.8.7/unstructured/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/partition/api.py` & `unstructured-0.8.7/unstructured/partition/api.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/partition/auto.py` & `unstructured-0.8.7/unstructured/partition/auto.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/partition/common.py` & `unstructured-0.8.7/unstructured/partition/common.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/partition/csv.py` & `unstructured-0.8.7/unstructured/partition/csv.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/partition/doc.py` & `unstructured-0.8.7/unstructured/partition/doc.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/partition/docx.py` & `unstructured-0.8.7/unstructured/partition/docx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/partition/email.py` & `unstructured-0.8.7/unstructured/partition/email.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/partition/epub.py` & `unstructured-0.8.7/unstructured/partition/epub.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/partition/html.py` & `unstructured-0.8.7/unstructured/partition/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/partition/image.py` & `unstructured-0.8.7/unstructured/partition/image.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/partition/json.py` & `unstructured-0.8.7/unstructured/partition/json.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/partition/md.py` & `unstructured-0.8.7/unstructured/partition/md.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/partition/msg.py` & `unstructured-0.8.7/unstructured/partition/msg.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/partition/odt.py` & `unstructured-0.8.7/unstructured/partition/odt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/partition/org.py` & `unstructured-0.8.7/unstructured/partition/org.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/partition/pdf.py` & `unstructured-0.8.7/unstructured/partition/pdf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/partition/ppt.py` & `unstructured-0.8.7/unstructured/partition/ppt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/partition/pptx.py` & `unstructured-0.8.7/unstructured/partition/pptx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/partition/rst.py` & `unstructured-0.8.7/unstructured/partition/rst.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/partition/rtf.py` & `unstructured-0.8.7/unstructured/partition/rtf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/partition/strategies.py` & `unstructured-0.8.7/unstructured/partition/strategies.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/partition/text.py` & `unstructured-0.8.7/unstructured/partition/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,40 @@
     is_bulleted_text,
     is_possible_narrative_text,
     is_possible_title,
     is_us_city_state_zip,
 )
 
 
+def split_by_paragraph(
+    file_text: str,
+    min_partition: Optional[int] = 0,
+    max_partition: Optional[int] = 1500,
+) -> List[str]:
+    split_paragraphs = re.split(PARAGRAPH_PATTERN, file_text.strip())
+
+    paragraphs = combine_paragraphs_less_than_min(
+        split_paragraphs=split_paragraphs,
+        max_partition=max_partition,
+        min_partition=min_partition,
+    )
+
+    file_content = []
+
+    for paragraph in paragraphs:
+        file_content.extend(
+            split_content_to_fit_max(
+                content=paragraph,
+                max_partition=max_partition,
+            ),
+        )
+
+    return file_content
+
+
 def _split_in_half_at_breakpoint(
     content: str,
     breakpoint: str = " ",
 ) -> List[str]:
     """Splits a segment of content at the breakpoint closest to the middle"""
     mid = len(content) // 2
     for i in range(len(content) // 2):
@@ -222,32 +248,20 @@
         file_text = paragraph_grouper(file_text)
     else:
         file_text = group_broken_paragraphs(file_text)
 
     if min_partition is not None and len(file_text) < min_partition:
         raise ValueError("`min_partition` cannot be larger than the length of file contents.")
 
-    split_paragraphs = re.split(PARAGRAPH_PATTERN, file_text.strip())
-
-    paragraphs = combine_paragraphs_less_than_min(
-        split_paragraphs=split_paragraphs,
-        max_partition=max_partition,
+    file_content = split_by_paragraph(
+        file_text,
         min_partition=min_partition,
+        max_partition=max_partition,
     )
 
-    file_content = []
-
-    for paragraph in paragraphs:
-        file_content.extend(
-            split_content_to_fit_max(
-                content=paragraph,
-                max_partition=max_partition,
-            ),
-        )
-
     elements: List[Element] = []
     metadata = (
         ElementMetadata(
             filename=metadata_filename or filename,
             date=metadata_date or last_modification_date,
         )
         if include_metadata
```

### Comparing `unstructured-0.8.6/unstructured/partition/text_type.py` & `unstructured-0.8.7/unstructured/partition/text_type.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/partition/tsv.py` & `unstructured-0.8.7/unstructured/partition/tsv.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/partition/xlsx.py` & `unstructured-0.8.7/unstructured/partition/xlsx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/partition/xml.py` & `unstructured-0.8.7/unstructured/partition/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/staging/argilla.py` & `unstructured-0.8.7/unstructured/staging/argilla.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/staging/base.py` & `unstructured-0.8.7/unstructured/staging/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/staging/baseplate.py` & `unstructured-0.8.7/unstructured/staging/baseplate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/staging/datasaur.py` & `unstructured-0.8.7/unstructured/staging/datasaur.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/staging/huggingface.py` & `unstructured-0.8.7/unstructured/staging/huggingface.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/staging/label_box.py` & `unstructured-0.8.7/unstructured/staging/label_box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/staging/label_studio.py` & `unstructured-0.8.7/unstructured/staging/label_studio.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/staging/prodigy.py` & `unstructured-0.8.7/unstructured/staging/prodigy.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/staging/weaviate.py` & `unstructured-0.8.7/unstructured/staging/weaviate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured/utils.py` & `unstructured-0.8.7/unstructured/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured.egg-info/PKG-INFO` & `unstructured-0.8.7/unstructured.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.8.6
+Version: 0.8.7
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
-Metadata-Version: 2.1 Name: unstructured Version: 0.8.6 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.8.7 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
```

### Comparing `unstructured-0.8.6/unstructured.egg-info/SOURCES.txt` & `unstructured-0.8.7/unstructured.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.6/unstructured.egg-info/requires.txt` & `unstructured-0.8.7/unstructured.egg-info/requires.txt`

 * *Files identical despite different names*

