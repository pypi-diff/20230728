# Comparing `tmp/vulcan-sql-0.7.0.tar.gz` & `tmp/vulcan-sql-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulcan-sql-0.7.0.tar", last modified: Tue Jul 25 08:01:44 2023, max compression
+gzip compressed data, was "vulcan-sql-0.7.1.tar", last modified: Fri Jul 28 03:53:46 2023, max compression
```

## Comparing `vulcan-sql-0.7.0.tar` & `vulcan-sql-0.7.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 canner     (501) staff       (20)        0 2023-07-25 08:01:44.713948 vulcan-sql-0.7.0/
--rw-r--r--   0 canner     (501) staff       (20)      397 2023-07-04 06:26:29.000000 vulcan-sql-0.7.0/MANIFEST.in
--rw-r--r--   0 canner     (501) staff       (20)      937 2023-07-25 08:01:44.713514 vulcan-sql-0.7.0/PKG-INFO
--rw-r--r--   0 canner     (501) staff       (20)      542 2023-07-04 02:03:53.000000 vulcan-sql-0.7.0/PUBLIC_README.md
--rw-r--r--   0 canner     (501) staff       (20)     4312 2023-07-25 07:55:01.000000 vulcan-sql-0.7.0/README.md
--rw-r--r--   0 canner     (501) staff       (20)       38 2023-07-25 08:01:44.714083 vulcan-sql-0.7.0/setup.cfg
--rw-r--r--   0 canner     (501) staff       (20)     1143 2023-07-25 08:00:46.000000 vulcan-sql-0.7.0/setup.py
-drwxr-xr-x   0 canner     (501) staff       (20)        0 2023-07-25 08:01:44.710866 vulcan-sql-0.7.0/vulcan_sql.egg-info/
--rw-r--r--   0 canner     (501) staff       (20)      937 2023-07-25 08:01:44.000000 vulcan-sql-0.7.0/vulcan_sql.egg-info/PKG-INFO
--rw-r--r--   0 canner     (501) staff       (20)      259 2023-07-25 08:01:44.000000 vulcan-sql-0.7.0/vulcan_sql.egg-info/SOURCES.txt
--rw-r--r--   0 canner     (501) staff       (20)        1 2023-07-25 08:01:44.000000 vulcan-sql-0.7.0/vulcan_sql.egg-info/dependency_links.txt
--rw-r--r--   0 canner     (501) staff       (20)       52 2023-07-25 08:01:44.000000 vulcan-sql-0.7.0/vulcan_sql.egg-info/entry_points.txt
--rw-r--r--   0 canner     (501) staff       (20)       10 2023-07-25 08:01:44.000000 vulcan-sql-0.7.0/vulcan_sql.egg-info/top_level.txt
-drwxr-xr-x   0 canner     (501) staff       (20)        0 2023-07-25 08:01:44.712454 vulcan-sql-0.7.0/vulcansql/
--rw-r--r--   0 canner     (501) staff       (20)      170 2023-07-04 02:03:53.000000 vulcan-sql-0.7.0/vulcansql/__init__.py
--rw-r--r--   0 canner     (501) staff       (20)     2147 2023-07-25 07:59:55.000000 vulcan-sql-0.7.0/vulcansql/cli.py
+drwxr-xr-x   0 canner     (501) staff       (20)        0 2023-07-28 03:53:46.416262 vulcan-sql-0.7.1/
+-rw-r--r--   0 canner     (501) staff       (20)      397 2023-07-04 06:26:29.000000 vulcan-sql-0.7.1/MANIFEST.in
+-rw-r--r--   0 canner     (501) staff       (20)      937 2023-07-28 03:53:46.415725 vulcan-sql-0.7.1/PKG-INFO
+-rw-r--r--   0 canner     (501) staff       (20)      542 2023-07-04 02:03:53.000000 vulcan-sql-0.7.1/PUBLIC_README.md
+-rw-r--r--   0 canner     (501) staff       (20)     4312 2023-07-27 10:31:34.000000 vulcan-sql-0.7.1/README.md
+-rw-r--r--   0 canner     (501) staff       (20)       38 2023-07-28 03:53:46.416409 vulcan-sql-0.7.1/setup.cfg
+-rw-r--r--   0 canner     (501) staff       (20)     1143 2023-07-28 03:52:42.000000 vulcan-sql-0.7.1/setup.py
+drwxr-xr-x   0 canner     (501) staff       (20)        0 2023-07-28 03:53:46.411651 vulcan-sql-0.7.1/vulcan_sql.egg-info/
+-rw-r--r--   0 canner     (501) staff       (20)      937 2023-07-28 03:53:46.000000 vulcan-sql-0.7.1/vulcan_sql.egg-info/PKG-INFO
+-rw-r--r--   0 canner     (501) staff       (20)      259 2023-07-28 03:53:46.000000 vulcan-sql-0.7.1/vulcan_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 canner     (501) staff       (20)        1 2023-07-28 03:53:46.000000 vulcan-sql-0.7.1/vulcan_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 canner     (501) staff       (20)       52 2023-07-28 03:53:46.000000 vulcan-sql-0.7.1/vulcan_sql.egg-info/entry_points.txt
+-rw-r--r--   0 canner     (501) staff       (20)       10 2023-07-28 03:53:46.000000 vulcan-sql-0.7.1/vulcan_sql.egg-info/top_level.txt
+drwxr-xr-x   0 canner     (501) staff       (20)        0 2023-07-28 03:53:46.414079 vulcan-sql-0.7.1/vulcansql/
+-rw-r--r--   0 canner     (501) staff       (20)      170 2023-07-04 02:03:53.000000 vulcan-sql-0.7.1/vulcansql/__init__.py
+-rw-r--r--   0 canner     (501) staff       (20)     2147 2023-07-25 07:59:55.000000 vulcan-sql-0.7.1/vulcansql/cli.py
```

### Comparing `vulcan-sql-0.7.0/PKG-INFO` & `vulcan-sql-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-sql
-Version: 0.7.0
+Version: 0.7.1
 Summary: VulcanSQL turns your SQL templates into data APIs for efficient data sharing. No backend skills required. Empower your data sharing, faster.
 Home-page: https://github.com/Canner/vulcan-sql
 Author: Canner Team
 Author-email: contact@cannerdata.com
 License: Apache 2.0
 Requires-Python: >=3.0.0
 Description-Content-Type: text/markdown
