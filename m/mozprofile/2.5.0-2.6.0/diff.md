# Comparing `tmp/mozprofile-2.5.0.tar.gz` & `tmp/mozprofile-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mozprofile-2.5.0.tar", last modified: Tue Mar 10 22:14:04 2020, max compression
+gzip compressed data, was "dist/mozprofile-2.6.0.tar", last modified: Fri Jul 28 13:51:58 2023, max compression
```

## Comparing `mozprofile-2.5.0.tar` & `mozprofile-2.6.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 gbrown    (1000) gbrown    (1000)        0 2020-03-10 22:14:04.000000 mozprofile-2.5.0/
-drwxr-xr-x   0 gbrown    (1000) gbrown    (1000)        0 2020-03-10 22:14:04.000000 mozprofile-2.5.0/mozprofile/
--rw-r--r--   0 gbrown    (1000) gbrown    (1000)    14295 2019-12-21 01:18:39.000000 mozprofile-2.5.0/mozprofile/permissions.py
--rw-r--r--   0 gbrown    (1000) gbrown    (1000)    12392 2019-12-21 01:18:39.000000 mozprofile-2.5.0/mozprofile/addons.py
--rw-r--r--   0 gbrown    (1000) gbrown    (1000)     7676 2019-12-21 01:18:39.000000 mozprofile-2.5.0/mozprofile/prefs.py
--rw-r--r--   0 gbrown    (1000) gbrown    (1000)     1052 2019-12-21 01:18:39.000000 mozprofile-2.5.0/mozprofile/view.py
--rw-r--r--   0 gbrown    (1000) gbrown    (1000)    18715 2019-12-21 01:18:39.000000 mozprofile-2.5.0/mozprofile/profile.py
--rw-r--r--   0 gbrown    (1000) gbrown    (1000)     2217 2019-12-21 01:18:39.000000 mozprofile-2.5.0/mozprofile/diff.py
--rw-r--r--   0 gbrown    (1000) gbrown    (1000)      769 2019-12-21 01:18:39.000000 mozprofile-2.5.0/mozprofile/__init__.py
--rwxr-xr-x   0 gbrown    (1000) gbrown    (1000)     5758 2019-12-21 01:18:39.000000 mozprofile-2.5.0/mozprofile/cli.py
--rw-r--r--   0 gbrown    (1000) gbrown    (1000)       67 2020-03-10 22:14:04.000000 mozprofile-2.5.0/setup.cfg
--rw-r--r--   0 gbrown    (1000) gbrown    (1000)      834 2020-03-10 22:14:04.000000 mozprofile-2.5.0/PKG-INFO
-drwxr-xr-x   0 gbrown    (1000) gbrown    (1000)        0 2020-03-10 22:14:04.000000 mozprofile-2.5.0/mozprofile.egg-info/
--rw-r--r--   0 gbrown    (1000) gbrown    (1000)      425 2020-03-10 22:14:04.000000 mozprofile-2.5.0/mozprofile.egg-info/SOURCES.txt
--rw-r--r--   0 gbrown    (1000) gbrown    (1000)        1 2020-03-10 22:14:04.000000 mozprofile-2.5.0/mozprofile.egg-info/not-zip-safe
--rw-r--r--   0 gbrown    (1000) gbrown    (1000)       11 2020-03-10 22:14:04.000000 mozprofile-2.5.0/mozprofile.egg-info/top_level.txt
--rw-r--r--   0 gbrown    (1000) gbrown    (1000)       72 2020-03-10 22:14:04.000000 mozprofile-2.5.0/mozprofile.egg-info/requires.txt
--rw-r--r--   0 gbrown    (1000) gbrown    (1000)        1 2020-03-10 22:14:04.000000 mozprofile-2.5.0/mozprofile.egg-info/dependency_links.txt
--rw-r--r--   0 gbrown    (1000) gbrown    (1000)      187 2020-03-10 22:14:04.000000 mozprofile-2.5.0/mozprofile.egg-info/entry_points.txt
--rw-r--r--   0 gbrown    (1000) gbrown    (1000)      834 2020-03-10 22:14:04.000000 mozprofile-2.5.0/mozprofile.egg-info/PKG-INFO
--rw-r--r--   0 gbrown    (1000) gbrown    (1000)     1779 2020-03-10 22:11:46.000000 mozprofile-2.5.0/setup.py
+drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2023-07-28 13:51:58.000000 mozprofile-2.6.0/
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      823 2023-07-28 13:51:58.000000 mozprofile-2.6.0/PKG-INFO
+drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2023-07-28 13:51:58.000000 mozprofile-2.6.0/mozprofile/
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      729 2023-03-10 23:28:57.000000 mozprofile-2.6.0/mozprofile/__init__.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)    13425 2023-03-10 23:28:57.000000 mozprofile-2.6.0/mozprofile/addons.py
+-rwxrwxr-x   0 gbrown    (1000) gbrown    (1000)     5780 2023-03-10 23:28:57.000000 mozprofile-2.6.0/mozprofile/cli.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     2342 2023-03-10 23:28:57.000000 mozprofile-2.6.0/mozprofile/diff.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)    10411 2023-03-22 17:09:12.000000 mozprofile-2.6.0/mozprofile/permissions.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     8511 2023-05-08 16:25:49.000000 mozprofile-2.6.0/mozprofile/prefs.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)    19762 2023-03-10 23:28:57.000000 mozprofile-2.6.0/mozprofile/profile.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     1182 2023-03-10 23:28:57.000000 mozprofile-2.6.0/mozprofile/view.py
+drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2023-07-28 13:51:58.000000 mozprofile-2.6.0/mozprofile.egg-info/
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      823 2023-07-28 13:51:58.000000 mozprofile-2.6.0/mozprofile.egg-info/PKG-INFO
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      425 2023-07-28 13:51:58.000000 mozprofile-2.6.0/mozprofile.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)        1 2023-07-28 13:51:58.000000 mozprofile-2.6.0/mozprofile.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      187 2023-07-28 13:51:58.000000 mozprofile-2.6.0/mozprofile.egg-info/entry_points.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)        1 2023-07-28 13:51:58.000000 mozprofile-2.6.0/mozprofile.egg-info/not-zip-safe
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       72 2023-07-28 13:51:58.000000 mozprofile-2.6.0/mozprofile.egg-info/requires.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       11 2023-07-28 13:51:58.000000 mozprofile-2.6.0/mozprofile.egg-info/top_level.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       67 2023-07-28 13:51:58.000000 mozprofile-2.6.0/setup.cfg
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     1629 2023-07-28 13:41:20.000000 mozprofile-2.6.0/setup.py
```

### Comparing `mozprofile-2.5.0/mozprofile/permissions.py` & `mozprofile-2.6.0/mozprofile/permissions.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,43 +3,44 @@
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
 
 """
 add permissions to the profile
 """
 
-from __future__ import absolute_import
-
 import codecs
 import os
-import sqlite3
 
 from six import string_types
 from six.moves.urllib import parse
-import six
 
-__all__ = ['MissingPrimaryLocationError', 'MultiplePrimaryLocationsError',
-           'DEFAULT_PORTS', 'DuplicateLocationError', 'BadPortLocationError',
-           'LocationsSyntaxError', 'Location', 'ServerLocations',
-           'Permissions']
+__all__ = [
+    "MissingPrimaryLocationError",
+    "MultiplePrimaryLocationsError",
+    "DEFAULT_PORTS",
+    "DuplicateLocationError",
+    "BadPortLocationError",
+    "LocationsSyntaxError",
+    "Location",
+    "ServerLocations",
+    "Permissions",
+]
 
 # http://hg.mozilla.org/mozilla-central/file/b871dfb2186f/build/automation.py.in#l28
-DEFAULT_PORTS = {'http': '8888',
-                 'https': '4443',
-                 'ws': '4443',
-                 'wss': '4443'}
+DEFAULT_PORTS = {"http": "8888", "https": "4443", "ws": "4443", "wss": "4443"}
 
 
 class LocationError(Exception):
     """Signifies an improperly formed location."""
 
     def __str__(self):
         s = "Bad location"
-        if self.message:
-            s += ": %s" % self.message
+        m = str(Exception.__str__(self))
+        if m:
+            s += ": %s" % m
         return s
 
 
 class MissingPrimaryLocationError(LocationError):
     """No primary location defined in locations file."""
 
     def __init__(self):
@@ -82,83 +83,85 @@
             s += "."
         return s
 
 
 class Location(object):
     """Represents a location line in server-locations.txt."""
 
-    attrs = ('scheme', 'host', 'port')
+    attrs = ("scheme", "host", "port")
 
     def __init__(self, scheme, host, port, options):
         for attr in self.attrs:
             setattr(self, attr, locals()[attr])
         self.options = options
         try:
             int(self.port)
         except ValueError:
             raise BadPortLocationError(self.port)
 
     def isEqual(self, location):
         """compare scheme://host:port, but ignore options"""
-        return len([i for i in self.attrs
-                    if getattr(self, i) == getattr(location, i)]) == len(self.attrs)
+        return len(
+            [i for i in self.attrs if getattr(self, i) == getattr(location, i)]
+        ) == len(self.attrs)
 
     __eq__ = isEqual
 
