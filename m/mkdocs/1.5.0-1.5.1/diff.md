# Comparing `tmp/mkdocs-1.5.0.tar.gz` & `tmp/mkdocs-1.5.1.tar.gz`

## Comparing `mkdocs-1.5.0.tar` & `mkdocs-1.5.1.tar`

### file list

```diff
@@ -1,236 +1,236 @@
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/__init__.py
--rw-r--r--   0        0        0    11907 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/__main__.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/exceptions.py
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/localization.py
--rw-r--r--   0        0        0    22697 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/plugins.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/py.typed
--rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/theme.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/commands/__init__.py
--rw-r--r--   0        0        0    13479 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/commands/build.py
--rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/commands/get_deps.py
--rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/commands/gh_deploy.py
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/commands/new.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/commands/serve.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/config/__init__.py
--rw-r--r--   0        0        0    13151 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/config/base.py
--rw-r--r--   0        0        0    43627 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/config/config_options.py
--rw-r--r--   0        0        0     7871 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/config/defaults.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/contrib/__init__.py
--rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/contrib/search/__init__.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/contrib/search/prebuild-index.js
--rw-r--r--   0        0        0     7965 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/contrib/search/search_index.py
--rw-r--r--   0        0        0    24525 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.ar.js
--rw-r--r--   0        0        0    10349 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.da.js
--rw-r--r--   0        0        0    13949 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.de.js
--rw-r--r--   0        0        0    15330 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.du.js
--rw-r--r--   0        0        0    24406 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.es.js
--rw-r--r--   0        0        0    20949 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.fi.js
--rw-r--r--   0        0        0    25654 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.fr.js
--rw-r--r--   0        0        0    21265 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.hu.js
--rw-r--r--   0        0        0    24077 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.it.js
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.ja.js
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.jp.js
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.multi.js
--rw-r--r--   0        0        0    15134 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.nl.js
--rw-r--r--   0        0        0     9947 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.no.js
--rw-r--r--   0        0        0    22141 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.pt.js
--rw-r--r--   0        0        0    23151 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.ro.js
--rw-r--r--   0        0        0    19108 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.ru.js
--rw-r--r--   0        0        0    13504 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.stemmer.support.js
--rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.sv.js
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.th.js
--rw-r--r--   0        0        0    38283 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.tr.js
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.vi.js
--rw-r--r--   0        0        0    22878 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/tinyseg.js
--rw-r--r--   0        0        0    99805 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/contrib/search/templates/search/lunr.js
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/contrib/search/templates/search/main.js
--rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/contrib/search/templates/search/worker.js
--rw-r--r--   0        0        0    12954 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/livereload/__init__.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/structure/__init__.py
--rw-r--r--   0        0        0    15152 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/structure/files.py
--rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/structure/nav.py
--rw-r--r--   0        0        0    17689 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/structure/pages.py
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/structure/toc.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/templates/sitemap.xml
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/__init__.py
--rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/base.py
--rw-r--r--   0        0        0    34742 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/build_tests.py
--rw-r--r--   0        0        0    25089 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/cli_tests.py
--rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/get_deps_tests.py
--rw-r--r--   0        0        0     7562 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/gh_deploy_tests.py
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/integration.py
--rw-r--r--   0        0        0    25502 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/livereload_tests.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/localization_tests.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/new_tests.py
--rw-r--r--   0        0        0    10915 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/plugin_tests.py
--rw-r--r--   0        0        0    24318 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/search_tests.py
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/theme_tests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/config/__init__.py
--rw-r--r--   0        0        0    10637 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/config/base_tests.py
--rw-r--r--   0        0        0    55357 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/config/config_options_legacy_tests.py
--rw-r--r--   0        0        0    82647 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/config/config_options_tests.py
--rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/config/config_tests.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/integration/projects.yaml
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/integration/complicated_config/mkdocs.yml
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/integration/complicated_config/documentation/custom.html
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/integration/complicated_config/documentation/index.md
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/integration/complicated_config/documentation/tweak.css
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/integration/complicated_config/documentation/tweak.js
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/integration/complicated_config/theme_tweaks/404.html
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/integration/minimal/mkdocs.yml
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/integration/minimal/docs/testing.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/integration/subpages/mkdocs.yml
--rw-r--r--   0        0        0    28320 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/integration/subpages/docs/image.png
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/integration/subpages/docs/index.md
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/integration/subpages/docs/metadata.md
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/integration/subpages/docs/non-index.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/integration/subpages/docs/page-title.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/integration/subpages/docs/pageTitle.md
--rw-r--r--   0        0        0    14085 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/integration/subpages/docs/sub1/image.png
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/integration/subpages/docs/sub1/index.md
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/integration/subpages/docs/sub1/non-index.md
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/integration/subpages/docs/sub1/sub1a/index.md
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/integration/subpages/docs/sub1/sub1a/non-index.md
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/integration/subpages/docs/sub2/index.md
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/integration/subpages/docs/sub2/non-index.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/integration/unicode/mkdocs.yml
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/integration/unicode/docs/index.md
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/integration/unicode/docs/Übersicht.md
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/integration/unicode/docs/♪.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/structure/__init__.py
--rw-r--r--   0        0        0    34219 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/structure/file_tests.py
--rw-r--r--   0        0        0    19090 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/structure/nav_tests.py
--rw-r--r--   0        0        0    52573 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/structure/page_tests.py
--rw-r--r--   0        0        0     5255 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/structure/toc_tests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/utils/__init__.py
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/utils/babel_stub_tests.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/utils/templates_tests.py
--rw-r--r--   0        0        0    21561 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/tests/utils/utils_tests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/__init__.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/babel.cfg
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/404.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/__init__.py
--rw-r--r--   0        0        0    10898 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/base.html
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/content.html
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/keyboard-modal.html
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/main.html
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/messages.pot
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/mkdocs_theme.yml
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/nav-sub.html
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/search-modal.html
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/toc.html
--rw-r--r--   0        0        0     6820 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/css/base.css
--rw-r--r--   0        0        0   163091 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/css/bootstrap.min.css
--rw-r--r--   0        0        0    31000 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/css/font-awesome.min.css
--rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/img/favicon.ico
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/img/grid.png
--rw-r--r--   0        0        0     7725 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/js/base.js
--rw-r--r--   0        0        0    58073 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/js/bootstrap.min.js
--rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/js/jquery-3.6.0.min.js
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/id/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/id/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/nb/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/nb/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/nn/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/nn/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/tr/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/404.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/__init__.py
--rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/base.html
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/breadcrumbs.html
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/footer.html
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/main.html
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/messages.pot
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/mkdocs_theme.yml
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/nav.html
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/search.html
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/searchbox.html
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/toc.html
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/versions.html
--rw-r--r--   0        0        0   135539 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/css/theme.css
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/css/theme_extra.css
--rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff
--rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff
--rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff2
--rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff
--rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff
--rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff2
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/img/favicon.ico
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/js/html5shiv.min.js
--rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/js/jquery-3.6.0.min.js
--rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/js/theme.js
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/js/theme_extra.js
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/id/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/id/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/tr/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    13370 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/utils/__init__.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/utils/babel_stub.py
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/utils/cache.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/utils/filters.py
--rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/utils/meta.py
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/utils/templates.py
--rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 mkdocs-1.5.0/mkdocs/utils/yaml.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 mkdocs-1.5.0/.gitignore
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 mkdocs-1.5.0/LICENSE
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 mkdocs-1.5.0/README.md
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 mkdocs-1.5.0/hatch_build.py
--rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 mkdocs-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 mkdocs-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/__init__.py
+-rw-r--r--   0        0        0    11907 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/__main__.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/exceptions.py
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/localization.py
+-rw-r--r--   0        0        0    22697 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/plugins.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/py.typed
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/theme.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/commands/__init__.py
+-rw-r--r--   0        0        0    13479 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/commands/build.py
+-rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/commands/get_deps.py
+-rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/commands/gh_deploy.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/commands/new.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/commands/serve.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/config/__init__.py
+-rw-r--r--   0        0        0    13151 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/config/base.py
+-rw-r--r--   0        0        0    43679 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/config/config_options.py
+-rw-r--r--   0        0        0     7871 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/config/defaults.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/__init__.py
+-rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/__init__.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/prebuild-index.js
+-rw-r--r--   0        0        0     7965 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/search_index.py
+-rw-r--r--   0        0        0    24525 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.ar.js
+-rw-r--r--   0        0        0    10349 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.da.js
+-rw-r--r--   0        0        0    13949 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.de.js
+-rw-r--r--   0        0        0    15330 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.du.js
+-rw-r--r--   0        0        0    24406 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.es.js
+-rw-r--r--   0        0        0    20949 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.fi.js
+-rw-r--r--   0        0        0    25654 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.fr.js
+-rw-r--r--   0        0        0    21265 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.hu.js
+-rw-r--r--   0        0        0    24077 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.it.js
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.ja.js
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.jp.js
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.multi.js
+-rw-r--r--   0        0        0    15134 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.nl.js
+-rw-r--r--   0        0        0     9947 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.no.js
+-rw-r--r--   0        0        0    22141 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.pt.js
+-rw-r--r--   0        0        0    23151 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.ro.js
+-rw-r--r--   0        0        0    19108 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.ru.js
+-rw-r--r--   0        0        0    13504 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.stemmer.support.js
+-rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.sv.js
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.th.js
+-rw-r--r--   0        0        0    38283 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.tr.js
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.vi.js
+-rw-r--r--   0        0        0    22878 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/tinyseg.js
+-rw-r--r--   0        0        0    99805 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/templates/search/lunr.js
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/templates/search/main.js
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/templates/search/worker.js
+-rw-r--r--   0        0        0    12954 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/livereload/__init__.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/structure/__init__.py
+-rw-r--r--   0        0        0    15376 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/structure/files.py
+-rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/structure/nav.py
+-rw-r--r--   0        0        0    17689 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/structure/pages.py
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/structure/toc.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/templates/sitemap.xml
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/__init__.py
+-rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/base.py
+-rw-r--r--   0        0        0    34742 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/build_tests.py
+-rw-r--r--   0        0        0    25089 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/cli_tests.py
+-rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/get_deps_tests.py
+-rw-r--r--   0        0        0     7562 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/gh_deploy_tests.py
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration.py
+-rw-r--r--   0        0        0    25502 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/livereload_tests.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/localization_tests.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/new_tests.py
+-rw-r--r--   0        0        0    10915 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/plugin_tests.py
+-rw-r--r--   0        0        0    24318 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/search_tests.py
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/theme_tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/config/__init__.py
+-rw-r--r--   0        0        0    10637 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/config/base_tests.py
+-rw-r--r--   0        0        0    55357 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/config/config_options_legacy_tests.py
+-rw-r--r--   0        0        0    82647 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/config/config_options_tests.py
+-rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/config/config_tests.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/projects.yaml
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/complicated_config/mkdocs.yml
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/complicated_config/documentation/custom.html
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/complicated_config/documentation/index.md
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/complicated_config/documentation/tweak.css
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/complicated_config/documentation/tweak.js
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/complicated_config/theme_tweaks/404.html
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/minimal/mkdocs.yml
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/minimal/docs/testing.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/subpages/mkdocs.yml
+-rw-r--r--   0        0        0    28320 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/subpages/docs/image.png
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/subpages/docs/index.md
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/subpages/docs/metadata.md
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/subpages/docs/non-index.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/subpages/docs/page-title.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/subpages/docs/pageTitle.md
+-rw-r--r--   0        0        0    14085 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/subpages/docs/sub1/image.png
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/subpages/docs/sub1/index.md
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/subpages/docs/sub1/non-index.md
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/subpages/docs/sub1/sub1a/index.md
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/subpages/docs/sub1/sub1a/non-index.md
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/subpages/docs/sub2/index.md
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/subpages/docs/sub2/non-index.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/unicode/mkdocs.yml
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/unicode/docs/index.md
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/unicode/docs/Übersicht.md
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/unicode/docs/♪.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/structure/__init__.py
+-rw-r--r--   0        0        0    34219 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/structure/file_tests.py
+-rw-r--r--   0        0        0    19090 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/structure/nav_tests.py
+-rw-r--r--   0        0        0    52573 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/structure/page_tests.py
+-rw-r--r--   0        0        0     5255 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/structure/toc_tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/utils/babel_stub_tests.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/utils/templates_tests.py
+-rw-r--r--   0        0        0    21561 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/utils/utils_tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/__init__.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/babel.cfg
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/404.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/__init__.py
+-rw-r--r--   0        0        0    10898 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/base.html
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/content.html
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/keyboard-modal.html
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/main.html
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/messages.pot
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/mkdocs_theme.yml
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/nav-sub.html
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/search-modal.html
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/toc.html
+-rw-r--r--   0        0        0     6820 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/css/base.css
+-rw-r--r--   0        0        0   163091 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/css/bootstrap.min.css
+-rw-r--r--   0        0        0    31000 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/css/font-awesome.min.css
+-rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/img/favicon.ico
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/img/grid.png
+-rw-r--r--   0        0        0     7725 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/js/base.js
+-rw-r--r--   0        0        0    58073 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/js/bootstrap.min.js
+-rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/js/jquery-3.6.0.min.js
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/id/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/id/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/nb/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/nb/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/nn/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/nn/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/tr/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/404.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/__init__.py
+-rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/base.html
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/breadcrumbs.html
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/footer.html
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/main.html
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/messages.pot
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/mkdocs_theme.yml
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/nav.html
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/search.html
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/searchbox.html
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/toc.html
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/versions.html
+-rw-r--r--   0        0        0   135539 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/theme.css
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/theme_extra.css
+-rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff
+-rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff2
+-rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff
+-rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff2
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/img/favicon.ico
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/js/html5shiv.min.js
+-rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/js/jquery-3.6.0.min.js
+-rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/js/theme.js
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/js/theme_extra.js
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/id/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/id/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/tr/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    13370 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/utils/__init__.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/utils/babel_stub.py
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/utils/cache.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/utils/filters.py
+-rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/utils/meta.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/utils/templates.py
+-rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/utils/yaml.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 mkdocs-1.5.1/.gitignore
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 mkdocs-1.5.1/LICENSE
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 mkdocs-1.5.1/README.md
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 mkdocs-1.5.1/hatch_build.py
+-rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 mkdocs-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 mkdocs-1.5.1/PKG-INFO
```

