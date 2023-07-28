# Comparing `tmp/mozInstall-2.0.1.tar.gz` & `tmp/mozInstall-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mozInstall-2.0.1.tar", last modified: Fri Nov 20 15:25:00 2020, max compression
+gzip compressed data, was "dist/mozInstall-2.1.0.tar", last modified: Fri Jul 28 13:42:55 2023, max compression
```

## Comparing `mozInstall-2.0.1.tar` & `mozInstall-2.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 wlach      (501) staff       (20)        0 2020-11-20 15:25:00.589648 mozInstall-2.0.1/
--rw-r--r--   0 wlach      (501) staff       (20)      810 2020-11-20 15:25:00.589766 mozInstall-2.0.1/PKG-INFO
-drwxr-xr-x   0 wlach      (501) staff       (20)        0 2020-11-20 15:25:00.587674 mozInstall-2.0.1/mozInstall.egg-info/
--rw-r--r--   0 wlach      (501) staff       (20)      810 2020-11-20 15:25:00.000000 mozInstall-2.0.1/mozInstall.egg-info/PKG-INFO
--rw-r--r--   0 wlach      (501) staff       (20)      305 2020-11-20 15:25:00.000000 mozInstall-2.0.1/mozInstall.egg-info/SOURCES.txt
--rw-r--r--   0 wlach      (501) staff       (20)        1 2020-11-20 15:25:00.000000 mozInstall-2.0.1/mozInstall.egg-info/dependency_links.txt
--rw-r--r--   0 wlach      (501) staff       (20)      254 2020-11-20 15:25:00.000000 mozInstall-2.0.1/mozInstall.egg-info/entry_points.txt
--rw-r--r--   0 wlach      (501) staff       (20)        1 2020-11-20 15:25:00.000000 mozInstall-2.0.1/mozInstall.egg-info/not-zip-safe
--rw-r--r--   0 wlach      (501) staff       (20)       47 2020-11-20 15:25:00.000000 mozInstall-2.0.1/mozInstall.egg-info/requires.txt
--rw-r--r--   0 wlach      (501) staff       (20)       11 2020-11-20 15:25:00.000000 mozInstall-2.0.1/mozInstall.egg-info/top_level.txt
-drwxr-xr-x   0 wlach      (501) staff       (20)        0 2020-11-20 15:25:00.588718 mozInstall-2.0.1/mozinstall/
--rw-r--r--   0 wlach      (501) staff       (20)      281 2020-11-18 17:09:47.000000 mozInstall-2.0.1/mozinstall/__init__.py
--rw-r--r--   0 wlach      (501) staff       (20)    11943 2020-11-18 17:09:48.000000 mozInstall-2.0.1/mozinstall/mozinstall.py
--rw-r--r--   0 wlach      (501) staff       (20)       67 2020-11-20 15:25:00.590180 mozInstall-2.0.1/setup.cfg
--rw-r--r--   0 wlach      (501) staff       (20)     2046 2020-11-18 17:19:29.000000 mozInstall-2.0.1/setup.py
+drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2023-07-28 13:42:55.000000 mozInstall-2.1.0/
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      799 2023-07-28 13:42:55.000000 mozInstall-2.1.0/PKG-INFO
+drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2023-07-28 13:42:55.000000 mozInstall-2.1.0/mozInstall.egg-info/
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      799 2023-07-28 13:42:55.000000 mozInstall-2.1.0/mozInstall.egg-info/PKG-INFO
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      305 2023-07-28 13:42:55.000000 mozInstall-2.1.0/mozInstall.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)        1 2023-07-28 13:42:55.000000 mozInstall-2.1.0/mozInstall.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      254 2023-07-28 13:42:55.000000 mozInstall-2.1.0/mozInstall.egg-info/entry_points.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)        1 2023-07-28 13:42:55.000000 mozInstall-2.1.0/mozInstall.egg-info/not-zip-safe
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       47 2023-07-28 13:42:55.000000 mozInstall-2.1.0/mozInstall.egg-info/requires.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       11 2023-07-28 13:42:55.000000 mozInstall-2.1.0/mozInstall.egg-info/top_level.txt
+drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2023-07-28 13:42:55.000000 mozInstall-2.1.0/mozinstall/
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      241 2023-03-10 23:28:57.000000 mozInstall-2.1.0/mozinstall/__init__.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)    14068 2023-03-10 23:28:57.000000 mozInstall-2.1.0/mozinstall/mozinstall.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       67 2023-07-28 13:42:55.000000 mozInstall-2.1.0/setup.cfg
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     2007 2023-07-28 13:41:20.000000 mozInstall-2.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `mozInstall-2.0.1/PKG-INFO` & `mozInstall-2.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: mozInstall
-Version: 2.0.1
+Version: 2.1.0
 Summary: package for installing and uninstalling Mozilla applications
 Home-page: https://wiki.mozilla.org/Auto-tools/Projects/Mozbase
 Author: Mozilla Automation and Tools team
 Author-email: tools@lists.mozilla.org
 License: MPL 2.0
-Description: see https://firefox-source-docs.mozilla.org/mozbase/index.html
 Keywords: mozilla
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
+
+see https://firefox-source-docs.mozilla.org/mozbase/index.html
+
```