+    def __hash__(self):
+        # pylint --py3k: W1641
+        return hash(tuple(getattr(attr) for attr in self.attrs))
+
     def url(self):
-        return '%s://%s:%s' % (self.scheme, self.host, self.port)
+        return "%s://%s:%s" % (self.scheme, self.host, self.port)
 
     def __str__(self):
-        return '%s  %s' % (self.url(), ','.join(self.options))
+        return "%s  %s" % (self.url(), ",".join(self.options))
 
 
 class ServerLocations(object):
     """Iterable collection of locations.
     Use provided functions to add new locations, rather that manipulating
     _locations directly, in order to check for errors and to ensure the
     callback is called, if given.
     """
 
-    def __init__(self, filename=None, add_callback=None):
-        self.add_callback = add_callback
+    def __init__(self, filename=None):
         self._locations = []
         self.hasPrimary = False
         if filename:
             self.read(filename)
 
     def __iter__(self):
         return self._locations.__iter__()
 
     def __len__(self):
         return len(self._locations)
 
-    def add(self, location, suppress_callback=False):
+    def add(self, location):
         if "primary" in location.options:
             if self.hasPrimary:
                 raise MultiplePrimaryLocationsError()
             self.hasPrimary = True
 
         self._locations.append(location)
-        if self.add_callback and not suppress_callback:
-            self.add_callback([location])
 
-    def add_host(self, host, port='80', scheme='http', options='privileged'):
+    def add_host(self, host, port="80", scheme="http", options="privileged"):
         if isinstance(options, string_types):
-            options = options.split(',')
+            options = options.split(",")
         self.add(Location(scheme, host, port, options))
 
     def read(self, filename, check_for_primary=True):
         """
         Reads the file and adds all valid locations to the ``self._locations`` array.
 
         :param filename: in the format of server-locations.txt_
         :param check_for_primary: if True, a ``MissingPrimaryLocationError`` exception is raised
           if no primary is found
 
-        .. _server-locations.txt: http://dxr.mozilla.org/mozilla-central/source/build/pgo/server-locations.txt # noqa
+        .. _server-locations.txt: http://searchfox.org/mozilla-central/source/build/pgo/server-locations.txt # noqa
 
         The only exception is that the port, if not defined, defaults to 80 or 443.
 
         FIXME: Shouldn't this default to the protocol-appropriate port?  Is
         there any reason to have defaults at all?
         """
 
@@ -173,166 +176,93 @@
             # check for comments and blank lines
             if line.startswith("#") or not line:
                 continue
 
             # split the server from the options
             try:
                 server, options = line.rsplit(None, 1)
-                options = options.split(',')
+                options = options.split(",")
             except ValueError:
                 server = line
                 options = []
 
             # parse the server url
-            if '://' not in server:
-                server = 'http://' + server
+            if "://" not in server:
+                server = "http://" + server
             scheme, netloc, path, query, fragment = parse.urlsplit(server)
             # get the host and port
             try:
-                host, port = netloc.rsplit(':', 1)
+                host, port = netloc.rsplit(":", 1)
             except ValueError:
                 host = netloc
-                port = DEFAULT_PORTS.get(scheme, '80')
+                port = DEFAULT_PORTS.get(scheme, "80")
 
             try:
                 location = Location(scheme, host, port, options)
-                self.add(location, suppress_callback=True)
+                self.add(location)
             except LocationError as e:
                 raise LocationsSyntaxError(lineno, e)
 
             new_locations.append(location)
 
         # ensure that a primary is found
         if check_for_primary and not self.hasPrimary:
-            raise LocationsSyntaxError(lineno + 1,
-                                       MissingPrimaryLocationError())
-
-        if self.add_callback:
-            self.add_callback(new_locations)
+            raise LocationsSyntaxError(lineno + 1, MissingPrimaryLocationError())
 
 
 class Permissions(object):
     """Allows handling of permissions for ``mozprofile``"""
 
-    def __init__(self, profileDir, locations=None):
-        self._profileDir = profileDir
-        self._locations = ServerLocations(add_callback=self.write_db)
+    def __init__(self, locations=None):
+        self._locations = ServerLocations()
         if locations:
             if isinstance(locations, ServerLocations):
                 self._locations = locations
-                self._locations.add_callback = self.write_db
-                self.write_db(self._locations._locations)
             elif isinstance(locations, list):
                 for l in locations:
                     self._locations.add_host(**l)
             elif isinstance(locations, dict):
                 self._locations.add_host(**locations)
             elif os.path.exists(locations):
                 self._locations.read(locations)
 
-    def write_db(self, locations):
-        """write permissions to the sqlite database"""
-
-        # Open database and create table
-        permDB = sqlite3.connect(os.path.join(self._profileDir, "permissions.sqlite"))
-        cursor = permDB.cursor()
-
-        # SQL copied from
-        # http://dxr.mozilla.org/mozilla-central/source/extensions/cookie/nsPermissionManager.cpp
-        cursor.execute("""CREATE TABLE IF NOT EXISTS moz_hosts (
-              id INTEGER PRIMARY KEY
-             ,origin TEXT
-             ,type TEXT
-             ,permission INTEGER
-             ,expireType INTEGER
-             ,expireTime INTEGER
-             ,modificationTime INTEGER
-           )""")
-
-        rows = cursor.execute("PRAGMA table_info(moz_hosts)")
-        count = len(rows.fetchall())
-
-        using_origin = False
-        # if the db contains 7 columns, we're using user_version 5
-        if count == 7:
-            statement = "INSERT INTO moz_hosts values(NULL, ?, ?, ?, 0, 0, 0)"
-            cursor.execute("PRAGMA user_version=5;")
-            using_origin = True
-        # if the db contains 9 columns, we're using user_version 4
-        elif count == 9:
-            statement = "INSERT INTO moz_hosts values(NULL, ?, ?, ?, 0, 0, 0, 0, 0)"
-            cursor.execute("PRAGMA user_version=4;")
-        # if the db contains 8 columns, we're using user_version 3
-        elif count == 8:
-            statement = "INSERT INTO moz_hosts values(NULL, ?, ?, ?, 0, 0, 0, 0)"
-            cursor.execute("PRAGMA user_version=3;")
-        else:
-            statement = "INSERT INTO moz_hosts values(NULL, ?, ?, ?, 0, 0)"
-            cursor.execute("PRAGMA user_version=2;")
-
-        for location in locations:
-            # set the permissions
-            permissions = {'allowXULXBL': 'noxul' not in location.options}
-            for perm, allow in six.iteritems(permissions):
-                if allow:
-                    permission_type = 1
-                else:
-                    permission_type = 2
-
-                if using_origin:
-                    # This is a crude approximation of the origin generation
-                    # logic from ContentPrincipal and nsStandardURL. It should
-                    # suffice for the permissions which the test runners will
-                    # want to insert into the system.
-                    origin = location.scheme + "://" + location.host
-                    if (location.scheme != 'http' or location.port != '80') and \
-                       (location.scheme != 'https' or location.port != '443'):
-                        origin += ':' + str(location.port)
-
-                    cursor.execute(statement,
-                                   (origin, perm, permission_type))
-                else:
-                    # The database is still using a legacy system based on hosts
-                    # We can insert the permission as a host
-                    #
-                    # XXX This codepath should not be hit, as tests are run with
-                    # fresh profiles. However, if it was hit, permissions would
-                    # not be added to the database correctly (bug 1183185).
-                    cursor.execute(statement,
-                                   (location.host, perm, permission_type))
-
-        # Commit and close
-        permDB.commit()
-        cursor.close()
-
     def network_prefs(self, proxy=None):
         """
         take known locations and generate preferences to handle permissions and proxy
         returns a tuple of prefs, user_prefs
         """
 
         prefs = []
 
         if proxy:
-            user_prefs = self.pac_prefs(proxy)
+            dohServerPort = proxy.get("dohServerPort")
+            if dohServerPort is not None:
+                # make sure we don't use proxy
+                user_prefs = [("network.proxy.type", 0)]
+                # Use TRR_ONLY mode
+                user_prefs.append(("network.trr.mode", 3))
+                trrUri = "https://foo.example.com:{}/dns-query".format(dohServerPort)
+                user_prefs.append(("network.trr.uri", trrUri))
+                user_prefs.append(("network.trr.bootstrapAddr", "127.0.0.1"))
+                user_prefs.append(("network.dns.force_use_https_rr", True))
+            else:
+                user_prefs = self.pac_prefs(proxy)
         else:
             user_prefs = []
 
         return prefs, user_prefs
 
     def pac_prefs(self, user_proxy=None):
         """
-        return preferences for Proxy Auto Config. originally taken from
-        http://dxr.mozilla.org/mozilla-central/source/build/automation.py.in
+        return preferences for Proxy Auto Config.
         """
         proxy = DEFAULT_PORTS.copy()
 
         # We need to proxy every server but the primary one.
-        origins = ["'%s'" % l.url()
-                   for l in self._locations]
+        origins = ["'%s'" % l.url() for l in self._locations]
         origins = ", ".join(origins)
         proxy["origins"] = origins
 
         for l in self._locations:
             if "primary" in l.options:
                 proxy["remote"] = l.host
                 proxy[l.scheme] = l.port