### Comparing `mkdocs-1.5.0/mkdocs/__main__.py` & `mkdocs-1.5.1/mkdocs/__main__.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/exceptions.py` & `mkdocs-1.5.1/mkdocs/exceptions.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/localization.py` & `mkdocs-1.5.1/mkdocs/localization.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/plugins.py` & `mkdocs-1.5.1/mkdocs/plugins.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/theme.py` & `mkdocs-1.5.1/mkdocs/theme.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/commands/build.py` & `mkdocs-1.5.1/mkdocs/commands/build.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/commands/get_deps.py` & `mkdocs-1.5.1/mkdocs/commands/get_deps.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/commands/gh_deploy.py` & `mkdocs-1.5.1/mkdocs/commands/gh_deploy.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/commands/new.py` & `mkdocs-1.5.1/mkdocs/commands/new.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/commands/serve.py` & `mkdocs-1.5.1/mkdocs/commands/serve.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/config/base.py` & `mkdocs-1.5.1/mkdocs/config/base.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/config/config_options.py` & `mkdocs-1.5.1/mkdocs/config/config_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -937,14 +937,17 @@
     def __init__(self, path: str = '', config_file_path=None):
         super().__init__(config_file_path=config_file_path)
         self.path = path
 
     def __str__(self):
         return self.path
 
