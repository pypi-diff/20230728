# Comparing `tmp/dnsblock_update-0.0.1.tar.gz` & `tmp/dnsblock_update-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnsblock_update-0.0.1.tar", last modified: Sat Apr 24 12:09:05 2021, max compression
+gzip compressed data, was "dnsblock_update-0.0.2.tar", last modified: Fri Jul 28 07:42:08 2023, max compression
```

## Comparing `dnsblock_update-0.0.1.tar` & `dnsblock_update-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-24 12:09:05.434079 dnsblock_update-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-04-24 12:08:50.000000 dnsblock_update-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1858 2021-04-24 12:09:05.434079 dnsblock_update-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      649 2021-04-24 12:08:50.000000 dnsblock_update-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      103 2021-04-24 12:08:50.000000 dnsblock_update-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-24 12:09:05.434079 dnsblock_update-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2460 2021-04-24 12:08:50.000000 dnsblock_update-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-24 12:09:05.434079 dnsblock_update-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-24 12:09:05.434079 dnsblock_update-0.0.1/src/dnsblock_update/
--rw-r--r--   0 runner    (1001) docker     (121)      692 2021-04-24 12:08:50.000000 dnsblock_update-0.0.1/src/dnsblock_update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       68 2021-04-24 12:08:50.000000 dnsblock_update-0.0.1/src/dnsblock_update/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2693 2021-04-24 12:08:50.000000 dnsblock_update-0.0.1/src/dnsblock_update/blocklist.py
--rw-r--r--   0 runner    (1001) docker     (121)      529 2021-04-24 12:08:50.000000 dnsblock_update-0.0.1/src/dnsblock_update/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-24 12:09:05.434079 dnsblock_update-0.0.1/src/dnsblock_update.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1858 2021-04-24 12:09:05.000000 dnsblock_update-0.0.1/src/dnsblock_update.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      382 2021-04-24 12:09:05.000000 dnsblock_update-0.0.1/src/dnsblock_update.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-24 12:09:05.000000 dnsblock_update-0.0.1/src/dnsblock_update.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-04-24 12:09:05.000000 dnsblock_update-0.0.1/src/dnsblock_update.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-04-24 12:09:05.000000 dnsblock_update-0.0.1/src/dnsblock_update.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:42:08.268038 dnsblock_update-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-28 07:41:52.000000 dnsblock_update-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-28 07:42:08.268038 dnsblock_update-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-28 07:41:52.000000 dnsblock_update-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-28 07:41:52.000000 dnsblock_update-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 07:42:08.268038 dnsblock_update-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-07-28 07:41:52.000000 dnsblock_update-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:42:08.268038 dnsblock_update-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:42:08.268038 dnsblock_update-0.0.2/src/dnsblock_update/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-28 07:41:52.000000 dnsblock_update-0.0.2/src/dnsblock_update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 07:41:52.000000 dnsblock_update-0.0.2/src/dnsblock_update/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-28 07:41:52.000000 dnsblock_update-0.0.2/src/dnsblock_update/blocklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-28 07:41:52.000000 dnsblock_update-0.0.2/src/dnsblock_update/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:42:08.268038 dnsblock_update-0.0.2/src/dnsblock_update.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-28 07:42:08.000000 dnsblock_update-0.0.2/src/dnsblock_update.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-28 07:42:08.000000 dnsblock_update-0.0.2/src/dnsblock_update.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 07:42:08.000000 dnsblock_update-0.0.2/src/dnsblock_update.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-28 07:42:08.000000 dnsblock_update-0.0.2/src/dnsblock_update.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-28 07:42:08.000000 dnsblock_update-0.0.2/src/dnsblock_update.egg-info/top_level.txt
```

### Comparing `dnsblock_update-0.0.1/LICENSE` & `dnsblock_update-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dnsblock_update-0.0.1/PKG-INFO` & `dnsblock_update-0.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,52 @@
 Metadata-Version: 2.1
 Name: dnsblock_update