@@ -345,15 +275,16 @@
         # If you must escape things in this string with backslashes, be aware
         # of the multiple layers of escaping at work:
         #
         # - Python will unescape backslashes;
         # - Writing out the prefs will escape things via JSON serialization;
         # - The prefs file reader will unescape backslashes;
         # - The JS engine parser will unescape backslashes.
-        pacURL = """data:text/plain,
+        pacURL = (
+            """data:text/plain,
 var knownOrigins = (function () {
   return [%(origins)s].reduce(function(t, h) { t[h] = true; return t; }, {})
 })();
 var uriRegex = new RegExp('^([a-z][-a-z0-9+.]*)' +
                           '://' +
                           '(?:[^/@]*@)?' +
                           '(.*?)' +
@@ -388,34 +319,17 @@
   }
   var schemeForOriginChecking = originSchemesRemap[originalScheme] || originalScheme;
 
   var origin = schemeForOriginChecking + '://' + host + ':' + port;
   if (!(origin in knownOrigins))
     return 'DIRECT';
   return proxyForScheme[originalScheme] || 'DIRECT';
-}""" % proxy
+}"""
+            % proxy
+        )
         pacURL = "".join(pacURL.splitlines())
 
         prefs = []
         prefs.append(("network.proxy.type", 2))
         prefs.append(("network.proxy.autoconfig_url", pacURL))
 
         return prefs
-
-    def clean_db(self):
-        """Removed permissions added by mozprofile."""
-
-        sqlite_file = os.path.join(self._profileDir, "permissions.sqlite")
-        if not os.path.exists(sqlite_file):
-            return
-
-        # Open database and create table
-        permDB = sqlite3.connect(sqlite_file)
-        cursor = permDB.cursor()
-
-        # TODO: only delete values that we add, this would require sending
-        # in the full permissions object
-        cursor.execute("DROP TABLE IF EXISTS moz_hosts")
-
-        # Commit and close
-        permDB.commit()
-        cursor.close()
```

### Comparing `mozprofile-2.5.0/mozprofile/addons.py` & `mozprofile-2.6.0/mozprofile/addons.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
+import binascii
+import hashlib
 import json
 import os
-import sys
 import shutil
+import sys
 import tempfile
 import zipfile
-import hashlib
-import binascii
 from xml.dom import minidom
-from six import reraise, string_types
 
 import mozfile
 from mozlog.unstructured import getLogger
+from six import reraise, string_types
 
 _SALT = binascii.hexlify(os.urandom(32))
 _TEMPORARY_ADDON_SUFFIX = "@temporary-addon"
 
 # Logger for 'mozprofile.addons' module
 module_logger = getLogger(__name__)
 
@@ -75,15 +73,15 @@
             try:
                 self.remove_addon(addon)
             except IOError:
                 pass
 
         # restore backups
         if self.backup_dir and os.path.isdir(self.backup_dir):
-            extensions_path = os.path.join(self.profile, 'extensions')
+            extensions_path = os.path.join(self.profile, "extensions")
 
             for backup in os.listdir(self.backup_dir):
                 backup_path = os.path.join(self.backup_dir, backup)
                 shutil.move(backup_path, extensions_path)
 
             if not os.listdir(self.backup_dir):
                 mozfile.remove(self.backup_dir)
@@ -94,22 +92,24 @@
     def get_addon_path(self, addon_id):
         """Returns the path to the installed add-on
 
         :param addon_id: id of the add-on to retrieve the path from
         """
         # By default we should expect add-ons being located under the
         # extensions folder.
-        extensions_path = os.path.join(self.profile, 'extensions')
-        paths = [os.path.join(extensions_path, addon_id),
-                 os.path.join(extensions_path, addon_id + '.xpi')]
+        extensions_path = os.path.join(self.profile, "extensions")
+        paths = [
+            os.path.join(extensions_path, addon_id),
+            os.path.join(extensions_path, addon_id + ".xpi"),
+        ]
         for path in paths:
             if os.path.exists(path):
                 return path
 
-        raise IOError('Add-on not found: %s' % addon_id)
+        raise IOError("Add-on not found: %s" % addon_id)
 
     @classmethod
     def is_addon(self, addon_path):
         """
         Checks if the given path is a valid addon
 
         :param addon_path: path to the add-on directory or XPI
@@ -123,44 +123,47 @@
     def _install_addon(self, path, unpack=False):
         addons = [path]
 
         # if path is not an add-on, try to install all contained add-ons
         try:
             self.addon_details(path)
         except AddonFormatError as e:
-            module_logger.warning('Could not install %s: %s' % (path, str(e)))
+            module_logger.warning("Could not install %s: %s" % (path, str(e)))
 
             # If the path doesn't exist, then we don't really care, just return
             if not os.path.isdir(path):
                 return
 
-            addons = [os.path.join(path, x) for x in os.listdir(path) if
-                      self.is_addon(os.path.join(path, x))]
+            addons = [
+                os.path.join(path, x)
+                for x in os.listdir(path)
+                if self.is_addon(os.path.join(path, x))
+            ]
             addons.sort()
 
         # install each addon
         for addon in addons:
             # determine the addon id
             addon_details = self.addon_details(addon)
-            addon_id = addon_details.get('id')
+            addon_id = addon_details.get("id")
 
             # if the add-on has to be unpacked force it now
             # note: we might want to let Firefox do it in case of addon details
             orig_path = None
-            if os.path.isfile(addon) and (unpack or addon_details['unpack']):
+            if os.path.isfile(addon) and (unpack or addon_details["unpack"]):
                 orig_path = addon
                 addon = tempfile.mkdtemp()
                 mozfile.extract(orig_path, addon)
 
             # copy the addon to the profile
-            extensions_path = os.path.join(self.profile, 'extensions')
+            extensions_path = os.path.join(self.profile, "extensions")
             addon_path = os.path.join(extensions_path, addon_id)
 
             if os.path.isfile(addon):
-                addon_path += '.xpi'
+                addon_path += ".xpi"
 
                 # move existing xpi file to backup location to restore later
                 if os.path.exists(addon_path):
                     self.backup_dir = self.backup_dir or tempfile.mkdtemp()
                     shutil.move(addon_path, self.backup_dir)
 
                 # copy new add-on to the extension folder
@@ -217,117 +220,132 @@
 
             {'id':      u'rainbow@colors.org', # id of the addon
              'version': u'1.4',                # version of the addon
              'name':    u'Rainbow',            # name of the addon
              'unpack':  False }                # whether to unpack the addon
         """
 
-        details = {
-            'id': None,
-            'unpack': False,
-            'name': None,
-            'version': None
-        }
+        details = {"id": None, "unpack": False, "name": None, "version": None}
 
         def get_namespace_id(doc, url):
             attributes = doc.documentElement.attributes
             namespace = ""
             for i in range(attributes.length):
                 if attributes.item(i).value == url:
                     if ":" in attributes.item(i).name:
                         # If the namespace is not the default one remove 'xlmns:'
-                        namespace = attributes.item(i).name.split(':')[1] + ":"
+                        namespace = attributes.item(i).name.split(":")[1] + ":"
                         break
             return namespace
 
         def get_text(element):
             """Retrieve the text value of a given node"""
             rc = []
             for node in element.childNodes:
                 if node.nodeType == node.TEXT_NODE:
                     rc.append(node.data)
-            return ''.join(rc).strip()
+            return "".join(rc).strip()
 
         if not os.path.exists(addon_path):
-            raise IOError('Add-on path does not exist: %s' % addon_path)
+            raise IOError("Add-on path does not exist: %s" % addon_path)
 
         is_webext = False
         try:
             if zipfile.is_zipfile(addon_path):
-                # Bug 944361 - We cannot use 'with' together with zipFile because
-                # it will cause an exception thrown in Python 2.6.
-                try:
-                    compressed_file = zipfile.ZipFile(addon_path, 'r')
+                with zipfile.ZipFile(addon_path, "r") as compressed_file:
                     filenames = [f.filename for f in (compressed_file).filelist]
-                    if 'install.rdf' in filenames:
-                        manifest = compressed_file.read('install.rdf')
-                    elif 'manifest.json' in filenames:
+                    if "install.rdf" in filenames:
+                        manifest = compressed_file.read("install.rdf")
+                    elif "manifest.json" in filenames:
                         is_webext = True
-                        manifest = compressed_file.read('manifest.json').decode()
+                        manifest = compressed_file.read("manifest.json").decode()
                         manifest = json.loads(manifest)
                     else:
                         raise KeyError("No manifest")
-                finally:
-                    compressed_file.close()
             elif os.path.isdir(addon_path):
