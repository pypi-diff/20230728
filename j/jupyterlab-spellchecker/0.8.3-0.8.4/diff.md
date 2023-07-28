# Comparing `tmp/jupyterlab_spellchecker-0.8.3.tar.gz` & `tmp/jupyterlab_spellchecker-0.8.4.tar.gz`

## Comparing `jupyterlab_spellchecker-0.8.3.tar` & `jupyterlab_spellchecker-0.8.4.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/.eslintrc.js
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/.prettierignore
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/.stylelintrc
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/.yarnrc.yml
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/CHANGELOG.md
--rw-r--r--   0        0        0    18535 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/demo.gif
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/install.json
--rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/setup.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/tsconfig.json
--rw-r--r--   0        0        0   206920 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/yarn.lock
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/dictionaries/README.txt
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/dictionaries/README_de_ALL_frami.txt
--rw-r--r--   0        0        0    15732 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/dictionaries/README_en_AU.txt
--rw-r--r--   0        0        0    15732 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/dictionaries/README_en_CA.txt
--rw-r--r--   0        0        0    15740 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/dictionaries/README_en_GB-ise.txt
--rw-r--r--   0        0        0    15732 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/dictionaries/README_en_US.txt
--rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/dictionaries/README_es_ES.txt
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/dictionaries/README_fr.txt
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/dictionaries/README_pt_PT.txt
--rw-r--r--   0        0        0    19218 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/dictionaries/de_AT_frami.aff
--rw-r--r--   0        0        0  4422326 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/dictionaries/de_AT_frami.dic
--rw-r--r--   0        0        0    19218 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/dictionaries/de_CH_frami.aff
--rw-r--r--   0        0        0  4416507 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/dictionaries/de_CH_frami.dic
--rw-r--r--   0        0        0    19218 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/dictionaries/de_DE_frami.aff
--rw-r--r--   0        0        0  4419933 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/dictionaries/de_DE_frami.dic
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/dictionaries/en_AU.aff
--rw-r--r--   0        0        0   553854 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/dictionaries/en_AU.dic
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/dictionaries/en_CA.aff
--rw-r--r--   0        0        0   551079 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/dictionaries/en_CA.dic
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/dictionaries/en_GB-ise.aff
--rw-r--r--   0        0        0   551624 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/dictionaries/en_GB-ise.dic
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/dictionaries/en_US.aff
--rw-r--r--   0        0        0   551260 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/dictionaries/en_US.dic
--rw-r--r--   0        0        0   167076 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/dictionaries/es_ES.aff
--rw-r--r--   0        0        0   861168 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/dictionaries/es_ES.dic
--rw-r--r--   0        0        0   256857 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/dictionaries/fr.aff
--rw-r--r--   0        0        0  1100397 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/dictionaries/fr.dic
--rw-r--r--   0        0        0    42765 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/dictionaries/pt_PT.aff
--rw-r--r--   0        0        0   456494 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/dictionaries/pt_PT.dic
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/jupyter-config/nb-config/jupyterlab-spellchecker.json
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/jupyter-config/server-config/jupyterlab-spellchecker.json
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/jupyterlab_spellchecker/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/jupyterlab_spellchecker/_version.py
--rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/jupyterlab_spellchecker/dictionaries.py
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/jupyterlab_spellchecker/handlers.py
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/jupyterlab_spellchecker/labextension/package.json
--rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/jupyterlab_spellchecker/labextension/schemas/@jupyterlab-contrib/spellchecker/package.json.orig
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/jupyterlab_spellchecker/labextension/schemas/@jupyterlab-contrib/spellchecker/plugin.json
--rw-r--r--   0        0        0    12695 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/jupyterlab_spellchecker/labextension/static/552.d2bec066859ae2b0c6d2.js
--rw-r--r--   0        0        0     7943 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/jupyterlab_spellchecker/labextension/static/581.7b781918df8ce52c9a8f.js
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/jupyterlab_spellchecker/labextension/static/747.2f89d796d954e37784cd.js
--rw-r--r--   0        0        0    13936 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/jupyterlab_spellchecker/labextension/static/995.266a0ca9063d6df0c41f.js
--rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/jupyterlab_spellchecker/labextension/static/remoteEntry.fe331f8109a0c7b472be.js
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/jupyterlab_spellchecker/labextension/static/style.js
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/jupyterlab_spellchecker/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/jupyterlab_spellchecker/tests/test_dictionaries.py
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/schema/plugin.json
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/src/handler.ts
--rw-r--r--   0        0        0    23907 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/src/index.ts
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/src/loader.d.ts
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/src/svg.d.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/style/base.css
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/style/index.js
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/style/icons/LICENSE
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/style/icons/ic-baseline-spellcheck.svg
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/.gitignore
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/LICENSE
--rw-r--r--   0        0        0     6347 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/README.md
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     9123 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/.eslintrc.js
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/.prettierignore
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/.stylelintrc
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/.yarnrc.yml
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/CHANGELOG.md
+-rw-r--r--   0        0        0    18535 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/demo.gif
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/install.json
+-rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/tsconfig.json
+-rw-r--r--   0        0        0   207618 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/yarn.lock
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/dictionaries/README.txt
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/dictionaries/README_de_ALL_frami.txt
+-rw-r--r--   0        0        0    15732 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/dictionaries/README_en_AU.txt
+-rw-r--r--   0        0        0    15732 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/dictionaries/README_en_CA.txt
+-rw-r--r--   0        0        0    15740 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/dictionaries/README_en_GB-ise.txt
+-rw-r--r--   0        0        0    15732 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/dictionaries/README_en_US.txt
+-rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/dictionaries/README_es_ES.txt
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/dictionaries/README_fr.txt
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/dictionaries/README_pt_PT.txt
+-rw-r--r--   0        0        0    19218 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/dictionaries/de_AT_frami.aff
+-rw-r--r--   0        0        0  4422326 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/dictionaries/de_AT_frami.dic
+-rw-r--r--   0        0        0    19218 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/dictionaries/de_CH_frami.aff
+-rw-r--r--   0        0        0  4416507 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/dictionaries/de_CH_frami.dic
+-rw-r--r--   0        0        0    19218 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/dictionaries/de_DE_frami.aff
+-rw-r--r--   0        0        0  4419933 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/dictionaries/de_DE_frami.dic
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/dictionaries/en_AU.aff
+-rw-r--r--   0        0        0   553854 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/dictionaries/en_AU.dic
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/dictionaries/en_CA.aff
+-rw-r--r--   0        0        0   551079 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/dictionaries/en_CA.dic
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/dictionaries/en_GB-ise.aff
+-rw-r--r--   0        0        0   551624 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/dictionaries/en_GB-ise.dic
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/dictionaries/en_US.aff
+-rw-r--r--   0        0        0   551260 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/dictionaries/en_US.dic
+-rw-r--r--   0        0        0   167076 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/dictionaries/es_ES.aff
+-rw-r--r--   0        0        0   861168 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/dictionaries/es_ES.dic
+-rw-r--r--   0        0        0   256857 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/dictionaries/fr.aff
+-rw-r--r--   0        0        0  1100397 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/dictionaries/fr.dic
+-rw-r--r--   0        0        0    42765 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/dictionaries/pt_PT.aff
+-rw-r--r--   0        0        0   456494 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/dictionaries/pt_PT.dic
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/jupyter-config/nb-config/jupyterlab-spellchecker.json
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/jupyter-config/server-config/jupyterlab-spellchecker.json
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/jupyterlab_spellchecker/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/jupyterlab_spellchecker/_version.py
+-rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/jupyterlab_spellchecker/dictionaries.py
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/jupyterlab_spellchecker/handlers.py
+-rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/jupyterlab_spellchecker/labextension/package.json
+-rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/jupyterlab_spellchecker/labextension/schemas/@jupyterlab-contrib/spellchecker/package.json.orig
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/jupyterlab_spellchecker/labextension/schemas/@jupyterlab-contrib/spellchecker/plugin.json
+-rw-r--r--   0        0        0    12696 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/jupyterlab_spellchecker/labextension/static/552.6d7597412aeadbbf15fe.js
+-rw-r--r--   0        0        0     7943 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/jupyterlab_spellchecker/labextension/static/581.7b781918df8ce52c9a8f.js
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/jupyterlab_spellchecker/labextension/static/747.2f89d796d954e37784cd.js
+-rw-r--r--   0        0        0    13936 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/jupyterlab_spellchecker/labextension/static/995.266a0ca9063d6df0c41f.js
+-rw-r--r--   0        0        0     7683 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/jupyterlab_spellchecker/labextension/static/remoteEntry.afbfa74351e195593c24.js
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/jupyterlab_spellchecker/labextension/static/style.js
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/jupyterlab_spellchecker/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/jupyterlab_spellchecker/tests/test_dictionaries.py
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/schema/plugin.json
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/src/handler.ts
+-rw-r--r--   0        0        0    23907 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/src/index.ts
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/src/loader.d.ts
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/src/svg.d.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/style/base.css
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/style/index.js
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/style/icons/LICENSE
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/style/icons/ic-baseline-spellcheck.svg
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/.gitignore
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/LICENSE
+-rw-r--r--   0        0        0     6347 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/README.md
+-rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0     9155 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.4/PKG-INFO
```

### Comparing `jupyterlab_spellchecker-0.8.3/.eslintrc.js` & `jupyterlab_spellchecker-0.8.4/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/CHANGELOG.md` & `jupyterlab_spellchecker-0.8.4/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+### 0.8.4 (2023-07-28)
+
+- bug fixes:
+  - require JupyterLab 4
+
 ### 0.8.3 (2023-06-05)
 
 - bug fixes:
   - fix old status persisting in status bar when switching editors (but not typing anything yet)
   - fix dictionaries not being copied over on install
   - spellcheck in block comments and line comments in languages with C-like syntax
 - enhancements:
```

### Comparing `jupyterlab_spellchecker-0.8.3/demo.gif` & `jupyterlab_spellchecker-0.8.4/demo.gif`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/package.json` & `jupyterlab_spellchecker-0.8.4/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9716435185185186%*

 * *Differences: {"'devDependencies'": "{'stylelint': '^15.10.1'}", "'version'": "'0.8.4'"}*

```diff
@@ -47,15 +47,15 @@
         "eslint-plugin-prettier": "^4.2.1",
         "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.8.7",
         "rimraf": "^4.4.1",
         "source-map-loader": "^1.0.2",
         "style-loader": "^3.3.1",
-        "stylelint": "^14.9.1",
+        "stylelint": "^15.10.1",
         "stylelint-config-prettier": "^9.0.4",
         "stylelint-config-recommended": "^8.0.0",
         "stylelint-config-standard": "^26.0.0",
         "stylelint-prettier": "^2.0.0",
         "typescript": "~5.0.2",
         "yjs": "^13.5.40"
     },
@@ -120,9 +120,9 @@
         "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w --sourceMap"
     },
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.8.3"
+    "version": "0.8.4"
 }
