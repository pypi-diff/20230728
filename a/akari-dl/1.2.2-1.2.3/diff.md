# Comparing `tmp/akari-dl-1.2.2.tar.gz` & `tmp/akari-dl-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akari-dl-1.2.2.tar", last modified: Mon Jul 24 23:43:33 2023, max compression
+gzip compressed data, was "akari-dl-1.2.3.tar", last modified: Fri Jul 28 20:33:22 2023, max compression
```

## Comparing `akari-dl-1.2.2.tar` & `akari-dl-1.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 23:43:33.354812 akari-dl-1.2.2/
--rw-rw-rw-   0        0        0     1235 2023-07-18 05:22:58.000000 akari-dl-1.2.2/LICENSE
--rw-rw-rw-   0        0        0      589 2023-07-24 23:43:33.353812 akari-dl-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     4541 2023-07-24 23:25:51.000000 akari-dl-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 23:43:33.337814 akari-dl-1.2.2/akari_dl/
--rw-rw-rw-   0        0        0     2792 2023-07-24 23:43:21.000000 akari-dl-1.2.2/akari_dl/__init__.py
--rw-rw-rw-   0        0        0     1829 2023-07-24 23:32:08.000000 akari-dl-1.2.2/akari_dl/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 23:43:33.352812 akari-dl-1.2.2/akari_dl/src/
--rw-rw-rw-   0        0        0        0 2023-07-24 23:42:55.000000 akari-dl-1.2.2/akari_dl/src/__init__.py
--rw-rw-rw-   0        0        0     2983 2023-07-24 23:38:21.000000 akari-dl-1.2.2/akari_dl/src/download_anime.py
--rw-rw-rw-   0        0        0      368 2023-07-24 23:25:51.000000 akari-dl-1.2.2/akari_dl/src/log_response.py
--rw-rw-rw-   0        0        0     1106 2023-07-24 23:38:25.000000 akari-dl-1.2.2/akari_dl/src/resolve_anime.py
--rw-rw-rw-   0        0        0     1231 2023-07-24 23:38:29.000000 akari-dl-1.2.2/akari_dl/src/resolve_website.py
--rw-rw-rw-   0        0        0     1155 2023-07-24 23:33:26.000000 akari-dl-1.2.2/akari_dl/src/website.py
-drwxrwxrwx   0        0        0        0 2023-07-24 23:43:33.347811 akari-dl-1.2.2/akari_dl.egg-info/
--rw-rw-rw-   0        0        0      589 2023-07-24 23:43:33.000000 akari-dl-1.2.2/akari_dl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2023-07-24 23:43:33.000000 akari-dl-1.2.2/akari_dl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 23:43:33.000000 akari-dl-1.2.2/akari_dl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-24 23:43:33.000000 akari-dl-1.2.2/akari_dl.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-07-24 23:43:33.000000 akari-dl-1.2.2/akari_dl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-24 23:43:33.000000 akari-dl-1.2.2/akari_dl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 23:43:33.354812 akari-dl-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      802 2023-07-24 23:43:27.000000 akari-dl-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 20:33:22.552896 akari-dl-1.2.3/
+-rw-rw-rw-   0        0        0     1235 2023-07-18 05:22:58.000000 akari-dl-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0      589 2023-07-28 20:33:22.551900 akari-dl-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4422 2023-07-27 00:56:35.000000 akari-dl-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 20:33:22.538109 akari-dl-1.2.3/akari_dl/
+-rw-rw-rw-   0        0        0     2792 2023-07-24 23:43:21.000000 akari-dl-1.2.3/akari_dl/__init__.py
+-rw-rw-rw-   0        0        0     1836 2023-07-28 20:28:36.000000 akari-dl-1.2.3/akari_dl/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 20:33:22.550897 akari-dl-1.2.3/akari_dl/src/
+-rw-rw-rw-   0        0        0      262 2023-07-28 20:28:10.000000 akari-dl-1.2.3/akari_dl/src/__init__.py
+-rw-rw-rw-   0        0        0     2913 2023-07-28 20:30:32.000000 akari-dl-1.2.3/akari_dl/src/download_anime.py
+-rw-rw-rw-   0        0        0      368 2023-07-24 23:25:51.000000 akari-dl-1.2.3/akari_dl/src/log_response.py
+-rw-rw-rw-   0        0        0     1078 2023-07-28 20:30:12.000000 akari-dl-1.2.3/akari_dl/src/resolve_anime.py
+-rw-rw-rw-   0        0        0     1210 2023-07-28 20:29:47.000000 akari-dl-1.2.3/akari_dl/src/resolve_website.py
+-rw-rw-rw-   0        0        0     1064 2023-07-28 20:29:35.000000 akari-dl-1.2.3/akari_dl/src/website.py
+drwxrwxrwx   0        0        0        0 2023-07-28 20:33:22.545626 akari-dl-1.2.3/akari_dl.egg-info/
+-rw-rw-rw-   0        0        0      589 2023-07-28 20:33:22.000000 akari-dl-1.2.3/akari_dl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-07-28 20:33:22.000000 akari-dl-1.2.3/akari_dl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 20:33:22.000000 akari-dl-1.2.3/akari_dl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-28 20:33:22.000000 akari-dl-1.2.3/akari_dl.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-07-28 20:33:22.000000 akari-dl-1.2.3/akari_dl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-28 20:33:22.000000 akari-dl-1.2.3/akari_dl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 20:33:22.552896 akari-dl-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      802 2023-07-28 20:32:07.000000 akari-dl-1.2.3/setup.py
```

### Comparing `akari-dl-1.2.2/LICENSE` & `akari-dl-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `akari-dl-1.2.2/PKG-INFO` & `akari-dl-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akari-dl
-Version: 1.2.2
+Version: 1.2.3
 Summary: A lightweight and open-source anime downloading CLI.
 Home-page: https://github.com/keisanng/akari-dl
 Author: keisan
 Author-email: <keisan@skiff.com>
 Project-URL: Documentation, https://github.com/keisanng/akari-dl#readme
 Project-URL: Tracker, https://github.com/users/keisanng/projects/3
 Requires-Python: >=3.10
```