-                try:
-                    with open(os.path.join(addon_path, 'install.rdf')) as f:
-                        manifest = f.read()
-                except IOError:
-                    with open(os.path.join(addon_path, 'manifest.json')) as f:
-                        manifest = json.loads(f.read())
-                        is_webext = True
+                entries = os.listdir(addon_path)
+                # Beginning with https://phabricator.services.mozilla.com/D126174
+                # directories may exist that contain one single XPI. If that's
+                # the case we need to process it just as we do above.
+                if len(entries) == 1 and zipfile.is_zipfile(
+                    os.path.join(addon_path, entries[0])
+                ):
+                    with zipfile.ZipFile(
+                        os.path.join(addon_path, entries[0]), "r"
+                    ) as compressed_file:
+                        filenames = [f.filename for f in (compressed_file).filelist]
+                        if "install.rdf" in filenames:
+                            manifest = compressed_file.read("install.rdf")
+                        elif "manifest.json" in filenames:
+                            is_webext = True
+                            manifest = compressed_file.read("manifest.json").decode()
+                            manifest = json.loads(manifest)
+                        else:
+                            raise KeyError("No manifest")
+                # Otherwise, treat is an already unpacked XPI.
+                else:
+                    try:
+                        with open(os.path.join(addon_path, "install.rdf")) as f:
+                            manifest = f.read()
+                    except IOError:
+                        with open(os.path.join(addon_path, "manifest.json")) as f:
+                            manifest = json.loads(f.read())
+                            is_webext = True
             else:
-                raise IOError('Add-on path is neither an XPI nor a directory: %s' % addon_path)
+                raise IOError(
+                    "Add-on path is neither an XPI nor a directory: %s" % addon_path
+                )
         except (IOError, KeyError) as e:
             reraise(AddonFormatError, AddonFormatError(str(e)), sys.exc_info()[2])
 
         if is_webext:
-            details['version'] = manifest['version']
-            details['name'] = manifest['name']
+            details["version"] = manifest["version"]
+            details["name"] = manifest["name"]
             # Bug 1572404 - we support two locations for gecko-specific
             # metadata.
-            for location in ('applications', 'browser_specific_settings'):
+            for location in ("applications", "browser_specific_settings"):
                 try:
-                    details['id'] = manifest[location]['gecko']['id']
+                    details["id"] = manifest[location]["gecko"]["id"]
                     break
                 except KeyError:
                     pass
-            if details['id'] is None:
-                details['id'] = cls._gen_iid(addon_path)
-            details['unpack'] = False
+            if details["id"] is None:
+                details["id"] = cls._gen_iid(addon_path)
+            details["unpack"] = False
         else:
             try:
                 doc = minidom.parseString(manifest)
 
                 # Get the namespaces abbreviations
-                em = get_namespace_id(doc, 'http://www.mozilla.org/2004/em-rdf#')
-                rdf = get_namespace_id(doc, 'http://www.w3.org/1999/02/22-rdf-syntax-ns#')
+                em = get_namespace_id(doc, "http://www.mozilla.org/2004/em-rdf#")
+                rdf = get_namespace_id(
+                    doc, "http://www.w3.org/1999/02/22-rdf-syntax-ns#"
+                )
 
-                description = doc.getElementsByTagName(rdf + 'Description').item(0)
+                description = doc.getElementsByTagName(rdf + "Description").item(0)
                 for entry, value in description.attributes.items():
                     # Remove the namespace prefix from the tag for comparison
                     entry = entry.replace(em, "")
                     if entry in details.keys():
                         details.update({entry: value})
                 for node in description.childNodes:
                     # Remove the namespace prefix from the tag for comparison
                     entry = node.nodeName.replace(em, "")
                     if entry in details.keys():
                         details.update({entry: get_text(node)})
             except Exception as e:
                 reraise(AddonFormatError, AddonFormatError(str(e)), sys.exc_info()[2])
 
         # turn unpack into a true/false value
-        if isinstance(details['unpack'], string_types):
-            details['unpack'] = details['unpack'].lower() == 'true'
+        if isinstance(details["unpack"], string_types):
+            details["unpack"] = details["unpack"].lower() == "true"
 
         # If no ID is set, the add-on is invalid
-        if details.get('id') is None and not is_webext:
-            raise AddonFormatError('Add-on id could not be found.')
+        if details.get("id") is None and not is_webext:
+            raise AddonFormatError("Add-on id could not be found.")
 
         return details
 
     def remove_addon(self, addon_id):
         """Remove the add-on as specified by the id
 
         :param addon_id: id of the add-on to be removed
```

### Comparing `mozprofile-2.5.0/mozprofile/prefs.py` & `mozprofile-2.6.0/mozprofile/prefs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """
 user preferences
 """
-from __future__ import absolute_import, print_function
-
 import json
-import mozfile
 import os
 import tokenize
 
-from six.moves.configparser import SafeConfigParser as ConfigParser
+import mozfile
+import six
 from six import StringIO, string_types
+from six.moves.configparser import SafeConfigParser as ConfigParser
+
+if six.PY3:
+
+    def unicode(input):
+        return input
 
-__all__ = ('PreferencesReadError', 'Preferences')
+
+__all__ = ("PreferencesReadError", "Preferences")
 
 
 class PreferencesReadError(Exception):
     """read error for prefrences files"""
 
 
 class Preferences(object):
@@ -64,17 +69,17 @@
         - anything enclosed in single quotes will be treated as a string
           with the ''s removed from both sides
         """
 
         if not isinstance(value, string_types):
             return value  # no op
         quote = "'"
-        if value == 'true':
+        if value == "true":
             return True
-        if value == 'false':
+        if value == "false":
             return False
         try:
             return int(value)
         except ValueError:
             pass
         if value.startswith(quote) and value.endswith(quote):
             value = value[1:-1]
@@ -82,17 +87,17 @@
 
     @classmethod
     def read(cls, path):
         """read preferences from a file"""
 
         section = None  # for .ini files
         basename = os.path.basename(path)
-        if ':' in basename:
+        if ":" in basename:
             # section of INI file
-            path, section = path.rsplit(':', 1)
+            path, section = path.rsplit(":", 1)
 
         if not os.path.exists(path) and not mozfile.is_url(path):
             raise PreferencesReadError("'%s' does not exist" % path)
 
         if section:
             try:
                 return cls.read_ini(path, section)
@@ -149,89 +154,110 @@
             raise PreferencesReadError("Malformed preferences: %s" % path)
         types = (bool, string_types, int)
         if [i for i in values if not any([isinstance(i, j) for j in types])]:
             raise PreferencesReadError("Only bool, string, and int values allowed")
         return prefs
 
     @classmethod
-    def read_prefs(cls, path, pref_setter='user_pref', interpolation=None):
+    def read_prefs(cls, path, pref_setter="user_pref", interpolation=None):
         """
         Read preferences from (e.g.) prefs.js
 
         :param path: The path to the preference file to read.
         :param pref_setter: The name of the function used to set preferences
                             in the preference file.
         :param interpolation: If provided, a dict that will be passed
                               to str.format to interpolate preference values.
         """
 
-        marker = '##//'  # magical marker
+        marker = "##//"  # magical marker
         lines = [i.strip() for i in mozfile.load(path).readlines()]
         _lines = []
+        multi_line_pref = None
         for line in lines:
             # decode bytes in case of URL processing
             if isinstance(line, bytes):
                 line = line.decode()
-            if not line.startswith(pref_setter):
+            pref_start = line.startswith(pref_setter)
+
+            # Handle preferences split over multiple lines
+            # Some lines may include brackets so do our best to ensure this
+            # is an actual expected end of function call by checking for a
+            # semi-colon as well.
+            if pref_start and not ");" in line:
+                multi_line_pref = line
+                continue
+            elif multi_line_pref:
+                multi_line_pref = multi_line_pref + line
+                if ");" in line:
+                    if "//" in multi_line_pref:
+                        multi_line_pref = multi_line_pref.replace("//", marker)
+                    _lines.append(multi_line_pref)
+                    multi_line_pref = None
                 continue
-            if '//' in line:
-                line = line.replace('//', marker)
+            elif not pref_start:
+                continue
+
+            if "//" in line:
+                line = line.replace("//", marker)
             _lines.append(line)
-        string = '\n'.join(_lines)
+        string = "\n".join(_lines)
 
         # skip trailing comments
         processed_tokens = []
         f_obj = StringIO(string)
         for token in tokenize.generate_tokens(f_obj.readline):
             if token[0] == tokenize.COMMENT:
                 continue
-            processed_tokens.append(token[:2])  # [:2] gets around http://bugs.python.org/issue9974
+            processed_tokens.append(
+                token[:2]
+            )  # [:2] gets around http://bugs.python.org/issue9974
         string = tokenize.untokenize(processed_tokens)
 
         retval = []
 
         def pref(a, b):
             if interpolation and isinstance(b, string_types):
                 b = b.format(**interpolation)
             retval.append((a, b))
-        lines = [i.strip().rstrip(';') for i in string.split('\n') if i.strip()]
 
-        _globals = {'retval': retval, 'true': True, 'false': False}
+        lines = [i.strip().rstrip(";") for i in string.split("\n") if i.strip()]
+
+        _globals = {"retval": retval, "true": True, "false": False}
         _globals[pref_setter] = pref
         for line in lines:
             try:
                 eval(line, _globals, {})
             except SyntaxError:
                 print(line)
                 raise
 
         # de-magic the marker
         for index, (key, value) in enumerate(retval):
             if isinstance(value, string_types) and marker in value:
