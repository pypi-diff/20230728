# Comparing `tmp/xarg-python-0.6.tar.gz` & `tmp/xarg-python-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xarg-python-0.6.tar", last modified: Mon May 15 09:16:17 2023, max compression
+gzip compressed data, was "xarg-python-0.7.tar", last modified: Fri Jul 28 05:40:58 2023, max compression
```

## Comparing `xarg-python-0.6.tar` & `xarg-python-0.7.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 09:16:17.000000 xarg-python-0.6/
--rw-rw-rw-   0        0        0      769 2023-05-15 09:16:17.000000 xarg-python-0.6/PKG-INFO
--rw-rw-rw-   0        0        0       55 2023-03-20 02:44:39.000000 xarg-python-0.6/README.md
--rw-rw-rw-   0        0        0      997 2023-05-15 09:16:17.000000 xarg-python-0.6/setup.cfg
--rw-rw-rw-   0        0        0       72 2023-05-15 02:35:00.000000 xarg-python-0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:16:17.000000 xarg-python-0.6/xarg/
--rw-rw-rw-   0        0        0     1622 2023-05-15 09:11:26.000000 xarg-python-0.6/xarg/xarg_checker.py
--rw-rw-rw-   0        0        0     2564 2023-05-15 09:13:32.000000 xarg-python-0.6/xarg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:16:17.000000 xarg-python-0.6/xarg_python.egg-info/
--rw-rw-rw-   0        0        0        1 2023-05-15 09:16:17.000000 xarg-python-0.6/xarg_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-15 09:16:17.000000 xarg-python-0.6/xarg_python.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      769 2023-05-15 09:16:17.000000 xarg-python-0.6/xarg_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2023-05-15 09:16:17.000000 xarg-python-0.6/xarg_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        5 2023-05-15 09:16:17.000000 xarg-python-0.6/xarg_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-15 09:16:17.000000 xarg-python-0.6/xarg_python.egg-info/zip-safe
+drwxrwxrwx   0 zou       (1000) zou       (1000)        0 2023-07-28 05:40:58.200827 xarg-python-0.7/
+-rwxrwxrwx   0 zou       (1000) zou       (1000)     1084 2023-03-20 02:44:39.000000 xarg-python-0.7/LICENSE
+-rwxrwxrwx   0 zou       (1000) zou       (1000)      838 2023-07-28 05:40:58.204338 xarg-python-0.7/PKG-INFO
+-rwxrwxrwx   0 zou       (1000) zou       (1000)      169 2023-07-26 08:37:12.000000 xarg-python-0.7/README.md
+-rwxrwxrwx   0 zou       (1000) zou       (1000)      957 2023-07-28 05:40:58.221382 xarg-python-0.7/setup.cfg
+-rwxrwxrwx   0 zou       (1000) zou       (1000)       72 2023-05-15 02:35:00.000000 xarg-python-0.7/setup.py
+drwxrwxrwx   0 zou       (1000) zou       (1000)        0 2023-07-28 05:40:57.732345 xarg-python-0.7/xarg/
+-rwxrwxrwx   0 zou       (1000) zou       (1000)      236 2023-07-26 06:35:52.000000 xarg-python-0.7/xarg/__init__.py
+-rwxrwxrwx   0 zou       (1000) zou       (1000)     1570 2023-07-25 09:06:50.000000 xarg-python-0.7/xarg/checker.py
+-rwxrwxrwx   0 zou       (1000) zou       (1000)     3303 2023-07-27 13:44:03.000000 xarg-python-0.7/xarg/decorator.py
+-rwxrwxrwx   0 zou       (1000) zou       (1000)     2476 2023-07-26 06:32:34.000000 xarg-python-0.7/xarg/parser.py
+drwxrwxrwx   0 zou       (1000) zou       (1000)        0 2023-07-28 05:40:58.139736 xarg-python-0.7/xarg_python.egg-info/
+-rwxrwxrwx   0 zou       (1000) zou       (1000)      838 2023-07-28 05:40:56.000000 xarg-python-0.7/xarg_python.egg-info/PKG-INFO
+-rwxrwxrwx   0 zou       (1000) zou       (1000)      310 2023-07-28 05:40:57.000000 xarg-python-0.7/xarg_python.egg-info/SOURCES.txt
+-rwxrwxrwx   0 zou       (1000) zou       (1000)        1 2023-07-28 05:40:56.000000 xarg-python-0.7/xarg_python.egg-info/dependency_links.txt
+-rwxrwxrwx   0 zou       (1000) zou       (1000)       43 2023-07-28 05:40:56.000000 xarg-python-0.7/xarg_python.egg-info/entry_points.txt
+-rwxrwxrwx   0 zou       (1000) zou       (1000)        5 2023-07-28 05:40:56.000000 xarg-python-0.7/xarg_python.egg-info/top_level.txt
+-rwxrwxrwx   0 zou       (1000) zou       (1000)        2 2023-05-15 09:16:17.000000 xarg-python-0.7/xarg_python.egg-info/zip-safe
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `xarg-python-0.6/PKG-INFO` & `xarg-python-0.7/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,31 @@
-Metadata-Version: 2.1
-Name: xarg-python
-Version: 0.6
-Summary: Simple command-line tool based on argparse.
-Home-page: https://github.com/zoumingzhe/xarg-python
-Author: mingzhe
-Author-email: zoumingzhe@qq.com
-License: MIT
-Project-URL: Source Code, https://github.com/zoumingzhe/xarg-python
-Project-URL: Bug Tracker, https://github.com/zoumingzhe/xarg-python/issues
-Project-URL: Documentation, https://github.com/zoumingzhe/xarg-python
-Description: xarg
-        ====
-        
-        Simple command-line tool based on argparse.
-        
-Keywords: command,command-line,argparse,xarg
-Platform: any
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: xarg-python
+Version: 0.7
+Summary: Simple command-line tool based on argparse.
+Home-page: https://github.com/zoumingzhe/xarg-python
+Author: mingzhe
+Author-email: zoumingzhe@qq.com
+License: MIT
+Project-URL: Source Code, https://github.com/zoumingzhe/xarg-python
+Project-URL: Bug Tracker, https://github.com/zoumingzhe/xarg-python/issues
+Project-URL: Documentation, https://github.com/zoumingzhe/xarg-python
+Keywords: command,command-line,argparse,xarg
+Platform: any
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+xarg
+====
+
+Simple command-line tool based on argparse.
+
+build
+-----
+
+```shell
+rm -rf "build" "dist" "*.egg-info"
+python setup.py check sdist bdist_wheel --universal
+```
```

