# Comparing `tmp/headjack_keymaker-0.0.1a4.tar.gz` & `tmp/headjack_keymaker-0.1.0.tar.gz`

## Comparing `headjack_keymaker-0.0.1a4.tar` & `headjack_keymaker-0.1.0.tar`

### file list

```diff
@@ -1,50 +1,389 @@
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/Makefile
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/netlify.toml
--rw-r--r--   0        0        0   140632 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/pdm.lock
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/.github/workflows/python-checks.yml
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/.pdm-build/.gitignore
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/.pdm-build/keymaker.pth
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/.pdm-build/keymaker-0.1.0+editable.dist-info/METADATA
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/.pdm-build/keymaker-0.1.0+editable.dist-info/WHEEL
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/.hugo_build.lock
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/README.md
--rwxr-xr-x   0        0        0     1085 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/build-docs.sh
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/archetypes/default.md
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/assets/jsconfig.json
--rw-r--r--   0        0        0   133768 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/assets/images/keymaker logo.png
--rw-r--r--   0        0        0    28606 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/assets/images/keymaker logo.svg
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/config/_default/config.toml
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/config/_default/markup.toml
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/config/_default/menu.toml
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/config/_default/outputs.toml
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/config/_default/params.toml
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/content/0.1.0/contributing.md
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/content/0.1.0/getting-started.md
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/content/0.1.0/questions-&-commands.md
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/content/0.1.0/posts/theme-doc/post.md
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/content/versions/_index.md
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/layouts/taxonomy/list.html
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/__about__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/__init__.py
--rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/prompt.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/types.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/constraints/__init__.py
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/constraints/base.py
--rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/constraints/logical.py
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/constraints/options.py
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/constraints/parser.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/constraints/regex.py
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/constraints/stops.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/models/__init__.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/models/base.py
--rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/models/huggingface.py
--rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/models/llama_cpp.py
--rw-r--r--   0        0        0    11968 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/models/openai.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/utils/__init__.py
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/utils/chat.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/.gitignore
--rw-r--r--   0        0        0    20350 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/README.md
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/pyproject.toml
--rw-r--r--   0        0        0    21292 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/PKG-INFO
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/.gitmodules
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/Makefile
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/netlify.toml
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/.github/workflows/python-checks.yml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/.pdm-build/.gitignore
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/.pdm-build/keymaker.pth
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/.pdm-build/keymaker-0.1.0+editable.dist-info/METADATA
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/.pdm-build/keymaker-0.1.0+editable.dist-info/WHEEL
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/.hugo_build.lock
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/README.md
+-rwxr-xr-x   0        0        0     1065 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/build-docs.sh
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/archetypes/default.md
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/assets/jsconfig.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/assets/scss/_bootstrap-variables.scss
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/config/_default/config.toml
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/content/0.1.0/docs/accessing-completions-chat-model/index.md
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/content/0.1.0/docs/advanced-usage-and-customization/index.md
+-rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/content/0.1.0/docs/constraints/index.md
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/content/0.1.0/docs/contributing/index.md
+-rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/content/0.1.0/docs/formatting-and-control-flow/index.md
+-rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/content/0.1.0/docs/getting-started/index.md
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/content/0.1.0/docs/models/index.md
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/content/0.1.0/docs/streaming-and-decoding/index.md
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/content/0.1.0/posts/theme-doc/post.md
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/content/versions/_index.md
+-rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/layouts/index.html
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/layouts/_default/baseof.html
+-rw-r--r--   0        0        0   101153 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/resources/_gen/assets/scss/css/style.scss_26962b449d539ee5c1301a7879e5bb0e.content
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/resources/_gen/assets/scss/css/style.scss_26962b449d539ee5c1301a7879e5bb0e.json
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/static/.DS_Store
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/static/favicon.png
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/static/css/termynal.css
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/static/images/.DS_Store
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/static/images/discord.svg
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/static/images/github-mark.svg
+-rw-r--r--   0        0        0    25173 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/static/images/keymaker-logo.png
+-rw-r--r--   0        0        0    28606 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/static/images/keymaker-logo.svg
+-rw-r--r--   0        0        0    13102 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/static/images/keymaker-logo.webp
+-rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/static/js/termynal.js
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/.eslintrc.js
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/.git
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/.gitignore
+-rw-r--r--   0        0        0     7851 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/CHANGELOG.md
+-rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/LICENSE
+-rw-r--r--   0        0        0    10485 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/README.md
+-rw-r--r--   0        0        0     9755 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/README.zh-cn.md
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/SECURITY.md
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/dependencies.json
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/go.mod
+-rw-r--r--   0        0        0   324863 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/package-lock.json
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/package.json
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/tailwind.config.js
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/theme.toml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/.github/FUNDING.yml
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/.github/dependabot.yml
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/.github/release.yml
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/.github/workflows/Lighthouse-CI.yml
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/.github/workflows/build.yml
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/.github/workflows/pages.yml
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/.github/workflows/update-algolia-search-index.yml
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/.github/workflows/update-dependencies.yml
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/archetypes/default.md
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_custom.scss
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_override.scss
+-rw-r--r--   0        0        0    16898 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_variables.scss
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/color.css
+-rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/main.css
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/style.scss
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/tailwind.css
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_core/_base.scss
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_core/_layout.scss
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_core/_media.scss
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_mixin/_blur.scss
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_mixin/_compatibility.scss
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_mixin/_index.scss
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_mixin/_link.scss
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_page/_404.scss
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_page/_archive.scss
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_page/_home.scss
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_page/_index.scss
+-rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_page/_single.scss
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_page/_special.scss
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_page/_taxonomy.scss
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_partial/_cookieconsent.scss
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_partial/_details.scss
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_partial/_fixed-button.scss
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_partial/_footer.scss
+-rw-r--r--   0        0        0    10501 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_partial/_header.scss
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_partial/_icon.scss
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_partial/_mask.scss
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_partial/_pagination.scss
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_partial/_archive/_tags.scss
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_partial/_archive/_terms.scss
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_partial/_single/_admonition.scss
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_partial/_single/_bilibili.scss
+-rw-r--r--   0        0        0     9878 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_partial/_single/_code.scss
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_partial/_single/_comment.scss
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_partial/_single/_echarts.scss
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_partial/_single/_footer.scss
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_partial/_single/_friend.scss
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_partial/_single/_katex.scss
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_partial/_single/_mapbox.scss
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_partial/_single/_mermaid.scss
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_partial/_single/_music.scss
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_partial/_single/_related.scss
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_partial/_single/_series.scss
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_partial/_single/_showcase.scss
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_partial/_single/_sponsor.scss
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/css/_partial/_single/_toc.scss
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/data/polyfill.yml
+-rw-r--r--   0        0        0     9360 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/data/social.yml
+-rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/data/cdn/jsdelivr.yml
+-rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/data/emoji/apple.yml
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/data/emoji/facebook.yml
+-rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/data/emoji/google.yml
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/data/emoji/twitter.yml
+-rw-r--r--   0        0        0    10454 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/images/avatar.webp
+-rw-r--r--   0        0        0     8137 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/js/sw.js
+-rw-r--r--   0        0        0    31061 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/js/theme.js
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/js/shims/aplayer.js
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/js/shims/artalk.js
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/js/shims/clipboard.js
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/js/shims/cookieconsent.js
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/js/shims/echarts.js
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/js/shims/katex.js
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/js/shims/tablesort.js
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/js/shims/twemoji.js
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/js/shims/twikoo.js
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/js/shims/valine.js
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/js/shims/waline.js
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/svg/version.template.svg
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/svg/icons/bilibili.svg
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/svg/icons/qq.svg
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/svg/icons/qqGroup.svg
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/assets/svg/icons/thingiverse.svg
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/schema.json
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/assets/css/_custom.scss
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/assets/css/_override.scss
+-rw-r--r--   0        0        0   119992 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/assets/images/Apple-Devices-Preview.webp
+-rw-r--r--   0        0        0    92580 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/assets/images/Wavelength.webp
+-rw-r--r--   0        0        0    10454 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/assets/images/avatar.webp
+-rw-r--r--   0        0        0   206162 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/assets/images/lighthouse-large.webp
+-rw-r--r--   0        0        0    21426 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/assets/images/lighthouse-small.webp
+-rw-r--r--   0        0        0   107566 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/assets/images/lighthouse.webp
+-rw-r--r--   0        0        0    13978 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/assets/images/screenshot.webp
+-rw-r--r--   0        0        0  4365824 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/assets/music/Wavelength.mp3
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/config/_default/author.toml
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/config/_default/hugo.en.toml
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/config/_default/hugo.toml
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/config/_default/hugo.zh-cn.toml
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/config/_default/markup.toml
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/config/_default/mediaTypes.toml
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/config/_default/menu.en.toml
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/config/_default/menu.zh-cn.toml
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/config/_default/outputFormats.toml
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/config/_default/outputs.toml
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/config/_default/params.en.toml
+-rw-r--r--   0        0        0    22046 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/config/_default/params.toml
+-rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/config/_default/params.zh-cn.toml
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/config/_default/permalinks.toml
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/config/_default/privacy.toml
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/config/_default/sitemap.toml
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/config/_default/taxonomies.toml
+-rw-r--r--   0        0        0     7065 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/about/index.en.md
+-rw-r--r--   0        0        0     6722 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/about/index.zh-cn.md
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/authors/_index.en.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/authors/_index.zh-cn.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/categories/documentation/_index.en.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/categories/documentation/_index.zh-cn.md
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/offline/index.en.md
+-rw-r--r--   0        0        0    95094 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/basic-markdown-syntax/featured-image.webp
+-rw-r--r--   0        0        0    19622 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/basic-markdown-syntax/index.en.md
+-rw-r--r--   0        0        0    19577 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/basic-markdown-syntax/index.zh-cn.md
+-rw-r--r--   0        0        0    16084 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/emoji-support/featured-image.webp
+-rw-r--r--   0        0        0    53734 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/emoji-support/index.en.md
+-rw-r--r--   0        0        0    55712 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/emoji-support/index.zh-cn.md
+-rw-r--r--   0        0        0    23755 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/how-to-DoIt/create-diagrams/index.en.md
+-rw-r--r--   0        0        0    23600 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/how-to-DoIt/create-diagrams/index.zh-cn.md
+-rw-r--r--   0        0        0    15844 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/pwa-support/Install-PWA.webp
+-rw-r--r--   0        0        0   249830 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/pwa-support/Installed-PWA.webp
+-rw-r--r--   0        0        0    15168 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/pwa-support/featured-image.webp
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/pwa-support/index.en.md
+-rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/pwa-support/index.zh-cn.md
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/tests/aplayer-tests/index.en.md
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/tests/author-fallback-tests/index.en.md
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/tests/author-single-tests/index.en.md
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/tests/bilibili-tests/index.en.md
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/tests/builtin-shortcodes-tests/index.en.md
+-rw-r--r--   0        0        0     4620 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/tests/echarts-tests/index.en.md
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/tests/extend-shortcodes-tests/index.en.md
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/tests/friend-link-tests/index.en.md
+-rw-r--r--   0        0        0    52218 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/tests/katex-tests/index.en.md
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/tests/mapbox-tests/index.en.md
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/tests/markdown-tests/index.en.md
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/tests/mermaid-tests/index.en.md
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/tests/music-tests/index.en.md
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/tests/related-tests/index.en.md
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/tests/series-taxonomy-tests/index.en.md
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/tests/series-taxonomy-tests/index.zh-cn.md
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/tests/showcase-tests/index.en.md
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/tests/toc-tests/index.en.md
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/tests/typeit-tests/index.en.md
+-rw-r--r--   0        0        0   112108 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/basic-configuration-preview.webp
+-rw-r--r--   0        0        0   140344 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/basic-configuration-preview.zh-cn.webp
+-rw-r--r--   0        0        0   160484 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/complete-configuration-preview.webp
+-rw-r--r--   0        0        0   172518 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/complete-configuration-preview.zh-cn.webp
+-rw-r--r--   0        0        0   227870 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/featured-image.webp
+-rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/index.en.md
+-rw-r--r--   0        0        0    41867 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/index.zh-cn.md
+-rw-r--r--   0        0        0   286589 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/language-switch.gif
+-rw-r--r--   0        0        0    14228 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-built-in-shortcodes/featured-image.webp
+-rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-built-in-shortcodes/index.en.md
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-built-in-shortcodes/index.zh-cn.md
+-rw-r--r--   0        0        0    95672 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-content/featured-image.webp
+-rw-r--r--   0        0        0    18785 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-content/index.en.md
+-rw-r--r--   0        0        0    17488 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-content/index.zh-cn.md
+-rw-r--r--   0        0        0   211304 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-content/summary.webp
+-rw-r--r--   0        0        0   200238 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-content/summary.zh-cn.webp
+-rw-r--r--   0        0        0    20254 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-extended-shortcodes/featured-image-preview.webp
+-rw-r--r--   0        0        0    27100 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-extended-shortcodes/featured-image.webp
+-rw-r--r--   0        0        0    40347 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-extended-shortcodes/index.en.md
+-rw-r--r--   0        0        0    38472 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-extended-shortcodes/index.zh-cn.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/series/_index.en.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/series/_index.zh-cn.md
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/series/getting-start/_index.en.md
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/series/getting-start/_index.zh-cn.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/series/how-to-doit/_index.en.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/series/how-to-doit/_index.zh-cn.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/series/test-series/_index.en.md
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/series/test-series/_index.zh-cn.md
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/showcase/index.en.md
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/showcase/index.zh-cn.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/tags/configuration/_index.en.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/tags/configuration/_index.zh-cn.md
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/tags/content/_index.en.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/tags/content/_index.zh-cn.md
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/tags/installation/_index.en.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/content/tags/installation/_index.zh-cn.md
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/data/authors/Dillon.toml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/data/authors/PCloud.toml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/static/_redirects
+-rw-r--r--   0        0        0    15832 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/static/android-chrome-192x192.png
+-rw-r--r--   0        0        0    48161 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/static/android-chrome-512x512.png
+-rw-r--r--   0        0        0    10397 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/static/apple-touch-icon.png
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/static/browserconfig.xml
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/static/favicon-16x16.png
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/static/favicon-32x32.png
+-rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/static/favicon.ico
+-rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/static/mstile-150x150.png
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/static/safari-pinned-tab.svg
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/static/site.webmanifest
+-rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/i18n/ar.toml
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/i18n/ca.toml
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/i18n/de.toml
+-rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/i18n/en.toml
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/i18n/es.toml
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/i18n/fr.toml
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/i18n/hi.toml
+-rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/i18n/id.toml
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/i18n/it.toml
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/i18n/ko.toml
+-rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/i18n/pl.toml
+-rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/i18n/pt-BR.toml
+-rw-r--r--   0        0        0     3766 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/i18n/pt-PT.toml
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/i18n/ro.toml
+-rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/i18n/ru.toml
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/i18n/sr.toml
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/i18n/te.toml
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/i18n/th.toml
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/i18n/tr.toml
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/i18n/uk.toml
+-rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/i18n/vi.toml
+-rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/i18n/zh-CN.toml
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/i18n/zh-TW.toml
+-rw-r--r--   0        0        0   493975 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/images/screenshot.png
+-rw-r--r--   0        0        0   100091 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/images/tn.png
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/404.html
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/index.html
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/index.json
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/index.rss.xml
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/robots.txt
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/sitemap.xml
+-rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/_default/baseof.html
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/_default/section.html
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/_default/single.html
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/_default/single.md
+-rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/_default/summary.html
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/_default/_markup/render-codeblock-mermaid.html
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/_default/_markup/render-heading.html
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/_default/_markup/render-image.html
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/_default/_markup/render-link.html
+-rw-r--r--   0        0        0    18065 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/assets.html
+-rw-r--r--   0        0        0    25678 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/comment.html
+-rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/footer.html
+-rw-r--r--   0        0        0    11552 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/header.html
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/init.html
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/paginator.html
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/recentlyUpdated.html
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/related.html
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/function/author.html
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/function/checkbox.html
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/function/content.html
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/function/escape.html
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/function/fontawesome.html
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/function/fraction.html
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/function/getRemoteImage.html
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/function/id.html
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/function/path.html
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/function/resource.html
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/function/ruby.html
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/function/suffixValidation.html
+-rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/head/link.html
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/head/meta.html
+-rw-r--r--   0        0        0     6877 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/head/seo.html
+-rw-r--r--   0        0        0     4408 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/home/profile.html
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/meta/author.html
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/plugin/analytics.html
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/plugin/compatibility.html
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/plugin/icon.html
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/plugin/image.html
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/plugin/link.html
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/plugin/script.html
+-rw-r--r--   0        0        0    11469 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/plugin/share.html
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/plugin/social.html
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/plugin/style.html
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/rss/item.html
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/scratch/commentScript.html
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/scratch/configScript.html
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/scratch/script.html
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/scratch/style.html
+-rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/single/footer.html
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/single/outdatedArticleReminder.html
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/partials/single/sponsor.html
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/posts/rss.xml
+-rw-r--r--   0        0        0    12543 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/posts/single.html
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/shortcodes/admonition.html
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/shortcodes/aplayer.html
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/shortcodes/audio.html
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/shortcodes/bilibili.html
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/shortcodes/echarts.html
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/shortcodes/friend.html
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/shortcodes/image.html
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/shortcodes/link.html
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/shortcodes/mapbox.html
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/shortcodes/math.html
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/shortcodes/mermaid.html
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/shortcodes/music.html
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/shortcodes/script.html
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/shortcodes/showcase.html
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/shortcodes/style.html
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/shortcodes/typeit.html
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/shortcodes/version.html
+-rw-r--r--   0        0        0     4550 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/taxonomy/list.html
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/taxonomy/rss.xml
+-rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/taxonomy/terms.html
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/keymaker/__about__.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/keymaker/__init__.py
+-rw-r--r--   0        0        0    17528 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/keymaker/prompt.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/keymaker/types.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/keymaker/constraints/__init__.py
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/keymaker/constraints/base.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/keymaker/constraints/json.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/keymaker/constraints/logical.py
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/keymaker/constraints/model.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/keymaker/constraints/options.py
+-rw-r--r--   0        0        0     5128 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/keymaker/constraints/parser.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/keymaker/constraints/regex.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/keymaker/constraints/stops.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/keymaker/models/__init__.py
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/keymaker/models/base.py
+-rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/keymaker/models/huggingface.py
+-rw-r--r--   0        0        0     5280 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/keymaker/models/llama_cpp.py
+-rw-r--r--   0        0        0    12482 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/keymaker/models/openai.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/keymaker/utils/__init__.py
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/keymaker/utils/chat.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/keymaker/utils/formatted_completion.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/keymaker/utils/general.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/tests/test_dummy.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/.gitignore
+-rw-r--r--   0        0        0    39732 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/README.md
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    40725 2020-02-02 00:00:00.000000 headjack_keymaker-0.1.0/PKG-INFO
```