-                retval[index] = (key, value.replace(marker, '//'))
+                retval[index] = (key, value.replace(marker, "//"))
 
         return retval
 
     @classmethod
-    def write(cls, _file, prefs, pref_string='user_pref(%s, %s);'):
+    def write(cls, _file, prefs, pref_string="user_pref(%s, %s);"):
         """write preferences to a file"""
 
         if isinstance(_file, string_types):
-            f = open(_file, 'a')
+            f = open(_file, "a")
         else:
             f = _file
 
         if isinstance(prefs, dict):
             # order doesn't matter
             prefs = prefs.items()
 
         # serialize -> JSON
-        _prefs = [(json.dumps(k), json.dumps(v))
-                  for k, v in prefs]
+        _prefs = [(json.dumps(k), json.dumps(v)) for k, v in prefs]
 
         # write the preferences
         for _pref in _prefs:
-            print(pref_string % _pref, file=f)
+            print(unicode(pref_string % _pref), file=f)
 
         # close the file if opened internally
         if isinstance(_file, string_types):
             f.close()
```

### Comparing `mozprofile-2.5.0/mozprofile/view.py` & `mozprofile-2.6.0/mozprofile/view.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 #!/usr/bin/env python
+# This Source Code Form is subject to the terms of the Mozilla Public
+# License, v. 2.0. If a copy of the MPL was not distributed with this
+# file, You can obtain one at http://mozilla.org/MPL/2.0/.
+
 
 """
 script to view mozilla profiles
 """
-from __future__ import absolute_import, print_function
-
-import mozprofile
 import optparse
 import os
 import sys
 
-__all__ = ['view_profile']
+import mozprofile
+
+__all__ = ["view_profile"]
 
 
 def view_profile(args=sys.argv[1:]):
 
-    usage = '%prog [options] profile_path <...>'
+    usage = "%prog [options] profile_path <...>"
     parser = optparse.OptionParser(usage=usage, description=__doc__)
     options, args = parser.parse_args(args)
     if not args:
         parser.print_usage()
         parser.exit()
 
     # check existence
-    missing = [i for i in args
-               if not os.path.exists(i)]
+    missing = [i for i in args if not os.path.exists(i)]
     if missing:
         if len(missing) > 1:
             missing_string = "Profiles do not exist"
         else:
             missing_string = "Profile does not exist"
-        parser.error("%s: %s" % (missing_string, ', '.join(missing)))
+        parser.error("%s: %s" % (missing_string, ", ".join(missing)))
 
     # print summary for each profile
     while args:
         path = args.pop(0)
         profile = mozprofile.Profile(path)
         print(profile.summary())
         if args:
-            print('-' * 4)
+            print("-" * 4)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     view_profile()
```

### Comparing `mozprofile-2.5.0/mozprofile/profile.py` & `mozprofile-2.6.0/mozprofile/profile.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
 import json
 import os
 import platform
 import tempfile
 import time
 import uuid
 from abc import ABCMeta, abstractmethod, abstractproperty
+from io import open
 from shutil import copytree
 
 import mozfile
-from six import string_types, python_2_unicode_compatible
+import six
+from six import python_2_unicode_compatible, string_types
+
+if six.PY3:
+
+    def unicode(input):
+        return input
+
 
 from .addons import AddonManager
 from .permissions import Permissions
 from .prefs import Preferences
 
-__all__ = ['BaseProfile',
-           'ChromeProfile',
-           'ChromiumProfile',
-           'Profile',
-           'FirefoxProfile',
-           'ThunderbirdProfile',
-           'create_profile']
+__all__ = [
+    "BaseProfile",
+    "ChromeProfile",
+    "ChromiumProfile",
+    "Profile",
+    "FirefoxProfile",
+    "ThunderbirdProfile",
+    "create_profile",
+]
 
 
+@six.add_metaclass(ABCMeta)
 class BaseProfile(object):
-    __metaclass__ = ABCMeta
-
     def __init__(self, profile=None, addons=None, preferences=None, restore=True):
         """Create a new Profile.
 
         All arguments are optional.
 
         :param profile: Path to a profile. If not specified, a new profile
                         directory will be created.
@@ -61,15 +68,15 @@
         # Handle profile creation
         self.restore = restore
         self.create_new = not profile
         if profile:
             # Ensure we have a full path to the profile
             self.profile = os.path.abspath(os.path.expanduser(profile))
         else:
-            self.profile = tempfile.mkdtemp(suffix='.mozrunner')
+            self.profile = tempfile.mkdtemp(suffix=".mozrunner")
 
     def __enter__(self):
         return self
 
     def __exit__(self, type, value, traceback):
         self.cleanup()
 
@@ -92,15 +99,15 @@
         """
         reset the profile to the beginning state
         """
         self.cleanup()
         self._reset()
 
     @abstractmethod
-    def set_preferences(self, preferences, filename='user.js'):
+    def set_preferences(self, preferences, filename="user.js"):
         pass
 
     @abstractproperty
     def preference_file_names(self):
         """A tuple of file basenames expected to contain preferences."""
 
     def merge(self, other, interpolation=None):
@@ -117,15 +124,15 @@
             path = os.path.join(other, basename)
             try:
                 prefs = Preferences.read_json(path)
             except ValueError:
                 prefs = Preferences.read_prefs(path, interpolation=interpolation)
             self.set_preferences(prefs, filename=basename)
 
-        extension_dir = os.path.join(other, 'extensions')
+        extension_dir = os.path.join(other, "extensions")
         if not os.path.isdir(extension_dir):
             return
 
         for basename in os.listdir(extension_dir):
             path = os.path.join(extension_dir, basename)
 
             if self.addons.is_addon(path):
@@ -139,15 +146,15 @@
         - ignore: callable passed to shutil.copytree
         - kwargs: arguments to the profile constructor
         """
         if not path_to:
             tempdir = tempfile.mkdtemp()  # need an unused temp dir name
             mozfile.remove(tempdir)  # copytree requires that dest does not exist
             path_to = tempdir
-        copytree(path_from, path_to, ignore=ignore)
+        copytree(path_from, path_to, ignore=ignore, ignore_dangling_symlinks=True)
 
         c = cls(path_to, **kwargs)
         c.create_new = True  # deletes a cloned profile when restore is True
         return c
 
     def exists(self):
         """returns whether the profile exists or not"""
