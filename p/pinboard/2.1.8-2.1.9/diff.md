# Comparing `tmp/pinboard-2.1.8-py2.py3-none-any.whl.zip` & `tmp/pinboard-2.1.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 14010 bytes, number of entries: 10
+Zip file size: 12642 bytes, number of entries: 11
 -rw-r--r--  2.0 unx     1280 b- defN 18-Feb-22 22:11 pinboard/__init__.py
 -rw-r--r--  2.0 unx      947 b- defN 17-Dec-27 16:51 pinboard/exceptions.py
--rw-r--r--  2.0 unx      793 b- defN 18-Oct-12 01:13 pinboard/metadata.py
--rw-r--r--  2.0 unx     7933 b- defN 18-Sep-17 00:51 pinboard/pinboard.py
--rwxr-xr-x  2.0 unx     1069 b- defN 18-Oct-12 00:56 pinboard-2.1.8.data/scripts/.pinboard.un~
--rwxr-xr-x  2.0 unx    13199 b- defN 18-Oct-12 01:13 pinboard-2.1.8.data/scripts/pinboard
--rw-r--r--  2.0 unx        9 b- defN 18-Oct-12 01:13 pinboard-2.1.8.dist-info/top_level.txt
--rw-r--r--  2.0 unx      110 b- defN 18-Oct-12 01:13 pinboard-2.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx    16066 b- defN 18-Oct-12 01:13 pinboard-2.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx      813 b- defN 18-Oct-12 01:13 pinboard-2.1.8.dist-info/RECORD
-10 files, 42219 bytes uncompressed, 12646 bytes compressed:  70.0%
+-rw-r--r--  2.0 unx      793 b- defN 23-Jul-28 13:41 pinboard/metadata.py
+-rw-r--r--  2.0 unx     7995 b- defN 23-Jul-28 13:10 pinboard/pinboard.py
+-rwxr-xr-x  2.0 unx    13202 b- defN 23-Jul-28 13:45 pinboard-2.1.9.data/scripts/pinboard
+-rw-r--r--  2.0 unx    10176 b- defN 23-Jul-28 13:45 pinboard-2.1.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1001 b- defN 23-Jul-28 13:45 pinboard-2.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      148 b- defN 23-Jul-28 13:45 pinboard-2.1.9.dist-info/NOTICE
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-28 13:45 pinboard-2.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-28 13:45 pinboard-2.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      881 b- defN 23-Jul-28 13:45 pinboard-2.1.9.dist-info/RECORD
+11 files, 36542 bytes uncompressed, 11158 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -6,26 +6,29 @@
 
 Filename: pinboard/metadata.py
 Comment: 
 
 Filename: pinboard/pinboard.py
 Comment: 
 
-Filename: pinboard-2.1.8.data/scripts/.pinboard.un~
+Filename: pinboard-2.1.9.data/scripts/pinboard
 Comment: 
 
-Filename: pinboard-2.1.8.data/scripts/pinboard
+Filename: pinboard-2.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: pinboard-2.1.8.dist-info/top_level.txt
+Filename: pinboard-2.1.9.dist-info/METADATA
 Comment: 
 
-Filename: pinboard-2.1.8.dist-info/WHEEL
+Filename: pinboard-2.1.9.dist-info/NOTICE
 Comment: 
 
-Filename: pinboard-2.1.8.dist-info/METADATA
+Filename: pinboard-2.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: pinboard-2.1.8.dist-info/RECORD
+Filename: pinboard-2.1.9.dist-info/top_level.txt
+Comment: 
+
+Filename: pinboard-2.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pinboard/metadata.py

```diff
@@ -8,14 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "2.1.8"
+__version__ = "2.1.9"
 __author__ = "Dan Loewenherz"
 __copyright__ = "Copyright 2015, Lionheart Software"
 __maintainer__ = "Dan Loewenherz"
 __email__ = "dan@lionheartsw.com"
 __license__ = "Apache 2.0"
```

## pinboard/pinboard.py

```diff
@@ -191,17 +191,18 @@
                 Error = error_mappings[e.code]
                 raise Error(e.url, e.code, e.msg, e.hdrs, e.fp)
             raise
         else:
             if parse_response:
                 json_response = json.load(response)
 
-                for field in Pinboard.DATE_FIELDS:
-                    if field in json_response:
-                        json_response[field] = Pinboard.datetime_from_string(json_response[field])
+                if "tags" not in self.components:
+                    for field in Pinboard.DATE_FIELDS:
+                        if field in json_response:
+                            json_response[field] = Pinboard.datetime_from_string(json_response[field])
 
                 if self.components == ["posts", "all"]:
                     return [Bookmark(k, self.token) for k in json_response]
                 elif self.components in [["posts", "get"], ["posts", "recent"]]:
                     json_response['posts'] = [Bookmark(k, self.token) for k in json_response['posts']]
                 elif self.components == ["posts", "dates"]:
                     json_response['dates'] = {Pinboard.date_from_string(k): int(v) \
```

## Comparing `pinboard-2.1.8.data/scripts/pinboard` & `pinboard-2.1.9.data/scripts/pinboard`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         return os.path.expanduser("~/.pinboardrc")
 
     @property
     def pinboard(self):
         try:
             config = configparser.RawConfigParser()
             with open(self.config_file, "r") as f:
-                config.readfp(f)
+                config.read_file(f)
         except:
             api_token = os.environ.get('PINBOARD_TOKEN') or self._login_action()
         else:
             api_token = config.get("authentication", "api_token")
 
         return pinboard.Pinboard(api_token)
```