+    def __fspath__(self):
+        return self.path
+
 
 class ExtraScript(SubConfig[ExtraScriptValue]):
     def run_validation(self, value: object) -> ExtraScriptValue:
         if isinstance(value, str):
             value = {'path': value, 'type': 'module' if value.endswith('.mjs') else ''}
         return super().run_validation(value)
```

### Comparing `mkdocs-1.5.0/mkdocs/config/defaults.py` & `mkdocs-1.5.1/mkdocs/config/defaults.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/contrib/search/__init__.py` & `mkdocs-1.5.1/mkdocs/contrib/search/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/contrib/search/prebuild-index.js` & `mkdocs-1.5.1/mkdocs/contrib/search/prebuild-index.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/contrib/search/search_index.py` & `mkdocs-1.5.1/mkdocs/contrib/search/search_index.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.ar.js` & `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.ar.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.da.js` & `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.da.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.de.js` & `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.de.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.du.js` & `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.du.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.es.js` & `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.es.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.fi.js` & `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.fi.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.fr.js` & `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.fr.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.hu.js` & `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.hu.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.it.js` & `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.it.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.ja.js` & `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.ja.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.multi.js` & `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.multi.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.nl.js` & `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.nl.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.no.js` & `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.no.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.pt.js` & `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.pt.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.ro.js` & `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.ro.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.ru.js` & `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.ru.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.stemmer.support.js` & `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.stemmer.support.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.sv.js` & `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.sv.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.th.js` & `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.th.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.tr.js` & `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.tr.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/lunr.vi.js` & `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.vi.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/contrib/search/lunr-language/tinyseg.js` & `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/tinyseg.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/contrib/search/templates/search/lunr.js` & `mkdocs-1.5.1/mkdocs/contrib/search/templates/search/lunr.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/contrib/search/templates/search/main.js` & `mkdocs-1.5.1/mkdocs/contrib/search/templates/search/main.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/contrib/search/templates/search/worker.js` & `mkdocs-1.5.1/mkdocs/contrib/search/templates/search/worker.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/livereload/__init__.py` & `mkdocs-1.5.1/mkdocs/livereload/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/structure/__init__.py` & `mkdocs-1.5.1/mkdocs/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/structure/files.py` & `mkdocs-1.5.1/mkdocs/structure/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -363,17 +363,23 @@
     # Skip README.md if an index file also exists in dir (part 2)
     for a, b in conflicting_files:
         if b.inclusion.is_included():
             if a.inclusion.is_included():
                 log.warning(
                     f"Excluding '{a.src_uri}' from the site because it conflicts with '{b.src_uri}'."
                 )
