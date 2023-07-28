# Comparing `tmp/pydeezer_asy-2.2.1.tar.gz` & `tmp/pydeezer_asy-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydeezer_asy-2.2.1.tar", last modified: Thu Jul 27 22:47:22 2023, max compression
+gzip compressed data, was "pydeezer_asy-2.2.5.tar", last modified: Fri Jul 28 17:51:39 2023, max compression
```

## Comparing `pydeezer_asy-2.2.1.tar` & `pydeezer_asy-2.2.5.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 22:47:22.361618 pydeezer_asy-2.2.1/
--rw-rw-rw-   0        0        0     1910 2023-07-27 22:47:22.360625 pydeezer_asy-2.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1546 2023-07-27 20:49:08.000000 pydeezer_asy-2.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 22:47:22.280835 pydeezer_asy-2.2.1/deezer_asy/
--rw-rw-rw-   0        0        0    31178 2023-07-27 22:39:56.000000 pydeezer_asy-2.2.1/deezer_asy/DeezerAsy.py
--rw-rw-rw-   0        0        0      136 2023-07-27 18:53:44.000000 pydeezer_asy-2.2.1/deezer_asy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 22:47:22.312785 pydeezer_asy-2.2.1/deezer_asy/constants/
--rw-rw-rw-   0        0        0      193 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.1/deezer_asy/constants/__init__.py
--rw-rw-rw-   0        0        0      789 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.1/deezer_asy/constants/api_methods.py
--rw-rw-rw-   0        0        0      191 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.1/deezer_asy/constants/api_urls.py
--rw-rw-rw-   0        0        0      124 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.1/deezer_asy/constants/image_hosts.py
--rw-rw-rw-   0        0        0      392 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.1/deezer_asy/constants/networking_settings.py
--rw-rw-rw-   0        0        0       72 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.1/deezer_asy/constants/search_types.py
--rw-rw-rw-   0        0        0      694 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.1/deezer_asy/constants/track_formats.py
--rw-rw-rw-   0        0        0      140 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.1/deezer_asy/exceptions.py
--rw-rw-rw-   0        0        0     2004 2023-07-07 16:54:00.000000 pydeezer_asy-2.2.1/deezer_asy/util.py
-drwxrwxrwx   0        0        0        0 2023-07-27 22:47:22.359623 pydeezer_asy-2.2.1/pydeezer_asy.egg-info/
--rw-rw-rw-   0        0        0     1910 2023-07-27 22:47:21.000000 pydeezer_asy-2.2.1/pydeezer_asy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      545 2023-07-27 22:47:22.000000 pydeezer_asy-2.2.1/pydeezer_asy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 22:47:21.000000 pydeezer_asy-2.2.1/pydeezer_asy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-07-27 22:47:21.000000 pydeezer_asy-2.2.1/pydeezer_asy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-27 22:47:21.000000 pydeezer_asy-2.2.1/pydeezer_asy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 22:47:22.361618 pydeezer_asy-2.2.1/setup.cfg
--rw-rw-rw-   0        0        0      774 2023-07-27 22:47:15.000000 pydeezer_asy-2.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 17:51:39.213268 pydeezer_asy-2.2.5/
+-rw-rw-rw-   0        0        0     3743 2023-07-28 17:51:39.211954 pydeezer_asy-2.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3379 2023-07-28 17:51:13.000000 pydeezer_asy-2.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 17:51:39.123712 pydeezer_asy-2.2.5/deezer_asy/
+-rw-rw-rw-   0        0        0    31843 2023-07-28 17:21:24.000000 pydeezer_asy-2.2.5/deezer_asy/DeezerAsy.py
+-rw-rw-rw-   0        0        0      168 2023-07-28 16:45:52.000000 pydeezer_asy-2.2.5/deezer_asy/__init__.py
+-rw-rw-rw-   0        0        0    29344 2023-07-28 17:21:32.000000 pydeezer_asy-2.2.5/deezer_asy/aiodeezer.py
+drwxrwxrwx   0        0        0        0 2023-07-28 17:51:39.150225 pydeezer_asy-2.2.5/deezer_asy/constants/
+-rw-rw-rw-   0        0        0      193 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.5/deezer_asy/constants/__init__.py
+-rw-rw-rw-   0        0        0      789 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.5/deezer_asy/constants/api_methods.py
+-rw-rw-rw-   0        0        0      191 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.5/deezer_asy/constants/api_urls.py
+-rw-rw-rw-   0        0        0      124 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.5/deezer_asy/constants/image_hosts.py
+-rw-rw-rw-   0        0        0      392 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.5/deezer_asy/constants/networking_settings.py
+-rw-rw-rw-   0        0        0       72 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.5/deezer_asy/constants/search_types.py
+-rw-rw-rw-   0        0        0      694 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.5/deezer_asy/constants/track_formats.py
+-rw-rw-rw-   0        0        0      140 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.5/deezer_asy/exceptions.py
+-rw-rw-rw-   0        0        0     2004 2023-07-07 16:54:00.000000 pydeezer_asy-2.2.5/deezer_asy/util.py
+drwxrwxrwx   0        0        0        0 2023-07-28 17:51:39.207831 pydeezer_asy-2.2.5/pydeezer_asy.egg-info/
+-rw-rw-rw-   0        0        0     3743 2023-07-28 17:51:38.000000 pydeezer_asy-2.2.5/pydeezer_asy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      569 2023-07-28 17:51:38.000000 pydeezer_asy-2.2.5/pydeezer_asy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 17:51:38.000000 pydeezer_asy-2.2.5/pydeezer_asy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-07-28 17:51:38.000000 pydeezer_asy-2.2.5/pydeezer_asy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-28 17:51:38.000000 pydeezer_asy-2.2.5/pydeezer_asy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 17:51:39.213268 pydeezer_asy-2.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      774 2023-07-28 17:51:30.000000 pydeezer_asy-2.2.5/setup.py
```

### Comparing `pydeezer_asy-2.2.1/deezer_asy/DeezerAsy.py` & `pydeezer_asy-2.2.5/deezer_asy/DeezerAsy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,37 @@
-import aiohttp, asyncio
+# Standard Library
+import hashlib
+from os import path, remove
+import logging
+
+# External Libraries
+import aiohttp
+import asyncio
+import aiofiles
+import httpx
 from yarl import URL
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
-import mutagen
-import aiofiles
 from mutagen.id3 import ID3, APIC
 from mutagen.easyid3 import EasyID3