@@ -174,30 +181,45 @@
     the profile as a context manager: ::
 
       with Profile() as profile:
           # do things with the profile
           pass
       # profile.cleanup() has been called here
     """
-    preference_file_names = ('user.js', 'prefs.js')
 
-    def __init__(self, profile=None, addons=None, preferences=None, locations=None,
-                 proxy=None, restore=True, whitelistpaths=None, **kwargs):
+    preference_file_names = ("user.js", "prefs.js")
+
+    def __init__(
+        self,
+        profile=None,
+        addons=None,
+        preferences=None,
+        locations=None,
+        proxy=None,
+        restore=True,
+        whitelistpaths=None,
+        **kwargs
+    ):
         """
         :param profile: Path to the profile
         :param addons: String of one or list of addons to install
         :param preferences: Dictionary or class of preferences
         :param locations: ServerLocations object
         :param proxy: Setup a proxy
         :param restore: Flag for removing all custom settings during cleanup
         :param whitelistpaths: List of paths to pass to Firefox to allow read
             access to from the content process sandbox.
         """
         super(Profile, self).__init__(
-            profile=profile, addons=addons, preferences=preferences, restore=restore, **kwargs)
+            profile=profile,
+            addons=addons,
+            preferences=preferences,
+            restore=restore,
+            **kwargs
+        )
 
         self._locations = locations
         self._proxy = proxy
         self._whitelistpaths = whitelistpaths
 
         # Initialize all class members
         self._reset()
@@ -208,94 +230,102 @@
         if not os.path.exists(self.profile):
             os.makedirs(self.profile)
 
         # Preferences files written to
         self.written_prefs = set()
 
         # Our magic markers
-        nonce = '%s %s' % (str(time.time()), uuid.uuid4())
-        self.delimeters = ('#MozRunner Prefs Start %s' % nonce,
-                           '#MozRunner Prefs End %s' % nonce)
+        nonce = "%s %s" % (str(time.time()), uuid.uuid4())
+        self.delimeters = (
+            "#MozRunner Prefs Start %s" % nonce,
+            "#MozRunner Prefs End %s" % nonce,
+        )
 
         # If sub-classes want to set default preferences
-        if hasattr(self.__class__, 'preferences'):
+        if hasattr(self.__class__, "preferences"):
             self.set_preferences(self.__class__.preferences)
         # Set additional preferences
         self.set_preferences(self._preferences)
 
-        self.permissions = Permissions(self.profile, self._locations)
+        self.permissions = Permissions(self._locations)
         prefs_js, user_js = self.permissions.network_prefs(self._proxy)
 
         if self._whitelistpaths:
             # On macOS we don't want to support a generalized read whitelist,
             # and the macOS sandbox policy language doesn't have support for
             # lists, so we handle these specially.
             if platform.system() == "Darwin":
                 assert len(self._whitelistpaths) <= 2
                 if len(self._whitelistpaths) == 2:
-                    prefs_js.append((
-                        "security.sandbox.content.mac.testing_read_path2",
-                        self._whitelistpaths[1]
-                    ))
-                prefs_js.append((
-                    "security.sandbox.content.mac.testing_read_path1",
-                    self._whitelistpaths[0]
-                ))
+                    prefs_js.append(
+                        (
+                            "security.sandbox.content.mac.testing_read_path2",
+                            self._whitelistpaths[1],
+                        )
+                    )
+                prefs_js.append(
+                    (
+                        "security.sandbox.content.mac.testing_read_path1",
+                        self._whitelistpaths[0],
+                    )
+                )
             else:
-                prefs_js.append(("security.sandbox.content.read_path_whitelist",
-                                 ",".join(self._whitelistpaths)))
-        self.set_preferences(prefs_js, 'prefs.js')
+                prefs_js.append(
+                    (
+                        "security.sandbox.content.read_path_whitelist",
+                        ",".join(self._whitelistpaths),
+                    )
+                )
+        self.set_preferences(prefs_js, "prefs.js")
         self.set_preferences(user_js)
 
         # handle add-on installation
         self.addons = AddonManager(self.profile, restore=self.restore)
         self.addons.install(self._addons)
 
     def cleanup(self):
         """Cleanup operations for the profile."""
 
         if self.restore:
             # If copies of those class instances exist ensure we correctly
             # reset them all (see bug 934484)
             self.clean_preferences()
-            if getattr(self, 'addons', None) is not None:
+            if getattr(self, "addons", None) is not None:
                 self.addons.clean()
-            if getattr(self, 'permissions', None) is not None:
-                self.permissions.clean_db()
         super(Profile, self).cleanup()
 
     def clean_preferences(self):
         """Removed preferences added by mozrunner."""
         for filename in self.written_prefs:
             if not os.path.exists(os.path.join(self.profile, filename)):
                 # file has been deleted
                 break
             while True:
                 if not self.pop_preferences(filename):
                     break
 
     # methods for preferences
 
-    def set_preferences(self, preferences, filename='user.js'):
+    def set_preferences(self, preferences, filename="user.js"):
         """Adds preferences dict to profile preferences"""
         prefs_file = os.path.join(self.profile, filename)
-        with open(prefs_file, 'a') as f:
+        with open(prefs_file, "a") as f:
             if not preferences:
                 return
 
             # note what files we've touched
             self.written_prefs.add(filename)
 
             # opening delimeter
-            f.write('\n%s\n' % self.delimeters[0])
+            f.write(unicode("\n%s\n" % self.delimeters[0]))
 
             Preferences.write(f, preferences)
 
             # closing delimeter
-            f.write('%s\n' % self.delimeters[1])
+            f.write(unicode("%s\n" % self.delimeters[1]))
 
     def set_persistent_preferences(self, preferences):
         """
         Adds preferences dict to profile preferences and save them during a
         profile reset
         """
 
@@ -303,158 +333,192 @@
         if isinstance(preferences, dict):
             preferences = preferences.items()
 
         # add new prefs to preserve them during reset
         for new_pref in preferences:
             # if dupe remove item from original list
             self._preferences = [
-                pref for pref in self._preferences if not new_pref[0] == pref[0]]
+                pref for pref in self._preferences if not new_pref[0] == pref[0]
+            ]
             self._preferences.append(new_pref)
 
-        self.set_preferences(preferences, filename='user.js')
+        self.set_preferences(preferences, filename="user.js")
 
     def pop_preferences(self, filename):
         """
         pop the last set of preferences added
         returns True if popped
         """
 
         path = os.path.join(self.profile, filename)
-        with open(path) as f:
+        with open(path, "r", encoding="utf-8") as f:
             lines = f.read().splitlines()
 
         def last_index(_list, value):
             """
             returns the last index of an item;
             this should actually be part of python code but it isn't
             """
             for index in reversed(range(len(_list))):
                 if _list[index] == value:
                     return index
+
         s = last_index(lines, self.delimeters[0])
         e = last_index(lines, self.delimeters[1])
 
         # ensure both markers are found
         if s is None:
-            assert e is None, '%s found without %s' % (self.delimeters[1], self.delimeters[0])
+            assert e is None, "%s found without %s" % (
+                self.delimeters[1],
+                self.delimeters[0],
+            )
             return False  # no preferences found
         elif e is None:
-            assert s is None, '%s found without %s' % (self.delimeters[0], self.delimeters[1])
+            assert s is None, "%s found without %s" % (
+                self.delimeters[0],
+                self.delimeters[1],
+            )
 
         # ensure the markers are in the proper order
-        assert e > s, '%s found at %s, while %s found at %s' % (self.delimeters[1], e,
-                                                                self.delimeters[0], s)
+        assert e > s, "%s found at %s, while %s found at %s" % (
+            self.delimeters[1],
+            e,
+            self.delimeters[0],
+            s,
+        )
 
         # write the prefs
-        cleaned_prefs = '\n'.join(lines[:s] + lines[e + 1:])
-        with open(path, 'w') as f:
+        cleaned_prefs = "\n".join(lines[:s] + lines[e + 1 :])
+        with open(path, "w") as f:
             f.write(cleaned_prefs)
         return True
 
     # methods for introspection
 
     def summary(self, return_parts=False):
         """
         returns string summarizing profile information.
         if return_parts is true, return the (Part_name, value) list
         of tuples instead of the assembled string
         """
 
-        parts = [('Path', self.profile)]  # profile path
+        parts = [("Path", self.profile)]  # profile path
 
         # directory tree
-        parts.append(('Files', '\n%s' % mozfile.tree(self.profile)))
+        parts.append(("Files", "\n%s" % mozfile.tree(self.profile)))
 
         # preferences
-        for prefs_file in ('user.js', 'prefs.js'):
+        for prefs_file in ("user.js", "prefs.js"):
             path = os.path.join(self.profile, prefs_file)
             if os.path.exists(path):
 
                 # prefs that get their own section
                 # This is currently only 'network.proxy.autoconfig_url'
                 # but could be expanded to include others
-                section_prefs = ['network.proxy.autoconfig_url']
+                section_prefs = ["network.proxy.autoconfig_url"]
                 line_length = 80
                 # buffer for 80 character display:
                 # length = 80 - len(key) - len(': ') - line_length_buffer
                 line_length_buffer = 10
-                line_length_buffer += len(': ')
+                line_length_buffer += len(": ")
 
                 def format_value(key, value):
                     if key not in section_prefs:
                         return value
                     max_length = line_length - len(key) - line_length_buffer
                     if len(value) > max_length:
-                        value = '%s...' % value[:max_length]
+                        value = "%s..." % value[:max_length]
                     return value
 
                 prefs = Preferences.read_prefs(path)
                 if prefs:
                     prefs = dict(prefs)
-                    parts.append((prefs_file,
-                                  '\n%s' % ('\n'.join(
-                                      ['%s: %s' % (key, format_value(key, prefs[key]))
-                                       for key in sorted(prefs.keys())]))))
+                    parts.append(
+                        (
+                            prefs_file,
+                            "\n%s"
+                            % (
+                                "\n".join(
+                                    [
+                                        "%s: %s" % (key, format_value(key, prefs[key]))
+                                        for key in sorted(prefs.keys())
+                                    ]
+                                )
+                            ),
+                        )
+                    )
 
                     # Currently hardcorded to 'network.proxy.autoconfig_url'
                     # but could be generalized, possibly with a generalized (simple)
                     # JS-parser
-                    network_proxy_autoconfig = prefs.get('network.proxy.autoconfig_url')
+                    network_proxy_autoconfig = prefs.get("network.proxy.autoconfig_url")
                     if network_proxy_autoconfig and network_proxy_autoconfig.strip():
                         network_proxy_autoconfig = network_proxy_autoconfig.strip()
-                        lines = network_proxy_autoconfig.replace(';', ';\n').splitlines()
+                        lines = network_proxy_autoconfig.replace(
+                            ";", ";\n"
+                        ).splitlines()
                         lines = [line.strip() for line in lines]
-                        origins_string = 'var origins = ['
-                        origins_end = '];'
+                        origins_string = "var origins = ["
+                        origins_end = "];"
                         if origins_string in lines[0]:
                             start = lines[0].find(origins_string)
                             end = lines[0].find(origins_end, start)
-                            splitline = [lines[0][:start],
-                                         lines[0][start:start + len(origins_string) - 1],
-                                         ]
-                            splitline.extend(lines[0][start + len(origins_string):end].replace(
-                                ',', ',\n').splitlines())
+                            splitline = [
+                                lines[0][:start],
+                                lines[0][start : start + len(origins_string) - 1],
+                            ]
+                            splitline.extend(
+                                lines[0][start + len(origins_string) : end]
+                                .replace(",", ",\n")
+                                .splitlines()
+                            )
                             splitline.append(lines[0][end:])
                             lines[0:1] = [i.strip() for i in splitline]
-                        parts.append(('Network Proxy Autoconfig, %s' % (prefs_file),
-                                      '\n%s' % '\n'.join(lines)))
+                        parts.append(
+                            (
+                                "Network Proxy Autoconfig, %s" % (prefs_file),
+                                "\n%s" % "\n".join(lines),
+                            )
+                        )
 
         if return_parts:
             return parts
 
-        retval = '%s\n' % ('\n\n'.join(['[%s]: %s' % (key, value)
-                                        for key, value in parts]))
+        retval = "%s\n" % (
+            "\n\n".join(["[%s]: %s" % (key, value) for key, value in parts])
+        )
         return retval
 
     def __str__(self):
         return self.summary()
 
 
 class FirefoxProfile(Profile):
     """Specialized Profile subclass for Firefox"""
+
     preferences = {}
 
 
 class ThunderbirdProfile(Profile):
     """Specialized Profile subclass for Thunderbird"""
 
     preferences = {
-        'extensions.update.enabled': False,
-        'extensions.update.notifyUser': False,
-        'browser.shell.checkDefaultBrowser': False,
-        'browser.tabs.warnOnClose': False,
-        'browser.warnOnQuit': False,
-        'browser.sessionstore.resume_from_crash': False,
+        "extensions.update.enabled": False,
+        "extensions.update.notifyUser": False,
+        "browser.shell.checkDefaultBrowser": False,
+        "browser.tabs.warnOnClose": False,
+        "browser.warnOnQuit": False,
+        "browser.sessionstore.resume_from_crash": False,
         # prevents the 'new e-mail address' wizard on new profile
-        'mail.provider.enabled': False,
+        "mail.provider.enabled": False,
     }
 
 
 class ChromiumProfile(BaseProfile):
-    preference_file_names = ('Preferences',)
+    preference_file_names = ("Preferences",)
 
     class AddonManager(list):
         def install(self, addons):
             if isinstance(addons, string_types):
                 addons = [addons]
             self.extend(addons)
 
@@ -463,64 +527,69 @@
             # Don't include testing/profiles on Google Chrome
             return False
 
     def __init__(self, **kwargs):
         super(ChromiumProfile, self).__init__(**kwargs)
 
         if self.create_new:
-            self.profile = os.path.join(self.profile, 'Default')
+            self.profile = os.path.join(self.profile, "Default")
         self._reset()
 
     def _reset(self):
         if not os.path.isdir(self.profile):
             os.makedirs(self.profile)
 
         if self._preferences:
             self.set_preferences(self._preferences)
 
         self.addons = self.AddonManager()
         if self._addons:
             self.addons.install(self._addons)
 
-    def set_preferences(self, preferences, filename='Preferences', **values):
+    def set_preferences(self, preferences, filename="Preferences", **values):
         pref_file = os.path.join(self.profile, filename)
 
         prefs = {}
         if os.path.isfile(pref_file):
-            with open(pref_file, 'r') as fh:
+            with open(pref_file, "r") as fh:
                 prefs.update(json.load(fh))
 
         prefs.update(preferences)
-        with open(pref_file, 'w') as fh:
+        with open(pref_file, "w") as fh:
             prefstr = json.dumps(prefs)
             prefstr % values  # interpolate prefs with values
-            fh.write(prefstr)
+            if six.PY2:
+                fh.write(unicode(prefstr))
+            else:
+                fh.write(prefstr)
 
 
 class ChromeProfile(ChromiumProfile):
     # update this if Google Chrome requires more
     # specific profiles
     pass
 
 
 profile_class = {
-    'chrome': ChromeProfile,
-    'chromium': ChromiumProfile,
-    'firefox': FirefoxProfile,
-    'thunderbird': ThunderbirdProfile,
+    "chrome": ChromeProfile,
+    "chromium": ChromiumProfile,
+    "firefox": FirefoxProfile,
+    "thunderbird": ThunderbirdProfile,
 }
 
 
 def create_profile(app, **kwargs):
     """Create a profile given an application name.
 
     :param app: String name of the application to create a profile for, e.g 'firefox'.
     :param kwargs: Same as the arguments for the Profile class (optional).
     :returns: An application specific Profile instance
     :raises: NotImplementedError
     """
     cls = profile_class.get(app)
 
     if not cls:
-        raise NotImplementedError("Profiles not supported for application '{}'".format(app))
+        raise NotImplementedError(
+            "Profiles not supported for application '{}'".format(app)
+        )
 
     return cls(**kwargs)
```

### Comparing `mozprofile-2.5.0/mozprofile/diff.py` & `mozprofile-2.6.0/mozprofile/diff.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 #!/usr/bin/env python
+# This Source Code Form is subject to the terms of the Mozilla Public
+# License, v. 2.0. If a copy of the MPL was not distributed with this
+# file, You can obtain one at http://mozilla.org/MPL/2.0/.
+
 
 """
 diff two profile summaries
 """
 
-from __future__ import absolute_import, print_function
-
 import difflib
-import profile
 import optparse
 import os
+import profile
 import sys
 
-__all__ = ['diff', 'diff_profiles']
+__all__ = ["diff", "diff_profiles"]
 
 
 def diff(profile1, profile2, diff_function=difflib.unified_diff):
 
     profiles = (profile1, profile2)
     parts = {}
     parts_dict = {}
@@ -25,60 +27,60 @@
 
         # first part, the path, isn't useful for diffing
         parts[index] = prof.summary(return_parts=True)[1:]
 
         parts_dict[index] = dict(parts[index])
 
     # keys the first profile is missing
-    first_missing = [i for i in parts_dict[1]
-                     if i not in parts_dict[0]]
-    parts[0].extend([(i, '') for i in first_missing])
+    first_missing = [i for i in parts_dict[1] if i not in parts_dict[0]]
+    parts[0].extend([(i, "") for i in first_missing])
 
     # diffs
     retval = []
     for key, value in parts[0]:
-        other = parts_dict[1].get(key, '')
+        other = parts_dict[1].get(key, "")
         value = value.strip()
         other = other.strip()
 
-        if key == 'Files':
+        if key == "Files":
             # first line of files is the path; we don't care to diff that
-            value = '\n'.join(value.splitlines()[1:])
+            value = "\n".join(value.splitlines()[1:])
             if other:
-                other = '\n'.join(other.splitlines()[1:])
+                other = "\n".join(other.splitlines()[1:])
 
         value = value.splitlines()
         other = other.splitlines()
-        section_diff = list(diff_function(value, other, profile1.profile, profile2.profile))
+        section_diff = list(
+            diff_function(value, other, profile1.profile, profile2.profile)
+        )
         if section_diff:
-            retval.append((key, '\n'.join(section_diff)))
+            retval.append((key, "\n".join(section_diff)))
 
     return retval
 
 
 def diff_profiles(args=sys.argv[1:]):
 
     # parse command line
-    usage = '%prog [options] profile1 profile2'
+    usage = "%prog [options] profile1 profile2"
     parser = optparse.OptionParser(usage=usage, description=__doc__)
     options, args = parser.parse_args(args)
     if len(args) != 2:
         parser.error("Must give two profile paths")
     missing = [arg for arg in args if not os.path.exists(arg)]
     if missing:
-        parser.error("Profile not found: %s" % (', '.join(missing)))
+        parser.error("Profile not found: %s" % (", ".join(missing)))
 
     # get the profile differences
-    diffs = diff(*([profile.Profile(arg)
-                    for arg in args]))
+    diffs = diff(*([profile.Profile(arg) for arg in args]))
 
     # display them
     while diffs:
         key, value = diffs.pop(0)
-        print('[%s]:\n' % key)
+        print("[%s]:\n" % key)
         print(value)
         if diffs:
-            print('-' * 4)
+            print("-" * 4)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     diff_profiles()
```

### Comparing `mozprofile-2.5.0/mozprofile/__init__.py` & `mozprofile-2.6.0/mozprofile/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 To use mozprofile as an API you can import mozprofile.profile_ and/or the AddonManager_.
 
 ``mozprofile.profile`` features a generic ``Profile`` class.  In addition,
 subclasses ``FirefoxProfile`` and ``ThundebirdProfile`` are available
 with preset preferences for those applications.
 """
 
