# Comparing `tmp/wfsx-1.0-py3-none-any.whl.zip` & `tmp/wfsx-1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 30941 bytes, number of entries: 19
+Zip file size: 30934 bytes, number of entries: 19
 -rw-rw-rw-  2.0 fat      413 b- defN 23-Jun-06 11:13 wfsx/CONST_j.py
 -rw-rw-rw-  2.0 fat     5163 b- defN 23-Jul-28 14:45 wfsx/Excel_x.py
 -rw-rw-rw-  2.0 fat     5280 b- defN 23-Jul-28 14:45 wfsx/Report.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-06 11:13 wfsx/__init__.py
 -rw-rw-rw-  2.0 fat     6310 b- defN 23-Jul-28 14:31 wfsx/api.py
 -rw-rw-rw-  2.0 fat     6019 b- defN 23-Jun-15 14:25 wfsx/apivalid.py
 -rw-rw-rw-  2.0 fat    16574 b- defN 23-Jul-28 14:41 wfsx/apivalidation.py
--rw-rw-rw-  2.0 fat    20708 b- defN 23-Jul-28 14:41 wfsx/common.py
+-rw-rw-rw-  2.0 fat    20705 b- defN 23-Jul-28 16:02 wfsx/common.py
 -rw-rw-rw-  2.0 fat     9505 b- defN 23-Jul-28 14:45 wfsx/dataextract.py
 -rw-rw-rw-  2.0 fat     2808 b- defN 23-Jun-06 11:13 wfsx/excel_json_reader.py
 -rw-rw-rw-  2.0 fat     4189 b- defN 23-Jun-16 15:41 wfsx/ghelper.py
 -rw-rw-rw-  2.0 fat     5407 b- defN 23-Jun-06 11:13 wfsx/parseexcel.py
 -rw-rw-rw-  2.0 fat     7022 b- defN 23-Jun-13 11:44 wfsx/plite.py
 -rw-rw-rw-  2.0 fat    23242 b- defN 23-Jul-28 14:45 wfsx/results_validate.py
--rw-rw-rw-  2.0 fat    11365 b- defN 23-Jul-28 15:28 wfsx-1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1235 b- defN 23-Jul-28 15:28 wfsx-1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-28 15:28 wfsx-1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-28 15:28 wfsx-1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1394 b- defN 23-Jul-28 15:28 wfsx-1.0.dist-info/RECORD
-19 files, 126731 bytes uncompressed, 28735 bytes compressed:  77.3%
+-rw-rw-rw-  2.0 fat    11365 b- defN 23-Jul-28 16:03 wfsx-1.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1235 b- defN 23-Jul-28 16:03 wfsx-1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-28 16:03 wfsx-1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-28 16:03 wfsx-1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1394 b- defN 23-Jul-28 16:03 wfsx-1.1.dist-info/RECORD
+19 files, 126728 bytes uncompressed, 28728 bytes compressed:  77.3%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: wfsx/plite.py
 Comment: 
 
 Filename: wfsx/results_validate.py
 Comment: 
 
-Filename: wfsx-1.0.dist-info/LICENSE
+Filename: wfsx-1.1.dist-info/LICENSE
 Comment: 
 
-Filename: wfsx-1.0.dist-info/METADATA
+Filename: wfsx-1.1.dist-info/METADATA
 Comment: 
 
-Filename: wfsx-1.0.dist-info/WHEEL
+Filename: wfsx-1.1.dist-info/WHEEL
 Comment: 
 
-Filename: wfsx-1.0.dist-info/top_level.txt
+Filename: wfsx-1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: wfsx-1.0.dist-info/RECORD
+Filename: wfsx-1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wfsx/common.py

```diff
@@ -252,15 +252,15 @@
             sLine, eLine = exeLine, None
     pathdata_file = mypath / 'test_dir' / 'test_onefms_api.py'
     with open(pathdata_file, 'w') as f:
         f.write('from cdxg import file_data\n')
         f.write('from utils.api import *\n')
         f.write('from cdxg.logging import log\n')
         f.write('from wfsx.common import get_tags, Create_New_Report, get_results, getepoint\n')
-        f.write('from test_dir.apiexecutor import apiSteps\n\n')
+        f.write('from utils.apiexecutor import apiSteps\n\n')
 
         f.write('mypath = Path.cwd()\n')
         f.write('config = configparser.ConfigParser()\n')
         f.write('config.read(mypath / "config.ini")\n')
         f.write('test_case_data = config.get("test_data_xl", "test_case_data_xl")\n')
         f.write('generate_test_ap = mypath / test_case_data\n')
         f.write('xHeaders = json.loads(config.get("Cookie_Headers", "xHeaders"))\n')
```

