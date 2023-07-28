# Comparing `tmp/autoparaselenium-0.2.0.tar.gz` & `tmp/autoparaselenium-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoparaselenium-0.2.0.tar", last modified: Sat Jun  3 18:15:16 2023, max compression
+gzip compressed data, was "autoparaselenium-0.3.0.tar", last modified: Fri Jul 28 04:25:45 2023, max compression
```

## Comparing `autoparaselenium-0.2.0.tar` & `autoparaselenium-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:15:16.645524 autoparaselenium-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:15:16.641524 autoparaselenium-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:15:16.641524 autoparaselenium-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-03 18:14:59.000000 autoparaselenium-0.2.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-03 18:14:59.000000 autoparaselenium-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-03 18:14:59.000000 autoparaselenium-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-03 18:15:16.645524 autoparaselenium-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-03 18:14:59.000000 autoparaselenium-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:15:16.641524 autoparaselenium-0.2.0/autoparaselenium/
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-03 18:14:59.000000 autoparaselenium-0.2.0/autoparaselenium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-03 18:14:59.000000 autoparaselenium-0.2.0/autoparaselenium/browser_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:15:16.645524 autoparaselenium-0.2.0/autoparaselenium/browsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 18:14:59.000000 autoparaselenium-0.2.0/autoparaselenium/browsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-06-03 18:14:59.000000 autoparaselenium-0.2.0/autoparaselenium/browsers/chrome.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-03 18:14:59.000000 autoparaselenium-0.2.0/autoparaselenium/browsers/firefox.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-03 18:14:59.000000 autoparaselenium-0.2.0/autoparaselenium/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-03 18:14:59.000000 autoparaselenium-0.2.0/autoparaselenium/setup_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:15:16.645524 autoparaselenium-0.2.0/autoparaselenium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-03 18:15:16.000000 autoparaselenium-0.2.0/autoparaselenium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-03 18:15:16.000000 autoparaselenium-0.2.0/autoparaselenium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 18:15:16.000000 autoparaselenium-0.2.0/autoparaselenium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-03 18:15:16.000000 autoparaselenium-0.2.0/autoparaselenium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-03 18:15:16.000000 autoparaselenium-0.2.0/autoparaselenium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-03 18:14:59.000000 autoparaselenium-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 18:15:16.645524 autoparaselenium-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:15:16.645524 autoparaselenium-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-03 18:14:59.000000 autoparaselenium-0.2.0/tests/test_browsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-03 18:14:59.000000 autoparaselenium-0.2.0/tests/test_everything.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-03 18:14:59.000000 autoparaselenium-0.2.0/tests/test_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:25:45.298641 autoparaselenium-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:25:45.294641 autoparaselenium-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:25:45.294641 autoparaselenium-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-28 04:25:26.000000 autoparaselenium-0.3.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 04:25:26.000000 autoparaselenium-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 04:25:26.000000 autoparaselenium-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-07-28 04:25:45.298641 autoparaselenium-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-28 04:25:26.000000 autoparaselenium-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:25:45.294641 autoparaselenium-0.3.0/autoparaselenium/
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-28 04:25:26.000000 autoparaselenium-0.3.0/autoparaselenium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-28 04:25:26.000000 autoparaselenium-0.3.0/autoparaselenium/browser_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:25:45.298641 autoparaselenium-0.3.0/autoparaselenium/browsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 04:25:26.000000 autoparaselenium-0.3.0/autoparaselenium/browsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-28 04:25:26.000000 autoparaselenium-0.3.0/autoparaselenium/browsers/chrome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-28 04:25:26.000000 autoparaselenium-0.3.0/autoparaselenium/browsers/firefox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-28 04:25:26.000000 autoparaselenium-0.3.0/autoparaselenium/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-28 04:25:26.000000 autoparaselenium-0.3.0/autoparaselenium/setup_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:25:45.294641 autoparaselenium-0.3.0/autoparaselenium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-07-28 04:25:45.000000 autoparaselenium-0.3.0/autoparaselenium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-28 04:25:45.000000 autoparaselenium-0.3.0/autoparaselenium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 04:25:45.000000 autoparaselenium-0.3.0/autoparaselenium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 04:25:45.000000 autoparaselenium-0.3.0/autoparaselenium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 04:25:45.000000 autoparaselenium-0.3.0/autoparaselenium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-28 04:25:26.000000 autoparaselenium-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 04:25:45.298641 autoparaselenium-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:25:45.298641 autoparaselenium-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-28 04:25:26.000000 autoparaselenium-0.3.0/tests/test_browsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-28 04:25:26.000000 autoparaselenium-0.3.0/tests/test_everything.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-28 04:25:26.000000 autoparaselenium-0.3.0/tests/test_pool.py
```

### Comparing `autoparaselenium-0.2.0/.github/workflows/pypi-publish.yml` & `autoparaselenium-0.3.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `autoparaselenium-0.2.0/LICENSE` & `autoparaselenium-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autoparaselenium-0.2.0/PKG-INFO` & `autoparaselenium-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoparaselenium
-Version: 0.2.0
+Version: 0.3.0
 Summary: A library to make parallel selenium tests that automatically download and setup webdrivers
 Author-email: Ronak Badhe <ronak.badhe@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autoparaselenium-0.2.0/README.md` & `autoparaselenium-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `autoparaselenium-0.2.0/autoparaselenium/__init__.py` & `autoparaselenium-0.3.0/autoparaselenium/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 import sys
 import time
 from concurrent.futures import ThreadPoolExecutor
 from contextlib import suppress
 from functools import partial, wraps
 from typing import Iterable, List, Optional
 
