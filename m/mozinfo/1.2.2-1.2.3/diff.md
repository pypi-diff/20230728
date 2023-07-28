# Comparing `tmp/mozinfo-1.2.2.tar.gz` & `tmp/mozinfo-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mozinfo-1.2.2.tar", last modified: Wed Jun 17 16:51:05 2020, max compression
+gzip compressed data, was "dist/mozinfo-1.2.3.tar", last modified: Fri Jul 28 13:50:36 2023, max compression
```

## Comparing `mozinfo-1.2.2.tar` & `mozinfo-1.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 edwin     (1000) edwin     (1000)        0 2020-06-17 16:51:05.000000 mozinfo-1.2.2/
--rw-r--r--   0 edwin     (1000) edwin     (1000)      596 2020-06-17 16:51:05.000000 mozinfo-1.2.2/PKG-INFO
-drwxr-xr-x   0 edwin     (1000) edwin     (1000)        0 2020-06-17 16:51:05.000000 mozinfo-1.2.2/mozinfo/
--rw-rw-rw-   0 edwin     (1000) edwin     (1000)     1235 2020-06-10 05:22:45.000000 mozinfo-1.2.2/mozinfo/__init__.py
--rwxrwxrwx   0 edwin     (1000) edwin     (1000)    10855 2020-06-10 05:22:45.000000 mozinfo-1.2.2/mozinfo/mozinfo.py
--rw-rw-rw-   0 edwin     (1000) edwin     (1000)     1291 2020-06-10 05:22:45.000000 mozinfo-1.2.2/mozinfo/string_version.py
-drwxr-xr-x   0 edwin     (1000) edwin     (1000)        0 2020-06-17 16:51:05.000000 mozinfo-1.2.2/mozinfo.egg-info/
--rw-r--r--   0 edwin     (1000) edwin     (1000)      596 2020-06-17 16:51:05.000000 mozinfo-1.2.2/mozinfo.egg-info/PKG-INFO
--rw-r--r--   0 edwin     (1000) edwin     (1000)      301 2020-06-17 16:51:05.000000 mozinfo-1.2.2/mozinfo.egg-info/SOURCES.txt
--rw-r--r--   0 edwin     (1000) edwin     (1000)        1 2020-06-17 16:51:05.000000 mozinfo-1.2.2/mozinfo.egg-info/dependency_links.txt
--rw-r--r--   0 edwin     (1000) edwin     (1000)       90 2020-06-17 16:51:05.000000 mozinfo-1.2.2/mozinfo.egg-info/entry_points.txt
--rw-r--r--   0 edwin     (1000) edwin     (1000)        1 2020-06-17 16:51:05.000000 mozinfo-1.2.2/mozinfo.egg-info/not-zip-safe
--rw-r--r--   0 edwin     (1000) edwin     (1000)       28 2020-06-17 16:51:05.000000 mozinfo-1.2.2/mozinfo.egg-info/requires.txt
--rw-r--r--   0 edwin     (1000) edwin     (1000)        8 2020-06-17 16:51:05.000000 mozinfo-1.2.2/mozinfo.egg-info/top_level.txt
--rw-rw-rw-   0 edwin     (1000) edwin     (1000)       67 2020-06-17 16:51:05.000000 mozinfo-1.2.2/setup.cfg
--rw-r--r--   0 edwin     (1000) edwin     (1000)     1318 2020-06-17 16:47:40.000000 mozinfo-1.2.2/setup.py
+drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2023-07-28 13:50:36.000000 mozinfo-1.2.3/
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      585 2023-07-28 13:50:36.000000 mozinfo-1.2.3/PKG-INFO
+drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2023-07-28 13:50:36.000000 mozinfo-1.2.3/mozinfo/
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     1194 2023-03-10 23:28:57.000000 mozinfo-1.2.3/mozinfo/__init__.py
+-rwxrwxr-x   0 gbrown    (1000) gbrown    (1000)    11598 2023-06-15 15:14:00.000000 mozinfo-1.2.3/mozinfo/mozinfo.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     2015 2023-03-10 23:28:57.000000 mozinfo-1.2.3/mozinfo/string_version.py
+drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2023-07-28 13:50:36.000000 mozinfo-1.2.3/mozinfo.egg-info/
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      585 2023-07-28 13:50:36.000000 mozinfo-1.2.3/mozinfo.egg-info/PKG-INFO
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      301 2023-07-28 13:50:36.000000 mozinfo-1.2.3/mozinfo.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)        1 2023-07-28 13:50:36.000000 mozinfo-1.2.3/mozinfo.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       90 2023-07-28 13:50:36.000000 mozinfo-1.2.3/mozinfo.egg-info/entry_points.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)        1 2023-07-28 13:50:36.000000 mozinfo-1.2.3/mozinfo.egg-info/not-zip-safe
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       28 2023-07-28 13:50:36.000000 mozinfo-1.2.3/mozinfo.egg-info/requires.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)        8 2023-07-28 13:50:36.000000 mozinfo-1.2.3/mozinfo.egg-info/top_level.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       67 2023-07-28 13:50:36.000000 mozinfo-1.2.3/setup.cfg
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     1278 2023-07-28 13:41:21.000000 mozinfo-1.2.3/setup.py
```

### Comparing `mozinfo-1.2.2/PKG-INFO` & `mozinfo-1.2.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: mozinfo
-Version: 1.2.2
+Version: 1.2.3
 Summary: Library to get system information for use in Mozilla testing
 Home-page: https://wiki.mozilla.org/Auto-tools/Projects/Mozbase
 Author: Mozilla Automation and Testing Team
 Author-email: tools@lists.mozilla.org
 License: MPL
