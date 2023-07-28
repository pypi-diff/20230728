# Comparing `tmp/comics-0.1.7.tar.gz` & `tmp/comics-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comics-0.1.7.tar", last modified: Sun Feb 19 00:37:38 2023, max compression
+gzip compressed data, was "comics-0.1.8.tar", last modified: Fri Jul 28 19:48:47 2023, max compression
```

## Comparing `comics-0.1.7.tar` & `comics-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0       83 2022-12-31 19:16:58.732722 comics-0.1.7/.flake8
--rw-r--r--   0        0        0      170 2022-12-31 19:48:44.859641 comics-0.1.7/.github/dependabot.yaml
--rw-r--r--   0        0        0      635 2022-12-31 20:03:22.695499 comics-0.1.7/.github/workflows/ci.yaml
--rw-r--r--   0        0        0     1788 2022-12-31 19:45:59.945244 comics-0.1.7/.gitignore
--rw-r--r--   0        0        0     1068 2022-10-10 03:22:39.202960 comics-0.1.7/LICENSE
--rw-r--r--   0        0        0      845 2022-12-31 20:02:43.875219 comics-0.1.7/Makefile
--rw-r--r--   0        0        0     3261 2023-02-19 00:35:26.418095 comics-0.1.7/README.md
--rw-r--r--   0        0        0      137 2023-02-19 00:35:26.455128 comics-0.1.7/comics/__init__.py
--rw-r--r--   0        0        0    97322 2023-01-01 18:54:01.381726 comics-0.1.7/comics/api.py
--rw-r--r--   0        0        0    10348 2023-02-10 01:04:18.594969 comics-0.1.7/comics/constants.py
--rw-r--r--   0        0        0     6490 2023-02-19 00:35:49.551442 comics-0.1.7/comics/gocomics.py
--rw-r--r--   0        0        0        0 2022-12-31 18:27:16.728649 comics-0.1.7/conftest.py
--rw-r--r--   0        0        0    86801 2022-12-31 22:45:37.897969 comics-0.1.7/docs/calvinandhobbes.png
--rw-r--r--   0        0        0   103621 2022-12-31 23:48:27.298973 comics-0.1.7/docs/dilbert.png
--rw-r--r--   0        0        0      859 2023-01-02 18:25:07.630221 comics-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       32 2023-01-02 19:08:56.000350 comics-0.1.7/requirements-dev.txt
--rw-r--r--   0        0        0       47 2022-10-10 03:22:39.205858 comics-0.1.7/requirements.txt
--rw-r--r--   0        0        0     1238 2023-01-02 18:25:13.573784 comics-0.1.7/setup.cfg
--rw-r--r--   0        0        0     2644 2023-01-06 04:40:47.310591 comics-0.1.7/tests/test_api.py
--rw-r--r--   0        0        0     1127 2022-12-31 20:15:17.689328 comics-0.1.7/tests/test_directory.py
--rw-r--r--   0        0        0      619 2023-02-19 00:35:26.500275 comics-0.1.7/tests/test_exceptions.py
--rw-r--r--   0        0        0     4108 1970-01-01 00:00:00.000000 comics-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       83 2022-12-31 19:16:58.732722 comics-0.1.8/.flake8
+-rw-r--r--   0        0        0      170 2022-12-31 19:48:44.859641 comics-0.1.8/.github/dependabot.yaml
+-rw-r--r--   0        0        0      635 2022-12-31 20:03:22.695499 comics-0.1.8/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0     1788 2022-12-31 19:45:59.945244 comics-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1068 2022-10-10 03:22:39.202960 comics-0.1.8/LICENSE
+-rw-r--r--   0        0        0      845 2023-02-19 00:39:34.200712 comics-0.1.8/Makefile
+-rw-r--r--   0        0        0     3271 2023-07-28 19:43:05.477095 comics-0.1.8/README.md
+-rw-r--r--   0        0        0      185 2023-07-28 19:42:54.729889 comics-0.1.8/comics/__init__.py
+-rw-r--r--   0        0        0    97328 2023-07-28 19:44:39.362819 comics-0.1.8/comics/api.py
+-rw-r--r--   0        0        0    10353 2023-07-28 19:44:44.973999 comics-0.1.8/comics/constants.py
+-rw-r--r--   0        0        0      132 2023-07-28 19:42:06.401915 comics-0.1.8/comics/exceptions.py
+-rw-r--r--   0        0        0     6450 2023-07-28 19:42:16.105937 comics-0.1.8/comics/gocomics.py
+-rw-r--r--   0        0        0        0 2022-12-31 18:27:16.728649 comics-0.1.8/conftest.py
+-rw-r--r--   0        0        0    86801 2022-12-31 22:45:37.897969 comics-0.1.8/docs/calvinandhobbes.png
+-rw-r--r--   0        0        0   103621 2022-12-31 23:48:27.298973 comics-0.1.8/docs/dilbert.png
+-rw-r--r--   0        0        0      859 2023-01-02 18:25:07.630221 comics-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-01-02 19:08:56.000350 comics-0.1.8/requirements-dev.txt
+-rw-r--r--   0        0        0       47 2022-10-10 03:22:39.205858 comics-0.1.8/requirements.txt
+-rw-r--r--   0        0        0     1238 2023-01-02 18:25:13.573784 comics-0.1.8/setup.cfg
+-rw-r--r--   0        0        0    22780 2023-07-28 19:45:36.780205 comics-0.1.8/tests/downloads/comics_test.png
+-rw-r--r--   0        0        0     2836 2023-07-28 19:37:23.630458 comics-0.1.8/tests/test_api.py
+-rw-r--r--   0        0        0     1220 2023-07-28 19:34:17.837788 comics-0.1.8/tests/test_directory.py
+-rw-r--r--   0        0        0      619 2023-02-19 00:35:26.500275 comics-0.1.8/tests/test_exceptions.py
+-rw-r--r--   0        0        0     4118 1970-01-01 00:00:00.000000 comics-0.1.8/PKG-INFO
```

### Comparing `comics-0.1.7/.github/workflows/ci.yaml` & `comics-0.1.8/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `comics-0.1.7/.gitignore` & `comics-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `comics-0.1.7/LICENSE` & `comics-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `comics-0.1.7/Makefile` & `comics-0.1.8/Makefile`

 * *Files identical despite different names*