### Comparing `mozInstall-2.0.1/mozInstall.egg-info/PKG-INFO` & `mozInstall-2.1.0/mozInstall.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: mozInstall
-Version: 2.0.1
+Version: 2.1.0
 Summary: package for installing and uninstalling Mozilla applications
 Home-page: https://wiki.mozilla.org/Auto-tools/Projects/Mozbase
 Author: Mozilla Automation and Tools team
 Author-email: tools@lists.mozilla.org
 License: MPL 2.0
-Description: see https://firefox-source-docs.mozilla.org/mozbase/index.html
 Keywords: mozilla
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
+
+see https://firefox-source-docs.mozilla.org/mozbase/index.html
+
```

### Comparing `mozInstall-2.0.1/mozinstall/mozinstall.py` & `mozInstall-2.1.0/mozinstall/mozinstall.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import, print_function
-
-from optparse import OptionParser
 import os
 import plistlib
 import shutil
 import subprocess
 import sys
 import tarfile
 import tempfile
 import time
 import zipfile
-
-import requests
-
-from six import PY3, reraise
+from optparse import OptionParser
 
 import mozfile
 import mozinfo
+import requests
+from six import PY3, reraise
 
 try:
     import pefile
 
     has_pefile = True
 except ImportError:
     has_pefile = False
@@ -132,14 +128,16 @@
     trbk = None
     try:
         install_dir = None
         if src.lower().endswith(".dmg"):
             install_dir = _install_dmg(src, dest)
         elif src.lower().endswith(".exe"):
             install_dir = _install_exe(src, dest)
+        elif src.lower().endswith(".msix"):
+            install_dir = _install_msix(src)
         elif zipfile.is_zipfile(src) or tarfile.is_tarfile(src):
             install_dir = mozfile.extract(src, dest)[0]
 
         return install_dir
 
     except BaseException:
         cls, exc, trbk = sys.exc_info()
@@ -212,14 +210,24 @@
 def uninstall(install_folder):
     """Uninstalls the application in the specified path. If it has been
     installed via an installer on Windows, use the uninstaller first.
 
     :param install_folder: Path of the installation folder
 
     """
+    # Uninstallation for MSIX applications is totally different than
+    # any other installs...
+    if "WindowsApps" in install_folder:
+        # At the time of writing, the package installation directory is always
+        # the package full name, so this assumption is valid (for now....).
+        packageFullName = install_folder.split("WindowsApps\\")[1].split("\\")[0]
+        cmd = f"powershell.exe Remove-AppxPackage -Package {packageFullName}"
+        subprocess.check_call(cmd)
+        return
+
     install_folder = os.path.realpath(install_folder)
     assert os.path.isdir(install_folder), (
         'installation folder "%s" exists.' % install_folder
     )
 
     # On Windows we have to use the uninstaller. If it's not available fallback
     # to the directory removal code
@@ -347,14 +355,55 @@
     cmd = '"%s" /extractdir=%s' % (src, os.path.realpath(dest))
 
     subprocess.check_call(cmd)
 
     return dest
 
 
+def _get_msix_install_location(pkg):
+    with zipfile.ZipFile(pkg) as zf:
+        # First, we pull the app identity out of the AppxManifest...
+        with zf.open("AppxManifest.xml") as am:
+            for line in am.readlines():
+                line = line.decode("utf-8")
+                if "<Identity" in line:
+                    for part in line.split(" "):
+                        if part.startswith("Name"):
+                            pkgname = part.split("=")[-1].strip('"\r\n')
+
+                            # ...then we can use it to find the install location
+                            # with this cmdlet
+                            cmd = (
+                                f'powershell.exe "Get-AppxPackage" "-Name" "{pkgname}"'
+                            )
+                            for line in (
+                                subprocess.check_output(cmd)
+                                .decode("utf-8")
+                                .splitlines()
+                            ):
+                                if line.startswith("InstallLocation"):
+                                    return "C:{}".format(line.split(":")[-1].strip())
+
+    raise Exception(f"Couldn't find install location of {pkg}")
+
+
+def _install_msix(src):
+    """Install the MSIX package and return the installation path.
+
+    Arguments:
+    src -- MSIX package to install
+
+    """
+    # possibly gets around UAC in vista (still need to run as administrator)
+    cmd = f'powershell.exe "Add-AppxPackage" "-Path" "{src}"'
+    subprocess.check_call(cmd)
+
+    return _get_msix_install_location(src)
+
+
 def install_cli(argv=sys.argv[1:]):
     parser = OptionParser(usage="usage: %prog [options] installer")
     parser.add_option(
         "-d",
         "--destination",
         dest="dest",
         default=os.getcwd(),
```

### Comparing `mozInstall-2.0.1/setup.py` & `mozInstall-2.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
 import os
+
 from setuptools import setup
 
 try:
     here = os.path.dirname(os.path.abspath(__file__))
     description = open(os.path.join(here, "README.md")).read()
 except IOError:
     description = None
 
-PACKAGE_VERSION = "2.0.1"
+PACKAGE_VERSION = "2.1.0"
 
 deps = [
     "mozinfo >= 0.7",
     "mozfile >= 1.0",
     "requests",
-    "six >= 1.10.0",
+    "six >= 1.13.0",
 ]
 
 setup(
     name="mozInstall",
     version=PACKAGE_VERSION,
     description="package for installing and uninstalling Mozilla applications",
     long_description="see https://firefox-source-docs.mozilla.org/mozbase/index.html",
```

