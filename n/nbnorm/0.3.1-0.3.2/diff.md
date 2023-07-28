# Comparing `tmp/nbnorm-0.3.1.tar.gz` & `tmp/nbnorm-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbnorm-0.3.1.tar", last modified: Wed Jan  4 10:17:35 2023, max compression
+gzip compressed data, was "nbnorm-0.3.2.tar", last modified: Fri Jul 28 15:41:07 2023, max compression
```

## Comparing `nbnorm-0.3.1.tar` & `nbnorm-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-01-04 10:17:35.865893 nbnorm-0.3.1/
--rw-r--r--   0 tparment (15010) diana    (200036)      506 2023-01-04 10:17:35.865506 nbnorm-0.3.1/PKG-INFO
--rw-r--r--   0 tparment (15010) diana    (200036)      226 2022-07-21 09:34:26.000000 nbnorm-0.3.1/README.md
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-01-04 10:17:35.861573 nbnorm-0.3.1/nbnorm/
--rw-r--r--   0 tparment (15010) diana    (200036)       32 2022-07-21 09:27:30.000000 nbnorm-0.3.1/nbnorm/__init__.py
--rwxr-xr-x   0 tparment (15010) diana    (200036)    17807 2023-01-04 10:07:43.000000 nbnorm-0.3.1/nbnorm/nbnorm.py
--rw-r--r--   0 tparment (15010) diana    (200036)       22 2023-01-04 10:16:51.000000 nbnorm-0.3.1/nbnorm/version.py
--rw-r--r--   0 tparment (15010) diana    (200036)     1482 2022-07-21 09:28:39.000000 nbnorm-0.3.1/nbnorm/xpath.py
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-01-04 10:17:35.865028 nbnorm-0.3.1/nbnorm.egg-info/
--rw-r--r--   0 tparment (15010) diana    (200036)      506 2023-01-04 10:17:35.000000 nbnorm-0.3.1/nbnorm.egg-info/PKG-INFO
--rw-r--r--   0 tparment (15010) diana    (200036)      299 2023-01-04 10:17:35.000000 nbnorm-0.3.1/nbnorm.egg-info/SOURCES.txt
--rw-r--r--   0 tparment (15010) diana    (200036)        1 2023-01-04 10:17:35.000000 nbnorm-0.3.1/nbnorm.egg-info/dependency_links.txt
--rw-r--r--   0 tparment (15010) diana    (200036)       46 2023-01-04 10:17:35.000000 nbnorm-0.3.1/nbnorm.egg-info/entry_points.txt
--rw-r--r--   0 tparment (15010) diana    (200036)        1 2022-07-21 09:47:04.000000 nbnorm-0.3.1/nbnorm.egg-info/not-zip-safe
--rw-r--r--   0 tparment (15010) diana    (200036)        9 2023-01-04 10:17:35.000000 nbnorm-0.3.1/nbnorm.egg-info/requires.txt
--rw-r--r--   0 tparment (15010) diana    (200036)        7 2023-01-04 10:17:35.000000 nbnorm-0.3.1/nbnorm.egg-info/top_level.txt
--rw-r--r--   0 tparment (15010) diana    (200036)       38 2023-01-04 10:17:35.865973 nbnorm-0.3.1/setup.cfg
--rwxr-xr-x   0 tparment (15010) diana    (200036)     1442 2022-07-21 09:35:19.000000 nbnorm-0.3.1/setup.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-07-28 15:41:07.995734 nbnorm-0.3.2/
+-rw-r--r--   0 tparment (15010) diana    (200036)      506 2023-07-28 15:41:07.995346 nbnorm-0.3.2/PKG-INFO
+-rw-r--r--   0 tparment (15010) diana    (200036)      226 2022-07-21 09:34:26.000000 nbnorm-0.3.2/README.md
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-07-28 15:41:07.991735 nbnorm-0.3.2/nbnorm/
+-rw-r--r--   0 tparment (15010) diana    (200036)       32 2022-07-21 09:27:30.000000 nbnorm-0.3.2/nbnorm/__init__.py
+-rwxr-xr-x   0 tparment (15010) diana    (200036)    18570 2023-07-28 15:07:09.000000 nbnorm-0.3.2/nbnorm/nbnorm.py
+-rw-r--r--   0 tparment (15010) diana    (200036)       22 2023-07-28 15:40:47.000000 nbnorm-0.3.2/nbnorm/version.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     1482 2022-07-21 09:28:39.000000 nbnorm-0.3.2/nbnorm/xpath.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-07-28 15:41:07.994862 nbnorm-0.3.2/nbnorm.egg-info/
+-rw-r--r--   0 tparment (15010) diana    (200036)      506 2023-07-28 15:41:07.000000 nbnorm-0.3.2/nbnorm.egg-info/PKG-INFO
+-rw-r--r--   0 tparment (15010) diana    (200036)      299 2023-07-28 15:41:07.000000 nbnorm-0.3.2/nbnorm.egg-info/SOURCES.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)        1 2023-07-28 15:41:07.000000 nbnorm-0.3.2/nbnorm.egg-info/dependency_links.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)       46 2023-07-28 15:41:07.000000 nbnorm-0.3.2/nbnorm.egg-info/entry_points.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)        1 2022-07-21 09:47:04.000000 nbnorm-0.3.2/nbnorm.egg-info/not-zip-safe
+-rw-r--r--   0 tparment (15010) diana    (200036)        9 2023-07-28 15:41:07.000000 nbnorm-0.3.2/nbnorm.egg-info/requires.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)        7 2023-07-28 15:41:07.000000 nbnorm-0.3.2/nbnorm.egg-info/top_level.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)       38 2023-07-28 15:41:07.995835 nbnorm-0.3.2/setup.cfg
+-rwxr-xr-x   0 tparment (15010) diana    (200036)     1442 2022-07-21 09:35:19.000000 nbnorm-0.3.2/setup.py
```

### Comparing `nbnorm-0.3.1/nbnorm/nbnorm.py` & `nbnorm-0.3.2/nbnorm/nbnorm.py`

 * *Files 4% similar despite different names*

```diff
@@ -227,23 +227,25 @@
 
     def ensure_style(self, style_rank, style_crumb):
         """
         make sure one of the first cells is a style cell
 
         the actual text is searched in a file named .style
         """
