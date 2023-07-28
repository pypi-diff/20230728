# Comparing `tmp/cookies_utilities-0.0.1.tar.gz` & `tmp/cookies_utilities-0.0.2.tar.gz`

## Comparing `cookies_utilities-0.0.1.tar` & `cookies_utilities-0.0.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/.readthedocs.yaml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/Makefile
--rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/make.bat
--rw-r--r--   0        0        0    21405 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/doctrees/cookies_utilities.doctree
--rw-r--r--   0        0        0    53778 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/doctrees/environment.pickle
--rw-r--r--   0        0        0     5093 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/doctrees/index.doctree
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/doctrees/modules.doctree
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/.buildinfo
--rw-r--r--   0        0        0    13211 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/cookies_utilities.html
--rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/genindex.html
--rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/index.html
--rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/modules.html
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/objects.inv
--rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/search.html
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/searchindex.js
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_sources/cookies_utilities.rst.txt
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_sources/index.rst.txt
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_sources/modules.rst.txt
--rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0        0        0    15715 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/basic.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/doctools.js
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/file.png
--rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/jquery.js
--rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/plus.png
--rw-r--r--   0        0        0     4892 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/pygments.css
--rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/searchtools.js
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/css/badge_only.css
--rw-r--r--   0        0        0   135314 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/css/theme.css
--rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/js/badge_only.js
--rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/js/html5shiv.min.js
--rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/build/html/_static/js/theme.js
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/source/conf.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/source/cookies_utilities.rst
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/source/index.rst
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/docs/source/modules.rst
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/src/cookies_utilities/__init__.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/src/cookies_utilities/stopwatch.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/tests/test_cookies_utilities.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/tests/test_stopwatch.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/LICENSE
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/README.md
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 cookies_utilities-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/.readthedocs.yaml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/Makefile
+-rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/make.bat
+-rw-r--r--   0        0        0    25667 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/doctrees/cookies_utilities.doctree
+-rw-r--r--   0        0        0    59389 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/doctrees/environment.pickle
+-rw-r--r--   0        0        0     5322 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/doctrees/index.doctree
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/doctrees/modules.doctree
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/.buildinfo
+-rw-r--r--   0        0        0    17149 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/cookies_utilities.html
+-rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/genindex.html
+-rw-r--r--   0        0        0     5460 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/index.html
+-rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/modules.html
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/objects.inv
+-rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/search.html
+-rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/searchindex.js
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_sources/cookies_utilities.rst.txt
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_sources/modules.rst.txt
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0        0        0    15715 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/basic.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/doctools.js
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/file.png
+-rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/jquery.js
+-rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/plus.png
+-rw-r--r--   0        0        0     4892 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/pygments.css
+-rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/badge_only.css
+-rw-r--r--   0        0        0   135314 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/theme.css
+-rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/js/badge_only.js
+-rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/js/theme.js
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/source/conf.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/source/cookies_utilities.rst
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/source/index.rst
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/source/modules.rst
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/src/cookies_utilities/__init__.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/src/cookies_utilities/stopwatch.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/tests/test_cookies_utilities.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/tests/test_stopwatch.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/README.md
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/PKG-INFO
```

### Comparing `cookies_utilities-0.0.1/docs/Makefile` & `cookies_utilities-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/make.bat` & `cookies_utilities-0.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/doctrees/cookies_utilities.doctree` & `cookies_utilities-0.0.2/docs/build/doctrees/cookies_utilities.doctree`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8005 9592 5300 0000 0000 008c 0f73 7068  ....S........sph
+00000000: 8005 9538 6400 0000 0000 008c 0f73 7068  ...8d........sph
 00000010: 696e 782e 6164 646e 6f64 6573 948c 0864  inx.addnodes...d
 00000020: 6f63 756d 656e 7494 9394 2981 947d 9428  ocument...)..}.(
 00000030: 8c09 7261 7773 6f75 7263 6594 8c00 948c  ..rawsource.....
 00000040: 0863 6869 6c64 7265 6e94 5d94 8c0e 646f  .children.]...do
 00000050: 6375 7469 6c73 2e6e 6f64 6573 948c 0773  cutils.nodes...s
 00000060: 6563 7469 6f6e 9493 9429 8194 7d94 2868  ection...)..}.(h
 00000070: 0568 0668 075d 9428 6809 8c05 7469 746c  .h.h.].(h...titl
@@ -52,1287 +52,1554 @@
 00000330: 7574 696c 6974 6965 7329 948c 1b63 6f6f  utilities)...coo
 00000340: 6b69 6573 5f75 7469 6c69 7469 6573 2e67  kies_utilities.g
 00000350: 6574 5f64 6174 6573 9468 064e 7494 6175  et_dates.h.Nt.au
 00000360: 682b 684f 681b 683e 681c 6803 681d 4e68  h+hOh.h>h.h.h.Nh
 00000370: 1e4e 7562 6800 8c04 6465 7363 9493 9429  .Nubh...desc...)
 00000380: 8194 7d94 2868 0568 0668 075d 9428 6800  ..}.(h.h.h.].(h.
 00000390: 8c0e 6465 7363 5f73 6967 6e61 7475 7265  ..desc_signature
-000003a0: 9493 9429 8194 7d94 2868 058c b667 6574  ...)..}.(h...get
+000003a0: 9493 9429 8194 7d94 2868 058c c567 6574  ...)..}.(h...get
 000003b0: 5f64 6174 6573 2873 7461 7274 3d27 3230  _dates(start='20
 000003c0: 3136 2d30 372d 3031 2030 323a 3030 3a30  16-07-01 02:00:0
 000003d0: 3027 2c20 656e 643d 2732 3031 362d 3037  0', end='2016-07
 000003e0: 2d30 3220 3031 3a30 303a 3030 272c 2066  -02 01:00:00', f
 000003f0: 6f72 6d61 743d 2725 592d 256d 2d25 6420  ormat='%Y-%m-%d 
 00000400: 2548 3a25 4d3a 2553 272c 2064 656c 7461  %H:%M:%S', delta
 00000410: 3d7b 2764 6179 7327 3a20 302c 2027 686f  ={'days': 0, 'ho
 00000420: 7572 7327 3a20 312c 2027 6d69 6e75 7465  urs': 1, 'minute
 00000430: 7327 3a20 302c 2027 7765 656b 7327 3a20  s': 0, 'weeks': 
-00000440: 307d 2c20 6361 7374 5f73 7472 3d54 7275  0}, cast_str=Tru
-00000450: 652c 2066 6f72 6d61 745f 6f75 743d 4e6f  e, format_out=No
-00000460: 6e65 2994 6807 5d94 2868 008c 0c64 6573  ne).h.].(h...des
-00000470: 635f 6164 646e 616d 6594 9394 2981 947d  c_addname...)..}
-00000480: 9428 6805 8c12 636f 6f6b 6965 735f 7574  .(h...cookies_ut
-00000490: 696c 6974 6965 732e 9468 075d 9468 168c  ilities..h.].h..
-000004a0: 1263 6f6f 6b69 6573 5f75 7469 6c69 7469  .cookies_utiliti
-000004b0: 6573 2e94 8594 8194 7d94 2868 1b68 6d68  es......}.(h.hmh
-000004c0: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
-000004d0: 2868 215d 9468 235d 9428 8c0b 7369 672d  (h!].h#].(..sig-
-000004e0: 7072 656e 616d 6594 8c0d 6465 7363 636c  prename...desccl
-000004f0: 6173 736e 616d 6594 6568 255d 9468 275d  assname.eh%].h']
-00000500: 9468 295d 948c 0978 6d6c 3a73 7061 6365  .h)]...xml:space
-00000510: 948c 0870 7265 7365 7276 6594 7568 2b68  ...preserve.uh+h
-00000520: 6b68 1b68 6768 1c68 0368 1d8c 7143 3a5c  kh.hgh.h.h..qC:\
-00000530: 5573 6572 735c 632d 6d69 685c 7370 6163  Users\c-mih\spac
-00000540: 655c 636f 6f6b 6965 735f 7574 696c 6974  e\cookies_utilit
-00000550: 6965 735c 7372 635c 636f 6f6b 6965 735f  ies\src\cookies_
-00000560: 7574 696c 6974 6965 735c 5f5f 696e 6974  utilities\__init
-00000570: 5f5f 2e70 793a 646f 6373 7472 696e 6720  __.py:docstring 
-00000580: 6f66 2063 6f6f 6b69 6573 5f75 7469 6c69  of cookies_utili
-00000590: 7469 6573 2e67 6574 5f64 6174 6573 9468  ties.get_dates.h
-000005a0: 1e4b 0175 6268 008c 0964 6573 635f 6e61  .K.ubh...desc_na
-000005b0: 6d65 9493 9429 8194 7d94 2868 058c 0967  me...)..}.(h...g
-000005c0: 6574 5f64 6174 6573 9468 075d 9468 168c  et_dates.h.].h..
-000005d0: 0967 6574 5f64 6174 6573 9485 9481 947d  .get_dates.....}
-000005e0: 9428 681b 6882 681c 6803 681d 4e68 1e4e  .(h.h.h.h.h.Nh.N
-000005f0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-00000600: 288c 0873 6967 2d6e 616d 6594 8c08 6465  (..sig-name...de
-00000610: 7363 6e61 6d65 9465 6825 5d94 6827 5d94  scname.eh%].h'].
-00000620: 6829 5d94 687d 687e 7568 2b68 8068 1b68  h)].h}h~uh+h.h.h
-00000630: 6768 1c68 0368 1d68 7f68 1e4b 0175 6268  gh.h.h.h.h.K.ubh
-00000640: 008c 1264 6573 635f 7061 7261 6d65 7465  ...desc_paramete
-00000650: 726c 6973 7494 9394 2981 947d 9428 6805  rlist...)..}.(h.
-00000660: 8cab 7374 6172 743d 2732 3031 362d 3037  ..start='2016-07
-00000670: 2d30 3120 3032 3a30 303a 3030 272c 2065  -01 02:00:00', e
-00000680: 6e64 3d27 3230 3136 2d30 372d 3032 2030  nd='2016-07-02 0
-00000690: 313a 3030 3a30 3027 2c20 666f 726d 6174  1:00:00', format
-000006a0: 3d27 2559 2d25 6d2d 2564 2025 483a 254d  ='%Y-%m-%d %H:%M
-000006b0: 3a25 5327 2c20 6465 6c74 613d 7b27 6461  :%S', delta={'da
-000006c0: 7973 273a 2030 2c20 2768 6f75 7273 273a  ys': 0, 'hours':
-000006d0: 2031 2c20 276d 696e 7574 6573 273a 2030   1, 'minutes': 0
-000006e0: 2c20 2777 6565 6b73 273a 2030 7d2c 2063  , 'weeks': 0}, c
-000006f0: 6173 745f 7374 723d 5472 7565 2c20 666f  ast_str=True, fo
-00000700: 726d 6174 5f6f 7574 3d4e 6f6e 6594 6807  rmat_out=None.h.
-00000710: 5d94 2868 008c 0e64 6573 635f 7061 7261  ].(h...desc_para
-00000720: 6d65 7465 7294 9394 2981 947d 9428 6805  meter...)..}.(h.
-00000730: 8c1b 7374 6172 743d 2732 3031 362d 3037  ..start='2016-07
-00000740: 2d30 3120 3032 3a30 303a 3030 2794 6807  -01 02:00:00'.h.
-00000750: 5d94 2868 008c 0d64 6573 635f 7369 675f  ].(h...desc_sig_
-00000760: 6e61 6d65 9493 9429 8194 7d94 2868 058c  name...)..}.(h..
-00000770: 0573 7461 7274 9468 075d 9468 168c 0573  .start.h.].h...s
-00000780: 7461 7274 9485 9481 947d 9428 681b 68a0  tart.....}.(h.h.
-00000790: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
-000007a0: 9428 6821 5d94 6823 5d94 8c01 6e94 6168  .(h!].h#]...n.ah
-000007b0: 255d 9468 275d 9468 295d 9475 682b 689e  %].h'].h)].uh+h.
-000007c0: 681b 689a 7562 6800 8c11 6465 7363 5f73  h.h.ubh...desc_s
-000007d0: 6967 5f6f 7065 7261 746f 7294 9394 2981  ig_operator...).
-000007e0: 947d 9428 6805 8c01 3d94 6807 5d94 6816  .}.(h...=.h.].h.
-000007f0: 8c01 3d94 8594 8194 7d94 2868 1b68 b168  ..=.....}.(h.h.h
-00000800: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
-00000810: 2868 215d 9468 235d 948c 016f 9461 6825  (h!].h#]...o.ah%
-00000820: 5d94 6827 5d94 6829 5d94 7568 2b68 af68  ].h'].h)].uh+h.h
-00000830: 1b68 9a75 6268 098c 0669 6e6c 696e 6594  .h.ubh...inline.
-00000840: 9394 2981 947d 9428 6805 8c15 2732 3031  ..)..}.(h...'201
-00000850: 362d 3037 2d30 3120 3032 3a30 303a 3030  6-07-01 02:00:00
-00000860: 2794 6807 5d94 6816 8c15 2732 3031 362d  '.h.].h...'2016-
+00000440: 307d 2c20 6765 6e69 7465 723d 4661 6c73  0}, geniter=Fals
+00000450: 652c 2063 6173 745f 7374 723d 5472 7565  e, cast_str=True
+00000460: 2c20 666f 726d 6174 5f6f 7574 3d4e 6f6e  , format_out=Non
+00000470: 6529 9468 075d 9428 6800 8c0c 6465 7363  e).h.].(h...desc
+00000480: 5f61 6464 6e61 6d65 9493 9429 8194 7d94  _addname...)..}.
+00000490: 2868 058c 1263 6f6f 6b69 6573 5f75 7469  (h...cookies_uti
+000004a0: 6c69 7469 6573 2e94 6807 5d94 6816 8c12  lities..h.].h...
+000004b0: 636f 6f6b 6965 735f 7574 696c 6974 6965  cookies_utilitie
+000004c0: 732e 9485 9481 947d 9428 681b 686d 681c  s......}.(h.hmh.
+000004d0: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
+000004e0: 6821 5d94 6823 5d94 288c 0b73 6967 2d70  h!].h#].(..sig-p
+000004f0: 7265 6e61 6d65 948c 0d64 6573 6363 6c61  rename...desccla
+00000500: 7373 6e61 6d65 9465 6825 5d94 6827 5d94  ssname.eh%].h'].
+00000510: 6829 5d94 8c09 786d 6c3a 7370 6163 6594  h)]...xml:space.
+00000520: 8c08 7072 6573 6572 7665 9475 682b 686b  ..preserve.uh+hk
+00000530: 681b 6867 681c 6803 681d 8c71 433a 5c55  h.hgh.h.h..qC:\U
+00000540: 7365 7273 5c63 2d6d 6968 5c73 7061 6365  sers\c-mih\space
+00000550: 5c63 6f6f 6b69 6573 5f75 7469 6c69 7469  \cookies_utiliti
+00000560: 6573 5c73 7263 5c63 6f6f 6b69 6573 5f75  es\src\cookies_u
+00000570: 7469 6c69 7469 6573 5c5f 5f69 6e69 745f  tilities\__init_
+00000580: 5f2e 7079 3a64 6f63 7374 7269 6e67 206f  _.py:docstring o
+00000590: 6620 636f 6f6b 6965 735f 7574 696c 6974  f cookies_utilit
+000005a0: 6965 732e 6765 745f 6461 7465 7394 681e  ies.get_dates.h.
+000005b0: 4b01 7562 6800 8c09 6465 7363 5f6e 616d  K.ubh...desc_nam
+000005c0: 6594 9394 2981 947d 9428 6805 8c09 6765  e...)..}.(h...ge
+000005d0: 745f 6461 7465 7394 6807 5d94 6816 8c09  t_dates.h.].h...
+000005e0: 6765 745f 6461 7465 7394 8594 8194 7d94  get_dates.....}.
+000005f0: 2868 1b68 8268 1c68 0368 1d4e 681e 4e75  (h.h.h.h.h.Nh.Nu
+00000600: 6261 681f 7d94 2868 215d 9468 235d 9428  bah.}.(h!].h#].(
+00000610: 8c08 7369 672d 6e61 6d65 948c 0864 6573  ..sig-name...des
+00000620: 636e 616d 6594 6568 255d 9468 275d 9468  cname.eh%].h'].h
+00000630: 295d 9468 7d68 7e75 682b 6880 681b 6867  )].h}h~uh+h.h.hg
+00000640: 681c 6803 681d 687f 681e 4b01 7562 6800  h.h.h.h.h.K.ubh.
+00000650: 8c12 6465 7363 5f70 6172 616d 6574 6572  ..desc_parameter
+00000660: 6c69 7374 9493 9429 8194 7d94 2868 058c  list...)..}.(h..
+00000670: ba73 7461 7274 3d27 3230 3136 2d30 372d  .start='2016-07-
+00000680: 3031 2030 323a 3030 3a30 3027 2c20 656e  01 02:00:00', en
+00000690: 643d 2732 3031 362d 3037 2d30 3220 3031  d='2016-07-02 01
+000006a0: 3a30 303a 3030 272c 2066 6f72 6d61 743d  :00:00', format=
+000006b0: 2725 592d 256d 2d25 6420 2548 3a25 4d3a  '%Y-%m-%d %H:%M:
+000006c0: 2553 272c 2064 656c 7461 3d7b 2764 6179  %S', delta={'day
+000006d0: 7327 3a20 302c 2027 686f 7572 7327 3a20  s': 0, 'hours': 
+000006e0: 312c 2027 6d69 6e75 7465 7327 3a20 302c  1, 'minutes': 0,
+000006f0: 2027 7765 656b 7327 3a20 307d 2c20 6765   'weeks': 0}, ge
+00000700: 6e69 7465 723d 4661 6c73 652c 2063 6173  niter=False, cas
+00000710: 745f 7374 723d 5472 7565 2c20 666f 726d  t_str=True, form
+00000720: 6174 5f6f 7574 3d4e 6f6e 6594 6807 5d94  at_out=None.h.].
+00000730: 2868 008c 0e64 6573 635f 7061 7261 6d65  (h...desc_parame
+00000740: 7465 7294 9394 2981 947d 9428 6805 8c1b  ter...)..}.(h...
+00000750: 7374 6172 743d 2732 3031 362d 3037 2d30  start='2016-07-0
+00000760: 3120 3032 3a30 303a 3030 2794 6807 5d94  1 02:00:00'.h.].
+00000770: 2868 008c 0d64 6573 635f 7369 675f 6e61  (h...desc_sig_na
+00000780: 6d65 9493 9429 8194 7d94 2868 058c 0573  me...)..}.(h...s
+00000790: 7461 7274 9468 075d 9468 168c 0573 7461  tart.h.].h...sta
+000007a0: 7274 9485 9481 947d 9428 681b 68a0 681c  rt.....}.(h.h.h.
+000007b0: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
+000007c0: 6821 5d94 6823 5d94 8c01 6e94 6168 255d  h!].h#]...n.ah%]
+000007d0: 9468 275d 9468 295d 9475 682b 689e 681b  .h'].h)].uh+h.h.
+000007e0: 689a 7562 6800 8c11 6465 7363 5f73 6967  h.ubh...desc_sig
+000007f0: 5f6f 7065 7261 746f 7294 9394 2981 947d  _operator...)..}
+00000800: 9428 6805 8c01 3d94 6807 5d94 6816 8c01  .(h...=.h.].h...
+00000810: 3d94 8594 8194 7d94 2868 1b68 b168 1c68  =.....}.(h.h.h.h
+00000820: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+00000830: 215d 9468 235d 948c 016f 9461 6825 5d94  !].h#]...o.ah%].
+00000840: 6827 5d94 6829 5d94 7568 2b68 af68 1b68  h'].h)].uh+h.h.h
+00000850: 9a75 6268 098c 0669 6e6c 696e 6594 9394  .ubh...inline...
+00000860: 2981 947d 9428 6805 8c15 2732 3031 362d  )..}.(h...'2016-
 00000870: 3037 2d30 3120 3032 3a30 303a 3030 2794  07-01 02:00:00'.
-00000880: 8594 8194 7d94 2868 1b68 c268 1c68 0368  ....}.(h.h.h.h.h
-00000890: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-000008a0: 9468 235d 948c 0d64 6566 6175 6c74 5f76  .h#]...default_v
-000008b0: 616c 7565 9461 6825 5d94 6827 5d94 6829  alue.ah%].h'].h)
-000008c0: 5d94 8c13 7375 7070 6f72 745f 736d 6172  ]...support_smar
-000008d0: 7471 756f 7465 7394 8975 682b 68c0 681b  tquotes..uh+h.h.
-000008e0: 689a 7562 6568 1f7d 9428 6821 5d94 6823  h.ubeh.}.(h!].h#
-000008f0: 5d94 6825 5d94 6827 5d94 6829 5d94 687d  ].h%].h'].h)].h}
-00000900: 687e 7568 2b68 9868 1b68 9475 6268 9929  h~uh+h.h.h.ubh.)
-00000910: 8194 7d94 2868 058c 1965 6e64 3d27 3230  ..}.(h...end='20
-00000920: 3136 2d30 372d 3032 2030 313a 3030 3a30  16-07-02 01:00:0
-00000930: 3027 9468 075d 9428 689f 2981 947d 9428  0'.h.].(h.)..}.(
-00000940: 6805 8c03 656e 6494 6807 5d94 6816 8c03  h...end.h.].h...
-00000950: 656e 6494 8594 8194 7d94 2868 1b68 dc68  end.....}.(h.h.h
-00000960: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
-00000970: 2868 215d 9468 235d 9468 ab61 6825 5d94  (h!].h#].h.ah%].
-00000980: 6827 5d94 6829 5d94 7568 2b68 9e68 1b68  h'].h)].uh+h.h.h
-00000990: d875 6268 b029 8194 7d94 2868 058c 013d  .ubh.)..}.(h...=
-000009a0: 9468 075d 9468 168c 013d 9485 9481 947d  .h.].h...=.....}
-000009b0: 9428 681b 68ea 681c 6803 681d 4e68 1e4e  .(h.h.h.h.h.Nh.N
-000009c0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-000009d0: 68bc 6168 255d 9468 275d 9468 295d 9475  h.ah%].h'].h)].u
-000009e0: 682b 68af 681b 68d8 7562 68c1 2981 947d  h+h.h.h.ubh.)..}
-000009f0: 9428 6805 8c15 2732 3031 362d 3037 2d30  .(h...'2016-07-0
-00000a00: 3220 3031 3a30 303a 3030 2794 6807 5d94  2 01:00:00'.h.].
-00000a10: 6816 8c15 2732 3031 362d 3037 2d30 3220  h...'2016-07-02 
-00000a20: 3031 3a30 303a 3030 2794 8594 8194 7d94  01:00:00'.....}.
-00000a30: 2868 1b68 f868 1c68 0368 1d4e 681e 4e75  (h.h.h.h.h.Nh.Nu
-00000a40: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-00000a50: cd61 6825 5d94 6827 5d94 6829 5d94 8c13  .ah%].h'].h)]...
-00000a60: 7375 7070 6f72 745f 736d 6172 7471 756f  support_smartquo
-00000a70: 7465 7394 8975 682b 68c0 681b 68d8 7562  tes..uh+h.h.h.ub
-00000a80: 6568 1f7d 9428 6821 5d94 6823 5d94 6825  eh.}.(h!].h#].h%
-00000a90: 5d94 6827 5d94 6829 5d94 687d 687e 7568  ].h'].h)].h}h~uh
-00000aa0: 2b68 9868 1b68 9475 6268 9929 8194 7d94  +h.h.h.ubh.)..}.
-00000ab0: 2868 058c 1a66 6f72 6d61 743d 2725 592d  (h...format='%Y-
-00000ac0: 256d 2d25 6420 2548 3a25 4d3a 2553 2794  %m-%d %H:%M:%S'.
-00000ad0: 6807 5d94 2868 9f29 8194 7d94 2868 058c  h.].(h.)..}.(h..
-00000ae0: 0666 6f72 6d61 7494 6807 5d94 6816 8c06  .format.h.].h...
-00000af0: 666f 726d 6174 9485 9481 947d 9428 681b  format.....}.(h.
-00000b00: 6a11 0100 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
-00000b10: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-00000b20: ab61 6825 5d94 6827 5d94 6829 5d94 7568  .ah%].h'].h)].uh
-00000b30: 2b68 9e68 1b6a 0d01 0000 7562 68b0 2981  +h.h.j....ubh.).
-00000b40: 947d 9428 6805 8c01 3d94 6807 5d94 6816  .}.(h...=.h.].h.
-00000b50: 8c01 3d94 8594 8194 7d94 2868 1b6a 1f01  ..=.....}.(h.j..
-00000b60: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
-00000b70: 1f7d 9428 6821 5d94 6823 5d94 68bc 6168  .}.(h!].h#].h.ah
-00000b80: 255d 9468 275d 9468 295d 9475 682b 68af  %].h'].h)].uh+h.
-00000b90: 681b 6a0d 0100 0075 6268 c129 8194 7d94  h.j....ubh.)..}.
-00000ba0: 2868 058c 1327 2559 2d25 6d2d 2564 2025  (h...'%Y-%m-%d %
-00000bb0: 483a 254d 3a25 5327 9468 075d 9468 168c  H:%M:%S'.h.].h..
-00000bc0: 1327 2559 2d25 6d2d 2564 2025 483a 254d  .'%Y-%m-%d %H:%M
-00000bd0: 3a25 5327 9485 9481 947d 9428 681b 6a2d  :%S'.....}.(h.j-
-00000be0: 0100 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
-00000bf0: 681f 7d94 2868 215d 9468 235d 9468 cd61  h.}.(h!].h#].h.a
-00000c00: 6825 5d94 6827 5d94 6829 5d94 8c13 7375  h%].h'].h)]...su
-00000c10: 7070 6f72 745f 736d 6172 7471 756f 7465  pport_smartquote
-00000c20: 7394 8975 682b 68c0 681b 6a0d 0100 0075  s..uh+h.h.j....u
-00000c30: 6265 681f 7d94 2868 215d 9468 235d 9468  beh.}.(h!].h#].h
-00000c40: 255d 9468 275d 9468 295d 9468 7d68 7e75  %].h'].h)].h}h~u
-00000c50: 682b 6898 681b 6894 7562 6899 2981 947d  h+h.h.h.ubh.)..}
-00000c60: 9428 6805 8c37 6465 6c74 613d 7b27 6461  .(h..7delta={'da
-00000c70: 7973 273a 2030 2c20 2768 6f75 7273 273a  ys': 0, 'hours':
-00000c80: 2031 2c20 276d 696e 7574 6573 273a 2030   1, 'minutes': 0
-00000c90: 2c20 2777 6565 6b73 273a 2030 7d94 6807  , 'weeks': 0}.h.
-00000ca0: 5d94 2868 9f29 8194 7d94 2868 058c 0564  ].(h.)..}.(h...d
-00000cb0: 656c 7461 9468 075d 9468 168c 0564 656c  elta.h.].h...del
-00000cc0: 7461 9485 9481 947d 9428 681b 6a46 0100  ta.....}.(h.jF..
-00000cd0: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
-00000ce0: 7d94 2868 215d 9468 235d 9468 ab61 6825  }.(h!].h#].h.ah%
-00000cf0: 5d94 6827 5d94 6829 5d94 7568 2b68 9e68  ].h'].h)].uh+h.h
-00000d00: 1b6a 4201 0000 7562 68b0 2981 947d 9428  .jB...ubh.)..}.(
-00000d10: 6805 8c01 3d94 6807 5d94 6816 8c01 3d94  h...=.h.].h...=.
-00000d20: 8594 8194 7d94 2868 1b6a 5401 0000 681c  ....}.(h.jT...h.
-00000d30: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
-00000d40: 6821 5d94 6823 5d94 68bc 6168 255d 9468  h!].h#].h.ah%].h
-00000d50: 275d 9468 295d 9475 682b 68af 681b 6a42  '].h)].uh+h.h.jB
-00000d60: 0100 0075 6268 c129 8194 7d94 2868 058c  ...ubh.)..}.(h..
-00000d70: 317b 2764 6179 7327 3a20 302c 2027 686f  1{'days': 0, 'ho
-00000d80: 7572 7327 3a20 312c 2027 6d69 6e75 7465  urs': 1, 'minute
-00000d90: 7327 3a20 302c 2027 7765 656b 7327 3a20  s': 0, 'weeks': 
-00000da0: 307d 9468 075d 9468 168c 317b 2764 6179  0}.h.].h..1{'day
-00000db0: 7327 3a20 302c 2027 686f 7572 7327 3a20  s': 0, 'hours': 
-00000dc0: 312c 2027 6d69 6e75 7465 7327 3a20 302c  1, 'minutes': 0,
-00000dd0: 2027 7765 656b 7327 3a20 307d 9485 9481   'weeks': 0}....
-00000de0: 947d 9428 681b 6a62 0100 0068 1c68 0368  .}.(h.jb...h.h.h
-00000df0: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-00000e00: 9468 235d 9468 cd61 6825 5d94 6827 5d94  .h#].h.ah%].h'].
-00000e10: 6829 5d94 8c13 7375 7070 6f72 745f 736d  h)]...support_sm
-00000e20: 6172 7471 756f 7465 7394 8975 682b 68c0  artquotes..uh+h.
-00000e30: 681b 6a42 0100 0075 6265 681f 7d94 2868  h.jB...ubeh.}.(h
-00000e40: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00000e50: 295d 9468 7d68 7e75 682b 6898 681b 6894  )].h}h~uh+h.h.h.
-00000e60: 7562 6899 2981 947d 9428 6805 8c0d 6361  ubh.)..}.(h...ca
-00000e70: 7374 5f73 7472 3d54 7275 6594 6807 5d94  st_str=True.h.].
-00000e80: 2868 9f29 8194 7d94 2868 058c 0863 6173  (h.)..}.(h...cas
-00000e90: 745f 7374 7294 6807 5d94 6816 8c08 6361  t_str.h.].h...ca
-00000ea0: 7374 5f73 7472 9485 9481 947d 9428 681b  st_str.....}.(h.
-00000eb0: 6a7b 0100 0068 1c68 0368 1d4e 681e 4e75  j{...h.h.h.Nh.Nu
-00000ec0: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-00000ed0: ab61 6825 5d94 6827 5d94 6829 5d94 7568  .ah%].h'].h)].uh
-00000ee0: 2b68 9e68 1b6a 7701 0000 7562 68b0 2981  +h.h.jw...ubh.).
-00000ef0: 947d 9428 6805 8c01 3d94 6807 5d94 6816  .}.(h...=.h.].h.
-00000f00: 8c01 3d94 8594 8194 7d94 2868 1b6a 8901  ..=.....}.(h.j..
-00000f10: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
-00000f20: 1f7d 9428 6821 5d94 6823 5d94 68bc 6168  .}.(h!].h#].h.ah
-00000f30: 255d 9468 275d 9468 295d 9475 682b 68af  %].h'].h)].uh+h.
-00000f40: 681b 6a77 0100 0075 6268 c129 8194 7d94  h.jw...ubh.)..}.
-00000f50: 2868 058c 0454 7275 6594 6807 5d94 6816  (h...True.h.].h.
-00000f60: 8c04 5472 7565 9485 9481 947d 9428 681b  ..True.....}.(h.
-00000f70: 6a97 0100 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
-00000f80: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-00000f90: cd61 6825 5d94 6827 5d94 6829 5d94 8c13  .ah%].h'].h)]...
-00000fa0: 7375 7070 6f72 745f 736d 6172 7471 756f  support_smartquo
-00000fb0: 7465 7394 8975 682b 68c0 681b 6a77 0100  tes..uh+h.h.jw..
-00000fc0: 0075 6265 681f 7d94 2868 215d 9468 235d  .ubeh.}.(h!].h#]
-00000fd0: 9468 255d 9468 275d 9468 295d 9468 7d68  .h%].h'].h)].h}h
-00000fe0: 7e75 682b 6898 681b 6894 7562 6899 2981  ~uh+h.h.h.ubh.).
-00000ff0: 947d 9428 6805 8c0f 666f 726d 6174 5f6f  .}.(h...format_o
-00001000: 7574 3d4e 6f6e 6594 6807 5d94 2868 9f29  ut=None.h.].(h.)
-00001010: 8194 7d94 2868 058c 0a66 6f72 6d61 745f  ..}.(h...format_
-00001020: 6f75 7494 6807 5d94 6816 8c0a 666f 726d  out.h.].h...form
-00001030: 6174 5f6f 7574 9485 9481 947d 9428 681b  at_out.....}.(h.
-00001040: 6ab0 0100 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
-00001050: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-00001060: ab61 6825 5d94 6827 5d94 6829 5d94 7568  .ah%].h'].h)].uh
-00001070: 2b68 9e68 1b6a ac01 0000 7562 68b0 2981  +h.h.j....ubh.).
-00001080: 947d 9428 6805 8c01 3d94 6807 5d94 6816  .}.(h...=.h.].h.
-00001090: 8c01 3d94 8594 8194 7d94 2868 1b6a be01  ..=.....}.(h.j..
-000010a0: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
-000010b0: 1f7d 9428 6821 5d94 6823 5d94 68bc 6168  .}.(h!].h#].h.ah
-000010c0: 255d 9468 275d 9468 295d 9475 682b 68af  %].h'].h)].uh+h.
-000010d0: 681b 6aac 0100 0075 6268 c129 8194 7d94  h.j....ubh.)..}.
-000010e0: 2868 058c 044e 6f6e 6594 6807 5d94 6816  (h...None.h.].h.
-000010f0: 8c04 4e6f 6e65 9485 9481 947d 9428 681b  ..None.....}.(h.
-00001100: 6acc 0100 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
-00001110: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-00001120: cd61 6825 5d94 6827 5d94 6829 5d94 8c13  .ah%].h'].h)]...
-00001130: 7375 7070 6f72 745f 736d 6172 7471 756f  support_smartquo
-00001140: 7465 7394 8975 682b 68c0 681b 6aac 0100  tes..uh+h.h.j...
-00001150: 0075 6265 681f 7d94 2868 215d 9468 235d  .ubeh.}.(h!].h#]
-00001160: 9468 255d 9468 275d 9468 295d 9468 7d68  .h%].h'].h)].h}h
-00001170: 7e75 682b 6898 681b 6894 7562 6568 1f7d  ~uh+h.h.h.ubeh.}
-00001180: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-00001190: 5d94 6829 5d94 687d 687e 7568 2b68 9268  ].h)].h}h~uh+h.h
-000011a0: 1b68 6768 1c68 0368 1d68 7f68 1e4b 0175  .hgh.h.h.h.h.K.u
-000011b0: 6265 681f 7d94 2868 215d 9468 5e61 6823  beh.}.(h!].h^ah#
-000011c0: 5d94 288c 0373 6967 948c 0a73 6967 2d6f  ].(..sig...sig-o
-000011d0: 626a 6563 7494 6568 255d 9468 275d 9468  bject.eh%].h'].h
-000011e0: 295d 948c 066d 6f64 756c 6594 8c11 636f  )]...module...co
-000011f0: 6f6b 6965 735f 7574 696c 6974 6965 7394  okies_utilities.
-00001200: 8c05 636c 6173 7394 6806 8c08 6675 6c6c  ..class.h...full
-00001210: 6e61 6d65 9468 848c 0a5f 746f 635f 7061  name.h..._toc_pa
-00001220: 7274 7394 6af0 0100 0068 8486 948c 095f  rts.j....h....._
-00001230: 746f 635f 6e61 6d65 948c 0b67 6574 5f64  toc_name...get_d
-00001240: 6174 6573 2829 9475 682b 6865 681d 687f  ates().uh+heh.h.
-00001250: 681e 4b01 681b 6862 681c 6803 7562 6800  h.K.h.hbh.h.ubh.
-00001260: 8c0c 6465 7363 5f63 6f6e 7465 6e74 9493  ..desc_content..
-00001270: 9429 8194 7d94 2868 0568 0668 075d 9428  .)..}.(h.h.h.].(
-00001280: 6809 8c09 7061 7261 6772 6170 6894 9394  h...paragraph...
-00001290: 2981 947d 9428 6805 8c58 5265 7475 726e  )..}.(h..XReturn
-000012a0: 7320 6120 6c69 7374 206f 6620 7469 6d65  s a list of time
-000012b0: 7320 6672 6f6d 2074 6865 2027 7374 6172  s from the 'star
-000012c0: 7427 2074 696d 6520 746f 2074 6865 2027  t' time to the '
-000012d0: 656e 6427 2074 696d 652c 0a69 6e63 7265  end' time,.incre
-000012e0: 6d65 6e74 6564 2062 7920 2764 656c 7461  mented by 'delta
-000012f0: 272e 9468 075d 9468 168c 6452 6574 7572  '..h.].h..dRetur
-00001300: 6e73 2061 206c 6973 7420 6f66 2074 696d  ns a list of tim
-00001310: 6573 2066 726f 6d20 7468 6520 e280 9873  es from the ...s
-00001320: 7461 7274 e280 9920 7469 6d65 2074 6f20  tart... time to 
-00001330: 7468 6520 e280 9865 6e64 e280 9920 7469  the ...end... ti
-00001340: 6d65 2c0a 696e 6372 656d 656e 7465 6420  me,.incremented 
-00001350: 6279 20e2 8098 6465 6c74 61e2 8099 2e94  by ...delta.....
-00001360: 8594 8194 7d94 2868 1b6a fe01 0000 681c  ....}.(h.j....h.
-00001370: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
-00001380: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-00001390: 6829 5d94 7568 2b6a fc01 0000 681d 8c71  h)].uh+j....h..q
-000013a0: 433a 5c55 7365 7273 5c63 2d6d 6968 5c73  C:\Users\c-mih\s
-000013b0: 7061 6365 5c63 6f6f 6b69 6573 5f75 7469  pace\cookies_uti
-000013c0: 6c69 7469 6573 5c73 7263 5c63 6f6f 6b69  lities\src\cooki
-000013d0: 6573 5f75 7469 6c69 7469 6573 5c5f 5f69  es_utilities\__i
-000013e0: 6e69 745f 5f2e 7079 3a64 6f63 7374 7269  nit__.py:docstri
-000013f0: 6e67 206f 6620 636f 6f6b 6965 735f 7574  ng of cookies_ut
-00001400: 696c 6974 6965 732e 6765 745f 6461 7465  ilities.get_date
-00001410: 7394 681e 4b01 681b 6af9 0100 0068 1c68  s.h.K.h.j....h.h
-00001420: 0375 6268 098c 0a66 6965 6c64 5f6c 6973  .ubh...field_lis
-00001430: 7494 9394 2981 947d 9428 6805 6806 6807  t...)..}.(h.h.h.
-00001440: 5d94 2868 098c 0566 6965 6c64 9493 9429  ].(h...field...)
-00001450: 8194 7d94 2868 0568 0668 075d 9428 6809  ..}.(h.h.h.].(h.
-00001460: 8c0a 6669 656c 645f 6e61 6d65 9493 9429  ..field_name...)
-00001470: 8194 7d94 2868 058c 0a50 6172 616d 6574  ..}.(h...Paramet
-00001480: 6572 7394 6807 5d94 6816 8c0a 5061 7261  ers.h.].h...Para
-00001490: 6d65 7465 7273 9485 9481 947d 9428 681b  meters.....}.(h.
-000014a0: 6a19 0200 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
-000014b0: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-000014c0: 255d 9468 275d 9468 295d 9475 682b 6a17  %].h'].h)].uh+j.
-000014d0: 0200 0068 1b6a 1402 0000 681d 687f 681e  ...h.j....h.h.h.
-000014e0: 4b00 7562 6809 8c0a 6669 656c 645f 626f  K.ubh...field_bo
-000014f0: 6479 9493 9429 8194 7d94 2868 0568 0668  dy...)..}.(h.h.h
-00001500: 075d 9468 098c 0b62 756c 6c65 745f 6c69  .].h...bullet_li
-00001510: 7374 9493 9429 8194 7d94 2868 0568 0668  st...)..}.(h.h.h
-00001520: 075d 9428 6809 8c09 6c69 7374 5f69 7465  .].(h...list_ite
-00001530: 6d94 9394 2981 947d 9428 6805 6806 6807  m...)..}.(h.h.h.
-00001540: 5d94 6afd 0100 0029 8194 7d94 2868 058c  ].j....)..}.(h..
-00001550: 2473 7461 7274 2028 7374 7269 6e67 2920  $start (string) 
-00001560: 2d2d 2053 7461 7274 2074 696d 6520 7374  -- Start time st
-00001570: 7269 6e67 2e94 6807 5d94 2868 008c 0e6c  ring..h.].(h...l
-00001580: 6974 6572 616c 5f73 7472 6f6e 6794 9394  iteral_strong...
-00001590: 2981 947d 9428 6805 8c05 7374 6172 7494  )..}.(h...start.
-000015a0: 6807 5d94 6816 8c05 7374 6172 7494 8594  h.].h...start...
-000015b0: 8194 7d94 2868 1b6a 3c02 0000 681c 6803  ..}.(h.j<...h.h.
-000015c0: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
-000015d0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-000015e0: 5d94 7568 2b6a 3a02 0000 681b 6a36 0200  ].uh+j:...h.j6..
-000015f0: 0075 6268 168c 0220 2894 8594 8194 7d94  .ubh... (.....}.
-00001600: 2868 1b6a 3602 0000 681c 6803 681d 4e68  (h.j6...h.h.h.Nh
-00001610: 1e4e 7562 6800 8c0c 7065 6e64 696e 675f  .Nubh...pending_
-00001620: 7872 6566 9493 9429 8194 7d94 2868 0568  xref...)..}.(h.h
-00001630: 0668 075d 9468 008c 106c 6974 6572 616c  .h.].h...literal
-00001640: 5f65 6d70 6861 7369 7394 9394 2981 947d  _emphasis...)..}
-00001650: 9428 6805 8c06 7374 7269 6e67 9468 075d  .(h...string.h.]
-00001660: 9468 168c 0673 7472 696e 6794 8594 8194  .h...string.....
-00001670: 7d94 2868 1b6a 5502 0000 681c 6803 681d  }.(h.jU...h.h.h.
-00001680: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
-00001690: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-000016a0: 7568 2b6a 5302 0000 681b 6a50 0200 0075  uh+jS...h.jP...u
-000016b0: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-000016c0: 255d 9468 275d 9468 295d 948c 0972 6566  %].h'].h)]...ref
-000016d0: 646f 6d61 696e 948c 0270 7994 8c0b 7265  domain...py...re
-000016e0: 6665 7870 6c69 6369 7494 898c 0772 6566  fexplicit....ref
-000016f0: 7479 7065 946a f101 0000 8c09 7265 6674  type.j......reft
-00001700: 6172 6765 7494 6a57 0200 008c 0b72 6566  arget.jW.....ref
-00001710: 7370 6563 6966 6963 9488 8c09 7079 3a6d  specific....py:m
-00001720: 6f64 756c 6594 6af0 0100 008c 0870 793a  odule.j......py:
-00001730: 636c 6173 7394 4e75 682b 6a4e 0200 0068  class.Nuh+jN...h
-00001740: 1b6a 3602 0000 7562 6816 8c01 2994 8594  .j6...ubh...)...
-00001750: 8194 7d94 2868 1b6a 3602 0000 681c 6803  ..}.(h.j6...h.h.
-00001760: 681d 4e68 1e4e 7562 6816 8c05 20e2 8093  h.Nh.Nubh... ...
-00001770: 2094 8594 8194 7d94 2868 1b6a 3602 0000   .....}.(h.j6...
-00001780: 681c 6803 681d 4e68 1e4e 7562 6816 8c12  h.h.h.Nh.Nubh...
-00001790: 5374 6172 7420 7469 6d65 2073 7472 696e  Start time strin
-000017a0: 672e 9485 9481 947d 9428 681b 6a36 0200  g......}.(h.j6..
-000017b0: 0068 1c68 0368 1d4e 681e 4e75 6265 681f  .h.h.h.Nh.Nubeh.
-000017c0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-000017d0: 275d 9468 295d 9475 682b 6afc 0100 0068  '].h)].uh+j....h
-000017e0: 1b6a 3302 0000 7562 6168 1f7d 9428 6821  .j3...ubah.}.(h!
-000017f0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00001800: 5d94 7568 2b6a 3102 0000 681b 6a2e 0200  ].uh+j1...h.j...
-00001810: 0075 626a 3202 0000 2981 947d 9428 6805  .ubj2...)..}.(h.
-00001820: 6806 6807 5d94 6afd 0100 0029 8194 7d94  h.h.].j....)..}.
-00001830: 2868 058c 2065 6e64 2028 7374 7269 6e67  (h.. end (string
-00001840: 2920 2d2d 2045 6e64 2074 696d 6520 7374  ) -- End time st
-00001850: 7269 6e67 2e94 6807 5d94 286a 3b02 0000  ring..h.].(j;...
-00001860: 2981 947d 9428 6805 8c03 656e 6494 6807  )..}.(h...end.h.
-00001870: 5d94 6816 8c03 656e 6494 8594 8194 7d94  ].h...end.....}.
-00001880: 2868 1b6a 9002 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
-00001890: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
-000018a0: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
-000018b0: 2b6a 3a02 0000 681b 6a8c 0200 0075 6268  +j:...h.j....ubh
-000018c0: 168c 0220 2894 8594 8194 7d94 2868 1b6a  ... (.....}.(h.j
-000018d0: 8c02 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
-000018e0: 6a4f 0200 0029 8194 7d94 2868 0568 0668  jO...)..}.(h.h.h
-000018f0: 075d 946a 5402 0000 2981 947d 9428 6805  .].jT...)..}.(h.
-00001900: 8c06 7374 7269 6e67 9468 075d 9468 168c  ..string.h.].h..
-00001910: 0673 7472 696e 6794 8594 8194 7d94 2868  .string.....}.(h
-00001920: 1b6a a502 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
-00001930: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-00001940: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
-00001950: 5302 0000 681b 6aa2 0200 0075 6261 681f  S...h.j....ubah.
-00001960: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-00001970: 275d 9468 295d 948c 0972 6566 646f 6d61  '].h)]...refdoma
-00001980: 696e 946a 6a02 0000 8c0b 7265 6665 7870  in.jj.....refexp
-00001990: 6c69 6369 7494 898c 0772 6566 7479 7065  licit....reftype
-000019a0: 946a f101 0000 8c09 7265 6674 6172 6765  .j......reftarge
-000019b0: 7494 6aa7 0200 006a 6e02 0000 886a 6f02  t.j....jn....jo.
-000019c0: 0000 6af0 0100 006a 7002 0000 4e75 682b  ..j....jp...Nuh+
-000019d0: 6a4e 0200 0068 1b6a 8c02 0000 7562 6816  jN...h.j....ubh.
-000019e0: 8c01 2994 8594 8194 7d94 2868 1b6a 8c02  ..).....}.(h.j..
-000019f0: 0000 681c 6803 681d 4e68 1e4e 7562 6816  ..h.h.h.Nh.Nubh.
-00001a00: 8c05 20e2 8093 2094 8594 8194 7d94 2868  .. ... .....}.(h
-00001a10: 1b6a 8c02 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
-00001a20: 7562 6816 8c10 456e 6420 7469 6d65 2073  ubh...End time s
-00001a30: 7472 696e 672e 9485 9481 947d 9428 681b  tring......}.(h.
-00001a40: 6a8c 0200 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
-00001a50: 6265 681f 7d94 2868 215d 9468 235d 9468  beh.}.(h!].h#].h
-00001a60: 255d 9468 275d 9468 295d 9475 682b 6afc  %].h'].h)].uh+j.
-00001a70: 0100 0068 1b6a 8902 0000 7562 6168 1f7d  ...h.j....ubah.}
-00001a80: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-00001a90: 5d94 6829 5d94 7568 2b6a 3102 0000 681b  ].h)].uh+j1...h.
-00001aa0: 6a2e 0200 0075 626a 3202 0000 2981 947d  j....ubj2...)..}
-00001ab0: 9428 6805 6806 6807 5d94 6afd 0100 0029  .(h.h.h.].j....)
-00001ac0: 8194 7d94 2868 058c 3b66 6f72 6d61 7420  ..}.(h..;format 
-00001ad0: 2873 7472 696e 6729 202d 2d20 436f 6e76  (string) -- Conv
-00001ae0: 6572 7369 6f6e 2066 6f72 6d61 7420 666f  ersion format fo
-00001af0: 7220 6461 7465 7469 6d65 2e73 7472 7074  r datetime.strpt
-00001b00: 696d 652e 9468 075d 9428 6a3b 0200 0029  ime..h.].(j;...)
-00001b10: 8194 7d94 2868 058c 0666 6f72 6d61 7494  ..}.(h...format.
-00001b20: 6807 5d94 6816 8c06 666f 726d 6174 9485  h.].h...format..
-00001b30: 9481 947d 9428 681b 6adc 0200 0068 1c68  ...}.(h.j....h.h
-00001b40: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
-00001b50: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00001b60: 295d 9475 682b 6a3a 0200 0068 1b6a d802  )].uh+j:...h.j..
-00001b70: 0000 7562 6816 8c02 2028 9485 9481 947d  ..ubh... (.....}
-00001b80: 9428 681b 6ad8 0200 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
-00001b90: 681e 4e75 626a 4f02 0000 2981 947d 9428  h.NubjO...)..}.(
-00001ba0: 6805 6806 6807 5d94 6a54 0200 0029 8194  h.h.h.].jT...)..
-00001bb0: 7d94 2868 058c 0673 7472 696e 6794 6807  }.(h...string.h.
-00001bc0: 5d94 6816 8c06 7374 7269 6e67 9485 9481  ].h...string....
-00001bd0: 947d 9428 681b 6af1 0200 0068 1c68 0368  .}.(h.j....h.h.h
-00001be0: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-00001bf0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00001c00: 9475 682b 6a53 0200 0068 1b6a ee02 0000  .uh+jS...h.j....
-00001c10: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-00001c20: 6825 5d94 6827 5d94 6829 5d94 8c09 7265  h%].h'].h)]...re
-00001c30: 6664 6f6d 6169 6e94 6a6a 0200 008c 0b72  fdomain.jj.....r
-00001c40: 6566 6578 706c 6963 6974 9489 8c07 7265  efexplicit....re
-00001c50: 6674 7970 6594 6af1 0100 008c 0972 6566  ftype.j......ref
-00001c60: 7461 7267 6574 946a f302 0000 6a6e 0200  target.j....jn..
-00001c70: 0088 6a6f 0200 006a f001 0000 6a70 0200  ..jo...j....jp..
-00001c80: 004e 7568 2b6a 4e02 0000 681b 6ad8 0200  .Nuh+jN...h.j...
-00001c90: 0075 6268 168c 0129 9485 9481 947d 9428  .ubh...).....}.(
-00001ca0: 681b 6ad8 0200 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
-00001cb0: 4e75 6268 168c 0520 e280 9320 9485 9481  Nubh... ... ....
-00001cc0: 947d 9428 681b 6ad8 0200 0068 1c68 0368  .}.(h.j....h.h.h
-00001cd0: 1d4e 681e 4e75 6268 168c 2843 6f6e 7665  .Nh.Nubh..(Conve
-00001ce0: 7273 696f 6e20 666f 726d 6174 2066 6f72  rsion format for
-00001cf0: 2064 6174 6574 696d 652e 7374 7270 7469   datetime.strpti
-00001d00: 6d65 2e94 8594 8194 7d94 2868 1b6a d802  me......}.(h.j..
-00001d10: 0000 681c 6803 681d 4e68 1e4e 7562 6568  ..h.h.h.Nh.Nubeh
-00001d20: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-00001d30: 6827 5d94 6829 5d94 7568 2b6a fc01 0000  h'].h)].uh+j....
-00001d40: 681b 6ad5 0200 0075 6261 681f 7d94 2868  h.j....ubah.}.(h
-00001d50: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00001d60: 295d 9475 682b 6a31 0200 0068 1b6a 2e02  )].uh+j1...h.j..
-00001d70: 0000 7562 6a32 0200 0029 8194 7d94 2868  ..ubj2...)..}.(h
-00001d80: 0568 0668 075d 946a fd01 0000 2981 947d  .h.h.].j....)..}
-00001d90: 9428 6805 8c39 6465 6c74 6120 2864 6963  .(h..9delta (dic
-00001da0: 7429 202d 2d20 5469 6d65 6465 6c74 6120  t) -- Timedelta 
-00001db0: 6173 2061 7267 7320 666f 7220 6461 7465  as args for date
-00001dc0: 7469 6d65 2e74 696d 6564 656c 7461 2e94  time.timedelta..
-00001dd0: 6807 5d94 286a 3b02 0000 2981 947d 9428  h.].(j;...)..}.(
-00001de0: 6805 8c05 6465 6c74 6194 6807 5d94 6816  h...delta.h.].h.
-00001df0: 8c05 6465 6c74 6194 8594 8194 7d94 2868  ..delta.....}.(h
-00001e00: 1b6a 2803 0000 681c 6803 681d 4e68 1e4e  .j(...h.h.h.Nh.N
-00001e10: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-00001e20: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
-00001e30: 3a02 0000 681b 6a24 0300 0075 6268 168c  :...h.j$...ubh..
-00001e40: 0220 2894 8594 8194 7d94 2868 1b6a 2403  . (.....}.(h.j$.
-00001e50: 0000 681c 6803 681d 4e68 1e4e 7562 6a4f  ..h.h.h.Nh.NubjO
-00001e60: 0200 0029 8194 7d94 2868 0568 0668 075d  ...)..}.(h.h.h.]
-00001e70: 946a 5402 0000 2981 947d 9428 6805 8c04  .jT...)..}.(h...
-00001e80: 6469 6374 9468 075d 9468 168c 0464 6963  dict.h.].h...dic
-00001e90: 7494 8594 8194 7d94 2868 1b6a 3d03 0000  t.....}.(h.j=...
-00001ea0: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
-00001eb0: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-00001ec0: 5d94 6829 5d94 7568 2b6a 5302 0000 681b  ].h)].uh+jS...h.
-00001ed0: 6a3a 0300 0075 6261 681f 7d94 2868 215d  j:...ubah.}.(h!]
-00001ee0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00001ef0: 948c 0972 6566 646f 6d61 696e 946a 6a02  ...refdomain.jj.
-00001f00: 0000 8c0b 7265 6665 7870 6c69 6369 7494  ....refexplicit.
-00001f10: 898c 0772 6566 7479 7065 946a f101 0000  ...reftype.j....
-00001f20: 8c09 7265 6674 6172 6765 7494 6a3f 0300  ..reftarget.j?..
-00001f30: 006a 6e02 0000 886a 6f02 0000 6af0 0100  .jn....jo...j...
-00001f40: 006a 7002 0000 4e75 682b 6a4e 0200 0068  .jp...Nuh+jN...h
-00001f50: 1b6a 2403 0000 7562 6816 8c01 2994 8594  .j$...ubh...)...
-00001f60: 8194 7d94 2868 1b6a 2403 0000 681c 6803  ..}.(h.j$...h.h.
-00001f70: 681d 4e68 1e4e 7562 6816 8c05 20e2 8093  h.Nh.Nubh... ...
-00001f80: 2094 8594 8194 7d94 2868 1b6a 2403 0000   .....}.(h.j$...
-00001f90: 681c 6803 681d 4e68 1e4e 7562 6816 8c29  h.h.h.Nh.Nubh..)
-00001fa0: 5469 6d65 6465 6c74 6120 6173 2061 7267  Timedelta as arg
-00001fb0: 7320 666f 7220 6461 7465 7469 6d65 2e74  s for datetime.t
-00001fc0: 696d 6564 656c 7461 2e94 8594 8194 7d94  imedelta......}.
-00001fd0: 2868 1b6a 2403 0000 681c 6803 681d 4e68  (h.j$...h.h.h.Nh
-00001fe0: 1e4e 7562 6568 1f7d 9428 6821 5d94 6823  .Nubeh.}.(h!].h#
-00001ff0: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
-00002000: 2b6a fc01 0000 681b 6a21 0300 0075 6261  +j....h.j!...uba
-00002010: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00002020: 9468 275d 9468 295d 9475 682b 6a31 0200  .h'].h)].uh+j1..
-00002030: 0068 1b6a 2e02 0000 7562 6a32 0200 0029  .h.j....ubj2...)
-00002040: 8194 7d94 2868 0568 0668 075d 946a fd01  ..}.(h.h.h.].j..
-00002050: 0000 2981 947d 9428 6805 8c46 6361 7374  ..)..}.(h..Fcast
-00002060: 5f73 7472 2028 626f 6f6c 2920 2d2d 2057  _str (bool) -- W
-00002070: 6865 7468 6572 2074 6f20 636f 6e76 6572  hether to conver
-00002080: 7420 6f75 7470 7574 2074 6f20 7374 7269  t output to stri
-00002090: 6e67 2028 6465 6661 756c 7420 7472 7565  ng (default true
-000020a0: 292e 9468 075d 9428 6a3b 0200 0029 8194  )..h.].(j;...)..
-000020b0: 7d94 2868 058c 0863 6173 745f 7374 7294  }.(h...cast_str.
-000020c0: 6807 5d94 6816 8c08 6361 7374 5f73 7472  h.].h...cast_str
-000020d0: 9485 9481 947d 9428 681b 6a74 0300 0068  .....}.(h.jt...h
-000020e0: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
-000020f0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
-00002100: 9468 295d 9475 682b 6a3a 0200 0068 1b6a  .h)].uh+j:...h.j
-00002110: 7003 0000 7562 6816 8c02 2028 9485 9481  p...ubh... (....
-00002120: 947d 9428 681b 6a70 0300 0068 1c68 0368  .}.(h.jp...h.h.h
-00002130: 1d4e 681e 4e75 626a 4f02 0000 2981 947d  .Nh.NubjO...)..}
-00002140: 9428 6805 6806 6807 5d94 6a54 0200 0029  .(h.h.h.].jT...)
-00002150: 8194 7d94 2868 058c 0462 6f6f 6c94 6807  ..}.(h...bool.h.
-00002160: 5d94 6816 8c04 626f 6f6c 9485 9481 947d  ].h...bool.....}
-00002170: 9428 681b 6a89 0300 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
-00002180: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
-00002190: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-000021a0: 682b 6a53 0200 0068 1b6a 8603 0000 7562  h+jS...h.j....ub
-000021b0: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-000021c0: 5d94 6827 5d94 6829 5d94 8c09 7265 6664  ].h'].h)]...refd
-000021d0: 6f6d 6169 6e94 6a6a 0200 008c 0b72 6566  omain.jj.....ref
-000021e0: 6578 706c 6963 6974 9489 8c07 7265 6674  explicit....reft
-000021f0: 7970 6594 6af1 0100 008c 0972 6566 7461  ype.j......refta
-00002200: 7267 6574 946a 8b03 0000 6a6e 0200 0088  rget.j....jn....
-00002210: 6a6f 0200 006a f001 0000 6a70 0200 004e  jo...j....jp...N
-00002220: 7568 2b6a 4e02 0000 681b 6a70 0300 0075  uh+jN...h.jp...u
-00002230: 6268 168c 0129 9485 9481 947d 9428 681b  bh...).....}.(h.
-00002240: 6a70 0300 0068 1c68 0368 1d4e 681e 4e75  jp...h.h.h.Nh.Nu
-00002250: 6268 168c 0520 e280 9320 9485 9481 947d  bh... ... .....}
-00002260: 9428 681b 6a70 0300 0068 1c68 0368 1d4e  .(h.jp...h.h.h.N
-00002270: 681e 4e75 6268 168c 3357 6865 7468 6572  h.Nubh..3Whether
-00002280: 2074 6f20 636f 6e76 6572 7420 6f75 7470   to convert outp
-00002290: 7574 2074 6f20 7374 7269 6e67 2028 6465  ut to string (de
-000022a0: 6661 756c 7420 7472 7565 292e 9485 9481  fault true).....
-000022b0: 947d 9428 681b 6a70 0300 0068 1c68 0368  .}.(h.jp...h.h.h
-000022c0: 1d4e 681e 4e75 6265 681f 7d94 2868 215d  .Nh.Nubeh.}.(h!]
-000022d0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-000022e0: 9475 682b 6afc 0100 0068 1b6a 6d03 0000  .uh+j....h.jm...
-000022f0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-00002300: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
-00002310: 3102 0000 681b 6a2e 0200 0075 626a 3202  1...h.j....ubj2.
-00002320: 0000 2981 947d 9428 6805 6806 6807 5d94  ..)..}.(h.h.h.].
-00002330: 6afd 0100 0029 8194 7d94 2868 058c 4d66  j....)..}.(h..Mf
-00002340: 6f72 6d61 745f 6f75 7420 2873 7472 696e  ormat_out (strin
-00002350: 6729 202d 2d20 436f 6e76 6572 7369 6f6e  g) -- Conversion
-00002360: 2066 6f72 6d61 7420 666f 7220 6f75 7470   format for outp
-00002370: 7574 2028 6465 6661 756c 7420 7361 6d65  ut (default same
-00002380: 2074 6f20 666f 726d 6174 292e 9468 075d   to format)..h.]
-00002390: 9428 6a3b 0200 0029 8194 7d94 2868 058c  .(j;...)..}.(h..
-000023a0: 0a66 6f72 6d61 745f 6f75 7494 6807 5d94  .format_out.h.].
-000023b0: 6816 8c0a 666f 726d 6174 5f6f 7574 9485  h...format_out..
-000023c0: 9481 947d 9428 681b 6ac0 0300 0068 1c68  ...}.(h.j....h.h
-000023d0: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
-000023e0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-000023f0: 295d 9475 682b 6a3a 0200 0068 1b6a bc03  )].uh+j:...h.j..
-00002400: 0000 7562 6816 8c02 2028 9485 9481 947d  ..ubh... (.....}
-00002410: 9428 681b 6abc 0300 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
-00002420: 681e 4e75 626a 4f02 0000 2981 947d 9428  h.NubjO...)..}.(
-00002430: 6805 6806 6807 5d94 6a54 0200 0029 8194  h.h.h.].jT...)..
-00002440: 7d94 2868 058c 0673 7472 696e 6794 6807  }.(h...string.h.
-00002450: 5d94 6816 8c06 7374 7269 6e67 9485 9481  ].h...string....
-00002460: 947d 9428 681b 6ad5 0300 0068 1c68 0368  .}.(h.j....h.h.h
-00002470: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-00002480: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00002490: 9475 682b 6a53 0200 0068 1b6a d203 0000  .uh+jS...h.j....
-000024a0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-000024b0: 6825 5d94 6827 5d94 6829 5d94 8c09 7265  h%].h'].h)]...re
-000024c0: 6664 6f6d 6169 6e94 6a6a 0200 008c 0b72  fdomain.jj.....r
-000024d0: 6566 6578 706c 6963 6974 9489 8c07 7265  efexplicit....re
-000024e0: 6674 7970 6594 6af1 0100 008c 0972 6566  ftype.j......ref
-000024f0: 7461 7267 6574 946a d703 0000 6a6e 0200  target.j....jn..
-00002500: 0088 6a6f 0200 006a f001 0000 6a70 0200  ..jo...j....jp..
-00002510: 004e 7568 2b6a 4e02 0000 681b 6abc 0300  .Nuh+jN...h.j...
-00002520: 0075 6268 168c 0129 9485 9481 947d 9428  .ubh...).....}.(
-00002530: 681b 6abc 0300 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
-00002540: 4e75 6268 168c 0520 e280 9320 9485 9481  Nubh... ... ....
-00002550: 947d 9428 681b 6abc 0300 0068 1c68 0368  .}.(h.j....h.h.h
-00002560: 1d4e 681e 4e75 6268 168c 2e43 6f6e 7665  .Nh.Nubh...Conve
-00002570: 7273 696f 6e20 666f 726d 6174 2066 6f72  rsion format for
-00002580: 206f 7574 7075 7420 2864 6566 6175 6c74   output (default
-00002590: 2073 616d 6520 746f 2094 8594 8194 7d94   same to .....}.
-000025a0: 2868 1b6a bc03 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
-000025b0: 1e4e 7562 6809 8c06 7374 726f 6e67 9493  .Nubh...strong..
-000025c0: 9429 8194 7d94 2868 058c 0a2a 2a66 6f72  .)..}.(h...**for
-000025d0: 6d61 742a 2a94 6807 5d94 6816 8c06 666f  mat**.h.].h...fo
-000025e0: 726d 6174 9485 9481 947d 9428 681b 6afb  rmat.....}.(h.j.
-000025f0: 0300 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
-00002600: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00002610: 9468 275d 9468 295d 9475 682b 6af9 0300  .h'].h)].uh+j...
-00002620: 0068 1b6a bc03 0000 681c 6803 681d 4e68  .h.j....h.h.h.Nh
-00002630: 1e4e 7562 6816 8c02 292e 9485 9481 947d  .Nubh...)......}
-00002640: 9428 681b 6abc 0300 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
-00002650: 681e 4e75 6265 681f 7d94 2868 215d 9468  h.Nubeh.}.(h!].h
-00002660: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-00002670: 682b 6afc 0100 0068 1b6a b903 0000 7562  h+j....h.j....ub
-00002680: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-00002690: 5d94 6827 5d94 6829 5d94 7568 2b6a 3102  ].h'].h)].uh+j1.
-000026a0: 0000 681b 6a2e 0200 0075 6265 681f 7d94  ..h.j....ubeh.}.
-000026b0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
-000026c0: 9468 295d 9475 682b 6a2c 0200 0068 1b6a  .h)].uh+j,...h.j
-000026d0: 2902 0000 7562 6168 1f7d 9428 6821 5d94  )...ubah.}.(h!].
-000026e0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-000026f0: 7568 2b6a 2702 0000 681b 6a14 0200 0075  uh+j'...h.j....u
-00002700: 6265 681f 7d94 2868 215d 9468 235d 9468  beh.}.(h!].h#].h
-00002710: 255d 9468 275d 9468 295d 9475 682b 6a12  %].h'].h)].uh+j.
-00002720: 0200 0068 1b6a 0f02 0000 7562 6a13 0200  ...h.j....ubj...
-00002730: 0029 8194 7d94 2868 0568 0668 075d 9428  .)..}.(h.h.h.].(
-00002740: 6a18 0200 0029 8194 7d94 2868 058c 0b52  j....)..}.(h...R
-00002750: 6574 7572 6e20 7479 7065 9468 075d 9468  eturn type.h.].h
-00002760: 168c 0b52 6574 7572 6e20 7479 7065 9485  ...Return type..
-00002770: 9481 947d 9428 681b 6a2e 0400 0068 1c68  ...}.(h.j....h.h
-00002780: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
-00002790: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-000027a0: 295d 9475 682b 6a17 0200 0068 1b6a 2b04  )].uh+j....h.j+.
-000027b0: 0000 681d 687f 681e 4b00 7562 6a28 0200  ..h.h.h.K.ubj(..
-000027c0: 0029 8194 7d94 2868 0568 0668 075d 946a  .)..}.(h.h.h.].j
-000027d0: fd01 0000 2981 947d 9428 6805 8c25 6c69  ....)..}.(h..%li
-000027e0: 7374 206f 6620 7374 7269 6e67 2028 6f72  st of string (or
-000027f0: 2064 6174 6574 696d 652e 6461 7465 7469   datetime.dateti
-00002800: 6d65 2994 6807 5d94 286a 4f02 0000 2981  me).h.].(jO...).
-00002810: 947d 9428 6805 6806 6807 5d94 6816 8c04  .}.(h.h.h.].h...
-00002820: 6c69 7374 9485 9481 947d 9428 681b 6a43  list.....}.(h.jC
-00002830: 0400 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
-00002840: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00002850: 9468 275d 9468 295d 948c 0972 6566 646f  .h'].h)]...refdo
-00002860: 6d61 696e 946a 6a02 0000 8c0b 7265 6665  main.jj.....refe
-00002870: 7870 6c69 6369 7494 898c 0772 6566 7479  xplicit....refty
-00002880: 7065 946a f101 0000 8c09 7265 6674 6172  pe.j......reftar
-00002890: 6765 7494 8c04 6c69 7374 946a 6e02 0000  get...list.jn...
-000028a0: 886a 6f02 0000 6af0 0100 006a 7002 0000  .jo...j....jp...
-000028b0: 4e75 682b 6a4e 0200 0068 1b6a 3f04 0000  Nuh+jN...h.j?...
-000028c0: 7562 6816 8c04 206f 6620 9485 9481 947d  ubh... of .....}
-000028d0: 9428 681b 6a3f 0400 0068 1c68 0368 1d4e  .(h.j?...h.h.h.N
-000028e0: 681e 4e75 626a 4f02 0000 2981 947d 9428  h.NubjO...)..}.(
-000028f0: 6805 6806 6807 5d94 6816 8c06 7374 7269  h.h.h.].h...stri
-00002900: 6e67 9485 9481 947d 9428 681b 6a59 0400  ng.....}.(h.jY..
-00002910: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
-00002920: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-00002930: 275d 9468 295d 948c 0972 6566 646f 6d61  '].h)]...refdoma
-00002940: 696e 946a 6a02 0000 8c0b 7265 6665 7870  in.jj.....refexp
-00002950: 6c69 6369 7494 898c 0772 6566 7479 7065  licit....reftype
-00002960: 946a f101 0000 8c09 7265 6674 6172 6765  .j......reftarge
-00002970: 7494 8c06 7374 7269 6e67 946a 6e02 0000  t...string.jn...
-00002980: 886a 6f02 0000 6af0 0100 006a 7002 0000  .jo...j....jp...
-00002990: 4e75 682b 6a4e 0200 0068 1b6a 3f04 0000  Nuh+jN...h.j?...
-000029a0: 7562 6816 8c05 2028 6f72 2094 8594 8194  ubh... (or .....
-000029b0: 7d94 2868 1b6a 3f04 0000 681c 6803 681d  }.(h.j?...h.h.h.
-000029c0: 4e68 1e4e 7562 6a4f 0200 0029 8194 7d94  Nh.NubjO...)..}.
-000029d0: 2868 0568 0668 075d 9468 168c 1164 6174  (h.h.h.].h...dat
-000029e0: 6574 696d 652e 6461 7465 7469 6d65 9485  etime.datetime..
-000029f0: 9481 947d 9428 681b 6a6f 0400 0068 1c68  ...}.(h.jo...h.h
-00002a00: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
-00002a10: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00002a20: 295d 948c 0972 6566 646f 6d61 696e 946a  )]...refdomain.j
-00002a30: 6a02 0000 8c0b 7265 6665 7870 6c69 6369  j.....refexplici
-00002a40: 7494 898c 0772 6566 7479 7065 946a f101  t....reftype.j..
-00002a50: 0000 8c09 7265 6674 6172 6765 7494 8c11  ....reftarget...
-00002a60: 6461 7465 7469 6d65 2e64 6174 6574 696d  datetime.datetim
-00002a70: 6594 6a6e 0200 0088 6a6f 0200 006a f001  e.jn....jo...j..
-00002a80: 0000 6a70 0200 004e 7568 2b6a 4e02 0000  ..jp...Nuh+jN...
-00002a90: 681b 6a3f 0400 0075 6268 168c 0129 9485  h.j?...ubh...)..
-00002aa0: 9481 947d 9428 681b 6a3f 0400 0068 1c68  ...}.(h.j?...h.h
-00002ab0: 0368 1d4e 681e 4e75 6265 681f 7d94 2868  .h.Nh.Nubeh.}.(h
-00002ac0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00002ad0: 295d 9475 682b 6afc 0100 0068 1b6a 3c04  )].uh+j....h.j<.
-00002ae0: 0000 7562 6168 1f7d 9428 6821 5d94 6823  ..ubah.}.(h!].h#
-00002af0: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
-00002b00: 2b6a 2702 0000 681b 6a2b 0400 0075 6265  +j'...h.j+...ube
-00002b10: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00002b20: 9468 275d 9468 295d 9475 682b 6a12 0200  .h'].h)].uh+j...
-00002b30: 0068 1b6a 0f02 0000 7562 6568 1f7d 9428  .h.j....ubeh.}.(
-00002b40: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-00002b50: 6829 5d94 7568 2b6a 0d02 0000 681b 6af9  h)].uh+j....h.j.
-00002b60: 0100 0068 1c68 0368 1d4e 681e 4e75 6265  ...h.h.h.Nh.Nube
-00002b70: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00002b80: 9468 275d 9468 295d 9475 682b 6af7 0100  .h'].h)].uh+j...
-00002b90: 0068 1b68 6268 1c68 0368 1d68 7f68 1e4b  .h.hbh.h.h.h.h.K
-00002ba0: 0175 6265 681f 7d94 2868 215d 9468 235d  .ubeh.}.(h!].h#]
-00002bb0: 9428 6a6a 0200 008c 0866 756e 6374 696f  .(jj.....functio
-00002bc0: 6e94 6568 255d 9468 275d 9468 295d 948c  n.eh%].h'].h)]..
-00002bd0: 0664 6f6d 6169 6e94 6a6a 0200 008c 076f  .domain.jj.....o
-00002be0: 626a 7479 7065 946a a604 0000 8c08 6465  bjtype.j......de
-00002bf0: 7363 7479 7065 946a a604 0000 8c07 6e6f  sctype.j......no
-00002c00: 696e 6465 7894 898c 0c6e 6f69 6e64 6578  index....noindex
-00002c10: 656e 7472 7994 898c 0f6e 6f63 6f6e 7465  entry....noconte
-00002c20: 6e74 7365 6e74 7279 9489 7568 2b68 6068  ntsentry..uh+h`h
-00002c30: 1c68 0368 1b68 3e68 1d4e 681e 4e75 626a  .h.h.h>h.Nh.Nubj
-00002c40: fd01 0000 2981 947d 9428 6805 8c0b 2a2a  ....)..}.(h...**
-00002c50: 4578 616d 706c 652a 2a94 6807 5d94 6afa  Example**.h.].j.
-00002c60: 0300 0029 8194 7d94 2868 056a b204 0000  ...)..}.(h.j....
-00002c70: 6807 5d94 6816 8c07 4578 616d 706c 6594  h.].h...Example.
-00002c80: 8594 8194 7d94 2868 1b6a b404 0000 681c  ....}.(h.j....h.
-00002c90: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
-00002ca0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-00002cb0: 6829 5d94 7568 2b6a f903 0000 681b 6ab0  h)].uh+j....h.j.
-00002cc0: 0400 0075 6261 681f 7d94 2868 215d 9468  ...ubah.}.(h!].h
-00002cd0: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-00002ce0: 682b 6afc 0100 0068 1d68 2c68 1e4b 0c68  h+j....h.h,h.K.h
-00002cf0: 1b68 3e68 1c68 0375 6268 098c 0d6c 6974  .h>h.h.ubh...lit
-00002d00: 6572 616c 5f62 6c6f 636b 9493 9429 8194  eral_block...)..
-00002d10: 7d94 2868 058c f969 6d70 6f72 7420 636f  }.(h...import co
-00002d20: 6f6b 6965 735f 7574 696c 6974 6965 7320  okies_utilities 
-00002d30: 6173 2063 750a 6461 7465 7320 3d20 6375  as cu.dates = cu
-00002d40: 2e67 6574 5f64 6174 6573 280a 2020 2020  .get_dates(.    
-00002d50: 7374 6172 743d 2732 3031 362d 3037 2d30  start='2016-07-0
-00002d60: 3120 3032 3a30 303a 3030 272c 0a20 2020  1 02:00:00',.   
-00002d70: 2065 6e64 3d27 3230 3136 2d30 372d 3032   end='2016-07-02
-00002d80: 2030 313a 3030 3a30 3027 2c0a 2020 2020   01:00:00',.    
-00002d90: 666f 726d 6174 3d27 2559 2d25 6d2d 2564  format='%Y-%m-%d
-00002da0: 2025 483a 254d 3a25 5327 2c0a 2020 2020   %H:%M:%S',.    
-00002db0: 6465 6c74 613d 7b27 686f 7572 7327 3a20  delta={'hours': 
-00002dc0: 317d 290a 2320 5b27 3230 3136 2d30 372d  1}).# ['2016-07-
-00002dd0: 3031 2030 323a 3030 3a30 3027 2c20 2732  01 02:00:00', '2
-00002de0: 3031 362d 3037 2d30 3120 3033 3a30 303a  016-07-01 03:00:
-00002df0: 3030 272c 202e 2e2e 2c20 2732 3031 362d  00', ..., '2016-
-00002e00: 3037 2d30 3220 3031 3a30 303a 3030 275d  07-02 01:00:00']
-00002e10: 9468 075d 9468 168c f969 6d70 6f72 7420  .h.].h...import 
-00002e20: 636f 6f6b 6965 735f 7574 696c 6974 6965  cookies_utilitie
-00002e30: 7320 6173 2063 750a 6461 7465 7320 3d20  s as cu.dates = 
-00002e40: 6375 2e67 6574 5f64 6174 6573 280a 2020  cu.get_dates(.  
-00002e50: 2020 7374 6172 743d 2732 3031 362d 3037    start='2016-07
-00002e60: 2d30 3120 3032 3a30 303a 3030 272c 0a20  -01 02:00:00',. 
-00002e70: 2020 2065 6e64 3d27 3230 3136 2d30 372d     end='2016-07-
-00002e80: 3032 2030 313a 3030 3a30 3027 2c0a 2020  02 01:00:00',.  
-00002e90: 2020 666f 726d 6174 3d27 2559 2d25 6d2d    format='%Y-%m-
-00002ea0: 2564 2025 483a 254d 3a25 5327 2c0a 2020  %d %H:%M:%S',.  
-00002eb0: 2020 6465 6c74 613d 7b27 686f 7572 7327    delta={'hours'
-00002ec0: 3a20 317d 290a 2320 5b27 3230 3136 2d30  : 1}).# ['2016-0
-00002ed0: 372d 3031 2030 323a 3030 3a30 3027 2c20  7-01 02:00:00', 
-00002ee0: 2732 3031 362d 3037 2d30 3120 3033 3a30  '2016-07-01 03:0
-00002ef0: 303a 3030 272c 202e 2e2e 2c20 2732 3031  0:00', ..., '201
-00002f00: 362d 3037 2d30 3220 3031 3a30 303a 3030  6-07-02 01:00:00
-00002f10: 275d 9485 9481 947d 9468 1b6a c904 0000  '].....}.h.j....
-00002f20: 7362 6168 1f7d 9428 6821 5d94 6823 5d94  sbah.}.(h!].h#].
-00002f30: 6825 5d94 6827 5d94 6829 5d94 687d 687e  h%].h'].h)].h}h~
-00002f40: 8c05 666f 7263 6594 898c 086c 616e 6775  ..force....langu
-00002f50: 6167 6594 8c06 7079 7468 6f6e 948c 0e68  age...python...h
-00002f60: 6967 686c 6967 6874 5f61 7267 7394 7d94  ighlight_args.}.
-00002f70: 7568 2b6a c704 0000 681d 682c 681e 4b0e  uh+j....h.h,h.K.
-00002f80: 681b 683e 681c 6803 7562 6568 1f7d 9428  h.h>h.h.ubeh.}.(
-00002f90: 6821 5d94 8c1b 636f 6f6b 6965 732d 7574  h!]...cookies-ut
-00002fa0: 696c 6974 6965 732d 6765 742d 6461 7465  ilities-get-date
-00002fb0: 7394 6168 235d 9468 255d 948c 1b63 6f6f  s.ah#].h%]...coo
-00002fc0: 6b69 6573 5f75 7469 6c69 7469 6573 2e67  kies_utilities.g
-00002fd0: 6574 5f64 6174 6573 9461 6827 5d94 6829  et_dates.ah'].h)
-00002fe0: 5d94 7568 2b68 0a68 1b68 2d68 1c68 0368  ].uh+h.h.h-h.h.h
-00002ff0: 1d68 2c68 1e4b 0875 6265 681f 7d94 2868  .h,h.K.ubeh.}.(h
-00003000: 215d 948c 0966 756e 6374 696f 6e73 9461  !]...functions.a
-00003010: 6823 5d94 6825 5d94 8c09 6675 6e63 7469  h#].h%]...functi
-00003020: 6f6e 7394 6168 275d 9468 295d 9475 682b  ons.ah'].h)].uh+
-00003030: 680a 681b 680c 681c 6803 681d 682c 681e  h.h.h.h.h.h.h,h.
-00003040: 4b05 7562 680b 2981 947d 9428 6805 6806  K.ubh.)..}.(h.h.
-00003050: 6807 5d94 2868 1029 8194 7d94 2868 058c  h.].(h.)..}.(h..
-00003060: 0743 6c61 7373 6573 9468 075d 9468 168c  .Classes.h.].h..
-00003070: 0743 6c61 7373 6573 9485 9481 947d 9428  .Classes.....}.(
-00003080: 681b 6aef 0400 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
-00003090: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
-000030a0: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
-000030b0: 680f 681b 6aec 0400 0068 1c68 0368 1d68  h.h.j....h.h.h.h
-000030c0: 2c68 1e4b 1975 6268 0b29 8194 7d94 2868  ,h.K.ubh.)..}.(h
-000030d0: 0568 0668 075d 9428 6810 2981 947d 9428  .h.h.].(h.)..}.(
-000030e0: 6805 8c1b 636f 6f6b 6965 735f 7574 696c  h...cookies_util
-000030f0: 6974 6965 732e 5374 6f70 7761 7463 6894  ities.Stopwatch.
-00003100: 6807 5d94 6816 8c1b 636f 6f6b 6965 735f  h.].h...cookies_
-00003110: 7574 696c 6974 6965 732e 5374 6f70 7761  utilities.Stopwa
-00003120: 7463 6894 8594 8194 7d94 2868 1b6a 0005  tch.....}.(h.j..
-00003130: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
-00003140: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-00003150: 6827 5d94 6829 5d94 7568 2b68 0f68 1b6a  h'].h)].uh+h.h.j
-00003160: fd04 0000 681c 6803 681d 682c 681e 4b1c  ....h.h.h.h,h.K.
-00003170: 7562 6850 2981 947d 9428 6805 6806 6807  ubhP)..}.(h.h.h.
-00003180: 5d94 681f 7d94 2868 215d 9468 235d 9468  ].h.}.(h!].h#].h
-00003190: 255d 9468 275d 9468 295d 948c 0765 6e74  %].h'].h)]...ent
-000031a0: 7269 6573 945d 9428 685c 8c26 5374 6f70  ries.].(h\.&Stop
-000031b0: 7761 7463 6820 2863 6c61 7373 2069 6e20  watch (class in 
-000031c0: 636f 6f6b 6965 735f 7574 696c 6974 6965  cookies_utilitie
-000031d0: 7329 948c 1b63 6f6f 6b69 6573 5f75 7469  s)...cookies_uti
-000031e0: 6c69 7469 6573 2e53 746f 7077 6174 6368  lities.Stopwatch
-000031f0: 9468 064e 7494 6175 682b 684f 681b 6afd  .h.Nt.auh+hOh.j.
-00003200: 0400 0068 1c68 0368 1d4e 681e 4e75 6268  ...h.h.h.Nh.Nubh
-00003210: 6129 8194 7d94 2868 0568 0668 075d 9428  a)..}.(h.h.h.].(
-00003220: 6866 2981 947d 9428 6805 8c0b 5374 6f70  hf)..}.(h...Stop
-00003230: 7761 7463 6828 2994 6807 5d94 2868 008c  watch().h.].(h..
-00003240: 0f64 6573 635f 616e 6e6f 7461 7469 6f6e  .desc_annotation
-00003250: 9493 9429 8194 7d94 2868 058c 325b 3c23  ...)..}.(h..2[<#
-00003260: 7465 7874 3a20 2763 6c61 7373 273e 2c20  text: 'class'>, 
-00003270: 3c64 6573 635f 7369 675f 7370 6163 653a  <desc_sig_space:
-00003280: 203c 2374 6578 743a 2027 2027 3e3e 5d94   <#text: ' '>>].
-00003290: 6807 5d94 2868 168c 0563 6c61 7373 9485  h.].(h...class..
-000032a0: 9481 947d 9428 681b 6a25 0500 0068 1c68  ...}.(h.j%...h.h
-000032b0: 0368 1d4e 681e 4e75 6268 008c 0e64 6573  .h.Nh.Nubh...des
-000032c0: 635f 7369 675f 7370 6163 6594 9394 2981  c_sig_space...).
-000032d0: 947d 9428 6805 8c01 2094 6807 5d94 6816  .}.(h... .h.].h.
-000032e0: 8c01 2094 8594 8194 7d94 2868 1b6a 2f05  .. .....}.(h.j/.
-000032f0: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
-00003300: 1f7d 9428 6821 5d94 6823 5d94 8c01 7794  .}.(h!].h#]...w.
-00003310: 6168 255d 9468 275d 9468 295d 9475 682b  ah%].h'].h)].uh+
-00003320: 6a2d 0500 0068 1b6a 2505 0000 7562 6568  j-...h.j%...ubeh
-00003330: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-00003340: 6827 5d94 6829 5d94 687d 687e 7568 2b6a  h'].h)].h}h~uh+j
-00003350: 2305 0000 681b 6a1f 0500 0068 1c68 0368  #...h.j....h.h.h
-00003360: 1d8c 7c43 3a5c 5573 6572 735c 632d 6d69  ..|C:\Users\c-mi
-00003370: 685c 7370 6163 655c 636f 6f6b 6965 735f  h\space\cookies_
-00003380: 7574 696c 6974 6965 735c 7372 635c 636f  utilities\src\co
-00003390: 6f6b 6965 735f 7574 696c 6974 6965 735c  okies_utilities\
-000033a0: 7374 6f70 7761 7463 682e 7079 3a64 6f63  stopwatch.py:doc
-000033b0: 7374 7269 6e67 206f 6620 636f 6f6b 6965  string of cookie
-000033c0: 735f 7574 696c 6974 6965 732e 7374 6f70  s_utilities.stop
-000033d0: 7761 7463 682e 5374 6f70 7761 7463 6894  watch.Stopwatch.
-000033e0: 681e 4b01 7562 686c 2981 947d 9428 6805  h.K.ubhl)..}.(h.
-000033f0: 8c12 636f 6f6b 6965 735f 7574 696c 6974  ..cookies_utilit
-00003400: 6965 732e 9468 075d 9468 168c 1263 6f6f  ies..h.].h...coo
-00003410: 6b69 6573 5f75 7469 6c69 7469 6573 2e94  kies_utilities..
-00003420: 8594 8194 7d94 2868 1b6a 4505 0000 681c  ....}.(h.jE...h.
-00003430: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
-00003440: 6821 5d94 6823 5d94 2868 7868 7965 6825  h!].h#].(hxhyeh%
-00003450: 5d94 6827 5d94 6829 5d94 687d 687e 7568  ].h'].h)].h}h~uh
-00003460: 2b68 6b68 1b6a 1f05 0000 681c 6803 681d  +hkh.j....h.h.h.
-00003470: 6a44 0500 0068 1e4b 0175 6268 8129 8194  jD...h.K.ubh.)..
-00003480: 7d94 2868 058c 0953 746f 7077 6174 6368  }.(h...Stopwatch
-00003490: 9468 075d 9468 168c 0953 746f 7077 6174  .h.].h...Stopwat
-000034a0: 6368 9485 9481 947d 9428 681b 6a53 0500  ch.....}.(h.jS..
-000034b0: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
-000034c0: 7d94 2868 215d 9468 235d 9428 688d 688e  }.(h!].h#].(h.h.
-000034d0: 6568 255d 9468 275d 9468 295d 9468 7d68  eh%].h'].h)].h}h
-000034e0: 7e75 682b 6880 681b 6a1f 0500 0068 1c68  ~uh+h.h.j....h.h
-000034f0: 0368 1d6a 4405 0000 681e 4b01 7562 6568  .h.jD...h.K.ubeh
-00003500: 1f7d 9428 6821 5d94 6a1a 0500 0061 6823  .}.(h!].j....ah#
-00003510: 5d94 286a ea01 0000 6aeb 0100 0065 6825  ].(j....j....eh%
-00003520: 5d94 6827 5d94 6829 5d94 6aef 0100 008c  ].h'].h)].j.....
-00003530: 1163 6f6f 6b69 6573 5f75 7469 6c69 7469  .cookies_utiliti
-00003540: 6573 946a f101 0000 6806 6af2 0100 006a  es.j....h.j....j
-00003550: 5505 0000 6af3 0100 006a 6705 0000 6a55  U...j....jg...jU
-00003560: 0500 0086 946a f501 0000 6a55 0500 0075  .....j....jU...u
-00003570: 682b 6865 681d 6a44 0500 0068 1e4b 0168  h+heh.jD...h.K.h
-00003580: 1b6a 1c05 0000 681c 6803 7562 6af8 0100  .j....h.h.ubj...
-00003590: 0029 8194 7d94 2868 0568 0668 075d 9428  .)..}.(h.h.h.].(
-000035a0: 6afd 0100 0029 8194 7d94 2868 058c 2853  j....)..}.(h..(S
-000035b0: 746f 7077 6174 6368 2066 6f72 206d 6561  topwatch for mea
-000035c0: 7375 7269 6e67 2070 726f 6365 7373 696e  suring processin
-000035d0: 6720 7469 6d65 2e94 6807 5d94 6816 8c28  g time..h.].h..(
-000035e0: 5374 6f70 7761 7463 6820 666f 7220 6d65  Stopwatch for me
-000035f0: 6173 7572 696e 6720 7072 6f63 6573 7369  asuring processi
-00003600: 6e67 2074 696d 652e 9485 9481 947d 9428  ng time......}.(
-00003610: 681b 6a6c 0500 0068 1c68 0368 1d4e 681e  h.jl...h.h.h.Nh.
-00003620: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
-00003630: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
-00003640: 6afc 0100 0068 1d8c 7c43 3a5c 5573 6572  j....h..|C:\User
-00003650: 735c 632d 6d69 685c 7370 6163 655c 636f  s\c-mih\space\co
-00003660: 6f6b 6965 735f 7574 696c 6974 6965 735c  okies_utilities\
-00003670: 7372 635c 636f 6f6b 6965 735f 7574 696c  src\cookies_util
-00003680: 6974 6965 735c 7374 6f70 7761 7463 682e  ities\stopwatch.
-00003690: 7079 3a64 6f63 7374 7269 6e67 206f 6620  py:docstring of 
-000036a0: 636f 6f6b 6965 735f 7574 696c 6974 6965  cookies_utilitie
-000036b0: 732e 7374 6f70 7761 7463 682e 5374 6f70  s.stopwatch.Stop
-000036c0: 7761 7463 6894 681e 4b01 681b 6a69 0500  watch.h.K.h.ji..
-000036d0: 0068 1c68 0375 6268 5029 8194 7d94 2868  .h.h.ubhP)..}.(h
-000036e0: 0568 0668 075d 9468 1f7d 9428 6821 5d94  .h.h.].h.}.(h!].
-000036f0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-00003700: 8c07 656e 7472 6965 7394 5d94 2868 5c8c  ..entries.].(h\.
-00003710: 2c70 7265 7373 2829 2028 636f 6f6b 6965  ,press() (cookie
-00003720: 735f 7574 696c 6974 6965 732e 5374 6f70  s_utilities.Stop
-00003730: 7761 7463 6820 6d65 7468 6f64 2994 8c21  watch method)..!
-00003740: 636f 6f6b 6965 735f 7574 696c 6974 6965  cookies_utilitie
-00003750: 732e 5374 6f70 7761 7463 682e 7072 6573  s.Stopwatch.pres
-00003760: 7394 6806 4e74 9461 7568 2b68 4f68 1b6a  s.h.Nt.auh+hOh.j
-00003770: 6905 0000 681c 6803 681d 4e68 1e4e 7562  i...h.h.h.Nh.Nub
-00003780: 6861 2981 947d 9428 6805 6806 6807 5d94  ha)..}.(h.h.h.].
-00003790: 2868 6629 8194 7d94 2868 058c 1753 746f  (hf)..}.(h...Sto
-000037a0: 7077 6174 6368 2e70 7265 7373 286b 6579  pwatch.press(key
-000037b0: 3d27 2729 9468 075d 9428 6881 2981 947d  ='').h.].(h.)..}
-000037c0: 9428 6805 8c05 7072 6573 7394 6807 5d94  .(h...press.h.].
-000037d0: 6816 8c05 7072 6573 7394 8594 8194 7d94  h...press.....}.
-000037e0: 2868 1b6a 9005 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
-000037f0: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
-00003800: 5d94 2868 8d68 8e65 6825 5d94 6827 5d94  ].(h.h.eh%].h'].
-00003810: 6829 5d94 687d 687e 7568 2b68 8068 1b6a  h)].h}h~uh+h.h.j
-00003820: 8c05 0000 681c 6803 681d 8c82 433a 5c55  ....h.h.h...C:\U
-00003830: 7365 7273 5c63 2d6d 6968 5c73 7061 6365  sers\c-mih\space
-00003840: 5c63 6f6f 6b69 6573 5f75 7469 6c69 7469  \cookies_utiliti
-00003850: 6573 5c73 7263 5c63 6f6f 6b69 6573 5f75  es\src\cookies_u
-00003860: 7469 6c69 7469 6573 5c73 746f 7077 6174  tilities\stopwat
-00003870: 6368 2e70 793a 646f 6373 7472 696e 6720  ch.py:docstring 
-00003880: 6f66 2063 6f6f 6b69 6573 5f75 7469 6c69  of cookies_utili
-00003890: 7469 6573 2e73 746f 7077 6174 6368 2e53  ties.stopwatch.S
-000038a0: 746f 7077 6174 6368 2e70 7265 7373 9468  topwatch.press.h
-000038b0: 1e4b 0175 6268 9329 8194 7d94 2868 058c  .K.ubh.)..}.(h..
-000038c0: 066b 6579 3d27 2794 6807 5d94 6899 2981  .key=''.h.].h.).
-000038d0: 947d 9428 6805 8c06 6b65 793d 2727 9468  .}.(h...key=''.h
-000038e0: 075d 9428 689f 2981 947d 9428 6805 8c03  .].(h.)..}.(h...
-000038f0: 6b65 7994 6807 5d94 6816 8c03 6b65 7994  key.h.].h...key.
-00003900: 8594 8194 7d94 2868 1b6a a705 0000 681c  ....}.(h.j....h.
-00003910: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
-00003920: 6821 5d94 6823 5d94 68ab 6168 255d 9468  h!].h#].h.ah%].h
-00003930: 275d 9468 295d 9475 682b 689e 681b 6aa3  '].h)].uh+h.h.j.
-00003940: 0500 0075 6268 b029 8194 7d94 2868 058c  ...ubh.)..}.(h..
-00003950: 013d 9468 075d 9468 168c 013d 9485 9481  .=.h.].h...=....
-00003960: 947d 9428 681b 6ab5 0500 0068 1c68 0368  .}.(h.j....h.h.h
-00003970: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-00003980: 9468 235d 9468 bc61 6825 5d94 6827 5d94  .h#].h.ah%].h'].
-00003990: 6829 5d94 7568 2b68 af68 1b6a a305 0000  h)].uh+h.h.j....
-000039a0: 7562 68c1 2981 947d 9428 6805 8c02 2727  ubh.)..}.(h...''
-000039b0: 9468 075d 9468 168c 0227 2794 8594 8194  .h.].h...''.....
-000039c0: 7d94 2868 1b6a c305 0000 681c 6803 681d  }.(h.j....h.h.h.
-000039d0: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
-000039e0: 6823 5d94 68cd 6168 255d 9468 275d 9468  h#].h.ah%].h'].h
-000039f0: 295d 948c 1373 7570 706f 7274 5f73 6d61  )]...support_sma
-00003a00: 7274 7175 6f74 6573 9489 7568 2b68 c068  rtquotes..uh+h.h
-00003a10: 1b6a a305 0000 7562 6568 1f7d 9428 6821  .j....ubeh.}.(h!
-00003a20: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00003a30: 5d94 687d 687e 7568 2b68 9868 1b6a 9f05  ].h}h~uh+h.h.j..
-00003a40: 0000 7562 6168 1f7d 9428 6821 5d94 6823  ..ubah.}.(h!].h#
-00003a50: 5d94 6825 5d94 6827 5d94 6829 5d94 687d  ].h%].h'].h)].h}
-00003a60: 687e 7568 2b68 9268 1b6a 8c05 0000 681c  h~uh+h.h.j....h.
-00003a70: 6803 681d 6a9e 0500 0068 1e4b 0175 6265  h.h.j....h.K.ube
-00003a80: 681f 7d94 2868 215d 946a 8705 0000 6168  h.}.(h!].j....ah
-00003a90: 235d 9428 6aea 0100 006a eb01 0000 6568  #].(j....j....eh
-00003aa0: 255d 9468 275d 9468 295d 946a ef01 0000  %].h'].h)].j....
-00003ab0: 8c11 636f 6f6b 6965 735f 7574 696c 6974  ..cookies_utilit
-00003ac0: 6965 7394 6af1 0100 006a 5505 0000 6af2  ies.j....jU...j.
-00003ad0: 0100 008c 0f53 746f 7077 6174 6368 2e70  .....Stopwatch.p
-00003ae0: 7265 7373 946a f301 0000 6ae4 0500 008c  ress.j....j.....
-00003af0: 0953 746f 7077 6174 6368 948c 0570 7265  .Stopwatch...pre
-00003b00: 7373 9487 946a f501 0000 8c11 5374 6f70  ss...j......Stop
-00003b10: 7761 7463 682e 7072 6573 7328 2994 7568  watch.press().uh
-00003b20: 2b68 6568 1d6a 9e05 0000 681e 4b01 681b  +heh.j....h.K.h.
-00003b30: 6a89 0500 0068 1c68 0375 626a f801 0000  j....h.h.ubj....
-00003b40: 2981 947d 9428 6805 6806 6807 5d94 286a  )..}.(h.h.h.].(j
-00003b50: fd01 0000 2981 947d 9428 6805 8c14 5072  ....)..}.(h...Pr
-00003b60: 6573 7320 7468 6520 7374 6f70 7761 7463  ess the stopwatc
-00003b70: 682e 9468 075d 9468 168c 1450 7265 7373  h..h.].h...Press
-00003b80: 2074 6865 2073 746f 7077 6174 6368 2e94   the stopwatch..
-00003b90: 8594 8194 7d94 2868 1b6a ed05 0000 681c  ....}.(h.j....h.
-00003ba0: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
-00003bb0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-00003bc0: 6829 5d94 7568 2b6a fc01 0000 681d 8c82  h)].uh+j....h...
-00003bd0: 433a 5c55 7365 7273 5c63 2d6d 6968 5c73  C:\Users\c-mih\s
-00003be0: 7061 6365 5c63 6f6f 6b69 6573 5f75 7469  pace\cookies_uti
-00003bf0: 6c69 7469 6573 5c73 7263 5c63 6f6f 6b69  lities\src\cooki
-00003c00: 6573 5f75 7469 6c69 7469 6573 5c73 746f  es_utilities\sto
-00003c10: 7077 6174 6368 2e70 793a 646f 6373 7472  pwatch.py:docstr
-00003c20: 696e 6720 6f66 2063 6f6f 6b69 6573 5f75  ing of cookies_u
-00003c30: 7469 6c69 7469 6573 2e73 746f 7077 6174  tilities.stopwat
-00003c40: 6368 2e53 746f 7077 6174 6368 2e70 7265  ch.Stopwatch.pre
-00003c50: 7373 9468 1e4b 0168 1b6a ea05 0000 681c  ss.h.K.h.j....h.
-00003c60: 6803 7562 6a0e 0200 0029 8194 7d94 2868  h.ubj....)..}.(h
-00003c70: 0568 0668 075d 946a 1302 0000 2981 947d  .h.h.].j....)..}
-00003c80: 9428 6805 6806 6807 5d94 286a 1802 0000  .(h.h.h.].(j....
-00003c90: 2981 947d 9428 6805 8c0a 5061 7261 6d65  )..}.(h...Parame
-00003ca0: 7465 7273 9468 075d 9468 168c 0a50 6172  ters.h.].h...Par
-00003cb0: 616d 6574 6572 7394 8594 8194 7d94 2868  ameters.....}.(h
-00003cc0: 1b6a 0206 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
-00003cd0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-00003ce0: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
-00003cf0: 1702 0000 681b 6aff 0500 0068 1d6a 9e05  ....h.j....h.j..
-00003d00: 0000 681e 4b00 7562 6a28 0200 0029 8194  ..h.K.ubj(...)..
-00003d10: 7d94 2868 0568 0668 075d 946a fd01 0000  }.(h.h.h.].j....
-00003d20: 2981 947d 9428 6805 8c38 6b65 7920 2873  )..}.(h..8key (s
-00003d30: 7472 696e 6729 202d 2d20 5468 6520 6964  tring) -- The id
-00003d40: 656e 6669 6361 746f 7220 666f 7220 7468  enficator for th
-00003d50: 6520 7469 6d65 2028 6f70 7469 6f6e 616c  e time (optional
-00003d60: 292e 9468 075d 9428 6a3b 0200 0029 8194  )..h.].(j;...)..
-00003d70: 7d94 2868 058c 036b 6579 9468 075d 9468  }.(h...key.h.].h
-00003d80: 168c 036b 6579 9485 9481 947d 9428 681b  ...key.....}.(h.
-00003d90: 6a17 0600 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
-00003da0: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-00003db0: 255d 9468 275d 9468 295d 9475 682b 6a3a  %].h'].h)].uh+j:
-00003dc0: 0200 0068 1b6a 1306 0000 7562 6816 8c02  ...h.j....ubh...
-00003dd0: 2028 9485 9481 947d 9428 681b 6a13 0600   (.....}.(h.j...
-00003de0: 0068 1c68 0368 1d4e 681e 4e75 626a 4f02  .h.h.h.Nh.NubjO.
-00003df0: 0000 2981 947d 9428 6805 6806 6807 5d94  ..)..}.(h.h.h.].
-00003e00: 6a54 0200 0029 8194 7d94 2868 058c 0673  jT...)..}.(h...s
-00003e10: 7472 696e 6794 6807 5d94 6816 8c06 7374  tring.h.].h...st
-00003e20: 7269 6e67 9485 9481 947d 9428 681b 6a2c  ring.....}.(h.j,
-00003e30: 0600 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
-00003e40: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00003e50: 9468 275d 9468 295d 9475 682b 6a53 0200  .h'].h)].uh+jS..
-00003e60: 0068 1b6a 2906 0000 7562 6168 1f7d 9428  .h.j)...ubah.}.(
-00003e70: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-00003e80: 6829 5d94 8c09 7265 6664 6f6d 6169 6e94  h)]...refdomain.
-00003e90: 8c02 7079 948c 0b72 6566 6578 706c 6963  ..py...refexplic
-00003ea0: 6974 9489 8c07 7265 6674 7970 6594 6af1  it....reftype.j.
-00003eb0: 0100 008c 0972 6566 7461 7267 6574 946a  .....reftarget.j
-00003ec0: 2e06 0000 6a6e 0200 0088 6a6f 0200 006a  ....jn....jo...j
-00003ed0: e405 0000 6a70 0200 006a 5505 0000 7568  ....jp...jU...uh
-00003ee0: 2b6a 4e02 0000 681b 6a13 0600 0075 6268  +jN...h.j....ubh
-00003ef0: 168c 0129 9485 9481 947d 9428 681b 6a13  ...).....}.(h.j.
-00003f00: 0600 0068 1c68 0368 1d4e 681e 4e75 6268  ...h.h.h.Nh.Nubh
-00003f10: 168c 0520 e280 9320 9485 9481 947d 9428  ... ... .....}.(
-00003f20: 681b 6a13 0600 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
-00003f30: 4e75 6268 168c 2854 6865 2069 6465 6e66  Nubh..(The idenf
-00003f40: 6963 6174 6f72 2066 6f72 2074 6865 2074  icator for the t
-00003f50: 696d 6520 286f 7074 696f 6e61 6c29 2e94  ime (optional)..
-00003f60: 8594 8194 7d94 2868 1b6a 1306 0000 681c  ....}.(h.j....h.
-00003f70: 6803 681d 4e68 1e4e 7562 6568 1f7d 9428  h.h.Nh.Nubeh.}.(
-00003f80: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-00003f90: 6829 5d94 7568 2b6a fc01 0000 681b 6a10  h)].uh+j....h.j.
-00003fa0: 0600 0075 6261 681f 7d94 2868 215d 9468  ...ubah.}.(h!].h
-00003fb0: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-00003fc0: 682b 6a27 0200 0068 1b6a ff05 0000 7562  h+j'...h.j....ub
-00003fd0: 6568 1f7d 9428 6821 5d94 6823 5d94 6825  eh.}.(h!].h#].h%
-00003fe0: 5d94 6827 5d94 6829 5d94 7568 2b6a 1202  ].h'].h)].uh+j..
-00003ff0: 0000 681b 6afc 0500 0075 6261 681f 7d94  ..h.j....ubah.}.
-00004000: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
-00004010: 9468 295d 9475 682b 6a0d 0200 0068 1b6a  .h)].uh+j....h.j
-00004020: ea05 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
-00004030: 6568 1f7d 9428 6821 5d94 6823 5d94 6825  eh.}.(h!].h#].h%
-00004040: 5d94 6827 5d94 6829 5d94 7568 2b6a f701  ].h'].h)].uh+j..
-00004050: 0000 681b 6a89 0500 0068 1c68 0368 1d6a  ..h.j....h.h.h.j
-00004060: 9e05 0000 681e 4b01 7562 6568 1f7d 9428  ....h.K.ubeh.}.(
-00004070: 6821 5d94 6823 5d94 286a 4106 0000 8c06  h!].h#].(jA.....
-00004080: 6d65 7468 6f64 9465 6825 5d94 6827 5d94  method.eh%].h'].
-00004090: 6829 5d94 6aaa 0400 006a 4106 0000 6aab  h)].j....jA...j.
-000040a0: 0400 006a 7206 0000 6aac 0400 006a 7206  ...jr...j....jr.
-000040b0: 0000 6aad 0400 0089 6aae 0400 0089 6aaf  ..j.....j.....j.
-000040c0: 0400 0089 7568 2b68 6068 1c68 0368 1b6a  ....uh+h`h.h.h.j
-000040d0: 6905 0000 681d 4e68 1e4e 7562 6850 2981  i...h.Nh.NubhP).
-000040e0: 947d 9428 6805 6806 6807 5d94 681f 7d94  .}.(h.h.h.].h.}.
-000040f0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
-00004100: 9468 295d 948c 0765 6e74 7269 6573 945d  .h)]...entries.]
-00004110: 9428 685c 8c2b 7368 6f77 2829 2028 636f  .(h\.+show() (co
-00004120: 6f6b 6965 735f 7574 696c 6974 6965 732e  okies_utilities.
-00004130: 5374 6f70 7761 7463 6820 6d65 7468 6f64  Stopwatch method
-00004140: 2994 8c20 636f 6f6b 6965 735f 7574 696c  ).. cookies_util
-00004150: 6974 6965 732e 5374 6f70 7761 7463 682e  ities.Stopwatch.
-00004160: 7368 6f77 9468 064e 7494 6175 682b 684f  show.h.Nt.auh+hO
-00004170: 681b 6a69 0500 0068 1c68 0368 1d8c 8143  h.ji...h.h.h...C
-00004180: 3a5c 5573 6572 735c 632d 6d69 685c 7370  :\Users\c-mih\sp
-00004190: 6163 655c 636f 6f6b 6965 735f 7574 696c  ace\cookies_util
-000041a0: 6974 6965 735c 7372 635c 636f 6f6b 6965  ities\src\cookie
-000041b0: 735f 7574 696c 6974 6965 735c 7374 6f70  s_utilities\stop
-000041c0: 7761 7463 682e 7079 3a64 6f63 7374 7269  watch.py:docstri
-000041d0: 6e67 206f 6620 636f 6f6b 6965 735f 7574  ng of cookies_ut
-000041e0: 696c 6974 6965 732e 7374 6f70 7761 7463  ilities.stopwatc
-000041f0: 682e 5374 6f70 7761 7463 682e 7368 6f77  h.Stopwatch.show
-00004200: 9468 1e4e 7562 6861 2981 947d 9428 6805  .h.Nubha)..}.(h.
-00004210: 6806 6807 5d94 2868 6629 8194 7d94 2868  h.h.].(hf)..}.(h
-00004220: 058c 1053 746f 7077 6174 6368 2e73 686f  ...Stopwatch.sho
-00004230: 7728 2994 6807 5d94 2868 8129 8194 7d94  w().h.].(h.)..}.
-00004240: 2868 058c 0473 686f 7794 6807 5d94 6816  (h...show.h.].h.
-00004250: 8c04 7368 6f77 9485 9481 947d 9428 681b  ..show.....}.(h.
-00004260: 6a8c 0600 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
-00004270: 6261 681f 7d94 2868 215d 9468 235d 9428  bah.}.(h!].h#].(
-00004280: 688d 688e 6568 255d 9468 275d 9468 295d  h.h.eh%].h'].h)]
-00004290: 9468 7d68 7e75 682b 6880 681b 6a88 0600  .h}h~uh+h.h.j...
-000042a0: 0068 1c68 0368 1d8c 8143 3a5c 5573 6572  .h.h.h...C:\User
-000042b0: 735c 632d 6d69 685c 7370 6163 655c 636f  s\c-mih\space\co
-000042c0: 6f6b 6965 735f 7574 696c 6974 6965 735c  okies_utilities\
-000042d0: 7372 635c 636f 6f6b 6965 735f 7574 696c  src\cookies_util
-000042e0: 6974 6965 735c 7374 6f70 7761 7463 682e  ities\stopwatch.
-000042f0: 7079 3a64 6f63 7374 7269 6e67 206f 6620  py:docstring of 
-00004300: 636f 6f6b 6965 735f 7574 696c 6974 6965  cookies_utilitie
-00004310: 732e 7374 6f70 7761 7463 682e 5374 6f70  s.stopwatch.Stop
-00004320: 7761 7463 682e 7368 6f77 9468 1e4b 0175  watch.show.h.K.u
-00004330: 6268 9329 8194 7d94 2868 058c 0228 2994  bh.)..}.(h...().
-00004340: 6807 5d94 681f 7d94 2868 215d 9468 235d  h.].h.}.(h!].h#]
-00004350: 9468 255d 9468 275d 9468 295d 9468 7d68  .h%].h'].h)].h}h
-00004360: 7e75 682b 6892 681b 6a88 0600 0068 1c68  ~uh+h.h.j....h.h
-00004370: 0368 1d6a 9a06 0000 681e 4b01 7562 6568  .h.j....h.K.ubeh
-00004380: 1f7d 9428 6821 5d94 6a82 0600 0061 6823  .}.(h!].j....ah#
-00004390: 5d94 286a ea01 0000 6aeb 0100 0065 6825  ].(j....j....eh%
-000043a0: 5d94 6827 5d94 6829 5d94 6aef 0100 008c  ].h'].h)].j.....
-000043b0: 1163 6f6f 6b69 6573 5f75 7469 6c69 7469  .cookies_utiliti
-000043c0: 6573 946a f101 0000 6a55 0500 006a f201  es.j....jU...j..
-000043d0: 0000 8c0e 5374 6f70 7761 7463 682e 7368  ....Stopwatch.sh
-000043e0: 6f77 946a f301 0000 6aab 0600 008c 0953  ow.j....j......S
-000043f0: 746f 7077 6174 6368 948c 0473 686f 7794  topwatch...show.
-00004400: 8794 6af5 0100 008c 1053 746f 7077 6174  ..j......Stopwat
-00004410: 6368 2e73 686f 7728 2994 7568 2b68 6568  ch.show().uh+heh
-00004420: 1d6a 9a06 0000 681e 4b01 681b 6a85 0600  .j....h.K.h.j...
-00004430: 0068 1c68 0375 626a f801 0000 2981 947d  .h.h.ubj....)..}
-00004440: 9428 6805 6806 6807 5d94 6afd 0100 0029  .(h.h.h.].j....)
-00004450: 8194 7d94 2868 058c 0f53 686f 7720 6c61  ..}.(h...Show la
-00004460: 7020 7469 6d65 732e 9468 075d 9468 168c  p times..h.].h..
-00004470: 0f53 686f 7720 6c61 7020 7469 6d65 732e  .Show lap times.
-00004480: 9485 9481 947d 9428 681b 6ab4 0600 0068  .....}.(h.j....h
-00004490: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
-000044a0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
-000044b0: 9468 295d 9475 682b 6afc 0100 0068 1d6a  .h)].uh+j....h.j
-000044c0: 8406 0000 681e 4b01 681b 6ab1 0600 0068  ....h.K.h.j....h
-000044d0: 1c68 0375 6261 681f 7d94 2868 215d 9468  .h.ubah.}.(h!].h
-000044e0: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-000044f0: 682b 6af7 0100 0068 1b6a 8506 0000 681c  h+j....h.j....h.
-00004500: 6803 681d 6a9a 0600 0068 1e4b 0175 6265  h.h.j....h.K.ube
-00004510: 681f 7d94 2868 215d 9468 235d 9428 8c02  h.}.(h!].h#].(..
-00004520: 7079 948c 066d 6574 686f 6494 6568 255d  py...method.eh%]
-00004530: 9468 275d 9468 295d 946a aa04 0000 6acb  .h'].h)].j....j.
-00004540: 0600 006a ab04 0000 6acc 0600 006a ac04  ...j....j....j..
-00004550: 0000 6acc 0600 006a ad04 0000 896a ae04  ..j....j.....j..
-00004560: 0000 896a af04 0000 8975 682b 6860 681c  ...j.....uh+h`h.
-00004570: 6803 681b 6a69 0500 0068 1d6a 8406 0000  h.h.ji...h.j....
-00004580: 681e 4e75 6265 681f 7d94 2868 215d 9468  h.Nubeh.}.(h!].h
-00004590: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-000045a0: 682b 6af7 0100 0068 1b6a 1c05 0000 681c  h+j....h.j....h.
-000045b0: 6803 681d 6a44 0500 0068 1e4b 0175 6265  h.h.jD...h.K.ube
-000045c0: 681f 7d94 2868 215d 9468 235d 9428 8c02  h.}.(h!].h#].(..
-000045d0: 7079 948c 0563 6c61 7373 9465 6825 5d94  py...class.eh%].
-000045e0: 6827 5d94 6829 5d94 6aaa 0400 006a d906  h'].h)].j....j..
-000045f0: 0000 6aab 0400 006a da06 0000 6aac 0400  ..j....j....j...
-00004600: 006a da06 0000 6aad 0400 0089 6aae 0400  .j....j.....j...
-00004610: 0089 6aaf 0400 0089 7568 2b68 6068 1c68  ..j.....uh+h`h.h
-00004620: 0368 1b6a fd04 0000 681d 4e68 1e4e 7562  .h.j....h.Nh.Nub
-00004630: 6809 8c07 636f 6d6d 656e 7494 9394 2981  h...comment...).
-00004640: 947d 9428 6805 8c12 3a73 686f 772d 696e  .}.(h...:show-in
-00004650: 6865 7269 7461 6e63 653a 9468 075d 9468  heritance:.h.].h
-00004660: 168c 123a 7368 6f77 2d69 6e68 6572 6974  ...:show-inherit
-00004670: 616e 6365 3a94 8594 8194 7d94 681b 6ae0  ance:.....}.h.j.
-00004680: 0600 0073 6261 681f 7d94 2868 215d 9468  ...sbah.}.(h!].h
-00004690: 235d 9468 255d 9468 275d 9468 295d 9468  #].h%].h'].h)].h
-000046a0: 7d68 7e75 682b 6ade 0600 0068 1b6a fd04  }h~uh+j....h.j..
-000046b0: 0000 681c 6803 681d 682c 681e 4b23 7562  ..h.h.h.h,h.K#ub
-000046c0: 6809 8c09 636f 6e74 6169 6e65 7294 9394  h...container...
-000046d0: 2981 947d 9428 6805 6806 6807 5d94 2868  )..}.(h.h.h.].(h
-000046e0: 098c 0763 6170 7469 6f6e 9493 9429 8194  ...caption...)..
-000046f0: 7d94 2868 058c 0745 7861 6d70 6c65 9468  }.(h...Example.h
-00004700: 075d 9468 168c 0745 7861 6d70 6c65 9485  .].h...Example..
-00004710: 9481 947d 9428 681b 6af5 0600 0068 1c68  ...}.(h.j....h.h
-00004720: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
-00004730: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00004740: 295d 9475 682b 6af3 0600 0068 1d68 2c68  )].uh+j....h.h,h
-00004750: 1e4b 2468 1b6a f006 0000 7562 6ac8 0400  .K$h.j....ubj...
-00004760: 0029 8194 7d94 2868 058c 8e69 6d70 6f72  .)..}.(h...impor
-00004770: 7420 636f 6f6b 6965 735f 7574 696c 6974  t cookies_utilit
-00004780: 6965 7320 6173 2063 750a 7377 203d 2063  ies as cu.sw = c
-00004790: 752e 5374 6f70 7761 7463 6828 290a 7377  u.Stopwatch().sw
-000047a0: 2e70 7265 7373 2827 7472 6169 6e20 7374  .press('train st
-000047b0: 6172 7427 290a 2320 7472 6169 6e0a 7377  art').# train.sw
-000047c0: 2e70 7265 7373 2827 7472 6169 6e20 656e  .press('train en
-000047d0: 6427 290a 2320 7465 7374 0a73 772e 7072  d').# test.sw.pr
-000047e0: 6573 7328 2774 6573 7420 656e 6427 290a  ess('test end').
-000047f0: 7377 2e73 686f 7728 2994 6807 5d94 6816  sw.show().h.].h.
-00004800: 8c8e 696d 706f 7274 2063 6f6f 6b69 6573  ..import cookies
-00004810: 5f75 7469 6c69 7469 6573 2061 7320 6375  _utilities as cu
-00004820: 0a73 7720 3d20 6375 2e53 746f 7077 6174  .sw = cu.Stopwat
-00004830: 6368 2829 0a73 772e 7072 6573 7328 2774  ch().sw.press('t
-00004840: 7261 696e 2073 7461 7274 2729 0a23 2074  rain start').# t
-00004850: 7261 696e 0a73 772e 7072 6573 7328 2774  rain.sw.press('t
-00004860: 7261 696e 2065 6e64 2729 0a23 2074 6573  rain end').# tes
-00004870: 740a 7377 2e70 7265 7373 2827 7465 7374  t.sw.press('test
-00004880: 2065 6e64 2729 0a73 772e 7368 6f77 2829   end').sw.show()
-00004890: 9485 9481 947d 9468 1b6a 0307 0000 7362  .....}.h.j....sb
-000048a0: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-000048b0: 5d94 6827 5d94 6829 5d94 687d 687e 6ad7  ].h'].h)].h}h~j.
-000048c0: 0400 0089 6ad8 0400 008c 0670 7974 686f  ....j......pytho
-000048d0: 6e94 6ada 0400 007d 9475 682b 6ac7 0400  n.j....}.uh+j...
-000048e0: 0068 1d68 2c68 1e4b 2468 1b6a f006 0000  .h.h,h.K$h.j....
-000048f0: 7562 6568 1f7d 9428 6821 5d94 8c03 6964  ubeh.}.(h!]...id
-00004900: 3194 6168 235d 948c 156c 6974 6572 616c  1.ah#]...literal
-00004910: 2d62 6c6f 636b 2d77 7261 7070 6572 9461  -block-wrapper.a
-00004920: 6825 5d94 6827 5d94 6829 5d94 8c0d 6c69  h%].h'].h)]...li
-00004930: 7465 7261 6c5f 626c 6f63 6b94 8875 682b  teral_block..uh+
-00004940: 6aee 0600 0068 1b6a fd04 0000 681c 6803  j....h.j....h.h.
-00004950: 681d 6806 681e 4e75 626a c804 0000 2981  h.h.h.Nubj....).
-00004960: 947d 9428 6805 8c54 7469 6d65 3128 7472  .}.(h..Ttime1(tr
-00004970: 6169 6e20 7374 6172 742d 7472 6169 6e20  ain start-train 
-00004980: 656e 6429 3a20 322e 3030 3073 0a74 696d  end): 2.000s.tim
-00004990: 6532 2874 7261 696e 2065 6e64 2d74 6573  e2(train end-tes
-000049a0: 7420 656e 6429 3a20 312e 3030 3073 0a74  t end): 1.000s.t
-000049b0: 6f74 616c 3a20 332e 3030 3073 9468 075d  otal: 3.000s.h.]
-000049c0: 9468 168c 5474 696d 6531 2874 7261 696e  .h..Ttime1(train
-000049d0: 2073 7461 7274 2d74 7261 696e 2065 6e64   start-train end
-000049e0: 293a 2032 2e30 3030 730a 7469 6d65 3228  ): 2.000s.time2(
-000049f0: 7472 6169 6e20 656e 642d 7465 7374 2065  train end-test e
-00004a00: 6e64 293a 2031 2e30 3030 730a 746f 7461  nd): 1.000s.tota
-00004a10: 6c3a 2033 2e30 3030 7394 8594 8194 7d94  l: 3.000s.....}.
-00004a20: 681b 6a1c 0700 0073 6261 681f 7d94 2868  h.j....sbah.}.(h
-00004a30: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00004a40: 295d 9468 7d68 7e6a d704 0000 896a d804  )].h}h~j.....j..
-00004a50: 0000 8c07 636f 6e73 6f6c 6594 6ada 0400  ....console.j...
-00004a60: 007d 9475 682b 6ac7 0400 0068 1d68 2c68  .}.uh+j....h.h,h
-00004a70: 1e4b 3068 1b6a fd04 0000 681c 6803 7562  .K0h.j....h.h.ub
-00004a80: 6568 1f7d 9428 6821 5d94 8c1b 636f 6f6b  eh.}.(h!]...cook
-00004a90: 6965 732d 7574 696c 6974 6965 732d 7374  ies-utilities-st
-00004aa0: 6f70 7761 7463 6894 6168 235d 9468 255d  opwatch.ah#].h%]
-00004ab0: 948c 1b63 6f6f 6b69 6573 5f75 7469 6c69  ...cookies_utili
-00004ac0: 7469 6573 2e73 746f 7077 6174 6368 9461  ties.stopwatch.a
-00004ad0: 6827 5d94 6829 5d94 7568 2b68 0a68 1b6a  h'].h)].uh+h.h.j
-00004ae0: ec04 0000 681c 6803 681d 682c 681e 4b1c  ....h.h.h.h,h.K.
-00004af0: 7562 6568 1f7d 9428 6821 5d94 8c07 636c  ubeh.}.(h!]...cl
-00004b00: 6173 7365 7394 6168 235d 9468 255d 948c  asses.ah#].h%]..
-00004b10: 0763 6c61 7373 6573 9461 6827 5d94 6829  .classes.ah'].h)
-00004b20: 5d94 7568 2b68 0a68 1b68 0c68 1c68 0368  ].uh+h.h.h.h.h.h
-00004b30: 1d68 2c68 1e4b 1975 6265 681f 7d94 2868  .h,h.K.ubeh.}.(h
-00004b40: 215d 948c 0d64 6f63 756d 656e 7461 7469  !]...documentati
-00004b50: 6f6e 9461 6823 5d94 6825 5d94 8c0d 646f  on.ah#].h%]...do
-00004b60: 6375 6d65 6e74 6174 696f 6e94 6168 275d  cumentation.ah']
-00004b70: 9468 295d 9475 682b 680a 681b 6803 681c  .h)].uh+h.h.h.h.
-00004b80: 6803 681d 682c 681e 4b02 7562 6168 1f7d  h.h.h,h.K.ubah.}
-00004b90: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-00004ba0: 5d94 6829 5d94 8c06 736f 7572 6365 9468  ].h)]...source.h
-00004bb0: 2c75 682b 6801 8c0e 6375 7272 656e 745f  ,uh+h...current_
-00004bc0: 736f 7572 6365 944e 8c0c 6375 7272 656e  source.N..curren
-00004bd0: 745f 6c69 6e65 944e 8c08 7365 7474 696e  t_line.N..settin
-00004be0: 6773 948c 1164 6f63 7574 696c 732e 6672  gs...docutils.fr
-00004bf0: 6f6e 7465 6e64 948c 0656 616c 7565 7394  ontend...Values.
-00004c00: 9394 2981 947d 9428 680f 4e8c 0967 656e  ..)..}.(h.N..gen
-00004c10: 6572 6174 6f72 944e 8c09 6461 7465 7374  erator.N..datest
-00004c20: 616d 7094 4e8c 0b73 6f75 7263 655f 6c69  amp.N..source_li
-00004c30: 6e6b 944e 8c0a 736f 7572 6365 5f75 726c  nk.N..source_url
-00004c40: 944e 8c0d 746f 635f 6261 636b 6c69 6e6b  .N..toc_backlink
-00004c50: 7394 8c05 656e 7472 7994 8c12 666f 6f74  s...entry...foot
-00004c60: 6e6f 7465 5f62 6163 6b6c 696e 6b73 944b  note_backlinks.K
-00004c70: 018c 0d73 6563 746e 756d 5f78 666f 726d  ...sectnum_xform
-00004c80: 944b 018c 0e73 7472 6970 5f63 6f6d 6d65  .K...strip_comme
-00004c90: 6e74 7394 4e8c 1b73 7472 6970 5f65 6c65  nts.N..strip_ele
-00004ca0: 6d65 6e74 735f 7769 7468 5f63 6c61 7373  ments_with_class
-00004cb0: 6573 944e 8c0d 7374 7269 705f 636c 6173  es.N..strip_clas
-00004cc0: 7365 7394 4e8c 0c72 6570 6f72 745f 6c65  ses.N..report_le
-00004cd0: 7665 6c94 4b02 8c0a 6861 6c74 5f6c 6576  vel.K...halt_lev
-00004ce0: 656c 944b 058c 1165 7869 745f 7374 6174  el.K...exit_stat
-00004cf0: 7573 5f6c 6576 656c 944b 058c 0564 6562  us_level.K...deb
-00004d00: 7567 944e 8c0e 7761 726e 696e 675f 7374  ug.N..warning_st
-00004d10: 7265 616d 944e 8c09 7472 6163 6562 6163  ream.N..tracebac
-00004d20: 6b94 888c 0e69 6e70 7574 5f65 6e63 6f64  k....input_encod
-00004d30: 696e 6794 8c09 7574 662d 382d 7369 6794  ing...utf-8-sig.
-00004d40: 8c1c 696e 7075 745f 656e 636f 6469 6e67  ..input_encoding
-00004d50: 5f65 7272 6f72 5f68 616e 646c 6572 948c  _error_handler..
-00004d60: 0673 7472 6963 7494 8c0f 6f75 7470 7574  .strict...output
-00004d70: 5f65 6e63 6f64 696e 6794 8c05 7574 662d  _encoding...utf-
-00004d80: 3894 8c1d 6f75 7470 7574 5f65 6e63 6f64  8...output_encod
-00004d90: 696e 675f 6572 726f 725f 6861 6e64 6c65  ing_error_handle
-00004da0: 7294 6a67 0700 008c 0e65 7272 6f72 5f65  r.jg.....error_e
-00004db0: 6e63 6f64 696e 6794 8c05 7574 662d 3894  ncoding...utf-8.
-00004dc0: 8c1c 6572 726f 725f 656e 636f 6469 6e67  ..error_encoding
-00004dd0: 5f65 7272 6f72 5f68 616e 646c 6572 948c  _error_handler..
-00004de0: 1062 6163 6b73 6c61 7368 7265 706c 6163  .backslashreplac
-00004df0: 6594 8c0d 6c61 6e67 7561 6765 5f63 6f64  e...language_cod
-00004e00: 6594 8c02 656e 948c 1372 6563 6f72 645f  e...en...record_
-00004e10: 6465 7065 6e64 656e 6369 6573 944e 8c06  dependencies.N..
-00004e20: 636f 6e66 6967 944e 8c09 6964 5f70 7265  config.N..id_pre
-00004e30: 6669 7894 6806 8c0e 6175 746f 5f69 645f  fix.h...auto_id_
-00004e40: 7072 6566 6978 948c 0269 6494 8c0d 6475  prefix...id...du
-00004e50: 6d70 5f73 6574 7469 6e67 7394 4e8c 0e64  mp_settings.N..d
-00004e60: 756d 705f 696e 7465 726e 616c 7394 4e8c  ump_internals.N.
-00004e70: 0f64 756d 705f 7472 616e 7366 6f72 6d73  .dump_transforms
-00004e80: 944e 8c0f 6475 6d70 5f70 7365 7564 6f5f  .N..dump_pseudo_
-00004e90: 786d 6c94 4e8c 1065 7870 6f73 655f 696e  xml.N..expose_in
-00004ea0: 7465 726e 616c 7394 4e8c 0e73 7472 6963  ternals.N..stric
-00004eb0: 745f 7669 7369 746f 7294 4e8c 0f5f 6469  t_visitor.N.._di
-00004ec0: 7361 626c 655f 636f 6e66 6967 944e 8c07  sable_config.N..
-00004ed0: 5f73 6f75 7263 6594 682c 8c0c 5f64 6573  _source.h,.._des
-00004ee0: 7469 6e61 7469 6f6e 944e 8c0d 5f63 6f6e  tination.N.._con
-00004ef0: 6669 675f 6669 6c65 7394 5d94 8c16 6669  fig_files.]...fi
-00004f00: 6c65 5f69 6e73 6572 7469 6f6e 5f65 6e61  le_insertion_ena
-00004f10: 626c 6564 9488 8c0b 7261 775f 656e 6162  bled....raw_enab
-00004f20: 6c65 6494 4b01 8c11 6c69 6e65 5f6c 656e  led.K...line_len
-00004f30: 6774 685f 6c69 6d69 7494 4d10 278c 0e70  gth_limit.M.'..p
-00004f40: 6570 5f72 6566 6572 656e 6365 7394 4e8c  ep_references.N.
-00004f50: 0c70 6570 5f62 6173 655f 7572 6c94 8c18  .pep_base_url...
-00004f60: 6874 7470 733a 2f2f 7065 7073 2e70 7974  https://peps.pyt
-00004f70: 686f 6e2e 6f72 672f 948c 1570 6570 5f66  hon.org/...pep_f
-00004f80: 696c 655f 7572 6c5f 7465 6d70 6c61 7465  ile_url_template
-00004f90: 948c 0870 6570 2d25 3034 6494 8c0e 7266  ...pep-%04d...rf
-00004fa0: 635f 7265 6665 7265 6e63 6573 944e 8c0c  c_references.N..
-00004fb0: 7266 635f 6261 7365 5f75 726c 948c 2668  rfc_base_url..&h
-00004fc0: 7474 7073 3a2f 2f64 6174 6174 7261 636b  ttps://datatrack
-00004fd0: 6572 2e69 6574 662e 6f72 672f 646f 632f  er.ietf.org/doc/
-00004fe0: 6874 6d6c 2f94 8c09 7461 625f 7769 6474  html/...tab_widt
-00004ff0: 6894 4b08 8c1d 7472 696d 5f66 6f6f 746e  h.K...trim_footn
-00005000: 6f74 655f 7265 6665 7265 6e63 655f 7370  ote_reference_sp
-00005010: 6163 6594 898c 1073 796e 7461 785f 6869  ace....syntax_hi
-00005020: 6768 6c69 6768 7494 8c04 6c6f 6e67 948c  ghlight...long..
-00005030: 0c73 6d61 7274 5f71 756f 7465 7394 888c  .smart_quotes...
-00005040: 1373 6d61 7274 7175 6f74 6573 5f6c 6f63  .smartquotes_loc
-00005050: 616c 6573 945d 948c 1d63 6861 7261 6374  ales.]...charact
-00005060: 6572 5f6c 6576 656c 5f69 6e6c 696e 655f  er_level_inline_
-00005070: 6d61 726b 7570 9489 8c0e 646f 6374 6974  markup....doctit
-00005080: 6c65 5f78 666f 726d 9489 8c0d 646f 6369  le_xform....doci
-00005090: 6e66 6f5f 7866 6f72 6d94 4b01 8c12 7365  nfo_xform.K...se
-000050a0: 6374 7375 6274 6974 6c65 5f78 666f 726d  ctsubtitle_xform
-000050b0: 9489 8c0d 696d 6167 655f 6c6f 6164 696e  ....image_loadin
-000050c0: 6794 8c04 6c69 6e6b 948c 1065 6d62 6564  g...link...embed
-000050d0: 5f73 7479 6c65 7368 6565 7494 898c 1563  _stylesheet....c
-000050e0: 6c6f 616b 5f65 6d61 696c 5f61 6464 7265  loak_email_addre
-000050f0: 7373 6573 9488 8c11 7365 6374 696f 6e5f  sses....section_
-00005100: 7365 6c66 5f6c 696e 6b94 898c 0365 6e76  self_link....env
-00005110: 944e 7562 8c08 7265 706f 7274 6572 944e  .Nub..reporter.N
-00005120: 8c10 696e 6469 7265 6374 5f74 6172 6765  ..indirect_targe
-00005130: 7473 945d 948c 1173 7562 7374 6974 7574  ts.]...substitut
-00005140: 696f 6e5f 6465 6673 947d 948c 1273 7562  ion_defs.}...sub
-00005150: 7374 6974 7574 696f 6e5f 6e61 6d65 7394  stitution_names.
-00005160: 7d94 8c08 7265 666e 616d 6573 947d 948c  }...refnames.}..
-00005170: 0672 6566 6964 7394 7d94 8c07 6e61 6d65  .refids.}...name
-00005180: 6964 7394 7d94 286a 4107 0000 6a3e 0700  ids.}.(jA...j>..
-00005190: 006a e904 0000 6ae6 0400 006a e104 0000  .j....j....j....
-000051a0: 6ade 0400 006a 3907 0000 6a36 0700 006a  j....j9...j6...j
-000051b0: 3107 0000 6a2e 0700 0075 8c09 6e61 6d65  1...j....u..name
-000051c0: 7479 7065 7394 7d94 286a 4107 0000 896a  types.}.(jA....j
-000051d0: e904 0000 896a e104 0000 896a 3907 0000  .....j.....j9...
-000051e0: 896a 3107 0000 8975 6821 7d94 286a 3e07  .j1....uh!}.(j>.
-000051f0: 0000 680c 6ae6 0400 0068 2d6a de04 0000  ..h.j....h-j....
-00005200: 683e 685e 6867 6a36 0700 006a ec04 0000  h>h^hgj6...j....
-00005210: 6a2e 0700 006a fd04 0000 6a1a 0500 006a  j....j....j....j
-00005220: 1f05 0000 6a87 0500 006a 8c05 0000 6a82  ....j....j....j.
-00005230: 0600 006a 8806 0000 6a15 0700 006a f006  ...j....j....j..
-00005240: 0000 758c 0d66 6f6f 746e 6f74 655f 7265  ..u..footnote_re
-00005250: 6673 947d 948c 0d63 6974 6174 696f 6e5f  fs.}...citation_
-00005260: 7265 6673 947d 948c 0d61 7574 6f66 6f6f  refs.}...autofoo
-00005270: 746e 6f74 6573 945d 948c 1161 7574 6f66  tnotes.]...autof
-00005280: 6f6f 746e 6f74 655f 7265 6673 945d 948c  ootnote_refs.]..
-00005290: 1073 796d 626f 6c5f 666f 6f74 6e6f 7465  .symbol_footnote
-000052a0: 7394 5d94 8c14 7379 6d62 6f6c 5f66 6f6f  s.]...symbol_foo
-000052b0: 746e 6f74 655f 7265 6673 945d 948c 0966  tnote_refs.]...f
-000052c0: 6f6f 746e 6f74 6573 945d 948c 0963 6974  ootnotes.]...cit
-000052d0: 6174 696f 6e73 945d 948c 1261 7574 6f66  ations.]...autof
-000052e0: 6f6f 746e 6f74 655f 7374 6172 7494 4b01  ootnote_start.K.
-000052f0: 8c15 7379 6d62 6f6c 5f66 6f6f 746e 6f74  ..symbol_footnot
-00005300: 655f 7374 6172 7494 4b00 8c0a 6964 5f63  e_start.K...id_c
-00005310: 6f75 6e74 6572 948c 0b63 6f6c 6c65 6374  ounter...collect
-00005320: 696f 6e73 948c 0743 6f75 6e74 6572 9493  ions...Counter..
-00005330: 947d 946a 7507 0000 4b01 7385 9452 948c  .}.ju...K.s..R..
-00005340: 0e70 6172 7365 5f6d 6573 7361 6765 7394  .parse_messages.
-00005350: 5d94 8c12 7472 616e 7366 6f72 6d5f 6d65  ]...transform_me
-00005360: 7373 6167 6573 945d 948c 0b74 7261 6e73  ssages.]...trans
-00005370: 666f 726d 6572 944e 8c0b 696e 636c 7564  former.N..includ
-00005380: 655f 6c6f 6794 5d94 8c0a 6465 636f 7261  e_log.]...decora
-00005390: 7469 6f6e 944e 681c 6803 7562 2e         tion.Nh.h.ub.
+00000880: 6807 5d94 6816 8c15 2732 3031 362d 3037  h.].h...'2016-07
+00000890: 2d30 3120 3032 3a30 303a 3030 2794 8594  -01 02:00:00'...
+000008a0: 8194 7d94 2868 1b68 c268 1c68 0368 1d4e  ..}.(h.h.h.h.h.N
+000008b0: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
+000008c0: 235d 948c 0d64 6566 6175 6c74 5f76 616c  #]...default_val
+000008d0: 7565 9461 6825 5d94 6827 5d94 6829 5d94  ue.ah%].h'].h)].
+000008e0: 8c13 7375 7070 6f72 745f 736d 6172 7471  ..support_smartq
+000008f0: 756f 7465 7394 8975 682b 68c0 681b 689a  uotes..uh+h.h.h.
+00000900: 7562 6568 1f7d 9428 6821 5d94 6823 5d94  ubeh.}.(h!].h#].
+00000910: 6825 5d94 6827 5d94 6829 5d94 687d 687e  h%].h'].h)].h}h~
+00000920: 7568 2b68 9868 1b68 9475 6268 9929 8194  uh+h.h.h.ubh.)..
+00000930: 7d94 2868 058c 1965 6e64 3d27 3230 3136  }.(h...end='2016
+00000940: 2d30 372d 3032 2030 313a 3030 3a30 3027  -07-02 01:00:00'
+00000950: 9468 075d 9428 689f 2981 947d 9428 6805  .h.].(h.)..}.(h.
+00000960: 8c03 656e 6494 6807 5d94 6816 8c03 656e  ..end.h.].h...en
+00000970: 6494 8594 8194 7d94 2868 1b68 dc68 1c68  d.....}.(h.h.h.h
+00000980: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+00000990: 215d 9468 235d 9468 ab61 6825 5d94 6827  !].h#].h.ah%].h'
+000009a0: 5d94 6829 5d94 7568 2b68 9e68 1b68 d875  ].h)].uh+h.h.h.u
+000009b0: 6268 b029 8194 7d94 2868 058c 013d 9468  bh.)..}.(h...=.h
+000009c0: 075d 9468 168c 013d 9485 9481 947d 9428  .].h...=.....}.(
+000009d0: 681b 68ea 681c 6803 681d 4e68 1e4e 7562  h.h.h.h.h.Nh.Nub
+000009e0: 6168 1f7d 9428 6821 5d94 6823 5d94 68bc  ah.}.(h!].h#].h.
+000009f0: 6168 255d 9468 275d 9468 295d 9475 682b  ah%].h'].h)].uh+
+00000a00: 68af 681b 68d8 7562 68c1 2981 947d 9428  h.h.h.ubh.)..}.(
+00000a10: 6805 8c15 2732 3031 362d 3037 2d30 3220  h...'2016-07-02 
+00000a20: 3031 3a30 303a 3030 2794 6807 5d94 6816  01:00:00'.h.].h.
+00000a30: 8c15 2732 3031 362d 3037 2d30 3220 3031  ..'2016-07-02 01
+00000a40: 3a30 303a 3030 2794 8594 8194 7d94 2868  :00:00'.....}.(h
+00000a50: 1b68 f868 1c68 0368 1d4e 681e 4e75 6261  .h.h.h.h.Nh.Nuba
+00000a60: 681f 7d94 2868 215d 9468 235d 9468 cd61  h.}.(h!].h#].h.a
+00000a70: 6825 5d94 6827 5d94 6829 5d94 8c13 7375  h%].h'].h)]...su
+00000a80: 7070 6f72 745f 736d 6172 7471 756f 7465  pport_smartquote
+00000a90: 7394 8975 682b 68c0 681b 68d8 7562 6568  s..uh+h.h.h.ubeh
+00000aa0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+00000ab0: 6827 5d94 6829 5d94 687d 687e 7568 2b68  h'].h)].h}h~uh+h
+00000ac0: 9868 1b68 9475 6268 9929 8194 7d94 2868  .h.h.ubh.)..}.(h
+00000ad0: 058c 1a66 6f72 6d61 743d 2725 592d 256d  ...format='%Y-%m
+00000ae0: 2d25 6420 2548 3a25 4d3a 2553 2794 6807  -%d %H:%M:%S'.h.
+00000af0: 5d94 2868 9f29 8194 7d94 2868 058c 0666  ].(h.)..}.(h...f
+00000b00: 6f72 6d61 7494 6807 5d94 6816 8c06 666f  ormat.h.].h...fo
+00000b10: 726d 6174 9485 9481 947d 9428 681b 6a11  rmat.....}.(h.j.
+00000b20: 0100 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
+00000b30: 681f 7d94 2868 215d 9468 235d 9468 ab61  h.}.(h!].h#].h.a
+00000b40: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
+00000b50: 9e68 1b6a 0d01 0000 7562 68b0 2981 947d  .h.j....ubh.)..}
+00000b60: 9428 6805 8c01 3d94 6807 5d94 6816 8c01  .(h...=.h.].h...
+00000b70: 3d94 8594 8194 7d94 2868 1b6a 1f01 0000  =.....}.(h.j....
+00000b80: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
+00000b90: 9428 6821 5d94 6823 5d94 68bc 6168 255d  .(h!].h#].h.ah%]
+00000ba0: 9468 275d 9468 295d 9475 682b 68af 681b  .h'].h)].uh+h.h.
+00000bb0: 6a0d 0100 0075 6268 c129 8194 7d94 2868  j....ubh.)..}.(h
+00000bc0: 058c 1327 2559 2d25 6d2d 2564 2025 483a  ...'%Y-%m-%d %H:
+00000bd0: 254d 3a25 5327 9468 075d 9468 168c 1327  %M:%S'.h.].h...'
+00000be0: 2559 2d25 6d2d 2564 2025 483a 254d 3a25  %Y-%m-%d %H:%M:%
+00000bf0: 5327 9485 9481 947d 9428 681b 6a2d 0100  S'.....}.(h.j-..
+00000c00: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
+00000c10: 7d94 2868 215d 9468 235d 9468 cd61 6825  }.(h!].h#].h.ah%
+00000c20: 5d94 6827 5d94 6829 5d94 8c13 7375 7070  ].h'].h)]...supp
+00000c30: 6f72 745f 736d 6172 7471 756f 7465 7394  ort_smartquotes.
+00000c40: 8975 682b 68c0 681b 6a0d 0100 0075 6265  .uh+h.h.j....ube
+00000c50: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00000c60: 9468 275d 9468 295d 9468 7d68 7e75 682b  .h'].h)].h}h~uh+
+00000c70: 6898 681b 6894 7562 6899 2981 947d 9428  h.h.h.ubh.)..}.(
+00000c80: 6805 8c37 6465 6c74 613d 7b27 6461 7973  h..7delta={'days
+00000c90: 273a 2030 2c20 2768 6f75 7273 273a 2031  ': 0, 'hours': 1
+00000ca0: 2c20 276d 696e 7574 6573 273a 2030 2c20  , 'minutes': 0, 
+00000cb0: 2777 6565 6b73 273a 2030 7d94 6807 5d94  'weeks': 0}.h.].
+00000cc0: 2868 9f29 8194 7d94 2868 058c 0564 656c  (h.)..}.(h...del
+00000cd0: 7461 9468 075d 9468 168c 0564 656c 7461  ta.h.].h...delta
+00000ce0: 9485 9481 947d 9428 681b 6a46 0100 0068  .....}.(h.jF...h
+00000cf0: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
+00000d00: 2868 215d 9468 235d 9468 ab61 6825 5d94  (h!].h#].h.ah%].
+00000d10: 6827 5d94 6829 5d94 7568 2b68 9e68 1b6a  h'].h)].uh+h.h.j
+00000d20: 4201 0000 7562 68b0 2981 947d 9428 6805  B...ubh.)..}.(h.
+00000d30: 8c01 3d94 6807 5d94 6816 8c01 3d94 8594  ..=.h.].h...=...
+00000d40: 8194 7d94 2868 1b6a 5401 0000 681c 6803  ..}.(h.jT...h.h.
+00000d50: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
+00000d60: 5d94 6823 5d94 68bc 6168 255d 9468 275d  ].h#].h.ah%].h']
+00000d70: 9468 295d 9475 682b 68af 681b 6a42 0100  .h)].uh+h.h.jB..
+00000d80: 0075 6268 c129 8194 7d94 2868 058c 317b  .ubh.)..}.(h..1{
+00000d90: 2764 6179 7327 3a20 302c 2027 686f 7572  'days': 0, 'hour
+00000da0: 7327 3a20 312c 2027 6d69 6e75 7465 7327  s': 1, 'minutes'
+00000db0: 3a20 302c 2027 7765 656b 7327 3a20 307d  : 0, 'weeks': 0}
+00000dc0: 9468 075d 9468 168c 317b 2764 6179 7327  .h.].h..1{'days'
+00000dd0: 3a20 302c 2027 686f 7572 7327 3a20 312c  : 0, 'hours': 1,
+00000de0: 2027 6d69 6e75 7465 7327 3a20 302c 2027   'minutes': 0, '
+00000df0: 7765 656b 7327 3a20 307d 9485 9481 947d  weeks': 0}.....}
+00000e00: 9428 681b 6a62 0100 0068 1c68 0368 1d4e  .(h.jb...h.h.h.N
+00000e10: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
+00000e20: 235d 9468 cd61 6825 5d94 6827 5d94 6829  #].h.ah%].h'].h)
+00000e30: 5d94 8c13 7375 7070 6f72 745f 736d 6172  ]...support_smar
+00000e40: 7471 756f 7465 7394 8975 682b 68c0 681b  tquotes..uh+h.h.
+00000e50: 6a42 0100 0075 6265 681f 7d94 2868 215d  jB...ubeh.}.(h!]
+00000e60: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+00000e70: 9468 7d68 7e75 682b 6898 681b 6894 7562  .h}h~uh+h.h.h.ub
+00000e80: 6899 2981 947d 9428 6805 8c0d 6765 6e69  h.)..}.(h...geni
+00000e90: 7465 723d 4661 6c73 6594 6807 5d94 2868  ter=False.h.].(h
+00000ea0: 9f29 8194 7d94 2868 058c 0767 656e 6974  .)..}.(h...genit
+00000eb0: 6572 9468 075d 9468 168c 0767 656e 6974  er.h.].h...genit
+00000ec0: 6572 9485 9481 947d 9428 681b 6a7b 0100  er.....}.(h.j{..
+00000ed0: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
+00000ee0: 7d94 2868 215d 9468 235d 9468 ab61 6825  }.(h!].h#].h.ah%
+00000ef0: 5d94 6827 5d94 6829 5d94 7568 2b68 9e68  ].h'].h)].uh+h.h
+00000f00: 1b6a 7701 0000 7562 68b0 2981 947d 9428  .jw...ubh.)..}.(
+00000f10: 6805 8c01 3d94 6807 5d94 6816 8c01 3d94  h...=.h.].h...=.
+00000f20: 8594 8194 7d94 2868 1b6a 8901 0000 681c  ....}.(h.j....h.
+00000f30: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
+00000f40: 6821 5d94 6823 5d94 68bc 6168 255d 9468  h!].h#].h.ah%].h
+00000f50: 275d 9468 295d 9475 682b 68af 681b 6a77  '].h)].uh+h.h.jw
+00000f60: 0100 0075 6268 c129 8194 7d94 2868 058c  ...ubh.)..}.(h..
+00000f70: 0546 616c 7365 9468 075d 9468 168c 0546  .False.h.].h...F
+00000f80: 616c 7365 9485 9481 947d 9428 681b 6a97  alse.....}.(h.j.
+00000f90: 0100 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
+00000fa0: 681f 7d94 2868 215d 9468 235d 9468 cd61  h.}.(h!].h#].h.a
+00000fb0: 6825 5d94 6827 5d94 6829 5d94 8c13 7375  h%].h'].h)]...su
+00000fc0: 7070 6f72 745f 736d 6172 7471 756f 7465  pport_smartquote
+00000fd0: 7394 8975 682b 68c0 681b 6a77 0100 0075  s..uh+h.h.jw...u
+00000fe0: 6265 681f 7d94 2868 215d 9468 235d 9468  beh.}.(h!].h#].h
+00000ff0: 255d 9468 275d 9468 295d 9468 7d68 7e75  %].h'].h)].h}h~u
+00001000: 682b 6898 681b 6894 7562 6899 2981 947d  h+h.h.h.ubh.)..}
+00001010: 9428 6805 8c0d 6361 7374 5f73 7472 3d54  .(h...cast_str=T
+00001020: 7275 6594 6807 5d94 2868 9f29 8194 7d94  rue.h.].(h.)..}.
+00001030: 2868 058c 0863 6173 745f 7374 7294 6807  (h...cast_str.h.
+00001040: 5d94 6816 8c08 6361 7374 5f73 7472 9485  ].h...cast_str..
+00001050: 9481 947d 9428 681b 6ab0 0100 0068 1c68  ...}.(h.j....h.h
+00001060: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+00001070: 215d 9468 235d 9468 ab61 6825 5d94 6827  !].h#].h.ah%].h'
+00001080: 5d94 6829 5d94 7568 2b68 9e68 1b6a ac01  ].h)].uh+h.h.j..
+00001090: 0000 7562 68b0 2981 947d 9428 6805 8c01  ..ubh.)..}.(h...
+000010a0: 3d94 6807 5d94 6816 8c01 3d94 8594 8194  =.h.].h...=.....
+000010b0: 7d94 2868 1b6a be01 0000 681c 6803 681d  }.(h.j....h.h.h.
+000010c0: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
+000010d0: 6823 5d94 68bc 6168 255d 9468 275d 9468  h#].h.ah%].h'].h
+000010e0: 295d 9475 682b 68af 681b 6aac 0100 0075  )].uh+h.h.j....u
+000010f0: 6268 c129 8194 7d94 2868 058c 0454 7275  bh.)..}.(h...Tru
+00001100: 6594 6807 5d94 6816 8c04 5472 7565 9485  e.h.].h...True..
+00001110: 9481 947d 9428 681b 6acc 0100 0068 1c68  ...}.(h.j....h.h
+00001120: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+00001130: 215d 9468 235d 9468 cd61 6825 5d94 6827  !].h#].h.ah%].h'
+00001140: 5d94 6829 5d94 8c13 7375 7070 6f72 745f  ].h)]...support_
+00001150: 736d 6172 7471 756f 7465 7394 8975 682b  smartquotes..uh+
+00001160: 68c0 681b 6aac 0100 0075 6265 681f 7d94  h.h.j....ubeh.}.
+00001170: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00001180: 9468 295d 9468 7d68 7e75 682b 6898 681b  .h)].h}h~uh+h.h.
+00001190: 6894 7562 6899 2981 947d 9428 6805 8c0f  h.ubh.)..}.(h...
+000011a0: 666f 726d 6174 5f6f 7574 3d4e 6f6e 6594  format_out=None.
+000011b0: 6807 5d94 2868 9f29 8194 7d94 2868 058c  h.].(h.)..}.(h..
+000011c0: 0a66 6f72 6d61 745f 6f75 7494 6807 5d94  .format_out.h.].
+000011d0: 6816 8c0a 666f 726d 6174 5f6f 7574 9485  h...format_out..
+000011e0: 9481 947d 9428 681b 6ae5 0100 0068 1c68  ...}.(h.j....h.h
+000011f0: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+00001200: 215d 9468 235d 9468 ab61 6825 5d94 6827  !].h#].h.ah%].h'
+00001210: 5d94 6829 5d94 7568 2b68 9e68 1b6a e101  ].h)].uh+h.h.j..
+00001220: 0000 7562 68b0 2981 947d 9428 6805 8c01  ..ubh.)..}.(h...
+00001230: 3d94 6807 5d94 6816 8c01 3d94 8594 8194  =.h.].h...=.....
+00001240: 7d94 2868 1b6a f301 0000 681c 6803 681d  }.(h.j....h.h.h.
+00001250: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
+00001260: 6823 5d94 68bc 6168 255d 9468 275d 9468  h#].h.ah%].h'].h
+00001270: 295d 9475 682b 68af 681b 6ae1 0100 0075  )].uh+h.h.j....u
+00001280: 6268 c129 8194 7d94 2868 058c 044e 6f6e  bh.)..}.(h...Non
+00001290: 6594 6807 5d94 6816 8c04 4e6f 6e65 9485  e.h.].h...None..
+000012a0: 9481 947d 9428 681b 6a01 0200 0068 1c68  ...}.(h.j....h.h
+000012b0: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+000012c0: 215d 9468 235d 9468 cd61 6825 5d94 6827  !].h#].h.ah%].h'
+000012d0: 5d94 6829 5d94 8c13 7375 7070 6f72 745f  ].h)]...support_
+000012e0: 736d 6172 7471 756f 7465 7394 8975 682b  smartquotes..uh+
+000012f0: 68c0 681b 6ae1 0100 0075 6265 681f 7d94  h.h.j....ubeh.}.
+00001300: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00001310: 9468 295d 9468 7d68 7e75 682b 6898 681b  .h)].h}h~uh+h.h.
+00001320: 6894 7562 6568 1f7d 9428 6821 5d94 6823  h.ubeh.}.(h!].h#
+00001330: 5d94 6825 5d94 6827 5d94 6829 5d94 687d  ].h%].h'].h)].h}
+00001340: 687e 7568 2b68 9268 1b68 6768 1c68 0368  h~uh+h.h.hgh.h.h
+00001350: 1d68 7f68 1e4b 0175 6265 681f 7d94 2868  .h.h.K.ubeh.}.(h
+00001360: 215d 9468 5e61 6823 5d94 288c 0373 6967  !].h^ah#].(..sig
+00001370: 948c 0a73 6967 2d6f 626a 6563 7494 6568  ...sig-object.eh
+00001380: 255d 9468 275d 9468 295d 948c 066d 6f64  %].h'].h)]...mod
+00001390: 756c 6594 8c11 636f 6f6b 6965 735f 7574  ule...cookies_ut
+000013a0: 696c 6974 6965 7394 8c05 636c 6173 7394  ilities...class.
+000013b0: 6806 8c08 6675 6c6c 6e61 6d65 9468 848c  h...fullname.h..
+000013c0: 0a5f 746f 635f 7061 7274 7394 6a25 0200  ._toc_parts.j%..
+000013d0: 0068 8486 948c 095f 746f 635f 6e61 6d65  .h....._toc_name
+000013e0: 948c 0b67 6574 5f64 6174 6573 2829 9475  ...get_dates().u
+000013f0: 682b 6865 681d 687f 681e 4b01 681b 6862  h+heh.h.h.K.h.hb
+00001400: 681c 6803 7562 6800 8c0c 6465 7363 5f63  h.h.ubh...desc_c
+00001410: 6f6e 7465 6e74 9493 9429 8194 7d94 2868  ontent...)..}.(h
+00001420: 0568 0668 075d 9428 6809 8c09 7061 7261  .h.h.].(h...para
+00001430: 6772 6170 6894 9394 2981 947d 9428 6805  graph...)..}.(h.
+00001440: 8c58 5265 7475 726e 7320 6120 6c69 7374  .XReturns a list
+00001450: 206f 6620 7469 6d65 7320 6672 6f6d 2074   of times from t
+00001460: 6865 2027 7374 6172 7427 2074 696d 6520  he 'start' time 
+00001470: 746f 2074 6865 2027 656e 6427 2074 696d  to the 'end' tim
+00001480: 652c 0a69 6e63 7265 6d65 6e74 6564 2062  e,.incremented b
+00001490: 7920 2764 656c 7461 272e 9468 075d 9468  y 'delta'..h.].h
+000014a0: 168c 6452 6574 7572 6e73 2061 206c 6973  ..dReturns a lis
+000014b0: 7420 6f66 2074 696d 6573 2066 726f 6d20  t of times from 
+000014c0: 7468 6520 e280 9873 7461 7274 e280 9920  the ...start... 
+000014d0: 7469 6d65 2074 6f20 7468 6520 e280 9865  time to the ...e
+000014e0: 6e64 e280 9920 7469 6d65 2c0a 696e 6372  nd... time,.incr
+000014f0: 656d 656e 7465 6420 6279 20e2 8098 6465  emented by ...de
+00001500: 6c74 61e2 8099 2e94 8594 8194 7d94 2868  lta.........}.(h
+00001510: 1b6a 3302 0000 681c 6803 681d 4e68 1e4e  .j3...h.h.h.Nh.N
+00001520: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00001530: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
+00001540: 3102 0000 681d 8c71 433a 5c55 7365 7273  1...h..qC:\Users
+00001550: 5c63 2d6d 6968 5c73 7061 6365 5c63 6f6f  \c-mih\space\coo
+00001560: 6b69 6573 5f75 7469 6c69 7469 6573 5c73  kies_utilities\s
+00001570: 7263 5c63 6f6f 6b69 6573 5f75 7469 6c69  rc\cookies_utili
+00001580: 7469 6573 5c5f 5f69 6e69 745f 5f2e 7079  ties\__init__.py
+00001590: 3a64 6f63 7374 7269 6e67 206f 6620 636f  :docstring of co
+000015a0: 6f6b 6965 735f 7574 696c 6974 6965 732e  okies_utilities.
+000015b0: 6765 745f 6461 7465 7394 681e 4b01 681b  get_dates.h.K.h.
+000015c0: 6a2e 0200 0068 1c68 0375 626a 3202 0000  j....h.h.ubj2...
+000015d0: 2981 947d 9428 6805 8c53 4966 2079 6f75  )..}.(h..SIf you
+000015e0: 2772 6520 7573 696e 6720 7468 6520 7265  're using the re
+000015f0: 7375 6c74 2061 7320 616e 2069 7465 7261  sult as an itera
+00001600: 746f 722c 2069 7420 6973 2072 6563 6f6d  tor, it is recom
+00001610: 6d65 6e64 6564 2074 6f20 7365 7420 2a67  mended to set *g
+00001620: 656e 6974 6572 3d54 7275 652a 2e94 6807  eniter=True*..h.
+00001630: 5d94 2868 168c 4649 6620 796f 75e2 8099  ].(h..FIf you...
+00001640: 7265 2075 7369 6e67 2074 6865 2072 6573  re using the res
+00001650: 756c 7420 6173 2061 6e20 6974 6572 6174  ult as an iterat
+00001660: 6f72 2c20 6974 2069 7320 7265 636f 6d6d  or, it is recomm
+00001670: 656e 6465 6420 746f 2073 6574 2094 8594  ended to set ...
+00001680: 8194 7d94 2868 1b6a 4202 0000 681c 6803  ..}.(h.jB...h.h.
+00001690: 681d 4e68 1e4e 7562 6809 8c08 656d 7068  h.Nh.Nubh...emph
+000016a0: 6173 6973 9493 9429 8194 7d94 2868 058c  asis...)..}.(h..
+000016b0: 0e2a 6765 6e69 7465 723d 5472 7565 2a94  .*geniter=True*.
+000016c0: 6807 5d94 6816 8c0c 6765 6e69 7465 723d  h.].h...geniter=
+000016d0: 5472 7565 9485 9481 947d 9428 681b 6a4c  True.....}.(h.jL
+000016e0: 0200 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
+000016f0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00001700: 9468 275d 9468 295d 9475 682b 6a4a 0200  .h'].h)].uh+jJ..
+00001710: 0068 1b6a 4202 0000 7562 6816 8c01 2e94  .h.jB...ubh.....
+00001720: 8594 8194 7d94 2868 1b6a 4202 0000 681c  ....}.(h.jB...h.
+00001730: 6803 681d 4e68 1e4e 7562 6568 1f7d 9428  h.h.Nh.Nubeh.}.(
+00001740: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+00001750: 6829 5d94 7568 2b6a 3102 0000 681d 6a41  h)].uh+j1...h.jA
+00001760: 0200 0068 1e4b 0468 1b6a 2e02 0000 681c  ...h.K.h.j....h.
+00001770: 6803 7562 6809 8c0a 6669 656c 645f 6c69  h.ubh...field_li
+00001780: 7374 9493 9429 8194 7d94 2868 0568 0668  st...)..}.(h.h.h
+00001790: 075d 9428 6809 8c05 6669 656c 6494 9394  .].(h...field...
+000017a0: 2981 947d 9428 6805 6806 6807 5d94 2868  )..}.(h.h.h.].(h
+000017b0: 098c 0a66 6965 6c64 5f6e 616d 6594 9394  ...field_name...
+000017c0: 2981 947d 9428 6805 8c0a 5061 7261 6d65  )..}.(h...Parame
+000017d0: 7465 7273 9468 075d 9468 168c 0a50 6172  ters.h.].h...Par
+000017e0: 616d 6574 6572 7394 8594 8194 7d94 2868  ameters.....}.(h
+000017f0: 1b6a 7002 0000 681c 6803 681d 4e68 1e4e  .jp...h.h.h.Nh.N
+00001800: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00001810: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
+00001820: 6e02 0000 681b 6a6b 0200 0068 1d68 7f68  n...h.jk...h.h.h
+00001830: 1e4b 0075 6268 098c 0a66 6965 6c64 5f62  .K.ubh...field_b
+00001840: 6f64 7994 9394 2981 947d 9428 6805 6806  ody...)..}.(h.h.
+00001850: 6807 5d94 6809 8c0b 6275 6c6c 6574 5f6c  h.].h...bullet_l
+00001860: 6973 7494 9394 2981 947d 9428 6805 6806  ist...)..}.(h.h.
+00001870: 6807 5d94 2868 098c 096c 6973 745f 6974  h.].(h...list_it
+00001880: 656d 9493 9429 8194 7d94 2868 0568 0668  em...)..}.(h.h.h
+00001890: 075d 946a 3202 0000 2981 947d 9428 6805  .].j2...)..}.(h.
+000018a0: 8c24 7374 6172 7420 2873 7472 696e 6729  .$start (string)
+000018b0: 202d 2d20 5374 6172 7420 7469 6d65 2073   -- Start time s
+000018c0: 7472 696e 672e 9468 075d 9428 6800 8c0e  tring..h.].(h...
+000018d0: 6c69 7465 7261 6c5f 7374 726f 6e67 9493  literal_strong..
+000018e0: 9429 8194 7d94 2868 058c 0573 7461 7274  .)..}.(h...start
+000018f0: 9468 075d 9468 168c 0573 7461 7274 9485  .h.].h...start..
+00001900: 9481 947d 9428 681b 6a93 0200 0068 1c68  ...}.(h.j....h.h
+00001910: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+00001920: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+00001930: 295d 9475 682b 6a91 0200 0068 1b6a 8d02  )].uh+j....h.j..
+00001940: 0000 7562 6816 8c02 2028 9485 9481 947d  ..ubh... (.....}
+00001950: 9428 681b 6a8d 0200 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
+00001960: 681e 4e75 6268 008c 0c70 656e 6469 6e67  h.Nubh...pending
+00001970: 5f78 7265 6694 9394 2981 947d 9428 6805  _xref...)..}.(h.
+00001980: 6806 6807 5d94 6800 8c10 6c69 7465 7261  h.h.].h...litera
+00001990: 6c5f 656d 7068 6173 6973 9493 9429 8194  l_emphasis...)..
+000019a0: 7d94 2868 058c 0673 7472 696e 6794 6807  }.(h...string.h.
+000019b0: 5d94 6816 8c06 7374 7269 6e67 9485 9481  ].h...string....
+000019c0: 947d 9428 681b 6aac 0200 0068 1c68 0368  .}.(h.j....h.h.h
+000019d0: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
+000019e0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+000019f0: 9475 682b 6aaa 0200 0068 1b6a a702 0000  .uh+j....h.j....
+00001a00: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00001a10: 6825 5d94 6827 5d94 6829 5d94 8c09 7265  h%].h'].h)]...re
+00001a20: 6664 6f6d 6169 6e94 8c02 7079 948c 0b72  fdomain...py...r
+00001a30: 6566 6578 706c 6963 6974 9489 8c07 7265  efexplicit....re
+00001a40: 6674 7970 6594 6a26 0200 008c 0972 6566  ftype.j&.....ref
+00001a50: 7461 7267 6574 946a ae02 0000 8c0b 7265  target.j......re
+00001a60: 6673 7065 6369 6669 6394 888c 0970 793a  fspecific....py:
+00001a70: 6d6f 6475 6c65 946a 2502 0000 8c08 7079  module.j%.....py
+00001a80: 3a63 6c61 7373 944e 7568 2b6a a502 0000  :class.Nuh+j....
+00001a90: 681b 6a8d 0200 0075 6268 168c 0129 9485  h.j....ubh...)..
+00001aa0: 9481 947d 9428 681b 6a8d 0200 0068 1c68  ...}.(h.j....h.h
+00001ab0: 0368 1d4e 681e 4e75 6268 168c 0520 e280  .h.Nh.Nubh... ..
+00001ac0: 9320 9485 9481 947d 9428 681b 6a8d 0200  . .....}.(h.j...
+00001ad0: 0068 1c68 0368 1d4e 681e 4e75 6268 168c  .h.h.h.Nh.Nubh..
+00001ae0: 1253 7461 7274 2074 696d 6520 7374 7269  .Start time stri
+00001af0: 6e67 2e94 8594 8194 7d94 2868 1b6a 8d02  ng......}.(h.j..
+00001b00: 0000 681c 6803 681d 4e68 1e4e 7562 6568  ..h.h.h.Nh.Nubeh
+00001b10: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+00001b20: 6827 5d94 6829 5d94 7568 2b6a 3102 0000  h'].h)].uh+j1...
+00001b30: 681b 6a8a 0200 0075 6261 681f 7d94 2868  h.j....ubah.}.(h
+00001b40: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+00001b50: 295d 9475 682b 6a88 0200 0068 1b6a 8502  )].uh+j....h.j..
+00001b60: 0000 7562 6a89 0200 0029 8194 7d94 2868  ..ubj....)..}.(h
+00001b70: 0568 0668 075d 946a 3202 0000 2981 947d  .h.h.].j2...)..}
+00001b80: 9428 6805 8c2c 656e 6420 2873 7472 696e  .(h..,end (strin
+00001b90: 6729 202d 2d20 456e 6420 7469 6d65 2073  g) -- End time s
+00001ba0: 7472 696e 6720 2869 6e63 6c75 7369 7665  tring (inclusive
+00001bb0: 292e 9468 075d 9428 6a92 0200 0029 8194  )..h.].(j....)..
+00001bc0: 7d94 2868 058c 0365 6e64 9468 075d 9468  }.(h...end.h.].h
+00001bd0: 168c 0365 6e64 9485 9481 947d 9428 681b  ...end.....}.(h.
+00001be0: 6ae7 0200 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
+00001bf0: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+00001c00: 255d 9468 275d 9468 295d 9475 682b 6a91  %].h'].h)].uh+j.
+00001c10: 0200 0068 1b6a e302 0000 7562 6816 8c02  ...h.j....ubh...
+00001c20: 2028 9485 9481 947d 9428 681b 6ae3 0200   (.....}.(h.j...
+00001c30: 0068 1c68 0368 1d4e 681e 4e75 626a a602  .h.h.h.Nh.Nubj..
+00001c40: 0000 2981 947d 9428 6805 6806 6807 5d94  ..)..}.(h.h.h.].
+00001c50: 6aab 0200 0029 8194 7d94 2868 058c 0673  j....)..}.(h...s
+00001c60: 7472 696e 6794 6807 5d94 6816 8c06 7374  tring.h.].h...st
+00001c70: 7269 6e67 9485 9481 947d 9428 681b 6afc  ring.....}.(h.j.
+00001c80: 0200 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
+00001c90: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00001ca0: 9468 275d 9468 295d 9475 682b 6aaa 0200  .h'].h)].uh+j...
+00001cb0: 0068 1b6a f902 0000 7562 6168 1f7d 9428  .h.j....ubah.}.(
+00001cc0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+00001cd0: 6829 5d94 8c09 7265 6664 6f6d 6169 6e94  h)]...refdomain.
+00001ce0: 6ac1 0200 008c 0b72 6566 6578 706c 6963  j......refexplic
+00001cf0: 6974 9489 8c07 7265 6674 7970 6594 6a26  it....reftype.j&
+00001d00: 0200 008c 0972 6566 7461 7267 6574 946a  .....reftarget.j
+00001d10: fe02 0000 6ac5 0200 0088 6ac6 0200 006a  ....j.....j....j
+00001d20: 2502 0000 6ac7 0200 004e 7568 2b6a a502  %...j....Nuh+j..
+00001d30: 0000 681b 6ae3 0200 0075 6268 168c 0129  ..h.j....ubh...)
+00001d40: 9485 9481 947d 9428 681b 6ae3 0200 0068  .....}.(h.j....h
+00001d50: 1c68 0368 1d4e 681e 4e75 6268 168c 0520  .h.h.Nh.Nubh... 
+00001d60: e280 9320 9485 9481 947d 9428 681b 6ae3  ... .....}.(h.j.
+00001d70: 0200 0068 1c68 0368 1d4e 681e 4e75 6268  ...h.h.h.Nh.Nubh
+00001d80: 168c 1c45 6e64 2074 696d 6520 7374 7269  ...End time stri
+00001d90: 6e67 2028 696e 636c 7573 6976 6529 2e94  ng (inclusive)..
+00001da0: 8594 8194 7d94 2868 1b6a e302 0000 681c  ....}.(h.j....h.
+00001db0: 6803 681d 4e68 1e4e 7562 6568 1f7d 9428  h.h.Nh.Nubeh.}.(
+00001dc0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+00001dd0: 6829 5d94 7568 2b6a 3102 0000 681b 6ae0  h)].uh+j1...h.j.
+00001de0: 0200 0075 6261 681f 7d94 2868 215d 9468  ...ubah.}.(h!].h
+00001df0: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+00001e00: 682b 6a88 0200 0068 1b6a 8502 0000 7562  h+j....h.j....ub
+00001e10: 6a89 0200 0029 8194 7d94 2868 0568 0668  j....)..}.(h.h.h
+00001e20: 075d 946a 3202 0000 2981 947d 9428 6805  .].j2...)..}.(h.
+00001e30: 8c3b 666f 726d 6174 2028 7374 7269 6e67  .;format (string
+00001e40: 2920 2d2d 2043 6f6e 7665 7273 696f 6e20  ) -- Conversion 
+00001e50: 666f 726d 6174 2066 6f72 2064 6174 6574  format for datet
+00001e60: 696d 652e 7374 7270 7469 6d65 2e94 6807  ime.strptime..h.
+00001e70: 5d94 286a 9202 0000 2981 947d 9428 6805  ].(j....)..}.(h.
+00001e80: 8c06 666f 726d 6174 9468 075d 9468 168c  ..format.h.].h..
+00001e90: 0666 6f72 6d61 7494 8594 8194 7d94 2868  .format.....}.(h
+00001ea0: 1b6a 3303 0000 681c 6803 681d 4e68 1e4e  .j3...h.h.h.Nh.N
+00001eb0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00001ec0: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
+00001ed0: 9102 0000 681b 6a2f 0300 0075 6268 168c  ....h.j/...ubh..
+00001ee0: 0220 2894 8594 8194 7d94 2868 1b6a 2f03  . (.....}.(h.j/.
+00001ef0: 0000 681c 6803 681d 4e68 1e4e 7562 6aa6  ..h.h.h.Nh.Nubj.
+00001f00: 0200 0029 8194 7d94 2868 0568 0668 075d  ...)..}.(h.h.h.]
+00001f10: 946a ab02 0000 2981 947d 9428 6805 8c06  .j....)..}.(h...
+00001f20: 7374 7269 6e67 9468 075d 9468 168c 0673  string.h.].h...s
+00001f30: 7472 696e 6794 8594 8194 7d94 2868 1b6a  tring.....}.(h.j
+00001f40: 4803 0000 681c 6803 681d 4e68 1e4e 7562  H...h.h.h.Nh.Nub
+00001f50: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00001f60: 5d94 6827 5d94 6829 5d94 7568 2b6a aa02  ].h'].h)].uh+j..
+00001f70: 0000 681b 6a45 0300 0075 6261 681f 7d94  ..h.jE...ubah.}.
+00001f80: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00001f90: 9468 295d 948c 0972 6566 646f 6d61 696e  .h)]...refdomain
+00001fa0: 946a c102 0000 8c0b 7265 6665 7870 6c69  .j......refexpli
+00001fb0: 6369 7494 898c 0772 6566 7479 7065 946a  cit....reftype.j
+00001fc0: 2602 0000 8c09 7265 6674 6172 6765 7494  &.....reftarget.
+00001fd0: 6a4a 0300 006a c502 0000 886a c602 0000  jJ...j.....j....
+00001fe0: 6a25 0200 006a c702 0000 4e75 682b 6aa5  j%...j....Nuh+j.
+00001ff0: 0200 0068 1b6a 2f03 0000 7562 6816 8c01  ...h.j/...ubh...
+00002000: 2994 8594 8194 7d94 2868 1b6a 2f03 0000  ).....}.(h.j/...
+00002010: 681c 6803 681d 4e68 1e4e 7562 6816 8c05  h.h.h.Nh.Nubh...
+00002020: 20e2 8093 2094 8594 8194 7d94 2868 1b6a   ... .....}.(h.j
+00002030: 2f03 0000 681c 6803 681d 4e68 1e4e 7562  /...h.h.h.Nh.Nub
+00002040: 6816 8c28 436f 6e76 6572 7369 6f6e 2066  h..(Conversion f
+00002050: 6f72 6d61 7420 666f 7220 6461 7465 7469  ormat for dateti
+00002060: 6d65 2e73 7472 7074 696d 652e 9485 9481  me.strptime.....
+00002070: 947d 9428 681b 6a2f 0300 0068 1c68 0368  .}.(h.j/...h.h.h
+00002080: 1d4e 681e 4e75 6265 681f 7d94 2868 215d  .Nh.Nubeh.}.(h!]
+00002090: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+000020a0: 9475 682b 6a31 0200 0068 1b6a 2c03 0000  .uh+j1...h.j,...
+000020b0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+000020c0: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
+000020d0: 8802 0000 681b 6a85 0200 0075 626a 8902  ....h.j....ubj..
+000020e0: 0000 2981 947d 9428 6805 6806 6807 5d94  ..)..}.(h.h.h.].
+000020f0: 6a32 0200 0029 8194 7d94 2868 058c 3964  j2...)..}.(h..9d
+00002100: 656c 7461 2028 6469 6374 2920 2d2d 2054  elta (dict) -- T
+00002110: 696d 6564 656c 7461 2061 7320 6172 6773  imedelta as args
+00002120: 2066 6f72 2064 6174 6574 696d 652e 7469   for datetime.ti
+00002130: 6d65 6465 6c74 612e 9468 075d 9428 6a92  medelta..h.].(j.
+00002140: 0200 0029 8194 7d94 2868 058c 0564 656c  ...)..}.(h...del
+00002150: 7461 9468 075d 9468 168c 0564 656c 7461  ta.h.].h...delta
+00002160: 9485 9481 947d 9428 681b 6a7f 0300 0068  .....}.(h.j....h
+00002170: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
+00002180: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00002190: 9468 295d 9475 682b 6a91 0200 0068 1b6a  .h)].uh+j....h.j
+000021a0: 7b03 0000 7562 6816 8c02 2028 9485 9481  {...ubh... (....
+000021b0: 947d 9428 681b 6a7b 0300 0068 1c68 0368  .}.(h.j{...h.h.h
+000021c0: 1d4e 681e 4e75 626a a602 0000 2981 947d  .Nh.Nubj....)..}
+000021d0: 9428 6805 6806 6807 5d94 6aab 0200 0029  .(h.h.h.].j....)
+000021e0: 8194 7d94 2868 058c 0464 6963 7494 6807  ..}.(h...dict.h.
+000021f0: 5d94 6816 8c04 6469 6374 9485 9481 947d  ].h...dict.....}
+00002200: 9428 681b 6a94 0300 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
+00002210: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
+00002220: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+00002230: 682b 6aaa 0200 0068 1b6a 9103 0000 7562  h+j....h.j....ub
+00002240: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00002250: 5d94 6827 5d94 6829 5d94 8c09 7265 6664  ].h'].h)]...refd
+00002260: 6f6d 6169 6e94 6ac1 0200 008c 0b72 6566  omain.j......ref
+00002270: 6578 706c 6963 6974 9489 8c07 7265 6674  explicit....reft
+00002280: 7970 6594 6a26 0200 008c 0972 6566 7461  ype.j&.....refta
+00002290: 7267 6574 946a 9603 0000 6ac5 0200 0088  rget.j....j.....
+000022a0: 6ac6 0200 006a 2502 0000 6ac7 0200 004e  j....j%...j....N
+000022b0: 7568 2b6a a502 0000 681b 6a7b 0300 0075  uh+j....h.j{...u
+000022c0: 6268 168c 0129 9485 9481 947d 9428 681b  bh...).....}.(h.
+000022d0: 6a7b 0300 0068 1c68 0368 1d4e 681e 4e75  j{...h.h.h.Nh.Nu
+000022e0: 6268 168c 0520 e280 9320 9485 9481 947d  bh... ... .....}
+000022f0: 9428 681b 6a7b 0300 0068 1c68 0368 1d4e  .(h.j{...h.h.h.N
+00002300: 681e 4e75 6268 168c 2954 696d 6564 656c  h.Nubh..)Timedel
+00002310: 7461 2061 7320 6172 6773 2066 6f72 2064  ta as args for d
+00002320: 6174 6574 696d 652e 7469 6d65 6465 6c74  atetime.timedelt
+00002330: 612e 9485 9481 947d 9428 681b 6a7b 0300  a......}.(h.j{..
+00002340: 0068 1c68 0368 1d4e 681e 4e75 6265 681f  .h.h.h.Nh.Nubeh.
+00002350: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00002360: 275d 9468 295d 9475 682b 6a31 0200 0068  '].h)].uh+j1...h
+00002370: 1b6a 7803 0000 7562 6168 1f7d 9428 6821  .jx...ubah.}.(h!
+00002380: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00002390: 5d94 7568 2b6a 8802 0000 681b 6a85 0200  ].uh+j....h.j...
+000023a0: 0075 626a 8902 0000 2981 947d 9428 6805  .ubj....)..}.(h.
+000023b0: 6806 6807 5d94 6a32 0200 0029 8194 7d94  h.h.].j2...)..}.
+000023c0: 2868 058c 4c67 656e 6974 6572 2028 626f  (h..Lgeniter (bo
+000023d0: 6f6c 2920 2d2d 2057 6865 7468 6572 2074  ol) -- Whether t
+000023e0: 6f20 7265 7475 726e 2061 7320 6120 6765  o return as a ge
+000023f0: 6e65 7261 746f 7220 6974 6572 6174 6f72  nerator iterator
+00002400: 2028 6465 6661 756c 7420 4661 6c73 6529   (default False)
+00002410: 2e94 6807 5d94 286a 9202 0000 2981 947d  ..h.].(j....)..}
+00002420: 9428 6805 8c07 6765 6e69 7465 7294 6807  .(h...geniter.h.
+00002430: 5d94 6816 8c07 6765 6e69 7465 7294 8594  ].h...geniter...
+00002440: 8194 7d94 2868 1b6a cb03 0000 681c 6803  ..}.(h.j....h.h.
+00002450: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
+00002460: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00002470: 5d94 7568 2b6a 9102 0000 681b 6ac7 0300  ].uh+j....h.j...
+00002480: 0075 6268 168c 0220 2894 8594 8194 7d94  .ubh... (.....}.
+00002490: 2868 1b6a c703 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
+000024a0: 1e4e 7562 6aa6 0200 0029 8194 7d94 2868  .Nubj....)..}.(h
+000024b0: 0568 0668 075d 946a ab02 0000 2981 947d  .h.h.].j....)..}
+000024c0: 9428 6805 8c04 626f 6f6c 9468 075d 9468  .(h...bool.h.].h
+000024d0: 168c 0462 6f6f 6c94 8594 8194 7d94 2868  ...bool.....}.(h
+000024e0: 1b6a e003 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
+000024f0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00002500: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
+00002510: aa02 0000 681b 6add 0300 0075 6261 681f  ....h.j....ubah.
+00002520: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00002530: 275d 9468 295d 948c 0972 6566 646f 6d61  '].h)]...refdoma
+00002540: 696e 946a c102 0000 8c0b 7265 6665 7870  in.j......refexp
+00002550: 6c69 6369 7494 898c 0772 6566 7479 7065  licit....reftype
+00002560: 946a 2602 0000 8c09 7265 6674 6172 6765  .j&.....reftarge
+00002570: 7494 6ae2 0300 006a c502 0000 886a c602  t.j....j.....j..
+00002580: 0000 6a25 0200 006a c702 0000 4e75 682b  ..j%...j....Nuh+
+00002590: 6aa5 0200 0068 1b6a c703 0000 7562 6816  j....h.j....ubh.
+000025a0: 8c01 2994 8594 8194 7d94 2868 1b6a c703  ..).....}.(h.j..
+000025b0: 0000 681c 6803 681d 4e68 1e4e 7562 6816  ..h.h.h.Nh.Nubh.
+000025c0: 8c05 20e2 8093 2094 8594 8194 7d94 2868  .. ... .....}.(h
+000025d0: 1b6a c703 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
+000025e0: 7562 6816 8c33 5768 6574 6865 7220 746f  ubh..3Whether to
+000025f0: 2072 6574 7572 6e20 6173 2061 2067 656e   return as a gen
+00002600: 6572 6174 6f72 2069 7465 7261 746f 7220  erator iterator 
+00002610: 2864 6566 6175 6c74 2094 8594 8194 7d94  (default .....}.
+00002620: 2868 1b6a c703 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
+00002630: 1e4e 7562 6a4b 0200 0029 8194 7d94 2868  .NubjK...)..}.(h
+00002640: 058c 072a 4661 6c73 652a 9468 075d 9468  ...*False*.h.].h
+00002650: 168c 0546 616c 7365 9485 9481 947d 9428  ...False.....}.(
+00002660: 681b 6a04 0400 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
+00002670: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
+00002680: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+00002690: 6a4a 0200 0068 1b6a c703 0000 681c 6803  jJ...h.j....h.h.
+000026a0: 681d 4e68 1e4e 7562 6816 8c02 292e 9485  h.Nh.Nubh...)...
+000026b0: 9481 947d 9428 681b 6ac7 0300 0068 1c68  ...}.(h.j....h.h
+000026c0: 0368 1d4e 681e 4e75 6265 681f 7d94 2868  .h.Nh.Nubeh.}.(h
+000026d0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+000026e0: 295d 9475 682b 6a31 0200 0068 1b6a c403  )].uh+j1...h.j..
+000026f0: 0000 7562 6168 1f7d 9428 6821 5d94 6823  ..ubah.}.(h!].h#
+00002700: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+00002710: 2b6a 8802 0000 681b 6a85 0200 0075 626a  +j....h.j....ubj
+00002720: 8902 0000 2981 947d 9428 6805 6806 6807  ....)..}.(h.h.h.
+00002730: 5d94 6a32 0200 0029 8194 7d94 2868 058c  ].j2...)..}.(h..
+00002740: 4663 6173 745f 7374 7220 2862 6f6f 6c29  Fcast_str (bool)
+00002750: 202d 2d20 5768 6574 6865 7220 746f 2063   -- Whether to c
+00002760: 6f6e 7665 7274 206f 7574 7075 7420 746f  onvert output to
+00002770: 2073 7472 696e 6720 2864 6566 6175 6c74   string (default
+00002780: 2054 7275 6529 2e94 6807 5d94 286a 9202   True)..h.].(j..
+00002790: 0000 2981 947d 9428 6805 8c08 6361 7374  ..)..}.(h...cast
+000027a0: 5f73 7472 9468 075d 9468 168c 0863 6173  _str.h.].h...cas
+000027b0: 745f 7374 7294 8594 8194 7d94 2868 1b6a  t_str.....}.(h.j
+000027c0: 2904 0000 681c 6803 681d 4e68 1e4e 7562  )...h.h.h.Nh.Nub
+000027d0: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+000027e0: 5d94 6827 5d94 6829 5d94 7568 2b6a 9102  ].h'].h)].uh+j..
+000027f0: 0000 681b 6a25 0400 0075 6268 168c 0220  ..h.j%...ubh... 
+00002800: 2894 8594 8194 7d94 2868 1b6a 2504 0000  (.....}.(h.j%...
+00002810: 681c 6803 681d 4e68 1e4e 7562 6aa6 0200  h.h.h.Nh.Nubj...
+00002820: 0029 8194 7d94 2868 0568 0668 075d 946a  .)..}.(h.h.h.].j
+00002830: ab02 0000 2981 947d 9428 6805 8c04 626f  ....)..}.(h...bo
+00002840: 6f6c 9468 075d 9468 168c 0462 6f6f 6c94  ol.h.].h...bool.
+00002850: 8594 8194 7d94 2868 1b6a 3e04 0000 681c  ....}.(h.j>...h.
+00002860: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
+00002870: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+00002880: 6829 5d94 7568 2b6a aa02 0000 681b 6a3b  h)].uh+j....h.j;
+00002890: 0400 0075 6261 681f 7d94 2868 215d 9468  ...ubah.}.(h!].h
+000028a0: 235d 9468 255d 9468 275d 9468 295d 948c  #].h%].h'].h)]..
+000028b0: 0972 6566 646f 6d61 696e 946a c102 0000  .refdomain.j....
+000028c0: 8c0b 7265 6665 7870 6c69 6369 7494 898c  ..refexplicit...
+000028d0: 0772 6566 7479 7065 946a 2602 0000 8c09  .reftype.j&.....
+000028e0: 7265 6674 6172 6765 7494 6a40 0400 006a  reftarget.j@...j
+000028f0: c502 0000 886a c602 0000 6a25 0200 006a  .....j....j%...j
+00002900: c702 0000 4e75 682b 6aa5 0200 0068 1b6a  ....Nuh+j....h.j
+00002910: 2504 0000 7562 6816 8c01 2994 8594 8194  %...ubh...).....
+00002920: 7d94 2868 1b6a 2504 0000 681c 6803 681d  }.(h.j%...h.h.h.
+00002930: 4e68 1e4e 7562 6816 8c05 20e2 8093 2094  Nh.Nubh... ... .
+00002940: 8594 8194 7d94 2868 1b6a 2504 0000 681c  ....}.(h.j%...h.
+00002950: 6803 681d 4e68 1e4e 7562 6816 8c2d 5768  h.h.Nh.Nubh..-Wh
+00002960: 6574 6865 7220 746f 2063 6f6e 7665 7274  ether to convert
+00002970: 206f 7574 7075 7420 746f 2073 7472 696e   output to strin
+00002980: 6720 2864 6566 6175 6c74 2094 8594 8194  g (default .....
+00002990: 7d94 2868 1b6a 2504 0000 681c 6803 681d  }.(h.j%...h.h.h.
+000029a0: 4e68 1e4e 7562 6a4b 0200 0029 8194 7d94  Nh.NubjK...)..}.
+000029b0: 2868 058c 062a 5472 7565 2a94 6807 5d94  (h...*True*.h.].
+000029c0: 6816 8c04 5472 7565 9485 9481 947d 9428  h...True.....}.(
+000029d0: 681b 6a62 0400 0068 1c68 0368 1d4e 681e  h.jb...h.h.h.Nh.
+000029e0: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
+000029f0: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+00002a00: 6a4a 0200 0068 1b6a 2504 0000 681c 6803  jJ...h.j%...h.h.
+00002a10: 681d 4e68 1e4e 7562 6816 8c02 292e 9485  h.Nh.Nubh...)...
+00002a20: 9481 947d 9428 681b 6a25 0400 0068 1c68  ...}.(h.j%...h.h
+00002a30: 0368 1d4e 681e 4e75 6265 681f 7d94 2868  .h.Nh.Nubeh.}.(h
+00002a40: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+00002a50: 295d 9475 682b 6a31 0200 0068 1b6a 2204  )].uh+j1...h.j".
+00002a60: 0000 7562 6168 1f7d 9428 6821 5d94 6823  ..ubah.}.(h!].h#
+00002a70: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+00002a80: 2b6a 8802 0000 681b 6a85 0200 0075 626a  +j....h.j....ubj
+00002a90: 8902 0000 2981 947d 9428 6805 6806 6807  ....)..}.(h.h.h.
+00002aa0: 5d94 6a32 0200 0029 8194 7d94 2868 058c  ].j2...)..}.(h..
+00002ab0: 4d66 6f72 6d61 745f 6f75 7420 2873 7472  Mformat_out (str
+00002ac0: 696e 6729 202d 2d20 436f 6e76 6572 7369  ing) -- Conversi
+00002ad0: 6f6e 2066 6f72 6d61 7420 666f 7220 6f75  on format for ou
+00002ae0: 7470 7574 2028 6465 6661 756c 7420 7361  tput (default sa
+00002af0: 6d65 2074 6f20 666f 726d 6174 292e 9468  me to format)..h
+00002b00: 075d 9428 6a92 0200 0029 8194 7d94 2868  .].(j....)..}.(h
+00002b10: 058c 0a66 6f72 6d61 745f 6f75 7494 6807  ...format_out.h.
+00002b20: 5d94 6816 8c0a 666f 726d 6174 5f6f 7574  ].h...format_out
+00002b30: 9485 9481 947d 9428 681b 6a87 0400 0068  .....}.(h.j....h
+00002b40: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
+00002b50: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00002b60: 9468 295d 9475 682b 6a91 0200 0068 1b6a  .h)].uh+j....h.j
+00002b70: 8304 0000 7562 6816 8c02 2028 9485 9481  ....ubh... (....
+00002b80: 947d 9428 681b 6a83 0400 0068 1c68 0368  .}.(h.j....h.h.h
+00002b90: 1d4e 681e 4e75 626a a602 0000 2981 947d  .Nh.Nubj....)..}
+00002ba0: 9428 6805 6806 6807 5d94 6aab 0200 0029  .(h.h.h.].j....)
+00002bb0: 8194 7d94 2868 058c 0673 7472 696e 6794  ..}.(h...string.
+00002bc0: 6807 5d94 6816 8c06 7374 7269 6e67 9485  h.].h...string..
+00002bd0: 9481 947d 9428 681b 6a9c 0400 0068 1c68  ...}.(h.j....h.h
+00002be0: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+00002bf0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+00002c00: 295d 9475 682b 6aaa 0200 0068 1b6a 9904  )].uh+j....h.j..
+00002c10: 0000 7562 6168 1f7d 9428 6821 5d94 6823  ..ubah.}.(h!].h#
+00002c20: 5d94 6825 5d94 6827 5d94 6829 5d94 8c09  ].h%].h'].h)]...
+00002c30: 7265 6664 6f6d 6169 6e94 6ac1 0200 008c  refdomain.j.....
+00002c40: 0b72 6566 6578 706c 6963 6974 9489 8c07  .refexplicit....
+00002c50: 7265 6674 7970 6594 6a26 0200 008c 0972  reftype.j&.....r
+00002c60: 6566 7461 7267 6574 946a 9e04 0000 6ac5  eftarget.j....j.
+00002c70: 0200 0088 6ac6 0200 006a 2502 0000 6ac7  ....j....j%...j.
+00002c80: 0200 004e 7568 2b6a a502 0000 681b 6a83  ...Nuh+j....h.j.
+00002c90: 0400 0075 6268 168c 0129 9485 9481 947d  ...ubh...).....}
+00002ca0: 9428 681b 6a83 0400 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
+00002cb0: 681e 4e75 6268 168c 0520 e280 9320 9485  h.Nubh... ... ..
+00002cc0: 9481 947d 9428 681b 6a83 0400 0068 1c68  ...}.(h.j....h.h
+00002cd0: 0368 1d4e 681e 4e75 6268 168c 2e43 6f6e  .h.Nh.Nubh...Con
+00002ce0: 7665 7273 696f 6e20 666f 726d 6174 2066  version format f
+00002cf0: 6f72 206f 7574 7075 7420 2864 6566 6175  or output (defau
+00002d00: 6c74 2073 616d 6520 746f 2094 8594 8194  lt same to .....
+00002d10: 7d94 2868 1b6a 8304 0000 681c 6803 681d  }.(h.j....h.h.h.
+00002d20: 4e68 1e4e 7562 6809 8c06 7374 726f 6e67  Nh.Nubh...strong
+00002d30: 9493 9429 8194 7d94 2868 058c 0a2a 2a66  ...)..}.(h...**f
+00002d40: 6f72 6d61 742a 2a94 6807 5d94 6816 8c06  ormat**.h.].h...
+00002d50: 666f 726d 6174 9485 9481 947d 9428 681b  format.....}.(h.
+00002d60: 6ac2 0400 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
+00002d70: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+00002d80: 255d 9468 275d 9468 295d 9475 682b 6ac0  %].h'].h)].uh+j.
+00002d90: 0400 0068 1b6a 8304 0000 681c 6803 681d  ...h.j....h.h.h.
+00002da0: 4e68 1e4e 7562 6816 8c02 292e 9485 9481  Nh.Nubh...).....
+00002db0: 947d 9428 681b 6a83 0400 0068 1c68 0368  .}.(h.j....h.h.h
+00002dc0: 1d4e 681e 4e75 6265 681f 7d94 2868 215d  .Nh.Nubeh.}.(h!]
+00002dd0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+00002de0: 9475 682b 6a31 0200 0068 1b6a 8004 0000  .uh+j1...h.j....
+00002df0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00002e00: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
+00002e10: 8802 0000 681b 6a85 0200 0075 6265 681f  ....h.j....ubeh.
+00002e20: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00002e30: 275d 9468 295d 9475 682b 6a83 0200 0068  '].h)].uh+j....h
+00002e40: 1b6a 8002 0000 7562 6168 1f7d 9428 6821  .j....ubah.}.(h!
+00002e50: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00002e60: 5d94 7568 2b6a 7e02 0000 681b 6a6b 0200  ].uh+j~...h.jk..
+00002e70: 0075 6265 681f 7d94 2868 215d 9468 235d  .ubeh.}.(h!].h#]
+00002e80: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+00002e90: 6a69 0200 0068 1b6a 6602 0000 7562 6a6a  ji...h.jf...ubjj
+00002ea0: 0200 0029 8194 7d94 2868 0568 0668 075d  ...)..}.(h.h.h.]
+00002eb0: 9428 6a6f 0200 0029 8194 7d94 2868 058c  .(jo...)..}.(h..
+00002ec0: 0b52 6574 7572 6e20 7479 7065 9468 075d  .Return type.h.]
+00002ed0: 9468 168c 0b52 6574 7572 6e20 7479 7065  .h...Return type
+00002ee0: 9485 9481 947d 9428 681b 6af5 0400 0068  .....}.(h.j....h
+00002ef0: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
+00002f00: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00002f10: 9468 295d 9475 682b 6a6e 0200 0068 1b6a  .h)].uh+jn...h.j
+00002f20: f204 0000 681d 687f 681e 4b00 7562 6a7f  ....h.h.h.K.ubj.
+00002f30: 0200 0029 8194 7d94 2868 0568 0668 075d  ...)..}.(h.h.h.]
+00002f40: 946a 3202 0000 2981 947d 9428 6805 8c3d  .j2...)..}.(h..=
+00002f50: 6c69 7374 2028 6f72 2067 656e 6572 6174  list (or generat
+00002f60: 6f72 2069 7465 7261 746f 7229 206f 6620  or iterator) of 
+00002f70: 7374 7269 6e67 2028 6f72 2064 6174 6574  string (or datet
+00002f80: 696d 652e 6461 7465 7469 6d65 2994 6807  ime.datetime).h.
+00002f90: 5d94 286a a602 0000 2981 947d 9428 6805  ].(j....)..}.(h.
+00002fa0: 6806 6807 5d94 6816 8c04 6c69 7374 9485  h.h.].h...list..
+00002fb0: 9481 947d 9428 681b 6a0a 0500 0068 1c68  ...}.(h.j....h.h
+00002fc0: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+00002fd0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+00002fe0: 295d 948c 0972 6566 646f 6d61 696e 946a  )]...refdomain.j
+00002ff0: c102 0000 8c0b 7265 6665 7870 6c69 6369  ......refexplici
+00003000: 7494 898c 0772 6566 7479 7065 946a 2602  t....reftype.j&.
+00003010: 0000 8c09 7265 6674 6172 6765 7494 8c04  ....reftarget...
+00003020: 6c69 7374 946a c502 0000 886a c602 0000  list.j.....j....
+00003030: 6a25 0200 006a c702 0000 4e75 682b 6aa5  j%...j....Nuh+j.
+00003040: 0200 0068 1b6a 0605 0000 7562 6816 8c05  ...h.j....ubh...
+00003050: 2028 6f72 2094 8594 8194 7d94 2868 1b6a   (or .....}.(h.j
+00003060: 0605 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
+00003070: 6aa6 0200 0029 8194 7d94 2868 0568 0668  j....)..}.(h.h.h
+00003080: 075d 9468 168c 1267 656e 6572 6174 6f72  .].h...generator
+00003090: 2069 7465 7261 746f 7294 8594 8194 7d94   iterator.....}.
+000030a0: 2868 1b6a 2005 0000 681c 6803 681d 4e68  (h.j ...h.h.h.Nh
+000030b0: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
+000030c0: 5d94 6825 5d94 6827 5d94 6829 5d94 8c09  ].h%].h'].h)]...
+000030d0: 7265 6664 6f6d 6169 6e94 6ac1 0200 008c  refdomain.j.....
+000030e0: 0b72 6566 6578 706c 6963 6974 9489 8c07  .refexplicit....
+000030f0: 7265 6674 7970 6594 6a26 0200 008c 0972  reftype.j&.....r
+00003100: 6566 7461 7267 6574 948c 1267 656e 6572  eftarget...gener
+00003110: 6174 6f72 2069 7465 7261 746f 7294 6ac5  ator iterator.j.
+00003120: 0200 0088 6ac6 0200 006a 2502 0000 6ac7  ....j....j%...j.
+00003130: 0200 004e 7568 2b6a a502 0000 681b 6a06  ...Nuh+j....h.j.
+00003140: 0500 0075 6268 168c 0529 206f 6620 9485  ...ubh...) of ..
+00003150: 9481 947d 9428 681b 6a06 0500 0068 1c68  ...}.(h.j....h.h
+00003160: 0368 1d4e 681e 4e75 626a a602 0000 2981  .h.Nh.Nubj....).
+00003170: 947d 9428 6805 6806 6807 5d94 6816 8c06  .}.(h.h.h.].h...
+00003180: 7374 7269 6e67 9485 9481 947d 9428 681b  string.....}.(h.
+00003190: 6a36 0500 0068 1c68 0368 1d4e 681e 4e75  j6...h.h.h.Nh.Nu
+000031a0: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+000031b0: 255d 9468 275d 9468 295d 948c 0972 6566  %].h'].h)]...ref
+000031c0: 646f 6d61 696e 946a c102 0000 8c0b 7265  domain.j......re
+000031d0: 6665 7870 6c69 6369 7494 898c 0772 6566  fexplicit....ref
+000031e0: 7479 7065 946a 2602 0000 8c09 7265 6674  type.j&.....reft
+000031f0: 6172 6765 7494 8c06 7374 7269 6e67 946a  arget...string.j
+00003200: c502 0000 886a c602 0000 6a25 0200 006a  .....j....j%...j
+00003210: c702 0000 4e75 682b 6aa5 0200 0068 1b6a  ....Nuh+j....h.j
+00003220: 0605 0000 7562 6816 8c05 2028 6f72 2094  ....ubh... (or .
+00003230: 8594 8194 7d94 681b 6a06 0500 0073 626a  ....}.h.j....sbj
+00003240: a602 0000 2981 947d 9428 6805 6806 6807  ....)..}.(h.h.h.
+00003250: 5d94 6816 8c11 6461 7465 7469 6d65 2e64  ].h...datetime.d
+00003260: 6174 6574 696d 6594 8594 8194 7d94 2868  atetime.....}.(h
+00003270: 1b6a 4c05 0000 681c 6803 681d 4e68 1e4e  .jL...h.h.h.Nh.N
+00003280: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00003290: 6825 5d94 6827 5d94 6829 5d94 8c09 7265  h%].h'].h)]...re
+000032a0: 6664 6f6d 6169 6e94 6ac1 0200 008c 0b72  fdomain.j......r
+000032b0: 6566 6578 706c 6963 6974 9489 8c07 7265  efexplicit....re
+000032c0: 6674 7970 6594 6a26 0200 008c 0972 6566  ftype.j&.....ref
+000032d0: 7461 7267 6574 948c 1164 6174 6574 696d  target...datetim
+000032e0: 652e 6461 7465 7469 6d65 946a c502 0000  e.datetime.j....
+000032f0: 886a c602 0000 6a25 0200 006a c702 0000  .j....j%...j....
+00003300: 4e75 682b 6aa5 0200 0068 1b6a 0605 0000  Nuh+j....h.j....
+00003310: 7562 6816 8c01 2994 8594 8194 7d94 2868  ubh...).....}.(h
+00003320: 1b6a 0605 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
+00003330: 7562 6568 1f7d 9428 6821 5d94 6823 5d94  ubeh.}.(h!].h#].
+00003340: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
+00003350: 3102 0000 681b 6a03 0500 0075 6261 681f  1...h.j....ubah.
+00003360: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00003370: 275d 9468 295d 9475 682b 6a7e 0200 0068  '].h)].uh+j~...h
+00003380: 1b6a f204 0000 7562 6568 1f7d 9428 6821  .j....ubeh.}.(h!
+00003390: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+000033a0: 5d94 7568 2b6a 6902 0000 681b 6a66 0200  ].uh+ji...h.jf..
+000033b0: 0075 6265 681f 7d94 2868 215d 9468 235d  .ubeh.}.(h!].h#]
+000033c0: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+000033d0: 6a64 0200 0068 1b6a 2e02 0000 681c 6803  jd...h.j....h.h.
+000033e0: 681d 4e68 1e4e 7562 6568 1f7d 9428 6821  h.Nh.Nubeh.}.(h!
+000033f0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00003400: 5d94 7568 2b6a 2c02 0000 681b 6862 681c  ].uh+j,...h.hbh.
+00003410: 6803 681d 687f 681e 4b01 7562 6568 1f7d  h.h.h.h.K.ubeh.}
+00003420: 9428 6821 5d94 6823 5d94 286a c102 0000  .(h!].h#].(j....
+00003430: 8c08 6675 6e63 7469 6f6e 9465 6825 5d94  ..function.eh%].
+00003440: 6827 5d94 6829 5d94 8c06 646f 6d61 696e  h'].h)]...domain
+00003450: 946a c102 0000 8c07 6f62 6a74 7970 6594  .j......objtype.
+00003460: 6a83 0500 008c 0864 6573 6374 7970 6594  j......desctype.
+00003470: 6a83 0500 008c 076e 6f69 6e64 6578 9489  j......noindex..
+00003480: 8c0c 6e6f 696e 6465 7865 6e74 7279 9489  ..noindexentry..
+00003490: 8c0f 6e6f 636f 6e74 656e 7473 656e 7472  ..nocontentsentr
+000034a0: 7994 8975 682b 6860 681c 6803 681b 683e  y..uh+h`h.h.h.h>
+000034b0: 681d 4e68 1e4e 7562 6a32 0200 0029 8194  h.Nh.Nubj2...)..
+000034c0: 7d94 2868 058c 0b2a 2a45 7861 6d70 6c65  }.(h...**Example
+000034d0: 2a2a 9468 075d 946a c104 0000 2981 947d  **.h.].j....)..}
+000034e0: 9428 6805 6a8f 0500 0068 075d 9468 168c  .(h.j....h.].h..
+000034f0: 0745 7861 6d70 6c65 9485 9481 947d 9428  .Example.....}.(
+00003500: 681b 6a91 0500 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
+00003510: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
+00003520: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+00003530: 6ac0 0400 0068 1b6a 8d05 0000 7562 6168  j....h.j....ubah
+00003540: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+00003550: 6827 5d94 6829 5d94 7568 2b6a 3102 0000  h'].h)].uh+j1...
+00003560: 681d 682c 681e 4b0c 681b 683e 681c 6803  h.h,h.K.h.h>h.h.
+00003570: 7562 6a32 0200 0029 8194 7d94 2868 058c  ubj2...)..}.(h..
+00003580: 2641 6e20 6578 616d 706c 6520 6f66 2069  &An example of i
+00003590: 6e63 7265 6d65 6e74 696e 6720 6279 206f  ncrementing by o
+000035a0: 6e65 2064 6179 2e94 6807 5d94 6816 8c26  ne day..h.].h..&
+000035b0: 416e 2065 7861 6d70 6c65 206f 6620 696e  An example of in
+000035c0: 6372 656d 656e 7469 6e67 2062 7920 6f6e  crementing by on
+000035d0: 6520 6461 792e 9485 9481 947d 9428 681b  e day......}.(h.
+000035e0: 6aa4 0500 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
+000035f0: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+00003600: 255d 9468 275d 9468 295d 9475 682b 6a31  %].h'].h)].uh+j1
+00003610: 0200 0068 1d68 2c68 1e4b 0e68 1b68 3e68  ...h.h,h.K.h.h>h
+00003620: 1c68 0375 6268 098c 0d6c 6974 6572 616c  .h.ubh...literal
+00003630: 5f62 6c6f 636b 9493 9429 8194 7d94 2868  _block...)..}.(h
+00003640: 058c ac69 6d70 6f72 7420 636f 6f6b 6965  ...import cookie
+00003650: 735f 7574 696c 6974 6965 7320 6173 2063  s_utilities as c
+00003660: 750a 6461 7465 7320 3d20 6375 2e67 6574  u.dates = cu.get
+00003670: 5f64 6174 6573 280a 2020 2020 7374 6172  _dates(.    star
+00003680: 743d 2732 3031 362f 3037 2f30 3127 2c20  t='2016/07/01', 
+00003690: 656e 643d 2732 3031 362f 3037 2f30 3327  end='2016/07/03'
+000036a0: 2c20 666f 726d 6174 3d27 2559 2f25 6d2f  , format='%Y/%m/
+000036b0: 2564 272c 0a20 2020 2064 656c 7461 3d7b  %d',.    delta={
+000036c0: 2764 6179 7327 3a20 317d 2c20 666f 726d  'days': 1}, form
+000036d0: 6174 5f6f 7574 3d27 2559 2d25 6d2d 2564  at_out='%Y-%m-%d
+000036e0: 2729 0a70 7269 6e74 2864 6174 6573 2994  ').print(dates).
+000036f0: 6807 5d94 6816 8cac 696d 706f 7274 2063  h.].h...import c
+00003700: 6f6f 6b69 6573 5f75 7469 6c69 7469 6573  ookies_utilities
+00003710: 2061 7320 6375 0a64 6174 6573 203d 2063   as cu.dates = c
+00003720: 752e 6765 745f 6461 7465 7328 0a20 2020  u.get_dates(.   
+00003730: 2073 7461 7274 3d27 3230 3136 2f30 372f   start='2016/07/
+00003740: 3031 272c 2065 6e64 3d27 3230 3136 2f30  01', end='2016/0
+00003750: 372f 3033 272c 2066 6f72 6d61 743d 2725  7/03', format='%
+00003760: 592f 256d 2f25 6427 2c0a 2020 2020 6465  Y/%m/%d',.    de
+00003770: 6c74 613d 7b27 6461 7973 273a 2031 7d2c  lta={'days': 1},
+00003780: 2066 6f72 6d61 745f 6f75 743d 2725 592d   format_out='%Y-
+00003790: 256d 2d25 6427 290a 7072 696e 7428 6461  %m-%d').print(da
+000037a0: 7465 7329 9485 9481 947d 9468 1b6a b405  tes).....}.h.j..
+000037b0: 0000 7362 6168 1f7d 9428 6821 5d94 6823  ..sbah.}.(h!].h#
+000037c0: 5d94 6825 5d94 6827 5d94 6829 5d94 687d  ].h%].h'].h)].h}
+000037d0: 687e 8c05 666f 7263 6594 898c 086c 616e  h~..force....lan
+000037e0: 6775 6167 6594 8c06 7079 7468 6f6e 948c  guage...python..
+000037f0: 0e68 6967 686c 6967 6874 5f61 7267 7394  .highlight_args.
+00003800: 7d94 7568 2b6a b205 0000 681d 682c 681e  }.uh+j....h.h,h.
+00003810: 4b10 681b 683e 681c 6803 7562 6ab3 0500  K.h.h>h.h.ubj...
+00003820: 0029 8194 7d94 2868 058c 2a5b 2732 3031  .)..}.(h..*['201
+00003830: 362d 3037 2d30 3127 2c20 2732 3031 362d  6-07-01', '2016-
+00003840: 3037 2d30 3227 2c20 2732 3031 362d 3037  07-02', '2016-07
+00003850: 2d30 3327 5d94 6807 5d94 6816 8c2a 5b27  -03'].h.].h..*['
+00003860: 3230 3136 2d30 372d 3031 272c 2027 3230  2016-07-01', '20
+00003870: 3136 2d30 372d 3032 272c 2027 3230 3136  16-07-02', '2016
+00003880: 2d30 372d 3033 275d 9485 9481 947d 9468  -07-03'].....}.h
+00003890: 1b6a c705 0000 7362 6168 1f7d 9428 6821  .j....sbah.}.(h!
+000038a0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+000038b0: 5d94 687d 687e 6ac2 0500 0089 6ac3 0500  ].h}h~j.....j...
+000038c0: 008c 0763 6f6e 736f 6c65 946a c505 0000  ...console.j....
+000038d0: 7d94 7568 2b6a b205 0000 681d 682c 681e  }.uh+j....h.h,h.
+000038e0: 4b18 681b 683e 681c 6803 7562 6a32 0200  K.h.h>h.h.ubj2..
+000038f0: 0029 8194 7d94 2868 058c 2941 6e20 6578  .)..}.(h..)An ex
+00003900: 616d 706c 6520 6f66 2069 6e63 7265 6d65  ample of increme
+00003910: 6e74 696e 6720 6279 2032 3020 6d69 6e75  nting by 20 minu
+00003920: 7465 732e 9468 075d 9468 168c 2941 6e20  tes..h.].h..)An 
+00003930: 6578 616d 706c 6520 6f66 2069 6e63 7265  example of incre
+00003940: 6d65 6e74 696e 6720 6279 2032 3020 6d69  menting by 20 mi
+00003950: 6e75 7465 732e 9485 9481 947d 9428 681b  nutes......}.(h.
+00003960: 6ad7 0500 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
+00003970: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+00003980: 255d 9468 275d 9468 295d 9475 682b 6a31  %].h'].h)].uh+j1
+00003990: 0200 0068 1d68 2c68 1e4b 1c68 1b68 3e68  ...h.h,h.K.h.h>h
+000039a0: 1c68 0375 626a b305 0000 2981 947d 9428  .h.ubj....)..}.(
+000039b0: 6805 8cb8 696d 706f 7274 2063 6f6f 6b69  h...import cooki
+000039c0: 6573 5f75 7469 6c69 7469 6573 2061 7320  es_utilities as 
+000039d0: 6375 0a64 6174 6573 203d 2063 752e 6765  cu.dates = cu.ge
+000039e0: 745f 6461 7465 7328 0a20 2020 2073 7461  t_dates(.    sta
+000039f0: 7274 3d27 3230 3136 2d30 372d 3031 2030  rt='2016-07-01 0
+00003a00: 323a 3030 3a30 3027 2c20 656e 643d 2732  2:00:00', end='2
+00003a10: 3031 362d 3037 2d30 3120 3033 3a30 303a  016-07-01 03:00:
+00003a20: 3030 272c 0a20 2020 2066 6f72 6d61 743d  00',.    format=
+00003a30: 2725 592d 256d 2d25 6420 2548 3a25 4d3a  '%Y-%m-%d %H:%M:
+00003a40: 2553 272c 0a20 2020 2064 656c 7461 3d7b  %S',.    delta={
+00003a50: 276d 696e 7574 6573 273a 2032 307d 290a  'minutes': 20}).
+00003a60: 7072 696e 7428 6461 7465 7329 9468 075d  print(dates).h.]
+00003a70: 9468 168c b869 6d70 6f72 7420 636f 6f6b  .h...import cook
+00003a80: 6965 735f 7574 696c 6974 6965 7320 6173  ies_utilities as
+00003a90: 2063 750a 6461 7465 7320 3d20 6375 2e67   cu.dates = cu.g
+00003aa0: 6574 5f64 6174 6573 280a 2020 2020 7374  et_dates(.    st
+00003ab0: 6172 743d 2732 3031 362d 3037 2d30 3120  art='2016-07-01 
+00003ac0: 3032 3a30 303a 3030 272c 2065 6e64 3d27  02:00:00', end='
+00003ad0: 3230 3136 2d30 372d 3031 2030 333a 3030  2016-07-01 03:00
+00003ae0: 3a30 3027 2c0a 2020 2020 666f 726d 6174  :00',.    format
+00003af0: 3d27 2559 2d25 6d2d 2564 2025 483a 254d  ='%Y-%m-%d %H:%M
+00003b00: 3a25 5327 2c0a 2020 2020 6465 6c74 613d  :%S',.    delta=
+00003b10: 7b27 6d69 6e75 7465 7327 3a20 3230 7d29  {'minutes': 20})
+00003b20: 0a70 7269 6e74 2864 6174 6573 2994 8594  .print(dates)...
+00003b30: 8194 7d94 681b 6ae5 0500 0073 6261 681f  ..}.h.j....sbah.
+00003b40: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00003b50: 275d 9468 295d 9468 7d68 7e6a c205 0000  '].h)].h}h~j....
+00003b60: 896a c305 0000 8c06 7079 7468 6f6e 946a  .j......python.j
+00003b70: c505 0000 7d94 7568 2b6a b205 0000 681d  ....}.uh+j....h.
+00003b80: 682c 681e 4b1e 681b 683e 681c 6803 7562  h,h.K.h.h>h.h.ub
+00003b90: 6ab3 0500 0029 8194 7d94 2868 058c 5c5b  j....)..}.(h..\[
+00003ba0: 2732 3031 362d 3037 2d30 3120 3032 3a30  '2016-07-01 02:0
+00003bb0: 303a 3030 272c 2027 3230 3136 2d30 372d  0:00', '2016-07-
+00003bc0: 3031 2030 323a 3230 3a30 3027 2c20 2732  01 02:20:00', '2
+00003bd0: 3031 362d 3037 2d30 3120 3032 3a34 303a  016-07-01 02:40:
+00003be0: 3030 272c 2027 3230 3136 2d30 372d 3031  00', '2016-07-01
+00003bf0: 2030 333a 3030 3a30 3027 5d94 6807 5d94   03:00:00'].h.].
+00003c00: 6816 8c5c 5b27 3230 3136 2d30 372d 3031  h..\['2016-07-01
+00003c10: 2030 323a 3030 3a30 3027 2c20 2732 3031   02:00:00', '201
+00003c20: 362d 3037 2d30 3120 3032 3a32 303a 3030  6-07-01 02:20:00
+00003c30: 272c 2027 3230 3136 2d30 372d 3031 2030  ', '2016-07-01 0
+00003c40: 323a 3430 3a30 3027 2c20 2732 3031 362d  2:40:00', '2016-
+00003c50: 3037 2d30 3120 3033 3a30 303a 3030 275d  07-01 03:00:00']
+00003c60: 9485 9481 947d 9468 1b6a f505 0000 7362  .....}.h.j....sb
+00003c70: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00003c80: 5d94 6827 5d94 6829 5d94 687d 687e 6ac2  ].h'].h)].h}h~j.
+00003c90: 0500 0089 6ac3 0500 008c 0763 6f6e 736f  ....j......conso
+00003ca0: 6c65 946a c505 0000 7d94 7568 2b6a b205  le.j....}.uh+j..
+00003cb0: 0000 681d 682c 681e 4b27 681b 683e 681c  ..h.h,h.K'h.h>h.
+00003cc0: 6803 7562 6a32 0200 0029 8194 7d94 2868  h.ubj2...)..}.(h
+00003cd0: 058c 3141 6e20 6578 616d 706c 6520 6f66  ..1An example of
+00003ce0: 2072 6574 7269 6576 696e 6720 6173 2061   retrieving as a
+00003cf0: 2067 656e 6572 6174 6f72 2069 7465 7261   generator itera
+00003d00: 746f 722e 9468 075d 9468 168c 3141 6e20  tor..h.].h..1An 
+00003d10: 6578 616d 706c 6520 6f66 2072 6574 7269  example of retri
+00003d20: 6576 696e 6720 6173 2061 2067 656e 6572  eving as a gener
+00003d30: 6174 6f72 2069 7465 7261 746f 722e 9485  ator iterator...
+00003d40: 9481 947d 9428 681b 6a05 0600 0068 1c68  ...}.(h.j....h.h
+00003d50: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+00003d60: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+00003d70: 295d 9475 682b 6a31 0200 0068 1d68 2c68  )].uh+j1...h.h,h
+00003d80: 1e4b 2b68 1b68 3e68 1c68 0375 626a b305  .K+h.h>h.h.ubj..
+00003d90: 0000 2981 947d 9428 6805 8ccc 696d 706f  ..)..}.(h...impo
+00003da0: 7274 2063 6f6f 6b69 6573 5f75 7469 6c69  rt cookies_utili
+00003db0: 7469 6573 2061 7320 6375 0a64 6174 6573  ties as cu.dates
+00003dc0: 203d 2063 752e 6765 745f 6461 7465 7328   = cu.get_dates(
+00003dd0: 0a20 2020 2073 7461 7274 3d27 3230 3136  .    start='2016
+00003de0: 2f30 372f 3031 272c 2065 6e64 3d27 3230  /07/01', end='20
+00003df0: 3136 2f30 372f 3033 272c 2066 6f72 6d61  16/07/03', forma
+00003e00: 743d 2725 592f 256d 2f25 6427 2c0a 2020  t='%Y/%m/%d',.  
+00003e10: 2020 6465 6c74 613d 7b27 6461 7973 273a    delta={'days':
+00003e20: 2031 7d2c 2067 656e 6974 6572 3d54 7275   1}, geniter=Tru
+00003e30: 6529 0a70 7269 6e74 2874 7970 6528 6461  e).print(type(da
+00003e40: 7465 7329 290a 666f 7220 6461 7465 2069  tes)).for date i
+00003e50: 6e20 6461 7465 733a 0a20 2020 2070 7269  n dates:.    pri
+00003e60: 6e74 2864 6174 6529 9468 075d 9468 168c  nt(date).h.].h..
+00003e70: cc69 6d70 6f72 7420 636f 6f6b 6965 735f  .import cookies_
+00003e80: 7574 696c 6974 6965 7320 6173 2063 750a  utilities as cu.
+00003e90: 6461 7465 7320 3d20 6375 2e67 6574 5f64  dates = cu.get_d
+00003ea0: 6174 6573 280a 2020 2020 7374 6172 743d  ates(.    start=
+00003eb0: 2732 3031 362f 3037 2f30 3127 2c20 656e  '2016/07/01', en
+00003ec0: 643d 2732 3031 362f 3037 2f30 3327 2c20  d='2016/07/03', 
+00003ed0: 666f 726d 6174 3d27 2559 2f25 6d2f 2564  format='%Y/%m/%d
+00003ee0: 272c 0a20 2020 2064 656c 7461 3d7b 2764  ',.    delta={'d
+00003ef0: 6179 7327 3a20 317d 2c20 6765 6e69 7465  ays': 1}, genite
+00003f00: 723d 5472 7565 290a 7072 696e 7428 7479  r=True).print(ty
+00003f10: 7065 2864 6174 6573 2929 0a66 6f72 2064  pe(dates)).for d
+00003f20: 6174 6520 696e 2064 6174 6573 3a0a 2020  ate in dates:.  
+00003f30: 2020 7072 696e 7428 6461 7465 2994 8594    print(date)...
+00003f40: 8194 7d94 681b 6a13 0600 0073 6261 681f  ..}.h.j....sbah.
+00003f50: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00003f60: 275d 9468 295d 9468 7d68 7e6a c205 0000  '].h)].h}h~j....
+00003f70: 896a c305 0000 8c06 7079 7468 6f6e 946a  .j......python.j
+00003f80: c505 0000 7d94 7568 2b6a b205 0000 681d  ....}.uh+j....h.
+00003f90: 682c 681e 4b2d 681b 683e 681c 6803 7562  h,h.K-h.h>h.h.ub
+00003fa0: 6ab3 0500 0029 8194 7d94 2868 058c 343c  j....)..}.(h..4<
+00003fb0: 636c 6173 7320 2767 656e 6572 6174 6f72  class 'generator
+00003fc0: 273e 0a32 3031 362f 3037 2f30 310a 3230  '>.2016/07/01.20
+00003fd0: 3136 2f30 372f 3032 0a32 3031 362f 3037  16/07/02.2016/07
+00003fe0: 2f30 3394 6807 5d94 6816 8c34 3c63 6c61  /03.h.].h..4<cla
+00003ff0: 7373 2027 6765 6e65 7261 746f 7227 3e0a  ss 'generator'>.
+00004000: 3230 3136 2f30 372f 3031 0a32 3031 362f  2016/07/01.2016/
+00004010: 3037 2f30 320a 3230 3136 2f30 372f 3033  07/02.2016/07/03
+00004020: 9485 9481 947d 9468 1b6a 2306 0000 7362  .....}.h.j#...sb
+00004030: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00004040: 5d94 6827 5d94 6829 5d94 687d 687e 6ac2  ].h'].h)].h}h~j.
+00004050: 0500 0089 6ac3 0500 008c 0763 6f6e 736f  ....j......conso
+00004060: 6c65 946a c505 0000 7d94 7568 2b6a b205  le.j....}.uh+j..
+00004070: 0000 681d 682c 681e 4b37 681b 683e 681c  ..h.h,h.K7h.h>h.
+00004080: 6803 7562 6568 1f7d 9428 6821 5d94 8c1b  h.ubeh.}.(h!]...
+00004090: 636f 6f6b 6965 732d 7574 696c 6974 6965  cookies-utilitie
+000040a0: 732d 6765 742d 6461 7465 7394 6168 235d  s-get-dates.ah#]
+000040b0: 9468 255d 948c 1b63 6f6f 6b69 6573 5f75  .h%]...cookies_u
+000040c0: 7469 6c69 7469 6573 2e67 6574 5f64 6174  tilities.get_dat
+000040d0: 6573 9461 6827 5d94 6829 5d94 7568 2b68  es.ah'].h)].uh+h
+000040e0: 0a68 1b68 2d68 1c68 0368 1d68 2c68 1e4b  .h.h-h.h.h.h,h.K
+000040f0: 0875 6265 681f 7d94 2868 215d 948c 0966  .ubeh.}.(h!]...f
+00004100: 756e 6374 696f 6e73 9461 6823 5d94 6825  unctions.ah#].h%
+00004110: 5d94 8c09 6675 6e63 7469 6f6e 7394 6168  ]...functions.ah
+00004120: 275d 9468 295d 9475 682b 680a 681b 680c  '].h)].uh+h.h.h.
+00004130: 681c 6803 681d 682c 681e 4b05 7562 680b  h.h.h.h,h.K.ubh.
+00004140: 2981 947d 9428 6805 6806 6807 5d94 2868  )..}.(h.h.h.].(h
+00004150: 1029 8194 7d94 2868 058c 0743 6c61 7373  .)..}.(h...Class
+00004160: 6573 9468 075d 9468 168c 0743 6c61 7373  es.h.].h...Class
+00004170: 6573 9485 9481 947d 9428 681b 6a46 0600  es.....}.(h.jF..
+00004180: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
+00004190: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+000041a0: 275d 9468 295d 9475 682b 680f 681b 6a43  '].h)].uh+h.h.jC
+000041b0: 0600 0068 1c68 0368 1d68 2c68 1e4b 3f75  ...h.h.h.h,h.K?u
+000041c0: 6268 0b29 8194 7d94 2868 0568 0668 075d  bh.)..}.(h.h.h.]
+000041d0: 9428 6810 2981 947d 9428 6805 8c1b 636f  .(h.)..}.(h...co
+000041e0: 6f6b 6965 735f 7574 696c 6974 6965 732e  okies_utilities.
+000041f0: 5374 6f70 7761 7463 6894 6807 5d94 6816  Stopwatch.h.].h.
+00004200: 8c1b 636f 6f6b 6965 735f 7574 696c 6974  ..cookies_utilit
+00004210: 6965 732e 5374 6f70 7761 7463 6894 8594  ies.Stopwatch...
+00004220: 8194 7d94 2868 1b6a 5706 0000 681c 6803  ..}.(h.jW...h.h.
+00004230: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
+00004240: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00004250: 5d94 7568 2b68 0f68 1b6a 5406 0000 681c  ].uh+h.h.jT...h.
+00004260: 6803 681d 682c 681e 4b42 7562 6850 2981  h.h.h,h.KBubhP).
+00004270: 947d 9428 6805 6806 6807 5d94 681f 7d94  .}.(h.h.h.].h.}.
+00004280: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00004290: 9468 295d 948c 0765 6e74 7269 6573 945d  .h)]...entries.]
+000042a0: 9428 685c 8c26 5374 6f70 7761 7463 6820  .(h\.&Stopwatch 
+000042b0: 2863 6c61 7373 2069 6e20 636f 6f6b 6965  (class in cookie
+000042c0: 735f 7574 696c 6974 6965 7329 948c 1b63  s_utilities)...c
+000042d0: 6f6f 6b69 6573 5f75 7469 6c69 7469 6573  ookies_utilities
+000042e0: 2e53 746f 7077 6174 6368 9468 064e 7494  .Stopwatch.h.Nt.
+000042f0: 6175 682b 684f 681b 6a54 0600 0068 1c68  auh+hOh.jT...h.h
+00004300: 0368 1d4e 681e 4e75 6268 6129 8194 7d94  .h.Nh.Nubha)..}.
+00004310: 2868 0568 0668 075d 9428 6866 2981 947d  (h.h.h.].(hf)..}
+00004320: 9428 6805 8c0b 5374 6f70 7761 7463 6828  .(h...Stopwatch(
+00004330: 2994 6807 5d94 2868 008c 0f64 6573 635f  ).h.].(h...desc_
+00004340: 616e 6e6f 7461 7469 6f6e 9493 9429 8194  annotation...)..
+00004350: 7d94 2868 058c 325b 3c23 7465 7874 3a20  }.(h..2[<#text: 
+00004360: 2763 6c61 7373 273e 2c20 3c64 6573 635f  'class'>, <desc_
+00004370: 7369 675f 7370 6163 653a 203c 2374 6578  sig_space: <#tex
+00004380: 743a 2027 2027 3e3e 5d94 6807 5d94 2868  t: ' '>>].h.].(h
+00004390: 168c 0563 6c61 7373 9485 9481 947d 9428  ...class.....}.(
+000043a0: 681b 6a7c 0600 0068 1c68 0368 1d4e 681e  h.j|...h.h.h.Nh.
+000043b0: 4e75 6268 008c 0e64 6573 635f 7369 675f  Nubh...desc_sig_
+000043c0: 7370 6163 6594 9394 2981 947d 9428 6805  space...)..}.(h.
+000043d0: 8c01 2094 6807 5d94 6816 8c01 2094 8594  .. .h.].h... ...
+000043e0: 8194 7d94 2868 1b6a 8606 0000 681c 6803  ..}.(h.j....h.h.
+000043f0: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
+00004400: 5d94 6823 5d94 8c01 7794 6168 255d 9468  ].h#]...w.ah%].h
+00004410: 275d 9468 295d 9475 682b 6a84 0600 0068  '].h)].uh+j....h
+00004420: 1b6a 7c06 0000 7562 6568 1f7d 9428 6821  .j|...ubeh.}.(h!
+00004430: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00004440: 5d94 687d 687e 7568 2b6a 7a06 0000 681b  ].h}h~uh+jz...h.
+00004450: 6a76 0600 0068 1c68 0368 1d8c 7c43 3a5c  jv...h.h.h..|C:\
+00004460: 5573 6572 735c 632d 6d69 685c 7370 6163  Users\c-mih\spac
+00004470: 655c 636f 6f6b 6965 735f 7574 696c 6974  e\cookies_utilit
+00004480: 6965 735c 7372 635c 636f 6f6b 6965 735f  ies\src\cookies_
+00004490: 7574 696c 6974 6965 735c 7374 6f70 7761  utilities\stopwa
+000044a0: 7463 682e 7079 3a64 6f63 7374 7269 6e67  tch.py:docstring
+000044b0: 206f 6620 636f 6f6b 6965 735f 7574 696c   of cookies_util
+000044c0: 6974 6965 732e 7374 6f70 7761 7463 682e  ities.stopwatch.
+000044d0: 5374 6f70 7761 7463 6894 681e 4b01 7562  Stopwatch.h.K.ub
+000044e0: 686c 2981 947d 9428 6805 8c12 636f 6f6b  hl)..}.(h...cook
+000044f0: 6965 735f 7574 696c 6974 6965 732e 9468  ies_utilities..h
+00004500: 075d 9468 168c 1263 6f6f 6b69 6573 5f75  .].h...cookies_u
+00004510: 7469 6c69 7469 6573 2e94 8594 8194 7d94  tilities......}.
+00004520: 2868 1b6a 9c06 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
+00004530: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
+00004540: 5d94 2868 7868 7965 6825 5d94 6827 5d94  ].(hxhyeh%].h'].
+00004550: 6829 5d94 687d 687e 7568 2b68 6b68 1b6a  h)].h}h~uh+hkh.j
+00004560: 7606 0000 681c 6803 681d 6a9b 0600 0068  v...h.h.h.j....h
+00004570: 1e4b 0175 6268 8129 8194 7d94 2868 058c  .K.ubh.)..}.(h..
+00004580: 0953 746f 7077 6174 6368 9468 075d 9468  .Stopwatch.h.].h
+00004590: 168c 0953 746f 7077 6174 6368 9485 9481  ...Stopwatch....
+000045a0: 947d 9428 681b 6aaa 0600 0068 1c68 0368  .}.(h.j....h.h.h
+000045b0: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
+000045c0: 9468 235d 9428 688d 688e 6568 255d 9468  .h#].(h.h.eh%].h
+000045d0: 275d 9468 295d 9468 7d68 7e75 682b 6880  '].h)].h}h~uh+h.
+000045e0: 681b 6a76 0600 0068 1c68 0368 1d6a 9b06  h.jv...h.h.h.j..
+000045f0: 0000 681e 4b01 7562 6568 1f7d 9428 6821  ..h.K.ubeh.}.(h!
+00004600: 5d94 6a71 0600 0061 6823 5d94 286a 1f02  ].jq...ah#].(j..
+00004610: 0000 6a20 0200 0065 6825 5d94 6827 5d94  ..j ...eh%].h'].
+00004620: 6829 5d94 6a24 0200 008c 1163 6f6f 6b69  h)].j$.....cooki
+00004630: 6573 5f75 7469 6c69 7469 6573 946a 2602  es_utilities.j&.
+00004640: 0000 6806 6a27 0200 006a ac06 0000 6a28  ..h.j'...j....j(
+00004650: 0200 006a be06 0000 6aac 0600 0086 946a  ...j....j......j
+00004660: 2a02 0000 6aac 0600 0075 682b 6865 681d  *...j....uh+heh.
+00004670: 6a9b 0600 0068 1e4b 0168 1b6a 7306 0000  j....h.K.h.js...
+00004680: 681c 6803 7562 6a2d 0200 0029 8194 7d94  h.h.ubj-...)..}.
+00004690: 2868 0568 0668 075d 9428 6a32 0200 0029  (h.h.h.].(j2...)
+000046a0: 8194 7d94 2868 058c 2853 746f 7077 6174  ..}.(h..(Stopwat
+000046b0: 6368 2066 6f72 206d 6561 7375 7269 6e67  ch for measuring
+000046c0: 2070 726f 6365 7373 696e 6720 7469 6d65   processing time
+000046d0: 2e94 6807 5d94 6816 8c28 5374 6f70 7761  ..h.].h..(Stopwa
+000046e0: 7463 6820 666f 7220 6d65 6173 7572 696e  tch for measurin
+000046f0: 6720 7072 6f63 6573 7369 6e67 2074 696d  g processing tim
+00004700: 652e 9485 9481 947d 9428 681b 6ac3 0600  e......}.(h.j...
+00004710: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
+00004720: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00004730: 275d 9468 295d 9475 682b 6a31 0200 0068  '].h)].uh+j1...h
+00004740: 1d8c 7c43 3a5c 5573 6572 735c 632d 6d69  ..|C:\Users\c-mi
+00004750: 685c 7370 6163 655c 636f 6f6b 6965 735f  h\space\cookies_
+00004760: 7574 696c 6974 6965 735c 7372 635c 636f  utilities\src\co
+00004770: 6f6b 6965 735f 7574 696c 6974 6965 735c  okies_utilities\
+00004780: 7374 6f70 7761 7463 682e 7079 3a64 6f63  stopwatch.py:doc
+00004790: 7374 7269 6e67 206f 6620 636f 6f6b 6965  string of cookie
+000047a0: 735f 7574 696c 6974 6965 732e 7374 6f70  s_utilities.stop
+000047b0: 7761 7463 682e 5374 6f70 7761 7463 6894  watch.Stopwatch.
+000047c0: 681e 4b01 681b 6ac0 0600 0068 1c68 0375  h.K.h.j....h.h.u
+000047d0: 6268 5029 8194 7d94 2868 0568 0668 075d  bhP)..}.(h.h.h.]
+000047e0: 9468 1f7d 9428 6821 5d94 6823 5d94 6825  .h.}.(h!].h#].h%
+000047f0: 5d94 6827 5d94 6829 5d94 8c07 656e 7472  ].h'].h)]...entr
+00004800: 6965 7394 5d94 2868 5c8c 2c70 7265 7373  ies.].(h\.,press
+00004810: 2829 2028 636f 6f6b 6965 735f 7574 696c  () (cookies_util
+00004820: 6974 6965 732e 5374 6f70 7761 7463 6820  ities.Stopwatch 
+00004830: 6d65 7468 6f64 2994 8c21 636f 6f6b 6965  method)..!cookie
+00004840: 735f 7574 696c 6974 6965 732e 5374 6f70  s_utilities.Stop
+00004850: 7761 7463 682e 7072 6573 7394 6806 4e74  watch.press.h.Nt
+00004860: 9461 7568 2b68 4f68 1b6a c006 0000 681c  .auh+hOh.j....h.
+00004870: 6803 681d 4e68 1e4e 7562 6861 2981 947d  h.h.Nh.Nubha)..}
+00004880: 9428 6805 6806 6807 5d94 2868 6629 8194  .(h.h.h.].(hf)..
+00004890: 7d94 2868 058c 1753 746f 7077 6174 6368  }.(h...Stopwatch
+000048a0: 2e70 7265 7373 286b 6579 3d27 2729 9468  .press(key='').h
+000048b0: 075d 9428 6881 2981 947d 9428 6805 8c05  .].(h.)..}.(h...
+000048c0: 7072 6573 7394 6807 5d94 6816 8c05 7072  press.h.].h...pr
+000048d0: 6573 7394 8594 8194 7d94 2868 1b6a e706  ess.....}.(h.j..
+000048e0: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
+000048f0: 1f7d 9428 6821 5d94 6823 5d94 2868 8d68  .}.(h!].h#].(h.h
+00004900: 8e65 6825 5d94 6827 5d94 6829 5d94 687d  .eh%].h'].h)].h}
+00004910: 687e 7568 2b68 8068 1b6a e306 0000 681c  h~uh+h.h.j....h.
+00004920: 6803 681d 8c82 433a 5c55 7365 7273 5c63  h.h...C:\Users\c
+00004930: 2d6d 6968 5c73 7061 6365 5c63 6f6f 6b69  -mih\space\cooki
+00004940: 6573 5f75 7469 6c69 7469 6573 5c73 7263  es_utilities\src
+00004950: 5c63 6f6f 6b69 6573 5f75 7469 6c69 7469  \cookies_utiliti
+00004960: 6573 5c73 746f 7077 6174 6368 2e70 793a  es\stopwatch.py:
+00004970: 646f 6373 7472 696e 6720 6f66 2063 6f6f  docstring of coo
+00004980: 6b69 6573 5f75 7469 6c69 7469 6573 2e73  kies_utilities.s
+00004990: 746f 7077 6174 6368 2e53 746f 7077 6174  topwatch.Stopwat
+000049a0: 6368 2e70 7265 7373 9468 1e4b 0175 6268  ch.press.h.K.ubh
+000049b0: 9329 8194 7d94 2868 058c 066b 6579 3d27  .)..}.(h...key='
+000049c0: 2794 6807 5d94 6899 2981 947d 9428 6805  '.h.].h.)..}.(h.
+000049d0: 8c06 6b65 793d 2727 9468 075d 9428 689f  ..key=''.h.].(h.
+000049e0: 2981 947d 9428 6805 8c03 6b65 7994 6807  )..}.(h...key.h.
+000049f0: 5d94 6816 8c03 6b65 7994 8594 8194 7d94  ].h...key.....}.
+00004a00: 2868 1b6a fe06 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
+00004a10: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
+00004a20: 5d94 68ab 6168 255d 9468 275d 9468 295d  ].h.ah%].h'].h)]
+00004a30: 9475 682b 689e 681b 6afa 0600 0075 6268  .uh+h.h.j....ubh
+00004a40: b029 8194 7d94 2868 058c 013d 9468 075d  .)..}.(h...=.h.]
+00004a50: 9468 168c 013d 9485 9481 947d 9428 681b  .h...=.....}.(h.
+00004a60: 6a0c 0700 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
+00004a70: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+00004a80: bc61 6825 5d94 6827 5d94 6829 5d94 7568  .ah%].h'].h)].uh
+00004a90: 2b68 af68 1b6a fa06 0000 7562 68c1 2981  +h.h.j....ubh.).
+00004aa0: 947d 9428 6805 8c02 2727 9468 075d 9468  .}.(h...''.h.].h
+00004ab0: 168c 0227 2794 8594 8194 7d94 2868 1b6a  ...''.....}.(h.j
+00004ac0: 1a07 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
+00004ad0: 6168 1f7d 9428 6821 5d94 6823 5d94 68cd  ah.}.(h!].h#].h.
+00004ae0: 6168 255d 9468 275d 9468 295d 948c 1373  ah%].h'].h)]...s
+00004af0: 7570 706f 7274 5f73 6d61 7274 7175 6f74  upport_smartquot
+00004b00: 6573 9489 7568 2b68 c068 1b6a fa06 0000  es..uh+h.h.j....
+00004b10: 7562 6568 1f7d 9428 6821 5d94 6823 5d94  ubeh.}.(h!].h#].
+00004b20: 6825 5d94 6827 5d94 6829 5d94 687d 687e  h%].h'].h)].h}h~
+00004b30: 7568 2b68 9868 1b6a f606 0000 7562 6168  uh+h.h.j....ubah
+00004b40: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+00004b50: 6827 5d94 6829 5d94 687d 687e 7568 2b68  h'].h)].h}h~uh+h
+00004b60: 9268 1b6a e306 0000 681c 6803 681d 6af5  .h.j....h.h.h.j.
+00004b70: 0600 0068 1e4b 0175 6265 681f 7d94 2868  ...h.K.ubeh.}.(h
+00004b80: 215d 946a de06 0000 6168 235d 9428 6a1f  !].j....ah#].(j.
+00004b90: 0200 006a 2002 0000 6568 255d 9468 275d  ...j ...eh%].h']
+00004ba0: 9468 295d 946a 2402 0000 8c11 636f 6f6b  .h)].j$.....cook
+00004bb0: 6965 735f 7574 696c 6974 6965 7394 6a26  ies_utilities.j&
+00004bc0: 0200 006a ac06 0000 6a27 0200 008c 0f53  ...j....j'.....S
+00004bd0: 746f 7077 6174 6368 2e70 7265 7373 946a  topwatch.press.j
+00004be0: 2802 0000 6a3b 0700 008c 0953 746f 7077  (...j;.....Stopw
+00004bf0: 6174 6368 948c 0570 7265 7373 9487 946a  atch...press...j
+00004c00: 2a02 0000 8c11 5374 6f70 7761 7463 682e  *.....Stopwatch.
+00004c10: 7072 6573 7328 2994 7568 2b68 6568 1d6a  press().uh+heh.j
+00004c20: f506 0000 681e 4b01 681b 6ae0 0600 0068  ....h.K.h.j....h
+00004c30: 1c68 0375 626a 2d02 0000 2981 947d 9428  .h.ubj-...)..}.(
+00004c40: 6805 6806 6807 5d94 286a 3202 0000 2981  h.h.h.].(j2...).
+00004c50: 947d 9428 6805 8c14 5072 6573 7320 7468  .}.(h...Press th
+00004c60: 6520 7374 6f70 7761 7463 682e 9468 075d  e stopwatch..h.]
+00004c70: 9468 168c 1450 7265 7373 2074 6865 2073  .h...Press the s
+00004c80: 746f 7077 6174 6368 2e94 8594 8194 7d94  topwatch......}.
+00004c90: 2868 1b6a 4407 0000 681c 6803 681d 4e68  (h.jD...h.h.h.Nh
+00004ca0: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
+00004cb0: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+00004cc0: 2b6a 3102 0000 681d 8c82 433a 5c55 7365  +j1...h...C:\Use
+00004cd0: 7273 5c63 2d6d 6968 5c73 7061 6365 5c63  rs\c-mih\space\c
+00004ce0: 6f6f 6b69 6573 5f75 7469 6c69 7469 6573  ookies_utilities
+00004cf0: 5c73 7263 5c63 6f6f 6b69 6573 5f75 7469  \src\cookies_uti
+00004d00: 6c69 7469 6573 5c73 746f 7077 6174 6368  lities\stopwatch
+00004d10: 2e70 793a 646f 6373 7472 696e 6720 6f66  .py:docstring of
+00004d20: 2063 6f6f 6b69 6573 5f75 7469 6c69 7469   cookies_utiliti
+00004d30: 6573 2e73 746f 7077 6174 6368 2e53 746f  es.stopwatch.Sto
+00004d40: 7077 6174 6368 2e70 7265 7373 9468 1e4b  pwatch.press.h.K
+00004d50: 0168 1b6a 4107 0000 681c 6803 7562 6a65  .h.jA...h.h.ubje
+00004d60: 0200 0029 8194 7d94 2868 0568 0668 075d  ...)..}.(h.h.h.]
+00004d70: 946a 6a02 0000 2981 947d 9428 6805 6806  .jj...)..}.(h.h.
+00004d80: 6807 5d94 286a 6f02 0000 2981 947d 9428  h.].(jo...)..}.(
+00004d90: 6805 8c0a 5061 7261 6d65 7465 7273 9468  h...Parameters.h
+00004da0: 075d 9468 168c 0a50 6172 616d 6574 6572  .].h...Parameter
+00004db0: 7394 8594 8194 7d94 2868 1b6a 5907 0000  s.....}.(h.jY...
+00004dc0: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
+00004dd0: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+00004de0: 5d94 6829 5d94 7568 2b6a 6e02 0000 681b  ].h)].uh+jn...h.
+00004df0: 6a56 0700 0068 1d6a f506 0000 681e 4b00  jV...h.j....h.K.
+00004e00: 7562 6a7f 0200 0029 8194 7d94 2868 0568  ubj....)..}.(h.h
+00004e10: 0668 075d 946a 3202 0000 2981 947d 9428  .h.].j2...)..}.(
+00004e20: 6805 8c38 6b65 7920 2873 7472 696e 6729  h..8key (string)
+00004e30: 202d 2d20 5468 6520 6964 656e 6669 6361   -- The idenfica
+00004e40: 746f 7220 666f 7220 7468 6520 7469 6d65  tor for the time
+00004e50: 2028 6f70 7469 6f6e 616c 292e 9468 075d   (optional)..h.]
+00004e60: 9428 6a92 0200 0029 8194 7d94 2868 058c  .(j....)..}.(h..
+00004e70: 036b 6579 9468 075d 9468 168c 036b 6579  .key.h.].h...key
+00004e80: 9485 9481 947d 9428 681b 6a6e 0700 0068  .....}.(h.jn...h
+00004e90: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
+00004ea0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00004eb0: 9468 295d 9475 682b 6a91 0200 0068 1b6a  .h)].uh+j....h.j
+00004ec0: 6a07 0000 7562 6816 8c02 2028 9485 9481  j...ubh... (....
+00004ed0: 947d 9428 681b 6a6a 0700 0068 1c68 0368  .}.(h.jj...h.h.h
+00004ee0: 1d4e 681e 4e75 626a a602 0000 2981 947d  .Nh.Nubj....)..}
+00004ef0: 9428 6805 6806 6807 5d94 6aab 0200 0029  .(h.h.h.].j....)
+00004f00: 8194 7d94 2868 058c 0673 7472 696e 6794  ..}.(h...string.
+00004f10: 6807 5d94 6816 8c06 7374 7269 6e67 9485  h.].h...string..
+00004f20: 9481 947d 9428 681b 6a83 0700 0068 1c68  ...}.(h.j....h.h
+00004f30: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+00004f40: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+00004f50: 295d 9475 682b 6aaa 0200 0068 1b6a 8007  )].uh+j....h.j..
+00004f60: 0000 7562 6168 1f7d 9428 6821 5d94 6823  ..ubah.}.(h!].h#
+00004f70: 5d94 6825 5d94 6827 5d94 6829 5d94 8c09  ].h%].h'].h)]...
+00004f80: 7265 6664 6f6d 6169 6e94 8c02 7079 948c  refdomain...py..
+00004f90: 0b72 6566 6578 706c 6963 6974 9489 8c07  .refexplicit....
+00004fa0: 7265 6674 7970 6594 6a26 0200 008c 0972  reftype.j&.....r
+00004fb0: 6566 7461 7267 6574 946a 8507 0000 6ac5  eftarget.j....j.
+00004fc0: 0200 0088 6ac6 0200 006a 3b07 0000 6ac7  ....j....j;...j.
+00004fd0: 0200 006a ac06 0000 7568 2b6a a502 0000  ...j....uh+j....
+00004fe0: 681b 6a6a 0700 0075 6268 168c 0129 9485  h.jj...ubh...)..
+00004ff0: 9481 947d 9428 681b 6a6a 0700 0068 1c68  ...}.(h.jj...h.h
+00005000: 0368 1d4e 681e 4e75 6268 168c 0520 e280  .h.Nh.Nubh... ..
+00005010: 9320 9485 9481 947d 9428 681b 6a6a 0700  . .....}.(h.jj..
+00005020: 0068 1c68 0368 1d4e 681e 4e75 6268 168c  .h.h.h.Nh.Nubh..
+00005030: 2854 6865 2069 6465 6e66 6963 6174 6f72  (The idenficator
+00005040: 2066 6f72 2074 6865 2074 696d 6520 286f   for the time (o
+00005050: 7074 696f 6e61 6c29 2e94 8594 8194 7d94  ptional)......}.
+00005060: 2868 1b6a 6a07 0000 681c 6803 681d 4e68  (h.jj...h.h.h.Nh
+00005070: 1e4e 7562 6568 1f7d 9428 6821 5d94 6823  .Nubeh.}.(h!].h#
+00005080: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+00005090: 2b6a 3102 0000 681b 6a67 0700 0075 6261  +j1...h.jg...uba
+000050a0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+000050b0: 9468 275d 9468 295d 9475 682b 6a7e 0200  .h'].h)].uh+j~..
+000050c0: 0068 1b6a 5607 0000 7562 6568 1f7d 9428  .h.jV...ubeh.}.(
+000050d0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+000050e0: 6829 5d94 7568 2b6a 6902 0000 681b 6a53  h)].uh+ji...h.jS
+000050f0: 0700 0075 6261 681f 7d94 2868 215d 9468  ...ubah.}.(h!].h
+00005100: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+00005110: 682b 6a64 0200 0068 1b6a 4107 0000 681c  h+jd...h.jA...h.
+00005120: 6803 681d 4e68 1e4e 7562 6568 1f7d 9428  h.h.Nh.Nubeh.}.(
+00005130: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+00005140: 6829 5d94 7568 2b6a 2c02 0000 681b 6ae0  h)].uh+j,...h.j.
+00005150: 0600 0068 1c68 0368 1d6a f506 0000 681e  ...h.h.h.j....h.
+00005160: 4b01 7562 6568 1f7d 9428 6821 5d94 6823  K.ubeh.}.(h!].h#
+00005170: 5d94 286a 9807 0000 8c06 6d65 7468 6f64  ].(j......method
+00005180: 9465 6825 5d94 6827 5d94 6829 5d94 6a87  .eh%].h'].h)].j.
+00005190: 0500 006a 9807 0000 6a88 0500 006a c907  ...j....j....j..
+000051a0: 0000 6a89 0500 006a c907 0000 6a8a 0500  ..j....j....j...
+000051b0: 0089 6a8b 0500 0089 6a8c 0500 0089 7568  ..j.....j.....uh
+000051c0: 2b68 6068 1c68 0368 1b6a c006 0000 681d  +h`h.h.h.j....h.
+000051d0: 4e68 1e4e 7562 6850 2981 947d 9428 6805  Nh.NubhP)..}.(h.
+000051e0: 6806 6807 5d94 681f 7d94 2868 215d 9468  h.h.].h.}.(h!].h
+000051f0: 235d 9468 255d 9468 275d 9468 295d 948c  #].h%].h'].h)]..
+00005200: 0765 6e74 7269 6573 945d 9428 685c 8c2b  .entries.].(h\.+
+00005210: 7368 6f77 2829 2028 636f 6f6b 6965 735f  show() (cookies_
+00005220: 7574 696c 6974 6965 732e 5374 6f70 7761  utilities.Stopwa
+00005230: 7463 6820 6d65 7468 6f64 2994 8c20 636f  tch method).. co
+00005240: 6f6b 6965 735f 7574 696c 6974 6965 732e  okies_utilities.
+00005250: 5374 6f70 7761 7463 682e 7368 6f77 9468  Stopwatch.show.h
+00005260: 064e 7494 6175 682b 684f 681b 6ac0 0600  .Nt.auh+hOh.j...
+00005270: 0068 1c68 0368 1d8c 8143 3a5c 5573 6572  .h.h.h...C:\User
+00005280: 735c 632d 6d69 685c 7370 6163 655c 636f  s\c-mih\space\co
+00005290: 6f6b 6965 735f 7574 696c 6974 6965 735c  okies_utilities\
+000052a0: 7372 635c 636f 6f6b 6965 735f 7574 696c  src\cookies_util
+000052b0: 6974 6965 735c 7374 6f70 7761 7463 682e  ities\stopwatch.
+000052c0: 7079 3a64 6f63 7374 7269 6e67 206f 6620  py:docstring of 
+000052d0: 636f 6f6b 6965 735f 7574 696c 6974 6965  cookies_utilitie
+000052e0: 732e 7374 6f70 7761 7463 682e 5374 6f70  s.stopwatch.Stop
+000052f0: 7761 7463 682e 7368 6f77 9468 1e4e 7562  watch.show.h.Nub
+00005300: 6861 2981 947d 9428 6805 6806 6807 5d94  ha)..}.(h.h.h.].
+00005310: 2868 6629 8194 7d94 2868 058c 1053 746f  (hf)..}.(h...Sto
+00005320: 7077 6174 6368 2e73 686f 7728 2994 6807  pwatch.show().h.
+00005330: 5d94 2868 8129 8194 7d94 2868 058c 0473  ].(h.)..}.(h...s
+00005340: 686f 7794 6807 5d94 6816 8c04 7368 6f77  how.h.].h...show
+00005350: 9485 9481 947d 9428 681b 6ae3 0700 0068  .....}.(h.j....h
+00005360: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
+00005370: 2868 215d 9468 235d 9428 688d 688e 6568  (h!].h#].(h.h.eh
+00005380: 255d 9468 275d 9468 295d 9468 7d68 7e75  %].h'].h)].h}h~u
+00005390: 682b 6880 681b 6adf 0700 0068 1c68 0368  h+h.h.j....h.h.h
+000053a0: 1d8c 8143 3a5c 5573 6572 735c 632d 6d69  ...C:\Users\c-mi
+000053b0: 685c 7370 6163 655c 636f 6f6b 6965 735f  h\space\cookies_
+000053c0: 7574 696c 6974 6965 735c 7372 635c 636f  utilities\src\co
+000053d0: 6f6b 6965 735f 7574 696c 6974 6965 735c  okies_utilities\
+000053e0: 7374 6f70 7761 7463 682e 7079 3a64 6f63  stopwatch.py:doc
+000053f0: 7374 7269 6e67 206f 6620 636f 6f6b 6965  string of cookie
+00005400: 735f 7574 696c 6974 6965 732e 7374 6f70  s_utilities.stop
+00005410: 7761 7463 682e 5374 6f70 7761 7463 682e  watch.Stopwatch.
+00005420: 7368 6f77 9468 1e4b 0175 6268 9329 8194  show.h.K.ubh.)..
+00005430: 7d94 2868 058c 0228 2994 6807 5d94 681f  }.(h...().h.].h.
+00005440: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00005450: 275d 9468 295d 9468 7d68 7e75 682b 6892  '].h)].h}h~uh+h.
+00005460: 681b 6adf 0700 0068 1c68 0368 1d6a f107  h.j....h.h.h.j..
+00005470: 0000 681e 4b01 7562 6568 1f7d 9428 6821  ..h.K.ubeh.}.(h!
+00005480: 5d94 6ad9 0700 0061 6823 5d94 286a 1f02  ].j....ah#].(j..
+00005490: 0000 6a20 0200 0065 6825 5d94 6827 5d94  ..j ...eh%].h'].
+000054a0: 6829 5d94 6a24 0200 008c 1163 6f6f 6b69  h)].j$.....cooki
+000054b0: 6573 5f75 7469 6c69 7469 6573 946a 2602  es_utilities.j&.
+000054c0: 0000 6aac 0600 006a 2702 0000 8c0e 5374  ..j....j'.....St
+000054d0: 6f70 7761 7463 682e 7368 6f77 946a 2802  opwatch.show.j(.
+000054e0: 0000 6a02 0800 008c 0953 746f 7077 6174  ..j......Stopwat
+000054f0: 6368 948c 0473 686f 7794 8794 6a2a 0200  ch...show...j*..
+00005500: 008c 1053 746f 7077 6174 6368 2e73 686f  ...Stopwatch.sho
+00005510: 7728 2994 7568 2b68 6568 1d6a f107 0000  w().uh+heh.j....
+00005520: 681e 4b01 681b 6adc 0700 0068 1c68 0375  h.K.h.j....h.h.u
+00005530: 626a 2d02 0000 2981 947d 9428 6805 6806  bj-...)..}.(h.h.
+00005540: 6807 5d94 6a32 0200 0029 8194 7d94 2868  h.].j2...)..}.(h
+00005550: 058c 0f53 686f 7720 6c61 7020 7469 6d65  ...Show lap time
+00005560: 732e 9468 075d 9468 168c 0f53 686f 7720  s..h.].h...Show 
+00005570: 6c61 7020 7469 6d65 732e 9485 9481 947d  lap times......}
+00005580: 9428 681b 6a0b 0800 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
+00005590: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
+000055a0: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+000055b0: 682b 6a31 0200 0068 1d6a db07 0000 681e  h+j1...h.j....h.
+000055c0: 4b01 681b 6a08 0800 0068 1c68 0375 6261  K.h.j....h.h.uba
+000055d0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+000055e0: 9468 275d 9468 295d 9475 682b 6a2c 0200  .h'].h)].uh+j,..
+000055f0: 0068 1b6a dc07 0000 681c 6803 681d 6af1  .h.j....h.h.h.j.
+00005600: 0700 0068 1e4b 0175 6265 681f 7d94 2868  ...h.K.ubeh.}.(h
+00005610: 215d 9468 235d 9428 8c02 7079 948c 066d  !].h#].(..py...m
+00005620: 6574 686f 6494 6568 255d 9468 275d 9468  ethod.eh%].h'].h
+00005630: 295d 946a 8705 0000 6a22 0800 006a 8805  )].j....j"...j..
+00005640: 0000 6a23 0800 006a 8905 0000 6a23 0800  ..j#...j....j#..
+00005650: 006a 8a05 0000 896a 8b05 0000 896a 8c05  .j.....j.....j..
+00005660: 0000 8975 682b 6860 681c 6803 681b 6ac0  ...uh+h`h.h.h.j.
+00005670: 0600 0068 1d6a db07 0000 681e 4e75 6265  ...h.j....h.Nube
+00005680: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00005690: 9468 275d 9468 295d 9475 682b 6a2c 0200  .h'].h)].uh+j,..
+000056a0: 0068 1b6a 7306 0000 681c 6803 681d 6a9b  .h.js...h.h.h.j.
+000056b0: 0600 0068 1e4b 0175 6265 681f 7d94 2868  ...h.K.ubeh.}.(h
+000056c0: 215d 9468 235d 9428 8c02 7079 948c 0563  !].h#].(..py...c
+000056d0: 6c61 7373 9465 6825 5d94 6827 5d94 6829  lass.eh%].h'].h)
+000056e0: 5d94 6a87 0500 006a 3008 0000 6a88 0500  ].j....j0...j...
+000056f0: 006a 3108 0000 6a89 0500 006a 3108 0000  .j1...j....j1...
+00005700: 6a8a 0500 0089 6a8b 0500 0089 6a8c 0500  j.....j.....j...
+00005710: 0089 7568 2b68 6068 1c68 0368 1b6a 5406  ..uh+h`h.h.h.jT.
+00005720: 0000 681d 4e68 1e4e 7562 6809 8c07 636f  ..h.Nh.Nubh...co
+00005730: 6d6d 656e 7494 9394 2981 947d 9428 6805  mment...)..}.(h.
+00005740: 8c12 3a73 686f 772d 696e 6865 7269 7461  ..:show-inherita
+00005750: 6e63 653a 9468 075d 9468 168c 123a 7368  nce:.h.].h...:sh
+00005760: 6f77 2d69 6e68 6572 6974 616e 6365 3a94  ow-inheritance:.
+00005770: 8594 8194 7d94 681b 6a37 0800 0073 6261  ....}.h.j7...sba
+00005780: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00005790: 9468 275d 9468 295d 9468 7d68 7e75 682b  .h'].h)].h}h~uh+
+000057a0: 6a35 0800 0068 1b6a 5406 0000 681c 6803  j5...h.jT...h.h.
+000057b0: 681d 682c 681e 4b49 7562 6a32 0200 0029  h.h,h.KIubj2...)
+000057c0: 8194 7d94 2868 058c 0b2a 2a45 7861 6d70  ..}.(h...**Examp
+000057d0: 6c65 2a2a 9468 075d 946a c104 0000 2981  le**.h.].j....).
+000057e0: 947d 9428 6805 6a47 0800 0068 075d 9468  .}.(h.jG...h.].h
+000057f0: 168c 0745 7861 6d70 6c65 9485 9481 947d  ...Example.....}
+00005800: 9428 681b 6a49 0800 0068 1c68 0368 1d4e  .(h.jI...h.h.h.N
+00005810: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
+00005820: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+00005830: 682b 6ac0 0400 0068 1b6a 4508 0000 7562  h+j....h.jE...ub
+00005840: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00005850: 5d94 6827 5d94 6829 5d94 7568 2b6a 3102  ].h'].h)].uh+j1.
+00005860: 0000 681d 682c 681e 4b4a 681b 6a54 0600  ..h.h,h.KJh.jT..
+00005870: 0068 1c68 0375 626a b305 0000 2981 947d  .h.h.ubj....)..}
+00005880: 9428 6805 8c8e 696d 706f 7274 2063 6f6f  .(h...import coo
+00005890: 6b69 6573 5f75 7469 6c69 7469 6573 2061  kies_utilities a
+000058a0: 7320 6375 0a73 7720 3d20 6375 2e53 746f  s cu.sw = cu.Sto
+000058b0: 7077 6174 6368 2829 0a73 772e 7072 6573  pwatch().sw.pres
+000058c0: 7328 2774 7261 696e 2073 7461 7274 2729  s('train start')
+000058d0: 0a23 2074 7261 696e 0a73 772e 7072 6573  .# train.sw.pres
+000058e0: 7328 2774 7261 696e 2065 6e64 2729 0a23  s('train end').#
+000058f0: 2074 6573 740a 7377 2e70 7265 7373 2827   test.sw.press('
+00005900: 7465 7374 2065 6e64 2729 0a73 772e 7368  test end').sw.sh
+00005910: 6f77 2829 9468 075d 9468 168c 8e69 6d70  ow().h.].h...imp
+00005920: 6f72 7420 636f 6f6b 6965 735f 7574 696c  ort cookies_util
+00005930: 6974 6965 7320 6173 2063 750a 7377 203d  ities as cu.sw =
+00005940: 2063 752e 5374 6f70 7761 7463 6828 290a   cu.Stopwatch().
+00005950: 7377 2e70 7265 7373 2827 7472 6169 6e20  sw.press('train 
+00005960: 7374 6172 7427 290a 2320 7472 6169 6e0a  start').# train.
+00005970: 7377 2e70 7265 7373 2827 7472 6169 6e20  sw.press('train 
+00005980: 656e 6427 290a 2320 7465 7374 0a73 772e  end').# test.sw.
+00005990: 7072 6573 7328 2774 6573 7420 656e 6427  press('test end'
+000059a0: 290a 7377 2e73 686f 7728 2994 8594 8194  ).sw.show().....
+000059b0: 7d94 681b 6a5c 0800 0073 6261 681f 7d94  }.h.j\...sbah.}.
+000059c0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+000059d0: 9468 295d 9468 7d68 7e6a c205 0000 896a  .h)].h}h~j.....j
+000059e0: c305 0000 8c06 7079 7468 6f6e 946a c505  ......python.j..
+000059f0: 0000 7d94 7568 2b6a b205 0000 681d 682c  ..}.uh+j....h.h,
+00005a00: 681e 4b4c 681b 6a54 0600 0068 1c68 0375  h.KLh.jT...h.h.u
+00005a10: 626a b305 0000 2981 947d 9428 6805 8c54  bj....)..}.(h..T
+00005a20: 7469 6d65 3128 7472 6169 6e20 7374 6172  time1(train star
+00005a30: 742d 7472 6169 6e20 656e 6429 3a20 322e  t-train end): 2.
+00005a40: 3030 3073 0a74 696d 6532 2874 7261 696e  000s.time2(train
+00005a50: 2065 6e64 2d74 6573 7420 656e 6429 3a20   end-test end): 
+00005a60: 312e 3030 3073 0a74 6f74 616c 3a20 332e  1.000s.total: 3.
+00005a70: 3030 3073 9468 075d 9468 168c 5474 696d  000s.h.].h..Ttim
+00005a80: 6531 2874 7261 696e 2073 7461 7274 2d74  e1(train start-t
+00005a90: 7261 696e 2065 6e64 293a 2032 2e30 3030  rain end): 2.000
+00005aa0: 730a 7469 6d65 3228 7472 6169 6e20 656e  s.time2(train en
+00005ab0: 642d 7465 7374 2065 6e64 293a 2031 2e30  d-test end): 1.0
+00005ac0: 3030 730a 746f 7461 6c3a 2033 2e30 3030  00s.total: 3.000
+00005ad0: 7394 8594 8194 7d94 681b 6a6c 0800 0073  s.....}.h.jl...s
+00005ae0: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+00005af0: 255d 9468 275d 9468 295d 9468 7d68 7e6a  %].h'].h)].h}h~j
+00005b00: c205 0000 896a c305 0000 8c07 636f 6e73  .....j......cons
+00005b10: 6f6c 6594 6ac5 0500 007d 9475 682b 6ab2  ole.j....}.uh+j.
+00005b20: 0500 0068 1d68 2c68 1e4b 5768 1b6a 5406  ...h.h,h.KWh.jT.
+00005b30: 0000 681c 6803 7562 6568 1f7d 9428 6821  ..h.h.ubeh.}.(h!
+00005b40: 5d94 8c1b 636f 6f6b 6965 732d 7574 696c  ]...cookies-util
+00005b50: 6974 6965 732d 7374 6f70 7761 7463 6894  ities-stopwatch.
+00005b60: 6168 235d 9468 255d 948c 1b63 6f6f 6b69  ah#].h%]...cooki
+00005b70: 6573 5f75 7469 6c69 7469 6573 2e73 746f  es_utilities.sto
+00005b80: 7077 6174 6368 9461 6827 5d94 6829 5d94  pwatch.ah'].h)].
+00005b90: 7568 2b68 0a68 1b6a 4306 0000 681c 6803  uh+h.h.jC...h.h.
+00005ba0: 681d 682c 681e 4b42 7562 6568 1f7d 9428  h.h,h.KBubeh.}.(
+00005bb0: 6821 5d94 8c07 636c 6173 7365 7394 6168  h!]...classes.ah
+00005bc0: 235d 9468 255d 948c 0763 6c61 7373 6573  #].h%]...classes
+00005bd0: 9461 6827 5d94 6829 5d94 7568 2b68 0a68  .ah'].h)].uh+h.h
+00005be0: 1b68 0c68 1c68 0368 1d68 2c68 1e4b 3f75  .h.h.h.h.h,h.K?u
+00005bf0: 6265 681f 7d94 2868 215d 948c 0d64 6f63  beh.}.(h!]...doc
+00005c00: 756d 656e 7461 7469 6f6e 9461 6823 5d94  umentation.ah#].
+00005c10: 6825 5d94 8c0d 646f 6375 6d65 6e74 6174  h%]...documentat
+00005c20: 696f 6e94 6168 275d 9468 295d 9475 682b  ion.ah'].h)].uh+
+00005c30: 680a 681b 6803 681c 6803 681d 682c 681e  h.h.h.h.h.h.h,h.
+00005c40: 4b02 7562 6168 1f7d 9428 6821 5d94 6823  K.ubah.}.(h!].h#
+00005c50: 5d94 6825 5d94 6827 5d94 6829 5d94 8c06  ].h%].h'].h)]...
+00005c60: 736f 7572 6365 9468 2c75 682b 6801 8c0e  source.h,uh+h...
+00005c70: 6375 7272 656e 745f 736f 7572 6365 944e  current_source.N
+00005c80: 8c0c 6375 7272 656e 745f 6c69 6e65 944e  ..current_line.N
+00005c90: 8c08 7365 7474 696e 6773 948c 1164 6f63  ..settings...doc
+00005ca0: 7574 696c 732e 6672 6f6e 7465 6e64 948c  utils.frontend..
+00005cb0: 0656 616c 7565 7394 9394 2981 947d 9428  .Values...)..}.(
+00005cc0: 680f 4e8c 0967 656e 6572 6174 6f72 944e  h.N..generator.N
+00005cd0: 8c09 6461 7465 7374 616d 7094 4e8c 0b73  ..datestamp.N..s
+00005ce0: 6f75 7263 655f 6c69 6e6b 944e 8c0a 736f  ource_link.N..so
+00005cf0: 7572 6365 5f75 726c 944e 8c0d 746f 635f  urce_url.N..toc_
+00005d00: 6261 636b 6c69 6e6b 7394 8c05 656e 7472  backlinks...entr
+00005d10: 7994 8c12 666f 6f74 6e6f 7465 5f62 6163  y...footnote_bac
+00005d20: 6b6c 696e 6b73 944b 018c 0d73 6563 746e  klinks.K...sectn
+00005d30: 756d 5f78 666f 726d 944b 018c 0e73 7472  um_xform.K...str
+00005d40: 6970 5f63 6f6d 6d65 6e74 7394 4e8c 1b73  ip_comments.N..s
+00005d50: 7472 6970 5f65 6c65 6d65 6e74 735f 7769  trip_elements_wi
+00005d60: 7468 5f63 6c61 7373 6573 944e 8c0d 7374  th_classes.N..st
+00005d70: 7269 705f 636c 6173 7365 7394 4e8c 0c72  rip_classes.N..r
+00005d80: 6570 6f72 745f 6c65 7665 6c94 4b02 8c0a  eport_level.K...
+00005d90: 6861 6c74 5f6c 6576 656c 944b 058c 1165  halt_level.K...e
+00005da0: 7869 745f 7374 6174 7573 5f6c 6576 656c  xit_status_level
+00005db0: 944b 058c 0564 6562 7567 944e 8c0e 7761  .K...debug.N..wa
+00005dc0: 726e 696e 675f 7374 7265 616d 944e 8c09  rning_stream.N..
+00005dd0: 7472 6163 6562 6163 6b94 888c 0e69 6e70  traceback....inp
+00005de0: 7574 5f65 6e63 6f64 696e 6794 8c09 7574  ut_encoding...ut
+00005df0: 662d 382d 7369 6794 8c1c 696e 7075 745f  f-8-sig...input_
+00005e00: 656e 636f 6469 6e67 5f65 7272 6f72 5f68  encoding_error_h
+00005e10: 616e 646c 6572 948c 0673 7472 6963 7494  andler...strict.
+00005e20: 8c0f 6f75 7470 7574 5f65 6e63 6f64 696e  ..output_encodin
+00005e30: 6794 8c05 7574 662d 3894 8c1d 6f75 7470  g...utf-8...outp
+00005e40: 7574 5f65 6e63 6f64 696e 675f 6572 726f  ut_encoding_erro
+00005e50: 725f 6861 6e64 6c65 7294 6ab7 0800 008c  r_handler.j.....
+00005e60: 0e65 7272 6f72 5f65 6e63 6f64 696e 6794  .error_encoding.
+00005e70: 8c05 7574 662d 3894 8c1c 6572 726f 725f  ..utf-8...error_
+00005e80: 656e 636f 6469 6e67 5f65 7272 6f72 5f68  encoding_error_h
+00005e90: 616e 646c 6572 948c 1062 6163 6b73 6c61  andler...backsla
+00005ea0: 7368 7265 706c 6163 6594 8c0d 6c61 6e67  shreplace...lang
+00005eb0: 7561 6765 5f63 6f64 6594 8c02 656e 948c  uage_code...en..
+00005ec0: 1372 6563 6f72 645f 6465 7065 6e64 656e  .record_dependen
+00005ed0: 6369 6573 944e 8c06 636f 6e66 6967 944e  cies.N..config.N
+00005ee0: 8c09 6964 5f70 7265 6669 7894 6806 8c0e  ..id_prefix.h...
+00005ef0: 6175 746f 5f69 645f 7072 6566 6978 948c  auto_id_prefix..
+00005f00: 0269 6494 8c0d 6475 6d70 5f73 6574 7469  .id...dump_setti
+00005f10: 6e67 7394 4e8c 0e64 756d 705f 696e 7465  ngs.N..dump_inte
+00005f20: 726e 616c 7394 4e8c 0f64 756d 705f 7472  rnals.N..dump_tr
+00005f30: 616e 7366 6f72 6d73 944e 8c0f 6475 6d70  ansforms.N..dump
+00005f40: 5f70 7365 7564 6f5f 786d 6c94 4e8c 1065  _pseudo_xml.N..e
+00005f50: 7870 6f73 655f 696e 7465 726e 616c 7394  xpose_internals.
+00005f60: 4e8c 0e73 7472 6963 745f 7669 7369 746f  N..strict_visito
+00005f70: 7294 4e8c 0f5f 6469 7361 626c 655f 636f  r.N.._disable_co
+00005f80: 6e66 6967 944e 8c07 5f73 6f75 7263 6594  nfig.N.._source.
+00005f90: 682c 8c0c 5f64 6573 7469 6e61 7469 6f6e  h,.._destination
+00005fa0: 944e 8c0d 5f63 6f6e 6669 675f 6669 6c65  .N.._config_file
+00005fb0: 7394 5d94 8c16 6669 6c65 5f69 6e73 6572  s.]...file_inser
+00005fc0: 7469 6f6e 5f65 6e61 626c 6564 9488 8c0b  tion_enabled....
+00005fd0: 7261 775f 656e 6162 6c65 6494 4b01 8c11  raw_enabled.K...
+00005fe0: 6c69 6e65 5f6c 656e 6774 685f 6c69 6d69  line_length_limi
+00005ff0: 7494 4d10 278c 0e70 6570 5f72 6566 6572  t.M.'..pep_refer
+00006000: 656e 6365 7394 4e8c 0c70 6570 5f62 6173  ences.N..pep_bas
+00006010: 655f 7572 6c94 8c18 6874 7470 733a 2f2f  e_url...https://
+00006020: 7065 7073 2e70 7974 686f 6e2e 6f72 672f  peps.python.org/
+00006030: 948c 1570 6570 5f66 696c 655f 7572 6c5f  ...pep_file_url_
+00006040: 7465 6d70 6c61 7465 948c 0870 6570 2d25  template...pep-%
+00006050: 3034 6494 8c0e 7266 635f 7265 6665 7265  04d...rfc_refere
+00006060: 6e63 6573 944e 8c0c 7266 635f 6261 7365  nces.N..rfc_base
+00006070: 5f75 726c 948c 2668 7474 7073 3a2f 2f64  _url..&https://d
+00006080: 6174 6174 7261 636b 6572 2e69 6574 662e  atatracker.ietf.
+00006090: 6f72 672f 646f 632f 6874 6d6c 2f94 8c09  org/doc/html/...
+000060a0: 7461 625f 7769 6474 6894 4b08 8c1d 7472  tab_width.K...tr
+000060b0: 696d 5f66 6f6f 746e 6f74 655f 7265 6665  im_footnote_refe
+000060c0: 7265 6e63 655f 7370 6163 6594 898c 1073  rence_space....s
+000060d0: 796e 7461 785f 6869 6768 6c69 6768 7494  yntax_highlight.
+000060e0: 8c04 6c6f 6e67 948c 0c73 6d61 7274 5f71  ..long...smart_q
+000060f0: 756f 7465 7394 888c 1373 6d61 7274 7175  uotes....smartqu
+00006100: 6f74 6573 5f6c 6f63 616c 6573 945d 948c  otes_locales.]..
+00006110: 1d63 6861 7261 6374 6572 5f6c 6576 656c  .character_level
+00006120: 5f69 6e6c 696e 655f 6d61 726b 7570 9489  _inline_markup..
+00006130: 8c0e 646f 6374 6974 6c65 5f78 666f 726d  ..doctitle_xform
+00006140: 9489 8c0d 646f 6369 6e66 6f5f 7866 6f72  ....docinfo_xfor
+00006150: 6d94 4b01 8c12 7365 6374 7375 6274 6974  m.K...sectsubtit
+00006160: 6c65 5f78 666f 726d 9489 8c0d 696d 6167  le_xform....imag
+00006170: 655f 6c6f 6164 696e 6794 8c04 6c69 6e6b  e_loading...link
+00006180: 948c 1065 6d62 6564 5f73 7479 6c65 7368  ...embed_stylesh
+00006190: 6565 7494 898c 1563 6c6f 616b 5f65 6d61  eet....cloak_ema
+000061a0: 696c 5f61 6464 7265 7373 6573 9488 8c11  il_addresses....
+000061b0: 7365 6374 696f 6e5f 7365 6c66 5f6c 696e  section_self_lin
+000061c0: 6b94 898c 0365 6e76 944e 7562 8c08 7265  k....env.Nub..re
+000061d0: 706f 7274 6572 944e 8c10 696e 6469 7265  porter.N..indire
+000061e0: 6374 5f74 6172 6765 7473 945d 948c 1173  ct_targets.]...s
+000061f0: 7562 7374 6974 7574 696f 6e5f 6465 6673  ubstitution_defs
+00006200: 947d 948c 1273 7562 7374 6974 7574 696f  .}...substitutio
+00006210: 6e5f 6e61 6d65 7394 7d94 8c08 7265 666e  n_names.}...refn
+00006220: 616d 6573 947d 948c 0672 6566 6964 7394  ames.}...refids.
+00006230: 7d94 8c07 6e61 6d65 6964 7394 7d94 286a  }...nameids.}.(j
+00006240: 9108 0000 6a8e 0800 006a 4006 0000 6a3d  ....j....j@...j=
+00006250: 0600 006a 3806 0000 6a35 0600 006a 8908  ...j8...j5...j..
+00006260: 0000 6a86 0800 006a 8108 0000 6a7e 0800  ..j....j....j~..
+00006270: 0075 8c09 6e61 6d65 7479 7065 7394 7d94  .u..nametypes.}.
+00006280: 286a 9108 0000 896a 4006 0000 896a 3806  (j.....j@....j8.
+00006290: 0000 896a 8908 0000 896a 8108 0000 8975  ...j.....j.....u
+000062a0: 6821 7d94 286a 8e08 0000 680c 6a3d 0600  h!}.(j....h.j=..
+000062b0: 0068 2d6a 3506 0000 683e 685e 6867 6a86  .h-j5...h>h^hgj.
+000062c0: 0800 006a 4306 0000 6a7e 0800 006a 5406  ...jC...j~...jT.
+000062d0: 0000 6a71 0600 006a 7606 0000 6ade 0600  ..jq...jv...j...
+000062e0: 006a e306 0000 6ad9 0700 006a df07 0000  .j....j....j....
+000062f0: 758c 0d66 6f6f 746e 6f74 655f 7265 6673  u..footnote_refs
+00006300: 947d 948c 0d63 6974 6174 696f 6e5f 7265  .}...citation_re
+00006310: 6673 947d 948c 0d61 7574 6f66 6f6f 746e  fs.}...autofootn
+00006320: 6f74 6573 945d 948c 1161 7574 6f66 6f6f  otes.]...autofoo
+00006330: 746e 6f74 655f 7265 6673 945d 948c 1073  tnote_refs.]...s
+00006340: 796d 626f 6c5f 666f 6f74 6e6f 7465 7394  ymbol_footnotes.
+00006350: 5d94 8c14 7379 6d62 6f6c 5f66 6f6f 746e  ]...symbol_footn
+00006360: 6f74 655f 7265 6673 945d 948c 0966 6f6f  ote_refs.]...foo
+00006370: 746e 6f74 6573 945d 948c 0963 6974 6174  tnotes.]...citat
+00006380: 696f 6e73 945d 948c 1261 7574 6f66 6f6f  ions.]...autofoo
+00006390: 746e 6f74 655f 7374 6172 7494 4b01 8c15  tnote_start.K...
+000063a0: 7379 6d62 6f6c 5f66 6f6f 746e 6f74 655f  symbol_footnote_
+000063b0: 7374 6172 7494 4b00 8c0a 6964 5f63 6f75  start.K...id_cou
+000063c0: 6e74 6572 948c 0b63 6f6c 6c65 6374 696f  nter...collectio
+000063d0: 6e73 948c 0743 6f75 6e74 6572 9493 947d  ns...Counter...}
+000063e0: 9485 9452 948c 0e70 6172 7365 5f6d 6573  ...R...parse_mes
+000063f0: 7361 6765 7394 5d94 8c12 7472 616e 7366  sages.]...transf
+00006400: 6f72 6d5f 6d65 7373 6167 6573 945d 948c  orm_messages.]..
+00006410: 0b74 7261 6e73 666f 726d 6572 944e 8c0b  .transformer.N..
+00006420: 696e 636c 7564 655f 6c6f 6794 5d94 8c0a  include_log.]...
+00006430: 6465 636f 7261 7469 6f6e 944e 681c 6803  decoration.Nh.h.
+00006440: 7562 2e                                  ub.
```

### Comparing `cookies_utilities-0.0.1/docs/build/doctrees/environment.pickle` & `cookies_utilities-0.0.2/docs/build/doctrees/environment.pickle`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8005 9507 d200 0000 0000 008c 1273 7068  .............sph
+00000000: 8005 95f2 e700 0000 0000 008c 1273 7068  .............sph
 00000010: 696e 782e 656e 7669 726f 6e6d 656e 7494  inx.environment.
 00000020: 8c10 4275 696c 6445 6e76 6972 6f6e 6d65  ..BuildEnvironme
 00000030: 6e74 9493 9429 8194 7d94 288c 0361 7070  nt...)..}.(..app
 00000040: 944e 8c0a 646f 6374 7265 6564 6972 948c  .N..doctreedir..
 00000050: 3a43 3a5c 5573 6572 735c 632d 6d69 685c  :C:\Users\c-mih\
 00000060: 7370 6163 655c 636f 6f6b 6965 735f 7574  space\cookies_ut
 00000070: 696c 6974 6965 735c 646f 6373 5c62 7569  ilities\docs\bui
@@ -19,15 +19,15 @@
 00000120: 6e78 2e65 7874 2e61 7574 6f64 6f63 9461  nx.ext.autodoc.a
 00000130: 8c07 7072 6f6a 6563 7494 8c11 636f 6f6b  ..project...cook
 00000140: 6965 735f 7574 696c 6974 6965 7394 8c09  ies_utilities...
 00000150: 636f 7079 7269 6768 7494 8c11 3230 3233  copyright...2023
 00000160: 2c20 436f 6f6b 6965 426f 7832 3694 8c06  , CookieBox26...
 00000170: 6175 7468 6f72 948c 0b43 6f6f 6b69 6542  author...CookieB
 00000180: 6f78 3236 948c 0772 656c 6561 7365 948c  ox26...release..
-00000190: 0530 2e30 2e34 948c 0e74 656d 706c 6174  .0.0.4...templat
+00000190: 0530 2e30 2e31 948c 0e74 656d 706c 6174  .0.0.1...templat
 000001a0: 6573 5f70 6174 6894 5d94 8c0a 5f74 656d  es_path.]..._tem
 000001b0: 706c 6174 6573 9461 8c10 6578 636c 7564  plates.a..exclud
 000001c0: 655f 7061 7474 6572 6e73 945d 948c 0a68  e_patterns.]...h
 000001d0: 746d 6c5f 7468 656d 6594 8c10 7370 6869  tml_theme...sphi
 000001e0: 6e78 5f72 7464 5f74 6865 6d65 948c 1068  nx_rtd_theme...h
 000001f0: 746d 6c5f 7374 6174 6963 5f70 6174 6894  tml_static_path.
 00000200: 5d94 8c07 5f73 7461 7469 6394 618c 0e65  ]..._static.a..e
@@ -178,19 +178,19 @@
 00000b10: 686f 7269 7a6f 6e74 616c 9468 c94e 8794  horizontal.h.N..
 00000b20: 6823 6824 6841 4e87 948c 0f68 746d 6c5f  h#h$hAN....html_
 00000b30: 7468 656d 655f 7061 7468 945d 9468 414e  theme_path.].hAN
 00000b40: 8794 8c12 6874 6d6c 5f74 6865 6d65 5f6f  ....html_theme_o
 00000b50: 7074 696f 6e73 947d 9468 414e 8794 8c0a  ptions.}.hAN....
 00000b60: 6874 6d6c 5f74 6974 6c65 948c 2563 6f6f  html_title..%coo
 00000b70: 6b69 6573 5f75 7469 6c69 7469 6573 2030  kies_utilities 0
-00000b80: 2e30 2e34 2064 6f63 756d 656e 7461 7469  .0.4 documentati
+00000b80: 2e30 2e31 2064 6f63 756d 656e 7461 7469  .0.1 documentati
 00000b90: 6f6e 9468 414e 8794 8c10 6874 6d6c 5f73  on.hAN....html_s
 00000ba0: 686f 7274 5f74 6974 6c65 948c 2563 6f6f  hort_title..%coo
 00000bb0: 6b69 6573 5f75 7469 6c69 7469 6573 2030  kies_utilities 0
-00000bc0: 2e30 2e34 2064 6f63 756d 656e 7461 7469  .0.4 documentati
+00000bc0: 2e30 2e31 2064 6f63 756d 656e 7461 7469  .0.1 documentati
 00000bd0: 6f6e 9468 414e 8794 8c0a 6874 6d6c 5f73  on.hAN....html_s
 00000be0: 7479 6c65 944e 6841 4e87 948c 0968 746d  tyle.NhAN....htm
 00000bf0: 6c5f 6c6f 676f 944e 6841 4e87 948c 0c68  l_logo.NhAN....h
 00000c00: 746d 6c5f 6661 7669 636f 6e94 4e68 414e  tml_favicon.NhAN
 00000c10: 8794 682a 682b 6841 4e87 9468 2c68 2d68  ..h*h+hAN..h,h-h
 00000c20: 414e 8794 6825 6826 6841 4e87 948c 0f68  AN..h%h&hAN....h
 00000c30: 746d 6c5f 6578 7472 615f 7061 7468 945d  tml_extra_path.]
@@ -331,15 +331,15 @@
 000014a0: 6e6f 7265 945d 948c 025e 2194 6168 404e  nore.]...^!.ah@N
 000014b0: 8794 8c1c 6c69 6e6b 6368 6563 6b5f 7261  ....linkcheck_ra
 000014c0: 7465 5f6c 696d 6974 5f74 696d 656f 7574  te_limit_timeout
 000014d0: 9447 4072 c000 0000 0000 6840 4e87 948c  .G@r......h@N...
 000014e0: 096d 616e 5f70 6167 6573 945d 9428 6859  .man_pages.].(hY
 000014f0: 8c11 636f 6f6b 6965 735f 7574 696c 6974  ..cookies_utilit
 00001500: 6965 7394 8c17 636f 6f6b 6965 735f 7574  ies...cookies_ut
-00001510: 696c 6974 6965 7320 302e 302e 3494 5d94  ilities 0.0.4.].
+00001510: 696c 6974 6965 7320 302e 302e 3194 5d94  ilities 0.0.1.].
 00001520: 681b 614b 0174 9461 6840 4e87 948c 0d6d  h.aK.t.ah@N....m
 00001530: 616e 5f73 686f 775f 7572 6c73 9489 6840  an_show_urls..h@
 00001540: 4e87 948c 1a6d 616e 5f6d 616b 655f 7365  N....man_make_se
 00001550: 6374 696f 6e5f 6469 7265 6374 6f72 7994  ction_directory.
 00001560: 8968 404e 8794 8c13 7369 6e67 6c65 6874  .h@N....singleht
 00001570: 6d6c 5f73 6964 6562 6172 7394 6a21 0100  ml_sidebars.j!..
 00001580: 0068 414e 8794 8c11 7465 7869 6e66 6f5f  .hAN....texinfo_
@@ -406,15 +406,15 @@
 00001950: 0565 6e2d 7573 946a 2a02 0000 4e87 948c  .en-us.j*...N...
 00001960: 1861 7070 6c65 6865 6c70 5f62 756e 646c  .applehelp_bundl
 00001970: 655f 7665 7273 696f 6e94 8c01 3194 6a2a  e_version...1.j*
 00001980: 0200 004e 8794 8c0e 6170 706c 6568 656c  ...N....applehel
 00001990: 705f 6963 6f6e 944e 6a2a 0200 004e 8794  p_icon.Nj*...N..
 000019a0: 8c14 6170 706c 6568 656c 705f 6b62 5f70  ..applehelp_kb_p
 000019b0: 726f 6475 6374 948c 1763 6f6f 6b69 6573  roduct...cookies
-000019c0: 5f75 7469 6c69 7469 6573 2d30 2e30 2e34  _utilities-0.0.4
+000019c0: 5f75 7469 6c69 7469 6573 2d30 2e30 2e31  _utilities-0.0.1
 000019d0: 946a 2a02 0000 4e87 948c 1061 7070 6c65  .j*...N....apple
 000019e0: 6865 6c70 5f6b 625f 7572 6c94 4e6a 2a02  help_kb_url.Nj*.
 000019f0: 0000 4e87 948c 1461 7070 6c65 6865 6c70  ..N....applehelp
 00001a00: 5f72 656d 6f74 655f 7572 6c94 4e6a 2a02  _remote_url.Nj*.
 00001a10: 0000 4e87 948c 1761 7070 6c65 6865 6c70  ..N....applehelp
 00001a20: 5f69 6e64 6578 5f61 6e63 686f 7273 9489  _index_anchors..
 00001a30: 6a2a 0200 004e 8794 8c19 6170 706c 6568  j*...N....appleh
@@ -491,17 +491,17 @@
 00001ea0: 7374 6174 7573 944b 018c 1363 6f6e 6669  status.K...confi
 00001eb0: 675f 7374 6174 7573 5f65 7874 7261 9468  g_status_extra.h
 00001ec0: 408c 0665 7665 6e74 7394 4e8c 0770 726f  @..events.N..pro
 00001ed0: 6a65 6374 948c 0e73 7068 696e 782e 7072  ject...sphinx.pr
 00001ee0: 6f6a 6563 7494 8c07 5072 6f6a 6563 7494  oject...Project.
 00001ef0: 9394 2981 947d 9428 8c06 7372 6364 6972  ..)..}.(..srcdir
 00001f00: 9468 0968 5d68 5e8c 0864 6f63 6e61 6d65  .h.h]h^..docname
-00001f10: 7394 8f94 288c 1163 6f6f 6b69 6573 5f75  s...(..cookies_u
-00001f20: 7469 6c69 7469 6573 948c 0569 6e64 6578  tilities...index
-00001f30: 948c 076d 6f64 756c 6573 9490 7562 8c07  ...modules..ub..
+00001f10: 7394 8f94 288c 076d 6f64 756c 6573 948c  s...(..modules..
+00001f20: 1163 6f6f 6b69 6573 5f75 7469 6c69 7469  .cookies_utiliti
+00001f30: 6573 948c 0569 6e64 6578 9490 7562 8c07  es...index..ub..
 00001f40: 7665 7273 696f 6e94 7d94 288c 1073 7068  version.}.(..sph
 00001f50: 696e 782e 646f 6d61 696e 732e 6394 4b02  inx.domains.c.K.
 00001f60: 8c18 7370 6869 6e78 2e64 6f6d 6169 6e73  ..sphinx.domains
 00001f70: 2e63 6861 6e67 6573 6574 944b 018c 1773  .changeset.K...s
 00001f80: 7068 696e 782e 646f 6d61 696e 732e 6369  phinx.domains.ci
 00001f90: 7461 7469 6f6e 944b 018c 1273 7068 696e  tation.K...sphin
 00001fa0: 782e 646f 6d61 696e 732e 6370 7094 4b08  x.domains.cpp.K.
@@ -544,29 +544,29 @@
 000021f0: 6564 9488 8c13 736d 6172 7471 756f 7465  ed....smartquote
 00002200: 735f 6c6f 6361 6c65 7394 5d94 8c03 656e  s_locales.]...en
 00002210: 7694 6803 8c1d 7472 696d 5f66 6f6f 746e  v.h...trim_footn
 00002220: 6f74 655f 7265 6665 7265 6e63 655f 7370  ote_reference_sp
 00002230: 6163 6594 898c 0d6c 616e 6775 6167 655f  ace....language_
 00002240: 636f 6465 9468 4c8c 0c73 6d61 7274 5f71  code.hL..smart_q
 00002250: 756f 7465 7394 8875 8c08 616c 6c5f 646f  uotes..u..all_do
-00002260: 6373 947d 9428 8c07 6d6f 6475 6c65 7394  cs.}.(..modules.
-00002270: 4741 d930 e28f 21f8 958c 0569 6e64 6578  GA.0..!....index
-00002280: 9447 41d9 30e4 1215 0978 6a9a 0200 0047  .GA.0....xj....G
-00002290: 41d9 30e5 806a 1626 758c 0c64 6570 656e  A.0..j.&u..depen
+00002260: 6373 947d 9428 8c05 696e 6465 7894 4741  cs.}.(..index.GA
+00002270: d930 f58e 8566 f98c 076d 6f64 756c 6573  .0...f...modules
+00002280: 9447 41d9 30f5 8e85 98cc 6a9b 0200 0047  .GA.0.....j....G
+00002290: 41d9 30fc 2a6e 55fe 758c 0c64 6570 656e  A.0.*nU.u..depen
 000022a0: 6465 6e63 6965 7394 8c0b 636f 6c6c 6563  dencies...collec
 000022b0: 7469 6f6e 7394 8c0b 6465 6661 756c 7464  tions...defaultd
 000022c0: 6963 7494 9394 8c08 6275 696c 7469 6e73  ict.....builtins
-000022d0: 948c 0373 6574 9493 9485 9452 9428 8c07  ...set.....R.(..
-000022e0: 6d6f 6475 6c65 7394 8f94 8c05 696e 6465  modules.....inde
-000022f0: 7894 8f94 6a9a 0200 008f 9428 8c28 2e2e  x...j......(.(..
+000022d0: 948c 0373 6574 9493 9485 9452 9428 8c05  ...set.....R.(..
+000022e0: 696e 6465 7894 8f94 8c07 6d6f 6475 6c65  index.....module
+000022f0: 7394 8f94 6a9b 0200 008f 9428 8c27 2e2e  s...j......(.'..
 00002300: 2f2e 2e2f 7372 632f 636f 6f6b 6965 735f  /../src/cookies_
-00002310: 7574 696c 6974 6965 732f 7374 6f70 7761  utilities/stopwa
-00002320: 7463 682e 7079 948c 272e 2e2f 2e2e 2f73  tch.py..'../../s
-00002330: 7263 2f63 6f6f 6b69 6573 5f75 7469 6c69  rc/cookies_utili
-00002340: 7469 6573 2f5f 5f69 6e69 745f 5f2e 7079  ties/__init__.py
+00002310: 7574 696c 6974 6965 732f 5f5f 696e 6974  utilities/__init
+00002320: 5f5f 2e70 7994 8c28 2e2e 2f2e 2e2f 7372  __.py..(../../sr
+00002330: 632f 636f 6f6b 6965 735f 7574 696c 6974  c/cookies_utilit
+00002340: 6965 732f 7374 6f70 7761 7463 682e 7079  ies/stopwatch.py
 00002350: 9490 758c 0869 6e63 6c75 6465 6494 6acf  ..u..included.j.
 00002360: 0200 006a d202 0000 8594 5294 8c0d 7265  ...j......R...re
 00002370: 7265 6164 5f61 6c77 6179 7394 8f94 8c16  read_always.....
 00002380: 5f70 6963 6b6c 6564 5f64 6f63 7472 6565  _pickled_doctree
 00002390: 5f63 6163 6865 947d 948c 185f 7772 6974  _cache.}..._writ
 000023a0: 655f 646f 635f 646f 6374 7265 655f 6361  e_doc_doctree_ca
 000023b0: 6368 6594 7d94 288c 1163 6f6f 6b69 6573  che.}.(..cookies
@@ -641,2722 +641,3072 @@
 00002800: 756a 0f03 0000 6859 6aff 0200 006a 2203  uj....hYj....j".
 00002810: 0000 6a00 0300 006a e902 0000 6a01 0300  ..j....j....j...
 00002820: 004e 6a02 0300 004e 7562 6ae6 0200 008c  .Nj....Nubj.....
 00002830: 0464 6573 6394 9394 2981 947d 9428 6aeb  .desc...)..}.(j.
 00002840: 0200 0068 406a ec02 0000 5d94 286a e602  ...h@j....].(j..
 00002850: 0000 8c0e 6465 7363 5f73 6967 6e61 7475  ....desc_signatu
 00002860: 7265 9493 9429 8194 7d94 286a eb02 0000  re...)..}.(j....
-00002870: 8cb6 6765 745f 6461 7465 7328 7374 6172  ..get_dates(star
+00002870: 8cc5 6765 745f 6461 7465 7328 7374 6172  ..get_dates(star
 00002880: 743d 2732 3031 362d 3037 2d30 3120 3032  t='2016-07-01 02
 00002890: 3a30 303a 3030 272c 2065 6e64 3d27 3230  :00:00', end='20
 000028a0: 3136 2d30 372d 3032 2030 313a 3030 3a30  16-07-02 01:00:0
 000028b0: 3027 2c20 666f 726d 6174 3d27 2559 2d25  0', format='%Y-%
 000028c0: 6d2d 2564 2025 483a 254d 3a25 5327 2c20  m-%d %H:%M:%S', 
 000028d0: 6465 6c74 613d 7b27 6461 7973 273a 2030  delta={'days': 0
 000028e0: 2c20 2768 6f75 7273 273a 2031 2c20 276d  , 'hours': 1, 'm
 000028f0: 696e 7574 6573 273a 2030 2c20 2777 6565  inutes': 0, 'wee
-00002900: 6b73 273a 2030 7d2c 2063 6173 745f 7374  ks': 0}, cast_st
-00002910: 723d 5472 7565 2c20 666f 726d 6174 5f6f  r=True, format_o
-00002920: 7574 3d4e 6f6e 6529 946a ec02 0000 5d94  ut=None).j....].
-00002930: 286a e602 0000 8c0c 6465 7363 5f61 6464  (j......desc_add
-00002940: 6e61 6d65 9493 9429 8194 7d94 286a eb02  name...)..}.(j..
-00002950: 0000 8c12 636f 6f6b 6965 735f 7574 696c  ....cookies_util
-00002960: 6974 6965 732e 946a ec02 0000 5d94 6afa  ities..j....].j.
-00002970: 0200 008c 1263 6f6f 6b69 6573 5f75 7469  .....cookies_uti
-00002980: 6c69 7469 6573 2e94 8594 8194 7d94 286a  lities......}.(j
-00002990: ff02 0000 6a50 0300 006a 0003 0000 6ae9  ....jP...j....j.
-000029a0: 0200 006a 0103 0000 4e6a 0203 0000 4e75  ...j....Nj....Nu
-000029b0: 6261 6a03 0300 007d 9428 6a05 0300 005d  baj....}.(j....]
-000029c0: 946a 0703 0000 5d94 288c 0b73 6967 2d70  .j....].(..sig-p
-000029d0: 7265 6e61 6d65 948c 0d64 6573 6363 6c61  rename...desccla
-000029e0: 7373 6e61 6d65 9465 6a09 0300 005d 946a  ssname.ej....].j
-000029f0: 0b03 0000 5d94 6a0d 0300 005d 948c 0978  ....].j....]...x
-00002a00: 6d6c 3a73 7061 6365 948c 0870 7265 7365  ml:space...prese
-00002a10: 7276 6594 756a 0f03 0000 6a4e 0300 006a  rve.uj....jN...j
-00002a20: ff02 0000 6a4a 0300 006a 0003 0000 6ae9  ....jJ...j....j.
-00002a30: 0200 006a 0103 0000 8c71 433a 5c55 7365  ...j.....qC:\Use
-00002a40: 7273 5c63 2d6d 6968 5c73 7061 6365 5c63  rs\c-mih\space\c
-00002a50: 6f6f 6b69 6573 5f75 7469 6c69 7469 6573  ookies_utilities
-00002a60: 5c73 7263 5c63 6f6f 6b69 6573 5f75 7469  \src\cookies_uti
-00002a70: 6c69 7469 6573 5c5f 5f69 6e69 745f 5f2e  lities\__init__.
-00002a80: 7079 3a64 6f63 7374 7269 6e67 206f 6620  py:docstring of 
-00002a90: 636f 6f6b 6965 735f 7574 696c 6974 6965  cookies_utilitie
-00002aa0: 732e 6765 745f 6461 7465 7394 6a02 0300  s.get_dates.j...
-00002ab0: 004b 0175 626a e602 0000 8c09 6465 7363  .K.ubj......desc
-00002ac0: 5f6e 616d 6594 9394 2981 947d 9428 6aeb  _name...)..}.(j.
-00002ad0: 0200 008c 0967 6574 5f64 6174 6573 946a  .....get_dates.j
-00002ae0: ec02 0000 5d94 6afa 0200 008c 0967 6574  ....].j......get
-00002af0: 5f64 6174 6573 9485 9481 947d 9428 6aff  _dates.....}.(j.
-00002b00: 0200 006a 6503 0000 6a00 0300 006a e902  ...je...j....j..
-00002b10: 0000 6a01 0300 004e 6a02 0300 004e 7562  ..j....Nj....Nub
-00002b20: 616a 0303 0000 7d94 286a 0503 0000 5d94  aj....}.(j....].
-00002b30: 6a07 0300 005d 9428 8c08 7369 672d 6e61  j....].(..sig-na
-00002b40: 6d65 948c 0864 6573 636e 616d 6594 656a  me...descname.ej
-00002b50: 0903 0000 5d94 6a0b 0300 005d 946a 0d03  ....].j....].j..
-00002b60: 0000 5d94 6a60 0300 006a 6103 0000 756a  ..].j`...ja...uj
-00002b70: 0f03 0000 6a63 0300 006a ff02 0000 6a4a  ....jc...j....jJ
-00002b80: 0300 006a 0003 0000 6ae9 0200 006a 0103  ...j....j....j..
-00002b90: 0000 6a62 0300 006a 0203 0000 4b01 7562  ..jb...j....K.ub
-00002ba0: 6ae6 0200 008c 1264 6573 635f 7061 7261  j......desc_para
-00002bb0: 6d65 7465 726c 6973 7494 9394 2981 947d  meterlist...)..}
-00002bc0: 9428 6aeb 0200 008c ab73 7461 7274 3d27  .(j......start='
-00002bd0: 3230 3136 2d30 372d 3031 2030 323a 3030  2016-07-01 02:00
-00002be0: 3a30 3027 2c20 656e 643d 2732 3031 362d  :00', end='2016-
-00002bf0: 3037 2d30 3220 3031 3a30 303a 3030 272c  07-02 01:00:00',
-00002c00: 2066 6f72 6d61 743d 2725 592d 256d 2d25   format='%Y-%m-%
-00002c10: 6420 2548 3a25 4d3a 2553 272c 2064 656c  d %H:%M:%S', del
-00002c20: 7461 3d7b 2764 6179 7327 3a20 302c 2027  ta={'days': 0, '
-00002c30: 686f 7572 7327 3a20 312c 2027 6d69 6e75  hours': 1, 'minu
-00002c40: 7465 7327 3a20 302c 2027 7765 656b 7327  tes': 0, 'weeks'
-00002c50: 3a20 307d 2c20 6361 7374 5f73 7472 3d54  : 0}, cast_str=T
-00002c60: 7275 652c 2066 6f72 6d61 745f 6f75 743d  rue, format_out=
-00002c70: 4e6f 6e65 946a ec02 0000 5d94 286a e602  None.j....].(j..
-00002c80: 0000 8c0e 6465 7363 5f70 6172 616d 6574  ....desc_paramet
-00002c90: 6572 9493 9429 8194 7d94 286a eb02 0000  er...)..}.(j....
-00002ca0: 8c1b 7374 6172 743d 2732 3031 362d 3037  ..start='2016-07
-00002cb0: 2d30 3120 3032 3a30 303a 3030 2794 6aec  -01 02:00:00'.j.
-00002cc0: 0200 005d 9428 6ae6 0200 008c 0d64 6573  ...].(j......des
-00002cd0: 635f 7369 675f 6e61 6d65 9493 9429 8194  c_sig_name...)..
-00002ce0: 7d94 286a eb02 0000 8c05 7374 6172 7494  }.(j......start.
-00002cf0: 6aec 0200 005d 946a fa02 0000 8c05 7374  j....].j......st
-00002d00: 6172 7494 8594 8194 7d94 286a ff02 0000  art.....}.(j....
-00002d10: 6a83 0300 006a 0003 0000 6ae9 0200 006a  j....j....j....j
-00002d20: 0103 0000 4e6a 0203 0000 4e75 6261 6a03  ....Nj....Nubaj.
-00002d30: 0300 007d 9428 6a05 0300 005d 946a 0703  ...}.(j....].j..
-00002d40: 0000 5d94 8c01 6e94 616a 0903 0000 5d94  ..]...n.aj....].
-00002d50: 6a0b 0300 005d 946a 0d03 0000 5d94 756a  j....].j....].uj
-00002d60: 0f03 0000 6a81 0300 006a ff02 0000 6a7d  ....j....j....j}
-00002d70: 0300 0075 626a e602 0000 8c11 6465 7363  ...ubj......desc
-00002d80: 5f73 6967 5f6f 7065 7261 746f 7294 9394  _sig_operator...
-00002d90: 2981 947d 9428 6aeb 0200 008c 013d 946a  )..}.(j......=.j
-00002da0: ec02 0000 5d94 6afa 0200 008c 013d 9485  ....].j......=..
-00002db0: 9481 947d 9428 6aff 0200 006a 9403 0000  ...}.(j....j....
-00002dc0: 6a00 0300 006a e902 0000 6a01 0300 004e  j....j....j....N
-00002dd0: 6a02 0300 004e 7562 616a 0303 0000 7d94  j....Nubaj....}.
-00002de0: 286a 0503 0000 5d94 6a07 0300 005d 948c  (j....].j....]..
-00002df0: 016f 9461 6a09 0300 005d 946a 0b03 0000  .o.aj....].j....
-00002e00: 5d94 6a0d 0300 005d 9475 6a0f 0300 006a  ].j....].uj....j
-00002e10: 9203 0000 6aff 0200 006a 7d03 0000 7562  ....j....j}...ub
-00002e20: 6aee 0200 0068 fa93 9429 8194 7d94 286a  j....h...)..}.(j
-00002e30: eb02 0000 8c15 2732 3031 362d 3037 2d30  ......'2016-07-0
-00002e40: 3120 3032 3a30 303a 3030 2794 6aec 0200  1 02:00:00'.j...
-00002e50: 005d 946a fa02 0000 8c15 2732 3031 362d  .].j......'2016-
-00002e60: 3037 2d30 3120 3032 3a30 303a 3030 2794  07-01 02:00:00'.
-00002e70: 8594 8194 7d94 286a ff02 0000 6aa4 0300  ....}.(j....j...
-00002e80: 006a 0003 0000 6ae9 0200 006a 0103 0000  .j....j....j....
-00002e90: 4e6a 0203 0000 4e75 6261 6a03 0300 007d  Nj....Nubaj....}
-00002ea0: 9428 6a05 0300 005d 946a 0703 0000 5d94  .(j....].j....].
-00002eb0: 8c0d 6465 6661 756c 745f 7661 6c75 6594  ..default_value.
-00002ec0: 616a 0903 0000 5d94 6a0b 0300 005d 946a  aj....].j....].j
-00002ed0: 0d03 0000 5d94 8c13 7375 7070 6f72 745f  ....]...support_
-00002ee0: 736d 6172 7471 756f 7465 7394 8975 6a0f  smartquotes..uj.
-00002ef0: 0300 0068 fa6a ff02 0000 6a7d 0300 0075  ...h.j....j}...u
-00002f00: 6265 6a03 0300 007d 9428 6a05 0300 005d  bej....}.(j....]
-00002f10: 946a 0703 0000 5d94 6a09 0300 005d 946a  .j....].j....].j
-00002f20: 0b03 0000 5d94 6a0d 0300 005d 946a 6003  ....].j....].j`.
-00002f30: 0000 6a61 0300 0075 6a0f 0300 006a 7b03  ..ja...uj....j{.
-00002f40: 0000 6aff 0200 006a 7703 0000 7562 6a7c  ..j....jw...ubj|
-00002f50: 0300 0029 8194 7d94 286a eb02 0000 8c19  ...)..}.(j......
-00002f60: 656e 643d 2732 3031 362d 3037 2d30 3220  end='2016-07-02 
-00002f70: 3031 3a30 303a 3030 2794 6aec 0200 005d  01:00:00'.j....]
-00002f80: 9428 6a82 0300 0029 8194 7d94 286a eb02  .(j....)..}.(j..
-00002f90: 0000 8c03 656e 6494 6aec 0200 005d 946a  ....end.j....].j
-00002fa0: fa02 0000 8c03 656e 6494 8594 8194 7d94  ......end.....}.
-00002fb0: 286a ff02 0000 6abe 0300 006a 0003 0000  (j....j....j....
-00002fc0: 6ae9 0200 006a 0103 0000 4e6a 0203 0000  j....j....Nj....
-00002fd0: 4e75 6261 6a03 0300 007d 9428 6a05 0300  Nubaj....}.(j...
-00002fe0: 005d 946a 0703 0000 5d94 6a8e 0300 0061  .].j....].j....a
-00002ff0: 6a09 0300 005d 946a 0b03 0000 5d94 6a0d  j....].j....].j.
-00003000: 0300 005d 9475 6a0f 0300 006a 8103 0000  ...].uj....j....
-00003010: 6aff 0200 006a ba03 0000 7562 6a93 0300  j....j....ubj...
-00003020: 0029 8194 7d94 286a eb02 0000 8c01 3d94  .)..}.(j......=.
-00003030: 6aec 0200 005d 946a fa02 0000 8c01 3d94  j....].j......=.
-00003040: 8594 8194 7d94 286a ff02 0000 6acc 0300  ....}.(j....j...
-00003050: 006a 0003 0000 6ae9 0200 006a 0103 0000  .j....j....j....
-00003060: 4e6a 0203 0000 4e75 6261 6a03 0300 007d  Nj....Nubaj....}
-00003070: 9428 6a05 0300 005d 946a 0703 0000 5d94  .(j....].j....].
-00003080: 6a9f 0300 0061 6a09 0300 005d 946a 0b03  j....aj....].j..
-00003090: 0000 5d94 6a0d 0300 005d 9475 6a0f 0300  ..].j....].uj...
-000030a0: 006a 9203 0000 6aff 0200 006a ba03 0000  .j....j....j....
-000030b0: 7562 6aa3 0300 0029 8194 7d94 286a eb02  ubj....)..}.(j..
-000030c0: 0000 8c15 2732 3031 362d 3037 2d30 3220  ....'2016-07-02 
-000030d0: 3031 3a30 303a 3030 2794 6aec 0200 005d  01:00:00'.j....]
-000030e0: 946a fa02 0000 8c15 2732 3031 362d 3037  .j......'2016-07
-000030f0: 2d30 3220 3031 3a30 303a 3030 2794 8594  -02 01:00:00'...
-00003100: 8194 7d94 286a ff02 0000 6ada 0300 006a  ..}.(j....j....j
-00003110: 0003 0000 6ae9 0200 006a 0103 0000 4e6a  ....j....j....Nj
-00003120: 0203 0000 4e75 6261 6a03 0300 007d 9428  ....Nubaj....}.(
-00003130: 6a05 0300 005d 946a 0703 0000 5d94 6aaf  j....].j....].j.
-00003140: 0300 0061 6a09 0300 005d 946a 0b03 0000  ...aj....].j....
-00003150: 5d94 6a0d 0300 005d 948c 1373 7570 706f  ].j....]...suppo
-00003160: 7274 5f73 6d61 7274 7175 6f74 6573 9489  rt_smartquotes..
-00003170: 756a 0f03 0000 68fa 6aff 0200 006a ba03  uj....h.j....j..
-00003180: 0000 7562 656a 0303 0000 7d94 286a 0503  ..ubej....}.(j..
-00003190: 0000 5d94 6a07 0300 005d 946a 0903 0000  ..].j....].j....
-000031a0: 5d94 6a0b 0300 005d 946a 0d03 0000 5d94  ].j....].j....].
-000031b0: 6a60 0300 006a 6103 0000 756a 0f03 0000  j`...ja...uj....
-000031c0: 6a7b 0300 006a ff02 0000 6a77 0300 0075  j{...j....jw...u
-000031d0: 626a 7c03 0000 2981 947d 9428 6aeb 0200  bj|...)..}.(j...
-000031e0: 008c 1a66 6f72 6d61 743d 2725 592d 256d  ...format='%Y-%m
-000031f0: 2d25 6420 2548 3a25 4d3a 2553 2794 6aec  -%d %H:%M:%S'.j.
-00003200: 0200 005d 9428 6a82 0300 0029 8194 7d94  ...].(j....)..}.
-00003210: 286a eb02 0000 8c06 666f 726d 6174 946a  (j......format.j
-00003220: ec02 0000 5d94 6afa 0200 008c 0666 6f72  ....].j......for
-00003230: 6d61 7494 8594 8194 7d94 286a ff02 0000  mat.....}.(j....
-00003240: 6af3 0300 006a 0003 0000 6ae9 0200 006a  j....j....j....j
-00003250: 0103 0000 4e6a 0203 0000 4e75 6261 6a03  ....Nj....Nubaj.
-00003260: 0300 007d 9428 6a05 0300 005d 946a 0703  ...}.(j....].j..
-00003270: 0000 5d94 6a8e 0300 0061 6a09 0300 005d  ..].j....aj....]
-00003280: 946a 0b03 0000 5d94 6a0d 0300 005d 9475  .j....].j....].u
-00003290: 6a0f 0300 006a 8103 0000 6aff 0200 006a  j....j....j....j
-000032a0: ef03 0000 7562 6a93 0300 0029 8194 7d94  ....ubj....)..}.
-000032b0: 286a eb02 0000 8c01 3d94 6aec 0200 005d  (j......=.j....]
-000032c0: 946a fa02 0000 8c01 3d94 8594 8194 7d94  .j......=.....}.
-000032d0: 286a ff02 0000 6a01 0400 006a 0003 0000  (j....j....j....
-000032e0: 6ae9 0200 006a 0103 0000 4e6a 0203 0000  j....j....Nj....
-000032f0: 4e75 6261 6a03 0300 007d 9428 6a05 0300  Nubaj....}.(j...
-00003300: 005d 946a 0703 0000 5d94 6a9f 0300 0061  .].j....].j....a
-00003310: 6a09 0300 005d 946a 0b03 0000 5d94 6a0d  j....].j....].j.
-00003320: 0300 005d 9475 6a0f 0300 006a 9203 0000  ...].uj....j....
-00003330: 6aff 0200 006a ef03 0000 7562 6aa3 0300  j....j....ubj...
-00003340: 0029 8194 7d94 286a eb02 0000 8c13 2725  .)..}.(j......'%
-00003350: 592d 256d 2d25 6420 2548 3a25 4d3a 2553  Y-%m-%d %H:%M:%S
-00003360: 2794 6aec 0200 005d 946a fa02 0000 8c13  '.j....].j......
-00003370: 2725 592d 256d 2d25 6420 2548 3a25 4d3a  '%Y-%m-%d %H:%M:
-00003380: 2553 2794 8594 8194 7d94 286a ff02 0000  %S'.....}.(j....
-00003390: 6a0f 0400 006a 0003 0000 6ae9 0200 006a  j....j....j....j
-000033a0: 0103 0000 4e6a 0203 0000 4e75 6261 6a03  ....Nj....Nubaj.
-000033b0: 0300 007d 9428 6a05 0300 005d 946a 0703  ...}.(j....].j..
-000033c0: 0000 5d94 6aaf 0300 0061 6a09 0300 005d  ..].j....aj....]
-000033d0: 946a 0b03 0000 5d94 6a0d 0300 005d 948c  .j....].j....]..
-000033e0: 1373 7570 706f 7274 5f73 6d61 7274 7175  .support_smartqu
-000033f0: 6f74 6573 9489 756a 0f03 0000 68fa 6aff  otes..uj....h.j.
-00003400: 0200 006a ef03 0000 7562 656a 0303 0000  ...j....ubej....
-00003410: 7d94 286a 0503 0000 5d94 6a07 0300 005d  }.(j....].j....]
-00003420: 946a 0903 0000 5d94 6a0b 0300 005d 946a  .j....].j....].j
-00003430: 0d03 0000 5d94 6a60 0300 006a 6103 0000  ....].j`...ja...
-00003440: 756a 0f03 0000 6a7b 0300 006a ff02 0000  uj....j{...j....
-00003450: 6a77 0300 0075 626a 7c03 0000 2981 947d  jw...ubj|...)..}
-00003460: 9428 6aeb 0200 008c 3764 656c 7461 3d7b  .(j.....7delta={
-00003470: 2764 6179 7327 3a20 302c 2027 686f 7572  'days': 0, 'hour
-00003480: 7327 3a20 312c 2027 6d69 6e75 7465 7327  s': 1, 'minutes'
-00003490: 3a20 302c 2027 7765 656b 7327 3a20 307d  : 0, 'weeks': 0}
-000034a0: 946a ec02 0000 5d94 286a 8203 0000 2981  .j....].(j....).
-000034b0: 947d 9428 6aeb 0200 008c 0564 656c 7461  .}.(j......delta
-000034c0: 946a ec02 0000 5d94 6afa 0200 008c 0564  .j....].j......d
-000034d0: 656c 7461 9485 9481 947d 9428 6aff 0200  elta.....}.(j...
-000034e0: 006a 2804 0000 6a00 0300 006a e902 0000  .j(...j....j....
-000034f0: 6a01 0300 004e 6a02 0300 004e 7562 616a  j....Nj....Nubaj
-00003500: 0303 0000 7d94 286a 0503 0000 5d94 6a07  ....}.(j....].j.
-00003510: 0300 005d 946a 8e03 0000 616a 0903 0000  ...].j....aj....
-00003520: 5d94 6a0b 0300 005d 946a 0d03 0000 5d94  ].j....].j....].
-00003530: 756a 0f03 0000 6a81 0300 006a ff02 0000  uj....j....j....
-00003540: 6a24 0400 0075 626a 9303 0000 2981 947d  j$...ubj....)..}
-00003550: 9428 6aeb 0200 008c 013d 946a ec02 0000  .(j......=.j....
-00003560: 5d94 6afa 0200 008c 013d 9485 9481 947d  ].j......=.....}
-00003570: 9428 6aff 0200 006a 3604 0000 6a00 0300  .(j....j6...j...
-00003580: 006a e902 0000 6a01 0300 004e 6a02 0300  .j....j....Nj...
-00003590: 004e 7562 616a 0303 0000 7d94 286a 0503  .Nubaj....}.(j..
-000035a0: 0000 5d94 6a07 0300 005d 946a 9f03 0000  ..].j....].j....
-000035b0: 616a 0903 0000 5d94 6a0b 0300 005d 946a  aj....].j....].j
-000035c0: 0d03 0000 5d94 756a 0f03 0000 6a92 0300  ....].uj....j...
-000035d0: 006a ff02 0000 6a24 0400 0075 626a a303  .j....j$...ubj..
-000035e0: 0000 2981 947d 9428 6aeb 0200 008c 317b  ..)..}.(j.....1{
-000035f0: 2764 6179 7327 3a20 302c 2027 686f 7572  'days': 0, 'hour
-00003600: 7327 3a20 312c 2027 6d69 6e75 7465 7327  s': 1, 'minutes'
-00003610: 3a20 302c 2027 7765 656b 7327 3a20 307d  : 0, 'weeks': 0}
-00003620: 946a ec02 0000 5d94 6afa 0200 008c 317b  .j....].j.....1{
-00003630: 2764 6179 7327 3a20 302c 2027 686f 7572  'days': 0, 'hour
-00003640: 7327 3a20 312c 2027 6d69 6e75 7465 7327  s': 1, 'minutes'
-00003650: 3a20 302c 2027 7765 656b 7327 3a20 307d  : 0, 'weeks': 0}
-00003660: 9485 9481 947d 9428 6aff 0200 006a 4404  .....}.(j....jD.
-00003670: 0000 6a00 0300 006a e902 0000 6a01 0300  ..j....j....j...
-00003680: 004e 6a02 0300 004e 7562 616a 0303 0000  .Nj....Nubaj....
-00003690: 7d94 286a 0503 0000 5d94 6a07 0300 005d  }.(j....].j....]
-000036a0: 946a af03 0000 616a 0903 0000 5d94 6a0b  .j....aj....].j.
-000036b0: 0300 005d 946a 0d03 0000 5d94 8c13 7375  ...].j....]...su
-000036c0: 7070 6f72 745f 736d 6172 7471 756f 7465  pport_smartquote
-000036d0: 7394 8975 6a0f 0300 0068 fa6a ff02 0000  s..uj....h.j....
-000036e0: 6a24 0400 0075 6265 6a03 0300 007d 9428  j$...ubej....}.(
-000036f0: 6a05 0300 005d 946a 0703 0000 5d94 6a09  j....].j....].j.
-00003700: 0300 005d 946a 0b03 0000 5d94 6a0d 0300  ...].j....].j...
-00003710: 005d 946a 6003 0000 6a61 0300 0075 6a0f  .].j`...ja...uj.
-00003720: 0300 006a 7b03 0000 6aff 0200 006a 7703  ...j{...j....jw.
-00003730: 0000 7562 6a7c 0300 0029 8194 7d94 286a  ..ubj|...)..}.(j
-00003740: eb02 0000 8c0d 6361 7374 5f73 7472 3d54  ......cast_str=T
-00003750: 7275 6594 6aec 0200 005d 9428 6a82 0300  rue.j....].(j...
-00003760: 0029 8194 7d94 286a eb02 0000 8c08 6361  .)..}.(j......ca
-00003770: 7374 5f73 7472 946a ec02 0000 5d94 6afa  st_str.j....].j.
-00003780: 0200 008c 0863 6173 745f 7374 7294 8594  .....cast_str...
-00003790: 8194 7d94 286a ff02 0000 6a5d 0400 006a  ..}.(j....j]...j
-000037a0: 0003 0000 6ae9 0200 006a 0103 0000 4e6a  ....j....j....Nj
-000037b0: 0203 0000 4e75 6261 6a03 0300 007d 9428  ....Nubaj....}.(
-000037c0: 6a05 0300 005d 946a 0703 0000 5d94 6a8e  j....].j....].j.
-000037d0: 0300 0061 6a09 0300 005d 946a 0b03 0000  ...aj....].j....
-000037e0: 5d94 6a0d 0300 005d 9475 6a0f 0300 006a  ].j....].uj....j
-000037f0: 8103 0000 6aff 0200 006a 5904 0000 7562  ....j....jY...ub
-00003800: 6a93 0300 0029 8194 7d94 286a eb02 0000  j....)..}.(j....
-00003810: 8c01 3d94 6aec 0200 005d 946a fa02 0000  ..=.j....].j....
-00003820: 8c01 3d94 8594 8194 7d94 286a ff02 0000  ..=.....}.(j....
-00003830: 6a6b 0400 006a 0003 0000 6ae9 0200 006a  jk...j....j....j
-00003840: 0103 0000 4e6a 0203 0000 4e75 6261 6a03  ....Nj....Nubaj.
-00003850: 0300 007d 9428 6a05 0300 005d 946a 0703  ...}.(j....].j..
-00003860: 0000 5d94 6a9f 0300 0061 6a09 0300 005d  ..].j....aj....]
-00003870: 946a 0b03 0000 5d94 6a0d 0300 005d 9475  .j....].j....].u
-00003880: 6a0f 0300 006a 9203 0000 6aff 0200 006a  j....j....j....j
-00003890: 5904 0000 7562 6aa3 0300 0029 8194 7d94  Y...ubj....)..}.
-000038a0: 286a eb02 0000 8c04 5472 7565 946a ec02  (j......True.j..
-000038b0: 0000 5d94 6afa 0200 008c 0454 7275 6594  ..].j......True.
-000038c0: 8594 8194 7d94 286a ff02 0000 6a79 0400  ....}.(j....jy..
-000038d0: 006a 0003 0000 6ae9 0200 006a 0103 0000  .j....j....j....
-000038e0: 4e6a 0203 0000 4e75 6261 6a03 0300 007d  Nj....Nubaj....}
-000038f0: 9428 6a05 0300 005d 946a 0703 0000 5d94  .(j....].j....].
-00003900: 6aaf 0300 0061 6a09 0300 005d 946a 0b03  j....aj....].j..
-00003910: 0000 5d94 6a0d 0300 005d 948c 1373 7570  ..].j....]...sup
-00003920: 706f 7274 5f73 6d61 7274 7175 6f74 6573  port_smartquotes
-00003930: 9489 756a 0f03 0000 68fa 6aff 0200 006a  ..uj....h.j....j
-00003940: 5904 0000 7562 656a 0303 0000 7d94 286a  Y...ubej....}.(j
-00003950: 0503 0000 5d94 6a07 0300 005d 946a 0903  ....].j....].j..
-00003960: 0000 5d94 6a0b 0300 005d 946a 0d03 0000  ..].j....].j....
-00003970: 5d94 6a60 0300 006a 6103 0000 756a 0f03  ].j`...ja...uj..
-00003980: 0000 6a7b 0300 006a ff02 0000 6a77 0300  ..j{...j....jw..
-00003990: 0075 626a 7c03 0000 2981 947d 9428 6aeb  .ubj|...)..}.(j.
-000039a0: 0200 008c 0f66 6f72 6d61 745f 6f75 743d  .....format_out=
-000039b0: 4e6f 6e65 946a ec02 0000 5d94 286a 8203  None.j....].(j..
-000039c0: 0000 2981 947d 9428 6aeb 0200 008c 0a66  ..)..}.(j......f
-000039d0: 6f72 6d61 745f 6f75 7494 6aec 0200 005d  ormat_out.j....]
-000039e0: 946a fa02 0000 8c0a 666f 726d 6174 5f6f  .j......format_o
-000039f0: 7574 9485 9481 947d 9428 6aff 0200 006a  ut.....}.(j....j
-00003a00: 9204 0000 6a00 0300 006a e902 0000 6a01  ....j....j....j.
-00003a10: 0300 004e 6a02 0300 004e 7562 616a 0303  ...Nj....Nubaj..
-00003a20: 0000 7d94 286a 0503 0000 5d94 6a07 0300  ..}.(j....].j...
-00003a30: 005d 946a 8e03 0000 616a 0903 0000 5d94  .].j....aj....].
-00003a40: 6a0b 0300 005d 946a 0d03 0000 5d94 756a  j....].j....].uj
-00003a50: 0f03 0000 6a81 0300 006a ff02 0000 6a8e  ....j....j....j.
-00003a60: 0400 0075 626a 9303 0000 2981 947d 9428  ...ubj....)..}.(
-00003a70: 6aeb 0200 008c 013d 946a ec02 0000 5d94  j......=.j....].
-00003a80: 6afa 0200 008c 013d 9485 9481 947d 9428  j......=.....}.(
-00003a90: 6aff 0200 006a a004 0000 6a00 0300 006a  j....j....j....j
-00003aa0: e902 0000 6a01 0300 004e 6a02 0300 004e  ....j....Nj....N
-00003ab0: 7562 616a 0303 0000 7d94 286a 0503 0000  ubaj....}.(j....
-00003ac0: 5d94 6a07 0300 005d 946a 9f03 0000 616a  ].j....].j....aj
-00003ad0: 0903 0000 5d94 6a0b 0300 005d 946a 0d03  ....].j....].j..
-00003ae0: 0000 5d94 756a 0f03 0000 6a92 0300 006a  ..].uj....j....j
-00003af0: ff02 0000 6a8e 0400 0075 626a a303 0000  ....j....ubj....
-00003b00: 2981 947d 9428 6aeb 0200 008c 044e 6f6e  )..}.(j......Non
-00003b10: 6594 6aec 0200 005d 946a fa02 0000 8c04  e.j....].j......
-00003b20: 4e6f 6e65 9485 9481 947d 9428 6aff 0200  None.....}.(j...
-00003b30: 006a ae04 0000 6a00 0300 006a e902 0000  .j....j....j....
-00003b40: 6a01 0300 004e 6a02 0300 004e 7562 616a  j....Nj....Nubaj
-00003b50: 0303 0000 7d94 286a 0503 0000 5d94 6a07  ....}.(j....].j.
-00003b60: 0300 005d 946a af03 0000 616a 0903 0000  ...].j....aj....
-00003b70: 5d94 6a0b 0300 005d 946a 0d03 0000 5d94  ].j....].j....].
-00003b80: 8c13 7375 7070 6f72 745f 736d 6172 7471  ..support_smartq
-00003b90: 756f 7465 7394 8975 6a0f 0300 0068 fa6a  uotes..uj....h.j
-00003ba0: ff02 0000 6a8e 0400 0075 6265 6a03 0300  ....j....ubej...
-00003bb0: 007d 9428 6a05 0300 005d 946a 0703 0000  .}.(j....].j....
-00003bc0: 5d94 6a09 0300 005d 946a 0b03 0000 5d94  ].j....].j....].
-00003bd0: 6a0d 0300 005d 946a 6003 0000 6a61 0300  j....].j`...ja..
-00003be0: 0075 6a0f 0300 006a 7b03 0000 6aff 0200  .uj....j{...j...
-00003bf0: 006a 7703 0000 7562 656a 0303 0000 7d94  .jw...ubej....}.
-00003c00: 286a 0503 0000 5d94 6a07 0300 005d 946a  (j....].j....].j
-00003c10: 0903 0000 5d94 6a0b 0300 005d 946a 0d03  ....].j....].j..
-00003c20: 0000 5d94 6a60 0300 006a 6103 0000 756a  ..].j`...ja...uj
-00003c30: 0f03 0000 6a75 0300 006a ff02 0000 6a4a  ....ju...j....jJ
-00003c40: 0300 006a 0003 0000 6ae9 0200 006a 0103  ...j....j....j..
-00003c50: 0000 6a62 0300 006a 0203 0000 4b01 7562  ..jb...j....K.ub
-00003c60: 656a 0303 0000 7d94 286a 0503 0000 5d94  ej....}.(j....].
-00003c70: 6a41 0300 0061 6a07 0300 005d 9428 8c03  jA...aj....].(..
-00003c80: 7369 6794 8c0a 7369 672d 6f62 6a65 6374  sig...sig-object
-00003c90: 9465 6a09 0300 005d 946a 0b03 0000 5d94  .ej....].j....].
-00003ca0: 6a0d 0300 005d 948c 066d 6f64 756c 6594  j....]...module.
-00003cb0: 8c11 636f 6f6b 6965 735f 7574 696c 6974  ..cookies_utilit
-00003cc0: 6965 7394 6a6a 0200 0068 408c 0866 756c  ies.jj...h@..ful
-00003cd0: 6c6e 616d 6594 6a67 0300 008c 0a5f 746f  lname.jg....._to
-00003ce0: 635f 7061 7274 7394 6ad2 0400 006a 6703  c_parts.j....jg.
-00003cf0: 0000 8694 8c09 5f74 6f63 5f6e 616d 6594  ......_toc_name.
-00003d00: 8c0b 6765 745f 6461 7465 7328 2994 756a  ..get_dates().uj
-00003d10: 0f03 0000 6a48 0300 006a 0103 0000 6a62  ....jH...j....jb
-00003d20: 0300 006a 0203 0000 4b01 6aff 0200 006a  ...j....K.j....j
-00003d30: 4503 0000 6a00 0300 006a e902 0000 7562  E...j....j....ub
-00003d40: 6ae6 0200 008c 0c64 6573 635f 636f 6e74  j......desc_cont
-00003d50: 656e 7494 9394 2981 947d 9428 6aeb 0200  ent...)..}.(j...
-00003d60: 0068 406a ec02 0000 5d94 286a ee02 0000  .h@j....].(j....
-00003d70: 8c09 7061 7261 6772 6170 6894 9394 2981  ..paragraph...).
-00003d80: 947d 9428 6aeb 0200 008c 5852 6574 7572  .}.(j.....XRetur
-00003d90: 6e73 2061 206c 6973 7420 6f66 2074 696d  ns a list of tim
-00003da0: 6573 2066 726f 6d20 7468 6520 2773 7461  es from the 'sta
-00003db0: 7274 2720 7469 6d65 2074 6f20 7468 6520  rt' time to the 
-00003dc0: 2765 6e64 2720 7469 6d65 2c0a 696e 6372  'end' time,.incr
-00003dd0: 656d 656e 7465 6420 6279 2027 6465 6c74  emented by 'delt
-00003de0: 6127 2e94 6aec 0200 005d 946a fa02 0000  a'..j....].j....
-00003df0: 8c64 5265 7475 726e 7320 6120 6c69 7374  .dReturns a list
-00003e00: 206f 6620 7469 6d65 7320 6672 6f6d 2074   of times from t
-00003e10: 6865 20e2 8098 7374 6172 74e2 8099 2074  he ...start... t
-00003e20: 696d 6520 746f 2074 6865 20e2 8098 656e  ime to the ...en
-00003e30: 64e2 8099 2074 696d 652c 0a69 6e63 7265  d... time,.incre
-00003e40: 6d65 6e74 6564 2062 7920 e280 9864 656c  mented by ...del
-00003e50: 7461 e280 992e 9485 9481 947d 9428 6aff  ta.........}.(j.
-00003e60: 0200 006a df04 0000 6a00 0300 006a e902  ...j....j....j..
-00003e70: 0000 6a01 0300 004e 6a02 0300 004e 7562  ..j....Nj....Nub
-00003e80: 616a 0303 0000 7d94 286a 0503 0000 5d94  aj....}.(j....].
-00003e90: 6a07 0300 005d 946a 0903 0000 5d94 6a0b  j....].j....].j.
-00003ea0: 0300 005d 946a 0d03 0000 5d94 756a 0f03  ...].j....].uj..
-00003eb0: 0000 6add 0400 006a 0103 0000 8c71 433a  ..j....j.....qC:
-00003ec0: 5c55 7365 7273 5c63 2d6d 6968 5c73 7061  \Users\c-mih\spa
-00003ed0: 6365 5c63 6f6f 6b69 6573 5f75 7469 6c69  ce\cookies_utili
-00003ee0: 7469 6573 5c73 7263 5c63 6f6f 6b69 6573  ties\src\cookies
-00003ef0: 5f75 7469 6c69 7469 6573 5c5f 5f69 6e69  _utilities\__ini
-00003f00: 745f 5f2e 7079 3a64 6f63 7374 7269 6e67  t__.py:docstring
-00003f10: 206f 6620 636f 6f6b 6965 735f 7574 696c   of cookies_util
-00003f20: 6974 6965 732e 6765 745f 6461 7465 7394  ities.get_dates.
-00003f30: 6a02 0300 004b 016a ff02 0000 6ada 0400  j....K.j....j...
-00003f40: 006a 0003 0000 6ae9 0200 0075 626a ee02  .j....j....ubj..
-00003f50: 0000 8c0a 6669 656c 645f 6c69 7374 9493  ....field_list..
-00003f60: 9429 8194 7d94 286a eb02 0000 6840 6aec  .)..}.(j....h@j.
-00003f70: 0200 005d 9428 6aee 0200 008c 0566 6965  ...].(j......fie
-00003f80: 6c64 9493 9429 8194 7d94 286a eb02 0000  ld...)..}.(j....
-00003f90: 6840 6aec 0200 005d 9428 6aee 0200 008c  h@j....].(j.....
-00003fa0: 0a66 6965 6c64 5f6e 616d 6594 9394 2981  .field_name...).
-00003fb0: 947d 9428 6aeb 0200 008c 0a50 6172 616d  .}.(j......Param
-00003fc0: 6574 6572 7394 6aec 0200 005d 946a fa02  eters.j....].j..
-00003fd0: 0000 8c0a 5061 7261 6d65 7465 7273 9485  ....Parameters..
-00003fe0: 9481 947d 9428 6aff 0200 006a fa04 0000  ...}.(j....j....
-00003ff0: 6a00 0300 006a e902 0000 6a01 0300 004e  j....j....j....N
-00004000: 6a02 0300 004e 7562 616a 0303 0000 7d94  j....Nubaj....}.
-00004010: 286a 0503 0000 5d94 6a07 0300 005d 946a  (j....].j....].j
-00004020: 0903 0000 5d94 6a0b 0300 005d 946a 0d03  ....].j....].j..
-00004030: 0000 5d94 756a 0f03 0000 6af8 0400 006a  ..].uj....j....j
-00004040: ff02 0000 6af5 0400 006a 0103 0000 6a62  ....j....j....jb
-00004050: 0300 006a 0203 0000 4b00 7562 6aee 0200  ...j....K.ubj...
-00004060: 008c 0a66 6965 6c64 5f62 6f64 7994 9394  ...field_body...
-00004070: 2981 947d 9428 6aeb 0200 0068 406a ec02  )..}.(j....h@j..
-00004080: 0000 5d94 6aee 0200 008c 0b62 756c 6c65  ..].j......bulle
-00004090: 745f 6c69 7374 9493 9429 8194 7d94 286a  t_list...)..}.(j
-000040a0: eb02 0000 6840 6aec 0200 005d 9428 6aee  ....h@j....].(j.
-000040b0: 0200 008c 096c 6973 745f 6974 656d 9493  .....list_item..
-000040c0: 9429 8194 7d94 286a eb02 0000 6840 6aec  .)..}.(j....h@j.
-000040d0: 0200 005d 946a de04 0000 2981 947d 9428  ...].j....)..}.(
-000040e0: 6aeb 0200 008c 2473 7461 7274 2028 7374  j.....$start (st
-000040f0: 7269 6e67 2920 2d2d 2053 7461 7274 2074  ring) -- Start t
-00004100: 696d 6520 7374 7269 6e67 2e94 6aec 0200  ime string..j...
-00004110: 005d 9428 6ae6 0200 008c 0e6c 6974 6572  .].(j......liter
-00004120: 616c 5f73 7472 6f6e 6794 9394 2981 947d  al_strong...)..}
-00004130: 9428 6aeb 0200 008c 0573 7461 7274 946a  .(j......start.j
-00004140: ec02 0000 5d94 6afa 0200 008c 0573 7461  ....].j......sta
-00004150: 7274 9485 9481 947d 9428 6aff 0200 006a  rt.....}.(j....j
-00004160: 1d05 0000 6a00 0300 006a e902 0000 6a01  ....j....j....j.
-00004170: 0300 004e 6a02 0300 004e 7562 616a 0303  ...Nj....Nubaj..
-00004180: 0000 7d94 286a 0503 0000 5d94 6a07 0300  ..}.(j....].j...
-00004190: 005d 946a 0903 0000 5d94 6a0b 0300 005d  .].j....].j....]
-000041a0: 946a 0d03 0000 5d94 756a 0f03 0000 6a1b  .j....].uj....j.
-000041b0: 0500 006a ff02 0000 6a17 0500 0075 626a  ...j....j....ubj
-000041c0: fa02 0000 8c02 2028 9485 9481 947d 9428  ...... (.....}.(
-000041d0: 6aff 0200 006a 1705 0000 6a00 0300 006a  j....j....j....j
-000041e0: e902 0000 6a01 0300 004e 6a02 0300 004e  ....j....Nj....N
-000041f0: 7562 6ae6 0200 008c 0c70 656e 6469 6e67  ubj......pending
-00004200: 5f78 7265 6694 9394 2981 947d 9428 6aeb  _xref...)..}.(j.
-00004210: 0200 0068 406a ec02 0000 5d94 6ae6 0200  ...h@j....].j...
-00004220: 008c 106c 6974 6572 616c 5f65 6d70 6861  ...literal_empha
-00004230: 7369 7394 9394 2981 947d 9428 6aeb 0200  sis...)..}.(j...
-00004240: 008c 0673 7472 696e 6794 6aec 0200 005d  ...string.j....]
-00004250: 946a fa02 0000 8c06 7374 7269 6e67 9485  .j......string..
-00004260: 9481 947d 9428 6aff 0200 006a 3605 0000  ...}.(j....j6...
-00004270: 6a00 0300 006a e902 0000 6a01 0300 004e  j....j....j....N
-00004280: 6a02 0300 004e 7562 616a 0303 0000 7d94  j....Nubaj....}.
-00004290: 286a 0503 0000 5d94 6a07 0300 005d 946a  (j....].j....].j
-000042a0: 0903 0000 5d94 6a0b 0300 005d 946a 0d03  ....].j....].j..
-000042b0: 0000 5d94 756a 0f03 0000 6a34 0500 006a  ..].uj....j4...j
-000042c0: ff02 0000 6a31 0500 0075 6261 6a03 0300  ....j1...ubaj...
-000042d0: 007d 9428 6a05 0300 005d 946a 0703 0000  .}.(j....].j....
-000042e0: 5d94 6a09 0300 005d 946a 0b03 0000 5d94  ].j....].j....].
-000042f0: 6a0d 0300 005d 948c 0972 6566 646f 6d61  j....]...refdoma
-00004300: 696e 948c 0270 7994 8c0b 7265 6665 7870  in...py...refexp
-00004310: 6c69 6369 7494 898c 0772 6566 7479 7065  licit....reftype
-00004320: 946a 6a02 0000 8c09 7265 6674 6172 6765  .jj.....reftarge
-00004330: 7494 6a38 0500 008c 0b72 6566 7370 6563  t.j8.....refspec
-00004340: 6966 6963 9488 8c09 7079 3a6d 6f64 756c  ific....py:modul
-00004350: 6594 6ad2 0400 008c 0870 793a 636c 6173  e.j......py:clas
-00004360: 7394 4e75 6a0f 0300 006a 2f05 0000 6aff  s.Nuj....j/...j.
-00004370: 0200 006a 1705 0000 7562 6afa 0200 008c  ...j....ubj.....
-00004380: 0129 9485 9481 947d 9428 6aff 0200 006a  .).....}.(j....j
-00004390: 1705 0000 6a00 0300 006a e902 0000 6a01  ....j....j....j.
-000043a0: 0300 004e 6a02 0300 004e 7562 6afa 0200  ...Nj....Nubj...
-000043b0: 008c 0520 e280 9320 9485 9481 947d 9428  ... ... .....}.(
-000043c0: 6aff 0200 006a 1705 0000 6a00 0300 006a  j....j....j....j
-000043d0: e902 0000 6a01 0300 004e 6a02 0300 004e  ....j....Nj....N
-000043e0: 7562 6afa 0200 008c 1253 7461 7274 2074  ubj......Start t
-000043f0: 696d 6520 7374 7269 6e67 2e94 8594 8194  ime string......
-00004400: 7d94 286a ff02 0000 6a17 0500 006a 0003  }.(j....j....j..
-00004410: 0000 6ae9 0200 006a 0103 0000 4e6a 0203  ..j....j....Nj..
-00004420: 0000 4e75 6265 6a03 0300 007d 9428 6a05  ..Nubej....}.(j.
-00004430: 0300 005d 946a 0703 0000 5d94 6a09 0300  ...].j....].j...
-00004440: 005d 946a 0b03 0000 5d94 6a0d 0300 005d  .].j....].j....]
-00004450: 9475 6a0f 0300 006a dd04 0000 6aff 0200  .uj....j....j...
-00004460: 006a 1405 0000 7562 616a 0303 0000 7d94  .j....ubaj....}.
-00004470: 286a 0503 0000 5d94 6a07 0300 005d 946a  (j....].j....].j
-00004480: 0903 0000 5d94 6a0b 0300 005d 946a 0d03  ....].j....].j..
-00004490: 0000 5d94 756a 0f03 0000 6a12 0500 006a  ..].uj....j....j
-000044a0: ff02 0000 6a0f 0500 0075 626a 1305 0000  ....j....ubj....
-000044b0: 2981 947d 9428 6aeb 0200 0068 406a ec02  )..}.(j....h@j..
-000044c0: 0000 5d94 6ade 0400 0029 8194 7d94 286a  ..].j....)..}.(j
-000044d0: eb02 0000 8c20 656e 6420 2873 7472 696e  ..... end (strin
-000044e0: 6729 202d 2d20 456e 6420 7469 6d65 2073  g) -- End time s
-000044f0: 7472 696e 672e 946a ec02 0000 5d94 286a  tring..j....].(j
-00004500: 1c05 0000 2981 947d 9428 6aeb 0200 008c  ....)..}.(j.....
-00004510: 0365 6e64 946a ec02 0000 5d94 6afa 0200  .end.j....].j...
-00004520: 008c 0365 6e64 9485 9481 947d 9428 6aff  ...end.....}.(j.
-00004530: 0200 006a 7105 0000 6a00 0300 006a e902  ...jq...j....j..
-00004540: 0000 6a01 0300 004e 6a02 0300 004e 7562  ..j....Nj....Nub
-00004550: 616a 0303 0000 7d94 286a 0503 0000 5d94  aj....}.(j....].
-00004560: 6a07 0300 005d 946a 0903 0000 5d94 6a0b  j....].j....].j.
-00004570: 0300 005d 946a 0d03 0000 5d94 756a 0f03  ...].j....].uj..
-00004580: 0000 6a1b 0500 006a ff02 0000 6a6d 0500  ..j....j....jm..
-00004590: 0075 626a fa02 0000 8c02 2028 9485 9481  .ubj...... (....
-000045a0: 947d 9428 6aff 0200 006a 6d05 0000 6a00  .}.(j....jm...j.
-000045b0: 0300 006a e902 0000 6a01 0300 004e 6a02  ...j....j....Nj.
-000045c0: 0300 004e 7562 6a30 0500 0029 8194 7d94  ...Nubj0...)..}.
-000045d0: 286a eb02 0000 6840 6aec 0200 005d 946a  (j....h@j....].j
-000045e0: 3505 0000 2981 947d 9428 6aeb 0200 008c  5...)..}.(j.....
-000045f0: 0673 7472 696e 6794 6aec 0200 005d 946a  .string.j....].j
-00004600: fa02 0000 8c06 7374 7269 6e67 9485 9481  ......string....
-00004610: 947d 9428 6aff 0200 006a 8605 0000 6a00  .}.(j....j....j.
-00004620: 0300 006a e902 0000 6a01 0300 004e 6a02  ...j....j....Nj.
-00004630: 0300 004e 7562 616a 0303 0000 7d94 286a  ...Nubaj....}.(j
-00004640: 0503 0000 5d94 6a07 0300 005d 946a 0903  ....].j....].j..
-00004650: 0000 5d94 6a0b 0300 005d 946a 0d03 0000  ..].j....].j....
-00004660: 5d94 756a 0f03 0000 6a34 0500 006a ff02  ].uj....j4...j..
-00004670: 0000 6a83 0500 0075 6261 6a03 0300 007d  ..j....ubaj....}
-00004680: 9428 6a05 0300 005d 946a 0703 0000 5d94  .(j....].j....].
-00004690: 6a09 0300 005d 946a 0b03 0000 5d94 6a0d  j....].j....].j.
-000046a0: 0300 005d 948c 0972 6566 646f 6d61 696e  ...]...refdomain
-000046b0: 946a 4b05 0000 8c0b 7265 6665 7870 6c69  .jK.....refexpli
-000046c0: 6369 7494 898c 0772 6566 7479 7065 946a  cit....reftype.j
-000046d0: 6a02 0000 8c09 7265 6674 6172 6765 7494  j.....reftarget.
-000046e0: 6a88 0500 006a 4f05 0000 886a 5005 0000  j....jO....jP...
-000046f0: 6ad2 0400 006a 5105 0000 4e75 6a0f 0300  j....jQ...Nuj...
-00004700: 006a 2f05 0000 6aff 0200 006a 6d05 0000  .j/...j....jm...
-00004710: 7562 6afa 0200 008c 0129 9485 9481 947d  ubj......).....}
-00004720: 9428 6aff 0200 006a 6d05 0000 6a00 0300  .(j....jm...j...
-00004730: 006a e902 0000 6a01 0300 004e 6a02 0300  .j....j....Nj...
-00004740: 004e 7562 6afa 0200 008c 0520 e280 9320  .Nubj...... ... 
-00004750: 9485 9481 947d 9428 6aff 0200 006a 6d05  .....}.(j....jm.
-00004760: 0000 6a00 0300 006a e902 0000 6a01 0300  ..j....j....j...
-00004770: 004e 6a02 0300 004e 7562 6afa 0200 008c  .Nj....Nubj.....
-00004780: 1045 6e64 2074 696d 6520 7374 7269 6e67  .End time string
-00004790: 2e94 8594 8194 7d94 286a ff02 0000 6a6d  ......}.(j....jm
-000047a0: 0500 006a 0003 0000 6ae9 0200 006a 0103  ...j....j....j..
-000047b0: 0000 4e6a 0203 0000 4e75 6265 6a03 0300  ..Nj....Nubej...
-000047c0: 007d 9428 6a05 0300 005d 946a 0703 0000  .}.(j....].j....
-000047d0: 5d94 6a09 0300 005d 946a 0b03 0000 5d94  ].j....].j....].
-000047e0: 6a0d 0300 005d 9475 6a0f 0300 006a dd04  j....].uj....j..
-000047f0: 0000 6aff 0200 006a 6a05 0000 7562 616a  ..j....jj...ubaj
-00004800: 0303 0000 7d94 286a 0503 0000 5d94 6a07  ....}.(j....].j.
-00004810: 0300 005d 946a 0903 0000 5d94 6a0b 0300  ...].j....].j...
-00004820: 005d 946a 0d03 0000 5d94 756a 0f03 0000  .].j....].uj....
-00004830: 6a12 0500 006a ff02 0000 6a0f 0500 0075  j....j....j....u
-00004840: 626a 1305 0000 2981 947d 9428 6aeb 0200  bj....)..}.(j...
-00004850: 0068 406a ec02 0000 5d94 6ade 0400 0029  .h@j....].j....)
-00004860: 8194 7d94 286a eb02 0000 8c3b 666f 726d  ..}.(j.....;form
-00004870: 6174 2028 7374 7269 6e67 2920 2d2d 2043  at (string) -- C
-00004880: 6f6e 7665 7273 696f 6e20 666f 726d 6174  onversion format
-00004890: 2066 6f72 2064 6174 6574 696d 652e 7374   for datetime.st
-000048a0: 7270 7469 6d65 2e94 6aec 0200 005d 9428  rptime..j....].(
-000048b0: 6a1c 0500 0029 8194 7d94 286a eb02 0000  j....)..}.(j....
-000048c0: 8c06 666f 726d 6174 946a ec02 0000 5d94  ..format.j....].
-000048d0: 6afa 0200 008c 0666 6f72 6d61 7494 8594  j......format...
-000048e0: 8194 7d94 286a ff02 0000 6abd 0500 006a  ..}.(j....j....j
-000048f0: 0003 0000 6ae9 0200 006a 0103 0000 4e6a  ....j....j....Nj
-00004900: 0203 0000 4e75 6261 6a03 0300 007d 9428  ....Nubaj....}.(
-00004910: 6a05 0300 005d 946a 0703 0000 5d94 6a09  j....].j....].j.
-00004920: 0300 005d 946a 0b03 0000 5d94 6a0d 0300  ...].j....].j...
-00004930: 005d 9475 6a0f 0300 006a 1b05 0000 6aff  .].uj....j....j.
-00004940: 0200 006a b905 0000 7562 6afa 0200 008c  ...j....ubj.....
-00004950: 0220 2894 8594 8194 7d94 286a ff02 0000  . (.....}.(j....
-00004960: 6ab9 0500 006a 0003 0000 6ae9 0200 006a  j....j....j....j
-00004970: 0103 0000 4e6a 0203 0000 4e75 626a 3005  ....Nj....Nubj0.
-00004980: 0000 2981 947d 9428 6aeb 0200 0068 406a  ..)..}.(j....h@j
-00004990: ec02 0000 5d94 6a35 0500 0029 8194 7d94  ....].j5...)..}.
-000049a0: 286a eb02 0000 8c06 7374 7269 6e67 946a  (j......string.j
-000049b0: ec02 0000 5d94 6afa 0200 008c 0673 7472  ....].j......str
-000049c0: 696e 6794 8594 8194 7d94 286a ff02 0000  ing.....}.(j....
-000049d0: 6ad2 0500 006a 0003 0000 6ae9 0200 006a  j....j....j....j
-000049e0: 0103 0000 4e6a 0203 0000 4e75 6261 6a03  ....Nj....Nubaj.
-000049f0: 0300 007d 9428 6a05 0300 005d 946a 0703  ...}.(j....].j..
-00004a00: 0000 5d94 6a09 0300 005d 946a 0b03 0000  ..].j....].j....
-00004a10: 5d94 6a0d 0300 005d 9475 6a0f 0300 006a  ].j....].uj....j
-00004a20: 3405 0000 6aff 0200 006a cf05 0000 7562  4...j....j....ub
-00004a30: 616a 0303 0000 7d94 286a 0503 0000 5d94  aj....}.(j....].
-00004a40: 6a07 0300 005d 946a 0903 0000 5d94 6a0b  j....].j....].j.
-00004a50: 0300 005d 946a 0d03 0000 5d94 8c09 7265  ...].j....]...re
-00004a60: 6664 6f6d 6169 6e94 6a4b 0500 008c 0b72  fdomain.jK.....r
-00004a70: 6566 6578 706c 6963 6974 9489 8c07 7265  efexplicit....re
-00004a80: 6674 7970 6594 6a6a 0200 008c 0972 6566  ftype.jj.....ref
-00004a90: 7461 7267 6574 946a d405 0000 6a4f 0500  target.j....jO..
-00004aa0: 0088 6a50 0500 006a d204 0000 6a51 0500  ..jP...j....jQ..
-00004ab0: 004e 756a 0f03 0000 6a2f 0500 006a ff02  .Nuj....j/...j..
-00004ac0: 0000 6ab9 0500 0075 626a fa02 0000 8c01  ..j....ubj......
-00004ad0: 2994 8594 8194 7d94 286a ff02 0000 6ab9  ).....}.(j....j.
-00004ae0: 0500 006a 0003 0000 6ae9 0200 006a 0103  ...j....j....j..
-00004af0: 0000 4e6a 0203 0000 4e75 626a fa02 0000  ..Nj....Nubj....
-00004b00: 8c05 20e2 8093 2094 8594 8194 7d94 286a  .. ... .....}.(j
-00004b10: ff02 0000 6ab9 0500 006a 0003 0000 6ae9  ....j....j....j.
-00004b20: 0200 006a 0103 0000 4e6a 0203 0000 4e75  ...j....Nj....Nu
-00004b30: 626a fa02 0000 8c28 436f 6e76 6572 7369  bj.....(Conversi
-00004b40: 6f6e 2066 6f72 6d61 7420 666f 7220 6461  on format for da
-00004b50: 7465 7469 6d65 2e73 7472 7074 696d 652e  tetime.strptime.
-00004b60: 9485 9481 947d 9428 6aff 0200 006a b905  .....}.(j....j..
-00004b70: 0000 6a00 0300 006a e902 0000 6a01 0300  ..j....j....j...
-00004b80: 004e 6a02 0300 004e 7562 656a 0303 0000  .Nj....Nubej....
-00004b90: 7d94 286a 0503 0000 5d94 6a07 0300 005d  }.(j....].j....]
-00004ba0: 946a 0903 0000 5d94 6a0b 0300 005d 946a  .j....].j....].j
-00004bb0: 0d03 0000 5d94 756a 0f03 0000 6add 0400  ....].uj....j...
-00004bc0: 006a ff02 0000 6ab6 0500 0075 6261 6a03  .j....j....ubaj.
-00004bd0: 0300 007d 9428 6a05 0300 005d 946a 0703  ...}.(j....].j..
-00004be0: 0000 5d94 6a09 0300 005d 946a 0b03 0000  ..].j....].j....
-00004bf0: 5d94 6a0d 0300 005d 9475 6a0f 0300 006a  ].j....].uj....j
-00004c00: 1205 0000 6aff 0200 006a 0f05 0000 7562  ....j....j....ub
-00004c10: 6a13 0500 0029 8194 7d94 286a eb02 0000  j....)..}.(j....
-00004c20: 6840 6aec 0200 005d 946a de04 0000 2981  h@j....].j....).
-00004c30: 947d 9428 6aeb 0200 008c 3964 656c 7461  .}.(j.....9delta
-00004c40: 2028 6469 6374 2920 2d2d 2054 696d 6564   (dict) -- Timed
-00004c50: 656c 7461 2061 7320 6172 6773 2066 6f72  elta as args for
-00004c60: 2064 6174 6574 696d 652e 7469 6d65 6465   datetime.timede
-00004c70: 6c74 612e 946a ec02 0000 5d94 286a 1c05  lta..j....].(j..
-00004c80: 0000 2981 947d 9428 6aeb 0200 008c 0564  ..)..}.(j......d
-00004c90: 656c 7461 946a ec02 0000 5d94 6afa 0200  elta.j....].j...
-00004ca0: 008c 0564 656c 7461 9485 9481 947d 9428  ...delta.....}.(
-00004cb0: 6aff 0200 006a 0906 0000 6a00 0300 006a  j....j....j....j
-00004cc0: e902 0000 6a01 0300 004e 6a02 0300 004e  ....j....Nj....N
-00004cd0: 7562 616a 0303 0000 7d94 286a 0503 0000  ubaj....}.(j....
-00004ce0: 5d94 6a07 0300 005d 946a 0903 0000 5d94  ].j....].j....].
-00004cf0: 6a0b 0300 005d 946a 0d03 0000 5d94 756a  j....].j....].uj
-00004d00: 0f03 0000 6a1b 0500 006a ff02 0000 6a05  ....j....j....j.
-00004d10: 0600 0075 626a fa02 0000 8c02 2028 9485  ...ubj...... (..
-00004d20: 9481 947d 9428 6aff 0200 006a 0506 0000  ...}.(j....j....
-00004d30: 6a00 0300 006a e902 0000 6a01 0300 004e  j....j....j....N
-00004d40: 6a02 0300 004e 7562 6a30 0500 0029 8194  j....Nubj0...)..
-00004d50: 7d94 286a eb02 0000 6840 6aec 0200 005d  }.(j....h@j....]
-00004d60: 946a 3505 0000 2981 947d 9428 6aeb 0200  .j5...)..}.(j...
-00004d70: 008c 0464 6963 7494 6aec 0200 005d 946a  ...dict.j....].j
-00004d80: fa02 0000 8c04 6469 6374 9485 9481 947d  ......dict.....}
-00004d90: 9428 6aff 0200 006a 1e06 0000 6a00 0300  .(j....j....j...
-00004da0: 006a e902 0000 6a01 0300 004e 6a02 0300  .j....j....Nj...
-00004db0: 004e 7562 616a 0303 0000 7d94 286a 0503  .Nubaj....}.(j..
-00004dc0: 0000 5d94 6a07 0300 005d 946a 0903 0000  ..].j....].j....
-00004dd0: 5d94 6a0b 0300 005d 946a 0d03 0000 5d94  ].j....].j....].
-00004de0: 756a 0f03 0000 6a34 0500 006a ff02 0000  uj....j4...j....
-00004df0: 6a1b 0600 0075 6261 6a03 0300 007d 9428  j....ubaj....}.(
-00004e00: 6a05 0300 005d 946a 0703 0000 5d94 6a09  j....].j....].j.
-00004e10: 0300 005d 946a 0b03 0000 5d94 6a0d 0300  ...].j....].j...
-00004e20: 005d 948c 0972 6566 646f 6d61 696e 946a  .]...refdomain.j
-00004e30: 4b05 0000 8c0b 7265 6665 7870 6c69 6369  K.....refexplici
-00004e40: 7494 898c 0772 6566 7479 7065 946a 6a02  t....reftype.jj.
-00004e50: 0000 8c09 7265 6674 6172 6765 7494 6a20  ....reftarget.j 
-00004e60: 0600 006a 4f05 0000 886a 5005 0000 6ad2  ...jO....jP...j.
-00004e70: 0400 006a 5105 0000 4e75 6a0f 0300 006a  ...jQ...Nuj....j
-00004e80: 2f05 0000 6aff 0200 006a 0506 0000 7562  /...j....j....ub
-00004e90: 6afa 0200 008c 0129 9485 9481 947d 9428  j......).....}.(
-00004ea0: 6aff 0200 006a 0506 0000 6a00 0300 006a  j....j....j....j
-00004eb0: e902 0000 6a01 0300 004e 6a02 0300 004e  ....j....Nj....N
-00004ec0: 7562 6afa 0200 008c 0520 e280 9320 9485  ubj...... ... ..
-00004ed0: 9481 947d 9428 6aff 0200 006a 0506 0000  ...}.(j....j....
-00004ee0: 6a00 0300 006a e902 0000 6a01 0300 004e  j....j....j....N
-00004ef0: 6a02 0300 004e 7562 6afa 0200 008c 2954  j....Nubj.....)T
-00004f00: 696d 6564 656c 7461 2061 7320 6172 6773  imedelta as args
-00004f10: 2066 6f72 2064 6174 6574 696d 652e 7469   for datetime.ti
-00004f20: 6d65 6465 6c74 612e 9485 9481 947d 9428  medelta......}.(
-00004f30: 6aff 0200 006a 0506 0000 6a00 0300 006a  j....j....j....j
-00004f40: e902 0000 6a01 0300 004e 6a02 0300 004e  ....j....Nj....N
-00004f50: 7562 656a 0303 0000 7d94 286a 0503 0000  ubej....}.(j....
-00004f60: 5d94 6a07 0300 005d 946a 0903 0000 5d94  ].j....].j....].
-00004f70: 6a0b 0300 005d 946a 0d03 0000 5d94 756a  j....].j....].uj
-00004f80: 0f03 0000 6add 0400 006a ff02 0000 6a02  ....j....j....j.
-00004f90: 0600 0075 6261 6a03 0300 007d 9428 6a05  ...ubaj....}.(j.
-00004fa0: 0300 005d 946a 0703 0000 5d94 6a09 0300  ...].j....].j...
-00004fb0: 005d 946a 0b03 0000 5d94 6a0d 0300 005d  .].j....].j....]
-00004fc0: 9475 6a0f 0300 006a 1205 0000 6aff 0200  .uj....j....j...
-00004fd0: 006a 0f05 0000 7562 6a13 0500 0029 8194  .j....ubj....)..
-00004fe0: 7d94 286a eb02 0000 6840 6aec 0200 005d  }.(j....h@j....]
-00004ff0: 946a de04 0000 2981 947d 9428 6aeb 0200  .j....)..}.(j...
-00005000: 008c 4663 6173 745f 7374 7220 2862 6f6f  ..Fcast_str (boo
-00005010: 6c29 202d 2d20 5768 6574 6865 7220 746f  l) -- Whether to
-00005020: 2063 6f6e 7665 7274 206f 7574 7075 7420   convert output 
-00005030: 746f 2073 7472 696e 6720 2864 6566 6175  to string (defau
-00005040: 6c74 2074 7275 6529 2e94 6aec 0200 005d  lt true)..j....]
-00005050: 9428 6a1c 0500 0029 8194 7d94 286a eb02  .(j....)..}.(j..
-00005060: 0000 8c08 6361 7374 5f73 7472 946a ec02  ....cast_str.j..
-00005070: 0000 5d94 6afa 0200 008c 0863 6173 745f  ..].j......cast_
-00005080: 7374 7294 8594 8194 7d94 286a ff02 0000  str.....}.(j....
-00005090: 6a55 0600 006a 0003 0000 6ae9 0200 006a  jU...j....j....j
-000050a0: 0103 0000 4e6a 0203 0000 4e75 6261 6a03  ....Nj....Nubaj.
-000050b0: 0300 007d 9428 6a05 0300 005d 946a 0703  ...}.(j....].j..
-000050c0: 0000 5d94 6a09 0300 005d 946a 0b03 0000  ..].j....].j....
-000050d0: 5d94 6a0d 0300 005d 9475 6a0f 0300 006a  ].j....].uj....j
-000050e0: 1b05 0000 6aff 0200 006a 5106 0000 7562  ....j....jQ...ub
-000050f0: 6afa 0200 008c 0220 2894 8594 8194 7d94  j...... (.....}.
-00005100: 286a ff02 0000 6a51 0600 006a 0003 0000  (j....jQ...j....
-00005110: 6ae9 0200 006a 0103 0000 4e6a 0203 0000  j....j....Nj....
-00005120: 4e75 626a 3005 0000 2981 947d 9428 6aeb  Nubj0...)..}.(j.
-00005130: 0200 0068 406a ec02 0000 5d94 6a35 0500  ...h@j....].j5..
-00005140: 0029 8194 7d94 286a eb02 0000 8c04 626f  .)..}.(j......bo
-00005150: 6f6c 946a ec02 0000 5d94 6afa 0200 008c  ol.j....].j.....
-00005160: 0462 6f6f 6c94 8594 8194 7d94 286a ff02  .bool.....}.(j..
-00005170: 0000 6a6a 0600 006a 0003 0000 6ae9 0200  ..jj...j....j...
-00005180: 006a 0103 0000 4e6a 0203 0000 4e75 6261  .j....Nj....Nuba
-00005190: 6a03 0300 007d 9428 6a05 0300 005d 946a  j....}.(j....].j
-000051a0: 0703 0000 5d94 6a09 0300 005d 946a 0b03  ....].j....].j..
-000051b0: 0000 5d94 6a0d 0300 005d 9475 6a0f 0300  ..].j....].uj...
-000051c0: 006a 3405 0000 6aff 0200 006a 6706 0000  .j4...j....jg...
-000051d0: 7562 616a 0303 0000 7d94 286a 0503 0000  ubaj....}.(j....
-000051e0: 5d94 6a07 0300 005d 946a 0903 0000 5d94  ].j....].j....].
-000051f0: 6a0b 0300 005d 946a 0d03 0000 5d94 8c09  j....].j....]...
-00005200: 7265 6664 6f6d 6169 6e94 6a4b 0500 008c  refdomain.jK....
-00005210: 0b72 6566 6578 706c 6963 6974 9489 8c07  .refexplicit....
-00005220: 7265 6674 7970 6594 6a6a 0200 008c 0972  reftype.jj.....r
-00005230: 6566 7461 7267 6574 946a 6c06 0000 6a4f  eftarget.jl...jO
-00005240: 0500 0088 6a50 0500 006a d204 0000 6a51  ....jP...j....jQ
-00005250: 0500 004e 756a 0f03 0000 6a2f 0500 006a  ...Nuj....j/...j
-00005260: ff02 0000 6a51 0600 0075 626a fa02 0000  ....jQ...ubj....
-00005270: 8c01 2994 8594 8194 7d94 286a ff02 0000  ..).....}.(j....
-00005280: 6a51 0600 006a 0003 0000 6ae9 0200 006a  jQ...j....j....j
-00005290: 0103 0000 4e6a 0203 0000 4e75 626a fa02  ....Nj....Nubj..
-000052a0: 0000 8c05 20e2 8093 2094 8594 8194 7d94  .... ... .....}.
-000052b0: 286a ff02 0000 6a51 0600 006a 0003 0000  (j....jQ...j....
-000052c0: 6ae9 0200 006a 0103 0000 4e6a 0203 0000  j....j....Nj....
-000052d0: 4e75 626a fa02 0000 8c33 5768 6574 6865  Nubj.....3Whethe
-000052e0: 7220 746f 2063 6f6e 7665 7274 206f 7574  r to convert out
-000052f0: 7075 7420 746f 2073 7472 696e 6720 2864  put to string (d
-00005300: 6566 6175 6c74 2074 7275 6529 2e94 8594  efault true)....
-00005310: 8194 7d94 286a ff02 0000 6a51 0600 006a  ..}.(j....jQ...j
-00005320: 0003 0000 6ae9 0200 006a 0103 0000 4e6a  ....j....j....Nj
-00005330: 0203 0000 4e75 6265 6a03 0300 007d 9428  ....Nubej....}.(
-00005340: 6a05 0300 005d 946a 0703 0000 5d94 6a09  j....].j....].j.
-00005350: 0300 005d 946a 0b03 0000 5d94 6a0d 0300  ...].j....].j...
-00005360: 005d 9475 6a0f 0300 006a dd04 0000 6aff  .].uj....j....j.
-00005370: 0200 006a 4e06 0000 7562 616a 0303 0000  ...jN...ubaj....
-00005380: 7d94 286a 0503 0000 5d94 6a07 0300 005d  }.(j....].j....]
-00005390: 946a 0903 0000 5d94 6a0b 0300 005d 946a  .j....].j....].j
-000053a0: 0d03 0000 5d94 756a 0f03 0000 6a12 0500  ....].uj....j...
-000053b0: 006a ff02 0000 6a0f 0500 0075 626a 1305  .j....j....ubj..
-000053c0: 0000 2981 947d 9428 6aeb 0200 0068 406a  ..)..}.(j....h@j
-000053d0: ec02 0000 5d94 6ade 0400 0029 8194 7d94  ....].j....)..}.
-000053e0: 286a eb02 0000 8c4d 666f 726d 6174 5f6f  (j.....Mformat_o
-000053f0: 7574 2028 7374 7269 6e67 2920 2d2d 2043  ut (string) -- C
-00005400: 6f6e 7665 7273 696f 6e20 666f 726d 6174  onversion format
-00005410: 2066 6f72 206f 7574 7075 7420 2864 6566   for output (def
-00005420: 6175 6c74 2073 616d 6520 746f 2066 6f72  ault same to for
-00005430: 6d61 7429 2e94 6aec 0200 005d 9428 6a1c  mat)..j....].(j.
-00005440: 0500 0029 8194 7d94 286a eb02 0000 8c0a  ...)..}.(j......
-00005450: 666f 726d 6174 5f6f 7574 946a ec02 0000  format_out.j....
-00005460: 5d94 6afa 0200 008c 0a66 6f72 6d61 745f  ].j......format_
-00005470: 6f75 7494 8594 8194 7d94 286a ff02 0000  out.....}.(j....
-00005480: 6aa1 0600 006a 0003 0000 6ae9 0200 006a  j....j....j....j
-00005490: 0103 0000 4e6a 0203 0000 4e75 6261 6a03  ....Nj....Nubaj.
-000054a0: 0300 007d 9428 6a05 0300 005d 946a 0703  ...}.(j....].j..
-000054b0: 0000 5d94 6a09 0300 005d 946a 0b03 0000  ..].j....].j....
-000054c0: 5d94 6a0d 0300 005d 9475 6a0f 0300 006a  ].j....].uj....j
-000054d0: 1b05 0000 6aff 0200 006a 9d06 0000 7562  ....j....j....ub
-000054e0: 6afa 0200 008c 0220 2894 8594 8194 7d94  j...... (.....}.
-000054f0: 286a ff02 0000 6a9d 0600 006a 0003 0000  (j....j....j....
-00005500: 6ae9 0200 006a 0103 0000 4e6a 0203 0000  j....j....Nj....
-00005510: 4e75 626a 3005 0000 2981 947d 9428 6aeb  Nubj0...)..}.(j.
-00005520: 0200 0068 406a ec02 0000 5d94 6a35 0500  ...h@j....].j5..
-00005530: 0029 8194 7d94 286a eb02 0000 8c06 7374  .)..}.(j......st
-00005540: 7269 6e67 946a ec02 0000 5d94 6afa 0200  ring.j....].j...
-00005550: 008c 0673 7472 696e 6794 8594 8194 7d94  ...string.....}.
-00005560: 286a ff02 0000 6ab6 0600 006a 0003 0000  (j....j....j....
-00005570: 6ae9 0200 006a 0103 0000 4e6a 0203 0000  j....j....Nj....
-00005580: 4e75 6261 6a03 0300 007d 9428 6a05 0300  Nubaj....}.(j...
-00005590: 005d 946a 0703 0000 5d94 6a09 0300 005d  .].j....].j....]
-000055a0: 946a 0b03 0000 5d94 6a0d 0300 005d 9475  .j....].j....].u
-000055b0: 6a0f 0300 006a 3405 0000 6aff 0200 006a  j....j4...j....j
-000055c0: b306 0000 7562 616a 0303 0000 7d94 286a  ....ubaj....}.(j
-000055d0: 0503 0000 5d94 6a07 0300 005d 946a 0903  ....].j....].j..
-000055e0: 0000 5d94 6a0b 0300 005d 946a 0d03 0000  ..].j....].j....
-000055f0: 5d94 8c09 7265 6664 6f6d 6169 6e94 6a4b  ]...refdomain.jK
-00005600: 0500 008c 0b72 6566 6578 706c 6963 6974  .....refexplicit
-00005610: 9489 8c07 7265 6674 7970 6594 6a6a 0200  ....reftype.jj..
-00005620: 008c 0972 6566 7461 7267 6574 946a b806  ...reftarget.j..
-00005630: 0000 6a4f 0500 0088 6a50 0500 006a d204  ..jO....jP...j..
-00005640: 0000 6a51 0500 004e 756a 0f03 0000 6a2f  ..jQ...Nuj....j/
-00005650: 0500 006a ff02 0000 6a9d 0600 0075 626a  ...j....j....ubj
-00005660: fa02 0000 8c01 2994 8594 8194 7d94 286a  ......).....}.(j
-00005670: ff02 0000 6a9d 0600 006a 0003 0000 6ae9  ....j....j....j.
-00005680: 0200 006a 0103 0000 4e6a 0203 0000 4e75  ...j....Nj....Nu
-00005690: 626a fa02 0000 8c05 20e2 8093 2094 8594  bj...... ... ...
-000056a0: 8194 7d94 286a ff02 0000 6a9d 0600 006a  ..}.(j....j....j
-000056b0: 0003 0000 6ae9 0200 006a 0103 0000 4e6a  ....j....j....Nj
-000056c0: 0203 0000 4e75 626a fa02 0000 8c2e 436f  ....Nubj......Co
-000056d0: 6e76 6572 7369 6f6e 2066 6f72 6d61 7420  nversion format 
-000056e0: 666f 7220 6f75 7470 7574 2028 6465 6661  for output (defa
-000056f0: 756c 7420 7361 6d65 2074 6f20 9485 9481  ult same to ....
-00005700: 947d 9428 6aff 0200 006a 9d06 0000 6a00  .}.(j....j....j.
-00005710: 0300 006a e902 0000 6a01 0300 004e 6a02  ...j....j....Nj.
-00005720: 0300 004e 7562 6aee 0200 008c 0673 7472  ...Nubj......str
-00005730: 6f6e 6794 9394 2981 947d 9428 6aeb 0200  ong...)..}.(j...
-00005740: 008c 0a2a 2a66 6f72 6d61 742a 2a94 6aec  ...**format**.j.
-00005750: 0200 005d 946a fa02 0000 8c06 666f 726d  ...].j......form
-00005760: 6174 9485 9481 947d 9428 6aff 0200 006a  at.....}.(j....j
-00005770: dc06 0000 6a00 0300 006a e902 0000 6a01  ....j....j....j.
-00005780: 0300 004e 6a02 0300 004e 7562 616a 0303  ...Nj....Nubaj..
-00005790: 0000 7d94 286a 0503 0000 5d94 6a07 0300  ..}.(j....].j...
-000057a0: 005d 946a 0903 0000 5d94 6a0b 0300 005d  .].j....].j....]
-000057b0: 946a 0d03 0000 5d94 756a 0f03 0000 6ada  .j....].uj....j.
-000057c0: 0600 006a ff02 0000 6a9d 0600 006a 0003  ...j....j....j..
-000057d0: 0000 6ae9 0200 006a 0103 0000 4e6a 0203  ..j....j....Nj..
-000057e0: 0000 4e75 626a fa02 0000 8c02 292e 9485  ..Nubj......)...
-000057f0: 9481 947d 9428 6aff 0200 006a 9d06 0000  ...}.(j....j....
-00005800: 6a00 0300 006a e902 0000 6a01 0300 004e  j....j....j....N
-00005810: 6a02 0300 004e 7562 656a 0303 0000 7d94  j....Nubej....}.
-00005820: 286a 0503 0000 5d94 6a07 0300 005d 946a  (j....].j....].j
-00005830: 0903 0000 5d94 6a0b 0300 005d 946a 0d03  ....].j....].j..
-00005840: 0000 5d94 756a 0f03 0000 6add 0400 006a  ..].uj....j....j
-00005850: ff02 0000 6a9a 0600 0075 6261 6a03 0300  ....j....ubaj...
-00005860: 007d 9428 6a05 0300 005d 946a 0703 0000  .}.(j....].j....
-00005870: 5d94 6a09 0300 005d 946a 0b03 0000 5d94  ].j....].j....].
-00005880: 6a0d 0300 005d 9475 6a0f 0300 006a 1205  j....].uj....j..
-00005890: 0000 6aff 0200 006a 0f05 0000 7562 656a  ..j....j....ubej
-000058a0: 0303 0000 7d94 286a 0503 0000 5d94 6a07  ....}.(j....].j.
-000058b0: 0300 005d 946a 0903 0000 5d94 6a0b 0300  ...].j....].j...
-000058c0: 005d 946a 0d03 0000 5d94 756a 0f03 0000  .].j....].uj....
-000058d0: 6a0d 0500 006a ff02 0000 6a0a 0500 0075  j....j....j....u
-000058e0: 6261 6a03 0300 007d 9428 6a05 0300 005d  baj....}.(j....]
-000058f0: 946a 0703 0000 5d94 6a09 0300 005d 946a  .j....].j....].j
-00005900: 0b03 0000 5d94 6a0d 0300 005d 9475 6a0f  ....].j....].uj.
-00005910: 0300 006a 0805 0000 6aff 0200 006a f504  ...j....j....j..
-00005920: 0000 7562 656a 0303 0000 7d94 286a 0503  ..ubej....}.(j..
-00005930: 0000 5d94 6a07 0300 005d 946a 0903 0000  ..].j....].j....
-00005940: 5d94 6a0b 0300 005d 946a 0d03 0000 5d94  ].j....].j....].
-00005950: 756a 0f03 0000 6af3 0400 006a ff02 0000  uj....j....j....
-00005960: 6af0 0400 0075 626a f404 0000 2981 947d  j....ubj....)..}
-00005970: 9428 6aeb 0200 0068 406a ec02 0000 5d94  .(j....h@j....].
-00005980: 286a f904 0000 2981 947d 9428 6aeb 0200  (j....)..}.(j...
-00005990: 008c 0b52 6574 7572 6e20 7479 7065 946a  ...Return type.j
-000059a0: ec02 0000 5d94 6afa 0200 008c 0b52 6574  ....].j......Ret
-000059b0: 7572 6e20 7479 7065 9485 9481 947d 9428  urn type.....}.(
-000059c0: 6aff 0200 006a 0f07 0000 6a00 0300 006a  j....j....j....j
-000059d0: e902 0000 6a01 0300 004e 6a02 0300 004e  ....j....Nj....N
-000059e0: 7562 616a 0303 0000 7d94 286a 0503 0000  ubaj....}.(j....
-000059f0: 5d94 6a07 0300 005d 946a 0903 0000 5d94  ].j....].j....].
-00005a00: 6a0b 0300 005d 946a 0d03 0000 5d94 756a  j....].j....].uj
-00005a10: 0f03 0000 6af8 0400 006a ff02 0000 6a0c  ....j....j....j.
-00005a20: 0700 006a 0103 0000 6a62 0300 006a 0203  ...j....jb...j..
-00005a30: 0000 4b00 7562 6a09 0500 0029 8194 7d94  ..K.ubj....)..}.
-00005a40: 286a eb02 0000 6840 6aec 0200 005d 946a  (j....h@j....].j
-00005a50: de04 0000 2981 947d 9428 6aeb 0200 008c  ....)..}.(j.....
-00005a60: 256c 6973 7420 6f66 2073 7472 696e 6720  %list of string 
-00005a70: 286f 7220 6461 7465 7469 6d65 2e64 6174  (or datetime.dat
-00005a80: 6574 696d 6529 946a ec02 0000 5d94 286a  etime).j....].(j
-00005a90: 3005 0000 2981 947d 9428 6aeb 0200 0068  0...)..}.(j....h
-00005aa0: 406a ec02 0000 5d94 6afa 0200 008c 046c  @j....].j......l
-00005ab0: 6973 7494 8594 8194 7d94 286a ff02 0000  ist.....}.(j....
-00005ac0: 6a24 0700 006a 0003 0000 6ae9 0200 006a  j$...j....j....j
-00005ad0: 0103 0000 4e6a 0203 0000 4e75 6261 6a03  ....Nj....Nubaj.
-00005ae0: 0300 007d 9428 6a05 0300 005d 946a 0703  ...}.(j....].j..
-00005af0: 0000 5d94 6a09 0300 005d 946a 0b03 0000  ..].j....].j....
-00005b00: 5d94 6a0d 0300 005d 948c 0972 6566 646f  ].j....]...refdo
-00005b10: 6d61 696e 946a 4b05 0000 8c0b 7265 6665  main.jK.....refe
-00005b20: 7870 6c69 6369 7494 898c 0772 6566 7479  xplicit....refty
-00005b30: 7065 946a 6a02 0000 8c09 7265 6674 6172  pe.jj.....reftar
-00005b40: 6765 7494 8c04 6c69 7374 946a 4f05 0000  get...list.jO...
-00005b50: 886a 5005 0000 6ad2 0400 006a 5105 0000  .jP...j....jQ...
-00005b60: 4e75 6a0f 0300 006a 2f05 0000 6aff 0200  Nuj....j/...j...
-00005b70: 006a 2007 0000 7562 6afa 0200 008c 0420  .j ...ubj...... 
-00005b80: 6f66 2094 8594 8194 7d94 286a ff02 0000  of .....}.(j....
-00005b90: 6a20 0700 006a 0003 0000 6ae9 0200 006a  j ...j....j....j
-00005ba0: 0103 0000 4e6a 0203 0000 4e75 626a 3005  ....Nj....Nubj0.
-00005bb0: 0000 2981 947d 9428 6aeb 0200 0068 406a  ..)..}.(j....h@j
-00005bc0: ec02 0000 5d94 6afa 0200 008c 0673 7472  ....].j......str
-00005bd0: 696e 6794 8594 8194 7d94 286a ff02 0000  ing.....}.(j....
-00005be0: 6a3a 0700 006a 0003 0000 6ae9 0200 006a  j:...j....j....j
-00005bf0: 0103 0000 4e6a 0203 0000 4e75 6261 6a03  ....Nj....Nubaj.
-00005c00: 0300 007d 9428 6a05 0300 005d 946a 0703  ...}.(j....].j..
-00005c10: 0000 5d94 6a09 0300 005d 946a 0b03 0000  ..].j....].j....
-00005c20: 5d94 6a0d 0300 005d 948c 0972 6566 646f  ].j....]...refdo
-00005c30: 6d61 696e 946a 4b05 0000 8c0b 7265 6665  main.jK.....refe
-00005c40: 7870 6c69 6369 7494 898c 0772 6566 7479  xplicit....refty
-00005c50: 7065 946a 6a02 0000 8c09 7265 6674 6172  pe.jj.....reftar
-00005c60: 6765 7494 8c06 7374 7269 6e67 946a 4f05  get...string.jO.
-00005c70: 0000 886a 5005 0000 6ad2 0400 006a 5105  ...jP...j....jQ.
-00005c80: 0000 4e75 6a0f 0300 006a 2f05 0000 6aff  ..Nuj....j/...j.
-00005c90: 0200 006a 2007 0000 7562 6afa 0200 008c  ...j ...ubj.....
-00005ca0: 0520 286f 7220 9485 9481 947d 9428 6aff  . (or .....}.(j.
-00005cb0: 0200 006a 2007 0000 6a00 0300 006a e902  ...j ...j....j..
-00005cc0: 0000 6a01 0300 004e 6a02 0300 004e 7562  ..j....Nj....Nub
-00005cd0: 6a30 0500 0029 8194 7d94 286a eb02 0000  j0...)..}.(j....
-00005ce0: 6840 6aec 0200 005d 946a fa02 0000 8c11  h@j....].j......
-00005cf0: 6461 7465 7469 6d65 2e64 6174 6574 696d  datetime.datetim
-00005d00: 6594 8594 8194 7d94 286a ff02 0000 6a50  e.....}.(j....jP
-00005d10: 0700 006a 0003 0000 6ae9 0200 006a 0103  ...j....j....j..
-00005d20: 0000 4e6a 0203 0000 4e75 6261 6a03 0300  ..Nj....Nubaj...
-00005d30: 007d 9428 6a05 0300 005d 946a 0703 0000  .}.(j....].j....
-00005d40: 5d94 6a09 0300 005d 946a 0b03 0000 5d94  ].j....].j....].
-00005d50: 6a0d 0300 005d 948c 0972 6566 646f 6d61  j....]...refdoma
-00005d60: 696e 946a 4b05 0000 8c0b 7265 6665 7870  in.jK.....refexp
-00005d70: 6c69 6369 7494 898c 0772 6566 7479 7065  licit....reftype
-00005d80: 946a 6a02 0000 8c09 7265 6674 6172 6765  .jj.....reftarge
-00005d90: 7494 8c11 6461 7465 7469 6d65 2e64 6174  t...datetime.dat
-00005da0: 6574 696d 6594 6a4f 0500 0088 6a50 0500  etime.jO....jP..
-00005db0: 006a d204 0000 6a51 0500 004e 756a 0f03  .j....jQ...Nuj..
-00005dc0: 0000 6a2f 0500 006a ff02 0000 6a20 0700  ..j/...j....j ..
-00005dd0: 0075 626a fa02 0000 8c01 2994 8594 8194  .ubj......).....
-00005de0: 7d94 286a ff02 0000 6a20 0700 006a 0003  }.(j....j ...j..
-00005df0: 0000 6ae9 0200 006a 0103 0000 4e6a 0203  ..j....j....Nj..
-00005e00: 0000 4e75 6265 6a03 0300 007d 9428 6a05  ..Nubej....}.(j.
-00005e10: 0300 005d 946a 0703 0000 5d94 6a09 0300  ...].j....].j...
-00005e20: 005d 946a 0b03 0000 5d94 6a0d 0300 005d  .].j....].j....]
-00005e30: 9475 6a0f 0300 006a dd04 0000 6aff 0200  .uj....j....j...
-00005e40: 006a 1d07 0000 7562 616a 0303 0000 7d94  .j....ubaj....}.
-00005e50: 286a 0503 0000 5d94 6a07 0300 005d 946a  (j....].j....].j
-00005e60: 0903 0000 5d94 6a0b 0300 005d 946a 0d03  ....].j....].j..
-00005e70: 0000 5d94 756a 0f03 0000 6a08 0500 006a  ..].uj....j....j
-00005e80: ff02 0000 6a0c 0700 0075 6265 6a03 0300  ....j....ubej...
-00005e90: 007d 9428 6a05 0300 005d 946a 0703 0000  .}.(j....].j....
-00005ea0: 5d94 6a09 0300 005d 946a 0b03 0000 5d94  ].j....].j....].
-00005eb0: 6a0d 0300 005d 9475 6a0f 0300 006a f304  j....].uj....j..
-00005ec0: 0000 6aff 0200 006a f004 0000 7562 656a  ..j....j....ubej
-00005ed0: 0303 0000 7d94 286a 0503 0000 5d94 6a07  ....}.(j....].j.
-00005ee0: 0300 005d 946a 0903 0000 5d94 6a0b 0300  ...].j....].j...
-00005ef0: 005d 946a 0d03 0000 5d94 756a 0f03 0000  .].j....].uj....
-00005f00: 6aee 0400 006a ff02 0000 6ada 0400 006a  j....j....j....j
-00005f10: 0003 0000 6ae9 0200 006a 0103 0000 4e6a  ....j....j....Nj
-00005f20: 0203 0000 4e75 6265 6a03 0300 007d 9428  ....Nubej....}.(
-00005f30: 6a05 0300 005d 946a 0703 0000 5d94 6a09  j....].j....].j.
-00005f40: 0300 005d 946a 0b03 0000 5d94 6a0d 0300  ...].j....].j...
-00005f50: 005d 9475 6a0f 0300 006a d804 0000 6aff  .].uj....j....j.
-00005f60: 0200 006a 4503 0000 6a00 0300 006a e902  ...jE...j....j..
-00005f70: 0000 6a01 0300 006a 6203 0000 6a02 0300  ..j....jb...j...
-00005f80: 004b 0175 6265 6a03 0300 007d 9428 6a05  .K.ubej....}.(j.
-00005f90: 0300 005d 946a 0703 0000 5d94 286a 4b05  ...].j....].(jK.
-00005fa0: 0000 8c08 6675 6e63 7469 6f6e 9465 6a09  ....function.ej.
-00005fb0: 0300 005d 946a 0b03 0000 5d94 6a0d 0300  ...].j....].j...
-00005fc0: 005d 9468 736a 4b05 0000 8c07 6f62 6a74  .].hsjK.....objt
-00005fd0: 7970 6594 6a87 0700 008c 0864 6573 6374  ype.j......desct
-00005fe0: 7970 6594 6a87 0700 008c 076e 6f69 6e64  ype.j......noind
-00005ff0: 6578 9489 8c0c 6e6f 696e 6465 7865 6e74  ex....noindexent
-00006000: 7279 9489 8c0f 6e6f 636f 6e74 656e 7473  ry....nocontents
-00006010: 656e 7472 7994 8975 6a0f 0300 006a 4303  entry..uj....jC.
-00006020: 0000 6a00 0300 006a e902 0000 6aff 0200  ..j....j....j...
-00006030: 006a 2203 0000 6a01 0300 004e 6a02 0300  .j"...j....Nj...
-00006040: 004e 7562 6ade 0400 0029 8194 7d94 286a  .Nubj....)..}.(j
-00006050: eb02 0000 8c0b 2a2a 4578 616d 706c 652a  ......**Example*
-00006060: 2a94 6aec 0200 005d 946a db06 0000 2981  *.j....].j....).
-00006070: 947d 9428 6aeb 0200 006a 9207 0000 6aec  .}.(j....j....j.
-00006080: 0200 005d 946a fa02 0000 8c07 4578 616d  ...].j......Exam
-00006090: 706c 6594 8594 8194 7d94 286a ff02 0000  ple.....}.(j....
-000060a0: 6a94 0700 006a 0003 0000 6ae9 0200 006a  j....j....j....j
-000060b0: 0103 0000 4e6a 0203 0000 4e75 6261 6a03  ....Nj....Nubaj.
-000060c0: 0300 007d 9428 6a05 0300 005d 946a 0703  ...}.(j....].j..
-000060d0: 0000 5d94 6a09 0300 005d 946a 0b03 0000  ..].j....].j....
-000060e0: 5d94 6a0d 0300 005d 9475 6a0f 0300 006a  ].j....].uj....j
-000060f0: da06 0000 6aff 0200 006a 9007 0000 7562  ....j....j....ub
-00006100: 616a 0303 0000 7d94 286a 0503 0000 5d94  aj....}.(j....].
-00006110: 6a07 0300 005d 946a 0903 0000 5d94 6a0b  j....].j....].j.
-00006120: 0300 005d 946a 0d03 0000 5d94 756a 0f03  ...].j....].uj..
-00006130: 0000 6add 0400 006a 0103 0000 6a10 0300  ..j....j....j...
-00006140: 006a 0203 0000 4b0c 6aff 0200 006a 2203  .j....K.j....j".
-00006150: 0000 6a00 0300 006a e902 0000 7562 6aee  ..j....j....ubj.
-00006160: 0200 008c 0d6c 6974 6572 616c 5f62 6c6f  .....literal_blo
-00006170: 636b 9493 9429 8194 7d94 286a eb02 0000  ck...)..}.(j....
-00006180: 8cf9 696d 706f 7274 2063 6f6f 6b69 6573  ..import cookies
-00006190: 5f75 7469 6c69 7469 6573 2061 7320 6375  _utilities as cu
-000061a0: 0a64 6174 6573 203d 2063 752e 6765 745f  .dates = cu.get_
-000061b0: 6461 7465 7328 0a20 2020 2073 7461 7274  dates(.    start
-000061c0: 3d27 3230 3136 2d30 372d 3031 2030 323a  ='2016-07-01 02:
-000061d0: 3030 3a30 3027 2c0a 2020 2020 656e 643d  00:00',.    end=
-000061e0: 2732 3031 362d 3037 2d30 3220 3031 3a30  '2016-07-02 01:0
-000061f0: 303a 3030 272c 0a20 2020 2066 6f72 6d61  0:00',.    forma
-00006200: 743d 2725 592d 256d 2d25 6420 2548 3a25  t='%Y-%m-%d %H:%
-00006210: 4d3a 2553 272c 0a20 2020 2064 656c 7461  M:%S',.    delta
-00006220: 3d7b 2768 6f75 7273 273a 2031 7d29 0a23  ={'hours': 1}).#
-00006230: 205b 2732 3031 362d 3037 2d30 3120 3032   ['2016-07-01 02
-00006240: 3a30 303a 3030 272c 2027 3230 3136 2d30  :00:00', '2016-0
-00006250: 372d 3031 2030 333a 3030 3a30 3027 2c20  7-01 03:00:00', 
-00006260: 2e2e 2e2c 2027 3230 3136 2d30 372d 3032  ..., '2016-07-02
-00006270: 2030 313a 3030 3a30 3027 5d94 6aec 0200   01:00:00'].j...
-00006280: 005d 946a fa02 0000 8cf9 696d 706f 7274  .].j......import
-00006290: 2063 6f6f 6b69 6573 5f75 7469 6c69 7469   cookies_utiliti
-000062a0: 6573 2061 7320 6375 0a64 6174 6573 203d  es as cu.dates =
-000062b0: 2063 752e 6765 745f 6461 7465 7328 0a20   cu.get_dates(. 
-000062c0: 2020 2073 7461 7274 3d27 3230 3136 2d30     start='2016-0
-000062d0: 372d 3031 2030 323a 3030 3a30 3027 2c0a  7-01 02:00:00',.
-000062e0: 2020 2020 656e 643d 2732 3031 362d 3037      end='2016-07
-000062f0: 2d30 3220 3031 3a30 303a 3030 272c 0a20  -02 01:00:00',. 
-00006300: 2020 2066 6f72 6d61 743d 2725 592d 256d     format='%Y-%m
-00006310: 2d25 6420 2548 3a25 4d3a 2553 272c 0a20  -%d %H:%M:%S',. 
-00006320: 2020 2064 656c 7461 3d7b 2768 6f75 7273     delta={'hours
-00006330: 273a 2031 7d29 0a23 205b 2732 3031 362d  ': 1}).# ['2016-
-00006340: 3037 2d30 3120 3032 3a30 303a 3030 272c  07-01 02:00:00',
-00006350: 2027 3230 3136 2d30 372d 3031 2030 333a   '2016-07-01 03:
-00006360: 3030 3a30 3027 2c20 2e2e 2e2c 2027 3230  00:00', ..., '20
-00006370: 3136 2d30 372d 3032 2030 313a 3030 3a30  16-07-02 01:00:0
-00006380: 3027 5d94 8594 8194 7d94 6aff 0200 006a  0'].....}.j....j
-00006390: a907 0000 7362 616a 0303 0000 7d94 286a  ....sbaj....}.(j
-000063a0: 0503 0000 5d94 6a07 0300 005d 946a 0903  ....].j....].j..
-000063b0: 0000 5d94 6a0b 0300 005d 946a 0d03 0000  ..].j....].j....
-000063c0: 5d94 6a60 0300 006a 6103 0000 8c05 666f  ].j`...ja.....fo
-000063d0: 7263 6594 8968 4b8c 0670 7974 686f 6e94  rce..hK..python.
-000063e0: 8c0e 6869 6768 6c69 6768 745f 6172 6773  ..highlight_args
-000063f0: 947d 9475 6a0f 0300 006a a707 0000 6a01  .}.uj....j....j.
-00006400: 0300 006a 1003 0000 6a02 0300 004b 0e6a  ...j....j....K.j
-00006410: ff02 0000 6a22 0300 006a 0003 0000 6ae9  ....j"...j....j.
-00006420: 0200 0075 6265 6a03 0300 007d 9428 6a05  ...ubej....}.(j.
-00006430: 0300 005d 948c 1b63 6f6f 6b69 6573 2d75  ...]...cookies-u
-00006440: 7469 6c69 7469 6573 2d67 6574 2d64 6174  tilities-get-dat
-00006450: 6573 9461 6a07 0300 005d 946a 0903 0000  es.aj....].j....
-00006460: 5d94 8c1b 636f 6f6b 6965 735f 7574 696c  ]...cookies_util
-00006470: 6974 6965 732e 6765 745f 6461 7465 7394  ities.get_dates.
-00006480: 616a 0b03 0000 5d94 6a0d 0300 005d 9475  aj....].j....].u
-00006490: 6a0f 0300 0068 306a ff02 0000 6a11 0300  j....h0j....j...
-000064a0: 006a 0003 0000 6ae9 0200 006a 0103 0000  .j....j....j....
-000064b0: 6a10 0300 006a 0203 0000 4b08 7562 656a  j....j....K.ubej
-000064c0: 0303 0000 7d94 286a 0503 0000 5d94 8c09  ....}.(j....]...
-000064d0: 6675 6e63 7469 6f6e 7394 616a 0703 0000  functions.aj....
-000064e0: 5d94 6a09 0300 005d 948c 0966 756e 6374  ].j....]...funct
-000064f0: 696f 6e73 9461 6a0b 0300 005d 946a 0d03  ions.aj....].j..
-00006500: 0000 5d94 756a 0f03 0000 6830 6aff 0200  ..].uj....h0j...
-00006510: 006a f002 0000 6a00 0300 006a e902 0000  .j....j....j....
-00006520: 6a01 0300 006a 1003 0000 6a02 0300 004b  j....j....j....K
-00006530: 0575 626a ef02 0000 2981 947d 9428 6aeb  .ubj....)..}.(j.
-00006540: 0200 0068 406a ec02 0000 5d94 286a f402  ...h@j....].(j..
-00006550: 0000 2981 947d 9428 6aeb 0200 008c 0743  ..)..}.(j......C
-00006560: 6c61 7373 6573 946a ec02 0000 5d94 6afa  lasses.j....].j.
-00006570: 0200 008c 0743 6c61 7373 6573 9485 9481  .....Classes....
-00006580: 947d 9428 6aff 0200 006a ce07 0000 6a00  .}.(j....j....j.
-00006590: 0300 006a e902 0000 6a01 0300 004e 6a02  ...j....j....Nj.
-000065a0: 0300 004e 7562 616a 0303 0000 7d94 286a  ...Nubaj....}.(j
-000065b0: 0503 0000 5d94 6a07 0300 005d 946a 0903  ....].j....].j..
-000065c0: 0000 5d94 6a0b 0300 005d 946a 0d03 0000  ..].j....].j....
-000065d0: 5d94 756a 0f03 0000 6af3 0200 006a ff02  ].uj....j....j..
-000065e0: 0000 6acb 0700 006a 0003 0000 6ae9 0200  ..j....j....j...
-000065f0: 006a 0103 0000 6a10 0300 006a 0203 0000  .j....j....j....
-00006600: 4b19 7562 6aef 0200 0029 8194 7d94 286a  K.ubj....)..}.(j
-00006610: eb02 0000 6840 6aec 0200 005d 9428 6af4  ....h@j....].(j.
-00006620: 0200 0029 8194 7d94 286a eb02 0000 8c1b  ...)..}.(j......
-00006630: 636f 6f6b 6965 735f 7574 696c 6974 6965  cookies_utilitie
-00006640: 732e 5374 6f70 7761 7463 6894 6aec 0200  s.Stopwatch.j...
-00006650: 005d 946a fa02 0000 8c1b 636f 6f6b 6965  .].j......cookie
-00006660: 735f 7574 696c 6974 6965 732e 5374 6f70  s_utilities.Stop
-00006670: 7761 7463 6894 8594 8194 7d94 286a ff02  watch.....}.(j..
-00006680: 0000 6adf 0700 006a 0003 0000 6ae9 0200  ..j....j....j...
-00006690: 006a 0103 0000 4e6a 0203 0000 4e75 6261  .j....Nj....Nuba
-000066a0: 6a03 0300 007d 9428 6a05 0300 005d 946a  j....}.(j....].j
-000066b0: 0703 0000 5d94 6a09 0300 005d 946a 0b03  ....].j....].j..
-000066c0: 0000 5d94 6a0d 0300 005d 9475 6a0f 0300  ..].j....].uj...
-000066d0: 006a f302 0000 6aff 0200 006a dc07 0000  .j....j....j....
-000066e0: 6a00 0300 006a e902 0000 6a01 0300 006a  j....j....j....j
-000066f0: 1003 0000 6a02 0300 004b 1c75 626a 3303  ....j....K.ubj3.
-00006700: 0000 2981 947d 9428 6aeb 0200 0068 406a  ..)..}.(j....h@j
-00006710: ec02 0000 5d94 6a03 0300 007d 9428 6a05  ....].j....}.(j.
-00006720: 0300 005d 946a 0703 0000 5d94 6a09 0300  ...].j....].j...
-00006730: 005d 946a 0b03 0000 5d94 6a0d 0300 005d  .].j....].j....]
-00006740: 948c 0765 6e74 7269 6573 945d 9428 6a3f  ...entries.].(j?
-00006750: 0300 008c 2653 746f 7077 6174 6368 2028  ....&Stopwatch (
-00006760: 636c 6173 7320 696e 2063 6f6f 6b69 6573  class in cookies
-00006770: 5f75 7469 6c69 7469 6573 2994 8c1b 636f  _utilities)...co
-00006780: 6f6b 6965 735f 7574 696c 6974 6965 732e  okies_utilities.
-00006790: 5374 6f70 7761 7463 6894 6840 4e74 9461  Stopwatch.h@Nt.a
-000067a0: 756a 0f03 0000 6859 6aff 0200 006a dc07  uj....hYj....j..
-000067b0: 0000 6a00 0300 006a e902 0000 6a01 0300  ..j....j....j...
-000067c0: 004e 6a02 0300 004e 7562 6a44 0300 0029  .Nj....NubjD...)
-000067d0: 8194 7d94 286a eb02 0000 6840 6aec 0200  ..}.(j....h@j...
-000067e0: 005d 9428 6a49 0300 0029 8194 7d94 286a  .].(jI...)..}.(j
-000067f0: eb02 0000 8c0b 5374 6f70 7761 7463 6828  ......Stopwatch(
-00006800: 2994 6aec 0200 005d 9428 6ae6 0200 008c  ).j....].(j.....
-00006810: 0f64 6573 635f 616e 6e6f 7461 7469 6f6e  .desc_annotation
-00006820: 9493 9429 8194 7d94 286a eb02 0000 8c32  ...)..}.(j.....2
-00006830: 5b3c 2374 6578 743a 2027 636c 6173 7327  [<#text: 'class'
-00006840: 3e2c 203c 6465 7363 5f73 6967 5f73 7061  >, <desc_sig_spa
-00006850: 6365 3a20 3c23 7465 7874 3a20 2720 273e  ce: <#text: ' '>
-00006860: 3e5d 946a ec02 0000 5d94 286a fa02 0000  >].j....].(j....
-00006870: 8c05 636c 6173 7394 8594 8194 7d94 286a  ..class.....}.(j
-00006880: ff02 0000 6a04 0800 006a 0003 0000 6ae9  ....j....j....j.
-00006890: 0200 006a 0103 0000 4e6a 0203 0000 4e75  ...j....Nj....Nu
-000068a0: 626a e602 0000 8c0e 6465 7363 5f73 6967  bj......desc_sig
-000068b0: 5f73 7061 6365 9493 9429 8194 7d94 286a  _space...)..}.(j
-000068c0: eb02 0000 8c01 2094 6aec 0200 005d 946a  ...... .j....].j
-000068d0: fa02 0000 8c01 2094 8594 8194 7d94 286a  ...... .....}.(j
-000068e0: ff02 0000 6a0e 0800 006a 0003 0000 6ae9  ....j....j....j.
-000068f0: 0200 006a 0103 0000 4e6a 0203 0000 4e75  ...j....Nj....Nu
-00006900: 6261 6a03 0300 007d 9428 6a05 0300 005d  baj....}.(j....]
-00006910: 946a 0703 0000 5d94 8c01 7794 616a 0903  .j....]...w.aj..
-00006920: 0000 5d94 6a0b 0300 005d 946a 0d03 0000  ..].j....].j....
-00006930: 5d94 756a 0f03 0000 6a0c 0800 006a ff02  ].uj....j....j..
-00006940: 0000 6a04 0800 0075 6265 6a03 0300 007d  ..j....ubej....}
-00006950: 9428 6a05 0300 005d 946a 0703 0000 5d94  .(j....].j....].
-00006960: 6a09 0300 005d 946a 0b03 0000 5d94 6a0d  j....].j....].j.
-00006970: 0300 005d 946a 6003 0000 6a61 0300 0075  ...].j`...ja...u
-00006980: 6a0f 0300 006a 0208 0000 6aff 0200 006a  j....j....j....j
-00006990: fe07 0000 6a00 0300 006a e902 0000 6a01  ....j....j....j.
-000069a0: 0300 008c 7c43 3a5c 5573 6572 735c 632d  ....|C:\Users\c-
-000069b0: 6d69 685c 7370 6163 655c 636f 6f6b 6965  mih\space\cookie
-000069c0: 735f 7574 696c 6974 6965 735c 7372 635c  s_utilities\src\
-000069d0: 636f 6f6b 6965 735f 7574 696c 6974 6965  cookies_utilitie
-000069e0: 735c 7374 6f70 7761 7463 682e 7079 3a64  s\stopwatch.py:d
-000069f0: 6f63 7374 7269 6e67 206f 6620 636f 6f6b  ocstring of cook
-00006a00: 6965 735f 7574 696c 6974 6965 732e 7374  ies_utilities.st
-00006a10: 6f70 7761 7463 682e 5374 6f70 7761 7463  opwatch.Stopwatc
-00006a20: 6894 6a02 0300 004b 0175 626a 4f03 0000  h.j....K.ubjO...
-00006a30: 2981 947d 9428 6aeb 0200 008c 1263 6f6f  )..}.(j......coo
-00006a40: 6b69 6573 5f75 7469 6c69 7469 6573 2e94  kies_utilities..
-00006a50: 6aec 0200 005d 946a fa02 0000 8c12 636f  j....].j......co
-00006a60: 6f6b 6965 735f 7574 696c 6974 6965 732e  okies_utilities.
-00006a70: 9485 9481 947d 9428 6aff 0200 006a 2408  .....}.(j....j$.
-00006a80: 0000 6a00 0300 006a e902 0000 6a01 0300  ..j....j....j...
-00006a90: 004e 6a02 0300 004e 7562 616a 0303 0000  .Nj....Nubaj....
-00006aa0: 7d94 286a 0503 0000 5d94 6a07 0300 005d  }.(j....].j....]
-00006ab0: 9428 6a5b 0300 006a 5c03 0000 656a 0903  .(j[...j\...ej..
-00006ac0: 0000 5d94 6a0b 0300 005d 946a 0d03 0000  ..].j....].j....
-00006ad0: 5d94 6a60 0300 006a 6103 0000 756a 0f03  ].j`...ja...uj..
-00006ae0: 0000 6a4e 0300 006a ff02 0000 6afe 0700  ..jN...j....j...
-00006af0: 006a 0003 0000 6ae9 0200 006a 0103 0000  .j....j....j....
-00006b00: 6a23 0800 006a 0203 0000 4b01 7562 6a64  j#...j....K.ubjd
-00006b10: 0300 0029 8194 7d94 286a eb02 0000 8c09  ...)..}.(j......
-00006b20: 5374 6f70 7761 7463 6894 6aec 0200 005d  Stopwatch.j....]
-00006b30: 946a fa02 0000 8c09 5374 6f70 7761 7463  .j......Stopwatc
-00006b40: 6894 8594 8194 7d94 286a ff02 0000 6a32  h.....}.(j....j2
-00006b50: 0800 006a 0003 0000 6ae9 0200 006a 0103  ...j....j....j..
-00006b60: 0000 4e6a 0203 0000 4e75 6261 6a03 0300  ..Nj....Nubaj...
-00006b70: 007d 9428 6a05 0300 005d 946a 0703 0000  .}.(j....].j....
-00006b80: 5d94 286a 7003 0000 6a71 0300 0065 6a09  ].(jp...jq...ej.
-00006b90: 0300 005d 946a 0b03 0000 5d94 6a0d 0300  ...].j....].j...
-00006ba0: 005d 946a 6003 0000 6a61 0300 0075 6a0f  .].j`...ja...uj.
-00006bb0: 0300 006a 6303 0000 6aff 0200 006a fe07  ...jc...j....j..
-00006bc0: 0000 6a00 0300 006a e902 0000 6a01 0300  ..j....j....j...
-00006bd0: 006a 2308 0000 6a02 0300 004b 0175 6265  .j#...j....K.ube
-00006be0: 6a03 0300 007d 9428 6a05 0300 005d 946a  j....}.(j....].j
-00006bf0: f907 0000 616a 0703 0000 5d94 286a cc04  ....aj....].(j..
-00006c00: 0000 6acd 0400 0065 6a09 0300 005d 946a  ..j....ej....].j
-00006c10: 0b03 0000 5d94 6a0d 0300 005d 946a d104  ....].j....].j..
-00006c20: 0000 8c11 636f 6f6b 6965 735f 7574 696c  ....cookies_util
-00006c30: 6974 6965 7394 6a6a 0200 0068 406a d304  ities.jj...h@j..
-00006c40: 0000 6a34 0800 006a d404 0000 6a46 0800  ..j4...j....jF..
-00006c50: 006a 3408 0000 8694 6ad6 0400 006a 3408  .j4.....j....j4.
-00006c60: 0000 756a 0f03 0000 6a48 0300 006a 0103  ..uj....jH...j..
-00006c70: 0000 6a23 0800 006a 0203 0000 4b01 6aff  ..j#...j....K.j.
-00006c80: 0200 006a fb07 0000 6a00 0300 006a e902  ...j....j....j..
-00006c90: 0000 7562 6ad9 0400 0029 8194 7d94 286a  ..ubj....)..}.(j
-00006ca0: eb02 0000 6840 6aec 0200 005d 9428 6ade  ....h@j....].(j.
-00006cb0: 0400 0029 8194 7d94 286a eb02 0000 8c28  ...)..}.(j.....(
-00006cc0: 5374 6f70 7761 7463 6820 666f 7220 6d65  Stopwatch for me
-00006cd0: 6173 7572 696e 6720 7072 6f63 6573 7369  asuring processi
-00006ce0: 6e67 2074 696d 652e 946a ec02 0000 5d94  ng time..j....].
-00006cf0: 6afa 0200 008c 2853 746f 7077 6174 6368  j.....(Stopwatch
-00006d00: 2066 6f72 206d 6561 7375 7269 6e67 2070   for measuring p
-00006d10: 726f 6365 7373 696e 6720 7469 6d65 2e94  rocessing time..
-00006d20: 8594 8194 7d94 286a ff02 0000 6a4b 0800  ....}.(j....jK..
-00006d30: 006a 0003 0000 6ae9 0200 006a 0103 0000  .j....j....j....
-00006d40: 4e6a 0203 0000 4e75 6261 6a03 0300 007d  Nj....Nubaj....}
-00006d50: 9428 6a05 0300 005d 946a 0703 0000 5d94  .(j....].j....].
-00006d60: 6a09 0300 005d 946a 0b03 0000 5d94 6a0d  j....].j....].j.
-00006d70: 0300 005d 9475 6a0f 0300 006a dd04 0000  ...].uj....j....
-00006d80: 6a01 0300 008c 7c43 3a5c 5573 6572 735c  j.....|C:\Users\
-00006d90: 632d 6d69 685c 7370 6163 655c 636f 6f6b  c-mih\space\cook
-00006da0: 6965 735f 7574 696c 6974 6965 735c 7372  ies_utilities\sr
-00006db0: 635c 636f 6f6b 6965 735f 7574 696c 6974  c\cookies_utilit
-00006dc0: 6965 735c 7374 6f70 7761 7463 682e 7079  ies\stopwatch.py
-00006dd0: 3a64 6f63 7374 7269 6e67 206f 6620 636f  :docstring of co
-00006de0: 6f6b 6965 735f 7574 696c 6974 6965 732e  okies_utilities.
-00006df0: 7374 6f70 7761 7463 682e 5374 6f70 7761  stopwatch.Stopwa
-00006e00: 7463 6894 6a02 0300 004b 016a ff02 0000  tch.j....K.j....
-00006e10: 6a48 0800 006a 0003 0000 6ae9 0200 0075  jH...j....j....u
-00006e20: 626a 3303 0000 2981 947d 9428 6aeb 0200  bj3...)..}.(j...
-00006e30: 0068 406a ec02 0000 5d94 6a03 0300 007d  .h@j....].j....}
-00006e40: 9428 6a05 0300 005d 946a 0703 0000 5d94  .(j....].j....].
-00006e50: 6a09 0300 005d 946a 0b03 0000 5d94 6a0d  j....].j....].j.
-00006e60: 0300 005d 948c 0765 6e74 7269 6573 945d  ...]...entries.]
-00006e70: 9428 6a3f 0300 008c 2c70 7265 7373 2829  .(j?....,press()
-00006e80: 2028 636f 6f6b 6965 735f 7574 696c 6974   (cookies_utilit
-00006e90: 6965 732e 5374 6f70 7761 7463 6820 6d65  ies.Stopwatch me
-00006ea0: 7468 6f64 2994 8c21 636f 6f6b 6965 735f  thod)..!cookies_
-00006eb0: 7574 696c 6974 6965 732e 5374 6f70 7761  utilities.Stopwa
-00006ec0: 7463 682e 7072 6573 7394 6840 4e74 9461  tch.press.h@Nt.a
-00006ed0: 756a 0f03 0000 6859 6aff 0200 006a 4808  uj....hYj....jH.
-00006ee0: 0000 6a00 0300 006a e902 0000 6a01 0300  ..j....j....j...
-00006ef0: 004e 6a02 0300 004e 7562 6a44 0300 0029  .Nj....NubjD...)
-00006f00: 8194 7d94 286a eb02 0000 6840 6aec 0200  ..}.(j....h@j...
-00006f10: 005d 9428 6a49 0300 0029 8194 7d94 286a  .].(jI...)..}.(j
-00006f20: eb02 0000 8c17 5374 6f70 7761 7463 682e  ......Stopwatch.
-00006f30: 7072 6573 7328 6b65 793d 2727 2994 6aec  press(key='').j.
-00006f40: 0200 005d 9428 6a64 0300 0029 8194 7d94  ...].(jd...)..}.
-00006f50: 286a eb02 0000 8c05 7072 6573 7394 6aec  (j......press.j.
-00006f60: 0200 005d 946a fa02 0000 8c05 7072 6573  ...].j......pres
-00006f70: 7394 8594 8194 7d94 286a ff02 0000 6a6f  s.....}.(j....jo
-00006f80: 0800 006a 0003 0000 6ae9 0200 006a 0103  ...j....j....j..
-00006f90: 0000 4e6a 0203 0000 4e75 6261 6a03 0300  ..Nj....Nubaj...
-00006fa0: 007d 9428 6a05 0300 005d 946a 0703 0000  .}.(j....].j....
-00006fb0: 5d94 286a 7003 0000 6a71 0300 0065 6a09  ].(jp...jq...ej.
-00006fc0: 0300 005d 946a 0b03 0000 5d94 6a0d 0300  ...].j....].j...
-00006fd0: 005d 946a 6003 0000 6a61 0300 0075 6a0f  .].j`...ja...uj.
-00006fe0: 0300 006a 6303 0000 6aff 0200 006a 6b08  ...jc...j....jk.
-00006ff0: 0000 6a00 0300 006a e902 0000 6a01 0300  ..j....j....j...
-00007000: 008c 8243 3a5c 5573 6572 735c 632d 6d69  ...C:\Users\c-mi
-00007010: 685c 7370 6163 655c 636f 6f6b 6965 735f  h\space\cookies_
-00007020: 7574 696c 6974 6965 735c 7372 635c 636f  utilities\src\co
-00007030: 6f6b 6965 735f 7574 696c 6974 6965 735c  okies_utilities\
-00007040: 7374 6f70 7761 7463 682e 7079 3a64 6f63  stopwatch.py:doc
-00007050: 7374 7269 6e67 206f 6620 636f 6f6b 6965  string of cookie
-00007060: 735f 7574 696c 6974 6965 732e 7374 6f70  s_utilities.stop
-00007070: 7761 7463 682e 5374 6f70 7761 7463 682e  watch.Stopwatch.
-00007080: 7072 6573 7394 6a02 0300 004b 0175 626a  press.j....K.ubj
-00007090: 7603 0000 2981 947d 9428 6aeb 0200 008c  v...)..}.(j.....
-000070a0: 066b 6579 3d27 2794 6aec 0200 005d 946a  .key=''.j....].j
-000070b0: 7c03 0000 2981 947d 9428 6aeb 0200 008c  |...)..}.(j.....
-000070c0: 066b 6579 3d27 2794 6aec 0200 005d 9428  .key=''.j....].(
-000070d0: 6a82 0300 0029 8194 7d94 286a eb02 0000  j....)..}.(j....
-000070e0: 8c03 6b65 7994 6aec 0200 005d 946a fa02  ..key.j....].j..
-000070f0: 0000 8c03 6b65 7994 8594 8194 7d94 286a  ....key.....}.(j
-00007100: ff02 0000 6a86 0800 006a 0003 0000 6ae9  ....j....j....j.
-00007110: 0200 006a 0103 0000 4e6a 0203 0000 4e75  ...j....Nj....Nu
-00007120: 6261 6a03 0300 007d 9428 6a05 0300 005d  baj....}.(j....]
-00007130: 946a 0703 0000 5d94 6a8e 0300 0061 6a09  .j....].j....aj.
-00007140: 0300 005d 946a 0b03 0000 5d94 6a0d 0300  ...].j....].j...
-00007150: 005d 9475 6a0f 0300 006a 8103 0000 6aff  .].uj....j....j.
-00007160: 0200 006a 8208 0000 7562 6a93 0300 0029  ...j....ubj....)
-00007170: 8194 7d94 286a eb02 0000 8c01 3d94 6aec  ..}.(j......=.j.
-00007180: 0200 005d 946a fa02 0000 8c01 3d94 8594  ...].j......=...
-00007190: 8194 7d94 286a ff02 0000 6a94 0800 006a  ..}.(j....j....j
-000071a0: 0003 0000 6ae9 0200 006a 0103 0000 4e6a  ....j....j....Nj
-000071b0: 0203 0000 4e75 6261 6a03 0300 007d 9428  ....Nubaj....}.(
-000071c0: 6a05 0300 005d 946a 0703 0000 5d94 6a9f  j....].j....].j.
-000071d0: 0300 0061 6a09 0300 005d 946a 0b03 0000  ...aj....].j....
-000071e0: 5d94 6a0d 0300 005d 9475 6a0f 0300 006a  ].j....].uj....j
-000071f0: 9203 0000 6aff 0200 006a 8208 0000 7562  ....j....j....ub
-00007200: 6aa3 0300 0029 8194 7d94 286a eb02 0000  j....)..}.(j....
-00007210: 8c02 2727 946a ec02 0000 5d94 6afa 0200  ..''.j....].j...
-00007220: 008c 0227 2794 8594 8194 7d94 286a ff02  ...''.....}.(j..
-00007230: 0000 6aa2 0800 006a 0003 0000 6ae9 0200  ..j....j....j...
-00007240: 006a 0103 0000 4e6a 0203 0000 4e75 6261  .j....Nj....Nuba
-00007250: 6a03 0300 007d 9428 6a05 0300 005d 946a  j....}.(j....].j
-00007260: 0703 0000 5d94 6aaf 0300 0061 6a09 0300  ....].j....aj...
-00007270: 005d 946a 0b03 0000 5d94 6a0d 0300 005d  .].j....].j....]
-00007280: 948c 1373 7570 706f 7274 5f73 6d61 7274  ...support_smart
-00007290: 7175 6f74 6573 9489 756a 0f03 0000 68fa  quotes..uj....h.
-000072a0: 6aff 0200 006a 8208 0000 7562 656a 0303  j....j....ubej..
-000072b0: 0000 7d94 286a 0503 0000 5d94 6a07 0300  ..}.(j....].j...
-000072c0: 005d 946a 0903 0000 5d94 6a0b 0300 005d  .].j....].j....]
-000072d0: 946a 0d03 0000 5d94 6a60 0300 006a 6103  .j....].j`...ja.
-000072e0: 0000 756a 0f03 0000 6a7b 0300 006a ff02  ..uj....j{...j..
-000072f0: 0000 6a7e 0800 0075 6261 6a03 0300 007d  ..j~...ubaj....}
-00007300: 9428 6a05 0300 005d 946a 0703 0000 5d94  .(j....].j....].
-00007310: 6a09 0300 005d 946a 0b03 0000 5d94 6a0d  j....].j....].j.
-00007320: 0300 005d 946a 6003 0000 6a61 0300 0075  ...].j`...ja...u
-00007330: 6a0f 0300 006a 7503 0000 6aff 0200 006a  j....ju...j....j
-00007340: 6b08 0000 6a00 0300 006a e902 0000 6a01  k...j....j....j.
-00007350: 0300 006a 7d08 0000 6a02 0300 004b 0175  ...j}...j....K.u
-00007360: 6265 6a03 0300 007d 9428 6a05 0300 005d  bej....}.(j....]
-00007370: 946a 6608 0000 616a 0703 0000 5d94 286a  .jf...aj....].(j
-00007380: cc04 0000 6acd 0400 0065 6a09 0300 005d  ....j....ej....]
-00007390: 946a 0b03 0000 5d94 6a0d 0300 005d 946a  .j....].j....].j
-000073a0: d104 0000 8c11 636f 6f6b 6965 735f 7574  ......cookies_ut
-000073b0: 696c 6974 6965 7394 6a6a 0200 006a 3408  ilities.jj...j4.
-000073c0: 0000 6ad3 0400 008c 0f53 746f 7077 6174  ..j......Stopwat
-000073d0: 6368 2e70 7265 7373 946a d404 0000 6ac3  ch.press.j....j.
-000073e0: 0800 008c 0953 746f 7077 6174 6368 948c  .....Stopwatch..
-000073f0: 0570 7265 7373 9487 946a d604 0000 8c11  .press...j......
-00007400: 5374 6f70 7761 7463 682e 7072 6573 7328  Stopwatch.press(
-00007410: 2994 756a 0f03 0000 6a48 0300 006a 0103  ).uj....jH...j..
-00007420: 0000 6a7d 0800 006a 0203 0000 4b01 6aff  ..j}...j....K.j.
-00007430: 0200 006a 6808 0000 6a00 0300 006a e902  ...jh...j....j..
-00007440: 0000 7562 6ad9 0400 0029 8194 7d94 286a  ..ubj....)..}.(j
-00007450: eb02 0000 6840 6aec 0200 005d 9428 6ade  ....h@j....].(j.
-00007460: 0400 0029 8194 7d94 286a eb02 0000 8c14  ...)..}.(j......
-00007470: 5072 6573 7320 7468 6520 7374 6f70 7761  Press the stopwa
-00007480: 7463 682e 946a ec02 0000 5d94 6afa 0200  tch..j....].j...
-00007490: 008c 1450 7265 7373 2074 6865 2073 746f  ...Press the sto
-000074a0: 7077 6174 6368 2e94 8594 8194 7d94 286a  pwatch......}.(j
-000074b0: ff02 0000 6acc 0800 006a 0003 0000 6ae9  ....j....j....j.
-000074c0: 0200 006a 0103 0000 4e6a 0203 0000 4e75  ...j....Nj....Nu
-000074d0: 6261 6a03 0300 007d 9428 6a05 0300 005d  baj....}.(j....]
-000074e0: 946a 0703 0000 5d94 6a09 0300 005d 946a  .j....].j....].j
-000074f0: 0b03 0000 5d94 6a0d 0300 005d 9475 6a0f  ....].j....].uj.
-00007500: 0300 006a dd04 0000 6a01 0300 008c 8243  ...j....j......C
-00007510: 3a5c 5573 6572 735c 632d 6d69 685c 7370  :\Users\c-mih\sp
-00007520: 6163 655c 636f 6f6b 6965 735f 7574 696c  ace\cookies_util
-00007530: 6974 6965 735c 7372 635c 636f 6f6b 6965  ities\src\cookie
-00007540: 735f 7574 696c 6974 6965 735c 7374 6f70  s_utilities\stop
-00007550: 7761 7463 682e 7079 3a64 6f63 7374 7269  watch.py:docstri
-00007560: 6e67 206f 6620 636f 6f6b 6965 735f 7574  ng of cookies_ut
-00007570: 696c 6974 6965 732e 7374 6f70 7761 7463  ilities.stopwatc
-00007580: 682e 5374 6f70 7761 7463 682e 7072 6573  h.Stopwatch.pres
-00007590: 7394 6a02 0300 004b 016a ff02 0000 6ac9  s.j....K.j....j.
-000075a0: 0800 006a 0003 0000 6ae9 0200 0075 626a  ...j....j....ubj
-000075b0: ef04 0000 2981 947d 9428 6aeb 0200 0068  ....)..}.(j....h
-000075c0: 406a ec02 0000 5d94 6af4 0400 0029 8194  @j....].j....)..
-000075d0: 7d94 286a eb02 0000 6840 6aec 0200 005d  }.(j....h@j....]
-000075e0: 9428 6af9 0400 0029 8194 7d94 286a eb02  .(j....)..}.(j..
-000075f0: 0000 8c0a 5061 7261 6d65 7465 7273 946a  ....Parameters.j
-00007600: ec02 0000 5d94 6afa 0200 008c 0a50 6172  ....].j......Par
-00007610: 616d 6574 6572 7394 8594 8194 7d94 286a  ameters.....}.(j
-00007620: ff02 0000 6ae1 0800 006a 0003 0000 6ae9  ....j....j....j.
-00007630: 0200 006a 0103 0000 4e6a 0203 0000 4e75  ...j....Nj....Nu
-00007640: 6261 6a03 0300 007d 9428 6a05 0300 005d  baj....}.(j....]
-00007650: 946a 0703 0000 5d94 6a09 0300 005d 946a  .j....].j....].j
-00007660: 0b03 0000 5d94 6a0d 0300 005d 9475 6a0f  ....].j....].uj.
-00007670: 0300 006a f804 0000 6aff 0200 006a de08  ...j....j....j..
-00007680: 0000 6a01 0300 006a 7d08 0000 6a02 0300  ..j....j}...j...
-00007690: 004b 0075 626a 0905 0000 2981 947d 9428  .K.ubj....)..}.(
-000076a0: 6aeb 0200 0068 406a ec02 0000 5d94 6ade  j....h@j....].j.
-000076b0: 0400 0029 8194 7d94 286a eb02 0000 8c38  ...)..}.(j.....8
-000076c0: 6b65 7920 2873 7472 696e 6729 202d 2d20  key (string) -- 
-000076d0: 5468 6520 6964 656e 6669 6361 746f 7220  The idenficator 
-000076e0: 666f 7220 7468 6520 7469 6d65 2028 6f70  for the time (op
-000076f0: 7469 6f6e 616c 292e 946a ec02 0000 5d94  tional)..j....].
-00007700: 286a 1c05 0000 2981 947d 9428 6aeb 0200  (j....)..}.(j...
-00007710: 008c 036b 6579 946a ec02 0000 5d94 6afa  ...key.j....].j.
-00007720: 0200 008c 036b 6579 9485 9481 947d 9428  .....key.....}.(
-00007730: 6aff 0200 006a f608 0000 6a00 0300 006a  j....j....j....j
-00007740: e902 0000 6a01 0300 004e 6a02 0300 004e  ....j....Nj....N
-00007750: 7562 616a 0303 0000 7d94 286a 0503 0000  ubaj....}.(j....
-00007760: 5d94 6a07 0300 005d 946a 0903 0000 5d94  ].j....].j....].
-00007770: 6a0b 0300 005d 946a 0d03 0000 5d94 756a  j....].j....].uj
-00007780: 0f03 0000 6a1b 0500 006a ff02 0000 6af2  ....j....j....j.
-00007790: 0800 0075 626a fa02 0000 8c02 2028 9485  ...ubj...... (..
-000077a0: 9481 947d 9428 6aff 0200 006a f208 0000  ...}.(j....j....
-000077b0: 6a00 0300 006a e902 0000 6a01 0300 004e  j....j....j....N
-000077c0: 6a02 0300 004e 7562 6a30 0500 0029 8194  j....Nubj0...)..
-000077d0: 7d94 286a eb02 0000 6840 6aec 0200 005d  }.(j....h@j....]
-000077e0: 946a 3505 0000 2981 947d 9428 6aeb 0200  .j5...)..}.(j...
-000077f0: 008c 0673 7472 696e 6794 6aec 0200 005d  ...string.j....]
-00007800: 946a fa02 0000 8c06 7374 7269 6e67 9485  .j......string..
-00007810: 9481 947d 9428 6aff 0200 006a 0b09 0000  ...}.(j....j....
-00007820: 6a00 0300 006a e902 0000 6a01 0300 004e  j....j....j....N
-00007830: 6a02 0300 004e 7562 616a 0303 0000 7d94  j....Nubaj....}.
-00007840: 286a 0503 0000 5d94 6a07 0300 005d 946a  (j....].j....].j
-00007850: 0903 0000 5d94 6a0b 0300 005d 946a 0d03  ....].j....].j..
-00007860: 0000 5d94 756a 0f03 0000 6a34 0500 006a  ..].uj....j4...j
-00007870: ff02 0000 6a08 0900 0075 6261 6a03 0300  ....j....ubaj...
-00007880: 007d 9428 6a05 0300 005d 946a 0703 0000  .}.(j....].j....
-00007890: 5d94 6a09 0300 005d 946a 0b03 0000 5d94  ].j....].j....].
-000078a0: 6a0d 0300 005d 948c 0972 6566 646f 6d61  j....]...refdoma
-000078b0: 696e 948c 0270 7994 8c0b 7265 6665 7870  in...py...refexp
-000078c0: 6c69 6369 7494 898c 0772 6566 7479 7065  licit....reftype
-000078d0: 946a 6a02 0000 8c09 7265 6674 6172 6765  .jj.....reftarge
-000078e0: 7494 6a0d 0900 006a 4f05 0000 886a 5005  t.j....jO....jP.
-000078f0: 0000 6ac3 0800 006a 5105 0000 6a34 0800  ..j....jQ...j4..
-00007900: 0075 6a0f 0300 006a 2f05 0000 6aff 0200  .uj....j/...j...
-00007910: 006a f208 0000 7562 6afa 0200 008c 0129  .j....ubj......)
-00007920: 9485 9481 947d 9428 6aff 0200 006a f208  .....}.(j....j..
-00007930: 0000 6a00 0300 006a e902 0000 6a01 0300  ..j....j....j...
-00007940: 004e 6a02 0300 004e 7562 6afa 0200 008c  .Nj....Nubj.....
-00007950: 0520 e280 9320 9485 9481 947d 9428 6aff  . ... .....}.(j.
-00007960: 0200 006a f208 0000 6a00 0300 006a e902  ...j....j....j..
-00007970: 0000 6a01 0300 004e 6a02 0300 004e 7562  ..j....Nj....Nub
-00007980: 6afa 0200 008c 2854 6865 2069 6465 6e66  j.....(The idenf
-00007990: 6963 6174 6f72 2066 6f72 2074 6865 2074  icator for the t
-000079a0: 696d 6520 286f 7074 696f 6e61 6c29 2e94  ime (optional)..
-000079b0: 8594 8194 7d94 286a ff02 0000 6af2 0800  ....}.(j....j...
-000079c0: 006a 0003 0000 6ae9 0200 006a 0103 0000  .j....j....j....
-000079d0: 4e6a 0203 0000 4e75 6265 6a03 0300 007d  Nj....Nubej....}
-000079e0: 9428 6a05 0300 005d 946a 0703 0000 5d94  .(j....].j....].
-000079f0: 6a09 0300 005d 946a 0b03 0000 5d94 6a0d  j....].j....].j.
-00007a00: 0300 005d 9475 6a0f 0300 006a dd04 0000  ...].uj....j....
-00007a10: 6aff 0200 006a ef08 0000 7562 616a 0303  j....j....ubaj..
-00007a20: 0000 7d94 286a 0503 0000 5d94 6a07 0300  ..}.(j....].j...
-00007a30: 005d 946a 0903 0000 5d94 6a0b 0300 005d  .].j....].j....]
-00007a40: 946a 0d03 0000 5d94 756a 0f03 0000 6a08  .j....].uj....j.
-00007a50: 0500 006a ff02 0000 6ade 0800 0075 6265  ...j....j....ube
-00007a60: 6a03 0300 007d 9428 6a05 0300 005d 946a  j....}.(j....].j
-00007a70: 0703 0000 5d94 6a09 0300 005d 946a 0b03  ....].j....].j..
-00007a80: 0000 5d94 6a0d 0300 005d 9475 6a0f 0300  ..].j....].uj...
-00007a90: 006a f304 0000 6aff 0200 006a db08 0000  .j....j....j....
-00007aa0: 7562 616a 0303 0000 7d94 286a 0503 0000  ubaj....}.(j....
-00007ab0: 5d94 6a07 0300 005d 946a 0903 0000 5d94  ].j....].j....].
-00007ac0: 6a0b 0300 005d 946a 0d03 0000 5d94 756a  j....].j....].uj
-00007ad0: 0f03 0000 6aee 0400 006a ff02 0000 6ac9  ....j....j....j.
-00007ae0: 0800 006a 0003 0000 6ae9 0200 006a 0103  ...j....j....j..
-00007af0: 0000 4e6a 0203 0000 4e75 6265 6a03 0300  ..Nj....Nubej...
-00007b00: 007d 9428 6a05 0300 005d 946a 0703 0000  .}.(j....].j....
-00007b10: 5d94 6a09 0300 005d 946a 0b03 0000 5d94  ].j....].j....].
-00007b20: 6a0d 0300 005d 9475 6a0f 0300 006a d804  j....].uj....j..
-00007b30: 0000 6aff 0200 006a 6808 0000 6a00 0300  ..j....jh...j...
-00007b40: 006a e902 0000 6a01 0300 006a 7d08 0000  .j....j....j}...
-00007b50: 6a02 0300 004b 0175 6265 6a03 0300 007d  j....K.ubej....}
-00007b60: 9428 6a05 0300 005d 946a 0703 0000 5d94  .(j....].j....].
-00007b70: 286a 2009 0000 8c06 6d65 7468 6f64 9465  (j .....method.e
-00007b80: 6a09 0300 005d 946a 0b03 0000 5d94 6a0d  j....].j....].j.
-00007b90: 0300 005d 9468 736a 2009 0000 6a8b 0700  ...].hsj ...j...
-00007ba0: 006a 5109 0000 6a8c 0700 006a 5109 0000  .jQ...j....jQ...
-00007bb0: 6a8d 0700 0089 6a8e 0700 0089 6a8f 0700  j.....j.....j...
-00007bc0: 0089 756a 0f03 0000 6a43 0300 006a 0003  ..uj....jC...j..
-00007bd0: 0000 6ae9 0200 006a ff02 0000 6a48 0800  ..j....j....jH..
-00007be0: 006a 0103 0000 4e6a 0203 0000 4e75 626a  .j....Nj....Nubj
-00007bf0: 3303 0000 2981 947d 9428 6aeb 0200 0068  3...)..}.(j....h
-00007c00: 406a ec02 0000 5d94 6a03 0300 007d 9428  @j....].j....}.(
-00007c10: 6a05 0300 005d 946a 0703 0000 5d94 6a09  j....].j....].j.
-00007c20: 0300 005d 946a 0b03 0000 5d94 6a0d 0300  ...].j....].j...
-00007c30: 005d 948c 0765 6e74 7269 6573 945d 9428  .]...entries.].(
-00007c40: 6a3f 0300 008c 2b73 686f 7728 2920 2863  j?....+show() (c
-00007c50: 6f6f 6b69 6573 5f75 7469 6c69 7469 6573  ookies_utilities
-00007c60: 2e53 746f 7077 6174 6368 206d 6574 686f  .Stopwatch metho
-00007c70: 6429 948c 2063 6f6f 6b69 6573 5f75 7469  d).. cookies_uti
-00007c80: 6c69 7469 6573 2e53 746f 7077 6174 6368  lities.Stopwatch
-00007c90: 2e73 686f 7794 6840 4e74 9461 756a 0f03  .show.h@Nt.auj..
-00007ca0: 0000 6859 6aff 0200 006a 4808 0000 6a00  ..hYj....jH...j.
-00007cb0: 0300 006a e902 0000 6a01 0300 008c 8143  ...j....j......C
-00007cc0: 3a5c 5573 6572 735c 632d 6d69 685c 7370  :\Users\c-mih\sp
-00007cd0: 6163 655c 636f 6f6b 6965 735f 7574 696c  ace\cookies_util
-00007ce0: 6974 6965 735c 7372 635c 636f 6f6b 6965  ities\src\cookie
-00007cf0: 735f 7574 696c 6974 6965 735c 7374 6f70  s_utilities\stop
-00007d00: 7761 7463 682e 7079 3a64 6f63 7374 7269  watch.py:docstri
-00007d10: 6e67 206f 6620 636f 6f6b 6965 735f 7574  ng of cookies_ut
-00007d20: 696c 6974 6965 732e 7374 6f70 7761 7463  ilities.stopwatc
-00007d30: 682e 5374 6f70 7761 7463 682e 7368 6f77  h.Stopwatch.show
-00007d40: 946a 0203 0000 4e75 626a 4403 0000 2981  .j....NubjD...).
-00007d50: 947d 9428 6aeb 0200 0068 406a ec02 0000  .}.(j....h@j....
-00007d60: 5d94 286a 4903 0000 2981 947d 9428 6aeb  ].(jI...)..}.(j.
-00007d70: 0200 008c 1053 746f 7077 6174 6368 2e73  .....Stopwatch.s
-00007d80: 686f 7728 2994 6aec 0200 005d 9428 6a64  how().j....].(jd
-00007d90: 0300 0029 8194 7d94 286a eb02 0000 8c04  ...)..}.(j......
-00007da0: 7368 6f77 946a ec02 0000 5d94 6afa 0200  show.j....].j...
-00007db0: 008c 0473 686f 7794 8594 8194 7d94 286a  ...show.....}.(j
-00007dc0: ff02 0000 6a6b 0900 006a 0003 0000 6ae9  ....jk...j....j.
-00007dd0: 0200 006a 0103 0000 4e6a 0203 0000 4e75  ...j....Nj....Nu
-00007de0: 6261 6a03 0300 007d 9428 6a05 0300 005d  baj....}.(j....]
-00007df0: 946a 0703 0000 5d94 286a 7003 0000 6a71  .j....].(jp...jq
-00007e00: 0300 0065 6a09 0300 005d 946a 0b03 0000  ...ej....].j....
-00007e10: 5d94 6a0d 0300 005d 946a 6003 0000 6a61  ].j....].j`...ja
-00007e20: 0300 0075 6a0f 0300 006a 6303 0000 6aff  ...uj....jc...j.
-00007e30: 0200 006a 6709 0000 6a00 0300 006a e902  ...jg...j....j..
-00007e40: 0000 6a01 0300 008c 8143 3a5c 5573 6572  ..j......C:\User
-00007e50: 735c 632d 6d69 685c 7370 6163 655c 636f  s\c-mih\space\co
-00007e60: 6f6b 6965 735f 7574 696c 6974 6965 735c  okies_utilities\
-00007e70: 7372 635c 636f 6f6b 6965 735f 7574 696c  src\cookies_util
-00007e80: 6974 6965 735c 7374 6f70 7761 7463 682e  ities\stopwatch.
-00007e90: 7079 3a64 6f63 7374 7269 6e67 206f 6620  py:docstring of 
-00007ea0: 636f 6f6b 6965 735f 7574 696c 6974 6965  cookies_utilitie
-00007eb0: 732e 7374 6f70 7761 7463 682e 5374 6f70  s.stopwatch.Stop
-00007ec0: 7761 7463 682e 7368 6f77 946a 0203 0000  watch.show.j....
-00007ed0: 4b01 7562 6a76 0300 0029 8194 7d94 286a  K.ubjv...)..}.(j
-00007ee0: eb02 0000 8c02 2829 946a ec02 0000 5d94  ......().j....].
-00007ef0: 6a03 0300 007d 9428 6a05 0300 005d 946a  j....}.(j....].j
-00007f00: 0703 0000 5d94 6a09 0300 005d 946a 0b03  ....].j....].j..
-00007f10: 0000 5d94 6a0d 0300 005d 946a 6003 0000  ..].j....].j`...
-00007f20: 6a61 0300 0075 6a0f 0300 006a 7503 0000  ja...uj....ju...
-00007f30: 6aff 0200 006a 6709 0000 6a00 0300 006a  j....jg...j....j
-00007f40: e902 0000 6a01 0300 006a 7909 0000 6a02  ....j....jy...j.
-00007f50: 0300 004b 0175 6265 6a03 0300 007d 9428  ...K.ubej....}.(
-00007f60: 6a05 0300 005d 946a 6109 0000 616a 0703  j....].ja...aj..
-00007f70: 0000 5d94 286a cc04 0000 6acd 0400 0065  ..].(j....j....e
-00007f80: 6a09 0300 005d 946a 0b03 0000 5d94 6a0d  j....].j....].j.
-00007f90: 0300 005d 946a d104 0000 8c11 636f 6f6b  ...].j......cook
-00007fa0: 6965 735f 7574 696c 6974 6965 7394 6a6a  ies_utilities.jj
-00007fb0: 0200 006a 3408 0000 6ad3 0400 008c 0e53  ...j4...j......S
-00007fc0: 746f 7077 6174 6368 2e73 686f 7794 6ad4  topwatch.show.j.
-00007fd0: 0400 006a 8a09 0000 8c09 5374 6f70 7761  ...j......Stopwa
-00007fe0: 7463 6894 8c04 7368 6f77 9487 946a d604  tch...show...j..
-00007ff0: 0000 8c10 5374 6f70 7761 7463 682e 7368  ....Stopwatch.sh
-00008000: 6f77 2829 9475 6a0f 0300 006a 4803 0000  ow().uj....jH...
-00008010: 6a01 0300 006a 7909 0000 6a02 0300 004b  j....jy...j....K
-00008020: 016a ff02 0000 6a64 0900 006a 0003 0000  .j....jd...j....
-00008030: 6ae9 0200 0075 626a d904 0000 2981 947d  j....ubj....)..}
-00008040: 9428 6aeb 0200 0068 406a ec02 0000 5d94  .(j....h@j....].
-00008050: 6ade 0400 0029 8194 7d94 286a eb02 0000  j....)..}.(j....
-00008060: 8c0f 5368 6f77 206c 6170 2074 696d 6573  ..Show lap times
-00008070: 2e94 6aec 0200 005d 946a fa02 0000 8c0f  ..j....].j......
-00008080: 5368 6f77 206c 6170 2074 696d 6573 2e94  Show lap times..
-00008090: 8594 8194 7d94 286a ff02 0000 6a93 0900  ....}.(j....j...
-000080a0: 006a 0003 0000 6ae9 0200 006a 0103 0000  .j....j....j....
-000080b0: 4e6a 0203 0000 4e75 6261 6a03 0300 007d  Nj....Nubaj....}
-000080c0: 9428 6a05 0300 005d 946a 0703 0000 5d94  .(j....].j....].
-000080d0: 6a09 0300 005d 946a 0b03 0000 5d94 6a0d  j....].j....].j.
-000080e0: 0300 005d 9475 6a0f 0300 006a dd04 0000  ...].uj....j....
-000080f0: 6a01 0300 006a 6309 0000 6a02 0300 004b  j....jc...j....K
-00008100: 016a ff02 0000 6a90 0900 006a 0003 0000  .j....j....j....
-00008110: 6ae9 0200 0075 6261 6a03 0300 007d 9428  j....ubaj....}.(
-00008120: 6a05 0300 005d 946a 0703 0000 5d94 6a09  j....].j....].j.
-00008130: 0300 005d 946a 0b03 0000 5d94 6a0d 0300  ...].j....].j...
-00008140: 005d 9475 6a0f 0300 006a d804 0000 6aff  .].uj....j....j.
-00008150: 0200 006a 6409 0000 6a00 0300 006a e902  ...jd...j....j..
-00008160: 0000 6a01 0300 006a 7909 0000 6a02 0300  ..j....jy...j...
-00008170: 004b 0175 6265 6a03 0300 007d 9428 6a05  .K.ubej....}.(j.
-00008180: 0300 005d 946a 0703 0000 5d94 288c 0270  ...].j....].(..p
-00008190: 7994 8c06 6d65 7468 6f64 9465 6a09 0300  y...method.ej...
-000081a0: 005d 946a 0b03 0000 5d94 6a0d 0300 005d  .].j....].j....]
-000081b0: 9468 736a aa09 0000 6a8b 0700 006a ab09  .hsj....j....j..
-000081c0: 0000 6a8c 0700 006a ab09 0000 6a8d 0700  ..j....j....j...
-000081d0: 0089 6a8e 0700 0089 6a8f 0700 0089 756a  ..j.....j.....uj
-000081e0: 0f03 0000 6a43 0300 006a 0003 0000 6ae9  ....jC...j....j.
-000081f0: 0200 006a ff02 0000 6a48 0800 006a 0103  ...j....jH...j..
-00008200: 0000 6a63 0900 006a 0203 0000 4e75 6265  ..jc...j....Nube
-00008210: 6a03 0300 007d 9428 6a05 0300 005d 946a  j....}.(j....].j
-00008220: 0703 0000 5d94 6a09 0300 005d 946a 0b03  ....].j....].j..
-00008230: 0000 5d94 6a0d 0300 005d 9475 6a0f 0300  ..].j....].uj...
-00008240: 006a d804 0000 6aff 0200 006a fb07 0000  .j....j....j....
-00008250: 6a00 0300 006a e902 0000 6a01 0300 006a  j....j....j....j
-00008260: 2308 0000 6a02 0300 004b 0175 6265 6a03  #...j....K.ubej.
-00008270: 0300 007d 9428 6a05 0300 005d 946a 0703  ...}.(j....].j..
-00008280: 0000 5d94 288c 0270 7994 8c05 636c 6173  ..].(..py...clas
-00008290: 7394 656a 0903 0000 5d94 6a0b 0300 005d  s.ej....].j....]
-000082a0: 946a 0d03 0000 5d94 6873 6ab8 0900 006a  .j....].hsj....j
-000082b0: 8b07 0000 6ab9 0900 006a 8c07 0000 6ab9  ....j....j....j.
-000082c0: 0900 006a 8d07 0000 896a 8e07 0000 896a  ...j.....j.....j
-000082d0: 8f07 0000 8975 6a0f 0300 006a 4303 0000  .....uj....jC...
-000082e0: 6a00 0300 006a e902 0000 6aff 0200 006a  j....j....j....j
-000082f0: dc07 0000 6a01 0300 004e 6a02 0300 004e  ....j....Nj....N
-00008300: 7562 6aee 0200 008c 0763 6f6d 6d65 6e74  ubj......comment
-00008310: 9493 9429 8194 7d94 286a eb02 0000 8c12  ...)..}.(j......
-00008320: 3a73 686f 772d 696e 6865 7269 7461 6e63  :show-inheritanc
-00008330: 653a 946a ec02 0000 5d94 6afa 0200 008c  e:.j....].j.....
-00008340: 123a 7368 6f77 2d69 6e68 6572 6974 616e  .:show-inheritan
-00008350: 6365 3a94 8594 8194 7d94 6aff 0200 006a  ce:.....}.j....j
-00008360: bf09 0000 7362 616a 0303 0000 7d94 286a  ....sbaj....}.(j
-00008370: 0503 0000 5d94 6a07 0300 005d 946a 0903  ....].j....].j..
-00008380: 0000 5d94 6a0b 0300 005d 946a 0d03 0000  ..].j....].j....
-00008390: 5d94 6a60 0300 006a 6103 0000 756a 0f03  ].j`...ja...uj..
-000083a0: 0000 6abd 0900 006a ff02 0000 6adc 0700  ..j....j....j...
-000083b0: 006a 0003 0000 6ae9 0200 006a 0103 0000  .j....j....j....
-000083c0: 6a10 0300 006a 0203 0000 4b23 7562 6aee  j....j....K#ubj.
-000083d0: 0200 008c 0963 6f6e 7461 696e 6572 9493  .....container..
-000083e0: 9429 8194 7d94 286a eb02 0000 6840 6aec  .)..}.(j....h@j.
-000083f0: 0200 005d 9428 6aee 0200 008c 0763 6170  ...].(j......cap
-00008400: 7469 6f6e 9493 9429 8194 7d94 286a eb02  tion...)..}.(j..
-00008410: 0000 8c07 4578 616d 706c 6594 6aec 0200  ....Example.j...
-00008420: 005d 946a fa02 0000 8c07 4578 616d 706c  .].j......Exampl
-00008430: 6594 8594 8194 7d94 286a ff02 0000 6ad4  e.....}.(j....j.
-00008440: 0900 006a 0003 0000 6ae9 0200 006a 0103  ...j....j....j..
-00008450: 0000 4e6a 0203 0000 4e75 6261 6a03 0300  ..Nj....Nubaj...
-00008460: 007d 9428 6a05 0300 005d 946a 0703 0000  .}.(j....].j....
-00008470: 5d94 6a09 0300 005d 946a 0b03 0000 5d94  ].j....].j....].
-00008480: 6a0d 0300 005d 9475 6a0f 0300 006a d209  j....].uj....j..
-00008490: 0000 6a01 0300 006a 1003 0000 6a02 0300  ..j....j....j...
-000084a0: 004b 246a ff02 0000 6acf 0900 0075 626a  .K$j....j....ubj
-000084b0: a807 0000 2981 947d 9428 6aeb 0200 008c  ....)..}.(j.....
-000084c0: 8e69 6d70 6f72 7420 636f 6f6b 6965 735f  .import cookies_
-000084d0: 7574 696c 6974 6965 7320 6173 2063 750a  utilities as cu.
-000084e0: 7377 203d 2063 752e 5374 6f70 7761 7463  sw = cu.Stopwatc
-000084f0: 6828 290a 7377 2e70 7265 7373 2827 7472  h().sw.press('tr
-00008500: 6169 6e20 7374 6172 7427 290a 2320 7472  ain start').# tr
-00008510: 6169 6e0a 7377 2e70 7265 7373 2827 7472  ain.sw.press('tr
-00008520: 6169 6e20 656e 6427 290a 2320 7465 7374  ain end').# test
-00008530: 0a73 772e 7072 6573 7328 2774 6573 7420  .sw.press('test 
-00008540: 656e 6427 290a 7377 2e73 686f 7728 2994  end').sw.show().
-00008550: 6aec 0200 005d 946a fa02 0000 8c8e 696d  j....].j......im
-00008560: 706f 7274 2063 6f6f 6b69 6573 5f75 7469  port cookies_uti
-00008570: 6c69 7469 6573 2061 7320 6375 0a73 7720  lities as cu.sw 
-00008580: 3d20 6375 2e53 746f 7077 6174 6368 2829  = cu.Stopwatch()
-00008590: 0a73 772e 7072 6573 7328 2774 7261 696e  .sw.press('train
-000085a0: 2073 7461 7274 2729 0a23 2074 7261 696e   start').# train
-000085b0: 0a73 772e 7072 6573 7328 2774 7261 696e  .sw.press('train
-000085c0: 2065 6e64 2729 0a23 2074 6573 740a 7377   end').# test.sw
-000085d0: 2e70 7265 7373 2827 7465 7374 2065 6e64  .press('test end
-000085e0: 2729 0a73 772e 7368 6f77 2829 9485 9481  ').sw.show()....
-000085f0: 947d 946a ff02 0000 6ae2 0900 0073 6261  .}.j....j....sba
-00008600: 6a03 0300 007d 9428 6a05 0300 005d 946a  j....}.(j....].j
-00008610: 0703 0000 5d94 6a09 0300 005d 946a 0b03  ....].j....].j..
-00008620: 0000 5d94 6a0d 0300 005d 946a 6003 0000  ..].j....].j`...
-00008630: 6a61 0300 006a b707 0000 8968 4b8c 0670  ja...j.....hK..p
-00008640: 7974 686f 6e94 6ab9 0700 007d 9475 6a0f  ython.j....}.uj.
-00008650: 0300 006a a707 0000 6a01 0300 006a 1003  ...j....j....j..
-00008660: 0000 6a02 0300 004b 246a ff02 0000 6acf  ..j....K$j....j.
-00008670: 0900 0075 6265 6a03 0300 007d 9428 6a05  ...ubej....}.(j.
-00008680: 0300 005d 948c 0369 6431 9461 6a07 0300  ...]...id1.aj...
-00008690: 005d 948c 156c 6974 6572 616c 2d62 6c6f  .]...literal-blo
-000086a0: 636b 2d77 7261 7070 6572 9461 6a09 0300  ck-wrapper.aj...
-000086b0: 005d 946a 0b03 0000 5d94 6a0d 0300 005d  .].j....].j....]
-000086c0: 948c 0d6c 6974 6572 616c 5f62 6c6f 636b  ...literal_block
-000086d0: 9488 756a 0f03 0000 6acd 0900 006a ff02  ..uj....j....j..
-000086e0: 0000 6adc 0700 006a 0003 0000 6ae9 0200  ..j....j....j...
-000086f0: 006a 0103 0000 6840 6a02 0300 004e 7562  .j....h@j....Nub
-00008700: 6aa8 0700 0029 8194 7d94 286a eb02 0000  j....)..}.(j....
-00008710: 8c54 7469 6d65 3128 7472 6169 6e20 7374  .Ttime1(train st
-00008720: 6172 742d 7472 6169 6e20 656e 6429 3a20  art-train end): 
-00008730: 322e 3030 3073 0a74 696d 6532 2874 7261  2.000s.time2(tra
-00008740: 696e 2065 6e64 2d74 6573 7420 656e 6429  in end-test end)
-00008750: 3a20 312e 3030 3073 0a74 6f74 616c 3a20  : 1.000s.total: 
-00008760: 332e 3030 3073 946a ec02 0000 5d94 6afa  3.000s.j....].j.
-00008770: 0200 008c 5474 696d 6531 2874 7261 696e  ....Ttime1(train
-00008780: 2073 7461 7274 2d74 7261 696e 2065 6e64   start-train end
-00008790: 293a 2032 2e30 3030 730a 7469 6d65 3228  ): 2.000s.time2(
-000087a0: 7472 6169 6e20 656e 642d 7465 7374 2065  train end-test e
-000087b0: 6e64 293a 2031 2e30 3030 730a 746f 7461  nd): 1.000s.tota
-000087c0: 6c3a 2033 2e30 3030 7394 8594 8194 7d94  l: 3.000s.....}.
-000087d0: 6aff 0200 006a fb09 0000 7362 616a 0303  j....j....sbaj..
-000087e0: 0000 7d94 286a 0503 0000 5d94 6a07 0300  ..}.(j....].j...
-000087f0: 005d 946a 0903 0000 5d94 6a0b 0300 005d  .].j....].j....]
-00008800: 946a 0d03 0000 5d94 6a60 0300 006a 6103  .j....].j`...ja.
-00008810: 0000 6ab7 0700 0089 684b 8c07 636f 6e73  ..j.....hK..cons
-00008820: 6f6c 6594 6ab9 0700 007d 9475 6a0f 0300  ole.j....}.uj...
-00008830: 006a a707 0000 6a01 0300 006a 1003 0000  .j....j....j....
-00008840: 6a02 0300 004b 306a ff02 0000 6adc 0700  j....K0j....j...
-00008850: 006a 0003 0000 6ae9 0200 0075 6265 6a03  .j....j....ubej.
-00008860: 0300 007d 9428 6a05 0300 005d 948c 1b63  ...}.(j....]...c
-00008870: 6f6f 6b69 6573 2d75 7469 6c69 7469 6573  ookies-utilities
-00008880: 2d73 746f 7077 6174 6368 9461 6a07 0300  -stopwatch.aj...
-00008890: 005d 946a 0903 0000 5d94 8c1b 636f 6f6b  .].j....]...cook
-000088a0: 6965 735f 7574 696c 6974 6965 732e 7374  ies_utilities.st
-000088b0: 6f70 7761 7463 6894 616a 0b03 0000 5d94  opwatch.aj....].
-000088c0: 6a0d 0300 005d 9475 6a0f 0300 0068 306a  j....].uj....h0j
-000088d0: ff02 0000 6acb 0700 006a 0003 0000 6ae9  ....j....j....j.
-000088e0: 0200 006a 0103 0000 6a10 0300 006a 0203  ...j....j....j..
-000088f0: 0000 4b1c 7562 656a 0303 0000 7d94 286a  ..K.ubej....}.(j
-00008900: 0503 0000 5d94 8c07 636c 6173 7365 7394  ....]...classes.
-00008910: 616a 0703 0000 5d94 6a09 0300 005d 948c  aj....].j....]..
-00008920: 0763 6c61 7373 6573 9461 6a0b 0300 005d  .classes.aj....]
-00008930: 946a 0d03 0000 5d94 756a 0f03 0000 6830  .j....].uj....h0
-00008940: 6aff 0200 006a f002 0000 6a00 0300 006a  j....j....j....j
-00008950: e902 0000 6a01 0300 006a 1003 0000 6a02  ....j....j....j.
-00008960: 0300 004b 1975 6265 6a03 0300 007d 9428  ...K.ubej....}.(
-00008970: 6a05 0300 005d 948c 0d64 6f63 756d 656e  j....]...documen
-00008980: 7461 7469 6f6e 9461 6a07 0300 005d 946a  tation.aj....].j
-00008990: 0903 0000 5d94 8c0d 646f 6375 6d65 6e74  ....]...document
-000089a0: 6174 696f 6e94 616a 0b03 0000 5d94 6a0d  ation.aj....].j.
-000089b0: 0300 005d 9475 6a0f 0300 0068 306a ff02  ...].uj....h0j..
-000089c0: 0000 6ae9 0200 006a 0003 0000 6ae9 0200  ..j....j....j...
-000089d0: 006a 0103 0000 6a10 0300 006a 0203 0000  .j....j....j....
-000089e0: 4b02 7562 616a 0303 0000 7d94 286a 0503  K.ubaj....}.(j..
-000089f0: 0000 5d94 6a07 0300 005d 946a 0903 0000  ..].j....].j....
-00008a00: 5d94 6a0b 0300 005d 946a 0d03 0000 5d94  ].j....].j....].
-00008a10: 8c06 736f 7572 6365 946a 1003 0000 756a  ..source.j....uj
-00008a20: 0f03 0000 6ae7 0200 008c 0e63 7572 7265  ....j......curre
-00008a30: 6e74 5f73 6f75 7263 6594 4e8c 0c63 7572  nt_source.N..cur
-00008a40: 7265 6e74 5f6c 696e 6594 4e8c 0873 6574  rent_line.N..set
-00008a50: 7469 6e67 7394 8c11 646f 6375 7469 6c73  tings...docutils
-00008a60: 2e66 726f 6e74 656e 6494 8c06 5661 6c75  .frontend...Valu
-00008a70: 6573 9493 9429 8194 7d94 286a f302 0000  es...)..}.(j....
-00008a80: 4e8c 0967 656e 6572 6174 6f72 944e 8c09  N..generator.N..
-00008a90: 6461 7465 7374 616d 7094 4e8c 0b73 6f75  datestamp.N..sou
-00008aa0: 7263 655f 6c69 6e6b 944e 8c0a 736f 7572  rce_link.N..sour
-00008ab0: 6365 5f75 726c 944e 8c0d 746f 635f 6261  ce_url.N..toc_ba
-00008ac0: 636b 6c69 6e6b 7394 8c05 656e 7472 7994  cklinks...entry.
-00008ad0: 8c12 666f 6f74 6e6f 7465 5f62 6163 6b6c  ..footnote_backl
-00008ae0: 696e 6b73 944b 018c 0d73 6563 746e 756d  inks.K...sectnum
-00008af0: 5f78 666f 726d 944b 018c 0e73 7472 6970  _xform.K...strip
-00008b00: 5f63 6f6d 6d65 6e74 7394 4e8c 1b73 7472  _comments.N..str
-00008b10: 6970 5f65 6c65 6d65 6e74 735f 7769 7468  ip_elements_with
-00008b20: 5f63 6c61 7373 6573 944e 8c0d 7374 7269  _classes.N..stri
-00008b30: 705f 636c 6173 7365 7394 4e8c 0c72 6570  p_classes.N..rep
-00008b40: 6f72 745f 6c65 7665 6c94 4b02 8c0a 6861  ort_level.K...ha
-00008b50: 6c74 5f6c 6576 656c 944b 058c 1165 7869  lt_level.K...exi
-00008b60: 745f 7374 6174 7573 5f6c 6576 656c 944b  t_status_level.K
-00008b70: 058c 0564 6562 7567 944e 8c0e 7761 726e  ...debug.N..warn
-00008b80: 696e 675f 7374 7265 616d 944e 8c09 7472  ing_stream.N..tr
-00008b90: 6163 6562 6163 6b94 888c 0e69 6e70 7574  aceback....input
-00008ba0: 5f65 6e63 6f64 696e 6794 6863 8c1c 696e  _encoding.hc..in
-00008bb0: 7075 745f 656e 636f 6469 6e67 5f65 7272  put_encoding_err
-00008bc0: 6f72 5f68 616e 646c 6572 948c 0673 7472  or_handler...str
-00008bd0: 6963 7494 8c0f 6f75 7470 7574 5f65 6e63  ict...output_enc
-00008be0: 6f64 696e 6794 8c05 7574 662d 3894 8c1d  oding...utf-8...
-00008bf0: 6f75 7470 7574 5f65 6e63 6f64 696e 675f  output_encoding_
-00008c00: 6572 726f 725f 6861 6e64 6c65 7294 6a45  error_handler.jE
-00008c10: 0a00 008c 0e65 7272 6f72 5f65 6e63 6f64  .....error_encod
-00008c20: 696e 6794 8c05 7574 662d 3894 8c1c 6572  ing...utf-8...er
-00008c30: 726f 725f 656e 636f 6469 6e67 5f65 7272  ror_encoding_err
-00008c40: 6f72 5f68 616e 646c 6572 948c 1062 6163  or_handler...bac
-00008c50: 6b73 6c61 7368 7265 706c 6163 6594 8c0d  kslashreplace...
-00008c60: 6c61 6e67 7561 6765 5f63 6f64 6594 684c  language_code.hL
-00008c70: 8c13 7265 636f 7264 5f64 6570 656e 6465  ..record_depende
-00008c80: 6e63 6965 7394 4e8c 0663 6f6e 6669 6794  ncies.N..config.
-00008c90: 4e8c 0969 645f 7072 6566 6978 9468 408c  N..id_prefix.h@.
-00008ca0: 0e61 7574 6f5f 6964 5f70 7265 6669 7894  .auto_id_prefix.
-00008cb0: 6ab1 0200 008c 0d64 756d 705f 7365 7474  j......dump_sett
-00008cc0: 696e 6773 944e 8c0e 6475 6d70 5f69 6e74  ings.N..dump_int
-00008cd0: 6572 6e61 6c73 944e 8c0f 6475 6d70 5f74  ernals.N..dump_t
-00008ce0: 7261 6e73 666f 726d 7394 4e8c 0f64 756d  ransforms.N..dum
-00008cf0: 705f 7073 6575 646f 5f78 6d6c 944e 8c10  p_pseudo_xml.N..
-00008d00: 6578 706f 7365 5f69 6e74 6572 6e61 6c73  expose_internals
-00008d10: 944e 8c0e 7374 7269 6374 5f76 6973 6974  .N..strict_visit
-00008d20: 6f72 944e 8c0f 5f64 6973 6162 6c65 5f63  or.N.._disable_c
-00008d30: 6f6e 6669 6794 4e8c 075f 736f 7572 6365  onfig.N.._source
-00008d40: 946a 1003 0000 8c0c 5f64 6573 7469 6e61  .j......_destina
-00008d50: 7469 6f6e 944e 8c0d 5f63 6f6e 6669 675f  tion.N.._config_
-00008d60: 6669 6c65 7394 5d94 8c16 6669 6c65 5f69  files.]...file_i
-00008d70: 6e73 6572 7469 6f6e 5f65 6e61 626c 6564  nsertion_enabled
-00008d80: 9488 8c0b 7261 775f 656e 6162 6c65 6494  ....raw_enabled.
-00008d90: 4b01 8c11 6c69 6e65 5f6c 656e 6774 685f  K...line_length_
-00008da0: 6c69 6d69 7494 4d10 278c 0e70 6570 5f72  limit.M.'..pep_r
-00008db0: 6566 6572 656e 6365 7394 4e8c 0c70 6570  eferences.N..pep
-00008dc0: 5f62 6173 655f 7572 6c94 6ab7 0200 008c  _base_url.j.....
-00008dd0: 1570 6570 5f66 696c 655f 7572 6c5f 7465  .pep_file_url_te
-00008de0: 6d70 6c61 7465 948c 0870 6570 2d25 3034  mplate...pep-%04
-00008df0: 6494 8c0e 7266 635f 7265 6665 7265 6e63  d...rfc_referenc
-00008e00: 6573 944e 8c0c 7266 635f 6261 7365 5f75  es.N..rfc_base_u
-00008e10: 726c 946a ba02 0000 8c09 7461 625f 7769  rl.j......tab_wi
-00008e20: 6474 6894 4b08 6875 898c 1073 796e 7461  dth.K.hu...synta
-00008e30: 785f 6869 6768 6c69 6768 7494 8c04 6c6f  x_highlight...lo
-00008e40: 6e67 948c 0c73 6d61 7274 5f71 756f 7465  ng...smart_quote
-00008e50: 7394 888c 1373 6d61 7274 7175 6f74 6573  s....smartquotes
-00008e60: 5f6c 6f63 616c 6573 946a c302 0000 8c1d  _locales.j......
-00008e70: 6368 6172 6163 7465 725f 6c65 7665 6c5f  character_level_
-00008e80: 696e 6c69 6e65 5f6d 6172 6b75 7094 898c  inline_markup...
-00008e90: 0e64 6f63 7469 746c 655f 7866 6f72 6d94  .doctitle_xform.
-00008ea0: 898c 0d64 6f63 696e 666f 5f78 666f 726d  ...docinfo_xform
-00008eb0: 944b 018c 1273 6563 7473 7562 7469 746c  .K...sectsubtitl
-00008ec0: 655f 7866 6f72 6d94 898c 0d69 6d61 6765  e_xform....image
-00008ed0: 5f6c 6f61 6469 6e67 946a b302 0000 8c10  _loading.j......
-00008ee0: 656d 6265 645f 7374 796c 6573 6865 6574  embed_stylesheet
-00008ef0: 9489 8c15 636c 6f61 6b5f 656d 6169 6c5f  ....cloak_email_
-00008f00: 6164 6472 6573 7365 7394 888c 1173 6563  addresses....sec
-00008f10: 7469 6f6e 5f73 656c 665f 6c69 6e6b 9489  tion_self_link..
-00008f20: 683c 4e75 628c 0872 6570 6f72 7465 7294  h<Nub..reporter.
-00008f30: 4e8c 1069 6e64 6972 6563 745f 7461 7267  N..indirect_targ
-00008f40: 6574 7394 5d94 8c11 7375 6273 7469 7475  ets.]...substitu
-00008f50: 7469 6f6e 5f64 6566 7394 7d94 8c12 7375  tion_defs.}...su
-00008f60: 6273 7469 7475 7469 6f6e 5f6e 616d 6573  bstitution_names
-00008f70: 947d 948c 0872 6566 6e61 6d65 7394 7d94  .}...refnames.}.
-00008f80: 8c06 7265 6669 6473 947d 948c 076e 616d  ..refids.}...nam
-00008f90: 6569 6473 947d 9428 6a20 0a00 006a 1d0a  eids.}.(j ...j..
-00008fa0: 0000 6ac8 0700 006a c507 0000 6ac0 0700  ..j....j....j...
-00008fb0: 006a bd07 0000 6a18 0a00 006a 150a 0000  .j....j....j....
-00008fc0: 6a10 0a00 006a 0d0a 0000 758c 096e 616d  j....j....u..nam
-00008fd0: 6574 7970 6573 947d 9428 6a20 0a00 0089  etypes.}.(j ....
-00008fe0: 6ac8 0700 0089 6ac0 0700 0089 6a18 0a00  j.....j.....j...
-00008ff0: 0089 6a10 0a00 0089 756a 0503 0000 7d94  ..j.....uj....}.
-00009000: 286a 1d0a 0000 6af0 0200 006a c507 0000  (j....j....j....
-00009010: 6a11 0300 006a bd07 0000 6a22 0300 006a  j....j....j"...j
-00009020: 4103 0000 6a4a 0300 006a 150a 0000 6acb  A...jJ...j....j.
-00009030: 0700 006a 0d0a 0000 6adc 0700 006a f907  ...j....j....j..
-00009040: 0000 6afe 0700 006a 6608 0000 6a6b 0800  ..j....jf...jk..
-00009050: 006a 6109 0000 6a67 0900 006a f409 0000  .ja...jg...j....
-00009060: 6acf 0900 0075 8c0d 666f 6f74 6e6f 7465  j....u..footnote
-00009070: 5f72 6566 7394 7d94 8c0d 6369 7461 7469  _refs.}...citati
-00009080: 6f6e 5f72 6566 7394 7d94 8c0d 6175 746f  on_refs.}...auto
-00009090: 666f 6f74 6e6f 7465 7394 5d94 8c11 6175  footnotes.]...au
-000090a0: 746f 666f 6f74 6e6f 7465 5f72 6566 7394  tofootnote_refs.
-000090b0: 5d94 8c10 7379 6d62 6f6c 5f66 6f6f 746e  ]...symbol_footn
-000090c0: 6f74 6573 945d 948c 1473 796d 626f 6c5f  otes.]...symbol_
-000090d0: 666f 6f74 6e6f 7465 5f72 6566 7394 5d94  footnote_refs.].
-000090e0: 8c09 666f 6f74 6e6f 7465 7394 5d94 8c09  ..footnotes.]...
-000090f0: 6369 7461 7469 6f6e 7394 5d94 8c12 6175  citations.]...au
-00009100: 746f 666f 6f74 6e6f 7465 5f73 7461 7274  tofootnote_start
-00009110: 944b 018c 1573 796d 626f 6c5f 666f 6f74  .K...symbol_foot
-00009120: 6e6f 7465 5f73 7461 7274 944b 008c 0a69  note_start.K...i
-00009130: 645f 636f 756e 7465 7294 6acd 0200 008c  d_counter.j.....
-00009140: 0743 6f75 6e74 6572 9493 947d 946a b102  .Counter...}.j..
-00009150: 0000 4b01 7385 9452 948c 0e70 6172 7365  ..K.s..R...parse
-00009160: 5f6d 6573 7361 6765 7394 5d94 8c12 7472  _messages.]...tr
-00009170: 616e 7366 6f72 6d5f 6d65 7373 6167 6573  ansform_messages
-00009180: 945d 948c 0b74 7261 6e73 666f 726d 6572  .]...transformer
-00009190: 944e 8c0b 696e 636c 7564 655f 6c6f 6794  .N..include_log.
-000091a0: 5d94 8c0a 6465 636f 7261 7469 6f6e 944e  ]...decoration.N
-000091b0: 6a00 0300 006a e902 0000 7562 8c05 696e  j....j....ub..in
-000091c0: 6465 7894 6ae8 0200 0029 8194 7d94 286a  dex.j....)..}.(j
-000091d0: eb02 0000 6840 6aec 0200 005d 946a ef02  ....h@j....].j..
-000091e0: 0000 2981 947d 9428 6aeb 0200 0068 406a  ..)..}.(j....h@j
-000091f0: ec02 0000 5d94 286a f402 0000 2981 947d  ....].(j....)..}
-00009200: 9428 6aeb 0200 008c 2c57 656c 636f 6d65  .(j.....,Welcome
-00009210: 2074 6f20 636f 6f6b 6965 735f 7574 696c   to cookies_util
-00009220: 6974 6965 7327 2064 6f63 756d 656e 7461  ities' documenta
-00009230: 7469 6f6e 2194 6aec 0200 005d 946a fa02  tion!.j....].j..
-00009240: 0000 8c2e 5765 6c63 6f6d 6520 746f 2063  ....Welcome to c
-00009250: 6f6f 6b69 6573 5f75 7469 6c69 7469 6573  ookies_utilities
-00009260: e280 9920 646f 6375 6d65 6e74 6174 696f  ... documentatio
-00009270: 6e21 9485 9481 947d 9428 6aff 0200 006a  n!.....}.(j....j
-00009280: aa0a 0000 6a00 0300 006a a40a 0000 6a01  ....j....j....j.
-00009290: 0300 004e 6a02 0300 004e 7562 616a 0303  ...Nj....Nubaj..
-000092a0: 0000 7d94 288c 0369 6473 945d 948c 0763  ..}.(..ids.]...c
-000092b0: 6c61 7373 6573 945d 948c 056e 616d 6573  lasses.]...names
-000092c0: 945d 948c 0864 7570 6e61 6d65 7394 5d94  .]...dupnames.].
-000092d0: 8c08 6261 636b 7265 6673 945d 9475 6a0f  ..backrefs.].uj.
-000092e0: 0300 008c 0574 6974 6c65 946a ff02 0000  .....title.j....
-000092f0: 6aa7 0a00 006a 0003 0000 6aa4 0a00 006a  j....j....j....j
-00009300: 0103 0000 8c3c 433a 5c55 7365 7273 5c63  .....<C:\Users\c
-00009310: 2d6d 6968 5c73 7061 6365 5c63 6f6f 6b69  -mih\space\cooki
-00009320: 6573 5f75 7469 6c69 7469 6573 5c64 6f63  es_utilities\doc
-00009330: 735c 736f 7572 6365 5c69 6e64 6578 2e72  s\source\index.r
-00009340: 7374 946a 0203 0000 4b02 7562 6aef 0200  st.j....K.ubj...
-00009350: 0029 8194 7d94 286a eb02 0000 6840 6aec  .)..}.(j....h@j.
-00009360: 0200 005d 9428 6af4 0200 0029 8194 7d94  ...].(j....)..}.
-00009370: 286a eb02 0000 8c05 4c69 6e6b 7394 6aec  (j......Links.j.
-00009380: 0200 005d 946a fa02 0000 8c05 4c69 6e6b  ...].j......Link
-00009390: 7394 8594 8194 7d94 286a ff02 0000 6ac2  s.....}.(j....j.
-000093a0: 0a00 006a 0003 0000 6aa4 0a00 006a 0103  ...j....j....j..
-000093b0: 0000 4e6a 0203 0000 4e75 6261 6a03 0300  ..Nj....Nubaj...
-000093c0: 007d 9428 6ab3 0a00 005d 946a b50a 0000  .}.(j....].j....
-000093d0: 5d94 6ab7 0a00 005d 946a b90a 0000 5d94  ].j....].j....].
-000093e0: 6abb 0a00 005d 9475 6a0f 0300 006a bd0a  j....].uj....j..
-000093f0: 0000 6aff 0200 006a bf0a 0000 6a00 0300  ..j....j....j...
-00009400: 006a a40a 0000 6a01 0300 006a be0a 0000  .j....j....j....
-00009410: 6a02 0300 004b 0575 626a 0e05 0000 2981  j....K.ubj....).
-00009420: 947d 9428 6aeb 0200 0068 406a ec02 0000  .}.(j....h@j....
-00009430: 5d94 286a 1305 0000 2981 947d 9428 6aeb  ].(j....)..}.(j.
-00009440: 0200 008c 3e60 5465 7374 5079 5049 203c  ....>`TestPyPI <
-00009450: 6874 7470 733a 2f2f 7465 7374 2e70 7970  https://test.pyp
-00009460: 692e 6f72 672f 7072 6f6a 6563 742f 636f  i.org/project/co
-00009470: 6f6b 6965 732d 7574 696c 6974 6965 732f  okies-utilities/
-00009480: 3e60 5f94 6aec 0200 005d 946a de04 0000  >`_.j....].j....
-00009490: 2981 947d 9428 6aeb 0200 006a d50a 0000  )..}.(j....j....
-000094a0: 6aec 0200 005d 9428 6aee 0200 008c 0972  j....].(j......r
-000094b0: 6566 6572 656e 6365 9493 9429 8194 7d94  eference...)..}.
-000094c0: 286a eb02 0000 6ad5 0a00 006a ec02 0000  (j....j....j....
-000094d0: 5d94 6afa 0200 008c 0854 6573 7450 7950  ].j......TestPyP
-000094e0: 4994 8594 8194 7d94 286a ff02 0000 6adc  I.....}.(j....j.
-000094f0: 0a00 006a 0003 0000 6aa4 0a00 006a 0103  ...j....j....j..
-00009500: 0000 4e6a 0203 0000 4e75 6261 6a03 0300  ..Nj....Nubaj...
-00009510: 007d 9428 6ab3 0a00 005d 946a b50a 0000  .}.(j....].j....
-00009520: 5d94 6ab7 0a00 005d 946a b90a 0000 5d94  ].j....].j....].
-00009530: 6abb 0a00 005d 948c 046e 616d 6594 8c08  j....]...name...
-00009540: 5465 7374 5079 5049 948c 0672 6566 7572  TestPyPI...refur
-00009550: 6994 8c30 6874 7470 733a 2f2f 7465 7374  i..0https://test
-00009560: 2e70 7970 692e 6f72 672f 7072 6f6a 6563  .pypi.org/projec
-00009570: 742f 636f 6f6b 6965 732d 7574 696c 6974  t/cookies-utilit
-00009580: 6965 732f 9475 6a0f 0300 008c 0972 6566  ies/.uj......ref
-00009590: 6572 656e 6365 946a ff02 0000 6ad7 0a00  erence.j....j...
-000095a0: 0075 626a ee02 0000 8c06 7461 7267 6574  .ubj......target
-000095b0: 9493 9429 8194 7d94 286a eb02 0000 8c33  ...)..}.(j.....3
-000095c0: 203c 6874 7470 733a 2f2f 7465 7374 2e70   <https://test.p
-000095d0: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
-000095e0: 636f 6f6b 6965 732d 7574 696c 6974 6965  cookies-utilitie
-000095f0: 732f 3e94 6aec 0200 005d 946a 0303 0000  s/>.j....].j....
-00009600: 7d94 286a b30a 0000 5d94 8c08 7465 7374  }.(j....]...test
-00009610: 7079 7069 9461 6ab5 0a00 005d 946a b70a  pypi.aj....].j..
-00009620: 0000 5d94 8c08 7465 7374 7079 7069 9461  ..]...testpypi.a
-00009630: 6ab9 0a00 005d 946a bb0a 0000 5d94 8c06  j....].j....]...
-00009640: 7265 6675 7269 946a ec0a 0000 756a 0f03  refuri.j....uj..
-00009650: 0000 8c06 7461 7267 6574 948c 0a72 6566  ....target...ref
-00009660: 6572 656e 6365 6494 4b01 6aff 0200 006a  erenced.K.j....j
-00009670: d70a 0000 7562 656a 0303 0000 7d94 286a  ....ubej....}.(j
-00009680: b30a 0000 5d94 6ab5 0a00 005d 946a b70a  ....].j....].j..
-00009690: 0000 5d94 6ab9 0a00 005d 946a bb0a 0000  ..].j....].j....
-000096a0: 5d94 756a 0f03 0000 8c09 7061 7261 6772  ].uj......paragr
-000096b0: 6170 6894 6a01 0300 006a be0a 0000 6a02  aph.j....j....j.
-000096c0: 0300 004b 076a ff02 0000 6ad3 0a00 0075  ...K.j....j....u
-000096d0: 6261 6a03 0300 007d 9428 6ab3 0a00 005d  baj....}.(j....]
-000096e0: 946a b50a 0000 5d94 6ab7 0a00 005d 946a  .j....].j....].j
-000096f0: b90a 0000 5d94 6abb 0a00 005d 9475 6a0f  ....].j....].uj.
-00009700: 0300 008c 096c 6973 745f 6974 656d 946a  .....list_item.j
-00009710: ff02 0000 6ad0 0a00 006a 0003 0000 6aa4  ....j....j....j.
-00009720: 0a00 006a 0103 0000 6abe 0a00 006a 0203  ...j....j....j..
-00009730: 0000 4e75 626a 1305 0000 2981 947d 9428  ..Nubj....)..}.(
-00009740: 6aeb 0200 008c 3d60 4769 7448 7562 203c  j.....=`GitHub <
-00009750: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00009760: 6f6d 2f43 6f6f 6b69 6542 6f78 3236 2f63  om/CookieBox26/c
-00009770: 6f6f 6b69 6573 5f75 7469 6c69 7469 6573  ookies_utilities
-00009780: 3e60 5f0a 946a ec02 0000 5d94 6ade 0400  >`_..j....].j...
-00009790: 0029 8194 7d94 286a eb02 0000 8c3c 6047  .)..}.(j.....<`G
-000097a0: 6974 4875 6220 3c68 7474 7073 3a2f 2f67  itHub <https://g
-000097b0: 6974 6875 622e 636f 6d2f 436f 6f6b 6965  ithub.com/Cookie
-000097c0: 426f 7832 362f 636f 6f6b 6965 735f 7574  Box26/cookies_ut
-000097d0: 696c 6974 6965 733e 605f 946a ec02 0000  ilities>`_.j....
-000097e0: 5d94 286a db0a 0000 2981 947d 9428 6aeb  ].(j....)..}.(j.
-000097f0: 0200 006a 130b 0000 6aec 0200 005d 946a  ...j....j....].j
-00009800: fa02 0000 8c06 4769 7448 7562 9485 9481  ......GitHub....
-00009810: 947d 9428 6aff 0200 006a 150b 0000 6a00  .}.(j....j....j.
-00009820: 0300 006a a40a 0000 6a01 0300 004e 6a02  ...j....j....Nj.
-00009830: 0300 004e 7562 616a 0303 0000 7d94 286a  ...Nubaj....}.(j
-00009840: b30a 0000 5d94 6ab5 0a00 005d 946a b70a  ....].j....].j..
-00009850: 0000 5d94 6ab9 0a00 005d 946a bb0a 0000  ..].j....].j....
-00009860: 5d94 8c04 6e61 6d65 948c 0647 6974 4875  ]...name...GitHu
-00009870: 6294 6aeb 0a00 008c 3068 7474 7073 3a2f  b.j.....0https:/
-00009880: 2f67 6974 6875 622e 636f 6d2f 436f 6f6b  /github.com/Cook
-00009890: 6965 426f 7832 362f 636f 6f6b 6965 735f  ieBox26/cookies_
-000098a0: 7574 696c 6974 6965 7394 756a 0f03 0000  utilities.uj....
-000098b0: 6aed 0a00 006a ff02 0000 6a11 0b00 0075  j....j....j....u
-000098c0: 626a ef0a 0000 2981 947d 9428 6aeb 0200  bj....)..}.(j...
-000098d0: 008c 3320 3c68 7474 7073 3a2f 2f67 6974  ..3 <https://git
-000098e0: 6875 622e 636f 6d2f 436f 6f6b 6965 426f  hub.com/CookieBo
-000098f0: 7832 362f 636f 6f6b 6965 735f 7574 696c  x26/cookies_util
-00009900: 6974 6965 733e 946a ec02 0000 5d94 6a03  ities>.j....].j.
-00009910: 0300 007d 9428 6ab3 0a00 005d 948c 0667  ...}.(j....]...g
-00009920: 6974 6875 6294 616a b50a 0000 5d94 6ab7  ithub.aj....].j.
-00009930: 0a00 005d 948c 0667 6974 6875 6294 616a  ...]...github.aj
-00009940: b90a 0000 5d94 6abb 0a00 005d 948c 0672  ....].j....]...r
-00009950: 6566 7572 6994 6a24 0b00 0075 6a0f 0300  efuri.j$...uj...
-00009960: 006a fd0a 0000 6afe 0a00 004b 016a ff02  .j....j....K.j..
-00009970: 0000 6a11 0b00 0075 6265 6a03 0300 007d  ..j....ubej....}
-00009980: 9428 6ab3 0a00 005d 946a b50a 0000 5d94  .(j....].j....].
-00009990: 6ab7 0a00 005d 946a b90a 0000 5d94 6abb  j....].j....].j.
-000099a0: 0a00 005d 9475 6a0f 0300 006a 050b 0000  ...].uj....j....
-000099b0: 6a01 0300 006a be0a 0000 6a02 0300 004b  j....j....j....K
-000099c0: 086a ff02 0000 6a0d 0b00 0075 6261 6a03  .j....j....ubaj.
-000099d0: 0300 007d 9428 6ab3 0a00 005d 946a b50a  ...}.(j....].j..
-000099e0: 0000 5d94 6ab7 0a00 005d 946a b90a 0000  ..].j....].j....
-000099f0: 5d94 6abb 0a00 005d 9475 6a0f 0300 006a  ].j....].uj....j
-00009a00: 0c0b 0000 6aff 0200 006a d00a 0000 6a00  ....j....j....j.
-00009a10: 0300 006a a40a 0000 6a01 0300 006a be0a  ...j....j....j..
-00009a20: 0000 6a02 0300 004e 7562 656a 0303 0000  ..j....Nubej....
-00009a30: 7d94 286a b30a 0000 5d94 6ab5 0a00 005d  }.(j....].j....]
-00009a40: 946a b70a 0000 5d94 6ab9 0a00 005d 946a  .j....].j....].j
-00009a50: bb0a 0000 5d94 8c06 6275 6c6c 6574 948c  ....]...bullet..
-00009a60: 012d 9475 6a0f 0300 008c 0b62 756c 6c65  .-.uj......bulle
-00009a70: 745f 6c69 7374 946a 0103 0000 6abe 0a00  t_list.j....j...
-00009a80: 006a 0203 0000 4b07 6aff 0200 006a bf0a  .j....K.j....j..
-00009a90: 0000 6a00 0300 006a a40a 0000 7562 6aee  ..j....j....ubj.
-00009aa0: 0200 008c 0863 6f6d 706f 756e 6494 9394  .....compound...
-00009ab0: 2981 947d 9428 6aeb 0200 0068 406a ec02  )..}.(j....h@j..
-00009ac0: 0000 5d94 6ae6 0200 008c 0774 6f63 7472  ..].j......toctr
-00009ad0: 6565 9493 9429 8194 7d94 286a eb02 0000  ee...)..}.(j....
-00009ae0: 6840 6aec 0200 005d 946a 0303 0000 7d94  h@j....].j....}.
-00009af0: 286a b30a 0000 5d94 6ab5 0a00 005d 946a  (j....].j....].j
-00009b00: b70a 0000 5d94 6ab9 0a00 005d 946a bb0a  ....].j....].j..
-00009b10: 0000 5d94 8c06 7061 7265 6e74 946a cb02  ..]...parent.j..
-00009b20: 0000 8c07 656e 7472 6965 7394 5d94 4e8c  ....entries.].N.
-00009b30: 1163 6f6f 6b69 6573 5f75 7469 6c69 7469  .cookies_utiliti
-00009b40: 6573 9486 9461 8c0c 696e 636c 7564 6566  es...a..includef
-00009b50: 696c 6573 945d 946a 5a0b 0000 618c 086d  iles.].jZ...a..m
-00009b60: 6178 6465 7074 6894 4b02 8c07 6361 7074  axdepth.K...capt
-00009b70: 696f 6e94 8c09 436f 6e74 656e 7473 3a94  ion...Contents:.
-00009b80: 8c04 676c 6f62 9489 8c06 6869 6464 656e  ..glob....hidden
-00009b90: 9489 8c0d 696e 636c 7564 6568 6964 6465  ....includehidde
-00009ba0: 6e94 898c 086e 756d 6265 7265 6494 4b00  n....numbered.K.
-00009bb0: 8c0a 7469 746c 6573 6f6e 6c79 9489 8c0a  ..titlesonly....
-00009bc0: 7261 7765 6e74 7269 6573 945d 948c 0a72  rawentries.]...r
-00009bd0: 6177 6361 7074 696f 6e94 6a60 0b00 0075  awcaption.j`...u
-00009be0: 6a0f 0300 008c 0774 6f63 7472 6565 946a  j......toctree.j
-00009bf0: 0103 0000 6abe 0a00 006a 0203 0000 4b0a  ....j....j....K.
-00009c00: 6aff 0200 006a 490b 0000 7562 616a 0303  j....jI...ubaj..
-00009c10: 0000 7d94 286a b30a 0000 5d94 6ab5 0a00  ..}.(j....].j...
-00009c20: 005d 948c 0f74 6f63 7472 6565 2d77 7261  .]...toctree-wra
-00009c30: 7070 6572 9461 6ab7 0a00 005d 946a b90a  pper.aj....].j..
-00009c40: 0000 5d94 6abb 0a00 005d 9475 6a0f 0300  ..].j....].uj...
-00009c50: 008c 0863 6f6d 706f 756e 6494 6aff 0200  ...compound.j...
-00009c60: 006a bf0a 0000 6a00 0300 006a a40a 0000  .j....j....j....
-00009c70: 6a01 0300 006a be0a 0000 6a02 0300 004e  j....j....j....N
-00009c80: 7562 656a 0303 0000 7d94 286a b30a 0000  ubej....}.(j....
-00009c90: 5d94 8c05 6c69 6e6b 7394 616a b50a 0000  ]...links.aj....
-00009ca0: 5d94 6ab7 0a00 005d 948c 056c 696e 6b73  ].j....]...links
-00009cb0: 9461 6ab9 0a00 005d 946a bb0a 0000 5d94  .aj....].j....].
-00009cc0: 756a 0f03 0000 8c07 7365 6374 696f 6e94  uj......section.
-00009cd0: 6aff 0200 006a a70a 0000 6a00 0300 006a  j....j....j....j
-00009ce0: a40a 0000 6a01 0300 006a be0a 0000 6a02  ....j....j....j.
-00009cf0: 0300 004b 0575 626a ef02 0000 2981 947d  ...K.ubj....)..}
-00009d00: 9428 6aeb 0200 0068 406a ec02 0000 5d94  .(j....h@j....].
-00009d10: 286a f402 0000 2981 947d 9428 6aeb 0200  (j....)..}.(j...
-00009d20: 008c 1249 6e64 6963 6573 2061 6e64 2074  ...Indices and t
-00009d30: 6162 6c65 7394 6aec 0200 005d 946a fa02  ables.j....].j..
-00009d40: 0000 8c12 496e 6469 6365 7320 616e 6420  ....Indices and 
-00009d50: 7461 626c 6573 9485 9481 947d 9428 6aff  tables.....}.(j.
-00009d60: 0200 006a 7e0b 0000 6a00 0300 006a a40a  ...j~...j....j..
-00009d70: 0000 6a01 0300 004e 6a02 0300 004e 7562  ..j....Nj....Nub
-00009d80: 616a 0303 0000 7d94 286a b30a 0000 5d94  aj....}.(j....].
-00009d90: 6ab5 0a00 005d 946a b70a 0000 5d94 6ab9  j....].j....].j.
-00009da0: 0a00 005d 946a bb0a 0000 5d94 756a 0f03  ...].j....].uj..
-00009db0: 0000 6abd 0a00 006a ff02 0000 6a7b 0b00  ..j....j....j{..
-00009dc0: 006a 0003 0000 6aa4 0a00 006a 0103 0000  .j....j....j....
-00009dd0: 6abe 0a00 006a 0203 0000 4b11 7562 6a0e  j....j....K.ubj.
-00009de0: 0500 0029 8194 7d94 286a eb02 0000 6840  ...)..}.(j....h@
-00009df0: 6aec 0200 005d 946a 1305 0000 2981 947d  j....].j....)..}
-00009e00: 9428 6aeb 0200 008c 0f3a 7265 663a 6067  .(j......:ref:`g
-00009e10: 656e 696e 6465 7860 946a ec02 0000 5d94  enindex`.j....].
-00009e20: 6ade 0400 0029 8194 7d94 286a eb02 0000  j....)..}.(j....
-00009e30: 6a91 0b00 006a ec02 0000 5d94 6a30 0500  j....j....].j0..
-00009e40: 0029 8194 7d94 286a eb02 0000 6a91 0b00  .)..}.(j....j...
-00009e50: 006a ec02 0000 5d94 6aa3 0300 0029 8194  .j....].j....)..
-00009e60: 7d94 286a eb02 0000 6a91 0b00 006a ec02  }.(j....j....j..
-00009e70: 0000 5d94 6afa 0200 008c 0867 656e 696e  ..].j......genin
-00009e80: 6465 7894 8594 8194 7d94 286a ff02 0000  dex.....}.(j....
-00009e90: 6a99 0b00 006a 0003 0000 6aa4 0a00 006a  j....j....j....j
-00009ea0: 0103 0000 4e6a 0203 0000 4e75 6261 6a03  ....Nj....Nubaj.
-00009eb0: 0300 007d 9428 6ab3 0a00 005d 946a b50a  ...}.(j....].j..
-00009ec0: 0000 5d94 288c 0478 7265 6694 8c03 7374  ..].(..xref...st
-00009ed0: 6494 8c07 7374 642d 7265 6694 656a b70a  d...std-ref.ej..
-00009ee0: 0000 5d94 6ab9 0a00 005d 946a bb0a 0000  ..].j....].j....
-00009ef0: 5d94 756a 0f03 0000 8c06 696e 6c69 6e65  ].uj......inline
-00009f00: 946a ff02 0000 6a96 0b00 0075 6261 6a03  .j....j....ubaj.
-00009f10: 0300 007d 9428 6ab3 0a00 005d 946a b50a  ...}.(j....].j..
-00009f20: 0000 5d94 6ab7 0a00 005d 946a b90a 0000  ..].j....].j....
-00009f30: 5d94 6abb 0a00 005d 948c 0672 6566 646f  ].j....]...refdo
-00009f40: 6394 6acb 0200 008c 0972 6566 646f 6d61  c.j......refdoma
-00009f50: 696e 946a a40b 0000 8c07 7265 6674 7970  in.j......reftyp
-00009f60: 6594 8c03 7265 6694 8c0b 7265 6665 7870  e...ref...refexp
-00009f70: 6c69 6369 7494 898c 0772 6566 7761 726e  licit....refwarn
-00009f80: 9488 8c09 7265 6674 6172 6765 7494 8c08  ....reftarget...
-00009f90: 6765 6e69 6e64 6578 9475 6a0f 0300 008c  genindex.uj.....
-00009fa0: 0c70 656e 6469 6e67 5f78 7265 6694 6a01  .pending_xref.j.
-00009fb0: 0300 006a be0a 0000 6a02 0300 004b 136a  ...j....j....K.j
-00009fc0: ff02 0000 6a93 0b00 0075 6261 6a03 0300  ....j....ubaj...
-00009fd0: 007d 9428 6ab3 0a00 005d 946a b50a 0000  .}.(j....].j....
-00009fe0: 5d94 6ab7 0a00 005d 946a b90a 0000 5d94  ].j....].j....].
-00009ff0: 6abb 0a00 005d 9475 6a0f 0300 006a 050b  j....].uj....j..
-0000a000: 0000 6a01 0300 006a be0a 0000 6a02 0300  ..j....j....j...
-0000a010: 004b 136a ff02 0000 6a8f 0b00 0075 6261  .K.j....j....uba
-0000a020: 6a03 0300 007d 9428 6ab3 0a00 005d 946a  j....}.(j....].j
-0000a030: b50a 0000 5d94 6ab7 0a00 005d 946a b90a  ....].j....].j..
-0000a040: 0000 5d94 6abb 0a00 005d 9475 6a0f 0300  ..].j....].uj...
-0000a050: 006a 0c0b 0000 6aff 0200 006a 8c0b 0000  .j....j....j....
-0000a060: 6a00 0300 006a a40a 0000 6a01 0300 006a  j....j....j....j
-0000a070: be0a 0000 6a02 0300 004e 7562 616a 0303  ....j....Nubaj..
-0000a080: 0000 7d94 286a b30a 0000 5d94 6ab5 0a00  ..}.(j....].j...
-0000a090: 005d 946a b70a 0000 5d94 6ab9 0a00 005d  .].j....].j....]
-0000a0a0: 946a bb0a 0000 5d94 6a44 0b00 008c 012a  .j....].jD.....*
-0000a0b0: 9475 6a0f 0300 006a 460b 0000 6a01 0300  .uj....jF...j...
-0000a0c0: 006a be0a 0000 6a02 0300 004b 136a ff02  .j....j....K.j..
-0000a0d0: 0000 6a7b 0b00 006a 0003 0000 6aa4 0a00  ..j{...j....j...
-0000a0e0: 0075 6265 6a03 0300 007d 9428 6ab3 0a00  .ubej....}.(j...
-0000a0f0: 005d 948c 1269 6e64 6963 6573 2d61 6e64  .]...indices-and
-0000a100: 2d74 6162 6c65 7394 616a b50a 0000 5d94  -tables.aj....].
-0000a110: 6ab7 0a00 005d 948c 1269 6e64 6963 6573  j....]...indices
-0000a120: 2061 6e64 2074 6162 6c65 7394 616a b90a   and tables.aj..
-0000a130: 0000 5d94 6abb 0a00 005d 9475 6a0f 0300  ..].j....].uj...
-0000a140: 006a 7a0b 0000 6aff 0200 006a a70a 0000  .jz...j....j....
-0000a150: 6a00 0300 006a a40a 0000 6a01 0300 006a  j....j....j....j
-0000a160: be0a 0000 6a02 0300 004b 1175 6265 6a03  ....j....K.ubej.
-0000a170: 0300 007d 9428 6ab3 0a00 005d 948c 2a77  ...}.(j....]..*w
-0000a180: 656c 636f 6d65 2d74 6f2d 636f 6f6b 6965  elcome-to-cookie
-0000a190: 732d 7574 696c 6974 6965 732d 646f 6375  s-utilities-docu
-0000a1a0: 6d65 6e74 6174 696f 6e94 616a b50a 0000  mentation.aj....
-0000a1b0: 5d94 6ab7 0a00 005d 948c 2c77 656c 636f  ].j....]..,welco
-0000a1c0: 6d65 2074 6f20 636f 6f6b 6965 735f 7574  me to cookies_ut
-0000a1d0: 696c 6974 6965 7327 2064 6f63 756d 656e  ilities' documen
-0000a1e0: 7461 7469 6f6e 2194 616a b90a 0000 5d94  tation!.aj....].
-0000a1f0: 6abb 0a00 005d 9475 6a0f 0300 006a 7a0b  j....].uj....jz.
-0000a200: 0000 6aff 0200 006a a40a 0000 6a00 0300  ..j....j....j...
-0000a210: 006a a40a 0000 6a01 0300 006a be0a 0000  .j....j....j....
-0000a220: 6a02 0300 004b 0275 6261 6a03 0300 007d  j....K.ubaj....}
-0000a230: 9428 6ab3 0a00 005d 946a b50a 0000 5d94  .(j....].j....].
-0000a240: 6ab7 0a00 005d 946a b90a 0000 5d94 6abb  j....].j....].j.
-0000a250: 0a00 005d 948c 0673 6f75 7263 6594 6abe  ...]...source.j.
-0000a260: 0a00 0075 6a0f 0300 008c 0864 6f63 756d  ...uj......docum
-0000a270: 656e 7494 6a2a 0a00 004e 6a2b 0a00 004e  ent.j*...Nj+...N
-0000a280: 6a2c 0a00 006a 2f0a 0000 2981 947d 9428  j,...j/...)..}.(
-0000a290: 6af3 0200 004e 6a32 0a00 004e 6a33 0a00  j....Nj2...Nj3..
-0000a2a0: 004e 6a34 0a00 004e 6a35 0a00 004e 6a36  .Nj4...Nj5...Nj6
-0000a2b0: 0a00 008c 0565 6e74 7279 946a 380a 0000  .....entry.j8...
-0000a2c0: 4b01 6a39 0a00 004b 016a 3a0a 0000 4e6a  K.j9...K.j:...Nj
-0000a2d0: 3b0a 0000 4e6a 3c0a 0000 4e6a 3d0a 0000  ;...Nj<...Nj=...
-0000a2e0: 4b02 6a3e 0a00 004b 056a 3f0a 0000 4b05  K.j>...K.j?...K.
-0000a2f0: 6a40 0a00 004e 6a41 0a00 004e 6a42 0a00  j@...NjA...NjB..
-0000a300: 0088 6a43 0a00 008c 0975 7466 2d38 2d73  ..jC.....utf-8-s
-0000a310: 6967 946a 440a 0000 8c06 7374 7269 6374  ig.jD.....strict
-0000a320: 946a 460a 0000 8c05 7574 662d 3894 6a48  .jF.....utf-8.jH
-0000a330: 0a00 006a e80b 0000 6a49 0a00 008c 0575  ...j....jI.....u
-0000a340: 7466 2d38 946a 4b0a 0000 8c10 6261 636b  tf-8.jK.....back
-0000a350: 736c 6173 6872 6570 6c61 6365 946a 4d0a  slashreplace.jM.
-0000a360: 0000 8c02 656e 946a 4e0a 0000 4e6a 4f0a  ....en.jN...NjO.
-0000a370: 0000 4e6a 500a 0000 6840 6a51 0a00 006a  ..NjP...h@jQ...j
-0000a380: b102 0000 6a52 0a00 004e 6a53 0a00 004e  ....jR...NjS...N
-0000a390: 6a54 0a00 004e 6a55 0a00 004e 6a56 0a00  jT...NjU...NjV..
-0000a3a0: 004e 6a57 0a00 004e 6a58 0a00 004e 6a59  .NjW...NjX...NjY
-0000a3b0: 0a00 006a be0a 0000 6a5a 0a00 004e 6a5b  ...j....jZ...Nj[
-0000a3c0: 0a00 005d 946a 5d0a 0000 886a 5e0a 0000  ...].j]....j^...
-0000a3d0: 4b01 6a5f 0a00 004d 1027 6a60 0a00 004e  K.j_...M.'j`...N
-0000a3e0: 6a61 0a00 006a b702 0000 6a62 0a00 008c  ja...j....jb....
-0000a3f0: 0870 6570 2d25 3034 6494 6a64 0a00 004e  .pep-%04d.jd...N
-0000a400: 6a65 0a00 006a ba02 0000 6a66 0a00 004b  je...j....jf...K
-0000a410: 0868 7589 6a67 0a00 008c 046c 6f6e 6794  .hu.jg.....long.
-0000a420: 6a69 0a00 0088 6a6a 0a00 006a c302 0000  ji....jj...j....
-0000a430: 6a6b 0a00 0089 6a6c 0a00 0089 6a6d 0a00  jk....jl....jm..
-0000a440: 004b 016a 6e0a 0000 896a 6f0a 0000 6ab3  .K.jn....jo...j.
-0000a450: 0200 006a 700a 0000 896a 710a 0000 886a  ...jp....jq....j
-0000a460: 720a 0000 8968 3c4e 7562 6a73 0a00 004e  r....h<Nubjs...N
-0000a470: 6a74 0a00 005d 946a 760a 0000 7d94 6a78  jt...].jv...}.jx
-0000a480: 0a00 007d 946a 7a0a 0000 7d94 6a7c 0a00  ...}.jz...}.j|..
-0000a490: 007d 946a 7e0a 0000 7d94 286a d90b 0000  .}.j~...}.(j....
-0000a4a0: 6ad6 0b00 006a 770b 0000 6a74 0b00 006a  j....jw...jt...j
-0000a4b0: f90a 0000 6af6 0a00 006a 2e0b 0000 6a2b  ....j....j....j+
-0000a4c0: 0b00 006a d10b 0000 6ace 0b00 0075 6a80  ...j....j....uj.
-0000a4d0: 0a00 007d 9428 6ad9 0b00 0089 6a77 0b00  ...}.(j.....jw..
-0000a4e0: 0089 6af9 0a00 0088 6a2e 0b00 0088 6ad1  ..j.....j.....j.
-0000a4f0: 0b00 0089 756a 0503 0000 7d94 286a d60b  ....uj....}.(j..
-0000a500: 0000 6aa7 0a00 006a 740b 0000 6abf 0a00  ..j....jt...j...
-0000a510: 006a f60a 0000 6af0 0a00 006a 2b0b 0000  .j....j....j+...
-0000a520: 6a25 0b00 006a ce0b 0000 6a7b 0b00 0075  j%...j....j{...u
-0000a530: 6a83 0a00 007d 946a 850a 0000 7d94 6a87  j....}.j....}.j.
-0000a540: 0a00 005d 946a 890a 0000 5d94 6a8b 0a00  ...].j....].j...
-0000a550: 005d 946a 8d0a 0000 5d94 6a8f 0a00 005d  .].j....].j....]
-0000a560: 946a 910a 0000 5d94 6a93 0a00 004b 016a  .j....].j....K.j
-0000a570: 940a 0000 4b00 6a95 0a00 006a 970a 0000  ....K.j....j....
-0000a580: 7d94 8594 5294 6a9b 0a00 005d 946a 9d0a  }...R.j....].j..
-0000a590: 0000 5d94 6a9f 0a00 004e 6aa0 0a00 005d  ..].j....Nj....]
-0000a5a0: 946a a20a 0000 4e6a 0003 0000 6aa4 0a00  .j....Nj....j...
-0000a5b0: 0075 628c 076d 6f64 756c 6573 946a e802  .ub..modules.j..
-0000a5c0: 0000 2981 947d 9428 6aeb 0200 0068 406a  ..)..}.(j....h@j
-0000a5d0: ec02 0000 5d94 6aef 0200 0029 8194 7d94  ....].j....)..}.
-0000a5e0: 286a eb02 0000 6840 6aec 0200 005d 9428  (j....h@j....].(
-0000a5f0: 6af4 0200 0029 8194 7d94 286a eb02 0000  j....)..}.(j....
-0000a600: 8c11 636f 6f6b 6965 735f 7574 696c 6974  ..cookies_utilit
-0000a610: 6965 7394 6aec 0200 005d 946a fa02 0000  ies.j....].j....
-0000a620: 8c11 636f 6f6b 6965 735f 7574 696c 6974  ..cookies_utilit
-0000a630: 6965 7394 8594 8194 7d94 286a ff02 0000  ies.....}.(j....
-0000a640: 6a0d 0c00 006a 0003 0000 6a07 0c00 006a  j....j....j....j
-0000a650: 0103 0000 4e6a 0203 0000 4e75 6261 6a03  ....Nj....Nubaj.
-0000a660: 0300 007d 9428 8c03 6964 7394 5d94 8c07  ...}.(..ids.]...
-0000a670: 636c 6173 7365 7394 5d94 8c05 6e61 6d65  classes.]...name
-0000a680: 7394 5d94 8c08 6475 706e 616d 6573 945d  s.]...dupnames.]
-0000a690: 948c 0862 6163 6b72 6566 7394 5d94 756a  ...backrefs.].uj
-0000a6a0: 0f03 0000 8c05 7469 746c 6594 6aff 0200  ......title.j...
-0000a6b0: 006a 0a0c 0000 6a00 0300 006a 070c 0000  .j....j....j....
-0000a6c0: 6a01 0300 008c 3e43 3a5c 5573 6572 735c  j.....>C:\Users\
-0000a6d0: 632d 6d69 685c 7370 6163 655c 636f 6f6b  c-mih\space\cook
-0000a6e0: 6965 735f 7574 696c 6974 6965 735c 646f  ies_utilities\do
-0000a6f0: 6373 5c73 6f75 7263 655c 6d6f 6475 6c65  cs\source\module
-0000a700: 732e 7273 7494 6a02 0300 004b 0275 626a  s.rst.j....K.ubj
-0000a710: 480b 0000 2981 947d 9428 6aeb 0200 0068  H...)..}.(j....h
-0000a720: 406a ec02 0000 5d94 6a4d 0b00 0029 8194  @j....].jM...)..
-0000a730: 7d94 286a eb02 0000 6840 6aec 0200 005d  }.(j....h@j....]
-0000a740: 946a 0303 0000 7d94 286a 160c 0000 5d94  .j....}.(j....].
-0000a750: 6a18 0c00 005d 946a 1a0c 0000 5d94 6a1c  j....].j....].j.
-0000a760: 0c00 005d 946a 1e0c 0000 5d94 8c06 7061  ...].j....]...pa
-0000a770: 7265 6e74 946a ca02 0000 8c07 656e 7472  rent.j......entr
-0000a780: 6965 7394 5d94 4e8c 1163 6f6f 6b69 6573  ies.].N..cookies
-0000a790: 5f75 7469 6c69 7469 6573 9486 9461 8c0c  _utilities...a..
-0000a7a0: 696e 636c 7564 6566 696c 6573 945d 946a  includefiles.].j
-0000a7b0: 310c 0000 618c 086d 6178 6465 7074 6894  1...a..maxdepth.
-0000a7c0: 4b04 8c07 6361 7074 696f 6e94 4e8c 0467  K...caption.N..g
-0000a7d0: 6c6f 6294 898c 0668 6964 6465 6e94 898c  lob....hidden...
-0000a7e0: 0d69 6e63 6c75 6465 6869 6464 656e 9489  .includehidden..
-0000a7f0: 8c08 6e75 6d62 6572 6564 944b 008c 0a74  ..numbered.K...t
-0000a800: 6974 6c65 736f 6e6c 7994 898c 0a72 6177  itlesonly....raw
-0000a810: 656e 7472 6965 7394 5d94 756a 0f03 0000  entries.].uj....
-0000a820: 8c07 746f 6374 7265 6594 6a01 0300 006a  ..toctree.j....j
-0000a830: 210c 0000 6a02 0300 004b 046a ff02 0000  !...j....K.j....
-0000a840: 6a22 0c00 0075 6261 6a03 0300 007d 9428  j"...ubaj....}.(
-0000a850: 6a16 0c00 005d 946a 180c 0000 5d94 8c0f  j....].j....]...
-0000a860: 746f 6374 7265 652d 7772 6170 7065 7294  toctree-wrapper.
-0000a870: 616a 1a0c 0000 5d94 6a1c 0c00 005d 946a  aj....].j....].j
-0000a880: 1e0c 0000 5d94 756a 0f03 0000 8c08 636f  ....].uj......co
-0000a890: 6d70 6f75 6e64 946a ff02 0000 6a0a 0c00  mpound.j....j...
-0000a8a0: 006a 0003 0000 6a07 0c00 006a 0103 0000  .j....j....j....
-0000a8b0: 6a21 0c00 006a 0203 0000 4e75 6265 6a03  j!...j....Nubej.
-0000a8c0: 0300 007d 9428 6a16 0c00 005d 948c 1163  ...}.(j....]...c
-0000a8d0: 6f6f 6b69 6573 2d75 7469 6c69 7469 6573  ookies-utilities
-0000a8e0: 9461 6a18 0c00 005d 946a 1a0c 0000 5d94  .aj....].j....].
-0000a8f0: 8c11 636f 6f6b 6965 735f 7574 696c 6974  ..cookies_utilit
-0000a900: 6965 7394 616a 1c0c 0000 5d94 6a1e 0c00  ies.aj....].j...
-0000a910: 005d 9475 6a0f 0300 008c 0773 6563 7469  .].uj......secti
-0000a920: 6f6e 946a ff02 0000 6a07 0c00 006a 0003  on.j....j....j..
-0000a930: 0000 6a07 0c00 006a 0103 0000 6a21 0c00  ..j....j....j!..
-0000a940: 006a 0203 0000 4b02 7562 616a 0303 0000  .j....K.ubaj....
-0000a950: 7d94 286a 160c 0000 5d94 6a18 0c00 005d  }.(j....].j....]
-0000a960: 946a 1a0c 0000 5d94 6a1c 0c00 005d 946a  .j....].j....].j
-0000a970: 1e0c 0000 5d94 8c06 736f 7572 6365 946a  ....]...source.j
-0000a980: 210c 0000 756a 0f03 0000 8c08 646f 6375  !...uj......docu
-0000a990: 6d65 6e74 946a 2a0a 0000 4e6a 2b0a 0000  ment.j*...Nj+...
-0000a9a0: 4e6a 2c0a 0000 6a2f 0a00 0029 8194 7d94  Nj,...j/...)..}.
-0000a9b0: 286a f302 0000 4e6a 320a 0000 4e6a 330a  (j....Nj2...Nj3.
-0000a9c0: 0000 4e6a 340a 0000 4e6a 350a 0000 4e6a  ..Nj4...Nj5...Nj
-0000a9d0: 360a 0000 8c05 656e 7472 7994 6a38 0a00  6.....entry.j8..
-0000a9e0: 004b 016a 390a 0000 4b01 6a3a 0a00 004e  .K.j9...K.j:...N
-0000a9f0: 6a3b 0a00 004e 6a3c 0a00 004e 6a3d 0a00  j;...Nj<...Nj=..
-0000aa00: 004b 026a 3e0a 0000 4b05 6a3f 0a00 004b  .K.j>...K.j?...K
-0000aa10: 056a 400a 0000 4e6a 410a 0000 4e6a 420a  .j@...NjA...NjB.
-0000aa20: 0000 886a 430a 0000 8c09 7574 662d 382d  ...jC.....utf-8-
-0000aa30: 7369 6794 6a44 0a00 008c 0673 7472 6963  sig.jD.....stric
-0000aa40: 7494 6a46 0a00 008c 0575 7466 2d38 946a  t.jF.....utf-8.j
-0000aa50: 480a 0000 6a5c 0c00 006a 490a 0000 8c05  H...j\...jI.....
-0000aa60: 7574 662d 3894 6a4b 0a00 008c 1062 6163  utf-8.jK.....bac
-0000aa70: 6b73 6c61 7368 7265 706c 6163 6594 6a4d  kslashreplace.jM
-0000aa80: 0a00 008c 0265 6e94 6a4e 0a00 004e 6a4f  .....en.jN...NjO
-0000aa90: 0a00 004e 6a50 0a00 0068 406a 510a 0000  ...NjP...h@jQ...
-0000aaa0: 6ab1 0200 006a 520a 0000 4e6a 530a 0000  j....jR...NjS...
-0000aab0: 4e6a 540a 0000 4e6a 550a 0000 4e6a 560a  NjT...NjU...NjV.
-0000aac0: 0000 4e6a 570a 0000 4e6a 580a 0000 4e6a  ..NjW...NjX...Nj
-0000aad0: 590a 0000 6a21 0c00 006a 5a0a 0000 4e6a  Y...j!...jZ...Nj
-0000aae0: 5b0a 0000 5d94 6a5d 0a00 0088 6a5e 0a00  [...].j]....j^..
-0000aaf0: 004b 016a 5f0a 0000 4d10 276a 600a 0000  .K.j_...M.'j`...
-0000ab00: 4e6a 610a 0000 6ab7 0200 006a 620a 0000  Nja...j....jb...
-0000ab10: 8c08 7065 702d 2530 3464 946a 640a 0000  ..pep-%04d.jd...
-0000ab20: 4e6a 650a 0000 6aba 0200 006a 660a 0000  Nje...j....jf...
-0000ab30: 4b08 6875 896a 670a 0000 8c04 6c6f 6e67  K.hu.jg.....long
-0000ab40: 946a 690a 0000 886a 6a0a 0000 6ac3 0200  .ji....jj...j...
-0000ab50: 006a 6b0a 0000 896a 6c0a 0000 896a 6d0a  .jk....jl....jm.
-0000ab60: 0000 4b01 6a6e 0a00 0089 6a6f 0a00 006a  ..K.jn....jo...j
-0000ab70: b302 0000 6a70 0a00 0089 6a71 0a00 0088  ....jp....jq....
-0000ab80: 6a72 0a00 0089 683c 4e75 626a 730a 0000  jr....h<Nubjs...
-0000ab90: 4e6a 740a 0000 5d94 6a76 0a00 007d 946a  Njt...].jv...}.j
-0000aba0: 780a 0000 7d94 6a7a 0a00 007d 946a 7c0a  x...}.jz...}.j|.
-0000abb0: 0000 7d94 6a7e 0a00 007d 946a 4c0c 0000  ..}.j~...}.jL...
-0000abc0: 6a49 0c00 0073 6a80 0a00 007d 946a 4c0c  jI...sj....}.jL.
-0000abd0: 0000 8973 6a05 0300 007d 946a 490c 0000  ...sj....}.jI...
-0000abe0: 6a0a 0c00 0073 6a83 0a00 007d 946a 850a  j....sj....}.j..
-0000abf0: 0000 7d94 6a87 0a00 005d 946a 890a 0000  ..}.j....].j....
-0000ac00: 5d94 6a8b 0a00 005d 946a 8d0a 0000 5d94  ].j....].j....].
-0000ac10: 6a8f 0a00 005d 946a 910a 0000 5d94 6a93  j....].j....].j.
-0000ac20: 0a00 004b 016a 940a 0000 4b00 6a95 0a00  ...K.j....K.j...
-0000ac30: 006a 970a 0000 7d94 8594 5294 6a9b 0a00  .j....}...R.j...
-0000ac40: 005d 946a 9d0a 0000 5d94 6a9f 0a00 004e  .].j....].j....N
-0000ac50: 6aa0 0a00 005d 946a a20a 0000 4e6a 0003  j....].j....Nj..
-0000ac60: 0000 6a07 0c00 0075 6275 8c08 6d65 7461  ..j....ubu..meta
-0000ac70: 6461 7461 946a cf02 0000 6ad0 0200 008c  data.j....j.....
-0000ac80: 0464 6963 7494 9394 8594 5294 8c06 7469  .dict.....R...ti
-0000ac90: 746c 6573 947d 9428 6aca 0200 006a f402  tles.}.(j....j..
-0000aca0: 0000 2981 947d 9428 6aeb 0200 0068 406a  ..)..}.(j....h@j
-0000acb0: ec02 0000 5d94 6afa 0200 008c 1163 6f6f  ....].j......coo
-0000acc0: 6b69 6573 5f75 7469 6c69 7469 6573 9485  kies_utilities..
-0000acd0: 9481 947d 946a ff02 0000 6a81 0c00 0073  ...}.j....j....s
-0000ace0: 6261 6a03 0300 007d 9428 6a16 0c00 005d  baj....}.(j....]
-0000acf0: 946a 180c 0000 5d94 6a1a 0c00 005d 946a  .j....].j....].j
-0000ad00: 1c0c 0000 5d94 6a1e 0c00 005d 9475 6a0f  ....].j....].uj.
-0000ad10: 0300 006a 200c 0000 7562 6acb 0200 006a  ...j ...ubj....j
-0000ad20: f402 0000 2981 947d 9428 6aeb 0200 0068  ....)..}.(j....h
-0000ad30: 406a ec02 0000 5d94 6afa 0200 008c 2e57  @j....].j......W
-0000ad40: 656c 636f 6d65 2074 6f20 636f 6f6b 6965  elcome to cookie
-0000ad50: 735f 7574 696c 6974 6965 73e2 8099 2064  s_utilities... d
-0000ad60: 6f63 756d 656e 7461 7469 6f6e 2194 8594  ocumentation!...
-0000ad70: 8194 7d94 6aff 0200 006a 8e0c 0000 7362  ..}.j....j....sb
-0000ad80: 616a 0303 0000 7d94 286a b30a 0000 5d94  aj....}.(j....].
-0000ad90: 6ab5 0a00 005d 946a b70a 0000 5d94 6ab9  j....].j....].j.
-0000ada0: 0a00 005d 946a bb0a 0000 5d94 756a 0f03  ...].j....].uj..
-0000adb0: 0000 6abd 0a00 0075 626a 9a02 0000 6af4  ..j....ubj....j.
-0000adc0: 0200 0029 8194 7d94 286a eb02 0000 6840  ...)..}.(j....h@
-0000add0: 6aec 0200 005d 946a fa02 0000 8c0d 446f  j....].j......Do
-0000ade0: 6375 6d65 6e74 6174 696f 6e94 8594 8194  cumentation.....
-0000adf0: 7d94 6aff 0200 006a 9b0c 0000 7362 616a  }.j....j....sbaj
-0000ae00: 0303 0000 7d94 286a 0503 0000 5d94 6a07  ....}.(j....].j.
-0000ae10: 0300 005d 946a 0903 0000 5d94 6a0b 0300  ...].j....].j...
-0000ae20: 005d 946a 0d03 0000 5d94 756a 0f03 0000  .].j....].uj....
-0000ae30: 6af3 0200 0075 6275 8c0a 6c6f 6e67 7469  j....ubu..longti
-0000ae40: 746c 6573 947d 9428 6aca 0200 006a 810c  tles.}.(j....j..
-0000ae50: 0000 6acb 0200 006a 8e0c 0000 6a9a 0200  ..j....j....j...
-0000ae60: 006a 9b0c 0000 758c 0474 6f63 7394 7d94  .j....u..tocs.}.
-0000ae70: 286a ca02 0000 6a0e 0500 0029 8194 7d94  (j....j....)..}.
-0000ae80: 286a eb02 0000 6840 6aec 0200 005d 946a  (j....h@j....].j
-0000ae90: 1305 0000 2981 947d 9428 6aeb 0200 0068  ....)..}.(j....h
-0000aea0: 406a ec02 0000 5d94 286a e602 0000 8c11  @j....].(j......
-0000aeb0: 636f 6d70 6163 745f 7061 7261 6772 6170  compact_paragrap
-0000aec0: 6894 9394 2981 947d 9428 6aeb 0200 0068  h...)..}.(j....h
-0000aed0: 406a ec02 0000 5d94 6adb 0a00 0029 8194  @j....].j....)..
-0000aee0: 7d94 286a eb02 0000 6840 6aec 0200 005d  }.(j....h@j....]
-0000aef0: 946a fa02 0000 8c11 636f 6f6b 6965 735f  .j......cookies_
-0000af00: 7574 696c 6974 6965 7394 8594 8194 7d94  utilities.....}.
-0000af10: 6aff 0200 006a b70c 0000 7362 616a 0303  j....j....sbaj..
-0000af20: 0000 7d94 286a 160c 0000 5d94 6a18 0c00  ..}.(j....].j...
-0000af30: 005d 946a 1a0c 0000 5d94 6a1c 0c00 005d  .].j....].j....]
-0000af40: 946a 1e0c 0000 5d94 8c08 696e 7465 726e  .j....]...intern
-0000af50: 616c 9488 8c06 7265 6675 7269 946a ca02  al....refuri.j..
-0000af60: 0000 8c0a 616e 6368 6f72 6e61 6d65 9468  ....anchorname.h
-0000af70: 4075 6a0f 0300 008c 0972 6566 6572 656e  @uj......referen
-0000af80: 6365 946a ff02 0000 6ab4 0c00 0075 6261  ce.j....j....uba
-0000af90: 6a03 0300 007d 9428 6a16 0c00 005d 946a  j....}.(j....].j
-0000afa0: 180c 0000 5d94 6a1a 0c00 005d 946a 1c0c  ....].j....].j..
-0000afb0: 0000 5d94 6a1e 0c00 005d 9475 6a0f 0300  ..].j....].uj...
-0000afc0: 008c 1163 6f6d 7061 6374 5f70 6172 6167  ...compact_parag
-0000afd0: 7261 7068 946a ff02 0000 6aaf 0c00 0075  raph.j....j....u
-0000afe0: 626a 0e05 0000 2981 947d 9428 6aeb 0200  bj....)..}.(j...
-0000aff0: 0068 406a ec02 0000 5d94 6a4d 0b00 0029  .h@j....].jM...)
-0000b000: 8194 7d94 286a eb02 0000 6840 6aec 0200  ..}.(j....h@j...
-0000b010: 005d 946a 0303 0000 7d94 286a 160c 0000  .].j....}.(j....
-0000b020: 5d94 6a18 0c00 005d 946a 1a0c 0000 5d94  ].j....].j....].
-0000b030: 6a1c 0c00 005d 946a 1e0c 0000 5d94 8c06  j....].j....]...
-0000b040: 7061 7265 6e74 946a ca02 0000 8c07 656e  parent.j......en
-0000b050: 7472 6965 7394 6a30 0c00 008c 0c69 6e63  tries.j0.....inc
-0000b060: 6c75 6465 6669 6c65 7394 6a34 0c00 008c  ludefiles.j4....
-0000b070: 086d 6178 6465 7074 6894 4b04 8c07 6361  .maxdepth.K...ca
-0000b080: 7074 696f 6e94 4e8c 0467 6c6f 6294 898c  ption.N..glob...
-0000b090: 0668 6964 6465 6e94 898c 0d69 6e63 6c75  .hidden....inclu
-0000b0a0: 6465 6869 6464 656e 9489 8c08 6e75 6d62  dehidden....numb
-0000b0b0: 6572 6564 944b 008c 0a74 6974 6c65 736f  ered.K...titleso
-0000b0c0: 6e6c 7994 898c 0a72 6177 656e 7472 6965  nly....rawentrie
-0000b0d0: 7394 6a3d 0c00 0075 6a0f 0300 006a 3e0c  s.j=...uj....j>.
-0000b0e0: 0000 6a01 0300 006a 210c 0000 6a02 0300  ..j....j!...j...
-0000b0f0: 004b 046a ff02 0000 6acf 0c00 0075 6261  .K.j....j....uba
-0000b100: 6a03 0300 007d 9428 6a16 0c00 005d 946a  j....}.(j....].j
-0000b110: 180c 0000 5d94 6a1a 0c00 005d 946a 1c0c  ....].j....].j..
-0000b120: 0000 5d94 6a1e 0c00 005d 9475 6a0f 0300  ..].j....].uj...
-0000b130: 008c 0b62 756c 6c65 745f 6c69 7374 946a  ...bullet_list.j
-0000b140: ff02 0000 6aaf 0c00 0075 6265 6a03 0300  ....j....ubej...
-0000b150: 007d 9428 6a16 0c00 005d 946a 180c 0000  .}.(j....].j....
-0000b160: 5d94 6a1a 0c00 005d 946a 1c0c 0000 5d94  ].j....].j....].
-0000b170: 6a1e 0c00 005d 9475 6a0f 0300 008c 096c  j....].uj......l
-0000b180: 6973 745f 6974 656d 946a ff02 0000 6aac  ist_item.j....j.
-0000b190: 0c00 0075 6261 6a03 0300 007d 9428 6a16  ...ubaj....}.(j.
-0000b1a0: 0c00 005d 946a 180c 0000 5d94 6a1a 0c00  ...].j....].j...
-0000b1b0: 005d 946a 1c0c 0000 5d94 6a1e 0c00 005d  .].j....].j....]
-0000b1c0: 9475 6a0f 0300 006a ec0c 0000 7562 6acb  .uj....j....ubj.
-0000b1d0: 0200 006a 0e05 0000 2981 947d 9428 6aeb  ...j....)..}.(j.
-0000b1e0: 0200 0068 406a ec02 0000 5d94 6a13 0500  ...h@j....].j...
-0000b1f0: 0029 8194 7d94 286a eb02 0000 6840 6aec  .)..}.(j....h@j.
-0000b200: 0200 005d 9428 6ab3 0c00 0029 8194 7d94  ...].(j....)..}.
-0000b210: 286a eb02 0000 6840 6aec 0200 005d 946a  (j....h@j....].j
-0000b220: db0a 0000 2981 947d 9428 6aeb 0200 0068  ....)..}.(j....h
-0000b230: 406a ec02 0000 5d94 6afa 0200 008c 2e57  @j....].j......W
-0000b240: 656c 636f 6d65 2074 6f20 636f 6f6b 6965  elcome to cookie
-0000b250: 735f 7574 696c 6974 6965 73e2 8099 2064  s_utilities... d
-0000b260: 6f63 756d 656e 7461 7469 6f6e 2194 8594  ocumentation!...
-0000b270: 8194 7d94 6aff 0200 006a 030d 0000 7362  ..}.j....j....sb
-0000b280: 616a 0303 0000 7d94 286a b30a 0000 5d94  aj....}.(j....].
-0000b290: 6ab5 0a00 005d 946a b70a 0000 5d94 6ab9  j....].j....].j.
-0000b2a0: 0a00 005d 946a bb0a 0000 5d94 8c08 696e  ...].j....]...in
-0000b2b0: 7465 726e 616c 9488 8c06 7265 6675 7269  ternal....refuri
-0000b2c0: 946a cb02 0000 8c0a 616e 6368 6f72 6e61  .j......anchorna
-0000b2d0: 6d65 9468 4075 6a0f 0300 006a ed0a 0000  me.h@uj....j....
-0000b2e0: 6aff 0200 006a 000d 0000 7562 616a 0303  j....j....ubaj..
-0000b2f0: 0000 7d94 286a b30a 0000 5d94 6ab5 0a00  ..}.(j....].j...
-0000b300: 005d 946a b70a 0000 5d94 6ab9 0a00 005d  .].j....].j....]
-0000b310: 946a bb0a 0000 5d94 756a 0f03 0000 8c11  .j....].uj......
-0000b320: 636f 6d70 6163 745f 7061 7261 6772 6170  compact_paragrap
-0000b330: 6894 6aff 0200 006a fd0c 0000 7562 6a0e  h.j....j....ubj.
-0000b340: 0500 0029 8194 7d94 286a eb02 0000 6840  ...)..}.(j....h@
-0000b350: 6aec 0200 005d 9428 6a13 0500 0029 8194  j....].(j....)..
-0000b360: 7d94 286a eb02 0000 6840 6aec 0200 005d  }.(j....h@j....]
-0000b370: 9428 6ab3 0c00 0029 8194 7d94 286a eb02  .(j....)..}.(j..
-0000b380: 0000 6840 6aec 0200 005d 946a db0a 0000  ..h@j....].j....
-0000b390: 2981 947d 9428 6aeb 0200 0068 406a ec02  )..}.(j....h@j..
-0000b3a0: 0000 5d94 6afa 0200 008c 054c 696e 6b73  ..].j......Links
-0000b3b0: 9485 9481 947d 946a ff02 0000 6a23 0d00  .....}.j....j#..
-0000b3c0: 0073 6261 6a03 0300 007d 9428 6ab3 0a00  .sbaj....}.(j...
-0000b3d0: 005d 946a b50a 0000 5d94 6ab7 0a00 005d  .].j....].j....]
-0000b3e0: 946a b90a 0000 5d94 6abb 0a00 005d 948c  .j....].j....]..
-0000b3f0: 0869 6e74 6572 6e61 6c94 888c 0672 6566  .internal....ref
-0000b400: 7572 6994 6acb 0200 008c 0a61 6e63 686f  uri.j......ancho
-0000b410: 726e 616d 6594 8c06 236c 696e 6b73 9475  rname...#links.u
-0000b420: 6a0f 0300 006a ed0a 0000 6aff 0200 006a  j....j....j....j
-0000b430: 200d 0000 7562 616a 0303 0000 7d94 286a   ...ubaj....}.(j
-0000b440: b30a 0000 5d94 6ab5 0a00 005d 946a b70a  ....].j....].j..
-0000b450: 0000 5d94 6ab9 0a00 005d 946a bb0a 0000  ..].j....].j....
-0000b460: 5d94 756a 0f03 0000 6a19 0d00 006a ff02  ].uj....j....j..
-0000b470: 0000 6a1d 0d00 0075 626a 0e05 0000 2981  ..j....ubj....).
-0000b480: 947d 9428 6aeb 0200 0068 406a ec02 0000  .}.(j....h@j....
-0000b490: 5d94 6a4d 0b00 0029 8194 7d94 286a eb02  ].jM...)..}.(j..
-0000b4a0: 0000 6840 6aec 0200 005d 946a 0303 0000  ..h@j....].j....
-0000b4b0: 7d94 286a b30a 0000 5d94 6ab5 0a00 005d  }.(j....].j....]
-0000b4c0: 946a b70a 0000 5d94 6ab9 0a00 005d 946a  .j....].j....].j
-0000b4d0: bb0a 0000 5d94 8c06 7061 7265 6e74 946a  ....]...parent.j
-0000b4e0: cb02 0000 8c07 656e 7472 6965 7394 6a59  ......entries.jY
-0000b4f0: 0b00 008c 0c69 6e63 6c75 6465 6669 6c65  .....includefile
-0000b500: 7394 6a5d 0b00 008c 086d 6178 6465 7074  s.j].....maxdept
-0000b510: 6894 4b02 8c07 6361 7074 696f 6e94 6a60  h.K...caption.j`
-0000b520: 0b00 008c 0467 6c6f 6294 898c 0668 6964  .....glob....hid
-0000b530: 6465 6e94 898c 0d69 6e63 6c75 6465 6869  den....includehi
-0000b540: 6464 656e 9489 8c08 6e75 6d62 6572 6564  dden....numbered
-0000b550: 944b 008c 0a74 6974 6c65 736f 6e6c 7994  .K...titlesonly.
-0000b560: 898c 0a72 6177 656e 7472 6965 7394 6a67  ...rawentries.jg
-0000b570: 0b00 008c 0a72 6177 6361 7074 696f 6e94  .....rawcaption.
-0000b580: 6a60 0b00 0075 6a0f 0300 006a 690b 0000  j`...uj....ji...
-0000b590: 6a01 0300 006a be0a 0000 6a02 0300 004b  j....j....j....K
-0000b5a0: 0a6a ff02 0000 6a3a 0d00 0075 6261 6a03  .j....j:...ubaj.
-0000b5b0: 0300 007d 9428 6ab3 0a00 005d 946a b50a  ...}.(j....].j..
-0000b5c0: 0000 5d94 6ab7 0a00 005d 946a b90a 0000  ..].j....].j....
-0000b5d0: 5d94 6abb 0a00 005d 9475 6a0f 0300 006a  ].j....].uj....j
-0000b5e0: 460b 0000 6aff 0200 006a 1d0d 0000 7562  F...j....j....ub
-0000b5f0: 656a 0303 0000 7d94 286a b30a 0000 5d94  ej....}.(j....].
-0000b600: 6ab5 0a00 005d 946a b70a 0000 5d94 6ab9  j....].j....].j.
-0000b610: 0a00 005d 946a bb0a 0000 5d94 756a 0f03  ...].j....].uj..
-0000b620: 0000 6a0c 0b00 006a ff02 0000 6a1a 0d00  ..j....j....j...
-0000b630: 0075 626a 1305 0000 2981 947d 9428 6aeb  .ubj....)..}.(j.
-0000b640: 0200 0068 406a ec02 0000 5d94 6ab3 0c00  ...h@j....].j...
-0000b650: 0029 8194 7d94 286a eb02 0000 6840 6aec  .)..}.(j....h@j.
-0000b660: 0200 005d 946a db0a 0000 2981 947d 9428  ...].j....)..}.(
-0000b670: 6aeb 0200 0068 406a ec02 0000 5d94 6afa  j....h@j....].j.
-0000b680: 0200 008c 1249 6e64 6963 6573 2061 6e64  .....Indices and
-0000b690: 2074 6162 6c65 7394 8594 8194 7d94 6aff   tables.....}.j.
-0000b6a0: 0200 006a 640d 0000 7362 616a 0303 0000  ...jd...sbaj....
-0000b6b0: 7d94 286a b30a 0000 5d94 6ab5 0a00 005d  }.(j....].j....]
-0000b6c0: 946a b70a 0000 5d94 6ab9 0a00 005d 946a  .j....].j....].j
-0000b6d0: bb0a 0000 5d94 8c08 696e 7465 726e 616c  ....]...internal
-0000b6e0: 9488 8c06 7265 6675 7269 946a cb02 0000  ....refuri.j....
-0000b6f0: 8c0a 616e 6368 6f72 6e61 6d65 948c 1323  ..anchorname...#
-0000b700: 696e 6469 6365 732d 616e 642d 7461 626c  indices-and-tabl
-0000b710: 6573 9475 6a0f 0300 006a ed0a 0000 6aff  es.uj....j....j.
-0000b720: 0200 006a 610d 0000 7562 616a 0303 0000  ...ja...ubaj....
-0000b730: 7d94 286a b30a 0000 5d94 6ab5 0a00 005d  }.(j....].j....]
-0000b740: 946a b70a 0000 5d94 6ab9 0a00 005d 946a  .j....].j....].j
-0000b750: bb0a 0000 5d94 756a 0f03 0000 6a19 0d00  ....].uj....j...
-0000b760: 006a ff02 0000 6a5e 0d00 0075 6261 6a03  .j....j^...ubaj.
-0000b770: 0300 007d 9428 6ab3 0a00 005d 946a b50a  ...}.(j....].j..
-0000b780: 0000 5d94 6ab7 0a00 005d 946a b90a 0000  ..].j....].j....
-0000b790: 5d94 6abb 0a00 005d 9475 6a0f 0300 006a  ].j....].uj....j
-0000b7a0: 0c0b 0000 6aff 0200 006a 1a0d 0000 7562  ....j....j....ub
-0000b7b0: 656a 0303 0000 7d94 286a b30a 0000 5d94  ej....}.(j....].
-0000b7c0: 6ab5 0a00 005d 946a b70a 0000 5d94 6ab9  j....].j....].j.
-0000b7d0: 0a00 005d 946a bb0a 0000 5d94 756a 0f03  ...].j....].uj..
-0000b7e0: 0000 6a46 0b00 006a ff02 0000 6afd 0c00  ..jF...j....j...
-0000b7f0: 0075 6265 6a03 0300 007d 9428 6ab3 0a00  .ubej....}.(j...
-0000b800: 005d 946a b50a 0000 5d94 6ab7 0a00 005d  .].j....].j....]
-0000b810: 946a b90a 0000 5d94 6abb 0a00 005d 9475  .j....].j....].u
-0000b820: 6a0f 0300 006a 0c0b 0000 6aff 0200 006a  j....j....j....j
-0000b830: fa0c 0000 7562 616a 0303 0000 7d94 286a  ....ubaj....}.(j
-0000b840: b30a 0000 5d94 6ab5 0a00 005d 946a b70a  ....].j....].j..
-0000b850: 0000 5d94 6ab9 0a00 005d 946a bb0a 0000  ..].j....].j....
-0000b860: 5d94 756a 0f03 0000 6a46 0b00 0075 626a  ].uj....jF...ubj
-0000b870: 9a02 0000 6a0e 0500 0029 8194 7d94 286a  ....j....)..}.(j
-0000b880: eb02 0000 6840 6aec 0200 005d 946a 1305  ....h@j....].j..
-0000b890: 0000 2981 947d 9428 6aeb 0200 0068 406a  ..)..}.(j....h@j
-0000b8a0: ec02 0000 5d94 286a b30c 0000 2981 947d  ....].(j....)..}
-0000b8b0: 9428 6aeb 0200 0068 406a ec02 0000 5d94  .(j....h@j....].
-0000b8c0: 6adb 0a00 0029 8194 7d94 286a eb02 0000  j....)..}.(j....
-0000b8d0: 6840 6aec 0200 005d 946a fa02 0000 8c0d  h@j....].j......
-0000b8e0: 446f 6375 6d65 6e74 6174 696f 6e94 8594  Documentation...
-0000b8f0: 8194 7d94 6aff 0200 006a 9c0d 0000 7362  ..}.j....j....sb
-0000b900: 616a 0303 0000 7d94 286a 0503 0000 5d94  aj....}.(j....].
-0000b910: 6a07 0300 005d 946a 0903 0000 5d94 6a0b  j....].j....].j.
-0000b920: 0300 005d 946a 0d03 0000 5d94 8c08 696e  ...].j....]...in
-0000b930: 7465 726e 616c 9488 8c06 7265 6675 7269  ternal....refuri
-0000b940: 946a 9a02 0000 8c0a 616e 6368 6f72 6e61  .j......anchorna
-0000b950: 6d65 9468 4075 6a0f 0300 006a da0a 0000  me.h@uj....j....
-0000b960: 6aff 0200 006a 990d 0000 7562 616a 0303  j....j....ubaj..
-0000b970: 0000 7d94 286a 0503 0000 5d94 6a07 0300  ..}.(j....].j...
-0000b980: 005d 946a 0903 0000 5d94 6a0b 0300 005d  .].j....].j....]
-0000b990: 946a 0d03 0000 5d94 756a 0f03 0000 6ab2  .j....].uj....j.
-0000b9a0: 0c00 006a ff02 0000 6a96 0d00 0075 626a  ...j....j....ubj
-0000b9b0: 0e05 0000 2981 947d 9428 6aeb 0200 0068  ....)..}.(j....h
-0000b9c0: 406a ec02 0000 5d94 286a 1305 0000 2981  @j....].(j....).
-0000b9d0: 947d 9428 6aeb 0200 0068 406a ec02 0000  .}.(j....h@j....
-0000b9e0: 5d94 286a b30c 0000 2981 947d 9428 6aeb  ].(j....)..}.(j.
-0000b9f0: 0200 0068 406a ec02 0000 5d94 6adb 0a00  ...h@j....].j...
-0000ba00: 0029 8194 7d94 286a eb02 0000 6840 6aec  .)..}.(j....h@j.
-0000ba10: 0200 005d 946a fa02 0000 8c09 4675 6e63  ...].j......Func
-0000ba20: 7469 6f6e 7394 8594 8194 7d94 6aff 0200  tions.....}.j...
-0000ba30: 006a bb0d 0000 7362 616a 0303 0000 7d94  .j....sbaj....}.
-0000ba40: 286a 0503 0000 5d94 6a07 0300 005d 946a  (j....].j....].j
-0000ba50: 0903 0000 5d94 6a0b 0300 005d 946a 0d03  ....].j....].j..
-0000ba60: 0000 5d94 8c08 696e 7465 726e 616c 9488  ..]...internal..
-0000ba70: 8c06 7265 6675 7269 946a 9a02 0000 8c0a  ..refuri.j......
-0000ba80: 616e 6368 6f72 6e61 6d65 948c 0a23 6675  anchorname...#fu
-0000ba90: 6e63 7469 6f6e 7394 756a 0f03 0000 6ada  nctions.uj....j.
-0000baa0: 0a00 006a ff02 0000 6ab8 0d00 0075 6261  ...j....j....uba
-0000bab0: 6a03 0300 007d 9428 6a05 0300 005d 946a  j....}.(j....].j
-0000bac0: 0703 0000 5d94 6a09 0300 005d 946a 0b03  ....].j....].j..
-0000bad0: 0000 5d94 6a0d 0300 005d 9475 6a0f 0300  ..].j....].uj...
-0000bae0: 006a b20c 0000 6aff 0200 006a b50d 0000  .j....j....j....
-0000baf0: 7562 6a0e 0500 0029 8194 7d94 286a eb02  ubj....)..}.(j..
-0000bb00: 0000 6840 6aec 0200 005d 946a 1305 0000  ..h@j....].j....
-0000bb10: 2981 947d 9428 6aeb 0200 0068 406a ec02  )..}.(j....h@j..
-0000bb20: 0000 5d94 286a b30c 0000 2981 947d 9428  ..].(j....)..}.(
-0000bb30: 6aeb 0200 0068 406a ec02 0000 5d94 6adb  j....h@j....].j.
-0000bb40: 0a00 0029 8194 7d94 286a eb02 0000 6840  ...)..}.(j....h@
-0000bb50: 6aec 0200 005d 946a fa02 0000 8c1b 636f  j....].j......co
-0000bb60: 6f6b 6965 735f 7574 696c 6974 6965 732e  okies_utilities.
-0000bb70: 6765 745f 6461 7465 7394 8594 8194 7d94  get_dates.....}.
-0000bb80: 6aff 0200 006a db0d 0000 7362 616a 0303  j....j....sbaj..
-0000bb90: 0000 7d94 286a 0503 0000 5d94 6a07 0300  ..}.(j....].j...
-0000bba0: 005d 946a 0903 0000 5d94 6a0b 0300 005d  .].j....].j....]
-0000bbb0: 946a 0d03 0000 5d94 8c08 696e 7465 726e  .j....]...intern
-0000bbc0: 616c 9488 8c06 7265 6675 7269 946a 9a02  al....refuri.j..
-0000bbd0: 0000 8c0a 616e 6368 6f72 6e61 6d65 948c  ....anchorname..
-0000bbe0: 1c23 636f 6f6b 6965 732d 7574 696c 6974  .#cookies-utilit
-0000bbf0: 6965 732d 6765 742d 6461 7465 7394 756a  ies-get-dates.uj
-0000bc00: 0f03 0000 6ada 0a00 006a ff02 0000 6ad8  ....j....j....j.
-0000bc10: 0d00 0075 6261 6a03 0300 007d 9428 6a05  ...ubaj....}.(j.
-0000bc20: 0300 005d 946a 0703 0000 5d94 6a09 0300  ...].j....].j...
-0000bc30: 005d 946a 0b03 0000 5d94 6a0d 0300 005d  .].j....].j....]
-0000bc40: 9475 6a0f 0300 006a b20c 0000 6aff 0200  .uj....j....j...
-0000bc50: 006a d50d 0000 7562 6a0e 0500 0029 8194  .j....ubj....)..
-0000bc60: 7d94 286a eb02 0000 6840 6aec 0200 005d  }.(j....h@j....]
-0000bc70: 946a 1305 0000 2981 947d 9428 6aeb 0200  .j....)..}.(j...
-0000bc80: 0068 406a ec02 0000 5d94 6ab3 0c00 0029  .h@j....].j....)
-0000bc90: 8194 7d94 286a eb02 0000 6840 6aec 0200  ..}.(j....h@j...
-0000bca0: 005d 946a db0a 0000 2981 947d 9428 6aeb  .].j....)..}.(j.
-0000bcb0: 0200 0068 406a ec02 0000 5d94 6aee 0200  ...h@j....].j...
-0000bcc0: 008c 076c 6974 6572 616c 9493 9429 8194  ...literal...)..
-0000bcd0: 7d94 286a eb02 0000 6840 6aec 0200 005d  }.(j....h@j....]
-0000bce0: 946a fa02 0000 8c0b 6765 745f 6461 7465  .j......get_date
-0000bcf0: 7328 2994 8594 8194 7d94 6aff 0200 006a  s().....}.j....j
-0000bd00: 000e 0000 7362 616a 0303 0000 7d94 286a  ....sbaj....}.(j
-0000bd10: 0503 0000 5d94 6a07 0300 005d 946a 0903  ....].j....].j..
-0000bd20: 0000 5d94 6a0b 0300 005d 946a 0d03 0000  ..].j....].j....
-0000bd30: 5d94 756a 0f03 0000 6afe 0d00 006a ff02  ].uj....j....j..
-0000bd40: 0000 6afb 0d00 0075 6261 6a03 0300 007d  ..j....ubaj....}
-0000bd50: 9428 6a05 0300 005d 946a 0703 0000 5d94  .(j....].j....].
-0000bd60: 6a09 0300 005d 946a 0b03 0000 5d94 6a0d  j....].j....].j.
-0000bd70: 0300 005d 948c 0869 6e74 6572 6e61 6c94  ...]...internal.
-0000bd80: 888c 0672 6566 7572 6994 6a9a 0200 008c  ...refuri.j.....
-0000bd90: 0a61 6e63 686f 726e 616d 6594 8c1c 2363  .anchorname...#c
-0000bda0: 6f6f 6b69 6573 5f75 7469 6c69 7469 6573  ookies_utilities
-0000bdb0: 2e67 6574 5f64 6174 6573 9475 6a0f 0300  .get_dates.uj...
-0000bdc0: 006a da0a 0000 6aff 0200 006a f80d 0000  .j....j....j....
-0000bdd0: 7562 616a 0303 0000 7d94 286a 0503 0000  ubaj....}.(j....
-0000bde0: 5d94 6a07 0300 005d 946a 0903 0000 5d94  ].j....].j....].
-0000bdf0: 6a0b 0300 005d 946a 0d03 0000 5d94 8c13  j....].j....]...
-0000be00: 736b 6970 5f73 6563 7469 6f6e 5f6e 756d  skip_section_num
-0000be10: 6265 7294 8875 6a0f 0300 006a b20c 0000  ber..uj....j....
-0000be20: 6aff 0200 006a f50d 0000 7562 616a 0303  j....j....ubaj..
-0000be30: 0000 7d94 286a 0503 0000 5d94 6a07 0300  ..}.(j....].j...
-0000be40: 005d 946a 0903 0000 5d94 6a0b 0300 005d  .].j....].j....]
-0000be50: 946a 0d03 0000 5d94 756a 0f03 0000 6a12  .j....].uj....j.
-0000be60: 0500 006a ff02 0000 6af2 0d00 0075 6261  ...j....j....uba
-0000be70: 6a03 0300 007d 9428 6a05 0300 005d 946a  j....}.(j....].j
-0000be80: 0703 0000 5d94 6a09 0300 005d 946a 0b03  ....].j....].j..
-0000be90: 0000 5d94 6a0d 0300 005d 9475 6a0f 0300  ..].j....].uj...
-0000bea0: 006a 0d05 0000 6aff 0200 006a d50d 0000  .j....j....j....
-0000beb0: 7562 656a 0303 0000 7d94 286a 0503 0000  ubej....}.(j....
-0000bec0: 5d94 6a07 0300 005d 946a 0903 0000 5d94  ].j....].j....].
-0000bed0: 6a0b 0300 005d 946a 0d03 0000 5d94 756a  j....].j....].uj
-0000bee0: 0f03 0000 6a12 0500 006a ff02 0000 6ad2  ....j....j....j.
-0000bef0: 0d00 0075 6261 6a03 0300 007d 9428 6a05  ...ubaj....}.(j.
-0000bf00: 0300 005d 946a 0703 0000 5d94 6a09 0300  ...].j....].j...
-0000bf10: 005d 946a 0b03 0000 5d94 6a0d 0300 005d  .].j....].j....]
-0000bf20: 9475 6a0f 0300 006a 0d05 0000 6aff 0200  .uj....j....j...
-0000bf30: 006a b50d 0000 7562 656a 0303 0000 7d94  .j....ubej....}.
-0000bf40: 286a 0503 0000 5d94 6a07 0300 005d 946a  (j....].j....].j
-0000bf50: 0903 0000 5d94 6a0b 0300 005d 946a 0d03  ....].j....].j..
-0000bf60: 0000 5d94 756a 0f03 0000 6a12 0500 006a  ..].uj....j....j
-0000bf70: ff02 0000 6ab2 0d00 0075 626a 1305 0000  ....j....ubj....
-0000bf80: 2981 947d 9428 6aeb 0200 0068 406a ec02  )..}.(j....h@j..
-0000bf90: 0000 5d94 286a b30c 0000 2981 947d 9428  ..].(j....)..}.(
-0000bfa0: 6aeb 0200 0068 406a ec02 0000 5d94 6adb  j....h@j....].j.
-0000bfb0: 0a00 0029 8194 7d94 286a eb02 0000 6840  ...)..}.(j....h@
-0000bfc0: 6aec 0200 005d 946a fa02 0000 8c07 436c  j....].j......Cl
-0000bfd0: 6173 7365 7394 8594 8194 7d94 6aff 0200  asses.....}.j...
-0000bfe0: 006a 420e 0000 7362 616a 0303 0000 7d94  .jB...sbaj....}.
-0000bff0: 286a 0503 0000 5d94 6a07 0300 005d 946a  (j....].j....].j
-0000c000: 0903 0000 5d94 6a0b 0300 005d 946a 0d03  ....].j....].j..
-0000c010: 0000 5d94 8c08 696e 7465 726e 616c 9488  ..]...internal..
-0000c020: 8c06 7265 6675 7269 946a 9a02 0000 8c0a  ..refuri.j......
-0000c030: 616e 6368 6f72 6e61 6d65 948c 0823 636c  anchorname...#cl
-0000c040: 6173 7365 7394 756a 0f03 0000 6ada 0a00  asses.uj....j...
-0000c050: 006a ff02 0000 6a3f 0e00 0075 6261 6a03  .j....j?...ubaj.
-0000c060: 0300 007d 9428 6a05 0300 005d 946a 0703  ...}.(j....].j..
-0000c070: 0000 5d94 6a09 0300 005d 946a 0b03 0000  ..].j....].j....
-0000c080: 5d94 6a0d 0300 005d 9475 6a0f 0300 006a  ].j....].uj....j
-0000c090: b20c 0000 6aff 0200 006a 3c0e 0000 7562  ....j....j<...ub
-0000c0a0: 6a0e 0500 0029 8194 7d94 286a eb02 0000  j....)..}.(j....
-0000c0b0: 6840 6aec 0200 005d 946a 1305 0000 2981  h@j....].j....).
-0000c0c0: 947d 9428 6aeb 0200 0068 406a ec02 0000  .}.(j....h@j....
-0000c0d0: 5d94 286a b30c 0000 2981 947d 9428 6aeb  ].(j....)..}.(j.
-0000c0e0: 0200 0068 406a ec02 0000 5d94 6adb 0a00  ...h@j....].j...
-0000c0f0: 0029 8194 7d94 286a eb02 0000 6840 6aec  .)..}.(j....h@j.
-0000c100: 0200 005d 946a fa02 0000 8c1b 636f 6f6b  ...].j......cook
-0000c110: 6965 735f 7574 696c 6974 6965 732e 5374  ies_utilities.St
-0000c120: 6f70 7761 7463 6894 8594 8194 7d94 6aff  opwatch.....}.j.
-0000c130: 0200 006a 620e 0000 7362 616a 0303 0000  ...jb...sbaj....
-0000c140: 7d94 286a 0503 0000 5d94 6a07 0300 005d  }.(j....].j....]
-0000c150: 946a 0903 0000 5d94 6a0b 0300 005d 946a  .j....].j....].j
-0000c160: 0d03 0000 5d94 8c08 696e 7465 726e 616c  ....]...internal
-0000c170: 9488 8c06 7265 6675 7269 946a 9a02 0000  ....refuri.j....
-0000c180: 8c0a 616e 6368 6f72 6e61 6d65 948c 1c23  ..anchorname...#
-0000c190: 636f 6f6b 6965 732d 7574 696c 6974 6965  cookies-utilitie
-0000c1a0: 732d 7374 6f70 7761 7463 6894 756a 0f03  s-stopwatch.uj..
-0000c1b0: 0000 6ada 0a00 006a ff02 0000 6a5f 0e00  ..j....j....j_..
-0000c1c0: 0075 6261 6a03 0300 007d 9428 6a05 0300  .ubaj....}.(j...
-0000c1d0: 005d 946a 0703 0000 5d94 6a09 0300 005d  .].j....].j....]
-0000c1e0: 946a 0b03 0000 5d94 6a0d 0300 005d 9475  .j....].j....].u
-0000c1f0: 6a0f 0300 006a b20c 0000 6aff 0200 006a  j....j....j....j
-0000c200: 5c0e 0000 7562 6a0e 0500 0029 8194 7d94  \...ubj....)..}.
-0000c210: 286a eb02 0000 6840 6aec 0200 005d 946a  (j....h@j....].j
-0000c220: 1305 0000 2981 947d 9428 6aeb 0200 0068  ....)..}.(j....h
-0000c230: 406a ec02 0000 5d94 286a b30c 0000 2981  @j....].(j....).
-0000c240: 947d 9428 6aeb 0200 0068 406a ec02 0000  .}.(j....h@j....
-0000c250: 5d94 6adb 0a00 0029 8194 7d94 286a eb02  ].j....)..}.(j..
-0000c260: 0000 6840 6aec 0200 005d 946a ff0d 0000  ..h@j....].j....
-0000c270: 2981 947d 9428 6aeb 0200 0068 406a ec02  )..}.(j....h@j..
-0000c280: 0000 5d94 6afa 0200 008c 0953 746f 7077  ..].j......Stopw
-0000c290: 6174 6368 9485 9481 947d 946a ff02 0000  atch.....}.j....
-0000c2a0: 6a85 0e00 0073 6261 6a03 0300 007d 9428  j....sbaj....}.(
-0000c2b0: 6a05 0300 005d 946a 0703 0000 5d94 6a09  j....].j....].j.
-0000c2c0: 0300 005d 946a 0b03 0000 5d94 6a0d 0300  ...].j....].j...
-0000c2d0: 005d 9475 6a0f 0300 006a fe0d 0000 6aff  .].uj....j....j.
-0000c2e0: 0200 006a 820e 0000 7562 616a 0303 0000  ...j....ubaj....
-0000c2f0: 7d94 286a 0503 0000 5d94 6a07 0300 005d  }.(j....].j....]
-0000c300: 946a 0903 0000 5d94 6a0b 0300 005d 946a  .j....].j....].j
-0000c310: 0d03 0000 5d94 8c08 696e 7465 726e 616c  ....]...internal
-0000c320: 9488 8c06 7265 6675 7269 946a 9a02 0000  ....refuri.j....
-0000c330: 8c0a 616e 6368 6f72 6e61 6d65 948c 1c23  ..anchorname...#
-0000c340: 636f 6f6b 6965 735f 7574 696c 6974 6965  cookies_utilitie
-0000c350: 732e 5374 6f70 7761 7463 6894 756a 0f03  s.Stopwatch.uj..
-0000c360: 0000 6ada 0a00 006a ff02 0000 6a7f 0e00  ..j....j....j...
-0000c370: 0075 6261 6a03 0300 007d 9428 6a05 0300  .ubaj....}.(j...
-0000c380: 005d 946a 0703 0000 5d94 6a09 0300 005d  .].j....].j....]
-0000c390: 946a 0b03 0000 5d94 6a0d 0300 005d 948c  .j....].j....]..
-0000c3a0: 1373 6b69 705f 7365 6374 696f 6e5f 6e75  .skip_section_nu
-0000c3b0: 6d62 6572 9488 756a 0f03 0000 6ab2 0c00  mber..uj....j...
-0000c3c0: 006a ff02 0000 6a7c 0e00 0075 626a 0e05  .j....j|...ubj..
-0000c3d0: 0000 2981 947d 9428 6aeb 0200 0068 406a  ..)..}.(j....h@j
-0000c3e0: ec02 0000 5d94 286a 1305 0000 2981 947d  ....].(j....)..}
-0000c3f0: 9428 6aeb 0200 0068 406a ec02 0000 5d94  .(j....h@j....].
-0000c400: 6ab3 0c00 0029 8194 7d94 286a eb02 0000  j....)..}.(j....
-0000c410: 6840 6aec 0200 005d 946a db0a 0000 2981  h@j....].j....).
-0000c420: 947d 9428 6aeb 0200 0068 406a ec02 0000  .}.(j....h@j....
-0000c430: 5d94 6aff 0d00 0029 8194 7d94 286a eb02  ].j....)..}.(j..
-0000c440: 0000 6840 6aec 0200 005d 946a fa02 0000  ..h@j....].j....
-0000c450: 8c11 5374 6f70 7761 7463 682e 7072 6573  ..Stopwatch.pres
-0000c460: 7328 2994 8594 8194 7d94 6aff 0200 006a  s().....}.j....j
-0000c470: af0e 0000 7362 616a 0303 0000 7d94 286a  ....sbaj....}.(j
-0000c480: 0503 0000 5d94 6a07 0300 005d 946a 0903  ....].j....].j..
-0000c490: 0000 5d94 6a0b 0300 005d 946a 0d03 0000  ..].j....].j....
-0000c4a0: 5d94 756a 0f03 0000 6afe 0d00 006a ff02  ].uj....j....j..
-0000c4b0: 0000 6aac 0e00 0075 6261 6a03 0300 007d  ..j....ubaj....}
-0000c4c0: 9428 6a05 0300 005d 946a 0703 0000 5d94  .(j....].j....].
-0000c4d0: 6a09 0300 005d 946a 0b03 0000 5d94 6a0d  j....].j....].j.
-0000c4e0: 0300 005d 948c 0869 6e74 6572 6e61 6c94  ...]...internal.
-0000c4f0: 888c 0672 6566 7572 6994 6a9a 0200 008c  ...refuri.j.....
-0000c500: 0a61 6e63 686f 726e 616d 6594 8c22 2363  .anchorname.."#c
-0000c510: 6f6f 6b69 6573 5f75 7469 6c69 7469 6573  ookies_utilities
-0000c520: 2e53 746f 7077 6174 6368 2e70 7265 7373  .Stopwatch.press
-0000c530: 9475 6a0f 0300 006a da0a 0000 6aff 0200  .uj....j....j...
-0000c540: 006a a90e 0000 7562 616a 0303 0000 7d94  .j....ubaj....}.
-0000c550: 286a 0503 0000 5d94 6a07 0300 005d 946a  (j....].j....].j
-0000c560: 0903 0000 5d94 6a0b 0300 005d 946a 0d03  ....].j....].j..
-0000c570: 0000 5d94 8c13 736b 6970 5f73 6563 7469  ..]...skip_secti
-0000c580: 6f6e 5f6e 756d 6265 7294 8875 6a0f 0300  on_number..uj...
-0000c590: 006a b20c 0000 6aff 0200 006a a60e 0000  .j....j....j....
-0000c5a0: 7562 616a 0303 0000 7d94 286a 0503 0000  ubaj....}.(j....
-0000c5b0: 5d94 6a07 0300 005d 946a 0903 0000 5d94  ].j....].j....].
-0000c5c0: 6a0b 0300 005d 946a 0d03 0000 5d94 756a  j....].j....].uj
-0000c5d0: 0f03 0000 6a12 0500 006a ff02 0000 6aa3  ....j....j....j.
-0000c5e0: 0e00 0075 626a 1305 0000 2981 947d 9428  ...ubj....)..}.(
-0000c5f0: 6aeb 0200 0068 406a ec02 0000 5d94 6ab3  j....h@j....].j.
-0000c600: 0c00 0029 8194 7d94 286a eb02 0000 6840  ...)..}.(j....h@
-0000c610: 6aec 0200 005d 946a db0a 0000 2981 947d  j....].j....)..}
-0000c620: 9428 6aeb 0200 0068 406a ec02 0000 5d94  .(j....h@j....].
-0000c630: 6aff 0d00 0029 8194 7d94 286a eb02 0000  j....)..}.(j....
-0000c640: 6840 6aec 0200 005d 946a fa02 0000 8c10  h@j....].j......
-0000c650: 5374 6f70 7761 7463 682e 7368 6f77 2829  Stopwatch.show()
-0000c660: 9485 9481 947d 946a ff02 0000 6adc 0e00  .....}.j....j...
-0000c670: 0073 6261 6a03 0300 007d 9428 6a05 0300  .sbaj....}.(j...
-0000c680: 005d 946a 0703 0000 5d94 6a09 0300 005d  .].j....].j....]
-0000c690: 946a 0b03 0000 5d94 6a0d 0300 005d 9475  .j....].j....].u
-0000c6a0: 6a0f 0300 006a fe0d 0000 6aff 0200 006a  j....j....j....j
-0000c6b0: d90e 0000 7562 616a 0303 0000 7d94 286a  ....ubaj....}.(j
-0000c6c0: 0503 0000 5d94 6a07 0300 005d 946a 0903  ....].j....].j..
-0000c6d0: 0000 5d94 6a0b 0300 005d 946a 0d03 0000  ..].j....].j....
-0000c6e0: 5d94 8c08 696e 7465 726e 616c 9488 8c06  ]...internal....
-0000c6f0: 7265 6675 7269 946a 9a02 0000 8c0a 616e  refuri.j......an
-0000c700: 6368 6f72 6e61 6d65 948c 2123 636f 6f6b  chorname..!#cook
-0000c710: 6965 735f 7574 696c 6974 6965 732e 5374  ies_utilities.St
-0000c720: 6f70 7761 7463 682e 7368 6f77 9475 6a0f  opwatch.show.uj.
-0000c730: 0300 006a da0a 0000 6aff 0200 006a d60e  ...j....j....j..
-0000c740: 0000 7562 616a 0303 0000 7d94 286a 0503  ..ubaj....}.(j..
-0000c750: 0000 5d94 6a07 0300 005d 946a 0903 0000  ..].j....].j....
-0000c760: 5d94 6a0b 0300 005d 946a 0d03 0000 5d94  ].j....].j....].
-0000c770: 8c13 736b 6970 5f73 6563 7469 6f6e 5f6e  ..skip_section_n
-0000c780: 756d 6265 7294 8875 6a0f 0300 006a b20c  umber..uj....j..
-0000c790: 0000 6aff 0200 006a d30e 0000 7562 616a  ..j....j....ubaj
-0000c7a0: 0303 0000 7d94 286a 0503 0000 5d94 6a07  ....}.(j....].j.
-0000c7b0: 0300 005d 946a 0903 0000 5d94 6a0b 0300  ...].j....].j...
-0000c7c0: 005d 946a 0d03 0000 5d94 756a 0f03 0000  .].j....].uj....
-0000c7d0: 6a12 0500 006a ff02 0000 6aa3 0e00 0075  j....j....j....u
-0000c7e0: 6265 6a03 0300 007d 9428 6a05 0300 005d  bej....}.(j....]
-0000c7f0: 946a 0703 0000 5d94 6a09 0300 005d 946a  .j....].j....].j
-0000c800: 0b03 0000 5d94 6a0d 0300 005d 9475 6a0f  ....].j....].uj.
-0000c810: 0300 006a 0d05 0000 6aff 0200 006a 7c0e  ...j....j....j|.
-0000c820: 0000 7562 656a 0303 0000 7d94 286a 0503  ..ubej....}.(j..
-0000c830: 0000 5d94 6a07 0300 005d 946a 0903 0000  ..].j....].j....
-0000c840: 5d94 6a0b 0300 005d 946a 0d03 0000 5d94  ].j....].j....].
-0000c850: 756a 0f03 0000 6a12 0500 006a ff02 0000  uj....j....j....
-0000c860: 6a79 0e00 0075 6261 6a03 0300 007d 9428  jy...ubaj....}.(
-0000c870: 6a05 0300 005d 946a 0703 0000 5d94 6a09  j....].j....].j.
-0000c880: 0300 005d 946a 0b03 0000 5d94 6a0d 0300  ...].j....].j...
-0000c890: 005d 9475 6a0f 0300 006a 0d05 0000 6aff  .].uj....j....j.
-0000c8a0: 0200 006a 5c0e 0000 7562 656a 0303 0000  ...j\...ubej....
-0000c8b0: 7d94 286a 0503 0000 5d94 6a07 0300 005d  }.(j....].j....]
-0000c8c0: 946a 0903 0000 5d94 6a0b 0300 005d 946a  .j....].j....].j
-0000c8d0: 0d03 0000 5d94 756a 0f03 0000 6a12 0500  ....].uj....j...
-0000c8e0: 006a ff02 0000 6a59 0e00 0075 6261 6a03  .j....jY...ubaj.
-0000c8f0: 0300 007d 9428 6a05 0300 005d 946a 0703  ...}.(j....].j..
-0000c900: 0000 5d94 6a09 0300 005d 946a 0b03 0000  ..].j....].j....
-0000c910: 5d94 6a0d 0300 005d 9475 6a0f 0300 006a  ].j....].uj....j
-0000c920: 0d05 0000 6aff 0200 006a 3c0e 0000 7562  ....j....j<...ub
-0000c930: 656a 0303 0000 7d94 286a 0503 0000 5d94  ej....}.(j....].
-0000c940: 6a07 0300 005d 946a 0903 0000 5d94 6a0b  j....].j....].j.
-0000c950: 0300 005d 946a 0d03 0000 5d94 756a 0f03  ...].j....].uj..
-0000c960: 0000 6a12 0500 006a ff02 0000 6ab2 0d00  ..j....j....j...
-0000c970: 0075 6265 6a03 0300 007d 9428 6a05 0300  .ubej....}.(j...
-0000c980: 005d 946a 0703 0000 5d94 6a09 0300 005d  .].j....].j....]
-0000c990: 946a 0b03 0000 5d94 6a0d 0300 005d 9475  .j....].j....].u
-0000c9a0: 6a0f 0300 006a 0d05 0000 6aff 0200 006a  j....j....j....j
-0000c9b0: 960d 0000 7562 656a 0303 0000 7d94 286a  ....ubej....}.(j
-0000c9c0: 0503 0000 5d94 6a07 0300 005d 946a 0903  ....].j....].j..
-0000c9d0: 0000 5d94 6a0b 0300 005d 946a 0d03 0000  ..].j....].j....
-0000c9e0: 5d94 756a 0f03 0000 6a12 0500 006a ff02  ].uj....j....j..
-0000c9f0: 0000 6a93 0d00 0075 6261 6a03 0300 007d  ..j....ubaj....}
-0000ca00: 9428 6a05 0300 005d 946a 0703 0000 5d94  .(j....].j....].
-0000ca10: 6a09 0300 005d 946a 0b03 0000 5d94 6a0d  j....].j....].j.
-0000ca20: 0300 005d 9475 6a0f 0300 006a 0d05 0000  ...].uj....j....
-0000ca30: 7562 758c 0f74 6f63 5f6e 756d 5f65 6e74  ubu..toc_num_ent
-0000ca40: 7269 6573 947d 9428 6aca 0200 004b 016a  ries.}.(j....K.j
-0000ca50: cb02 0000 4b03 6a9a 0200 004b 0975 8c0e  ....K.j....K.u..
-0000ca60: 746f 635f 7365 636e 756d 6265 7273 947d  toc_secnumbers.}
-0000ca70: 948c 0e74 6f63 5f66 6967 6e75 6d62 6572  ...toc_fignumber
-0000ca80: 7394 7d94 8c10 746f 6374 7265 655f 696e  s.}...toctree_in
-0000ca90: 636c 7564 6573 947d 9428 6aca 0200 005d  cludes.}.(j....]
-0000caa0: 946a 310c 0000 616a cb02 0000 5d94 6a5a  .j1...aj....].jZ
-0000cab0: 0b00 0061 758c 1066 696c 6573 5f74 6f5f  ...au..files_to_
-0000cac0: 7265 6275 696c 6494 7d94 8c11 636f 6f6b  rebuild.}...cook
-0000cad0: 6965 735f 7574 696c 6974 6965 7394 8f94  ies_utilities...
-0000cae0: 286a cb02 0000 6aca 0200 0090 738c 0d67  (j....j.....s..g
-0000caf0: 6c6f 625f 746f 6374 7265 6573 948f 948c  lob_toctrees....
-0000cb00: 116e 756d 6265 7265 645f 746f 6374 7265  .numbered_toctre
-0000cb10: 6573 948f 948c 0a64 6f6d 6169 6e64 6174  es.....domaindat
-0000cb20: 6194 7d94 288c 0163 947d 9428 8c0b 726f  a.}.(..c.}.(..ro
-0000cb30: 6f74 5f73 796d 626f 6c94 6a9f 0200 008c  ot_symbol.j.....
-0000cb40: 0653 796d 626f 6c94 9394 2981 947d 9428  .Symbol...)..}.(
-0000cb50: 6aff 0200 004e 8c0c 7369 626c 696e 6741  j....N..siblingA
-0000cb60: 626f 7665 944e 8c0c 7369 626c 696e 6742  bove.N..siblingB
-0000cb70: 656c 6f77 944e 8c05 6964 656e 7494 4e8c  elow.N..ident.N.
-0000cb80: 0b64 6563 6c61 7261 7469 6f6e 944e 8c07  .declaration.N..
-0000cb90: 646f 636e 616d 6594 4e6a 0203 0000 4e8c  docname.Nj....N.
-0000cba0: 0f69 7352 6564 6563 6c61 7261 7469 6f6e  .isRedeclaration
-0000cbb0: 9489 8c09 5f63 6869 6c64 7265 6e94 5d94  ...._children.].
-0000cbc0: 8c0d 5f61 6e6f 6e43 6869 6c64 7265 6e94  .._anonChildren.
-0000cbd0: 5d94 7562 8c07 6f62 6a65 6374 7394 7d94  ].ub..objects.}.
-0000cbe0: 6a9d 0200 004b 0075 8c09 6368 616e 6765  j....K.u..change
-0000cbf0: 7365 7494 7d94 288c 0763 6861 6e67 6573  set.}.(..changes
-0000cc00: 947d 946a 9d02 0000 4b00 758c 0863 6974  .}.j....K.u..cit
-0000cc10: 6174 696f 6e94 7d94 286a 9d02 0000 4b00  ation.}.(j....K.
-0000cc20: 8c09 6369 7461 7469 6f6e 7394 7d94 8c0d  ..citations.}...
-0000cc30: 6369 7461 7469 6f6e 5f72 6566 7394 7d94  citation_refs.}.
-0000cc40: 758c 0363 7070 947d 9428 6a4c 0f00 006a  u..cpp.}.(jL...j
-0000cc50: a202 0000 6a4d 0f00 0093 9429 8194 7d94  ....jM.....)..}.
-0000cc60: 286a ff02 0000 4e6a 510f 0000 4e6a 520f  (j....NjQ...NjR.
-0000cc70: 0000 4e8c 0969 6465 6e74 4f72 4f70 944e  ..N..identOrOp.N
-0000cc80: 8c0e 7465 6d70 6c61 7465 5061 7261 6d73  ..templateParams
-0000cc90: 944e 8c0c 7465 6d70 6c61 7465 4172 6773  .N..templateArgs
-0000cca0: 944e 6a54 0f00 004e 6a55 0f00 004e 6a02  .NjT...NjU...Nj.
-0000ccb0: 0300 004e 6a56 0f00 0089 6a57 0f00 005d  ...NjV....jW...]
-0000ccc0: 946a 590f 0000 5d94 7562 8c05 6e61 6d65  .jY...].ub..name
-0000ccd0: 7394 7d94 6a9d 0200 004b 0075 8c05 696e  s.}.j....K.u..in
-0000cce0: 6465 7894 7d94 286a 9d02 0000 4b00 8c07  dex.}.(j....K...
-0000ccf0: 656e 7472 6965 7394 7d94 286a ca02 0000  entries.}.(j....
-0000cd00: 5d94 6acb 0200 005d 946a 9a02 0000 5d94  ].j....].j....].
-0000cd10: 286a 4203 0000 6afa 0700 006a 6708 0000  (jB...j....jg...
-0000cd20: 6a62 0900 0065 7575 8c02 6a73 947d 9428  jb...euu..js.}.(
-0000cd30: 6a5b 0f00 007d 948c 076d 6f64 756c 6573  j[...}...modules
-0000cd40: 947d 946a 9d02 0000 4b00 758c 046d 6174  .}.j....K.u..mat
-0000cd50: 6894 7d94 286a 5b0f 0000 7d94 8c0d 6861  h.}.(j[...}...ha
-0000cd60: 735f 6571 7561 7469 6f6e 7394 7d94 286a  s_equations.}.(j
-0000cd70: ca02 0000 896a cb02 0000 896a 9a02 0000  .....j.....j....
-0000cd80: 8975 6a9d 0200 004b 0075 8c02 7079 947d  .uj....K.u..py.}
-0000cd90: 9428 6a5b 0f00 007d 9428 8c1b 636f 6f6b  .(j[...}.(..cook
-0000cda0: 6965 735f 7574 696c 6974 6965 732e 6765  ies_utilities.ge
-0000cdb0: 745f 6461 7465 7394 8c15 7370 6869 6e78  t_dates...sphinx
-0000cdc0: 2e64 6f6d 6169 6e73 2e70 7974 686f 6e94  .domains.python.
-0000cdd0: 8c0b 4f62 6a65 6374 456e 7472 7994 9394  ..ObjectEntry...
-0000cde0: 286a 9a02 0000 6a41 0300 006a 8707 0000  (j....jA...j....
-0000cdf0: 8974 9481 948c 1b63 6f6f 6b69 6573 5f75  .t.....cookies_u
-0000ce00: 7469 6c69 7469 6573 2e53 746f 7077 6174  tilities.Stopwat
-0000ce10: 6368 946a 8a0f 0000 286a 9a02 0000 6af9  ch.j....(j....j.
-0000ce20: 0700 006a b909 0000 8974 9481 948c 2563  ...j.....t....%c
-0000ce30: 6f6f 6b69 6573 5f75 7469 6c69 7469 6573  ookies_utilities
-0000ce40: 2e73 746f 7077 6174 6368 2e53 746f 7077  .stopwatch.Stopw
-0000ce50: 6174 6368 946a 8a0f 0000 286a 9a02 0000  atch.j....(j....
-0000ce60: 6af9 0700 006a b909 0000 8874 9481 948c  j....j.....t....
-0000ce70: 2163 6f6f 6b69 6573 5f75 7469 6c69 7469  !cookies_utiliti
-0000ce80: 6573 2e53 746f 7077 6174 6368 2e70 7265  es.Stopwatch.pre
-0000ce90: 7373 946a 8a0f 0000 286a 9a02 0000 6a66  ss.j....(j....jf
-0000cea0: 0800 006a 5109 0000 8974 9481 948c 2063  ...jQ....t.... c
-0000ceb0: 6f6f 6b69 6573 5f75 7469 6c69 7469 6573  ookies_utilities
-0000cec0: 2e53 746f 7077 6174 6368 2e73 686f 7794  .Stopwatch.show.
-0000ced0: 6a8a 0f00 0028 6a9a 0200 006a 6109 0000  j....(j....ja...
-0000cee0: 6aab 0900 0089 7494 8194 756a 7d0f 0000  j.....t...uj}...
-0000cef0: 7d94 6a9d 0200 004b 0075 8c03 7273 7494  }.j....K.u..rst.
-0000cf00: 7d94 286a 5b0f 0000 7d94 6a9d 0200 004b  }.(j[...}.j....K
-0000cf10: 0075 8c03 7374 6494 7d94 288c 0b70 726f  .u..std.}.(..pro
-0000cf20: 676f 7074 696f 6e73 947d 946a 5b0f 0000  goptions.}.j[...
-0000cf30: 7d94 8c06 6c61 6265 6c73 947d 9428 8c08  }...labels.}.(..
-0000cf40: 6765 6e69 6e64 6578 946a a40f 0000 6840  genindex.j....h@
-0000cf50: 8c0d 7370 6869 6e78 2e6c 6f63 616c 6594  ..sphinx.locale.
-0000cf60: 8c11 5f54 7261 6e73 6c61 7469 6f6e 5072  .._TranslationPr
-0000cf70: 6f78 7994 9394 2981 948c 0673 7068 696e  oxy...)....sphin
-0000cf80: 7894 8c07 6765 6e65 7261 6c94 8c05 496e  x...general...In
-0000cf90: 6465 7894 8794 6287 948c 086d 6f64 696e  dex...b....modin
-0000cfa0: 6465 7894 8c0b 7079 2d6d 6f64 696e 6465  dex...py-modinde
-0000cfb0: 7894 6840 6aa7 0f00 0029 8194 6aa9 0f00  x.h@j....)..j...
-0000cfc0: 006a aa0f 0000 8c0c 4d6f 6475 6c65 2049  .j......Module I
-0000cfd0: 6e64 6578 9487 9462 8794 8c06 7365 6172  ndex...b....sear
-0000cfe0: 6368 946a b40f 0000 6840 6aa7 0f00 0029  ch.j....h@j....)
-0000cff0: 8194 6aa9 0f00 006a aa0f 0000 8c0b 5365  ..j....j......Se
-0000d000: 6172 6368 2050 6167 6594 8794 6287 948c  arch Page...b...
-0000d010: 0b70 792d 6d6f 6469 6e64 6578 948c 0b70  .py-modindex...p
-0000d020: 792d 6d6f 6469 6e64 6578 9468 408c 1350  y-modindex.h@..P
-0000d030: 7974 686f 6e20 4d6f 6475 6c65 2049 6e64  ython Module Ind
-0000d040: 6578 9487 9475 8c0a 616e 6f6e 6c61 6265  ex...u..anonlabe
-0000d050: 6c73 947d 9428 6aa4 0f00 006a a40f 0000  ls.}.(j....j....
-0000d060: 6840 8694 6aae 0f00 006a af0f 0000 6840  h@..j....j....h@
-0000d070: 8694 6ab4 0f00 006a b40f 0000 6840 8694  ..j....j....h@..
-0000d080: 6ab9 0f00 006a ba0f 0000 6840 8694 756a  j....j....h@..uj
-0000d090: 9d02 0000 4b00 8c05 7465 726d 7394 7d94  ....K...terms.}.
-0000d0a0: 7575 8c06 696d 6167 6573 948c 0b73 7068  uu..images...sph
-0000d0b0: 696e 782e 7574 696c 948c 1046 696c 656e  inx.util...Filen
-0000d0c0: 616d 6555 6e69 7144 6963 7494 9394 2981  ameUniqDict...).
-0000d0d0: 948f 9462 8c07 646c 6669 6c65 7394 6ac6  ...b..dlfiles.j.
-0000d0e0: 0f00 008c 0d44 6f77 6e6c 6f61 6446 696c  .....DownloadFil
-0000d0f0: 6573 9493 9429 8194 8c12 6f72 6967 696e  es...)....origin
-0000d100: 616c 5f69 6d61 6765 5f75 7269 947d 948c  al_image_uri.}..
-0000d110: 0974 656d 705f 6461 7461 947d 948c 0b72  .temp_data.}...r
-0000d120: 6566 5f63 6f6e 7465 7874 947d 948c 145f  ef_context.}..._
-0000d130: 7365 6172 6368 5f69 6e64 6578 5f74 6974  search_index_tit
-0000d140: 6c65 7394 7d94 8c17 5f73 6561 7263 685f  les.}..._search_
-0000d150: 696e 6465 785f 6669 6c65 6e61 6d65 7394  index_filenames.
-0000d160: 7d94 8c15 5f73 6561 7263 685f 696e 6465  }..._search_inde
-0000d170: 785f 6d61 7070 696e 6794 7d94 8c1b 5f73  x_mapping.}..._s
-0000d180: 6561 7263 685f 696e 6465 785f 7469 746c  earch_index_titl
-0000d190: 655f 6d61 7070 696e 6794 7d94 8c18 5f73  e_mapping.}..._s
-0000d1a0: 6561 7263 685f 696e 6465 785f 616c 6c5f  earch_index_all_
-0000d1b0: 7469 746c 6573 947d 948c 1b5f 7365 6172  titles.}..._sear
-0000d1c0: 6368 5f69 6e64 6578 5f69 6e64 6578 5f65  ch_index_index_e
-0000d1d0: 6e74 7269 6573 947d 948c 165f 7365 6172  ntries.}..._sear
-0000d1e0: 6368 5f69 6e64 6578 5f6f 626a 7479 7065  ch_index_objtype
-0000d1f0: 7394 7d94 8c16 5f73 6561 7263 685f 696e  s.}..._search_in
-0000d200: 6465 785f 6f62 6a6e 616d 6573 947d 9475  dex_objnames.}.u
-0000d210: 622e                                     b.
+00002900: 6b73 273a 2030 7d2c 2067 656e 6974 6572  ks': 0}, geniter
+00002910: 3d46 616c 7365 2c20 6361 7374 5f73 7472  =False, cast_str
+00002920: 3d54 7275 652c 2066 6f72 6d61 745f 6f75  =True, format_ou
+00002930: 743d 4e6f 6e65 2994 6aec 0200 005d 9428  t=None).j....].(
+00002940: 6ae6 0200 008c 0c64 6573 635f 6164 646e  j......desc_addn
+00002950: 616d 6594 9394 2981 947d 9428 6aeb 0200  ame...)..}.(j...
+00002960: 008c 1263 6f6f 6b69 6573 5f75 7469 6c69  ...cookies_utili
+00002970: 7469 6573 2e94 6aec 0200 005d 946a fa02  ties..j....].j..
+00002980: 0000 8c12 636f 6f6b 6965 735f 7574 696c  ....cookies_util
+00002990: 6974 6965 732e 9485 9481 947d 9428 6aff  ities......}.(j.
+000029a0: 0200 006a 5003 0000 6a00 0300 006a e902  ...jP...j....j..
+000029b0: 0000 6a01 0300 004e 6a02 0300 004e 7562  ..j....Nj....Nub
+000029c0: 616a 0303 0000 7d94 286a 0503 0000 5d94  aj....}.(j....].
+000029d0: 6a07 0300 005d 9428 8c0b 7369 672d 7072  j....].(..sig-pr
+000029e0: 656e 616d 6594 8c0d 6465 7363 636c 6173  ename...descclas
+000029f0: 736e 616d 6594 656a 0903 0000 5d94 6a0b  sname.ej....].j.
+00002a00: 0300 005d 946a 0d03 0000 5d94 8c09 786d  ...].j....]...xm
+00002a10: 6c3a 7370 6163 6594 8c08 7072 6573 6572  l:space...preser
+00002a20: 7665 9475 6a0f 0300 006a 4e03 0000 6aff  ve.uj....jN...j.
+00002a30: 0200 006a 4a03 0000 6a00 0300 006a e902  ...jJ...j....j..
+00002a40: 0000 6a01 0300 008c 7143 3a5c 5573 6572  ..j.....qC:\User
+00002a50: 735c 632d 6d69 685c 7370 6163 655c 636f  s\c-mih\space\co
+00002a60: 6f6b 6965 735f 7574 696c 6974 6965 735c  okies_utilities\
+00002a70: 7372 635c 636f 6f6b 6965 735f 7574 696c  src\cookies_util
+00002a80: 6974 6965 735c 5f5f 696e 6974 5f5f 2e70  ities\__init__.p
+00002a90: 793a 646f 6373 7472 696e 6720 6f66 2063  y:docstring of c
+00002aa0: 6f6f 6b69 6573 5f75 7469 6c69 7469 6573  ookies_utilities
+00002ab0: 2e67 6574 5f64 6174 6573 946a 0203 0000  .get_dates.j....
+00002ac0: 4b01 7562 6ae6 0200 008c 0964 6573 635f  K.ubj......desc_
+00002ad0: 6e61 6d65 9493 9429 8194 7d94 286a eb02  name...)..}.(j..
+00002ae0: 0000 8c09 6765 745f 6461 7465 7394 6aec  ....get_dates.j.
+00002af0: 0200 005d 946a fa02 0000 8c09 6765 745f  ...].j......get_
+00002b00: 6461 7465 7394 8594 8194 7d94 286a ff02  dates.....}.(j..
+00002b10: 0000 6a65 0300 006a 0003 0000 6ae9 0200  ..je...j....j...
+00002b20: 006a 0103 0000 4e6a 0203 0000 4e75 6261  .j....Nj....Nuba
+00002b30: 6a03 0300 007d 9428 6a05 0300 005d 946a  j....}.(j....].j
+00002b40: 0703 0000 5d94 288c 0873 6967 2d6e 616d  ....].(..sig-nam
+00002b50: 6594 8c08 6465 7363 6e61 6d65 9465 6a09  e...descname.ej.
+00002b60: 0300 005d 946a 0b03 0000 5d94 6a0d 0300  ...].j....].j...
+00002b70: 005d 946a 6003 0000 6a61 0300 0075 6a0f  .].j`...ja...uj.
+00002b80: 0300 006a 6303 0000 6aff 0200 006a 4a03  ...jc...j....jJ.
+00002b90: 0000 6a00 0300 006a e902 0000 6a01 0300  ..j....j....j...
+00002ba0: 006a 6203 0000 6a02 0300 004b 0175 626a  .jb...j....K.ubj
+00002bb0: e602 0000 8c12 6465 7363 5f70 6172 616d  ......desc_param
+00002bc0: 6574 6572 6c69 7374 9493 9429 8194 7d94  eterlist...)..}.
+00002bd0: 286a eb02 0000 8cba 7374 6172 743d 2732  (j......start='2
+00002be0: 3031 362d 3037 2d30 3120 3032 3a30 303a  016-07-01 02:00:
+00002bf0: 3030 272c 2065 6e64 3d27 3230 3136 2d30  00', end='2016-0
+00002c00: 372d 3032 2030 313a 3030 3a30 3027 2c20  7-02 01:00:00', 
+00002c10: 666f 726d 6174 3d27 2559 2d25 6d2d 2564  format='%Y-%m-%d
+00002c20: 2025 483a 254d 3a25 5327 2c20 6465 6c74   %H:%M:%S', delt
+00002c30: 613d 7b27 6461 7973 273a 2030 2c20 2768  a={'days': 0, 'h
+00002c40: 6f75 7273 273a 2031 2c20 276d 696e 7574  ours': 1, 'minut
+00002c50: 6573 273a 2030 2c20 2777 6565 6b73 273a  es': 0, 'weeks':
+00002c60: 2030 7d2c 2067 656e 6974 6572 3d46 616c   0}, geniter=Fal
+00002c70: 7365 2c20 6361 7374 5f73 7472 3d54 7275  se, cast_str=Tru
+00002c80: 652c 2066 6f72 6d61 745f 6f75 743d 4e6f  e, format_out=No
+00002c90: 6e65 946a ec02 0000 5d94 286a e602 0000  ne.j....].(j....
+00002ca0: 8c0e 6465 7363 5f70 6172 616d 6574 6572  ..desc_parameter
+00002cb0: 9493 9429 8194 7d94 286a eb02 0000 8c1b  ...)..}.(j......
+00002cc0: 7374 6172 743d 2732 3031 362d 3037 2d30  start='2016-07-0
+00002cd0: 3120 3032 3a30 303a 3030 2794 6aec 0200  1 02:00:00'.j...
+00002ce0: 005d 9428 6ae6 0200 008c 0d64 6573 635f  .].(j......desc_
+00002cf0: 7369 675f 6e61 6d65 9493 9429 8194 7d94  sig_name...)..}.
+00002d00: 286a eb02 0000 8c05 7374 6172 7494 6aec  (j......start.j.
+00002d10: 0200 005d 946a fa02 0000 8c05 7374 6172  ...].j......star
+00002d20: 7494 8594 8194 7d94 286a ff02 0000 6a83  t.....}.(j....j.
+00002d30: 0300 006a 0003 0000 6ae9 0200 006a 0103  ...j....j....j..
+00002d40: 0000 4e6a 0203 0000 4e75 6261 6a03 0300  ..Nj....Nubaj...
+00002d50: 007d 9428 6a05 0300 005d 946a 0703 0000  .}.(j....].j....
+00002d60: 5d94 8c01 6e94 616a 0903 0000 5d94 6a0b  ]...n.aj....].j.
+00002d70: 0300 005d 946a 0d03 0000 5d94 756a 0f03  ...].j....].uj..
+00002d80: 0000 6a81 0300 006a ff02 0000 6a7d 0300  ..j....j....j}..
+00002d90: 0075 626a e602 0000 8c11 6465 7363 5f73  .ubj......desc_s
+00002da0: 6967 5f6f 7065 7261 746f 7294 9394 2981  ig_operator...).
+00002db0: 947d 9428 6aeb 0200 008c 013d 946a ec02  .}.(j......=.j..
+00002dc0: 0000 5d94 6afa 0200 008c 013d 9485 9481  ..].j......=....
+00002dd0: 947d 9428 6aff 0200 006a 9403 0000 6a00  .}.(j....j....j.
+00002de0: 0300 006a e902 0000 6a01 0300 004e 6a02  ...j....j....Nj.
+00002df0: 0300 004e 7562 616a 0303 0000 7d94 286a  ...Nubaj....}.(j
+00002e00: 0503 0000 5d94 6a07 0300 005d 948c 016f  ....].j....]...o
+00002e10: 9461 6a09 0300 005d 946a 0b03 0000 5d94  .aj....].j....].
+00002e20: 6a0d 0300 005d 9475 6a0f 0300 006a 9203  j....].uj....j..
+00002e30: 0000 6aff 0200 006a 7d03 0000 7562 6aee  ..j....j}...ubj.
+00002e40: 0200 0068 fa93 9429 8194 7d94 286a eb02  ...h...)..}.(j..
+00002e50: 0000 8c15 2732 3031 362d 3037 2d30 3120  ....'2016-07-01 
+00002e60: 3032 3a30 303a 3030 2794 6aec 0200 005d  02:00:00'.j....]
+00002e70: 946a fa02 0000 8c15 2732 3031 362d 3037  .j......'2016-07
+00002e80: 2d30 3120 3032 3a30 303a 3030 2794 8594  -01 02:00:00'...
+00002e90: 8194 7d94 286a ff02 0000 6aa4 0300 006a  ..}.(j....j....j
+00002ea0: 0003 0000 6ae9 0200 006a 0103 0000 4e6a  ....j....j....Nj
+00002eb0: 0203 0000 4e75 6261 6a03 0300 007d 9428  ....Nubaj....}.(
+00002ec0: 6a05 0300 005d 946a 0703 0000 5d94 8c0d  j....].j....]...
+00002ed0: 6465 6661 756c 745f 7661 6c75 6594 616a  default_value.aj
+00002ee0: 0903 0000 5d94 6a0b 0300 005d 946a 0d03  ....].j....].j..
+00002ef0: 0000 5d94 8c13 7375 7070 6f72 745f 736d  ..]...support_sm
+00002f00: 6172 7471 756f 7465 7394 8975 6a0f 0300  artquotes..uj...
+00002f10: 0068 fa6a ff02 0000 6a7d 0300 0075 6265  .h.j....j}...ube
+00002f20: 6a03 0300 007d 9428 6a05 0300 005d 946a  j....}.(j....].j
+00002f30: 0703 0000 5d94 6a09 0300 005d 946a 0b03  ....].j....].j..
+00002f40: 0000 5d94 6a0d 0300 005d 946a 6003 0000  ..].j....].j`...
+00002f50: 6a61 0300 0075 6a0f 0300 006a 7b03 0000  ja...uj....j{...
+00002f60: 6aff 0200 006a 7703 0000 7562 6a7c 0300  j....jw...ubj|..
+00002f70: 0029 8194 7d94 286a eb02 0000 8c19 656e  .)..}.(j......en
+00002f80: 643d 2732 3031 362d 3037 2d30 3220 3031  d='2016-07-02 01
+00002f90: 3a30 303a 3030 2794 6aec 0200 005d 9428  :00:00'.j....].(
+00002fa0: 6a82 0300 0029 8194 7d94 286a eb02 0000  j....)..}.(j....
+00002fb0: 8c03 656e 6494 6aec 0200 005d 946a fa02  ..end.j....].j..
+00002fc0: 0000 8c03 656e 6494 8594 8194 7d94 286a  ....end.....}.(j
+00002fd0: ff02 0000 6abe 0300 006a 0003 0000 6ae9  ....j....j....j.
+00002fe0: 0200 006a 0103 0000 4e6a 0203 0000 4e75  ...j....Nj....Nu
+00002ff0: 6261 6a03 0300 007d 9428 6a05 0300 005d  baj....}.(j....]
+00003000: 946a 0703 0000 5d94 6a8e 0300 0061 6a09  .j....].j....aj.
+00003010: 0300 005d 946a 0b03 0000 5d94 6a0d 0300  ...].j....].j...
+00003020: 005d 9475 6a0f 0300 006a 8103 0000 6aff  .].uj....j....j.
+00003030: 0200 006a ba03 0000 7562 6a93 0300 0029  ...j....ubj....)
+00003040: 8194 7d94 286a eb02 0000 8c01 3d94 6aec  ..}.(j......=.j.
+00003050: 0200 005d 946a fa02 0000 8c01 3d94 8594  ...].j......=...
+00003060: 8194 7d94 286a ff02 0000 6acc 0300 006a  ..}.(j....j....j
+00003070: 0003 0000 6ae9 0200 006a 0103 0000 4e6a  ....j....j....Nj
+00003080: 0203 0000 4e75 6261 6a03 0300 007d 9428  ....Nubaj....}.(
+00003090: 6a05 0300 005d 946a 0703 0000 5d94 6a9f  j....].j....].j.
+000030a0: 0300 0061 6a09 0300 005d 946a 0b03 0000  ...aj....].j....
+000030b0: 5d94 6a0d 0300 005d 9475 6a0f 0300 006a  ].j....].uj....j
+000030c0: 9203 0000 6aff 0200 006a ba03 0000 7562  ....j....j....ub
+000030d0: 6aa3 0300 0029 8194 7d94 286a eb02 0000  j....)..}.(j....
+000030e0: 8c15 2732 3031 362d 3037 2d30 3220 3031  ..'2016-07-02 01
+000030f0: 3a30 303a 3030 2794 6aec 0200 005d 946a  :00:00'.j....].j
+00003100: fa02 0000 8c15 2732 3031 362d 3037 2d30  ......'2016-07-0
+00003110: 3220 3031 3a30 303a 3030 2794 8594 8194  2 01:00:00'.....
+00003120: 7d94 286a ff02 0000 6ada 0300 006a 0003  }.(j....j....j..
+00003130: 0000 6ae9 0200 006a 0103 0000 4e6a 0203  ..j....j....Nj..
+00003140: 0000 4e75 6261 6a03 0300 007d 9428 6a05  ..Nubaj....}.(j.
+00003150: 0300 005d 946a 0703 0000 5d94 6aaf 0300  ...].j....].j...
+00003160: 0061 6a09 0300 005d 946a 0b03 0000 5d94  .aj....].j....].
+00003170: 6a0d 0300 005d 948c 1373 7570 706f 7274  j....]...support
+00003180: 5f73 6d61 7274 7175 6f74 6573 9489 756a  _smartquotes..uj
+00003190: 0f03 0000 68fa 6aff 0200 006a ba03 0000  ....h.j....j....
+000031a0: 7562 656a 0303 0000 7d94 286a 0503 0000  ubej....}.(j....
+000031b0: 5d94 6a07 0300 005d 946a 0903 0000 5d94  ].j....].j....].
+000031c0: 6a0b 0300 005d 946a 0d03 0000 5d94 6a60  j....].j....].j`
+000031d0: 0300 006a 6103 0000 756a 0f03 0000 6a7b  ...ja...uj....j{
+000031e0: 0300 006a ff02 0000 6a77 0300 0075 626a  ...j....jw...ubj
+000031f0: 7c03 0000 2981 947d 9428 6aeb 0200 008c  |...)..}.(j.....
+00003200: 1a66 6f72 6d61 743d 2725 592d 256d 2d25  .format='%Y-%m-%
+00003210: 6420 2548 3a25 4d3a 2553 2794 6aec 0200  d %H:%M:%S'.j...
+00003220: 005d 9428 6a82 0300 0029 8194 7d94 286a  .].(j....)..}.(j
+00003230: eb02 0000 8c06 666f 726d 6174 946a ec02  ......format.j..
+00003240: 0000 5d94 6afa 0200 008c 0666 6f72 6d61  ..].j......forma
+00003250: 7494 8594 8194 7d94 286a ff02 0000 6af3  t.....}.(j....j.
+00003260: 0300 006a 0003 0000 6ae9 0200 006a 0103  ...j....j....j..
+00003270: 0000 4e6a 0203 0000 4e75 6261 6a03 0300  ..Nj....Nubaj...
+00003280: 007d 9428 6a05 0300 005d 946a 0703 0000  .}.(j....].j....
+00003290: 5d94 6a8e 0300 0061 6a09 0300 005d 946a  ].j....aj....].j
+000032a0: 0b03 0000 5d94 6a0d 0300 005d 9475 6a0f  ....].j....].uj.
+000032b0: 0300 006a 8103 0000 6aff 0200 006a ef03  ...j....j....j..
+000032c0: 0000 7562 6a93 0300 0029 8194 7d94 286a  ..ubj....)..}.(j
+000032d0: eb02 0000 8c01 3d94 6aec 0200 005d 946a  ......=.j....].j
+000032e0: fa02 0000 8c01 3d94 8594 8194 7d94 286a  ......=.....}.(j
+000032f0: ff02 0000 6a01 0400 006a 0003 0000 6ae9  ....j....j....j.
+00003300: 0200 006a 0103 0000 4e6a 0203 0000 4e75  ...j....Nj....Nu
+00003310: 6261 6a03 0300 007d 9428 6a05 0300 005d  baj....}.(j....]
+00003320: 946a 0703 0000 5d94 6a9f 0300 0061 6a09  .j....].j....aj.
+00003330: 0300 005d 946a 0b03 0000 5d94 6a0d 0300  ...].j....].j...
+00003340: 005d 9475 6a0f 0300 006a 9203 0000 6aff  .].uj....j....j.
+00003350: 0200 006a ef03 0000 7562 6aa3 0300 0029  ...j....ubj....)
+00003360: 8194 7d94 286a eb02 0000 8c13 2725 592d  ..}.(j......'%Y-
+00003370: 256d 2d25 6420 2548 3a25 4d3a 2553 2794  %m-%d %H:%M:%S'.
+00003380: 6aec 0200 005d 946a fa02 0000 8c13 2725  j....].j......'%
+00003390: 592d 256d 2d25 6420 2548 3a25 4d3a 2553  Y-%m-%d %H:%M:%S
+000033a0: 2794 8594 8194 7d94 286a ff02 0000 6a0f  '.....}.(j....j.
+000033b0: 0400 006a 0003 0000 6ae9 0200 006a 0103  ...j....j....j..
+000033c0: 0000 4e6a 0203 0000 4e75 6261 6a03 0300  ..Nj....Nubaj...
+000033d0: 007d 9428 6a05 0300 005d 946a 0703 0000  .}.(j....].j....
+000033e0: 5d94 6aaf 0300 0061 6a09 0300 005d 946a  ].j....aj....].j
+000033f0: 0b03 0000 5d94 6a0d 0300 005d 948c 1373  ....].j....]...s
+00003400: 7570 706f 7274 5f73 6d61 7274 7175 6f74  upport_smartquot
+00003410: 6573 9489 756a 0f03 0000 68fa 6aff 0200  es..uj....h.j...
+00003420: 006a ef03 0000 7562 656a 0303 0000 7d94  .j....ubej....}.
+00003430: 286a 0503 0000 5d94 6a07 0300 005d 946a  (j....].j....].j
+00003440: 0903 0000 5d94 6a0b 0300 005d 946a 0d03  ....].j....].j..
+00003450: 0000 5d94 6a60 0300 006a 6103 0000 756a  ..].j`...ja...uj
+00003460: 0f03 0000 6a7b 0300 006a ff02 0000 6a77  ....j{...j....jw
+00003470: 0300 0075 626a 7c03 0000 2981 947d 9428  ...ubj|...)..}.(
+00003480: 6aeb 0200 008c 3764 656c 7461 3d7b 2764  j.....7delta={'d
+00003490: 6179 7327 3a20 302c 2027 686f 7572 7327  ays': 0, 'hours'
+000034a0: 3a20 312c 2027 6d69 6e75 7465 7327 3a20  : 1, 'minutes': 
+000034b0: 302c 2027 7765 656b 7327 3a20 307d 946a  0, 'weeks': 0}.j
+000034c0: ec02 0000 5d94 286a 8203 0000 2981 947d  ....].(j....)..}
+000034d0: 9428 6aeb 0200 008c 0564 656c 7461 946a  .(j......delta.j
+000034e0: ec02 0000 5d94 6afa 0200 008c 0564 656c  ....].j......del
+000034f0: 7461 9485 9481 947d 9428 6aff 0200 006a  ta.....}.(j....j
+00003500: 2804 0000 6a00 0300 006a e902 0000 6a01  (...j....j....j.
+00003510: 0300 004e 6a02 0300 004e 7562 616a 0303  ...Nj....Nubaj..
+00003520: 0000 7d94 286a 0503 0000 5d94 6a07 0300  ..}.(j....].j...
+00003530: 005d 946a 8e03 0000 616a 0903 0000 5d94  .].j....aj....].
+00003540: 6a0b 0300 005d 946a 0d03 0000 5d94 756a  j....].j....].uj
+00003550: 0f03 0000 6a81 0300 006a ff02 0000 6a24  ....j....j....j$
+00003560: 0400 0075 626a 9303 0000 2981 947d 9428  ...ubj....)..}.(
+00003570: 6aeb 0200 008c 013d 946a ec02 0000 5d94  j......=.j....].
+00003580: 6afa 0200 008c 013d 9485 9481 947d 9428  j......=.....}.(
+00003590: 6aff 0200 006a 3604 0000 6a00 0300 006a  j....j6...j....j
+000035a0: e902 0000 6a01 0300 004e 6a02 0300 004e  ....j....Nj....N
+000035b0: 7562 616a 0303 0000 7d94 286a 0503 0000  ubaj....}.(j....
+000035c0: 5d94 6a07 0300 005d 946a 9f03 0000 616a  ].j....].j....aj
+000035d0: 0903 0000 5d94 6a0b 0300 005d 946a 0d03  ....].j....].j..
+000035e0: 0000 5d94 756a 0f03 0000 6a92 0300 006a  ..].uj....j....j
+000035f0: ff02 0000 6a24 0400 0075 626a a303 0000  ....j$...ubj....
+00003600: 2981 947d 9428 6aeb 0200 008c 317b 2764  )..}.(j.....1{'d
+00003610: 6179 7327 3a20 302c 2027 686f 7572 7327  ays': 0, 'hours'
+00003620: 3a20 312c 2027 6d69 6e75 7465 7327 3a20  : 1, 'minutes': 
+00003630: 302c 2027 7765 656b 7327 3a20 307d 946a  0, 'weeks': 0}.j
+00003640: ec02 0000 5d94 6afa 0200 008c 317b 2764  ....].j.....1{'d
+00003650: 6179 7327 3a20 302c 2027 686f 7572 7327  ays': 0, 'hours'
+00003660: 3a20 312c 2027 6d69 6e75 7465 7327 3a20  : 1, 'minutes': 
+00003670: 302c 2027 7765 656b 7327 3a20 307d 9485  0, 'weeks': 0}..
+00003680: 9481 947d 9428 6aff 0200 006a 4404 0000  ...}.(j....jD...
+00003690: 6a00 0300 006a e902 0000 6a01 0300 004e  j....j....j....N
+000036a0: 6a02 0300 004e 7562 616a 0303 0000 7d94  j....Nubaj....}.
+000036b0: 286a 0503 0000 5d94 6a07 0300 005d 946a  (j....].j....].j
+000036c0: af03 0000 616a 0903 0000 5d94 6a0b 0300  ....aj....].j...
+000036d0: 005d 946a 0d03 0000 5d94 8c13 7375 7070  .].j....]...supp
+000036e0: 6f72 745f 736d 6172 7471 756f 7465 7394  ort_smartquotes.
+000036f0: 8975 6a0f 0300 0068 fa6a ff02 0000 6a24  .uj....h.j....j$
+00003700: 0400 0075 6265 6a03 0300 007d 9428 6a05  ...ubej....}.(j.
+00003710: 0300 005d 946a 0703 0000 5d94 6a09 0300  ...].j....].j...
+00003720: 005d 946a 0b03 0000 5d94 6a0d 0300 005d  .].j....].j....]
+00003730: 946a 6003 0000 6a61 0300 0075 6a0f 0300  .j`...ja...uj...
+00003740: 006a 7b03 0000 6aff 0200 006a 7703 0000  .j{...j....jw...
+00003750: 7562 6a7c 0300 0029 8194 7d94 286a eb02  ubj|...)..}.(j..
+00003760: 0000 8c0d 6765 6e69 7465 723d 4661 6c73  ....geniter=Fals
+00003770: 6594 6aec 0200 005d 9428 6a82 0300 0029  e.j....].(j....)
+00003780: 8194 7d94 286a eb02 0000 8c07 6765 6e69  ..}.(j......geni
+00003790: 7465 7294 6aec 0200 005d 946a fa02 0000  ter.j....].j....
+000037a0: 8c07 6765 6e69 7465 7294 8594 8194 7d94  ..geniter.....}.
+000037b0: 286a ff02 0000 6a5d 0400 006a 0003 0000  (j....j]...j....
+000037c0: 6ae9 0200 006a 0103 0000 4e6a 0203 0000  j....j....Nj....
+000037d0: 4e75 6261 6a03 0300 007d 9428 6a05 0300  Nubaj....}.(j...
+000037e0: 005d 946a 0703 0000 5d94 6a8e 0300 0061  .].j....].j....a
+000037f0: 6a09 0300 005d 946a 0b03 0000 5d94 6a0d  j....].j....].j.
+00003800: 0300 005d 9475 6a0f 0300 006a 8103 0000  ...].uj....j....
+00003810: 6aff 0200 006a 5904 0000 7562 6a93 0300  j....jY...ubj...
+00003820: 0029 8194 7d94 286a eb02 0000 8c01 3d94  .)..}.(j......=.
+00003830: 6aec 0200 005d 946a fa02 0000 8c01 3d94  j....].j......=.
+00003840: 8594 8194 7d94 286a ff02 0000 6a6b 0400  ....}.(j....jk..
+00003850: 006a 0003 0000 6ae9 0200 006a 0103 0000  .j....j....j....
+00003860: 4e6a 0203 0000 4e75 6261 6a03 0300 007d  Nj....Nubaj....}
+00003870: 9428 6a05 0300 005d 946a 0703 0000 5d94  .(j....].j....].
+00003880: 6a9f 0300 0061 6a09 0300 005d 946a 0b03  j....aj....].j..
+00003890: 0000 5d94 6a0d 0300 005d 9475 6a0f 0300  ..].j....].uj...
+000038a0: 006a 9203 0000 6aff 0200 006a 5904 0000  .j....j....jY...
+000038b0: 7562 6aa3 0300 0029 8194 7d94 286a eb02  ubj....)..}.(j..
+000038c0: 0000 8c05 4661 6c73 6594 6aec 0200 005d  ....False.j....]
+000038d0: 946a fa02 0000 8c05 4661 6c73 6594 8594  .j......False...
+000038e0: 8194 7d94 286a ff02 0000 6a79 0400 006a  ..}.(j....jy...j
+000038f0: 0003 0000 6ae9 0200 006a 0103 0000 4e6a  ....j....j....Nj
+00003900: 0203 0000 4e75 6261 6a03 0300 007d 9428  ....Nubaj....}.(
+00003910: 6a05 0300 005d 946a 0703 0000 5d94 6aaf  j....].j....].j.
+00003920: 0300 0061 6a09 0300 005d 946a 0b03 0000  ...aj....].j....
+00003930: 5d94 6a0d 0300 005d 948c 1373 7570 706f  ].j....]...suppo
+00003940: 7274 5f73 6d61 7274 7175 6f74 6573 9489  rt_smartquotes..
+00003950: 756a 0f03 0000 68fa 6aff 0200 006a 5904  uj....h.j....jY.
+00003960: 0000 7562 656a 0303 0000 7d94 286a 0503  ..ubej....}.(j..
+00003970: 0000 5d94 6a07 0300 005d 946a 0903 0000  ..].j....].j....
+00003980: 5d94 6a0b 0300 005d 946a 0d03 0000 5d94  ].j....].j....].
+00003990: 6a60 0300 006a 6103 0000 756a 0f03 0000  j`...ja...uj....
+000039a0: 6a7b 0300 006a ff02 0000 6a77 0300 0075  j{...j....jw...u
+000039b0: 626a 7c03 0000 2981 947d 9428 6aeb 0200  bj|...)..}.(j...
+000039c0: 008c 0d63 6173 745f 7374 723d 5472 7565  ...cast_str=True
+000039d0: 946a ec02 0000 5d94 286a 8203 0000 2981  .j....].(j....).
+000039e0: 947d 9428 6aeb 0200 008c 0863 6173 745f  .}.(j......cast_
+000039f0: 7374 7294 6aec 0200 005d 946a fa02 0000  str.j....].j....
+00003a00: 8c08 6361 7374 5f73 7472 9485 9481 947d  ..cast_str.....}
+00003a10: 9428 6aff 0200 006a 9204 0000 6a00 0300  .(j....j....j...
+00003a20: 006a e902 0000 6a01 0300 004e 6a02 0300  .j....j....Nj...
+00003a30: 004e 7562 616a 0303 0000 7d94 286a 0503  .Nubaj....}.(j..
+00003a40: 0000 5d94 6a07 0300 005d 946a 8e03 0000  ..].j....].j....
+00003a50: 616a 0903 0000 5d94 6a0b 0300 005d 946a  aj....].j....].j
+00003a60: 0d03 0000 5d94 756a 0f03 0000 6a81 0300  ....].uj....j...
+00003a70: 006a ff02 0000 6a8e 0400 0075 626a 9303  .j....j....ubj..
+00003a80: 0000 2981 947d 9428 6aeb 0200 008c 013d  ..)..}.(j......=
+00003a90: 946a ec02 0000 5d94 6afa 0200 008c 013d  .j....].j......=
+00003aa0: 9485 9481 947d 9428 6aff 0200 006a a004  .....}.(j....j..
+00003ab0: 0000 6a00 0300 006a e902 0000 6a01 0300  ..j....j....j...
+00003ac0: 004e 6a02 0300 004e 7562 616a 0303 0000  .Nj....Nubaj....
+00003ad0: 7d94 286a 0503 0000 5d94 6a07 0300 005d  }.(j....].j....]
+00003ae0: 946a 9f03 0000 616a 0903 0000 5d94 6a0b  .j....aj....].j.
+00003af0: 0300 005d 946a 0d03 0000 5d94 756a 0f03  ...].j....].uj..
+00003b00: 0000 6a92 0300 006a ff02 0000 6a8e 0400  ..j....j....j...
+00003b10: 0075 626a a303 0000 2981 947d 9428 6aeb  .ubj....)..}.(j.
+00003b20: 0200 008c 0454 7275 6594 6aec 0200 005d  .....True.j....]
+00003b30: 946a fa02 0000 8c04 5472 7565 9485 9481  .j......True....
+00003b40: 947d 9428 6aff 0200 006a ae04 0000 6a00  .}.(j....j....j.
+00003b50: 0300 006a e902 0000 6a01 0300 004e 6a02  ...j....j....Nj.
+00003b60: 0300 004e 7562 616a 0303 0000 7d94 286a  ...Nubaj....}.(j
+00003b70: 0503 0000 5d94 6a07 0300 005d 946a af03  ....].j....].j..
+00003b80: 0000 616a 0903 0000 5d94 6a0b 0300 005d  ..aj....].j....]
+00003b90: 946a 0d03 0000 5d94 8c13 7375 7070 6f72  .j....]...suppor
+00003ba0: 745f 736d 6172 7471 756f 7465 7394 8975  t_smartquotes..u
+00003bb0: 6a0f 0300 0068 fa6a ff02 0000 6a8e 0400  j....h.j....j...
+00003bc0: 0075 6265 6a03 0300 007d 9428 6a05 0300  .ubej....}.(j...
+00003bd0: 005d 946a 0703 0000 5d94 6a09 0300 005d  .].j....].j....]
+00003be0: 946a 0b03 0000 5d94 6a0d 0300 005d 946a  .j....].j....].j
+00003bf0: 6003 0000 6a61 0300 0075 6a0f 0300 006a  `...ja...uj....j
+00003c00: 7b03 0000 6aff 0200 006a 7703 0000 7562  {...j....jw...ub
+00003c10: 6a7c 0300 0029 8194 7d94 286a eb02 0000  j|...)..}.(j....
+00003c20: 8c0f 666f 726d 6174 5f6f 7574 3d4e 6f6e  ..format_out=Non
+00003c30: 6594 6aec 0200 005d 9428 6a82 0300 0029  e.j....].(j....)
+00003c40: 8194 7d94 286a eb02 0000 8c0a 666f 726d  ..}.(j......form
+00003c50: 6174 5f6f 7574 946a ec02 0000 5d94 6afa  at_out.j....].j.
+00003c60: 0200 008c 0a66 6f72 6d61 745f 6f75 7494  .....format_out.
+00003c70: 8594 8194 7d94 286a ff02 0000 6ac7 0400  ....}.(j....j...
+00003c80: 006a 0003 0000 6ae9 0200 006a 0103 0000  .j....j....j....
+00003c90: 4e6a 0203 0000 4e75 6261 6a03 0300 007d  Nj....Nubaj....}
+00003ca0: 9428 6a05 0300 005d 946a 0703 0000 5d94  .(j....].j....].
+00003cb0: 6a8e 0300 0061 6a09 0300 005d 946a 0b03  j....aj....].j..
+00003cc0: 0000 5d94 6a0d 0300 005d 9475 6a0f 0300  ..].j....].uj...
+00003cd0: 006a 8103 0000 6aff 0200 006a c304 0000  .j....j....j....
+00003ce0: 7562 6a93 0300 0029 8194 7d94 286a eb02  ubj....)..}.(j..
+00003cf0: 0000 8c01 3d94 6aec 0200 005d 946a fa02  ....=.j....].j..
+00003d00: 0000 8c01 3d94 8594 8194 7d94 286a ff02  ....=.....}.(j..
+00003d10: 0000 6ad5 0400 006a 0003 0000 6ae9 0200  ..j....j....j...
+00003d20: 006a 0103 0000 4e6a 0203 0000 4e75 6261  .j....Nj....Nuba
+00003d30: 6a03 0300 007d 9428 6a05 0300 005d 946a  j....}.(j....].j
+00003d40: 0703 0000 5d94 6a9f 0300 0061 6a09 0300  ....].j....aj...
+00003d50: 005d 946a 0b03 0000 5d94 6a0d 0300 005d  .].j....].j....]
+00003d60: 9475 6a0f 0300 006a 9203 0000 6aff 0200  .uj....j....j...
+00003d70: 006a c304 0000 7562 6aa3 0300 0029 8194  .j....ubj....)..
+00003d80: 7d94 286a eb02 0000 8c04 4e6f 6e65 946a  }.(j......None.j
+00003d90: ec02 0000 5d94 6afa 0200 008c 044e 6f6e  ....].j......Non
+00003da0: 6594 8594 8194 7d94 286a ff02 0000 6ae3  e.....}.(j....j.
+00003db0: 0400 006a 0003 0000 6ae9 0200 006a 0103  ...j....j....j..
+00003dc0: 0000 4e6a 0203 0000 4e75 6261 6a03 0300  ..Nj....Nubaj...
+00003dd0: 007d 9428 6a05 0300 005d 946a 0703 0000  .}.(j....].j....
+00003de0: 5d94 6aaf 0300 0061 6a09 0300 005d 946a  ].j....aj....].j
+00003df0: 0b03 0000 5d94 6a0d 0300 005d 948c 1373  ....].j....]...s
+00003e00: 7570 706f 7274 5f73 6d61 7274 7175 6f74  upport_smartquot
+00003e10: 6573 9489 756a 0f03 0000 68fa 6aff 0200  es..uj....h.j...
+00003e20: 006a c304 0000 7562 656a 0303 0000 7d94  .j....ubej....}.
+00003e30: 286a 0503 0000 5d94 6a07 0300 005d 946a  (j....].j....].j
+00003e40: 0903 0000 5d94 6a0b 0300 005d 946a 0d03  ....].j....].j..
+00003e50: 0000 5d94 6a60 0300 006a 6103 0000 756a  ..].j`...ja...uj
+00003e60: 0f03 0000 6a7b 0300 006a ff02 0000 6a77  ....j{...j....jw
+00003e70: 0300 0075 6265 6a03 0300 007d 9428 6a05  ...ubej....}.(j.
+00003e80: 0300 005d 946a 0703 0000 5d94 6a09 0300  ...].j....].j...
+00003e90: 005d 946a 0b03 0000 5d94 6a0d 0300 005d  .].j....].j....]
+00003ea0: 946a 6003 0000 6a61 0300 0075 6a0f 0300  .j`...ja...uj...
+00003eb0: 006a 7503 0000 6aff 0200 006a 4a03 0000  .ju...j....jJ...
+00003ec0: 6a00 0300 006a e902 0000 6a01 0300 006a  j....j....j....j
+00003ed0: 6203 0000 6a02 0300 004b 0175 6265 6a03  b...j....K.ubej.
+00003ee0: 0300 007d 9428 6a05 0300 005d 946a 4103  ...}.(j....].jA.
+00003ef0: 0000 616a 0703 0000 5d94 288c 0373 6967  ..aj....].(..sig
+00003f00: 948c 0a73 6967 2d6f 626a 6563 7494 656a  ...sig-object.ej
+00003f10: 0903 0000 5d94 6a0b 0300 005d 946a 0d03  ....].j....].j..
+00003f20: 0000 5d94 8c06 6d6f 6475 6c65 948c 1163  ..]...module...c
+00003f30: 6f6f 6b69 6573 5f75 7469 6c69 7469 6573  ookies_utilities
+00003f40: 946a 6a02 0000 6840 8c08 6675 6c6c 6e61  .jj...h@..fullna
+00003f50: 6d65 946a 6703 0000 8c0a 5f74 6f63 5f70  me.jg....._toc_p
+00003f60: 6172 7473 946a 0705 0000 6a67 0300 0086  arts.j....jg....
+00003f70: 948c 095f 746f 635f 6e61 6d65 948c 0b67  ..._toc_name...g
+00003f80: 6574 5f64 6174 6573 2829 9475 6a0f 0300  et_dates().uj...
+00003f90: 006a 4803 0000 6a01 0300 006a 6203 0000  .jH...j....jb...
+00003fa0: 6a02 0300 004b 016a ff02 0000 6a45 0300  j....K.j....jE..
+00003fb0: 006a 0003 0000 6ae9 0200 0075 626a e602  .j....j....ubj..
+00003fc0: 0000 8c0c 6465 7363 5f63 6f6e 7465 6e74  ....desc_content
+00003fd0: 9493 9429 8194 7d94 286a eb02 0000 6840  ...)..}.(j....h@
+00003fe0: 6aec 0200 005d 9428 6aee 0200 008c 0970  j....].(j......p
+00003ff0: 6172 6167 7261 7068 9493 9429 8194 7d94  aragraph...)..}.
+00004000: 286a eb02 0000 8c58 5265 7475 726e 7320  (j.....XReturns 
+00004010: 6120 6c69 7374 206f 6620 7469 6d65 7320  a list of times 
+00004020: 6672 6f6d 2074 6865 2027 7374 6172 7427  from the 'start'
+00004030: 2074 696d 6520 746f 2074 6865 2027 656e   time to the 'en
+00004040: 6427 2074 696d 652c 0a69 6e63 7265 6d65  d' time,.increme
+00004050: 6e74 6564 2062 7920 2764 656c 7461 272e  nted by 'delta'.
+00004060: 946a ec02 0000 5d94 6afa 0200 008c 6452  .j....].j.....dR
+00004070: 6574 7572 6e73 2061 206c 6973 7420 6f66  eturns a list of
+00004080: 2074 696d 6573 2066 726f 6d20 7468 6520   times from the 
+00004090: e280 9873 7461 7274 e280 9920 7469 6d65  ...start... time
+000040a0: 2074 6f20 7468 6520 e280 9865 6e64 e280   to the ...end..
+000040b0: 9920 7469 6d65 2c0a 696e 6372 656d 656e  . time,.incremen
+000040c0: 7465 6420 6279 20e2 8098 6465 6c74 61e2  ted by ...delta.
+000040d0: 8099 2e94 8594 8194 7d94 286a ff02 0000  ........}.(j....
+000040e0: 6a14 0500 006a 0003 0000 6ae9 0200 006a  j....j....j....j
+000040f0: 0103 0000 4e6a 0203 0000 4e75 6261 6a03  ....Nj....Nubaj.
+00004100: 0300 007d 9428 6a05 0300 005d 946a 0703  ...}.(j....].j..
+00004110: 0000 5d94 6a09 0300 005d 946a 0b03 0000  ..].j....].j....
+00004120: 5d94 6a0d 0300 005d 9475 6a0f 0300 006a  ].j....].uj....j
+00004130: 1205 0000 6a01 0300 008c 7143 3a5c 5573  ....j.....qC:\Us
+00004140: 6572 735c 632d 6d69 685c 7370 6163 655c  ers\c-mih\space\
+00004150: 636f 6f6b 6965 735f 7574 696c 6974 6965  cookies_utilitie
+00004160: 735c 7372 635c 636f 6f6b 6965 735f 7574  s\src\cookies_ut
+00004170: 696c 6974 6965 735c 5f5f 696e 6974 5f5f  ilities\__init__
+00004180: 2e70 793a 646f 6373 7472 696e 6720 6f66  .py:docstring of
+00004190: 2063 6f6f 6b69 6573 5f75 7469 6c69 7469   cookies_utiliti
+000041a0: 6573 2e67 6574 5f64 6174 6573 946a 0203  es.get_dates.j..
+000041b0: 0000 4b01 6aff 0200 006a 0f05 0000 6a00  ..K.j....j....j.
+000041c0: 0300 006a e902 0000 7562 6a13 0500 0029  ...j....ubj....)
+000041d0: 8194 7d94 286a eb02 0000 8c53 4966 2079  ..}.(j.....SIf y
+000041e0: 6f75 2772 6520 7573 696e 6720 7468 6520  ou're using the 
+000041f0: 7265 7375 6c74 2061 7320 616e 2069 7465  result as an ite
+00004200: 7261 746f 722c 2069 7420 6973 2072 6563  rator, it is rec
+00004210: 6f6d 6d65 6e64 6564 2074 6f20 7365 7420  ommended to set 
+00004220: 2a67 656e 6974 6572 3d54 7275 652a 2e94  *geniter=True*..
+00004230: 6aec 0200 005d 9428 6afa 0200 008c 4649  j....].(j.....FI
+00004240: 6620 796f 75e2 8099 7265 2075 7369 6e67  f you...re using
+00004250: 2074 6865 2072 6573 756c 7420 6173 2061   the result as a
+00004260: 6e20 6974 6572 6174 6f72 2c20 6974 2069  n iterator, it i
+00004270: 7320 7265 636f 6d6d 656e 6465 6420 746f  s recommended to
+00004280: 2073 6574 2094 8594 8194 7d94 286a ff02   set .....}.(j..
+00004290: 0000 6a23 0500 006a 0003 0000 6ae9 0200  ..j#...j....j...
+000042a0: 006a 0103 0000 4e6a 0203 0000 4e75 626a  .j....Nj....Nubj
+000042b0: ee02 0000 8c08 656d 7068 6173 6973 9493  ......emphasis..
+000042c0: 9429 8194 7d94 286a eb02 0000 8c0e 2a67  .)..}.(j......*g
+000042d0: 656e 6974 6572 3d54 7275 652a 946a ec02  eniter=True*.j..
+000042e0: 0000 5d94 6afa 0200 008c 0c67 656e 6974  ..].j......genit
+000042f0: 6572 3d54 7275 6594 8594 8194 7d94 286a  er=True.....}.(j
+00004300: ff02 0000 6a2d 0500 006a 0003 0000 6ae9  ....j-...j....j.
+00004310: 0200 006a 0103 0000 4e6a 0203 0000 4e75  ...j....Nj....Nu
+00004320: 6261 6a03 0300 007d 9428 6a05 0300 005d  baj....}.(j....]
+00004330: 946a 0703 0000 5d94 6a09 0300 005d 946a  .j....].j....].j
+00004340: 0b03 0000 5d94 6a0d 0300 005d 9475 6a0f  ....].j....].uj.
+00004350: 0300 006a 2b05 0000 6aff 0200 006a 2305  ...j+...j....j#.
+00004360: 0000 7562 6afa 0200 008c 012e 9485 9481  ..ubj...........
+00004370: 947d 9428 6aff 0200 006a 2305 0000 6a00  .}.(j....j#...j.
+00004380: 0300 006a e902 0000 6a01 0300 004e 6a02  ...j....j....Nj.
+00004390: 0300 004e 7562 656a 0303 0000 7d94 286a  ...Nubej....}.(j
+000043a0: 0503 0000 5d94 6a07 0300 005d 946a 0903  ....].j....].j..
+000043b0: 0000 5d94 6a0b 0300 005d 946a 0d03 0000  ..].j....].j....
+000043c0: 5d94 756a 0f03 0000 6a12 0500 006a 0103  ].uj....j....j..
+000043d0: 0000 6a22 0500 006a 0203 0000 4b04 6aff  ..j"...j....K.j.
+000043e0: 0200 006a 0f05 0000 6a00 0300 006a e902  ...j....j....j..
+000043f0: 0000 7562 6aee 0200 008c 0a66 6965 6c64  ..ubj......field
+00004400: 5f6c 6973 7494 9394 2981 947d 9428 6aeb  _list...)..}.(j.
+00004410: 0200 0068 406a ec02 0000 5d94 286a ee02  ...h@j....].(j..
+00004420: 0000 8c05 6669 656c 6494 9394 2981 947d  ....field...)..}
+00004430: 9428 6aeb 0200 0068 406a ec02 0000 5d94  .(j....h@j....].
+00004440: 286a ee02 0000 8c0a 6669 656c 645f 6e61  (j......field_na
+00004450: 6d65 9493 9429 8194 7d94 286a eb02 0000  me...)..}.(j....
+00004460: 8c0a 5061 7261 6d65 7465 7273 946a ec02  ..Parameters.j..
+00004470: 0000 5d94 6afa 0200 008c 0a50 6172 616d  ..].j......Param
+00004480: 6574 6572 7394 8594 8194 7d94 286a ff02  eters.....}.(j..
+00004490: 0000 6a51 0500 006a 0003 0000 6ae9 0200  ..jQ...j....j...
+000044a0: 006a 0103 0000 4e6a 0203 0000 4e75 6261  .j....Nj....Nuba
+000044b0: 6a03 0300 007d 9428 6a05 0300 005d 946a  j....}.(j....].j
+000044c0: 0703 0000 5d94 6a09 0300 005d 946a 0b03  ....].j....].j..
+000044d0: 0000 5d94 6a0d 0300 005d 9475 6a0f 0300  ..].j....].uj...
+000044e0: 006a 4f05 0000 6aff 0200 006a 4c05 0000  .jO...j....jL...
+000044f0: 6a01 0300 006a 6203 0000 6a02 0300 004b  j....jb...j....K
+00004500: 0075 626a ee02 0000 8c0a 6669 656c 645f  .ubj......field_
+00004510: 626f 6479 9493 9429 8194 7d94 286a eb02  body...)..}.(j..
+00004520: 0000 6840 6aec 0200 005d 946a ee02 0000  ..h@j....].j....
+00004530: 8c0b 6275 6c6c 6574 5f6c 6973 7494 9394  ..bullet_list...
+00004540: 2981 947d 9428 6aeb 0200 0068 406a ec02  )..}.(j....h@j..
+00004550: 0000 5d94 286a ee02 0000 8c09 6c69 7374  ..].(j......list
+00004560: 5f69 7465 6d94 9394 2981 947d 9428 6aeb  _item...)..}.(j.
+00004570: 0200 0068 406a ec02 0000 5d94 6a13 0500  ...h@j....].j...
+00004580: 0029 8194 7d94 286a eb02 0000 8c24 7374  .)..}.(j.....$st
+00004590: 6172 7420 2873 7472 696e 6729 202d 2d20  art (string) -- 
+000045a0: 5374 6172 7420 7469 6d65 2073 7472 696e  Start time strin
+000045b0: 672e 946a ec02 0000 5d94 286a e602 0000  g..j....].(j....
+000045c0: 8c0e 6c69 7465 7261 6c5f 7374 726f 6e67  ..literal_strong
+000045d0: 9493 9429 8194 7d94 286a eb02 0000 8c05  ...)..}.(j......
+000045e0: 7374 6172 7494 6aec 0200 005d 946a fa02  start.j....].j..
+000045f0: 0000 8c05 7374 6172 7494 8594 8194 7d94  ....start.....}.
+00004600: 286a ff02 0000 6a74 0500 006a 0003 0000  (j....jt...j....
+00004610: 6ae9 0200 006a 0103 0000 4e6a 0203 0000  j....j....Nj....
+00004620: 4e75 6261 6a03 0300 007d 9428 6a05 0300  Nubaj....}.(j...
+00004630: 005d 946a 0703 0000 5d94 6a09 0300 005d  .].j....].j....]
+00004640: 946a 0b03 0000 5d94 6a0d 0300 005d 9475  .j....].j....].u
+00004650: 6a0f 0300 006a 7205 0000 6aff 0200 006a  j....jr...j....j
+00004660: 6e05 0000 7562 6afa 0200 008c 0220 2894  n...ubj...... (.
+00004670: 8594 8194 7d94 286a ff02 0000 6a6e 0500  ....}.(j....jn..
+00004680: 006a 0003 0000 6ae9 0200 006a 0103 0000  .j....j....j....
+00004690: 4e6a 0203 0000 4e75 626a e602 0000 8c0c  Nj....Nubj......
+000046a0: 7065 6e64 696e 675f 7872 6566 9493 9429  pending_xref...)
+000046b0: 8194 7d94 286a eb02 0000 6840 6aec 0200  ..}.(j....h@j...
+000046c0: 005d 946a e602 0000 8c10 6c69 7465 7261  .].j......litera
+000046d0: 6c5f 656d 7068 6173 6973 9493 9429 8194  l_emphasis...)..
+000046e0: 7d94 286a eb02 0000 8c06 7374 7269 6e67  }.(j......string
+000046f0: 946a ec02 0000 5d94 6afa 0200 008c 0673  .j....].j......s
+00004700: 7472 696e 6794 8594 8194 7d94 286a ff02  tring.....}.(j..
+00004710: 0000 6a8d 0500 006a 0003 0000 6ae9 0200  ..j....j....j...
+00004720: 006a 0103 0000 4e6a 0203 0000 4e75 6261  .j....Nj....Nuba
+00004730: 6a03 0300 007d 9428 6a05 0300 005d 946a  j....}.(j....].j
+00004740: 0703 0000 5d94 6a09 0300 005d 946a 0b03  ....].j....].j..
+00004750: 0000 5d94 6a0d 0300 005d 9475 6a0f 0300  ..].j....].uj...
+00004760: 006a 8b05 0000 6aff 0200 006a 8805 0000  .j....j....j....
+00004770: 7562 616a 0303 0000 7d94 286a 0503 0000  ubaj....}.(j....
+00004780: 5d94 6a07 0300 005d 946a 0903 0000 5d94  ].j....].j....].
+00004790: 6a0b 0300 005d 946a 0d03 0000 5d94 8c09  j....].j....]...
+000047a0: 7265 6664 6f6d 6169 6e94 8c02 7079 948c  refdomain...py..
+000047b0: 0b72 6566 6578 706c 6963 6974 9489 8c07  .refexplicit....
+000047c0: 7265 6674 7970 6594 6a6a 0200 008c 0972  reftype.jj.....r
+000047d0: 6566 7461 7267 6574 946a 8f05 0000 8c0b  eftarget.j......
+000047e0: 7265 6673 7065 6369 6669 6394 888c 0970  refspecific....p
+000047f0: 793a 6d6f 6475 6c65 946a 0705 0000 8c08  y:module.j......
+00004800: 7079 3a63 6c61 7373 944e 756a 0f03 0000  py:class.Nuj....
+00004810: 6a86 0500 006a ff02 0000 6a6e 0500 0075  j....j....jn...u
+00004820: 626a fa02 0000 8c01 2994 8594 8194 7d94  bj......).....}.
+00004830: 286a ff02 0000 6a6e 0500 006a 0003 0000  (j....jn...j....
+00004840: 6ae9 0200 006a 0103 0000 4e6a 0203 0000  j....j....Nj....
+00004850: 4e75 626a fa02 0000 8c05 20e2 8093 2094  Nubj...... ... .
+00004860: 8594 8194 7d94 286a ff02 0000 6a6e 0500  ....}.(j....jn..
+00004870: 006a 0003 0000 6ae9 0200 006a 0103 0000  .j....j....j....
+00004880: 4e6a 0203 0000 4e75 626a fa02 0000 8c12  Nj....Nubj......
+00004890: 5374 6172 7420 7469 6d65 2073 7472 696e  Start time strin
+000048a0: 672e 9485 9481 947d 9428 6aff 0200 006a  g......}.(j....j
+000048b0: 6e05 0000 6a00 0300 006a e902 0000 6a01  n...j....j....j.
+000048c0: 0300 004e 6a02 0300 004e 7562 656a 0303  ...Nj....Nubej..
+000048d0: 0000 7d94 286a 0503 0000 5d94 6a07 0300  ..}.(j....].j...
+000048e0: 005d 946a 0903 0000 5d94 6a0b 0300 005d  .].j....].j....]
+000048f0: 946a 0d03 0000 5d94 756a 0f03 0000 6a12  .j....].uj....j.
+00004900: 0500 006a ff02 0000 6a6b 0500 0075 6261  ...j....jk...uba
+00004910: 6a03 0300 007d 9428 6a05 0300 005d 946a  j....}.(j....].j
+00004920: 0703 0000 5d94 6a09 0300 005d 946a 0b03  ....].j....].j..
+00004930: 0000 5d94 6a0d 0300 005d 9475 6a0f 0300  ..].j....].uj...
+00004940: 006a 6905 0000 6aff 0200 006a 6605 0000  .ji...j....jf...
+00004950: 7562 6a6a 0500 0029 8194 7d94 286a eb02  ubjj...)..}.(j..
+00004960: 0000 6840 6aec 0200 005d 946a 1305 0000  ..h@j....].j....
+00004970: 2981 947d 9428 6aeb 0200 008c 2c65 6e64  )..}.(j.....,end
+00004980: 2028 7374 7269 6e67 2920 2d2d 2045 6e64   (string) -- End
+00004990: 2074 696d 6520 7374 7269 6e67 2028 696e   time string (in
+000049a0: 636c 7573 6976 6529 2e94 6aec 0200 005d  clusive)..j....]
+000049b0: 9428 6a73 0500 0029 8194 7d94 286a eb02  .(js...)..}.(j..
+000049c0: 0000 8c03 656e 6494 6aec 0200 005d 946a  ....end.j....].j
+000049d0: fa02 0000 8c03 656e 6494 8594 8194 7d94  ......end.....}.
+000049e0: 286a ff02 0000 6ac8 0500 006a 0003 0000  (j....j....j....
+000049f0: 6ae9 0200 006a 0103 0000 4e6a 0203 0000  j....j....Nj....
+00004a00: 4e75 6261 6a03 0300 007d 9428 6a05 0300  Nubaj....}.(j...
+00004a10: 005d 946a 0703 0000 5d94 6a09 0300 005d  .].j....].j....]
+00004a20: 946a 0b03 0000 5d94 6a0d 0300 005d 9475  .j....].j....].u
+00004a30: 6a0f 0300 006a 7205 0000 6aff 0200 006a  j....jr...j....j
+00004a40: c405 0000 7562 6afa 0200 008c 0220 2894  ....ubj...... (.
+00004a50: 8594 8194 7d94 286a ff02 0000 6ac4 0500  ....}.(j....j...
+00004a60: 006a 0003 0000 6ae9 0200 006a 0103 0000  .j....j....j....
+00004a70: 4e6a 0203 0000 4e75 626a 8705 0000 2981  Nj....Nubj....).
+00004a80: 947d 9428 6aeb 0200 0068 406a ec02 0000  .}.(j....h@j....
+00004a90: 5d94 6a8c 0500 0029 8194 7d94 286a eb02  ].j....)..}.(j..
+00004aa0: 0000 8c06 7374 7269 6e67 946a ec02 0000  ....string.j....
+00004ab0: 5d94 6afa 0200 008c 0673 7472 696e 6794  ].j......string.
+00004ac0: 8594 8194 7d94 286a ff02 0000 6add 0500  ....}.(j....j...
+00004ad0: 006a 0003 0000 6ae9 0200 006a 0103 0000  .j....j....j....
+00004ae0: 4e6a 0203 0000 4e75 6261 6a03 0300 007d  Nj....Nubaj....}
+00004af0: 9428 6a05 0300 005d 946a 0703 0000 5d94  .(j....].j....].
+00004b00: 6a09 0300 005d 946a 0b03 0000 5d94 6a0d  j....].j....].j.
+00004b10: 0300 005d 9475 6a0f 0300 006a 8b05 0000  ...].uj....j....
+00004b20: 6aff 0200 006a da05 0000 7562 616a 0303  j....j....ubaj..
+00004b30: 0000 7d94 286a 0503 0000 5d94 6a07 0300  ..}.(j....].j...
+00004b40: 005d 946a 0903 0000 5d94 6a0b 0300 005d  .].j....].j....]
+00004b50: 946a 0d03 0000 5d94 8c09 7265 6664 6f6d  .j....]...refdom
+00004b60: 6169 6e94 6aa2 0500 008c 0b72 6566 6578  ain.j......refex
+00004b70: 706c 6963 6974 9489 8c07 7265 6674 7970  plicit....reftyp
+00004b80: 6594 6a6a 0200 008c 0972 6566 7461 7267  e.jj.....reftarg
+00004b90: 6574 946a df05 0000 6aa6 0500 0088 6aa7  et.j....j.....j.
+00004ba0: 0500 006a 0705 0000 6aa8 0500 004e 756a  ...j....j....Nuj
+00004bb0: 0f03 0000 6a86 0500 006a ff02 0000 6ac4  ....j....j....j.
+00004bc0: 0500 0075 626a fa02 0000 8c01 2994 8594  ...ubj......)...
+00004bd0: 8194 7d94 286a ff02 0000 6ac4 0500 006a  ..}.(j....j....j
+00004be0: 0003 0000 6ae9 0200 006a 0103 0000 4e6a  ....j....j....Nj
+00004bf0: 0203 0000 4e75 626a fa02 0000 8c05 20e2  ....Nubj...... .
+00004c00: 8093 2094 8594 8194 7d94 286a ff02 0000  .. .....}.(j....
+00004c10: 6ac4 0500 006a 0003 0000 6ae9 0200 006a  j....j....j....j
+00004c20: 0103 0000 4e6a 0203 0000 4e75 626a fa02  ....Nj....Nubj..
+00004c30: 0000 8c1c 456e 6420 7469 6d65 2073 7472  ....End time str
+00004c40: 696e 6720 2869 6e63 6c75 7369 7665 292e  ing (inclusive).
+00004c50: 9485 9481 947d 9428 6aff 0200 006a c405  .....}.(j....j..
+00004c60: 0000 6a00 0300 006a e902 0000 6a01 0300  ..j....j....j...
+00004c70: 004e 6a02 0300 004e 7562 656a 0303 0000  .Nj....Nubej....
+00004c80: 7d94 286a 0503 0000 5d94 6a07 0300 005d  }.(j....].j....]
+00004c90: 946a 0903 0000 5d94 6a0b 0300 005d 946a  .j....].j....].j
+00004ca0: 0d03 0000 5d94 756a 0f03 0000 6a12 0500  ....].uj....j...
+00004cb0: 006a ff02 0000 6ac1 0500 0075 6261 6a03  .j....j....ubaj.
+00004cc0: 0300 007d 9428 6a05 0300 005d 946a 0703  ...}.(j....].j..
+00004cd0: 0000 5d94 6a09 0300 005d 946a 0b03 0000  ..].j....].j....
+00004ce0: 5d94 6a0d 0300 005d 9475 6a0f 0300 006a  ].j....].uj....j
+00004cf0: 6905 0000 6aff 0200 006a 6605 0000 7562  i...j....jf...ub
+00004d00: 6a6a 0500 0029 8194 7d94 286a eb02 0000  jj...)..}.(j....
+00004d10: 6840 6aec 0200 005d 946a 1305 0000 2981  h@j....].j....).
+00004d20: 947d 9428 6aeb 0200 008c 3b66 6f72 6d61  .}.(j.....;forma
+00004d30: 7420 2873 7472 696e 6729 202d 2d20 436f  t (string) -- Co
+00004d40: 6e76 6572 7369 6f6e 2066 6f72 6d61 7420  nversion format 
+00004d50: 666f 7220 6461 7465 7469 6d65 2e73 7472  for datetime.str
+00004d60: 7074 696d 652e 946a ec02 0000 5d94 286a  ptime..j....].(j
+00004d70: 7305 0000 2981 947d 9428 6aeb 0200 008c  s...)..}.(j.....
+00004d80: 0666 6f72 6d61 7494 6aec 0200 005d 946a  .format.j....].j
+00004d90: fa02 0000 8c06 666f 726d 6174 9485 9481  ......format....
+00004da0: 947d 9428 6aff 0200 006a 1406 0000 6a00  .}.(j....j....j.
+00004db0: 0300 006a e902 0000 6a01 0300 004e 6a02  ...j....j....Nj.
+00004dc0: 0300 004e 7562 616a 0303 0000 7d94 286a  ...Nubaj....}.(j
+00004dd0: 0503 0000 5d94 6a07 0300 005d 946a 0903  ....].j....].j..
+00004de0: 0000 5d94 6a0b 0300 005d 946a 0d03 0000  ..].j....].j....
+00004df0: 5d94 756a 0f03 0000 6a72 0500 006a ff02  ].uj....jr...j..
+00004e00: 0000 6a10 0600 0075 626a fa02 0000 8c02  ..j....ubj......
+00004e10: 2028 9485 9481 947d 9428 6aff 0200 006a   (.....}.(j....j
+00004e20: 1006 0000 6a00 0300 006a e902 0000 6a01  ....j....j....j.
+00004e30: 0300 004e 6a02 0300 004e 7562 6a87 0500  ...Nj....Nubj...
+00004e40: 0029 8194 7d94 286a eb02 0000 6840 6aec  .)..}.(j....h@j.
+00004e50: 0200 005d 946a 8c05 0000 2981 947d 9428  ...].j....)..}.(
+00004e60: 6aeb 0200 008c 0673 7472 696e 6794 6aec  j......string.j.
+00004e70: 0200 005d 946a fa02 0000 8c06 7374 7269  ...].j......stri
+00004e80: 6e67 9485 9481 947d 9428 6aff 0200 006a  ng.....}.(j....j
+00004e90: 2906 0000 6a00 0300 006a e902 0000 6a01  )...j....j....j.
+00004ea0: 0300 004e 6a02 0300 004e 7562 616a 0303  ...Nj....Nubaj..
+00004eb0: 0000 7d94 286a 0503 0000 5d94 6a07 0300  ..}.(j....].j...
+00004ec0: 005d 946a 0903 0000 5d94 6a0b 0300 005d  .].j....].j....]
+00004ed0: 946a 0d03 0000 5d94 756a 0f03 0000 6a8b  .j....].uj....j.
+00004ee0: 0500 006a ff02 0000 6a26 0600 0075 6261  ...j....j&...uba
+00004ef0: 6a03 0300 007d 9428 6a05 0300 005d 946a  j....}.(j....].j
+00004f00: 0703 0000 5d94 6a09 0300 005d 946a 0b03  ....].j....].j..
+00004f10: 0000 5d94 6a0d 0300 005d 948c 0972 6566  ..].j....]...ref
+00004f20: 646f 6d61 696e 946a a205 0000 8c0b 7265  domain.j......re
+00004f30: 6665 7870 6c69 6369 7494 898c 0772 6566  fexplicit....ref
+00004f40: 7479 7065 946a 6a02 0000 8c09 7265 6674  type.jj.....reft
+00004f50: 6172 6765 7494 6a2b 0600 006a a605 0000  arget.j+...j....
+00004f60: 886a a705 0000 6a07 0500 006a a805 0000  .j....j....j....
+00004f70: 4e75 6a0f 0300 006a 8605 0000 6aff 0200  Nuj....j....j...
+00004f80: 006a 1006 0000 7562 6afa 0200 008c 0129  .j....ubj......)
+00004f90: 9485 9481 947d 9428 6aff 0200 006a 1006  .....}.(j....j..
+00004fa0: 0000 6a00 0300 006a e902 0000 6a01 0300  ..j....j....j...
+00004fb0: 004e 6a02 0300 004e 7562 6afa 0200 008c  .Nj....Nubj.....
+00004fc0: 0520 e280 9320 9485 9481 947d 9428 6aff  . ... .....}.(j.
+00004fd0: 0200 006a 1006 0000 6a00 0300 006a e902  ...j....j....j..
+00004fe0: 0000 6a01 0300 004e 6a02 0300 004e 7562  ..j....Nj....Nub
+00004ff0: 6afa 0200 008c 2843 6f6e 7665 7273 696f  j.....(Conversio
+00005000: 6e20 666f 726d 6174 2066 6f72 2064 6174  n format for dat
+00005010: 6574 696d 652e 7374 7270 7469 6d65 2e94  etime.strptime..
+00005020: 8594 8194 7d94 286a ff02 0000 6a10 0600  ....}.(j....j...
+00005030: 006a 0003 0000 6ae9 0200 006a 0103 0000  .j....j....j....
+00005040: 4e6a 0203 0000 4e75 6265 6a03 0300 007d  Nj....Nubej....}
+00005050: 9428 6a05 0300 005d 946a 0703 0000 5d94  .(j....].j....].
+00005060: 6a09 0300 005d 946a 0b03 0000 5d94 6a0d  j....].j....].j.
+00005070: 0300 005d 9475 6a0f 0300 006a 1205 0000  ...].uj....j....
+00005080: 6aff 0200 006a 0d06 0000 7562 616a 0303  j....j....ubaj..
+00005090: 0000 7d94 286a 0503 0000 5d94 6a07 0300  ..}.(j....].j...
+000050a0: 005d 946a 0903 0000 5d94 6a0b 0300 005d  .].j....].j....]
+000050b0: 946a 0d03 0000 5d94 756a 0f03 0000 6a69  .j....].uj....ji
+000050c0: 0500 006a ff02 0000 6a66 0500 0075 626a  ...j....jf...ubj
+000050d0: 6a05 0000 2981 947d 9428 6aeb 0200 0068  j...)..}.(j....h
+000050e0: 406a ec02 0000 5d94 6a13 0500 0029 8194  @j....].j....)..
+000050f0: 7d94 286a eb02 0000 8c39 6465 6c74 6120  }.(j.....9delta 
+00005100: 2864 6963 7429 202d 2d20 5469 6d65 6465  (dict) -- Timede
+00005110: 6c74 6120 6173 2061 7267 7320 666f 7220  lta as args for 
+00005120: 6461 7465 7469 6d65 2e74 696d 6564 656c  datetime.timedel
+00005130: 7461 2e94 6aec 0200 005d 9428 6a73 0500  ta..j....].(js..
+00005140: 0029 8194 7d94 286a eb02 0000 8c05 6465  .)..}.(j......de
+00005150: 6c74 6194 6aec 0200 005d 946a fa02 0000  lta.j....].j....
+00005160: 8c05 6465 6c74 6194 8594 8194 7d94 286a  ..delta.....}.(j
+00005170: ff02 0000 6a60 0600 006a 0003 0000 6ae9  ....j`...j....j.
+00005180: 0200 006a 0103 0000 4e6a 0203 0000 4e75  ...j....Nj....Nu
+00005190: 6261 6a03 0300 007d 9428 6a05 0300 005d  baj....}.(j....]
+000051a0: 946a 0703 0000 5d94 6a09 0300 005d 946a  .j....].j....].j
+000051b0: 0b03 0000 5d94 6a0d 0300 005d 9475 6a0f  ....].j....].uj.
+000051c0: 0300 006a 7205 0000 6aff 0200 006a 5c06  ...jr...j....j\.
+000051d0: 0000 7562 6afa 0200 008c 0220 2894 8594  ..ubj...... (...
+000051e0: 8194 7d94 286a ff02 0000 6a5c 0600 006a  ..}.(j....j\...j
+000051f0: 0003 0000 6ae9 0200 006a 0103 0000 4e6a  ....j....j....Nj
+00005200: 0203 0000 4e75 626a 8705 0000 2981 947d  ....Nubj....)..}
+00005210: 9428 6aeb 0200 0068 406a ec02 0000 5d94  .(j....h@j....].
+00005220: 6a8c 0500 0029 8194 7d94 286a eb02 0000  j....)..}.(j....
+00005230: 8c04 6469 6374 946a ec02 0000 5d94 6afa  ..dict.j....].j.
+00005240: 0200 008c 0464 6963 7494 8594 8194 7d94  .....dict.....}.
+00005250: 286a ff02 0000 6a75 0600 006a 0003 0000  (j....ju...j....
+00005260: 6ae9 0200 006a 0103 0000 4e6a 0203 0000  j....j....Nj....
+00005270: 4e75 6261 6a03 0300 007d 9428 6a05 0300  Nubaj....}.(j...
+00005280: 005d 946a 0703 0000 5d94 6a09 0300 005d  .].j....].j....]
+00005290: 946a 0b03 0000 5d94 6a0d 0300 005d 9475  .j....].j....].u
+000052a0: 6a0f 0300 006a 8b05 0000 6aff 0200 006a  j....j....j....j
+000052b0: 7206 0000 7562 616a 0303 0000 7d94 286a  r...ubaj....}.(j
+000052c0: 0503 0000 5d94 6a07 0300 005d 946a 0903  ....].j....].j..
+000052d0: 0000 5d94 6a0b 0300 005d 946a 0d03 0000  ..].j....].j....
+000052e0: 5d94 8c09 7265 6664 6f6d 6169 6e94 6aa2  ]...refdomain.j.
+000052f0: 0500 008c 0b72 6566 6578 706c 6963 6974  .....refexplicit
+00005300: 9489 8c07 7265 6674 7970 6594 6a6a 0200  ....reftype.jj..
+00005310: 008c 0972 6566 7461 7267 6574 946a 7706  ...reftarget.jw.
+00005320: 0000 6aa6 0500 0088 6aa7 0500 006a 0705  ..j.....j....j..
+00005330: 0000 6aa8 0500 004e 756a 0f03 0000 6a86  ..j....Nuj....j.
+00005340: 0500 006a ff02 0000 6a5c 0600 0075 626a  ...j....j\...ubj
+00005350: fa02 0000 8c01 2994 8594 8194 7d94 286a  ......).....}.(j
+00005360: ff02 0000 6a5c 0600 006a 0003 0000 6ae9  ....j\...j....j.
+00005370: 0200 006a 0103 0000 4e6a 0203 0000 4e75  ...j....Nj....Nu
+00005380: 626a fa02 0000 8c05 20e2 8093 2094 8594  bj...... ... ...
+00005390: 8194 7d94 286a ff02 0000 6a5c 0600 006a  ..}.(j....j\...j
+000053a0: 0003 0000 6ae9 0200 006a 0103 0000 4e6a  ....j....j....Nj
+000053b0: 0203 0000 4e75 626a fa02 0000 8c29 5469  ....Nubj.....)Ti
+000053c0: 6d65 6465 6c74 6120 6173 2061 7267 7320  medelta as args 
+000053d0: 666f 7220 6461 7465 7469 6d65 2e74 696d  for datetime.tim
+000053e0: 6564 656c 7461 2e94 8594 8194 7d94 286a  edelta......}.(j
+000053f0: ff02 0000 6a5c 0600 006a 0003 0000 6ae9  ....j\...j....j.
+00005400: 0200 006a 0103 0000 4e6a 0203 0000 4e75  ...j....Nj....Nu
+00005410: 6265 6a03 0300 007d 9428 6a05 0300 005d  bej....}.(j....]
+00005420: 946a 0703 0000 5d94 6a09 0300 005d 946a  .j....].j....].j
+00005430: 0b03 0000 5d94 6a0d 0300 005d 9475 6a0f  ....].j....].uj.
+00005440: 0300 006a 1205 0000 6aff 0200 006a 5906  ...j....j....jY.
+00005450: 0000 7562 616a 0303 0000 7d94 286a 0503  ..ubaj....}.(j..
+00005460: 0000 5d94 6a07 0300 005d 946a 0903 0000  ..].j....].j....
+00005470: 5d94 6a0b 0300 005d 946a 0d03 0000 5d94  ].j....].j....].
+00005480: 756a 0f03 0000 6a69 0500 006a ff02 0000  uj....ji...j....
+00005490: 6a66 0500 0075 626a 6a05 0000 2981 947d  jf...ubjj...)..}
+000054a0: 9428 6aeb 0200 0068 406a ec02 0000 5d94  .(j....h@j....].
+000054b0: 6a13 0500 0029 8194 7d94 286a eb02 0000  j....)..}.(j....
+000054c0: 8c4c 6765 6e69 7465 7220 2862 6f6f 6c29  .Lgeniter (bool)
+000054d0: 202d 2d20 5768 6574 6865 7220 746f 2072   -- Whether to r
+000054e0: 6574 7572 6e20 6173 2061 2067 656e 6572  eturn as a gener
+000054f0: 6174 6f72 2069 7465 7261 746f 7220 2864  ator iterator (d
+00005500: 6566 6175 6c74 2046 616c 7365 292e 946a  efault False)..j
+00005510: ec02 0000 5d94 286a 7305 0000 2981 947d  ....].(js...)..}
+00005520: 9428 6aeb 0200 008c 0767 656e 6974 6572  .(j......geniter
+00005530: 946a ec02 0000 5d94 6afa 0200 008c 0767  .j....].j......g
+00005540: 656e 6974 6572 9485 9481 947d 9428 6aff  eniter.....}.(j.
+00005550: 0200 006a ac06 0000 6a00 0300 006a e902  ...j....j....j..
+00005560: 0000 6a01 0300 004e 6a02 0300 004e 7562  ..j....Nj....Nub
+00005570: 616a 0303 0000 7d94 286a 0503 0000 5d94  aj....}.(j....].
+00005580: 6a07 0300 005d 946a 0903 0000 5d94 6a0b  j....].j....].j.
+00005590: 0300 005d 946a 0d03 0000 5d94 756a 0f03  ...].j....].uj..
+000055a0: 0000 6a72 0500 006a ff02 0000 6aa8 0600  ..jr...j....j...
+000055b0: 0075 626a fa02 0000 8c02 2028 9485 9481  .ubj...... (....
+000055c0: 947d 9428 6aff 0200 006a a806 0000 6a00  .}.(j....j....j.
+000055d0: 0300 006a e902 0000 6a01 0300 004e 6a02  ...j....j....Nj.
+000055e0: 0300 004e 7562 6a87 0500 0029 8194 7d94  ...Nubj....)..}.
+000055f0: 286a eb02 0000 6840 6aec 0200 005d 946a  (j....h@j....].j
+00005600: 8c05 0000 2981 947d 9428 6aeb 0200 008c  ....)..}.(j.....
+00005610: 0462 6f6f 6c94 6aec 0200 005d 946a fa02  .bool.j....].j..
+00005620: 0000 8c04 626f 6f6c 9485 9481 947d 9428  ....bool.....}.(
+00005630: 6aff 0200 006a c106 0000 6a00 0300 006a  j....j....j....j
+00005640: e902 0000 6a01 0300 004e 6a02 0300 004e  ....j....Nj....N
+00005650: 7562 616a 0303 0000 7d94 286a 0503 0000  ubaj....}.(j....
+00005660: 5d94 6a07 0300 005d 946a 0903 0000 5d94  ].j....].j....].
+00005670: 6a0b 0300 005d 946a 0d03 0000 5d94 756a  j....].j....].uj
+00005680: 0f03 0000 6a8b 0500 006a ff02 0000 6abe  ....j....j....j.
+00005690: 0600 0075 6261 6a03 0300 007d 9428 6a05  ...ubaj....}.(j.
+000056a0: 0300 005d 946a 0703 0000 5d94 6a09 0300  ...].j....].j...
+000056b0: 005d 946a 0b03 0000 5d94 6a0d 0300 005d  .].j....].j....]
+000056c0: 948c 0972 6566 646f 6d61 696e 946a a205  ...refdomain.j..
+000056d0: 0000 8c0b 7265 6665 7870 6c69 6369 7494  ....refexplicit.
+000056e0: 898c 0772 6566 7479 7065 946a 6a02 0000  ...reftype.jj...
+000056f0: 8c09 7265 6674 6172 6765 7494 6ac3 0600  ..reftarget.j...
+00005700: 006a a605 0000 886a a705 0000 6a07 0500  .j.....j....j...
+00005710: 006a a805 0000 4e75 6a0f 0300 006a 8605  .j....Nuj....j..
+00005720: 0000 6aff 0200 006a a806 0000 7562 6afa  ..j....j....ubj.
+00005730: 0200 008c 0129 9485 9481 947d 9428 6aff  .....).....}.(j.
+00005740: 0200 006a a806 0000 6a00 0300 006a e902  ...j....j....j..
+00005750: 0000 6a01 0300 004e 6a02 0300 004e 7562  ..j....Nj....Nub
+00005760: 6afa 0200 008c 0520 e280 9320 9485 9481  j...... ... ....
+00005770: 947d 9428 6aff 0200 006a a806 0000 6a00  .}.(j....j....j.
+00005780: 0300 006a e902 0000 6a01 0300 004e 6a02  ...j....j....Nj.
+00005790: 0300 004e 7562 6afa 0200 008c 3357 6865  ...Nubj.....3Whe
+000057a0: 7468 6572 2074 6f20 7265 7475 726e 2061  ther to return a
+000057b0: 7320 6120 6765 6e65 7261 746f 7220 6974  s a generator it
+000057c0: 6572 6174 6f72 2028 6465 6661 756c 7420  erator (default 
+000057d0: 9485 9481 947d 9428 6aff 0200 006a a806  .....}.(j....j..
+000057e0: 0000 6a00 0300 006a e902 0000 6a01 0300  ..j....j....j...
+000057f0: 004e 6a02 0300 004e 7562 6a2c 0500 0029  .Nj....Nubj,...)
+00005800: 8194 7d94 286a eb02 0000 8c07 2a46 616c  ..}.(j......*Fal
+00005810: 7365 2a94 6aec 0200 005d 946a fa02 0000  se*.j....].j....
+00005820: 8c05 4661 6c73 6594 8594 8194 7d94 286a  ..False.....}.(j
+00005830: ff02 0000 6ae5 0600 006a 0003 0000 6ae9  ....j....j....j.
+00005840: 0200 006a 0103 0000 4e6a 0203 0000 4e75  ...j....Nj....Nu
+00005850: 6261 6a03 0300 007d 9428 6a05 0300 005d  baj....}.(j....]
+00005860: 946a 0703 0000 5d94 6a09 0300 005d 946a  .j....].j....].j
+00005870: 0b03 0000 5d94 6a0d 0300 005d 9475 6a0f  ....].j....].uj.
+00005880: 0300 006a 2b05 0000 6aff 0200 006a a806  ...j+...j....j..
+00005890: 0000 6a00 0300 006a e902 0000 6a01 0300  ..j....j....j...
+000058a0: 004e 6a02 0300 004e 7562 6afa 0200 008c  .Nj....Nubj.....
+000058b0: 0229 2e94 8594 8194 7d94 286a ff02 0000  .)......}.(j....
+000058c0: 6aa8 0600 006a 0003 0000 6ae9 0200 006a  j....j....j....j
+000058d0: 0103 0000 4e6a 0203 0000 4e75 6265 6a03  ....Nj....Nubej.
+000058e0: 0300 007d 9428 6a05 0300 005d 946a 0703  ...}.(j....].j..
+000058f0: 0000 5d94 6a09 0300 005d 946a 0b03 0000  ..].j....].j....
+00005900: 5d94 6a0d 0300 005d 9475 6a0f 0300 006a  ].j....].uj....j
+00005910: 1205 0000 6aff 0200 006a a506 0000 7562  ....j....j....ub
+00005920: 616a 0303 0000 7d94 286a 0503 0000 5d94  aj....}.(j....].
+00005930: 6a07 0300 005d 946a 0903 0000 5d94 6a0b  j....].j....].j.
+00005940: 0300 005d 946a 0d03 0000 5d94 756a 0f03  ...].j....].uj..
+00005950: 0000 6a69 0500 006a ff02 0000 6a66 0500  ..ji...j....jf..
+00005960: 0075 626a 6a05 0000 2981 947d 9428 6aeb  .ubjj...)..}.(j.
+00005970: 0200 0068 406a ec02 0000 5d94 6a13 0500  ...h@j....].j...
+00005980: 0029 8194 7d94 286a eb02 0000 8c46 6361  .)..}.(j.....Fca
+00005990: 7374 5f73 7472 2028 626f 6f6c 2920 2d2d  st_str (bool) --
+000059a0: 2057 6865 7468 6572 2074 6f20 636f 6e76   Whether to conv
+000059b0: 6572 7420 6f75 7470 7574 2074 6f20 7374  ert output to st
+000059c0: 7269 6e67 2028 6465 6661 756c 7420 5472  ring (default Tr
+000059d0: 7565 292e 946a ec02 0000 5d94 286a 7305  ue)..j....].(js.
+000059e0: 0000 2981 947d 9428 6aeb 0200 008c 0863  ..)..}.(j......c
+000059f0: 6173 745f 7374 7294 6aec 0200 005d 946a  ast_str.j....].j
+00005a00: fa02 0000 8c08 6361 7374 5f73 7472 9485  ......cast_str..
+00005a10: 9481 947d 9428 6aff 0200 006a 0a07 0000  ...}.(j....j....
+00005a20: 6a00 0300 006a e902 0000 6a01 0300 004e  j....j....j....N
+00005a30: 6a02 0300 004e 7562 616a 0303 0000 7d94  j....Nubaj....}.
+00005a40: 286a 0503 0000 5d94 6a07 0300 005d 946a  (j....].j....].j
+00005a50: 0903 0000 5d94 6a0b 0300 005d 946a 0d03  ....].j....].j..
+00005a60: 0000 5d94 756a 0f03 0000 6a72 0500 006a  ..].uj....jr...j
+00005a70: ff02 0000 6a06 0700 0075 626a fa02 0000  ....j....ubj....
+00005a80: 8c02 2028 9485 9481 947d 9428 6aff 0200  .. (.....}.(j...
+00005a90: 006a 0607 0000 6a00 0300 006a e902 0000  .j....j....j....
+00005aa0: 6a01 0300 004e 6a02 0300 004e 7562 6a87  j....Nj....Nubj.
+00005ab0: 0500 0029 8194 7d94 286a eb02 0000 6840  ...)..}.(j....h@
+00005ac0: 6aec 0200 005d 946a 8c05 0000 2981 947d  j....].j....)..}
+00005ad0: 9428 6aeb 0200 008c 0462 6f6f 6c94 6aec  .(j......bool.j.
+00005ae0: 0200 005d 946a fa02 0000 8c04 626f 6f6c  ...].j......bool
+00005af0: 9485 9481 947d 9428 6aff 0200 006a 1f07  .....}.(j....j..
+00005b00: 0000 6a00 0300 006a e902 0000 6a01 0300  ..j....j....j...
+00005b10: 004e 6a02 0300 004e 7562 616a 0303 0000  .Nj....Nubaj....
+00005b20: 7d94 286a 0503 0000 5d94 6a07 0300 005d  }.(j....].j....]
+00005b30: 946a 0903 0000 5d94 6a0b 0300 005d 946a  .j....].j....].j
+00005b40: 0d03 0000 5d94 756a 0f03 0000 6a8b 0500  ....].uj....j...
+00005b50: 006a ff02 0000 6a1c 0700 0075 6261 6a03  .j....j....ubaj.
+00005b60: 0300 007d 9428 6a05 0300 005d 946a 0703  ...}.(j....].j..
+00005b70: 0000 5d94 6a09 0300 005d 946a 0b03 0000  ..].j....].j....
+00005b80: 5d94 6a0d 0300 005d 948c 0972 6566 646f  ].j....]...refdo
+00005b90: 6d61 696e 946a a205 0000 8c0b 7265 6665  main.j......refe
+00005ba0: 7870 6c69 6369 7494 898c 0772 6566 7479  xplicit....refty
+00005bb0: 7065 946a 6a02 0000 8c09 7265 6674 6172  pe.jj.....reftar
+00005bc0: 6765 7494 6a21 0700 006a a605 0000 886a  get.j!...j.....j
+00005bd0: a705 0000 6a07 0500 006a a805 0000 4e75  ....j....j....Nu
+00005be0: 6a0f 0300 006a 8605 0000 6aff 0200 006a  j....j....j....j
+00005bf0: 0607 0000 7562 6afa 0200 008c 0129 9485  ....ubj......)..
+00005c00: 9481 947d 9428 6aff 0200 006a 0607 0000  ...}.(j....j....
+00005c10: 6a00 0300 006a e902 0000 6a01 0300 004e  j....j....j....N
+00005c20: 6a02 0300 004e 7562 6afa 0200 008c 0520  j....Nubj...... 
+00005c30: e280 9320 9485 9481 947d 9428 6aff 0200  ... .....}.(j...
+00005c40: 006a 0607 0000 6a00 0300 006a e902 0000  .j....j....j....
+00005c50: 6a01 0300 004e 6a02 0300 004e 7562 6afa  j....Nj....Nubj.
+00005c60: 0200 008c 2d57 6865 7468 6572 2074 6f20  ....-Whether to 
+00005c70: 636f 6e76 6572 7420 6f75 7470 7574 2074  convert output t
+00005c80: 6f20 7374 7269 6e67 2028 6465 6661 756c  o string (defaul
+00005c90: 7420 9485 9481 947d 9428 6aff 0200 006a  t .....}.(j....j
+00005ca0: 0607 0000 6a00 0300 006a e902 0000 6a01  ....j....j....j.
+00005cb0: 0300 004e 6a02 0300 004e 7562 6a2c 0500  ...Nj....Nubj,..
+00005cc0: 0029 8194 7d94 286a eb02 0000 8c06 2a54  .)..}.(j......*T
+00005cd0: 7275 652a 946a ec02 0000 5d94 6afa 0200  rue*.j....].j...
+00005ce0: 008c 0454 7275 6594 8594 8194 7d94 286a  ...True.....}.(j
+00005cf0: ff02 0000 6a43 0700 006a 0003 0000 6ae9  ....jC...j....j.
+00005d00: 0200 006a 0103 0000 4e6a 0203 0000 4e75  ...j....Nj....Nu
+00005d10: 6261 6a03 0300 007d 9428 6a05 0300 005d  baj....}.(j....]
+00005d20: 946a 0703 0000 5d94 6a09 0300 005d 946a  .j....].j....].j
+00005d30: 0b03 0000 5d94 6a0d 0300 005d 9475 6a0f  ....].j....].uj.
+00005d40: 0300 006a 2b05 0000 6aff 0200 006a 0607  ...j+...j....j..
+00005d50: 0000 6a00 0300 006a e902 0000 6a01 0300  ..j....j....j...
+00005d60: 004e 6a02 0300 004e 7562 6afa 0200 008c  .Nj....Nubj.....
+00005d70: 0229 2e94 8594 8194 7d94 286a ff02 0000  .)......}.(j....
+00005d80: 6a06 0700 006a 0003 0000 6ae9 0200 006a  j....j....j....j
+00005d90: 0103 0000 4e6a 0203 0000 4e75 6265 6a03  ....Nj....Nubej.
+00005da0: 0300 007d 9428 6a05 0300 005d 946a 0703  ...}.(j....].j..
+00005db0: 0000 5d94 6a09 0300 005d 946a 0b03 0000  ..].j....].j....
+00005dc0: 5d94 6a0d 0300 005d 9475 6a0f 0300 006a  ].j....].uj....j
+00005dd0: 1205 0000 6aff 0200 006a 0307 0000 7562  ....j....j....ub
+00005de0: 616a 0303 0000 7d94 286a 0503 0000 5d94  aj....}.(j....].
+00005df0: 6a07 0300 005d 946a 0903 0000 5d94 6a0b  j....].j....].j.
+00005e00: 0300 005d 946a 0d03 0000 5d94 756a 0f03  ...].j....].uj..
+00005e10: 0000 6a69 0500 006a ff02 0000 6a66 0500  ..ji...j....jf..
+00005e20: 0075 626a 6a05 0000 2981 947d 9428 6aeb  .ubjj...)..}.(j.
+00005e30: 0200 0068 406a ec02 0000 5d94 6a13 0500  ...h@j....].j...
+00005e40: 0029 8194 7d94 286a eb02 0000 8c4d 666f  .)..}.(j.....Mfo
+00005e50: 726d 6174 5f6f 7574 2028 7374 7269 6e67  rmat_out (string
+00005e60: 2920 2d2d 2043 6f6e 7665 7273 696f 6e20  ) -- Conversion 
+00005e70: 666f 726d 6174 2066 6f72 206f 7574 7075  format for outpu
+00005e80: 7420 2864 6566 6175 6c74 2073 616d 6520  t (default same 
+00005e90: 746f 2066 6f72 6d61 7429 2e94 6aec 0200  to format)..j...
+00005ea0: 005d 9428 6a73 0500 0029 8194 7d94 286a  .].(js...)..}.(j
+00005eb0: eb02 0000 8c0a 666f 726d 6174 5f6f 7574  ......format_out
+00005ec0: 946a ec02 0000 5d94 6afa 0200 008c 0a66  .j....].j......f
+00005ed0: 6f72 6d61 745f 6f75 7494 8594 8194 7d94  ormat_out.....}.
+00005ee0: 286a ff02 0000 6a68 0700 006a 0003 0000  (j....jh...j....
+00005ef0: 6ae9 0200 006a 0103 0000 4e6a 0203 0000  j....j....Nj....
+00005f00: 4e75 6261 6a03 0300 007d 9428 6a05 0300  Nubaj....}.(j...
+00005f10: 005d 946a 0703 0000 5d94 6a09 0300 005d  .].j....].j....]
+00005f20: 946a 0b03 0000 5d94 6a0d 0300 005d 9475  .j....].j....].u
+00005f30: 6a0f 0300 006a 7205 0000 6aff 0200 006a  j....jr...j....j
+00005f40: 6407 0000 7562 6afa 0200 008c 0220 2894  d...ubj...... (.
+00005f50: 8594 8194 7d94 286a ff02 0000 6a64 0700  ....}.(j....jd..
+00005f60: 006a 0003 0000 6ae9 0200 006a 0103 0000  .j....j....j....
+00005f70: 4e6a 0203 0000 4e75 626a 8705 0000 2981  Nj....Nubj....).
+00005f80: 947d 9428 6aeb 0200 0068 406a ec02 0000  .}.(j....h@j....
+00005f90: 5d94 6a8c 0500 0029 8194 7d94 286a eb02  ].j....)..}.(j..
+00005fa0: 0000 8c06 7374 7269 6e67 946a ec02 0000  ....string.j....
+00005fb0: 5d94 6afa 0200 008c 0673 7472 696e 6794  ].j......string.
+00005fc0: 8594 8194 7d94 286a ff02 0000 6a7d 0700  ....}.(j....j}..
+00005fd0: 006a 0003 0000 6ae9 0200 006a 0103 0000  .j....j....j....
+00005fe0: 4e6a 0203 0000 4e75 6261 6a03 0300 007d  Nj....Nubaj....}
+00005ff0: 9428 6a05 0300 005d 946a 0703 0000 5d94  .(j....].j....].
+00006000: 6a09 0300 005d 946a 0b03 0000 5d94 6a0d  j....].j....].j.
+00006010: 0300 005d 9475 6a0f 0300 006a 8b05 0000  ...].uj....j....
+00006020: 6aff 0200 006a 7a07 0000 7562 616a 0303  j....jz...ubaj..
+00006030: 0000 7d94 286a 0503 0000 5d94 6a07 0300  ..}.(j....].j...
+00006040: 005d 946a 0903 0000 5d94 6a0b 0300 005d  .].j....].j....]
+00006050: 946a 0d03 0000 5d94 8c09 7265 6664 6f6d  .j....]...refdom
+00006060: 6169 6e94 6aa2 0500 008c 0b72 6566 6578  ain.j......refex
+00006070: 706c 6963 6974 9489 8c07 7265 6674 7970  plicit....reftyp
+00006080: 6594 6a6a 0200 008c 0972 6566 7461 7267  e.jj.....reftarg
+00006090: 6574 946a 7f07 0000 6aa6 0500 0088 6aa7  et.j....j.....j.
+000060a0: 0500 006a 0705 0000 6aa8 0500 004e 756a  ...j....j....Nuj
+000060b0: 0f03 0000 6a86 0500 006a ff02 0000 6a64  ....j....j....jd
+000060c0: 0700 0075 626a fa02 0000 8c01 2994 8594  ...ubj......)...
+000060d0: 8194 7d94 286a ff02 0000 6a64 0700 006a  ..}.(j....jd...j
+000060e0: 0003 0000 6ae9 0200 006a 0103 0000 4e6a  ....j....j....Nj
+000060f0: 0203 0000 4e75 626a fa02 0000 8c05 20e2  ....Nubj...... .
+00006100: 8093 2094 8594 8194 7d94 286a ff02 0000  .. .....}.(j....
+00006110: 6a64 0700 006a 0003 0000 6ae9 0200 006a  jd...j....j....j
+00006120: 0103 0000 4e6a 0203 0000 4e75 626a fa02  ....Nj....Nubj..
+00006130: 0000 8c2e 436f 6e76 6572 7369 6f6e 2066  ....Conversion f
+00006140: 6f72 6d61 7420 666f 7220 6f75 7470 7574  ormat for output
+00006150: 2028 6465 6661 756c 7420 7361 6d65 2074   (default same t
+00006160: 6f20 9485 9481 947d 9428 6aff 0200 006a  o .....}.(j....j
+00006170: 6407 0000 6a00 0300 006a e902 0000 6a01  d...j....j....j.
+00006180: 0300 004e 6a02 0300 004e 7562 6aee 0200  ...Nj....Nubj...
+00006190: 008c 0673 7472 6f6e 6794 9394 2981 947d  ...strong...)..}
+000061a0: 9428 6aeb 0200 008c 0a2a 2a66 6f72 6d61  .(j......**forma
+000061b0: 742a 2a94 6aec 0200 005d 946a fa02 0000  t**.j....].j....
+000061c0: 8c06 666f 726d 6174 9485 9481 947d 9428  ..format.....}.(
+000061d0: 6aff 0200 006a a307 0000 6a00 0300 006a  j....j....j....j
+000061e0: e902 0000 6a01 0300 004e 6a02 0300 004e  ....j....Nj....N
+000061f0: 7562 616a 0303 0000 7d94 286a 0503 0000  ubaj....}.(j....
+00006200: 5d94 6a07 0300 005d 946a 0903 0000 5d94  ].j....].j....].
+00006210: 6a0b 0300 005d 946a 0d03 0000 5d94 756a  j....].j....].uj
+00006220: 0f03 0000 6aa1 0700 006a ff02 0000 6a64  ....j....j....jd
+00006230: 0700 006a 0003 0000 6ae9 0200 006a 0103  ...j....j....j..
+00006240: 0000 4e6a 0203 0000 4e75 626a fa02 0000  ..Nj....Nubj....
+00006250: 8c02 292e 9485 9481 947d 9428 6aff 0200  ..)......}.(j...
+00006260: 006a 6407 0000 6a00 0300 006a e902 0000  .jd...j....j....
+00006270: 6a01 0300 004e 6a02 0300 004e 7562 656a  j....Nj....Nubej
+00006280: 0303 0000 7d94 286a 0503 0000 5d94 6a07  ....}.(j....].j.
+00006290: 0300 005d 946a 0903 0000 5d94 6a0b 0300  ...].j....].j...
+000062a0: 005d 946a 0d03 0000 5d94 756a 0f03 0000  .].j....].uj....
+000062b0: 6a12 0500 006a ff02 0000 6a61 0700 0075  j....j....ja...u
+000062c0: 6261 6a03 0300 007d 9428 6a05 0300 005d  baj....}.(j....]
+000062d0: 946a 0703 0000 5d94 6a09 0300 005d 946a  .j....].j....].j
+000062e0: 0b03 0000 5d94 6a0d 0300 005d 9475 6a0f  ....].j....].uj.
+000062f0: 0300 006a 6905 0000 6aff 0200 006a 6605  ...ji...j....jf.
+00006300: 0000 7562 656a 0303 0000 7d94 286a 0503  ..ubej....}.(j..
+00006310: 0000 5d94 6a07 0300 005d 946a 0903 0000  ..].j....].j....
+00006320: 5d94 6a0b 0300 005d 946a 0d03 0000 5d94  ].j....].j....].
+00006330: 756a 0f03 0000 6a64 0500 006a ff02 0000  uj....jd...j....
+00006340: 6a61 0500 0075 6261 6a03 0300 007d 9428  ja...ubaj....}.(
+00006350: 6a05 0300 005d 946a 0703 0000 5d94 6a09  j....].j....].j.
+00006360: 0300 005d 946a 0b03 0000 5d94 6a0d 0300  ...].j....].j...
+00006370: 005d 9475 6a0f 0300 006a 5f05 0000 6aff  .].uj....j_...j.
+00006380: 0200 006a 4c05 0000 7562 656a 0303 0000  ...jL...ubej....
+00006390: 7d94 286a 0503 0000 5d94 6a07 0300 005d  }.(j....].j....]
+000063a0: 946a 0903 0000 5d94 6a0b 0300 005d 946a  .j....].j....].j
+000063b0: 0d03 0000 5d94 756a 0f03 0000 6a4a 0500  ....].uj....jJ..
+000063c0: 006a ff02 0000 6a47 0500 0075 626a 4b05  .j....jG...ubjK.
+000063d0: 0000 2981 947d 9428 6aeb 0200 0068 406a  ..)..}.(j....h@j
+000063e0: ec02 0000 5d94 286a 5005 0000 2981 947d  ....].(jP...)..}
+000063f0: 9428 6aeb 0200 008c 0b52 6574 7572 6e20  .(j......Return 
+00006400: 7479 7065 946a ec02 0000 5d94 6afa 0200  type.j....].j...
+00006410: 008c 0b52 6574 7572 6e20 7479 7065 9485  ...Return type..
+00006420: 9481 947d 9428 6aff 0200 006a d607 0000  ...}.(j....j....
+00006430: 6a00 0300 006a e902 0000 6a01 0300 004e  j....j....j....N
+00006440: 6a02 0300 004e 7562 616a 0303 0000 7d94  j....Nubaj....}.
+00006450: 286a 0503 0000 5d94 6a07 0300 005d 946a  (j....].j....].j
+00006460: 0903 0000 5d94 6a0b 0300 005d 946a 0d03  ....].j....].j..
+00006470: 0000 5d94 756a 0f03 0000 6a4f 0500 006a  ..].uj....jO...j
+00006480: ff02 0000 6ad3 0700 006a 0103 0000 6a62  ....j....j....jb
+00006490: 0300 006a 0203 0000 4b00 7562 6a60 0500  ...j....K.ubj`..
+000064a0: 0029 8194 7d94 286a eb02 0000 6840 6aec  .)..}.(j....h@j.
+000064b0: 0200 005d 946a 1305 0000 2981 947d 9428  ...].j....)..}.(
+000064c0: 6aeb 0200 008c 3d6c 6973 7420 286f 7220  j.....=list (or 
+000064d0: 6765 6e65 7261 746f 7220 6974 6572 6174  generator iterat
+000064e0: 6f72 2920 6f66 2073 7472 696e 6720 286f  or) of string (o
+000064f0: 7220 6461 7465 7469 6d65 2e64 6174 6574  r datetime.datet
+00006500: 696d 6529 946a ec02 0000 5d94 286a 8705  ime).j....].(j..
+00006510: 0000 2981 947d 9428 6aeb 0200 0068 406a  ..)..}.(j....h@j
+00006520: ec02 0000 5d94 6afa 0200 008c 046c 6973  ....].j......lis
+00006530: 7494 8594 8194 7d94 286a ff02 0000 6aeb  t.....}.(j....j.
+00006540: 0700 006a 0003 0000 6ae9 0200 006a 0103  ...j....j....j..
+00006550: 0000 4e6a 0203 0000 4e75 6261 6a03 0300  ..Nj....Nubaj...
+00006560: 007d 9428 6a05 0300 005d 946a 0703 0000  .}.(j....].j....
+00006570: 5d94 6a09 0300 005d 946a 0b03 0000 5d94  ].j....].j....].
+00006580: 6a0d 0300 005d 948c 0972 6566 646f 6d61  j....]...refdoma
+00006590: 696e 946a a205 0000 8c0b 7265 6665 7870  in.j......refexp
+000065a0: 6c69 6369 7494 898c 0772 6566 7479 7065  licit....reftype
+000065b0: 946a 6a02 0000 8c09 7265 6674 6172 6765  .jj.....reftarge
+000065c0: 7494 8c04 6c69 7374 946a a605 0000 886a  t...list.j.....j
+000065d0: a705 0000 6a07 0500 006a a805 0000 4e75  ....j....j....Nu
+000065e0: 6a0f 0300 006a 8605 0000 6aff 0200 006a  j....j....j....j
+000065f0: e707 0000 7562 6afa 0200 008c 0520 286f  ....ubj...... (o
+00006600: 7220 9485 9481 947d 9428 6aff 0200 006a  r .....}.(j....j
+00006610: e707 0000 6a00 0300 006a e902 0000 6a01  ....j....j....j.
+00006620: 0300 004e 6a02 0300 004e 7562 6a87 0500  ...Nj....Nubj...
+00006630: 0029 8194 7d94 286a eb02 0000 6840 6aec  .)..}.(j....h@j.
+00006640: 0200 005d 946a fa02 0000 8c12 6765 6e65  ...].j......gene
+00006650: 7261 746f 7220 6974 6572 6174 6f72 9485  rator iterator..
+00006660: 9481 947d 9428 6aff 0200 006a 0108 0000  ...}.(j....j....
+00006670: 6a00 0300 006a e902 0000 6a01 0300 004e  j....j....j....N
+00006680: 6a02 0300 004e 7562 616a 0303 0000 7d94  j....Nubaj....}.
+00006690: 286a 0503 0000 5d94 6a07 0300 005d 946a  (j....].j....].j
+000066a0: 0903 0000 5d94 6a0b 0300 005d 946a 0d03  ....].j....].j..
+000066b0: 0000 5d94 8c09 7265 6664 6f6d 6169 6e94  ..]...refdomain.
+000066c0: 6aa2 0500 008c 0b72 6566 6578 706c 6963  j......refexplic
+000066d0: 6974 9489 8c07 7265 6674 7970 6594 6a6a  it....reftype.jj
+000066e0: 0200 008c 0972 6566 7461 7267 6574 948c  .....reftarget..
+000066f0: 1267 656e 6572 6174 6f72 2069 7465 7261  .generator itera
+00006700: 746f 7294 6aa6 0500 0088 6aa7 0500 006a  tor.j.....j....j
+00006710: 0705 0000 6aa8 0500 004e 756a 0f03 0000  ....j....Nuj....
+00006720: 6a86 0500 006a ff02 0000 6ae7 0700 0075  j....j....j....u
+00006730: 626a fa02 0000 8c05 2920 6f66 2094 8594  bj......) of ...
+00006740: 8194 7d94 286a ff02 0000 6ae7 0700 006a  ..}.(j....j....j
+00006750: 0003 0000 6ae9 0200 006a 0103 0000 4e6a  ....j....j....Nj
+00006760: 0203 0000 4e75 626a 8705 0000 2981 947d  ....Nubj....)..}
+00006770: 9428 6aeb 0200 0068 406a ec02 0000 5d94  .(j....h@j....].
+00006780: 6afa 0200 008c 0673 7472 696e 6794 8594  j......string...
+00006790: 8194 7d94 286a ff02 0000 6a17 0800 006a  ..}.(j....j....j
+000067a0: 0003 0000 6ae9 0200 006a 0103 0000 4e6a  ....j....j....Nj
+000067b0: 0203 0000 4e75 6261 6a03 0300 007d 9428  ....Nubaj....}.(
+000067c0: 6a05 0300 005d 946a 0703 0000 5d94 6a09  j....].j....].j.
+000067d0: 0300 005d 946a 0b03 0000 5d94 6a0d 0300  ...].j....].j...
+000067e0: 005d 948c 0972 6566 646f 6d61 696e 946a  .]...refdomain.j
+000067f0: a205 0000 8c0b 7265 6665 7870 6c69 6369  ......refexplici
+00006800: 7494 898c 0772 6566 7479 7065 946a 6a02  t....reftype.jj.
+00006810: 0000 8c09 7265 6674 6172 6765 7494 8c06  ....reftarget...
+00006820: 7374 7269 6e67 946a a605 0000 886a a705  string.j.....j..
+00006830: 0000 6a07 0500 006a a805 0000 4e75 6a0f  ..j....j....Nuj.
+00006840: 0300 006a 8605 0000 6aff 0200 006a e707  ...j....j....j..
+00006850: 0000 7562 6afa 0200 008c 0520 286f 7220  ..ubj...... (or 
+00006860: 9485 9481 947d 946a ff02 0000 6ae7 0700  .....}.j....j...
+00006870: 0073 626a 8705 0000 2981 947d 9428 6aeb  .sbj....)..}.(j.
+00006880: 0200 0068 406a ec02 0000 5d94 6afa 0200  ...h@j....].j...
+00006890: 008c 1164 6174 6574 696d 652e 6461 7465  ...datetime.date
+000068a0: 7469 6d65 9485 9481 947d 9428 6aff 0200  time.....}.(j...
+000068b0: 006a 2d08 0000 6a00 0300 006a e902 0000  .j-...j....j....
+000068c0: 6a01 0300 004e 6a02 0300 004e 7562 616a  j....Nj....Nubaj
+000068d0: 0303 0000 7d94 286a 0503 0000 5d94 6a07  ....}.(j....].j.
+000068e0: 0300 005d 946a 0903 0000 5d94 6a0b 0300  ...].j....].j...
+000068f0: 005d 946a 0d03 0000 5d94 8c09 7265 6664  .].j....]...refd
+00006900: 6f6d 6169 6e94 6aa2 0500 008c 0b72 6566  omain.j......ref
+00006910: 6578 706c 6963 6974 9489 8c07 7265 6674  explicit....reft
+00006920: 7970 6594 6a6a 0200 008c 0972 6566 7461  ype.jj.....refta
+00006930: 7267 6574 948c 1164 6174 6574 696d 652e  rget...datetime.
+00006940: 6461 7465 7469 6d65 946a a605 0000 886a  datetime.j.....j
+00006950: a705 0000 6a07 0500 006a a805 0000 4e75  ....j....j....Nu
+00006960: 6a0f 0300 006a 8605 0000 6aff 0200 006a  j....j....j....j
+00006970: e707 0000 7562 6afa 0200 008c 0129 9485  ....ubj......)..
+00006980: 9481 947d 9428 6aff 0200 006a e707 0000  ...}.(j....j....
+00006990: 6a00 0300 006a e902 0000 6a01 0300 004e  j....j....j....N
+000069a0: 6a02 0300 004e 7562 656a 0303 0000 7d94  j....Nubej....}.
+000069b0: 286a 0503 0000 5d94 6a07 0300 005d 946a  (j....].j....].j
+000069c0: 0903 0000 5d94 6a0b 0300 005d 946a 0d03  ....].j....].j..
+000069d0: 0000 5d94 756a 0f03 0000 6a12 0500 006a  ..].uj....j....j
+000069e0: ff02 0000 6ae4 0700 0075 6261 6a03 0300  ....j....ubaj...
+000069f0: 007d 9428 6a05 0300 005d 946a 0703 0000  .}.(j....].j....
+00006a00: 5d94 6a09 0300 005d 946a 0b03 0000 5d94  ].j....].j....].
+00006a10: 6a0d 0300 005d 9475 6a0f 0300 006a 5f05  j....].uj....j_.
+00006a20: 0000 6aff 0200 006a d307 0000 7562 656a  ..j....j....ubej
+00006a30: 0303 0000 7d94 286a 0503 0000 5d94 6a07  ....}.(j....].j.
+00006a40: 0300 005d 946a 0903 0000 5d94 6a0b 0300  ...].j....].j...
+00006a50: 005d 946a 0d03 0000 5d94 756a 0f03 0000  .].j....].uj....
+00006a60: 6a4a 0500 006a ff02 0000 6a47 0500 0075  jJ...j....jG...u
+00006a70: 6265 6a03 0300 007d 9428 6a05 0300 005d  bej....}.(j....]
+00006a80: 946a 0703 0000 5d94 6a09 0300 005d 946a  .j....].j....].j
+00006a90: 0b03 0000 5d94 6a0d 0300 005d 9475 6a0f  ....].j....].uj.
+00006aa0: 0300 006a 4505 0000 6aff 0200 006a 0f05  ...jE...j....j..
+00006ab0: 0000 6a00 0300 006a e902 0000 6a01 0300  ..j....j....j...
+00006ac0: 004e 6a02 0300 004e 7562 656a 0303 0000  .Nj....Nubej....
+00006ad0: 7d94 286a 0503 0000 5d94 6a07 0300 005d  }.(j....].j....]
+00006ae0: 946a 0903 0000 5d94 6a0b 0300 005d 946a  .j....].j....].j
+00006af0: 0d03 0000 5d94 756a 0f03 0000 6a0d 0500  ....].uj....j...
+00006b00: 006a ff02 0000 6a45 0300 006a 0003 0000  .j....jE...j....
+00006b10: 6ae9 0200 006a 0103 0000 6a62 0300 006a  j....j....jb...j
+00006b20: 0203 0000 4b01 7562 656a 0303 0000 7d94  ....K.ubej....}.
+00006b30: 286a 0503 0000 5d94 6a07 0300 005d 9428  (j....].j....].(
+00006b40: 6aa2 0500 008c 0866 756e 6374 696f 6e94  j......function.
+00006b50: 656a 0903 0000 5d94 6a0b 0300 005d 946a  ej....].j....].j
+00006b60: 0d03 0000 5d94 6873 6aa2 0500 008c 076f  ....].hsj......o
+00006b70: 626a 7479 7065 946a 6408 0000 8c08 6465  bjtype.jd.....de
+00006b80: 7363 7479 7065 946a 6408 0000 8c07 6e6f  sctype.jd.....no
+00006b90: 696e 6465 7894 898c 0c6e 6f69 6e64 6578  index....noindex
+00006ba0: 656e 7472 7994 898c 0f6e 6f63 6f6e 7465  entry....noconte
+00006bb0: 6e74 7365 6e74 7279 9489 756a 0f03 0000  ntsentry..uj....
+00006bc0: 6a43 0300 006a 0003 0000 6ae9 0200 006a  jC...j....j....j
+00006bd0: ff02 0000 6a22 0300 006a 0103 0000 4e6a  ....j"...j....Nj
+00006be0: 0203 0000 4e75 626a 1305 0000 2981 947d  ....Nubj....)..}
+00006bf0: 9428 6aeb 0200 008c 0b2a 2a45 7861 6d70  .(j......**Examp
+00006c00: 6c65 2a2a 946a ec02 0000 5d94 6aa2 0700  le**.j....].j...
+00006c10: 0029 8194 7d94 286a eb02 0000 6a6f 0800  .)..}.(j....jo..
+00006c20: 006a ec02 0000 5d94 6afa 0200 008c 0745  .j....].j......E
+00006c30: 7861 6d70 6c65 9485 9481 947d 9428 6aff  xample.....}.(j.
+00006c40: 0200 006a 7108 0000 6a00 0300 006a e902  ...jq...j....j..
+00006c50: 0000 6a01 0300 004e 6a02 0300 004e 7562  ..j....Nj....Nub
+00006c60: 616a 0303 0000 7d94 286a 0503 0000 5d94  aj....}.(j....].
+00006c70: 6a07 0300 005d 946a 0903 0000 5d94 6a0b  j....].j....].j.
+00006c80: 0300 005d 946a 0d03 0000 5d94 756a 0f03  ...].j....].uj..
+00006c90: 0000 6aa1 0700 006a ff02 0000 6a6d 0800  ..j....j....jm..
+00006ca0: 0075 6261 6a03 0300 007d 9428 6a05 0300  .ubaj....}.(j...
+00006cb0: 005d 946a 0703 0000 5d94 6a09 0300 005d  .].j....].j....]
+00006cc0: 946a 0b03 0000 5d94 6a0d 0300 005d 9475  .j....].j....].u
+00006cd0: 6a0f 0300 006a 1205 0000 6a01 0300 006a  j....j....j....j
+00006ce0: 1003 0000 6a02 0300 004b 0c6a ff02 0000  ....j....K.j....
+00006cf0: 6a22 0300 006a 0003 0000 6ae9 0200 0075  j"...j....j....u
+00006d00: 626a 1305 0000 2981 947d 9428 6aeb 0200  bj....)..}.(j...
+00006d10: 008c 2641 6e20 6578 616d 706c 6520 6f66  ..&An example of
+00006d20: 2069 6e63 7265 6d65 6e74 696e 6720 6279   incrementing by
+00006d30: 206f 6e65 2064 6179 2e94 6aec 0200 005d   one day..j....]
+00006d40: 946a fa02 0000 8c26 416e 2065 7861 6d70  .j.....&An examp
+00006d50: 6c65 206f 6620 696e 6372 656d 656e 7469  le of incrementi
+00006d60: 6e67 2062 7920 6f6e 6520 6461 792e 9485  ng by one day...
+00006d70: 9481 947d 9428 6aff 0200 006a 8408 0000  ...}.(j....j....
+00006d80: 6a00 0300 006a e902 0000 6a01 0300 004e  j....j....j....N
+00006d90: 6a02 0300 004e 7562 616a 0303 0000 7d94  j....Nubaj....}.
+00006da0: 286a 0503 0000 5d94 6a07 0300 005d 946a  (j....].j....].j
+00006db0: 0903 0000 5d94 6a0b 0300 005d 946a 0d03  ....].j....].j..
+00006dc0: 0000 5d94 756a 0f03 0000 6a12 0500 006a  ..].uj....j....j
+00006dd0: 0103 0000 6a10 0300 006a 0203 0000 4b0e  ....j....j....K.
+00006de0: 6aff 0200 006a 2203 0000 6a00 0300 006a  j....j"...j....j
+00006df0: e902 0000 7562 6aee 0200 008c 0d6c 6974  ....ubj......lit
+00006e00: 6572 616c 5f62 6c6f 636b 9493 9429 8194  eral_block...)..
+00006e10: 7d94 286a eb02 0000 8cac 696d 706f 7274  }.(j......import
+00006e20: 2063 6f6f 6b69 6573 5f75 7469 6c69 7469   cookies_utiliti
+00006e30: 6573 2061 7320 6375 0a64 6174 6573 203d  es as cu.dates =
+00006e40: 2063 752e 6765 745f 6461 7465 7328 0a20   cu.get_dates(. 
+00006e50: 2020 2073 7461 7274 3d27 3230 3136 2f30     start='2016/0
+00006e60: 372f 3031 272c 2065 6e64 3d27 3230 3136  7/01', end='2016
+00006e70: 2f30 372f 3033 272c 2066 6f72 6d61 743d  /07/03', format=
+00006e80: 2725 592f 256d 2f25 6427 2c0a 2020 2020  '%Y/%m/%d',.    
+00006e90: 6465 6c74 613d 7b27 6461 7973 273a 2031  delta={'days': 1
+00006ea0: 7d2c 2066 6f72 6d61 745f 6f75 743d 2725  }, format_out='%
+00006eb0: 592d 256d 2d25 6427 290a 7072 696e 7428  Y-%m-%d').print(
+00006ec0: 6461 7465 7329 946a ec02 0000 5d94 6afa  dates).j....].j.
+00006ed0: 0200 008c ac69 6d70 6f72 7420 636f 6f6b  .....import cook
+00006ee0: 6965 735f 7574 696c 6974 6965 7320 6173  ies_utilities as
+00006ef0: 2063 750a 6461 7465 7320 3d20 6375 2e67   cu.dates = cu.g
+00006f00: 6574 5f64 6174 6573 280a 2020 2020 7374  et_dates(.    st
+00006f10: 6172 743d 2732 3031 362f 3037 2f30 3127  art='2016/07/01'
+00006f20: 2c20 656e 643d 2732 3031 362f 3037 2f30  , end='2016/07/0
+00006f30: 3327 2c20 666f 726d 6174 3d27 2559 2f25  3', format='%Y/%
+00006f40: 6d2f 2564 272c 0a20 2020 2064 656c 7461  m/%d',.    delta
+00006f50: 3d7b 2764 6179 7327 3a20 317d 2c20 666f  ={'days': 1}, fo
+00006f60: 726d 6174 5f6f 7574 3d27 2559 2d25 6d2d  rmat_out='%Y-%m-
+00006f70: 2564 2729 0a70 7269 6e74 2864 6174 6573  %d').print(dates
+00006f80: 2994 8594 8194 7d94 6aff 0200 006a 9408  ).....}.j....j..
+00006f90: 0000 7362 616a 0303 0000 7d94 286a 0503  ..sbaj....}.(j..
+00006fa0: 0000 5d94 6a07 0300 005d 946a 0903 0000  ..].j....].j....
+00006fb0: 5d94 6a0b 0300 005d 946a 0d03 0000 5d94  ].j....].j....].
+00006fc0: 6a60 0300 006a 6103 0000 8c05 666f 7263  j`...ja.....forc
+00006fd0: 6594 8968 4b8c 0670 7974 686f 6e94 8c0e  e..hK..python...
+00006fe0: 6869 6768 6c69 6768 745f 6172 6773 947d  highlight_args.}
+00006ff0: 9475 6a0f 0300 006a 9208 0000 6a01 0300  .uj....j....j...
+00007000: 006a 1003 0000 6a02 0300 004b 106a ff02  .j....j....K.j..
+00007010: 0000 6a22 0300 006a 0003 0000 6ae9 0200  ..j"...j....j...
+00007020: 0075 626a 9308 0000 2981 947d 9428 6aeb  .ubj....)..}.(j.
+00007030: 0200 008c 2a5b 2732 3031 362d 3037 2d30  ....*['2016-07-0
+00007040: 3127 2c20 2732 3031 362d 3037 2d30 3227  1', '2016-07-02'
+00007050: 2c20 2732 3031 362d 3037 2d30 3327 5d94  , '2016-07-03'].
+00007060: 6aec 0200 005d 946a fa02 0000 8c2a 5b27  j....].j.....*['
+00007070: 3230 3136 2d30 372d 3031 272c 2027 3230  2016-07-01', '20
+00007080: 3136 2d30 372d 3032 272c 2027 3230 3136  16-07-02', '2016
+00007090: 2d30 372d 3033 275d 9485 9481 947d 946a  -07-03'].....}.j
+000070a0: ff02 0000 6aa6 0800 0073 6261 6a03 0300  ....j....sbaj...
+000070b0: 007d 9428 6a05 0300 005d 946a 0703 0000  .}.(j....].j....
+000070c0: 5d94 6a09 0300 005d 946a 0b03 0000 5d94  ].j....].j....].
+000070d0: 6a0d 0300 005d 946a 6003 0000 6a61 0300  j....].j`...ja..
+000070e0: 006a a208 0000 8968 4b8c 0763 6f6e 736f  .j.....hK..conso
+000070f0: 6c65 946a a408 0000 7d94 756a 0f03 0000  le.j....}.uj....
+00007100: 6a92 0800 006a 0103 0000 6a10 0300 006a  j....j....j....j
+00007110: 0203 0000 4b18 6aff 0200 006a 2203 0000  ....K.j....j"...
+00007120: 6a00 0300 006a e902 0000 7562 6a13 0500  j....j....ubj...
+00007130: 0029 8194 7d94 286a eb02 0000 8c29 416e  .)..}.(j.....)An
+00007140: 2065 7861 6d70 6c65 206f 6620 696e 6372   example of incr
+00007150: 656d 656e 7469 6e67 2062 7920 3230 206d  ementing by 20 m
+00007160: 696e 7574 6573 2e94 6aec 0200 005d 946a  inutes..j....].j
+00007170: fa02 0000 8c29 416e 2065 7861 6d70 6c65  .....)An example
+00007180: 206f 6620 696e 6372 656d 656e 7469 6e67   of incrementing
+00007190: 2062 7920 3230 206d 696e 7574 6573 2e94   by 20 minutes..
+000071a0: 8594 8194 7d94 286a ff02 0000 6ab6 0800  ....}.(j....j...
+000071b0: 006a 0003 0000 6ae9 0200 006a 0103 0000  .j....j....j....
+000071c0: 4e6a 0203 0000 4e75 6261 6a03 0300 007d  Nj....Nubaj....}
+000071d0: 9428 6a05 0300 005d 946a 0703 0000 5d94  .(j....].j....].
+000071e0: 6a09 0300 005d 946a 0b03 0000 5d94 6a0d  j....].j....].j.
+000071f0: 0300 005d 9475 6a0f 0300 006a 1205 0000  ...].uj....j....
+00007200: 6a01 0300 006a 1003 0000 6a02 0300 004b  j....j....j....K
+00007210: 1c6a ff02 0000 6a22 0300 006a 0003 0000  .j....j"...j....
+00007220: 6ae9 0200 0075 626a 9308 0000 2981 947d  j....ubj....)..}
+00007230: 9428 6aeb 0200 008c b869 6d70 6f72 7420  .(j......import 
+00007240: 636f 6f6b 6965 735f 7574 696c 6974 6965  cookies_utilitie
+00007250: 7320 6173 2063 750a 6461 7465 7320 3d20  s as cu.dates = 
+00007260: 6375 2e67 6574 5f64 6174 6573 280a 2020  cu.get_dates(.  
+00007270: 2020 7374 6172 743d 2732 3031 362d 3037    start='2016-07
+00007280: 2d30 3120 3032 3a30 303a 3030 272c 2065  -01 02:00:00', e
+00007290: 6e64 3d27 3230 3136 2d30 372d 3031 2030  nd='2016-07-01 0
+000072a0: 333a 3030 3a30 3027 2c0a 2020 2020 666f  3:00:00',.    fo
+000072b0: 726d 6174 3d27 2559 2d25 6d2d 2564 2025  rmat='%Y-%m-%d %
+000072c0: 483a 254d 3a25 5327 2c0a 2020 2020 6465  H:%M:%S',.    de
+000072d0: 6c74 613d 7b27 6d69 6e75 7465 7327 3a20  lta={'minutes': 
+000072e0: 3230 7d29 0a70 7269 6e74 2864 6174 6573  20}).print(dates
+000072f0: 2994 6aec 0200 005d 946a fa02 0000 8cb8  ).j....].j......
+00007300: 696d 706f 7274 2063 6f6f 6b69 6573 5f75  import cookies_u
+00007310: 7469 6c69 7469 6573 2061 7320 6375 0a64  tilities as cu.d
+00007320: 6174 6573 203d 2063 752e 6765 745f 6461  ates = cu.get_da
+00007330: 7465 7328 0a20 2020 2073 7461 7274 3d27  tes(.    start='
+00007340: 3230 3136 2d30 372d 3031 2030 323a 3030  2016-07-01 02:00
+00007350: 3a30 3027 2c20 656e 643d 2732 3031 362d  :00', end='2016-
+00007360: 3037 2d30 3120 3033 3a30 303a 3030 272c  07-01 03:00:00',
+00007370: 0a20 2020 2066 6f72 6d61 743d 2725 592d  .    format='%Y-
+00007380: 256d 2d25 6420 2548 3a25 4d3a 2553 272c  %m-%d %H:%M:%S',
+00007390: 0a20 2020 2064 656c 7461 3d7b 276d 696e  .    delta={'min
+000073a0: 7574 6573 273a 2032 307d 290a 7072 696e  utes': 20}).prin
+000073b0: 7428 6461 7465 7329 9485 9481 947d 946a  t(dates).....}.j
+000073c0: ff02 0000 6ac4 0800 0073 6261 6a03 0300  ....j....sbaj...
+000073d0: 007d 9428 6a05 0300 005d 946a 0703 0000  .}.(j....].j....
+000073e0: 5d94 6a09 0300 005d 946a 0b03 0000 5d94  ].j....].j....].
+000073f0: 6a0d 0300 005d 946a 6003 0000 6a61 0300  j....].j`...ja..
+00007400: 006a a208 0000 8968 4b8c 0670 7974 686f  .j.....hK..pytho
+00007410: 6e94 6aa4 0800 007d 9475 6a0f 0300 006a  n.j....}.uj....j
+00007420: 9208 0000 6a01 0300 006a 1003 0000 6a02  ....j....j....j.
+00007430: 0300 004b 1e6a ff02 0000 6a22 0300 006a  ...K.j....j"...j
+00007440: 0003 0000 6ae9 0200 0075 626a 9308 0000  ....j....ubj....
+00007450: 2981 947d 9428 6aeb 0200 008c 5c5b 2732  )..}.(j.....\['2
+00007460: 3031 362d 3037 2d30 3120 3032 3a30 303a  016-07-01 02:00:
+00007470: 3030 272c 2027 3230 3136 2d30 372d 3031  00', '2016-07-01
+00007480: 2030 323a 3230 3a30 3027 2c20 2732 3031   02:20:00', '201
+00007490: 362d 3037 2d30 3120 3032 3a34 303a 3030  6-07-01 02:40:00
+000074a0: 272c 2027 3230 3136 2d30 372d 3031 2030  ', '2016-07-01 0
+000074b0: 333a 3030 3a30 3027 5d94 6aec 0200 005d  3:00:00'].j....]
+000074c0: 946a fa02 0000 8c5c 5b27 3230 3136 2d30  .j.....\['2016-0
+000074d0: 372d 3031 2030 323a 3030 3a30 3027 2c20  7-01 02:00:00', 
+000074e0: 2732 3031 362d 3037 2d30 3120 3032 3a32  '2016-07-01 02:2
+000074f0: 303a 3030 272c 2027 3230 3136 2d30 372d  0:00', '2016-07-
+00007500: 3031 2030 323a 3430 3a30 3027 2c20 2732  01 02:40:00', '2
+00007510: 3031 362d 3037 2d30 3120 3033 3a30 303a  016-07-01 03:00:
+00007520: 3030 275d 9485 9481 947d 946a ff02 0000  00'].....}.j....
+00007530: 6ad4 0800 0073 6261 6a03 0300 007d 9428  j....sbaj....}.(
+00007540: 6a05 0300 005d 946a 0703 0000 5d94 6a09  j....].j....].j.
+00007550: 0300 005d 946a 0b03 0000 5d94 6a0d 0300  ...].j....].j...
+00007560: 005d 946a 6003 0000 6a61 0300 006a a208  .].j`...ja...j..
+00007570: 0000 8968 4b8c 0763 6f6e 736f 6c65 946a  ...hK..console.j
+00007580: a408 0000 7d94 756a 0f03 0000 6a92 0800  ....}.uj....j...
+00007590: 006a 0103 0000 6a10 0300 006a 0203 0000  .j....j....j....
+000075a0: 4b27 6aff 0200 006a 2203 0000 6a00 0300  K'j....j"...j...
+000075b0: 006a e902 0000 7562 6a13 0500 0029 8194  .j....ubj....)..
+000075c0: 7d94 286a eb02 0000 8c31 416e 2065 7861  }.(j.....1An exa
+000075d0: 6d70 6c65 206f 6620 7265 7472 6965 7669  mple of retrievi
+000075e0: 6e67 2061 7320 6120 6765 6e65 7261 746f  ng as a generato
+000075f0: 7220 6974 6572 6174 6f72 2e94 6aec 0200  r iterator..j...
+00007600: 005d 946a fa02 0000 8c31 416e 2065 7861  .].j.....1An exa
+00007610: 6d70 6c65 206f 6620 7265 7472 6965 7669  mple of retrievi
+00007620: 6e67 2061 7320 6120 6765 6e65 7261 746f  ng as a generato
+00007630: 7220 6974 6572 6174 6f72 2e94 8594 8194  r iterator......
+00007640: 7d94 286a ff02 0000 6ae4 0800 006a 0003  }.(j....j....j..
+00007650: 0000 6ae9 0200 006a 0103 0000 4e6a 0203  ..j....j....Nj..
+00007660: 0000 4e75 6261 6a03 0300 007d 9428 6a05  ..Nubaj....}.(j.
+00007670: 0300 005d 946a 0703 0000 5d94 6a09 0300  ...].j....].j...
+00007680: 005d 946a 0b03 0000 5d94 6a0d 0300 005d  .].j....].j....]
+00007690: 9475 6a0f 0300 006a 1205 0000 6a01 0300  .uj....j....j...
+000076a0: 006a 1003 0000 6a02 0300 004b 2b6a ff02  .j....j....K+j..
+000076b0: 0000 6a22 0300 006a 0003 0000 6ae9 0200  ..j"...j....j...
+000076c0: 0075 626a 9308 0000 2981 947d 9428 6aeb  .ubj....)..}.(j.
+000076d0: 0200 008c cc69 6d70 6f72 7420 636f 6f6b  .....import cook
+000076e0: 6965 735f 7574 696c 6974 6965 7320 6173  ies_utilities as
+000076f0: 2063 750a 6461 7465 7320 3d20 6375 2e67   cu.dates = cu.g
+00007700: 6574 5f64 6174 6573 280a 2020 2020 7374  et_dates(.    st
+00007710: 6172 743d 2732 3031 362f 3037 2f30 3127  art='2016/07/01'
+00007720: 2c20 656e 643d 2732 3031 362f 3037 2f30  , end='2016/07/0
+00007730: 3327 2c20 666f 726d 6174 3d27 2559 2f25  3', format='%Y/%
+00007740: 6d2f 2564 272c 0a20 2020 2064 656c 7461  m/%d',.    delta
+00007750: 3d7b 2764 6179 7327 3a20 317d 2c20 6765  ={'days': 1}, ge
+00007760: 6e69 7465 723d 5472 7565 290a 7072 696e  niter=True).prin
+00007770: 7428 7479 7065 2864 6174 6573 2929 0a66  t(type(dates)).f
+00007780: 6f72 2064 6174 6520 696e 2064 6174 6573  or date in dates
+00007790: 3a0a 2020 2020 7072 696e 7428 6461 7465  :.    print(date
+000077a0: 2994 6aec 0200 005d 946a fa02 0000 8ccc  ).j....].j......
+000077b0: 696d 706f 7274 2063 6f6f 6b69 6573 5f75  import cookies_u
+000077c0: 7469 6c69 7469 6573 2061 7320 6375 0a64  tilities as cu.d
+000077d0: 6174 6573 203d 2063 752e 6765 745f 6461  ates = cu.get_da
+000077e0: 7465 7328 0a20 2020 2073 7461 7274 3d27  tes(.    start='
+000077f0: 3230 3136 2f30 372f 3031 272c 2065 6e64  2016/07/01', end
+00007800: 3d27 3230 3136 2f30 372f 3033 272c 2066  ='2016/07/03', f
+00007810: 6f72 6d61 743d 2725 592f 256d 2f25 6427  ormat='%Y/%m/%d'
+00007820: 2c0a 2020 2020 6465 6c74 613d 7b27 6461  ,.    delta={'da
+00007830: 7973 273a 2031 7d2c 2067 656e 6974 6572  ys': 1}, geniter
+00007840: 3d54 7275 6529 0a70 7269 6e74 2874 7970  =True).print(typ
+00007850: 6528 6461 7465 7329 290a 666f 7220 6461  e(dates)).for da
+00007860: 7465 2069 6e20 6461 7465 733a 0a20 2020  te in dates:.   
+00007870: 2070 7269 6e74 2864 6174 6529 9485 9481   print(date)....
+00007880: 947d 946a ff02 0000 6af2 0800 0073 6261  .}.j....j....sba
+00007890: 6a03 0300 007d 9428 6a05 0300 005d 946a  j....}.(j....].j
+000078a0: 0703 0000 5d94 6a09 0300 005d 946a 0b03  ....].j....].j..
+000078b0: 0000 5d94 6a0d 0300 005d 946a 6003 0000  ..].j....].j`...
+000078c0: 6a61 0300 006a a208 0000 8968 4b8c 0670  ja...j.....hK..p
+000078d0: 7974 686f 6e94 6aa4 0800 007d 9475 6a0f  ython.j....}.uj.
+000078e0: 0300 006a 9208 0000 6a01 0300 006a 1003  ...j....j....j..
+000078f0: 0000 6a02 0300 004b 2d6a ff02 0000 6a22  ..j....K-j....j"
+00007900: 0300 006a 0003 0000 6ae9 0200 0075 626a  ...j....j....ubj
+00007910: 9308 0000 2981 947d 9428 6aeb 0200 008c  ....)..}.(j.....
+00007920: 343c 636c 6173 7320 2767 656e 6572 6174  4<class 'generat
+00007930: 6f72 273e 0a32 3031 362f 3037 2f30 310a  or'>.2016/07/01.
+00007940: 3230 3136 2f30 372f 3032 0a32 3031 362f  2016/07/02.2016/
+00007950: 3037 2f30 3394 6aec 0200 005d 946a fa02  07/03.j....].j..
+00007960: 0000 8c34 3c63 6c61 7373 2027 6765 6e65  ...4<class 'gene
+00007970: 7261 746f 7227 3e0a 3230 3136 2f30 372f  rator'>.2016/07/
+00007980: 3031 0a32 3031 362f 3037 2f30 320a 3230  01.2016/07/02.20
+00007990: 3136 2f30 372f 3033 9485 9481 947d 946a  16/07/03.....}.j
+000079a0: ff02 0000 6a02 0900 0073 6261 6a03 0300  ....j....sbaj...
+000079b0: 007d 9428 6a05 0300 005d 946a 0703 0000  .}.(j....].j....
+000079c0: 5d94 6a09 0300 005d 946a 0b03 0000 5d94  ].j....].j....].
+000079d0: 6a0d 0300 005d 946a 6003 0000 6a61 0300  j....].j`...ja..
+000079e0: 006a a208 0000 8968 4b8c 0763 6f6e 736f  .j.....hK..conso
+000079f0: 6c65 946a a408 0000 7d94 756a 0f03 0000  le.j....}.uj....
+00007a00: 6a92 0800 006a 0103 0000 6a10 0300 006a  j....j....j....j
+00007a10: 0203 0000 4b37 6aff 0200 006a 2203 0000  ....K7j....j"...
+00007a20: 6a00 0300 006a e902 0000 7562 656a 0303  j....j....ubej..
+00007a30: 0000 7d94 286a 0503 0000 5d94 8c1b 636f  ..}.(j....]...co
+00007a40: 6f6b 6965 732d 7574 696c 6974 6965 732d  okies-utilities-
+00007a50: 6765 742d 6461 7465 7394 616a 0703 0000  get-dates.aj....
+00007a60: 5d94 6a09 0300 005d 948c 1b63 6f6f 6b69  ].j....]...cooki
+00007a70: 6573 5f75 7469 6c69 7469 6573 2e67 6574  es_utilities.get
+00007a80: 5f64 6174 6573 9461 6a0b 0300 005d 946a  _dates.aj....].j
+00007a90: 0d03 0000 5d94 756a 0f03 0000 6830 6aff  ....].uj....h0j.
+00007aa0: 0200 006a 1103 0000 6a00 0300 006a e902  ...j....j....j..
+00007ab0: 0000 6a01 0300 006a 1003 0000 6a02 0300  ..j....j....j...
+00007ac0: 004b 0875 6265 6a03 0300 007d 9428 6a05  .K.ubej....}.(j.
+00007ad0: 0300 005d 948c 0966 756e 6374 696f 6e73  ...]...functions
+00007ae0: 9461 6a07 0300 005d 946a 0903 0000 5d94  .aj....].j....].
+00007af0: 8c09 6675 6e63 7469 6f6e 7394 616a 0b03  ..functions.aj..
+00007b00: 0000 5d94 6a0d 0300 005d 9475 6a0f 0300  ..].j....].uj...
+00007b10: 0068 306a ff02 0000 6af0 0200 006a 0003  .h0j....j....j..
+00007b20: 0000 6ae9 0200 006a 0103 0000 6a10 0300  ..j....j....j...
+00007b30: 006a 0203 0000 4b05 7562 6aef 0200 0029  .j....K.ubj....)
+00007b40: 8194 7d94 286a eb02 0000 6840 6aec 0200  ..}.(j....h@j...
+00007b50: 005d 9428 6af4 0200 0029 8194 7d94 286a  .].(j....)..}.(j
+00007b60: eb02 0000 8c07 436c 6173 7365 7394 6aec  ......Classes.j.
+00007b70: 0200 005d 946a fa02 0000 8c07 436c 6173  ...].j......Clas
+00007b80: 7365 7394 8594 8194 7d94 286a ff02 0000  ses.....}.(j....
+00007b90: 6a25 0900 006a 0003 0000 6ae9 0200 006a  j%...j....j....j
+00007ba0: 0103 0000 4e6a 0203 0000 4e75 6261 6a03  ....Nj....Nubaj.
+00007bb0: 0300 007d 9428 6a05 0300 005d 946a 0703  ...}.(j....].j..
+00007bc0: 0000 5d94 6a09 0300 005d 946a 0b03 0000  ..].j....].j....
+00007bd0: 5d94 6a0d 0300 005d 9475 6a0f 0300 006a  ].j....].uj....j
+00007be0: f302 0000 6aff 0200 006a 2209 0000 6a00  ....j....j"...j.
+00007bf0: 0300 006a e902 0000 6a01 0300 006a 1003  ...j....j....j..
+00007c00: 0000 6a02 0300 004b 3f75 626a ef02 0000  ..j....K?ubj....
+00007c10: 2981 947d 9428 6aeb 0200 0068 406a ec02  )..}.(j....h@j..
+00007c20: 0000 5d94 286a f402 0000 2981 947d 9428  ..].(j....)..}.(
+00007c30: 6aeb 0200 008c 1b63 6f6f 6b69 6573 5f75  j......cookies_u
+00007c40: 7469 6c69 7469 6573 2e53 746f 7077 6174  tilities.Stopwat
+00007c50: 6368 946a ec02 0000 5d94 6afa 0200 008c  ch.j....].j.....
+00007c60: 1b63 6f6f 6b69 6573 5f75 7469 6c69 7469  .cookies_utiliti
+00007c70: 6573 2e53 746f 7077 6174 6368 9485 9481  es.Stopwatch....
+00007c80: 947d 9428 6aff 0200 006a 3609 0000 6a00  .}.(j....j6...j.
+00007c90: 0300 006a e902 0000 6a01 0300 004e 6a02  ...j....j....Nj.
+00007ca0: 0300 004e 7562 616a 0303 0000 7d94 286a  ...Nubaj....}.(j
+00007cb0: 0503 0000 5d94 6a07 0300 005d 946a 0903  ....].j....].j..
+00007cc0: 0000 5d94 6a0b 0300 005d 946a 0d03 0000  ..].j....].j....
+00007cd0: 5d94 756a 0f03 0000 6af3 0200 006a ff02  ].uj....j....j..
+00007ce0: 0000 6a33 0900 006a 0003 0000 6ae9 0200  ..j3...j....j...
+00007cf0: 006a 0103 0000 6a10 0300 006a 0203 0000  .j....j....j....
+00007d00: 4b42 7562 6a33 0300 0029 8194 7d94 286a  KBubj3...)..}.(j
+00007d10: eb02 0000 6840 6aec 0200 005d 946a 0303  ....h@j....].j..
+00007d20: 0000 7d94 286a 0503 0000 5d94 6a07 0300  ..}.(j....].j...
+00007d30: 005d 946a 0903 0000 5d94 6a0b 0300 005d  .].j....].j....]
+00007d40: 946a 0d03 0000 5d94 8c07 656e 7472 6965  .j....]...entrie
+00007d50: 7394 5d94 286a 3f03 0000 8c26 5374 6f70  s.].(j?....&Stop
+00007d60: 7761 7463 6820 2863 6c61 7373 2069 6e20  watch (class in 
+00007d70: 636f 6f6b 6965 735f 7574 696c 6974 6965  cookies_utilitie
+00007d80: 7329 948c 1b63 6f6f 6b69 6573 5f75 7469  s)...cookies_uti
+00007d90: 6c69 7469 6573 2e53 746f 7077 6174 6368  lities.Stopwatch
+00007da0: 9468 404e 7494 6175 6a0f 0300 0068 596a  .h@Nt.auj....hYj
+00007db0: ff02 0000 6a33 0900 006a 0003 0000 6ae9  ....j3...j....j.
+00007dc0: 0200 006a 0103 0000 4e6a 0203 0000 4e75  ...j....Nj....Nu
+00007dd0: 626a 4403 0000 2981 947d 9428 6aeb 0200  bjD...)..}.(j...
+00007de0: 0068 406a ec02 0000 5d94 286a 4903 0000  .h@j....].(jI...
+00007df0: 2981 947d 9428 6aeb 0200 008c 0b53 746f  )..}.(j......Sto
+00007e00: 7077 6174 6368 2829 946a ec02 0000 5d94  pwatch().j....].
+00007e10: 286a e602 0000 8c0f 6465 7363 5f61 6e6e  (j......desc_ann
+00007e20: 6f74 6174 696f 6e94 9394 2981 947d 9428  otation...)..}.(
+00007e30: 6aeb 0200 008c 325b 3c23 7465 7874 3a20  j.....2[<#text: 
+00007e40: 2763 6c61 7373 273e 2c20 3c64 6573 635f  'class'>, <desc_
+00007e50: 7369 675f 7370 6163 653a 203c 2374 6578  sig_space: <#tex
+00007e60: 743a 2027 2027 3e3e 5d94 6aec 0200 005d  t: ' '>>].j....]
+00007e70: 9428 6afa 0200 008c 0563 6c61 7373 9485  .(j......class..
+00007e80: 9481 947d 9428 6aff 0200 006a 5b09 0000  ...}.(j....j[...
+00007e90: 6a00 0300 006a e902 0000 6a01 0300 004e  j....j....j....N
+00007ea0: 6a02 0300 004e 7562 6ae6 0200 008c 0e64  j....Nubj......d
+00007eb0: 6573 635f 7369 675f 7370 6163 6594 9394  esc_sig_space...
+00007ec0: 2981 947d 9428 6aeb 0200 008c 0120 946a  )..}.(j...... .j
+00007ed0: ec02 0000 5d94 6afa 0200 008c 0120 9485  ....].j...... ..
+00007ee0: 9481 947d 9428 6aff 0200 006a 6509 0000  ...}.(j....je...
+00007ef0: 6a00 0300 006a e902 0000 6a01 0300 004e  j....j....j....N
+00007f00: 6a02 0300 004e 7562 616a 0303 0000 7d94  j....Nubaj....}.
+00007f10: 286a 0503 0000 5d94 6a07 0300 005d 948c  (j....].j....]..
+00007f20: 0177 9461 6a09 0300 005d 946a 0b03 0000  .w.aj....].j....
+00007f30: 5d94 6a0d 0300 005d 9475 6a0f 0300 006a  ].j....].uj....j
+00007f40: 6309 0000 6aff 0200 006a 5b09 0000 7562  c...j....j[...ub
+00007f50: 656a 0303 0000 7d94 286a 0503 0000 5d94  ej....}.(j....].
+00007f60: 6a07 0300 005d 946a 0903 0000 5d94 6a0b  j....].j....].j.
+00007f70: 0300 005d 946a 0d03 0000 5d94 6a60 0300  ...].j....].j`..
+00007f80: 006a 6103 0000 756a 0f03 0000 6a59 0900  .ja...uj....jY..
+00007f90: 006a ff02 0000 6a55 0900 006a 0003 0000  .j....jU...j....
+00007fa0: 6ae9 0200 006a 0103 0000 8c7c 433a 5c55  j....j.....|C:\U
+00007fb0: 7365 7273 5c63 2d6d 6968 5c73 7061 6365  sers\c-mih\space
+00007fc0: 5c63 6f6f 6b69 6573 5f75 7469 6c69 7469  \cookies_utiliti
+00007fd0: 6573 5c73 7263 5c63 6f6f 6b69 6573 5f75  es\src\cookies_u
+00007fe0: 7469 6c69 7469 6573 5c73 746f 7077 6174  tilities\stopwat
+00007ff0: 6368 2e70 793a 646f 6373 7472 696e 6720  ch.py:docstring 
+00008000: 6f66 2063 6f6f 6b69 6573 5f75 7469 6c69  of cookies_utili
+00008010: 7469 6573 2e73 746f 7077 6174 6368 2e53  ties.stopwatch.S
+00008020: 746f 7077 6174 6368 946a 0203 0000 4b01  topwatch.j....K.
+00008030: 7562 6a4f 0300 0029 8194 7d94 286a eb02  ubjO...)..}.(j..
+00008040: 0000 8c12 636f 6f6b 6965 735f 7574 696c  ....cookies_util
+00008050: 6974 6965 732e 946a ec02 0000 5d94 6afa  ities..j....].j.
+00008060: 0200 008c 1263 6f6f 6b69 6573 5f75 7469  .....cookies_uti
+00008070: 6c69 7469 6573 2e94 8594 8194 7d94 286a  lities......}.(j
+00008080: ff02 0000 6a7b 0900 006a 0003 0000 6ae9  ....j{...j....j.
+00008090: 0200 006a 0103 0000 4e6a 0203 0000 4e75  ...j....Nj....Nu
+000080a0: 6261 6a03 0300 007d 9428 6a05 0300 005d  baj....}.(j....]
+000080b0: 946a 0703 0000 5d94 286a 5b03 0000 6a5c  .j....].(j[...j\
+000080c0: 0300 0065 6a09 0300 005d 946a 0b03 0000  ...ej....].j....
+000080d0: 5d94 6a0d 0300 005d 946a 6003 0000 6a61  ].j....].j`...ja
+000080e0: 0300 0075 6a0f 0300 006a 4e03 0000 6aff  ...uj....jN...j.
+000080f0: 0200 006a 5509 0000 6a00 0300 006a e902  ...jU...j....j..
+00008100: 0000 6a01 0300 006a 7a09 0000 6a02 0300  ..j....jz...j...
+00008110: 004b 0175 626a 6403 0000 2981 947d 9428  .K.ubjd...)..}.(
+00008120: 6aeb 0200 008c 0953 746f 7077 6174 6368  j......Stopwatch
+00008130: 946a ec02 0000 5d94 6afa 0200 008c 0953  .j....].j......S
+00008140: 746f 7077 6174 6368 9485 9481 947d 9428  topwatch.....}.(
+00008150: 6aff 0200 006a 8909 0000 6a00 0300 006a  j....j....j....j
+00008160: e902 0000 6a01 0300 004e 6a02 0300 004e  ....j....Nj....N
+00008170: 7562 616a 0303 0000 7d94 286a 0503 0000  ubaj....}.(j....
+00008180: 5d94 6a07 0300 005d 9428 6a70 0300 006a  ].j....].(jp...j
+00008190: 7103 0000 656a 0903 0000 5d94 6a0b 0300  q...ej....].j...
+000081a0: 005d 946a 0d03 0000 5d94 6a60 0300 006a  .].j....].j`...j
+000081b0: 6103 0000 756a 0f03 0000 6a63 0300 006a  a...uj....jc...j
+000081c0: ff02 0000 6a55 0900 006a 0003 0000 6ae9  ....jU...j....j.
+000081d0: 0200 006a 0103 0000 6a7a 0900 006a 0203  ...j....jz...j..
+000081e0: 0000 4b01 7562 656a 0303 0000 7d94 286a  ..K.ubej....}.(j
+000081f0: 0503 0000 5d94 6a50 0900 0061 6a07 0300  ....].jP...aj...
+00008200: 005d 9428 6a01 0500 006a 0205 0000 656a  .].(j....j....ej
+00008210: 0903 0000 5d94 6a0b 0300 005d 946a 0d03  ....].j....].j..
+00008220: 0000 5d94 6a06 0500 008c 1163 6f6f 6b69  ..].j......cooki
+00008230: 6573 5f75 7469 6c69 7469 6573 946a 6a02  es_utilities.jj.
+00008240: 0000 6840 6a08 0500 006a 8b09 0000 6a09  ..h@j....j....j.
+00008250: 0500 006a 9d09 0000 6a8b 0900 0086 946a  ...j....j......j
+00008260: 0b05 0000 6a8b 0900 0075 6a0f 0300 006a  ....j....uj....j
+00008270: 4803 0000 6a01 0300 006a 7a09 0000 6a02  H...j....jz...j.
+00008280: 0300 004b 016a ff02 0000 6a52 0900 006a  ...K.j....jR...j
+00008290: 0003 0000 6ae9 0200 0075 626a 0e05 0000  ....j....ubj....
+000082a0: 2981 947d 9428 6aeb 0200 0068 406a ec02  )..}.(j....h@j..
+000082b0: 0000 5d94 286a 1305 0000 2981 947d 9428  ..].(j....)..}.(
+000082c0: 6aeb 0200 008c 2853 746f 7077 6174 6368  j.....(Stopwatch
+000082d0: 2066 6f72 206d 6561 7375 7269 6e67 2070   for measuring p
+000082e0: 726f 6365 7373 696e 6720 7469 6d65 2e94  rocessing time..
+000082f0: 6aec 0200 005d 946a fa02 0000 8c28 5374  j....].j.....(St
+00008300: 6f70 7761 7463 6820 666f 7220 6d65 6173  opwatch for meas
+00008310: 7572 696e 6720 7072 6f63 6573 7369 6e67  uring processing
+00008320: 2074 696d 652e 9485 9481 947d 9428 6aff   time......}.(j.
+00008330: 0200 006a a209 0000 6a00 0300 006a e902  ...j....j....j..
+00008340: 0000 6a01 0300 004e 6a02 0300 004e 7562  ..j....Nj....Nub
+00008350: 616a 0303 0000 7d94 286a 0503 0000 5d94  aj....}.(j....].
+00008360: 6a07 0300 005d 946a 0903 0000 5d94 6a0b  j....].j....].j.
+00008370: 0300 005d 946a 0d03 0000 5d94 756a 0f03  ...].j....].uj..
+00008380: 0000 6a12 0500 006a 0103 0000 8c7c 433a  ..j....j.....|C:
+00008390: 5c55 7365 7273 5c63 2d6d 6968 5c73 7061  \Users\c-mih\spa
+000083a0: 6365 5c63 6f6f 6b69 6573 5f75 7469 6c69  ce\cookies_utili
+000083b0: 7469 6573 5c73 7263 5c63 6f6f 6b69 6573  ties\src\cookies
+000083c0: 5f75 7469 6c69 7469 6573 5c73 746f 7077  _utilities\stopw
+000083d0: 6174 6368 2e70 793a 646f 6373 7472 696e  atch.py:docstrin
+000083e0: 6720 6f66 2063 6f6f 6b69 6573 5f75 7469  g of cookies_uti
+000083f0: 6c69 7469 6573 2e73 746f 7077 6174 6368  lities.stopwatch
+00008400: 2e53 746f 7077 6174 6368 946a 0203 0000  .Stopwatch.j....
+00008410: 4b01 6aff 0200 006a 9f09 0000 6a00 0300  K.j....j....j...
+00008420: 006a e902 0000 7562 6a33 0300 0029 8194  .j....ubj3...)..
+00008430: 7d94 286a eb02 0000 6840 6aec 0200 005d  }.(j....h@j....]
+00008440: 946a 0303 0000 7d94 286a 0503 0000 5d94  .j....}.(j....].
+00008450: 6a07 0300 005d 946a 0903 0000 5d94 6a0b  j....].j....].j.
+00008460: 0300 005d 946a 0d03 0000 5d94 8c07 656e  ...].j....]...en
+00008470: 7472 6965 7394 5d94 286a 3f03 0000 8c2c  tries.].(j?....,
+00008480: 7072 6573 7328 2920 2863 6f6f 6b69 6573  press() (cookies
+00008490: 5f75 7469 6c69 7469 6573 2e53 746f 7077  _utilities.Stopw
+000084a0: 6174 6368 206d 6574 686f 6429 948c 2163  atch method)..!c
+000084b0: 6f6f 6b69 6573 5f75 7469 6c69 7469 6573  ookies_utilities
+000084c0: 2e53 746f 7077 6174 6368 2e70 7265 7373  .Stopwatch.press
+000084d0: 9468 404e 7494 6175 6a0f 0300 0068 596a  .h@Nt.auj....hYj
+000084e0: ff02 0000 6a9f 0900 006a 0003 0000 6ae9  ....j....j....j.
+000084f0: 0200 006a 0103 0000 4e6a 0203 0000 4e75  ...j....Nj....Nu
+00008500: 626a 4403 0000 2981 947d 9428 6aeb 0200  bjD...)..}.(j...
+00008510: 0068 406a ec02 0000 5d94 286a 4903 0000  .h@j....].(jI...
+00008520: 2981 947d 9428 6aeb 0200 008c 1753 746f  )..}.(j......Sto
+00008530: 7077 6174 6368 2e70 7265 7373 286b 6579  pwatch.press(key
+00008540: 3d27 2729 946a ec02 0000 5d94 286a 6403  ='').j....].(jd.
+00008550: 0000 2981 947d 9428 6aeb 0200 008c 0570  ..)..}.(j......p
+00008560: 7265 7373 946a ec02 0000 5d94 6afa 0200  ress.j....].j...
+00008570: 008c 0570 7265 7373 9485 9481 947d 9428  ...press.....}.(
+00008580: 6aff 0200 006a c609 0000 6a00 0300 006a  j....j....j....j
+00008590: e902 0000 6a01 0300 004e 6a02 0300 004e  ....j....Nj....N
+000085a0: 7562 616a 0303 0000 7d94 286a 0503 0000  ubaj....}.(j....
+000085b0: 5d94 6a07 0300 005d 9428 6a70 0300 006a  ].j....].(jp...j
+000085c0: 7103 0000 656a 0903 0000 5d94 6a0b 0300  q...ej....].j...
+000085d0: 005d 946a 0d03 0000 5d94 6a60 0300 006a  .].j....].j`...j
+000085e0: 6103 0000 756a 0f03 0000 6a63 0300 006a  a...uj....jc...j
+000085f0: ff02 0000 6ac2 0900 006a 0003 0000 6ae9  ....j....j....j.
+00008600: 0200 006a 0103 0000 8c82 433a 5c55 7365  ...j......C:\Use
+00008610: 7273 5c63 2d6d 6968 5c73 7061 6365 5c63  rs\c-mih\space\c
+00008620: 6f6f 6b69 6573 5f75 7469 6c69 7469 6573  ookies_utilities
+00008630: 5c73 7263 5c63 6f6f 6b69 6573 5f75 7469  \src\cookies_uti
+00008640: 6c69 7469 6573 5c73 746f 7077 6174 6368  lities\stopwatch
+00008650: 2e70 793a 646f 6373 7472 696e 6720 6f66  .py:docstring of
+00008660: 2063 6f6f 6b69 6573 5f75 7469 6c69 7469   cookies_utiliti
+00008670: 6573 2e73 746f 7077 6174 6368 2e53 746f  es.stopwatch.Sto
+00008680: 7077 6174 6368 2e70 7265 7373 946a 0203  pwatch.press.j..
+00008690: 0000 4b01 7562 6a76 0300 0029 8194 7d94  ..K.ubjv...)..}.
+000086a0: 286a eb02 0000 8c06 6b65 793d 2727 946a  (j......key=''.j
+000086b0: ec02 0000 5d94 6a7c 0300 0029 8194 7d94  ....].j|...)..}.
+000086c0: 286a eb02 0000 8c06 6b65 793d 2727 946a  (j......key=''.j
+000086d0: ec02 0000 5d94 286a 8203 0000 2981 947d  ....].(j....)..}
+000086e0: 9428 6aeb 0200 008c 036b 6579 946a ec02  .(j......key.j..
+000086f0: 0000 5d94 6afa 0200 008c 036b 6579 9485  ..].j......key..
+00008700: 9481 947d 9428 6aff 0200 006a dd09 0000  ...}.(j....j....
+00008710: 6a00 0300 006a e902 0000 6a01 0300 004e  j....j....j....N
+00008720: 6a02 0300 004e 7562 616a 0303 0000 7d94  j....Nubaj....}.
+00008730: 286a 0503 0000 5d94 6a07 0300 005d 946a  (j....].j....].j
+00008740: 8e03 0000 616a 0903 0000 5d94 6a0b 0300  ....aj....].j...
+00008750: 005d 946a 0d03 0000 5d94 756a 0f03 0000  .].j....].uj....
+00008760: 6a81 0300 006a ff02 0000 6ad9 0900 0075  j....j....j....u
+00008770: 626a 9303 0000 2981 947d 9428 6aeb 0200  bj....)..}.(j...
+00008780: 008c 013d 946a ec02 0000 5d94 6afa 0200  ...=.j....].j...
+00008790: 008c 013d 9485 9481 947d 9428 6aff 0200  ...=.....}.(j...
+000087a0: 006a eb09 0000 6a00 0300 006a e902 0000  .j....j....j....
+000087b0: 6a01 0300 004e 6a02 0300 004e 7562 616a  j....Nj....Nubaj
+000087c0: 0303 0000 7d94 286a 0503 0000 5d94 6a07  ....}.(j....].j.
+000087d0: 0300 005d 946a 9f03 0000 616a 0903 0000  ...].j....aj....
+000087e0: 5d94 6a0b 0300 005d 946a 0d03 0000 5d94  ].j....].j....].
+000087f0: 756a 0f03 0000 6a92 0300 006a ff02 0000  uj....j....j....
+00008800: 6ad9 0900 0075 626a a303 0000 2981 947d  j....ubj....)..}
+00008810: 9428 6aeb 0200 008c 0227 2794 6aec 0200  .(j......''.j...
+00008820: 005d 946a fa02 0000 8c02 2727 9485 9481  .].j......''....
+00008830: 947d 9428 6aff 0200 006a f909 0000 6a00  .}.(j....j....j.
+00008840: 0300 006a e902 0000 6a01 0300 004e 6a02  ...j....j....Nj.
+00008850: 0300 004e 7562 616a 0303 0000 7d94 286a  ...Nubaj....}.(j
+00008860: 0503 0000 5d94 6a07 0300 005d 946a af03  ....].j....].j..
+00008870: 0000 616a 0903 0000 5d94 6a0b 0300 005d  ..aj....].j....]
+00008880: 946a 0d03 0000 5d94 8c13 7375 7070 6f72  .j....]...suppor
+00008890: 745f 736d 6172 7471 756f 7465 7394 8975  t_smartquotes..u
+000088a0: 6a0f 0300 0068 fa6a ff02 0000 6ad9 0900  j....h.j....j...
+000088b0: 0075 6265 6a03 0300 007d 9428 6a05 0300  .ubej....}.(j...
+000088c0: 005d 946a 0703 0000 5d94 6a09 0300 005d  .].j....].j....]
+000088d0: 946a 0b03 0000 5d94 6a0d 0300 005d 946a  .j....].j....].j
+000088e0: 6003 0000 6a61 0300 0075 6a0f 0300 006a  `...ja...uj....j
+000088f0: 7b03 0000 6aff 0200 006a d509 0000 7562  {...j....j....ub
+00008900: 616a 0303 0000 7d94 286a 0503 0000 5d94  aj....}.(j....].
+00008910: 6a07 0300 005d 946a 0903 0000 5d94 6a0b  j....].j....].j.
+00008920: 0300 005d 946a 0d03 0000 5d94 6a60 0300  ...].j....].j`..
+00008930: 006a 6103 0000 756a 0f03 0000 6a75 0300  .ja...uj....ju..
+00008940: 006a ff02 0000 6ac2 0900 006a 0003 0000  .j....j....j....
+00008950: 6ae9 0200 006a 0103 0000 6ad4 0900 006a  j....j....j....j
+00008960: 0203 0000 4b01 7562 656a 0303 0000 7d94  ....K.ubej....}.
+00008970: 286a 0503 0000 5d94 6abd 0900 0061 6a07  (j....].j....aj.
+00008980: 0300 005d 9428 6a01 0500 006a 0205 0000  ...].(j....j....
+00008990: 656a 0903 0000 5d94 6a0b 0300 005d 946a  ej....].j....].j
+000089a0: 0d03 0000 5d94 6a06 0500 008c 1163 6f6f  ....].j......coo
+000089b0: 6b69 6573 5f75 7469 6c69 7469 6573 946a  kies_utilities.j
+000089c0: 6a02 0000 6a8b 0900 006a 0805 0000 8c0f  j...j....j......
+000089d0: 5374 6f70 7761 7463 682e 7072 6573 7394  Stopwatch.press.
+000089e0: 6a09 0500 006a 1a0a 0000 8c09 5374 6f70  j....j......Stop
+000089f0: 7761 7463 6894 8c05 7072 6573 7394 8794  watch...press...
+00008a00: 6a0b 0500 008c 1153 746f 7077 6174 6368  j......Stopwatch
+00008a10: 2e70 7265 7373 2829 9475 6a0f 0300 006a  .press().uj....j
+00008a20: 4803 0000 6a01 0300 006a d409 0000 6a02  H...j....j....j.
+00008a30: 0300 004b 016a ff02 0000 6abf 0900 006a  ...K.j....j....j
+00008a40: 0003 0000 6ae9 0200 0075 626a 0e05 0000  ....j....ubj....
+00008a50: 2981 947d 9428 6aeb 0200 0068 406a ec02  )..}.(j....h@j..
+00008a60: 0000 5d94 286a 1305 0000 2981 947d 9428  ..].(j....)..}.(
+00008a70: 6aeb 0200 008c 1450 7265 7373 2074 6865  j......Press the
+00008a80: 2073 746f 7077 6174 6368 2e94 6aec 0200   stopwatch..j...
+00008a90: 005d 946a fa02 0000 8c14 5072 6573 7320  .].j......Press 
+00008aa0: 7468 6520 7374 6f70 7761 7463 682e 9485  the stopwatch...
+00008ab0: 9481 947d 9428 6aff 0200 006a 230a 0000  ...}.(j....j#...
+00008ac0: 6a00 0300 006a e902 0000 6a01 0300 004e  j....j....j....N
+00008ad0: 6a02 0300 004e 7562 616a 0303 0000 7d94  j....Nubaj....}.
+00008ae0: 286a 0503 0000 5d94 6a07 0300 005d 946a  (j....].j....].j
+00008af0: 0903 0000 5d94 6a0b 0300 005d 946a 0d03  ....].j....].j..
+00008b00: 0000 5d94 756a 0f03 0000 6a12 0500 006a  ..].uj....j....j
+00008b10: 0103 0000 8c82 433a 5c55 7365 7273 5c63  ......C:\Users\c
+00008b20: 2d6d 6968 5c73 7061 6365 5c63 6f6f 6b69  -mih\space\cooki
+00008b30: 6573 5f75 7469 6c69 7469 6573 5c73 7263  es_utilities\src
+00008b40: 5c63 6f6f 6b69 6573 5f75 7469 6c69 7469  \cookies_utiliti
+00008b50: 6573 5c73 746f 7077 6174 6368 2e70 793a  es\stopwatch.py:
+00008b60: 646f 6373 7472 696e 6720 6f66 2063 6f6f  docstring of coo
+00008b70: 6b69 6573 5f75 7469 6c69 7469 6573 2e73  kies_utilities.s
+00008b80: 746f 7077 6174 6368 2e53 746f 7077 6174  topwatch.Stopwat
+00008b90: 6368 2e70 7265 7373 946a 0203 0000 4b01  ch.press.j....K.
+00008ba0: 6aff 0200 006a 200a 0000 6a00 0300 006a  j....j ...j....j
+00008bb0: e902 0000 7562 6a46 0500 0029 8194 7d94  ....ubjF...)..}.
+00008bc0: 286a eb02 0000 6840 6aec 0200 005d 946a  (j....h@j....].j
+00008bd0: 4b05 0000 2981 947d 9428 6aeb 0200 0068  K...)..}.(j....h
+00008be0: 406a ec02 0000 5d94 286a 5005 0000 2981  @j....].(jP...).
+00008bf0: 947d 9428 6aeb 0200 008c 0a50 6172 616d  .}.(j......Param
+00008c00: 6574 6572 7394 6aec 0200 005d 946a fa02  eters.j....].j..
+00008c10: 0000 8c0a 5061 7261 6d65 7465 7273 9485  ....Parameters..
+00008c20: 9481 947d 9428 6aff 0200 006a 380a 0000  ...}.(j....j8...
+00008c30: 6a00 0300 006a e902 0000 6a01 0300 004e  j....j....j....N
+00008c40: 6a02 0300 004e 7562 616a 0303 0000 7d94  j....Nubaj....}.
+00008c50: 286a 0503 0000 5d94 6a07 0300 005d 946a  (j....].j....].j
+00008c60: 0903 0000 5d94 6a0b 0300 005d 946a 0d03  ....].j....].j..
+00008c70: 0000 5d94 756a 0f03 0000 6a4f 0500 006a  ..].uj....jO...j
+00008c80: ff02 0000 6a35 0a00 006a 0103 0000 6ad4  ....j5...j....j.
+00008c90: 0900 006a 0203 0000 4b00 7562 6a60 0500  ...j....K.ubj`..
+00008ca0: 0029 8194 7d94 286a eb02 0000 6840 6aec  .)..}.(j....h@j.
+00008cb0: 0200 005d 946a 1305 0000 2981 947d 9428  ...].j....)..}.(
+00008cc0: 6aeb 0200 008c 386b 6579 2028 7374 7269  j.....8key (stri
+00008cd0: 6e67 2920 2d2d 2054 6865 2069 6465 6e66  ng) -- The idenf
+00008ce0: 6963 6174 6f72 2066 6f72 2074 6865 2074  icator for the t
+00008cf0: 696d 6520 286f 7074 696f 6e61 6c29 2e94  ime (optional)..
+00008d00: 6aec 0200 005d 9428 6a73 0500 0029 8194  j....].(js...)..
+00008d10: 7d94 286a eb02 0000 8c03 6b65 7994 6aec  }.(j......key.j.
+00008d20: 0200 005d 946a fa02 0000 8c03 6b65 7994  ...].j......key.
+00008d30: 8594 8194 7d94 286a ff02 0000 6a4d 0a00  ....}.(j....jM..
+00008d40: 006a 0003 0000 6ae9 0200 006a 0103 0000  .j....j....j....
+00008d50: 4e6a 0203 0000 4e75 6261 6a03 0300 007d  Nj....Nubaj....}
+00008d60: 9428 6a05 0300 005d 946a 0703 0000 5d94  .(j....].j....].
+00008d70: 6a09 0300 005d 946a 0b03 0000 5d94 6a0d  j....].j....].j.
+00008d80: 0300 005d 9475 6a0f 0300 006a 7205 0000  ...].uj....jr...
+00008d90: 6aff 0200 006a 490a 0000 7562 6afa 0200  j....jI...ubj...
+00008da0: 008c 0220 2894 8594 8194 7d94 286a ff02  ... (.....}.(j..
+00008db0: 0000 6a49 0a00 006a 0003 0000 6ae9 0200  ..jI...j....j...
+00008dc0: 006a 0103 0000 4e6a 0203 0000 4e75 626a  .j....Nj....Nubj
+00008dd0: 8705 0000 2981 947d 9428 6aeb 0200 0068  ....)..}.(j....h
+00008de0: 406a ec02 0000 5d94 6a8c 0500 0029 8194  @j....].j....)..
+00008df0: 7d94 286a eb02 0000 8c06 7374 7269 6e67  }.(j......string
+00008e00: 946a ec02 0000 5d94 6afa 0200 008c 0673  .j....].j......s
+00008e10: 7472 696e 6794 8594 8194 7d94 286a ff02  tring.....}.(j..
+00008e20: 0000 6a62 0a00 006a 0003 0000 6ae9 0200  ..jb...j....j...
+00008e30: 006a 0103 0000 4e6a 0203 0000 4e75 6261  .j....Nj....Nuba
+00008e40: 6a03 0300 007d 9428 6a05 0300 005d 946a  j....}.(j....].j
+00008e50: 0703 0000 5d94 6a09 0300 005d 946a 0b03  ....].j....].j..
+00008e60: 0000 5d94 6a0d 0300 005d 9475 6a0f 0300  ..].j....].uj...
+00008e70: 006a 8b05 0000 6aff 0200 006a 5f0a 0000  .j....j....j_...
+00008e80: 7562 616a 0303 0000 7d94 286a 0503 0000  ubaj....}.(j....
+00008e90: 5d94 6a07 0300 005d 946a 0903 0000 5d94  ].j....].j....].
+00008ea0: 6a0b 0300 005d 946a 0d03 0000 5d94 8c09  j....].j....]...
+00008eb0: 7265 6664 6f6d 6169 6e94 8c02 7079 948c  refdomain...py..
+00008ec0: 0b72 6566 6578 706c 6963 6974 9489 8c07  .refexplicit....
+00008ed0: 7265 6674 7970 6594 6a6a 0200 008c 0972  reftype.jj.....r
+00008ee0: 6566 7461 7267 6574 946a 640a 0000 6aa6  eftarget.jd...j.
+00008ef0: 0500 0088 6aa7 0500 006a 1a0a 0000 6aa8  ....j....j....j.
+00008f00: 0500 006a 8b09 0000 756a 0f03 0000 6a86  ...j....uj....j.
+00008f10: 0500 006a ff02 0000 6a49 0a00 0075 626a  ...j....jI...ubj
+00008f20: fa02 0000 8c01 2994 8594 8194 7d94 286a  ......).....}.(j
+00008f30: ff02 0000 6a49 0a00 006a 0003 0000 6ae9  ....jI...j....j.
+00008f40: 0200 006a 0103 0000 4e6a 0203 0000 4e75  ...j....Nj....Nu
+00008f50: 626a fa02 0000 8c05 20e2 8093 2094 8594  bj...... ... ...
+00008f60: 8194 7d94 286a ff02 0000 6a49 0a00 006a  ..}.(j....jI...j
+00008f70: 0003 0000 6ae9 0200 006a 0103 0000 4e6a  ....j....j....Nj
+00008f80: 0203 0000 4e75 626a fa02 0000 8c28 5468  ....Nubj.....(Th
+00008f90: 6520 6964 656e 6669 6361 746f 7220 666f  e idenficator fo
+00008fa0: 7220 7468 6520 7469 6d65 2028 6f70 7469  r the time (opti
+00008fb0: 6f6e 616c 292e 9485 9481 947d 9428 6aff  onal)......}.(j.
+00008fc0: 0200 006a 490a 0000 6a00 0300 006a e902  ...jI...j....j..
+00008fd0: 0000 6a01 0300 004e 6a02 0300 004e 7562  ..j....Nj....Nub
+00008fe0: 656a 0303 0000 7d94 286a 0503 0000 5d94  ej....}.(j....].
+00008ff0: 6a07 0300 005d 946a 0903 0000 5d94 6a0b  j....].j....].j.
+00009000: 0300 005d 946a 0d03 0000 5d94 756a 0f03  ...].j....].uj..
+00009010: 0000 6a12 0500 006a ff02 0000 6a46 0a00  ..j....j....jF..
+00009020: 0075 6261 6a03 0300 007d 9428 6a05 0300  .ubaj....}.(j...
+00009030: 005d 946a 0703 0000 5d94 6a09 0300 005d  .].j....].j....]
+00009040: 946a 0b03 0000 5d94 6a0d 0300 005d 9475  .j....].j....].u
+00009050: 6a0f 0300 006a 5f05 0000 6aff 0200 006a  j....j_...j....j
+00009060: 350a 0000 7562 656a 0303 0000 7d94 286a  5...ubej....}.(j
+00009070: 0503 0000 5d94 6a07 0300 005d 946a 0903  ....].j....].j..
+00009080: 0000 5d94 6a0b 0300 005d 946a 0d03 0000  ..].j....].j....
+00009090: 5d94 756a 0f03 0000 6a4a 0500 006a ff02  ].uj....jJ...j..
+000090a0: 0000 6a32 0a00 0075 6261 6a03 0300 007d  ..j2...ubaj....}
+000090b0: 9428 6a05 0300 005d 946a 0703 0000 5d94  .(j....].j....].
+000090c0: 6a09 0300 005d 946a 0b03 0000 5d94 6a0d  j....].j....].j.
+000090d0: 0300 005d 9475 6a0f 0300 006a 4505 0000  ...].uj....jE...
+000090e0: 6aff 0200 006a 200a 0000 6a00 0300 006a  j....j ...j....j
+000090f0: e902 0000 6a01 0300 004e 6a02 0300 004e  ....j....Nj....N
+00009100: 7562 656a 0303 0000 7d94 286a 0503 0000  ubej....}.(j....
+00009110: 5d94 6a07 0300 005d 946a 0903 0000 5d94  ].j....].j....].
+00009120: 6a0b 0300 005d 946a 0d03 0000 5d94 756a  j....].j....].uj
+00009130: 0f03 0000 6a0d 0500 006a ff02 0000 6abf  ....j....j....j.
+00009140: 0900 006a 0003 0000 6ae9 0200 006a 0103  ...j....j....j..
+00009150: 0000 6ad4 0900 006a 0203 0000 4b01 7562  ..j....j....K.ub
+00009160: 656a 0303 0000 7d94 286a 0503 0000 5d94  ej....}.(j....].
+00009170: 6a07 0300 005d 9428 6a77 0a00 008c 066d  j....].(jw.....m
+00009180: 6574 686f 6494 656a 0903 0000 5d94 6a0b  ethod.ej....].j.
+00009190: 0300 005d 946a 0d03 0000 5d94 6873 6a77  ...].j....].hsjw
+000091a0: 0a00 006a 6808 0000 6aa8 0a00 006a 6908  ...jh...j....ji.
+000091b0: 0000 6aa8 0a00 006a 6a08 0000 896a 6b08  ..j....jj....jk.
+000091c0: 0000 896a 6c08 0000 8975 6a0f 0300 006a  ...jl....uj....j
+000091d0: 4303 0000 6a00 0300 006a e902 0000 6aff  C...j....j....j.
+000091e0: 0200 006a 9f09 0000 6a01 0300 004e 6a02  ...j....j....Nj.
+000091f0: 0300 004e 7562 6a33 0300 0029 8194 7d94  ...Nubj3...)..}.
+00009200: 286a eb02 0000 6840 6aec 0200 005d 946a  (j....h@j....].j
+00009210: 0303 0000 7d94 286a 0503 0000 5d94 6a07  ....}.(j....].j.
+00009220: 0300 005d 946a 0903 0000 5d94 6a0b 0300  ...].j....].j...
+00009230: 005d 946a 0d03 0000 5d94 8c07 656e 7472  .].j....]...entr
+00009240: 6965 7394 5d94 286a 3f03 0000 8c2b 7368  ies.].(j?....+sh
+00009250: 6f77 2829 2028 636f 6f6b 6965 735f 7574  ow() (cookies_ut
+00009260: 696c 6974 6965 732e 5374 6f70 7761 7463  ilities.Stopwatc
+00009270: 6820 6d65 7468 6f64 2994 8c20 636f 6f6b  h method).. cook
+00009280: 6965 735f 7574 696c 6974 6965 732e 5374  ies_utilities.St
+00009290: 6f70 7761 7463 682e 7368 6f77 9468 404e  opwatch.show.h@N
+000092a0: 7494 6175 6a0f 0300 0068 596a ff02 0000  t.auj....hYj....
+000092b0: 6a9f 0900 006a 0003 0000 6ae9 0200 006a  j....j....j....j
+000092c0: 0103 0000 8c81 433a 5c55 7365 7273 5c63  ......C:\Users\c
+000092d0: 2d6d 6968 5c73 7061 6365 5c63 6f6f 6b69  -mih\space\cooki
+000092e0: 6573 5f75 7469 6c69 7469 6573 5c73 7263  es_utilities\src
+000092f0: 5c63 6f6f 6b69 6573 5f75 7469 6c69 7469  \cookies_utiliti
+00009300: 6573 5c73 746f 7077 6174 6368 2e70 793a  es\stopwatch.py:
+00009310: 646f 6373 7472 696e 6720 6f66 2063 6f6f  docstring of coo
+00009320: 6b69 6573 5f75 7469 6c69 7469 6573 2e73  kies_utilities.s
+00009330: 746f 7077 6174 6368 2e53 746f 7077 6174  topwatch.Stopwat
+00009340: 6368 2e73 686f 7794 6a02 0300 004e 7562  ch.show.j....Nub
+00009350: 6a44 0300 0029 8194 7d94 286a eb02 0000  jD...)..}.(j....
+00009360: 6840 6aec 0200 005d 9428 6a49 0300 0029  h@j....].(jI...)
+00009370: 8194 7d94 286a eb02 0000 8c10 5374 6f70  ..}.(j......Stop
+00009380: 7761 7463 682e 7368 6f77 2829 946a ec02  watch.show().j..
+00009390: 0000 5d94 286a 6403 0000 2981 947d 9428  ..].(jd...)..}.(
+000093a0: 6aeb 0200 008c 0473 686f 7794 6aec 0200  j......show.j...
+000093b0: 005d 946a fa02 0000 8c04 7368 6f77 9485  .].j......show..
+000093c0: 9481 947d 9428 6aff 0200 006a c20a 0000  ...}.(j....j....
+000093d0: 6a00 0300 006a e902 0000 6a01 0300 004e  j....j....j....N
+000093e0: 6a02 0300 004e 7562 616a 0303 0000 7d94  j....Nubaj....}.
+000093f0: 286a 0503 0000 5d94 6a07 0300 005d 9428  (j....].j....].(
+00009400: 6a70 0300 006a 7103 0000 656a 0903 0000  jp...jq...ej....
+00009410: 5d94 6a0b 0300 005d 946a 0d03 0000 5d94  ].j....].j....].
+00009420: 6a60 0300 006a 6103 0000 756a 0f03 0000  j`...ja...uj....
+00009430: 6a63 0300 006a ff02 0000 6abe 0a00 006a  jc...j....j....j
+00009440: 0003 0000 6ae9 0200 006a 0103 0000 8c81  ....j....j......
+00009450: 433a 5c55 7365 7273 5c63 2d6d 6968 5c73  C:\Users\c-mih\s
+00009460: 7061 6365 5c63 6f6f 6b69 6573 5f75 7469  pace\cookies_uti
+00009470: 6c69 7469 6573 5c73 7263 5c63 6f6f 6b69  lities\src\cooki
+00009480: 6573 5f75 7469 6c69 7469 6573 5c73 746f  es_utilities\sto
+00009490: 7077 6174 6368 2e70 793a 646f 6373 7472  pwatch.py:docstr
+000094a0: 696e 6720 6f66 2063 6f6f 6b69 6573 5f75  ing of cookies_u
+000094b0: 7469 6c69 7469 6573 2e73 746f 7077 6174  tilities.stopwat
+000094c0: 6368 2e53 746f 7077 6174 6368 2e73 686f  ch.Stopwatch.sho
+000094d0: 7794 6a02 0300 004b 0175 626a 7603 0000  w.j....K.ubjv...
+000094e0: 2981 947d 9428 6aeb 0200 008c 0228 2994  )..}.(j......().
+000094f0: 6aec 0200 005d 946a 0303 0000 7d94 286a  j....].j....}.(j
+00009500: 0503 0000 5d94 6a07 0300 005d 946a 0903  ....].j....].j..
+00009510: 0000 5d94 6a0b 0300 005d 946a 0d03 0000  ..].j....].j....
+00009520: 5d94 6a60 0300 006a 6103 0000 756a 0f03  ].j`...ja...uj..
+00009530: 0000 6a75 0300 006a ff02 0000 6abe 0a00  ..ju...j....j...
+00009540: 006a 0003 0000 6ae9 0200 006a 0103 0000  .j....j....j....
+00009550: 6ad0 0a00 006a 0203 0000 4b01 7562 656a  j....j....K.ubej
+00009560: 0303 0000 7d94 286a 0503 0000 5d94 6ab8  ....}.(j....].j.
+00009570: 0a00 0061 6a07 0300 005d 9428 6a01 0500  ...aj....].(j...
+00009580: 006a 0205 0000 656a 0903 0000 5d94 6a0b  .j....ej....].j.
+00009590: 0300 005d 946a 0d03 0000 5d94 6a06 0500  ...].j....].j...
+000095a0: 008c 1163 6f6f 6b69 6573 5f75 7469 6c69  ...cookies_utili
+000095b0: 7469 6573 946a 6a02 0000 6a8b 0900 006a  ties.jj...j....j
+000095c0: 0805 0000 8c0e 5374 6f70 7761 7463 682e  ......Stopwatch.
+000095d0: 7368 6f77 946a 0905 0000 6ae1 0a00 008c  show.j....j.....
+000095e0: 0953 746f 7077 6174 6368 948c 0473 686f  .Stopwatch...sho
+000095f0: 7794 8794 6a0b 0500 008c 1053 746f 7077  w...j......Stopw
+00009600: 6174 6368 2e73 686f 7728 2994 756a 0f03  atch.show().uj..
+00009610: 0000 6a48 0300 006a 0103 0000 6ad0 0a00  ..jH...j....j...
+00009620: 006a 0203 0000 4b01 6aff 0200 006a bb0a  .j....K.j....j..
+00009630: 0000 6a00 0300 006a e902 0000 7562 6a0e  ..j....j....ubj.
+00009640: 0500 0029 8194 7d94 286a eb02 0000 6840  ...)..}.(j....h@
+00009650: 6aec 0200 005d 946a 1305 0000 2981 947d  j....].j....)..}
+00009660: 9428 6aeb 0200 008c 0f53 686f 7720 6c61  .(j......Show la
+00009670: 7020 7469 6d65 732e 946a ec02 0000 5d94  p times..j....].
+00009680: 6afa 0200 008c 0f53 686f 7720 6c61 7020  j......Show lap 
+00009690: 7469 6d65 732e 9485 9481 947d 9428 6aff  times......}.(j.
+000096a0: 0200 006a ea0a 0000 6a00 0300 006a e902  ...j....j....j..
+000096b0: 0000 6a01 0300 004e 6a02 0300 004e 7562  ..j....Nj....Nub
+000096c0: 616a 0303 0000 7d94 286a 0503 0000 5d94  aj....}.(j....].
+000096d0: 6a07 0300 005d 946a 0903 0000 5d94 6a0b  j....].j....].j.
+000096e0: 0300 005d 946a 0d03 0000 5d94 756a 0f03  ...].j....].uj..
+000096f0: 0000 6a12 0500 006a 0103 0000 6aba 0a00  ..j....j....j...
+00009700: 006a 0203 0000 4b01 6aff 0200 006a e70a  .j....K.j....j..
+00009710: 0000 6a00 0300 006a e902 0000 7562 616a  ..j....j....ubaj
+00009720: 0303 0000 7d94 286a 0503 0000 5d94 6a07  ....}.(j....].j.
+00009730: 0300 005d 946a 0903 0000 5d94 6a0b 0300  ...].j....].j...
+00009740: 005d 946a 0d03 0000 5d94 756a 0f03 0000  .].j....].uj....
+00009750: 6a0d 0500 006a ff02 0000 6abb 0a00 006a  j....j....j....j
+00009760: 0003 0000 6ae9 0200 006a 0103 0000 6ad0  ....j....j....j.
+00009770: 0a00 006a 0203 0000 4b01 7562 656a 0303  ...j....K.ubej..
+00009780: 0000 7d94 286a 0503 0000 5d94 6a07 0300  ..}.(j....].j...
+00009790: 005d 9428 8c02 7079 948c 066d 6574 686f  .].(..py...metho
+000097a0: 6494 656a 0903 0000 5d94 6a0b 0300 005d  d.ej....].j....]
+000097b0: 946a 0d03 0000 5d94 6873 6a01 0b00 006a  .j....].hsj....j
+000097c0: 6808 0000 6a02 0b00 006a 6908 0000 6a02  h...j....ji...j.
+000097d0: 0b00 006a 6a08 0000 896a 6b08 0000 896a  ...jj....jk....j
+000097e0: 6c08 0000 8975 6a0f 0300 006a 4303 0000  l....uj....jC...
+000097f0: 6a00 0300 006a e902 0000 6aff 0200 006a  j....j....j....j
+00009800: 9f09 0000 6a01 0300 006a ba0a 0000 6a02  ....j....j....j.
+00009810: 0300 004e 7562 656a 0303 0000 7d94 286a  ...Nubej....}.(j
+00009820: 0503 0000 5d94 6a07 0300 005d 946a 0903  ....].j....].j..
+00009830: 0000 5d94 6a0b 0300 005d 946a 0d03 0000  ..].j....].j....
+00009840: 5d94 756a 0f03 0000 6a0d 0500 006a ff02  ].uj....j....j..
+00009850: 0000 6a52 0900 006a 0003 0000 6ae9 0200  ..jR...j....j...
+00009860: 006a 0103 0000 6a7a 0900 006a 0203 0000  .j....jz...j....
+00009870: 4b01 7562 656a 0303 0000 7d94 286a 0503  K.ubej....}.(j..
+00009880: 0000 5d94 6a07 0300 005d 9428 8c02 7079  ..].j....].(..py
+00009890: 948c 0563 6c61 7373 9465 6a09 0300 005d  ...class.ej....]
+000098a0: 946a 0b03 0000 5d94 6a0d 0300 005d 9468  .j....].j....].h
+000098b0: 736a 0f0b 0000 6a68 0800 006a 100b 0000  sj....jh...j....
+000098c0: 6a69 0800 006a 100b 0000 6a6a 0800 0089  ji...j....jj....
+000098d0: 6a6b 0800 0089 6a6c 0800 0089 756a 0f03  jk....jl....uj..
+000098e0: 0000 6a43 0300 006a 0003 0000 6ae9 0200  ..jC...j....j...
+000098f0: 006a ff02 0000 6a33 0900 006a 0103 0000  .j....j3...j....
+00009900: 4e6a 0203 0000 4e75 626a ee02 0000 8c07  Nj....Nubj......
+00009910: 636f 6d6d 656e 7494 9394 2981 947d 9428  comment...)..}.(
+00009920: 6aeb 0200 008c 123a 7368 6f77 2d69 6e68  j......:show-inh
+00009930: 6572 6974 616e 6365 3a94 6aec 0200 005d  eritance:.j....]
+00009940: 946a fa02 0000 8c12 3a73 686f 772d 696e  .j......:show-in
+00009950: 6865 7269 7461 6e63 653a 9485 9481 947d  heritance:.....}
+00009960: 946a ff02 0000 6a16 0b00 0073 6261 6a03  .j....j....sbaj.
+00009970: 0300 007d 9428 6a05 0300 005d 946a 0703  ...}.(j....].j..
+00009980: 0000 5d94 6a09 0300 005d 946a 0b03 0000  ..].j....].j....
+00009990: 5d94 6a0d 0300 005d 946a 6003 0000 6a61  ].j....].j`...ja
+000099a0: 0300 0075 6a0f 0300 006a 140b 0000 6aff  ...uj....j....j.
+000099b0: 0200 006a 3309 0000 6a00 0300 006a e902  ...j3...j....j..
+000099c0: 0000 6a01 0300 006a 1003 0000 6a02 0300  ..j....j....j...
+000099d0: 004b 4975 626a 1305 0000 2981 947d 9428  .KIubj....)..}.(
+000099e0: 6aeb 0200 008c 0b2a 2a45 7861 6d70 6c65  j......**Example
+000099f0: 2a2a 946a ec02 0000 5d94 6aa2 0700 0029  **.j....].j....)
+00009a00: 8194 7d94 286a eb02 0000 6a26 0b00 006a  ..}.(j....j&...j
+00009a10: ec02 0000 5d94 6afa 0200 008c 0745 7861  ....].j......Exa
+00009a20: 6d70 6c65 9485 9481 947d 9428 6aff 0200  mple.....}.(j...
+00009a30: 006a 280b 0000 6a00 0300 006a e902 0000  .j(...j....j....
+00009a40: 6a01 0300 004e 6a02 0300 004e 7562 616a  j....Nj....Nubaj
+00009a50: 0303 0000 7d94 286a 0503 0000 5d94 6a07  ....}.(j....].j.
+00009a60: 0300 005d 946a 0903 0000 5d94 6a0b 0300  ...].j....].j...
+00009a70: 005d 946a 0d03 0000 5d94 756a 0f03 0000  .].j....].uj....
+00009a80: 6aa1 0700 006a ff02 0000 6a24 0b00 0075  j....j....j$...u
+00009a90: 6261 6a03 0300 007d 9428 6a05 0300 005d  baj....}.(j....]
+00009aa0: 946a 0703 0000 5d94 6a09 0300 005d 946a  .j....].j....].j
+00009ab0: 0b03 0000 5d94 6a0d 0300 005d 9475 6a0f  ....].j....].uj.
+00009ac0: 0300 006a 1205 0000 6a01 0300 006a 1003  ...j....j....j..
+00009ad0: 0000 6a02 0300 004b 4a6a ff02 0000 6a33  ..j....KJj....j3
+00009ae0: 0900 006a 0003 0000 6ae9 0200 0075 626a  ...j....j....ubj
+00009af0: 9308 0000 2981 947d 9428 6aeb 0200 008c  ....)..}.(j.....
+00009b00: 8e69 6d70 6f72 7420 636f 6f6b 6965 735f  .import cookies_
+00009b10: 7574 696c 6974 6965 7320 6173 2063 750a  utilities as cu.
+00009b20: 7377 203d 2063 752e 5374 6f70 7761 7463  sw = cu.Stopwatc
+00009b30: 6828 290a 7377 2e70 7265 7373 2827 7472  h().sw.press('tr
+00009b40: 6169 6e20 7374 6172 7427 290a 2320 7472  ain start').# tr
+00009b50: 6169 6e0a 7377 2e70 7265 7373 2827 7472  ain.sw.press('tr
+00009b60: 6169 6e20 656e 6427 290a 2320 7465 7374  ain end').# test
+00009b70: 0a73 772e 7072 6573 7328 2774 6573 7420  .sw.press('test 
+00009b80: 656e 6427 290a 7377 2e73 686f 7728 2994  end').sw.show().
+00009b90: 6aec 0200 005d 946a fa02 0000 8c8e 696d  j....].j......im
+00009ba0: 706f 7274 2063 6f6f 6b69 6573 5f75 7469  port cookies_uti
+00009bb0: 6c69 7469 6573 2061 7320 6375 0a73 7720  lities as cu.sw 
+00009bc0: 3d20 6375 2e53 746f 7077 6174 6368 2829  = cu.Stopwatch()
+00009bd0: 0a73 772e 7072 6573 7328 2774 7261 696e  .sw.press('train
+00009be0: 2073 7461 7274 2729 0a23 2074 7261 696e   start').# train
+00009bf0: 0a73 772e 7072 6573 7328 2774 7261 696e  .sw.press('train
+00009c00: 2065 6e64 2729 0a23 2074 6573 740a 7377   end').# test.sw
+00009c10: 2e70 7265 7373 2827 7465 7374 2065 6e64  .press('test end
+00009c20: 2729 0a73 772e 7368 6f77 2829 9485 9481  ').sw.show()....
+00009c30: 947d 946a ff02 0000 6a3b 0b00 0073 6261  .}.j....j;...sba
+00009c40: 6a03 0300 007d 9428 6a05 0300 005d 946a  j....}.(j....].j
+00009c50: 0703 0000 5d94 6a09 0300 005d 946a 0b03  ....].j....].j..
+00009c60: 0000 5d94 6a0d 0300 005d 946a 6003 0000  ..].j....].j`...
+00009c70: 6a61 0300 006a a208 0000 8968 4b8c 0670  ja...j.....hK..p
+00009c80: 7974 686f 6e94 6aa4 0800 007d 9475 6a0f  ython.j....}.uj.
+00009c90: 0300 006a 9208 0000 6a01 0300 006a 1003  ...j....j....j..
+00009ca0: 0000 6a02 0300 004b 4c6a ff02 0000 6a33  ..j....KLj....j3
+00009cb0: 0900 006a 0003 0000 6ae9 0200 0075 626a  ...j....j....ubj
+00009cc0: 9308 0000 2981 947d 9428 6aeb 0200 008c  ....)..}.(j.....
+00009cd0: 5474 696d 6531 2874 7261 696e 2073 7461  Ttime1(train sta
+00009ce0: 7274 2d74 7261 696e 2065 6e64 293a 2032  rt-train end): 2
+00009cf0: 2e30 3030 730a 7469 6d65 3228 7472 6169  .000s.time2(trai
+00009d00: 6e20 656e 642d 7465 7374 2065 6e64 293a  n end-test end):
+00009d10: 2031 2e30 3030 730a 746f 7461 6c3a 2033   1.000s.total: 3
+00009d20: 2e30 3030 7394 6aec 0200 005d 946a fa02  .000s.j....].j..
+00009d30: 0000 8c54 7469 6d65 3128 7472 6169 6e20  ...Ttime1(train 
+00009d40: 7374 6172 742d 7472 6169 6e20 656e 6429  start-train end)
+00009d50: 3a20 322e 3030 3073 0a74 696d 6532 2874  : 2.000s.time2(t
+00009d60: 7261 696e 2065 6e64 2d74 6573 7420 656e  rain end-test en
+00009d70: 6429 3a20 312e 3030 3073 0a74 6f74 616c  d): 1.000s.total
+00009d80: 3a20 332e 3030 3073 9485 9481 947d 946a  : 3.000s.....}.j
+00009d90: ff02 0000 6a4b 0b00 0073 6261 6a03 0300  ....jK...sbaj...
+00009da0: 007d 9428 6a05 0300 005d 946a 0703 0000  .}.(j....].j....
+00009db0: 5d94 6a09 0300 005d 946a 0b03 0000 5d94  ].j....].j....].
+00009dc0: 6a0d 0300 005d 946a 6003 0000 6a61 0300  j....].j`...ja..
+00009dd0: 006a a208 0000 8968 4b8c 0763 6f6e 736f  .j.....hK..conso
+00009de0: 6c65 946a a408 0000 7d94 756a 0f03 0000  le.j....}.uj....
+00009df0: 6a92 0800 006a 0103 0000 6a10 0300 006a  j....j....j....j
+00009e00: 0203 0000 4b57 6aff 0200 006a 3309 0000  ....KWj....j3...
+00009e10: 6a00 0300 006a e902 0000 7562 656a 0303  j....j....ubej..
+00009e20: 0000 7d94 286a 0503 0000 5d94 8c1b 636f  ..}.(j....]...co
+00009e30: 6f6b 6965 732d 7574 696c 6974 6965 732d  okies-utilities-
+00009e40: 7374 6f70 7761 7463 6894 616a 0703 0000  stopwatch.aj....
+00009e50: 5d94 6a09 0300 005d 948c 1b63 6f6f 6b69  ].j....]...cooki
+00009e60: 6573 5f75 7469 6c69 7469 6573 2e73 746f  es_utilities.sto
+00009e70: 7077 6174 6368 9461 6a0b 0300 005d 946a  pwatch.aj....].j
+00009e80: 0d03 0000 5d94 756a 0f03 0000 6830 6aff  ....].uj....h0j.
+00009e90: 0200 006a 2209 0000 6a00 0300 006a e902  ...j"...j....j..
+00009ea0: 0000 6a01 0300 006a 1003 0000 6a02 0300  ..j....j....j...
+00009eb0: 004b 4275 6265 6a03 0300 007d 9428 6a05  .KBubej....}.(j.
+00009ec0: 0300 005d 948c 0763 6c61 7373 6573 9461  ...]...classes.a
+00009ed0: 6a07 0300 005d 946a 0903 0000 5d94 8c07  j....].j....]...
+00009ee0: 636c 6173 7365 7394 616a 0b03 0000 5d94  classes.aj....].
+00009ef0: 6a0d 0300 005d 9475 6a0f 0300 0068 306a  j....].uj....h0j
+00009f00: ff02 0000 6af0 0200 006a 0003 0000 6ae9  ....j....j....j.
+00009f10: 0200 006a 0103 0000 6a10 0300 006a 0203  ...j....j....j..
+00009f20: 0000 4b3f 7562 656a 0303 0000 7d94 286a  ..K?ubej....}.(j
+00009f30: 0503 0000 5d94 8c0d 646f 6375 6d65 6e74  ....]...document
+00009f40: 6174 696f 6e94 616a 0703 0000 5d94 6a09  ation.aj....].j.
+00009f50: 0300 005d 948c 0d64 6f63 756d 656e 7461  ...]...documenta
+00009f60: 7469 6f6e 9461 6a0b 0300 005d 946a 0d03  tion.aj....].j..
+00009f70: 0000 5d94 756a 0f03 0000 6830 6aff 0200  ..].uj....h0j...
+00009f80: 006a e902 0000 6a00 0300 006a e902 0000  .j....j....j....
+00009f90: 6a01 0300 006a 1003 0000 6a02 0300 004b  j....j....j....K
+00009fa0: 0275 6261 6a03 0300 007d 9428 6a05 0300  .ubaj....}.(j...
+00009fb0: 005d 946a 0703 0000 5d94 6a09 0300 005d  .].j....].j....]
+00009fc0: 946a 0b03 0000 5d94 6a0d 0300 005d 948c  .j....].j....]..
+00009fd0: 0673 6f75 7263 6594 6a10 0300 0075 6a0f  .source.j....uj.
+00009fe0: 0300 006a e702 0000 8c0e 6375 7272 656e  ...j......curren
+00009ff0: 745f 736f 7572 6365 944e 8c0c 6375 7272  t_source.N..curr
+0000a000: 656e 745f 6c69 6e65 944e 8c08 7365 7474  ent_line.N..sett
+0000a010: 696e 6773 948c 1164 6f63 7574 696c 732e  ings...docutils.
+0000a020: 6672 6f6e 7465 6e64 948c 0656 616c 7565  frontend...Value
+0000a030: 7394 9394 2981 947d 9428 6af3 0200 004e  s...)..}.(j....N
+0000a040: 8c09 6765 6e65 7261 746f 7294 4e8c 0964  ..generator.N..d
+0000a050: 6174 6573 7461 6d70 944e 8c0b 736f 7572  atestamp.N..sour
+0000a060: 6365 5f6c 696e 6b94 4e8c 0a73 6f75 7263  ce_link.N..sourc
+0000a070: 655f 7572 6c94 4e8c 0d74 6f63 5f62 6163  e_url.N..toc_bac
+0000a080: 6b6c 696e 6b73 948c 0565 6e74 7279 948c  klinks...entry..
+0000a090: 1266 6f6f 746e 6f74 655f 6261 636b 6c69  .footnote_backli
+0000a0a0: 6e6b 7394 4b01 8c0d 7365 6374 6e75 6d5f  nks.K...sectnum_
+0000a0b0: 7866 6f72 6d94 4b01 8c0e 7374 7269 705f  xform.K...strip_
+0000a0c0: 636f 6d6d 656e 7473 944e 8c1b 7374 7269  comments.N..stri
+0000a0d0: 705f 656c 656d 656e 7473 5f77 6974 685f  p_elements_with_
+0000a0e0: 636c 6173 7365 7394 4e8c 0d73 7472 6970  classes.N..strip
+0000a0f0: 5f63 6c61 7373 6573 944e 8c0c 7265 706f  _classes.N..repo
+0000a100: 7274 5f6c 6576 656c 944b 028c 0a68 616c  rt_level.K...hal
+0000a110: 745f 6c65 7665 6c94 4b05 8c11 6578 6974  t_level.K...exit
+0000a120: 5f73 7461 7475 735f 6c65 7665 6c94 4b05  _status_level.K.
+0000a130: 8c05 6465 6275 6794 4e8c 0e77 6172 6e69  ..debug.N..warni
+0000a140: 6e67 5f73 7472 6561 6d94 4e8c 0974 7261  ng_stream.N..tra
+0000a150: 6365 6261 636b 9488 8c0e 696e 7075 745f  ceback....input_
+0000a160: 656e 636f 6469 6e67 9468 638c 1c69 6e70  encoding.hc..inp
+0000a170: 7574 5f65 6e63 6f64 696e 675f 6572 726f  ut_encoding_erro
+0000a180: 725f 6861 6e64 6c65 7294 8c06 7374 7269  r_handler...stri
+0000a190: 6374 948c 0f6f 7574 7075 745f 656e 636f  ct...output_enco
+0000a1a0: 6469 6e67 948c 0575 7466 2d38 948c 1d6f  ding...utf-8...o
+0000a1b0: 7574 7075 745f 656e 636f 6469 6e67 5f65  utput_encoding_e
+0000a1c0: 7272 6f72 5f68 616e 646c 6572 946a 950b  rror_handler.j..
+0000a1d0: 0000 8c0e 6572 726f 725f 656e 636f 6469  ....error_encodi
+0000a1e0: 6e67 948c 0575 7466 2d38 948c 1c65 7272  ng...utf-8...err
+0000a1f0: 6f72 5f65 6e63 6f64 696e 675f 6572 726f  or_encoding_erro
+0000a200: 725f 6861 6e64 6c65 7294 8c10 6261 636b  r_handler...back
+0000a210: 736c 6173 6872 6570 6c61 6365 948c 0d6c  slashreplace...l
+0000a220: 616e 6775 6167 655f 636f 6465 9468 4c8c  anguage_code.hL.
+0000a230: 1372 6563 6f72 645f 6465 7065 6e64 656e  .record_dependen
+0000a240: 6369 6573 944e 8c06 636f 6e66 6967 944e  cies.N..config.N
+0000a250: 8c09 6964 5f70 7265 6669 7894 6840 8c0e  ..id_prefix.h@..
+0000a260: 6175 746f 5f69 645f 7072 6566 6978 946a  auto_id_prefix.j
+0000a270: b102 0000 8c0d 6475 6d70 5f73 6574 7469  ......dump_setti
+0000a280: 6e67 7394 4e8c 0e64 756d 705f 696e 7465  ngs.N..dump_inte
+0000a290: 726e 616c 7394 4e8c 0f64 756d 705f 7472  rnals.N..dump_tr
+0000a2a0: 616e 7366 6f72 6d73 944e 8c0f 6475 6d70  ansforms.N..dump
+0000a2b0: 5f70 7365 7564 6f5f 786d 6c94 4e8c 1065  _pseudo_xml.N..e
+0000a2c0: 7870 6f73 655f 696e 7465 726e 616c 7394  xpose_internals.
+0000a2d0: 4e8c 0e73 7472 6963 745f 7669 7369 746f  N..strict_visito
+0000a2e0: 7294 4e8c 0f5f 6469 7361 626c 655f 636f  r.N.._disable_co
+0000a2f0: 6e66 6967 944e 8c07 5f73 6f75 7263 6594  nfig.N.._source.
+0000a300: 6a10 0300 008c 0c5f 6465 7374 696e 6174  j......_destinat
+0000a310: 696f 6e94 4e8c 0d5f 636f 6e66 6967 5f66  ion.N.._config_f
+0000a320: 696c 6573 945d 948c 1666 696c 655f 696e  iles.]...file_in
+0000a330: 7365 7274 696f 6e5f 656e 6162 6c65 6494  sertion_enabled.
+0000a340: 888c 0b72 6177 5f65 6e61 626c 6564 944b  ...raw_enabled.K
+0000a350: 018c 116c 696e 655f 6c65 6e67 7468 5f6c  ...line_length_l
+0000a360: 696d 6974 944d 1027 8c0e 7065 705f 7265  imit.M.'..pep_re
+0000a370: 6665 7265 6e63 6573 944e 8c0c 7065 705f  ferences.N..pep_
+0000a380: 6261 7365 5f75 726c 946a b702 0000 8c15  base_url.j......
+0000a390: 7065 705f 6669 6c65 5f75 726c 5f74 656d  pep_file_url_tem
+0000a3a0: 706c 6174 6594 8c08 7065 702d 2530 3464  plate...pep-%04d
+0000a3b0: 948c 0e72 6663 5f72 6566 6572 656e 6365  ...rfc_reference
+0000a3c0: 7394 4e8c 0c72 6663 5f62 6173 655f 7572  s.N..rfc_base_ur
+0000a3d0: 6c94 6aba 0200 008c 0974 6162 5f77 6964  l.j......tab_wid
+0000a3e0: 7468 944b 0868 7589 8c10 7379 6e74 6178  th.K.hu...syntax
+0000a3f0: 5f68 6967 686c 6967 6874 948c 046c 6f6e  _highlight...lon
+0000a400: 6794 8c0c 736d 6172 745f 7175 6f74 6573  g...smart_quotes
+0000a410: 9488 8c13 736d 6172 7471 756f 7465 735f  ....smartquotes_
+0000a420: 6c6f 6361 6c65 7394 6ac3 0200 008c 1d63  locales.j......c
+0000a430: 6861 7261 6374 6572 5f6c 6576 656c 5f69  haracter_level_i
+0000a440: 6e6c 696e 655f 6d61 726b 7570 9489 8c0e  nline_markup....
+0000a450: 646f 6374 6974 6c65 5f78 666f 726d 9489  doctitle_xform..
+0000a460: 8c0d 646f 6369 6e66 6f5f 7866 6f72 6d94  ..docinfo_xform.
+0000a470: 4b01 8c12 7365 6374 7375 6274 6974 6c65  K...sectsubtitle
+0000a480: 5f78 666f 726d 9489 8c0d 696d 6167 655f  _xform....image_
+0000a490: 6c6f 6164 696e 6794 6ab3 0200 008c 1065  loading.j......e
+0000a4a0: 6d62 6564 5f73 7479 6c65 7368 6565 7494  mbed_stylesheet.
+0000a4b0: 898c 1563 6c6f 616b 5f65 6d61 696c 5f61  ...cloak_email_a
+0000a4c0: 6464 7265 7373 6573 9488 8c11 7365 6374  ddresses....sect
+0000a4d0: 696f 6e5f 7365 6c66 5f6c 696e 6b94 8968  ion_self_link..h
+0000a4e0: 3c4e 7562 8c08 7265 706f 7274 6572 944e  <Nub..reporter.N
+0000a4f0: 8c10 696e 6469 7265 6374 5f74 6172 6765  ..indirect_targe
+0000a500: 7473 945d 948c 1173 7562 7374 6974 7574  ts.]...substitut
+0000a510: 696f 6e5f 6465 6673 947d 948c 1273 7562  ion_defs.}...sub
+0000a520: 7374 6974 7574 696f 6e5f 6e61 6d65 7394  stitution_names.
+0000a530: 7d94 8c08 7265 666e 616d 6573 947d 948c  }...refnames.}..
+0000a540: 0672 6566 6964 7394 7d94 8c07 6e61 6d65  .refids.}...name
+0000a550: 6964 7394 7d94 286a 700b 0000 6a6d 0b00  ids.}.(jp...jm..
+0000a560: 006a 1f09 0000 6a1c 0900 006a 1709 0000  .j....j....j....
+0000a570: 6a14 0900 006a 680b 0000 6a65 0b00 006a  j....jh...je...j
+0000a580: 600b 0000 6a5d 0b00 0075 8c09 6e61 6d65  `...j]...u..name
+0000a590: 7479 7065 7394 7d94 286a 700b 0000 896a  types.}.(jp....j
+0000a5a0: 1f09 0000 896a 1709 0000 896a 680b 0000  .....j.....jh...
+0000a5b0: 896a 600b 0000 8975 6a05 0300 007d 9428  .j`....uj....}.(
+0000a5c0: 6a6d 0b00 006a f002 0000 6a1c 0900 006a  jm...j....j....j
+0000a5d0: 1103 0000 6a14 0900 006a 2203 0000 6a41  ....j....j"...jA
+0000a5e0: 0300 006a 4a03 0000 6a65 0b00 006a 2209  ...jJ...je...j".
+0000a5f0: 0000 6a5d 0b00 006a 3309 0000 6a50 0900  ..j]...j3...jP..
+0000a600: 006a 5509 0000 6abd 0900 006a c209 0000  .jU...j....j....
+0000a610: 6ab8 0a00 006a be0a 0000 758c 0d66 6f6f  j....j....u..foo
+0000a620: 746e 6f74 655f 7265 6673 947d 948c 0d63  tnote_refs.}...c
+0000a630: 6974 6174 696f 6e5f 7265 6673 947d 948c  itation_refs.}..
+0000a640: 0d61 7574 6f66 6f6f 746e 6f74 6573 945d  .autofootnotes.]
+0000a650: 948c 1161 7574 6f66 6f6f 746e 6f74 655f  ...autofootnote_
+0000a660: 7265 6673 945d 948c 1073 796d 626f 6c5f  refs.]...symbol_
+0000a670: 666f 6f74 6e6f 7465 7394 5d94 8c14 7379  footnotes.]...sy
+0000a680: 6d62 6f6c 5f66 6f6f 746e 6f74 655f 7265  mbol_footnote_re
+0000a690: 6673 945d 948c 0966 6f6f 746e 6f74 6573  fs.]...footnotes
+0000a6a0: 945d 948c 0963 6974 6174 696f 6e73 945d  .]...citations.]
+0000a6b0: 948c 1261 7574 6f66 6f6f 746e 6f74 655f  ...autofootnote_
+0000a6c0: 7374 6172 7494 4b01 8c15 7379 6d62 6f6c  start.K...symbol
+0000a6d0: 5f66 6f6f 746e 6f74 655f 7374 6172 7494  _footnote_start.
+0000a6e0: 4b00 8c0a 6964 5f63 6f75 6e74 6572 946a  K...id_counter.j
+0000a6f0: cd02 0000 8c07 436f 756e 7465 7294 9394  ......Counter...
+0000a700: 7d94 8594 5294 8c0e 7061 7273 655f 6d65  }...R...parse_me
+0000a710: 7373 6167 6573 945d 948c 1274 7261 6e73  ssages.]...trans
+0000a720: 666f 726d 5f6d 6573 7361 6765 7394 5d94  form_messages.].
+0000a730: 8c0b 7472 616e 7366 6f72 6d65 7294 4e8c  ..transformer.N.
+0000a740: 0b69 6e63 6c75 6465 5f6c 6f67 945d 948c  .include_log.]..
+0000a750: 0a64 6563 6f72 6174 696f 6e94 4e6a 0003  .decoration.Nj..
+0000a760: 0000 6ae9 0200 0075 628c 0569 6e64 6578  ..j....ub..index
+0000a770: 946a e802 0000 2981 947d 9428 6aeb 0200  .j....)..}.(j...
+0000a780: 0068 406a ec02 0000 5d94 6aef 0200 0029  .h@j....].j....)
+0000a790: 8194 7d94 286a eb02 0000 6840 6aec 0200  ..}.(j....h@j...
+0000a7a0: 005d 9428 6af4 0200 0029 8194 7d94 286a  .].(j....)..}.(j
+0000a7b0: eb02 0000 8c2c 5765 6c63 6f6d 6520 746f  .....,Welcome to
+0000a7c0: 2063 6f6f 6b69 6573 5f75 7469 6c69 7469   cookies_utiliti
+0000a7d0: 6573 2720 646f 6375 6d65 6e74 6174 696f  es' documentatio
+0000a7e0: 6e21 946a ec02 0000 5d94 6afa 0200 008c  n!.j....].j.....
+0000a7f0: 2e57 656c 636f 6d65 2074 6f20 636f 6f6b  .Welcome to cook
+0000a800: 6965 735f 7574 696c 6974 6965 73e2 8099  ies_utilities...
+0000a810: 2064 6f63 756d 656e 7461 7469 6f6e 2194   documentation!.
+0000a820: 8594 8194 7d94 286a ff02 0000 6afa 0b00  ....}.(j....j...
+0000a830: 006a 0003 0000 6af4 0b00 006a 0103 0000  .j....j....j....
+0000a840: 4e6a 0203 0000 4e75 6261 6a03 0300 007d  Nj....Nubaj....}
+0000a850: 9428 8c03 6964 7394 5d94 8c07 636c 6173  .(..ids.]...clas
+0000a860: 7365 7394 5d94 8c05 6e61 6d65 7394 5d94  ses.]...names.].
+0000a870: 8c08 6475 706e 616d 6573 945d 948c 0862  ..dupnames.]...b
+0000a880: 6163 6b72 6566 7394 5d94 756a 0f03 0000  ackrefs.].uj....
+0000a890: 8c05 7469 746c 6594 6aff 0200 006a f70b  ..title.j....j..
+0000a8a0: 0000 6a00 0300 006a f40b 0000 6a01 0300  ..j....j....j...
+0000a8b0: 008c 3c43 3a5c 5573 6572 735c 632d 6d69  ..<C:\Users\c-mi
+0000a8c0: 685c 7370 6163 655c 636f 6f6b 6965 735f  h\space\cookies_
+0000a8d0: 7574 696c 6974 6965 735c 646f 6373 5c73  utilities\docs\s
+0000a8e0: 6f75 7263 655c 696e 6465 782e 7273 7494  ource\index.rst.
+0000a8f0: 6a02 0300 004b 0275 626a ef02 0000 2981  j....K.ubj....).
+0000a900: 947d 9428 6aeb 0200 0068 406a ec02 0000  .}.(j....h@j....
+0000a910: 5d94 286a f402 0000 2981 947d 9428 6aeb  ].(j....)..}.(j.
+0000a920: 0200 008c 054c 696e 6b73 946a ec02 0000  .....Links.j....
+0000a930: 5d94 6afa 0200 008c 054c 696e 6b73 9485  ].j......Links..
+0000a940: 9481 947d 9428 6aff 0200 006a 120c 0000  ...}.(j....j....
+0000a950: 6a00 0300 006a f40b 0000 6a01 0300 004e  j....j....j....N
+0000a960: 6a02 0300 004e 7562 616a 0303 0000 7d94  j....Nubaj....}.
+0000a970: 286a 030c 0000 5d94 6a05 0c00 005d 946a  (j....].j....].j
+0000a980: 070c 0000 5d94 6a09 0c00 005d 946a 0b0c  ....].j....].j..
+0000a990: 0000 5d94 756a 0f03 0000 6a0d 0c00 006a  ..].uj....j....j
+0000a9a0: ff02 0000 6a0f 0c00 006a 0003 0000 6af4  ....j....j....j.
+0000a9b0: 0b00 006a 0103 0000 6a0e 0c00 006a 0203  ...j....j....j..
+0000a9c0: 0000 4b05 7562 6a15 0b00 0029 8194 7d94  ..K.ubj....)..}.
+0000a9d0: 286a eb02 0000 8c40 2d20 6054 6573 7450  (j.....@- `TestP
+0000a9e0: 7950 4920 3c68 7474 7073 3a2f 2f74 6573  yPI <https://tes
+0000a9f0: 742e 7079 7069 2e6f 7267 2f70 726f 6a65  t.pypi.org/proje
+0000aa00: 6374 2f63 6f6f 6b69 6573 2d75 7469 6c69  ct/cookies-utili
+0000aa10: 7469 6573 2f3e 605f 946a ec02 0000 5d94  ties/>`_.j....].
+0000aa20: 6afa 0200 008c 402d 2060 5465 7374 5079  j.....@- `TestPy
+0000aa30: 5049 203c 6874 7470 733a 2f2f 7465 7374  PI <https://test
+0000aa40: 2e70 7970 692e 6f72 672f 7072 6f6a 6563  .pypi.org/projec
+0000aa50: 742f 636f 6f6b 6965 732d 7574 696c 6974  t/cookies-utilit
+0000aa60: 6965 732f 3e60 5f94 8594 8194 7d94 6aff  ies/>`_.....}.j.
+0000aa70: 0200 006a 200c 0000 7362 616a 0303 0000  ...j ...sbaj....
+0000aa80: 7d94 286a 030c 0000 5d94 6a05 0c00 005d  }.(j....].j....]
+0000aa90: 946a 070c 0000 5d94 6a09 0c00 005d 946a  .j....].j....].j
+0000aaa0: 0b0c 0000 5d94 8c09 786d 6c3a 7370 6163  ....]...xml:spac
+0000aab0: 6594 8c08 7072 6573 6572 7665 9475 6a0f  e...preserve.uj.
+0000aac0: 0300 008c 0763 6f6d 6d65 6e74 946a ff02  .....comment.j..
+0000aad0: 0000 6a0f 0c00 006a 0003 0000 6af4 0b00  ..j....j....j...
+0000aae0: 006a 0103 0000 6a0e 0c00 006a 0203 0000  .j....j....j....
+0000aaf0: 4b08 7562 6a65 0500 0029 8194 7d94 286a  K.ubje...)..}.(j
+0000ab00: eb02 0000 6840 6aec 0200 005d 9428 6a6a  ....h@j....].(jj
+0000ab10: 0500 0029 8194 7d94 286a eb02 0000 8c35  ...)..}.(j.....5
+0000ab20: 6050 7950 4920 3c68 7474 7073 3a2f 2f70  `PyPI <https://p
+0000ab30: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+0000ab40: 636f 6f6b 6965 732d 7574 696c 6974 6965  cookies-utilitie
+0000ab50: 732f 3e60 5f94 6aec 0200 005d 946a 1305  s/>`_.j....].j..
+0000ab60: 0000 2981 947d 9428 6aeb 0200 006a 360c  ..)..}.(j....j6.
+0000ab70: 0000 6aec 0200 005d 9428 6aee 0200 008c  ..j....].(j.....
+0000ab80: 0972 6566 6572 656e 6365 9493 9429 8194  .reference...)..
+0000ab90: 7d94 286a eb02 0000 6a36 0c00 006a ec02  }.(j....j6...j..
+0000aba0: 0000 5d94 6afa 0200 008c 0450 7950 4994  ..].j......PyPI.
+0000abb0: 8594 8194 7d94 286a ff02 0000 6a3d 0c00  ....}.(j....j=..
+0000abc0: 006a 0003 0000 6af4 0b00 006a 0103 0000  .j....j....j....
+0000abd0: 4e6a 0203 0000 4e75 6261 6a03 0300 007d  Nj....Nubaj....}
+0000abe0: 9428 6a03 0c00 005d 946a 050c 0000 5d94  .(j....].j....].
+0000abf0: 6a07 0c00 005d 946a 090c 0000 5d94 6a0b  j....].j....].j.
+0000ac00: 0c00 005d 948c 046e 616d 6594 8c04 5079  ...]...name...Py
+0000ac10: 5049 948c 0672 6566 7572 6994 8c2b 6874  PI...refuri..+ht
+0000ac20: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+0000ac30: 726f 6a65 6374 2f63 6f6f 6b69 6573 2d75  roject/cookies-u
+0000ac40: 7469 6c69 7469 6573 2f94 756a 0f03 0000  tilities/.uj....
+0000ac50: 8c09 7265 6665 7265 6e63 6594 6aff 0200  ..reference.j...
+0000ac60: 006a 380c 0000 7562 6aee 0200 008c 0674  .j8...ubj......t
+0000ac70: 6172 6765 7494 9394 2981 947d 9428 6aeb  arget...)..}.(j.
+0000ac80: 0200 008c 2e20 3c68 7474 7073 3a2f 2f70  ..... <https://p
+0000ac90: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+0000aca0: 636f 6f6b 6965 732d 7574 696c 6974 6965  cookies-utilitie
+0000acb0: 732f 3e94 6aec 0200 005d 946a 0303 0000  s/>.j....].j....
+0000acc0: 7d94 286a 030c 0000 5d94 8c04 7079 7069  }.(j....]...pypi
+0000acd0: 9461 6a05 0c00 005d 946a 070c 0000 5d94  .aj....].j....].
+0000ace0: 8c04 7079 7069 9461 6a09 0c00 005d 946a  ..pypi.aj....].j
+0000acf0: 0b0c 0000 5d94 8c06 7265 6675 7269 946a  ....]...refuri.j
+0000ad00: 4d0c 0000 756a 0f03 0000 8c06 7461 7267  M...uj......targ
+0000ad10: 6574 948c 0a72 6566 6572 656e 6365 6494  et...referenced.
+0000ad20: 4b01 6aff 0200 006a 380c 0000 7562 656a  K.j....j8...ubej
+0000ad30: 0303 0000 7d94 286a 030c 0000 5d94 6a05  ....}.(j....].j.
+0000ad40: 0c00 005d 946a 070c 0000 5d94 6a09 0c00  ...].j....].j...
+0000ad50: 005d 946a 0b0c 0000 5d94 756a 0f03 0000  .].j....].uj....
+0000ad60: 8c09 7061 7261 6772 6170 6894 6a01 0300  ..paragraph.j...
+0000ad70: 006a 0e0c 0000 6a02 0300 004b 096a ff02  .j....j....K.j..
+0000ad80: 0000 6a34 0c00 0075 6261 6a03 0300 007d  ..j4...ubaj....}
+0000ad90: 9428 6a03 0c00 005d 946a 050c 0000 5d94  .(j....].j....].
+0000ada0: 6a07 0c00 005d 946a 090c 0000 5d94 6a0b  j....].j....].j.
+0000adb0: 0c00 005d 9475 6a0f 0300 008c 096c 6973  ...].uj......lis
+0000adc0: 745f 6974 656d 946a ff02 0000 6a31 0c00  t_item.j....j1..
+0000add0: 006a 0003 0000 6af4 0b00 006a 0103 0000  .j....j....j....
+0000ade0: 6a0e 0c00 006a 0203 0000 4e75 626a 6a05  j....j....Nubjj.
+0000adf0: 0000 2981 947d 9428 6aeb 0200 008c 3d60  ..)..}.(j.....=`
+0000ae00: 4769 7448 7562 203c 6874 7470 733a 2f2f  GitHub <https://
+0000ae10: 6769 7468 7562 2e63 6f6d 2f43 6f6f 6b69  github.com/Cooki
+0000ae20: 6542 6f78 3236 2f63 6f6f 6b69 6573 5f75  eBox26/cookies_u
+0000ae30: 7469 6c69 7469 6573 3e60 5f0a 946a ec02  tilities>`_..j..
+0000ae40: 0000 5d94 6a13 0500 0029 8194 7d94 286a  ..].j....)..}.(j
+0000ae50: eb02 0000 8c3c 6047 6974 4875 6220 3c68  .....<`GitHub <h
+0000ae60: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+0000ae70: 6d2f 436f 6f6b 6965 426f 7832 362f 636f  m/CookieBox26/co
+0000ae80: 6f6b 6965 735f 7574 696c 6974 6965 733e  okies_utilities>
+0000ae90: 605f 946a ec02 0000 5d94 286a 3c0c 0000  `_.j....].(j<...
+0000aea0: 2981 947d 9428 6aeb 0200 006a 740c 0000  )..}.(j....jt...
+0000aeb0: 6aec 0200 005d 946a fa02 0000 8c06 4769  j....].j......Gi
+0000aec0: 7448 7562 9485 9481 947d 9428 6aff 0200  tHub.....}.(j...
+0000aed0: 006a 760c 0000 6a00 0300 006a f40b 0000  .jv...j....j....
+0000aee0: 6a01 0300 004e 6a02 0300 004e 7562 616a  j....Nj....Nubaj
+0000aef0: 0303 0000 7d94 286a 030c 0000 5d94 6a05  ....}.(j....].j.
+0000af00: 0c00 005d 946a 070c 0000 5d94 6a09 0c00  ...].j....].j...
+0000af10: 005d 946a 0b0c 0000 5d94 8c04 6e61 6d65  .].j....]...name
+0000af20: 948c 0647 6974 4875 6294 6a4c 0c00 008c  ...GitHub.jL....
+0000af30: 3068 7474 7073 3a2f 2f67 6974 6875 622e  0https://github.
+0000af40: 636f 6d2f 436f 6f6b 6965 426f 7832 362f  com/CookieBox26/
+0000af50: 636f 6f6b 6965 735f 7574 696c 6974 6965  cookies_utilitie
+0000af60: 7394 756a 0f03 0000 6a4e 0c00 006a ff02  s.uj....jN...j..
+0000af70: 0000 6a72 0c00 0075 626a 500c 0000 2981  ..jr...ubjP...).
+0000af80: 947d 9428 6aeb 0200 008c 3320 3c68 7474  .}.(j.....3 <htt
+0000af90: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+0000afa0: 436f 6f6b 6965 426f 7832 362f 636f 6f6b  CookieBox26/cook
+0000afb0: 6965 735f 7574 696c 6974 6965 733e 946a  ies_utilities>.j
+0000afc0: ec02 0000 5d94 6a03 0300 007d 9428 6a03  ....].j....}.(j.
+0000afd0: 0c00 005d 948c 0667 6974 6875 6294 616a  ...]...github.aj
+0000afe0: 050c 0000 5d94 6a07 0c00 005d 948c 0667  ....].j....]...g
+0000aff0: 6974 6875 6294 616a 090c 0000 5d94 6a0b  ithub.aj....].j.
+0000b000: 0c00 005d 948c 0672 6566 7572 6994 6a85  ...]...refuri.j.
+0000b010: 0c00 0075 6a0f 0300 006a 5e0c 0000 6a5f  ...uj....j^...j_
+0000b020: 0c00 004b 016a ff02 0000 6a72 0c00 0075  ...K.j....jr...u
+0000b030: 6265 6a03 0300 007d 9428 6a03 0c00 005d  bej....}.(j....]
+0000b040: 946a 050c 0000 5d94 6a07 0c00 005d 946a  .j....].j....].j
+0000b050: 090c 0000 5d94 6a0b 0c00 005d 9475 6a0f  ....].j....].uj.
+0000b060: 0300 006a 660c 0000 6a01 0300 006a 0e0c  ...jf...j....j..
+0000b070: 0000 6a02 0300 004b 0a6a ff02 0000 6a6e  ..j....K.j....jn
+0000b080: 0c00 0075 6261 6a03 0300 007d 9428 6a03  ...ubaj....}.(j.
+0000b090: 0c00 005d 946a 050c 0000 5d94 6a07 0c00  ...].j....].j...
+0000b0a0: 005d 946a 090c 0000 5d94 6a0b 0c00 005d  .].j....].j....]
+0000b0b0: 9475 6a0f 0300 006a 6d0c 0000 6aff 0200  .uj....jm...j...
+0000b0c0: 006a 310c 0000 6a00 0300 006a f40b 0000  .j1...j....j....
+0000b0d0: 6a01 0300 006a 0e0c 0000 6a02 0300 004e  j....j....j....N
+0000b0e0: 7562 656a 0303 0000 7d94 286a 030c 0000  ubej....}.(j....
+0000b0f0: 5d94 6a05 0c00 005d 946a 070c 0000 5d94  ].j....].j....].
+0000b100: 6a09 0c00 005d 946a 0b0c 0000 5d94 8c06  j....].j....]...
+0000b110: 6275 6c6c 6574 948c 012d 9475 6a0f 0300  bullet...-.uj...
+0000b120: 008c 0b62 756c 6c65 745f 6c69 7374 946a  ...bullet_list.j
+0000b130: 0103 0000 6a0e 0c00 006a 0203 0000 4b09  ....j....j....K.
+0000b140: 6aff 0200 006a 0f0c 0000 6a00 0300 006a  j....j....j....j
+0000b150: f40b 0000 7562 6aee 0200 008c 0863 6f6d  ....ubj......com
+0000b160: 706f 756e 6494 9394 2981 947d 9428 6aeb  pound...)..}.(j.
+0000b170: 0200 0068 406a ec02 0000 5d94 6ae6 0200  ...h@j....].j...
+0000b180: 008c 0774 6f63 7472 6565 9493 9429 8194  ...toctree...)..
+0000b190: 7d94 286a eb02 0000 6840 6aec 0200 005d  }.(j....h@j....]
+0000b1a0: 946a 0303 0000 7d94 286a 030c 0000 5d94  .j....}.(j....].
+0000b1b0: 6a05 0c00 005d 946a 070c 0000 5d94 6a09  j....].j....].j.
+0000b1c0: 0c00 005d 946a 0b0c 0000 5d94 8c06 7061  ...].j....]...pa
+0000b1d0: 7265 6e74 946a ca02 0000 8c07 656e 7472  rent.j......entr
+0000b1e0: 6965 7394 5d94 4e8c 1163 6f6f 6b69 6573  ies.].N..cookies
+0000b1f0: 5f75 7469 6c69 7469 6573 9486 9461 8c0c  _utilities...a..
+0000b200: 696e 636c 7564 6566 696c 6573 945d 946a  includefiles.].j
+0000b210: bb0c 0000 618c 086d 6178 6465 7074 6894  ....a..maxdepth.
+0000b220: 4b02 8c07 6361 7074 696f 6e94 8c09 436f  K...caption...Co
+0000b230: 6e74 656e 7473 3a94 8c04 676c 6f62 9489  ntents:...glob..
+0000b240: 8c06 6869 6464 656e 9489 8c0d 696e 636c  ..hidden....incl
+0000b250: 7564 6568 6964 6465 6e94 898c 086e 756d  udehidden....num
+0000b260: 6265 7265 6494 4b00 8c0a 7469 746c 6573  bered.K...titles
+0000b270: 6f6e 6c79 9489 8c0a 7261 7765 6e74 7269  only....rawentri
+0000b280: 6573 945d 948c 0a72 6177 6361 7074 696f  es.]...rawcaptio
+0000b290: 6e94 6ac1 0c00 0075 6a0f 0300 008c 0774  n.j....uj......t
+0000b2a0: 6f63 7472 6565 946a 0103 0000 6a0e 0c00  octree.j....j...
+0000b2b0: 006a 0203 0000 4b0c 6aff 0200 006a aa0c  .j....K.j....j..
+0000b2c0: 0000 7562 616a 0303 0000 7d94 286a 030c  ..ubaj....}.(j..
+0000b2d0: 0000 5d94 6a05 0c00 005d 948c 0f74 6f63  ..].j....]...toc
+0000b2e0: 7472 6565 2d77 7261 7070 6572 9461 6a07  tree-wrapper.aj.
+0000b2f0: 0c00 005d 946a 090c 0000 5d94 6a0b 0c00  ...].j....].j...
+0000b300: 005d 9475 6a0f 0300 008c 0863 6f6d 706f  .].uj......compo
+0000b310: 756e 6494 6aff 0200 006a 0f0c 0000 6a00  und.j....j....j.
+0000b320: 0300 006a f40b 0000 6a01 0300 006a 0e0c  ...j....j....j..
+0000b330: 0000 6a02 0300 004e 7562 656a 0303 0000  ..j....Nubej....
+0000b340: 7d94 286a 030c 0000 5d94 8c05 6c69 6e6b  }.(j....]...link
+0000b350: 7394 616a 050c 0000 5d94 6a07 0c00 005d  s.aj....].j....]
+0000b360: 948c 056c 696e 6b73 9461 6a09 0c00 005d  ...links.aj....]
+0000b370: 946a 0b0c 0000 5d94 756a 0f03 0000 8c07  .j....].uj......
+0000b380: 7365 6374 696f 6e94 6aff 0200 006a f70b  section.j....j..
+0000b390: 0000 6a00 0300 006a f40b 0000 6a01 0300  ..j....j....j...
+0000b3a0: 006a 0e0c 0000 6a02 0300 004b 0575 626a  .j....j....K.ubj
+0000b3b0: ef02 0000 2981 947d 9428 6aeb 0200 0068  ....)..}.(j....h
+0000b3c0: 406a ec02 0000 5d94 286a f402 0000 2981  @j....].(j....).
+0000b3d0: 947d 9428 6aeb 0200 008c 1249 6e64 6963  .}.(j......Indic
+0000b3e0: 6573 2061 6e64 2074 6162 6c65 7394 6aec  es and tables.j.
+0000b3f0: 0200 005d 946a fa02 0000 8c12 496e 6469  ...].j......Indi
+0000b400: 6365 7320 616e 6420 7461 626c 6573 9485  ces and tables..
+0000b410: 9481 947d 9428 6aff 0200 006a df0c 0000  ...}.(j....j....
+0000b420: 6a00 0300 006a f40b 0000 6a01 0300 004e  j....j....j....N
+0000b430: 6a02 0300 004e 7562 616a 0303 0000 7d94  j....Nubaj....}.
+0000b440: 286a 030c 0000 5d94 6a05 0c00 005d 946a  (j....].j....].j
+0000b450: 070c 0000 5d94 6a09 0c00 005d 946a 0b0c  ....].j....].j..
+0000b460: 0000 5d94 756a 0f03 0000 6a0d 0c00 006a  ..].uj....j....j
+0000b470: ff02 0000 6adc 0c00 006a 0003 0000 6af4  ....j....j....j.
+0000b480: 0b00 006a 0103 0000 6a0e 0c00 006a 0203  ...j....j....j..
+0000b490: 0000 4b13 7562 6a65 0500 0029 8194 7d94  ..K.ubje...)..}.
+0000b4a0: 286a eb02 0000 6840 6aec 0200 005d 946a  (j....h@j....].j
+0000b4b0: 6a05 0000 2981 947d 9428 6aeb 0200 008c  j...)..}.(j.....
+0000b4c0: 0f3a 7265 663a 6067 656e 696e 6465 7860  .:ref:`genindex`
+0000b4d0: 946a ec02 0000 5d94 6a13 0500 0029 8194  .j....].j....)..
+0000b4e0: 7d94 286a eb02 0000 6af2 0c00 006a ec02  }.(j....j....j..
+0000b4f0: 0000 5d94 6a87 0500 0029 8194 7d94 286a  ..].j....)..}.(j
+0000b500: eb02 0000 6af2 0c00 006a ec02 0000 5d94  ....j....j....].
+0000b510: 6aa3 0300 0029 8194 7d94 286a eb02 0000  j....)..}.(j....
+0000b520: 6af2 0c00 006a ec02 0000 5d94 6afa 0200  j....j....].j...
+0000b530: 008c 0867 656e 696e 6465 7894 8594 8194  ...genindex.....
+0000b540: 7d94 286a ff02 0000 6afa 0c00 006a 0003  }.(j....j....j..
+0000b550: 0000 6af4 0b00 006a 0103 0000 4e6a 0203  ..j....j....Nj..
+0000b560: 0000 4e75 6261 6a03 0300 007d 9428 6a03  ..Nubaj....}.(j.
+0000b570: 0c00 005d 946a 050c 0000 5d94 288c 0478  ...].j....].(..x
+0000b580: 7265 6694 8c03 7374 6494 8c07 7374 642d  ref...std...std-
+0000b590: 7265 6694 656a 070c 0000 5d94 6a09 0c00  ref.ej....].j...
+0000b5a0: 005d 946a 0b0c 0000 5d94 756a 0f03 0000  .].j....].uj....
+0000b5b0: 8c06 696e 6c69 6e65 946a ff02 0000 6af7  ..inline.j....j.
+0000b5c0: 0c00 0075 6261 6a03 0300 007d 9428 6a03  ...ubaj....}.(j.
+0000b5d0: 0c00 005d 946a 050c 0000 5d94 6a07 0c00  ...].j....].j...
+0000b5e0: 005d 946a 090c 0000 5d94 6a0b 0c00 005d  .].j....].j....]
+0000b5f0: 948c 0672 6566 646f 6394 6aca 0200 008c  ...refdoc.j.....
+0000b600: 0972 6566 646f 6d61 696e 946a 050d 0000  .refdomain.j....
+0000b610: 8c07 7265 6674 7970 6594 8c03 7265 6694  ..reftype...ref.
+0000b620: 8c0b 7265 6665 7870 6c69 6369 7494 898c  ..refexplicit...
+0000b630: 0772 6566 7761 726e 9488 8c09 7265 6674  .refwarn....reft
+0000b640: 6172 6765 7494 8c08 6765 6e69 6e64 6578  arget...genindex
+0000b650: 9475 6a0f 0300 008c 0c70 656e 6469 6e67  .uj......pending
+0000b660: 5f78 7265 6694 6a01 0300 006a 0e0c 0000  _xref.j....j....
+0000b670: 6a02 0300 004b 156a ff02 0000 6af4 0c00  j....K.j....j...
+0000b680: 0075 6261 6a03 0300 007d 9428 6a03 0c00  .ubaj....}.(j...
+0000b690: 005d 946a 050c 0000 5d94 6a07 0c00 005d  .].j....].j....]
+0000b6a0: 946a 090c 0000 5d94 6a0b 0c00 005d 9475  .j....].j....].u
+0000b6b0: 6a0f 0300 006a 660c 0000 6a01 0300 006a  j....jf...j....j
+0000b6c0: 0e0c 0000 6a02 0300 004b 156a ff02 0000  ....j....K.j....
+0000b6d0: 6af0 0c00 0075 6261 6a03 0300 007d 9428  j....ubaj....}.(
+0000b6e0: 6a03 0c00 005d 946a 050c 0000 5d94 6a07  j....].j....].j.
+0000b6f0: 0c00 005d 946a 090c 0000 5d94 6a0b 0c00  ...].j....].j...
+0000b700: 005d 9475 6a0f 0300 006a 6d0c 0000 6aff  .].uj....jm...j.
+0000b710: 0200 006a ed0c 0000 6a00 0300 006a f40b  ...j....j....j..
+0000b720: 0000 6a01 0300 006a 0e0c 0000 6a02 0300  ..j....j....j...
+0000b730: 004e 7562 616a 0303 0000 7d94 286a 030c  .Nubaj....}.(j..
+0000b740: 0000 5d94 6a05 0c00 005d 946a 070c 0000  ..].j....].j....
+0000b750: 5d94 6a09 0c00 005d 946a 0b0c 0000 5d94  ].j....].j....].
+0000b760: 6aa5 0c00 008c 012a 9475 6a0f 0300 006a  j......*.uj....j
+0000b770: a70c 0000 6a01 0300 006a 0e0c 0000 6a02  ....j....j....j.
+0000b780: 0300 004b 156a ff02 0000 6adc 0c00 006a  ...K.j....j....j
+0000b790: 0003 0000 6af4 0b00 0075 6265 6a03 0300  ....j....ubej...
+0000b7a0: 007d 9428 6a03 0c00 005d 948c 1269 6e64  .}.(j....]...ind
+0000b7b0: 6963 6573 2d61 6e64 2d74 6162 6c65 7394  ices-and-tables.
+0000b7c0: 616a 050c 0000 5d94 6a07 0c00 005d 948c  aj....].j....]..
+0000b7d0: 1269 6e64 6963 6573 2061 6e64 2074 6162  .indices and tab
+0000b7e0: 6c65 7394 616a 090c 0000 5d94 6a0b 0c00  les.aj....].j...
+0000b7f0: 005d 9475 6a0f 0300 006a db0c 0000 6aff  .].uj....j....j.
+0000b800: 0200 006a f70b 0000 6a00 0300 006a f40b  ...j....j....j..
+0000b810: 0000 6a01 0300 006a 0e0c 0000 6a02 0300  ..j....j....j...
+0000b820: 004b 1375 6265 6a03 0300 007d 9428 6a03  .K.ubej....}.(j.
+0000b830: 0c00 005d 948c 2a77 656c 636f 6d65 2d74  ...]..*welcome-t
+0000b840: 6f2d 636f 6f6b 6965 732d 7574 696c 6974  o-cookies-utilit
+0000b850: 6965 732d 646f 6375 6d65 6e74 6174 696f  ies-documentatio
+0000b860: 6e94 616a 050c 0000 5d94 6a07 0c00 005d  n.aj....].j....]
+0000b870: 948c 2c77 656c 636f 6d65 2074 6f20 636f  ..,welcome to co
+0000b880: 6f6b 6965 735f 7574 696c 6974 6965 7327  okies_utilities'
+0000b890: 2064 6f63 756d 656e 7461 7469 6f6e 2194   documentation!.
+0000b8a0: 616a 090c 0000 5d94 6a0b 0c00 005d 9475  aj....].j....].u
+0000b8b0: 6a0f 0300 006a db0c 0000 6aff 0200 006a  j....j....j....j
+0000b8c0: f40b 0000 6a00 0300 006a f40b 0000 6a01  ....j....j....j.
+0000b8d0: 0300 006a 0e0c 0000 6a02 0300 004b 0275  ...j....j....K.u
+0000b8e0: 6261 6a03 0300 007d 9428 6a03 0c00 005d  baj....}.(j....]
+0000b8f0: 946a 050c 0000 5d94 6a07 0c00 005d 946a  .j....].j....].j
+0000b900: 090c 0000 5d94 6a0b 0c00 005d 948c 0673  ....].j....]...s
+0000b910: 6f75 7263 6594 6a0e 0c00 0075 6a0f 0300  ource.j....uj...
+0000b920: 008c 0864 6f63 756d 656e 7494 6a7a 0b00  ...document.jz..
+0000b930: 004e 6a7b 0b00 004e 6a7c 0b00 006a 7f0b  .Nj{...Nj|...j..
+0000b940: 0000 2981 947d 9428 6af3 0200 004e 6a82  ..)..}.(j....Nj.
+0000b950: 0b00 004e 6a83 0b00 004e 6a84 0b00 004e  ...Nj....Nj....N
+0000b960: 6a85 0b00 004e 6a86 0b00 008c 0565 6e74  j....Nj......ent
+0000b970: 7279 946a 880b 0000 4b01 6a89 0b00 004b  ry.j....K.j....K
+0000b980: 016a 8a0b 0000 4e6a 8b0b 0000 4e6a 8c0b  .j....Nj....Nj..
+0000b990: 0000 4e6a 8d0b 0000 4b02 6a8e 0b00 004b  ..Nj....K.j....K
+0000b9a0: 056a 8f0b 0000 4b05 6a90 0b00 004e 6a91  .j....K.j....Nj.
+0000b9b0: 0b00 004e 6a92 0b00 0088 6a93 0b00 008c  ...Nj.....j.....
+0000b9c0: 0975 7466 2d38 2d73 6967 946a 940b 0000  .utf-8-sig.j....
+0000b9d0: 8c06 7374 7269 6374 946a 960b 0000 8c05  ..strict.j......
+0000b9e0: 7574 662d 3894 6a98 0b00 006a 490d 0000  utf-8.j....jI...
+0000b9f0: 6a99 0b00 008c 0575 7466 2d38 946a 9b0b  j......utf-8.j..
+0000ba00: 0000 8c10 6261 636b 736c 6173 6872 6570  ....backslashrep
+0000ba10: 6c61 6365 946a 9d0b 0000 8c02 656e 946a  lace.j......en.j
+0000ba20: 9e0b 0000 4e6a 9f0b 0000 4e6a a00b 0000  ....Nj....Nj....
+0000ba30: 6840 6aa1 0b00 006a b102 0000 6aa2 0b00  h@j....j....j...
+0000ba40: 004e 6aa3 0b00 004e 6aa4 0b00 004e 6aa5  .Nj....Nj....Nj.
+0000ba50: 0b00 004e 6aa6 0b00 004e 6aa7 0b00 004e  ...Nj....Nj....N
+0000ba60: 6aa8 0b00 004e 6aa9 0b00 006a 0e0c 0000  j....Nj....j....
+0000ba70: 6aaa 0b00 004e 6aab 0b00 005d 946a ad0b  j....Nj....].j..
+0000ba80: 0000 886a ae0b 0000 4b01 6aaf 0b00 004d  ...j....K.j....M
+0000ba90: 1027 6ab0 0b00 004e 6ab1 0b00 006a b702  .'j....Nj....j..
+0000baa0: 0000 6ab2 0b00 008c 0870 6570 2d25 3034  ..j......pep-%04
+0000bab0: 6494 6ab4 0b00 004e 6ab5 0b00 006a ba02  d.j....Nj....j..
+0000bac0: 0000 6ab6 0b00 004b 0868 7589 6ab7 0b00  ..j....K.hu.j...
+0000bad0: 008c 046c 6f6e 6794 6ab9 0b00 0088 6aba  ...long.j.....j.
+0000bae0: 0b00 006a c302 0000 6abb 0b00 0089 6abc  ...j....j.....j.
+0000baf0: 0b00 0089 6abd 0b00 004b 016a be0b 0000  ....j....K.j....
+0000bb00: 896a bf0b 0000 6ab3 0200 006a c00b 0000  .j....j....j....
+0000bb10: 896a c10b 0000 886a c20b 0000 8968 3c4e  .j.....j.....h<N
+0000bb20: 7562 6ac3 0b00 004e 6ac4 0b00 005d 946a  ubj....Nj....].j
+0000bb30: c60b 0000 7d94 6ac8 0b00 007d 946a ca0b  ....}.j....}.j..
+0000bb40: 0000 7d94 6acc 0b00 007d 946a ce0b 0000  ..}.j....}.j....
+0000bb50: 7d94 286a 3a0d 0000 6a37 0d00 006a d80c  }.(j:...j7...j..
+0000bb60: 0000 6ad5 0c00 006a 5a0c 0000 6a57 0c00  ..j....jZ...jW..
+0000bb70: 006a 8f0c 0000 6a8c 0c00 006a 320d 0000  .j....j....j2...
+0000bb80: 6a2f 0d00 0075 6ad0 0b00 007d 9428 6a3a  j/...uj....}.(j:
+0000bb90: 0d00 0089 6ad8 0c00 0089 6a5a 0c00 0088  ....j.....jZ....
+0000bba0: 6a8f 0c00 0088 6a32 0d00 0089 756a 0503  j.....j2....uj..
+0000bbb0: 0000 7d94 286a 370d 0000 6af7 0b00 006a  ..}.(j7...j....j
+0000bbc0: d50c 0000 6a0f 0c00 006a 570c 0000 6a51  ....j....jW...jQ
+0000bbd0: 0c00 006a 8c0c 0000 6a86 0c00 006a 2f0d  ...j....j....j/.
+0000bbe0: 0000 6adc 0c00 0075 6ad3 0b00 007d 946a  ..j....uj....}.j
+0000bbf0: d50b 0000 7d94 6ad7 0b00 005d 946a d90b  ....}.j....].j..
+0000bc00: 0000 5d94 6adb 0b00 005d 946a dd0b 0000  ..].j....].j....
+0000bc10: 5d94 6adf 0b00 005d 946a e10b 0000 5d94  ].j....].j....].
+0000bc20: 6ae3 0b00 004b 016a e40b 0000 4b00 6ae5  j....K.j....K.j.
+0000bc30: 0b00 006a e70b 0000 7d94 8594 5294 6aeb  ...j....}...R.j.
+0000bc40: 0b00 005d 946a ed0b 0000 5d94 6aef 0b00  ...].j....].j...
+0000bc50: 004e 6af0 0b00 005d 946a f20b 0000 4e6a  .Nj....].j....Nj
+0000bc60: 0003 0000 6af4 0b00 0075 628c 076d 6f64  ....j....ub..mod
+0000bc70: 756c 6573 946a e802 0000 2981 947d 9428  ules.j....)..}.(
+0000bc80: 6aeb 0200 0068 406a ec02 0000 5d94 6aef  j....h@j....].j.
+0000bc90: 0200 0029 8194 7d94 286a eb02 0000 6840  ...)..}.(j....h@
+0000bca0: 6aec 0200 005d 9428 6af4 0200 0029 8194  j....].(j....)..
+0000bcb0: 7d94 286a eb02 0000 8c11 636f 6f6b 6965  }.(j......cookie
+0000bcc0: 735f 7574 696c 6974 6965 7394 6aec 0200  s_utilities.j...
+0000bcd0: 005d 946a fa02 0000 8c11 636f 6f6b 6965  .].j......cookie
+0000bce0: 735f 7574 696c 6974 6965 7394 8594 8194  s_utilities.....
+0000bcf0: 7d94 286a ff02 0000 6a6e 0d00 006a 0003  }.(j....jn...j..
+0000bd00: 0000 6a68 0d00 006a 0103 0000 4e6a 0203  ..jh...j....Nj..
+0000bd10: 0000 4e75 6261 6a03 0300 007d 9428 6a03  ..Nubaj....}.(j.
+0000bd20: 0c00 005d 946a 050c 0000 5d94 6a07 0c00  ...].j....].j...
+0000bd30: 005d 946a 090c 0000 5d94 6a0b 0c00 005d  .].j....].j....]
+0000bd40: 9475 6a0f 0300 006a 0d0c 0000 6aff 0200  .uj....j....j...
+0000bd50: 006a 6b0d 0000 6a00 0300 006a 680d 0000  .jk...j....jh...
+0000bd60: 6a01 0300 008c 3e43 3a5c 5573 6572 735c  j.....>C:\Users\
+0000bd70: 632d 6d69 685c 7370 6163 655c 636f 6f6b  c-mih\space\cook
+0000bd80: 6965 735f 7574 696c 6974 6965 735c 646f  ies_utilities\do
+0000bd90: 6373 5c73 6f75 7263 655c 6d6f 6475 6c65  cs\source\module
+0000bda0: 732e 7273 7494 6a02 0300 004b 0275 626a  s.rst.j....K.ubj
+0000bdb0: a90c 0000 2981 947d 9428 6aeb 0200 0068  ....)..}.(j....h
+0000bdc0: 406a ec02 0000 5d94 6aae 0c00 0029 8194  @j....].j....)..
+0000bdd0: 7d94 286a eb02 0000 6840 6aec 0200 005d  }.(j....h@j....]
+0000bde0: 946a 0303 0000 7d94 286a 030c 0000 5d94  .j....}.(j....].
+0000bdf0: 6a05 0c00 005d 946a 070c 0000 5d94 6a09  j....].j....].j.
+0000be00: 0c00 005d 946a 0b0c 0000 5d94 6ab8 0c00  ...].j....].j...
+0000be10: 006a cb02 0000 6ab9 0c00 005d 944e 8c11  .j....j....].N..
+0000be20: 636f 6f6b 6965 735f 7574 696c 6974 6965  cookies_utilitie
+0000be30: 7394 8694 616a bd0c 0000 5d94 6a8a 0d00  s...aj....].j...
+0000be40: 0061 6abf 0c00 004b 046a c00c 0000 4e6a  .aj....K.j....Nj
+0000be50: c20c 0000 896a c30c 0000 896a c40c 0000  .....j.....j....
+0000be60: 896a c50c 0000 4b00 6ac6 0c00 0089 6ac7  .j....K.j.....j.
+0000be70: 0c00 005d 9475 6a0f 0300 006a ca0c 0000  ...].uj....j....
+0000be80: 6a01 0300 006a 7c0d 0000 6a02 0300 004b  j....j|...j....K
+0000be90: 046a ff02 0000 6a7d 0d00 0075 6261 6a03  .j....j}...ubaj.
+0000bea0: 0300 007d 9428 6a03 0c00 005d 946a 050c  ...}.(j....].j..
+0000beb0: 0000 5d94 6ace 0c00 0061 6a07 0c00 005d  ..].j....aj....]
+0000bec0: 946a 090c 0000 5d94 6a0b 0c00 005d 9475  .j....].j....].u
+0000bed0: 6a0f 0300 006a d20c 0000 6aff 0200 006a  j....j....j....j
+0000bee0: 6b0d 0000 6a00 0300 006a 680d 0000 6a01  k...j....jh...j.
+0000bef0: 0300 006a 7c0d 0000 6a02 0300 004e 7562  ...j|...j....Nub
+0000bf00: 656a 0303 0000 7d94 286a 030c 0000 5d94  ej....}.(j....].
+0000bf10: 8c11 636f 6f6b 6965 732d 7574 696c 6974  ..cookies-utilit
+0000bf20: 6965 7394 616a 050c 0000 5d94 6a07 0c00  ies.aj....].j...
+0000bf30: 005d 948c 1163 6f6f 6b69 6573 5f75 7469  .]...cookies_uti
+0000bf40: 6c69 7469 6573 9461 6a09 0c00 005d 946a  lities.aj....].j
+0000bf50: 0b0c 0000 5d94 756a 0f03 0000 6adb 0c00  ....].uj....j...
+0000bf60: 006a ff02 0000 6a68 0d00 006a 0003 0000  .j....jh...j....
+0000bf70: 6a68 0d00 006a 0103 0000 6a7c 0d00 006a  jh...j....j|...j
+0000bf80: 0203 0000 4b02 7562 616a 0303 0000 7d94  ....K.ubaj....}.
+0000bf90: 286a 030c 0000 5d94 6a05 0c00 005d 946a  (j....].j....].j
+0000bfa0: 070c 0000 5d94 6a09 0c00 005d 946a 0b0c  ....].j....].j..
+0000bfb0: 0000 5d94 8c06 736f 7572 6365 946a 7c0d  ..]...source.j|.
+0000bfc0: 0000 756a 0f03 0000 6a44 0d00 006a 7a0b  ..uj....jD...jz.
+0000bfd0: 0000 4e6a 7b0b 0000 4e6a 7c0b 0000 6a7f  ..Nj{...Nj|...j.
+0000bfe0: 0b00 0029 8194 7d94 286a f302 0000 4e6a  ...)..}.(j....Nj
+0000bff0: 820b 0000 4e6a 830b 0000 4e6a 840b 0000  ....Nj....Nj....
+0000c000: 4e6a 850b 0000 4e6a 860b 0000 6a47 0d00  Nj....Nj....jG..
+0000c010: 006a 880b 0000 4b01 6a89 0b00 004b 016a  .j....K.j....K.j
+0000c020: 8a0b 0000 4e6a 8b0b 0000 4e6a 8c0b 0000  ....Nj....Nj....
+0000c030: 4e6a 8d0b 0000 4b02 6a8e 0b00 004b 056a  Nj....K.j....K.j
+0000c040: 8f0b 0000 4b05 6a90 0b00 004e 6a91 0b00  ....K.j....Nj...
+0000c050: 004e 6a92 0b00 0088 6a93 0b00 006a 480d  .Nj.....j....jH.
+0000c060: 0000 6a94 0b00 006a 490d 0000 6a96 0b00  ..j....jI...j...
+0000c070: 006a 4a0d 0000 6a98 0b00 006a 490d 0000  .jJ...j....jI...
+0000c080: 6a99 0b00 006a 4b0d 0000 6a9b 0b00 006a  j....jK...j....j
+0000c090: 4c0d 0000 6a9d 0b00 006a 4d0d 0000 6a9e  L...j....jM...j.
+0000c0a0: 0b00 004e 6a9f 0b00 004e 6aa0 0b00 0068  ...Nj....Nj....h
+0000c0b0: 406a a10b 0000 6ab1 0200 006a a20b 0000  @j....j....j....
+0000c0c0: 4e6a a30b 0000 4e6a a40b 0000 4e6a a50b  Nj....Nj....Nj..
+0000c0d0: 0000 4e6a a60b 0000 4e6a a70b 0000 4e6a  ..Nj....Nj....Nj
+0000c0e0: a80b 0000 4e6a a90b 0000 6a7c 0d00 006a  ....Nj....j|...j
+0000c0f0: aa0b 0000 4e6a ab0b 0000 6a4e 0d00 006a  ....Nj....jN...j
+0000c100: ad0b 0000 886a ae0b 0000 4b01 6aaf 0b00  .....j....K.j...
+0000c110: 004d 1027 6ab0 0b00 004e 6ab1 0b00 006a  .M.'j....Nj....j
+0000c120: b702 0000 6ab2 0b00 006a 4f0d 0000 6ab4  ....j....jO...j.
+0000c130: 0b00 004e 6ab5 0b00 006a ba02 0000 6ab6  ...Nj....j....j.
+0000c140: 0b00 004b 0868 7589 6ab7 0b00 006a 500d  ...K.hu.j....jP.
+0000c150: 0000 6ab9 0b00 0088 6aba 0b00 006a c302  ..j.....j....j..
+0000c160: 0000 6abb 0b00 0089 6abc 0b00 0089 6abd  ..j.....j.....j.
+0000c170: 0b00 004b 016a be0b 0000 896a bf0b 0000  ...K.j.....j....
+0000c180: 6ab3 0200 006a c00b 0000 896a c10b 0000  j....j.....j....
+0000c190: 886a c20b 0000 8968 3c4e 7562 6ac3 0b00  .j.....h<Nubj...
+0000c1a0: 004e 6ac4 0b00 005d 946a c60b 0000 7d94  .Nj....].j....}.
+0000c1b0: 6ac8 0b00 007d 946a ca0b 0000 7d94 6acc  j....}.j....}.j.
+0000c1c0: 0b00 007d 946a ce0b 0000 7d94 6a99 0d00  ...}.j....}.j...
+0000c1d0: 006a 960d 0000 736a d00b 0000 7d94 6a99  .j....sj....}.j.
+0000c1e0: 0d00 0089 736a 0503 0000 7d94 6a96 0d00  ....sj....}.j...
+0000c1f0: 006a 6b0d 0000 736a d30b 0000 7d94 6ad5  .jk...sj....}.j.
+0000c200: 0b00 007d 946a d70b 0000 5d94 6ad9 0b00  ...}.j....].j...
+0000c210: 005d 946a db0b 0000 5d94 6add 0b00 005d  .].j....].j....]
+0000c220: 946a df0b 0000 5d94 6ae1 0b00 005d 946a  .j....].j....].j
+0000c230: e30b 0000 4b01 6ae4 0b00 004b 006a e50b  ....K.j....K.j..
+0000c240: 0000 6ae7 0b00 007d 9485 9452 946a eb0b  ..j....}...R.j..
+0000c250: 0000 5d94 6aed 0b00 005d 946a ef0b 0000  ..].j....].j....
+0000c260: 4e6a f00b 0000 5d94 6af2 0b00 004e 6a00  Nj....].j....Nj.
+0000c270: 0300 006a 680d 0000 7562 758c 086d 6574  ...jh...ubu..met
+0000c280: 6164 6174 6194 6acf 0200 006a d002 0000  adata.j....j....
+0000c290: 8c04 6469 6374 9493 9485 9452 948c 0674  ..dict.....R...t
+0000c2a0: 6974 6c65 7394 7d94 286a ca02 0000 6af4  itles.}.(j....j.
+0000c2b0: 0200 0029 8194 7d94 286a eb02 0000 6840  ...)..}.(j....h@
+0000c2c0: 6aec 0200 005d 946a fa02 0000 8c2e 5765  j....].j......We
+0000c2d0: 6c63 6f6d 6520 746f 2063 6f6f 6b69 6573  lcome to cookies
+0000c2e0: 5f75 7469 6c69 7469 6573 e280 9920 646f  _utilities... do
+0000c2f0: 6375 6d65 6e74 6174 696f 6e21 9485 9481  cumentation!....
+0000c300: 947d 946a ff02 0000 6ac2 0d00 0073 6261  .}.j....j....sba
+0000c310: 6a03 0300 007d 9428 6a03 0c00 005d 946a  j....}.(j....].j
+0000c320: 050c 0000 5d94 6a07 0c00 005d 946a 090c  ....].j....].j..
+0000c330: 0000 5d94 6a0b 0c00 005d 9475 6a0f 0300  ..].j....].uj...
+0000c340: 006a 0d0c 0000 7562 6acb 0200 006a f402  .j....ubj....j..
+0000c350: 0000 2981 947d 9428 6aeb 0200 0068 406a  ..)..}.(j....h@j
+0000c360: ec02 0000 5d94 6afa 0200 008c 1163 6f6f  ....].j......coo
+0000c370: 6b69 6573 5f75 7469 6c69 7469 6573 9485  kies_utilities..
+0000c380: 9481 947d 946a ff02 0000 6acf 0d00 0073  ...}.j....j....s
+0000c390: 6261 6a03 0300 007d 9428 6a03 0c00 005d  baj....}.(j....]
+0000c3a0: 946a 050c 0000 5d94 6a07 0c00 005d 946a  .j....].j....].j
+0000c3b0: 090c 0000 5d94 6a0b 0c00 005d 9475 6a0f  ....].j....].uj.
+0000c3c0: 0300 006a 0d0c 0000 7562 6a9b 0200 006a  ...j....ubj....j
+0000c3d0: f402 0000 2981 947d 9428 6aeb 0200 0068  ....)..}.(j....h
+0000c3e0: 406a ec02 0000 5d94 6afa 0200 008c 0d44  @j....].j......D
+0000c3f0: 6f63 756d 656e 7461 7469 6f6e 9485 9481  ocumentation....
+0000c400: 947d 946a ff02 0000 6adc 0d00 0073 6261  .}.j....j....sba
+0000c410: 6a03 0300 007d 9428 6a05 0300 005d 946a  j....}.(j....].j
+0000c420: 0703 0000 5d94 6a09 0300 005d 946a 0b03  ....].j....].j..
+0000c430: 0000 5d94 6a0d 0300 005d 9475 6a0f 0300  ..].j....].uj...
+0000c440: 006a f302 0000 7562 758c 0a6c 6f6e 6774  .j....ubu..longt
+0000c450: 6974 6c65 7394 7d94 286a ca02 0000 6ac2  itles.}.(j....j.
+0000c460: 0d00 006a cb02 0000 6acf 0d00 006a 9b02  ...j....j....j..
+0000c470: 0000 6adc 0d00 0075 8c04 746f 6373 947d  ..j....u..tocs.}
+0000c480: 9428 6aca 0200 006a 6505 0000 2981 947d  .(j....je...)..}
+0000c490: 9428 6aeb 0200 0068 406a ec02 0000 5d94  .(j....h@j....].
+0000c4a0: 6a6a 0500 0029 8194 7d94 286a eb02 0000  jj...)..}.(j....
+0000c4b0: 6840 6aec 0200 005d 9428 6ae6 0200 008c  h@j....].(j.....
+0000c4c0: 1163 6f6d 7061 6374 5f70 6172 6167 7261  .compact_paragra
+0000c4d0: 7068 9493 9429 8194 7d94 286a eb02 0000  ph...)..}.(j....
+0000c4e0: 6840 6aec 0200 005d 946a 3c0c 0000 2981  h@j....].j<...).
+0000c4f0: 947d 9428 6aeb 0200 0068 406a ec02 0000  .}.(j....h@j....
+0000c500: 5d94 6afa 0200 008c 2e57 656c 636f 6d65  ].j......Welcome
+0000c510: 2074 6f20 636f 6f6b 6965 735f 7574 696c   to cookies_util
+0000c520: 6974 6965 73e2 8099 2064 6f63 756d 656e  ities... documen
+0000c530: 7461 7469 6f6e 2194 8594 8194 7d94 6aff  tation!.....}.j.
+0000c540: 0200 006a f80d 0000 7362 616a 0303 0000  ...j....sbaj....
+0000c550: 7d94 286a 030c 0000 5d94 6a05 0c00 005d  }.(j....].j....]
+0000c560: 946a 070c 0000 5d94 6a09 0c00 005d 946a  .j....].j....].j
+0000c570: 0b0c 0000 5d94 8c08 696e 7465 726e 616c  ....]...internal
+0000c580: 9488 8c06 7265 6675 7269 946a ca02 0000  ....refuri.j....
+0000c590: 8c0a 616e 6368 6f72 6e61 6d65 9468 4075  ..anchorname.h@u
+0000c5a0: 6a0f 0300 006a 4e0c 0000 6aff 0200 006a  j....jN...j....j
+0000c5b0: f50d 0000 7562 616a 0303 0000 7d94 286a  ....ubaj....}.(j
+0000c5c0: 030c 0000 5d94 6a05 0c00 005d 946a 070c  ....].j....].j..
+0000c5d0: 0000 5d94 6a09 0c00 005d 946a 0b0c 0000  ..].j....].j....
+0000c5e0: 5d94 756a 0f03 0000 8c11 636f 6d70 6163  ].uj......compac
+0000c5f0: 745f 7061 7261 6772 6170 6894 6aff 0200  t_paragraph.j...
+0000c600: 006a f00d 0000 7562 6a65 0500 0029 8194  .j....ubje...)..
+0000c610: 7d94 286a eb02 0000 6840 6aec 0200 005d  }.(j....h@j....]
+0000c620: 9428 6a6a 0500 0029 8194 7d94 286a eb02  .(jj...)..}.(j..
+0000c630: 0000 6840 6aec 0200 005d 9428 6af4 0d00  ..h@j....].(j...
+0000c640: 0029 8194 7d94 286a eb02 0000 6840 6aec  .)..}.(j....h@j.
+0000c650: 0200 005d 946a 3c0c 0000 2981 947d 9428  ...].j<...)..}.(
+0000c660: 6aeb 0200 0068 406a ec02 0000 5d94 6afa  j....h@j....].j.
+0000c670: 0200 008c 054c 696e 6b73 9485 9481 947d  .....Links.....}
+0000c680: 946a ff02 0000 6a18 0e00 0073 6261 6a03  .j....j....sbaj.
+0000c690: 0300 007d 9428 6a03 0c00 005d 946a 050c  ...}.(j....].j..
+0000c6a0: 0000 5d94 6a07 0c00 005d 946a 090c 0000  ..].j....].j....
+0000c6b0: 5d94 6a0b 0c00 005d 948c 0869 6e74 6572  ].j....]...inter
+0000c6c0: 6e61 6c94 888c 0672 6566 7572 6994 6aca  nal....refuri.j.
+0000c6d0: 0200 008c 0a61 6e63 686f 726e 616d 6594  .....anchorname.
+0000c6e0: 8c06 236c 696e 6b73 9475 6a0f 0300 006a  ..#links.uj....j
+0000c6f0: 4e0c 0000 6aff 0200 006a 150e 0000 7562  N...j....j....ub
+0000c700: 616a 0303 0000 7d94 286a 030c 0000 5d94  aj....}.(j....].
+0000c710: 6a05 0c00 005d 946a 070c 0000 5d94 6a09  j....].j....].j.
+0000c720: 0c00 005d 946a 0b0c 0000 5d94 756a 0f03  ...].j....].uj..
+0000c730: 0000 6a0e 0e00 006a ff02 0000 6a12 0e00  ..j....j....j...
+0000c740: 0075 626a 6505 0000 2981 947d 9428 6aeb  .ubje...)..}.(j.
+0000c750: 0200 0068 406a ec02 0000 5d94 6aae 0c00  ...h@j....].j...
+0000c760: 0029 8194 7d94 286a eb02 0000 6840 6aec  .)..}.(j....h@j.
+0000c770: 0200 005d 946a 0303 0000 7d94 286a 030c  ...].j....}.(j..
+0000c780: 0000 5d94 6a05 0c00 005d 946a 070c 0000  ..].j....].j....
+0000c790: 5d94 6a09 0c00 005d 946a 0b0c 0000 5d94  ].j....].j....].
+0000c7a0: 8c06 7061 7265 6e74 946a ca02 0000 8c07  ..parent.j......
+0000c7b0: 656e 7472 6965 7394 6aba 0c00 008c 0c69  entries.j......i
+0000c7c0: 6e63 6c75 6465 6669 6c65 7394 6abe 0c00  ncludefiles.j...
+0000c7d0: 008c 086d 6178 6465 7074 6894 4b02 8c07  ...maxdepth.K...
+0000c7e0: 6361 7074 696f 6e94 6ac1 0c00 008c 0467  caption.j......g
+0000c7f0: 6c6f 6294 898c 0668 6964 6465 6e94 898c  lob....hidden...
+0000c800: 0d69 6e63 6c75 6465 6869 6464 656e 9489  .includehidden..
+0000c810: 8c08 6e75 6d62 6572 6564 944b 008c 0a74  ..numbered.K...t
+0000c820: 6974 6c65 736f 6e6c 7994 898c 0a72 6177  itlesonly....raw
+0000c830: 656e 7472 6965 7394 6ac8 0c00 008c 0a72  entries.j......r
+0000c840: 6177 6361 7074 696f 6e94 6ac1 0c00 0075  awcaption.j....u
+0000c850: 6a0f 0300 006a ca0c 0000 6a01 0300 006a  j....j....j....j
+0000c860: 0e0c 0000 6a02 0300 004b 0c6a ff02 0000  ....j....K.j....
+0000c870: 6a2f 0e00 0075 6261 6a03 0300 007d 9428  j/...ubaj....}.(
+0000c880: 6a03 0c00 005d 946a 050c 0000 5d94 6a07  j....].j....].j.
+0000c890: 0c00 005d 946a 090c 0000 5d94 6a0b 0c00  ...].j....].j...
+0000c8a0: 005d 9475 6a0f 0300 006a a70c 0000 6aff  .].uj....j....j.
+0000c8b0: 0200 006a 120e 0000 7562 656a 0303 0000  ...j....ubej....
+0000c8c0: 7d94 286a 030c 0000 5d94 6a05 0c00 005d  }.(j....].j....]
+0000c8d0: 946a 070c 0000 5d94 6a09 0c00 005d 946a  .j....].j....].j
+0000c8e0: 0b0c 0000 5d94 756a 0f03 0000 6a6d 0c00  ....].uj....jm..
+0000c8f0: 006a ff02 0000 6a0f 0e00 0075 626a 6a05  .j....j....ubjj.
+0000c900: 0000 2981 947d 9428 6aeb 0200 0068 406a  ..)..}.(j....h@j
+0000c910: ec02 0000 5d94 6af4 0d00 0029 8194 7d94  ....].j....)..}.
+0000c920: 286a eb02 0000 6840 6aec 0200 005d 946a  (j....h@j....].j
+0000c930: 3c0c 0000 2981 947d 9428 6aeb 0200 0068  <...)..}.(j....h
+0000c940: 406a ec02 0000 5d94 6afa 0200 008c 1249  @j....].j......I
+0000c950: 6e64 6963 6573 2061 6e64 2074 6162 6c65  ndices and table
+0000c960: 7394 8594 8194 7d94 6aff 0200 006a 590e  s.....}.j....jY.
+0000c970: 0000 7362 616a 0303 0000 7d94 286a 030c  ..sbaj....}.(j..
+0000c980: 0000 5d94 6a05 0c00 005d 946a 070c 0000  ..].j....].j....
+0000c990: 5d94 6a09 0c00 005d 946a 0b0c 0000 5d94  ].j....].j....].
+0000c9a0: 8c08 696e 7465 726e 616c 9488 8c06 7265  ..internal....re
+0000c9b0: 6675 7269 946a ca02 0000 8c0a 616e 6368  furi.j......anch
+0000c9c0: 6f72 6e61 6d65 948c 1323 696e 6469 6365  orname...#indice
+0000c9d0: 732d 616e 642d 7461 626c 6573 9475 6a0f  s-and-tables.uj.
+0000c9e0: 0300 006a 4e0c 0000 6aff 0200 006a 560e  ...jN...j....jV.
+0000c9f0: 0000 7562 616a 0303 0000 7d94 286a 030c  ..ubaj....}.(j..
+0000ca00: 0000 5d94 6a05 0c00 005d 946a 070c 0000  ..].j....].j....
+0000ca10: 5d94 6a09 0c00 005d 946a 0b0c 0000 5d94  ].j....].j....].
+0000ca20: 756a 0f03 0000 6a0e 0e00 006a ff02 0000  uj....j....j....
+0000ca30: 6a53 0e00 0075 6261 6a03 0300 007d 9428  jS...ubaj....}.(
+0000ca40: 6a03 0c00 005d 946a 050c 0000 5d94 6a07  j....].j....].j.
+0000ca50: 0c00 005d 946a 090c 0000 5d94 6a0b 0c00  ...].j....].j...
+0000ca60: 005d 9475 6a0f 0300 006a 6d0c 0000 6aff  .].uj....jm...j.
+0000ca70: 0200 006a 0f0e 0000 7562 656a 0303 0000  ...j....ubej....
+0000ca80: 7d94 286a 030c 0000 5d94 6a05 0c00 005d  }.(j....].j....]
+0000ca90: 946a 070c 0000 5d94 6a09 0c00 005d 946a  .j....].j....].j
+0000caa0: 0b0c 0000 5d94 756a 0f03 0000 6aa7 0c00  ....].uj....j...
+0000cab0: 006a ff02 0000 6af0 0d00 0075 6265 6a03  .j....j....ubej.
+0000cac0: 0300 007d 9428 6a03 0c00 005d 946a 050c  ...}.(j....].j..
+0000cad0: 0000 5d94 6a07 0c00 005d 946a 090c 0000  ..].j....].j....
+0000cae0: 5d94 6a0b 0c00 005d 9475 6a0f 0300 006a  ].j....].uj....j
+0000caf0: 6d0c 0000 6aff 0200 006a ed0d 0000 7562  m...j....j....ub
+0000cb00: 616a 0303 0000 7d94 286a 030c 0000 5d94  aj....}.(j....].
+0000cb10: 6a05 0c00 005d 946a 070c 0000 5d94 6a09  j....].j....].j.
+0000cb20: 0c00 005d 946a 0b0c 0000 5d94 756a 0f03  ...].j....].uj..
+0000cb30: 0000 6aa7 0c00 0075 626a cb02 0000 6a65  ..j....ubj....je
+0000cb40: 0500 0029 8194 7d94 286a eb02 0000 6840  ...)..}.(j....h@
+0000cb50: 6aec 0200 005d 946a 6a05 0000 2981 947d  j....].jj...)..}
+0000cb60: 9428 6aeb 0200 0068 406a ec02 0000 5d94  .(j....h@j....].
+0000cb70: 286a f40d 0000 2981 947d 9428 6aeb 0200  (j....)..}.(j...
+0000cb80: 0068 406a ec02 0000 5d94 6a3c 0c00 0029  .h@j....].j<...)
+0000cb90: 8194 7d94 286a eb02 0000 6840 6aec 0200  ..}.(j....h@j...
+0000cba0: 005d 946a fa02 0000 8c11 636f 6f6b 6965  .].j......cookie
+0000cbb0: 735f 7574 696c 6974 6965 7394 8594 8194  s_utilities.....
+0000cbc0: 7d94 6aff 0200 006a 910e 0000 7362 616a  }.j....j....sbaj
+0000cbd0: 0303 0000 7d94 286a 030c 0000 5d94 6a05  ....}.(j....].j.
+0000cbe0: 0c00 005d 946a 070c 0000 5d94 6a09 0c00  ...].j....].j...
+0000cbf0: 005d 946a 0b0c 0000 5d94 8c08 696e 7465  .].j....]...inte
+0000cc00: 726e 616c 9488 8c06 7265 6675 7269 946a  rnal....refuri.j
+0000cc10: cb02 0000 8c0a 616e 6368 6f72 6e61 6d65  ......anchorname
+0000cc20: 9468 4075 6a0f 0300 006a 4e0c 0000 6aff  .h@uj....jN...j.
+0000cc30: 0200 006a 8e0e 0000 7562 616a 0303 0000  ...j....ubaj....
+0000cc40: 7d94 286a 030c 0000 5d94 6a05 0c00 005d  }.(j....].j....]
+0000cc50: 946a 070c 0000 5d94 6a09 0c00 005d 946a  .j....].j....].j
+0000cc60: 0b0c 0000 5d94 756a 0f03 0000 6a0e 0e00  ....].uj....j...
+0000cc70: 006a ff02 0000 6a8b 0e00 0075 626a 6505  .j....j....ubje.
+0000cc80: 0000 2981 947d 9428 6aeb 0200 0068 406a  ..)..}.(j....h@j
+0000cc90: ec02 0000 5d94 6aae 0c00 0029 8194 7d94  ....].j....)..}.
+0000cca0: 286a eb02 0000 6840 6aec 0200 005d 946a  (j....h@j....].j
+0000ccb0: 0303 0000 7d94 286a 030c 0000 5d94 6a05  ....}.(j....].j.
+0000ccc0: 0c00 005d 946a 070c 0000 5d94 6a09 0c00  ...].j....].j...
+0000ccd0: 005d 946a 0b0c 0000 5d94 8c06 7061 7265  .].j....]...pare
+0000cce0: 6e74 946a cb02 0000 8c07 656e 7472 6965  nt.j......entrie
+0000ccf0: 7394 6a89 0d00 008c 0c69 6e63 6c75 6465  s.j......include
+0000cd00: 6669 6c65 7394 6a8c 0d00 008c 086d 6178  files.j......max
+0000cd10: 6465 7074 6894 4b04 8c07 6361 7074 696f  depth.K...captio
+0000cd20: 6e94 4e8c 0467 6c6f 6294 898c 0668 6964  n.N..glob....hid
+0000cd30: 6465 6e94 898c 0d69 6e63 6c75 6465 6869  den....includehi
+0000cd40: 6464 656e 9489 8c08 6e75 6d62 6572 6564  dden....numbered
+0000cd50: 944b 008c 0a74 6974 6c65 736f 6e6c 7994  .K...titlesonly.
+0000cd60: 898c 0a72 6177 656e 7472 6965 7394 6a8d  ...rawentries.j.
+0000cd70: 0d00 0075 6a0f 0300 006a ca0c 0000 6a01  ...uj....j....j.
+0000cd80: 0300 006a 7c0d 0000 6a02 0300 004b 046a  ...j|...j....K.j
+0000cd90: ff02 0000 6aa7 0e00 0075 6261 6a03 0300  ....j....ubaj...
+0000cda0: 007d 9428 6a03 0c00 005d 946a 050c 0000  .}.(j....].j....
+0000cdb0: 5d94 6a07 0c00 005d 946a 090c 0000 5d94  ].j....].j....].
+0000cdc0: 6a0b 0c00 005d 9475 6a0f 0300 006a a70c  j....].uj....j..
+0000cdd0: 0000 6aff 0200 006a 8b0e 0000 7562 656a  ..j....j....ubej
+0000cde0: 0303 0000 7d94 286a 030c 0000 5d94 6a05  ....}.(j....].j.
+0000cdf0: 0c00 005d 946a 070c 0000 5d94 6a09 0c00  ...].j....].j...
+0000ce00: 005d 946a 0b0c 0000 5d94 756a 0f03 0000  .].j....].uj....
+0000ce10: 6a6d 0c00 006a ff02 0000 6a88 0e00 0075  jm...j....j....u
+0000ce20: 6261 6a03 0300 007d 9428 6a03 0c00 005d  baj....}.(j....]
+0000ce30: 946a 050c 0000 5d94 6a07 0c00 005d 946a  .j....].j....].j
+0000ce40: 090c 0000 5d94 6a0b 0c00 005d 9475 6a0f  ....].j....].uj.
+0000ce50: 0300 006a a70c 0000 7562 6a9b 0200 006a  ...j....ubj....j
+0000ce60: 6505 0000 2981 947d 9428 6aeb 0200 0068  e...)..}.(j....h
+0000ce70: 406a ec02 0000 5d94 6a6a 0500 0029 8194  @j....].jj...)..
+0000ce80: 7d94 286a eb02 0000 6840 6aec 0200 005d  }.(j....h@j....]
+0000ce90: 9428 6af4 0d00 0029 8194 7d94 286a eb02  .(j....)..}.(j..
+0000cea0: 0000 6840 6aec 0200 005d 946a 3c0c 0000  ..h@j....].j<...
+0000ceb0: 2981 947d 9428 6aeb 0200 0068 406a ec02  )..}.(j....h@j..
+0000cec0: 0000 5d94 6afa 0200 008c 0d44 6f63 756d  ..].j......Docum
+0000ced0: 656e 7461 7469 6f6e 9485 9481 947d 946a  entation.....}.j
+0000cee0: ff02 0000 6ad9 0e00 0073 6261 6a03 0300  ....j....sbaj...
+0000cef0: 007d 9428 6a05 0300 005d 946a 0703 0000  .}.(j....].j....
+0000cf00: 5d94 6a09 0300 005d 946a 0b03 0000 5d94  ].j....].j....].
+0000cf10: 6a0d 0300 005d 948c 0869 6e74 6572 6e61  j....]...interna
+0000cf20: 6c94 888c 0672 6566 7572 6994 6a9b 0200  l....refuri.j...
+0000cf30: 008c 0a61 6e63 686f 726e 616d 6594 6840  ...anchorname.h@
+0000cf40: 756a 0f03 0000 6a3b 0c00 006a ff02 0000  uj....j;...j....
+0000cf50: 6ad6 0e00 0075 6261 6a03 0300 007d 9428  j....ubaj....}.(
+0000cf60: 6a05 0300 005d 946a 0703 0000 5d94 6a09  j....].j....].j.
+0000cf70: 0300 005d 946a 0b03 0000 5d94 6a0d 0300  ...].j....].j...
+0000cf80: 005d 9475 6a0f 0300 006a f30d 0000 6aff  .].uj....j....j.
+0000cf90: 0200 006a d30e 0000 7562 6a65 0500 0029  ...j....ubje...)
+0000cfa0: 8194 7d94 286a eb02 0000 6840 6aec 0200  ..}.(j....h@j...
+0000cfb0: 005d 9428 6a6a 0500 0029 8194 7d94 286a  .].(jj...)..}.(j
+0000cfc0: eb02 0000 6840 6aec 0200 005d 9428 6af4  ....h@j....].(j.
+0000cfd0: 0d00 0029 8194 7d94 286a eb02 0000 6840  ...)..}.(j....h@
+0000cfe0: 6aec 0200 005d 946a 3c0c 0000 2981 947d  j....].j<...)..}
+0000cff0: 9428 6aeb 0200 0068 406a ec02 0000 5d94  .(j....h@j....].
+0000d000: 6afa 0200 008c 0946 756e 6374 696f 6e73  j......Functions
+0000d010: 9485 9481 947d 946a ff02 0000 6af8 0e00  .....}.j....j...
+0000d020: 0073 6261 6a03 0300 007d 9428 6a05 0300  .sbaj....}.(j...
+0000d030: 005d 946a 0703 0000 5d94 6a09 0300 005d  .].j....].j....]
+0000d040: 946a 0b03 0000 5d94 6a0d 0300 005d 948c  .j....].j....]..
+0000d050: 0869 6e74 6572 6e61 6c94 888c 0672 6566  .internal....ref
+0000d060: 7572 6994 6a9b 0200 008c 0a61 6e63 686f  uri.j......ancho
+0000d070: 726e 616d 6594 8c0a 2366 756e 6374 696f  rname...#functio
+0000d080: 6e73 9475 6a0f 0300 006a 3b0c 0000 6aff  ns.uj....j;...j.
+0000d090: 0200 006a f50e 0000 7562 616a 0303 0000  ...j....ubaj....
+0000d0a0: 7d94 286a 0503 0000 5d94 6a07 0300 005d  }.(j....].j....]
+0000d0b0: 946a 0903 0000 5d94 6a0b 0300 005d 946a  .j....].j....].j
+0000d0c0: 0d03 0000 5d94 756a 0f03 0000 6af3 0d00  ....].uj....j...
+0000d0d0: 006a ff02 0000 6af2 0e00 0075 626a 6505  .j....j....ubje.
+0000d0e0: 0000 2981 947d 9428 6aeb 0200 0068 406a  ..)..}.(j....h@j
+0000d0f0: ec02 0000 5d94 6a6a 0500 0029 8194 7d94  ....].jj...)..}.
+0000d100: 286a eb02 0000 6840 6aec 0200 005d 9428  (j....h@j....].(
+0000d110: 6af4 0d00 0029 8194 7d94 286a eb02 0000  j....)..}.(j....
+0000d120: 6840 6aec 0200 005d 946a 3c0c 0000 2981  h@j....].j<...).
+0000d130: 947d 9428 6aeb 0200 0068 406a ec02 0000  .}.(j....h@j....
+0000d140: 5d94 6afa 0200 008c 1b63 6f6f 6b69 6573  ].j......cookies
+0000d150: 5f75 7469 6c69 7469 6573 2e67 6574 5f64  _utilities.get_d
+0000d160: 6174 6573 9485 9481 947d 946a ff02 0000  ates.....}.j....
+0000d170: 6a18 0f00 0073 6261 6a03 0300 007d 9428  j....sbaj....}.(
+0000d180: 6a05 0300 005d 946a 0703 0000 5d94 6a09  j....].j....].j.
+0000d190: 0300 005d 946a 0b03 0000 5d94 6a0d 0300  ...].j....].j...
+0000d1a0: 005d 948c 0869 6e74 6572 6e61 6c94 888c  .]...internal...
+0000d1b0: 0672 6566 7572 6994 6a9b 0200 008c 0a61  .refuri.j......a
+0000d1c0: 6e63 686f 726e 616d 6594 8c1c 2363 6f6f  nchorname...#coo
+0000d1d0: 6b69 6573 2d75 7469 6c69 7469 6573 2d67  kies-utilities-g
+0000d1e0: 6574 2d64 6174 6573 9475 6a0f 0300 006a  et-dates.uj....j
+0000d1f0: 3b0c 0000 6aff 0200 006a 150f 0000 7562  ;...j....j....ub
+0000d200: 616a 0303 0000 7d94 286a 0503 0000 5d94  aj....}.(j....].
+0000d210: 6a07 0300 005d 946a 0903 0000 5d94 6a0b  j....].j....].j.
+0000d220: 0300 005d 946a 0d03 0000 5d94 756a 0f03  ...].j....].uj..
+0000d230: 0000 6af3 0d00 006a ff02 0000 6a12 0f00  ..j....j....j...
+0000d240: 0075 626a 6505 0000 2981 947d 9428 6aeb  .ubje...)..}.(j.
+0000d250: 0200 0068 406a ec02 0000 5d94 6a6a 0500  ...h@j....].jj..
+0000d260: 0029 8194 7d94 286a eb02 0000 6840 6aec  .)..}.(j....h@j.
+0000d270: 0200 005d 946a f40d 0000 2981 947d 9428  ...].j....)..}.(
+0000d280: 6aeb 0200 0068 406a ec02 0000 5d94 6a3c  j....h@j....].j<
+0000d290: 0c00 0029 8194 7d94 286a eb02 0000 6840  ...)..}.(j....h@
+0000d2a0: 6aec 0200 005d 946a ee02 0000 8c07 6c69  j....].j......li
+0000d2b0: 7465 7261 6c94 9394 2981 947d 9428 6aeb  teral...)..}.(j.
+0000d2c0: 0200 0068 406a ec02 0000 5d94 6afa 0200  ...h@j....].j...
+0000d2d0: 008c 0b67 6574 5f64 6174 6573 2829 9485  ...get_dates()..
+0000d2e0: 9481 947d 946a ff02 0000 6a3d 0f00 0073  ...}.j....j=...s
+0000d2f0: 6261 6a03 0300 007d 9428 6a05 0300 005d  baj....}.(j....]
+0000d300: 946a 0703 0000 5d94 6a09 0300 005d 946a  .j....].j....].j
+0000d310: 0b03 0000 5d94 6a0d 0300 005d 9475 6a0f  ....].j....].uj.
+0000d320: 0300 006a 3b0f 0000 6aff 0200 006a 380f  ...j;...j....j8.
+0000d330: 0000 7562 616a 0303 0000 7d94 286a 0503  ..ubaj....}.(j..
+0000d340: 0000 5d94 6a07 0300 005d 946a 0903 0000  ..].j....].j....
+0000d350: 5d94 6a0b 0300 005d 946a 0d03 0000 5d94  ].j....].j....].
+0000d360: 8c08 696e 7465 726e 616c 9488 8c06 7265  ..internal....re
+0000d370: 6675 7269 946a 9b02 0000 8c0a 616e 6368  furi.j......anch
+0000d380: 6f72 6e61 6d65 948c 1c23 636f 6f6b 6965  orname...#cookie
+0000d390: 735f 7574 696c 6974 6965 732e 6765 745f  s_utilities.get_
+0000d3a0: 6461 7465 7394 756a 0f03 0000 6a3b 0c00  dates.uj....j;..
+0000d3b0: 006a ff02 0000 6a35 0f00 0075 6261 6a03  .j....j5...ubaj.
+0000d3c0: 0300 007d 9428 6a05 0300 005d 946a 0703  ...}.(j....].j..
+0000d3d0: 0000 5d94 6a09 0300 005d 946a 0b03 0000  ..].j....].j....
+0000d3e0: 5d94 6a0d 0300 005d 948c 1373 6b69 705f  ].j....]...skip_
+0000d3f0: 7365 6374 696f 6e5f 6e75 6d62 6572 9488  section_number..
+0000d400: 756a 0f03 0000 6af3 0d00 006a ff02 0000  uj....j....j....
+0000d410: 6a32 0f00 0075 6261 6a03 0300 007d 9428  j2...ubaj....}.(
+0000d420: 6a05 0300 005d 946a 0703 0000 5d94 6a09  j....].j....].j.
+0000d430: 0300 005d 946a 0b03 0000 5d94 6a0d 0300  ...].j....].j...
+0000d440: 005d 9475 6a0f 0300 006a 6905 0000 6aff  .].uj....ji...j.
+0000d450: 0200 006a 2f0f 0000 7562 616a 0303 0000  ...j/...ubaj....
+0000d460: 7d94 286a 0503 0000 5d94 6a07 0300 005d  }.(j....].j....]
+0000d470: 946a 0903 0000 5d94 6a0b 0300 005d 946a  .j....].j....].j
+0000d480: 0d03 0000 5d94 756a 0f03 0000 6a64 0500  ....].uj....jd..
+0000d490: 006a ff02 0000 6a12 0f00 0075 6265 6a03  .j....j....ubej.
+0000d4a0: 0300 007d 9428 6a05 0300 005d 946a 0703  ...}.(j....].j..
+0000d4b0: 0000 5d94 6a09 0300 005d 946a 0b03 0000  ..].j....].j....
+0000d4c0: 5d94 6a0d 0300 005d 9475 6a0f 0300 006a  ].j....].uj....j
+0000d4d0: 6905 0000 6aff 0200 006a 0f0f 0000 7562  i...j....j....ub
+0000d4e0: 616a 0303 0000 7d94 286a 0503 0000 5d94  aj....}.(j....].
+0000d4f0: 6a07 0300 005d 946a 0903 0000 5d94 6a0b  j....].j....].j.
+0000d500: 0300 005d 946a 0d03 0000 5d94 756a 0f03  ...].j....].uj..
+0000d510: 0000 6a64 0500 006a ff02 0000 6af2 0e00  ..jd...j....j...
+0000d520: 0075 6265 6a03 0300 007d 9428 6a05 0300  .ubej....}.(j...
+0000d530: 005d 946a 0703 0000 5d94 6a09 0300 005d  .].j....].j....]
+0000d540: 946a 0b03 0000 5d94 6a0d 0300 005d 9475  .j....].j....].u
+0000d550: 6a0f 0300 006a 6905 0000 6aff 0200 006a  j....ji...j....j
+0000d560: ef0e 0000 7562 6a6a 0500 0029 8194 7d94  ....ubjj...)..}.
+0000d570: 286a eb02 0000 6840 6aec 0200 005d 9428  (j....h@j....].(
+0000d580: 6af4 0d00 0029 8194 7d94 286a eb02 0000  j....)..}.(j....
+0000d590: 6840 6aec 0200 005d 946a 3c0c 0000 2981  h@j....].j<...).
+0000d5a0: 947d 9428 6aeb 0200 0068 406a ec02 0000  .}.(j....h@j....
+0000d5b0: 5d94 6afa 0200 008c 0743 6c61 7373 6573  ].j......Classes
+0000d5c0: 9485 9481 947d 946a ff02 0000 6a7f 0f00  .....}.j....j...
+0000d5d0: 0073 6261 6a03 0300 007d 9428 6a05 0300  .sbaj....}.(j...
+0000d5e0: 005d 946a 0703 0000 5d94 6a09 0300 005d  .].j....].j....]
+0000d5f0: 946a 0b03 0000 5d94 6a0d 0300 005d 948c  .j....].j....]..
+0000d600: 0869 6e74 6572 6e61 6c94 888c 0672 6566  .internal....ref
+0000d610: 7572 6994 6a9b 0200 008c 0a61 6e63 686f  uri.j......ancho
+0000d620: 726e 616d 6594 8c08 2363 6c61 7373 6573  rname...#classes
+0000d630: 9475 6a0f 0300 006a 3b0c 0000 6aff 0200  .uj....j;...j...
+0000d640: 006a 7c0f 0000 7562 616a 0303 0000 7d94  .j|...ubaj....}.
+0000d650: 286a 0503 0000 5d94 6a07 0300 005d 946a  (j....].j....].j
+0000d660: 0903 0000 5d94 6a0b 0300 005d 946a 0d03  ....].j....].j..
+0000d670: 0000 5d94 756a 0f03 0000 6af3 0d00 006a  ..].uj....j....j
+0000d680: ff02 0000 6a79 0f00 0075 626a 6505 0000  ....jy...ubje...
+0000d690: 2981 947d 9428 6aeb 0200 0068 406a ec02  )..}.(j....h@j..
+0000d6a0: 0000 5d94 6a6a 0500 0029 8194 7d94 286a  ..].jj...)..}.(j
+0000d6b0: eb02 0000 6840 6aec 0200 005d 9428 6af4  ....h@j....].(j.
+0000d6c0: 0d00 0029 8194 7d94 286a eb02 0000 6840  ...)..}.(j....h@
+0000d6d0: 6aec 0200 005d 946a 3c0c 0000 2981 947d  j....].j<...)..}
+0000d6e0: 9428 6aeb 0200 0068 406a ec02 0000 5d94  .(j....h@j....].
+0000d6f0: 6afa 0200 008c 1b63 6f6f 6b69 6573 5f75  j......cookies_u
+0000d700: 7469 6c69 7469 6573 2e53 746f 7077 6174  tilities.Stopwat
+0000d710: 6368 9485 9481 947d 946a ff02 0000 6a9f  ch.....}.j....j.
+0000d720: 0f00 0073 6261 6a03 0300 007d 9428 6a05  ...sbaj....}.(j.
+0000d730: 0300 005d 946a 0703 0000 5d94 6a09 0300  ...].j....].j...
+0000d740: 005d 946a 0b03 0000 5d94 6a0d 0300 005d  .].j....].j....]
+0000d750: 948c 0869 6e74 6572 6e61 6c94 888c 0672  ...internal....r
+0000d760: 6566 7572 6994 6a9b 0200 008c 0a61 6e63  efuri.j......anc
+0000d770: 686f 726e 616d 6594 8c1c 2363 6f6f 6b69  horname...#cooki
+0000d780: 6573 2d75 7469 6c69 7469 6573 2d73 746f  es-utilities-sto
+0000d790: 7077 6174 6368 9475 6a0f 0300 006a 3b0c  pwatch.uj....j;.
+0000d7a0: 0000 6aff 0200 006a 9c0f 0000 7562 616a  ..j....j....ubaj
+0000d7b0: 0303 0000 7d94 286a 0503 0000 5d94 6a07  ....}.(j....].j.
+0000d7c0: 0300 005d 946a 0903 0000 5d94 6a0b 0300  ...].j....].j...
+0000d7d0: 005d 946a 0d03 0000 5d94 756a 0f03 0000  .].j....].uj....
+0000d7e0: 6af3 0d00 006a ff02 0000 6a99 0f00 0075  j....j....j....u
+0000d7f0: 626a 6505 0000 2981 947d 9428 6aeb 0200  bje...)..}.(j...
+0000d800: 0068 406a ec02 0000 5d94 6a6a 0500 0029  .h@j....].jj...)
+0000d810: 8194 7d94 286a eb02 0000 6840 6aec 0200  ..}.(j....h@j...
+0000d820: 005d 9428 6af4 0d00 0029 8194 7d94 286a  .].(j....)..}.(j
+0000d830: eb02 0000 6840 6aec 0200 005d 946a 3c0c  ....h@j....].j<.
+0000d840: 0000 2981 947d 9428 6aeb 0200 0068 406a  ..)..}.(j....h@j
+0000d850: ec02 0000 5d94 6a3c 0f00 0029 8194 7d94  ....].j<...)..}.
+0000d860: 286a eb02 0000 6840 6aec 0200 005d 946a  (j....h@j....].j
+0000d870: fa02 0000 8c09 5374 6f70 7761 7463 6894  ......Stopwatch.
+0000d880: 8594 8194 7d94 6aff 0200 006a c20f 0000  ....}.j....j....
+0000d890: 7362 616a 0303 0000 7d94 286a 0503 0000  sbaj....}.(j....
+0000d8a0: 5d94 6a07 0300 005d 946a 0903 0000 5d94  ].j....].j....].
+0000d8b0: 6a0b 0300 005d 946a 0d03 0000 5d94 756a  j....].j....].uj
+0000d8c0: 0f03 0000 6a3b 0f00 006a ff02 0000 6abf  ....j;...j....j.
+0000d8d0: 0f00 0075 6261 6a03 0300 007d 9428 6a05  ...ubaj....}.(j.
+0000d8e0: 0300 005d 946a 0703 0000 5d94 6a09 0300  ...].j....].j...
+0000d8f0: 005d 946a 0b03 0000 5d94 6a0d 0300 005d  .].j....].j....]
+0000d900: 948c 0869 6e74 6572 6e61 6c94 888c 0672  ...internal....r
+0000d910: 6566 7572 6994 6a9b 0200 008c 0a61 6e63  efuri.j......anc
+0000d920: 686f 726e 616d 6594 8c1c 2363 6f6f 6b69  horname...#cooki
+0000d930: 6573 5f75 7469 6c69 7469 6573 2e53 746f  es_utilities.Sto
+0000d940: 7077 6174 6368 9475 6a0f 0300 006a 3b0c  pwatch.uj....j;.
+0000d950: 0000 6aff 0200 006a bc0f 0000 7562 616a  ..j....j....ubaj
+0000d960: 0303 0000 7d94 286a 0503 0000 5d94 6a07  ....}.(j....].j.
+0000d970: 0300 005d 946a 0903 0000 5d94 6a0b 0300  ...].j....].j...
+0000d980: 005d 946a 0d03 0000 5d94 8c13 736b 6970  .].j....]...skip
+0000d990: 5f73 6563 7469 6f6e 5f6e 756d 6265 7294  _section_number.
+0000d9a0: 8875 6a0f 0300 006a f30d 0000 6aff 0200  .uj....j....j...
+0000d9b0: 006a b90f 0000 7562 6a65 0500 0029 8194  .j....ubje...)..
+0000d9c0: 7d94 286a eb02 0000 6840 6aec 0200 005d  }.(j....h@j....]
+0000d9d0: 9428 6a6a 0500 0029 8194 7d94 286a eb02  .(jj...)..}.(j..
+0000d9e0: 0000 6840 6aec 0200 005d 946a f40d 0000  ..h@j....].j....
+0000d9f0: 2981 947d 9428 6aeb 0200 0068 406a ec02  )..}.(j....h@j..
+0000da00: 0000 5d94 6a3c 0c00 0029 8194 7d94 286a  ..].j<...)..}.(j
+0000da10: eb02 0000 6840 6aec 0200 005d 946a 3c0f  ....h@j....].j<.
+0000da20: 0000 2981 947d 9428 6aeb 0200 0068 406a  ..)..}.(j....h@j
+0000da30: ec02 0000 5d94 6afa 0200 008c 1153 746f  ....].j......Sto
+0000da40: 7077 6174 6368 2e70 7265 7373 2829 9485  pwatch.press()..
+0000da50: 9481 947d 946a ff02 0000 6aec 0f00 0073  ...}.j....j....s
+0000da60: 6261 6a03 0300 007d 9428 6a05 0300 005d  baj....}.(j....]
+0000da70: 946a 0703 0000 5d94 6a09 0300 005d 946a  .j....].j....].j
+0000da80: 0b03 0000 5d94 6a0d 0300 005d 9475 6a0f  ....].j....].uj.
+0000da90: 0300 006a 3b0f 0000 6aff 0200 006a e90f  ...j;...j....j..
+0000daa0: 0000 7562 616a 0303 0000 7d94 286a 0503  ..ubaj....}.(j..
+0000dab0: 0000 5d94 6a07 0300 005d 946a 0903 0000  ..].j....].j....
+0000dac0: 5d94 6a0b 0300 005d 946a 0d03 0000 5d94  ].j....].j....].
+0000dad0: 8c08 696e 7465 726e 616c 9488 8c06 7265  ..internal....re
+0000dae0: 6675 7269 946a 9b02 0000 8c0a 616e 6368  furi.j......anch
+0000daf0: 6f72 6e61 6d65 948c 2223 636f 6f6b 6965  orname.."#cookie
+0000db00: 735f 7574 696c 6974 6965 732e 5374 6f70  s_utilities.Stop
+0000db10: 7761 7463 682e 7072 6573 7394 756a 0f03  watch.press.uj..
+0000db20: 0000 6a3b 0c00 006a ff02 0000 6ae6 0f00  ..j;...j....j...
+0000db30: 0075 6261 6a03 0300 007d 9428 6a05 0300  .ubaj....}.(j...
+0000db40: 005d 946a 0703 0000 5d94 6a09 0300 005d  .].j....].j....]
+0000db50: 946a 0b03 0000 5d94 6a0d 0300 005d 948c  .j....].j....]..
+0000db60: 1373 6b69 705f 7365 6374 696f 6e5f 6e75  .skip_section_nu
+0000db70: 6d62 6572 9488 756a 0f03 0000 6af3 0d00  mber..uj....j...
+0000db80: 006a ff02 0000 6ae3 0f00 0075 6261 6a03  .j....j....ubaj.
+0000db90: 0300 007d 9428 6a05 0300 005d 946a 0703  ...}.(j....].j..
+0000dba0: 0000 5d94 6a09 0300 005d 946a 0b03 0000  ..].j....].j....
+0000dbb0: 5d94 6a0d 0300 005d 9475 6a0f 0300 006a  ].j....].uj....j
+0000dbc0: 6905 0000 6aff 0200 006a e00f 0000 7562  i...j....j....ub
+0000dbd0: 6a6a 0500 0029 8194 7d94 286a eb02 0000  jj...)..}.(j....
+0000dbe0: 6840 6aec 0200 005d 946a f40d 0000 2981  h@j....].j....).
+0000dbf0: 947d 9428 6aeb 0200 0068 406a ec02 0000  .}.(j....h@j....
+0000dc00: 5d94 6a3c 0c00 0029 8194 7d94 286a eb02  ].j<...)..}.(j..
+0000dc10: 0000 6840 6aec 0200 005d 946a 3c0f 0000  ..h@j....].j<...
+0000dc20: 2981 947d 9428 6aeb 0200 0068 406a ec02  )..}.(j....h@j..
+0000dc30: 0000 5d94 6afa 0200 008c 1053 746f 7077  ..].j......Stopw
+0000dc40: 6174 6368 2e73 686f 7728 2994 8594 8194  atch.show().....
+0000dc50: 7d94 6aff 0200 006a 1910 0000 7362 616a  }.j....j....sbaj
+0000dc60: 0303 0000 7d94 286a 0503 0000 5d94 6a07  ....}.(j....].j.
+0000dc70: 0300 005d 946a 0903 0000 5d94 6a0b 0300  ...].j....].j...
+0000dc80: 005d 946a 0d03 0000 5d94 756a 0f03 0000  .].j....].uj....
+0000dc90: 6a3b 0f00 006a ff02 0000 6a16 1000 0075  j;...j....j....u
+0000dca0: 6261 6a03 0300 007d 9428 6a05 0300 005d  baj....}.(j....]
+0000dcb0: 946a 0703 0000 5d94 6a09 0300 005d 946a  .j....].j....].j
+0000dcc0: 0b03 0000 5d94 6a0d 0300 005d 948c 0869  ....].j....]...i
+0000dcd0: 6e74 6572 6e61 6c94 888c 0672 6566 7572  nternal....refur
+0000dce0: 6994 6a9b 0200 008c 0a61 6e63 686f 726e  i.j......anchorn
+0000dcf0: 616d 6594 8c21 2363 6f6f 6b69 6573 5f75  ame..!#cookies_u
+0000dd00: 7469 6c69 7469 6573 2e53 746f 7077 6174  tilities.Stopwat
+0000dd10: 6368 2e73 686f 7794 756a 0f03 0000 6a3b  ch.show.uj....j;
+0000dd20: 0c00 006a ff02 0000 6a13 1000 0075 6261  ...j....j....uba
+0000dd30: 6a03 0300 007d 9428 6a05 0300 005d 946a  j....}.(j....].j
+0000dd40: 0703 0000 5d94 6a09 0300 005d 946a 0b03  ....].j....].j..
+0000dd50: 0000 5d94 6a0d 0300 005d 948c 1373 6b69  ..].j....]...ski
+0000dd60: 705f 7365 6374 696f 6e5f 6e75 6d62 6572  p_section_number
+0000dd70: 9488 756a 0f03 0000 6af3 0d00 006a ff02  ..uj....j....j..
+0000dd80: 0000 6a10 1000 0075 6261 6a03 0300 007d  ..j....ubaj....}
+0000dd90: 9428 6a05 0300 005d 946a 0703 0000 5d94  .(j....].j....].
+0000dda0: 6a09 0300 005d 946a 0b03 0000 5d94 6a0d  j....].j....].j.
+0000ddb0: 0300 005d 9475 6a0f 0300 006a 6905 0000  ...].uj....ji...
+0000ddc0: 6aff 0200 006a e00f 0000 7562 656a 0303  j....j....ubej..
+0000ddd0: 0000 7d94 286a 0503 0000 5d94 6a07 0300  ..}.(j....].j...
+0000dde0: 005d 946a 0903 0000 5d94 6a0b 0300 005d  .].j....].j....]
+0000ddf0: 946a 0d03 0000 5d94 756a 0f03 0000 6a64  .j....].uj....jd
+0000de00: 0500 006a ff02 0000 6ab9 0f00 0075 6265  ...j....j....ube
+0000de10: 6a03 0300 007d 9428 6a05 0300 005d 946a  j....}.(j....].j
+0000de20: 0703 0000 5d94 6a09 0300 005d 946a 0b03  ....].j....].j..
+0000de30: 0000 5d94 6a0d 0300 005d 9475 6a0f 0300  ..].j....].uj...
+0000de40: 006a 6905 0000 6aff 0200 006a b60f 0000  .ji...j....j....
+0000de50: 7562 616a 0303 0000 7d94 286a 0503 0000  ubaj....}.(j....
+0000de60: 5d94 6a07 0300 005d 946a 0903 0000 5d94  ].j....].j....].
+0000de70: 6a0b 0300 005d 946a 0d03 0000 5d94 756a  j....].j....].uj
+0000de80: 0f03 0000 6a64 0500 006a ff02 0000 6a99  ....jd...j....j.
+0000de90: 0f00 0075 6265 6a03 0300 007d 9428 6a05  ...ubej....}.(j.
+0000dea0: 0300 005d 946a 0703 0000 5d94 6a09 0300  ...].j....].j...
+0000deb0: 005d 946a 0b03 0000 5d94 6a0d 0300 005d  .].j....].j....]
+0000dec0: 9475 6a0f 0300 006a 6905 0000 6aff 0200  .uj....ji...j...
+0000ded0: 006a 960f 0000 7562 616a 0303 0000 7d94  .j....ubaj....}.
+0000dee0: 286a 0503 0000 5d94 6a07 0300 005d 946a  (j....].j....].j
+0000def0: 0903 0000 5d94 6a0b 0300 005d 946a 0d03  ....].j....].j..
+0000df00: 0000 5d94 756a 0f03 0000 6a64 0500 006a  ..].uj....jd...j
+0000df10: ff02 0000 6a79 0f00 0075 6265 6a03 0300  ....jy...ubej...
+0000df20: 007d 9428 6a05 0300 005d 946a 0703 0000  .}.(j....].j....
+0000df30: 5d94 6a09 0300 005d 946a 0b03 0000 5d94  ].j....].j....].
+0000df40: 6a0d 0300 005d 9475 6a0f 0300 006a 6905  j....].uj....ji.
+0000df50: 0000 6aff 0200 006a ef0e 0000 7562 656a  ..j....j....ubej
+0000df60: 0303 0000 7d94 286a 0503 0000 5d94 6a07  ....}.(j....].j.
+0000df70: 0300 005d 946a 0903 0000 5d94 6a0b 0300  ...].j....].j...
+0000df80: 005d 946a 0d03 0000 5d94 756a 0f03 0000  .].j....].uj....
+0000df90: 6a64 0500 006a ff02 0000 6ad3 0e00 0075  jd...j....j....u
+0000dfa0: 6265 6a03 0300 007d 9428 6a05 0300 005d  bej....}.(j....]
+0000dfb0: 946a 0703 0000 5d94 6a09 0300 005d 946a  .j....].j....].j
+0000dfc0: 0b03 0000 5d94 6a0d 0300 005d 9475 6a0f  ....].j....].uj.
+0000dfd0: 0300 006a 6905 0000 6aff 0200 006a d00e  ...ji...j....j..
+0000dfe0: 0000 7562 616a 0303 0000 7d94 286a 0503  ..ubaj....}.(j..
+0000dff0: 0000 5d94 6a07 0300 005d 946a 0903 0000  ..].j....].j....
+0000e000: 5d94 6a0b 0300 005d 946a 0d03 0000 5d94  ].j....].j....].
+0000e010: 756a 0f03 0000 6a64 0500 0075 6275 8c0f  uj....jd...ubu..
+0000e020: 746f 635f 6e75 6d5f 656e 7472 6965 7394  toc_num_entries.
+0000e030: 7d94 286a ca02 0000 4b03 6acb 0200 004b  }.(j....K.j....K
+0000e040: 016a 9b02 0000 4b09 758c 0e74 6f63 5f73  .j....K.u..toc_s
+0000e050: 6563 6e75 6d62 6572 7394 7d94 8c0e 746f  ecnumbers.}...to
+0000e060: 635f 6669 676e 756d 6265 7273 947d 948c  c_fignumbers.}..
+0000e070: 1074 6f63 7472 6565 5f69 6e63 6c75 6465  .toctree_include
+0000e080: 7394 7d94 286a ca02 0000 5d94 6abb 0c00  s.}.(j....].j...
+0000e090: 0061 6acb 0200 005d 946a 8a0d 0000 6175  .aj....].j....au
+0000e0a0: 8c10 6669 6c65 735f 746f 5f72 6562 7569  ..files_to_rebui
+0000e0b0: 6c64 947d 948c 1163 6f6f 6b69 6573 5f75  ld.}...cookies_u
+0000e0c0: 7469 6c69 7469 6573 948f 9428 6acb 0200  tilities...(j...
+0000e0d0: 006a ca02 0000 9073 8c0d 676c 6f62 5f74  .j.....s..glob_t
+0000e0e0: 6f63 7472 6565 7394 8f94 8c11 6e75 6d62  octrees.....numb
+0000e0f0: 6572 6564 5f74 6f63 7472 6565 7394 8f94  ered_toctrees...
+0000e100: 8c0a 646f 6d61 696e 6461 7461 947d 9428  ..domaindata.}.(
+0000e110: 8c01 6394 7d94 288c 0b72 6f6f 745f 7379  ..c.}.(..root_sy
+0000e120: 6d62 6f6c 946a 9f02 0000 8c06 5379 6d62  mbol.j......Symb
+0000e130: 6f6c 9493 9429 8194 7d94 286a ff02 0000  ol...)..}.(j....
+0000e140: 4e8c 0c73 6962 6c69 6e67 4162 6f76 6594  N..siblingAbove.
+0000e150: 4e8c 0c73 6962 6c69 6e67 4265 6c6f 7794  N..siblingBelow.
+0000e160: 4e8c 0569 6465 6e74 944e 8c0b 6465 636c  N..ident.N..decl
+0000e170: 6172 6174 696f 6e94 4e8c 0764 6f63 6e61  aration.N..docna
+0000e180: 6d65 944e 6a02 0300 004e 8c0f 6973 5265  me.Nj....N..isRe
+0000e190: 6465 636c 6172 6174 696f 6e94 898c 095f  declaration...._
+0000e1a0: 6368 696c 6472 656e 945d 948c 0d5f 616e  children.]..._an
+0000e1b0: 6f6e 4368 696c 6472 656e 945d 9475 628c  onChildren.].ub.
+0000e1c0: 076f 626a 6563 7473 947d 946a 9d02 0000  .objects.}.j....
+0000e1d0: 4b00 758c 0963 6861 6e67 6573 6574 947d  K.u..changeset.}
+0000e1e0: 9428 8c07 6368 616e 6765 7394 7d94 6a9d  .(..changes.}.j.
+0000e1f0: 0200 004b 0075 8c08 6369 7461 7469 6f6e  ...K.u..citation
+0000e200: 947d 9428 6a9d 0200 004b 008c 0963 6974  .}.(j....K...cit
+0000e210: 6174 696f 6e73 947d 948c 0d63 6974 6174  ations.}...citat
+0000e220: 696f 6e5f 7265 6673 947d 9475 8c03 6370  ion_refs.}.u..cp
+0000e230: 7094 7d94 286a 8910 0000 6aa2 0200 006a  p.}.(j....j....j
+0000e240: 8a10 0000 9394 2981 947d 9428 6aff 0200  ......)..}.(j...
+0000e250: 004e 6a8e 1000 004e 6a8f 1000 004e 8c09  .Nj....Nj....N..
+0000e260: 6964 656e 744f 724f 7094 4e8c 0e74 656d  identOrOp.N..tem
+0000e270: 706c 6174 6550 6172 616d 7394 4e8c 0c74  plateParams.N..t
+0000e280: 656d 706c 6174 6541 7267 7394 4e6a 9110  emplateArgs.Nj..
+0000e290: 0000 4e6a 9210 0000 4e6a 0203 0000 4e6a  ..Nj....Nj....Nj
+0000e2a0: 9310 0000 896a 9410 0000 5d94 6a96 1000  .....j....].j...
+0000e2b0: 005d 9475 628c 056e 616d 6573 947d 946a  .].ub..names.}.j
+0000e2c0: 9d02 0000 4b00 758c 0569 6e64 6578 947d  ....K.u..index.}
+0000e2d0: 9428 6a9d 0200 004b 008c 0765 6e74 7269  .(j....K...entri
+0000e2e0: 6573 947d 9428 6aca 0200 005d 946a cb02  es.}.(j....].j..
+0000e2f0: 0000 5d94 6a9b 0200 005d 9428 6a42 0300  ..].j....].(jB..
+0000e300: 006a 5109 0000 6abe 0900 006a b90a 0000  .jQ...j....j....
+0000e310: 6575 758c 026a 7394 7d94 286a 9810 0000  euu..js.}.(j....
+0000e320: 7d94 8c07 6d6f 6475 6c65 7394 7d94 6a9d  }...modules.}.j.
+0000e330: 0200 004b 0075 8c04 6d61 7468 947d 9428  ...K.u..math.}.(
+0000e340: 6a98 1000 007d 948c 0d68 6173 5f65 7175  j....}...has_equ
+0000e350: 6174 696f 6e73 947d 9428 6aca 0200 0089  ations.}.(j.....
+0000e360: 6acb 0200 0089 6a9b 0200 0089 756a 9d02  j.....j.....uj..
+0000e370: 0000 4b00 758c 0270 7994 7d94 286a 9810  ..K.u..py.}.(j..
+0000e380: 0000 7d94 288c 1b63 6f6f 6b69 6573 5f75  ..}.(..cookies_u
+0000e390: 7469 6c69 7469 6573 2e67 6574 5f64 6174  tilities.get_dat
+0000e3a0: 6573 948c 1573 7068 696e 782e 646f 6d61  es...sphinx.doma
+0000e3b0: 696e 732e 7079 7468 6f6e 948c 0b4f 626a  ins.python...Obj
+0000e3c0: 6563 7445 6e74 7279 9493 9428 6a9b 0200  ectEntry...(j...
+0000e3d0: 006a 4103 0000 6a64 0800 0089 7494 8194  .jA...jd....t...
+0000e3e0: 8c1b 636f 6f6b 6965 735f 7574 696c 6974  ..cookies_utilit
+0000e3f0: 6965 732e 5374 6f70 7761 7463 6894 6ac7  ies.Stopwatch.j.
+0000e400: 1000 0028 6a9b 0200 006a 5009 0000 6a10  ...(j....jP...j.
+0000e410: 0b00 0089 7494 8194 8c25 636f 6f6b 6965  ....t....%cookie
+0000e420: 735f 7574 696c 6974 6965 732e 7374 6f70  s_utilities.stop
+0000e430: 7761 7463 682e 5374 6f70 7761 7463 6894  watch.Stopwatch.
+0000e440: 6ac7 1000 0028 6a9b 0200 006a 5009 0000  j....(j....jP...
+0000e450: 6a10 0b00 0088 7494 8194 8c21 636f 6f6b  j.....t....!cook
+0000e460: 6965 735f 7574 696c 6974 6965 732e 5374  ies_utilities.St
+0000e470: 6f70 7761 7463 682e 7072 6573 7394 6ac7  opwatch.press.j.
+0000e480: 1000 0028 6a9b 0200 006a bd09 0000 6aa8  ...(j....j....j.
+0000e490: 0a00 0089 7494 8194 8c20 636f 6f6b 6965  ....t.... cookie
+0000e4a0: 735f 7574 696c 6974 6965 732e 5374 6f70  s_utilities.Stop
+0000e4b0: 7761 7463 682e 7368 6f77 946a c710 0000  watch.show.j....
+0000e4c0: 286a 9b02 0000 6ab8 0a00 006a 020b 0000  (j....j....j....
+0000e4d0: 8974 9481 9475 6aba 1000 007d 946a 9d02  .t...uj....}.j..
+0000e4e0: 0000 4b00 758c 0372 7374 947d 9428 6a98  ..K.u..rst.}.(j.
+0000e4f0: 1000 007d 946a 9d02 0000 4b00 758c 0373  ...}.j....K.u..s
+0000e500: 7464 947d 9428 8c0b 7072 6f67 6f70 7469  td.}.(..progopti
+0000e510: 6f6e 7394 7d94 6a98 1000 007d 948c 066c  ons.}.j....}...l
+0000e520: 6162 656c 7394 7d94 288c 0867 656e 696e  abels.}.(..genin
+0000e530: 6465 7894 6ae1 1000 0068 408c 0d73 7068  dex.j....h@..sph
+0000e540: 696e 782e 6c6f 6361 6c65 948c 115f 5472  inx.locale..._Tr
+0000e550: 616e 736c 6174 696f 6e50 726f 7879 9493  anslationProxy..
+0000e560: 9429 8194 8c06 7370 6869 6e78 948c 0767  .)....sphinx...g
+0000e570: 656e 6572 616c 948c 0549 6e64 6578 9487  eneral...Index..
+0000e580: 9462 8794 8c08 6d6f 6469 6e64 6578 948c  .b....modindex..
+0000e590: 0b70 792d 6d6f 6469 6e64 6578 9468 406a  .py-modindex.h@j
+0000e5a0: e410 0000 2981 946a e610 0000 6ae7 1000  ....)..j....j...
+0000e5b0: 008c 0c4d 6f64 756c 6520 496e 6465 7894  ...Module Index.
+0000e5c0: 8794 6287 948c 0673 6561 7263 6894 6af1  ..b....search.j.
+0000e5d0: 1000 0068 406a e410 0000 2981 946a e610  ...h@j....)..j..
+0000e5e0: 0000 6ae7 1000 008c 0b53 6561 7263 6820  ..j......Search 
+0000e5f0: 5061 6765 9487 9462 8794 8c0b 7079 2d6d  Page...b....py-m
+0000e600: 6f64 696e 6465 7894 8c0b 7079 2d6d 6f64  odindex...py-mod
+0000e610: 696e 6465 7894 6840 8c13 5079 7468 6f6e  index.h@..Python
+0000e620: 204d 6f64 756c 6520 496e 6465 7894 8794   Module Index...
+0000e630: 758c 0a61 6e6f 6e6c 6162 656c 7394 7d94  u..anonlabels.}.
+0000e640: 286a e110 0000 6ae1 1000 0068 4086 946a  (j....j....h@..j
+0000e650: eb10 0000 6aec 1000 0068 4086 946a f110  ....j....h@..j..
+0000e660: 0000 6af1 1000 0068 4086 946a f610 0000  ..j....h@..j....
+0000e670: 6af7 1000 0068 4086 9475 6a9d 0200 004b  j....h@..uj....K
+0000e680: 008c 0574 6572 6d73 947d 9475 758c 0669  ...terms.}.uu..i
+0000e690: 6d61 6765 7394 8c0b 7370 6869 6e78 2e75  mages...sphinx.u
+0000e6a0: 7469 6c94 8c10 4669 6c65 6e61 6d65 556e  til...FilenameUn
+0000e6b0: 6971 4469 6374 9493 9429 8194 8f94 628c  iqDict...)....b.
+0000e6c0: 0764 6c66 696c 6573 946a 0311 0000 8c0d  .dlfiles.j......
+0000e6d0: 446f 776e 6c6f 6164 4669 6c65 7394 9394  DownloadFiles...
+0000e6e0: 2981 948c 126f 7269 6769 6e61 6c5f 696d  )....original_im
+0000e6f0: 6167 655f 7572 6994 7d94 8c09 7465 6d70  age_uri.}...temp
+0000e700: 5f64 6174 6194 7d94 8c0b 7265 665f 636f  _data.}...ref_co
+0000e710: 6e74 6578 7494 7d94 8c14 5f73 6561 7263  ntext.}..._searc
+0000e720: 685f 696e 6465 785f 7469 746c 6573 947d  h_index_titles.}
+0000e730: 948c 175f 7365 6172 6368 5f69 6e64 6578  ..._search_index
+0000e740: 5f66 696c 656e 616d 6573 947d 948c 155f  _filenames.}..._
+0000e750: 7365 6172 6368 5f69 6e64 6578 5f6d 6170  search_index_map
+0000e760: 7069 6e67 947d 948c 1b5f 7365 6172 6368  ping.}..._search
+0000e770: 5f69 6e64 6578 5f74 6974 6c65 5f6d 6170  _index_title_map
+0000e780: 7069 6e67 947d 948c 185f 7365 6172 6368  ping.}..._search
+0000e790: 5f69 6e64 6578 5f61 6c6c 5f74 6974 6c65  _index_all_title
+0000e7a0: 7394 7d94 8c1b 5f73 6561 7263 685f 696e  s.}..._search_in
+0000e7b0: 6465 785f 696e 6465 785f 656e 7472 6965  dex_index_entrie
+0000e7c0: 7394 7d94 8c16 5f73 6561 7263 685f 696e  s.}..._search_in
+0000e7d0: 6465 785f 6f62 6a74 7970 6573 947d 948c  dex_objtypes.}..
+0000e7e0: 165f 7365 6172 6368 5f69 6e64 6578 5f6f  ._search_index_o
+0000e7f0: 626a 6e61 6d65 7394 7d94 7562 2e         bjnames.}.ub.
```

### Comparing `cookies_utilities-0.0.1/docs/build/doctrees/index.doctree` & `cookies_utilities-0.0.2/docs/build/doctrees/index.doctree`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8005 95da 1300 0000 0000 008c 0f73 7068  .............sph
+00000000: 8005 95bf 1400 0000 0000 008c 0f73 7068  .............sph
 00000010: 696e 782e 6164 646e 6f64 6573 948c 0864  inx.addnodes...d
 00000020: 6f63 756d 656e 7494 9394 2981 947d 9428  ocument...)..}.(
 00000030: 8c09 7261 7773 6f75 7263 6594 8c00 948c  ..rawsource.....
 00000040: 0863 6869 6c64 7265 6e94 5d94 8c0e 646f  .children.]...do
 00000050: 6375 7469 6c73 2e6e 6f64 6573 948c 0773  cutils.nodes...s
 00000060: 6563 7469 6f6e 9493 9429 8194 7d94 2868  ection...)..}.(h
 00000070: 0568 0668 075d 9428 6809 8c05 7469 746c  .h.h.].(h...titl
@@ -31,289 +31,303 @@
 000001e0: 6807 5d94 2868 1029 8194 7d94 2868 058c  h.].(h.)..}.(h..
 000001f0: 054c 696e 6b73 9468 075d 9468 168c 054c  .Links.h.].h...L
 00000200: 696e 6b73 9485 9481 947d 9428 681b 6830  inks.....}.(h.h0
 00000210: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
 00000220: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
 00000230: 5d94 6829 5d94 7568 2b68 0f68 1b68 2d68  ].h)].uh+h.h.h-h
 00000240: 1c68 0368 1d68 2c68 1e4b 0575 6268 098c  .h.h.h,h.K.ubh..
-00000250: 0b62 756c 6c65 745f 6c69 7374 9493 9429  .bullet_list...)
-00000260: 8194 7d94 2868 0568 0668 075d 9428 6809  ..}.(h.h.h.].(h.
-00000270: 8c09 6c69 7374 5f69 7465 6d94 9394 2981  ..list_item...).
-00000280: 947d 9428 6805 8c3e 6054 6573 7450 7950  .}.(h..>`TestPyP
-00000290: 4920 3c68 7474 7073 3a2f 2f74 6573 742e  I <https://test.
-000002a0: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
-000002b0: 2f63 6f6f 6b69 6573 2d75 7469 6c69 7469  /cookies-utiliti
-000002c0: 6573 2f3e 605f 9468 075d 9468 098c 0970  es/>`_.h.].h...p
-000002d0: 6172 6167 7261 7068 9493 9429 8194 7d94  aragraph...)..}.
-000002e0: 2868 0568 4768 075d 9428 6809 8c09 7265  (h.hGh.].(h...re
-000002f0: 6665 7265 6e63 6594 9394 2981 947d 9428  ference...)..}.(
-00000300: 6805 6847 6807 5d94 6816 8c08 5465 7374  h.hGh.].h...Test
-00000310: 5079 5049 9485 9481 947d 9428 681b 6850  PyPI.....}.(h.hP
-00000320: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
-00000330: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-00000340: 5d94 6829 5d94 8c04 6e61 6d65 948c 0854  ].h)]...name...T
-00000350: 6573 7450 7950 4994 8c06 7265 6675 7269  estPyPI...refuri
-00000360: 948c 3068 7474 7073 3a2f 2f74 6573 742e  ..0https://test.
-00000370: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
-00000380: 2f63 6f6f 6b69 6573 2d75 7469 6c69 7469  /cookies-utiliti
-00000390: 6573 2f94 7568 2b68 4e68 1b68 4b75 6268  es/.uh+hNh.hKubh
-000003a0: 098c 0674 6172 6765 7494 9394 2981 947d  ...target...)..}
-000003b0: 9428 6805 8c33 203c 6874 7470 733a 2f2f  .(h..3 <https://
-000003c0: 7465 7374 2e70 7970 692e 6f72 672f 7072  test.pypi.org/pr
-000003d0: 6f6a 6563 742f 636f 6f6b 6965 732d 7574  oject/cookies-ut
-000003e0: 696c 6974 6965 732f 3e94 6807 5d94 681f  ilities/>.h.].h.
-000003f0: 7d94 2868 215d 948c 0874 6573 7470 7970  }.(h!]...testpyp
-00000400: 6994 6168 235d 9468 255d 948c 0874 6573  i.ah#].h%]...tes
-00000410: 7470 7970 6994 6168 275d 9468 295d 948c  tpypi.ah'].h)]..
-00000420: 0672 6566 7572 6994 6860 7568 2b68 618c  .refuri.h`uh+ha.
-00000430: 0a72 6566 6572 656e 6365 6494 4b01 681b  .referenced.K.h.
-00000440: 684b 7562 6568 1f7d 9428 6821 5d94 6823  hKubeh.}.(h!].h#
-00000450: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
-00000460: 2b68 4968 1d68 2c68 1e4b 0768 1b68 4575  +hIh.h,h.K.h.hEu
-00000470: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-00000480: 255d 9468 275d 9468 295d 9475 682b 6843  %].h'].h)].uh+hC
-00000490: 681b 6840 681c 6803 681d 682c 681e 4e75  h.h@h.h.h.h,h.Nu
-000004a0: 6268 4429 8194 7d94 2868 058c 3d60 4769  bhD)..}.(h..=`Gi
-000004b0: 7448 7562 203c 6874 7470 733a 2f2f 6769  tHub <https://gi
-000004c0: 7468 7562 2e63 6f6d 2f43 6f6f 6b69 6542  thub.com/CookieB
-000004d0: 6f78 3236 2f63 6f6f 6b69 6573 5f75 7469  ox26/cookies_uti
-000004e0: 6c69 7469 6573 3e60 5f0a 9468 075d 9468  lities>`_..h.].h
-000004f0: 4a29 8194 7d94 2868 058c 3c60 4769 7448  J)..}.(h..<`GitH
-00000500: 7562 203c 6874 7470 733a 2f2f 6769 7468  ub <https://gith
-00000510: 7562 2e63 6f6d 2f43 6f6f 6b69 6542 6f78  ub.com/CookieBox
-00000520: 3236 2f63 6f6f 6b69 6573 5f75 7469 6c69  26/cookies_utili
-00000530: 7469 6573 3e60 5f94 6807 5d94 2868 4f29  ties>`_.h.].(hO)
-00000540: 8194 7d94 2868 0568 8368 075d 9468 168c  ..}.(h.h.h.].h..
-00000550: 0647 6974 4875 6294 8594 8194 7d94 2868  .GitHub.....}.(h
-00000560: 1b68 8568 1c68 0368 1d4e 681e 4e75 6261  .h.h.h.h.Nh.Nuba
-00000570: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00000580: 9468 275d 9468 295d 948c 046e 616d 6594  .h'].h)]...name.
-00000590: 8c06 4769 7448 7562 9468 5f8c 3068 7474  ..GitHub.h_.0htt
-000005a0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000005b0: 436f 6f6b 6965 426f 7832 362f 636f 6f6b  CookieBox26/cook
-000005c0: 6965 735f 7574 696c 6974 6965 7394 7568  ies_utilities.uh
-000005d0: 2b68 4e68 1b68 8175 6268 6229 8194 7d94  +hNh.h.ubhb)..}.
-000005e0: 2868 058c 3320 3c68 7474 7073 3a2f 2f67  (h..3 <https://g
-000005f0: 6974 6875 622e 636f 6d2f 436f 6f6b 6965  ithub.com/Cookie
-00000600: 426f 7832 362f 636f 6f6b 6965 735f 7574  Box26/cookies_ut
-00000610: 696c 6974 6965 733e 9468 075d 9468 1f7d  ilities>.h.].h.}
-00000620: 9428 6821 5d94 8c06 6769 7468 7562 9461  .(h!]...github.a
-00000630: 6823 5d94 6825 5d94 8c06 6769 7468 7562  h#].h%]...github
-00000640: 9461 6827 5d94 6829 5d94 8c06 7265 6675  .ah'].h)]...refu
-00000650: 7269 9468 9475 682b 6861 6870 4b01 681b  ri.h.uh+hahpK.h.
-00000660: 6881 7562 6568 1f7d 9428 6821 5d94 6823  h.ubeh.}.(h!].h#
-00000670: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
-00000680: 2b68 4968 1d68 2c68 1e4b 0868 1b68 7d75  +hIh.h,h.K.h.h}u
-00000690: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-000006a0: 255d 9468 275d 9468 295d 9475 682b 6843  %].h'].h)].uh+hC
-000006b0: 681b 6840 681c 6803 681d 682c 681e 4e75  h.h@h.h.h.h,h.Nu
-000006c0: 6265 681f 7d94 2868 215d 9468 235d 9468  beh.}.(h!].h#].h
-000006d0: 255d 9468 275d 9468 295d 948c 0662 756c  %].h'].h)]...bul
-000006e0: 6c65 7494 8c01 2d94 7568 2b68 3e68 1d68  let...-.uh+h>h.h
-000006f0: 2c68 1e4b 0768 1b68 2d68 1c68 0375 6268  ,h.K.h.h-h.h.ubh
-00000700: 098c 0863 6f6d 706f 756e 6494 9394 2981  ...compound...).
-00000710: 947d 9428 6805 6806 6807 5d94 6800 8c07  .}.(h.h.h.].h...
-00000720: 746f 6374 7265 6594 9394 2981 947d 9428  toctree...)..}.(
-00000730: 6805 6806 6807 5d94 681f 7d94 2868 215d  h.h.h.].h.}.(h!]
+00000250: 0763 6f6d 6d65 6e74 9493 9429 8194 7d94  .comment...)..}.
+00000260: 2868 058c 402d 2060 5465 7374 5079 5049  (h..@- `TestPyPI
+00000270: 203c 6874 7470 733a 2f2f 7465 7374 2e70   <https://test.p
+00000280: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+00000290: 636f 6f6b 6965 732d 7574 696c 6974 6965  cookies-utilitie
+000002a0: 732f 3e60 5f94 6807 5d94 6816 8c40 2d20  s/>`_.h.].h..@- 
+000002b0: 6054 6573 7450 7950 4920 3c68 7474 7073  `TestPyPI <https
+000002c0: 3a2f 2f74 6573 742e 7079 7069 2e6f 7267  ://test.pypi.org
+000002d0: 2f70 726f 6a65 6374 2f63 6f6f 6b69 6573  /project/cookies
+000002e0: 2d75 7469 6c69 7469 6573 2f3e 605f 9485  -utilities/>`_..
+000002f0: 9481 947d 9468 1b68 4073 6261 681f 7d94  ...}.h.h@sbah.}.
+00000300: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00000310: 9468 295d 948c 0978 6d6c 3a73 7061 6365  .h)]...xml:space
+00000320: 948c 0870 7265 7365 7276 6594 7568 2b68  ...preserve.uh+h
+00000330: 3e68 1b68 2d68 1c68 0368 1d68 2c68 1e4b  >h.h-h.h.h.h,h.K
+00000340: 0875 6268 098c 0b62 756c 6c65 745f 6c69  .ubh...bullet_li
+00000350: 7374 9493 9429 8194 7d94 2868 0568 0668  st...)..}.(h.h.h
+00000360: 075d 9428 6809 8c09 6c69 7374 5f69 7465  .].(h...list_ite
+00000370: 6d94 9394 2981 947d 9428 6805 8c35 6050  m...)..}.(h..5`P
+00000380: 7950 4920 3c68 7474 7073 3a2f 2f70 7970  yPI <https://pyp
+00000390: 692e 6f72 672f 7072 6f6a 6563 742f 636f  i.org/project/co
+000003a0: 6f6b 6965 732d 7574 696c 6974 6965 732f  okies-utilities/
+000003b0: 3e60 5f94 6807 5d94 6809 8c09 7061 7261  >`_.h.].h...para
+000003c0: 6772 6170 6894 9394 2981 947d 9428 6805  graph...)..}.(h.
+000003d0: 6859 6807 5d94 2868 098c 0972 6566 6572  hYh.].(h...refer
+000003e0: 656e 6365 9493 9429 8194 7d94 2868 0568  ence...)..}.(h.h
+000003f0: 5968 075d 9468 168c 0450 7950 4994 8594  Yh.].h...PyPI...
+00000400: 8194 7d94 2868 1b68 6268 1c68 0368 1d4e  ..}.(h.hbh.h.h.N
+00000410: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
+00000420: 235d 9468 255d 9468 275d 9468 295d 948c  #].h%].h'].h)]..
+00000430: 046e 616d 6594 8c04 5079 5049 948c 0672  .name...PyPI...r
+00000440: 6566 7572 6994 8c2b 6874 7470 733a 2f2f  efuri..+https://
+00000450: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+00000460: 2f63 6f6f 6b69 6573 2d75 7469 6c69 7469  /cookies-utiliti
+00000470: 6573 2f94 7568 2b68 6068 1b68 5d75 6268  es/.uh+h`h.h]ubh
+00000480: 098c 0674 6172 6765 7494 9394 2981 947d  ...target...)..}
+00000490: 9428 6805 8c2e 203c 6874 7470 733a 2f2f  .(h... <https://
+000004a0: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+000004b0: 2f63 6f6f 6b69 6573 2d75 7469 6c69 7469  /cookies-utiliti
+000004c0: 6573 2f3e 9468 075d 9468 1f7d 9428 6821  es/>.h.].h.}.(h!
+000004d0: 5d94 8c04 7079 7069 9461 6823 5d94 6825  ]...pypi.ah#].h%
+000004e0: 5d94 8c04 7079 7069 9461 6827 5d94 6829  ]...pypi.ah'].h)
+000004f0: 5d94 8c06 7265 6675 7269 9468 7275 682b  ]...refuri.hruh+
+00000500: 6873 8c0a 7265 6665 7265 6e63 6564 944b  hs..referenced.K
+00000510: 0168 1b68 5d75 6265 681f 7d94 2868 215d  .h.h]ubeh.}.(h!]
+00000520: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+00000530: 9475 682b 685b 681d 682c 681e 4b09 681b  .uh+h[h.h,h.K.h.
+00000540: 6857 7562 6168 1f7d 9428 6821 5d94 6823  hWubah.}.(h!].h#
+00000550: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+00000560: 2b68 5568 1b68 5268 1c68 0368 1d68 2c68  +hUh.hRh.h.h.h,h
+00000570: 1e4e 7562 6856 2981 947d 9428 6805 8c3d  .NubhV)..}.(h..=
+00000580: 6047 6974 4875 6220 3c68 7474 7073 3a2f  `GitHub <https:/
+00000590: 2f67 6974 6875 622e 636f 6d2f 436f 6f6b  /github.com/Cook
+000005a0: 6965 426f 7832 362f 636f 6f6b 6965 735f  ieBox26/cookies_
+000005b0: 7574 696c 6974 6965 733e 605f 0a94 6807  utilities>`_..h.
+000005c0: 5d94 685c 2981 947d 9428 6805 8c3c 6047  ].h\)..}.(h..<`G
+000005d0: 6974 4875 6220 3c68 7474 7073 3a2f 2f67  itHub <https://g
+000005e0: 6974 6875 622e 636f 6d2f 436f 6f6b 6965  ithub.com/Cookie
+000005f0: 426f 7832 362f 636f 6f6b 6965 735f 7574  Box26/cookies_ut
+00000600: 696c 6974 6965 733e 605f 9468 075d 9428  ilities>`_.h.].(
+00000610: 6861 2981 947d 9428 6805 6895 6807 5d94  ha)..}.(h.h.h.].
+00000620: 6816 8c06 4769 7448 7562 9485 9481 947d  h...GitHub.....}
+00000630: 9428 681b 6897 681c 6803 681d 4e68 1e4e  .(h.h.h.h.h.Nh.N
+00000640: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00000650: 6825 5d94 6827 5d94 6829 5d94 8c04 6e61  h%].h'].h)]...na
+00000660: 6d65 948c 0647 6974 4875 6294 6871 8c30  me...GitHub.hq.0
+00000670: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000680: 6f6d 2f43 6f6f 6b69 6542 6f78 3236 2f63  om/CookieBox26/c
+00000690: 6f6f 6b69 6573 5f75 7469 6c69 7469 6573  ookies_utilities
+000006a0: 9475 682b 6860 681b 6893 7562 6874 2981  .uh+h`h.h.ubht).
+000006b0: 947d 9428 6805 8c33 203c 6874 7470 733a  .}.(h..3 <https:
+000006c0: 2f2f 6769 7468 7562 2e63 6f6d 2f43 6f6f  //github.com/Coo
+000006d0: 6b69 6542 6f78 3236 2f63 6f6f 6b69 6573  kieBox26/cookies
+000006e0: 5f75 7469 6c69 7469 6573 3e94 6807 5d94  _utilities>.h.].
+000006f0: 681f 7d94 2868 215d 948c 0667 6974 6875  h.}.(h!]...githu
+00000700: 6294 6168 235d 9468 255d 948c 0667 6974  b.ah#].h%]...git
+00000710: 6875 6294 6168 275d 9468 295d 948c 0672  hub.ah'].h)]...r
+00000720: 6566 7572 6994 68a6 7568 2b68 7368 824b  efuri.h.uh+hsh.K
+00000730: 0168 1b68 9375 6265 681f 7d94 2868 215d  .h.h.ubeh.}.(h!]
 00000740: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00000750: 9468 1b8c 0569 6e64 6578 948c 0765 6e74  .h...index...ent
-00000760: 7269 6573 945d 944e 8c11 636f 6f6b 6965  ries.].N..cookie
-00000770: 735f 7574 696c 6974 6965 7394 8694 618c  s_utilities...a.
-00000780: 0c69 6e63 6c75 6465 6669 6c65 7394 5d94  .includefiles.].
-00000790: 68c9 618c 086d 6178 6465 7074 6894 4b02  h.a..maxdepth.K.
-000007a0: 8c07 6361 7074 696f 6e94 8c09 436f 6e74  ..caption...Cont
-000007b0: 656e 7473 3a94 8c04 676c 6f62 9489 8c06  ents:...glob....
-000007c0: 6869 6464 656e 9489 8c0d 696e 636c 7564  hidden....includ
-000007d0: 6568 6964 6465 6e94 898c 086e 756d 6265  ehidden....numbe
-000007e0: 7265 6494 4b00 8c0a 7469 746c 6573 6f6e  red.K...titleson
-000007f0: 6c79 9489 8c0a 7261 7765 6e74 7269 6573  ly....rawentries
-00000800: 945d 948c 0a72 6177 6361 7074 696f 6e94  .]...rawcaption.
-00000810: 68cf 7568 2b68 bb68 1d68 2c68 1e4b 0a68  h.uh+h.h.h,h.K.h
-00000820: 1b68 b875 6261 681f 7d94 2868 215d 9468  .h.ubah.}.(h!].h
-00000830: 235d 948c 0f74 6f63 7472 6565 2d77 7261  #]...toctree-wra
-00000840: 7070 6572 9461 6825 5d94 6827 5d94 6829  pper.ah%].h'].h)
-00000850: 5d94 7568 2b68 b668 1b68 2d68 1c68 0368  ].uh+h.h.h-h.h.h
-00000860: 1d68 2c68 1e4e 7562 6568 1f7d 9428 6821  .h,h.Nubeh.}.(h!
-00000870: 5d94 8c05 6c69 6e6b 7394 6168 235d 9468  ]...links.ah#].h
-00000880: 255d 948c 056c 696e 6b73 9461 6827 5d94  %]...links.ah'].
-00000890: 6829 5d94 7568 2b68 0a68 1b68 0c68 1c68  h)].uh+h.h.h.h.h
-000008a0: 0368 1d68 2c68 1e4b 0575 6268 0b29 8194  .h.h,h.K.ubh.)..
-000008b0: 7d94 2868 0568 0668 075d 9428 6810 2981  }.(h.h.h.].(h.).
-000008c0: 947d 9428 6805 8c12 496e 6469 6365 7320  .}.(h...Indices 
-000008d0: 616e 6420 7461 626c 6573 9468 075d 9468  and tables.h.].h
-000008e0: 168c 1249 6e64 6963 6573 2061 6e64 2074  ...Indices and t
-000008f0: 6162 6c65 7394 8594 8194 7d94 2868 1b68  ables.....}.(h.h
-00000900: ea68 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
-00000910: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-00000920: 275d 9468 295d 9475 682b 680f 681b 68e7  '].h)].uh+h.h.h.
-00000930: 681c 6803 681d 682c 681e 4b11 7562 683f  h.h.h.h,h.K.ubh?
-00000940: 2981 947d 9428 6805 6806 6807 5d94 6844  )..}.(h.h.h.].hD
-00000950: 2981 947d 9428 6805 8c0f 3a72 6566 3a60  )..}.(h...:ref:`
-00000960: 6765 6e69 6e64 6578 6094 6807 5d94 684a  genindex`.h.].hJ
-00000970: 2981 947d 9428 6805 68fd 6807 5d94 6800  )..}.(h.h.h.].h.
-00000980: 8c0c 7065 6e64 696e 675f 7872 6566 9493  ..pending_xref..
-00000990: 9429 8194 7d94 2868 0568 fd68 075d 9468  .)..}.(h.h.h.].h
-000009a0: 098c 0669 6e6c 696e 6594 9394 2981 947d  ...inline...)..}
-000009b0: 9428 6805 68fd 6807 5d94 6816 8c08 6765  .(h.h.h.].h...ge
-000009c0: 6e69 6e64 6578 9485 9481 947d 9428 681b  nindex.....}.(h.
-000009d0: 6a09 0100 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
-000009e0: 6261 681f 7d94 2868 215d 9468 235d 9428  bah.}.(h!].h#].(
-000009f0: 8c04 7872 6566 948c 0373 7464 948c 0773  ..xref...std...s
-00000a00: 7464 2d72 6566 9465 6825 5d94 6827 5d94  td-ref.eh%].h'].
-00000a10: 6829 5d94 7568 2b6a 0701 0000 681b 6a04  h)].uh+j....h.j.
-00000a20: 0100 0075 6261 681f 7d94 2868 215d 9468  ...ubah.}.(h!].h
-00000a30: 235d 9468 255d 9468 275d 9468 295d 948c  #].h%].h'].h)]..
-00000a40: 0672 6566 646f 6394 68c6 8c09 7265 6664  .refdoc.h...refd
-00000a50: 6f6d 6169 6e94 6a14 0100 008c 0772 6566  omain.j......ref
-00000a60: 7479 7065 948c 0372 6566 948c 0b72 6566  type...ref...ref
-00000a70: 6578 706c 6963 6974 9489 8c07 7265 6677  explicit....refw
-00000a80: 6172 6e94 888c 0972 6566 7461 7267 6574  arn....reftarget
-00000a90: 948c 0867 656e 696e 6465 7894 7568 2b6a  ...genindex.uh+j
-00000aa0: 0201 0000 681d 682c 681e 4b13 681b 68ff  ....h.h,h.K.h.h.
-00000ab0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-00000ac0: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
-00000ad0: 4968 1d68 2c68 1e4b 1368 1b68 fb75 6261  Ih.h,h.K.h.h.uba
-00000ae0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00000af0: 9468 275d 9468 295d 9475 682b 6843 681b  .h'].h)].uh+hCh.
-00000b00: 68f8 681c 6803 681d 682c 681e 4e75 6261  h.h.h.h.h,h.Nuba
-00000b10: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00000b20: 9468 275d 9468 295d 9468 b48c 012a 9475  .h'].h)].h...*.u
-00000b30: 682b 683e 681d 682c 681e 4b13 681b 68e7  h+h>h.h,h.K.h.h.
-00000b40: 681c 6803 7562 6568 1f7d 9428 6821 5d94  h.h.ubeh.}.(h!].
-00000b50: 8c12 696e 6469 6365 732d 616e 642d 7461  ..indices-and-ta
-00000b60: 626c 6573 9461 6823 5d94 6825 5d94 8c12  bles.ah#].h%]...
-00000b70: 696e 6469 6365 7320 616e 6420 7461 626c  indices and tabl
-00000b80: 6573 9461 6827 5d94 6829 5d94 7568 2b68  es.ah'].h)].uh+h
-00000b90: 0a68 1b68 0c68 1c68 0368 1d68 2c68 1e4b  .h.h.h.h.h.h,h.K
-00000ba0: 1175 6265 681f 7d94 2868 215d 948c 2a77  .ubeh.}.(h!]..*w
-00000bb0: 656c 636f 6d65 2d74 6f2d 636f 6f6b 6965  elcome-to-cookie
-00000bc0: 732d 7574 696c 6974 6965 732d 646f 6375  s-utilities-docu
-00000bd0: 6d65 6e74 6174 696f 6e94 6168 235d 9468  mentation.ah#].h
-00000be0: 255d 948c 2c77 656c 636f 6d65 2074 6f20  %]..,welcome to 
-00000bf0: 636f 6f6b 6965 735f 7574 696c 6974 6965  cookies_utilitie
-00000c00: 7327 2064 6f63 756d 656e 7461 7469 6f6e  s' documentation
-00000c10: 2194 6168 275d 9468 295d 9475 682b 680a  !.ah'].h)].uh+h.
-00000c20: 681b 6803 681c 6803 681d 682c 681e 4b02  h.h.h.h.h.h,h.K.
-00000c30: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-00000c40: 6825 5d94 6827 5d94 6829 5d94 8c06 736f  h%].h'].h)]...so
-00000c50: 7572 6365 9468 2c75 682b 6801 8c0e 6375  urce.h,uh+h...cu
-00000c60: 7272 656e 745f 736f 7572 6365 944e 8c0c  rrent_source.N..
-00000c70: 6375 7272 656e 745f 6c69 6e65 944e 8c08  current_line.N..
-00000c80: 7365 7474 696e 6773 948c 1164 6f63 7574  settings...docut
-00000c90: 696c 732e 6672 6f6e 7465 6e64 948c 0656  ils.frontend...V
-00000ca0: 616c 7565 7394 9394 2981 947d 9428 680f  alues...)..}.(h.
-00000cb0: 4e8c 0967 656e 6572 6174 6f72 944e 8c09  N..generator.N..
-00000cc0: 6461 7465 7374 616d 7094 4e8c 0b73 6f75  datestamp.N..sou
-00000cd0: 7263 655f 6c69 6e6b 944e 8c0a 736f 7572  rce_link.N..sour
-00000ce0: 6365 5f75 726c 944e 8c0d 746f 635f 6261  ce_url.N..toc_ba
-00000cf0: 636b 6c69 6e6b 7394 8c05 656e 7472 7994  cklinks...entry.
-00000d00: 8c12 666f 6f74 6e6f 7465 5f62 6163 6b6c  ..footnote_backl
-00000d10: 696e 6b73 944b 018c 0d73 6563 746e 756d  inks.K...sectnum
-00000d20: 5f78 666f 726d 944b 018c 0e73 7472 6970  _xform.K...strip
-00000d30: 5f63 6f6d 6d65 6e74 7394 4e8c 1b73 7472  _comments.N..str
-00000d40: 6970 5f65 6c65 6d65 6e74 735f 7769 7468  ip_elements_with
-00000d50: 5f63 6c61 7373 6573 944e 8c0d 7374 7269  _classes.N..stri
-00000d60: 705f 636c 6173 7365 7394 4e8c 0c72 6570  p_classes.N..rep
-00000d70: 6f72 745f 6c65 7665 6c94 4b02 8c0a 6861  ort_level.K...ha
-00000d80: 6c74 5f6c 6576 656c 944b 058c 1165 7869  lt_level.K...exi
-00000d90: 745f 7374 6174 7573 5f6c 6576 656c 944b  t_status_level.K
-00000da0: 058c 0564 6562 7567 944e 8c0e 7761 726e  ...debug.N..warn
-00000db0: 696e 675f 7374 7265 616d 944e 8c09 7472  ing_stream.N..tr
-00000dc0: 6163 6562 6163 6b94 888c 0e69 6e70 7574  aceback....input
-00000dd0: 5f65 6e63 6f64 696e 6794 8c09 7574 662d  _encoding...utf-
-00000de0: 382d 7369 6794 8c1c 696e 7075 745f 656e  8-sig...input_en
-00000df0: 636f 6469 6e67 5f65 7272 6f72 5f68 616e  coding_error_han
-00000e00: 646c 6572 948c 0673 7472 6963 7494 8c0f  dler...strict...
-00000e10: 6f75 7470 7574 5f65 6e63 6f64 696e 6794  output_encoding.
-00000e20: 8c05 7574 662d 3894 8c1d 6f75 7470 7574  ..utf-8...output
-00000e30: 5f65 6e63 6f64 696e 675f 6572 726f 725f  _encoding_error_
-00000e40: 6861 6e64 6c65 7294 6a6d 0100 008c 0e65  handler.jm.....e
-00000e50: 7272 6f72 5f65 6e63 6f64 696e 6794 8c05  rror_encoding...
-00000e60: 7574 662d 3894 8c1c 6572 726f 725f 656e  utf-8...error_en
-00000e70: 636f 6469 6e67 5f65 7272 6f72 5f68 616e  coding_error_han
-00000e80: 646c 6572 948c 1062 6163 6b73 6c61 7368  dler...backslash
-00000e90: 7265 706c 6163 6594 8c0d 6c61 6e67 7561  replace...langua
-00000ea0: 6765 5f63 6f64 6594 8c02 656e 948c 1372  ge_code...en...r
-00000eb0: 6563 6f72 645f 6465 7065 6e64 656e 6369  ecord_dependenci
-00000ec0: 6573 944e 8c06 636f 6e66 6967 944e 8c09  es.N..config.N..
-00000ed0: 6964 5f70 7265 6669 7894 6806 8c0e 6175  id_prefix.h...au
-00000ee0: 746f 5f69 645f 7072 6566 6978 948c 0269  to_id_prefix...i
-00000ef0: 6494 8c0d 6475 6d70 5f73 6574 7469 6e67  d...dump_setting
-00000f00: 7394 4e8c 0e64 756d 705f 696e 7465 726e  s.N..dump_intern
-00000f10: 616c 7394 4e8c 0f64 756d 705f 7472 616e  als.N..dump_tran
-00000f20: 7366 6f72 6d73 944e 8c0f 6475 6d70 5f70  sforms.N..dump_p
-00000f30: 7365 7564 6f5f 786d 6c94 4e8c 1065 7870  seudo_xml.N..exp
-00000f40: 6f73 655f 696e 7465 726e 616c 7394 4e8c  ose_internals.N.
-00000f50: 0e73 7472 6963 745f 7669 7369 746f 7294  .strict_visitor.
-00000f60: 4e8c 0f5f 6469 7361 626c 655f 636f 6e66  N.._disable_conf
-00000f70: 6967 944e 8c07 5f73 6f75 7263 6594 682c  ig.N.._source.h,
-00000f80: 8c0c 5f64 6573 7469 6e61 7469 6f6e 944e  .._destination.N
-00000f90: 8c0d 5f63 6f6e 6669 675f 6669 6c65 7394  .._config_files.
-00000fa0: 5d94 8c16 6669 6c65 5f69 6e73 6572 7469  ]...file_inserti
-00000fb0: 6f6e 5f65 6e61 626c 6564 9488 8c0b 7261  on_enabled....ra
-00000fc0: 775f 656e 6162 6c65 6494 4b01 8c11 6c69  w_enabled.K...li
-00000fd0: 6e65 5f6c 656e 6774 685f 6c69 6d69 7494  ne_length_limit.
-00000fe0: 4d10 278c 0e70 6570 5f72 6566 6572 656e  M.'..pep_referen
-00000ff0: 6365 7394 4e8c 0c70 6570 5f62 6173 655f  ces.N..pep_base_
-00001000: 7572 6c94 8c18 6874 7470 733a 2f2f 7065  url...https://pe
-00001010: 7073 2e70 7974 686f 6e2e 6f72 672f 948c  ps.python.org/..
-00001020: 1570 6570 5f66 696c 655f 7572 6c5f 7465  .pep_file_url_te
-00001030: 6d70 6c61 7465 948c 0870 6570 2d25 3034  mplate...pep-%04
-00001040: 6494 8c0e 7266 635f 7265 6665 7265 6e63  d...rfc_referenc
-00001050: 6573 944e 8c0c 7266 635f 6261 7365 5f75  es.N..rfc_base_u
-00001060: 726c 948c 2668 7474 7073 3a2f 2f64 6174  rl..&https://dat
-00001070: 6174 7261 636b 6572 2e69 6574 662e 6f72  atracker.ietf.or
-00001080: 672f 646f 632f 6874 6d6c 2f94 8c09 7461  g/doc/html/...ta
-00001090: 625f 7769 6474 6894 4b08 8c1d 7472 696d  b_width.K...trim
-000010a0: 5f66 6f6f 746e 6f74 655f 7265 6665 7265  _footnote_refere
-000010b0: 6e63 655f 7370 6163 6594 898c 1073 796e  nce_space....syn
-000010c0: 7461 785f 6869 6768 6c69 6768 7494 8c04  tax_highlight...
-000010d0: 6c6f 6e67 948c 0c73 6d61 7274 5f71 756f  long...smart_quo
-000010e0: 7465 7394 888c 1373 6d61 7274 7175 6f74  tes....smartquot
-000010f0: 6573 5f6c 6f63 616c 6573 945d 948c 1d63  es_locales.]...c
-00001100: 6861 7261 6374 6572 5f6c 6576 656c 5f69  haracter_level_i
-00001110: 6e6c 696e 655f 6d61 726b 7570 9489 8c0e  nline_markup....
-00001120: 646f 6374 6974 6c65 5f78 666f 726d 9489  doctitle_xform..
-00001130: 8c0d 646f 6369 6e66 6f5f 7866 6f72 6d94  ..docinfo_xform.
-00001140: 4b01 8c12 7365 6374 7375 6274 6974 6c65  K...sectsubtitle
-00001150: 5f78 666f 726d 9489 8c0d 696d 6167 655f  _xform....image_
-00001160: 6c6f 6164 696e 6794 8c04 6c69 6e6b 948c  loading...link..
-00001170: 1065 6d62 6564 5f73 7479 6c65 7368 6565  .embed_styleshee
-00001180: 7494 898c 1563 6c6f 616b 5f65 6d61 696c  t....cloak_email
-00001190: 5f61 6464 7265 7373 6573 9488 8c11 7365  _addresses....se
-000011a0: 6374 696f 6e5f 7365 6c66 5f6c 696e 6b94  ction_self_link.
-000011b0: 898c 0365 6e76 944e 7562 8c08 7265 706f  ...env.Nub..repo
-000011c0: 7274 6572 944e 8c10 696e 6469 7265 6374  rter.N..indirect
-000011d0: 5f74 6172 6765 7473 945d 948c 1173 7562  _targets.]...sub
-000011e0: 7374 6974 7574 696f 6e5f 6465 6673 947d  stitution_defs.}
-000011f0: 948c 1273 7562 7374 6974 7574 696f 6e5f  ...substitution_
-00001200: 6e61 6d65 7394 7d94 8c08 7265 666e 616d  names.}...refnam
-00001210: 6573 947d 948c 0672 6566 6964 7394 7d94  es.}...refids.}.
-00001220: 8c07 6e61 6d65 6964 7394 7d94 286a 4701  ..nameids.}.(jG.
-00001230: 0000 6a44 0100 0068 e468 e168 6c68 6968  ..jD...h.h.hlhih
-00001240: 9e68 9b6a 3f01 0000 6a3c 0100 0075 8c09  .h.j?...j<...u..
-00001250: 6e61 6d65 7479 7065 7394 7d94 286a 4701  nametypes.}.(jG.
-00001260: 0000 8968 e489 686c 8868 9e88 6a3f 0100  ...h..hl.h..j?..
-00001270: 0089 7568 217d 9428 6a44 0100 0068 0c68  ..uh!}.(jD...h.h
-00001280: e168 2d68 6968 6368 9b68 956a 3c01 0000  .h-hihch.h.j<...
-00001290: 68e7 758c 0d66 6f6f 746e 6f74 655f 7265  h.u..footnote_re
-000012a0: 6673 947d 948c 0d63 6974 6174 696f 6e5f  fs.}...citation_
-000012b0: 7265 6673 947d 948c 0d61 7574 6f66 6f6f  refs.}...autofoo
-000012c0: 746e 6f74 6573 945d 948c 1161 7574 6f66  tnotes.]...autof
-000012d0: 6f6f 746e 6f74 655f 7265 6673 945d 948c  ootnote_refs.]..
-000012e0: 1073 796d 626f 6c5f 666f 6f74 6e6f 7465  .symbol_footnote
-000012f0: 7394 5d94 8c14 7379 6d62 6f6c 5f66 6f6f  s.]...symbol_foo
-00001300: 746e 6f74 655f 7265 6673 945d 948c 0966  tnote_refs.]...f
-00001310: 6f6f 746e 6f74 6573 945d 948c 0963 6974  ootnotes.]...cit
-00001320: 6174 696f 6e73 945d 948c 1261 7574 6f66  ations.]...autof
-00001330: 6f6f 746e 6f74 655f 7374 6172 7494 4b01  ootnote_start.K.
-00001340: 8c15 7379 6d62 6f6c 5f66 6f6f 746e 6f74  ..symbol_footnot
-00001350: 655f 7374 6172 7494 4b00 8c0a 6964 5f63  e_start.K...id_c
-00001360: 6f75 6e74 6572 948c 0b63 6f6c 6c65 6374  ounter...collect
-00001370: 696f 6e73 948c 0743 6f75 6e74 6572 9493  ions...Counter..
-00001380: 947d 9485 9452 948c 0e70 6172 7365 5f6d  .}...R...parse_m
-00001390: 6573 7361 6765 7394 5d94 8c12 7472 616e  essages.]...tran
-000013a0: 7366 6f72 6d5f 6d65 7373 6167 6573 945d  sform_messages.]
-000013b0: 948c 0b74 7261 6e73 666f 726d 6572 944e  ...transformer.N
-000013c0: 8c0b 696e 636c 7564 655f 6c6f 6794 5d94  ..include_log.].
-000013d0: 8c0a 6465 636f 7261 7469 6f6e 944e 681c  ..decoration.Nh.
-000013e0: 6803 7562 2e                             h.ub.
+00000750: 9475 682b 685b 681d 682c 681e 4b0a 681b  .uh+h[h.h,h.K.h.
+00000760: 688f 7562 6168 1f7d 9428 6821 5d94 6823  h.ubah.}.(h!].h#
+00000770: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+00000780: 2b68 5568 1b68 5268 1c68 0368 1d68 2c68  +hUh.hRh.h.h.h,h
+00000790: 1e4e 7562 6568 1f7d 9428 6821 5d94 6823  .Nubeh.}.(h!].h#
+000007a0: 5d94 6825 5d94 6827 5d94 6829 5d94 8c06  ].h%].h'].h)]...
+000007b0: 6275 6c6c 6574 948c 012d 9475 682b 6850  bullet...-.uh+hP
+000007c0: 681d 682c 681e 4b09 681b 682d 681c 6803  h.h,h.K.h.h-h.h.
+000007d0: 7562 6809 8c08 636f 6d70 6f75 6e64 9493  ubh...compound..
+000007e0: 9429 8194 7d94 2868 0568 0668 075d 9468  .)..}.(h.h.h.].h
+000007f0: 008c 0774 6f63 7472 6565 9493 9429 8194  ...toctree...)..
+00000800: 7d94 2868 0568 0668 075d 9468 1f7d 9428  }.(h.h.h.].h.}.(
+00000810: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+00000820: 6829 5d94 681b 8c05 696e 6465 7894 8c07  h)].h...index...
+00000830: 656e 7472 6965 7394 5d94 4e8c 1163 6f6f  entries.].N..coo
+00000840: 6b69 6573 5f75 7469 6c69 7469 6573 9486  kies_utilities..
+00000850: 9461 8c0c 696e 636c 7564 6566 696c 6573  .a..includefiles
+00000860: 945d 9468 db61 8c08 6d61 7864 6570 7468  .].h.a..maxdepth
+00000870: 944b 028c 0763 6170 7469 6f6e 948c 0943  .K...caption...C
+00000880: 6f6e 7465 6e74 733a 948c 0467 6c6f 6294  ontents:...glob.
+00000890: 898c 0668 6964 6465 6e94 898c 0d69 6e63  ...hidden....inc
+000008a0: 6c75 6465 6869 6464 656e 9489 8c08 6e75  ludehidden....nu
+000008b0: 6d62 6572 6564 944b 008c 0a74 6974 6c65  mbered.K...title
+000008c0: 736f 6e6c 7994 898c 0a72 6177 656e 7472  sonly....rawentr
+000008d0: 6965 7394 5d94 8c0a 7261 7763 6170 7469  ies.]...rawcapti
+000008e0: 6f6e 9468 e175 682b 68cd 681d 682c 681e  on.h.uh+h.h.h,h.
+000008f0: 4b0c 681b 68ca 7562 6168 1f7d 9428 6821  K.h.h.ubah.}.(h!
+00000900: 5d94 6823 5d94 8c0f 746f 6374 7265 652d  ].h#]...toctree-
+00000910: 7772 6170 7065 7294 6168 255d 9468 275d  wrapper.ah%].h']
+00000920: 9468 295d 9475 682b 68c8 681b 682d 681c  .h)].uh+h.h.h-h.
+00000930: 6803 681d 682c 681e 4e75 6265 681f 7d94  h.h.h,h.Nubeh.}.
+00000940: 2868 215d 948c 056c 696e 6b73 9461 6823  (h!]...links.ah#
+00000950: 5d94 6825 5d94 8c05 6c69 6e6b 7394 6168  ].h%]...links.ah
+00000960: 275d 9468 295d 9475 682b 680a 681b 680c  '].h)].uh+h.h.h.
+00000970: 681c 6803 681d 682c 681e 4b05 7562 680b  h.h.h.h,h.K.ubh.
+00000980: 2981 947d 9428 6805 6806 6807 5d94 2868  )..}.(h.h.h.].(h
+00000990: 1029 8194 7d94 2868 058c 1249 6e64 6963  .)..}.(h...Indic
+000009a0: 6573 2061 6e64 2074 6162 6c65 7394 6807  es and tables.h.
+000009b0: 5d94 6816 8c12 496e 6469 6365 7320 616e  ].h...Indices an
+000009c0: 6420 7461 626c 6573 9485 9481 947d 9428  d tables.....}.(
+000009d0: 681b 68fc 681c 6803 681d 4e68 1e4e 7562  h.h.h.h.h.Nh.Nub
+000009e0: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+000009f0: 5d94 6827 5d94 6829 5d94 7568 2b68 0f68  ].h'].h)].uh+h.h
+00000a00: 1b68 f968 1c68 0368 1d68 2c68 1e4b 1375  .h.h.h.h.h,h.K.u
+00000a10: 6268 5129 8194 7d94 2868 0568 0668 075d  bhQ)..}.(h.h.h.]
+00000a20: 9468 5629 8194 7d94 2868 058c 0f3a 7265  .hV)..}.(h...:re
+00000a30: 663a 6067 656e 696e 6465 7860 9468 075d  f:`genindex`.h.]
+00000a40: 9468 5c29 8194 7d94 2868 056a 0f01 0000  .h\)..}.(h.j....
+00000a50: 6807 5d94 6800 8c0c 7065 6e64 696e 675f  h.].h...pending_
+00000a60: 7872 6566 9493 9429 8194 7d94 2868 056a  xref...)..}.(h.j
+00000a70: 0f01 0000 6807 5d94 6809 8c06 696e 6c69  ....h.].h...inli
+00000a80: 6e65 9493 9429 8194 7d94 2868 056a 0f01  ne...)..}.(h.j..
+00000a90: 0000 6807 5d94 6816 8c08 6765 6e69 6e64  ..h.].h...genind
+00000aa0: 6578 9485 9481 947d 9428 681b 6a1b 0100  ex.....}.(h.j...
+00000ab0: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
+00000ac0: 7d94 2868 215d 9468 235d 9428 8c04 7872  }.(h!].h#].(..xr
+00000ad0: 6566 948c 0373 7464 948c 0773 7464 2d72  ef...std...std-r
+00000ae0: 6566 9465 6825 5d94 6827 5d94 6829 5d94  ef.eh%].h'].h)].
+00000af0: 7568 2b6a 1901 0000 681b 6a16 0100 0075  uh+j....h.j....u
+00000b00: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+00000b10: 255d 9468 275d 9468 295d 948c 0672 6566  %].h'].h)]...ref
+00000b20: 646f 6394 68d8 8c09 7265 6664 6f6d 6169  doc.h...refdomai
+00000b30: 6e94 6a26 0100 008c 0772 6566 7479 7065  n.j&.....reftype
+00000b40: 948c 0372 6566 948c 0b72 6566 6578 706c  ...ref...refexpl
+00000b50: 6963 6974 9489 8c07 7265 6677 6172 6e94  icit....refwarn.
+00000b60: 888c 0972 6566 7461 7267 6574 948c 0867  ...reftarget...g
+00000b70: 656e 696e 6465 7894 7568 2b6a 1401 0000  enindex.uh+j....
+00000b80: 681d 682c 681e 4b15 681b 6a11 0100 0075  h.h,h.K.h.j....u
+00000b90: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+00000ba0: 255d 9468 275d 9468 295d 9475 682b 685b  %].h'].h)].uh+h[
+00000bb0: 681d 682c 681e 4b15 681b 6a0d 0100 0075  h.h,h.K.h.j....u
+00000bc0: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+00000bd0: 255d 9468 275d 9468 295d 9475 682b 6855  %].h'].h)].uh+hU
+00000be0: 681b 6a0a 0100 0068 1c68 0368 1d68 2c68  h.j....h.h.h.h,h
+00000bf0: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
+00000c00: 5d94 6825 5d94 6827 5d94 6829 5d94 68c6  ].h%].h'].h)].h.
+00000c10: 8c01 2a94 7568 2b68 5068 1d68 2c68 1e4b  ..*.uh+hPh.h,h.K
+00000c20: 1568 1b68 f968 1c68 0375 6265 681f 7d94  .h.h.h.h.ubeh.}.
+00000c30: 2868 215d 948c 1269 6e64 6963 6573 2d61  (h!]...indices-a
+00000c40: 6e64 2d74 6162 6c65 7394 6168 235d 9468  nd-tables.ah#].h
+00000c50: 255d 948c 1269 6e64 6963 6573 2061 6e64  %]...indices and
+00000c60: 2074 6162 6c65 7394 6168 275d 9468 295d   tables.ah'].h)]
+00000c70: 9475 682b 680a 681b 680c 681c 6803 681d  .uh+h.h.h.h.h.h.
+00000c80: 682c 681e 4b13 7562 6568 1f7d 9428 6821  h,h.K.ubeh.}.(h!
+00000c90: 5d94 8c2a 7765 6c63 6f6d 652d 746f 2d63  ]..*welcome-to-c
+00000ca0: 6f6f 6b69 6573 2d75 7469 6c69 7469 6573  ookies-utilities
+00000cb0: 2d64 6f63 756d 656e 7461 7469 6f6e 9461  -documentation.a
+00000cc0: 6823 5d94 6825 5d94 8c2c 7765 6c63 6f6d  h#].h%]..,welcom
+00000cd0: 6520 746f 2063 6f6f 6b69 6573 5f75 7469  e to cookies_uti
+00000ce0: 6c69 7469 6573 2720 646f 6375 6d65 6e74  lities' document
+00000cf0: 6174 696f 6e21 9461 6827 5d94 6829 5d94  ation!.ah'].h)].
+00000d00: 7568 2b68 0a68 1b68 0368 1c68 0368 1d68  uh+h.h.h.h.h.h.h
+00000d10: 2c68 1e4b 0275 6261 681f 7d94 2868 215d  ,h.K.ubah.}.(h!]
+00000d20: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+00000d30: 948c 0673 6f75 7263 6594 682c 7568 2b68  ...source.h,uh+h
+00000d40: 018c 0e63 7572 7265 6e74 5f73 6f75 7263  ...current_sourc
+00000d50: 6594 4e8c 0c63 7572 7265 6e74 5f6c 696e  e.N..current_lin
+00000d60: 6594 4e8c 0873 6574 7469 6e67 7394 8c11  e.N..settings...
+00000d70: 646f 6375 7469 6c73 2e66 726f 6e74 656e  docutils.fronten
+00000d80: 6494 8c06 5661 6c75 6573 9493 9429 8194  d...Values...)..
+00000d90: 7d94 2868 0f4e 8c09 6765 6e65 7261 746f  }.(h.N..generato
+00000da0: 7294 4e8c 0964 6174 6573 7461 6d70 944e  r.N..datestamp.N
+00000db0: 8c0b 736f 7572 6365 5f6c 696e 6b94 4e8c  ..source_link.N.
+00000dc0: 0a73 6f75 7263 655f 7572 6c94 4e8c 0d74  .source_url.N..t
+00000dd0: 6f63 5f62 6163 6b6c 696e 6b73 948c 0565  oc_backlinks...e
+00000de0: 6e74 7279 948c 1266 6f6f 746e 6f74 655f  ntry...footnote_
+00000df0: 6261 636b 6c69 6e6b 7394 4b01 8c0d 7365  backlinks.K...se
+00000e00: 6374 6e75 6d5f 7866 6f72 6d94 4b01 8c0e  ctnum_xform.K...
+00000e10: 7374 7269 705f 636f 6d6d 656e 7473 944e  strip_comments.N
+00000e20: 8c1b 7374 7269 705f 656c 656d 656e 7473  ..strip_elements
+00000e30: 5f77 6974 685f 636c 6173 7365 7394 4e8c  _with_classes.N.
+00000e40: 0d73 7472 6970 5f63 6c61 7373 6573 944e  .strip_classes.N
+00000e50: 8c0c 7265 706f 7274 5f6c 6576 656c 944b  ..report_level.K
+00000e60: 028c 0a68 616c 745f 6c65 7665 6c94 4b05  ...halt_level.K.
+00000e70: 8c11 6578 6974 5f73 7461 7475 735f 6c65  ..exit_status_le
+00000e80: 7665 6c94 4b05 8c05 6465 6275 6794 4e8c  vel.K...debug.N.
+00000e90: 0e77 6172 6e69 6e67 5f73 7472 6561 6d94  .warning_stream.
+00000ea0: 4e8c 0974 7261 6365 6261 636b 9488 8c0e  N..traceback....
+00000eb0: 696e 7075 745f 656e 636f 6469 6e67 948c  input_encoding..
+00000ec0: 0975 7466 2d38 2d73 6967 948c 1c69 6e70  .utf-8-sig...inp
+00000ed0: 7574 5f65 6e63 6f64 696e 675f 6572 726f  ut_encoding_erro
+00000ee0: 725f 6861 6e64 6c65 7294 8c06 7374 7269  r_handler...stri
+00000ef0: 6374 948c 0f6f 7574 7075 745f 656e 636f  ct...output_enco
+00000f00: 6469 6e67 948c 0575 7466 2d38 948c 1d6f  ding...utf-8...o
+00000f10: 7574 7075 745f 656e 636f 6469 6e67 5f65  utput_encoding_e
+00000f20: 7272 6f72 5f68 616e 646c 6572 946a 7f01  rror_handler.j..
+00000f30: 0000 8c0e 6572 726f 725f 656e 636f 6469  ....error_encodi
+00000f40: 6e67 948c 0575 7466 2d38 948c 1c65 7272  ng...utf-8...err
+00000f50: 6f72 5f65 6e63 6f64 696e 675f 6572 726f  or_encoding_erro
+00000f60: 725f 6861 6e64 6c65 7294 8c10 6261 636b  r_handler...back
+00000f70: 736c 6173 6872 6570 6c61 6365 948c 0d6c  slashreplace...l
+00000f80: 616e 6775 6167 655f 636f 6465 948c 0265  anguage_code...e
+00000f90: 6e94 8c13 7265 636f 7264 5f64 6570 656e  n...record_depen
+00000fa0: 6465 6e63 6965 7394 4e8c 0663 6f6e 6669  dencies.N..confi
+00000fb0: 6794 4e8c 0969 645f 7072 6566 6978 9468  g.N..id_prefix.h
+00000fc0: 068c 0e61 7574 6f5f 6964 5f70 7265 6669  ...auto_id_prefi
+00000fd0: 7894 8c02 6964 948c 0d64 756d 705f 7365  x...id...dump_se
+00000fe0: 7474 696e 6773 944e 8c0e 6475 6d70 5f69  ttings.N..dump_i
+00000ff0: 6e74 6572 6e61 6c73 944e 8c0f 6475 6d70  nternals.N..dump
+00001000: 5f74 7261 6e73 666f 726d 7394 4e8c 0f64  _transforms.N..d
+00001010: 756d 705f 7073 6575 646f 5f78 6d6c 944e  ump_pseudo_xml.N
+00001020: 8c10 6578 706f 7365 5f69 6e74 6572 6e61  ..expose_interna
+00001030: 6c73 944e 8c0e 7374 7269 6374 5f76 6973  ls.N..strict_vis
+00001040: 6974 6f72 944e 8c0f 5f64 6973 6162 6c65  itor.N.._disable
+00001050: 5f63 6f6e 6669 6794 4e8c 075f 736f 7572  _config.N.._sour
+00001060: 6365 9468 2c8c 0c5f 6465 7374 696e 6174  ce.h,.._destinat
+00001070: 696f 6e94 4e8c 0d5f 636f 6e66 6967 5f66  ion.N.._config_f
+00001080: 696c 6573 945d 948c 1666 696c 655f 696e  iles.]...file_in
+00001090: 7365 7274 696f 6e5f 656e 6162 6c65 6494  sertion_enabled.
+000010a0: 888c 0b72 6177 5f65 6e61 626c 6564 944b  ...raw_enabled.K
+000010b0: 018c 116c 696e 655f 6c65 6e67 7468 5f6c  ...line_length_l
+000010c0: 696d 6974 944d 1027 8c0e 7065 705f 7265  imit.M.'..pep_re
+000010d0: 6665 7265 6e63 6573 944e 8c0c 7065 705f  ferences.N..pep_
+000010e0: 6261 7365 5f75 726c 948c 1868 7474 7073  base_url...https
+000010f0: 3a2f 2f70 6570 732e 7079 7468 6f6e 2e6f  ://peps.python.o
+00001100: 7267 2f94 8c15 7065 705f 6669 6c65 5f75  rg/...pep_file_u
+00001110: 726c 5f74 656d 706c 6174 6594 8c08 7065  rl_template...pe
+00001120: 702d 2530 3464 948c 0e72 6663 5f72 6566  p-%04d...rfc_ref
+00001130: 6572 656e 6365 7394 4e8c 0c72 6663 5f62  erences.N..rfc_b
+00001140: 6173 655f 7572 6c94 8c26 6874 7470 733a  ase_url..&https:
+00001150: 2f2f 6461 7461 7472 6163 6b65 722e 6965  //datatracker.ie
+00001160: 7466 2e6f 7267 2f64 6f63 2f68 746d 6c2f  tf.org/doc/html/
+00001170: 948c 0974 6162 5f77 6964 7468 944b 088c  ...tab_width.K..
+00001180: 1d74 7269 6d5f 666f 6f74 6e6f 7465 5f72  .trim_footnote_r
+00001190: 6566 6572 656e 6365 5f73 7061 6365 9489  eference_space..
+000011a0: 8c10 7379 6e74 6178 5f68 6967 686c 6967  ..syntax_highlig
+000011b0: 6874 948c 046c 6f6e 6794 8c0c 736d 6172  ht...long...smar
+000011c0: 745f 7175 6f74 6573 9488 8c13 736d 6172  t_quotes....smar
+000011d0: 7471 756f 7465 735f 6c6f 6361 6c65 7394  tquotes_locales.
+000011e0: 5d94 8c1d 6368 6172 6163 7465 725f 6c65  ]...character_le
+000011f0: 7665 6c5f 696e 6c69 6e65 5f6d 6172 6b75  vel_inline_marku
+00001200: 7094 898c 0e64 6f63 7469 746c 655f 7866  p....doctitle_xf
+00001210: 6f72 6d94 898c 0d64 6f63 696e 666f 5f78  orm....docinfo_x
+00001220: 666f 726d 944b 018c 1273 6563 7473 7562  form.K...sectsub
+00001230: 7469 746c 655f 7866 6f72 6d94 898c 0d69  title_xform....i
+00001240: 6d61 6765 5f6c 6f61 6469 6e67 948c 046c  mage_loading...l
+00001250: 696e 6b94 8c10 656d 6265 645f 7374 796c  ink...embed_styl
+00001260: 6573 6865 6574 9489 8c15 636c 6f61 6b5f  esheet....cloak_
+00001270: 656d 6169 6c5f 6164 6472 6573 7365 7394  email_addresses.
+00001280: 888c 1173 6563 7469 6f6e 5f73 656c 665f  ...section_self_
+00001290: 6c69 6e6b 9489 8c03 656e 7694 4e75 628c  link....env.Nub.
+000012a0: 0872 6570 6f72 7465 7294 4e8c 1069 6e64  .reporter.N..ind
+000012b0: 6972 6563 745f 7461 7267 6574 7394 5d94  irect_targets.].
+000012c0: 8c11 7375 6273 7469 7475 7469 6f6e 5f64  ..substitution_d
+000012d0: 6566 7394 7d94 8c12 7375 6273 7469 7475  efs.}...substitu
+000012e0: 7469 6f6e 5f6e 616d 6573 947d 948c 0872  tion_names.}...r
+000012f0: 6566 6e61 6d65 7394 7d94 8c06 7265 6669  efnames.}...refi
+00001300: 6473 947d 948c 076e 616d 6569 6473 947d  ds.}...nameids.}
+00001310: 9428 6a59 0100 006a 5601 0000 68f6 68f3  .(jY...jV...h.h.
+00001320: 687e 687b 68b0 68ad 6a51 0100 006a 4e01  h~h{h.h.jQ...jN.
+00001330: 0000 758c 096e 616d 6574 7970 6573 947d  ..u..nametypes.}
+00001340: 9428 6a59 0100 0089 68f6 8968 7e88 68b0  .(jY....h..h~.h.
+00001350: 886a 5101 0000 8975 6821 7d94 286a 5601  .jQ....uh!}.(jV.
+00001360: 0000 680c 68f3 682d 687b 6875 68ad 68a7  ..h.h.h-h{huh.h.
+00001370: 6a4e 0100 0068 f975 8c0d 666f 6f74 6e6f  jN...h.u..footno
+00001380: 7465 5f72 6566 7394 7d94 8c0d 6369 7461  te_refs.}...cita
+00001390: 7469 6f6e 5f72 6566 7394 7d94 8c0d 6175  tion_refs.}...au
+000013a0: 746f 666f 6f74 6e6f 7465 7394 5d94 8c11  tofootnotes.]...
+000013b0: 6175 746f 666f 6f74 6e6f 7465 5f72 6566  autofootnote_ref
+000013c0: 7394 5d94 8c10 7379 6d62 6f6c 5f66 6f6f  s.]...symbol_foo
+000013d0: 746e 6f74 6573 945d 948c 1473 796d 626f  tnotes.]...symbo
+000013e0: 6c5f 666f 6f74 6e6f 7465 5f72 6566 7394  l_footnote_refs.
+000013f0: 5d94 8c09 666f 6f74 6e6f 7465 7394 5d94  ]...footnotes.].
+00001400: 8c09 6369 7461 7469 6f6e 7394 5d94 8c12  ..citations.]...
+00001410: 6175 746f 666f 6f74 6e6f 7465 5f73 7461  autofootnote_sta
+00001420: 7274 944b 018c 1573 796d 626f 6c5f 666f  rt.K...symbol_fo
+00001430: 6f74 6e6f 7465 5f73 7461 7274 944b 008c  otnote_start.K..
+00001440: 0a69 645f 636f 756e 7465 7294 8c0b 636f  .id_counter...co
+00001450: 6c6c 6563 7469 6f6e 7394 8c07 436f 756e  llections...Coun
+00001460: 7465 7294 9394 7d94 8594 5294 8c0e 7061  ter...}...R...pa
+00001470: 7273 655f 6d65 7373 6167 6573 945d 948c  rse_messages.]..
+00001480: 1274 7261 6e73 666f 726d 5f6d 6573 7361  .transform_messa
+00001490: 6765 7394 5d94 8c0b 7472 616e 7366 6f72  ges.]...transfor
+000014a0: 6d65 7294 4e8c 0b69 6e63 6c75 6465 5f6c  mer.N..include_l
+000014b0: 6f67 945d 948c 0a64 6563 6f72 6174 696f  og.]...decoratio
+000014c0: 6e94 4e68 1c68 0375 622e                 n.Nh.h.ub.
```

### Comparing `cookies_utilities-0.0.1/docs/build/doctrees/modules.doctree` & `cookies_utilities-0.0.2/docs/build/doctrees/modules.doctree`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/genindex.html` & `cookies_utilities-0.0.2/docs/build/html/genindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Index &mdash; cookies_utilities 0.0.4 documentation</title>
+  <title>Index &mdash; cookies_utilities 0.0.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script src="_static/jquery.js"></script>
```

### Comparing `cookies_utilities-0.0.1/docs/build/html/index.html` & `cookies_utilities-0.0.2/docs/build/html/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Welcome to cookies_utilities’ documentation! &mdash; cookies_utilities 0.0.4 documentation</title>
+  <title>Welcome to cookies_utilities’ documentation! &mdash; cookies_utilities 0.0.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script src="_static/jquery.js"></script>
@@ -71,15 +71,15 @@
            <div itemprop="articleBody">
              
   <section id="welcome-to-cookies-utilities-documentation">
 <h1>Welcome to cookies_utilities’ documentation!<a class="headerlink" href="#welcome-to-cookies-utilities-documentation" title="Permalink to this heading"></a></h1>
 <section id="links">
 <h2>Links<a class="headerlink" href="#links" title="Permalink to this heading"></a></h2>
 <ul class="simple">
-<li><p><a class="reference external" href="https://test.pypi.org/project/cookies-utilities/">TestPyPI</a></p></li>
+<li><p><a class="reference external" href="https://pypi.org/project/cookies-utilities/">PyPI</a></p></li>
 <li><p><a class="reference external" href="https://github.com/CookieBox26/cookies_utilities">GitHub</a></p></li>
 </ul>
 <div class="toctree-wrapper compound">
 <p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="cookies_utilities.html">Documentation</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="cookies_utilities.html#functions">Functions</a></li>
```

#### html2text {}

```diff
@@ -10,15 +10,15 @@
     * Documentation
    cookies_utilities
     * Welcome to cookies_utilitiesâ documentation!
     * View_page_source
 ===============================================================================
 ****** Welcome to cookies_utilitiesâ documentation!ï ******
 ***** Linksï *****
-    * TestPyPI
+    * PyPI
     * GitHub
 Contents:
     * Documentation
           o Functions
           o Classes
 
 ***** Indices and tablesï *****
```

### Comparing `cookies_utilities-0.0.1/docs/build/html/modules.html` & `cookies_utilities-0.0.2/docs/build/html/modules.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>cookies_utilities &mdash; cookies_utilities 0.0.4 documentation</title>
+  <title>cookies_utilities &mdash; cookies_utilities 0.0.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script src="_static/jquery.js"></script>
```

### Comparing `cookies_utilities-0.0.1/docs/build/html/search.html` & `cookies_utilities-0.0.2/docs/build/html/search.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Search &mdash; cookies_utilities 0.0.4 documentation</title>
+  <title>Search &mdash; cookies_utilities 0.0.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
     
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
```

### Comparing `cookies_utilities-0.0.1/docs/build/html/searchindex.js` & `cookies_utilities-0.0.2/docs/build/html/searchindex.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -68,18 +68,18 @@
         "rtype": [],
         "type": 0,
         "bool": 0,
         "whether": 0,
         "convert": 0,
         "output": 0,
         "same": 0,
-        "testpypi": 1,
+        "testpypi": [],
         "http": [],
         "test": 0,
-        "pypi": [],
+        "pypi": 1,
         "org": [],
         "project": [],
         "cooki": [],
         "util": [],
         "github": 1,
         "com": [],
         "cookiebox26": [],
@@ -92,15 +92,35 @@
         "time1": 0,
         "000": 0,
         "time2": 0,
         "total": 0,
         "2": 0,
         "3": 0,
         "usag": [],
-        "exampl": 0
+        "exampl": 0,
+        "inclus": 0,
+        "genit": 0,
+        "fals": 0,
+        "If": 0,
+        "you": 0,
+        "re": 0,
+        "us": 0,
+        "result": 0,
+        "an": 0,
+        "iter": 0,
+        "i": 0,
+        "recommend": 0,
+        "set": 0,
+        "gener": 0,
+        "04": [],
+        "20": 0,
+        "print": 0,
+        "40": 0,
+        "one": 0,
+        "retriev": 0
     },
     "objects": {
         "cookies_utilities": [
             [0, 0, 1, "", "Stopwatch"],
             [0, 2, 1, "", "get_dates"]
         ],
         "cookies_utilities.Stopwatch": [
@@ -145,29 +165,29 @@
         "sphinx.domains.math": 2,
         "sphinx.domains.python": 3,
         "sphinx.domains.rst": 2,
         "sphinx.domains.std": 2,
         "sphinx": 57
     },
     "alltitles": {
-        "cookies_utilities": [
-            [2, "cookies-utilities"]
-        ],
         "Welcome to cookies_utilities\u2019 documentation!": [
             [1, "welcome-to-cookies-utilities-documentation"]
         ],
         "Links": [
             [1, "links"]
         ],
         "Contents:": [
             [1, null]
         ],
         "Indices and tables": [
             [1, "indices-and-tables"]
         ],
+        "cookies_utilities": [
+            [2, "cookies-utilities"]
+        ],
         "Documentation": [
             [0, "documentation"]
         ],
         "Functions": [
             [0, "functions"]
         ],
         "cookies_utilities.get_dates": [
```

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js` & `cookies_utilities-0.0.2/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/basic.css` & `cookies_utilities-0.0.2/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/doctools.js` & `cookies_utilities-0.0.2/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/jquery.js` & `cookies_utilities-0.0.2/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/language_data.js` & `cookies_utilities-0.0.2/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/pygments.css` & `cookies_utilities-0.0.2/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/searchtools.js` & `cookies_utilities-0.0.2/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/sphinx_highlight.js` & `cookies_utilities-0.0.2/docs/build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/css/badge_only.css` & `cookies_utilities-0.0.2/docs/build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/css/theme.css` & `cookies_utilities-0.0.2/docs/build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/fontawesome-webfont.eot` & `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/fontawesome-webfont.svg` & `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf` & `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/fontawesome-webfont.woff` & `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2` & `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/lato-bold-italic.woff` & `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/lato-bold-italic.woff2` & `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/lato-bold.woff` & `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/lato-bold.woff2` & `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/lato-normal-italic.woff` & `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/lato-normal-italic.woff2` & `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/lato-normal.woff` & `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/css/fonts/lato-normal.woff2` & `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/js/badge_only.js` & `cookies_utilities-0.0.2/docs/build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/js/html5shiv-printshiv.min.js` & `cookies_utilities-0.0.2/docs/build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/js/html5shiv.min.js` & `cookies_utilities-0.0.2/docs/build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/build/html/_static/js/theme.js` & `cookies_utilities-0.0.2/docs/build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/docs/source/conf.py` & `cookies_utilities-0.0.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/src/cookies_utilities/stopwatch.py` & `cookies_utilities-0.0.2/src/cookies_utilities/stopwatch.py`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/LICENSE` & `cookies_utilities-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.1/README.md` & `cookies_utilities-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Cookie's Utilities
 
 Utility functions and classes.
 
-- [TestPyPI](https://test.pypi.org/project/cookies-utilities/)
-- [Documentation](https://cookies-utilities.readthedocs.io/en/latest/index.html)
+<!-- - [TestPyPI](https://test.pypi.org/project/cookies-utilities/) -->
+<!-- - [PyPI](https://pypi.org/project/cookies-utilities/) -->
+- [Documentation (released)](https://cookies-utilities.readthedocs.io/en/stable/)
+- [Documentation (main branch HEAD)](https://cookies-utilities.readthedocs.io/en/latest/)
 
 ---
 
 ### Development Guide
 
 Please execute the following at the root of the repository.
 
@@ -45,16 +47,17 @@
 The following files will be generated.
 
 ```
 ./dist/cookies_utilities-0.0.1.tar.gz
 ./dist/cookies_utilities-0.0.1-py3-none-any.whl
 ```
 
-#### Upload the distribution archives to TestPyPI
+#### Upload the distribution archives to TestPyPI (PyPI)
 
 Please run the following commands. More details are [here](https://packaging.python.org/en/latest/tutorials/packaging-projects/#uploading-the-distribution-archives).
 
 ```
 pip install --upgrade twine
-python -m twine upload --repository testpypi dist/*
+python -m twine upload --repository testpypi dist/*  # TestPyPI
+python -m twine upload dist/*  # PyPI
 ```
```

### Comparing `cookies_utilities-0.0.1/pyproject.toml` & `cookies_utilities-0.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cookies_utilities"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="CookieBox26", email="cookie-box@cookie-box.info" },
 ]
 description = "Utility functions."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 GitHub = "https://github.com/CookieBox26/cookies_utilities"
-Documentation = "https://cookies-utilities.readthedocs.io/en/latest/index.html"
+Documentation = "https://cookies-utilities.readthedocs.io/en/stable/"
```

### Comparing `cookies_utilities-0.0.1/PKG-INFO` & `cookies_utilities-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: cookies_utilities
-Version: 0.0.1
+Version: 0.0.2
 Summary: Utility functions.
 Project-URL: GitHub, https://github.com/CookieBox26/cookies_utilities
-Project-URL: Documentation, https://cookies-utilities.readthedocs.io/en/latest/index.html
+Project-URL: Documentation, https://cookies-utilities.readthedocs.io/en/stable/
 Author-email: CookieBox26 <cookie-box@cookie-box.info>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Cookie's Utilities
 
 Utility functions and classes.
 
-- [TestPyPI](https://test.pypi.org/project/cookies-utilities/)
-- [Documentation](https://cookies-utilities.readthedocs.io/en/latest/index.html)
+<!-- - [TestPyPI](https://test.pypi.org/project/cookies-utilities/) -->
+<!-- - [PyPI](https://pypi.org/project/cookies-utilities/) -->
+- [Documentation (released)](https://cookies-utilities.readthedocs.io/en/stable/)
+- [Documentation (main branch HEAD)](https://cookies-utilities.readthedocs.io/en/latest/)
 
 ---
 
 ### Development Guide
 
 Please execute the following at the root of the repository.
 
@@ -59,16 +61,17 @@
 The following files will be generated.
 
 ```
 ./dist/cookies_utilities-0.0.1.tar.gz
 ./dist/cookies_utilities-0.0.1-py3-none-any.whl
 ```
 
-#### Upload the distribution archives to TestPyPI
+#### Upload the distribution archives to TestPyPI (PyPI)
 
 Please run the following commands. More details are [here](https://packaging.python.org/en/latest/tutorials/packaging-projects/#uploading-the-distribution-archives).
 
 ```
 pip install --upgrade twine
-python -m twine upload --repository testpypi dist/*
+python -m twine upload --repository testpypi dist/*  # TestPyPI
+python -m twine upload dist/*  # PyPI
 ```
```

