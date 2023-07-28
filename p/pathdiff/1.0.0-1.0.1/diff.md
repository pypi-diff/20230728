# Comparing `tmp/pathdiff-1.0.0.tar.gz` & `tmp/pathdiff-1.0.1.tar.gz`

## Comparing `pathdiff-1.0.0.tar` & `pathdiff-1.0.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 pathdiff-1.0.0/src/pathdiff/__about__.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pathdiff-1.0.0/src/pathdiff/__init__.py
--rw-r--r--   0        0        0    14854 2020-02-02 00:00:00.000000 pathdiff-1.0.0/src/pathdiff/pathdiff.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test1/f1/file1.txt
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test1/f1/file2.txt
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test1/f1/file3.txt
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test1/f1/file4.txt
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test1/f1/file5.txt
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test1/f1/file6.txt
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test1/f2/file7.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test1/f2/file8.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test1/f2/file9.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test2/path1/file1.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test2/path1/file2.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test2/path1/file3-1.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test2/path1/f1/file1.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test2/path1/f1/file2.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test2/path1/f1/file3-1.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test2/path1/f1/f1/file1.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test2/path1/f1/f1/file2.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test2/path1/f1/f1/file3-1.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test2/path1/f2/file4.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test2/path1/f3/f1/file5.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test2/path1/f4/f1/file6.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test2/path1/f5/f1/file7-1.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test2/path1/f6/f1-1/file8.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test2/path2/file1.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test2/path2/file2.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test2/path2/file3-2.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test2/path2/f1/file1.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test2/path2/f1/file2.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test2/path2/f1/file3-2.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test2/path2/f1/f1/file1.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test2/path2/f1/f1/file2.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test2/path2/f1/f1/file3-2.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test2/path2/f2/file4.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test2/path2/f3/f1/file5.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test2/path2/f4/f1/file6.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test2/path2/f5/f1/file7-2.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test2/path2/f6/f1-2/file8.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test3/path1/file3.txt
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test3/path1/file7.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test3/path1/file8.txt
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test3/path1/file9-1.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test3/path1/f1/f1/file1.txt
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test3/path1/f1/f1/file4-1.txt
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test3/path1/f1/f1/file5.txt
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test3/path1/f1/f1/file6-1.txt
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test3/path1/f1/f1/file7.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test3/path1/f1/f1/file8.txt
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test3/path1/f1/f1/file9.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test3/path1/f2/file2.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test3/path2/file1.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test3/path2/file2.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test3/path2/file3.txt
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test3/path2/file4-2.txt
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test3/path2/file5.txt
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test3/path2/file6-2.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test3/path2/file8.txt
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pathdiff-1.0.0/tests/test3/path2/file9.txt
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pathdiff-1.0.0/.gitignore
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pathdiff-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 pathdiff-1.0.0/README.md
--rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 pathdiff-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 pathdiff-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 pathdiff-1.0.1/src/pathdiff/__about__.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pathdiff-1.0.1/src/pathdiff/__init__.py
+-rw-r--r--   0        0        0    14854 2020-02-02 00:00:00.000000 pathdiff-1.0.1/src/pathdiff/pathdiff.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test1/f1/file1.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test1/f1/file2.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test1/f1/file3.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test1/f1/file4.txt
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test1/f1/file5.txt
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test1/f1/file6.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test1/f2/file7.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test1/f2/file8.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test1/f2/file9.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test2/path1/file1.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test2/path1/file2.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test2/path1/file3-1.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test2/path1/f1/file1.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test2/path1/f1/file2.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test2/path1/f1/file3-1.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test2/path1/f1/f1/file1.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test2/path1/f1/f1/file2.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test2/path1/f1/f1/file3-1.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test2/path1/f2/file4.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test2/path1/f3/f1/file5.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test2/path1/f4/f1/file6.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test2/path1/f5/f1/file7-1.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test2/path1/f6/f1-1/file8.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test2/path2/file1.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test2/path2/file2.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test2/path2/file3-2.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test2/path2/f1/file1.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test2/path2/f1/file2.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test2/path2/f1/file3-2.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test2/path2/f1/f1/file1.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test2/path2/f1/f1/file2.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test2/path2/f1/f1/file3-2.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test2/path2/f2/file4.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test2/path2/f3/f1/file5.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test2/path2/f4/f1/file6.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test2/path2/f5/f1/file7-2.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test2/path2/f6/f1-2/file8.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test3/path1/file3.txt
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test3/path1/file7.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test3/path1/file8.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test3/path1/file9-1.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test3/path1/f1/f1/file1.txt
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test3/path1/f1/f1/file4-1.txt
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test3/path1/f1/f1/file5.txt
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test3/path1/f1/f1/file6-1.txt
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test3/path1/f1/f1/file7.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test3/path1/f1/f1/file8.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test3/path1/f1/f1/file9.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test3/path1/f2/file2.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test3/path2/file1.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test3/path2/file2.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test3/path2/file3.txt
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test3/path2/file4-2.txt
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test3/path2/file5.txt
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test3/path2/file6-2.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test3/path2/file8.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pathdiff-1.0.1/tests/test3/path2/file9.txt
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pathdiff-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pathdiff-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     4805 2020-02-02 00:00:00.000000 pathdiff-1.0.1/README.md
+-rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 pathdiff-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5821 2020-02-02 00:00:00.000000 pathdiff-1.0.1/PKG-INFO
```

### Comparing `pathdiff-1.0.0/src/pathdiff/pathdiff.py` & `pathdiff-1.0.1/src/pathdiff/pathdiff.py`

 * *Files identical despite different names*

### Comparing `pathdiff-1.0.0/LICENSE.txt` & `pathdiff-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pathdiff-1.0.0/pyproject.toml` & `pathdiff-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pathdiff-1.0.0/PKG-INFO` & `pathdiff-1.0.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathdiff
-Version: 1.0.0
+Version: 1.0.1
 Summary: A tool for detecting duplicate files and comparing directories.
 Project-URL: Documentation, https://github.com/manvithn/pathdiff#readme
 Project-URL: Issues, https://github.com/manvithn/pathdiff/issues
 Project-URL: Source, https://github.com/manvithn/pathdiff
 Author-email: Manvith Narahari <manvithn@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -24,23 +24,24 @@
 
 # pathdiff
 
 [![PyPI - Version](https://img.shields.io/pypi/v/pathdiff.svg)](https://pypi.org/project/pathdiff)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pathdiff.svg)](https://pypi.org/project/pathdiff)
 
 Pathdiff is a tool for:
+
 1. Detecting duplicate files in directories (Based on https://stackoverflow.com/a/36113168/300783)
 2. Comparing directories for differences in structure and content
 
 There are a number of alternative tools for both usecases, but this is a simple
 implementation that can be easily modified (unlike complex gui tools) and
 provides small conveniences like progress bars (unlike more basic command line
 tools like diff).
 
------
+---
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [License](#license)
 
@@ -51,60 +52,116 @@
 ```
 
 ## Usage
 
 ```console
 ❯ pathdiff find-duplicates tests/test1
 Fetching files from tests/test1
-|████████████████████████████████████████| 9 in 0.1s (85.56/s)
+|████████████████████████████████████████| 9 in 0.1s (88.59/s)
 Fetching file sizes
-|████████████████████████████████████████| 9/9 [100%] in 0.1s (87.68/s)
+|████████████████████████████████████████| 9/9 [100%] in 0.1s (88.10/s)
 Computing small hashes
-|████████████████████████████████████████| 9/9 [100%] in 0.1s (85.21/s)
+|████████████████████████████████████████| 9/9 [100%] in 0.1s (88.25/s)
 Computing full hashes
-|████████████████████████████████████████| 9/9 [100%] in 0.1s (83.98/s)
+|████████████████████████████████████████| 9/9 [100%] in 0.1s (88.01/s)
 
 Duplicates found:
-tests/test1/path1/file2.txt
-tests/test1/path1/file3.txt
-tests/test1/path1/file1.txt
+tests/test1/f2/file7.txt
+tests/test1/f1/file4.txt
 
 
 Duplicates found:
-tests/test1/path1/file4.txt
-tests/test1/path2/file7.txt
+tests/test1/f1/file2.txt
+tests/test1/f1/file3.txt
+tests/test1/f1/file1.txt
 
 
 Duplicates found:
-tests/test1/path1/file5.txt
-tests/test1/path1/file6.txt
+tests/test1/f2/file8.txt
+tests/test1/f2/file9.txt
 
 
 Duplicates found:
-tests/test1/path2/file8.txt
-tests/test1/path2/file9.txt
+tests/test1/f1/file5.txt
+tests/test1/f1/file6.txt
 ```
 
 ```console
 ❯ pathdiff compare-directories tests/test2/path1 tests/test2/path2
 Comparing directories tests/test2/path1 and tests/test2/path2
 Comparing directory structures
-|████████████████████████████████████████| 12 in 0.1s (114.04/s)
+|████████████████████████████████████████| 28 in 0.1s (265.55/s)
 Comparing common files
-|████████████████████████████████████████| 4/4 [100%] in 0.1s (37.66/s)
+|████████████████████████████████████████| 9/9 [100%] in 0.1s (85.30/s)
+
+Paths found in tests/test2/path1 but not found in tests/test2/path2:
+file3-1.txt
+f6/f1-1
+f5/f1/file7-1.txt
+f1/file3-1.txt
+f1/f1/file3-1.txt
+
+Paths found in tests/test2/path2 but not found in tests/test2/path1:
+file3-2.txt
+f6/f1-2
+f5/f1/file7-2.txt
+f1/file3-2.txt
+f1/f1/file3-2.txt
 
-Files found in tests/test2/path1 but not found in tests/test2/path2:
+Files found in tests/test2/path1 and tests/test2/path2 but contents do not match:
 file2.txt
-file1.txt
+f4/f1/file6.txt
+f1/file2.txt
+f1/f1/file2.txt
+```
 
-Files found in tests/test2/path2 but not found in tests/test2/path1:
-file8.txt
-file7.txt
+```console
+❯ pathdiff compare-contents tests/test3/path1 tests/test3/path2
+Comparing contents in directories tests/test3/path1 and tests/test3/path2
+Fetching files from tests/test3/path1
+|████████████████████████████████████████| 12 in 0.1s (118.00/s)
+Fetching files from tests/test3/path2
+|████████████████████████████████████████| 8 in 0.1s (77.02/s)
+Fetching file sizes
+|████████████████████████████████████████| 20/20 [100%] in 0.1s (196.16/s)
+Computing small hashes
+|████████████████████████████████████████| 20/20 [100%] in 0.1s (196.73/s)
+Computing full hashes
+|████████████████████████████████████████| 16/16 [100%] in 0.1s (155.59/s)
 
-Files found in tests/test2/path1 and tests/test2/path2 but contents do not match:
+Files found in tests/test3/path1 but not found in tests/test3/path2 (by content, names may match):
+f1/f1/file5.txt
+f1/f1/file4-1.txt
+
+Files found in tests/test3/path2 but not found in tests/test3/path1 (by content, names may match):
 file5.txt
-file6.txt
+file4-2.txt
+
+Files which do not match one-to-one or have different names:
+Group of duplicate files:
+Duplicates from tests/test3/path1:
+file7.txt
+f1/f1/file7.txt
+Duplicates from tests/test3/path2:
+
+Group of duplicate files:
+Duplicates from tests/test3/path1:
+file9-1.txt
+f1/f1/file9.txt
+Duplicates from tests/test3/path2:
+file9.txt
+Group of duplicate files:
+Duplicates from tests/test3/path1:
+file8.txt
+f1/f1/file8.txt
+Duplicates from tests/test3/path2:
+file8.txt
+Group of duplicate files:
+Duplicates from tests/test3/path1:
+f1/f1/file6-1.txt
+Duplicates from tests/test3/path2:
+file6-2.txt
 ```
 
 ## License
 
 `pathdiff` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