```

### Comparing `jupyterlab_spellchecker-0.8.3/tsconfig.json` & `jupyterlab_spellchecker-0.8.4/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/yarn.lock` & `jupyterlab_spellchecker-0.8.4/yarn.lock`

 * *Files 1% similar despite different names*

```diff
@@ -288,20 +288,46 @@
     "@codemirror/state": ^6.1.4
     style-mod: ^4.0.0
     w3c-keyname: ^2.2.4
   checksum: f8fbb8e8cf1bc23de8cd64b1e645112d13f72cd2f1609fb9047d616908c2189ff518b89f21484371e7a37ba1804288452558e96488791f0c850f62b8e28dc163
   languageName: node
   linkType: hard
 
-"@csstools/selector-specificity@npm:^2.0.2":
-  version: 2.2.0
-  resolution: "@csstools/selector-specificity@npm:2.2.0"
+"@csstools/css-parser-algorithms@npm:^2.3.0":
+  version: 2.3.0
+  resolution: "@csstools/css-parser-algorithms@npm:2.3.0"
+  peerDependencies:
+    "@csstools/css-tokenizer": ^2.1.1
+  checksum: 3be22a0cfcfe0dc4bb140e2f266590addf21c5052d9e69334da860b3839fbd4369c3d158cbc396032d5ed96d01d2b5d8ebdb5497f75c9830ed9ce99853e3f915
+  languageName: node
+  linkType: hard
+
+"@csstools/css-tokenizer@npm:^2.1.1":
+  version: 2.1.1
+  resolution: "@csstools/css-tokenizer@npm:2.1.1"
+  checksum: d6ac4b08d7fdfc146755542f00b208af7248efd6cf2eb0f0f7d2ba3583a81f08ed9be6047d78b046925708b5bd0886f487edeeee2f90f0f34030dcbef4122d0e
+  languageName: node
+  linkType: hard
+
+"@csstools/media-query-list-parser@npm:^2.1.2":
+  version: 2.1.2
+  resolution: "@csstools/media-query-list-parser@npm:2.1.2"
   peerDependencies:
-    postcss-selector-parser: ^6.0.10
-  checksum: 97c89f23b3b527d7bd51ed299969ed2b9fbb219a367948b44aefec228b8eda6ae0ad74fe8a82f9aac8ff32cfd00bb6d0c98d1daeab2e8fc6d5c4af25e5be5673
+    "@csstools/css-parser-algorithms": ^2.3.0
+    "@csstools/css-tokenizer": ^2.1.1
+  checksum: 04936573ba837f14d7d637e172342c473665679c6497bbc0d548d93d08cb22e22151bb19e0e20422954c0b2aa50c3f38c9fc5f45c136e31bc863c656cb79df1b
+  languageName: node
+  linkType: hard
+
+"@csstools/selector-specificity@npm:^3.0.0":
+  version: 3.0.0
+  resolution: "@csstools/selector-specificity@npm:3.0.0"
+  peerDependencies:
+    postcss-selector-parser: ^6.0.13
+  checksum: 4a2dfe69998a499155d9dab4c2a0e7ae7594d8db98bb8a487d2d5347c0c501655051eb5eacad3fe323c86b0ba8212fe092c27fc883621e6ac2a27662edfc3528
   languageName: node
   linkType: hard
 
 "@discoveryjs/json-ext@npm:^0.5.0":
   version: 0.5.3
   resolution: "@discoveryjs/json-ext@npm:0.5.3"
   checksum: fea319569f9894391ff1ddb5f59f9dfebe611ac202e7e97d9719ff9f7a726388e6a0a7e5ae8e54cf009ae1748269760d5842bfda5b9cbf834ceda28711baf89d
@@ -454,15 +480,15 @@
     eslint-plugin-prettier: ^4.2.1
     mkdirp: ^1.0.3
     npm-run-all: ^4.1.5
     prettier: ^2.8.7
     rimraf: ^4.4.1
     source-map-loader: ^1.0.2
     style-loader: ^3.3.1
-    stylelint: ^14.9.1
+    stylelint: ^15.10.1
     stylelint-config-prettier: ^9.0.4
     stylelint-config-recommended: ^8.0.0
     stylelint-config-standard: ^26.0.0
     stylelint-prettier: ^2.0.0
     typescript: ~5.0.2
     typo-js: ^1.1.0
     yjs: ^13.5.40
@@ -1517,15 +1543,15 @@
 "@types/json-schema@npm:^7.0.8":
   version: 7.0.11
   resolution: "@types/json-schema@npm:7.0.11"
   checksum: 527bddfe62db9012fccd7627794bd4c71beb77601861055d87e3ee464f2217c85fca7a4b56ae677478367bbd248dbde13553312b7d4dbc702a2f2bbf60c4018d
   languageName: node
   linkType: hard
 
-"@types/minimist@npm:^1.2.0":
+"@types/minimist@npm:^1.2.2":
   version: 1.2.2
   resolution: "@types/minimist@npm:1.2.2"
   checksum: b8da83c66eb4aac0440e64674b19564d9d86c80ae273144db9681e5eeff66f238ade9515f5006ffbfa955ceff8b89ad2bd8ec577d7caee74ba101431fb07045d
   languageName: node
   linkType: hard
 
 "@types/node@npm:*":
@@ -1538,21 +1564,14 @@
 "@types/normalize-package-data@npm:^2.4.0":
   version: 2.4.1
   resolution: "@types/normalize-package-data@npm:2.4.1"
   checksum: e87bccbf11f95035c89a132b52b79ce69a1e3652fe55962363063c9c0dae0fe2477ebc585e03a9652adc6f381d24ba5589cc5e51849df4ced3d3e004a7d40ed5
   languageName: node
   linkType: hard
 
-"@types/parse-json@npm:^4.0.0":
-  version: 4.0.0
-  resolution: "@types/parse-json@npm:4.0.0"
-  checksum: fd6bce2b674b6efc3db4c7c3d336bd70c90838e8439de639b909ce22f3720d21344f52427f1d9e57b265fcb7f6c018699b99e5e0c208a1a4823014269a6bf35b
-  languageName: node
-  linkType: hard
-
 "@types/prop-types@npm:*":
   version: 15.7.3
   resolution: "@types/prop-types@npm:15.7.3"
   checksum: 41831d53c44c9eeafdaf9762bcb4553c13a3bbf990745ed9065a1cc3581b80633113b53fd49b202bf51731b258da5d0a9aa09c9035d5af7f78b0f6bc273f1325
   languageName: node
   linkType: hard
 
@@ -2177,29 +2196,30 @@
 "callsites@npm:^3.0.0":
   version: 3.1.0
   resolution: "callsites@npm:3.1.0"
   checksum: 072d17b6abb459c2ba96598918b55868af677154bec7e73d222ef95a8fdb9bbf7dae96a8421085cdad8cd190d86653b5b6dc55a4484f2e5b2e27d5e0c3fc15b3
   languageName: node
   linkType: hard
 
-"camelcase-keys@npm:^6.2.2":
-  version: 6.2.2
-  resolution: "camelcase-keys@npm:6.2.2"
+"camelcase-keys@npm:^7.0.0":
+  version: 7.0.2
+  resolution: "camelcase-keys@npm:7.0.2"
   dependencies:
-    camelcase: ^5.3.1
-    map-obj: ^4.0.0
-    quick-lru: ^4.0.1
-  checksum: 43c9af1adf840471e54c68ab3e5fe8a62719a6b7dbf4e2e86886b7b0ff96112c945736342b837bd2529ec9d1c7d1934e5653318478d98e0cf22c475c04658e2a
+    camelcase: ^6.3.0
+    map-obj: ^4.1.0
+    quick-lru: ^5.1.1
+    type-fest: ^1.2.1
+  checksum: b5821cc48dd00e8398a30c5d6547f06837ab44de123f1b3a603d0a03399722b2fc67a485a7e47106eb02ef543c3b50c5ebaabc1242cde4b63a267c3258d2365b
   languageName: node
   linkType: hard
 
-"camelcase@npm:^5.3.1":
-  version: 5.3.1
-  resolution: "camelcase@npm:5.3.1"
-  checksum: e6effce26b9404e3c0f301498184f243811c30dfe6d0b9051863bd8e4034d09c8c2923794f280d6827e5aa055f6c434115ff97864a16a963366fb35fd673024b
+"camelcase@npm:^6.3.0":
+  version: 6.3.0
+  resolution: "camelcase@npm:6.3.0"
+  checksum: 8c96818a9076434998511251dcb2761a94817ea17dbdc37f47ac080bd088fc62c7369429a19e2178b993497132c8cbcf5cc1f44ba963e76782ba469c0474938d
   languageName: node
   linkType: hard
 
 "caniuse-lite@npm:^1.0.30001219":
   version: 1.0.30001228
   resolution: "caniuse-lite@npm:1.0.30001228"
   checksum: d7ea2234d3ad1841dab6cd0b6ee16e89958f5893ef2e024a7447d6f889f496e40b6dafe000f391b8d4f0c0ef08671dbb5969fd66e6f74d402994865ce5705a53
@@ -2345,24 +2365,23 @@
 "concat-map@npm:0.0.1":
   version: 0.0.1
   resolution: "concat-map@npm:0.0.1"
   checksum: 902a9f5d8967a3e2faf138d5cb784b9979bad2e6db5357c5b21c568df4ebe62bcb15108af1b2253744844eb964fc023fbd9afbbbb6ddd0bcc204c6fb5b7bf3af
   languageName: node
   linkType: hard
 
-"cosmiconfig@npm:^7.1.0":
-  version: 7.1.0
-  resolution: "cosmiconfig@npm:7.1.0"
+"cosmiconfig@npm:^8.2.0":
+  version: 8.2.0
+  resolution: "cosmiconfig@npm:8.2.0"
   dependencies:
-    "@types/parse-json": ^4.0.0
     import-fresh: ^3.2.1
+    js-yaml: ^4.1.0
     parse-json: ^5.0.0
     path-type: ^4.0.0
-    yaml: ^1.10.0
-  checksum: c53bf7befc1591b2651a22414a5e786cd5f2eeaa87f3678a3d49d6069835a9d8d1aef223728e98aa8fec9a95bf831120d245096db12abe019fecb51f5696c96f
+  checksum: 836d5d8efa750f3fb17b03d6ca74cd3154ed025dffd045304b3ef59637f662bde1e5dc88f8830080d180ec60841719cf4ea2ce73fb21ec694b16865c478ff297
   languageName: node
   linkType: hard
 
 "crelt@npm:^1.0.5":
   version: 1.0.6
   resolution: "crelt@npm:1.0.6"
   checksum: dad842093371ad702afbc0531bfca2b0a8dd920b23a42f26e66dabbed9aad9acd5b9030496359545ef3937c3aced0fd4ac39f7a2d280a23ddf9eb7fdcb94a69f