### Comparing `comics-0.1.7/README.md` & `comics-0.1.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -92,27 +92,27 @@
 
 ## Exceptions
 
 An exception will be thrown if the query date is unregistered or before the comic's origin date:
 
 ```python
 import comics
-from comics import InvalidDateError
+from comics.exceptions import InvalidDateError
 
 try:
     peanuts = comics.peanuts.date("1900-01-01")
     peanuts.download()
 except InvalidDateError:
-    print("Whoops - an invalid date was queried.")
+    print("Whoops, an invalid date was queried.")
 ```
 
 ## Contribute
 
-- [Issues Tracker](https://github.com/irahorecka/comics/issues)
-- [Source Code](https://github.com/irahorecka/comics/tree/master/comics)
+* [Issues Tracker](https://github.com/irahorecka/comics/issues)
+* [Source Code](https://github.com/irahorecka/comics/tree/master/comics)
 
 ## Support
 
 If you are having issues or would like to propose a new feature, please use the [issues tracker](https://github.com/irahorecka/comics/issues).
 
 <div align="center">
     <img src="docs/dilbert.png">
```

### Comparing `comics-0.1.7/comics/api.py` & `comics-0.1.8/comics/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 comics/api
 ~~~~~~~~~~
 """
 
 from datetime import datetime
 
-from .gocomics import ComicsAPI
+from comics.gocomics import ComicsAPI
 
 
 class aaggghhh(ComicsAPI):
     """GoComics endpoint for 'Aaggghhh'."""
 
     title = "Aaggghhh"
     start_date = datetime.strptime("2017-10-10", "%Y-%m-%d")
```

### Comparing `comics-0.1.7/comics/constants.py` & `comics-0.1.8/comics/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 comics/constants
 ~~~~~~~~~~~~~~~~
 """
 
-from . import api
+from comics import api
 
 # fmt: off
 COMICS_CLASS = (
     api.a_problem_like_jamal, api.aaggghhh, api.adam_at_home, api.adult_children, api.agnes,
     api.aj_and_magnus, api.al_goodwyn_editorial_cartoons, api.alis_house, api.alley_oop, api.amanda_the_great,
     api.andertoons, api.andy_capp, api.angry_little_girls, api.animal_crackers, api.annie, api.arlo_and_janis,
     api.art_by_moga, api.ask_shagg, api.at_tavicat, api.aunty_acid, api.baby_blues, api.back_in_the_day,
```

### Comparing `comics-0.1.7/comics/gocomics.py` & `comics-0.1.8/comics/gocomics.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from io import BytesIO
 
 import dateutil.parser
 import requests
 from bs4 import BeautifulSoup
 from PIL import Image
 
+from comics.exceptions import InvalidDateError
+
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 _BASE_URL = "https://www.gocomics.com"
 _BASE_RANDOM_URL = "https://www.gocomics.com/random"
 
 
 def bypass_comics_cache(func):
     """Comcics cache wrapper that checks and bypasses specific cached arguments."""
@@ -41,18 +43,14 @@
             if url.startswith(_BASE_RANDOM_URL) or is_stream
             else func(*args, **kwargs)
         )
 
     return wrapper
 
 
-class InvalidDateError(Exception):
-    """An invalid publication date was queried."""
-
-
 class ComicsAPI:
     """Constructs user interface with GoComics."""
 
     title = "NULL"
     start_date = datetime.today()
     _endpoint = "NULL"
```

### Comparing `comics-0.1.7/docs/calvinandhobbes.png` & `comics-0.1.8/docs/calvinandhobbes.png`

 * *Files identical despite different names*

### Comparing `comics-0.1.7/docs/dilbert.png` & `comics-0.1.8/docs/dilbert.png`

 * *Files identical despite different names*

### Comparing `comics-0.1.7/pyproject.toml` & `comics-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `comics-0.1.7/setup.cfg` & `comics-0.1.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `comics-0.1.7/tests/test_api.py` & `comics-0.1.8/tests/test_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import requests
 from pytest import mark
 from PIL import Image
 
 import comics
 
+
 # fmt: off
 attributes = (
     (comics.calvin_and_hobbes, "Calvin and Hobbes", "2017-02-14", "https://www.gocomics.com/calvinandhobbes/2017/02/14"),
     (comics.dilbert, "Dilbert Classics", "2016-01-22", "https://www.gocomics.com/dilbert-classics/2016/01/22"),
     (comics.foxtrot, "FoxTrot", "1992-04-17", "https://www.gocomics.com/foxtrot/1992/04/17"),
     (comics.garfield, "Garfield", "2010-06-30", "https://www.gocomics.com/garfield/2010/06/30"),
     (comics.peanuts, "Peanuts", "1965-07-04", "https://www.gocomics.com/peanuts/1965/07/04"),
@@ -41,17 +42,18 @@
     random_date = ch_random.date
     ch_date = comics.calvin_and_hobbes.date(random_date)
     assert ch_random.date == ch_date.date
     assert ch_random.url == ch_date.url
 
 
 def test_stream():
-    """Test comic image stream instance."""
+    """Test comic image stream instance and status code."""
     ch = comics.calvin_and_hobbes.random_date()
     assert isinstance(ch.stream(), requests.models.Response)
+    assert ch.stream().status_code == 200
 
 
 def test_download_comic_and_verify_content():
     """Test proper comic download execution and valid download image content."""
     ch = comics.calvin_and_hobbes.random_date()
     _download_comic_and_verify_content(ch)
 
@@ -68,12 +70,14 @@
     """Private function. Verify proper download execution and valid download image content
     of a `Comics` instance.
 
     Args:
         comics_inst (Comics): `Comics` instance.
     """
     img_filepath = Path(__file__).parent / "downloads" / "comics_test.png"
+    # Start by deleting the image if present - this allows me to keep the file tracked in Git to enable
+    # GitHub Actions testing
+    os.remove(img_filepath)
     # Verify download method works
     comics_inst.download(img_filepath)
     # Raises `PIL.UnidentifiedImageError` if invalid image
     Image.open(img_filepath).verify()
-    os.remove(img_filepath)
```

### Comparing `comics-0.1.7/tests/test_directory.py` & `comics-0.1.8/tests/test_directory.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,18 @@
     # Check if all comics directory is a tuple of sorted comic endpoints
     assert all_comics == tuple(sorted(all_comics))
 
 
 @mark.parametrize("params", (("fox", 3), ("calvin", 2), ("se", 30), ("rm", 6), ("at", 42)))
 def test_directory_search(params):
     """Tests proper return of comic endpoints when calling `comics.directory.search`
-    method with search keywords (case insensitive)."""
+    method with search keywords (case insensitive).
+
+    Args:
+        params (tuple): Args to unpack for testing number of search results.
+    """
     search_kwd, num_results = params
     assert len(comics.directory.search(search_kwd)) == num_results
     # Test case insensitivity
     assert len(comics.directory.search(search_kwd.upper())) == num_results
     assert len(comics.directory.search(search_kwd.title())) == num_results
     assert len(comics.directory.search(search_kwd.capitalize())) == num_results
```

### Comparing `comics-0.1.7/tests/test_exceptions.py` & `comics-0.1.8/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `comics-0.1.7/PKG-INFO` & `comics-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comics
-Version: 0.1.7
+Version: 0.1.8
 Summary: comics
 Home-page: https://github.com/irahorecka/comics
 Author: Ira Horecka
 Author-email: ira89@icloud.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
@@ -116,27 +116,27 @@
 
 ## Exceptions
 
 An exception will be thrown if the query date is unregistered or before the comic's origin date:
 
 ```python
 import comics
-from comics import InvalidDateError
+from comics.exceptions import InvalidDateError
 
 try:
     peanuts = comics.peanuts.date("1900-01-01")
     peanuts.download()
 except InvalidDateError:
-    print("Whoops - an invalid date was queried.")
+    print("Whoops, an invalid date was queried.")
 ```
 
 ## Contribute
 
-- [Issues Tracker](https://github.com/irahorecka/comics/issues)
-- [Source Code](https://github.com/irahorecka/comics/tree/master/comics)
+* [Issues Tracker](https://github.com/irahorecka/comics/issues)
+* [Source Code](https://github.com/irahorecka/comics/tree/master/comics)
 
 ## Support
 
 If you are having issues or would like to propose a new feature, please use the [issues tracker](https://github.com/irahorecka/comics/issues).
 
 <div align="center">
     <img src="docs/dilbert.png">
```