-from os import path, remove
-import hashlib
-import httpx, json
+from mutagen.mp3 import MP3
 
+#
 from .constants import *
-
-from .exceptions import LoginError
-from .exceptions import APIRequestError
-from .exceptions import DownloadLinkDecryptionError
-
+from .exceptions import (
+    LoginError,
+    APIRequestError,
+    DownloadLinkDecryptionError
+)
 from . import util
 
-import logging
 
 
 class DeezerAsy:
-    def __init__(self, arl, loop=None, logger:logging.Logger=None, _httpx:bool=False) -> None:
+    def __init__(self, arl, loop=None, logger:logging.Logger=None, _httpx:bool=False, *args) -> None:
         self.logger = logger
         self.token = None
         self._temp_coockie = True
         self._main_session = None
         self.httpx = _httpx
         self.arl = arl
         self.cookies = {'arl': self.arl}
@@ -47,16 +52,20 @@
         if self.httpx: self.cookies = self._temp_coockie
         
     
 
     async def close_session(self):
         if self.logger: self.logger.info('[CLOSING] Closing a local session')
         if self._main_session:
-            await self._main_session.close()
-
+            try:
+                await self._main_session.close()
+            except Exception as err:
+                if self.logger: self.logger.error(f'Failed to close session: {str(err)}')
+        else: 
+            if self.logger: self.logger.error('The session could not be closed, it is missing or already closed')
     """
         MAIN API
     """
     async def get_cookies(self):
         """Get cookies in the domain of {api_urls.DEEZER_URL}
 
         Returns:
@@ -658,15 +667,14 @@
             with_metadata {bool} -- If true, will write id3 tags into the file. (default: {True})
             with_lyrics {bool} -- If true, will find and save lyrics of the given track. (default: {True})
             tag_separator {str} -- Separator to separate multiple artists (default: {", "})
         
         Returns:
             dict -- {'track': path_to_audio, 'lyric': path_to_lrc or None}
         """
-
         ###########################
         if with_lyrics:
             if "LYRICS" in track:
                 lyric_data = track["LYRICS"]
             else:
                 try:
                     if "DATA" in track:
@@ -677,21 +685,25 @@
                         _lyric_data = await self.get_track_lyrics(
                             track["SNG_ID"])
                         lyric_data = _lyric_data["info"]
                 except APIRequestError:
                     with_lyrics = False
 
         track = track["DATA"] if "DATA" in track else track
