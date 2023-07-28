# Comparing `tmp/mozversion-2.3.0.tar.gz` & `tmp/mozversion-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mozversion-2.3.0.tar", last modified: Tue Mar 10 22:14:41 2020, max compression
+gzip compressed data, was "dist/mozversion-2.4.0.tar", last modified: Fri Jul 28 13:53:04 2023, max compression
```

## Comparing `mozversion-2.3.0.tar` & `mozversion-2.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 gbrown    (1000) gbrown    (1000)        0 2020-03-10 22:14:41.000000 mozversion-2.3.0/
--rw-r--r--   0 gbrown    (1000) gbrown    (1000)       67 2020-03-10 22:14:41.000000 mozversion-2.3.0/setup.cfg
-drwxr-xr-x   0 gbrown    (1000) gbrown    (1000)        0 2020-03-10 22:14:41.000000 mozversion-2.3.0/mozversion/
--rw-r--r--   0 gbrown    (1000) gbrown    (1000)      914 2019-12-21 01:18:39.000000 mozversion-2.3.0/mozversion/errors.py
--rw-r--r--   0 gbrown    (1000) gbrown    (1000)     5185 2019-12-21 01:18:39.000000 mozversion-2.3.0/mozversion/mozversion.py
--rw-r--r--   0 gbrown    (1000) gbrown    (1000)      345 2019-12-21 01:18:39.000000 mozversion-2.3.0/mozversion/__init__.py
--rw-r--r--   0 gbrown    (1000) gbrown    (1000)      486 2020-03-10 22:14:41.000000 mozversion-2.3.0/PKG-INFO
--rw-r--r--   0 gbrown    (1000) gbrown    (1000)     1139 2020-03-10 22:11:46.000000 mozversion-2.3.0/setup.py
-drwxr-xr-x   0 gbrown    (1000) gbrown    (1000)        0 2020-03-10 22:14:41.000000 mozversion-2.3.0/mozversion.egg-info/
--rw-r--r--   0 gbrown    (1000) gbrown    (1000)      326 2020-03-10 22:14:40.000000 mozversion-2.3.0/mozversion.egg-info/SOURCES.txt
--rw-r--r--   0 gbrown    (1000) gbrown    (1000)        1 2020-03-10 22:14:40.000000 mozversion-2.3.0/mozversion.egg-info/not-zip-safe
--rw-r--r--   0 gbrown    (1000) gbrown    (1000)       11 2020-03-10 22:14:40.000000 mozversion-2.3.0/mozversion.egg-info/top_level.txt
--rw-r--r--   0 gbrown    (1000) gbrown    (1000)       24 2020-03-10 22:14:40.000000 mozversion-2.3.0/mozversion.egg-info/requires.txt
--rw-r--r--   0 gbrown    (1000) gbrown    (1000)        1 2020-03-10 22:14:40.000000 mozversion-2.3.0/mozversion.egg-info/dependency_links.txt
--rw-r--r--   0 gbrown    (1000) gbrown    (1000)       95 2020-03-10 22:14:40.000000 mozversion-2.3.0/mozversion.egg-info/entry_points.txt
--rw-r--r--   0 gbrown    (1000) gbrown    (1000)      486 2020-03-10 22:14:40.000000 mozversion-2.3.0/mozversion.egg-info/PKG-INFO
+drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2023-07-28 13:53:04.000000 mozversion-2.4.0/
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      475 2023-07-28 13:53:04.000000 mozversion-2.4.0/PKG-INFO
+drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2023-07-28 13:53:04.000000 mozversion-2.4.0/mozversion/
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      304 2023-03-10 23:28:57.000000 mozversion-2.4.0/mozversion/__init__.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      873 2023-03-10 23:28:57.000000 mozversion-2.4.0/mozversion/errors.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     5221 2023-05-11 19:05:22.000000 mozversion-2.4.0/mozversion/mozversion.py
+drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2023-07-28 13:53:04.000000 mozversion-2.4.0/mozversion.egg-info/
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      475 2023-07-28 13:53:04.000000 mozversion-2.4.0/mozversion.egg-info/PKG-INFO
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      326 2023-07-28 13:53:04.000000 mozversion-2.4.0/mozversion.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)        1 2023-07-28 13:53:04.000000 mozversion-2.4.0/mozversion.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       95 2023-07-28 13:53:04.000000 mozversion-2.4.0/mozversion.egg-info/entry_points.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)        1 2023-07-28 13:53:04.000000 mozversion-2.4.0/mozversion.egg-info/not-zip-safe
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       24 2023-07-28 13:53:04.000000 mozversion-2.4.0/mozversion.egg-info/requires.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       11 2023-07-28 13:53:04.000000 mozversion-2.4.0/mozversion.egg-info/top_level.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       67 2023-07-28 13:53:04.000000 mozversion-2.4.0/setup.cfg
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     1058 2023-07-28 13:41:20.000000 mozversion-2.4.0/setup.py
```

### Comparing `mozversion-2.3.0/mozversion/errors.py` & `mozversion-2.4.0/mozversion/errors.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
 
 class VersionError(Exception):