-Description: see https://firefox-source-docs.mozilla.org/mozbase/index.html
 Keywords: mozilla
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Development Status :: 5 - Production/Stable
+
+see https://firefox-source-docs.mozilla.org/mozbase/index.html
+
```

### Comparing `mozinfo-1.2.2/mozinfo/__init__.py` & `mozinfo-1.2.3/mozinfo/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # flake8: noqa
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
 """
 interface to transform introspected system information to a format palatable to
 Mozilla
 
 Module variables:
 
 .. attribute:: bits
@@ -54,8 +52,7 @@
 
 """
 
 from . import mozinfo
 from .mozinfo import *
 
 __all__ = mozinfo.__all__
-
```

### Comparing `mozinfo-1.2.2/mozinfo/mozinfo.py` & `mozinfo-1.2.3/mozinfo/mozinfo.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,147 +4,186 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
 # TODO: it might be a good idea of adding a system name (e.g. 'Ubuntu' for
 # linux) to the information; I certainly wouldn't want anyone parsing this
 # information and having behaviour depend on it
 
-from __future__ import absolute_import, print_function
-
 import os
 import platform
 import re
 import sys
+from ctypes.util import find_library
 
 from .string_version import StringVersion
-from ctypes.util import find_library
 
 # keep a copy of the os module since updating globals overrides this
 _os = os
 
 
 class unknown(object):
     """marker class for unknown information"""
 
+    # pylint: disable=W1629
     def __nonzero__(self):
         return False
 
+    def __bool__(self):
+        return False
+
     def __str__(self):
-        return 'UNKNOWN'
+        return "UNKNOWN"
 
 
 unknown = unknown()  # singleton
 
 
 def get_windows_version():
     import ctypes
 
     class OSVERSIONINFOEXW(ctypes.Structure):
-        _fields_ = [('dwOSVersionInfoSize', ctypes.c_ulong),
-                    ('dwMajorVersion', ctypes.c_ulong),
-                    ('dwMinorVersion', ctypes.c_ulong),
-                    ('dwBuildNumber', ctypes.c_ulong),
-                    ('dwPlatformId', ctypes.c_ulong),
-                    ('szCSDVersion', ctypes.c_wchar * 128),
-                    ('wServicePackMajor', ctypes.c_ushort),
-                    ('wServicePackMinor', ctypes.c_ushort),
-                    ('wSuiteMask', ctypes.c_ushort),
-                    ('wProductType', ctypes.c_byte),
-                    ('wReserved', ctypes.c_byte)]
+        _fields_ = [
+            ("dwOSVersionInfoSize", ctypes.c_ulong),
+            ("dwMajorVersion", ctypes.c_ulong),
+            ("dwMinorVersion", ctypes.c_ulong),
+            ("dwBuildNumber", ctypes.c_ulong),
+            ("dwPlatformId", ctypes.c_ulong),
+            ("szCSDVersion", ctypes.c_wchar * 128),
+            ("wServicePackMajor", ctypes.c_ushort),
+            ("wServicePackMinor", ctypes.c_ushort),
+            ("wSuiteMask", ctypes.c_ushort),
+            ("wProductType", ctypes.c_byte),
+            ("wReserved", ctypes.c_byte),
+        ]
 
     os_version = OSVERSIONINFOEXW()
     os_version.dwOSVersionInfoSize = ctypes.sizeof(os_version)
     retcode = ctypes.windll.Ntdll.RtlGetVersion(ctypes.byref(os_version))
     if retcode != 0:
         raise OSError
 