### Comparing `xarg-python-0.6/setup.cfg` & `xarg-python-0.7/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,60 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2078 6172 672d 7079 7468 6f6e 0d0a   = xarg-python..
-00000020: 7665 7273 696f 6e20 3d20 6174 7472 3a20  version = attr: 
-00000030: 7861 7267 2e5f 5f76 6572 7369 6f6e 5f5f  xarg.__version__
-00000040: 0d0a 6b65 7977 6f72 6473 203d 2063 6f6d  ..keywords = com
-00000050: 6d61 6e64 2c20 636f 6d6d 616e 642d 6c69  mand, command-li
-00000060: 6e65 2c20 6172 6770 6172 7365 2c20 7861  ne, argparse, xa
-00000070: 7267 0d0a 6465 7363 7269 7074 696f 6e20  rg..description 
-00000080: 3d20 5369 6d70 6c65 2063 6f6d 6d61 6e64  = Simple command
-00000090: 2d6c 696e 6520 746f 6f6c 2062 6173 6564  -line tool based
-000000a0: 206f 6e20 6172 6770 6172 7365 2e0d 0a61   on argparse...a
-000000b0: 7574 686f 7220 3d20 6d69 6e67 7a68 650d  uthor = mingzhe.
-000000c0: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
-000000d0: 7a6f 756d 696e 677a 6865 4071 712e 636f  zoumingzhe@qq.co
-000000e0: 6d0d 0a75 726c 203d 2068 7474 7073 3a2f  m..url = https:/
-000000f0: 2f67 6974 6875 622e 636f 6d2f 7a6f 756d  /github.com/zoum
-00000100: 696e 677a 6865 2f78 6172 672d 7079 7468  ingzhe/xarg-pyth
-00000110: 6f6e 0d0a 6c6f 6e67 5f64 6573 6372 6970  on..long_descrip
-00000120: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
-00000130: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
-00000140: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
-00000150: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
-00000160: 6b64 6f77 6e0d 0a6c 6963 656e 7365 203d  kdown..license =
-00000170: 204d 4954 0d0a 6c69 6365 6e73 655f 6669   MIT..license_fi
-00000180: 6c65 7320 3d20 4c49 4345 4e53 450d 0a70  les = LICENSE..p
-00000190: 6c61 7466 6f72 6d73 203d 2061 6e79 0d0a  latforms = any..
-000001a0: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
-000001b0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-000001c0: 6775 6167 6520 3a3a 2050 7974 686f 6e0d  guage :: Python.
-000001d0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-000001e0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000001f0: 203a 3a20 330d 0a70 726f 6a65 6374 5f75   :: 3..project_u
-00000200: 726c 7320 3d20 0d0a 0953 6f75 7263 6520  rls = ...Source 
-00000210: 436f 6465 203d 2068 7474 7073 3a2f 2f67  Code = https://g
-00000220: 6974 6875 622e 636f 6d2f 7a6f 756d 696e  ithub.com/zoumin
-00000230: 677a 6865 2f78 6172 672d 7079 7468 6f6e  gzhe/xarg-python
-00000240: 0d0a 0942 7567 2054 7261 636b 6572 203d  ...Bug Tracker =
-00000250: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000260: 636f 6d2f 7a6f 756d 696e 677a 6865 2f78  com/zoumingzhe/x
-00000270: 6172 672d 7079 7468 6f6e 2f69 7373 7565  arg-python/issue
-00000280: 730d 0a09 446f 6375 6d65 6e74 6174 696f  s...Documentatio
-00000290: 6e20 3d20 6874 7470 733a 2f2f 6769 7468  n = https://gith
-000002a0: 7562 2e63 6f6d 2f7a 6f75 6d69 6e67 7a68  ub.com/zoumingzh
-000002b0: 652f 7861 7267 2d70 7974 686f 6e0d 0a0d  e/xarg-python...
-000002c0: 0a5b 6f70 7469 6f6e 735d 0d0a 7a69 705f  .[options]..zip_
-000002d0: 7361 6665 203d 2054 7275 650d 0a69 6e63  safe = True..inc
-000002e0: 6c75 6465 5f70 6163 6b61 6765 5f64 6174  lude_package_dat
-000002f0: 6120 3d20 5472 7565 0d0a 7079 7468 6f6e  a = True..python
-00000300: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
-00000310: 360d 0a70 6163 6b61 6765 7320 3d20 6669  6..packages = fi
-00000320: 6e64 3a0d 0a0d 0a5b 6f70 7469 6f6e 732e  nd:....[options.
-00000330: 656e 7472 795f 706f 696e 7473 5d0d 0a63  entry_points]..c
-00000340: 6f6e 736f 6c65 5f73 6372 6970 7473 203d  onsole_scripts =
-00000350: 200d 0a09 7861 7267 203d 2078 6172 672e   ...xarg = xarg.
-00000360: 6578 616d 706c 653a 6d61 696e 0d0a 0d0a  example:main....
-00000370: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
-00000380: 732e 6669 6e64 5d0d 0a77 6865 7265 203d  s.find]..where =
-00000390: 202e 0d0a 696e 636c 7564 6520 3d20 7861   ...include = xa
-000003a0: 7267 0d0a 6578 636c 7564 6520 3d20 7861  rg..exclude = xa
-000003b0: 7267 2e74 6573 740d 0a0d 0a5b 6567 675f  rg.test....[egg_
-000003c0: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
-000003d0: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
-000003e0: 300d 0a0d 0a                             0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 7861 7267 2d70 7974 686f 6e0a 7665  = xarg-python.ve
+00000020: 7273 696f 6e20 3d20 6174 7472 3a20 7861  rsion = attr: xa
+00000030: 7267 2e5f 5f76 6572 7369 6f6e 5f5f 0a6b  rg.__version__.k
+00000040: 6579 776f 7264 7320 3d20 636f 6d6d 616e  eywords = comman
+00000050: 642c 2063 6f6d 6d61 6e64 2d6c 696e 652c  d, command-line,
+00000060: 2061 7267 7061 7273 652c 2078 6172 670a   argparse, xarg.
+00000070: 6465 7363 7269 7074 696f 6e20 3d20 5369  description = Si
+00000080: 6d70 6c65 2063 6f6d 6d61 6e64 2d6c 696e  mple command-lin
+00000090: 6520 746f 6f6c 2062 6173 6564 206f 6e20  e tool based on 
+000000a0: 6172 6770 6172 7365 2e0a 6175 7468 6f72  argparse..author
+000000b0: 203d 206d 696e 677a 6865 0a61 7574 686f   = mingzhe.autho
+000000c0: 725f 656d 6169 6c20 3d20 7a6f 756d 696e  r_email = zoumin
+000000d0: 677a 6865 4071 712e 636f 6d0a 7572 6c20  gzhe@qq.com.url 
+000000e0: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
+000000f0: 2e63 6f6d 2f7a 6f75 6d69 6e67 7a68 652f  .com/zoumingzhe/
+00000100: 7861 7267 2d70 7974 686f 6e0a 6c6f 6e67  xarg-python.long
+00000110: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
+00000120: 696c 653a 2052 4541 444d 452e 6d64 0a6c  ile: README.md.l
+00000130: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
+00000140: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
+00000150: 6578 742f 6d61 726b 646f 776e 0a6c 6963  ext/markdown.lic
+00000160: 656e 7365 203d 204d 4954 0a6c 6963 656e  ense = MIT.licen
+00000170: 7365 5f66 696c 6573 203d 204c 4943 454e  se_files = LICEN
+00000180: 5345 0a70 6c61 7466 6f72 6d73 203d 2061  SE.platforms = a
+00000190: 6e79 0a63 6c61 7373 6966 6965 7273 203d  ny.classifiers =
+000001a0: 200a 0950 726f 6772 616d 6d69 6e67 204c   ..Programming L
+000001b0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000001c0: 6e0a 0950 726f 6772 616d 6d69 6e67 204c  n..Programming L
+000001d0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000001e0: 6e20 3a3a 2033 0a70 726f 6a65 6374 5f75  n :: 3.project_u
+000001f0: 726c 7320 3d20 0a09 536f 7572 6365 2043  rls = ..Source C
+00000200: 6f64 6520 3d20 6874 7470 733a 2f2f 6769  ode = https://gi
+00000210: 7468 7562 2e63 6f6d 2f7a 6f75 6d69 6e67  thub.com/zouming
+00000220: 7a68 652f 7861 7267 2d70 7974 686f 6e0a  zhe/xarg-python.
+00000230: 0942 7567 2054 7261 636b 6572 203d 2068  .Bug Tracker = h
+00000240: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000250: 6d2f 7a6f 756d 696e 677a 6865 2f78 6172  m/zoumingzhe/xar
+00000260: 672d 7079 7468 6f6e 2f69 7373 7565 730a  g-python/issues.
+00000270: 0944 6f63 756d 656e 7461 7469 6f6e 203d  .Documentation =
+00000280: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000290: 636f 6d2f 7a6f 756d 696e 677a 6865 2f78  com/zoumingzhe/x
+000002a0: 6172 672d 7079 7468 6f6e 0a0a 5b6f 7074  arg-python..[opt
+000002b0: 696f 6e73 5d0a 7a69 705f 7361 6665 203d  ions].zip_safe =
+000002c0: 2054 7275 650a 696e 636c 7564 655f 7061   True.include_pa
+000002d0: 636b 6167 655f 6461 7461 203d 2054 7275  ckage_data = Tru
+000002e0: 650a 7079 7468 6f6e 5f72 6571 7569 7265  e.python_require
+000002f0: 7320 3d20 3e3d 332e 360a 7061 636b 6167  s = >=3.6.packag
+00000300: 6573 203d 2066 696e 643a 0a0a 5b6f 7074  es = find:..[opt
+00000310: 696f 6e73 2e65 6e74 7279 5f70 6f69 6e74  ions.entry_point
+00000320: 735d 0a63 6f6e 736f 6c65 5f73 6372 6970  s].console_scrip
+00000330: 7473 203d 200a 0978 6172 6720 3d20 7861  ts = ..xarg = xa
+00000340: 7267 2e65 7861 6d70 6c65 3a6d 6169 6e0a  rg.example:main.
+00000350: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
+00000360: 6573 2e66 696e 645d 0a77 6865 7265 203d  es.find].where =
+00000370: 202e 0a69 6e63 6c75 6465 203d 2078 6172   ..include = xar
+00000380: 670a 6578 636c 7564 6520 3d20 7861 7267  g.exclude = xarg
+00000390: 2e74 6573 740a 0a5b 6567 675f 696e 666f  .test..[egg_info
+000003a0: 5d0a 7461 675f 6275 696c 6420 3d20 0a74  ].tag_build = .t
+000003b0: 6167 5f64 6174 6520 3d20 300a 0a         ag_date = 0..
```

### Comparing `xarg-python-0.6/xarg/xarg_checker.py` & `xarg-python-0.7/xarg/checker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #!/usr/bin/python3
 # coding:utf-8