-
     def __init__(self, message):
         Exception.__init__(self, message)
 
 
 class AppNotFoundError(VersionError):
     """Exception for the application not found"""
 
@@ -18,15 +15,15 @@
         VersionError.__init__(self, message)
 
 
 class LocalAppNotFoundError(AppNotFoundError):
     """Exception for local application not found"""
 
     def __init__(self, path):
-        AppNotFoundError.__init__(self, 'Application not found at: %s' % path)
+        AppNotFoundError.__init__(self, "Application not found at: %s" % path)
 
 
 class RemoteAppNotFoundError(AppNotFoundError):
     """Exception for remote application not found"""
 
     def __init__(self, message):
         AppNotFoundError.__init__(self, message)
```

### Comparing `mozversion-2.3.0/mozversion/mozversion.py` & `mozversion-2.4.0/mozversion/mozversion.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,154 +1,153 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
 import argparse
 import io
 import os
-from six.moves import configparser
 import sys
 import zipfile
 
 import mozlog
+from six.moves import configparser
 
 from mozversion import errors
 
-
-INI_DATA_MAPPING = (('application', 'App'), ('platform', 'Build'))
+INI_DATA_MAPPING = (("application", "App"), ("platform", "Build"))
 
 
 class Version(object):
-
     def __init__(self):
         self._info = {}
-        self._logger = mozlog.get_default_logger(component='mozversion')
+        self._logger = mozlog.get_default_logger(component="mozversion")
         if not self._logger:
-            self._logger = mozlog.unstructured.getLogger('mozversion')
+            self._logger = mozlog.unstructured.getLogger("mozversion")
 
     def get_gecko_info(self, path):
         for type, section in INI_DATA_MAPPING:
             config_file = os.path.join(path, "%s.ini" % type)
             if os.path.exists(config_file):
-                self._parse_ini_file(open(config_file), type, section)
+                try:
+                    with open(config_file) as fp:
+                        self._parse_ini_file(fp, type, section)
+                except OSError:
+                    self._logger.warning("Unable to read %s" % config_file)
             else:
-                self._logger.warning('Unable to find %s' % config_file)
+                self._logger.warning("Unable to find %s" % config_file)
 
     def _parse_ini_file(self, fp, type, section):
         config = configparser.RawConfigParser()
-        config.readfp(fp)
-        name_map = {'codename': 'display_name',
-                    'milestone': 'version',
-                    'sourcerepository': 'repository',
-                    'sourcestamp': 'changeset'}
+        config.read_file(fp)
+        name_map = {
+            "codename": "display_name",
+            "milestone": "version",
+            "sourcerepository": "repository",
+            "sourcestamp": "changeset",
+        }
         for key, value in config.items(section):
             name = name_map.get(key, key).lower()
-            self._info['%s_%s' % (type, name)] = config.has_option(
-                section, key) and config.get(section, key) or None
+            self._info["%s_%s" % (type, name)] = (
+                config.has_option(section, key) and config.get(section, key) or None
+            )
 
-        if not self._info.get('application_display_name'):
-            self._info['application_display_name'] = \
-                self._info.get('application_name')
+        if not self._info.get("application_display_name"):
+            self._info["application_display_name"] = self._info.get("application_name")
 
 
 class LocalFennecVersion(Version):
-
     def __init__(self, path, **kwargs):
         Version.__init__(self, **kwargs)
         self.get_gecko_info(path)
 
     def get_gecko_info(self, path):
-        archive = zipfile.ZipFile(path, 'r')
+        archive = zipfile.ZipFile(path, "r")
         archive_list = archive.namelist()
         for type, section in INI_DATA_MAPPING:
             filename = "%s.ini" % type
             if filename in archive_list:
-                fp = io.TextIOWrapper(archive.open(filename))
-                self._parse_ini_file(fp, type, section)
+                with io.TextIOWrapper(archive.open(filename)) as fp:
+                    self._parse_ini_file(fp, type, section)
             else:
-                self._logger.warning('Unable to find %s' % filename)
+                self._logger.warning("Unable to find %s" % filename)
 
         if "package-name.txt" in archive_list:
-            fp = io.TextIOWrapper(archive.open("package-name.txt"))
-            self._info["package_name"] = fp.readlines()[0].strip()
+            with io.TextIOWrapper(archive.open("package-name.txt")) as fp:
+                self._info["package_name"] = fp.readlines()[0].strip()
 
 
 class LocalVersion(Version):
-
     def __init__(self, binary, **kwargs):
         Version.__init__(self, **kwargs)
 
         if binary:
             # on Windows, the binary may be specified with or without the
             # .exe extension
