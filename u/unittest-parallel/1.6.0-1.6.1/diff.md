# Comparing `tmp/unittest-parallel-1.6.0.tar.gz` & `tmp/unittest-parallel-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unittest-parallel-1.6.0.tar", last modified: Wed Jun 28 17:25:25 2023, max compression
+gzip compressed data, was "unittest-parallel-1.6.1.tar", last modified: Fri Jul 28 20:39:38 2023, max compression
```

## Comparing `unittest-parallel-1.6.0.tar` & `unittest-parallel-1.6.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2023-06-28 17:25:25.612262 unittest-parallel-1.6.0/
--rw-r--r--   0 craighobbs   (501) staff       (20)     1081 2023-06-11 21:05:16.000000 unittest-parallel-1.6.0/LICENSE
--rw-r--r--   0 craighobbs   (501) staff       (20)     3784 2023-06-28 17:25:25.612313 unittest-parallel-1.6.0/PKG-INFO
--rw-r--r--   0 craighobbs   (501) staff       (20)     2894 2023-06-28 17:22:10.000000 unittest-parallel-1.6.0/README.md
--rw-r--r--   0 craighobbs   (501) staff       (20)       50 2023-06-11 21:05:16.000000 unittest-parallel-1.6.0/pyproject.toml
--rw-r--r--   0 craighobbs   (501) staff       (20)     1029 2023-06-28 17:25:25.612541 unittest-parallel-1.6.0/setup.cfg
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2023-06-28 17:25:25.610780 unittest-parallel-1.6.0/src/
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2023-06-28 17:25:25.611539 unittest-parallel-1.6.0/src/unittest_parallel/
--rw-r--r--   0 craighobbs   (501) staff       (20)      102 2023-06-11 21:05:16.000000 unittest-parallel-1.6.0/src/unittest_parallel/__init__.py
--rw-r--r--   0 craighobbs   (501) staff       (20)      241 2023-06-11 21:05:16.000000 unittest-parallel-1.6.0/src/unittest_parallel/__main__.py
--rw-r--r--   0 craighobbs   (501) staff       (20)    14314 2023-06-28 17:22:10.000000 unittest-parallel-1.6.0/src/unittest_parallel/main.py
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2023-06-28 17:25:25.612170 unittest-parallel-1.6.0/src/unittest_parallel.egg-info/
--rw-r--r--   0 craighobbs   (501) staff       (20)     3784 2023-06-28 17:25:25.000000 unittest-parallel-1.6.0/src/unittest_parallel.egg-info/PKG-INFO
--rw-r--r--   0 craighobbs   (501) staff       (20)      412 2023-06-28 17:25:25.000000 unittest-parallel-1.6.0/src/unittest_parallel.egg-info/SOURCES.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)        1 2023-06-28 17:25:25.000000 unittest-parallel-1.6.0/src/unittest_parallel.egg-info/dependency_links.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)       66 2023-06-28 17:25:25.000000 unittest-parallel-1.6.0/src/unittest_parallel.egg-info/entry_points.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)       14 2023-06-28 17:25:25.000000 unittest-parallel-1.6.0/src/unittest_parallel.egg-info/requires.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)       18 2023-06-28 17:25:25.000000 unittest-parallel-1.6.0/src/unittest_parallel.egg-info/top_level.txt
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2023-07-28 20:39:38.048272 unittest-parallel-1.6.1/
+-rw-r--r--   0 craighobbs   (501) staff       (20)     1081 2023-07-11 15:37:54.000000 unittest-parallel-1.6.1/LICENSE
+-rw-r--r--   0 craighobbs   (501) staff       (20)     3784 2023-07-28 20:39:38.048326 unittest-parallel-1.6.1/PKG-INFO
+-rw-r--r--   0 craighobbs   (501) staff       (20)     2894 2023-07-11 15:37:54.000000 unittest-parallel-1.6.1/README.md
+-rw-r--r--   0 craighobbs   (501) staff       (20)       50 2023-07-11 15:37:54.000000 unittest-parallel-1.6.1/pyproject.toml
+-rw-r--r--   0 craighobbs   (501) staff       (20)     1029 2023-07-28 20:39:38.048567 unittest-parallel-1.6.1/setup.cfg
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2023-07-28 20:39:38.046734 unittest-parallel-1.6.1/src/
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2023-07-28 20:39:38.047522 unittest-parallel-1.6.1/src/unittest_parallel/
+-rw-r--r--   0 craighobbs   (501) staff       (20)      102 2023-07-11 15:37:54.000000 unittest-parallel-1.6.1/src/unittest_parallel/__init__.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)      241 2023-07-11 15:37:54.000000 unittest-parallel-1.6.1/src/unittest_parallel/__main__.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)    14266 2023-07-28 20:33:25.000000 unittest-parallel-1.6.1/src/unittest_parallel/main.py
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2023-07-28 20:39:38.048172 unittest-parallel-1.6.1/src/unittest_parallel.egg-info/
+-rw-r--r--   0 craighobbs   (501) staff       (20)     3784 2023-07-28 20:39:38.000000 unittest-parallel-1.6.1/src/unittest_parallel.egg-info/PKG-INFO
+-rw-r--r--   0 craighobbs   (501) staff       (20)      412 2023-07-28 20:39:38.000000 unittest-parallel-1.6.1/src/unittest_parallel.egg-info/SOURCES.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)        1 2023-07-28 20:39:38.000000 unittest-parallel-1.6.1/src/unittest_parallel.egg-info/dependency_links.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)       66 2023-07-28 20:39:38.000000 unittest-parallel-1.6.1/src/unittest_parallel.egg-info/entry_points.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)       14 2023-07-28 20:39:38.000000 unittest-parallel-1.6.1/src/unittest_parallel.egg-info/requires.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)       18 2023-07-28 20:39:38.000000 unittest-parallel-1.6.1/src/unittest_parallel.egg-info/top_level.txt
```

### Comparing `unittest-parallel-1.6.0/LICENSE` & `unittest-parallel-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unittest-parallel-1.6.0/PKG-INFO` & `unittest-parallel-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unittest-parallel
-Version: 1.6.0
+Version: 1.6.1
 Summary: Parallel unit test runner with coverage support
 Home-page: https://github.com/craigahobbs/unittest-parallel
 Author: Craig A. Hobbs
 Author-email: craigahobbs@gmail.com
 License: MIT
 Keywords: test,unittest,coverage,parallel
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `unittest-parallel-1.6.0/README.md` & `unittest-parallel-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `unittest-parallel-1.6.0/setup.cfg` & `unittest-parallel-1.6.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = unittest-parallel
-version = 1.6.0
+version = 1.6.1
 url = https://github.com/craigahobbs/unittest-parallel
 author = Craig A. Hobbs
 author_email = craigahobbs@gmail.com
 license = MIT
 description = Parallel unit test runner with coverage support
 long_description = file:README.md
 long_description_content_type = text/markdown