### Comparing `headjack_keymaker-0.0.1a4/.pre-commit-config.yaml` & `headjack_keymaker-0.1.0/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -42,11 +42,11 @@
     - types-PyYAML
     - types-tabulate
 - repo: https://github.com/asottile/add-trailing-comma
   rev: v2.2.1
   hooks:
   - id: add-trailing-comma
 - repo: https://github.com/hadialqattan/pycln
-  rev: v1.1.0 # Possible releases: https://github.com/hadialqattan/pycln/tags
+  rev: v2.1.7 # Possible releases: https://github.com/hadialqattan/pycln/tags
   hooks:
   - id: pycln
     args: [--config=pyproject.toml]
```

### Comparing `headjack_keymaker-0.0.1a4/.github/workflows/python-checks.yml` & `headjack_keymaker-0.1.0/.github/workflows/python-checks.yml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a4/.pdm-build/keymaker-0.1.0+editable.dist-info/METADATA` & `headjack_keymaker-0.1.0/.pdm-build/keymaker-0.1.0+editable.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a4/docs/build-docs.sh` & `headjack_keymaker-0.1.0/docs/build-docs.sh`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 fi
 
 VERSION=$1         # 0.1.0
 SET_AS_LATEST=$2   # false
 BASE_URL=$3        # http://localhost:1313
 
 if [ "$SET_AS_LATEST" = true ] ; then
-    hugo -d public --contentDir content/${VERSION}/ --configDir config --baseURL $BASE_URL --cleanDestinationDir
+    hugo -d public --contentDir content/${VERSION}/ --configDir config --cleanDestinationDir
 fi
 
 # Build the versions site (sits outside of docs sites for each version)
 hugo -d public/versions --contentDir content/versions/ --configDir config --baseURL $BASE_URL --environment versions --cleanDestinationDir
 
 # Build the docs site for specified version
 hugo -d public/${VERSION} --contentDir content/${VERSION}/ --configDir config --baseURL "${BASE_URL}${VERSION}" --cleanDestinationDir
```