@@ -2414,14 +2433,24 @@
     semver: ^7.3.8
   peerDependencies:
     webpack: ^5.0.0
   checksum: 7c1784247bdbe76dc5c55fb1ac84f1d4177a74c47259942c9cfdb7a8e6baef11967a0bc85ac285f26bd26d5059decb848af8154a03fdb4f4894f41212f45eef3
   languageName: node
   linkType: hard
 
+"css-tree@npm:^2.3.1":
+  version: 2.3.1
+  resolution: "css-tree@npm:2.3.1"
+  dependencies:
+    mdn-data: 2.0.30
+    source-map-js: ^1.0.1
+  checksum: 493cc24b5c22b05ee5314b8a0d72d8a5869491c1458017ae5ed75aeb6c3596637dbe1b11dac2548974624adec9f7a1f3a6cf40593dc1f9185eb0e8279543fbc0
+  languageName: node
+  linkType: hard
+
 "cssesc@npm:^3.0.0":
   version: 3.0.0
   resolution: "cssesc@npm:3.0.0"
   bin:
     cssesc: bin/cssesc
   checksum: f8c4ababffbc5e2ddf2fa9957dda1ee4af6048e22aeda1869d0d00843223c1b13ad3f5d88b51caa46c994225eacb636b764eb807a8883e2fb6f99b4f4e8c48b2
   languageName: node
@@ -2482,21 +2511,28 @@
   dependencies:
     decamelize: ^1.1.0
     map-obj: ^1.0.0
   checksum: fc645fe20b7bda2680bbf9481a3477257a7f9304b1691036092b97ab04c0ab53e3bf9fcc2d2ae382536568e402ec41fb11e1d4c3836a9abe2d813dd9ef4311e0
   languageName: node
   linkType: hard
 
-"decamelize@npm:^1.1.0, decamelize@npm:^1.2.0":
+"decamelize@npm:^1.1.0":
   version: 1.2.0
   resolution: "decamelize@npm:1.2.0"
   checksum: ad8c51a7e7e0720c70ec2eeb1163b66da03e7616d7b98c9ef43cce2416395e84c1e9548dd94f5f6ffecfee9f8b94251fc57121a8b021f2ff2469b2bae247b8aa
   languageName: node
   linkType: hard
 
+"decamelize@npm:^5.0.0":
+  version: 5.0.1
+  resolution: "decamelize@npm:5.0.1"
+  checksum: 7c3b1ed4b3e60e7fbc00a35fb248298527c1cdfe603e41dfcf05e6c4a8cb9efbee60630deb677ed428908fb4e74e322966c687a094d1478ddc9c3a74e9dc7140
+  languageName: node
+  linkType: hard
+
 "deep-is@npm:^0.1.3":
   version: 0.1.3
   resolution: "deep-is@npm:0.1.3"
   checksum: c15b04c3848a89880c94e25b077c19b47d9a30dd99048e70e5f95d943e7b246bee1da0c1376b56b01bc045be2cae7d9b1c856e68e47e9805634327de7c6cb6d5
   languageName: node
   linkType: hard
 
@@ -2872,15 +2908,15 @@
 "fast-diff@npm:^1.1.2":
   version: 1.2.0
   resolution: "fast-diff@npm:1.2.0"
   checksum: 1b5306eaa9e826564d9e5ffcd6ebd881eb5f770b3f977fcbf38f05c824e42172b53c79920e8429c54eb742ce15a0caf268b0fdd5b38f6de52234c4a8368131ae
   languageName: node
   linkType: hard
 
-"fast-glob@npm:^3.2.12, fast-glob@npm:^3.2.9":
+"fast-glob@npm:^3.2.9, fast-glob@npm:^3.3.0":
   version: 3.3.0
   resolution: "fast-glob@npm:3.3.0"
   dependencies:
     "@nodelib/fs.stat": ^2.0.2
     "@nodelib/fs.walk": ^1.2.3
     glob-parent: ^5.1.2
     merge2: ^1.3.0
@@ -2947,15 +2983,15 @@
 "find-root@npm:^1.0.0":
   version: 1.1.0
   resolution: "find-root@npm:1.1.0"
   checksum: b2a59fe4b6c932eef36c45a048ae8f93c85640212ebe8363164814990ee20f154197505965f3f4f102efc33bfb1cbc26fd17c4a2fc739ebc51b886b137cbefaf
   languageName: node
   linkType: hard
 
-"find-up@npm:^4.0.0, find-up@npm:^4.1.0":
+"find-up@npm:^4.0.0":
   version: 4.1.0
   resolution: "find-up@npm:4.1.0"
   dependencies:
     locate-path: ^5.0.0
     path-exists: ^4.0.0
   checksum: 4c172680e8f8c1f78839486e14a43ef82e9decd0e74145f40707cc42e7420506d5ec92d9a11c22bd2c48fb0c384ea05dd30e10dd152fefeec6f2f75282a8b844
   languageName: node
@@ -3216,15 +3252,15 @@
   resolution: "hosted-git-info@npm:4.1.0"
   dependencies:
     lru-cache: ^6.0.0
   checksum: c3f87b3c2f7eb8c2748c8f49c0c2517c9a95f35d26f4bf54b2a8cba05d2e668f3753548b6ea366b18ec8dadb4e12066e19fa382a01496b0ffa0497eb23cbe461
   languageName: node
   linkType: hard
 
-"html-tags@npm:^3.2.0":
+"html-tags@npm:^3.3.1":
   version: 3.3.1
   resolution: "html-tags@npm:3.3.1"
   checksum: b4ef1d5a76b678e43cce46e3783d563607b1d550cab30b4f511211564574770aa8c658a400b100e588bc60b8234e59b35ff72c7851cc28f3b5403b13a2c6cbce
   languageName: node
   linkType: hard
 
 "htmlparser2@npm:^6.0.0":
@@ -3253,15 +3289,15 @@
   resolution: "icss-utils@npm:5.1.0"
   peerDependencies:
     postcss: ^8.1.0
   checksum: 5c324d283552b1269cfc13a503aaaa172a280f914e5b81544f3803bc6f06a3b585fb79f66f7c771a2c052db7982c18bf92d001e3b47282e3abbbb4c4cc488d68
   languageName: node
   linkType: hard
 
-"ignore@npm:^5.2.0, ignore@npm:^5.2.1":
+"ignore@npm:^5.2.0, ignore@npm:^5.2.4":
   version: 5.2.4
   resolution: "ignore@npm:5.2.4"
   checksum: 3d4c309c6006e2621659311783eaea7ebcd41fe4ca1d78c91c473157ad6666a57a2df790fe0d07a12300d9aac2888204d7be8d59f9aaf665b1c7fcdb432517ef
   languageName: node
   linkType: hard
 
 "import-fresh@npm:^3.0.0, import-fresh@npm:^3.2.1":
@@ -3296,18 +3332,18 @@
 "imurmurhash@npm:^0.1.4":
   version: 0.1.4
   resolution: "imurmurhash@npm:0.1.4"
   checksum: 7cae75c8cd9a50f57dadd77482359f659eaebac0319dd9368bcd1714f55e65badd6929ca58569da2b6494ef13fdd5598cd700b1eba23f8b79c5f19d195a3ecf7
   languageName: node
   linkType: hard
 
-"indent-string@npm:^4.0.0":
-  version: 4.0.0
-  resolution: "indent-string@npm:4.0.0"
-  checksum: 824cfb9929d031dabf059bebfe08cf3137365e112019086ed3dcff6a0a7b698cb80cf67ccccde0e25b9e2d7527aa6cc1fed1ac490c752162496caba3e6699612
+"indent-string@npm:^5.0.0":
+  version: 5.0.0
+  resolution: "indent-string@npm:5.0.0"
+  checksum: e466c27b6373440e6d84fbc19e750219ce25865cb82d578e41a6053d727e5520dc5725217d6eb1cc76005a1bb1696a0f106d84ce7ebda3033b963a38583fb3b3
   languageName: node
   linkType: hard
 
 "inflight@npm:^1.0.4":
   version: 1.0.6
   resolution: "inflight@npm:1.0.6"
   dependencies:
@@ -3650,18 +3686,18 @@
 "kind-of@npm:^6.0.2, kind-of@npm:^6.0.3":
   version: 6.0.3
   resolution: "kind-of@npm:6.0.3"
   checksum: 3ab01e7b1d440b22fe4c31f23d8d38b4d9b91d9f291df683476576493d5dfd2e03848a8b05813dd0c3f0e835bc63f433007ddeceb71f05cb25c45ae1b19c6d3b
   languageName: node
   linkType: hard
 
-"known-css-properties@npm:^0.26.0":
-  version: 0.26.0
-  resolution: "known-css-properties@npm:0.26.0"
-  checksum: e706f4af9d2683202df9f717e7d713f0f8c3330f155842c40d8f3b2a5837956c34aeb7ba08760977ccde1afce8b5377e29b40eb3e5c0b42bef28ddd108543cfb
+"known-css-properties@npm:^0.27.0":
+  version: 0.27.0
+  resolution: "known-css-properties@npm:0.27.0"
+  checksum: 8584fcf0526f984fe5a358af20200dec3b944373dd005dc23a3ce988895e1acd03e7d69c49533dda07d6d9b6d53990ed1119bd9d3e927f17545f8764c434a5cd
   languageName: node
   linkType: hard
 
 "levn@npm:^0.4.1":
   version: 0.4.1
   resolution: "levn@npm:0.4.1"
   dependencies:
@@ -3823,15 +3859,15 @@
 "map-obj@npm:^1.0.0":
   version: 1.0.1
   resolution: "map-obj@npm:1.0.1"
   checksum: 9949e7baec2a336e63b8d4dc71018c117c3ce6e39d2451ccbfd3b8350c547c4f6af331a4cbe1c83193d7c6b786082b6256bde843db90cb7da2a21e8fcc28afed
   languageName: node
   linkType: hard
 
-"map-obj@npm:^4.0.0":
+"map-obj@npm:^4.1.0":
   version: 4.3.0
   resolution: "map-obj@npm:4.3.0"
   checksum: fbc554934d1a27a1910e842bc87b177b1a556609dd803747c85ece420692380827c6ae94a95cce4407c054fa0964be3bf8226f7f2cb2e9eeee432c7c1985684e
   languageName: node
   linkType: hard
 
 "markdown-to-jsx@npm:^7.2.1":
@@ -3846,38 +3882,45 @@
 "mathml-tag-names@npm:^2.1.3":
   version: 2.1.3
   resolution: "mathml-tag-names@npm:2.1.3"
   checksum: 1201a25a137d6b9e328facd67912058b8b45b19a6c4cc62641c9476195da28a275ca6e0eca070af5378b905c2b11abc1114676ba703411db0b9ce007de921ad0
   languageName: node
   linkType: hard
 