-    return os_version.dwMajorVersion, os_version.dwMinorVersion, os_version.dwBuildNumber
+    return (
+        os_version.dwMajorVersion,
+        os_version.dwMinorVersion,
+        os_version.dwBuildNumber,
+    )
 
 
 # get system information
-info = {'os': unknown,
-        'processor': unknown,
-        'version': unknown,
-        'os_version': unknown,
-        'bits': unknown,
-        'has_sandbox': unknown,
-        'webrender': False,
-        'automation': bool(os.environ.get("MOZ_AUTOMATION", False)),
-        }
+info = {
+    "os": unknown,
+    "processor": unknown,
+    "version": unknown,
+    "os_version": unknown,
+    "bits": unknown,
+    "has_sandbox": unknown,
+    "display": None,
+    "automation": bool(os.environ.get("MOZ_AUTOMATION", False)),
+}
 (system, node, release, version, machine, processor) = platform.uname()
 (bits, linkage) = platform.architecture()
 
 # get os information and related data
 if system in ["Microsoft", "Windows"]:
-    info['os'] = 'win'
+    info["os"] = "win"
     # There is a Python bug on Windows to determine platform values
     # http://bugs.python.org/issue7860
     if "PROCESSOR_ARCHITEW6432" in os.environ:
         processor = os.environ.get("PROCESSOR_ARCHITEW6432", processor)
     else:
-        processor = os.environ.get('PROCESSOR_ARCHITECTURE', processor)
-    system = os.environ.get("OS", system).replace('_', ' ')
+        processor = os.environ.get("PROCESSOR_ARCHITECTURE", processor)
+    system = os.environ.get("OS", system).replace("_", " ")
     (major, minor, _, _, service_pack) = os.sys.getwindowsversion()
-    info['service_pack'] = service_pack
+    info["service_pack"] = service_pack
     if major >= 6 and minor >= 2:
         # On windows >= 8.1 the system call that getwindowsversion uses has
         # been frozen to always return the same values. In this case we call
         # the RtlGetVersion API directly, which still provides meaningful
         # values, at least for now.
         major, minor, build_number = get_windows_version()
         version = "%d.%d.%d" % (major, minor, build_number)
 
     os_version = "%d.%d" % (major, minor)
-elif system.startswith(('MINGW', 'MSYS_NT')):
+elif system.startswith(("MINGW", "MSYS_NT")):
     # windows/mingw python build (msys)
-    info['os'] = 'win'
+    info["os"] = "win"
     os_version = version = unknown
 elif system == "Linux":
     # Attempt to use distro package to determine Linux distribution first.
     # Failing that, fall back to use the platform method.
     # Note that platform.linux_distribution() will be deprecated as of 3.8
     # and this block will be removed once support for 2.7/3.5 is dropped.
     try:
         from distro import linux_distribution
     except ImportError:
         from platform import linux_distribution
 
     output = linux_distribution()
-    (distribution, os_version, codename) = tuple(
-        str(item.title()) for item in output)
+    (distribution, os_version, codename) = tuple(str(item.title()) for item in output)
 
     if not processor:
         processor = machine
     if not distribution:
-        distribution = 'lfs'
+        distribution = "lfs"
     if not os_version:
         os_version = release
     if not codename:
-        codename = 'unknown'
+        codename = "unknown"
     version = "%s %s" % (distribution, os_version)
 
-    info['os'] = 'linux'
-    info['linux_distro'] = distribution
-elif system in ['DragonFly', 'FreeBSD', 'NetBSD', 'OpenBSD']:
-    info['os'] = 'bsd'
+    if os.environ.get("WAYLAND_DISPLAY"):
+        info["display"] = "wayland"
+    elif os.environ.get("DISPLAY"):
+        info["display"] = "x11"
+
+    info["os"] = "linux"
+    info["linux_distro"] = distribution
+elif system in ["DragonFly", "FreeBSD", "NetBSD", "OpenBSD"]:
+    info["os"] = "bsd"
     version = os_version = sys.platform
 elif system == "Darwin":
     (release, versioninfo, machine) = platform.mac_ver()
     version = "OS X %s" % release
-    versionNums = release.split('.')[:2]
+    versionNums = release.split(".")[:2]
     os_version = "%s.%s" % (versionNums[0], versionNums[1])
-    info['os'] = 'mac'
-elif sys.platform in ('solaris', 'sunos5'):
-    info['os'] = 'unix'
+    info["os"] = "mac"
+elif sys.platform in ("solaris", "sunos5"):
+    info["os"] = "unix"
     os_version = version = sys.platform
 else:
     os_version = version = unknown
 