### Comparing `headjack_keymaker-0.0.1a4/docs/assets/images/keymaker logo.svg` & `headjack_keymaker-0.1.0/docs/static/images/keymaker-logo.svg`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a4/docs/config/_default/markup.toml` & `headjack_keymaker-0.1.0/docs/themes/DoIt/exampleSite/config/_default/markup.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a4/docs/content/0.1.0/contributing.md` & `headjack_keymaker-0.1.0/docs/content/0.1.0/docs/contributing/index.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a4/docs/layouts/taxonomy/list.html` & `headjack_keymaker-0.1.0/docs/themes/DoIt/layouts/taxonomy/list.html`

 * *Files 4% similar despite different names*

```diff
@@ -65,21 +65,31 @@
                         </a>
                         <span class="archive-item-date">
                             {{- $.Site.Params.dateFormat | default "2006-01-02" | .Date.Format -}}
                         </span>
                     </article>
                 {{- end -}}
             {{- else -}}
-                {{- range .Pages.GroupBy "Weight" -}}
-                {{range .Pages.ByTitle}}
-                    <article class="archive-item">
-                        <a href="{{ .RelPermalink }}" class="archive-item-link">
-                            {{- .Title -}}
-                        </a>
-                    </article>
+                {{- $pages := .Pages.GroupByDate "2006" -}}
+                {{- with .Site.Params.list.paginate | default .Site.Params.paginate -}}
+                    {{- $pages = $.Paginate $pages . -}}
+                {{- else -}}
+                    {{- $pages = .Paginate $pages -}}
                 {{- end -}}
+                {{- range $pages.PageGroups -}}
+                    <h3 class="group-title">{{ .Key }}</h3>
+                    {{- range .Pages -}}
+                        <article class="archive-item">
+                            <a href="{{ .RelPermalink }}" class="archive-item-link">
+                                {{- .Title -}}
+                            </a>
+                            <span class="archive-item-date">
+                                {{- $.Site.Params.list.dateFormat | default "01-02" | .Date.Format -}}
+                            </span>
+                        </article>
+                    {{- end -}}
                 {{- end -}}
             {{- end -}}
             {{- partial "paginator.html" . -}}
         {{- end -}}
     </div>
 {{- end -}}
```

#### html2text {}

```diff
@@ -18,11 +18,16 @@
      "function/content.html" | safeHTML -}}
 {{- end -}} {{- /* Paginate */ -}} {{- if .Pages -}} {{- $taxonomy :
 = .Data.Singular -}} {{- if eq $taxonomy "series" -}} {{- $pages :
 = .Pages.ByParam "series_weight" -}} {{- with .Site.Params.list.paginate |
 default .Site.Params.paginate -}} {{- $pages = $.Paginate $pages . -}} {{- else
 -}} {{- $pages = .Paginate $pages -}} {{- end -}} {{- range $pages.Pages -}}  {
 {-_.Title_-}}  {{- $.Site.Params.dateFormat | default "2006-01-02" |
-.Date.Format -}}   {{- end -}} {{- else -}} {{- range .Pages.GroupBy "Weight" -
-}} {{range .Pages.ByTitle}}  {{-_.Title_-}}  {{- end -}} {{- end -}} {{- end -
-}} {{- partial "paginator.html" . -}} {{- end -}}
+.Date.Format -}}   {{- end -}} {{- else -}} {{- $pages := .Pages.GroupByDate
+"2006" -}} {{- with .Site.Params.list.paginate | default .Site.Params.paginate
+-}} {{- $pages = $.Paginate $pages . -}} {{- else -}} {{- $pages = .Paginate
+$pages -}} {{- end -}} {{- range $pages.PageGroups -}}
+**** {{ .Key }} ****
+{{- range .Pages -}}  {{-_.Title_-}}  {{- $.Site.Params.list.dateFormat |
+default "01-02" | .Date.Format -}}   {{- end -}} {{- end -}} {{- end -}} {{-
+partial "paginator.html" . -}} {{- end -}}
 {{- end -}}
```