## Comparing `wfsx-1.0.dist-info/LICENSE` & `wfsx-1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `wfsx-1.0.dist-info/METADATA` & `wfsx-1.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wfsx
-Version: 1.0
+Version: 1.1
 Summary: api automation testing framework based on unittest.
 Home-page: https://github.com/saasaa831/wfsx/
 Author: saasaa
 Author-email: saasaa@saa.com
 License: Apache 2.0
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
```

## Comparing `wfsx-1.0.dist-info/RECORD` & `wfsx-1.1.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 wfsx/CONST_j.py,sha256=K1qp18BcG4QXmeYaMLqd8j6-_rnMj1kQ67RmtsWMFvw,413
 wfsx/Excel_x.py,sha256=-RhqrKWTi2ias2f8sMpembEYSectGn6zvhlDEaGIkIc,5163
 wfsx/Report.py,sha256=kbydYbBv0YmoOdgCQ2y92nuBNUZmYcwq4gbajGUbKMc,5280
 wfsx/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 wfsx/api.py,sha256=4RvVwxzel6i3jpIWOw8pzM_LOCc9P9lqk8QKrvOJGXM,6310
 wfsx/apivalid.py,sha256=OZz8aFjH9BSmrvJNY7XwV1yjUYHpd7Fa6pyO-X0z0G8,6019
 wfsx/apivalidation.py,sha256=Hl6G6bv66BVnlN6iZjxATfe19LyB7yfvSHQQZ_Ue0Sg,16574
-wfsx/common.py,sha256=VpuqUalXOnZHtz5fJRuC9PRiqFs97BNWoCGDUTJNOKs,20708
+wfsx/common.py,sha256=JMA43pYw9PAaAotrKs9wTiPUdqbKeti_MqEmVqCpqmo,20705
 wfsx/dataextract.py,sha256=OtbdeKfQXC4BT1ye7Kxp0zfjnZgitkU2kYF3X-xqbso,9505
 wfsx/excel_json_reader.py,sha256=z4vQkNRLKCO7x3UAeI8EVd9vjY5GDTEYDOVTj2jqICA,2808
 wfsx/ghelper.py,sha256=oYgGDv8YZOKAX6vg4gel0kjpaAwZ40137AQhAFDFnW8,4189
 wfsx/parseexcel.py,sha256=uXXUcI9AiDHqdaKd8oGAxu_3OXFmuw66CLRXvJRXHtc,5407
 wfsx/plite.py,sha256=d2yNK_XkO17OFQbr4Ecf_OSkDgys9vzdefnm03Lm3Ck,7022
 wfsx/results_validate.py,sha256=Jzx6xUHcbrTQuKhc9q48vKR7BXmSrEbD8T7SB45c_NM,23242
-wfsx-1.0.dist-info/LICENSE,sha256=O6YYwBy5W9D4kClOvrHiQlSfu479SgduHM03YRmz8mE,11365
-wfsx-1.0.dist-info/METADATA,sha256=zJs5NT7DxZl2yEus0LaCpGD3OhqHdgIL2U6DdhVw09g,1235
-wfsx-1.0.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-wfsx-1.0.dist-info/top_level.txt,sha256=ylpSMw0AVSmfULYBvc6iiXmLKtra7xinB3IPH0sBALs,5
-wfsx-1.0.dist-info/RECORD,,
+wfsx-1.1.dist-info/LICENSE,sha256=O6YYwBy5W9D4kClOvrHiQlSfu479SgduHM03YRmz8mE,11365
+wfsx-1.1.dist-info/METADATA,sha256=l921sY1rrSiQoqk98_ImDXm9loVnx9WQ1F7lAFyNzlo,1235
+wfsx-1.1.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+wfsx-1.1.dist-info/top_level.txt,sha256=ylpSMw0AVSmfULYBvc6iiXmLKtra7xinB3IPH0sBALs,5
+wfsx-1.1.dist-info/RECORD,,
```