-from autoparaselenium.browsers import chrome, firefox
 from autoparaselenium.browser_pool import BrowserPool
+from autoparaselenium.browsers import chrome, firefox
 from autoparaselenium.models import Conf, Extension
 
-
 _browser_pool: Optional[BrowserPool] = None
 all_ = [chrome, firefox]
 
-_test_count = 0 # manual reference counting since threading borks with destructors
+_test_count = 0  # manual reference counting since threading borks with destructors
 
 
-def configure(*_, extensions: List[Extension] = [], headless=True, selenium_dir="drivers"):
+def configure(
+    *_, extensions: List[Extension] = [], headless=True, selenium_dir="drivers"
+):
     global _browser_pool
 
     if _browser_pool is not None:
         return
 
     conf = Conf(extensions=extensions, headless=headless, selenium_dir=selenium_dir)
     for browser in [chrome, firefox]:
@@ -33,15 +34,14 @@
 
 def run_on(*browsers):
     browsers = [*browsers]
 
     if not browsers:
         raise TypeError("Please specify a browser or browser list to run on")
 
-
     if isinstance(browsers[0], Iterable):
         browsers = [*it.chain(*browsers)]
 
     if len(browsers) == 1:
         return partial(__wrap_test, browsers[0])
 
     def wrapper(test):
@@ -66,43 +66,46 @@
 
 def __wrap_test(browser, test):
     global _test_count
 
     _test_count += 1
 
     if _browser_pool is None:
-        raise RuntimeError("Please call autoparaselenium.configure() before creating tests")
+        raise RuntimeError(
+            "Please call autoparaselenium.configure() before creating tests"
+        )
 
     def inner():
         global _test_count
 
         try:
             _test_count -= 1
             driver = _browser_pool.acquire(browser)
-            driver.get("data:,") # initialize driver website
+            driver.get("data:,")  # initialize driver website
             test(driver)
         finally:
             with suppress(Exception):
                 _browser_pool.release(driver)
 
             if _test_count == 0:
-                time.sleep(0.10) # idk but seems like it needs a bit of time before you can close the pool
+                time.sleep(
+                    0.10
+                )  # idk but seems like it needs a bit of time before you can close the pool
                 _browser_pool.clean_up()
 