-            if not os.path.exists(binary) and not os.path.exists(binary +
-                                                                 '.exe'):
-                raise IOError('Binary path does not exist: %s' % binary)
+            if not os.path.exists(binary) and not os.path.exists(binary + ".exe"):
+                raise IOError("Binary path does not exist: %s" % binary)
             path = os.path.dirname(os.path.realpath(binary))
         else:
             path = os.getcwd()
 
         if not self.check_location(path):
-            if sys.platform == 'darwin':
-                resources_path = os.path.join(os.path.dirname(path),
-                                              'Resources')
+            if sys.platform == "darwin":
+                resources_path = os.path.join(os.path.dirname(path), "Resources")
                 if self.check_location(resources_path):
                     path = resources_path
                 else:
                     raise errors.LocalAppNotFoundError(path)
 
             else:
                 raise errors.LocalAppNotFoundError(path)
 
         self.get_gecko_info(path)
 
     def check_location(self, path):
-        return (os.path.exists(os.path.join(path, 'application.ini'))
-                and os.path.exists(os.path.join(path, 'platform.ini')))
+        return os.path.exists(os.path.join(path, "application.ini")) and os.path.exists(
+            os.path.join(path, "platform.ini")
+        )
 
 
 def get_version(binary=None):
     """
     Returns the application version information as a dict. You can specify
     a path to the binary of the application or an Android APK file (to get
     version information for Firefox for Android). If this is omitted then the
     current directory is checked for the existance of an application.ini
     file.
 
     :param binary: Path to the binary for the application or Android APK file
     """
-    if binary and zipfile.is_zipfile(binary) and 'AndroidManifest.xml' in \
-       zipfile.ZipFile(binary, 'r').namelist():
+    if (
+        binary
+        and zipfile.is_zipfile(binary)
+        and "AndroidManifest.xml" in zipfile.ZipFile(binary, "r").namelist()
+    ):
         version = LocalFennecVersion(binary)
     else:
         version = LocalVersion(binary)
 
     for (key, value) in sorted(version._info.items()):
         if value:
-            version._logger.info('%s: %s' % (key, value))
+            version._logger.info("%s: %s" % (key, value))
 
     return version._info
 
 
 def cli(args=sys.argv[1:]):
     parser = argparse.ArgumentParser(
-        description='Display version information for Mozilla applications')
-    parser.add_argument(
-        '--binary',
-        help='path to application binary or apk')
+        description="Display version information for Mozilla applications"
+    )
+    parser.add_argument("--binary", help="path to application binary or apk")
     mozlog.commandline.add_logging_group(
-        parser,
-        include_formatters=mozlog.commandline.TEXT_FORMATTERS
+        parser, include_formatters=mozlog.commandline.TEXT_FORMATTERS
     )
 
     args = parser.parse_args()
 
-    mozlog.commandline.setup_logging(
-        'mozversion', args, {'mach': sys.stdout})
+    mozlog.commandline.setup_logging("mozversion", args, {"mach": sys.stdout})
 
     get_version(binary=args.binary)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     cli()
```

### Comparing `mozversion-2.3.0/setup.py` & `mozversion-2.4.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
 from setuptools import setup
 
-PACKAGE_VERSION = '2.3.0'
+PACKAGE_VERSION = "2.4.0"
 
 
-setup(name='mozversion',
-      version=PACKAGE_VERSION,
-      description='Library to get version information for applications',
-      long_description="see https://firefox-source-docs.mozilla.org/mozbase/index.html",
-      classifiers=['Programming Language :: Python :: 2.7',
-                   'Programming Language :: Python :: 3.5'],
-      keywords='mozilla',
-      author='Mozilla Automation and Testing Team',
-      author_email='tools@lists.mozilla.org',
-      url='https://wiki.mozilla.org/Auto-tools/Projects/Mozbase',
-      license='MPL',
-      packages=['mozversion'],
-      include_package_data=True,
-      zip_safe=False,
-      install_requires=['mozlog >= 6.0',
-                        'six >= 1.10.0'],
-      entry_points="""
+setup(
+    name="mozversion",
+    version=PACKAGE_VERSION,
+    description="Library to get version information for applications",
+    long_description="see https://firefox-source-docs.mozilla.org/mozbase/index.html",
+    classifiers=[
+        "Programming Language :: Python :: 2.7",
+        "Programming Language :: Python :: 3.5",
+    ],
+    keywords="mozilla",
+    author="Mozilla Automation and Testing Team",
+    author_email="tools@lists.mozilla.org",
+    url="https://wiki.mozilla.org/Auto-tools/Projects/Mozbase",
+    license="MPL",
+    packages=["mozversion"],
+    include_package_data=True,
+    zip_safe=False,
+    install_requires=["mozlog >= 6.0", "six >= 1.13.0"],
+    entry_points="""
       # -*- Entry points: -*-
       [console_scripts]
       mozversion = mozversion:cli
-      """)
+      """,
+)
```