-info['version'] = version
-info['os_version'] = StringVersion(os_version)
+info["apple_silicon"] = False
+if (
+    info["os"] == "mac"
+    and float(os_version) > 10.15
+    and processor == "arm"
+    and bits == "64bit"
+):
+    info["apple_silicon"] = True
+
+info["apple_catalina"] = False
+if info["os"] == "mac" and float(os_version) == 10.15:
+    info["apple_catalina"] = True
+
+info["win10_2004"] = False
+if info["os"] == "win" and version == "10.0.19041":
+    info["win10_2004"] = True
+
+info["win10_2009"] = False
+if info["os"] == "win" and version == "10.0.19045":
+    info["win10_2009"] = True
+
+info["win11_2009"] = False
+if info["os"] == "win" and version == "10.0.22621":
+    info["win11_2009"] = True
+
+info["version"] = version
+info["os_version"] = StringVersion(os_version)
+
 
 # processor type and bits
 if processor in ["i386", "i686"]:
     if bits == "32bit":
         processor = "x86"
     elif bits == "64bit":
         processor = "x86_64"
@@ -152,76 +191,88 @@
     bits = "64bit"
     processor = "x86_64"
 elif processor.upper() == "ARM64":
     bits = "64bit"
     processor = "aarch64"
 elif processor == "Power Macintosh":
     processor = "ppc"
-bits = re.search('(\d+)bit', bits).group(1)
-info.update({'processor': processor,
-             'bits': int(bits),
-             })
+bits = re.search("(\d+)bit", bits).group(1)
+info.update(
+    {
+        "processor": processor,
+        "bits": int(bits),
+    }
+)
 
-if info['os'] == 'linux':
+if info["os"] == "linux":
     import ctypes
     import errno
+
     PR_SET_SECCOMP = 22
     SECCOMP_MODE_FILTER = 2
-    ctypes.CDLL(find_library("c"), use_errno=True).prctl(PR_SET_SECCOMP, SECCOMP_MODE_FILTER, 0)
-    info['has_sandbox'] = ctypes.get_errno() == errno.EFAULT
+    ctypes.CDLL(find_library("c"), use_errno=True).prctl(
+        PR_SET_SECCOMP, SECCOMP_MODE_FILTER, 0
+    )
+    info["has_sandbox"] = ctypes.get_errno() == errno.EFAULT
 else:
-    info['has_sandbox'] = True
+    info["has_sandbox"] = True
 
 # standard value of choices, for easy inspection
-choices = {'os': ['linux', 'bsd', 'win', 'mac', 'unix'],
-           'bits': [32, 64],
-           'processor': ['x86', 'x86_64', 'ppc']}
+choices = {
+    "os": ["linux", "bsd", "win", "mac", "unix"],
+    "bits": [32, 64],
+    "processor": ["x86", "x86_64", "ppc"],
+}
 
 
 def sanitize(info):
     """Do some sanitization of input values, primarily
     to handle universal Mac builds."""
     if "processor" in info and info["processor"] == "universal-x86-x86_64":
         # If we're running on OS X 10.6 or newer, assume 64-bit
         if release[:4] >= "10.6":  # Note this is a string comparison
             info["processor"] = "x86_64"
             info["bits"] = 64
         else:
             info["processor"] = "x86"
             info["bits"] = 32
 
+
 # method for updating information
 
 
 def update(new_info):
     """
     Update the info.
 
     :param new_info: Either a dict containing the new info or a path/url
                      to a json file containing the new info.
     """
     from six import string_types
+
     if isinstance(new_info, string_types):
         # lazy import
-        import mozfile
         import json
+
+        import mozfile
+
         f = mozfile.load(new_info)
         new_info = json.loads(f.read())
         f.close()
 
     info.update(new_info)
     sanitize(info)
     globals().update(info)
 
     # convenience data for os access
-    for os_name in choices['os']:
-        globals()['is' + os_name.title()] = info['os'] == os_name
+    for os_name in choices["os"]:
+        globals()["is" + os_name.title()] = info["os"] == os_name
     # unix is special
     if isLinux or isBsd:  # noqa