-            files.remove(a)
+            try:
+                files.remove(a)
+            except ValueError:
+                pass  # Catching this to avoid errors if attempting to remove the same file twice.
         else:
-            files.remove(b)
+            try:
+                files.remove(b)
+            except ValueError:
+                pass
 
     return Files(files)
 
 
 def _file_sort_key(f: str):
     """Always sort `index` or `README` as first filename in list."""
     return (os.path.splitext(f)[0] not in ('index', 'README'), f)
```

### Comparing `mkdocs-1.5.0/mkdocs/structure/nav.py` & `mkdocs-1.5.1/mkdocs/structure/nav.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/structure/pages.py` & `mkdocs-1.5.1/mkdocs/structure/pages.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/structure/toc.py` & `mkdocs-1.5.1/mkdocs/structure/toc.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/templates/sitemap.xml` & `mkdocs-1.5.1/mkdocs/templates/sitemap.xml`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/tests/base.py` & `mkdocs-1.5.1/mkdocs/tests/base.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/tests/build_tests.py` & `mkdocs-1.5.1/mkdocs/tests/build_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/tests/cli_tests.py` & `mkdocs-1.5.1/mkdocs/tests/cli_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/tests/get_deps_tests.py` & `mkdocs-1.5.1/mkdocs/tests/get_deps_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/tests/gh_deploy_tests.py` & `mkdocs-1.5.1/mkdocs/tests/gh_deploy_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/tests/integration.py` & `mkdocs-1.5.1/mkdocs/tests/integration.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/tests/livereload_tests.py` & `mkdocs-1.5.1/mkdocs/tests/livereload_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/tests/localization_tests.py` & `mkdocs-1.5.1/mkdocs/tests/localization_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/tests/new_tests.py` & `mkdocs-1.5.1/mkdocs/tests/new_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/tests/plugin_tests.py` & `mkdocs-1.5.1/mkdocs/tests/plugin_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/tests/search_tests.py` & `mkdocs-1.5.1/mkdocs/tests/search_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/tests/theme_tests.py` & `mkdocs-1.5.1/mkdocs/tests/theme_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/tests/config/base_tests.py` & `mkdocs-1.5.1/mkdocs/tests/config/base_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/tests/config/config_options_legacy_tests.py` & `mkdocs-1.5.1/mkdocs/tests/config/config_options_legacy_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/tests/config/config_options_tests.py` & `mkdocs-1.5.1/mkdocs/tests/config/config_options_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/tests/config/config_tests.py` & `mkdocs-1.5.1/mkdocs/tests/config/config_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/tests/integration/projects.yaml` & `mkdocs-1.5.1/mkdocs/tests/integration/projects.yaml`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/tests/integration/complicated_config/mkdocs.yml` & `mkdocs-1.5.1/mkdocs/tests/integration/complicated_config/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/tests/integration/subpages/docs/image.png` & `mkdocs-1.5.1/mkdocs/tests/integration/subpages/docs/image.png`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/tests/integration/subpages/docs/sub1/image.png` & `mkdocs-1.5.1/mkdocs/tests/integration/subpages/docs/sub1/image.png`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/tests/structure/file_tests.py` & `mkdocs-1.5.1/mkdocs/tests/structure/file_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/tests/structure/nav_tests.py` & `mkdocs-1.5.1/mkdocs/tests/structure/nav_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/tests/structure/page_tests.py` & `mkdocs-1.5.1/mkdocs/tests/structure/page_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/tests/structure/toc_tests.py` & `mkdocs-1.5.1/mkdocs/tests/structure/toc_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/tests/utils/babel_stub_tests.py` & `mkdocs-1.5.1/mkdocs/tests/utils/babel_stub_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/tests/utils/templates_tests.py` & `mkdocs-1.5.1/mkdocs/tests/utils/templates_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/tests/utils/utils_tests.py` & `mkdocs-1.5.1/mkdocs/tests/utils/utils_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/base.html` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/base.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/keyboard-modal.html` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/keyboard-modal.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/messages.pot` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/messages.pot`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/search-modal.html` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/search-modal.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/toc.html` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/toc.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/css/base.css` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/css/base.css`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/css/bootstrap.min.css` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/css/font-awesome.min.css` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.eot` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.svg` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.ttf` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff2` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/img/favicon.ico` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/img/grid.png` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/img/grid.png`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/js/base.js` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/js/base.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/js/bootstrap.min.js` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/js/jquery-3.6.0.min.js` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.mo` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.po` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.mo` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.po` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.mo` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.po` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.mo` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.po` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/id/LC_MESSAGES/messages.mo` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/id/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/id/LC_MESSAGES/messages.po` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/id/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.mo` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.po` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.mo` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.po` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/nb/LC_MESSAGES/messages.mo` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/nb/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/nb/LC_MESSAGES/messages.po` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/nb/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/nn/LC_MESSAGES/messages.mo` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/nn/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/nn/LC_MESSAGES/messages.po` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/nn/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.mo` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.po` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.mo` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.po` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/tr/LC_MESSAGES/messages.mo` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/tr/LC_MESSAGES/messages.po` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.mo` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.po` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.mo` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.po` & `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/base.html` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/base.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/breadcrumbs.html` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/footer.html` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/footer.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/messages.pot` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/messages.pot`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/nav.html` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/nav.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/search.html` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/search.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/versions.html` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/versions.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/css/theme.css` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/theme.css`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/css/theme_extra.css` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/theme_extra.css`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff2` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff2` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.eot` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.svg` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.ttf` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff2` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff2` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff2` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff2` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff2` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/img/favicon.ico` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/js/html5shiv.min.js` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/js/jquery-3.6.0.min.js` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/js/theme.js` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/js/theme.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.mo` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.po` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.mo` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.po` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.mo` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.po` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.mo` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.po` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/id/LC_MESSAGES/messages.mo` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/id/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/id/LC_MESSAGES/messages.po` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/id/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.mo` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.po` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.mo` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.po` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.mo` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.po` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.mo` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.po` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/tr/LC_MESSAGES/messages.mo` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/tr/LC_MESSAGES/messages.po` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.mo` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.po` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.mo` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.po` & `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/utils/__init__.py` & `mkdocs-1.5.1/mkdocs/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/utils/babel_stub.py` & `mkdocs-1.5.1/mkdocs/utils/babel_stub.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/utils/cache.py` & `mkdocs-1.5.1/mkdocs/utils/cache.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/utils/meta.py` & `mkdocs-1.5.1/mkdocs/utils/meta.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/utils/templates.py` & `mkdocs-1.5.1/mkdocs/utils/templates.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/mkdocs/utils/yaml.py` & `mkdocs-1.5.1/mkdocs/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/.gitignore` & `mkdocs-1.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/LICENSE` & `mkdocs-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/README.md` & `mkdocs-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/pyproject.toml` & `mkdocs-1.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.0/PKG-INFO` & `mkdocs-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs
-Version: 1.5.0
+Version: 1.5.1
 Summary: Project documentation with Markdown.
 Project-URL: Documentation, https://www.mkdocs.org/
 Project-URL: Source, https://github.com/mkdocs/mkdocs
 Project-URL: Issues, https://github.com/mkdocs/mkdocs/issues
 Project-URL: History, https://www.mkdocs.org/about/release-notes/
 Author-email: Tom Christie <tom@tomchristie.com>
 License-Expression: BSD-2-Clause
```