-        return self._ensure_item("style", "code", style_rank, style_crumb, ".style")
+        return self._ensure_item(
+            "style", "code", style_rank, style_crumb, ".style")
 
     def ensure_license(self, license_rank, license_crumb):
         """
         make sure one of the first cells is a license cell
 
         the actual text is searched in a file named .license
         """
-        return self._ensure_item("license", "markdown", license_rank, license_crumb, ".license")
+        return self._ensure_item(
+            "license", "markdown", license_rank, license_crumb, ".license")
 
 
 
     # I keep the code for these 2 but don't need this any longer
     # as I have all kinds of shortcuts and interactive tools now
     # plus, nbconvert(at least in jupyter) has preprocessor options to deal
     # with this as well
@@ -453,15 +455,15 @@
                 even if already present""")
     parser.add_argument(
         "-s", "--style-rank", dest='style_rank', default=None, action='store', type=int,
         help="""make sure the style cell is up-to-date with .style;
                 provide the style rank, used only for inserting a missing cell;
                 default is to not manage style""")
     parser.add_argument(
-        "-S", "--style-crumb", default="HTML(",
+        "-S", "--style-crumb", default=r"HTML\(",
         help="a cell that contains that string is considered a style cell")
     parser.add_argument(
         "-l", "--license-rank", dest='license_rank', default=None, action='store', type=int,
         help="""make sure the license cell is up-to-date with .license;
                 provide the license cell rank, used only for inserting a missing cell;
                 default is to not manage license""")
     parser.add_argument(
@@ -479,19 +481,40 @@
     parser.add_argument(
         "-u", "--urls", default=False, action='store_true',
         help="tries to spot direct URLs, i.e. used outside of markdown []()")
     parser.add_argument(
         "-v", "--verbose", dest="verbose", action="store_true", default=False,
         help="show current nbhosting.title")
     parser.add_argument(
-        "notebooks", nargs="+",
+        "notebooks", nargs="*",
         help="the notebooks to normalize")
+    parser.add_argument(
+        "--summary", action="store_true", default=False,
+        help="show summary of all settings - exit immediately"
+    )
 
     args = parser.parse_args()
 
+    if args.summary:
+        print(f"nbhosting.title: {args.title}")
+        print(f"force title: {args.force_title}")
+        print(f"style rank: {args.style_rank}")
+        print(f"style crumb: {args.style_crumb}")
+        print(f"license rank: {args.license_rank}")
+        print(f"license crumb: {args.license_crumb}")
+        print(f"rise: {args.rise}")
+        print(f"extensions: {args.extensions}")
+        print(f"backquotes: {args.backquotes}")
+        print(f"urls: {args.urls}")
+        exit(0)
+
+    if not args.notebooks:
+        parser.print_help()
+        sys.exit(1)
+
     for notebook in args.notebooks:
         if args.verbose:
             print(f"{sys.argv[0]} is opening notebook {notebook}")
         full_monty(
             notebook, title=args.title, force_title=args.force_title,
             license_rank=args.license_rank, license_crumb=args.license_crumb,
             style_rank=args.style_rank, style_crumb=args.style_crumb,
```

### Comparing `nbnorm-0.3.1/nbnorm/xpath.py` & `nbnorm-0.3.2/nbnorm/xpath.py`

 * *Files identical despite different names*

### Comparing `nbnorm-0.3.1/setup.py` & `nbnorm-0.3.2/setup.py`

 * *Files identical despite different names*