+"mdn-data@npm:2.0.30":
+  version: 2.0.30
+  resolution: "mdn-data@npm:2.0.30"
+  checksum: d6ac5ac7439a1607df44b22738ecf83f48e66a0874e4482d6424a61c52da5cde5750f1d1229b6f5fa1b80a492be89465390da685b11f97d62b8adcc6e88189aa
+  languageName: node
+  linkType: hard
+
 "memorystream@npm:^0.3.1":
   version: 0.3.1
   resolution: "memorystream@npm:0.3.1"
   checksum: f18b42440d24d09516d01466c06adf797df7873f0d40aa7db02e5fb9ed83074e5e65412d0720901d7069363465f82dc4f8bcb44f0cde271567a61426ce6ca2e9
   languageName: node
   linkType: hard
 
-"meow@npm:^9.0.0":
-  version: 9.0.0
-  resolution: "meow@npm:9.0.0"
-  dependencies:
-    "@types/minimist": ^1.2.0
-    camelcase-keys: ^6.2.2
-    decamelize: ^1.2.0
+"meow@npm:^10.1.5":
+  version: 10.1.5
+  resolution: "meow@npm:10.1.5"
+  dependencies:
+    "@types/minimist": ^1.2.2
+    camelcase-keys: ^7.0.0
+    decamelize: ^5.0.0
     decamelize-keys: ^1.1.0
     hard-rejection: ^2.1.0
     minimist-options: 4.1.0
-    normalize-package-data: ^3.0.0
-    read-pkg-up: ^7.0.1
-    redent: ^3.0.0
-    trim-newlines: ^3.0.0
-    type-fest: ^0.18.0
-    yargs-parser: ^20.2.3
-  checksum: 99799c47247f4daeee178e3124f6ef6f84bde2ba3f37652865d5d8f8b8adcf9eedfc551dd043e2455cd8206545fd848e269c0c5ab6b594680a0ad4d3617c9639
+    normalize-package-data: ^3.0.2
+    read-pkg-up: ^8.0.0
+    redent: ^4.0.0
+    trim-newlines: ^4.0.2
+    type-fest: ^1.2.2
+    yargs-parser: ^20.2.9
+  checksum: dd5f0caa4af18517813547dc66741dcbf52c4c23def5062578d39b11189fd9457aee5c1f2263a5cd6592a465023df8357e8ac876b685b64dbcf545e3f66c23a7
   languageName: node
   linkType: hard
 
 "merge-stream@npm:^2.0.0":
   version: 2.0.0
   resolution: "merge-stream@npm:2.0.0"
   checksum: 6fa4dcc8d86629705cea944a4b88ef4cb0e07656ebf223fa287443256414283dd25d91c1cd84c77987f2aec5927af1a9db6085757cb43d90eb170ebf4b47f4f4
@@ -3913,15 +3956,15 @@
   resolution: "mime-types@npm:2.1.30"
   dependencies:
     mime-db: 1.47.0
   checksum: 53c36729b1c4f6029fd5957d5859e62eff4b86311a6e1dce87937583dc8971fec9f359ffcff4be93d26bb5ddd03f1b5ffc7626912031ce0a63510d7896521b2e
   languageName: node
   linkType: hard
 
-"min-indent@npm:^1.0.0":
+"min-indent@npm:^1.0.1":
   version: 1.0.1
   resolution: "min-indent@npm:1.0.1"
   checksum: bfc6dd03c5eaf623a4963ebd94d087f6f4bbbfd8c41329a7f09706b0cb66969c4ddd336abeb587bc44bc6f08e13bf90f0b374f9d71f9f01e04adc2cd6f083ef1
   languageName: node
   linkType: hard
 
 "mini-css-extract-plugin@npm:^2.7.0":
@@ -4050,27 +4093,27 @@
 "node-releases@npm:^1.1.71":
   version: 1.1.72
   resolution: "node-releases@npm:1.1.72"
   checksum: 84dacd44e6595c76e3097b69051b24bf5c3bdb374efc9bef343200ffa183fce10a31ba1c763af51d897ba0f6d00cd1e10eb34a03146688ce4cb051f1d80c402b
   languageName: node
   linkType: hard
 
-"normalize-package-data@npm:^2.3.2, normalize-package-data@npm:^2.5.0":
+"normalize-package-data@npm:^2.3.2":
   version: 2.5.0
   resolution: "normalize-package-data@npm:2.5.0"
   dependencies:
     hosted-git-info: ^2.1.4
     resolve: ^1.10.0
     semver: 2 || 3 || 4 || 5
     validate-npm-package-license: ^3.0.1
   checksum: 7999112efc35a6259bc22db460540cae06564aa65d0271e3bdfa86876d08b0e578b7b5b0028ee61b23f1cae9fc0e7847e4edc0948d3068a39a2a82853efc8499
   languageName: node
   linkType: hard
 
-"normalize-package-data@npm:^3.0.0":
+"normalize-package-data@npm:^3.0.2":
   version: 3.0.3
   resolution: "normalize-package-data@npm:3.0.3"
   dependencies:
     hosted-git-info: ^4.0.1
     is-core-module: ^2.5.0
     semver: ^7.3.4
     validate-npm-package-license: ^3.0.1
@@ -4220,15 +4263,15 @@
   dependencies:
     error-ex: ^1.3.1
     json-parse-better-errors: ^1.0.1
   checksum: 0fe227d410a61090c247e34fa210552b834613c006c2c64d9a05cfe9e89cf8b4246d1246b1a99524b53b313e9ac024438d0680f67e33eaed7e6f38db64cfe7b5
   languageName: node
   linkType: hard
 
-"parse-json@npm:^5.0.0":
+"parse-json@npm:^5.0.0, parse-json@npm:^5.2.0":
   version: 5.2.0
   resolution: "parse-json@npm:5.2.0"
   dependencies:
     "@babel/code-frame": ^7.0.0
     error-ex: ^1.3.1
     json-parse-even-better-errors: ^2.3.0
     lines-and-columns: ^1.1.6
@@ -4346,21 +4389,14 @@
   resolution: "pkg-dir@npm:4.2.0"
   dependencies:
     find-up: ^4.0.0
   checksum: 9863e3f35132bf99ae1636d31ff1e1e3501251d480336edb1c211133c8d58906bed80f154a1d723652df1fda91e01c7442c2eeaf9dc83157c7ae89087e43c8d6
   languageName: node
   linkType: hard
 
-"postcss-media-query-parser@npm:^0.2.3":
-  version: 0.2.3
-  resolution: "postcss-media-query-parser@npm:0.2.3"
-  checksum: 8000d4d95b912994928ff86137f5ab0ed4c4ee1498af2336e93d708ae8827a690cd7acbaed55d14684cf44d82c8d44b031c1c69ae6bcd2f9620ea67573888090
-  languageName: node
-  linkType: hard
-
 "postcss-modules-extract-imports@npm:^3.0.0":
   version: 3.0.0
   resolution: "postcss-modules-extract-imports@npm:3.0.0"
   peerDependencies:
     postcss: ^8.1.0
   checksum: 4b65f2f1382d89c4bc3c0a1bdc5942f52f3cb19c110c57bd591ffab3a5fee03fcf831604168205b0c1b631a3dce2255c70b61aaae3ef39d69cd7eb450c2552d2
   languageName: node
@@ -4413,15 +4449,15 @@
   resolution: "postcss-safe-parser@npm:6.0.0"
   peerDependencies:
     postcss: ^8.3.3
   checksum: 06c733eaad83a3954367e7ee02ddfe3796e7a44d4299ccf9239f40964a4daac153c7d77613f32964b5a86c0c6c2f6167738f31d578b73b17cb69d0c4446f0ebe
   languageName: node
   linkType: hard
 
-"postcss-selector-parser@npm:^6.0.11":
+"postcss-selector-parser@npm:^6.0.13":
   version: 6.0.13
   resolution: "postcss-selector-parser@npm:6.0.13"
   dependencies:
     cssesc: ^3.0.0
     util-deprecate: ^1.0.2
   checksum: f89163338a1ce3b8ece8e9055cd5a3165e79a15e1c408e18de5ad8f87796b61ec2d48a2902d179ae0c4b5de10fccd3a325a4e660596549b040bc5ad1b465f096
   languageName: node
@@ -4447,25 +4483,36 @@
 "postcss-value-parser@npm:^4.2.0":
   version: 4.2.0
   resolution: "postcss-value-parser@npm:4.2.0"
   checksum: 819ffab0c9d51cf0acbabf8996dffbfafbafa57afc0e4c98db88b67f2094cb44488758f06e5da95d7036f19556a4a732525e84289a425f4f6fd8e412a9d7442f
   languageName: node
   linkType: hard
 
-"postcss@npm:^8.3.11, postcss@npm:^8.4.19, postcss@npm:^8.4.21":
+"postcss@npm:^8.3.11, postcss@npm:^8.4.21":
   version: 8.4.24
   resolution: "postcss@npm:8.4.24"
   dependencies:
     nanoid: ^3.3.6
     picocolors: ^1.0.0
     source-map-js: ^1.0.2
   checksum: 814e2126dacfea313588eda09cc99a9b4c26ec55c059188aa7a916d20d26d483483106dc5ff9e560731b59f45c5bb91b945dfadc670aed875cc90ddbbf4e787d
   languageName: node
   linkType: hard
 
+"postcss@npm:^8.4.24":
+  version: 8.4.25
+  resolution: "postcss@npm:8.4.25"
+  dependencies:
+    nanoid: ^3.3.6
+    picocolors: ^1.0.0
+    source-map-js: ^1.0.2
+  checksum: 9ed3ab8af43ad5210c28f56f916fd9b8c9f94fbeaebbf645dcf579bc28bdd8056c2a7ecc934668d399b81fedb6128f0c4b299f931e50454964bc911c25a3a0a2
+  languageName: node
+  linkType: hard
+
 "prelude-ls@npm:^1.2.1":
   version: 1.2.1
   resolution: "prelude-ls@npm:1.2.1"
   checksum: cd192ec0d0a8e4c6da3bb80e4f62afe336df3f76271ac6deb0e6a36187133b6073a19e9727a1ff108cd8b9982e4768850d413baa71214dd80c7979617dca827a
   languageName: node
   linkType: hard
 
@@ -4529,18 +4576,18 @@
 "queue-microtask@npm:^1.2.2":
   version: 1.2.3
   resolution: "queue-microtask@npm:1.2.3"
   checksum: b676f8c040cdc5b12723ad2f91414d267605b26419d5c821ff03befa817ddd10e238d22b25d604920340fd73efd8ba795465a0377c4adf45a4a41e4234e42dc4
   languageName: node
   linkType: hard
 
-"quick-lru@npm:^4.0.1":
-  version: 4.0.1
-  resolution: "quick-lru@npm:4.0.1"
-  checksum: bea46e1abfaa07023e047d3cf1716a06172c4947886c053ede5c50321893711577cb6119360f810cc3ffcd70c4d7db4069c3cee876b358ceff8596e062bd1154
+"quick-lru@npm:^5.1.1":
+  version: 5.1.1
+  resolution: "quick-lru@npm:5.1.1"
+  checksum: a516faa25574be7947969883e6068dbe4aa19e8ef8e8e0fd96cddd6d36485e9106d85c0041a27153286b0770b381328f4072aa40d3b18a19f5f7d2b78b94b5ed
   languageName: node
   linkType: hard
 
 "randombytes@npm:^2.1.0":
   version: 2.1.0
   resolution: "randombytes@npm:2.1.0"
   dependencies:
@@ -4580,64 +4627,64 @@
   resolution: "react@npm:18.2.0"
   dependencies:
     loose-envify: ^1.1.0
   checksum: 88e38092da8839b830cda6feef2e8505dec8ace60579e46aa5490fc3dc9bba0bd50336507dc166f43e3afc1c42939c09fe33b25fae889d6f402721dcd78fca1b
   languageName: node
   linkType: hard
 
-"read-pkg-up@npm:^7.0.1":
-  version: 7.0.1
-  resolution: "read-pkg-up@npm:7.0.1"
+"read-pkg-up@npm:^8.0.0":
+  version: 8.0.0
+  resolution: "read-pkg-up@npm:8.0.0"
   dependencies:
-    find-up: ^4.1.0
-    read-pkg: ^5.2.0
-    type-fest: ^0.8.1
-  checksum: e4e93ce70e5905b490ca8f883eb9e48b5d3cebc6cd4527c25a0d8f3ae2903bd4121c5ab9c5a3e217ada0141098eeb661313c86fa008524b089b8ed0b7f165e44
+    find-up: ^5.0.0
+    read-pkg: ^6.0.0
+    type-fest: ^1.0.1
+  checksum: fe4c80401656b40b408884457fffb5a8015c03b1018cfd8e48f8d82a5e9023e24963603aeb2755608d964593e046c15b34d29b07d35af9c7aa478be81805209c
   languageName: node
   linkType: hard
 
 "read-pkg@npm:^3.0.0":
   version: 3.0.0
   resolution: "read-pkg@npm:3.0.0"
   dependencies:
     load-json-file: ^4.0.0
     normalize-package-data: ^2.3.2
     path-type: ^3.0.0
   checksum: 398903ebae6c7e9965419a1062924436cc0b6f516c42c4679a90290d2f87448ed8f977e7aa2dbba4aa1ac09248628c43e493ac25b2bc76640e946035200e34c6
   languageName: node
   linkType: hard
 
-"read-pkg@npm:^5.2.0":
-  version: 5.2.0
-  resolution: "read-pkg@npm:5.2.0"
+"read-pkg@npm:^6.0.0":
+  version: 6.0.0
+  resolution: "read-pkg@npm:6.0.0"
   dependencies:
     "@types/normalize-package-data": ^2.4.0
-    normalize-package-data: ^2.5.0
-    parse-json: ^5.0.0
-    type-fest: ^0.6.0
-  checksum: eb696e60528b29aebe10e499ba93f44991908c57d70f2d26f369e46b8b9afc208ef11b4ba64f67630f31df8b6872129e0a8933c8c53b7b4daf0eace536901222
+    normalize-package-data: ^3.0.2
+    parse-json: ^5.2.0
+    type-fest: ^1.0.1
+  checksum: 0cebdff381128e923815c643074a87011070e5fc352bee575d327d6485da3317fab6d802a7b03deeb0be7be8d3ad1640397b3d5d2f044452caf4e8d1736bf94f
   languageName: node
   linkType: hard
 
 "rechoir@npm:^0.8.0":
   version: 0.8.0
   resolution: "rechoir@npm:0.8.0"
   dependencies:
     resolve: ^1.20.0
   checksum: ad3caed8afdefbc33fbc30e6d22b86c35b3d51c2005546f4e79bcc03c074df804b3640ad18945e6bef9ed12caedc035655ec1082f64a5e94c849ff939dc0a788
   languageName: node
   linkType: hard
 
-"redent@npm:^3.0.0":
-  version: 3.0.0
-  resolution: "redent@npm:3.0.0"
+"redent@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "redent@npm:4.0.0"
   dependencies:
-    indent-string: ^4.0.0
-    strip-indent: ^3.0.0
-  checksum: fa1ef20404a2d399235e83cc80bd55a956642e37dd197b4b612ba7327bf87fa32745aeb4a1634b2bab25467164ab4ed9c15be2c307923dd08b0fe7c52431ae6b
+    indent-string: ^5.0.0
+    strip-indent: ^4.0.0
+  checksum: 6944e7b1d8f3fd28c2515f5c605b9f7f0ea0f4edddf41890bbbdd4d9ee35abb7540c3b278f03ff827bd278bb6ff4a5bd8692ca406b748c5c1c3ce7355e9fbf8f
   languageName: node
   linkType: hard
 
 "regexp-match-indices@npm:^1.0.2":
   version: 1.0.2
   resolution: "regexp-match-indices@npm:1.0.2"
   dependencies:
@@ -4866,19 +4913,19 @@
     ajv-formats: ^2.1.1
     ajv-keywords: ^5.1.0
   checksum: 26a0463d47683258106e6652e9aeb0823bf0b85843039e068b57da1892f7ae6b6b1094d48e9ed5ba5cbe9f7166469d880858b9d91abe8bd249421eb813850cde
   languageName: node
   linkType: hard
 
 "semver@npm:2 || 3 || 4 || 5, semver@npm:^5.4.1, semver@npm:^5.5.0":
-  version: 5.7.1
-  resolution: "semver@npm:5.7.1"
+  version: 5.7.2
+  resolution: "semver@npm:5.7.2"
   bin:
-    semver: ./bin/semver
-  checksum: 57fd0acfd0bac382ee87cd52cd0aaa5af086a7dc8d60379dfe65fea491fb2489b6016400813930ecd61fd0952dae75c115287a1b16c234b1550887117744dfaf
+    semver: bin/semver
+  checksum: fb4ab5e0dd1c22ce0c937ea390b4a822147a9c53dbd2a9a0132f12fe382902beef4fbf12cf51bb955248d8d15874ce8cd89532569756384f994309825f10b686
   languageName: node
   linkType: hard
 
 "semver@npm:^7.3.4, semver@npm:^7.3.7, semver@npm:^7.3.8":
   version: 7.5.3
   resolution: "semver@npm:7.5.3"
   dependencies:
@@ -4942,18 +4989,18 @@
 "shell-quote@npm:^1.6.1":
   version: 1.7.3
   resolution: "shell-quote@npm:1.7.3"
   checksum: aca58e73a3a5d933d02e0bdddedc53ee14f7c2ec264f97ac915b9d4482d077a38e422aa664631d60a672cd3cdb4054eb2e6c0303f54882453dacb6483e482d34
   languageName: node
   linkType: hard
 
-"signal-exit@npm:^3.0.7":
-  version: 3.0.7
-  resolution: "signal-exit@npm:3.0.7"
-  checksum: a2f098f247adc367dffc27845853e9959b9e88b01cb301658cfe4194352d8d2bb32e18467c786a7fe15f1d44b233ea35633d076d5e737870b7139949d1ab6318
+"signal-exit@npm:^4.0.1":
+  version: 4.0.2
+  resolution: "signal-exit@npm:4.0.2"
+  checksum: 41f5928431cc6e91087bf0343db786a6313dd7c6fd7e551dbc141c95bb5fb26663444fd9df8ea47c5d7fc202f60aa7468c3162a9365cbb0615fc5e1b1328fe31
   languageName: node
   linkType: hard
 
 "slash@npm:^3.0.0":
   version: 3.0.0
   resolution: "slash@npm:3.0.0"
   checksum: 94a93fff615f25a999ad4b83c9d5e257a7280c90a32a7cb8b4a87996e4babf322e469c42b7f649fd5796edd8687652f3fb452a86dc97a816f01113183393f11c
@@ -4974,15 +5021,15 @@
 "source-list-map@npm:^2.0.0":
   version: 2.0.1
   resolution: "source-list-map@npm:2.0.1"
   checksum: 806efc6f75e7cd31e4815e7a3aaf75a45c704871ea4075cb2eb49882c6fca28998f44fc5ac91adb6de03b2882ee6fb02f951fdc85e6a22b338c32bfe19557938
   languageName: node
   linkType: hard
 
-"source-map-js@npm:^1.0.2":
+"source-map-js@npm:^1.0.1, source-map-js@npm:^1.0.2":
   version: 1.0.2
   resolution: "source-map-js@npm:1.0.2"
   checksum: c049a7fc4deb9a7e9b481ae3d424cc793cb4845daa690bc5a05d428bf41bf231ced49b4cf0c9e77f9d42fdb3d20d6187619fc586605f5eabe995a316da8d377c
   languageName: node
   linkType: hard
 
 "source-map-loader@npm:^1.0.2":
@@ -5121,20 +5168,20 @@
 "strip-bom@npm:^3.0.0":
   version: 3.0.0
   resolution: "strip-bom@npm:3.0.0"
   checksum: 8d50ff27b7ebe5ecc78f1fe1e00fcdff7af014e73cf724b46fb81ef889eeb1015fc5184b64e81a2efe002180f3ba431bdd77e300da5c6685d702780fbf0c8d5b
   languageName: node
   linkType: hard
 
-"strip-indent@npm:^3.0.0":
-  version: 3.0.0
-  resolution: "strip-indent@npm:3.0.0"
+"strip-indent@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "strip-indent@npm:4.0.0"
   dependencies:
-    min-indent: ^1.0.0
-  checksum: 18f045d57d9d0d90cd16f72b2313d6364fd2cb4bf85b9f593523ad431c8720011a4d5f08b6591c9d580f446e78855c5334a30fb91aa1560f5d9f95ed1b4a0530
+    min-indent: ^1.0.1
+  checksum: 06cbcd93da721c46bc13caeb1c00af93a9b18146a1c95927672d2decab6a25ad83662772417cea9317a2507fb143253ecc23c4415b64f5828cef9b638a744598
   languageName: node
   linkType: hard
 
 "strip-json-comments@npm:^3.1.0, strip-json-comments@npm:^3.1.1":
   version: 3.1.1
   resolution: "strip-json-comments@npm:3.1.1"
   checksum: 492f73e27268f9b1c122733f28ecb0e7e8d8a531a6662efbd08e22cccb3f9475e90a1b82cab06a392f6afae6d2de636f977e231296400d0ec5304ba70f166443
@@ -5204,59 +5251,61 @@
   peerDependencies:
     prettier: ">=2.0.0"
     stylelint: ">=14.0.0"
   checksum: 6ce7628517a492e0c2e6104f654c9bc710f1aaf035c8b5274e187b68e8d510e70bae5ded2cb65df76aa01096460b9dfe02f844fea13bfba7e3dcca13baec2ff4
   languageName: node
   linkType: hard
 
-"stylelint@npm:^14.9.1":
-  version: 14.16.1
-  resolution: "stylelint@npm:14.16.1"
-  dependencies:
-    "@csstools/selector-specificity": ^2.0.2
+"stylelint@npm:^15.10.1":
+  version: 15.10.1
+  resolution: "stylelint@npm:15.10.1"
+  dependencies:
+    "@csstools/css-parser-algorithms": ^2.3.0
+    "@csstools/css-tokenizer": ^2.1.1
+    "@csstools/media-query-list-parser": ^2.1.2
+    "@csstools/selector-specificity": ^3.0.0
     balanced-match: ^2.0.0
     colord: ^2.9.3