-        globals()['isUnix'] = True
+        globals()["isUnix"] = True
 
 
 def find_and_update_from_json(*dirs, **kwargs):
     """Find a mozinfo.json file, load it, and update global symbol table.
 
     This method will first check the relevant objdir directory for the
     necessary mozinfo.json file, if the current script is being run from a
@@ -235,23 +286,24 @@
 
     If no valid files are found, this method no-ops unless the raise_exception
     kwargs is provided with explicit boolean value of True.
 
     :param tuple dirs: Directories in which to look for the file.
     :param dict kwargs: optional values:
                         raise_exception: if True, exceptions are raised.
-                                         False by default.
+                        False by default.
     :returns: None: default behavior if mozinfo.json cannot be found.
               json_path: string representation of mozinfo.json path.
     :raises: IOError: if raise_exception is True and file is not found.
     """
     # First, see if we're in an objdir
     try:
-        from mozbuild.base import MozbuildObject, BuildEnvironmentNotFoundException
         from mozboot.mozconfig import MozconfigFindException
+        from mozbuild.base import BuildEnvironmentNotFoundException, MozbuildObject
+
         build = MozbuildObject.from_environment()
         json_path = _os.path.join(build.topobjdir, "mozinfo.json")
         if _os.path.isfile(json_path):
             update(json_path)
             return json_path
     except ImportError:
         pass
@@ -263,74 +315,83 @@
         json_path = _os.path.join(d, "mozinfo.json")
         if _os.path.isfile(json_path):
             update(json_path)
             return json_path
 
     # by default, exceptions are suppressed. Set this to True if otherwise
     # desired.
-    if kwargs.get('raise_exception', False):
-        raise IOError('mozinfo.json could not be found.')
+    if kwargs.get("raise_exception", False):
+        raise IOError("mozinfo.json could not be found.")
     return None
 
 
 def output_to_file(path):
     import json
-    with open(path, 'w') as f:
+
+    with open(path, "w") as f:
         f.write(json.dumps(info))
 
 
 update({})
 
 # exports
 __all__ = list(info.keys())
-__all__ += ['is' + os_name.title() for os_name in choices['os']]
+__all__ += ["is" + os_name.title() for os_name in choices["os"]]
 __all__ += [
-    'info',
-    'unknown',
-    'main',
-    'choices',
-    'update',
-    'find_and_update_from_json',
-    'output_to_file',
-    'StringVersion',
+    "info",
+    "unknown",
+    "main",
+    "choices",
+    "update",
+    "find_and_update_from_json",
+    "output_to_file",
+    "StringVersion",
 ]
 
 
 def main(args=None):
 
     # parse the command line
     from optparse import OptionParser
+
     parser = OptionParser(description=__doc__)
     for key in choices:
-        parser.add_option('--%s' % key, dest=key,
-                          action='store_true', default=False,
-                          help="display choices for %s" % key)
+        parser.add_option(
+            "--%s" % key,
+            dest=key,
+            action="store_true",
+            default=False,
+            help="display choices for %s" % key,
+        )
     options, args = parser.parse_args()
 
     # args are JSON blobs to override info
     if args:
         # lazy import
         import json
+
         for arg in args:
             if _os.path.exists(arg):
                 string = open(arg).read()
             else:
                 string = arg
             update(json.loads(string))
 
     # print out choices if requested
     flag = False
     for key, value in options.__dict__.items():
         if value is True:
-            print('%s choices: %s' % (key, ' '.join([str(choice)
-                                                     for choice in choices[key]])))
+            print(
+                "%s choices: %s"
+                % (key, " ".join([str(choice) for choice in choices[key]]))
+            )
             flag = True
     if flag:
         return
 
     # otherwise, print out all info
     for key, value in info.items():
-        print('%s: %s' % (key, value))
+        print("%s: %s" % (key, value))
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `mozinfo-1.2.2/mozinfo.egg-info/PKG-INFO` & `mozinfo-1.2.3/mozinfo.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: mozinfo
-Version: 1.2.2
+Version: 1.2.3
 Summary: Library to get system information for use in Mozilla testing
 Home-page: https://wiki.mozilla.org/Auto-tools/Projects/Mozbase
 Author: Mozilla Automation and Testing Team
 Author-email: tools@lists.mozilla.org
 License: MPL
-Description: see https://firefox-source-docs.mozilla.org/mozbase/index.html
 Keywords: mozilla
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Development Status :: 5 - Production/Stable
+
+see https://firefox-source-docs.mozilla.org/mozbase/index.html
+
```

### Comparing `mozinfo-1.2.2/setup.py` & `mozinfo-1.2.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
 from setuptools import setup
 
-PACKAGE_VERSION = "1.2.2"
+PACKAGE_VERSION = "1.2.3"
 
 # dependencies
 deps = [
     "distro >= 1.4.0",
     "mozfile >= 0.12",
 ]
```