### Comparing `headjack_keymaker-0.0.1a4/keymaker/constraints/base.py` & `headjack_keymaker-0.1.0/keymaker/constraints/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """Base Constraint interface"""
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Any, Optional, Tuple
+from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from keymaker.models.base import Model
 
 from keymaker.types import TokenConstraint
 
 
 class Constraint(ABC):
     @abstractmethod
-    def constrain_tokens(
+    async def constrain_tokens(
         self,
         base_text: str,
         completion_text: str,
         model: "Model",
-        state: Optional[Any] = None,
-    ) -> Tuple[TokenConstraint, Any]:
+    ) -> TokenConstraint:
         """Constrain the token ids that can be sampled from the model's vocabulary.
 
             Args:
                 base_text (str): The text to which the completion_text should be appended.
                 completion_text (str): The text completed thus far; one token will be added between calls
                 model (Model): The language model to be used.
 
@@ -38,7 +37,12 @@
 
         return OrConstraint([self, other])
 
     def __and__(self, other):
         from keymaker.constraints.logical import AndConstraint
 
         return AndConstraint([self, other])
+
+    def __invert__(self):
+        from keymaker.constraints.logical import NotConstraint
+
+        return NotConstraint(self)
```

### Comparing `headjack_keymaker-0.0.1a4/keymaker/constraints/logical.py` & `headjack_keymaker-0.1.0/keymaker/constraints/logical.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Common logical constraints for combining other constraints"""
 
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, List, Sequence, Tuple, cast
+from typing import TYPE_CHECKING, List, Sequence, cast
 
 from keymaker.constraints.base import Constraint
 from keymaker.types import TokenConstraint
 
 if TYPE_CHECKING:
     from keymaker.models.base import Model
 
@@ -16,84 +16,81 @@
 
     Attributes:
         constraint (Constraint): The constraint to negate.
     """
 
     constraint: Constraint
 
-    def constrain_tokens(
+    async def constrain_tokens(
         self,
         base_text: str,
         completion_text: str,
         model: "Model",
-        state: None = None,
-    ) -> Tuple[TokenConstraint, None]:
-        selected_tokens = self.constraint.constrain_tokens(base_text, completion_text, model)
+    ) -> TokenConstraint:
+        selected_tokens = await self.constraint.constrain_tokens(base_text, completion_text, model)
         if selected_tokens is None or isinstance(selected_tokens, str):
-            return selected_tokens, None
-        return {tok for tok in model.tokens if tok not in selected_tokens}, None
+            return selected_tokens
+        return {tok for tok in model.tokens if tok not in selected_tokens}
 
 
 @dataclass
 class AndConstraint(Constraint):
     """Constrain token ids that can be sampled by applying multiple constraints.
 
     Attributes:
         constraints (List[Constraint]): The list of constraints to apply.
     """
 
     constraints: Sequence[Constraint]
 
-    def constrain_tokens(
+    async def constrain_tokens(
         self,
         base_text: str,
         completion_text: str,
         model: "Model",
-        state: None = None,
-    ) -> Tuple[TokenConstraint, None]:
+    ) -> TokenConstraint:
         ret = None
         completions: List[str] = []
         for constraint in self.constraints:
             completions = []
-            selected_tokens = constraint.constrain_tokens(base_text, completion_text, model)
+            selected_tokens = await constraint.constrain_tokens(base_text, completion_text, model)
             if selected_tokens is None:
                 # Do nothing because all tokens are valid
                 pass
             if isinstance(selected_tokens, str):
                 completions.append(selected_tokens)
             if isinstance(selected_tokens, set):
                 ret = (cast(set, ret) & selected_tokens) if ret is not None else selected_tokens
         if len(completions) == len(self.constraints):
             if len(set(completions)) != 1:
                 raise ValueError(f"Got different completions for constraints `{self}`. Completions: `{set(completions)}`")
-            return completions[0], None
-        return ret, None
+            return completions[0]
+        return ret
 
 
 @dataclass
 class OrConstraint(Constraint):
     """Constrain token ids that can be sampled by applying multiple constraints.
 
     Attributes:
         constraints (List[Constraint]): The list of constraints to apply.
     """
 
     constraints: Sequence[Constraint]
 
-    def constrain_tokens(
+    async def constrain_tokens(
         self,
         base_text: str,
         completion_text: str,
         model: "Model",
-        state: None = None,
-    ) -> Tuple[TokenConstraint, None]:
+    ) -> TokenConstraint:
         ret = set()  # type: ignore
         for constraint in self.constraints:
-            selected_tokens = constraint.constrain_tokens(base_text, completion_text, model)
+            selected_tokens = await constraint.constrain_tokens(base_text, completion_text, model)
             if selected_tokens is None:
                 # One allows everything so overall the or does
-                return None, None
+                return None
             if isinstance(selected_tokens, str):
-                return selected_tokens, None
+                return selected_tokens
             if isinstance(selected_tokens, set):
                 ret |= selected_tokens
-        return ret, None
+        return ret
```

### Comparing `headjack_keymaker-0.0.1a4/keymaker/constraints/options.py` & `headjack_keymaker-0.1.0/keymaker/constraints/options.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Constraints over sets of fixed options"""
 from concurrent.futures import ThreadPoolExecutor
 from dataclasses import dataclass
-from typing import Set, Tuple
+from typing import Set
 
 from keymaker.constraints.base import Constraint
 from keymaker.models.base import Model
 from keymaker.types import TokenConstraint
 
 
 @dataclass
@@ -17,38 +17,37 @@
     options: Set[str]
     short_circuit: bool = True  # early return when available options based on completed text are <=1
 
     def _is_valid_token(self, token_id: int, partial_completion: str, model: Model) -> bool:
         decoded_token = model.tokens[token_id]
         return any(option.startswith(partial_completion + decoded_token) for option in self.options)
 
-    def constrain_tokens(
+    async def constrain_tokens(
         self,
         base_text: str,
         completion_text: str,
         model: Model,
-        state: None = None,
-    ) -> Tuple[TokenConstraint, None]:
+    ) -> TokenConstraint:
         if completion_text in self.options:
-            return completion_text, None
+            return completion_text
 
         if completion_text and self.short_circuit:
             limited_options = set()
             for option in self.options:
                 if option.startswith(completion_text):
                     limited_options.add(option)
                     if len(limited_options) > 1:
                         break
             if len(limited_options) == 0:
-                return set(), None
+                return set()
             if len(limited_options) == 1:
-                return limited_options.pop(), None
+                return limited_options.pop()
 
         with ThreadPoolExecutor():
             valid_token_ids = set(
                 filter(
                     lambda token_id: self._is_valid_token(token_id, completion_text, model),
                     model.tokens.keys(),
                 ),
             )
 
-        return valid_token_ids, None
+        return valid_token_ids
```

### Comparing `headjack_keymaker-0.0.1a4/keymaker/constraints/parser.py` & `headjack_keymaker-0.1.0/keymaker/constraints/parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,109 +1,146 @@
 from concurrent.futures import ThreadPoolExecutor
-from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Set, Tuple
+from dataclasses import dataclass
+from functools import lru_cache
+from typing import List, Optional, Union
 
 import regex as re
-from lark import Lark, UnexpectedInput
+from parsy import ParseError, Parser
 
 from keymaker.constraints.base import Constraint
+from keymaker.models.base import Model
 from keymaker.types import TokenConstraint
 
-if TYPE_CHECKING:
-    from keymaker.models.base import Model
+try:
+    from lark import Lark, UnexpectedCharacters, UnexpectedEOF
+except ImportError:
+    Lark = None
 
 
 @dataclass
 class ParserConstraint(Constraint):
     """Constrain token ids that can be sampled based on a context-free grammar or a pre-built parser.
 
     Attributes:
         grammar (str, optional): The context-free grammar to use for parsing. Either the grammar or a pre-built parser
             must be provided.
         parser (Lark, optional): A pre-built parser that will be used for parsing. Either the grammar or a pre-built
             parser must be provided.
 
-    Notes:
-        The `parser` attribute takes precedence over `grammar` if both are provided.
-        Based on https://github.com/r2d4/parserllm.
     """
 
-    grammar: Optional[str] = None
-    parser: Optional[Lark] = None
-    terminal_terminate_on_match: Dict[str, bool] = field(default_factory=lambda: dict(CNAME=False))
+    parser: Optional[Union[Parser, "Lark"]] = None
+    terminate_on_parse: bool = True
+    ignore_pattern: str = r"\s*"
 
     def __post_init__(self):