-from __future__ import absolute_import
-
 from mozprofile.addons import *
 from mozprofile.cli import *
 from mozprofile.diff import *
 from mozprofile.permissions import *
 from mozprofile.prefs import *
 from mozprofile.profile import *
 from mozprofile.view import *
```

### Comparing `mozprofile-2.5.0/mozprofile/cli.py` & `mozprofile-2.6.0/mozprofile/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,34 +6,38 @@
 
 """
 Creates and/or modifies a Firefox profile.
 The profile can be modified by passing in addons to install or preferences to set.
 If no profile is specified, a new profile is created and the path of the
 resulting profile is printed.
 """
-from __future__ import absolute_import, print_function
-
 import sys
 from optparse import OptionParser
+
 from .prefs import Preferences
-from .profile import FirefoxProfile
-from .profile import Profile
+from .profile import FirefoxProfile, Profile
 
-__all__ = ['MozProfileCLI', 'cli', 'KeyValueParseError', 'parse_key_value', 'parse_preferences']
+__all__ = [
+    "MozProfileCLI",
+    "cli",
+    "KeyValueParseError",
+    "parse_key_value",
+    "parse_preferences",
+]
 
 
 class KeyValueParseError(Exception):
     """Error when parsing strings of serialized key-values."""
 
     def __init__(self, msg, errors=()):
         self.errors = errors
         Exception.__init__(self, msg)
 
 