-    cosmiconfig: ^7.1.0
+    cosmiconfig: ^8.2.0
     css-functions-list: ^3.1.0
+    css-tree: ^2.3.1
     debug: ^4.3.4
-    fast-glob: ^3.2.12
+    fast-glob: ^3.3.0
     fastest-levenshtein: ^1.0.16
     file-entry-cache: ^6.0.1
     global-modules: ^2.0.0
     globby: ^11.1.0
     globjoin: ^0.1.4
-    html-tags: ^3.2.0
-    ignore: ^5.2.1
+    html-tags: ^3.3.1
+    ignore: ^5.2.4
     import-lazy: ^4.0.0
     imurmurhash: ^0.1.4
     is-plain-object: ^5.0.0
-    known-css-properties: ^0.26.0
+    known-css-properties: ^0.27.0
     mathml-tag-names: ^2.1.3
-    meow: ^9.0.0
+    meow: ^10.1.5
     micromatch: ^4.0.5
     normalize-path: ^3.0.0
     picocolors: ^1.0.0
-    postcss: ^8.4.19
-    postcss-media-query-parser: ^0.2.3
+    postcss: ^8.4.24
     postcss-resolve-nested-selector: ^0.1.1
     postcss-safe-parser: ^6.0.0
-    postcss-selector-parser: ^6.0.11
+    postcss-selector-parser: ^6.0.13
     postcss-value-parser: ^4.2.0
     resolve-from: ^5.0.0
     string-width: ^4.2.3
     strip-ansi: ^6.0.1
     style-search: ^0.1.0
-    supports-hyperlinks: ^2.3.0
+    supports-hyperlinks: ^3.0.0
     svg-tags: ^1.0.0
     table: ^6.8.1
-    v8-compile-cache: ^2.3.0
-    write-file-atomic: ^4.0.2
+    write-file-atomic: ^5.0.1
   bin:
-    stylelint: bin/stylelint.js
-  checksum: bc24050415e3c357a76d8ca2799e74ce31f33c9158b4086462512b0191db5d6a161b81ef35b064039c6eacf98a5553e45fca4c5f21eb4d45e7f1d44b2d226e9b
+    stylelint: bin/stylelint.mjs
+  checksum: 8eeae81fe4ed2dfc580d7c401806dbb058c14631abfafd0821db32f1e649aee62e3d39dda3462c6122826df91bd9799409be926e91b55b007622f51e44eb94c1
   languageName: node
   linkType: hard
 
 "supports-color@npm:^5.3.0":
   version: 5.5.0
   resolution: "supports-color@npm:5.5.0"
   dependencies:
@@ -5279,21 +5328,21 @@
   resolution: "supports-color@npm:8.1.1"
   dependencies:
     has-flag: ^4.0.0
   checksum: c052193a7e43c6cdc741eb7f378df605636e01ad434badf7324f17fb60c69a880d8d8fcdcb562cf94c2350e57b937d7425ab5b8326c67c2adc48f7c87c1db406
   languageName: node
   linkType: hard
 
-"supports-hyperlinks@npm:^2.3.0":
-  version: 2.3.0
-  resolution: "supports-hyperlinks@npm:2.3.0"
+"supports-hyperlinks@npm:^3.0.0":
+  version: 3.0.0
+  resolution: "supports-hyperlinks@npm:3.0.0"
   dependencies:
     has-flag: ^4.0.0
     supports-color: ^7.0.0
-  checksum: 9ee0de3c8ce919d453511b2b1588a8205bd429d98af94a01df87411391010fe22ca463f268c84b2ce2abad019dfff8452aa02806eeb5c905a8d7ad5c4f4c52b8
+  checksum: 41021305de5255b10d821bf93c7a781f783e1693d0faec293d7fc7ccf17011b90bde84b0295fa92ba75c6c390351fe84fdd18848cad4bf656e464a958243c3e7
   languageName: node
   linkType: hard
 
 "supports-preserve-symlinks-flag@npm:^1.0.0":
   version: 1.0.0
   resolution: "supports-preserve-symlinks-flag@npm:1.0.0"
   checksum: 53b1e247e68e05db7b3808b99b892bd36fb096e6fba213a06da7fab22045e97597db425c724f2bbd6c99a3c295e1e73f3e4de78592289f38431049e1277ca0ae
@@ -5384,18 +5433,18 @@
   resolution: "tr46@npm:2.1.0"
   dependencies:
     punycode: ^2.1.1
   checksum: ffe6049b9dca3ae329b059aada7f515b0f0064c611b39b51ff6b53897e954650f6f63d9319c6c008d36ead477c7b55e5f64c9dc60588ddc91ff720d64eb710b3
   languageName: node
   linkType: hard
 
-"trim-newlines@npm:^3.0.0":
-  version: 3.0.1
-  resolution: "trim-newlines@npm:3.0.1"
-  checksum: b530f3fadf78e570cf3c761fb74fef655beff6b0f84b29209bac6c9622db75ad1417f4a7b5d54c96605dcd72734ad44526fef9f396807b90839449eb543c6206
+"trim-newlines@npm:^4.0.2":
+  version: 4.1.1
+  resolution: "trim-newlines@npm:4.1.1"
+  checksum: 5b09f8e329e8f33c1111ef26906332ba7ba7248cde3e26fc054bb3d69f2858bf5feedca9559c572ff91f33e52977c28e0d41c387df6a02a633cbb8c2d8238627
   languageName: node
   linkType: hard
 
 "tslib@npm:^1.8.1":
   version: 1.14.1
   resolution: "tslib@npm:1.14.1"
   checksum: dbe628ef87f66691d5d2959b3e41b9ca0045c3ee3c7c7b906cc1e328b39f199bb1ad9e671c39025bd56122ac57dfbf7385a94843b1cc07c60a4db74795829acd
@@ -5418,39 +5467,25 @@
   resolution: "type-check@npm:0.4.0"
   dependencies:
     prelude-ls: ^1.2.1
   checksum: ec688ebfc9c45d0c30412e41ca9c0cdbd704580eb3a9ccf07b9b576094d7b86a012baebc95681999dd38f4f444afd28504cb3a89f2ef16b31d4ab61a0739025a
   languageName: node
   linkType: hard
 
-"type-fest@npm:^0.18.0":
-  version: 0.18.1
-  resolution: "type-fest@npm:0.18.1"
-  checksum: e96dcee18abe50ec82dab6cbc4751b3a82046da54c52e3b2d035b3c519732c0b3dd7a2fa9df24efd1a38d953d8d4813c50985f215f1957ee5e4f26b0fe0da395
-  languageName: node
-  linkType: hard
-
 "type-fest@npm:^0.20.2":
   version: 0.20.2
   resolution: "type-fest@npm:0.20.2"
   checksum: 4fb3272df21ad1c552486f8a2f8e115c09a521ad7a8db3d56d53718d0c907b62c6e9141ba5f584af3f6830d0872c521357e512381f24f7c44acae583ad517d73
   languageName: node
   linkType: hard
 
-"type-fest@npm:^0.6.0":
-  version: 0.6.0
-  resolution: "type-fest@npm:0.6.0"
-  checksum: b2188e6e4b21557f6e92960ec496d28a51d68658018cba8b597bd3ef757721d1db309f120ae987abeeda874511d14b776157ff809f23c6d1ce8f83b9b2b7d60f
-  languageName: node
-  linkType: hard
-
-"type-fest@npm:^0.8.1":
-  version: 0.8.1
-  resolution: "type-fest@npm:0.8.1"
-  checksum: d61c4b2eba24009033ae4500d7d818a94fd6d1b481a8111612ee141400d5f1db46f199c014766b9fa9b31a6a7374d96fc748c6d688a78a3ce5a33123839becb7
+"type-fest@npm:^1.0.1, type-fest@npm:^1.2.1, type-fest@npm:^1.2.2":
+  version: 1.4.0
+  resolution: "type-fest@npm:1.4.0"
+  checksum: b011c3388665b097ae6a109a437a04d6f61d81b7357f74cbcb02246f2f5bd72b888ae33631b99871388122ba0a87f4ff1c94078e7119ff22c70e52c0ff828201
   languageName: node
   linkType: hard
 
 "typescript@npm:~5.0.2":
   version: 5.0.4
   resolution: "typescript@npm:5.0.4"
   bin:
@@ -5528,21 +5563,14 @@
 "util-deprecate@npm:^1.0.2":
   version: 1.0.2
   resolution: "util-deprecate@npm:1.0.2"
   checksum: 474acf1146cb2701fe3b074892217553dfcf9a031280919ba1b8d651a068c9b15d863b7303cb15bd00a862b498e6cf4ad7b4a08fb134edd5a6f7641681cb54a2
   languageName: node
   linkType: hard
 
-"v8-compile-cache@npm:^2.3.0":
-  version: 2.3.0
-  resolution: "v8-compile-cache@npm:2.3.0"
-  checksum: adb0a271eaa2297f2f4c536acbfee872d0dd26ec2d76f66921aa7fc437319132773483344207bdbeee169225f4739016d8d2dbf0553913a52bb34da6d0334f8e
-  languageName: node
-  linkType: hard
-
 "validate-npm-package-license@npm:^3.0.1":
   version: 3.0.4
   resolution: "validate-npm-package-license@npm:3.0.4"
   dependencies:
     spdx-correct: ^3.0.0
     spdx-expression-parse: ^3.0.0
   checksum: 35703ac889d419cf2aceef63daeadbe4e77227c39ab6287eeb6c1b36a746b364f50ba22e88591f5d017bc54685d8137bc2d328d0a896e4d3fd22093c0f32a9ad
@@ -5834,21 +5862,21 @@
 "wrappy@npm:1":
   version: 1.0.2
   resolution: "wrappy@npm:1.0.2"
   checksum: 159da4805f7e84a3d003d8841557196034155008f817172d4e986bd591f74aa82aa7db55929a54222309e01079a65a92a9e6414da5a6aa4b01ee44a511ac3ee5
   languageName: node
   linkType: hard
 
-"write-file-atomic@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "write-file-atomic@npm:4.0.2"
+"write-file-atomic@npm:^5.0.1":
+  version: 5.0.1
+  resolution: "write-file-atomic@npm:5.0.1"
   dependencies:
     imurmurhash: ^0.1.4
-    signal-exit: ^3.0.7
-  checksum: 5da60bd4eeeb935eec97ead3df6e28e5917a6bd317478e4a85a5285e8480b8ed96032bbcc6ecd07b236142a24f3ca871c924ec4a6575e623ec1b11bf8c1c253c
+    signal-exit: ^4.0.1
+  checksum: 8dbb0e2512c2f72ccc20ccedab9986c7d02d04039ed6e8780c987dc4940b793339c50172a1008eed7747001bfacc0ca47562668a069a7506c46c77d7ba3926a9
   languageName: node
   linkType: hard
 
 "ws@npm:^8.11.0":
   version: 8.13.0
   resolution: "ws@npm:8.13.0"
   peerDependencies:
@@ -5875,22 +5903,15 @@
 "yallist@npm:^4.0.0":
   version: 4.0.0
   resolution: "yallist@npm:4.0.0"
   checksum: 343617202af32df2a15a3be36a5a8c0c8545208f3d3dfbc6bb7c3e3b7e8c6f8e7485432e4f3b88da3031a6e20afa7c711eded32ddfb122896ac5d914e75848d5
   languageName: node
   linkType: hard
 
-"yaml@npm:^1.10.0":
-  version: 1.10.2
-  resolution: "yaml@npm:1.10.2"
-  checksum: ce4ada136e8a78a0b08dc10b4b900936912d15de59905b2bf415b4d33c63df1d555d23acb2a41b23cf9fb5da41c256441afca3d6509de7247daa062fd2c5ea5f
-  languageName: node
-  linkType: hard
-
-"yargs-parser@npm:^20.2.3":
+"yargs-parser@npm:^20.2.9":
   version: 20.2.9
   resolution: "yargs-parser@npm:20.2.9"
   checksum: 8bb69015f2b0ff9e17b2c8e6bfe224ab463dd00ca211eece72a4cd8a906224d2703fb8a326d36fdd0e68701e201b2a60ed7cf81ce0fd9b3799f9fe7745977ae3
   languageName: node
   linkType: hard
 
 "yjs@npm:^13.5.40":
```

### Comparing `jupyterlab_spellchecker-0.8.3/dictionaries/README_de_ALL_frami.txt` & `jupyterlab_spellchecker-0.8.4/dictionaries/README_de_ALL_frami.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/dictionaries/README_en_AU.txt` & `jupyterlab_spellchecker-0.8.4/dictionaries/README_en_AU.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/dictionaries/README_en_CA.txt` & `jupyterlab_spellchecker-0.8.4/dictionaries/README_en_CA.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/dictionaries/README_en_GB-ise.txt` & `jupyterlab_spellchecker-0.8.4/dictionaries/README_en_GB-ise.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/dictionaries/README_en_US.txt` & `jupyterlab_spellchecker-0.8.4/dictionaries/README_en_US.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/dictionaries/README_es_ES.txt` & `jupyterlab_spellchecker-0.8.4/dictionaries/README_es_ES.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/dictionaries/README_fr.txt` & `jupyterlab_spellchecker-0.8.4/dictionaries/README_fr.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/dictionaries/README_pt_PT.txt` & `jupyterlab_spellchecker-0.8.4/dictionaries/README_pt_PT.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/dictionaries/de_AT_frami.aff` & `jupyterlab_spellchecker-0.8.4/dictionaries/de_AT_frami.aff`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/dictionaries/de_AT_frami.dic` & `jupyterlab_spellchecker-0.8.4/dictionaries/de_AT_frami.dic`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/dictionaries/de_CH_frami.aff` & `jupyterlab_spellchecker-0.8.4/dictionaries/de_CH_frami.aff`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/dictionaries/de_CH_frami.dic` & `jupyterlab_spellchecker-0.8.4/dictionaries/de_CH_frami.dic`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/dictionaries/de_DE_frami.aff` & `jupyterlab_spellchecker-0.8.4/dictionaries/de_DE_frami.aff`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/dictionaries/de_DE_frami.dic` & `jupyterlab_spellchecker-0.8.4/dictionaries/de_DE_frami.dic`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/dictionaries/en_AU.aff` & `jupyterlab_spellchecker-0.8.4/dictionaries/en_AU.aff`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/dictionaries/en_AU.dic` & `jupyterlab_spellchecker-0.8.4/dictionaries/en_AU.dic`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/dictionaries/en_CA.aff` & `jupyterlab_spellchecker-0.8.4/dictionaries/en_CA.aff`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/dictionaries/en_CA.dic` & `jupyterlab_spellchecker-0.8.4/dictionaries/en_CA.dic`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/dictionaries/en_GB-ise.aff` & `jupyterlab_spellchecker-0.8.4/dictionaries/en_GB-ise.aff`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/dictionaries/en_GB-ise.dic` & `jupyterlab_spellchecker-0.8.4/dictionaries/en_GB-ise.dic`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/dictionaries/en_US.aff` & `jupyterlab_spellchecker-0.8.4/dictionaries/en_US.aff`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/dictionaries/en_US.dic` & `jupyterlab_spellchecker-0.8.4/dictionaries/en_US.dic`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/dictionaries/es_ES.aff` & `jupyterlab_spellchecker-0.8.4/dictionaries/es_ES.aff`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/dictionaries/es_ES.dic` & `jupyterlab_spellchecker-0.8.4/dictionaries/es_ES.dic`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/dictionaries/fr.aff` & `jupyterlab_spellchecker-0.8.4/dictionaries/fr.aff`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/dictionaries/fr.dic` & `jupyterlab_spellchecker-0.8.4/dictionaries/fr.dic`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/dictionaries/pt_PT.aff` & `jupyterlab_spellchecker-0.8.4/dictionaries/pt_PT.aff`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/dictionaries/pt_PT.dic` & `jupyterlab_spellchecker-0.8.4/dictionaries/pt_PT.dic`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/jupyterlab_spellchecker/__init__.py` & `jupyterlab_spellchecker-0.8.4/jupyterlab_spellchecker/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/jupyterlab_spellchecker/dictionaries.py` & `jupyterlab_spellchecker-0.8.4/jupyterlab_spellchecker/dictionaries.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/jupyterlab_spellchecker/handlers.py` & `jupyterlab_spellchecker-0.8.4/jupyterlab_spellchecker/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/jupyterlab_spellchecker/labextension/package.json` & `jupyterlab_spellchecker-0.8.4/jupyterlab_spellchecker/labextension/schemas/@jupyterlab-contrib/spellchecker/package.json.orig`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9660879629629631%*

 * *Differences: {"'devDependencies'": "{'stylelint': '^15.10.1'}",*

 * * "'jupyterlab'": "{delete: ['_build']}",*

 * * "'version'": "'0.8.4'"}*

```diff
@@ -47,15 +47,15 @@
         "eslint-plugin-prettier": "^4.2.1",
         "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.8.7",
         "rimraf": "^4.4.1",
         "source-map-loader": "^1.0.2",
         "style-loader": "^3.3.1",
-        "stylelint": "^14.9.1",
+        "stylelint": "^15.10.1",
         "stylelint-config-prettier": "^9.0.4",
         "stylelint-config-recommended": "^8.0.0",
         "stylelint-config-standard": "^26.0.0",
         "stylelint-prettier": "^2.0.0",
         "typescript": "~5.0.2",
         "yjs": "^13.5.40"
     },
@@ -64,19 +64,14 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "schema/**/*.{json,}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "style/index.js"
     ],
     "homepage": "https://github.com/jupyterlab-contrib/spellchecker",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.fe331f8109a0c7b472be.js",
-            "style": "./style"
-        },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab-spellchecker"
                 },
                 "managers": [
                     "pip",
@@ -125,9 +120,9 @@
         "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w --sourceMap"
     },
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.8.3"
+    "version": "0.8.4"
 }
```

### Comparing `jupyterlab_spellchecker-0.8.3/jupyterlab_spellchecker/labextension/schemas/@jupyterlab-contrib/spellchecker/package.json.orig` & `jupyterlab_spellchecker-0.8.4/jupyterlab_spellchecker/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9660879629629631%*

 * *Differences: {"'devDependencies'": "{'stylelint': '^15.10.1'}",*

 * * "'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.afbfa74351e195593c24.js'), "*

 * *                 "('extension', './extension'), ('style', './style')])}",*

 * * "'version'": "'0.8.4'"}*

```diff
@@ -47,15 +47,15 @@
         "eslint-plugin-prettier": "^4.2.1",
         "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.8.7",
         "rimraf": "^4.4.1",
         "source-map-loader": "^1.0.2",
         "style-loader": "^3.3.1",
-        "stylelint": "^14.9.1",
+        "stylelint": "^15.10.1",
         "stylelint-config-prettier": "^9.0.4",
         "stylelint-config-recommended": "^8.0.0",
         "stylelint-config-standard": "^26.0.0",
         "stylelint-prettier": "^2.0.0",
         "typescript": "~5.0.2",
         "yjs": "^13.5.40"
     },
@@ -64,14 +64,19 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "schema/**/*.{json,}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "style/index.js"
     ],
     "homepage": "https://github.com/jupyterlab-contrib/spellchecker",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.afbfa74351e195593c24.js",
+            "style": "./style"
+        },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab-spellchecker"
                 },
                 "managers": [
                     "pip",
@@ -120,9 +125,9 @@
         "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w --sourceMap"
     },
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.8.3"
+    "version": "0.8.4"
 }
```