-        if self.grammar and self.parser:
-            raise ValueError("Provided values for both `grammar` and `parser`. Choose only one.")
-        if not (self.grammar or self.parser):
-            raise ValueError("Must provide one of `grammar` or `parser`.")
-        if self.grammar:
-            self.parser = Lark(self.grammar)
+        self._terminal_regexes = None
+        if Lark is not None and isinstance(self.parser, Lark):
+            self._extract_terminal_regex()
 
-        self.terminal_regexes = self.extract_terminal_regex(self.parser)
-
-    @staticmethod
-    def extract_terminal_regex(parser: Lark) -> Dict[str, re.Pattern]:
+    def _extract_terminal_regex(self):
         regex_map = {}
-        for term in parser.terminals:  # type: ignore
+        for term in self.parser.terminals:  # type: ignore
             if term.pattern:
-                regex_map[term.name] = re.compile(term.pattern.to_regexp())
-        return regex_map
-
-    @staticmethod
-    def next_lex(input_str: str, parser: Lark) -> Set[str]:
-        try:
-            parser.parse(input_str)  # type: ignore
-        except UnexpectedInput as e:
-            ret = set()
-            try:
-                ret |= set(e.expected)
-            except AttributeError:
-                pass
-            try:
-                ret |= set(e.allowed)
-            except AttributeError:
-                pass
-            return ret
-        return set()
+                regex_map[term.name] = term.pattern.to_regexp()
+        self._terminal_regexes = regex_map
 
     def _is_valid_token(self, patterns: List[re.Pattern[str]], token_id: int, partial_completion: str, model: "Model") -> bool:
         poss_completion = partial_completion + model.tokens[token_id]
         return any((pattern.fullmatch(poss_completion, partial=True) for pattern in patterns))
 
-    def constrain_tokens(
+    @lru_cache
+    def _compile_re(self, pattern: str) -> re.Pattern[str]:
+        try:
+            return re.compile(self.ignore_pattern + pattern + self.ignore_pattern)
+        except Exception:
+            return re.compile(self.ignore_pattern + re.escape(pattern) + self.ignore_pattern)
+
+    async def _constrain_tokens_parsy(
         self,
         base_text: str,
         completion_text: str,
         model: "Model",
-        state: Optional[Any] = None,
-    ) -> Tuple[TokenConstraint, Any]:
+    ) -> TokenConstraint:
         # find what rules from the parser are valid next
-        valid_next_lex = self.next_lex(completion_text, self.parser)
-        if len(valid_next_lex) == 0:
-            return set(), None
-        if len(valid_next_lex) == 1 and '$END' in valid_next_lex:
-            return completion_text, None
-
-        last_lex = state['last_lex'] if state else set()
-        start_idx = state['start_idx'] if state else 0
-
-        # strip that last lex if there is a match
-        # our parser regex patterns only tell us the next completion pattern
-        # and cannot be complete of what we have already selected
-        for lex in last_lex:
-            if self.terminal_regexes[lex].fullmatch(completion_text[start_idx:]):
-                start_idx = len(completion_text)
-                last_lex = set()
-                break
+        add_eos = False
+        try:
+            self.parser.parse(completion_text)  # type: ignore
+            if self.terminate_on_parse:
+                return completion_text
+            else:
+                add_eos = True
+        except ParseError as e:
+            valid_next_lex, index = e.expected, e.index
+            if self.terminate_on_parse:
+                try:
+                    test = completion_text[:index]
+                    self.parser.parse(test)  # type: ignore
+                    return test
+                except Exception:
+                    pass
+
+        regex_patterns = [self._compile_re(lex) for lex in valid_next_lex]
+
+        with ThreadPoolExecutor():
+            valid_token_ids = set(
+                filter(
+                    lambda token_id: self._is_valid_token(regex_patterns, token_id, completion_text[index:], model),
+                    model.tokens.keys(),
+                ),
+            )
+        if add_eos:
+            valid_token_ids.add(model.eos_token_id)
+        return valid_token_ids
 
-        regex_pattern = [self.terminal_regexes[t] for t in valid_next_lex | last_lex]
+    async def _constrain_tokens_lark(
+        self,
+        base_text: str,
+        completion_text: str,
+        model: "Model",
+    ) -> TokenConstraint:
+        index = None
+        add_eos = False
+        try:
+            self.parser.parse(completion_text)  # type: ignore
+            if self.terminate_on_parse:
+                return completion_text
+            else:
+                add_eos = True
+        except UnexpectedCharacters as e:
+            valid_next_lex = {self._terminal_regexes[lex] for lex in e.allowed}
+            index = e.pos_in_stream
+
+        except UnexpectedEOF as e:
+            valid_next_lex = {self._terminal_regexes[lex] for lex in e.expected}
+            index = len(completion_text)
+
+        if index and self.terminate_on_parse:
+            try:
+                test = completion_text[:index]
+                self.parser.parse(test)  # type: ignore
+                return test
+            except Exception:
+                pass
+
+        regex_patterns = [self._compile_re(lex) for lex in valid_next_lex]
 
         with ThreadPoolExecutor():
             valid_token_ids = set(
                 filter(
-                    lambda token_id: self._is_valid_token(regex_pattern, token_id, completion_text[start_idx:], model),
+                    lambda token_id: self._is_valid_token(regex_patterns, token_id, completion_text[index:], model),
                     model.tokens.keys(),
                 ),
             )
+        if add_eos:
+            valid_token_ids.add(model.eos_token_id)
+        return valid_token_ids
 
-        return valid_token_ids, {'start_idx': start_idx, 'last_lex': valid_next_lex}
+    async def constrain_tokens(
+        self,
+        base_text: str,
+        completion_text: str,
+        model: Model,
+    ) -> TokenConstraint:
+        if isinstance(self.parser, Parser):
+            return await self._constrain_tokens_parsy(base_text, completion_text, model)
+        return await self._constrain_tokens_lark(base_text, completion_text, model)
```

### Comparing `headjack_keymaker-0.0.1a4/keymaker/constraints/regex.py` & `headjack_keymaker-0.1.0/keymaker/constraints/regex.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Constraints for regex patterns"""
 from concurrent.futures import ThreadPoolExecutor
 from dataclasses import dataclass
-from typing import Tuple, Union
+from typing import Union
 
 import regex as re
 
 from keymaker.constraints.base import Constraint
 from keymaker.models.base import Model
 from keymaker.types import TokenConstraint
 
@@ -27,28 +27,31 @@
     def __post_init__(self):
         self._pattern: re.Pattern[str] = re.compile(self.pattern) if isinstance(self.pattern, str) else self.pattern
 
     def _is_valid_token(self, token_id: int, partial_completion: str, model: "Model") -> bool:
         decoded_token = model.tokens[token_id]
         return self._pattern.fullmatch(partial_completion + decoded_token, partial=True)
 
-    def constrain_tokens(
+    async def constrain_tokens(
         self,
         base_text: str,
         completion_text: str,
         model: "Model",
-        state: None = None,
-    ) -> Tuple[TokenConstraint, None]:
-        if self.terminate_on_match:
-            m = self._pattern.match(completion_text)
-            if m and m.start() == 0:
-                return completion_text, None
+    ) -> TokenConstraint:
+        add_eos = False
+        match = self._pattern.match(completion_text)
+        if match and match.start() == 0:
+            if self.terminate_on_match:
+                return completion_text[: match.end()]
+            else:
+                add_eos = True
 
         with ThreadPoolExecutor():
             valid_token_ids = set(
                 filter(
                     lambda token_id: self._is_valid_token(token_id, completion_text, model),
                     model.tokens.keys(),
                 ),
             )
-
-        return valid_token_ids, None
+        if add_eos:
+            valid_token_ids.add(model.eos_token_id)
+        return valid_token_ids
```

### Comparing `headjack_keymaker-0.0.1a4/keymaker/constraints/stops.py` & `headjack_keymaker-0.1.0/keymaker/constraints/stops.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Constraints for stop patterns"""
 from dataclasses import dataclass
-from typing import Tuple
 
 import regex as re
 
 from keymaker.constraints.base import Constraint
 from keymaker.models.base import Model
 from keymaker.types import TokenConstraint
 