### Comparing `akari-dl-1.2.2/README.md` & `akari-dl-1.2.3/README.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-# akari-dl
-
-A lightweight and open-source anime downloading CLI.
-
-1. [akari-dl](#akari-dl)
-   1. [About](#about)
-   2. [Installation](#installation)
-      1. [pypi/pip](#pypipip)
-      2. [Build](#build)
-   3. [Usage](#usage)
-      1. [Arguments](#arguments)
-         1. [Positional](#positional)
-         2. [Optional](#optional)
-      2. [Configuration](#configuration)
-   4. [Supported Websites](#supported-websites)
-   5. [Known Limitations](#known-limitations)
-      1. [Video Downloaded in Bad Resolution or Wrong Format](#video-downloaded-in-bad-resolution-or-wrong-format)
-   6. [Disclaimer](#disclaimer)
-
-## About
-
-akari-dl downloads anime video files from direct download and streaming websites based on user configuration to avoid more annoying downloading methods like torrenting and manually downloading.
-
-## Installation
-
-Granted you have [Python 3.10+](https://www.python.org/downloads/) in your [PATH](https://realpython.com/add-python-to-path/).
-
-### pypi/pip
-
-```bash
-pip install -U akari-dl
-```
-
-### Build
-
-1. `git clone https://github.com/keisanng/akari-dl.git`
-2. `cd akari-dl`
-3. [Activate virtual environment](https://python.land/virtual-environments/virtualenv#Python_venv_activation)
-4. `py -m venv .venv`
-5. `pip install requests-html`
-6. `python setup.py sdist`
-7. `pip install .` (or path to akari-dl if you're not in it anymore)
-
-## Usage
-
-User
-
-```bash
-akari-dl tokyoinsider "hidamari sketch" path/to/output
-```
-
-Advanced user (see [configuration](#configuration))
-
-```bash
-akari-dl "hidamari sketch"
-```
-
-Developer
-
-```bash
-py -m akari_dl tokyoinsider "hidamari sketch" path/to/output
-```
-
-In your output path, akari-dl will create a folder where all the desired anime episodes will be.
-
-### Arguments
-
-#### Positional
-
-1. `website`
-   - Specify the name of what website to direct-download anime from (see [supported websites](https://github.com/keisanng/akari-dl#supported-websites).)
-2. `anime`
-   - Specify what anime to download by title (in [Romaji](https://en.wikipedia.org/wiki/Romanization_of_Japanese).)
-3. `output`
-   - Specify path to output downloaded video files to.
-
-#### Optional
-
-- **Help**
-  - `-h`; `--help`
-- **Version**
-  - `-v`; `--version`
-  - Print the current version of akari-dl.
-- **Episodes**
-  - `-e`; `--episodes`
-  - Specify the amount of episodes to download (downloads all if not specified) [NOT YET IMPLEMENTED.]
-- **Specials**
-  - `-s`; `--specials`
-  - Enable downloading of special episodes (only works with websites that list the specials on the same page as the episodes.)
-- **Debug**
-  - `-d`; `--d`
-  - Run akari-dl in debug mode; log each connections html body and http headers and prints logging messages.
-
-### Configuration
-
-Upon initialization, akari-dl will ask you where to store the config file and when given a path it will create the config file. Using the configuration file, you can shorten akari-dl usage from `akari-dl <website> <anime> <output>` to `akari-dl <anime>` by specifying default website and output path as well as being able to specify other default behaviors such as debug mode.
-
-## Supported Websites
-
-1. [<img src="https://www.tokyoinsider.com/favicon.ico" style="width:24px;"/> Tokyoinsider](https://www.tokyoinsider.com)
-2. [<img src="https://chauthanh.info/favicon.ico" style="width:24px;"/> ChauThanh](https://chaunthanh.info)
-
-[*Request a **ddl** site here.*](https://github.com/keisanng/akari-dl/issues)
-
-*Or if you're an administrator of a site and want it removed from the project **[contact me](mailto:keisan@skiff.com)**.*
-
-## Known Limitations
-
-### Video Downloaded in Bad Resolution or Wrong Format
-
-As of now, akari-dl will scrape the first link in the markup of the anime's page for video file. In the near future there will be options to download for file format or resolution specifically - just not now.
-
-## Disclaimer
-
-akari-dl tries to hide it's scraping behavior.
-
-> The core aim of this project is to co-relate automation and efficiency to extract what is provided to a user on the internet. All content available through the project is hosted by external non-affiliated sources. All content served through this project is publicly accessible. If your site is listed in this project, the code is pretty much public. Take necessary measures to counter the exploits used to extract content in your site.
-
-*Applicable excerpt from <https://github.com/justfoolingaround/animdl/blob/master/disclaimer.md>.*
+# akari-dl
+
+A lightweight and open-source anime downloading CLI.
+
+1. [akari-dl](#akari-dl)
+   1. [About](#about)
+   2. [Installation](#installation)
+      1. [pypi/pip](#pypipip)
+      2. [Build](#build)
+   3. [Usage](#usage)
+      1. [Arguments](#arguments)
+         1. [Positional](#positional)
+         2. [Optional](#optional)
+      2. [Configuration](#configuration)
+   4. [Supported Websites](#supported-websites)
+   5. [Known Limitations](#known-limitations)
+      1. [Video Downloaded in Bad Resolution or Wrong Format](#video-downloaded-in-bad-resolution-or-wrong-format)
+   6. [Disclaimer](#disclaimer)
+
+## About
+
+akari-dl downloads anime video files from direct download and streaming websites based on user configuration to avoid more annoying downloading methods like torrenting and manually downloading.
+
+## Installation
+
+Granted you have [Python 3.10+](https://www.python.org/downloads/) in your [PATH](https://realpython.com/add-python-to-path/).
+
+### pypi/pip
+
+```bash
+pip install -U akari-dl
+```
+
+### Build
+
+1. `git clone https://github.com/keisanng/akari-dl.git`
+2. `cd akari-dl`
+3. [Activate virtual environment](https://python.land/virtual-environments/virtualenv#Python_venv_activation)
+4. `py -m venv .venv`
+5. `pip install requests-html`
+6. `python setup.py sdist`
+7. `pip install .` (or path to akari-dl if you're not in it anymore)
+
+## Usage
+
+User
+
+```bash
+akari-dl tokyoinsider "hidamari sketch" path/to/output
+```
+
+Advanced user (see [configuration](#configuration))
+
+```bash
+akari-dl "hidamari sketch"
+```
+
+Developer
+
+```bash
+py -m akari_dl tokyoinsider "hidamari sketch" path/to/output
+```
+
+In your output path, akari-dl will create a folder where all the desired anime episodes will be.
+
+### Arguments
+
+#### Positional
+
+1. `website`
+   - Specify the name of what website to direct-download anime from (see [supported websites](https://github.com/keisanng/akari-dl#supported-websites).)
+2. `anime`
+   - Specify what anime to download by title (in [Romaji](https://en.wikipedia.org/wiki/Romanization_of_Japanese).)
+3. `output`
+   - Specify path to output downloaded video files to.
+
+#### Optional
+
+- **Help**
+  - `-h`; `--help`
+- **Version**
+  - `-v`; `--version`
+  - Print the current version of akari-dl.
+- **Episodes**
+  - `-e`; `--episodes`
+  - Specify the amount of episodes to download (downloads all if not specified) [NOT YET IMPLEMENTED.]
+- **Specials**
+  - `-s`; `--specials`
+  - Enable downloading of special episodes (only works with websites that list the specials on the same page as the episodes.)
+- **Debug**
+  - `-d`; `--d`
+  - Run akari-dl in debug mode; log each connections html body and http headers and prints logging messages.
+
+### Configuration
+
+Upon initialization, akari-dl will ask you where to store the config file and when given a path it will create the config file. Using the configuration file, you can shorten akari-dl usage from `akari-dl <website> <anime> <output>` to `akari-dl <anime>` by specifying default website and output path as well as being able to specify other default behaviors such as debug mode.
+
+## Supported Websites
+
+1. [<img src="https://www.tokyoinsider.com/favicon.ico" style="width:24px;"/> Tokyoinsider](https://www.tokyoinsider.com)
+2. [<img src="https://chauthanh.info/favicon.ico" style="width:24px;"/> ChauThanh](https://chaunthanh.info)
+
+[*Request a **ddl** site here.*](https://github.com/keisanng/akari-dl/issues)
+
+*Or if you're an administrator of a site and want it removed from the project **[contact me](mailto:keisan@skiff.com)**.*
+
+## Known Limitations
+
+### Video Downloaded in Bad Resolution or Wrong Format
+
+As of now, akari-dl will scrape the first link in the markup of the anime's page for video file. In the near future there will be options to download for file format or resolution specifically - just not now.
+
+## Disclaimer
+
+akari-dl tries to hide it's scraping behavior.
+
+> The core aim of this project is to co-relate automation and efficiency to extract what is provided to a user on the internet. All content available through the project is hosted by external non-affiliated sources. All content served through this project is publicly accessible. If your site is listed in this project, the code is pretty much public. Take necessary measures to counter the exploits used to extract content in your site.
+
+*Applicable excerpt from <https://github.com/justfoolingaround/animdl/blob/master/disclaimer.md>.*
```

### Comparing `akari-dl-1.2.2/akari_dl/__init__.py` & `akari-dl-1.2.3/akari_dl/__init__.py`

 * *Files identical despite different names*

### Comparing `akari-dl-1.2.2/akari_dl/__main__.py` & `akari-dl-1.2.3/akari_dl/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from . import conf_parser, arg_parser, logger
-from .src.website import Website
+from akari_dl import conf_parser, arg_parser, logger
+from akari_dl.src import Website
 
 def main():
   args = arg_parser.parse_args()
 
   if args.debug or conf_parser["debug"]:
     logger.basicConfig(level=logger.NOTSET)
```

### Comparing `akari-dl-1.2.2/akari_dl/src/download_anime.py` & `akari-dl-1.2.3/akari_dl/src/download_anime.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,14 @@
   folder_path = os.path.join(self.output_path, anime_slug)
 
   download_episodes(self, folder_path, episodes_regular)
 
   if self.specials_enabled is True:
     folder_path = os.path.join(self.output_path, anime_slug, "Specials")
 
-    download_episodes(self, folder_path, episodes_special)
-    # try:
-      # download_episodes(self, folder_path, episodes_special)
-    # except Exception as error:
-      # print(f"Download failed: {error}")
-      # exit()
+    try:
+      download_episodes(self, folder_path, episodes_special)
+    except Exception as error:
+      print(f"Download failed: {error}")
+      exit()
 
   return f"Finished downloading {self.anime}."
```

### Comparing `akari-dl-1.2.2/akari_dl/src/resolve_anime.py` & `akari-dl-1.2.3/akari_dl/src/resolve_anime.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from akari_dl import conf_parser
-from akari_dl.src.log_response import log_response
+import akari_dl
+from akari_dl import src  
 
 def resolve_anime(self):
   """
     Verify user-specified anime exists on user-specified website via resolved url
     and return the link of the first entry of the anime's name on the website.
   """
   print(f"Searching for \"{self.anime}\"...")
 
   self.response = self.session.get(f"{self.url}/{self.search}{self.anime}", timeout=30)
-  if conf_parser["debug"]:
-    log_response(self.response)
+  if akari_dl.conf_parser["debug"]:
+    src.log_response(self.response)
 
   try:
     anchors = self.response.html.find(self.anchors[0])
     if self.name == "tokyoinsider":
       anchors += self.response.html.find("table > tr > .c_h2b > a")
   except Exception:
     print("Anime not found.")
```

### Comparing `akari-dl-1.2.2/akari_dl/src/resolve_website.py` & `akari-dl-1.2.3/akari_dl/src/resolve_website.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from akari_dl import conf_parser
-from akari_dl.src.log_response import log_response
+import akari_dl
+from akari_dl import src
 
 def resolve_website(self):
   """
     Resolve working url and login for user-specified website.
   """
   print(f"Connecting to {self.name}...")
 
@@ -20,21 +20,21 @@
       except Exception:
         try:
           print(f"Failed to connect to {self.name} via https://{url}... trying https://{self.domains[i]}.")
         except IndexError:
           print(f"Failed to connect to {self.name}.")
           exit()
   else:
-    if conf_parser["debug"]:
+    if akari_dl.conf_parser["debug"]:
       self.response = self.session.get(f"https://{self.domains}")
     else:
       try:
         self.response = self.session.get(f"https://{self.domains}")
       except Exception:
         print(f"Failed to connect to {self.name}.")
         exit()
 
-  if conf_parser["debug"]:
-    log_response(self.response)
+  if akari_dl.conf_parser["debug"]:
+    src.log_response(self.response)
   print(f"Connected to {self.response.url[:-1]}.")
 
   return self.response.url[:-1]
```

### Comparing `akari-dl-1.2.2/akari_dl/src/website.py` & `akari-dl-1.2.3/akari_dl/src/website.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # pylint: disable=missing-module-docstring, missing-class-docstring, missing-function-docstring, not-callable
 
 from os import PathLike
 import requests_html
 
-from resolve_website import resolve_website
-from resolve_anime import resolve_anime
-from download_anime import download_anime
+from akari_dl import src
 
 class Website:
   def __init__(self, name=str, anime=str, output=PathLike, episodes=int, specials=bool, domains=str|tuple, search=str, anchors=tuple):
 
     self.name = name
     self.anime = anime
     self.output_path = output
@@ -23,16 +21,16 @@
 
     self.url = str
     self.endpoint = None
     self.session  = requests_html.HTMLSession()
 
 
   def resolve_website(self):
-    self.url = resolve_website(self)
+    self.url = src.resolve_website(self)
 
 
   def resolve_anime(self):
-    self.endpoint = resolve_anime(self)
+    self.endpoint = src.resolve_anime(self)
 
 
   def download_anime(self):
-    download_anime(self)
+    src.download_anime(self)
```

### Comparing `akari-dl-1.2.2/akari_dl.egg-info/PKG-INFO` & `akari-dl-1.2.3/akari_dl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akari-dl
-Version: 1.2.2
+Version: 1.2.3
 Summary: A lightweight and open-source anime downloading CLI.
 Home-page: https://github.com/keisanng/akari-dl
 Author: keisan
 Author-email: <keisan@skiff.com>
 Project-URL: Documentation, https://github.com/keisanng/akari-dl#readme
 Project-URL: Tracker, https://github.com/users/keisanng/projects/3
 Requires-Python: >=3.10
```

### Comparing `akari-dl-1.2.2/setup.py` & `akari-dl-1.2.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
   name="akari-dl",
-  version="1.2.2",
+  version="1.2.3",
   author="keisan",
   author_email="<keisan@skiff.com>",
   description="A lightweight and open-source anime downloading CLI.",
   long_description="akari-dl downloads anime video files from direct download websites based on user configuration to avoid more annoying downloading methods like torrenting and manually downloading.",
   url="https://github.com/keisanng/akari-dl",
   project_urls={
     "Documentation": "https://github.com/keisanng/akari-dl#readme",
```