### Comparing `jupyterlab_spellchecker-0.8.3/jupyterlab_spellchecker/labextension/schemas/@jupyterlab-contrib/spellchecker/plugin.json` & `jupyterlab_spellchecker-0.8.4/jupyterlab_spellchecker/labextension/schemas/@jupyterlab-contrib/spellchecker/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/jupyterlab_spellchecker/labextension/static/552.d2bec066859ae2b0c6d2.js` & `jupyterlab_spellchecker-0.8.4/jupyterlab_spellchecker/labextension/static/552.6d7597412aeadbbf15fe.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -3,36 +3,36 @@
     [552], {
         552: (e, t, s) => {
             s.r(t), s.d(t, {
                 default: () => G,
                 spellcheckIcon: () => A
             });
             var n = s(373),
-                i = s(189),
-                a = s(350),
+                i = s(580),
+                a = s(172),
                 o = s(778),
-                l = s(56),
-                r = s(834),
-                c = s(927),
-                h = s(926),
-                g = s(993),
-                d = s(238),
+                l = s(663),
+                r = s(760),
+                c = s(408),
+                h = s(354),
+                g = s(987),
+                d = s(790),
                 u = s(379),
                 p = s.n(u),
                 m = s(795),
                 _ = s.n(m),
                 y = s(569),
                 f = s.n(y),
                 k = s(565),
                 b = s.n(k),
                 w = s(216),
                 x = s.n(w),
                 T = s(589),
                 v = s.n(T),
-                E = s(760),
+                E = s(660),
                 S = {};
             S.styleTagTransform = v(), S.setAttributes = b(), S.insert = f().bind(null, "head"), S.domAPI = _(), S.insertStyleElement = x(), p()(E.Z, S), E.Z && E.Z.locals && E.Z.locals;
             var C = s(446),
                 I = s(211),
                 L = s(204),
                 R = s(851);
             const A = new i.LabIcon({
@@ -367,15 +367,15 @@
                         console.debug("Attempting to load spellchecker");
                         const l = new M(e, t, s, n || h.nullTranslator, i, a, o);
                         console.debug("Spellchecker loaded ", l)
                     }
                 },
                 G = O
         },
-        760: (e, t, s) => {
+        660: (e, t, s) => {
             s.d(t, {
                 Z: () => l
             });
             var n = s(81),
                 i = s.n(n),
                 a = s(645),
                 o = s.n(a)()(i());
```

### Comparing `jupyterlab_spellchecker-0.8.3/jupyterlab_spellchecker/labextension/static/581.7b781918df8ce52c9a8f.js` & `jupyterlab_spellchecker-0.8.4/jupyterlab_spellchecker/labextension/static/581.7b781918df8ce52c9a8f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/jupyterlab_spellchecker/labextension/static/747.2f89d796d954e37784cd.js` & `jupyterlab_spellchecker-0.8.4/jupyterlab_spellchecker/labextension/static/747.2f89d796d954e37784cd.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/jupyterlab_spellchecker/labextension/static/995.266a0ca9063d6df0c41f.js` & `jupyterlab_spellchecker-0.8.4/jupyterlab_spellchecker/labextension/static/995.266a0ca9063d6df0c41f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/jupyterlab_spellchecker/labextension/static/remoteEntry.fe331f8109a0c7b472be.js` & `jupyterlab_spellchecker-0.8.4/jupyterlab_spellchecker/labextension/static/remoteEntry.afbfa74351e195593c24.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, l, u, f, s, c, d, p, h, v, b, m, y, g = {
+    var e, r, t, n, o, a, i, l, u, f, s, d, c, p, h, b, v, m, y, g = {
             34: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(995), t.e(552)]).then((() => () => t(552))),
                         "./extension": () => Promise.all([t.e(995), t.e(552)]).then((() => () => t(552))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -43,20 +43,20 @@
         }), r
     }, w.d = (e, r) => {
         for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
-        552: "d2bec066859ae2b0c6d2",
+        552: "6d7597412aeadbbf15fe",
         581: "7b781918df8ce52c9a8f",
         747: "2f89d796d954e37784cd",
         995: "266a0ca9063d6df0c41f"
     } [e] + ".js?v=" + {
-        552: "d2bec066859ae2b0c6d2",
+        552: "6d7597412aeadbbf15fe",
         581: "7b781918df8ce52c9a8f",
         747: "2f89d796d954e37784cd",
         995: "266a0ca9063d6df0c41f"
     } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
@@ -72,24 +72,24 @@
                     var s = u[f];
                     if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
                         i = s;
                         break
                     }
                 }
             i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, w.nc && i.setAttribute("nonce", w.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
-            var c = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(d);
+            var d = (r, n) => {
+                    i.onerror = i.onload = null, clearTimeout(c);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                d = setTimeout(c.bind(null, void 0, {
+                c = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = c.bind(null, i.onerror), i.onload = c.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, w.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -111,15 +111,15 @@
                         (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     u = [];
-                return "default" === t && (l("@jupyterlab-contrib/spellchecker", "0.8.3", (() => Promise.all([w.e(995), w.e(552)]).then((() => () => w(552))))), l("typo-js", "1.2.0", (() => w.e(581).then((() => () => w(581)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@jupyterlab-contrib/spellchecker", "0.8.4", (() => Promise.all([w.e(995), w.e(552)]).then((() => () => w(552))))), l("typo-js", "1.2.0", (() => w.e(581).then((() => () => w(581)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -169,96 +169,96 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var f, s, c = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !u || ("u" == c ? l > n && !o : "" == c != o);
+                var f, s, d = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !u || ("u" == d ? l > n && !o : "" == d != o);
                 if ("u" == s) {
-                    if (!u || "u" != c) return !1
+                    if (!u || "u" != d) return !1
                 } else if (u)
-                    if (c == s)
+                    if (d == s)
                         if (l <= n) {
                             if (f != e[l]) return !1
                         } else {
                             if (o ? f > e[l] : f < e[l]) return !1;
                             f != e[l] && (u = !1)
                         }
-                else if ("s" != c && "n" != c) {
+                else if ("s" != d && "n" != d) {
                     if (o || l <= n) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= n || s < c != o) return !1;
+                    if (l <= n || s < d != o) return !1;
                     u = !1
-                } else "s" != c && "n" != c && (u = !1, l--)
+                } else "s" != d && "n" != d && (u = !1, l--)
             }
         }
-        var d = [],
-            p = d.pop.bind(d);
+        var c = [],
+            p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            d.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
         }
         return !!p()
     }, i = (e, r) => {
         var t = w.S[e];
         if (!t || !w.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
         var o = l(e, t);
-        return a(n, o) || c(u(e, t, o, n)), d(e[t][o])
+        return a(n, o) || d(u(e, t, o, n)), c(e[t][o])
     }, s = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
-    }, c = e => {
+    }, d = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, d = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, o) {
+    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, o) {
         var a = w.I(r);
         return a && a.then ? a.then(e.bind(e, r, w.S[r], t, n, o)) : e(r, w.S[r], t, n, o)
-    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), v = p(((e, r, t, n, o) => {
+    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), b = p(((e, r, t, n, o) => {
         var a = r && w.o(r, t) && s(r, t, n);
-        return a ? d(a) : o()
-    })), b = {}, m = {
-        56: () => h("default", "@jupyterlab/settingregistry", [1, 4, 0, 2]),
-        189: () => h("default", "@jupyterlab/ui-components", [1, 4, 0, 2]),
+        return a ? c(a) : o()
+    })), v = {}, m = {
+        172: () => h("default", "@jupyterlab/apputils", [1, 4, 1, 3]),
         204: () => h("default", "@codemirror/state", [1, 6, 2, 0]),
         211: () => h("default", "@codemirror/view", [1, 6, 9, 6]),
-        238: () => h("default", "@jupyterlab/services", [1, 7, 0, 2]),
-        350: () => h("default", "@jupyterlab/apputils", [1, 4, 1, 2]),
+        354: () => h("default", "@jupyterlab/translation", [1, 4, 0, 3]),
         373: () => h("default", "@codemirror/language", [1, 6, 0, 0]),
-        397: () => v("default", "typo-js", [1, 1, 1, 0], (() => w.e(581).then((() => () => w(581))))),
+        397: () => b("default", "typo-js", [1, 1, 1, 0], (() => w.e(581).then((() => () => w(581))))),
+        408: () => h("default", "@jupyterlab/codemirror", [1, 4, 0, 3]),
+        580: () => h("default", "@jupyterlab/ui-components", [1, 4, 0, 3]),
+        663: () => h("default", "@jupyterlab/settingregistry", [1, 4, 0, 3]),
+        760: () => h("default", "@jupyterlab/statusbar", [1, 4, 0, 3]),
         778: () => h("default", "@lumino/widgets", [1, 2, 0, 1]),
-        834: () => h("default", "@jupyterlab/statusbar", [1, 4, 0, 2]),
+        790: () => h("default", "@jupyterlab/services", [1, 7, 0, 3]),
         851: () => h("default", "@lezer/common", [1, 1, 0, 0]),
-        926: () => h("default", "@jupyterlab/translation", [1, 4, 0, 2]),
-        927: () => h("default", "@jupyterlab/codemirror", [1, 4, 0, 2]),
-        993: () => h("default", "@jupyterlab/coreutils", [1, 6, 0, 2])
+        987: () => h("default", "@jupyterlab/coreutils", [1, 6, 0, 3])
     }, y = {
-        552: [56, 189, 204, 211, 238, 350, 373, 397, 778, 834, 851, 926, 927, 993]
+        552: [172, 204, 211, 354, 373, 397, 408, 580, 663, 760, 778, 790, 851, 987]
     }, w.f.consumes = (e, r) => {
         w.o(y, e) && y[e].forEach((e => {
-            if (w.o(b, e)) return r.push(b[e]);
+            if (w.o(v, e)) return r.push(v[e]);
             var t = r => {
-                    b[e] = 0, w.m[e] = t => {
+                    v[e] = 0, w.m[e] = t => {
                         delete w.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete b[e], w.m[e] = t => {
+                    delete v[e], w.m[e] = t => {
                         throw delete w.c[e], r
                     }
                 };
             try {
                 var o = m[e]();
-                o.then ? r.push(b[e] = o.then(t).catch(n)) : t(o)
+                o.then ? r.push(v[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             551: 0
```

### Comparing `jupyterlab_spellchecker-0.8.3/jupyterlab_spellchecker/labextension/static/third-party-licenses.json` & `jupyterlab_spellchecker-0.8.4/jupyterlab_spellchecker/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/jupyterlab_spellchecker/tests/test_dictionaries.py` & `jupyterlab_spellchecker-0.8.4/jupyterlab_spellchecker/tests/test_dictionaries.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/schema/plugin.json` & `jupyterlab_spellchecker-0.8.4/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/src/handler.ts` & `jupyterlab_spellchecker-0.8.4/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/src/index.ts` & `jupyterlab_spellchecker-0.8.4/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/style/index.css` & `jupyterlab_spellchecker-0.8.4/style/index.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/style/icons/LICENSE` & `jupyterlab_spellchecker-0.8.4/style/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/.gitignore` & `jupyterlab_spellchecker-0.8.4/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/LICENSE` & `jupyterlab_spellchecker-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/README.md` & `jupyterlab_spellchecker-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.3/pyproject.toml` & `jupyterlab_spellchecker-0.8.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,16 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "jupyter_server>=2.0.1,<3"
+    "jupyter_server>=2.0.1,<3",
+    "jupyterlab>=4,<5"
 ]
 dynamic = ["version", "description", "authors", "keywords"]
 
 [project.urls]
 Source = "https://github.com/jupyterlab-contrib/spellchecker"
 Issues = "https://github.com/jupyterlab-contrib/spellchecker/issues"
```

### Comparing `jupyterlab_spellchecker-0.8.3/PKG-INFO` & `jupyterlab_spellchecker-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-spellchecker
-Version: 0.8.3
+Version: 0.8.4
 Summary: A spell checker for JupyterLab.
 Project-URL: Source, https://github.com/jupyterlab-contrib/spellchecker
 Project-URL: Issues, https://github.com/jupyterlab-contrib/spellchecker/issues
 Author: JupyterLab Spellchecker Development Team
 License: BSD 3-Clause License
         
         Copyright (c) 2020, ijmbarr All rights reserved.
@@ -44,14 +44,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Requires-Dist: jupyter-server<3,>=2.0.1
+Requires-Dist: jupyterlab<5,>=4
 Description-Content-Type: text/markdown
 
 # jupyterlab-spellchecker
 
 [![Extension status](https://img.shields.io/badge/status-ready-success 'ready to be used')](https://jupyterlab-contrib.github.io/)
 [![Github Actions Status](https://github.com/jupyterlab-contrib/spellchecker/workflows/Build/badge.svg)](https://github.com/jupyterlab-contrib/spellchecker/actions)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyterlab-contrib/spellchecker/master?urlpath=lab)
```