@@ -20,20 +19,19 @@
 
     stop: str
     include: bool = True
 
     def __post_init__(self):
         self._pattern = re.compile(rf"(?P<completion>.*?)(?P<stop>{self.stop})")
 
-    def constrain_tokens(
+    async def constrain_tokens(
         self,
         base_text: str,
         completion_text: str,
         model: Model,
-        state: None = None,
-    ) -> Tuple[TokenConstraint, None]:
+    ) -> TokenConstraint:
         match = self._pattern.search(completion_text)
         if match:
             if not self.include:
-                return match.group('completion'), None
-            return match.group('completion') + match.group('stop'), None
-        return None, None
+                return completion_text
+            return completion_text + match.group('stop')
+        return None
```

### Comparing `headjack_keymaker-0.0.1a4/keymaker/models/__init__.py` & `headjack_keymaker-0.1.0/keymaker/models/__init__.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a4/keymaker/models/base.py` & `headjack_keymaker-0.1.0/keymaker/models/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Base model interface"""
 from abc import ABC, abstractmethod
-from typing import AsyncGenerator, ClassVar, FrozenSet, List, Optional, Set
+from typing import AsyncGenerator, ClassVar, FrozenSet, List, Optional, Set, Tuple
 
 from keymaker.types import Decoder, DecodingStrategy, SelectedTokens, TokenIds, Tokens
 
 
 class Model(ABC):
     """
     A base model from which to derive all models that generate text
@@ -40,15 +40,15 @@
 
     async def sample(
         self,
         text: str,
         selected_tokens: Optional[SelectedTokens] = None,
         decoder: Optional[Decoder] = None,
         timeout: float = 10.0,
-    ) -> List[str]:
+    ) -> Tuple[List[str], List[float]]:
         """Sample from the language model given the input text and the selected tokens to constrain the sampling.
 
         Args:
             text (str): The input text to the language model.
             selected_tokens (Optional[Set[int]]): The set of token ids to constrain the sampling. Defaults to None.
 
         Returns:
@@ -57,18 +57,19 @@
         gen = self.generate(
             text=text,
             max_tokens=self.sample_chunk_size,
             selected_tokens=selected_tokens,
             decoder=decoder,
             timeout=timeout,
         )
-        ret = []
-        async for tok in gen:  # type: ignore
+        ret, probs = [], []
+        async for tok, prob in gen:  # type: ignore
             ret.append(tok)
-        return ret
+            probs += prob
+        return ret, probs
 
     @abstractmethod
     def encode(self, text: str) -> TokenIds:
         """Encode the input text as token ids.
 
         Args:
             text (str): The input text to encode.
@@ -98,7 +99,11 @@
     def eos_token_id(self) -> int:
         """Get the token id of the end of sequence (eos) token."""
 
     @property
     @abstractmethod
     def bos_token_id(self) -> int:
         """Get the token id of the beginning of sequence (bos) token."""
+
+
+class ChatModel(Model):
+    """Base model for chat based models"""
```

### Comparing `headjack_keymaker-0.0.1a4/keymaker/models/huggingface.py` & `headjack_keymaker-0.1.0/keymaker/models/huggingface.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """A simple huggingface-based Model implementation for basic local inference and testing"""
 
 import asyncio
 from dataclasses import dataclass
-from typing import AsyncGenerator, FrozenSet, Optional
+from typing import AsyncGenerator, FrozenSet, List, Optional, Tuple
 
 import numpy as np
 import torch
 from transformers import AutoModelForCausalLM, AutoTokenizer
 
 from keymaker.models.base import Model
 from keymaker.types import Decoder, DecodingStrategy, SelectedTokens, TokenIds, Tokens
@@ -36,14 +36,15 @@
 
     def __post_init__(self):
         if self.model_name is None and self.model is None and self.tokenizer is None:
             raise ValueError("must specify either `model_name` or both `model` and `tokenizer`")
         if (self.model is not None and self.tokenizer is None) or (self.model is None and self.tokenizer is not None):
             raise ValueError("must specify either `model_name` or both `model` and `tokenizer`")
         self.model = self.model or AutoModelForCausalLM.from_pretrained(self.model_name)
+
         self.tokenizer = self.tokenizer or AutoTokenizer.from_pretrained(self.model_name)
         self.tokens = transformers_tokens(self.tokenizer)
 
     def encode(self, text: str) -> TokenIds:
         return self.tokenizer.encode(text, add_special_tokens=True)  # type: ignore
 
     def decode(self, ids: TokenIds) -> str:
@@ -74,15 +75,15 @@
     async def generate(  # type: ignore
         self,
         text: str,
         max_tokens: int = 1,
         selected_tokens: Optional[SelectedTokens] = None,
         decoder: Optional[Decoder] = None,
         timeout: float = 10.0,
-    ) -> AsyncGenerator[str, None]:
+    ) -> AsyncGenerator[Tuple[str, List[float]], None]:
         decoder = decoder or Decoder()
         if decoder.strategy not in self.supported_decodings:
             raise ValueError(f"Unsupported decoding strategy for Huggingface model `{decoder.strategy}`.")
         gen_kwargs = {}
         if temperature := decoder.temperature:
             gen_kwargs['temperature'] = temperature
         if top_p := decoder.top_p:
@@ -99,15 +100,39 @@
             max_new_tokens = max_tokens - n_gen
             output = await asyncio.to_thread(
                 self.model.generate,  # type: ignore
                 input_ids=torch.tensor(prompt_token_ids).unsqueeze(0).to(self.model.device),  # type: ignore
                 max_new_tokens=max_new_tokens,
                 logits_processor=self._logit_processor(selected_tokens),
                 pad_token_id=self.tokenizer.eos_token_id,  # type: ignore
+                return_dict_in_generate=True,
+                output_scores=True,
                 **gen_kwargs,
             )
-            new_token_ids = output[0, len(prompt_token_ids) :].detach().cpu().tolist()  # noqa: E203
+            new_token_ids = output.sequences[0, len(prompt_token_ids) :].detach().cpu().tolist()  # noqa: E203
+
+            logprobs = np.log(
+                [
+                    logits.detach().cpu().squeeze().softmax(0)[tok_id].item()
+                    for tok_id, logits in zip(new_token_ids, output.scores)
+                ],
+            ).tolist()
             prompt_token_ids += new_token_ids
             tok_str = self.tokenizer.decode(new_token_ids, skip_special_tokens=True)  # type: ignore
             text += tok_str
             n_gen += max_new_tokens
-            yield tok_str
+            yield tok_str, logprobs
+
+    async def probs(  # type: ignore
+        self,
+        text: str,
+    ) -> List[Tuple[str, float]]:
+        prompt_token_ids = self.tokenizer.encode(text)  # type: ignore
+        output = await asyncio.to_thread(
+            self.model.generate,  # type: ignore
+            input_ids=torch.tensor(prompt_token_ids).unsqueeze(0).to(self.model.device),  # type: ignore
+            max_new_tokens=1,
+            pad_token_id=self.tokenizer.eos_token_id,  # type: ignore
+            return_dict_in_generate=True,
+            output_scores=True,
+        )
+        return list(zip(self.tokens.values(), output.scores[0].detach().cpu().squeeze().softmax(0).tolist()))
```

### Comparing `headjack_keymaker-0.0.1a4/keymaker/models/llama_cpp.py` & `headjack_keymaker-0.1.0/keymaker/models/llama_cpp.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 """A model for use with an in-memory Llama Cpp"""
 
 from dataclasses import dataclass
-from typing import Any, AsyncGenerator, Dict, FrozenSet, Optional
+from typing import Any, AsyncGenerator, Dict, FrozenSet, List, Optional, Tuple
 
 import numpy as np
 
 from keymaker.models.base import Model
 from keymaker.types import Decoder, DecodingStrategy, SelectedTokens, TokenIds, Tokens
 
 try:
     import llama_cpp
     from llama_cpp import Llama
     from starlette.concurrency import iterate_in_threadpool, run_in_threadpool
 except ImportError:
     raise ImportError("llama-cpp-python is an optional dependency and is not installed.")
 
 
+import math
+
+_log = math.log
+math.log = lambda x: _log(x + 1e-10)  # type: ignore
+
+
 def try_decode(tok_bytes: bytes) -> str:
     try:
         return tok_bytes.decode('utf-8')
     except Exception:
         return str(tok_bytes)[2:-1]
 
 
 def llama_tokens(llm: "Llama") -> Tokens:  # type: ignore
     vocab_len = llm.n_vocab()  # type: ignore