-# Copyright (c) 2023 ZouMingzhe <zoumingzhe@qq.com>
 
 prefix_chars = '-'
 
 
 def check_name_pos(fn):
     '''
     check positional argument name
```

### Comparing `xarg-python-0.6/xarg/__init__.py` & `xarg-python-0.7/xarg/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 #!/usr/bin/python3
 # coding:utf-8
-# Copyright (c) 2023 ZouMingzhe <zoumingzhe@qq.com>
-
-__version__ = "0.6"
 
 from argparse import ArgumentParser
 from argparse import _SubParsersAction
 from typing import Optional
 
-from .xarg_checker import check_name_opt
-from .xarg_checker import check_name_pos
-from .xarg_checker import check_nargs_opt
+from .checker import check_name_opt
+from .checker import check_name_pos
+from .checker import check_nargs_opt
 
 
 class argp(ArgumentParser):
     '''
     Simple command-line tool based on argparse.
     '''
```

### Comparing `xarg-python-0.6/xarg_python.egg-info/PKG-INFO` & `xarg-python-0.7/xarg_python.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,31 @@
-Metadata-Version: 2.1
-Name: xarg-python
-Version: 0.6
-Summary: Simple command-line tool based on argparse.
-Home-page: https://github.com/zoumingzhe/xarg-python
-Author: mingzhe
-Author-email: zoumingzhe@qq.com
-License: MIT
-Project-URL: Source Code, https://github.com/zoumingzhe/xarg-python
-Project-URL: Bug Tracker, https://github.com/zoumingzhe/xarg-python/issues
-Project-URL: Documentation, https://github.com/zoumingzhe/xarg-python
-Description: xarg
-        ====
-        
-        Simple command-line tool based on argparse.
-        
-Keywords: command,command-line,argparse,xarg
-Platform: any
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: xarg-python
+Version: 0.7
+Summary: Simple command-line tool based on argparse.
+Home-page: https://github.com/zoumingzhe/xarg-python
+Author: mingzhe
+Author-email: zoumingzhe@qq.com
+License: MIT
+Project-URL: Source Code, https://github.com/zoumingzhe/xarg-python
+Project-URL: Bug Tracker, https://github.com/zoumingzhe/xarg-python/issues
+Project-URL: Documentation, https://github.com/zoumingzhe/xarg-python
+Keywords: command,command-line,argparse,xarg
+Platform: any
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+xarg
+====
+
+Simple command-line tool based on argparse.
+
+build
+-----
+
+```shell
+rm -rf "build" "dist" "*.egg-info"
+python setup.py check sdist bdist_wheel --universal
+```
```