-
     inner.__name__ = f"{test.__name__}__{'chrome' if browser is chrome else 'firefox'}"
     inner.__doc__ = test.__doc__
 
     return inner
 
 
 def __get_threads(args=sys.argv):
     if "--tests-per-worker" not in args:
         return 1
     tests_per_worker_idx = args.index("--tests-per-worker")
-    next_arg = "".join(args[tests_per_worker_idx + 1: tests_per_worker_idx + 2])
+    next_arg = "".join(args[tests_per_worker_idx + 1 : tests_per_worker_idx + 2])
     if next_arg == "auto":
         return os.cpu_count() // 2 + 1
     try:
         return int("0" + next_arg) // 2 + 1
     except ValueError:
         return 1
```

### Comparing `autoparaselenium-0.2.0/autoparaselenium/browser_pool.py` & `autoparaselenium-0.3.0/autoparaselenium/browser_pool.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from concurrent.futures import ThreadPoolExecutor
 from contextlib import suppress
-from threading import Lock
 from queue import Queue
+from threading import Lock
 
 from selenium import webdriver
 
-from autoparaselenium.models import Conf
 from autoparaselenium.browsers import chrome, firefox
+from autoparaselenium.models import Conf
+
 
 class BrowserPool:
     def __init__(self, conf: Conf, threads: int):
         self._conf = conf
         self._threads = threads
 
         self._chromes = Queue()
@@ -19,33 +20,28 @@
         with ThreadPoolExecutor(max_workers=threads) as pool:
             for driver in pool.map(self.__open_browser, [chrome] * threads):
                 self._chromes.put(driver)
 
             for driver in pool.map(self.__open_browser, [firefox] * threads):
                 self._firefoxes.put(driver)
 
-
     def acquire(self, browser):
         return self.__get_queue(browser).get(browser)
 
-
     def release(self, driver):
         browser = chrome if isinstance(driver, webdriver.Chrome) else firefox
         self.__get_queue(browser).put(driver)
 
-
     def __get_queue(self, browser):
         return self._chromes if browser is chrome else self._firefoxes
 
-
     def __open_browser(self, browser):
         driver = browser.get_selenium(self._conf.selenium_dir, self._conf)
         with suppress(Exception):
             driver.switch_to.window("1")
         return driver
 
-
     def clean_up(self):
         for q in [self._chromes, self._firefoxes]:
             while not q.empty():
                 driver = q.get()
                 driver.quit()
```

### Comparing `autoparaselenium-0.2.0/autoparaselenium/browsers/chrome.py` & `autoparaselenium-0.3.0/autoparaselenium/browsers/chrome.py`

 * *Files 18% similar despite different names*

```diff
@@ -61,22 +61,50 @@
     return browser
 
 
 def setup_driver(pwd: Path) -> None:
     chrome_version = __get_chrome_version()
     driver_version = __get_chromedriver_version(pwd)
     if driver_version is None or driver_version < chrome_version:
-        r = requests.get(
-            "https://chromedriver.storage.googleapis.com"
-            f"/LATEST_RELEASE_{chrome_version}"
-        )
-        version = r.text.strip()
-        if (pwd / "chromedriver").exists():
-            os.remove(pwd / "chromedriver")
-        __setup_driver(version)(pwd)
+        print(driver_version, chrome_version)
+        # chromedriver changed its LATEST_RELEASE_{version} api and download link
+        # for chrome >= 115
+        if chrome_version < 115:
+            r = requests.get(
+                "https://chromedriver.storage.googleapis.com"
+                f"/LATEST_RELEASE_{chrome_version}"
+            )
+            version = r.text.strip()
+            if (pwd / "chromedriver").exists():
+                os.remove(pwd / "chromedriver")
+            __setup_driver_old(version)(pwd)
+        else:
+            r = requests.get(
+                "https://googlechromelabs.github.io/chrome-for-testing/"
+                "latest-versions-per-milestone-with-downloads.json"
+            )
+            supported_platforms = {
+                "linux64": "linux",
+                "mac-x64": "darwin",
+                "win64": "win",
+            }
+            downloads = {
+                supported_platforms.get(entry["platform"]): [
+                    entry["url"],
+                    su.unzip,
+                ]
+                for entry in (
+                    r.json()["milestones"][str(chrome_version)]["downloads"][
+                        "chromedriver"
+                    ]
+                )
+            }
+            if (pwd / "chromedriver").exists():
+                os.remove(pwd / "chromedriver")
+            su.setup_driver(downloads, __platform_drivers, pwd)
         os.chmod(pwd / "chromedriver", stat.S_IEXEC)
 
 
 def __get_chromedriver_version(pwd: Path) -> Optional[int]:
     with suppress(Exception):
         # version returned will be the major version
         p = sb.Popen([str(pwd / "chromedriver"), "--version"], stdout=sb.PIPE)
@@ -124,15 +152,15 @@
 
 __platform_binaries = {
     "darwin": "/Applications/Google Chrome.app/Contents/MacOS/Google Chrome",
     "win": os.path.expanduser(r"~\AppData\Local\Google\Chrome\Application\chrome.exe"),
     "linux": "/usr/bin/google-chrome",
 }
 
-__setup_driver = lambda version: partial(
+__setup_driver_old = lambda version: partial(
     su.setup_driver,
     {
         "win": [
             "https://chromedriver.storage.googleapis.com"
             f"/{version}/"
             "chromedriver_win32.zip",
             su.unzip,
```

### Comparing `autoparaselenium-0.2.0/autoparaselenium/browsers/firefox.py` & `autoparaselenium-0.3.0/autoparaselenium/browsers/firefox.py`

 * *Files identical despite different names*

### Comparing `autoparaselenium-0.2.0/autoparaselenium/setup_utils.py` & `autoparaselenium-0.3.0/autoparaselenium/setup_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,11 +33,19 @@
     location.touch()
 
 
 def setup_driver(platform_install, platform_drivers, pwd: Path) -> None:
     if not Path(pwd / platform_drivers[platform]).exists():
         __download_and_extract(*platform_install[platform], pwd)
 
+    # sometimes webdriver is nested in a folder after zip extraction
+    if not Path(pwd / platform_drivers[platform]).exists():
+        (pwd / platform_drivers[platform]).hardlink_to(
+            next(pwd.rglob(platform_drivers[platform]))
+        )
+
 
-def __download_and_extract(url: str, extract: Callable[[str, str], None], pwd: Path) -> None:
+def __download_and_extract(
+    url: str, extract: Callable[[str, str], None], pwd: Path
+) -> None:
     download(url, pwd / "temp")
     extract(pwd / "temp", pwd)
```

### Comparing `autoparaselenium-0.2.0/autoparaselenium.egg-info/PKG-INFO` & `autoparaselenium-0.3.0/autoparaselenium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoparaselenium
-Version: 0.2.0
+Version: 0.3.0
 Summary: A library to make parallel selenium tests that automatically download and setup webdrivers
 Author-email: Ronak Badhe <ronak.badhe@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autoparaselenium-0.2.0/autoparaselenium.egg-info/SOURCES.txt` & `autoparaselenium-0.3.0/autoparaselenium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autoparaselenium-0.2.0/pyproject.toml` & `autoparaselenium-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autoparaselenium-0.2.0/tests/test_browsers.py` & `autoparaselenium-0.3.0/tests/test_browsers.py`

 * *Files identical despite different names*

### Comparing `autoparaselenium-0.2.0/tests/test_everything.py` & `autoparaselenium-0.3.0/tests/test_everything.py`

 * *Files identical despite different names*