-    decoded_already = set()
+    # decoded_already = set()
     tokens = {}
     for i in range(vocab_len - 1):
         decoded = try_decode(llm.detokenize([i]))  # type: ignore
-        if decoded and (decoded not in decoded_already):
+        if decoded:  # and (decoded not in decoded_already):
             tokens[i] = decoded
-            decoded_already.add(decoded)
+            # decoded_already.add(decoded)
     return tokens
 
 
 @dataclass
 class LlamaCpp(Model):
     """
     A LlamaCpp-based Model implementation
@@ -54,15 +60,15 @@
     llama_kwargs: Optional[Dict[str, Any]] = None
 
     def __post_init__(self):
         if self.model_path is None and self.model is None:
             raise ValueError("must specify either `model_name` or `model`")
         if self.model_path is not None and self.model is not None:
             raise ValueError("must specify either `model_name` or `model` not both")
-        self.model = self.model or Llama(model_path=self.model_path, **(self.llama_kwargs or {}))  # type: ignore
+        self.model = self.model or Llama(model_path=self.model_path, logits_all=True, **(self.llama_kwargs or {}))  # type: ignore
         self.tokens = llama_tokens(self.model)
         if self.cache_type is not None:
             if self.cache_type == "disk":
                 cache = llama_cpp.LlamaDiskCache(capacity_bytes=self.cache_size)  # type: ignore
             else:
                 cache = llama_cpp.LlamaRAMCache(capacity_bytes=self.cache_size)  # type: ignore
             self.model.set_cache(cache)
@@ -82,15 +88,15 @@
         return self.model.token_bos()  # type: ignore
 
     def _logit_processor(self, selected_tokens: Optional[SelectedTokens] = None):
         logits_processor = None
         if selected_tokens is not None:
 
             def _logits_processor(input_ids, scores):
-                mask = np.ones_like(scores) * -1e10
+                mask = np.zeros_like(scores) + -100
                 for token_id in selected_tokens:
                     mask[token_id] = 0
                 scores = scores + mask
                 return scores
 
             logits_processor = _logits_processor
         return logits_processor
@@ -98,26 +104,40 @@
     async def generate(  # type: ignore
         self,
         text: str,
         max_tokens: int = 1,
         selected_tokens: Optional[SelectedTokens] = None,
         decoder: Optional[Decoder] = None,
         timeout: float = 10.0,
-    ) -> AsyncGenerator[str, None]:
+    ) -> AsyncGenerator[Tuple[str, List[float]], None]:
         decoder = decoder or Decoder()
         if decoder.strategy not in self.supported_decodings:
             raise ValueError(f"Unsupported decoding strategy for LlamaCpp model `{decoder.strategy}`.")
 
-        gen_kwargs = {'prompt': text, 'stream': True, 'max_tokens': max_tokens}
+        gen_kwargs = {'prompt': text, 'stream': True, 'max_tokens': max_tokens, "logprobs": 15}
         if temperature := decoder.temperature:
             gen_kwargs['temp'] = temperature
         if top_p := decoder.top_p:
             gen_kwargs['top_p'] = top_p
         if top_k := decoder.top_k:
             gen_kwargs['top_k'] = top_k
 
+        if decoder.strategy == DecodingStrategy.GREEDY:
+            # try to make the sampling as deterministic as possible
+            # to select only the one top token
+            gen_kwargs['top_p'] = (
+                1 / self.vocab_size
+            )  # select only n tokens to get over .01, should virually always be a single token
+            if 'top_k' in gen_kwargs:
+                gen_kwargs['top_k'] = 1
+
         if logits_processor := self._logit_processor(selected_tokens):
             gen_kwargs['logits_processor'] = logits_processor
 
         token_generator = await run_in_threadpool(self.model, **gen_kwargs)  # type: ignore
         async for chunk in iterate_in_threadpool(token_generator):
-            yield chunk['choices'][0]['text']
+            delta = chunk['choices'][0]
+            if delta['text'] == "":
+                break
+            token = delta['text']
+            logprob = delta['logprobs']['top_logprobs'][0][token] if delta['logprobs'] else [0]
+            yield token, [logprob]
```

### Comparing `headjack_keymaker-0.0.1a4/keymaker/models/openai.py` & `headjack_keymaker-0.1.0/keymaker/models/openai.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 """Models to use with any openai compatible api endpoints"""
 import warnings
 from dataclasses import dataclass
-from typing import Any, AsyncGenerator, Dict, FrozenSet, Optional
+from functools import lru_cache
+from typing import Any, AsyncGenerator, Dict, FrozenSet, List, Optional, Tuple
 
 import aiohttp
 import openai
 import tiktoken
 from tiktoken import Encoding
 
-from keymaker.models.base import Model
+from keymaker.models.base import ChatModel, Model
 from keymaker.types import Decoder, DecodingStrategy, SelectedTokens, TokenIds, Tokens
 from keymaker.utils.chat import split_tags
 
 
+@lru_cache(10)
 def openai_tokens(tokenizer: Encoding) -> Tokens:
     vocab_len = len(tokenizer.token_byte_values())
     tokens = {i: tokenizer.decode([i]) for i in range(vocab_len - 1)}
     for i in range(vocab_len, tokenizer.max_token_value):
         tokens[i] = f"<|special_{i}|>"
     return tokens
 
 
 @dataclass
-class OpenAIChat(Model):
+class OpenAIChat(ChatModel):
     model_name: str = "gpt-3.5-turbo"
     supported_decodings: FrozenSet[DecodingStrategy] = frozenset(  # type: ignore
         (
             DecodingStrategy.GREEDY,
             DecodingStrategy.SAMPLE,
         ),
     )
     role_tag_start: str = "%"
     role_tag_end: str = "%"
-    default_role: str = "assistant"
+    default_role: str = "user"
     allowed_roles: FrozenSet[str] = frozenset(("system", "user", "assistant"))
     max_retries: int = 10
     retry_sleep_time: float = 1.0
     max_token_selection: int = 300
     max_total_tokens: int = 4000
     sample_chunk_size: int = 12  # tokens generated by `generate` on behalf of `sample`
 
@@ -87,16 +89,21 @@
         if top_p := decoder.top_p:
             gen_kwargs['top_p'] = top_p
         if top_k := decoder.top_k:
             gen_kwargs['top_k'] = top_k
         if decoder.strategy == DecodingStrategy.GREEDY:
             # try to make the sampling as deterministic as possible
             # to select only the one top token
-            gen_kwargs['top_p'] = 0.01  # select only n tokens to get over .01, should virually always be a single token
-            if 'top_k' in gen_kwargs:
+            gen_kwargs['temperature'] = 0
+            gen_kwargs['top_p'] = (
+                1 / self.vocab_size
+            )  # select only n tokens to get over 1/self.vocab_size, should always be a single token
+            if (
+                'top_k' in gen_kwargs
+            ):  # non-openai yet openai-compliant apis may also support topk while the official api does not
                 gen_kwargs['top_k'] = 1
 
         payload = {
             "messages": messages,
             "logit_bias": logit_bias,
             "model": self.model_name,
             "max_tokens": max_tokens,
@@ -112,33 +119,32 @@
     async def generate(  # type: ignore
         self,
         text: str,
         max_tokens: int = 1,
         selected_tokens: Optional[SelectedTokens] = None,
         decoder: Optional[Decoder] = None,
         timeout: float = 10.0,
-    ) -> AsyncGenerator[str, None]:
+    ) -> AsyncGenerator[Tuple[str, List[None]], None]:
         bias = 100
         # if there are more tokens to keep than ignore, invert the bias
         if selected_tokens and len(selected_tokens) > (self.vocab_size / 2):
             selected_tokens = self._all_token_ids - selected_tokens
             bias = -100
 
         if selected_tokens and len(selected_tokens) > self.max_token_selection:
             warnings.warn(
                 f"Trying to mask {len(selected_tokens)} tokens which "
                 f"is more than {self.max_token_selection} mask limit "
                 f"of {self}. Consider stricter constraints. Will select"
                 "lowest token ids up to this limit.",
             )
+            selected_tokens = sorted(list(selected_tokens))[: self.max_token_selection]  # type: ignore
         logit_bias = {}
         if selected_tokens:
             for i, idx in enumerate(selected_tokens):
-                if i >= self.max_token_selection:
-                    break
                 logit_bias[str(idx)] = bias
 
         def result_handler(response):
             delta = response["choices"][0]["delta"]
             return (
                 "" if "content" not in delta else delta["content"],  # content
                 "finish_reason" in delta and delta["finish_reason"] is not None,  # complete generation
@@ -168,15 +174,15 @@
                     break
                 else:
                     error = False
                     content, done = result_handler(chat_completion)
                     if content.startswith(eos_token):
                         break
                     if content:
-                        yield content
+                        yield (content, [None])
                     if done:
                         break
             if not error:
                 break
 
 
 @dataclass
@@ -234,18 +240,20 @@
         if top_p := decoder.top_p:
             gen_kwargs['top_p'] = top_p
         if top_k := decoder.top_k:
             gen_kwargs['top_k'] = top_k
         if decoder.strategy == DecodingStrategy.GREEDY:
             # try to make the sampling as deterministic as possible
             # to select only the one top token
-            gen_kwargs['top_p'] = 0.01  # select only n tokens to get over .01, should virually always be a single token
+            gen_kwargs['top_p'] = (
+                1 / self.vocab_size
+            )  # select only n tokens to get over 1/self.vocab_size, should always be a single token
             if 'top_k' in gen_kwargs:
                 gen_kwargs['top_k'] = 1
-        payload = {"prompt": text, "logit_bias": logit_bias, "model": self.model_name, "max_tokens": max_tokens, **gen_kwargs}  # type: ignore
+        payload = {"prompt": text, "logit_bias": logit_bias, "model": self.model_name, "max_tokens": max_tokens, "logprobs": 5, **gen_kwargs}  # type: ignore
 
         async with aiohttp.ClientSession() as session:
             openai.aiosession.set(session)
             completion_stream = await openai.Completion.acreate(**payload, stream=True)
 
             async for completion in completion_stream:
                 yield completion
@@ -266,25 +274,24 @@
         if selected_tokens and len(selected_tokens) > self.max_token_selection:
             warnings.warn(
                 f"Trying to mask {len(selected_tokens)} tokens which "
                 f"is more than {self.max_token_selection} mask limit "
                 f"of {self}. Consider stricter constraints. Will select"
                 "lowest token ids up to this limit.",
             )
+            selected_tokens = sorted(list(selected_tokens))[: self.max_token_selection]  # type: ignore
         logit_bias = {}
         if selected_tokens:
             for i, idx in enumerate(selected_tokens):
-                if i >= self.max_token_selection:
-                    break
                 logit_bias[str(idx)] = bias
 
         def result_handler(response):
             delta = response.choices[0]
             return (
-                "" if "text" not in delta else delta["text"],  # content
+                ("", 1) if "text" not in delta else (delta["text"], delta['logprobs']['token_logprobs']),  # content
                 "finish_reason" in delta and delta["finish_reason"] is not None,  # complete generation
             )
 
         eos_token = self.decode([self.eos_token_id])
         error = False
         retries = 0
         for retries in range(self.max_retries):
@@ -304,16 +311,16 @@
                         if retry
                         else "",
                     )
                     error = True
                     break
                 else:
                     error = False
-                    content, done = result_handler(completion)
+                    (content, logprob), done = result_handler(completion)
                     if content.startswith(eos_token):
                         break
                     if content:
-                        yield content
+                        yield (content, list(logprob))
                     if done:
                         break
             if not error:
                 break
```

### Comparing `headjack_keymaker-0.0.1a4/keymaker/utils/chat.py` & `headjack_keymaker-0.1.0/keymaker/utils/chat.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import TYPE_CHECKING, Dict, FrozenSet, List
 
-import regex as re
-
 if TYPE_CHECKING:
     from keymaker import Prompt
 
+from parsy import alt, regex, seq, string
+
 
 def split_tags(
     text: str,
     tag_start: str = "%",
     tag_end: str = "%",
     default_role: str = "assistant",
     roles: FrozenSet[str] = frozenset(("system", "user", "assistant")),
@@ -26,48 +26,39 @@
     Returns:
         List[Dict[str, str]]: A list of messages, where each message is a dictionary with keys 'role' and 'content'.
 
     Raises:
         Exception: If an end tag is found with no start tag, or if an unknown or mismatched tag is found.
 
     Examples:
-        >>> split_tags('\nYou are a friendly bot\n%/system%\n%user%Can you help me calculate stuff?%/user%\nYes, how may I help you?\n%user%\nI want to know the square root of 10%/user%\n%assistant%\nSure the square root of 10 is ...\n%/assistant%')
+        >>> split_tags('%system%\nYou are a friendly bot\n%/system%\n%user%Can you help me calculate stuff?%/user%\nYes, how may I help you?\n%user%\nI want to know the square root of 10%/user%\n%assistant%\nSure the square root of 10 is ...\n%/assistant%')
         [{'role': 'assistant', 'content': 'You are a friendly bot\n'}, {'role': 'system', 'content': ''}, {'role': 'user', 'content': 'Can you help me calculate stuff?'}, {'role': 'assistant', 'content': 'Yes, how may I help you?\n'}, {'role': 'user', 'co...
     """
     text = str(text)