-Version: 0.0.1
+Version: 0.0.2
 Summary: Blocklist Updater for DNS Masq
 Home-page: https://github.com/raynigon/dnsblock-update
 Author: Simon Schneider
 Author-email: dev@raynigon.com
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/raynigon/dnsblock-update/issues
-Project-URL: Funding, https://donate.pypi.org
-Project-URL: Say Thanks!, http://saythanks.io/to/example
-Project-URL: Source, https://github.com/pypa/sampleproject/
-Description: # dnsblock-update
-        Blocklist Updater for DNSmasq
-        
-        ## Usage
-        
-        ### Installation
-        
-        Run the following command:
-        ```pip3 install dnsblock_update```
-        
-        ### Configuration
-        
-        Create a configuration file with the following content:
-        ```yaml
-        dnsmasq: 
-          path: "result.conf"   # Generated DNSMasq configuration
-        repository:
-          path: "./repo/"       # Path to the cache repository used by the updater
-        blocklists:
-          - name: "notracking"                      # name of the blocklist
-            url: https://example.com/blacklist.txt  # url of the blocklist
-        ```
-        
-        ### Execution
-        
-        Create a cronjob:
-        ```
-        0 2 * * * /usr/bin/python3 -m dnsblock_update /etc/dnsblock_update/config.yml
-        ```
-        
+Project-URL: Source, https://github.com/raynigon/dnsblock-update/
 Keywords: dnsmasq
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
+License-File: LICENSE
+
+# dnsblock-update
+Blocklist Updater for DNSmasq
+
+## Usage
+
+### Installation
+
+Run the following command:
+```pip3 install dnsblock_update```
+
+### Configuration
+
+Create a configuration file with the following content:
+```yaml
+dnsmasq: 
+  path: "result.conf"   # Generated DNSMasq configuration
+repository:
+  path: "./repo/"       # Path to the cache repository used by the updater
+blocklists:
+  - name: "notracking"                      # name of the blocklist
+    url: https://example.com/blacklist.txt  # url of the blocklist
+```
+
+### Execution
+
+Create a cronjob:
+```
+0 2 * * * /usr/bin/python3 -m dnsblock_update /etc/dnsblock_update/config.yml
+```
```

### Comparing `dnsblock_update-0.0.1/README.md` & `dnsblock_update-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dnsblock_update-0.0.1/setup.py` & `dnsblock_update-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name='dnsblock_update',
-    version='0.0.1',
+    version='0.0.2',
     author='Simon Schneider',
     author_email='dev@raynigon.com',
     description='Blocklist Updater for DNS Masq',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url = 'https://github.com/raynigon/dnsblock-update',
     classifiers=[
@@ -33,17 +33,15 @@
         'Programming Language :: Python :: 3.9',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent'
     ],
     keywords='dnsmasq',
     project_urls={
         'Bug Reports': 'https://github.com/raynigon/dnsblock-update/issues',
-        'Funding': 'https://donate.pypi.org',
-        'Say Thanks!': 'http://saythanks.io/to/example',
-        'Source': 'https://github.com/pypa/sampleproject/',
+        'Source': 'https://github.com/raynigon/dnsblock-update/',
     },
     python_requires='>=3.6, <4',
     install_requires=[
         'requests',
         'pyyaml'
     ],
     extras_require={
```

### Comparing `dnsblock_update-0.0.1/src/dnsblock_update/__init__.py` & `dnsblock_update-0.0.2/src/dnsblock_update/__init__.py`

 * *Files identical despite different names*

### Comparing `dnsblock_update-0.0.1/src/dnsblock_update/blocklist.py` & `dnsblock_update-0.0.2/src/dnsblock_update/blocklist.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import requests
 import re
 import os
 import json
 
 from typing import List
 
-BLOCKLIST_ENTRY_PATTERN=re.compile(r"address=/[A-z0-9-_.]*/#")
+BLOCKLIST_ENTRY_PATTERN=re.compile(r"(?:address=/[A-z0-9-_.]*/)|(?:server=/[A-z0-9-_.]*/)")
 
 class Blocklist:
 
     def __init__(self, name, url):
         self.name = name
         self.url = url
         self.etag = None
@@ -17,14 +17,18 @@
         self.entries = []
 
     def load(self, repository):
         repo_path = os.path.join(repository, self.name+".json")
         if os.path.exists(repo_path):
             self.__load_from_repo(repo_path)
             response=requests.head(self.url)
+            while response.status_code > 299 and response.status_code < 400:
+                response=requests.get(response.headers["location"])
+            if "etag" not in response.headers.keys():
+                raise Exception(f"Unable to check repository for {self.url} due to missing etag")
             etag = response.headers["etag"].replace("\"", "")
             if self.etag != etag:
                 print(f"E-Tag mismatch, stored {self.etag}, current {etag}")
                 self.header = ""
                 self.entries = []
                 self.__download(repository)
         else:
@@ -36,14 +40,20 @@
             data = json.load(file)
         self.etag = data["etag"]
         self.header = data["header"]
         self.entries = data["entries"]
 
     def __download(self, repository):
         response=requests.get(self.url)
+        while response.status_code > 299 and response.status_code < 400:
+            response=requests.get(response.headers["location"])
+        if response.status_code > 299:
+            raise Exception(f"Unable to download from {self.url} due to unexpected status {response.status_code}")
+        if "etag" not in response.headers.keys():
+            raise Exception(f"Unable to download from {self.url} due to missing etag")
         self.etag = response.headers["etag"].replace("\"", "")
         lines = response.text.splitlines()
         for line in lines:
             if self.__is_ignored(line):
                 continue
             if self.__is_header(line):
                 self.header += f"{line}\n"
@@ -51,14 +61,16 @@
             if self.__is_entry(line):
                 self.__add_entry(line)
                 continue
             print(f"Unknown Line Type: {line}\n")
         self.__reinvalidate_cache(repository)
 
     def __reinvalidate_cache(self, repository):
+        if not os.path.exists(repository):
+            os.makedirs(repository)
         repo_path = os.path.join(repository, self.name+".json")
         data = {
             "name": self.name,
             "url": self.url,
             "etag": self.etag,
             "header": self.header,
             "entries": self.entries
```

### Comparing `dnsblock_update-0.0.1/src/dnsblock_update/config.py` & `dnsblock_update-0.0.2/src/dnsblock_update/config.py`

 * *Files identical despite different names*