```

### Comparing `vulcan-sql-0.7.0/PUBLIC_README.md` & `vulcan-sql-0.7.1/PUBLIC_README.md`

 * *Files identical despite different names*

### Comparing `vulcan-sql-0.7.0/README.md` & `vulcan-sql-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `vulcan-sql-0.7.0/setup.py` & `vulcan-sql-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # read the contents of your README file
 directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(directory, "PUBLIC_README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup_kwargs = {
     'name': 'vulcan-sql',
-    'version': '0.7.0',
+    'version': '0.7.1',
     'description': 'VulcanSQL turns your SQL templates into data APIs for efficient data sharing. No backend skills required. Empower your data sharing, faster.',
     'long_description': long_description,
     'long_description_content_type': "text/markdown",
     'author': 'Canner Team',
     'author_email': 'contact@cannerdata.com',
     'license': "Apache 2.0",
     'url': 'https://github.com/Canner/vulcan-sql',
```

### Comparing `vulcan-sql-0.7.0/vulcan_sql.egg-info/PKG-INFO` & `vulcan-sql-0.7.1/vulcan_sql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-sql
-Version: 0.7.0
+Version: 0.7.1
 Summary: VulcanSQL turns your SQL templates into data APIs for efficient data sharing. No backend skills required. Empower your data sharing, faster.
 Home-page: https://github.com/Canner/vulcan-sql
 Author: Canner Team
 Author-email: contact@cannerdata.com
 License: Apache 2.0
 Requires-Python: >=3.0.0
 Description-Content-Type: text/markdown
```

### Comparing `vulcan-sql-0.7.0/vulcansql/cli.py` & `vulcan-sql-0.7.1/vulcansql/cli.py`

 * *Files identical despite different names*