```

### Comparing `unittest-parallel-1.6.0/src/unittest_parallel/main.py` & `unittest-parallel-1.6.1/src/unittest_parallel/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -164,15 +164,18 @@
         if not is_success:
             parser.exit(status=len(errors) + len(failures) + unexpected_successes)
 
         # Coverage?
         if args.coverage:
 
             # Combine the coverage files
-            cov = coverage.Coverage(config_file=args.coverage_rcfile)
+            cov_options = {}
+            if args.coverage_rcfile is not None:
+                cov_options['config_file'] = args.coverage_rcfile
+            cov = coverage.Coverage(**cov_options)
             cov.combine(data_paths=[os.path.join(temp_dir, x) for x in os.listdir(temp_dir)])
 
             # Coverage report
             print(file=sys.stderr)
             percent_covered = cov.report(ignore_errors=True, file=sys.stderr)
             print(f'Total coverage is {percent_covered:.2f}%', file=sys.stderr)
 
@@ -200,22 +203,24 @@
     # Running tests with coverage?
     if args.coverage:
         # Generate a random coverage data file name - file is deleted along with containing directory
         with tempfile.NamedTemporaryFile(dir=temp_dir, delete=False) as coverage_file:
             pass
 
         # Create the coverage object
-        cov = coverage.Coverage(
-            config_file=args.coverage_rcfile,
-            data_file=coverage_file.name,
-            branch=args.coverage_branch,
-            include=args.coverage_include,
-            omit=(args.coverage_omit if args.coverage_omit else []) + [__file__],
-            source=args.coverage_source
-        )
+        cov_options = {
+            'branch': args.coverage_branch,
+            'data_file': coverage_file.name,
+            'include': args.coverage_include,
+            'omit': (args.coverage_omit if args.coverage_omit else []) + [__file__],
+            'source': args.coverage_source
+        }
+        if args.coverage_rcfile is not None:
+            cov_options['config_file'] = args.coverage_rcfile
+        cov = coverage.Coverage(**cov_options)
         try:
             # Start measuring code coverage
             cov.start()
 
             # Yield for unit test running
             yield cov
         finally:
@@ -308,49 +313,42 @@
         stream = type(stream)(sys.stderr)
         super().__init__(stream, descriptions, verbosity)
 
     def startTest(self, test):
         if self.showAll:
             self.stream.writeln(f'{self.getDescription(test)} ...')
             self.stream.flush()
-        # pylint: disable=bad-super-call
         super(unittest.TextTestResult, self).startTest(test)
 
     def _add_helper(self, test, dots_message, show_all_message):
         if self.showAll:
             self.stream.writeln(f'{self.getDescription(test)} ... {show_all_message}')
         elif self.dots:
             self.stream.write(dots_message)
         self.stream.flush()
 
     def addSuccess(self, test):
-        # pylint: disable=bad-super-call
         super(unittest.TextTestResult, self).addSuccess(test)
         self._add_helper(test, '.', 'ok')
 
     def addError(self, test, err):
-        # pylint: disable=bad-super-call
         super(unittest.TextTestResult, self).addError(test, err)
         self._add_helper(test, 'E', 'ERROR')
 
     def addFailure(self, test, err):
-        # pylint: disable=bad-super-call
         super(unittest.TextTestResult, self).addFailure(test, err)
         self._add_helper(test, 'F', 'FAIL')
 
     def addSkip(self, test, reason):
-        # pylint: disable=bad-super-call
         super(unittest.TextTestResult, self).addSkip(test, reason)
         self._add_helper(test, 's', f'skipped {reason!r}')
 
     def addExpectedFailure(self, test, err):
-        # pylint: disable=bad-super-call
         super(unittest.TextTestResult, self).addExpectedFailure(test, err)
         self._add_helper(test, 'x', 'expected failure')
 
     def addUnexpectedSuccess(self, test):
-        # pylint: disable=bad-super-call
         super(unittest.TextTestResult, self).addUnexpectedSuccess(test)
         self._add_helper(test, 'u', 'unexpected success')
 
     def printErrors(self):
         pass
```

### Comparing `unittest-parallel-1.6.0/src/unittest_parallel.egg-info/PKG-INFO` & `unittest-parallel-1.6.1/src/unittest_parallel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unittest-parallel
-Version: 1.6.0
+Version: 1.6.1
 Summary: Parallel unit test runner with coverage support
 Home-page: https://github.com/craigahobbs/unittest-parallel
 Author: Craig A. Hobbs
 Author-email: craigahobbs@gmail.com
 License: MIT
 Keywords: test,unittest,coverage,parallel
 Classifier: Development Status :: 5 - Production/Stable
```