-def parse_key_value(strings, separator='=', context='key, value'):
+def parse_key_value(strings, separator="=", context="key, value"):
     """Parse string-serialized key-value pairs in the form of `key = value`.
 
     Args:
         strings (list): List of strings to parse.
         separator (str): Identifier used to split the strings.
 
     Returns:
@@ -43,20 +47,21 @@
         KeyValueParseError
     """
 
     # syntax check
     missing = [string for string in strings if separator not in string]
     if missing:
         raise KeyValueParseError(
-            "Error: syntax error in %s: %s" %
-            (context, ','.join(missing)), errors=missing)
+            "Error: syntax error in %s: %s" % (context, ",".join(missing)),
+            errors=missing,
+        )
     return [string.split(separator, 1) for string in strings]
 
 
-def parse_preferences(prefs, context='--setpref='):
+def parse_preferences(prefs, context="--setpref="):
     """Parse preferences specified on the command line.
 
     Args:
         prefs (list): A list of strings, usually of the form "<pref>=<value>".
 
     Returns:
         dict: A dictionary of the form {<pref>: <value>} where values have been
@@ -70,86 +75,112 @@
 
     return {k: Preferences.cast(v) for k, v in prefs.items()}
 
 
 class MozProfileCLI(object):
     """The Command Line Interface for ``mozprofile``."""
 
-    module = 'mozprofile'
+    module = "mozprofile"
     profile_class = Profile
 
     def __init__(self, args=sys.argv[1:], add_options=None):
         self.parser = OptionParser(description=__doc__)
         self.add_options(self.parser)
         if add_options:
             add_options(self.parser)
         (self.options, self.args) = self.parser.parse_args(args)
 
     def add_options(self, parser):
 
-        parser.add_option("-p", "--profile", dest="profile",
-                          help="The path to the profile to operate on. "
-                          "If none, creates a new profile in temp directory")
-        parser.add_option("-a", "--addon", dest="addons",
-                          action="append", default=[],
-                          help="Addon paths to install. Can be a filepath, "
-                          "a directory containing addons, or a url")
-        parser.add_option("--pref", dest="prefs",
-                          action='append', default=[],
-                          help="A preference to set. "
-                          "Must be a key-value pair separated by a ':'")
-        parser.add_option("--preferences", dest="prefs_files",
-                          action='append', default=[],
-                          metavar="FILE",
-                          help="read preferences from a JSON or INI file. "
-                          "For INI, use 'file.ini:section' to specify a particular section.")
+        parser.add_option(
+            "-p",
+            "--profile",
+            dest="profile",
+            help="The path to the profile to operate on. "
+            "If none, creates a new profile in temp directory",
+        )
+        parser.add_option(
+            "-a",
+            "--addon",
+            dest="addons",
+            action="append",
+            default=[],
+            help="Addon paths to install. Can be a filepath, "
+            "a directory containing addons, or a url",
+        )
+        parser.add_option(
+            "--pref",
+            dest="prefs",
+            action="append",
+            default=[],
+            help="A preference to set. " "Must be a key-value pair separated by a ':'",
+        )
+        parser.add_option(
+            "--preferences",
+            dest="prefs_files",
+            action="append",
+            default=[],
+            metavar="FILE",
+            help="read preferences from a JSON or INI file. "
+            "For INI, use 'file.ini:section' to specify a particular section.",
+        )
 
     def profile_args(self):
         """arguments to instantiate the profile class"""
-        return dict(profile=self.options.profile,
-                    addons=self.options.addons,
-                    preferences=self.preferences())
+        return dict(
+            profile=self.options.profile,
+            addons=self.options.addons,
+            preferences=self.preferences(),
+        )
 
     def preferences(self):
         """profile preferences"""
 
         # object to hold preferences
         prefs = Preferences()
 
         # add preferences files
         for prefs_file in self.options.prefs_files:
             prefs.add_file(prefs_file)
 
         # change CLI preferences into 2-tuples
-        cli_prefs = parse_key_value(self.options.prefs, separator=':')
+        cli_prefs = parse_key_value(self.options.prefs, separator=":")
 
         # string preferences
         prefs.add(cli_prefs, cast=True)
 
         return prefs()
 
     def profile(self, restore=False):
         """create the profile"""
 
         kwargs = self.profile_args()
-        kwargs['restore'] = restore
+        kwargs["restore"] = restore
         return self.profile_class(**kwargs)
 
 
 def cli(args=sys.argv[1:]):
-    """ Handles the command line arguments for ``mozprofile`` via ``sys.argv``"""
+    """Handles the command line arguments for ``mozprofile`` via ``sys.argv``"""
 
     # add a view method for this cli method only
     def add_options(parser):
-        parser.add_option('--view', dest='view',
-                          action='store_true', default=False,
-                          help="view summary of profile following invocation")
-        parser.add_option('--firefox', dest='firefox_profile',
-                          action='store_true', default=False,
-                          help="use FirefoxProfile defaults")
+        parser.add_option(
+            "--view",
+            dest="view",
+            action="store_true",
+            default=False,
+            help="view summary of profile following invocation",
+        )
+        parser.add_option(
+            "--firefox",
+            dest="firefox_profile",
+            action="store_true",
+            default=False,
+            help="use FirefoxProfile defaults",
+        )
 
     # process the command line
     cli = MozProfileCLI(args, add_options)
 
     if cli.args:
         cli.parser.error("Program doesn't support positional arguments.")
 
@@ -165,9 +196,9 @@
         return
 
     # if no profile was passed in print the newly created profile
     if not cli.options.profile:
         print(profile.profile)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     cli()
```

### Comparing `mozprofile-2.5.0/PKG-INFO` & `mozprofile-2.6.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: mozprofile
-Version: 2.5.0
+Version: 2.6.0
 Summary: Library to create and modify Mozilla application profiles
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
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: manifest
+
+see https://firefox-source-docs.mozilla.org/mozbase/index.html
+
```

### Comparing `mozprofile-2.5.0/mozprofile.egg-info/PKG-INFO` & `mozprofile-2.6.0/mozprofile.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: mozprofile
-Version: 2.5.0
+Version: 2.6.0
 Summary: Library to create and modify Mozilla application profiles
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
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: manifest
+
+see https://firefox-source-docs.mozilla.org/mozbase/index.html
+
```

### Comparing `mozprofile-2.5.0/setup.py` & `mozprofile-2.6.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
 from setuptools import setup
 
-PACKAGE_NAME = 'mozprofile'
-PACKAGE_VERSION = '2.5.0'
+PACKAGE_NAME = "mozprofile"
+PACKAGE_VERSION = "2.6.0"
 
 deps = [
-    'mozfile>=1.2',
-    'mozlog>=6.0',
-    'six>=1.10.0,<2',
+    "mozfile>=1.2",
+    "mozlog>=6.0",
+    "six>=1.13.0,<2",
 ]
 
-setup(name=PACKAGE_NAME,
-      version=PACKAGE_VERSION,
-      description="Library to create and modify Mozilla application profiles",
-      long_description="see https://firefox-source-docs.mozilla.org/mozbase/index.html",
-      classifiers=['Environment :: Console',
-                   'Intended Audience :: Developers',
-                   'License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)',
-                   'Natural Language :: English',
-                   'Operating System :: OS Independent',
-                   'Programming Language :: Python :: 2.7',
-                   'Programming Language :: Python :: 3.5',
-                   'Topic :: Software Development :: Libraries :: Python Modules',
-                   ],
-      keywords='mozilla',
-      author='Mozilla Automation and Tools team',
-      author_email='tools@lists.mozilla.org',
-      url='https://wiki.mozilla.org/Auto-tools/Projects/Mozbase',
-      license='MPL 2.0',
-      packages=['mozprofile'],
-      include_package_data=True,
-      zip_safe=False,
-      install_requires=deps,
-      extras_require={'manifest': ['manifestparser >= 0.6']},
-      tests_require=['wptserve'],
-      entry_points="""
+setup(
+    name=PACKAGE_NAME,
+    version=PACKAGE_VERSION,
+    description="Library to create and modify Mozilla application profiles",
+    long_description="see https://firefox-source-docs.mozilla.org/mozbase/index.html",
+    classifiers=[
+        "Environment :: Console",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
+        "Natural Language :: English",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python :: 2.7",
+        "Programming Language :: Python :: 3.5",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+    ],
+    keywords="mozilla",
+    author="Mozilla Automation and Tools team",
+    author_email="tools@lists.mozilla.org",
+    url="https://wiki.mozilla.org/Auto-tools/Projects/Mozbase",
+    license="MPL 2.0",
+    packages=["mozprofile"],
+    include_package_data=True,
+    zip_safe=False,
+    install_requires=deps,
+    extras_require={"manifest": ["manifestparser >= 0.6"]},
+    tests_require=["wptserve"],
+    entry_points="""
       # -*- Entry points: -*-
       [console_scripts]
       mozprofile = mozprofile:cli
       view-profile = mozprofile:view_profile
       diff-profiles = mozprofile:diff_profiles
-      """, )
+      """,
+)
```