-        tags = await self.get_track_tags(track, separator=tag_separator, with_cover=False)
+        tags = await self.get_track_tags(track, separator=tag_separator, with_cover=with_metadata)
+        title = tags["title"]
+        if self.logger: 
+            artist = tags['artist']
+            self.logger.info(f'[DL]: Download started [{artist} - {title}]')
+        
         url, quality_key = await self.get_track_download_url(
             track, quality, fallback=fallback, renew=renew, **kwargs)
         blowfish_key = util.get_blowfish_key(track["SNG_ID"])
 
         quality = track_formats.TRACK_FORMAT_MAP[quality_key]
-        title = tags["title"]
         ext = quality["ext"]
 
         if not filename:
             filename =  title + ext
         if not str(filename).endswith(ext):
             filename += ext
 
@@ -731,22 +743,25 @@
 
                             await f.write(dec_data)
                     except:
                         print(type(chunk))
                     i += 1
 
         if with_metadata:
+            if self.logger: self.logger.info(f'[DL]: Tag editing [{artist} - {title}]')
             if ext.lower() == ".flac":
                 pass #self._write_flac_tags(download_path, track, tags=tags)
             else:
                 await self._write_mp3_tags(download_path, track, tags=tags)
         if with_lyrics:
+            if self.logger: self.logger.info(f'[DL]: Download lyrics [{artist} - {title}]')
             lyrics_path = path.join(download_dir, filename[:-len(ext)])
             lyric_check = await self.save_lyrics(lyric_data, lyrics_path)
             if not lyric_check[0]:
+                if self.logger: self.logger.info(f'[DL]: Lyric not found, cancel [{artist} - {title}]')
                 self.loop.run_in_executor(None, remove, lyric_check[1])
                 return {'track': download_path, 'lyruc': None}
 
             return {'track': download_path, 'lyruc': lyric_check[1]}
 
         return {'track': download_path, 'lyruc': None}
     async def get_tracks(self, track_ids):
@@ -829,39 +844,35 @@
         return (True, save_path)
     
     """
         TAG EDIT
 
         p.s: It might be blocking the thread, not sure
     """
-    def __update_mp3(self, path, tags):
-        audio = mutagen.File(path, easy=True)
-        if audio is None:
-            raise ValueError("Invalid file format")
-
+    def __update_mp3(self, _path, tags):
+        audio = MP3(_path, ID3=EasyID3)
         audio.delete()
         EasyID3.RegisterTextKey("label", "TPUB")
 
         cover = tags["_albumart"]
         del tags["_albumart"]
 
         for key, val in tags.items():
             if val:
                 audio[key] = str(val)
-        
+        audio.save()
 
         if cover:
-            cover_handle = ID3(path)
+            cover_handle = ID3(_path)
             cover_handle["APIC"] = APIC(
                 type=3,
                 mime=cover["mime_type"],
                 data=cover["image"]
             )
-            cover_handle.save(path)
-        audio.save()
+            cover_handle.save(_path)
     async def _write_mp3_tags(self, path, track, tags=None):
         track = track["DATA"] if "DATA" in track else track
 
         if not tags:
             tags = await self.get_track_tags(track)
 
         _ = await self.loop.run_in_executor(None, self.__update_mp3, path, tags)
```

### Comparing `pydeezer_asy-2.2.1/deezer_asy/constants/api_methods.py` & `pydeezer_asy-2.2.5/deezer_asy/constants/api_methods.py`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-2.2.1/deezer_asy/constants/track_formats.py` & `pydeezer_asy-2.2.5/deezer_asy/constants/track_formats.py`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-2.2.1/deezer_asy/util.py` & `pydeezer_asy-2.2.5/deezer_asy/util.py`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-2.2.1/pydeezer_asy.egg-info/SOURCES.txt` & `pydeezer_asy-2.2.5/pydeezer_asy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 README.md
 setup.py
 deezer_asy/DeezerAsy.py
 deezer_asy/__init__.py
+deezer_asy/aiodeezer.py
 deezer_asy/exceptions.py
 deezer_asy/util.py
 deezer_asy/constants/__init__.py
 deezer_asy/constants/api_methods.py
 deezer_asy/constants/api_urls.py
 deezer_asy/constants/image_hosts.py
 deezer_asy/constants/networking_settings.py
```

### Comparing `pydeezer_asy-2.2.1/setup.py` & `pydeezer_asy-2.2.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name='pydeezer_asy',
-    version='2.2.1',
+    version='2.2.5',
     description='Asynchronous version of the `py-deezer` module',
     author='drhspfn',
     author_email="drhspfn@gmail.com",
     packages=setuptools.find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/drhspfn/deezer-asy",
```

