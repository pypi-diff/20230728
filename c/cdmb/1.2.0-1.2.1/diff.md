# Comparing `tmp/cdmb-1.2.0.tar.gz` & `tmp/cdmb-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdmb-1.2.0.tar", max compression
+gzip compressed data, was "cdmb-1.2.1.tar", max compression
```

## Comparing `cdmb-1.2.0.tar` & `cdmb-1.2.1.tar`

### file list

```diff
@@ -1,104 +1,113 @@
--rw-r--r--   0        0        0    19345 2023-07-18 08:48:03.514975 cdmb-1.2.0/LICENSE
--rw-r--r--   0        0        0    35035 2023-07-18 08:48:03.514975 cdmb-1.2.0/README.md
--rw-r--r--   0        0        0    65792 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/CommonDataModel.py
--rw-r--r--   0        0        0      991 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/__init__.py
--rw-r--r--   0        0        0     8532 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/cohort/Cohort.py
--rw-r--r--   0        0        0     4576 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/cohort/Crosswalks.py
--rw-r--r--   0        0        0      120 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/cohort/__init__.py
--rw-r--r--   0        0        0     2921 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/entities/Catalog.py
--rw-r--r--   0        0        0    15180 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/entities/Entity.py
--rw-r--r--   0        0        0    22831 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/entities/Rule.py
--rw-r--r--   0        0        0    10189 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/entities/RuleSet.py
--rw-r--r--   0        0        0    11975 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/entities/Variable.py
--rw-r--r--   0        0        0      498 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/entities/__init__.py
--rw-r--r--   0        0        0     4637 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/project/Author.py
--rw-r--r--   0        0        0    12717 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/project/Metadata.py
--rw-r--r--   0        0        0       33 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/project/__init__.py
--rw-r--r--   0        0        0     6027 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/relationships/Relationship.py
--rw-r--r--   0        0        0       28 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/relationships/__init__.py
--rw-r--r--   0        0        0     1786 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/templates/Utils.py
--rw-r--r--   0        0        0       21 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/templates/__init__.py
--rw-r--r--   0        0        0       50 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/templates/files/.gitignore
--rw-r--r--   0        0        0    18656 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/templates/files/LICENSE.md
--rw-r--r--   0        0        0     6080 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/templates/files/README.md
--rw-r--r--   0        0        0       41 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/templates/files/_quarto.yml
--rw-r--r--   0        0        0    10224 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/templates/files/check_load.py
--rw-r--r--   0        0        0     2947 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/templates/files/dqa.py
--rw-r--r--   0        0        0      151 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/templates/files/man_container_deployment.md
--rw-r--r--   0        0        0     2855 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/templates/files/r_report_template.qmd
--rw-r--r--   0        0        0    10161 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/templates/files/validator.py
--rw-r--r--   0        0        0     3228 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/templates/files/validator_report.qmd
--rw-r--r--   0        0        0      554 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/typing/CommonDataModelTyping.py
--rw-r--r--   0        0        0       36 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/typing/__init__.py
--rw-r--r--   0        0        0    12526 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/ui/UILauncher.py
--rw-r--r--   0        0        0       65 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/ui/__init__.py
--rw-r--r--   0        0        0   111554 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/0.83e0eb50.css
--rw-r--r--   0        0        0      412 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/2.b838d5a7.css
--rw-r--r--   0        0        0     4495 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/4.18440754.css
--rw-r--r--   0        0        0     3111 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/6.bf404883.css
--rw-r--r--   0        0        0       34 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/Indicator.1d121e74.css
--rw-r--r--   0        0        0   111782 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/_layout.f2858481.css
--rw-r--r--   0        0        0     4491 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/_page.11cd5570.css
--rw-r--r--   0        0        0      412 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/_page.b838d5a7.css
--rw-r--r--   0        0        0     3111 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/_page.bf404883.css
--rw-r--r--   0        0        0    12580 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/eu_flag.c3360867.jpg
--rw-r--r--   0        0        0    25582 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/favicon.157dca14.png
--rw-r--r--   0        0        0    77364 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-all-400-normal.1e3b098c.woff
--rw-r--r--   0        0        0     9104 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-cyrillic-400-normal.c7d433fd.woff2
--rw-r--r--   0        0        0    15772 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-cyrillic-ext-400-normal.3df7909e.woff2
--rw-r--r--   0        0        0    10520 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-greek-400-normal.a8be01ce.woff2
--rw-r--r--   0        0        0     7508 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-greek-ext-400-normal.9e2fe623.woff2
--rw-r--r--   0        0        0    16284 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-latin-400-normal.e43b3538.woff2
--rw-r--r--   0        0        0    11364 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-latin-ext-400-normal.6bfabd30.woff2
--rw-r--r--   0        0        0     1753 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/github.1ea8d62e.svg
--rw-r--r--   0        0        0    21305 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/logo_Data_Science_VPM.15dffd2d.png
--rw-r--r--   0        0        0    11196 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/logo_Data_Science_VPM.dcd54a0d.webp
--rw-r--r--   0        0        0     3663 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Alert.2febe6fa.js
--rw-r--r--   0        0        0    10431 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Button.68ac352c.js
--rw-r--r--   0        0        0     6362 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/CloseButton.0aecb936.js
--rw-r--r--   0        0        0    13044 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Divider.623c8765.js
--rw-r--r--   0        0        0     2206 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Fileupload.78d706fe.js
--rw-r--r--   0        0        0    15049 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/FloatingLabelInput.21cd1ebc.js
--rw-r--r--   0        0        0     1844 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Heading.759b5df3.js
--rw-r--r--   0        0        0      817 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Indicator.svelte_svelte_type_style_lang.e2c519f7.js
--rw-r--r--   0        0        0     9203 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Modal.b90503ef.js
--rw-r--r--   0        0        0    45009 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/SimpleGrid.f308d3bd.js
--rw-r--r--   0        0        0    41583 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Space.5d3c5051.js
--rw-r--r--   0        0        0     9044 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/TableHeadCell.a7fa45f2.js
--rw-r--r--   0        0        0     4606 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Textarea.17eddb3d.js
--rw-r--r--   0        0        0     1484 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Trash.33219cd3.js
--rw-r--r--   0        0        0    15089 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/combinator.becf7b0b.js
--rw-r--r--   0        0        0       27 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/environment.9aa685ef.js
--rw-r--r--   0        0        0      820 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/index.5b757cee.js
--rw-r--r--   0        0        0     1667 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/index.b7a14a97.js
--rw-r--r--   0        0        0    16042 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/index.d8ca07a9.js
--rw-r--r--   0        0        0     9918 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/navigation.8bb60df9.js
--rw-r--r--   0        0        0     2496 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/singletons.3dbe6478.js
--rw-r--r--   0        0        0      414 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/store.247e7f87.js
--rw-r--r--   0        0        0    11736 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/store.4d7a1ebc.js
--rw-r--r--   0        0        0      814 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/store.6cd3ab0e.js
--rw-r--r--   0        0        0     1379 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/store.c28f1804.js
--rw-r--r--   0        0        0      266 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/stores.d0e64236.js
--rw-r--r--   0        0        0     9868 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/entry/app.34f7a124.js
--rw-r--r--   0        0        0    23923 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/entry/start.07ad94a0.js
--rw-r--r--   0        0        0    13097 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/0.51906aee.js
--rw-r--r--   0        0        0      800 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/1.e22fd99e.js
--rw-r--r--   0        0        0    20534 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/2.7284b9d4.js
--rw-r--r--   0        0        0    27325 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/3.510394aa.js
--rw-r--r--   0        0        0    56093 2023-07-18 08:48:03.522975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/4.828fc947.js
--rw-r--r--   0        0        0   122218 2023-07-18 08:48:03.522975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/5.faf63ad8.js
--rw-r--r--   0        0        0    68782 2023-07-18 08:48:03.522975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/6.c31223f5.js
--rw-r--r--   0        0        0    61580 2023-07-18 08:48:03.522975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/7.56d911fb.js
--rw-r--r--   0        0        0    28637 2023-07-18 08:48:03.522975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/8.ed4ac5b3.js
--rw-r--r--   0        0        0       27 2023-07-18 08:48:03.522975 cdmb-1.2.0/cdmb/ui/static_ui/_app/version.json
--rw-r--r--   0        0        0    13602 2023-07-18 08:48:03.522975 cdmb-1.2.0/cdmb/ui/static_ui/about.html
--rw-r--r--   0        0        0    17310 2023-07-18 08:48:03.522975 cdmb-1.2.0/cdmb/ui/static_ui/cohort.html
--rw-r--r--   0        0        0     5151 2023-07-18 08:48:03.522975 cdmb-1.2.0/cdmb/ui/static_ui/entities.html
--rw-r--r--   0        0        0    25582 2023-07-18 08:48:03.522975 cdmb-1.2.0/cdmb/ui/static_ui/favicon.png
--rw-r--r--   0        0        0    10045 2023-07-18 08:48:03.522975 cdmb-1.2.0/cdmb/ui/static_ui/index.html
--rw-r--r--   0        0        0    21009 2023-07-18 08:48:03.522975 cdmb-1.2.0/cdmb/ui/static_ui/project.html
--rw-r--r--   0        0        0       67 2023-07-18 08:48:03.522975 cdmb-1.2.0/cdmb/ui/static_ui/robots.txt
--rw-r--r--   0        0        0    15250 2023-07-18 08:48:03.522975 cdmb-1.2.0/cdmb/ui/static_ui/summary.html
--rw-r--r--   0        0        0     8887 2023-07-18 08:48:03.522975 cdmb-1.2.0/cdmb/ui/static_ui/validation.html
--rw-r--r--   0        0        0     1472 2023-07-18 08:48:03.522975 cdmb-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    36684 1970-01-01 00:00:00.000000 cdmb-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    19345 2023-07-28 08:42:03.835159 cdmb-1.2.1/LICENSE
+-rw-r--r--   0        0        0    35035 2023-07-28 08:42:03.835159 cdmb-1.2.1/README.md
+-rw-r--r--   0        0        0    65792 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/CommonDataModel.py
+-rw-r--r--   0        0        0      991 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/__init__.py
+-rw-r--r--   0        0        0     8532 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/cohort/Cohort.py
+-rw-r--r--   0        0        0     4576 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/cohort/Crosswalks.py
+-rw-r--r--   0        0        0      120 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/cohort/__init__.py
+-rw-r--r--   0        0        0     2921 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/entities/Catalog.py
+-rw-r--r--   0        0        0    15180 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/entities/Entity.py
+-rw-r--r--   0        0        0    22831 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/entities/Rule.py
+-rw-r--r--   0        0        0    10189 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/entities/RuleSet.py
+-rw-r--r--   0        0        0    11975 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/entities/Variable.py
+-rw-r--r--   0        0        0      498 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/entities/__init__.py
+-rw-r--r--   0        0        0     4637 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/project/Author.py
+-rw-r--r--   0        0        0    12717 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/project/Metadata.py
+-rw-r--r--   0        0        0       33 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/project/__init__.py
+-rw-r--r--   0        0        0     6027 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/relationships/Relationship.py
+-rw-r--r--   0        0        0       28 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/relationships/__init__.py
+-rw-r--r--   0        0        0     1786 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/templates/Utils.py
+-rw-r--r--   0        0        0       21 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/templates/__init__.py
+-rw-r--r--   0        0        0       50 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/templates/files/.gitignore
+-rw-r--r--   0        0        0    18656 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/templates/files/LICENSE.md
+-rw-r--r--   0        0        0     6145 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/templates/files/README.md
+-rw-r--r--   0        0        0       41 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/templates/files/_quarto.yml
+-rw-r--r--   0        0        0    11437 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/templates/files/check_load.py
+-rw-r--r--   0        0        0     3022 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/templates/files/dqa.py
+-rw-r--r--   0        0        0      151 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/templates/files/man_container_deployment.md
+-rw-r--r--   0        0        0     2855 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/templates/files/r_report_template.qmd
+-rw-r--r--   0        0        0    10160 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/templates/files/validator.py
+-rw-r--r--   0        0        0     3249 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/templates/files/validator_report.qmd
+-rw-r--r--   0        0        0      554 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/typing/CommonDataModelTyping.py
+-rw-r--r--   0        0        0       36 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/typing/__init__.py
+-rw-r--r--   0        0        0    12526 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/ui/UILauncher.py
+-rw-r--r--   0        0        0       65 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/ui/__init__.py
+-rw-r--r--   0        0        0   111554 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/0.83e0eb50.css
+-rw-r--r--   0        0        0      412 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/2.b838d5a7.css
+-rw-r--r--   0        0        0     4495 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/4.18440754.css
+-rw-r--r--   0        0        0     3111 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/6.bf404883.css
+-rw-r--r--   0        0        0       34 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/Indicator.1d121e74.css
+-rw-r--r--   0        0        0   111782 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/_layout.f2858481.css
+-rw-r--r--   0        0        0     4491 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/_page.11cd5570.css
+-rw-r--r--   0        0        0      412 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/_page.b838d5a7.css
+-rw-r--r--   0        0        0     3111 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/_page.bf404883.css
+-rw-r--r--   0        0        0    12580 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/eu_flag.c3360867.jpg
+-rw-r--r--   0        0        0    25582 2023-07-28 08:42:03.839159 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/favicon.157dca14.png
+-rw-r--r--   0        0        0    77364 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-all-400-normal.1e3b098c.woff
+-rw-r--r--   0        0        0     9104 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-cyrillic-400-normal.c7d433fd.woff2
+-rw-r--r--   0        0        0    15772 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-cyrillic-ext-400-normal.3df7909e.woff2
+-rw-r--r--   0        0        0    10520 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-greek-400-normal.a8be01ce.woff2
+-rw-r--r--   0        0        0     7508 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-greek-ext-400-normal.9e2fe623.woff2
+-rw-r--r--   0        0        0    16284 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-latin-400-normal.e43b3538.woff2
+-rw-r--r--   0        0        0    11364 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-latin-ext-400-normal.6bfabd30.woff2
+-rw-r--r--   0        0        0     1753 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/github.1ea8d62e.svg
+-rw-r--r--   0        0        0    21305 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/logo_Data_Science_VPM.15dffd2d.png
+-rw-r--r--   0        0        0    11196 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/logo_Data_Science_VPM.dcd54a0d.webp
+-rw-r--r--   0        0        0     3663 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/Alert.2febe6fa.js
+-rw-r--r--   0        0        0    10431 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/Button.68ac352c.js
+-rw-r--r--   0        0        0     6362 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/CloseButton.0aecb936.js
+-rw-r--r--   0        0        0    13044 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/Divider.623c8765.js
+-rw-r--r--   0        0        0     2206 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/Fileupload.78d706fe.js
+-rw-r--r--   0        0        0    15049 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/FloatingLabelInput.21cd1ebc.js
+-rw-r--r--   0        0        0     1844 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/Heading.759b5df3.js
+-rw-r--r--   0        0        0      817 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/Indicator.svelte_svelte_type_style_lang.e2c519f7.js
+-rw-r--r--   0        0        0     9203 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/Modal.b90503ef.js
+-rw-r--r--   0        0        0    45009 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/SimpleGrid.f308d3bd.js
+-rw-r--r--   0        0        0    41583 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/Space.5d3c5051.js
+-rw-r--r--   0        0        0     9044 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/TableHeadCell.a7fa45f2.js
+-rw-r--r--   0        0        0     4606 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/Textarea.17eddb3d.js
+-rw-r--r--   0        0        0     1484 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/Trash.33219cd3.js
+-rw-r--r--   0        0        0    15089 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/combinator.becf7b0b.js
+-rw-r--r--   0        0        0       27 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/environment.9aa685ef.js
+-rw-r--r--   0        0        0      820 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/index.5b757cee.js
+-rw-r--r--   0        0        0     1667 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/index.b7a14a97.js
+-rw-r--r--   0        0        0    16042 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/index.d8ca07a9.js
+-rw-r--r--   0        0        0     9918 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/navigation.6f463652.js
+-rw-r--r--   0        0        0     2498 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/singletons.786bc78c.js
+-rw-r--r--   0        0        0      414 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/store.247e7f87.js
+-rw-r--r--   0        0        0    11736 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/store.4d7a1ebc.js
+-rw-r--r--   0        0        0      814 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/store.6cd3ab0e.js
+-rw-r--r--   0        0        0     1379 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/store.c28f1804.js
+-rw-r--r--   0        0        0      266 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/stores.9ff5ee36.js
+-rw-r--r--   0        0        0     9868 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/entry/app.34f7a124.js
+-rw-r--r--   0        0        0     9868 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/entry/app.dbae3456.js
+-rw-r--r--   0        0        0    23923 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/entry/start.07ad94a0.js
+-rw-r--r--   0        0        0    23923 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/entry/start.124d4eb5.js
+-rw-r--r--   0        0        0    13097 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/nodes/0.51906aee.js
+-rw-r--r--   0        0        0    13097 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/nodes/0.5b2f9699.js
+-rw-r--r--   0        0        0      800 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/nodes/1.29a1247d.js
+-rw-r--r--   0        0        0      800 2023-07-28 08:42:03.843160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/nodes/1.e22fd99e.js
+-rw-r--r--   0        0        0    20534 2023-07-28 08:42:03.847160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/nodes/2.7284b9d4.js
+-rw-r--r--   0        0        0    27325 2023-07-28 08:42:03.847160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/nodes/3.510394aa.js
+-rw-r--r--   0        0        0    56093 2023-07-28 08:42:03.847160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/nodes/4.828fc947.js
+-rw-r--r--   0        0        0    56093 2023-07-28 08:42:03.847160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/nodes/4.afb48e27.js
+-rw-r--r--   0        0        0   122218 2023-07-28 08:42:03.847160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/nodes/5.18dad174.js
+-rw-r--r--   0        0        0   122218 2023-07-28 08:42:03.847160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/nodes/5.faf63ad8.js
+-rw-r--r--   0        0        0    68796 2023-07-28 08:42:03.847160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/nodes/6.bc3f5285.js
+-rw-r--r--   0        0        0    68782 2023-07-28 08:42:03.847160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/nodes/6.c31223f5.js
+-rw-r--r--   0        0        0    61580 2023-07-28 08:42:03.847160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/nodes/7.56d911fb.js
+-rw-r--r--   0        0        0    61580 2023-07-28 08:42:03.847160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/nodes/7.ce4f2d9c.js
+-rw-r--r--   0        0        0    28651 2023-07-28 08:42:03.847160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/nodes/8.1e29d0ba.js
+-rw-r--r--   0        0        0    28637 2023-07-28 08:42:03.847160 cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/nodes/8.ed4ac5b3.js
+-rw-r--r--   0        0        0       27 2023-07-28 08:42:03.847160 cdmb-1.2.1/cdmb/ui/static_ui/_app/version.json
+-rw-r--r--   0        0        0    13602 2023-07-28 08:42:03.847160 cdmb-1.2.1/cdmb/ui/static_ui/about.html
+-rw-r--r--   0        0        0    17310 2023-07-28 08:42:03.847160 cdmb-1.2.1/cdmb/ui/static_ui/cohort.html
+-rw-r--r--   0        0        0     5151 2023-07-28 08:42:03.847160 cdmb-1.2.1/cdmb/ui/static_ui/entities.html
+-rw-r--r--   0        0        0    25582 2023-07-28 08:42:03.847160 cdmb-1.2.1/cdmb/ui/static_ui/favicon.png
+-rw-r--r--   0        0        0    10046 2023-07-28 08:42:03.851160 cdmb-1.2.1/cdmb/ui/static_ui/index.html
+-rw-r--r--   0        0        0    21010 2023-07-28 08:42:03.851160 cdmb-1.2.1/cdmb/ui/static_ui/project.html
+-rw-r--r--   0        0        0       67 2023-07-28 08:42:03.851160 cdmb-1.2.1/cdmb/ui/static_ui/robots.txt
+-rw-r--r--   0        0        0    15250 2023-07-28 08:42:03.851160 cdmb-1.2.1/cdmb/ui/static_ui/summary.html
+-rw-r--r--   0        0        0     8887 2023-07-28 08:42:03.851160 cdmb-1.2.1/cdmb/ui/static_ui/validation.html
+-rw-r--r--   0        0        0     1472 2023-07-28 08:42:03.851160 cdmb-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0    36684 1970-01-01 00:00:00.000000 cdmb-1.2.1/PKG-INFO
```

### Comparing `cdmb-1.2.0/LICENSE` & `cdmb-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/README.md` & `cdmb-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/CommonDataModel.py` & `cdmb-1.2.1/cdmb/CommonDataModel.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/__init__.py` & `cdmb-1.2.1/cdmb/__init__.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/cohort/Cohort.py` & `cdmb-1.2.1/cdmb/cohort/Cohort.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/cohort/Crosswalks.py` & `cdmb-1.2.1/cdmb/cohort/Crosswalks.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/entities/Catalog.py` & `cdmb-1.2.1/cdmb/entities/Catalog.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/entities/Entity.py` & `cdmb-1.2.1/cdmb/entities/Entity.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/entities/Rule.py` & `cdmb-1.2.1/cdmb/entities/Rule.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/entities/RuleSet.py` & `cdmb-1.2.1/cdmb/entities/RuleSet.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/entities/Variable.py` & `cdmb-1.2.1/cdmb/entities/Variable.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/project/Author.py` & `cdmb-1.2.1/cdmb/project/Author.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/project/Metadata.py` & `cdmb-1.2.1/cdmb/project/Metadata.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/relationships/Relationship.py` & `cdmb-1.2.1/cdmb/relationships/Relationship.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/templates/Utils.py` & `cdmb-1.2.1/cdmb/templates/Utils.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/templates/files/LICENSE.md` & `cdmb-1.2.1/cdmb/templates/files/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/templates/files/README.md` & `cdmb-1.2.1/cdmb/templates/files/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ![Logo of the project](https://cienciadedatosysalud.org/wp-content/uploads/logo-Data-Science-VPM.png)
 
-<small><i>This project follows the structure build using the [Common Data Model Builder](https://github.com/cienciadedatosysalud/cdmb), a tool that allows you to create common data models to facilitate interoperability and reproducibility of the analyses.</i></small>
+<small><i>This project follows the structure built using the [Common Data Model Builder](https://github.com/cienciadedatosysalud/cdmb), a tool that allows you to create common data models to facilitate interoperability and reproducibility of the analyses.</i></small>
 
 
 # Your project title
 
 ---
 
 # Outputs
@@ -72,23 +72,23 @@
 
 
 # Authoring
 
 | Surname, name | Affiliation | ![orcid](https://orcid.org/sites/default/files/images/orcid_16x16.png) ORCID |
 |---------------|-------------|------------------------------------------------------------------------------|
 
-
+# Previous version(s):
 
 # How to contribute
 - Repository: https://github.com/your_user/your_repository/
 - Issue tracker: https://github.com/your_user/your_repository/issues
 
 # References
 - Data Science for Health Services and Policy Research group: https://cienciadedatosysalud.org/en/
 - Common Data Model Builder library :https://github.com/cienciadedatosysalud/cdmb
 - Analytic Software Pipeline Interface for Reproducible Execution (ASPIRE): https://github.com/cienciadedatosysalud/ASPIRE
-- ORCID: https://orcid.org/
-- Zenodo: https://zenodo.org/
+- Atlas VPM community in Zenodo: https://zenodo.org/communities/atlasvpm
 - Research Object Crate (RO-Crate): https://www.researchobject.org/ro-crate/
+- ORCID: https://orcid.org/
 
 <a href="https://creativecommons.org/licenses/by/4.0/" target="_blank" ><img src="https://img.shields.io/badge/license-CC--BY%204.0-lightgrey" alt="License: CC-BY 4.0"></a>
```

### Comparing `cdmb-1.2.0/cdmb/templates/files/check_load.py` & `cdmb-1.2.1/cdmb/templates/files/check_load.py`

 * *Files 16% similar despite different names*

```diff
@@ -84,14 +84,40 @@
         else:
             logging.warning(f"Format '{f}' not found, will be interpreted as String object.")
             dtype_[c] = pd.StringDtype()
     df = read_file(entity_structure, dtype_, parse_dates)
     load_file(entity_structure, df)
 
 
+def create_entity_table_if_not_exists(entity_name_, entity_variables_, entity_formats_):
+    format_translation = {
+        "string": "VARCHAR",
+        "boolean": "BOOLEAN",
+        "date": "DATE",
+        "datetime": "TIMESTAMP",
+        "integer": "BIGINT",
+        "double": "DOUBLE"
+    }
+    query = f"""CREATE TABLE IF NOT EXISTS {entity_name_}({entity_variables_[0]} {format_translation.get(entity_formats_[0], "VARCHAR")}"""
+    for (variable_, format_) in zip(entity_variables_[1:], entity_formats_[1:]):
+        query += f""", {variable_} {format_translation.get(format_)}"""
+    query += ");"
+    try:
+        logging.info(f"Trying to connect to the database ...")
+        logging.info(f"Trying to create the table for entity \"{entity_name_}\"")
+        logging.info(f"Table structure:\n {query}")
+        con = duckdb.connect(database_path, read_only=False)
+        con.execute(query)
+        logging.info(f"Table successfully created!")
+    except Exception as e:
+        logging.error("Something went wrong in the creation of the table")
+        logging.error(str(e))
+    finally:
+        con.close()
+
 def create_entity_table(entity_name_, entity_variables_, entity_formats_):
     format_translation = {
         "string": "VARCHAR",
         "boolean": "BOOLEAN",
         "date": "DATE",
         "datetime": "TIMESTAMP",
         "integer": "BIGINT",
@@ -162,14 +188,15 @@
                 logging.error("properties \"name\" or \"variables\" not found in entity! Check specifications!")
                 exit(1)
             entity_name = entity['name']
             logging.info(f"Processing entity \"{entity_name}\"...")
             try:
                 entity_variables = [variable['label'] for variable in entity['variables']]
                 entity_formats = [str(variable['format']).lower() for variable in entity['variables']]
+                create_entity_table_if_not_exists(entity_name,entity_variables,entity_formats)
             except Exception as e:
                 logging.error("Variables must have the properties \"label\" and \"format\"")
                 logging.error(str(e))
                 exit(1)
 
             uploaded_filename_ = None
             uploaded_filename_list = []
```

### Comparing `cdmb-1.2.0/cdmb/templates/files/dqa.py` & `cdmb-1.2.1/cdmb/templates/files/dqa.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,19 +48,20 @@
             logging.error("properties \"name\" not found in entity! Check specifications!")
             exit(1)
         entity_name = entity['name']
         title = configuration_file['metadata']['use_case'] + ' - ' + entity_name + ' | Profiling Report'
         query = "Select * from {entity}".format(entity=entity_name)
         df_entity = con.query(query).to_df()
         logging.info(f"\"{entity_name}\" entity contains {len(df_entity)} records")
-        profile = ProfileReport(df_entity, title=title, minimal=True)
-        html_out = os.path.join(output_path, "dqa_{usecase}_{entity_}.html".format(
-            usecase=use_case_name,
-            entity_=str(entity_name).replace(' ', '_')
-        ))
-        json_out = os.path.join(output_path, "dqa_{usecase}_{entity_}.json".format(
-            usecase=use_case_name,
-            entity_=str(entity_name).replace(' ', '_')
-        ))
-        profile.to_file(html_out)
-        profile.to_file(json_out)
+        if len(df_entity) > 0:
+            profile = ProfileReport(df_entity, title=title, minimal=True)
+            html_out = os.path.join(output_path, "dqa_{usecase}_{entity_}.html".format(
+                usecase=use_case_name,
+                entity_=str(entity_name).replace(' ', '_')
+            ))
+            json_out = os.path.join(output_path, "dqa_{usecase}_{entity_}.json".format(
+                usecase=use_case_name,
+                entity_=str(entity_name).replace(' ', '_')
+            ))
+            profile.to_file(html_out)
+            profile.to_file(json_out)
     con.close()
```

### Comparing `cdmb-1.2.0/cdmb/templates/files/r_report_template.qmd` & `cdmb-1.2.1/cdmb/templates/files/r_report_template.qmd`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/templates/files/validator.py` & `cdmb-1.2.1/cdmb/templates/files/validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,14 @@
                     "total_wrong_lines": result_entity['total_registries']
                 })
                 pass
 
         result_entity['rules'] = result_rules
         response.append(result_entity)
         con.execute(f"DROP VIEW IF EXISTS {view_name};")
-
     try:
         with open(os.path.join(output_path, 'validator_output.json'), 'w') as f:
             json_object = json.dumps({'info':response}, indent=4)
             f.write(json_object)
             logging.info(f"validator_output.json created.")
     except Exception as e:
         logging.error(f"Something went wrong trying to write \"validator_output\" files")
```

### Comparing `cdmb-1.2.0/cdmb/templates/files/validator_report.qmd` & `cdmb-1.2.1/cdmb/templates/files/validator_report.qmd`

 * *Files 18% similar despite different names*

```diff
@@ -87,24 +87,24 @@
   
   cat("\n <hr/>")
   cat("### Validation against catalogs \n")
   df2 <- as.data.frame(catalog_checking_df[i])
   df2$total_wrong_lines <- cell_spec(df2$total_wrong_lines, background = ifelse(df2$total_wrong_lines > (0.2*entities_total_registries[i]), "orange", ""))
   
   cat(df2 %>%
-  kbl(., "html", escape = F, col.names = c("Variable label", "Wrong values","No. wrong registries","Line number")) %>%  kable_styling(bootstrap_options = c("striped", "hover", "responsive"), full_width = T))
+  kbl(., "html", escape = F, col.names = c("Variable label", "Wrong values","Fails (line number)","Number of lines")) %>%  kable_styling(bootstrap_options = c("striped", "hover", "responsive"), full_width = T))
   
   
   cat("\n <hr/>")
   cat("### Validation of rules\n")
   df3 <- as.data.frame(rules_df[i])
 
   df3$total_wrong_lines <- cell_spec(df3$total_wrong_lines, background = ifelse(df3$total_wrong_lines > (0.2*entities_total_registries[i]), "orange", ""))
    cat(df3 %>%
-  kbl(., "html", escape = F, col.names = c("Rule", "Passes","Fails","Line number")) %>%  kable_styling(bootstrap_options = c("striped", "hover", "responsive"), full_width = T))
+  kbl(., "html", escape = F, col.names = c("Rule", "Passes","Fails (line number)","Number of lines")) %>%  kable_styling(bootstrap_options = c("striped", "hover", "responsive"), full_width = T))
   cat("\n \n")
 
 }
   cat(":::")
 
 ```
```

### Comparing `cdmb-1.2.0/cdmb/typing/CommonDataModelTyping.py` & `cdmb-1.2.1/cdmb/typing/CommonDataModelTyping.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/UILauncher.py` & `cdmb-1.2.1/cdmb/ui/UILauncher.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/0.83e0eb50.css` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/0.83e0eb50.css`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/4.18440754.css` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/4.18440754.css`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/6.bf404883.css` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/6.bf404883.css`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/_layout.f2858481.css` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/_layout.f2858481.css`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/_page.11cd5570.css` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/_page.11cd5570.css`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/_page.bf404883.css` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/_page.bf404883.css`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/eu_flag.c3360867.jpg` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/eu_flag.c3360867.jpg`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/favicon.157dca14.png` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/favicon.157dca14.png`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-all-400-normal.1e3b098c.woff` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-all-400-normal.1e3b098c.woff`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-cyrillic-400-normal.c7d433fd.woff2` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-cyrillic-400-normal.c7d433fd.woff2`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-cyrillic-ext-400-normal.3df7909e.woff2` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-cyrillic-ext-400-normal.3df7909e.woff2`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-greek-400-normal.a8be01ce.woff2` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-greek-400-normal.a8be01ce.woff2`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-greek-ext-400-normal.9e2fe623.woff2` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-greek-ext-400-normal.9e2fe623.woff2`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-latin-400-normal.e43b3538.woff2` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-latin-400-normal.e43b3538.woff2`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-latin-ext-400-normal.6bfabd30.woff2` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-latin-ext-400-normal.6bfabd30.woff2`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/github.1ea8d62e.svg` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/github.1ea8d62e.svg`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/logo_Data_Science_VPM.15dffd2d.png` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/logo_Data_Science_VPM.15dffd2d.png`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/logo_Data_Science_VPM.dcd54a0d.webp` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/assets/logo_Data_Science_VPM.dcd54a0d.webp`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Alert.2febe6fa.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/Alert.2febe6fa.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Button.68ac352c.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/Button.68ac352c.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/CloseButton.0aecb936.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/CloseButton.0aecb936.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Divider.623c8765.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/Divider.623c8765.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Fileupload.78d706fe.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/Fileupload.78d706fe.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/FloatingLabelInput.21cd1ebc.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/FloatingLabelInput.21cd1ebc.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Heading.759b5df3.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/Heading.759b5df3.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Indicator.svelte_svelte_type_style_lang.e2c519f7.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/Indicator.svelte_svelte_type_style_lang.e2c519f7.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Modal.b90503ef.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/Modal.b90503ef.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/SimpleGrid.f308d3bd.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/SimpleGrid.f308d3bd.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Space.5d3c5051.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/Space.5d3c5051.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/TableHeadCell.a7fa45f2.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/TableHeadCell.a7fa45f2.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Textarea.17eddb3d.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/Textarea.17eddb3d.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Trash.33219cd3.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/Trash.33219cd3.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/combinator.becf7b0b.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/combinator.becf7b0b.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/index.5b757cee.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/index.5b757cee.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/index.b7a14a97.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/index.b7a14a97.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/index.d8ca07a9.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/index.d8ca07a9.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/navigation.8bb60df9.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/navigation.6f463652.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -42,15 +42,15 @@
     c as I
 } from "./Indicator.svelte_svelte_type_style_lang.e2c519f7.js";
 import {
     c as fe
 } from "./SimpleGrid.f308d3bd.js";
 import {
     j as ce
-} from "./singletons.3dbe6478.js";
+} from "./singletons.786bc78c.js";
 
 function de(n) {
     let e, t, a;
     const s = n[5].default,
         i = O(s, n, n[4], null);
     let o = [n[1], {
             class: t = I(n[0], n[2].class)
```

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/singletons.3dbe6478.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/singletons.786bc78c.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 import {
     w as c
 } from "./index.5b757cee.js";
 var _;
-const k = ((_ = globalThis.__sveltekit_hkc33l) == null ? void 0 : _.base) ?? "";
+const v = ((_ = globalThis.__sveltekit_101jss1) == null ? void 0 : _.base) ?? "";
 var h;
-const v = ((h = globalThis.__sveltekit_hkc33l) == null ? void 0 : h.assets) ?? k,
-    m = "1688566708786",
+const k = ((h = globalThis.__sveltekit_101jss1) == null ? void 0 : h.assets) ?? v,
+    m = "1690531797400",
     R = "sveltekit:snapshot",
     S = "sveltekit:scroll",
     T = "sveltekit:index",
     f = {
         tap: 1,
         hover: 2,
         viewport: 3,
@@ -71,43 +71,43 @@
 
 function U(e) {
     let t = null,
         n = null,
         a = null,
         l = null,
         r = null,
-        s = null,
-        o = e;
-    for (; o && o !== document.documentElement;) a === null && (a = i(o, "preload-code")), l === null && (l = i(o, "preload-data")), t === null && (t = i(o, "keepfocus")), n === null && (n = i(o, "noscroll")), r === null && (r = i(o, "reload")), s === null && (s = i(o, "replacestate")), o = g(o);
+        o = null,
+        s = e;
+    for (; s && s !== document.documentElement;) a === null && (a = i(s, "preload-code")), l === null && (l = i(s, "preload-data")), t === null && (t = i(s, "keepfocus")), n === null && (n = i(s, "noscroll")), r === null && (r = i(s, "reload")), o === null && (o = i(s, "replacestate")), s = g(s);
     return {
         preload_code: d[a ?? "off"],
         preload_data: d[l ?? "off"],
         keep_focus: t === "off" ? !1 : t === "" ? !0 : null,
         noscroll: n === "off" ? !1 : n === "" ? !0 : null,
         reload: r === "off" ? !1 : r === "" ? !0 : null,
-        replace_state: s === "off" ? !1 : s === "" ? !0 : null
+        replace_state: o === "off" ? !1 : o === "" ? !0 : null
     }
 }
 
 function p(e) {
     const t = c(e);
     let n = !0;
 
     function a() {
-        n = !0, t.update(s => s)
+        n = !0, t.update(o => o)
     }
 
-    function l(s) {
-        n = !1, t.set(s)
+    function l(o) {
+        n = !1, t.set(o)
     }
 
-    function r(s) {
-        let o;
+    function r(o) {
+        let s;
         return t.subscribe(u => {
-            (o === void 0 || n && u !== o) && s(o = u)
+            (s === void 0 || n && u !== s) && o(s = u)
         })
     }
     return {
         notify: a,
         set: l,
         subscribe: r
     }
@@ -118,23 +118,23 @@
         set: e,
         subscribe: t
     } = c(!1);
     let n;
     async function a() {
         clearTimeout(n);
         try {
-            const l = await fetch(`${v}/_app/version.json`, {
+            const l = await fetch(`${k}/_app/version.json`, {
                 headers: {
                     pragma: "no-cache",
                     "cache-control": "no-cache"
                 }
             });
             if (!l.ok) return !1;
-            const s = (await l.json()).version !== m;
-            return s && (e(!0), clearTimeout(n)), s
+            const o = (await l.json()).version !== m;
+            return o && (e(!0), clearTimeout(n)), o
         } catch {
             return !1
         }
     }
     return {
         subscribe: t,
         check: a
@@ -142,23 +142,23 @@
 }
 
 function E(e, t) {
     return e.origin !== location.origin || !e.pathname.startsWith(t)
 }
 let b;
 
-function L(e) {
+function j(e) {
     b = e.client
 }
 
-function N(e) {
+function L(e) {
     return (...t) => b[e](...t)
 }
-const P = {
+const N = {
     url: p({}),
     page: p({}),
     navigating: c(null),
     updated: w()
 };
 export {
-    T as I, f as P, S, R as a, O as b, U as c, I as d, k as e, x as f, y as g, L as h, E as i, N as j, P as s
+    T as I, f as P, S, R as a, O as b, U as c, I as d, v as e, x as f, y as g, j as h, E as i, L as j, N as s
 };
```

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/store.4d7a1ebc.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/store.4d7a1ebc.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/store.6cd3ab0e.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/store.6cd3ab0e.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/store.c28f1804.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/chunks/store.c28f1804.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/entry/app.34f7a124.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/entry/app.34f7a124.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/entry/start.07ad94a0.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/entry/start.07ad94a0.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/0.51906aee.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/nodes/0.51906aee.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/1.e22fd99e.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/nodes/1.e22fd99e.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/2.7284b9d4.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/nodes/2.7284b9d4.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/3.510394aa.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/nodes/3.510394aa.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/4.828fc947.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/nodes/4.828fc947.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/5.faf63ad8.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/nodes/5.faf63ad8.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/6.c31223f5.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/nodes/6.c31223f5.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/7.56d911fb.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/nodes/7.56d911fb.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/8.ed4ac5b3.js` & `cdmb-1.2.1/cdmb/ui/static_ui/_app/immutable/nodes/8.ed4ac5b3.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/about.html` & `cdmb-1.2.1/cdmb/ui/static_ui/about.html`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/cohort.html` & `cdmb-1.2.1/cdmb/ui/static_ui/cohort.html`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 	<div class="corner svelte-1xklbfh"><a href="https://github.com/cienciadedatosysalud" target="_blank" class="svelte-1xklbfh"><img src="/_app/immutable/assets/github.1ea8d62e.svg" alt="GitHub" class="svelte-1xklbfh"></a></div></header>
 
 
 
 
   <main class="svelte-nv0ll5">
-<div class="fixed right-6 bottom-6 group"><button type="button" name="Open actions menu" aria-controls="ljpt12ug" aria-expanded="false" class="text-center font-medium focus:ring-4 focus:outline-none inline-flex items-center justify-center px-5 py-2.5 text-sm text-white bg-yellow-400 hover:bg-yellow-500 focus:ring-yellow-300 dark:focus:ring-yellow-900 rounded-full !p-3">
+<div class="fixed right-6 bottom-6 group"><button type="button" name="Open actions menu" aria-controls="lkmazr6d" aria-expanded="false" class="text-center font-medium focus:ring-4 focus:outline-none inline-flex items-center justify-center px-5 py-2.5 text-sm text-white bg-yellow-400 hover:bg-yellow-500 focus:ring-yellow-300 dark:focus:ring-yellow-900 rounded-full !p-3">
       <svg aria-hidden="true" class="w-8 h-8 transition-transform group-hover:rotate-45" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6v6m0 0v6m0-6h6m-6 0H6"></path></svg>
     
     <span class="sr-only">Open actions menu</span></button>
   <div></div>
 
 </div>
 <h1>Cohort definition</h1>
@@ -97,20 +97,20 @@
 		<div class="inline-flex rounded-lg shadow-sm w-full" role="group">
   <textarea color="red" id="textarea-id2" placeholder="(If there are no exclusion criteria, write, for example, 'None' to express the absence of exclusion criteria)" rows="4" name="message" maxlength="500" class="w-full rounded-lg bg-gray-50 dark:bg-gray-700 text-gray-900 dark:placeholder-gray-400 dark:text-white  border border-gray-200 dark:border-gray-600 p-2.5 text-sm focus:ring-blue-500 focus:border-blue-500 dark:focus:ring-blue-500 dark:focus:border-blue-500"></textarea>
   
 			<div class="text-sm px-3 border-gray-300 dark:border-gray-600 text-gray-500 bg-gray-200 dark:bg-gray-600 dark:text-gray-400 dark:border-r-gray-700 dark:last:border-r-gray-600 inline-flex items-center border-t border-b first:border-l border-r first:rounded-l-lg last:rounded-r-lg">0/500</div></div></div>
 
 	<div>
   <label for="date-id1" class="text-sm font-medium block text-gray-900 dark:text-gray-300 mb-2">Beginning of study period</label>
-		<div class="date-time-field  svelte-1bsxr9h"><input type="text" value="2023-07-05" placeholder="2020-12-31 23:00:00"  class="svelte-1bsxr9h">
+		<div class="date-time-field  svelte-1bsxr9h"><input type="text" value="2023-07-28" placeholder="2020-12-31 23:00:00"  class="svelte-1bsxr9h">
   
 </div></div>
 	<div>
   <label for="date-id2" class="text-sm font-medium block text-gray-900 dark:text-gray-300 mb-2">End of study period</label>
-		<div class="date-time-field  svelte-1bsxr9h"><input type="text" value="2023-07-05" placeholder="2020-12-31 23:00:00"  class="svelte-1bsxr9h">
+		<div class="date-time-field  svelte-1bsxr9h"><input type="text" value="2023-07-28" placeholder="2020-12-31 23:00:00"  class="svelte-1bsxr9h">
   
 </div></div></div>
 
 
 
 <div class="svelteui-c-iGtvjx svelteui-c-iGtvjx-iPJLV-css svelteui-c-PJLV svelteui-c-PJLV-iPJLV-css"></div>
```

#### html2text {}

```diff
@@ -26,17 +26,17 @@
 Description is a required input
 Inclusion criteria *
 0/500
 Inclusion criteria is a required input
 Exclusion criteria
 0/500
 Beginning of study period
-[2023-07-05          ]
+[2023-07-28          ]
 End of study period
-[2023-07-05          ]
+[2023-07-28          ]
 Crosswalks
 ***** Upload your crosswalks files *****
 Download crosswalks template
 Cohort definition inclusions
 Nature [One of: Choose option .../Condition/Intervention/Drugs/Any]
 Column name [One of: Choose option ...]
 Upload your crosswalks file [File]
```

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/entities.html` & `cdmb-1.2.1/cdmb/ui/static_ui/entities.html`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 	<div class="corner svelte-1xklbfh"><a href="https://github.com/cienciadedatosysalud" target="_blank" class="svelte-1xklbfh"><img src="/_app/immutable/assets/github.1ea8d62e.svg" alt="GitHub" class="svelte-1xklbfh"></a></div></header>
 
 
 
 
   <main class="svelte-nv0ll5">
-<div class="fixed right-6 bottom-6 group"><button type="button" name="Open actions menu" aria-controls="ljpt12uh" aria-expanded="false" class="text-center font-medium focus:ring-4 focus:outline-none inline-flex items-center justify-center px-5 py-2.5 text-sm text-white bg-yellow-400 hover:bg-yellow-500 focus:ring-yellow-300 dark:focus:ring-yellow-900 rounded-full !p-3">
+<div class="fixed right-6 bottom-6 group"><button type="button" name="Open actions menu" aria-controls="lkmazr6e" aria-expanded="false" class="text-center font-medium focus:ring-4 focus:outline-none inline-flex items-center justify-center px-5 py-2.5 text-sm text-white bg-yellow-400 hover:bg-yellow-500 focus:ring-yellow-300 dark:focus:ring-yellow-900 rounded-full !p-3">
       <svg aria-hidden="true" class="w-8 h-8 transition-transform group-hover:rotate-45" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6v6m0 0v6m0-6h6m-6 0H6"></path></svg>
     
     <span class="sr-only">Open actions menu</span></button>
   <div></div>
 
 </div>
 <h1>Entities definition</h1>
```

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/favicon.png` & `cdmb-1.2.1/cdmb/ui/static_ui/favicon.png`

 * *Files identical despite different names*

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/index.html` & `cdmb-1.2.1/cdmb/ui/static_ui/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 	<meta charset="utf-8" />
 	<link rel="icon" href="./favicon.png" />
 	<meta name="viewport" content="width=device-width" />
 	<meta http-equiv="content-security-policy" content="">
 		<link href="./_app/immutable/assets/0.83e0eb50.css" rel="stylesheet">
 		<link href="./_app/immutable/assets/Indicator.1d121e74.css" rel="stylesheet">
 		<link href="./_app/immutable/assets/2.b838d5a7.css" rel="stylesheet">
-		<link rel="modulepreload" href="./_app/immutable/entry/start.07ad94a0.js">
+		<link rel="modulepreload" href="./_app/immutable/entry/start.124d4eb5.js">
 		<link rel="modulepreload" href="./_app/immutable/chunks/index.d8ca07a9.js">
-		<link rel="modulepreload" href="./_app/immutable/chunks/singletons.3dbe6478.js">
+		<link rel="modulepreload" href="./_app/immutable/chunks/singletons.786bc78c.js">
 		<link rel="modulepreload" href="./_app/immutable/chunks/index.5b757cee.js">
-		<link rel="modulepreload" href="./_app/immutable/entry/app.34f7a124.js">
-		<link rel="modulepreload" href="./_app/immutable/nodes/0.51906aee.js">
-		<link rel="modulepreload" href="./_app/immutable/chunks/stores.d0e64236.js">
+		<link rel="modulepreload" href="./_app/immutable/entry/app.dbae3456.js">
+		<link rel="modulepreload" href="./_app/immutable/nodes/0.5b2f9699.js">
+		<link rel="modulepreload" href="./_app/immutable/chunks/stores.9ff5ee36.js">
 		<link rel="modulepreload" href="./_app/immutable/chunks/Indicator.svelte_svelte_type_style_lang.e2c519f7.js">
 		<link rel="modulepreload" href="./_app/immutable/chunks/index.b7a14a97.js">
 		<link rel="modulepreload" href="./_app/immutable/chunks/Alert.2febe6fa.js">
 		<link rel="modulepreload" href="./_app/immutable/chunks/CloseButton.0aecb936.js">
 		<link rel="modulepreload" href="./_app/immutable/chunks/store.4d7a1ebc.js">
 		<link rel="modulepreload" href="./_app/immutable/nodes/2.7284b9d4.js">
 		<link rel="modulepreload" href="./_app/immutable/chunks/Space.5d3c5051.js">
@@ -197,26 +197,26 @@
 
 </div>
 
 
 			
 			<script>
 				{
-					__sveltekit_hkc33l = {
+					__sveltekit_101jss1 = {
 						base: new URL(".", location).pathname.slice(0, -1),
 						env: {}
 					};
 
 					const element = document.currentScript.parentElement;
 
 					const data = [null,null];
 
 					Promise.all([
-						import("./_app/immutable/entry/start.07ad94a0.js"),
-						import("./_app/immutable/entry/app.34f7a124.js")
+						import("./_app/immutable/entry/start.124d4eb5.js"),
+						import("./_app/immutable/entry/app.dbae3456.js")
 					]).then(([kit, app]) => {
 						kit.start(app, element, {
 							node_ids: [0, 2],
 							data,
 							form: null,
 							error: null
 						});
```

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/project.html` & `cdmb-1.2.1/cdmb/ui/static_ui/project.html`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 	<div class="corner svelte-1xklbfh"><a href="https://github.com/cienciadedatosysalud" target="_blank" class="svelte-1xklbfh"><img src="/_app/immutable/assets/github.1ea8d62e.svg" alt="GitHub" class="svelte-1xklbfh"></a></div></header>
 
 
 
 
   <main class="svelte-nv0ll5">
-<div class="fixed right-6 bottom-6 group"><button type="button" name="Open actions menu" aria-controls="ljpt12ui" aria-expanded="false" class="text-center font-medium focus:ring-4 focus:outline-none inline-flex items-center justify-center px-5 py-2.5 text-sm text-white bg-yellow-400 hover:bg-yellow-500 focus:ring-yellow-300 dark:focus:ring-yellow-900 rounded-full !p-3">
+<div class="fixed right-6 bottom-6 group"><button type="button" name="Open actions menu" aria-controls="lkmazr6f" aria-expanded="false" class="text-center font-medium focus:ring-4 focus:outline-none inline-flex items-center justify-center px-5 py-2.5 text-sm text-white bg-yellow-400 hover:bg-yellow-500 focus:ring-yellow-300 dark:focus:ring-yellow-900 rounded-full !p-3">
       <svg aria-hidden="true" class="w-8 h-8 transition-transform group-hover:rotate-45" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6v6m0 0v6m0-6h6m-6 0H6"></path></svg>
     
     <span class="sr-only">Open actions menu</span></button>
   <div></div>
 
 </div>
 
@@ -131,15 +131,15 @@
 	<div>
   <label class="text-sm font-medium block text-gray-900 dark:text-gray-300 mb-2" for="input-addon-md">Spatial coverage</label>
 		<div class="inline-flex rounded-lg shadow-sm w-full" role="group">
   
     <input placeholder="Spatial coverage" id="input-addon-md" maxlength="250" class="block w-full disabled:cursor-not-allowed disabled:opacity-50 focus:border-blue-500 focus:ring-blue-500 dark:focus:border-blue-500 dark:focus:ring-blue-500 bg-gray-50 text-gray-900 dark:bg-gray-700 dark:text-white dark:placeholder-gray-400 border-gray-300 dark:border-gray-600 p-2.5 text-sm size first:rounded-l-lg last:rounded-r-lg border-l-0 first:border-l last:border-r" value="">
   
   
-			<div class="text-sm px-3 border-gray-300 dark:border-gray-600 text-gray-500 bg-gray-200 dark:bg-gray-600 dark:text-gray-400 dark:border-r-gray-700 dark:last:border-r-gray-600 inline-flex items-center border-t border-b first:border-l border-r first:rounded-l-lg last:rounded-r-lg">/250</div></div></div>
+			<div class="text-sm px-3 border-gray-300 dark:border-gray-600 text-gray-500 bg-gray-200 dark:bg-gray-600 dark:text-gray-400 dark:border-r-gray-700 dark:last:border-r-gray-600 inline-flex items-center border-t border-b first:border-l border-r first:rounded-l-lg last:rounded-r-lg">0/250</div></div></div>
 	<div>
   <label class="text-sm font-medium block text-gray-900 dark:text-gray-300 mb-2" for="license_1">License</label>
 		<select id="license_1" class="block w-full text-gray-900 bg-gray-50 border border-gray-300 rounded-lg focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500 text-sm p-2.5 mt-2"><option disabled selected value="">Choose option ...</option><option value="CC BY 4.0 https://creativecommons.org/licenses/by/4.0/">CC BY 4.0 https://creativecommons.org/licenses/by/4.0/</option><option value="CC BY-SA 4.0 https://creativecommons.org/licenses/by-sa/4.0/">CC BY-SA 4.0 https://creativecommons.org/licenses/by-sa/4.0/</option><option value="CC BY-NC 4.0 https://creativecommons.org/licenses/by-nc/4.0/">CC BY-NC 4.0 https://creativecommons.org/licenses/by-nc/4.0/</option><option value="CC BY-NC-SA 4.0 https://creativecommons.org/licenses/by-nc-sa/4.0/">CC BY-NC-SA 4.0 https://creativecommons.org/licenses/by-nc-sa/4.0/</option><option value="CC BY-ND 4.0 https://creativecommons.org/licenses/by-nd/4.0/">CC BY-ND 4.0 https://creativecommons.org/licenses/by-nd/4.0/</option><option value="CC BY-NC-ND 4.0 https://creativecommons.org/licenses/by-nc-nd/4.0/">CC BY-NC-ND 4.0 https://creativecommons.org/licenses/by-nc-nd/4.0/</option><option value="CC0 1.0 https://creativecommons.org/publicdomain/zero/1.0/">CC0 1.0 https://creativecommons.org/publicdomain/zero/1.0/</option></select>
 		<p class="text-xs font-normal text-gray-500 dark:text-gray-300 text-gray-900 dark:text-gray-300 pt-2">For more information, visit
 			<a target="_blank" href="https://creativecommons.org/about/cclicenses/" class="text-blue-600 dark:text-blue-500 hover:underline">About CC Licenses</a>
 			.
 		</p></div></div>
@@ -194,18 +194,18 @@
 <div class="svelteui-Divider-horizontal svelteui-c-ggdQTf svelteui-c-ggdQTf-iPJLV-css svelteui-c-PJLV svelteui-c-PJLV-iPJLV-css"></div>
 
 
 
 <div class="svelteui-c-iGtvjx svelteui-c-iGtvjx-iPJLV-css svelteui-c-PJLV svelteui-c-PJLV-iPJLV-css"></div>
 <div>
   <label class="text-sm font-medium block text-gray-900 dark:text-gray-300 mb-2" for="input-addon-md">Keywords</label>
-	<div class="inline-flex rounded-lg shadow-sm" role="group"><div class="svelte-tags-input-layout svelte-1ubt6my"><label for="sti_j7cmai0bo" class="sr-only svelte-1ubt6my">svelte-tags-input</label>
+	<div class="inline-flex rounded-lg shadow-sm" role="group"><div class="svelte-tags-input-layout svelte-1ubt6my"><label for="sti_ff4ptxmtf" class="sr-only svelte-1ubt6my">svelte-tags-input</label>
 
     
-    <input type="text" id="sti_j7cmai0bo" name="svelte-tags-input" class="svelte-tags-input svelte-1ubt6my" placeholder=""  autocomplete="off" value=""></div>
+    <input type="text" id="sti_ff4ptxmtf" name="svelte-tags-input" class="svelte-tags-input svelte-1ubt6my" placeholder=""  autocomplete="off" value=""></div>
 
 
 		<div class="text-sm px-3 border-gray-300 dark:border-gray-600 text-gray-500 bg-gray-200 dark:bg-gray-600 dark:text-gray-400 dark:border-r-gray-700 dark:last:border-r-gray-600 inline-flex items-center border-t border-b first:border-l border-r first:rounded-l-lg last:rounded-r-lg">0/10</div></div>
 	<p class="text-xs font-normal text-gray-500 dark:text-gray-300 text-gray-900 dark:text-gray-300 pt-2">Press ENTER to add a new one.</p></div>
```

#### html2text {}

```diff
@@ -41,15 +41,15 @@
 [                    ]
 0/250
 Version does not comply with the semantic versioning Semantic Versioning 2.0.0
 format
 For more information, visit Semantic_Versioning_2.0.0 .
 Spatial coverage
 [                    ]
-/250
+0/250
 License [One of: Choose option .../CC BY 4.0 https://creativecommons.org/
 licenses/by/4.0//CC BY-SA 4.0 https://creativecommons.org/licenses/by-sa/4.0//
 CC BY-NC 4.0 https://creativecommons.org/licenses/by-nc/4.0//CC BY-NC-SA 4.0
 https://creativecommons.org/licenses/by-nc-sa/4.0//CC BY-ND 4.0 https://
 creativecommons.org/licenses/by-nd/4.0//CC BY-NC-ND 4.0 https://
 creativecommons.org/licenses/by-nc-nd/4.0//CC0 1.0 https://creativecommons.org/
 publicdomain/zero/1.0/]
```

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/summary.html` & `cdmb-1.2.1/cdmb/ui/static_ui/summary.html`

 * *Files 1% similar despite different names*

```diff
@@ -161,16 +161,16 @@
 			<th class="px-6 py-3">End of study period</th>
 			<th class="px-6 py-3">Has crosswalks?</th>
 			<th class="px-6 py-3">Are there any files left to upload?</th></tr></thead>
 	<tbody><tr class="border-b last:border-b-0 bg-white dark:bg-gray-800 dark:border-gray-700"><td class="px-6 py-4 whitespace-nowrap font-medium  text-gray-900 dark:text-white"></td>
 			<td class="px-6 py-4 whitespace-nowrap font-medium  text-gray-900 dark:text-white"></td>
 			<td style="white-space: initial;" class="px-6 py-4 whitespace-nowrap font-medium  text-gray-900 dark:text-white"></td>
 			<td style="white-space: initial;" class="px-6 py-4 whitespace-nowrap font-medium  text-gray-900 dark:text-white"></td>
-			<td class="px-6 py-4 whitespace-nowrap font-medium  text-gray-900 dark:text-white">Wed Jul 05 2023</td>
-			<td class="px-6 py-4 whitespace-nowrap font-medium  text-gray-900 dark:text-white">Wed Jul 05 2023</td>
+			<td class="px-6 py-4 whitespace-nowrap font-medium  text-gray-900 dark:text-white">Fri Jul 28 2023</td>
+			<td class="px-6 py-4 whitespace-nowrap font-medium  text-gray-900 dark:text-white">Fri Jul 28 2023</td>
 			<td class="px-6 py-4 whitespace-nowrap font-medium  text-gray-900 dark:text-white">No</td>
 			<td class="px-6 py-4 whitespace-nowrap font-medium  text-gray-900 dark:text-white"><strong>No</strong></td></tr></tbody></table></div>
```

#### html2text {}

```diff
@@ -25,15 +25,15 @@
 Description is a required input. Go to COHORT_DEFINITION section.
 Main information
 Project         Cohort
                                  Beginning                           Are there
 Project Version Name Description of study   End of study Has         any files
                                  period     period       crosswalks? left to
                                                                      upload?
-                                 Wed Jul 05 Wed Jul 05   No          No
+                                 Fri Jul 28 Fri Jul 28   No          No
                                  2023       2023
 Entities
                                              No. variables with Has validation
 Entity name Time-varying Number of variables catalog (Data has  rules?
                                              to be provided)
 Build CDM
 Creating Metadata
```

### Comparing `cdmb-1.2.0/cdmb/ui/static_ui/validation.html` & `cdmb-1.2.1/cdmb/ui/static_ui/validation.html`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 	<div class="corner svelte-1xklbfh"><a href="https://github.com/cienciadedatosysalud" target="_blank" class="svelte-1xklbfh"><img src="/_app/immutable/assets/github.1ea8d62e.svg" alt="GitHub" class="svelte-1xklbfh"></a></div></header>
 
 
 
 
   <main class="svelte-nv0ll5">
-<div class="fixed right-6 bottom-6 group"><button type="button" name="Open actions menu" aria-controls="ljpt12uj" aria-expanded="false" class="text-center font-medium focus:ring-4 focus:outline-none inline-flex items-center justify-center px-5 py-2.5 text-sm text-white bg-yellow-400 hover:bg-yellow-500 focus:ring-yellow-300 dark:focus:ring-yellow-900 rounded-full !p-3">
+<div class="fixed right-6 bottom-6 group"><button type="button" name="Open actions menu" aria-controls="lkmazr6g" aria-expanded="false" class="text-center font-medium focus:ring-4 focus:outline-none inline-flex items-center justify-center px-5 py-2.5 text-sm text-white bg-yellow-400 hover:bg-yellow-500 focus:ring-yellow-300 dark:focus:ring-yellow-900 rounded-full !p-3">
       <svg aria-hidden="true" class="w-8 h-8 transition-transform group-hover:rotate-45" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6v6m0 0v6m0-6h6m-6 0H6"></path></svg>
     
     <span class="sr-only">Open actions menu</span></button>
   <div></div>
 
 </div>
 <h1>Validation files</h1>
```

### Comparing `cdmb-1.2.0/pyproject.toml` & `cdmb-1.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cdmb"
-version = "1.2.0"
+version = "1.2.1"
 description = "Common Data Model Builder library"
 authors = [
     "Javier González-Galindo <jgonzalezga.iacs@aragon.es>",
     "Francisco Estupiñan-Romero <festupinnan.iacs@aragon.es>",
     "Santiago Royo-Sierra <sroyo.iacs@aragon.es>"
 ]
```

### Comparing `cdmb-1.2.0/PKG-INFO` & `cdmb-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdmb
-Version: 1.2.0
+Version: 1.2.1
 Summary: Common Data Model Builder library
 Home-page: https://github.com/cienciadedatosysalud/cdmb
 License: CC-BY-NC-4.0
 Keywords: common data model,real-world data,health data,synthetic data,secondary use,health,healthcare
 Author: Javier González-Galindo
 Author-email: jgonzalezga.iacs@aragon.es
 Maintainer: Javier González-Galindo
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cdmb Version: 1.2.0 Summary: Common Data Model
+Metadata-Version: 2.1 Name: cdmb Version: 1.2.1 Summary: Common Data Model
 Builder library Home-page: https://github.com/cienciadedatosysalud/cdmb
 License: CC-BY-NC-4.0 Keywords: common data model,real-world data,health
 data,synthetic data,secondary use,health,healthcare Author: Javier GonzÃ¡lez-
 Galindo Author-email: jgonzalezga.iacs@aragon.es Maintainer: Javier GonzÃ¡lez-
 Galindo Maintainer-email: jgonzalezga.iacs@aragon.es Requires-Python:
 >=3.9,<4.0 Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Healthcare Industry Classifier: Intended Audience :: Science/
```