-    messages = []
-
-    while text:
-        # first we check to see if the text is untagged
-        match_role = None
-        match = re.search(
-            rf"(?P<content>\s*.*?)\s*(?P<tag>{tag_start}/?(?P<role>.*?){tag_end}\s*|$)",
-            text,
-        )
-        if match:
-            content = match.group("content")
-            if match.group("tag").startswith(f"{tag_start}/"):
-                raise Exception(f"Found end tag with no start `{match.group('tag')}`.")
-            if match.group("role") is not None and match.group("role") not in roles:
-                raise Exception(f"Unknown role `{match.group('role')}`.")
-            if content.strip():
-                messages.append({"role": default_role, "content": content.strip()})
-            text = text[match.span("tag")[1] :]  # noqa: E203
-            match_role = match.group("role")
-        if not text:
-            break
-        # now that we have defaulted any untagged text, we can handle the next tagged portion
-        match = re.search(rf"\s*.*?(?P<tag>{tag_start}/?(?P<role>.*?){tag_end}\s*)", text)
-        content = text[: match.span("tag")[0]]
-        if (match_role is not None and match.group("role") != match_role) or (not match.group("tag").startswith(f"{tag_start}/")):
-            raise Exception(f"Unclosed tag `{match_role}`. Found `{match.group('role')}`.")
-        messages.append({"role": match_role, "content": content.strip()})
-        text = text[match.span("tag")[1] :]  # noqa: E203
+    role = alt(*(string(s) for s in roles))
+    tag_begin = seq(
+        string(tag_start),
+        role,
+        string(tag_end),
+    )
+    tag_complete = seq(
+        string(tag_start),
+        string("/"),
+        role,
+        string(tag_end),
+    )
+
+    content = regex(r"([^%]+|\n(?!\s*%))+")
+
+    message = seq(tag_begin, content, tag_complete).map(lambda x: {'role': x[0][1], 'content': x[1]}) | content.map(
+        lambda x: {'role': default_role, 'content': x},
+    )
 
-    return messages
+    message_parser = message.at_least(1)
+    return message_parser.parse(text)
 
 
 def strip_tags(
     prompt: "Prompt",
     tag_start: str = "%",
     tag_end: str = "%",
     roles_seps: Dict[str, str] = {
```

### Comparing `headjack_keymaker-0.0.1a4/.gitignore` & `headjack_keymaker-0.1.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 *.ipynb
+pdm.lock
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
```

### Comparing `headjack_keymaker-0.0.1a4/pyproject.toml` & `headjack_keymaker-0.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     {name = "circargs", email = "nick@ouellet.dev"},
     {name = "Nick Ouellet", email = "nick@ouellet.dev"},
 ]
 dependencies = [
     "regex>=2023.6.3",
     "tiktoken>=0.4.0",
     "openai>=0.27.8",
+    "lark>=1.1.5",
+    "parsy>=2.1",
 ]
 
 requires-python = ">=3.8,<4.0"
 readme = "README.md"
 license = {text = "Apache 2.0"}
 
 [project.optional-dependencies]
@@ -39,15 +41,14 @@
     "coverage<8.0.0,>=7.2.3",
     "httpx>=0.24.0",
 ]
 
 [project.urls]
 repository = "https://github.com/KnowledgeForge/keymaker"
 
-
 [tool.hatch.version]
 path = "keymaker/__about__.py"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.black]
```

