# Comparing `tmp/ox-2.3.930.tar.gz` & `tmp/ox-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ox-2.3.930.tar", last modified: Thu Jun 11 18:18:54 2020, max compression
+gzip compressed data, was "dist/ox-3.0.0.tar", last modified: Fri Jul 28 16:53:13 2023, max compression
```

## Comparing `ox-2.3.930.tar` & `ox-3.0.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2020-06-11 18:18:54.000000 ox-2.3.930/
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2020-06-11 18:18:54.000000 ox-2.3.930/ox/
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2020-06-11 18:18:54.000000 ox-2.3.930/ox/torrent/
--rw-r--r--   0 j         (1000) j         (1000)     2358 2016-06-08 13:07:01.000000 ox-2.3.930/ox/torrent/__init__.py
--rw-r--r--   0 j         (1000) j         (1000)     7668 2016-08-27 18:28:16.000000 ox-2.3.930/ox/torrent/bencode.py
--rw-r--r--   0 j         (1000) j         (1000)     3873 2016-10-07 11:58:43.000000 ox-2.3.930/ox/torrent/bencode3.py
--rw-r--r--   0 j         (1000) j         (1000)    11346 2014-10-29 00:45:28.000000 ox-2.3.930/ox/torrent/makemetafile.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2020-06-11 18:18:54.000000 ox-2.3.930/ox/web/
--rw-r--r--   0 j         (1000) j         (1000)      178 2014-10-02 18:17:11.000000 ox-2.3.930/ox/web/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)      700 2014-10-02 18:17:11.000000 ox-2.3.930/ox/web/abebooks.py
--rw-r--r--   0 j         (1000) j         (1000)     3351 2014-10-02 18:17:11.000000 ox-2.3.930/ox/web/allmovie.py
--rw-r--r--   0 j         (1000) j         (1000)     2889 2015-06-05 15:05:14.000000 ox-2.3.930/ox/web/amazon.py
--rw-r--r--   0 j         (1000) j         (1000)     3071 2016-06-08 13:11:26.000000 ox-2.3.930/ox/web/apple.py
--rw-rw-r--   0 j         (1000) j         (1000)     1086 2015-12-25 15:08:13.000000 ox-2.3.930/ox/web/archive.py
--rw-rw-r--   0 j         (1000) j         (1000)     2404 2014-10-02 18:17:11.000000 ox-2.3.930/ox/web/arsenalberlin.py
--rw-r--r--   0 j         (1000) j         (1000)      910 2016-08-22 19:13:05.000000 ox-2.3.930/ox/web/auth.py
--rw-r--r--   0 j         (1000) j         (1000)     4396 2018-07-01 11:13:14.000000 ox-2.3.930/ox/web/criterion.py
--rw-r--r--   0 j         (1000) j         (1000)      921 2016-06-08 13:31:42.000000 ox-2.3.930/ox/web/dailymotion.py
--rw-r--r--   0 j         (1000) j         (1000)      909 2017-06-18 09:08:00.000000 ox-2.3.930/ox/web/duckduckgo.py
--rw-r--r--   0 j         (1000) j         (1000)     1637 2016-06-08 13:13:39.000000 ox-2.3.930/ox/web/epguides.py
--rw-r--r--   0 j         (1000) j         (1000)     1449 2014-10-02 18:17:11.000000 ox-2.3.930/ox/web/filmsdivision.py
--rw-r--r--   0 j         (1000) j         (1000)     1976 2014-10-02 18:17:11.000000 ox-2.3.930/ox/web/flixter.py
--rw-r--r--   0 j         (1000) j         (1000)     1337 2014-10-02 18:17:11.000000 ox-2.3.930/ox/web/freebase.py
--rw-r--r--   0 j         (1000) j         (1000)     1436 2016-05-21 13:15:06.000000 ox-2.3.930/ox/web/google.py
--rw-r--r--   0 j         (1000) j         (1000)    28748 2020-05-12 08:46:04.000000 ox-2.3.930/ox/web/imdb.py
--rw-r--r--   0 j         (1000) j         (1000)    11599 2018-08-01 09:14:13.000000 ox-2.3.930/ox/web/impawards.py
--rw-r--r--   0 j         (1000) j         (1000)     7844 2014-10-05 17:53:46.000000 ox-2.3.930/ox/web/itunes.py
--rw-rw-r--   0 j         (1000) j         (1000)     1513 2014-10-02 18:17:11.000000 ox-2.3.930/ox/web/lookupbyisbn.py
--rw-r--r--   0 j         (1000) j         (1000)      803 2014-10-02 18:17:11.000000 ox-2.3.930/ox/web/lyricsfly.py
--rw-r--r--   0 j         (1000) j         (1000)     2234 2016-06-08 13:15:29.000000 ox-2.3.930/ox/web/metacritic.py
--rw-r--r--   0 j         (1000) j         (1000)     1376 2014-10-02 18:17:11.000000 ox-2.3.930/ox/web/movieposterdb.py
--rw-r--r--   0 j         (1000) j         (1000)     1490 2017-09-19 10:16:07.000000 ox-2.3.930/ox/web/opensubtitles.py
--rw-r--r--   0 j         (1000) j         (1000)      207 2014-10-02 18:17:11.000000 ox-2.3.930/ox/web/oxdb.py
--rw-r--r--   0 j         (1000) j         (1000)      487 2019-08-02 14:26:09.000000 ox-2.3.930/ox/web/piratecinema.py
--rw-r--r--   0 j         (1000) j         (1000)     1821 2016-06-08 13:16:13.000000 ox-2.3.930/ox/web/rottentomatoes.py
--rw-r--r--   0 j         (1000) j         (1000)     3017 2019-08-03 21:34:38.000000 ox-2.3.930/ox/web/siteparser.py
--rw-r--r--   0 j         (1000) j         (1000)    12331 2016-06-08 13:17:44.000000 ox-2.3.930/ox/web/spiegel.py
--rw-r--r--   0 j         (1000) j         (1000)     1446 2016-05-21 12:58:33.000000 ox-2.3.930/ox/web/startpage.py
--rw-r--r--   0 j         (1000) j         (1000)     3758 2016-05-21 12:55:05.000000 ox-2.3.930/ox/web/thepiratebay.py
--rw-r--r--   0 j         (1000) j         (1000)     1184 2014-10-02 18:17:11.000000 ox-2.3.930/ox/web/tv.py
--rw-rw-r--   0 j         (1000) j         (1000)     1360 2014-10-02 18:17:11.000000 ox-2.3.930/ox/web/twitter.py
--rw-rw-r--   0 j         (1000) j         (1000)     5951 2015-06-05 13:46:57.000000 ox-2.3.930/ox/web/ubu.py
--rw-r--r--   0 j         (1000) j         (1000)      493 2014-10-02 18:17:11.000000 ox-2.3.930/ox/web/vimeo.py
--rw-r--r--   0 j         (1000) j         (1000)     1045 2019-10-01 20:18:20.000000 ox-2.3.930/ox/web/wetransfer.py
--rw-r--r--   0 j         (1000) j         (1000)     5366 2019-08-08 14:16:35.000000 ox-2.3.930/ox/web/wikipedia.py
--rw-r--r--   0 j         (1000) j         (1000)     7368 2017-09-19 10:16:18.000000 ox-2.3.930/ox/web/youtube.py
--rw-r--r--   0 j         (1000) j         (1000)      739 2020-06-11 18:18:53.000000 ox-2.3.930/ox/__init__.py
--rw-r--r--   0 j         (1000) j         (1000)       17 2020-03-12 21:07:10.000000 ox-2.3.930/ox/__version.py
--rw-rw-r--   0 j         (1000) j         (1000)     8703 2019-07-23 14:08:55.000000 ox-2.3.930/ox/api.py
--rw-r--r--   0 j         (1000) j         (1000)    16289 2020-06-06 10:08:08.000000 ox-2.3.930/ox/cache.py
--rw-r--r--   0 j         (1000) j         (1000)    12144 2019-12-21 18:29:29.000000 ox-2.3.930/ox/file.py
--rw-rw-r--   0 j         (1000) j         (1000)    12841 2016-06-08 13:29:34.000000 ox-2.3.930/ox/fixunicode.py
--rw-r--r--   0 j         (1000) j         (1000)     3330 2018-01-11 20:40:25.000000 ox-2.3.930/ox/form.py
--rw-r--r--   0 j         (1000) j         (1000)    11716 2016-06-08 12:48:59.000000 ox-2.3.930/ox/format.py
--rw-rw-r--   0 j         (1000) j         (1000)    50515 2016-08-23 16:12:17.000000 ox-2.3.930/ox/geo.py
--rw-r--r--   0 j         (1000) j         (1000)    16378 2016-06-08 10:41:44.000000 ox-2.3.930/ox/html.py
--rw-r--r--   0 j         (1000) j         (1000)    10239 2016-06-08 10:34:42.000000 ox-2.3.930/ox/image.py
--rw-r--r--   0 j         (1000) j         (1000)     7935 2016-06-08 10:36:02.000000 ox-2.3.930/ox/iso.py
--rw-r--r--   0 j         (1000) j         (1000)     7335 2020-05-26 08:17:32.000000 ox-2.3.930/ox/js.py
--rw-r--r--   0 j         (1000) j         (1000)      885 2016-08-28 14:09:57.000000 ox-2.3.930/ox/jsonc.py
--rw-r--r--   0 j         (1000) j         (1000)      777 2012-08-21 06:41:58.000000 ox-2.3.930/ox/location.py
--rw-rw-r--   0 j         (1000) j         (1000)    20989 2017-02-18 12:01:37.000000 ox-2.3.930/ox/movie.py
--rw-r--r--   0 j         (1000) j         (1000)     6014 2020-06-06 09:35:34.000000 ox-2.3.930/ox/net.py
--rw-r--r--   0 j         (1000) j         (1000)     6424 2016-06-08 13:02:36.000000 ox-2.3.930/ox/normalize.py
--rw-rw-r--   0 j         (1000) j         (1000)     1232 2016-06-08 12:56:35.000000 ox-2.3.930/ox/oembed.py
--rw-r--r--   0 j         (1000) j         (1000)     3706 2019-11-21 10:33:23.000000 ox-2.3.930/ox/srt.py
--rw-r--r--   0 j         (1000) j         (1000)    24156 2017-08-02 17:54:03.000000 ox-2.3.930/ox/text.py
--rw-r--r--   0 j         (1000) j         (1000)      392 2014-05-17 16:29:40.000000 ox-2.3.930/ox/utils.py
--rw-r--r--   0 j         (1000) j         (1000)     1139 2016-07-03 13:24:06.000000 ox-2.3.930/ox/vtt.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2020-06-11 18:18:54.000000 ox-2.3.930/ox.egg-info/
--rw-r--r--   0 j         (1000) j         (1000)      649 2020-06-11 18:18:54.000000 ox-2.3.930/ox.egg-info/PKG-INFO
--rw-r--r--   0 j         (1000) j         (1000)     1256 2020-06-11 18:18:54.000000 ox-2.3.930/ox.egg-info/SOURCES.txt
--rw-r--r--   0 j         (1000) j         (1000)        1 2020-06-11 18:18:54.000000 ox-2.3.930/ox.egg-info/dependency_links.txt
--rw-r--r--   0 j         (1000) j         (1000)       19 2020-06-11 18:18:54.000000 ox-2.3.930/ox.egg-info/requires.txt
--rw-r--r--   0 j         (1000) j         (1000)        3 2020-06-11 18:18:54.000000 ox-2.3.930/ox.egg-info/top_level.txt
--rw-r--r--   0 j         (1000) j         (1000)      957 2018-12-23 19:04:02.000000 ox-2.3.930/README.md
--rw-r--r--   0 j         (1000) j         (1000)     2112 2020-06-11 18:18:53.000000 ox-2.3.930/setup.py
--rw-r--r--   0 j         (1000) j         (1000)      649 2020-06-11 18:18:54.000000 ox-2.3.930/PKG-INFO
--rw-r--r--   0 j         (1000) j         (1000)       38 2020-06-11 18:18:54.000000 ox-2.3.930/setup.cfg
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-28 16:53:13.000000 ox-3.0.0/
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-28 16:53:13.000000 ox-3.0.0/ox/
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-28 16:53:13.000000 ox-3.0.0/ox/torrent/
+-rw-r--r--   0 j         (1000) j         (1000)     2313 2023-07-27 16:38:09.000000 ox-3.0.0/ox/torrent/__init__.py
+-rw-r--r--   0 j         (1000) j         (1000)     3873 2016-10-07 11:58:43.000000 ox-3.0.0/ox/torrent/bencode3.py
+-rw-r--r--   0 j         (1000) j         (1000)    11275 2023-07-27 16:38:09.000000 ox-3.0.0/ox/torrent/makemetafile.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-28 16:53:13.000000 ox-3.0.0/ox/web/
+-rw-r--r--   0 j         (1000) j         (1000)      178 2023-07-27 10:59:07.000000 ox-3.0.0/ox/web/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)      700 2023-07-27 10:59:07.000000 ox-3.0.0/ox/web/abebooks.py
+-rw-r--r--   0 j         (1000) j         (1000)     3347 2023-07-27 16:38:09.000000 ox-3.0.0/ox/web/allmovie.py
+-rw-r--r--   0 j         (1000) j         (1000)     2879 2023-07-27 16:38:09.000000 ox-3.0.0/ox/web/amazon.py
+-rw-r--r--   0 j         (1000) j         (1000)     3033 2023-07-27 16:38:09.000000 ox-3.0.0/ox/web/apple.py
+-rw-r--r--   0 j         (1000) j         (1000)     1047 2023-07-27 16:38:09.000000 ox-3.0.0/ox/web/archive.py
+-rw-r--r--   0 j         (1000) j         (1000)     2398 2023-07-27 16:38:09.000000 ox-3.0.0/ox/web/arsenalberlin.py
+-rw-r--r--   0 j         (1000) j         (1000)      910 2023-07-27 10:59:07.000000 ox-3.0.0/ox/web/auth.py
+-rw-r--r--   0 j         (1000) j         (1000)     4694 2023-07-27 16:38:09.000000 ox-3.0.0/ox/web/criterion.py
+-rw-r--r--   0 j         (1000) j         (1000)      911 2023-07-27 16:38:09.000000 ox-3.0.0/ox/web/dailymotion.py
+-rw-r--r--   0 j         (1000) j         (1000)      894 2023-07-27 16:38:09.000000 ox-3.0.0/ox/web/duckduckgo.py
+-rw-r--r--   0 j         (1000) j         (1000)     1637 2023-07-27 10:59:07.000000 ox-3.0.0/ox/web/epguides.py
+-rw-r--r--   0 j         (1000) j         (1000)     1449 2023-07-27 10:59:07.000000 ox-3.0.0/ox/web/filmsdivision.py
+-rw-r--r--   0 j         (1000) j         (1000)     1974 2023-07-27 16:38:09.000000 ox-3.0.0/ox/web/flixter.py
+-rw-r--r--   0 j         (1000) j         (1000)     1337 2023-07-27 10:59:07.000000 ox-3.0.0/ox/web/freebase.py
+-rw-r--r--   0 j         (1000) j         (1000)     2266 2023-07-27 16:38:09.000000 ox-3.0.0/ox/web/google.py
+-rw-r--r--   0 j         (1000) j         (1000)    33811 2023-07-27 16:38:09.000000 ox-3.0.0/ox/web/imdb.py
+-rw-r--r--   0 j         (1000) j         (1000)    11599 2023-07-27 10:59:07.000000 ox-3.0.0/ox/web/impawards.py
+-rw-r--r--   0 j         (1000) j         (1000)     7834 2023-07-27 16:38:09.000000 ox-3.0.0/ox/web/itunes.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1513 2023-07-27 10:59:07.000000 ox-3.0.0/ox/web/lookupbyisbn.py
+-rw-r--r--   0 j         (1000) j         (1000)      803 2023-07-27 10:59:07.000000 ox-3.0.0/ox/web/lyricsfly.py
+-rw-r--r--   0 j         (1000) j         (1000)     2224 2023-07-27 16:38:09.000000 ox-3.0.0/ox/web/metacritic.py
+-rw-r--r--   0 j         (1000) j         (1000)     1376 2023-07-27 10:59:07.000000 ox-3.0.0/ox/web/movieposterdb.py
+-rw-r--r--   0 j         (1000) j         (1000)     1490 2023-07-27 10:59:07.000000 ox-3.0.0/ox/web/opensubtitles.py
+-rw-r--r--   0 j         (1000) j         (1000)      207 2023-07-27 10:59:07.000000 ox-3.0.0/ox/web/oxdb.py
+-rw-r--r--   0 j         (1000) j         (1000)      487 2023-07-27 10:59:07.000000 ox-3.0.0/ox/web/piratecinema.py
+-rw-r--r--   0 j         (1000) j         (1000)     1821 2023-07-27 10:59:07.000000 ox-3.0.0/ox/web/rottentomatoes.py
+-rw-r--r--   0 j         (1000) j         (1000)     3165 2023-07-27 16:38:09.000000 ox-3.0.0/ox/web/siteparser.py
+-rw-r--r--   0 j         (1000) j         (1000)    12331 2023-07-27 10:59:07.000000 ox-3.0.0/ox/web/spiegel.py
+-rw-r--r--   0 j         (1000) j         (1000)     1431 2023-07-27 16:38:09.000000 ox-3.0.0/ox/web/startpage.py
+-rw-r--r--   0 j         (1000) j         (1000)     3748 2023-07-27 16:38:09.000000 ox-3.0.0/ox/web/thepiratebay.py
+-rw-r--r--   0 j         (1000) j         (1000)     1184 2023-07-27 10:59:07.000000 ox-3.0.0/ox/web/tv.py
+-rw-r--r--   0 j         (1000) j         (1000)     1350 2023-07-27 16:38:09.000000 ox-3.0.0/ox/web/twitter.py
+-rw-rw-r--   0 j         (1000) j         (1000)     5951 2023-07-27 10:59:07.000000 ox-3.0.0/ox/web/ubu.py
+-rw-r--r--   0 j         (1000) j         (1000)      493 2023-07-27 10:59:07.000000 ox-3.0.0/ox/web/vimeo.py
+-rw-r--r--   0 j         (1000) j         (1000)     1045 2023-07-27 10:59:07.000000 ox-3.0.0/ox/web/wetransfer.py
+-rw-r--r--   0 j         (1000) j         (1000)     5313 2023-07-27 16:38:09.000000 ox-3.0.0/ox/web/wikipedia.py
+-rw-r--r--   0 j         (1000) j         (1000)     7333 2023-07-27 16:38:09.000000 ox-3.0.0/ox/web/youtube.py
+-rw-r--r--   0 j         (1000) j         (1000)      737 2023-07-28 16:53:12.000000 ox-3.0.0/ox/__init__.py
+-rw-r--r--   0 j         (1000) j         (1000)       15 2023-07-27 22:57:43.000000 ox-3.0.0/ox/__version.py
+-rw-r--r--   0 j         (1000) j         (1000)     7846 2023-07-27 16:38:09.000000 ox-3.0.0/ox/api.py
+-rw-r--r--   0 j         (1000) j         (1000)    15595 2023-07-27 16:38:09.000000 ox-3.0.0/ox/cache.py
+-rw-r--r--   0 j         (1000) j         (1000)    12310 2023-07-27 10:59:14.000000 ox-3.0.0/ox/file.py
+-rw-r--r--   0 j         (1000) j         (1000)    12798 2023-07-27 16:38:09.000000 ox-3.0.0/ox/fixunicode.py
+-rw-r--r--   0 j         (1000) j         (1000)     3249 2023-07-27 16:38:09.000000 ox-3.0.0/ox/form.py
+-rw-r--r--   0 j         (1000) j         (1000)    11668 2023-07-27 16:38:09.000000 ox-3.0.0/ox/format.py
+-rw-rw-r--   0 j         (1000) j         (1000)    50515 2023-07-27 10:59:14.000000 ox-3.0.0/ox/geo.py
+-rw-r--r--   0 j         (1000) j         (1000)    16460 2023-07-27 16:38:09.000000 ox-3.0.0/ox/html.py
+-rw-r--r--   0 j         (1000) j         (1000)    10239 2023-07-27 10:59:14.000000 ox-3.0.0/ox/image.py
+-rw-r--r--   0 j         (1000) j         (1000)     7935 2023-07-27 10:59:14.000000 ox-3.0.0/ox/iso.py
+-rw-r--r--   0 j         (1000) j         (1000)     6998 2023-07-27 16:38:09.000000 ox-3.0.0/ox/js.py
+-rw-r--r--   0 j         (1000) j         (1000)      601 2023-07-27 10:59:14.000000 ox-3.0.0/ox/json_info.py
+-rw-r--r--   0 j         (1000) j         (1000)      885 2023-07-27 10:59:14.000000 ox-3.0.0/ox/jsonc.py
+-rw-r--r--   0 j         (1000) j         (1000)      777 2023-07-27 10:59:14.000000 ox-3.0.0/ox/location.py
+-rw-rw-r--   0 j         (1000) j         (1000)    20989 2023-07-27 10:59:14.000000 ox-3.0.0/ox/movie.py
+-rw-r--r--   0 j         (1000) j         (1000)     5643 2023-07-27 16:38:09.000000 ox-3.0.0/ox/net.py
+-rw-r--r--   0 j         (1000) j         (1000)     6385 2023-07-27 16:38:09.000000 ox-3.0.0/ox/normalize.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1232 2023-07-27 10:59:14.000000 ox-3.0.0/ox/oembed.py
+-rw-r--r--   0 j         (1000) j         (1000)     3592 2023-07-27 16:38:09.000000 ox-3.0.0/ox/srt.py
+-rw-r--r--   0 j         (1000) j         (1000)    24103 2023-07-27 16:38:09.000000 ox-3.0.0/ox/text.py
+-rw-r--r--   0 j         (1000) j         (1000)      392 2023-07-27 10:59:14.000000 ox-3.0.0/ox/utils.py
+-rw-r--r--   0 j         (1000) j         (1000)     1139 2023-07-27 10:59:14.000000 ox-3.0.0/ox/vtt.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-28 16:53:13.000000 ox-3.0.0/ox.egg-info/
+-rw-r--r--   0 j         (1000) j         (1000)      701 2023-07-28 16:53:12.000000 ox-3.0.0/ox.egg-info/PKG-INFO
+-rw-r--r--   0 j         (1000) j         (1000)     1250 2023-07-28 16:53:12.000000 ox-3.0.0/ox.egg-info/SOURCES.txt
+-rw-r--r--   0 j         (1000) j         (1000)        1 2023-07-28 16:53:12.000000 ox-3.0.0/ox.egg-info/dependency_links.txt
+-rw-r--r--   0 j         (1000) j         (1000)        8 2023-07-28 16:53:12.000000 ox-3.0.0/ox.egg-info/requires.txt
+-rw-r--r--   0 j         (1000) j         (1000)        3 2023-07-28 16:53:12.000000 ox-3.0.0/ox.egg-info/top_level.txt
+-rw-r--r--   0 j         (1000) j         (1000)      957 2018-12-23 19:04:02.000000 ox-3.0.0/README.md
+-rw-r--r--   0 j         (1000) j         (1000)     2192 2023-07-28 16:53:12.000000 ox-3.0.0/setup.py
+-rw-rw-r--   0 j         (1000) j         (1000)      701 2023-07-28 16:53:13.000000 ox-3.0.0/PKG-INFO
+-rw-rw-r--   0 j         (1000) j         (1000)       38 2023-07-28 16:53:13.000000 ox-3.0.0/setup.cfg
```

### Comparing `ox-2.3.930/ox/torrent/__init__.py` & `ox-3.0.0/ox/torrent/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 # -*- coding: utf-8 -*-
 # vi:si:et:sw=4:sts=4:ts=4
 # GPL 2007-2012
 
 from threading import Event
 from hashlib import sha1
 import os
-from six import PY2
 
-if PY2:
-    from .bencode import bencode, bdecode
-else:
-    from .bencode3 import bencode, bdecode
+from .bencode3 import bencode, bdecode
 
 __all__ = ['create_torrent', 'get_info_hash', 'get_torrent_info', 'get_files', 'get_torrent_size']
 
 def create_torrent(file, url, params={}, flag=Event(),
                    progress=lambda x: None, progress_percent=1):
     "Creates a torrent for a given file, using url as tracker url"
     from .makemetafile import make_meta_file
@@ -51,15 +47,16 @@
         if key != 'pieces':
             tinfo[key] = info[key]
     for key in metainfo:
         if key != 'info':
             tinfo[key] = metainfo[key]
     tinfo['size'] = file_length
     tinfo['hash'] = sha1(bencode(info)).hexdigest()
-    tinfo['announce'] = metainfo['announce']
+    if 'announce' in metainfo:
+        tinfo['announce'] = metainfo['announce']
     if file:
         tinfo['timestamp'] = os.stat(file).st_ctime
     return tinfo
 
 def get_files(data):
     files = []
     info = get_torrent_info(data=data)
```

### Comparing `ox-2.3.930/ox/torrent/bencode3.py` & `ox-3.0.0/ox/torrent/bencode3.py`

 * *Files identical despite different names*

### Comparing `ox-2.3.930/ox/torrent/makemetafile.py` & `ox-3.0.0/ox/torrent/makemetafile.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,15 @@
 
 from os.path import getsize, split, join, abspath, isdir
 from os import listdir
 from hashlib import sha1 as sha
 from copy import copy
 import re
 
-from six import PY2
-if PY2:
-    from .bencode import bencode
-else:
-    from .bencode3 import bencode
+from .bencode3 import bencode
 from threading import Event
 from time import time
 from traceback import print_exc
 try:
     from sys import getfilesystemencoding
     ENCODING = getfilesystemencoding()
 except:
```

### Comparing `ox-2.3.930/ox/web/abebooks.py` & `ox-3.0.0/ox/web/abebooks.py`

 * *Files identical despite different names*

### Comparing `ox-2.3.930/ox/web/allmovie.py` & `ox-3.0.0/ox/web/allmovie.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 
 def get_id(url):
     return url.split("/")[-1]
 
 def get_data(id):
     '''
     >>> get_data('129689')['cast'][1][1]
-    u'Marianne'
+    'Marianne'
     >>> get_data('129689')['credits'][0][0]
-    u'Jean-Luc Godard'
+    'Jean-Luc Godard'
     >>> get_data('129689')['posters'][0]
-    u'http://image.allmusic.com/00/adg/cov200/dru800/u812/u81260bbffr.jpg'
+    'http://image.allmusic.com/00/adg/cov200/dru800/u812/u81260bbffr.jpg'
     >>> get_data('129689')['rating']
-    u'4.5'
+    '4.5'
     '''
     if id.startswith('http'):
         id = get_id(id)
     data = {
         "url": get_url(id)
     }
     html = read_url(data["url"], unicode=True)
```

### Comparing `ox-2.3.930/ox/web/amazon.py` & `ox-3.0.0/ox/web/amazon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # vi:si:et:sw=4:sts=4:ts=4
 from __future__ import print_function
 import re
-from six.moves.urllib.parse import quote
+from urllib.parse import quote
 
 from ox import find_re, strip_tags, decode_html
 from ox.cache import read_url
 
 import lxml.html
```

### Comparing `ox-2.3.930/ox/web/apple.py` & `ox-3.0.0/ox/web/apple.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from __future__ import print_function
 import json
 import re
 
-from six import text_type
 from ox.cache import read_url
 
 HEADERS = {
     'User-Agent': 'iTunes/10.4 (Macintosh; Intel Mac OS X 10.7) AppleWebKit/534.48.3',
     'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8',
     'Accept-Language': 'en-us, en;q=0.50',
     'X-Apple-Store-Front': '143441-1,12',
     'X-Apple-Tz': '7200',
     'Accept-Encoding': 'gzip, deflate'
 }
 USER_AGENT = 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_7) '
 USER_AGENT += 'AppleWebKit/534.48.3 (KHTML, like Gecko) Version/5.1 Safari/534.48.3'
 
 def get_movie_data(title, director):
-    if isinstance(title, text_type):
+    if isinstance(title, str):
         title = title.encode('utf-8')
-    if isinstance(director, text_type):
+    if isinstance(director, str):
         director = director.encode('utf-8')
     data = {}
     # itunes section (preferred source for link)
     url = 'http://ax.search.itunes.apple.com/WebObjects/MZSearch.woa/wa/advancedSearch'
     url += '?media=movie&movieTerm=' + title
     url += '&actorNames=&directorProducerName=' + director
     url += '&releaseYearTerm=&descriptionTerm=&genreIndex=1&ratingIndex=1'
```

### Comparing `ox-2.3.930/ox/web/archive.py` & `ox-3.0.0/ox/web/archive.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # -*- coding: utf-8 -*-
 # vi:si:et:sw=4:sts=4:ts=4
 from .. import cache
 from ..utils import json
 
-from six import string_types
-
 def get_id(url):
     return url.split("/")[-1]
 
 def get_url(id):
     return "http://www.archive.org/details/%s" % id
 
 def get_data(id):
@@ -17,15 +15,15 @@
     details = cache.read_url('%s?output=json' % url)
     details = json.loads(details)
     for key in ('title', 'description', 'runtime'):
         if key in details['metadata']:
             data[key] = details['metadata'][key]
             if isinstance(data[key], list):
                 data[key] = data[key][0]
-            if isinstance(data[key], string_types):
+            if isinstance(data[key], str):
                 data[key] = data[key].strip()
                 if data[key][0] == '[' and data[key][-1] == ']':
                     data[key] = data[key][1:-1] 
     data['url'] = url
     data['image'] = 'http://archive.org/download/%s/format=thumbnail' % id
     data['ogg'] = 'http://archive.org/download/%s/format=Ogg+video' % id
     data['mp4'] = 'http://archive.org/download/%s/format=512Kb+MPEG4' % id
```

### Comparing `ox-2.3.930/ox/web/arsenalberlin.py` & `ox-3.0.0/ox/web/arsenalberlin.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,39 +15,39 @@
         url = 'http://films.arsenal-berlin.de/index.php/Detail/Object/Show/object_id/%d' % id
     html = read_url(url, unicode=True)
     if 'ID does not exist' in html:
         return None
     if 'Willkommen in der Datenbank des Arsenal' in html:
         return None
     data = {}
-    data[u'id'] = id
-    data[u'url'] = url
+    data['id'] = id
+    data['url'] = url
     m = re.compile('<h1>(.*?)</h1>').findall(html)
     if m:
-        data[u'title'] = m[0]
+        data['title'] = m[0]
     m = re.compile("<b>Director: </b><a href='.*?'>(.*?)</a>").findall(html)
     if m:
-        data[u'director'] = m[0]
+        data['director'] = m[0]
 
     m = re.compile("caUI.initImageScroller\(\[\{url:'(.*?)'").findall(html)
     if m:
-        data[u'image'] = m[0]
+        data['image'] = m[0]
 
     units = re.compile("<div class='unit'>(.*?)</div>", re.DOTALL).findall(html)
     for x in map(re.compile('<b>(.*?)</b>: (.*)', re.DOTALL).findall, units):
         if x:
             #data[x[0][0].lower()] = strip_tags(x[0][1])
             key = x[0][0].lower()
             data[key] = x[0][1]
             if key == "forum catalogue pdf":
                 data[key] = find_re(data[key], '"(http:.*?)"')
             else:
                 data[key] = strip_tags(data[key])
     if "running time (minutes)" in data:
-        data[u'runtime'] = float(data.pop("running time (minutes)").replace(',', '.')) * 60
+        data['runtime'] = float(data.pop("running time (minutes)").replace(',', '.')) * 60
     for key in ('year', 'length in metres', 'forum participation year', 'number of reels'):
         if key in data and data[key].isdigit():
             data[key] = int(data[key])
     return data
 
 def backup(filename):
     if os.path.exists(filename):
```

### Comparing `ox-2.3.930/ox/web/auth.py` & `ox-3.0.0/ox/web/auth.py`

 * *Files identical despite different names*

### Comparing `ox-2.3.930/ox/web/criterion.py` & `ox-3.0.0/ox/web/criterion.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,40 +15,44 @@
 
 def get_url(id):
     return "https://www.criterion.com/films/%s" % id
 
 def get_data(id, timeout=ox.cache.cache_timeout, get_imdb=False):
     '''
     >>> get_data('1333').get('imdbId')
-    u'0060304'
+    '0060304'
 
     >>> get_data('236')['posters'][0]
-    u'http://s3.amazonaws.com/criterion-production/release_images/1586/ThirdManReplace.jpg'
+    'http://s3.amazonaws.com/criterion-production/release_images/1586/ThirdManReplace.jpg'
 
     >>> get_data('786')['posters'][0]
-    u'http://s3.amazonaws.com/criterion-production/product_images/185/343_box_348x490.jpg'
+    'http://s3.amazonaws.com/criterion-production/product_images/185/343_box_348x490.jpg'
     '''
     data = {
         "id": id,
         "url": get_url(id)
     }
     try:
         html = read_url(data["url"], timeout=timeout, unicode=True)
     except:
         html = read_url(data["url"], timeout=timeout).decode('utf-8', 'ignore')
 
     data["number"] = find_re(html, "<b>Spine #(\d+)")
 
     data["title"] = decode_html(find_re(html, "<h1 class=\"header__primarytitle\".*?>(.*?)</h1>"))
-    data["title"] = data["title"].split(u' \u2014 The Television Version')[0].strip()
+    data["title"] = data["title"].split(' \u2014 The Television Version')[0].strip()
     results = find_re(html, '<ul class="film-meta-list">(.*?)</ul>')
     info = re.compile('<li itemprop="(.*?)".*?>(.*?)</li>', re.DOTALL).findall(results)
     info = {k: strip_tags(v).strip() for k, v in info}
+    meta = re.compile('<meta.*? name="(.*?)".*? content="(.*?)"', re.DOTALL).findall(html)
+    meta = {k: v.strip() for k, v in meta}
     if 'director' in info:
         data['director'] = info['director']
+    elif 'director' in meta:
+        data['director'] = meta['director']
     if 'countryOfOrigin' in info:
         data['country'] = [c.strip() for c in decode_html(info['countryOfOrigin']).split(', ')]
     if 'inLanguage' in info:
         data['language'] = [l.strip() for l in decode_html(info['inLanguage']).split(', ')]
     for v in re.compile('<li>(.*?)</li>', re.DOTALL).findall(results):
         if 'datePublished' in v:
             data['year'] = strip_tags(v).strip()
@@ -76,15 +80,16 @@
     data['posters'] = [re.sub('(\?\d+)$', '', p) for p in data['posters']]
     data['posters'] = [p for p in data['posters'] if p]
 
     posters = find_re(html, '<div class="product-box-art".*?>(.*?)</div>')
     for poster in re.compile('<img src="(.*?)"').findall(posters):
         data['posters'].append(poster)
 
-    result = find_re(html, "<img alt=\"Film Still\" height=\"252\" src=\"(.*?)\"")
+    result = re.compile('<div class="gallery-item ">.*?src="(.*?)"', re.DOTALL).findall(html)
+    #result = find_re(html, "<img alt=\"Film Still\" height=\"252\" src=\"(.*?)\"")
     if result:
         data["stills"] = [result]
         data["trailers"] = []
     else:
         data["stills"] = list(filter(lambda x: x, [find_re(html, "\"thumbnailURL\", \"(.*?)\"")]))
         data["trailers"] = list(filter(lambda x: x, [find_re(html, "\"videoURL\", \"(.*?)\"")]))
```

### Comparing `ox-2.3.930/ox/web/dailymotion.py` & `ox-3.0.0/ox/web/dailymotion.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # vi:si:et:sw=4:sts=4:ts=4
 import re
-from six.moves.urllib.parse import unquote
+from urllib.parse import unquote
 from ox.cache import read_url
 
 
 def get_video_url(url):
     '''
     >>> get_video_url('http://www.dailymotion.com/relevance/search/priere%2Bpour%2Brefuznik/video/x3opar_priere-pour-refuznik-1-jeanluc-goda_shortfilms').split('?auth')[0]
     'http://www.dailymotion.com/cdn/FLV-320x240/video/x3opar_priere-pour-refuznik-1-jean-luc-god_shortfilms.flv'
```

### Comparing `ox-2.3.930/ox/web/duckduckgo.py` & `ox-3.0.0/ox/web/duckduckgo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # vi:si:et:sw=4:sts=4:ts=4
 import re
 
-from six.moves import urllib
+import urllib
 import ox
 from ox import strip_tags, decode_html
 from ox.cache import read_url
 import lxml.html
 
 
 def find(query, timeout=ox.cache.cache_timeout):
```

### Comparing `ox-2.3.930/ox/web/epguides.py` & `ox-3.0.0/ox/web/epguides.py`

 * *Files identical despite different names*

### Comparing `ox-2.3.930/ox/web/filmsdivision.py` & `ox-3.0.0/ox/web/filmsdivision.py`

 * *Files identical despite different names*

### Comparing `ox-2.3.930/ox/web/flixter.py` & `ox-3.0.0/ox/web/flixter.py`

 * *Files 14% similar despite different names*

```diff
@@ -54,18 +54,18 @@
     if not 'title' in data:
         return None
     return data
 
 def get_id(url=None, imdb=None):
     '''
     >>> get_id(imdb='0133093')
-    u'the-matrix'
+    'the-matrix'
 
     #>>> get_id(imdb='0060304')
-    #u'2-or-3-things-i-know-about-her'
+    #'2-or-3-things-i-know-about-her'
     '''
     if imdb:
         i = ImdbCombined(imdb)
         title = i['title']
         return title.replace(' ', '-').lower().replace("'", '')
     return url.split('/')[-1]
```

### Comparing `ox-2.3.930/ox/web/freebase.py` & `ox-3.0.0/ox/web/freebase.py`

 * *Files identical despite different names*

### Comparing `ox-2.3.930/ox/web/google.py` & `ox-3.0.0/ox/web/startpage.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
 # vi:si:et:sw=4:sts=4:ts=4
-import re
-from six.moves import urllib
+import urllib
 
+import lxml.html
 import ox
-from ox import strip_tags, decode_html
 
 DEFAULT_MAX_RESULTS = 10
 DEFAULT_TIMEOUT = 24*60*60
 
 def read_url(url, data=None, headers=ox.net.DEFAULT_HEADERS, timeout=DEFAULT_TIMEOUT):
     return ox.cache.read_url(url, data, headers, timeout, unicode=True)
 
@@ -17,28 +16,29 @@
         s = s.encode('utf-8')
     return urllib.parse.quote_plus(s)
 
 def find(query, max_results=DEFAULT_MAX_RESULTS, timeout=DEFAULT_TIMEOUT):
     """
     Return max_results tuples with title, url, description 
 
-    >>> str(find("The Matrix site:imdb.com", 1)[0][0])
+    >>> find("The Matrix site:imdb.com", 1)[0][0]
     'The Matrix (1999) - IMDb'
 
-    >>> str(find("The Matrix site:imdb.com", 1)[0][1])
+    >>> find("The Matrix site:imdb.com", 1)[0][1]
     'http://www.imdb.com/title/tt0133093/'
     """
     results = []
-    offset = 0
-    while len(results) < max_results:
-        url = 'http://google.com/search?q=%s' % quote_plus(query)
-        if offset:
-            url += '&start=%d' % offset
-        data = read_url(url, timeout=timeout)
-        data = re.sub('<span class="f">(.*?)</span>', '\\1', data)
-        for a in re.compile('<a href="(htt\S+?)".*?>(.*?)</a>.*?<span class="st">(.*?)<\/span>').findall(data):
-            results.append((strip_tags(decode_html(a[1])), a[0], strip_tags(decode_html(a[2]))))
+    url = 'https://eu1.startpage.com/do/search?nosteeraway=1&abp=1&language=english&cmd=process_search&query=%s&x=0&y=0&cat=web&engine0=v1all' % quote_plus(query)
+
+    data = read_url(url, timeout=timeout)
+    doc = lxml.html.document_fromstring(data)
+    for r in doc.xpath("//div[contains(@class, 'result')]"):
+        t = r.find('h3')
+        if t is not None:
+            title = t.text_content().strip()
+            url = t.find('a').attrib['href']
+            description = r.find_class('desc')[0].text_content()
+            results.append((title, url, description))
             if len(results) >= max_results:
                 break
-        offset += 10
     return results
```

### Comparing `ox-2.3.930/ox/web/imdb.py` & `ox-3.0.0/ox/web/imdb.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 # vi:si:et:sw=4:sts=4:ts=4
-from __future__ import print_function
+from collections import defaultdict
 
+import json
 import re
 import time
 import unicodedata
 
-from six.moves.urllib.parse import urlencode
-from six import text_type, string_types
+from urllib.parse import urlencode
 
 from .. import find_re, strip_tags, decode_html
 from .. import cache
 
 
 from . siteparser import SiteParser
 from . import duckduckgo
 from ..utils import datetime
-from ..geo import normalize_country_name
+from ..geo import normalize_country_name, get_country_name
 
 
 def prepare_url(url, data=None, headers=cache.DEFAULT_HEADERS, timeout=cache.cache_timeout, valid=None, unicode=False):
     headers = headers.copy()
     # https://webapps.stackexchange.com/questions/11003/how-can-i-disable-reconfigure-imdbs-automatic-geo-location-so-it-does-not-defau
-    headers['X-Forwarded-For'] = '72.21.206.80'
+    #headers['X-Forwarded-For'] = '72.21.206.80'
     headers['Accept-Language'] = 'en'
 
     return url, data, headers, timeout, unicode
 
 def read_url(url, data=None, headers=cache.DEFAULT_HEADERS, timeout=cache.cache_timeout, valid=None, unicode=False):
     url, data, headers, timeout, unicode = prepare_url(url, data, headers, timeout, valid, unicode)
     return cache.read_url(url, data, headers, timeout, unicode=unicode)
@@ -102,36 +102,160 @@
                 re.sub('\s+', ' ', d.strip()) for d in data.strip().split('<br>')
             ] if data else []
         ],
         'type': 'list'
     }
 
 
+def tech_spec(metadata):
+    tech = {}
+    for row in metadata['props']['pageProps']['contentData']['section']['items']:
+        title = {
+            'aspect ratio': 'aspectratio',
+            'sound mix': 'sound',
+        }.get(row['rowTitle'].lower(), row['rowTitle'].lower())
+        tech[title] = []
+        for content in row['listContent']:
+            value = content['text']
+            tech[title].append(value)
+    return tech
+
+
+def movie_connections(metadata):
+    
+    connections = {}
+    if 'props' not in metadata:
+        return connections
+    for row in metadata['props']['pageProps']['contentData']['categories']:
+        title = {
+        }.get(row['name'], row['name'])
+        if title not in connections:
+            connections[title] = []
+
+        for item in row['section']['items']:
+            item_ = {
+                'id': item['id'][2:],
+            }
+
+            item_['title'] = re.compile('<a.*?>(.*?)</a>').findall(item['listContent'][0]['html'])[0]
+            if len(item['listContent']) >=2:
+                item_['description'] = strip_tags(item['listContent'][1]['html'])
+            connections[title].append(item_)
+    return connections
+
+
+def get_category_by_id(metadata, id):
+    for category in metadata['props']['pageProps']['contentData']['categories']:
+        if category['id'] == id:
+            return category
+
+
+def get_release_date(metadata):
+    releases = get_category_by_id(metadata, 'releases')
+    def parse_date(d):
+        parsed = None
+        for fmt in (
+            '%B %d, %Y',
+            '%d %B %Y',
+            '%B %Y',
+        ):
+            try:
+                parsed = datetime.strptime(d, fmt)
+                break
+            except:
+                pass
+        if not parsed:
+            return None
+        return '%d-%02d-%02d' % (parsed.year, parsed.month, parsed.day)
+
+    dates = []
+    for item in releases['section']['items']:
+        content = item['listContent'][0]
+        date = parse_date(content['text'])
+        if date:
+            dates.append(date)
+
+    if dates:
+        return min(dates)
+
+def get_locations(metadata):
+    try:
+        locations = [
+            row['cardText']
+            for row in metadata['props']['pageProps']['contentData']['categories'][0]['section']['items']
+        ]
+    except:
+        locations = []
+    return locations
+
+
+def get_keywords(metadata):
+    try:
+        keywords = [
+            row['rowTitle']
+            for row in metadata['props']['pageProps']['contentData']['section']['items']
+        ]
+    except:
+        keywords = []
+    return keywords
+
+
+def get_entity_metadata(metadata):
+    data = {}
+    entity = metadata['props']['pageProps']['contentData']['entityMetadata']
+    data['title'] = entity['titleText']['text']
+    data['originalTitle'] = entity['originalTitleText']['text']
+    data['year'] = entity['releaseYear']['year']
+    data['plot'] = entity['plot']['plotText']['plainText']
+    data['country'] = [get_country_name(c['id']) for c in entity['countriesOfOrigin']['countries']]
+    data['poster'] = metadata['props']['pageProps']['contentData']['posterData']['image']['url']
+    return data
+
+
+def alternative_titles(metadata):
+    titles = defaultdict(list)
+    akas = get_category_by_id(metadata, 'akas')
+
+    skip = [
+        metadata['props']['pageProps']['contentData']['entityMetadata']['titleText']['text'],
+        metadata['props']['pageProps']['contentData']['entityMetadata']['originalTitleText']['text']
+    ]
+    for row in akas['section']['items']:
+        content = row['listContent'][0]
+        title = content['text']
+        country = row['rowTitle']
+        if title in skip:
+            continue
+        titles[title].append(country)
+        #if content.get('subText'):
+        #    titles[-1]['subText'] = content['subText']
+    return [kv for kv in titles.items()]
+
+
 '''
 'posterIds': {
     'page': 'posters',
     're': '/unknown-thumbnail/media/rm(.*?)/tt',
     'type': 'list'
 },
 '''
 
 class Imdb(SiteParser):
     '''
-    >>> Imdb('0068646')['title'] == text_type(u'The Godfather')
+    >>> Imdb('0068646')['title'] == 'The Godfather'
     True
 
-    >>> Imdb('0133093')['title'] == text_type(u'The Matrix')
+    >>> Imdb('0133093')['title'] == 'The Matrix'
     True
     '''
     regex = {
         'alternativeTitles': {
             'page': 'releaseinfo',
             're': [
-                '<h4[^>]*?id="akas"[^>]*?>(.*?)</table>',
-                "td[^>]*?>(.*?)</td>.*?<td[^>]*?>(.*?)</td>"
+                '<li role="presentation" class="ipc-metadata-list__item" data-testid="list-item"><button class="ipc-metadata-list-item__label" role="button" tabindex="0" aria-disabled="false">([^>]+)</button.*?<li role="presentation" class="ipc-inline-list__item"><label class="ipc-metadata-list-item__list-content-item"[^>]*?>([^<]+)</label>',
             ],
             'type': 'list'
         },
         'aspectratio': {
             'page': 'reference',
             're': [
                 'Aspect Ratio</td>.*?ipl-inline-list__item">\s+([\d\.\:\ ]+)',
@@ -148,58 +272,31 @@
                 ' <table class="cast_list">(.*?)</table>',
                 '<td.*?itemprop="actor".*?>.*?>(.*?)</a>.*?<td class="character">(.*?)</td>',
                 lambda ll: [strip_tags(l) for l in ll] if isinstance(ll, list) else strip_tags(ll)
             ],
             'type': 'list'
         },
         'cinematographer': reference_section('cinematographers'),
-        'connections': {
-            'page': 'movieconnections',
-            're': '<h4 class="li_group">(.*?)</h4>(.*?)(<\/div>\n  <a|<script)',
-            'type': 'list'
-        },
         'country': zebra_list('Country', more=['<a.*?>(.*?)</a>']),
-        'creator': {
-            'page': '',
-            're': [
-                '<div class="credit_summary_item">.*?<h4.*?>Creator.?:</h4>(.*?)</div>',
-                '<a href="/name/.*?>(.*?)</a>',
-                lambda ll: strip_tags(ll)
-            ],
-            'type': 'list'
-        },
         'director': reference_section('directors'),
         'editor': reference_section('editors'),
         'composer': reference_section('composers'),
         'episodeTitle': {
             'page': 'reference',
             're': '<h3 itemprop="name">(.*?)<',
             'type': 'string'
         },
-        'filmingLocations': {
-            'page': 'locations',
-            're': [
-                '<a href="/search/title\?locations=.*?".*?>(.*?)</a>',
-                lambda data: data.strip(),
-            ],
-            'type': 'list'
-        },
         'genre': zebra_list('Genres', more=['<a.*?>(.*?)</a>']),
         'gross': zebra_table('Cumulative Worldwide Gross', more=[
             lambda data: find_re(decode_html(data).replace(',', ''), '\d+')
         ], type='int'),
-        'keyword': {
-            'page': 'keywords',
-            're': 'data-item-keyword="(.*?)"',
-            'type': 'list'
-        },
         'language': zebra_list('Language', more=['<a.*?>(.*?)</a>']),
         'originalTitle': {
             'page': 'releaseinfo',
-            're': '<td.*?>\s*?\(original title\)\s*?</td>\s*<td.*?>(.*?)</td>',
+            're': '<li role="presentation" class="ipc-metadata-list__item" data-testid="list-item"><button class="ipc-metadata-list-item__label" role="button" tabindex="0" aria-disabled="false">\(original title\)</button.*?<li role="presentation" class="ipc-inline-list__item"><label class="ipc-metadata-list-item__list-content-item"[^>]*?>([^<]+)</label>',
             'type': 'string'
         },
         'summary': zebra_table('Plot Summary', more=[
             '<p>(.*?)<em'
         ]),
         'storyline': {
             'page': '',
@@ -224,22 +321,14 @@
             'page': 'reference',
             're': [
                 '<div class="ipl-rating-star ">(.*?)</div>',
                 'ipl-rating-star__rating">([\d,.]+?)</span>',
             ],
             'type': 'float'
         },
-        'releasedate': {
-            'page': 'releaseinfo',
-            're': [
-                '<td class="release-date-item__date".*?>(.*?)</td>',
-                strip_tags,
-            ],
-            'type': 'list'
-        },
         #FIXME using some /offsite/ redirect now
         #'reviews': {
         #    'page': 'externalreviews',
         #    're': [
         #        '<ul class="simpleList">(.*?)</ul>',
         #        '<li>.*?<a href="(http.*?)".*?>(.*?)</a>.*?</li>'
         #    ],
@@ -247,19 +336,14 @@
         #},
         'runtime': zebra_list('Runtime'),
         'color': zebra_list('Color', more=[
             '<a.*?>([^(<]+)',
             lambda r: r[0] if isinstance(r, list) else r,
             strip_tags
         ]),
-        'sound': zebra_list('Sound Mix', more=[
-            '<a.*?>([^(<]+)',
-            lambda r: r[0] if isinstance(r, list) else r,
-            strip_tags
-        ]),
         'season': {
             'page': 'reference',
             're': [
                 '<ul class="ipl-inline-list titlereference-overview-season-episode-numbers">(.*?)</ul>',
                 'Season (\d+)',
              ],
             'type': 'int'
@@ -280,15 +364,15 @@
         'isSeries': {
             'page': 'reference',
             're': 'property=\'og:title\'.*?content=".*?(TV series|TV mini-series).*?"',
             'type': 'string'
         },
         'title': {
             'page': 'releaseinfo',
-            're': 'h3 itemprop="name">.*?>(.*?)</a>',
+            're': '<h2.*?>(.*?)</h2>',
             'type': 'string'
         },
         'trivia': {
             'page': 'trivia',
             're': [
                 '<div class="sodatext">(.*?)<(br|/div)',
                 lambda data: data[0]
@@ -319,41 +403,56 @@
                 '>(.*?)</h4>.*?(<table.*?</table>)',
                 lambda data: [d for d in data if d]
             ],
             'type': 'list'
         },
         'laboratory': technical('Laboratory'),
         'camera': technical('Camera'),
-        'negative format': technical('Negative Format'),
-        'cinematographic process': technical('Cinematographic Process'),
-        'printed film format': technical('Printed Film Format'),
     }
 
     def read_url(self, url, timeout):
+        if self.debug:
+            print(url)
         if url not in self._cache:
             self._cache[url] = read_url(url, timeout=timeout, unicode=True)
         return self._cache[url]
 
+    def get_page_data(self, page, timeout=-1):
+        url = self.get_url(page)
+        data = self.read_url(url, timeout)
+        pdata = re.compile('<script id="__NEXT_DATA__" type="application/json">(.*?)</script>', re.DOTALL).findall(data)
+        if pdata:
+            pdata = pdata[0]
+            return json.loads(pdata)
+        return {}
+
     def __init__(self, id, timeout=-1):
         # http://www.imdb.com/help/show_leaf?titlelanguagedisplay
         self.baseUrl = "http://www.imdb.com/title/tt%s/" % id
+        self._id = id
+        if timeout != 0:
+            self._cache = {}
+            url = self.baseUrl + 'releaseinfo'
+            page = self.read_url(url, timeout=-1)
+            if '<h2>See also</h2>' in page:
+                timeout = 0
         super(Imdb, self).__init__(timeout)
 
         url = self.baseUrl + 'reference'
         page = self.read_url(url, timeout=-1)
         if '<title>IMDb: Page not found</title>' in page \
             or 'The requested URL was not found on our server.' in page:
             return
         if "<p>We're sorry, something went wrong.</p>" in page:
             time.sleep(1)
             super(Imdb, self).__init__(0)
 
         if 'alternativeTitles' in self:
             if len(self['alternativeTitles']) == 2 and \
-               isinstance(self['alternativeTitles'][0], string_types):
+               isinstance(self['alternativeTitles'][0], str):
                self['alternativeTitles'] = [self['alternativeTitles']]
 
         for key in ('country', 'genre', 'language', 'sound', 'color'):
             if key in self:
                 self[key] = [x[0] if len(x) == 1 and isinstance(x, list) else x for x in self[key]]
                 self[key] = list(filter(lambda x: x.lower() != 'home', self[key]))
 
@@ -410,94 +509,31 @@
         if 'runtime' in self and not self['runtime']:
             del self['runtime']
 
         if 'sound' in self:
             self['sound'] = list(sorted(set(self['sound'])))
 
         if 'cast' in self:
-            if isinstance(self['cast'][0], string_types):
+            if isinstance(self['cast'][0], str):
                 self['cast'] = [self['cast']]
             self['actor'] = [c[0] for c in self['cast']]
             def cleanup_character(c):
                 c = c.replace('(uncredited)', '').strip()
                 c = re.sub('\s+', ' ', c)
                 return c
             self['cast'] = [{'actor': x[0], 'character': cleanup_character(x[1])}
                             for x in self['cast']]
 
-        if 'connections' in self:
-            cc={}
-            if len(self['connections']) == 3 and isinstance(self['connections'][0], string_types):
-                self['connections'] = [self['connections']]
-            for rel, data, _ in self['connections']:
-                if isinstance(rel, bytes):
-                    rel = rel.decode('utf-8')
-                #cc[rel] = re.compile('<a href="/title/tt(\d+)/">(.*?)</a>').findall(data)
-                def get_conn(c):
-                    r = {
-                        'id': c[0],
-                        'title': cleanup_title(c[1]),
-                    }
-                    description = c[2].split('<br />')
-                    if len(description) == 2 and description[-1].strip() != '-':
-                        r['description'] = description[-1].strip()
-                    return r
-                cc[rel] = list(map(get_conn, re.compile('<a href="/title/tt(\d+)/?">(.*?)</a>(.*?)<\/div', re.DOTALL).findall(data)))
-
-            self['connections'] = cc
 
         if 'isSeries' in self:
             del self['isSeries']
             self['isSeries'] = True
         if 'episodeTitle' in self:
             self['episodeTitle'] = re.sub('Episode \#\d+\.\d+', '', self['episodeTitle'])
 
-        if 'series' in self:
-            series = Imdb(self['series'], timeout=timeout)
-            self['seriesTitle'] = series['title']
-            if 'episodeTitle' in self:
-                self['seriesTitle'] = series['title']
-                if 'season' in self and 'episode' in self:
-                    self['title'] = "%s (S%02dE%02d) %s" % (
-                        self['seriesTitle'], self['season'], self['episode'], self['episodeTitle'])
-                else:
-                    self['title'] = "%s (S01) %s" % (self['seriesTitle'], self['episodeTitle'])
-                    self['season'] = 1
-                self['title'] = self['title'].strip()
-            if 'director' in self:
-                self['episodeDirector'] = self['director']
-
-            if 'creator' not in series and 'director' in series:
-                series['creator'] = series['director']
-                if len(series['creator']) > 10:
-                    series['creator'] = series['director'][:1]
-
-            for key in ['creator', 'country']:
-                if key in series:
-                    self[key] = series[key]
-
-            if 'year' in series:
-                self['seriesYear'] = series['year']
-                if 'year' not in self:
-                    self['year'] = series['year']
-
-            if 'year' in self:
-                self['episodeYear'] = self['year']
-            if 'creator' in self:
-                self['seriesDirector'] = self['creator']
-            if 'originalTitle' in self:
-                del self['originalTitle']
-        else:
-            for key in ('seriesTitle', 'episodeTitle', 'season', 'episode'):
-                if key in self:
-                    del self[key]
-        if 'creator' in self:
-            if 'director' in self:
-                self['episodeDirector'] = self['director']
-            self['director'] = self['creator']
 
         #make lists unique but keep order
         for key in ('director', 'language'):
             if key in self:
                 self[key] = [x for i,x in enumerate(self[key])
                              if x not in self[key][i+1:]]
 
@@ -507,36 +543,51 @@
                     self[key] = [i[0] for i in self[key] if i]
                 self[key] = sorted(list(set(self[key])), key=lambda a: self[key].index(a))
 
 
         if 'budget' in self and 'gross' in self:
             self['profit'] = self['gross'] - self['budget']
 
-        if 'releasedate' in self:
-            def parse_date(d):
-                try:
-                    d = datetime.strptime(d, '%d %B %Y')
-                except:
-                    try:
-                        d = datetime.strptime(d, '%B %Y')
-                    except:
-                        return 'x'
-                return '%d-%02d-%02d' % (d.year, d.month, d.day)
-            self['releasedate'] = min([
-                parse_date(d) for d in self['releasedate']
-            ])
-            if self['releasedate'] == 'x':
-                del self['releasedate']
+        metadata = self.get_page_data('releaseinfo')
+        releasedate = get_release_date(metadata)
+        if releasedate:
+            self['releasedate'] = releasedate
+
+        metadata = self.get_page_data('keywords')
+        keywords = get_keywords(metadata)
+        if keywords:
+            self['keyword'] = keywords
+
+        metadata = self.get_page_data('locations')
+        locations = get_locations(metadata)
+        if locations:
+            self['filmingLocations'] = locations
 
         if 'summary' not in self and 'storyline' in self:
             self['summary'] = self.pop('storyline')
         if 'summary' in self:
             if isinstance(self['summary'], list):
                 self['summary'] = self['summary'][0]
             self['summary'] = strip_tags(self['summary'].split('</p')[0]).split('  Written by\n')[0].strip()
+        else:
+
+            try:
+                summary = metadata['props']['pageProps']['contentData']['entityMetadata']['plot']['plotText']['plainText']
+                self['summary'] = summary
+
+            except:
+                pass
+
+        #self['connections'] = movie_connections(self.get_page_data('movieconnections'))
+        self['connections'] = self._get_connections()
+
+        spec = tech_spec(self.get_page_data('technical'))
+        for key in spec:
+            if not self.get(key):
+                self[key] = spec[key]
 
         if 'credits' in self:
             credits = [
                 [
                     strip_tags(d[0].replace(' by', '')).strip(),
                     [
                         [
@@ -577,14 +628,123 @@
                 ('writer', 'Series Writing Credits'),
                 ('cinematographer', 'Series Cinematography'),
             ):
                 if key not in self:
                     series_credit = [c for c in self['credits'] if c.get('deparment') == deparment]
                     if series_credit:
                         self[key] = [c['name'] for c in series_credit]
+        creator = []
+        for c in self.get('credits', []):
+            if '(created by)' in c['roles'] and c['name'] not in creator:
+                creator.append(c['name'])
+            if '(creator)' in c['roles'] and c['name'] not in creator:
+                creator.append(c['name'])
+        if creator:
+            self['creator'] = creator
+
+        if 'series' in self:
+            series = Imdb(self['series'], timeout=timeout)
+            self['seriesTitle'] = series['title']
+            if 'episodeTitle' in self:
+                self['seriesTitle'] = series['title']
+                if 'season' in self and 'episode' in self:
+                    self['title'] = "%s (S%02dE%02d) %s" % (
+                        self['seriesTitle'], self['season'], self['episode'], self['episodeTitle'])
+                else:
+                    self['title'] = "%s (S01) %s" % (self['seriesTitle'], self['episodeTitle'])
+                    self['season'] = 1
+                self['title'] = self['title'].strip()
+            if 'director' in self:
+                self['episodeDirector'] = self['director']
+
+            if 'creator' not in series and 'director' in series:
+                series['creator'] = series['director']
+                if len(series['creator']) > 10:
+                    series['creator'] = series['director'][:1]
+
+            for key in ['creator', 'country']:
+                if key in series:
+                    self[key] = series[key]
+
+            if 'year' in series:
+                self['seriesYear'] = series['year']
+                if 'year' not in self:
+                    self['year'] = series['year']
+
+            if 'year' in self:
+                self['episodeYear'] = self['year']
+            if 'creator' in self:
+                self['seriesDirector'] = self['creator']
+            if 'originalTitle' in self:
+                del self['originalTitle']
+        else:
+            for key in ('seriesTitle', 'episodeTitle', 'season', 'episode'):
+                if key in self:
+                    del self[key]
+        if 'creator' in self:
+            if 'director' in self:
+                self['episodeDirector'] = self['director']
+            self['director'] = self['creator']
+
+    def _get_connections(self):
+        query = '''query {
+    title(id: "tt%s") {
+        id
+        titleText {
+           text
+        }
+        connections(first: 5000) {
+            edges {
+                node {
+                    associatedTitle {
+                        id
+                        titleText {
+                            text
+                        }
+                    }
+                    category {
+                        text
+                    }
+                    text
+                }
+            }
+        }
+    }
+}
+''' % self._id
+        url = 'https://caching.graphql.imdb.com/'
+        headers = cache.DEFAULT_HEADERS.copy()
+        headers.update({
+             'Accept': 'application/graphql+json, application/json',
+             'Origin': 'https://www.imdb.com',
+             'Referer': 'https://www.imdb.com',
+             'x-imdb-user-country': 'US',
+             'x-imdb-user-language': 'en-US',
+             'content-type': 'application/json',
+             'Accept-Language': 'en,en-US;q=0.5'
+        })
+        #response = requests.post(url, json=
+        response = json.loads(read_url(url, data=json.dumps({
+            "query": query
+        }), headers=headers))
+        connections = {}
+        for c in response['data']['title']['connections']['edges']:
+            cat = c['node']['category']['text']
+            if cat not in connections:
+                connections[cat] = []
+            connection = {
+                'id': c['node']['associatedTitle']['id'][2:],
+                'title': c['node']['associatedTitle']['titleText']['text'],
+            }
+            description = c['node'].get('text', '')
+            if description:
+                connection['description'] = description
+            connections[cat].append(connection)
+        return connections
+
 
 class ImdbCombined(Imdb):
     def __init__(self, id, timeout=-1):
         _regex = {}
         for key in self.regex:
             if self.regex[key]['page'] in ('releaseinfo', 'reference'):
                 _regex[key] = self.regex[key]
```

### Comparing `ox-2.3.930/ox/web/impawards.py` & `ox-3.0.0/ox/web/impawards.py`

 * *Files identical despite different names*

### Comparing `ox-2.3.930/ox/web/itunes.py` & `ox-3.0.0/ox/web/itunes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # vi:si:et:sw=4:sts=4:ts=4
 # encoding: utf-8
 from __future__ import print_function
 import re
-from six.moves.urllib.parse import urlencode
+from urllib.parse import urlencode
 
 from ox.cache import read_url
 from ox.html import decode_html, strip_tags
 from ox.text import find_re
 from ox.text import find_string
```

### Comparing `ox-2.3.930/ox/web/lookupbyisbn.py` & `ox-3.0.0/ox/web/lookupbyisbn.py`

 * *Files identical despite different names*

### Comparing `ox-2.3.930/ox/web/lyricsfly.py` & `ox-3.0.0/ox/web/lyricsfly.py`

 * *Files identical despite different names*

### Comparing `ox-2.3.930/ox/web/metacritic.py` & `ox-3.0.0/ox/web/metacritic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # vi:si:et:sw=4:sts=4:ts=4
 import re
 
-from six.moves.urllib.parse import quote
+from urllib.parse import quote
 from lxml.html import document_fromstring
 
 from ox.cache import read_url
 from ox import find_re, strip_tags
 
 def get_url(id=None, imdb=None):
     if imdb:
```

### Comparing `ox-2.3.930/ox/web/movieposterdb.py` & `ox-3.0.0/ox/web/movieposterdb.py`

 * *Files identical despite different names*

### Comparing `ox-2.3.930/ox/web/opensubtitles.py` & `ox-3.0.0/ox/web/opensubtitles.py`

 * *Files identical despite different names*

### Comparing `ox-2.3.930/ox/web/rottentomatoes.py` & `ox-3.0.0/ox/web/rottentomatoes.py`

 * *Files identical despite different names*

### Comparing `ox-2.3.930/ox/web/siteparser.py` & `ox-3.0.0/ox/web/siteparser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # -*- coding: utf-8 -*-
 # vi:si:et:sw=4:sts=4:ts=4
 import re
+import json
 from multiprocessing.pool import ThreadPool
 
-from six import string_types
-
 from ..cache import read_url
 from .. import decode_html
 from ..utils import datetime
 
 
 def cleanup(key, data, data_type):
     if data:
-        if isinstance(data[0], string_types):
+        if isinstance(data[0], str):
             #FIXME: some types need strip_tags
             #data = [strip_tags(decode_html(p)).strip() for p in data]
             data = [decode_html(p).strip() for p in data]
         elif isinstance(data[0], list) or isinstance(data[0], tuple):
             data = [cleanup(key, p, data_type) for p in data]
-        while len(data) == 1 and not isinstance(data, string_types):
+        while len(data) == 1 and not isinstance(data, str):
             data = data[0]
-        if data_type == 'list' and isinstance(data, string_types):
+        if data_type == 'list' and isinstance(data, str):
             data = [data, ]
     elif data_type != 'list':
         data = ''
     return data
 
 class SiteParser(dict):
     baseUrl = ''
     regex = {}
     pool = ThreadPool(8)
+    debug = False
 
     def get_url(self, page):
         return "%s%s" % (self.baseUrl, page)
 
     def read_url(self, url, timeout):
         if url not in self._cache:
             self._cache[url] = read_url(url, timeout=timeout, unicode=True)
@@ -43,26 +43,26 @@
         self._cache = {}
         urls = list(set(self.get_url(self.regex[key]['page']) for key in self.regex))
         self.pool.map(self.get_url, urls)
 
         for key in self.regex:
             url = self.get_url(self.regex[key]['page'])
             data = self.read_url(url, timeout)
-            if isinstance(self.regex[key]['re'], string_types):
+            if isinstance(self.regex[key]['re'], str):
                 data = re.compile(self.regex[key]['re'], re.DOTALL).findall(data)
                 data = cleanup(key, data, self.regex[key]['type'])
             elif callable(self.regex[key]['re']):
                 data = self.regex[key]['re'](data)
             else:
                 for r in self.regex[key]['re']:
                     if callable(r):
                         f = r
                     else:
                         f = re.compile(r, re.DOTALL).findall
-                    if isinstance(data, string_types):
+                    if isinstance(data, str):
                         data = f(data)
                     else:
                         data = [f(d) for d in data]
                         data = cleanup(key, data, self.regex[key]['type'])
             def apply_f(f, data):
                 if data and isinstance(data[0], list):
                     data = [f(d) for d in data]
@@ -72,10 +72,14 @@
             if self.regex[key]['type'] == 'float' and data:
                 data = apply_f(float, data)
             elif self.regex[key]['type'] == 'int' and data:
                 data = apply_f(int, data)
             elif self.regex[key]['type'] == 'date':
                 parse_date = lambda d: d and datetime.strptime('-'.join(d), '%m-%d-%Y').strftime('%Y-%m-%d')
                 data = apply_f(parse_date, data)
+            elif self.regex[key]['type'] == 'json':
+                if isinstance(data, list) and len(data) == 1:
+                    data = data[0]
+                    data = json.loads(data)
             if data:
                 self[key] = data
```

### Comparing `ox-2.3.930/ox/web/spiegel.py` & `ox-3.0.0/ox/web/spiegel.py`

 * *Files identical despite different names*

### Comparing `ox-2.3.930/ox/web/startpage.py` & `ox-3.0.0/ox/web/google.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,69 @@
 # -*- coding: utf-8 -*-
 # vi:si:et:sw=4:sts=4:ts=4
-from six.moves import urllib
+import re
+import urllib
 
-import lxml.html
 import ox
+from ox import strip_tags, decode_html
 
 DEFAULT_MAX_RESULTS = 10
 DEFAULT_TIMEOUT = 24*60*60
 
 def read_url(url, data=None, headers=ox.net.DEFAULT_HEADERS, timeout=DEFAULT_TIMEOUT):
     return ox.cache.read_url(url, data, headers, timeout, unicode=True)
 
 def quote_plus(s):
     if not isinstance(s, bytes):
         s = s.encode('utf-8')
     return urllib.parse.quote_plus(s)
 
+
+def infobox(query, timeout=DEFAULT_TIMEOUT):
+    import lxml.html
+    data = read_url(url, timeout=timeout)
+    doc = lxml.html.document_fromstring(data)
+    k = 'kp-wholepage'
+    wholepage = doc.cssselect('.' + k)
+    infobox = {}
+    if wholepage:
+        page = wholepage[0]
+        for a in page.cssselect('a'):
+            if a.attrib.get('href', '').startswith('http'):
+                domain = '.'.join(a.attrib['href'].split('/')[2].split('.')[-2:])
+                infobox[domain] = a.attrib['href']
+        for e in page.cssselect('*[data-attrid]'):
+            key = e.attrib['data-attrid']
+            value = e.text_content()
+            if value and key not in (
+                'kc:/film/film:media_actions_wholepage',
+                'action:watch_film'
+            ):
+                infobox[key] = value
+    return infobox
+
+
 def find(query, max_results=DEFAULT_MAX_RESULTS, timeout=DEFAULT_TIMEOUT):
     """
     Return max_results tuples with title, url, description 
 
-    >>> find("The Matrix site:imdb.com", 1)[0][0]
+    >>> str(find("The Matrix site:imdb.com", 1)[0][0])
     'The Matrix (1999) - IMDb'
 
-    >>> find("The Matrix site:imdb.com", 1)[0][1]
+    >>> str(find("The Matrix site:imdb.com", 1)[0][1])
     'http://www.imdb.com/title/tt0133093/'
     """
     results = []
-    url = 'https://eu1.startpage.com/do/search?nosteeraway=1&abp=1&language=english&cmd=process_search&query=%s&x=0&y=0&cat=web&engine0=v1all' % quote_plus(query)
-
-    data = read_url(url, timeout=timeout)
-    doc = lxml.html.document_fromstring(data)
-    for r in doc.xpath("//div[contains(@class, 'result')]"):
-        t = r.find('h3')
-        if t is not None:
-            title = t.text_content().strip()
-            url = t.find('a').attrib['href']
-            description = r.find_class('desc')[0].text_content()
-            results.append((title, url, description))
+    offset = 0
+    while len(results) < max_results:
+        url = 'http://google.com/search?q=%s' % quote_plus(query)
+        if offset:
+            url += '&start=%d' % offset
+        data = read_url(url, timeout=timeout)
+        data = re.sub('<span class="f">(.*?)</span>', '\\1', data)
+        for a in re.compile('<a href="(htt\S+?)".*?>(.*?)</a>.*?<span class="st">(.*?)<\/span>').findall(data):
+            results.append((strip_tags(decode_html(a[1])), a[0], strip_tags(decode_html(a[2]))))
             if len(results) >= max_results:
                 break
+        offset += 10
     return results
```

### Comparing `ox-2.3.930/ox/web/thepiratebay.py` & `ox-3.0.0/ox/web/thepiratebay.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # vi:si:et:sw=4:sts=4:ts=4
 from datetime import datetime
 import re
 
-from six.moves.urllib.parse import quote
+from urllib.parse import quote
 
 from ox import find_re, cache, strip_tags, decode_html, get_torrent_info, normalize_newlines
 from ox.normalize import normalize_imdbid
 import ox
 
 cache_timeout = 24*60*60 # cache search only for 24 hours
```

### Comparing `ox-2.3.930/ox/web/tv.py` & `ox-3.0.0/ox/web/tv.py`

 * *Files identical despite different names*

### Comparing `ox-2.3.930/ox/web/twitter.py` & `ox-3.0.0/ox/web/twitter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # vi:si:et:sw=4:sts=4:ts=4
 import re
 from datetime import datetime
-from six.moves.urllib.parse import quote
+from urllib.parse import quote
 
 import lxml.html
 import ox
 from ox.cache import read_url
 
 def find(query=None, user=None, timeout=60):
     if user:
```

### Comparing `ox-2.3.930/ox/web/ubu.py` & `ox-3.0.0/ox/web/ubu.py`

 * *Files identical despite different names*

### Comparing `ox-2.3.930/ox/web/wetransfer.py` & `ox-3.0.0/ox/web/wetransfer.py`

 * *Files identical despite different names*

### Comparing `ox-2.3.930/ox/web/wikipedia.py` & `ox-3.0.0/ox/web/wikipedia.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
 # vi:si:et:sw=4:sts=4:ts=4
 from __future__ import print_function
 
 import re
 
-from six.moves import urllib
-from six import string_types
+import urllib
 
 from ox.utils import json
 from ox.cache import read_url
 from ox import find_re
 
 
 def get_id(url):
@@ -65,15 +64,15 @@
                 key = key.strip()
                 value = d[1].strip()
                 value = value.replace('<!-- see WP:ALT -->', '')
                 if '<br>' in value:
                     value = value.split('<br>')
                 if value:
                     if key in filmbox:
-                        if isinstance(value, list) and isinstance(filmbox[key], string_types):
+                        if isinstance(value, list) and isinstance(filmbox[key], str):
                             filmbox[key] = [filmbox[key]] + value
                         else:
                             filmbox[key] += value
                         if isinstance(filmbox[key], list):
                             filmbox[key] = [k for k in filmbox[key] if k]
                     else:
                         filmbox[key] = value
```

### Comparing `ox-2.3.930/ox/web/youtube.py` & `ox-3.0.0/ox/web/youtube.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # vi:si:et:sw=4:sts=4:ts=4
-from six.moves.urllib.parse import quote, unquote_plus
-from six.moves import urllib
-from six.moves import http_cookiejar as cookielib
+from urllib.parse import quote, unquote_plus
+import urllib
+from http import cookiejar as cookielib
 import re
 from xml.dom.minidom import parseString
 import json
 
 import ox
 from ox.cache import read_url, cache_timeout
```

### Comparing `ox-2.3.930/ox/__init__.py` & `ox-3.0.0/ox/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # vi:si:et:sw=4:sts=4:ts=4
 # GPL 2011
 try:
     from . import __version
     __version__ = __version.VERSION
 except:
-    __version__ = '2.3.930'
+    __version__ = '3.0.x'
 
 from . import cache
 from . import js
 from . import jsonc
 from . import net
 from . import srt
 from . import utils
```

### Comparing `ox-2.3.930/ox/api.py` & `ox-3.0.0/ox/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # -*- coding: utf-8 -*-
 # vi:si:et:sw=4:sts=4:ts=4
 # GPL 2011
 from __future__ import print_function
 from types import MethodType
 import gzip
+import mimetypes
 import os
 import shutil
 import sys
 import time
 
-from six.moves import http_cookiejar as cookielib
-from six import BytesIO, PY2
-from six.moves import urllib
-from six.moves.urllib.parse import urlparse
+from http import cookiejar as cookielib
+from io import BytesIO
+import urllib
+from urllib.parse import urlparse
+import requests
 
 from . import __version__
 from .utils import json
 from .form import MultiPartForm
 
 __all__ = ['getAPI', 'API']
 
@@ -33,78 +35,59 @@
     debuglevel = 0
 
     def __init__(self, url, cj=None):
         if cj:
             self._cj = cj
         else:
             self._cj = cookielib.CookieJar()
-        self._opener = urllib.request.build_opener(urllib.request.HTTPCookieProcessor(self._cj),
-                                            urllib.request.HTTPHandler(debuglevel=self.debuglevel))
-        self._opener.addheaders = [
-            ('User-Agent', '%s/%s' % (self.__name__, self.__version__))
-        ]
 
+        self._requests_session = requests.Session()
+        self._requests_session.cookies = self._cj
+        self._requests_session.headers = {
+            'User-Agent': '%s/%s' % (self.__name__, self.__version__),
+            'Accept-Encoding': 'gzip, deflate',
+        }
         self.url = url
         r = self._request('api', {'docs': True})
         self._properties = r['data']['actions']
         self._actions = r['data']['actions'].keys()
         for a in r['data']['actions']:
             self._add_action(a)
 
     def _add_method(self, method, name):
         if name is None:
             name = method.func_name
-        if PY2:
-            setattr(self, name, MethodType(method, self, type(self)))
-        else:
-            setattr(self, name, MethodType(method, self))
+        setattr(self, name, MethodType(method, self))
 
     def _add_action(self, action):
         def method(self, *args, **kw):
             if args and kw:
                 raise ValueError('pass either a dictionary or kwargs, not both')
             if not kw:
                 if args:
                     kw = args[0]
                 else:
                     kw = None
             return self._request(action, kw)
         if 'doc' in self._properties[action]:
             method.__doc__ = self._properties[action]['doc']
-        if PY2:
-            method.func_name = str(action)
-        else:
-            method.func_name = action
+        method.func_name = action
         self._add_method(method, action)
 
-    def _json_request(self, url, form):
+    def _json_request(self, url, data, files=None):
         result = {}
         try:
-            body = form.body()
-            if PY2:
-                if not isinstance(url, bytes):
-                    url = url.encode('utf-8')
-                request = urllib.request.Request(url)
-                request.add_data(body)
-            else:
-                request = urllib.request.Request(url, data=body, method='POST')
-            request.add_header('Content-Type', form.get_content_type())
-            request.add_header('Content-Length', str(len(body)))
-            request.add_header('Accept-Encoding', 'gzip, deflate')
-            f = self._opener.open(request)
-            result = f.read()
-            if f.headers.get('content-encoding', None) == 'gzip':
-                result = gzip.GzipFile(fileobj=BytesIO(result)).read()
-            result = result.decode('utf-8')
-            return json.loads(result)
+            request = self._requests_session.post(url, data=data, files=files)
+            result = request.json()
+            return result
         except urllib.error.HTTPError as e:
             if self.DEBUG:
                 import webbrowser
                 if e.code >= 500:
-                    with open('/tmp/error.html', 'w') as f:
+                    with open('/tmp/error.html', 'wb') as f:
                         f.write(e.read())
                     webbrowser.open_new_tab('/tmp/error.html')
 
             result = e.read()
             try:
                 result = result.decode('utf-8')
                 result = json.loads(result)
@@ -121,46 +104,39 @@
                 if result:
                     with open('/tmp/error.html', 'w') as f:
                         f.write(str(result))
                     webbrowser.open_new_tab('/tmp/error.html')
             raise
 
     def _request(self, action, data=None):
-        form = MultiPartForm()
-        form.add_field('action', action)
+        form = {
+            'action': action
+        }
         if data:
-            form.add_field('data', json.dumps(data))
+            form['data'] = json.dumps(data)
         return self._json_request(self.url, form)
 
     def get_url(self, url):
-        request = urllib.request.Request(url, method='GET')
-        f = self._opener.open(request)
-        result = f.read()
-        return result
+        return self._requests_session.get(url).content
 
     def save_url(self, url, filename, overwrite=False):
         chunk_size = 16 * 1024
         if not os.path.exists(filename) or overwrite:
             dirname = os.path.dirname(filename)
             if dirname and not os.path.exists(dirname):
                 os.makedirs(dirname)
-            request = urllib.request.Request(url, method='GET')
             tmpname = filename + '.tmp'
             with open(tmpname, 'wb') as fd:
-                u = self._opener.open(request)
-                for chunk in iter(lambda: u.read(chunk_size), b''):
+                r = self._requests_session.get(url)
+                for chunk in iter(lambda: r.read(chunk_size), b''):
                     fd.write(chunk)
             shutil.move(tmpname, filename)
 
-    def upload_chunks(self, url, filename, data=None):
-        form = MultiPartForm()
-        if data:
-            for key in data:
-                form.add_field(key, data[key])
-        data = self._json_request(url, form)
+    def upload_chunks(self, url, filename, data=None, silent=False):
+        data = self._json_request(url, data)
 
         def full_url(path):
             if path.startswith('/'):
                 u = urlparse(url)
                 path = '%s://%s%s' % (u.scheme, u.netloc, path)
             return path
 
@@ -173,45 +149,54 @@
                 done = data['offset']
                 f.seek(done)
                 resume_offset = done
             else:
                 resume_offset = 0
             chunk = f.read(CHUNK_SIZE)
             fname = os.path.basename(filename)
+            mime_type = mimetypes.guess_type(fname)[0] or 'application/octet-stream'
             if not isinstance(fname, bytes):
                 fname = fname.encode('utf-8')
             while chunk:
-                form = MultiPartForm()
-                form.add_file('chunk', fname, chunk)
+                meta = {
+                    'offset': str(done)
+                }
                 if len(chunk) < CHUNK_SIZE or f.tell() == fsize:
-                    form.add_field('done', '1')
-                form.add_field('offset', str(done))
+                    meta['done'] = '1'
+                files = [
+                    ('chunk', (fname, chunk, mime_type))
+                ]
                 try:
-                    data = self._json_request(uploadUrl, form)
+                    data = self._json_request(uploadUrl, meta, files=files)
                 except KeyboardInterrupt:
-                    print("\ninterrupted by user.")
+                    if not slient:
+                        print("\ninterrupted by user.")
                     sys.exit(1)
                 except:
-                    print("uploading chunk failed, will try again in 5 seconds\r", end='')
+                    if not slient:
+                        print("uploading chunk failed, will try again in 5 seconds\r", end='')
                     sys.stdout.flush()
                     data = {'result': -1}
                     time.sleep(5)
                 if data and 'status' in data:
                     if data['status']['code'] == 403:
-                        print("login required")
+                        if not slient:
+                            print("login required")
                         return False
                     if data['status']['code'] != 200:
-                        print("request returned error, will try again in 5 seconds")
+                        if not slient:
+                            print("request returned error, will try again in 5 seconds")
                         if self.DEBUG:
                             print(data)
                         time.sleep(5)
                 if data and data.get('result') == 1:
                     done += len(chunk)
                     if data.get('offset') not in (None, done):
-                        print('server offset out of sync, continue from', data['offset'])
+                        if not slient:
+                            print('server offset out of sync, continue from', data['offset'])
                         done = data['offset']
                         f.seek(done)
                     chunk = f.read(CHUNK_SIZE)
             if data and 'result' in data and data.get('result') == 1:
                 return data.get('id', True)
             else:
                 return False
```

### Comparing `ox-2.3.930/ox/cache.py` & `ox-3.0.0/ox/cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,32 +6,29 @@
 import gzip
 import hashlib
 import os
 import sqlite3
 import time
 import zlib
 
-from six import BytesIO
-from six.moves import urllib
-from six import PY2
-try:
-    import requests
-    USE_REQUESTS = True
-    requests_session = requests.Session()
-except:
-    USE_REQUESTS = False
+from io import BytesIO
+import urllib
+import requests
+from requests.structures import CaseInsensitiveDict
+
 
 from .utils import json
 from .file import makedirs
 
 from . import net
 from .net import DEFAULT_HEADERS, detect_encoding
 
 
 cache_timeout = 30*24*60*60  # default is 30 days
+requests_session = requests.Session()
 
 COMPRESS_TYPES = (
     'text/html',
     'text/plain',
     'text/xml',
     'text/x-wiki',
     'application/json',
@@ -65,15 +62,15 @@
     return False
 
 def get_headers(url, data=None, headers=None, timeout=cache_timeout):
     url_headers = store.get(url, data, headers, timeout, "headers")
     if not url_headers:
         url_headers = net.get_headers(url, data, headers)
         store.set(url, data, -1, url_headers)
-    return url_headers
+    return CaseInsensitiveDict(url_headers)
 
 def get_json(url, data=None, headers=None, timeout=cache_timeout):
     return json.loads(read_url(url, data, headers, timeout).decode('utf-8'))
 
 class InvalidResult(Exception):
     """Base class for exceptions in this module."""
     def __init__(self, result, headers):
@@ -97,40 +94,28 @@
     if net.DEBUG:
         print('ox.cache.read_url', url)
     # FIXME: send last-modified / etag from cache and only update if needed
     # url = _fix_unicode_url(url)
     result = store.get(url, data, headers, timeout)
     url_headers = {}
     if not result:
-        if USE_REQUESTS:
-            if headers is None:
-                headers = DEFAULT_HEADERS.copy()
+        if headers is None:
+            headers = DEFAULT_HEADERS.copy()
+        if data:
+            r = requests_session.post(url, data=data, headers=headers)
+        else:
             r = requests_session.get(url, headers=headers)
-            for key in r.headers:
-                url_headers[key.lower()] = r.headers[key]
-            result = r.content
-            url_headers['Status'] = "%s" % r.status_code
-            if not valid or valid(result, url_headers):
-                store.set(url, post_data=data, data=result, headers=url_headers)
-            else:
-                raise InvalidResult(result, url_headers)
+        for key in r.headers:
+            url_headers[key.lower()] = r.headers[key]
+        result = r.content
+        url_headers['Status'] = "%s" % r.status_code
+        if not valid or valid(result, url_headers):
+            store.set(url, post_data=data, data=result, headers=url_headers)
         else:
-            try:
-                url_headers, result = net.read_url(url, data, headers, return_headers=True)
-            except urllib.error.HTTPError as e:
-                e.headers['Status'] = "%s" % e.code
-                for key in e.headers:
-                    url_headers[key.lower()] = e.headers[key]
-                result = e.read()
-                if url_headers.get('content-encoding', None) == 'gzip':
-                    result = gzip.GzipFile(fileobj=BytesIO(result)).read()
-            if not valid or valid(result, url_headers):
-                store.set(url, post_data=data, data=result, headers=url_headers)
-            else:
-                raise InvalidResult(result, url_headers)
+            raise InvalidResult(result, url_headers)
     if unicode:
         ctype = url_headers.get('content-type', '').lower()
         if 'charset' in ctype:
             encoding = ctype.split('charset=')[-1]
         else:
             encoding = detect_encoding(result)
         if not encoding:
@@ -235,16 +220,14 @@
         for row in c:
             r = row[0]
             if value == 'headers':
                 r = json.loads(r)
             elif value == 'data':
                 if row[1] == 1:
                     r = zlib.decompress(r)
-                elif PY2:
-                    r = str(r)
             break
 
         c.close()
         conn.close()
         return r
 
     def delete(self, url, data=None, headers=None):
@@ -275,14 +258,16 @@
         created = time.mktime(time.localtime())
         content_type = headers.get('content-type', '').split(';')[0].strip()
         if content_type in COMPRESS_TYPES:
             compressed = 1
             data = zlib.compress(data)
         else:
             compressed = 0
+        if isinstance(data, str):
+            data = data.encode("utf-8")
         data = sqlite3.Binary(data)
 
         #fixme: this looks wrong
         try:
             _headers = json.dumps(headers)
         except:
             for h in headers:
```

### Comparing `ox-2.3.930/ox/file.py` & `ox-3.0.0/ox/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,31 @@
 from .utils import json
 
 __all__ = ['sha1sum', 'oshash', 'avinfo', 'makedirs', 'iexists']
 
 EXTENSIONS = {
     'audio': [
         'aac', 'aif', 'aiff', 'amr',
-        'flac', 'm4a', 'mp3', 'oga', 'ogg', 'wav', 'wma', 'opus'
+        'flac', 'm4a', 'mp3', 'oga', 'ogg', 'wav', 'wma', 'opus',
+        'ra',  # Real Audio
     ],
     'image': [
         'bmp', 'gif', 'jpeg', 'jpg', 'png', 'svg', 'webp'
     ],
     'subtitle': [
         'idx', 'srt', 'sub', 'vtt'
     ],
     'video': [
         '3gp',
-        'avi', 'divx', 'dv', 'flv', 'm2t', 'm2ts', 'm4v', 'mkv', 'mov', 'mp4',
-        'mpeg', 'mpg', 'mts', 'ogm', 'ogv', 'rm', 'rmvb', 'vob', 'webm', 'wmv', 'asf',
+        'avi', 'divx', 'dv', 'flv', 'm2t', 'm2ts', 'm2v', 'm4v', 'mkv', 'mov', 'mp4',
+        'mpeg', 'mpg', 'mts', 'ogm', 'ogv', 'vob', 'webm', 'wmv', 'asf',
         'mod', 'tod',  # http://en.wikipedia.org/wiki/MOD_and_TOD
-        'mxf', 'ts'
+        'mxf', 'ts',
+        'dat',  # VOD files
+        'rm', 'rmvb',  # Real Media
     ],
 }
 
 def cmd(program):
     local = os.path.expanduser('~/.ox/bin/%s' % program)
     if os.path.exists(local):
         program = local
@@ -268,17 +271,19 @@
                             'codec_name': 'codec',
                         }.get(key, key)] = s[key]
                 info['subtitles'].append(stream)
             else:
                 pass
                 # print s
         for v in info['video']:
-            if 'rotate' in info.get('metadata', {}) and int(info['metadata']['rotate']) in (-180, -90, 90, 180):
-                v['width'], v['height'] = v['height'], v['width']
             k = 'display_aspect_ratio'
+            if 'rotate' in info.get('metadata', {}) and int(info['metadata']['rotate']) in (-90, 90):
+                v['width'], v['height'] = v['height'], v['width']
+                if k in v:
+                    v[k] = ':'.join(reversed(v[k].split(':')))
             if k not in v and 'width' in v \
                     or (k in v and v[k] == '0:1'):
                 v[k] = '%d:%d' % (v['width'], v['height'])
                 v['pixel_aspect_ratio'] = '1:1'
     info['oshash'] = oshash(filename)
     info['path'] = filename
     if 'size' not in info:
```

### Comparing `ox-2.3.930/ox/fixunicode.py` & `ox-3.0.0/ox/fixunicode.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # -*- coding: utf-8 -*-
 # from http://blog.lumino.so/2012/08/20/fix-unicode-mistakes-with-python/
 # MIT
 from __future__ import print_function
 
 import unicodedata
 
-from six import unichr, text_type
 
 __all__ = ['fix_bad_unicode']
 
 def fix_bad_unicode(text):
     """
     Something you will find all over the place, in real-world text, is text
     that's mistakenly encoded as utf-8, decoded in some ugly format like
@@ -147,15 +146,15 @@
       therefore, someone who is using them will probably get Unicode right)
     - Improbable control characters, such as 0x81
 
     Moderately weird things:
     - Improbable single-byte characters, such as ƒ or ¬
     - Letters in somewhat rare scripts
     '''
-    assert isinstance(text, text_type)
+    assert isinstance(text, str)
     errors = 0
     very_weird_things = 0
     weird_things = 0
     prev_letter_script = None
     for pos in range(len(text)):
         char = text[pos]
         index = ord(char)
@@ -285,15 +284,15 @@
     0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,  # 0xe0
     1, 0, 0, 0, 0, 0, 0, 2, 0, 0, 0, 0, 0, 0, 0, 0,  # 0xf0
 )
 
 # Pre-cache the Unicode data saying which of these first 256 characters are
 # letters. We'll need it often.
 SINGLE_BYTE_LETTERS = [
-    unicodedata.category(unichr(i)).startswith('L')
+    unicodedata.category(chr(i)).startswith('L')
     for i in range(256)
 ]
 
 # A table telling us how to interpret the first word of a letter's Unicode
 # name. The number indicates how frequently we expect this script to be used
 # on computers. Many scripts not included here are assumed to have a frequency
 # of "0" -- if you're going to write in Linear B using Unicode, you're
```

### Comparing `ox-2.3.930/ox/form.py` & `ox-3.0.0/ox/form.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 
 import itertools
 import mimetypes
 import os
 import hashlib
 import sys
 
-from six import PY2
-
 
 __all__ = ['MultiPartForm']
 
 # from /usr/lib/python3.4/email/generator.py
 # Helper used by Generator._make_boundary
 _width = len(repr(sys.maxsize-1))
 _fmt = '%%0%dd' % _width
@@ -59,16 +57,14 @@
         if mimetype is None:
             mimetype = mimetypes.guess_type(filename)[0] or 'application/octet-stream'
         self.files.append((fieldname, filename, mimetype, body))
         return
 
     def __str__(self):
         body = self.body()
-        if not PY2:
-            body = body.decode('utf-8')
         return body
 
     def body(self):
         """Return a byte string representing the form data, including attached files."""
         # Build a list of lists, each containing "lines" of the
         # request.  Each part is separated by a boundary string.
         # Once the list is built, return a string where each
```

### Comparing `ox-2.3.930/ox/format.py` & `ox-3.0.0/ox/format.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # -*- coding: utf-8 -*-
 # vi:si:et:sw=4:sts=4:ts=4
 import math
 import re
 import string
 
-from six import text_type
-
 def toAZ(num):
     """
     Converts an integer to bijective base 26 string using A-Z
 
     >>> for i in range(1, 1000): assert fromAZ(toAZ(i)) == i
 
     >>> toAZ(1)
@@ -104,15 +102,15 @@
 
     >>> to32(347485647)
     'ABCDEF'
 
     >>> to32(555306645)
     'GHJKMN'
 
-    >>> to32(800197332334559L)
+    >>> to32(800197332334559)
     'PQRSTVWXYZ'
 
     >>> to32(32)
     '10'
 
     >>> to32(119292)
     '3MFW'
@@ -222,44 +220,44 @@
         q, r = divmod(q, 36)
         converted.insert(0, letters[r])
     return "".join(converted) or '0'
 
 def from36(q):
     return int(q, 36)
 
-def int_value(strValue, default=u''):
+def int_value(strValue, default=''):
     """
     >>> int_value('abc23')
-    u'23'
+    '23'
 
     >>> int_value(' abc23')
-    u'23'
+    '23'
 
     >>> int_value('ab')
-    u''
+    ''
     """
     try:
-        val = re.compile('(\d+)').findall(text_type(strValue).strip())[0]
+        val = re.compile('(\d+)').findall(str(strValue).strip())[0]
     except:
         val = default
     return val
 
-def float_value(strValue, default=u''):
+def float_value(strValue, default=''):
     """
     >>> float_value('abc23.4')
-    u'23.4'
+    '23.4'
 
     >>> float_value(' abc23.4')
-    u'23.4'
+    '23.4'
 
     >>> float_value('ab')
-    u''
+    ''
     """
     try:
-        val = re.compile('([\d.]+)').findall(text_type(strValue).strip())[0]
+        val = re.compile('([\d.]+)').findall(str(strValue).strip())[0]
     except:
         val = default
     return val
 
 def format_number(number, longName, shortName):
     """
     Return the number in a human-readable format (23 KB, 23.4 MB, 23.42 GB)
```

### Comparing `ox-2.3.930/ox/geo.py` & `ox-3.0.0/ox/geo.py`

 * *Files identical despite different names*

### Comparing `ox-2.3.930/ox/html.py` & `ox-3.0.0/ox/html.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
 # vi:si:et:sw=4:sts=4:ts=4
 # GPL 2008
 import re
 import string
-from six.moves.html_entities import name2codepoint
-from six import unichr, PY2, string_types
+from html.entities import name2codepoint
 
 letters = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz'
 
 # Configuration for add_links() function
 
 LEADING_PUNCTUATION = ['(', '<', '&lt;']
 TRAILING_PUNCTUATION = ['.', ',', ')', '>', '\n', '&gt;', "'", '"']
@@ -22,25 +21,24 @@
                             '|'.join([re.escape(x) for x in LEADING_PUNCTUATION]),
                             '|'.join([re.escape(x) for x in TRAILING_PUNCTUATION])))
 simple_email_re = re.compile(r'^\S+@[a-zA-Z0-9._-]+\.[a-zA-Z0-9._-]+$')
 link_target_attribute_re = re.compile(r'(<a [^>]*?)target=[^\s>]+')
 html_gunk_re = re.compile(r'(?:<br clear="all">|<i><\/i>|<b><\/b>|<em><\/em>|<strong><\/strong>|<\/?smallcaps>|<\/?uppercase>)', re.IGNORECASE)
 hard_coded_bullets_re = re.compile(r'((?:<p>(?:%s).*?[a-zA-Z].*?</p>\s*)+)' % '|'.join([re.escape(x) for x in DOTS]), re.DOTALL)
 trailing_empty_content_re = re.compile(r'(?:<p>(?:&nbsp;|\s|<br \/>)*?</p>\s*)+\Z')
-if PY2:
-    del x  # Temporary variable
+
 
 def escape(html):
     '''
     Returns the given HTML with ampersands, quotes and carets encoded
 
     >>> escape('html "test" & <brothers>')
     'html &quot;test&quot; &amp; &lt;brothers&gt;'
     '''
-    if not isinstance(html, string_types):
+    if not isinstance(html, str):
         html = str(html)
     return html.replace('&', '&amp;').replace('<', '&lt;').replace('>', '&gt;').replace('"', '&quot;').replace("'", '&apos;')
 
 def linebreaks(value):
     '''
     Converts newlines into <p> and <br />
     '''
@@ -143,39 +141,39 @@
 # This pattern matches a character entity reference (a decimal numeric
 # references, a hexadecimal numeric reference, or a named reference).
 charrefpat = re.compile(r'&(#(\d+|x[\da-fA-F]+)|[\w.:-]+);?')
 
 def decode_html(html):
     """
     >>> decode_html('me &amp; you and &#36;&#38;%')
-    u'me & you and $&%'
+    'me & you and $&%'
     >>> decode_html('&#x80;')
-    u'\u20ac'
+    '\u20ac'
     >>> decode_html('Anniversary of Daoud&apos;s Republic')
-    u"Anniversary of Daoud's Republic"
+    "Anniversary of Daoud's Republic"
     """
     if isinstance(html, bytes):
         html = html.decode('utf-8')
-    uchr = unichr
+    uchr = chr
 
     def entitydecode(match, uchr=uchr):
         entity = match.group(1)
         if entity == '#x80':
-            return u'€'
+            return '€'
         elif entity.startswith('#x'):
             return uchr(int(entity[2:], 16))
         elif entity.startswith('#'):
             return uchr(int(entity[1:]))
         elif entity in name2codepoint:
             return uchr(name2codepoint[entity])
         elif entity == 'apos':
             return "'"
         else:
             return match.group(0)
-    return charrefpat.sub(entitydecode, html).replace(u'\xa0', ' ')
+    return charrefpat.sub(entitydecode, html).replace('\xa0', ' ')
 
 def highlight(text, query, hlClass="hl"):
     """
     >>> highlight('me &amp; you and &#36;&#38;%', 'and')
     'me &amp; you <span class="hl">and</span> &#36;&#38;%'
     """
     if query:
@@ -185,59 +183,59 @@
         for i in m:
             text = re.sub("(%s)" % re.escape(i).replace('\ ', '.'), '<span class="%s">\\1</span>' % hlClass, text)
         text = text.replace('|', '<br />')
     return text
 
 def escape_html(value):
     '''
-    >>> escape_html(u'<script> foo')
-    u'&lt;script&gt; foo'
-    >>> escape_html(u'&lt;script&gt; foo')
-    u'&lt;script&gt; foo'
+    >>> escape_html('<script> foo')
+    '&lt;script&gt; foo'
+    >>> escape_html('&lt;script&gt; foo')
+    '&lt;script&gt; foo'
     '''
     return escape(decode_html(value))
 
 def sanitize_html(html, tags=None, global_attributes=[]):
     '''
     >>> sanitize_html('http://foo.com, bar')
-    u'<a href="http://foo.com">http://foo.com</a>, bar'
+    '<a href="http://foo.com">http://foo.com</a>, bar'
     >>> sanitize_html('http://foo.com/foobar?foo, bar')
-    u'<a href="http://foo.com/foobar?foo">http://foo.com/foobar?foo</a>, bar'
+    '<a href="http://foo.com/foobar?foo">http://foo.com/foobar?foo</a>, bar'
     >>> sanitize_html('(see: www.foo.com)')
-    u'(see: <a href="http://www.foo.com">www.foo.com</a>)'
+    '(see: <a href="http://www.foo.com">www.foo.com</a>)'
     >>> sanitize_html('foo@bar.com')
-    u'<a href="mailto:foo@bar.com">foo@bar.com</a>'
+    '<a href="mailto:foo@bar.com">foo@bar.com</a>'
     >>> sanitize_html(sanitize_html('foo@bar.com'))
-    u'<a href="mailto:foo@bar.com">foo@bar.com</a>'
+    '<a href="mailto:foo@bar.com">foo@bar.com</a>'
     >>> sanitize_html('<a href="http://foo.com" onmouseover="alert()">foo</a>')
-    u'<a href="http://foo.com">foo</a>'
+    '<a href="http://foo.com">foo</a>'
     >>> sanitize_html('<a href="javascript:alert()">foo</a>')
-    u'&lt;a href="javascript:alert()"&gt;foo&lt;/a&gt;'
+    '&lt;a href="javascript:alert()"&gt;foo&lt;/a&gt;'
     >>> sanitize_html('[http://foo.com foo]')
-    u'<a href="http://foo.com">foo</a>'
+    '<a href="http://foo.com">foo</a>'
     >>> sanitize_html('<div style="direction: rtl">foo</div>')
-    u'<div style="direction: rtl">foo</div>'
+    '<div style="direction: rtl">foo</div>'
     >>> sanitize_html('<script>alert()</script>')
-    u'&lt;script&gt;alert()&lt;/script&gt;'
+    '&lt;script&gt;alert()&lt;/script&gt;'
     >>> sanitize_html("'foo' < 'bar' && \\"foo\\" > \\"bar\\"")
-    u'\\'foo\\' &lt; \\'bar\\' &amp;&amp; "foo" &gt; "bar"'
+    '\\'foo\\' &lt; \\'bar\\' &amp;&amp; "foo" &gt; "bar"'
     >>> sanitize_html('<b>foo')
-    u'<b>foo</b>'
+    '<b>foo</b>'
     >>> sanitize_html('<b>foo</b></b>')
-    u'<b>foo</b>'
+    '<b>foo</b>'
     >>> sanitize_html('Anniversary of Daoud&apos;s Republic')
-    u"Anniversary of Daoud's Republic"
+    "Anniversary of Daoud's Republic"
     >>> sanitize_html('')
-    u''
+    ''
     >>> sanitize_html(' ')
-    u' '
-    >>> sanitize_html(u'&nbsp;')  # canonicalised to a space: okay, I suppose
-    u' '
-    >>> sanitize_html(u'\u00a0')  # also nbsp
-    u' '
+    ' '
+    >>> sanitize_html('&nbsp;')  # canonicalised to a space: okay, I suppose
+    ' '
+    >>> sanitize_html('\u00a0')  # also nbsp
+    ' '
     '''
     if not tags:
         valid_url = '^((https?:\/\/|\/|mailto:).*?)'
         tags = [
             # inline formatting
             {'name': 'b'},
             {'name': 'bdi'},
@@ -286,16 +284,18 @@
             {'name': 'thead'},
             {'name': 'tr'},
             # other
             {'name': '[]'},
             {
                 'name': 'a',
                 'required': ['href'],
+                'optional': ['target'],
                 'validation': {
-                    'href': valid_url
+                    'href': valid_url,
+                    'target': '^_blank$',
                 }
             },
             {'name': 'br'},
             {
                 'name': 'iframe',
                 'optional': ['width', 'height'],
                 'required': ['src'],
@@ -408,40 +408,45 @@
 
 def sanitize_fragment(html):
     '''
     Ensures that tags are closed (or not, as appropriate), attributes
     are quoted, etc. Does not strip potentially-malicious HTML: use
     sanitize_html() for that.
 
-    >>> sanitize_fragment(u'<span lang="en">')
-    u'<span lang="en"></span>'
-    >>> sanitize_fragment(u'<span lang=en></span>')
-    u'<span lang="en"></span>'
-    >>> sanitize_fragment(u'<br><br/></br>')
-    u'<br><br>'
-    >>> sanitize_fragment(u'<a href="javascript:alert()">foo</a>')
-    u'<a href="javascript:alert()">foo</a>'
-    >>> sanitize_fragment(u'')
-    u''
-    >>> sanitize_fragment(u' ')
-    u' '
-    >>> sanitize_fragment(u'&nbsp;')
-    u'\\xa0'
-    >>> sanitize_fragment(u'\\u00a0')  # nbsp
-    u'\\xa0'
-    >>> sanitize_fragment(u'\\ufeff')  # zero-width no-break space
-    u'\\ufeff'
+    >>> sanitize_fragment('<span lang="en">')
+    '<span lang="en"></span>'
+    >>> sanitize_fragment('<span lang=en></span>')
+    '<span lang="en"></span>'
+    >>> sanitize_fragment('<br><br/></br>')
+    '<br><br>'
+    >>> sanitize_fragment('<a href="javascript:alert()">foo</a>')
+    '<a href="javascript:alert()">foo</a>'
+    >>> sanitize_fragment('')
+    ''
+    >>> sanitize_fragment(' ')
+    ' '
+    >>> sanitize_fragment('&nbsp;')
+    '\\xa0'
+    >>> sanitize_fragment('\\u00a0')  # nbsp
+    '\\xa0'
+    >>> sanitize_fragment('\\ufeff')  # zero-width no-break space
+    '\\ufeff'
     '''
 
     '''
     #html5lib reorders arguments, so not usable
     import html5lib
     return html5lib.parseFragment(html).toxml().decode('utf-8')
     '''
     if not html.strip():
         return html
     import lxml.html
-    body = lxml.html.document_fromstring(html).find('body')
+    try:
+        body = lxml.html.document_fromstring(html).find('body')
+    except lxml.etree.ParserError as e:
+        if e.args and e.args[0] == 'Document is empty':
+            return html
+        raise e
     html = lxml.html.tostring(body, encoding='utf-8')[6:-7].decode('utf-8')
     if html.startswith('<p>') and html.endswith('</p>'):
         html = html[3:-4]
     return html
```

### Comparing `ox-2.3.930/ox/image.py` & `ox-3.0.0/ox/image.py`

 * *Files identical despite different names*

### Comparing `ox-2.3.930/ox/iso.py` & `ox-3.0.0/ox/iso.py`

 * *Files identical despite different names*

### Comparing `ox-2.3.930/ox/js.py` & `ox-3.0.0/ox/js.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,17 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 # vi:si:et:sw=4:sts=4:ts=4
 
-from six import PY2
 from .utils import json
 
 def minify(source, comment=''):
     # see https://github.com/douglascrockford/JSMin/blob/master/README
     def get_next_non_whitespace_token():
         pass
-    # python2 performance with unicode string is terrible
-    if PY2:
-        if isinstance(source, unicode):  # pylint: disable=undefined-variable
-            source = source.encode('utf-8')
-        if isinstance(comment, unicode):  # pylint: disable=undefined-variable
-            comment = comment.encode('utf-8')
     tokens = tokenize(source)
     length = len(tokens)
     minified = '/*' + comment + '*/' if comment else ''
     for i, token in enumerate(tokens):
         if token['type'] in ['linebreak', 'whitespace']:
             prevToken = None if i == 0 else tokens[i - 1]
             next = i + 1
```

### Comparing `ox-2.3.930/ox/jsonc.py` & `ox-3.0.0/ox/jsonc.py`

 * *Files identical despite different names*

### Comparing `ox-2.3.930/ox/location.py` & `ox-3.0.0/ox/location.py`

 * *Files identical despite different names*

### Comparing `ox-2.3.930/ox/movie.py` & `ox-3.0.0/ox/movie.py`

 * *Files identical despite different names*

### Comparing `ox-2.3.930/ox/net.py` & `ox-3.0.0/ox/net.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,18 @@
 from __future__ import print_function
 import gzip
 import json
 import os
 import re
 import struct
 
-try:
-    import requests
-    USE_REQUESTS = True
-except:
-    USE_REQUESTS = False
-from six import BytesIO, PY2
-from six.moves import urllib
+import requests
+
+from io import BytesIO
+import urllib
 from chardet.universaldetector import UniversalDetector
 
 
 DEBUG = False
 # Default headers for HTTP requests.
 DEFAULT_HEADERS = {
     'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64; rv:78.0) Gecko/20100101 Firefox/78.0',
@@ -55,22 +52,18 @@
 
 def get_json(url, data=None, headers=None):
     return json.loads(read_url(url, data, headers).decode('utf-8'))  # pylint: disable=no-member
 
 def open_url(url, data=None, headers=None):
     if headers is None:
         headers = DEFAULT_HEADERS.copy()
-    if PY2:
-        if not isinstance(url, bytes):
-            url = url.encode('utf-8')
-    else:
-        if isinstance(url, bytes):
-            url = url.decode('utf-8')
+    if isinstance(url, bytes):
+        url = url.decode('utf-8')
     url = url.replace(' ', '%20')
-    if data and not PY2 and not isinstance(data, bytes):
+    if data and not isinstance(data, bytes):
         data = data.encode('utf-8')
     req = urllib.request.Request(url, data, headers)
     return urllib.request.urlopen(req)
 
 def read_url(url, data=None, headers=None, return_headers=False, unicode=False):
     if DEBUG:
         print('ox.net.read_url', url)
@@ -119,24 +112,19 @@
 
 def save_url(url, filename, overwrite=False):
     if not os.path.exists(filename) or overwrite:
         dirname = os.path.dirname(filename)
         if dirname and not os.path.exists(dirname):
             os.makedirs(dirname)
         headers = DEFAULT_HEADERS.copy()
-        if USE_REQUESTS:
-            r = requests.get(url, headers=headers, stream=True)
-            with open(filename, 'wb') as f:
-                for chunk in r.iter_content(chunk_size=1024):
-                    if chunk:  # filter out keep-alive new chunks
-                        f.write(chunk)
-        else:
-            data = read_url(url)
-            with open(filename, 'wb') as f:
-                f.write(data)
+        r = requests.get(url, headers=headers, stream=True)
+        with open(filename, 'wb') as f:
+            for chunk in r.iter_content(chunk_size=1024):
+                if chunk:  # filter out keep-alive new chunks
+                    f.write(chunk)
 
 def _get_size(url):
     req = urllib.request.Request(url, headers=DEFAULT_HEADERS.copy())
     req.get_method = lambda: 'HEAD'
     u = urllib.request.urlopen(req)
     if u.code != 200 or 'Content-Length' not in u.headers:
         raise IOError
```

### Comparing `ox-2.3.930/ox/normalize.py` & `ox-3.0.0/ox/normalize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # -*- coding: utf-8 -*-
 # vi:si:et:sw=4:sts=4:ts=4
 # GPL 2008
 import re
 import unicodedata
 
-from six import string_types
-
 
 _articles = ('the', 'la', 'a', 'die', 'der', 'le', 'el',
              "l'", 'il', 'das', 'les', 'o', 'ein', 'i', 'un', 'los', 'de',
              'an', 'una', 'las', 'eine', 'den', 'gli', 'het', 'os', 'lo',
              'az', 'det', 'ha-', 'een', 'ang', 'oi', 'ta', 'al-', 'dem',
              'mga', 'uno', "un'", 'ett', u'\xcf', 'eines', u'\xc7', 'els',
              u'\xd4\xef', u'\xcf\xe9')
@@ -99,15 +97,15 @@
     >>> normalize_imdbid('http://www.imdb.com/title/tt0159206/')
     '0159206'
     >>> normalize_imdbid(159206)
     '0159206'
     >>> normalize_imdbid('tt0159206')
     '0159206'
     """
-    if isinstance(imdbId, string_types):
+    if isinstance(imdbId, str):
         imdbId = re.sub('.*(\d{7}).*', '\\1', imdbId)
     elif isinstance(imdbId, int):
         imdbId = "%07d" % imdbId
     return imdbId
 
 
 # Common suffixes in surnames.
```

### Comparing `ox-2.3.930/ox/oembed.py` & `ox-3.0.0/ox/oembed.py`

 * *Files identical despite different names*

### Comparing `ox-2.3.930/ox/srt.py` & `ox-3.0.0/ox/srt.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
 # vi:si:et:sw=4:sts=4:ts=4
 from __future__ import division, print_function
 import codecs
 import re
 
 import chardet
-from six import PY2
 import ox
 
 
 __all__ = []
 
 
 def _detect_encoding(fp):
@@ -20,18 +19,15 @@
         (0xFF, 0xFE, None, None): "utf_16_le",
         (0xEF, 0xBB, 0xBF, None): "utf_8",
     }
 
     # go to beginning of file and get the first 4 bytes
     oldFP = fp.tell()
     fp.seek(0)
-    if PY2:
-        (byte1, byte2, byte3, byte4) = [ord(b) for b in fp.read(4)]
-    else:
-        (byte1, byte2, byte3, byte4) = fp.read(4)
+    (byte1, byte2, byte3, byte4) = fp.read(4)
 
     # try bom detection using 4 bytes, 3 bytes, or 2 bytes
     bomDetection = bomDict.get((byte1, byte2, byte3, byte4))
     if not bomDetection:
         bomDetection = bomDict.get((byte1, byte2, byte3, None))
         if not bomDetection:
             bomDetection = bomDict.get((byte1, byte2, None, None))
```

### Comparing `ox-2.3.930/ox/text.py` & `ox-3.0.0/ox/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,1510 +1,1507 @@
 00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
 00000010: 662d 3820 2d2a 2d0a 2320 7669 3a73 693a  f-8 -*-.# vi:si:
 00000020: 6574 3a73 773d 343a 7374 733d 343a 7473  et:sw=4:sts=4:ts
 00000030: 3d34 0a23 2047 504c 2032 3030 380a 696d  =4.# GPL 2008.im
-00000040: 706f 7274 206d 6174 680a 696d 706f 7274  port math.import
-00000050: 2072 650a 696d 706f 7274 2075 6e69 636f   re.import unico
-00000060: 6465 6461 7461 0a0a 6672 6f6d 2073 6978  dedata..from six
-00000070: 2e6d 6f76 6573 2069 6d70 6f72 7420 7265  .moves import re
-00000080: 6475 6365 0a0a 4152 5449 434c 4553 203d  duce..ARTICLES =
-00000090: 206c 6973 7428 7365 7428 5b0a 2020 2020   list(set([.    
-000000a0: 2320 6465 6620 7367 2c20 6465 6620 706c  # def sg, def pl
-000000b0: 2c20 696e 6465 6620 7367 2c20 696e 6465  , indef sg, inde
-000000c0: 6620 706c 2028 6561 6368 206d 2f66 2f6e  f pl (each m/f/n
-000000d0: 290a 2020 2020 2764 6572 272c 2027 6469  ).    'der', 'di
-000000e0: 6527 2c20 2764 6173 272c 2027 6569 6e27  e', 'das', 'ein'
-000000f0: 2c20 2765 696e 6527 2c20 2023 2064 650a  , 'eine',  # de.
-00000100: 2020 2020 2774 6865 272c 2027 6127 2c20      'the', 'a', 
-00000110: 2761 6e27 2c20 2023 2065 6e0a 2020 2020  'an',  # en.    
-00000120: 2765 6c27 2c20 276c 6127 2c20 276c 6f27  'el', 'la', 'lo'
-00000130: 2c20 276c 6f73 272c 2027 6c61 7327 2c20  , 'los', 'las', 
-00000140: 2775 6e27 2c20 2775 6e61 272c 2027 756e  'un', 'una', 'un
-00000150: 6f73 272c 2027 756e 6173 272c 2020 2320  os', 'unas',  # 
-00000160: 6573 0a20 2020 2027 6c65 272c 2022 6c27  es.    'le', "l'
-00000170: 222c 2027 6c61 272c 2027 6c65 7327 2c20  ", 'la', 'les', 
-00000180: 2775 6e27 2c20 2775 6e65 272c 2027 6465  'un', 'une', 'de
-00000190: 7327 2c20 2023 2066 720a 2020 2020 2769  s',  # fr.    'i
-000001a0: 6c27 2c20 276c 6f27 2c20 226c 2722 2027  l', 'lo', "l'" '
-000001b0: 6c61 272c 2027 5f69 272c 2027 676c 6927  la', '_i', 'gli'
-000001c0: 2c20 276c 6527 2c20 2023 2069 740a 2020  , 'le',  # it.  
-000001d0: 2020 2764 6527 2c20 2768 6574 272c 2027    'de', 'het', '
-000001e0: 6565 6e27 2c20 2023 206e 6c0a 2020 2020  een',  # nl.    
-000001f0: 276f 272c 2027 6127 2c20 276f 7327 2c20  'o', 'a', 'os', 
-00000200: 275f 6173 272c 2027 756d 272c 2027 756d  '_as', 'um', 'um
-00000210: 6127 2c20 275f 756e 7327 2c20 2775 6d61  a', '_uns', 'uma
-00000220: 7327 2020 2320 7074 0a20 2020 2023 2073  s'  # pt.    # s
-00000230: 6f6d 6520 5f64 6973 6162 6c65 6420 6265  ome _disabled be
-00000240: 6361 7573 6520 6f66 2063 6f6c 6c69 7369  cause of collisi
-00000250: 6f6e 730a 5d29 290a 2320 6576 6572 7920  ons.])).# every 
-00000260: 6769 7665 6e20 6e61 6d65 2069 6e20 3078  given name in 0x
-00000270: 4442 2074 6861 7420 6d61 7463 6865 7320  DB that matches 
-00000280: 5878 7878 2d79 7979 7920 4c61 7374 6e61  Xxxx-yyyy Lastna
-00000290: 6d65 0a41 5349 414e 5f46 4952 5354 5f4e  me.ASIAN_FIRST_N
-000002a0: 414d 4553 203d 205b 0a20 2020 2027 6127  AMES = [.    'a'
-000002b0: 2c20 2761 6527 2c20 2761 656e 6727 2c20  , 'ae', 'aeng', 
-000002c0: 2761 6827 2c20 2761 6927 2c20 2761 6e27  'ah', 'ai', 'an'
-000002d0: 2c20 2762 6163 6b27 2c20 2762 6165 272c  , 'back', 'bae',
-000002e0: 2027 6261 6e27 2c20 2762 616e 6727 2c20   'ban', 'bang', 
-000002f0: 2762 616f 272c 200a 2020 2020 2762 656f  'bao', .    'beo
-00000300: 6d27 2c20 2762 6927 2c20 2762 696e 272c  m', 'bi', 'bin',
-00000310: 2027 626f 272c 2027 626f 6b27 2c20 2762   'bo', 'bok', 'b
-00000320: 6f6e 272c 2027 626f 6e67 272c 2027 6275  on', 'bong', 'bu
-00000330: 272c 2027 6275 6d27 2c20 2762 7965 6f6e  ', 'bum', 'byeon
-00000340: 6727 2c20 0a20 2020 2027 6279 6f75 6e67  g', .    'byoung
-00000350: 272c 2027 6279 756e 6727 2c20 2763 6169  ', 'byung', 'cai
-00000360: 272c 2027 6368 6165 272c 2027 6368 616e  ', 'chae', 'chan
-00000370: 272c 2027 6368 616e 6727 2c20 2763 6861  ', 'chang', 'cha
-00000380: 6f27 2c20 2763 6865 616c 272c 2027 6368  o', 'cheal', 'ch
-00000390: 656e 272c 200a 2020 2020 2763 6865 6e67  en', .    'cheng
-000003a0: 272c 2027 6368 656f 6c27 2c20 2763 6865  ', 'cheol', 'che
-000003b0: 6f6e 272c 2027 6368 656f 6e67 272c 2027  on', 'cheong', '
-000003c0: 6368 6575 6c27 2c20 2763 6869 272c 2027  cheul', 'chi', '
-000003d0: 6368 6961 272c 2027 6368 6961 6f27 2c20  chia', 'chiao', 
-000003e0: 0a20 2020 2027 6368 6965 6827 2c20 2763  .    'chieh', 'c
-000003f0: 6869 656e 272c 2027 6368 6968 272c 2027  hien', 'chih', '
-00000400: 6368 696e 272c 2027 6368 696e 6727 2c20  chin', 'ching', 
-00000410: 2763 686f 272c 2027 6368 6f69 272c 2027  'cho', 'choi', '
-00000420: 6368 6f6e 6727 2c20 2763 686f 6f27 2c20  chong', 'choo', 
-00000430: 0a20 2020 2027 6368 7527 2c20 2763 6875  .    'chu', 'chu
-00000440: 616e 272c 2027 6368 7565 6e27 2c20 2763  an', 'chuen', 'c
-00000450: 6875 6c27 2c20 2763 6875 6e27 2c20 2763  hul', 'chun', 'c
-00000460: 6875 6e67 272c 2027 6368 756f 272c 2027  hung', 'chuo', '
-00000470: 6368 7969 272c 2027 6461 272c 200a 2020  chyi', 'da', .  
-00000480: 2020 2764 6165 272c 2027 6461 6827 2c20    'dae', 'dah', 
-00000490: 2764 616c 272c 2027 6461 6e27 2c20 2764  'dal', 'dan', 'd
-000004a0: 656f 6b27 2c20 2764 6f27 2c20 2764 6f6e  eok', 'do', 'don
-000004b0: 6727 2c20 2764 6f6f 272c 2027 6475 656b  g', 'doo', 'duek
-000004c0: 272c 2027 6475 6b27 2c20 0a20 2020 2027  ', 'duk', .    '
-000004d0: 6527 2c20 2765 6c27 2c20 2765 6e27 2c20  e', 'el', 'en', 
-000004e0: 2765 7569 272c 2027 6575 6c27 2c20 2765  'eui', 'eul', 'e
-000004f0: 756e 272c 2027 6575 6e67 272c 2027 6661  un', 'eung', 'fa
-00000500: 6927 2c20 2766 616e 272c 2027 6661 6e67  i', 'fan', 'fang
-00000510: 272c 2027 6665 6927 2c20 0a20 2020 2027  ', 'fei', .    '
-00000520: 6665 6e27 2c20 2766 656e 6727 2c20 2766  fen', 'feng', 'f
-00000530: 6f27 2c20 2766 6f6f 272c 2027 6675 272c  o', 'foo', 'fu',
-00000540: 2027 6761 272c 2027 6761 6527 2c20 2767   'ga', 'gae', 'g
-00000550: 616d 272c 2027 6761 6e67 272c 2027 6765  am', 'gang', 'ge
-00000560: 272c 2027 6765 6e27 2c20 0a20 2020 2027  ', 'gen', .    '
-00000570: 6765 6f6e 272c 2027 6765 756e 272c 2027  geon', 'geun', '
-00000580: 6769 272c 2027 6769 6c27 2c20 2767 696e  gi', 'gil', 'gin
-00000590: 272c 2027 676e 6164 272c 2027 676f 6b27  ', 'gnad', 'gok'
-000005a0: 2c20 2767 6f6f 272c 2027 676f 6f6b 272c  , 'goo', 'gook',
-000005b0: 2027 6775 272c 200a 2020 2020 2767 756e   'gu', .    'gun
-000005c0: 272c 2027 6777 616e 272c 2027 6779 6527  ', 'gwan', 'gye'
-000005d0: 2c20 2767 7965 6f6e 6727 2c20 2767 7975  , 'gyeong', 'gyu
-000005e0: 272c 2027 6779 756e 272c 2027 6861 272c  ', 'gyun', 'ha',
-000005f0: 2027 6861 6527 2c20 2768 616b 272c 2027   'hae', 'hak', '
-00000600: 6861 6e27 2c20 0a20 2020 2027 6861 6e67  han', .    'hang
-00000610: 272c 2027 6861 6f27 2c20 2768 6527 2c20  ', 'hao', 'he', 
-00000620: 2768 6565 272c 2027 6865 6e67 272c 2027  'hee', 'heng', '
-00000630: 6865 6f6e 272c 2027 6869 6527 2c20 2768  heon', 'hie', 'h
-00000640: 6f27 2c20 2768 6f69 272c 2027 686f 6e67  o', 'hoi', 'hong
-00000650: 272c 200a 2020 2020 2768 6f6f 272c 2027  ', .    'hoo', '
-00000660: 686f 6f6e 272c 2027 686f 7527 2c20 2768  hoon', 'hou', 'h
-00000670: 7369 272c 2027 6873 6961 6e67 272c 2027  si', 'hsiang', '
-00000680: 6873 6961 6f27 2c20 2768 7369 6568 272c  hsiao', 'hsieh',
-00000690: 2027 6873 6965 6e27 2c20 2768 7369 6e27   'hsien', 'hsin'
-000006a0: 2c20 0a20 2020 2027 6873 696e 6727 2c20  , .    'hsing', 
-000006b0: 2768 7369 756e 6727 2c20 2768 7527 2c20  'hsiung', 'hu', 
-000006c0: 2768 7561 272c 2027 6875 6169 272c 2027  'hua', 'huai', '
-000006d0: 6875 616e 6727 2c20 2768 7565 272c 2027  huang', 'hue', '
-000006e0: 6875 6927 2c20 2768 756e 272c 200a 2020  hui', 'hun', .  
-000006f0: 2020 2768 756e 6727 2c20 2768 7761 272c    'hung', 'hwa',
-00000700: 2027 6877 616e 272c 2027 6877 616e 6727   'hwan', 'hwang'
-00000710: 2c20 2768 7965 272c 2027 6879 656f 6b27  , 'hye', 'hyeok'
-00000720: 2c20 2768 7965 6f6e 272c 2027 6879 656f  , 'hyeon', 'hyeo
-00000730: 6e67 272c 2027 6879 6f27 2c20 0a20 2020  ng', 'hyo', .   
-00000740: 2027 6879 756b 272c 2027 6879 756e 272c   'hyuk', 'hyun',
-00000750: 2027 6879 756e 6727 2c20 2769 272c 2027   'hyung', 'i', '
-00000760: 696b 272c 2027 696c 272c 2027 696e 272c  ik', 'il', 'in',
-00000770: 2027 6a61 272c 2027 6a61 6527 2c20 276a   'ja', 'jae', 'j
-00000780: 616e 272c 2027 6a61 6e67 272c 200a 2020  an', 'jang', .  
-00000790: 2020 276a 6527 2c20 276a 6565 272c 2027    'je', 'jee', '
-000007a0: 6a65 6e27 2c20 276a 656f 6b27 2c20 276a  jen', 'jeok', 'j
-000007b0: 656f 6e67 272c 2027 6a65 756e 6727 2c20  eong', 'jeung', 
-000007c0: 276a 6927 2c20 276a 6961 272c 2027 6a69  'ji', 'jia', 'ji
-000007d0: 616e 272c 2027 6a69 6b27 2c20 0a20 2020  an', 'jik', .   
-000007e0: 2027 6a69 6e27 2c20 276a 696e 6727 2c20   'jin', 'jing', 
-000007f0: 276a 6f27 2c20 276a 6f6e 6727 2c20 276a  'jo', 'jong', 'j
-00000800: 6f6f 272c 2027 6a6f 6f6e 272c 2027 6a75  oo', 'joon', 'ju
-00000810: 272c 2027 6a75 616e 272c 2027 6a75 6e27  ', 'juan', 'jun'
-00000820: 2c20 276a 756e 6727 2c20 0a20 2020 2027  , 'jung', .    '
-00000830: 6b61 272c 2027 6b61 6927 2c20 276b 616d  ka', 'kai', 'kam
-00000840: 272c 2027 6b61 6e27 2c20 276b 616e 6727  ', 'kan', 'kang'
-00000850: 2c20 276b 6170 272c 2027 6b61 7227 2c20  , 'kap', 'kar', 
-00000860: 276b 6527 2c20 276b 6565 272c 2027 6b65  'ke', 'kee', 'ke
-00000870: 6927 2c20 0a20 2020 2027 6b65 6e67 272c  i', .    'keng',
-00000880: 2027 6b65 756d 272c 2027 6b65 756e 6727   'keum', 'keung'
-00000890: 2c20 276b 6927 2c20 276b 696c 272c 2027  , 'ki', 'kil', '
-000008a0: 6b69 6e27 2c20 276b 6974 272c 2027 6b6f  kin', 'kit', 'ko
-000008b0: 7427 2c20 276b 7527 2c20 276b 7561 272c  t', 'ku', 'kua',
-000008c0: 200a 2020 2020 276b 7561 6e27 2c20 276b   .    'kuan', 'k
-000008d0: 7561 6e67 272c 2027 6b75 656e 272c 2027  uang', 'kuen', '
-000008e0: 6b75 6e27 2c20 276b 756f 272c 2027 6b77  kun', 'kuo', 'kw
-000008f0: 616e 6727 2c20 276b 776f 6b27 2c20 276b  ang', 'kwok', 'k
-00000900: 776f 6e27 2c20 276b 776f 6e67 272c 200a  won', 'kwong', .
-00000910: 2020 2020 276b 7965 6f6e 6727 2c20 276b      'kyeong', 'k
-00000920: 796f 272c 2027 6b79 6f6f 6e27 2c20 276b  yo', 'kyoon', 'k
-00000930: 796f 7527 2c20 276b 796f 756e 6727 2c20  you', 'kyoung', 
-00000940: 276b 7975 272c 2027 6b79 756e 272c 2027  'kyu', 'kyun', '
-00000950: 6b79 756e 6727 2c20 276c 6169 272c 200a  kyung', 'lai', .
-00000960: 2020 2020 276c 6175 272c 2027 6c65 6527      'lau', 'lee'
-00000970: 2c20 276c 6569 272c 2027 6c65 6e67 272c  , 'lei', 'leng',
-00000980: 2027 6c65 756e 6727 2c20 276c 6927 2c20   'leung', 'li', 
-00000990: 276c 6961 6e67 272c 2027 6c69 656e 272c  'liang', 'lien',
-000009a0: 2027 6c69 6e27 2c20 276c 696e 6727 2c20   'lin', 'ling', 
-000009b0: 0a20 2020 2027 6c6f 636b 272c 2027 6c6f  .    'lock', 'lo
-000009c0: 6e67 272c 2027 6c75 6e27 2c20 276c 756e  ng', 'lun', 'lun
-000009d0: 6727 2c20 276d 6165 6e67 272c 2027 6d61  g', 'maeng', 'ma
-000009e0: 6e27 2c20 276d 6569 272c 2027 6d69 272c  n', 'mei', 'mi',
-000009f0: 2027 6d69 616f 272c 2027 6d69 6e27 2c20   'miao', 'min', 
-00000a00: 0a20 2020 2027 6d69 6e67 272c 2027 6d6f  .    'ming', 'mo
-00000a10: 272c 2027 6d6f 6b27 2c20 276d 6f6f 272c  ', 'mok', 'moo',
-00000a20: 2027 6d6f 6f6b 272c 2027 6d6f 6f6e 272c   'mook', 'moon',
-00000a30: 2027 6d75 272c 2027 6d75 6e27 2c20 276d   'mu', 'mun', 'm
-00000a40: 7965 6f6e 6727 2c20 0a20 2020 2027 6d79  yeong', .    'my
-00000a50: 6f65 6e67 272c 2027 6d79 6f6e 6727 2c20  oeng', 'myong', 
-00000a60: 276d 7975 6e67 272c 2027 6e61 272c 2027  'myung', 'na', '
-00000a70: 6e61 6527 2c20 276e 6169 272c 2027 6e61  nae', 'nai', 'na
-00000a80: 6d27 2c20 276e 616e 272c 2027 6e65 756e  m', 'nan', 'neun
-00000a90: 6727 2c20 0a20 2020 2027 6e67 6172 7527  g', .    'ngaru'
-00000aa0: 2c20 276e 6927 2c20 276e 6f27 2c20 276e  , 'ni', 'no', 'n
-00000ab0: 7965 6f27 2c20 276f 6827 2c20 276f 6b27  yeo', 'oh', 'ok'
-00000ac0: 2c20 276f 7527 2c20 2770 6169 272c 2027  , 'ou', 'pai', '
-00000ad0: 7065 6927 2c20 2770 656e 272c 2027 7065  pei', 'pen', 'pe
-00000ae0: 6e67 272c 200a 2020 2020 2770 6927 2c20  ng', .    'pi', 
-00000af0: 2770 696c 272c 2027 7069 6e27 2c20 2770  'pil', 'pin', 'p
-00000b00: 696e 6727 2c20 2770 6f27 2c20 2770 7569  ing', 'po', 'pui
-00000b10: 272c 2027 7079 6f27 2c20 2770 7975 6e67  ', 'pyo', 'pyung
-00000b20: 272c 2027 7169 6e67 272c 2027 7175 6e27  ', 'qing', 'qun'
-00000b30: 2c20 0a20 2020 2027 7261 272c 2027 7261  , .    'ra', 'ra
-00000b40: 6b27 2c20 2772 616d 272c 2027 7261 6e27  k', 'ram', 'ran'
-00000b50: 2c20 2772 6575 6d27 2c20 2772 6927 2c20  , 'reum', 'ri', 
-00000b60: 2772 696d 272c 2027 7269 6e27 2c20 2772  'rim', 'rin', 'r
-00000b70: 6f65 272c 2027 726f 6b27 2c20 2772 7527  oe', 'rok', 'ru'
-00000b80: 2c20 0a20 2020 2027 7275 6927 2c20 2772  , .    'rui', 'r
-00000b90: 7965 6f6e 272c 2027 7279 6f6c 272c 2027  yeon', 'ryol', '
-00000ba0: 7279 6f6e 6727 2c20 2773 6127 2c20 2773  ryong', 'sa', 's
-00000bb0: 6165 272c 2027 7361 6e27 2c20 2773 616e  ae', 'san', 'san
-00000bc0: 6727 2c20 2773 6527 2c20 2773 656f 272c  g', 'se', 'seo',
-00000bd0: 200a 2020 2020 2773 656f 6227 2c20 2773   .    'seob', 's
-00000be0: 656f 6b27 2c20 2773 656f 6c27 2c20 2773  eok', 'seol', 's
-00000bf0: 656f 6e27 2c20 2773 656f 6e67 272c 2027  eon', 'seong', '
-00000c00: 7365 756e 6727 2c20 2773 6861 6e27 2c20  seung', 'shan', 
-00000c10: 2773 6865 6e27 2c20 2773 6865 6e67 272c  'shen', 'sheng',
-00000c20: 200a 2020 2020 2773 6869 272c 2027 7368   .    'shi', 'sh
-00000c30: 6961 272c 2027 7368 6961 6e67 272c 2027  ia', 'shiang', '
-00000c40: 7368 6968 272c 2027 7368 696b 272c 2027  shih', 'shik', '
-00000c50: 7368 696d 272c 2027 7368 696e 272c 2027  shim', 'shin', '
-00000c60: 7368 696e 6727 2c20 2773 686f 7527 2c20  shing', 'shou', 
-00000c70: 0a20 2020 2027 7368 7527 2c20 2773 6875  .    'shu', 'shu
-00000c80: 6e27 2c20 2773 6927 2c20 2773 696b 272c  n', 'si', 'sik',
-00000c90: 2027 7369 6e27 2c20 2773 6975 272c 2027   'sin', 'siu', '
-00000ca0: 736f 272c 2027 736f 6e67 272c 2027 736f  so', 'song', 'so
-00000cb0: 6f27 2c20 2773 6f6f 6b27 2c20 0a20 2020  o', 'sook', .   
-00000cc0: 2027 736f 6f6e 272c 2027 7375 272c 2027   'soon', 'su', '
-00000cd0: 7375 6b27 2c20 2773 756e 272c 2027 7375  suk', 'sun', 'su
-00000ce0: 6e67 272c 2027 7375 7027 2c20 2773 7a75  ng', 'sup', 'szu
-00000cf0: 272c 2022 7427 6965 6e22 2c20 2774 6127  ', "t'ien", 'ta'
-00000d00: 2c20 2774 6165 272c 200a 2020 2020 2774  , 'tae', .    't
-00000d10: 6165 6b27 2c20 2774 6169 272c 2027 7461  aek', 'tai', 'ta
-00000d20: 6b27 2c20 2774 6527 2c20 2774 6927 2c20  k', 'te', 'ti', 
-00000d30: 2774 6961 6e27 2c20 2774 696e 6727 2c20  'tian', 'ting', 
-00000d40: 2774 6f27 2c20 2774 6f61 272c 2027 7473  'to', 'toa', 'ts
-00000d50: 6169 272c 200a 2020 2020 2774 7361 6e27  ai', .    'tsan'
-00000d60: 2c20 2774 7365 272c 2027 7473 6f27 2c20  , 'tse', 'tso', 
-00000d70: 2774 7375 6927 2c20 2774 756e 6727 2c20  'tsui', 'tung', 
-00000d80: 2774 7a75 272c 2027 7561 272c 2027 7569  'tzu', 'ua', 'ui
-00000d90: 272c 2027 756e 272c 2027 7761 6827 2c20  ', 'un', 'wah', 
-00000da0: 0a20 2020 2027 7761 6927 2c20 2777 616e  .    'wai', 'wan
-00000db0: 272c 2027 7765 6927 2c20 2777 656e 272c  ', 'wei', 'wen',
-00000dc0: 2027 7765 6f6e 272c 2027 7769 6e67 272c   'weon', 'wing',
-00000dd0: 2027 7769 7427 2c20 2777 6f6c 272c 2027   'wit', 'wol', '
-00000de0: 776f 6e27 2c20 2777 6f6f 272c 200a 2020  won', 'woo', .  
-00000df0: 2020 2777 6f6f 6b27 2c20 2777 6f6f 6e27    'wook', 'woon'
-00000e00: 2c20 2777 6f6f 6e67 272c 2027 7775 6b27  , 'woong', 'wuk'
-00000e10: 2c20 2778 6961 6f27 2c20 2779 6127 2c20  , 'xiao', 'ya', 
-00000e20: 2779 616e 272c 2027 7961 6e67 272c 2027  'yan', 'yang', '
-00000e30: 7961 6f27 2c20 2779 6527 2c20 0a20 2020  yao', 'ye', .   
-00000e40: 2027 7965 6127 2c20 2779 6565 272c 2027   'yea', 'yee', '
-00000e50: 7965 6827 2c20 2779 656e 272c 2027 7965  yeh', 'yen', 'ye
-00000e60: 6f27 2c20 2779 656f 6c27 2c20 2779 656f  o', 'yeol', 'yeo
-00000e70: 6e27 2c20 2779 656f 6e67 272c 2027 7965  n', 'yeong', 'ye
-00000e80: 6f70 272c 2027 7969 272c 200a 2020 2020  op', 'yi', .    
-00000e90: 2779 696e 272c 2027 7969 6e67 272c 2027  'yin', 'ying', '
-00000ea0: 7969 7527 2c20 2779 6f65 6e67 272c 2027  yiu', 'yoeng', '
-00000eb0: 796f 6e67 272c 2027 796f 6f27 2c20 2779  yong', 'yoo', 'y
-00000ec0: 6f6f 6e27 2c20 2779 6f75 272c 2027 796f  oon', 'you', 'yo
-00000ed0: 756e 6727 2c20 2779 7527 2c20 0a20 2020  ung', 'yu', .   
-00000ee0: 2027 7975 616e 272c 2027 7975 6527 2c20   'yuan', 'yue', 
-00000ef0: 2779 7565 6e27 2c20 2779 756b 272c 2027  'yuen', 'yuk', '
-00000f00: 7975 6c6c 272c 2027 7975 6e27 2c20 2779  yull', 'yun', 'y
-00000f10: 756e 6527 2c20 2779 756e 6727 2c20 277a  une', 'yung', 'z
-00000f20: 6869 272c 200a 2020 2020 277a 686f 6e67  hi', .    'zhong
-00000f30: 272c 2027 7a68 7527 0a5d 0a23 2073 6565  ', 'zhu'.].# see
-00000f40: 2068 7474 703a 2f2f 656e 2e77 696b 6970   http://en.wikip
-00000f50: 6564 6961 2e6f 7267 2f77 696b 692f 4c69  edia.org/wiki/Li
-00000f60: 7374 5f6f 665f 636f 6d6d 6f6e 5f43 6869  st_of_common_Chi
-00000f70: 6e65 7365 5f73 7572 6e61 6d65 730a 2320  nese_surnames.# 
-00000f80: 616e 6420 6874 7470 3a2f 2f65 6e2e 7769  and http://en.wi
-00000f90: 6b69 7065 6469 612e 6f72 672f 7769 6b69  kipedia.org/wiki
-00000fa0: 2f4c 6973 745f 6f66 5f4b 6f72 6561 6e5f  /List_of_Korean_
-00000fb0: 6661 6d69 6c79 5f6e 616d 6573 0a41 5349  family_names.ASI
-00000fc0: 414e 5f4c 4153 545f 4e41 4d45 5320 3d20  AN_LAST_NAMES = 
-00000fd0: 5b0a 2020 2020 2763 6861 6e27 2c20 2763  [.    'chan', 'c
-00000fe0: 6861 6e67 272c 2027 6368 616f 272c 0a20  hang', 'chao',. 
-00000ff0: 2020 2027 6368 656e 272c 2027 6368 656f     'chen', 'cheo
-00001000: 6e67 272c 2027 6368 6575 6e67 272c 0a20  ng', 'cheung',. 
-00001010: 2020 2027 6368 6f6e 6727 2c20 2763 686f     'chong', 'cho
-00001020: 6f27 2c0a 2020 2020 2763 6875 272c 2027  o',.    'chu', '
-00001030: 6368 756e 272c 0a20 2020 2027 686f 7527  chun',.    'hou'
-00001040: 2c20 2768 7369 6568 272c 2027 6873 7527  , 'hsieh', 'hsu'
-00001050: 2c20 2768 7527 2c20 2768 7561 6e67 272c  , 'hu', 'huang',
-00001060: 0a20 2020 2027 6b75 6f27 2c0a 2020 2020  .    'kuo',.    
-00001070: 276c 6927 2c20 276c 6961 6e67 272c 2027  'li', 'liang', '
-00001080: 6c69 6e27 2c20 276c 6975 272c 0a20 2020  lin', 'liu',.   
-00001090: 2027 5f70 6172 6b27 2c0a 2020 2020 2773   '_park',.    's
-000010a0: 756e 272c 2027 7375 6e67 272c 0a20 2020  un', 'sung',.   
-000010b0: 2027 7473 616f 272c 0a20 2020 2027 7761   'tsao',.    'wa
-000010c0: 6e67 272c 2027 576f 6e67 272c 0a20 2020  ng', 'Wong',.   
-000010d0: 2027 7961 6e67 272c 2027 7965 6f6e 6727   'yang', 'yeong'
-000010e0: 2c20 2779 6575 6e67 270a 5d0a 5052 4546  , 'yeung'.].PREF
-000010f0: 4958 4553 203d 205b 0a20 2020 2027 616c  IXES = [.    'al
-00001100: 272c 2027 6269 6e27 2c20 2764 6127 2c20  ', 'bin', 'da', 
-00001110: 2764 6527 2c20 2764 656c 272c 2027 6465  'de', 'del', 'de
-00001120: 6d27 2c20 2764 656e 272c 2027 6465 7227  m', 'den', 'der'
-00001130: 2c20 2764 6927 2c20 2764 6f73 272c 2027  , 'di', 'dos', '
-00001140: 6475 272c 0a20 2020 2027 6527 2c20 2765  du',.    'e', 'e
-00001150: 6c27 2c20 276c 6127 2c20 2773 616e 272c  l', 'la', 'san',
-00001160: 2027 7468 6527 2c20 2776 616e 272c 2027   'the', 'van', '
-00001170: 766f 6d27 2c20 2776 6f6e 272c 2027 7927  vom', 'von', 'y'
-00001180: 2c20 277a 7527 0a5d 0a4d 4944 4649 5845  , 'zu'.].MIDFIXE
-00001190: 5320 3d20 5b27 756e 6427 5d0a 5355 4646  S = ['und'].SUFF
-000011a0: 4958 4553 203d 205b 2769 6927 2c20 2769  IXES = ['ii', 'i
-000011b0: 6969 272c 2027 6a72 272c 2027 6a72 2e27  ii', 'jr', 'jr.'
-000011c0: 2c20 2770 682e 642e 272c 2027 7068 6427  , 'ph.d.', 'phd'
-000011d0: 2c20 2773 7227 2c20 2773 722e 275d 0a0a  , 'sr', 'sr.']..
-000011e0: 5541 5f41 4c49 4153 4553 203d 207b 0a20  UA_ALIASES = {. 
-000011f0: 2020 2027 6272 6f77 7365 7227 3a20 7b0a     'browser': {.
-00001200: 2020 2020 2020 2020 2743 6872 6f6d 6527          'Chrome'
-00001210: 3a20 2728 4372 694f 537c 4372 4d6f 2927  : '(CriOS|CrMo)'
-00001220: 2c0a 2020 2020 2020 2020 2746 6972 6566  ,.        'Firef
-00001230: 6f78 273a 2027 2846 656e 6e65 637c 4669  ox': '(Fennec|Fi
-00001240: 7265 6269 7264 7c49 6365 7765 6173 656c  rebird|Iceweasel
-00001250: 7c4d 696e 6566 6965 6c64 7c4e 616d 6f72  |Minefield|Namor
-00001260: 6f6b 617c 5068 6f65 6e69 787c 5365 614d  oka|Phoenix|SeaM
-00001270: 6f6e 6b65 797c 5368 6972 6574 6f6b 6f29  onkey|Shiretoko)
-00001280: 272c 0a20 2020 2020 2020 2027 4e6f 6b69  ',.        'Noki
-00001290: 6120 4272 6f77 7365 7227 3a20 2728 4f76  a Browser': '(Ov
-000012a0: 6942 726f 7773 6572 2927 0a20 2020 207d  iBrowser)'.    }
-000012b0: 2c0a 2020 2020 2772 6f62 6f74 273a 207b  ,.    'robot': {
-000012c0: 7d2c 0a20 2020 2027 7379 7374 656d 273a  },.    'system':
-000012d0: 207b 0a20 2020 2020 2020 2027 4253 4427   {.        'BSD'
-000012e0: 3a20 2728 4672 6565 4253 447c 4e65 7442  : '(FreeBSD|NetB
-000012f0: 5344 7c4f 7065 6e42 5344 2927 2c0a 2020  SD|OpenBSD)',.  
-00001300: 2020 2020 2020 274c 696e 7578 273a 2027        'Linux': '
-00001310: 2843 724f 537c 4d65 6547 6f7c 7765 624f  (CrOS|MeeGo|webO
-00001320: 5329 272c 0a20 2020 2020 2020 2027 556e  S)',.        'Un
-00001330: 6978 273a 2027 2841 4958 7c48 502d 5558  ix': '(AIX|HP-UX
-00001340: 7c49 5249 587c 5375 6e4f 5329 270a 2020  |IRIX|SunOS)'.  
-00001350: 2020 7d0a 7d0a 5541 5f4e 414d 4553 203d    }.}.UA_NAMES =
-00001360: 207b 0a20 2020 2027 6272 6f77 7365 7227   {.    'browser'
-00001370: 3a20 7b0a 2020 2020 2020 2020 2763 6872  : {.        'chr
-00001380: 6f6d 6566 7261 6d65 273a 2027 4368 726f  omeframe': 'Chro
-00001390: 6d65 2046 7261 6d65 272c 0a20 2020 2020  me Frame',.     
-000013a0: 2020 2027 4642 466f 7249 5068 6f6e 6527     'FBForIPhone'
-000013b0: 3a20 2757 6562 4b69 7427 2c0a 2020 2020  : 'WebKit',.    
-000013c0: 2020 2020 2747 6563 6b6f 273a 2027 4d6f      'Gecko': 'Mo
-000013d0: 7a69 6c6c 6127 2c0a 2020 2020 2020 2020  zilla',.        
-000013e0: 2749 454d 6f62 696c 6527 3a20 2749 6e74  'IEMobile': 'Int
-000013f0: 6572 6e65 7420 4578 706c 6f72 6572 272c  ernet Explorer',
-00001400: 0a20 2020 2020 2020 2027 6b6f 6e71 7565  .        'konque
-00001410: 726f 7227 3a20 274b 6f6e 7175 6572 6f72  ror': 'Konqueror
-00001420: 272c 0a20 2020 2020 2020 2027 4d6f 7a69  ',.        'Mozi
-00001430: 6c6c 6127 3a20 274e 6574 7363 6170 6527  lla': 'Netscape'
-00001440: 2c0a 2020 2020 2020 2020 274d 5349 4527  ,.        'MSIE'
-00001450: 3a20 2749 6e74 6572 6e65 7420 4578 706c  : 'Internet Expl
-00001460: 6f72 6572 272c 0a20 2020 2020 2020 2027  orer',.        '
-00001470: 4e6f 6b69 6142 726f 7773 6572 273a 2027  NokiaBrowser': '
-00001480: 4e6f 6b69 6120 4272 6f77 7365 7227 2c0a  Nokia Browser',.
-00001490: 2020 2020 2020 2020 2754 7269 6465 6e74          'Trident
-000014a0: 273a 2027 496e 7465 726e 6574 2045 7870  ': 'Internet Exp
-000014b0: 6c6f 7265 7227 0a20 2020 207d 2c0a 2020  lorer'.    },.  
-000014c0: 2020 2772 6f62 6f74 273a 207b 7d2c 0a20    'robot': {},. 
-000014d0: 2020 2027 7379 7374 656d 273a 207b 0a20     'system': {. 
-000014e0: 2020 2020 2020 2027 4242 273a 2027 426c         'BB': 'Bl
-000014f0: 6163 6b42 6572 7279 272c 0a20 2020 2020  ackBerry',.     
-00001500: 2020 2027 4350 5520 4f53 273a 2027 694f     'CPU OS': 'iO
-00001510: 5327 2c0a 2020 2020 2020 2020 2769 5068  S',.        'iPh
-00001520: 6f6e 6527 3a20 2769 4f53 272c 0a20 2020  one': 'iOS',.   
-00001530: 2020 2020 2027 6950 686f 6e65 204f 5327       'iPhone OS'
-00001540: 3a20 2769 4f53 272c 0a20 2020 2020 2020  : 'iOS',.       
-00001550: 2027 4a32 4d45 2f4d 4944 5027 3a20 274a   'J2ME/MIDP': 'J
-00001560: 6176 6127 2c0a 2020 2020 2020 2020 274d  ava',.        'M
-00001570: 6163 5f50 6f77 6572 5043 273a 2027 4d61  ac_PowerPC': 'Ma
-00001580: 6320 4f53 272c 0a20 2020 2020 2020 2027  c OS',.        '
-00001590: 4d61 635f 5050 4327 3a20 274d 6163 204f  Mac_PPC': 'Mac O
-000015a0: 5327 2c0a 2020 2020 2020 2020 274d 6163  S',.        'Mac
-000015b0: 696e 746f 7368 273a 2027 4d61 6320 4f53  intosh': 'Mac OS
-000015c0: 272c 0a20 2020 2020 2020 2027 504c 4159  ',.        'PLAY
-000015d0: 5354 4154 494f 4e27 3a20 2750 6c61 7953  STATION': 'PlayS
-000015e0: 7461 7469 6f6e 272c 0a20 2020 2020 2020  tation',.       
-000015f0: 2027 5327 3a20 274e 6f6b 6961 272c 0a20   'S': 'Nokia',. 
-00001600: 2020 2020 2020 2027 5365 7269 6573 273a         'Series':
-00001610: 2027 4e6f 6b69 6127 2c0a 2020 2020 2020   'Nokia',.      
-00001620: 2020 2757 696e 273a 2027 5769 6e64 6f77    'Win': 'Window
-00001630: 7327 2c0a 2020 2020 2020 2020 2757 696e  s',.        'Win
-00001640: 646f 7773 2050 686f 6e65 204f 5327 3a20  dows Phone OS': 
-00001650: 2757 696e 646f 7773 2050 686f 6e65 272c  'Windows Phone',
-00001660: 0a20 2020 2020 2020 2027 5831 3127 3a20  .        'X11': 
-00001670: 274c 696e 7578 270a 2020 2020 7d0a 7d0a  'Linux'.    }.}.
-00001680: 5541 5f52 4547 4558 5053 203d 207b 0a20  UA_REGEXPS = {. 
-00001690: 2020 2027 6272 6f77 7365 7227 3a20 5b0a     'browser': [.
-000016a0: 2020 2020 2020 2020 2728 4361 6d69 6e6f          '(Camino
-000016b0: 295c 2f28 5c64 2b29 272c 0a20 2020 2020  )\/(\d+)',.     
-000016c0: 2020 2027 2843 6869 6d65 7261 295c 2f28     '(Chimera)\/(
-000016d0: 5c64 2b29 272c 0a20 2020 2020 2020 2027  \d+)',.        '
-000016e0: 2863 6872 6f6d 6566 7261 6d65 295c 2f28  (chromeframe)\/(
-000016f0: 5c64 2b29 272c 0a20 2020 2020 2020 2027  \d+)',.        '
-00001700: 2845 6467 6529 5c2f 285c 642b 2927 2c0a  (Edge)\/(\d+)',.
-00001710: 2020 2020 2020 2020 2728 4570 6970 6861          '(Epipha
-00001720: 6e79 295c 2f28 5c64 2b29 272c 2020 2320  ny)\/(\d+)',  # 
-00001730: 6265 666f 7265 2043 6872 6f6d 652c 2043  before Chrome, C
-00001740: 6872 6f6d 6975 6d20 616e 6420 5361 6661  hromium and Safa
-00001750: 7269 0a20 2020 2020 2020 2027 2843 6872  ri.        '(Chr
-00001760: 6f6d 6975 6d29 5c2f 285c 642b 2927 2c20  omium)\/(\d+)', 
-00001770: 2023 2062 6566 6f72 6520 4368 726f 6d65   # before Chrome
-00001780: 0a20 2020 2020 2020 2027 2843 6872 6f6d  .        '(Chrom
-00001790: 6529 5c2f 285c 642b 2927 2c0a 2020 2020  e)\/(\d+)',.    
-000017a0: 2020 2020 2728 4642 466f 7249 5068 6f6e      '(FBForIPhon
-000017b0: 6529 272c 0a20 2020 2020 2020 2027 2846  e)',.        '(F
-000017c0: 6972 6566 6f78 295c 2f28 5c64 2b29 272c  irefox)\/(\d+)',
-000017d0: 0a20 2020 2020 2020 2027 2847 616c 656f  .        '(Galeo
-000017e0: 6e29 5c2f 285c 642b 2927 2c0a 2020 2020  n)\/(\d+)',.    
-000017f0: 2020 2020 2728 4945 4d6f 6269 6c65 295c      '(IEMobile)\
-00001800: 2f28 5c64 2b29 272c 0a20 2020 2020 2020  /(\d+)',.       
-00001810: 2027 2869 4361 6229 2028 5c64 2b29 272c   '(iCab) (\d+)',
-00001820: 0a20 2020 2020 2020 2027 2869 4361 6229  .        '(iCab)
-00001830: 5c2f 285c 642b 2927 2c0a 2020 2020 2020  \/(\d+)',.      
-00001840: 2020 2728 6b6f 6e71 7565 726f 7229 5c2f    '(konqueror)\/
-00001850: 285c 642b 2927 2c0a 2020 2020 2020 2020  (\d+)',.        
-00001860: 2728 4b6f 6e71 7565 726f 7229 5c2f 285c  '(Konqueror)\/(\
-00001870: 642b 2927 2c0a 2020 2020 2020 2020 2728  d+)',.        '(
-00001880: 4c79 6e78 295c 2f28 5c64 2b29 272c 0a20  Lynx)\/(\d+)',. 
-00001890: 2020 2020 2020 2027 284e 6574 7363 6170         '(Netscap
-000018a0: 6529 5c64 3f5c 2f28 5c64 2b29 272c 0a20  e)\d?\/(\d+)',. 
-000018b0: 2020 2020 2020 2027 284e 6f6b 6961 4272         '(NokiaBr
-000018c0: 6f77 7365 7229 5c2f 285c 642b 2927 2c0a  owser)\/(\d+)',.
-000018d0: 2020 2020 2020 2020 2728 4f6d 6e69 5765          '(OmniWe
-000018e0: 6229 5c2f 285c 642b 2927 2c0a 2020 2020  b)\/(\d+)',.    
-000018f0: 2020 2020 2728 4f70 6572 6129 5c2f 2e2b      '(Opera)\/.+
-00001900: 5665 7273 696f 6e5c 2f28 5c64 2b29 272c  Version\/(\d+)',
-00001910: 0a20 2020 2020 2020 2027 284f 7669 4272  .        '(OviBr
-00001920: 6f77 7365 7229 5c2f 285c 642b 2927 2c0a  owser)\/(\d+)',.
-00001930: 2020 2020 2020 2020 2756 6572 7369 6f6e          'Version
-00001940: 5c2f 285c 642b 292e 2b28 5361 6661 7269  \/(\d+).+(Safari
-00001950: 2927 2c0a 2020 2020 2020 2020 2728 5765  )',.        '(We
-00001960: 624b 6974 295c 2f28 5c64 2b29 272c 0a20  bKit)\/(\d+)',. 
-00001970: 2020 2020 2020 2027 284d 5349 4529 2028         '(MSIE) (
-00001980: 5c64 5c64 3f28 3f21 5c64 2929 272c 2020  \d\d?(?!\d))',  
-00001990: 2320 6c61 7374 2c20 7369 6e63 6520 4f70  # last, since Op
-000019a0: 6572 6120 7573 6564 2074 6f20 6d61 736b  era used to mask
-000019b0: 2061 7320 4d53 4945 0a20 2020 2020 2020   as MSIE.       
-000019c0: 2027 2854 7269 6465 6e74 295c 2f2e 2a3f   '(Trident)\/.*?
-000019d0: 7276 3a28 5c64 2b29 272c 0a20 2020 2020  rv:(\d+)',.     
-000019e0: 2020 2027 2847 6563 6b6f 2927 2c0a 2020     '(Gecko)',.  
-000019f0: 2020 2020 2020 2728 4d6f 7a69 6c6c 6129        '(Mozilla)
-00001a00: 5c2f 2833 7c34 2927 0a20 2020 205d 2c0a  \/(3|4)'.    ],.
-00001a10: 2020 2020 2772 6f62 6f74 273a 205b 0a20      'robot': [. 
-00001a20: 2020 2020 2020 2027 2842 696e 6750 7265         '(BingPre
-00001a30: 7669 6577 295c 2f28 5c64 2b29 272c 0a20  view)\/(\d+)',. 
-00001a40: 2020 2020 2020 2027 2847 6f6f 676c 6520         '(Google 
-00001a50: 5765 6220 5072 6576 6965 7729 2e2b 4368  Web Preview).+Ch
-00001a60: 726f 6d65 5c2f 285c 642b 2927 2c0a 2020  rome\/(\d+)',.  
-00001a70: 2020 2020 2020 2728 476f 6f67 6c65 626f        '(Googlebo
-00001a80: 7429 5c2f 285c 642b 2927 2c0a 2020 2020  t)\/(\d+)',.    
-00001a90: 2020 2020 2728 5765 6243 7261 776c 6572      '(WebCrawler
-00001aa0: 295c 2f28 5c64 2b29 272c 0a20 2020 2020  )\/(\d+)',.     
-00001ab0: 2020 2027 2859 6168 6f6f 2120 536c 7572     '(Yahoo! Slur
-00001ac0: 7029 5c2f 285c 642b 2927 2c0a 2020 2020  p)\/(\d+)',.    
-00001ad0: 2020 2020 2728 5961 6e64 6578 426f 7429      '(YandexBot)
-00001ae0: 5c2f 285b 5c64 5c2e 5d2b 2927 2c0a 2020  \/([\d\.]+)',.  
-00001af0: 2020 2020 2020 2728 5961 6e64 6578 4d6f        '(YandexMo
-00001b00: 6269 6c65 426f 7429 5c2f 285b 5c64 5c2e  bileBot)\/([\d\.
-00001b10: 5d2b 2927 2c0a 2020 2020 5d2c 0a20 2020  ]+)',.    ],.   
-00001b20: 2027 7379 7374 656d 273a 205b 0a20 2020   'system': [.   
-00001b30: 2020 2020 2027 2841 6e64 726f 6964 2920       '(Android) 
-00001b40: 285c 642b 2927 2c0a 2020 2020 2020 2020  (\d+)',.        
-00001b50: 2728 416e 6472 6f69 6429 272c 0a20 2020  '(Android)',.   
-00001b60: 2020 2020 2027 2842 4229 285c 642b 2927       '(BB)(\d+)'
-00001b70: 2c0a 2020 2020 2020 2020 2728 4265 4f53  ,.        '(BeOS
-00001b80: 2927 2c0a 2020 2020 2020 2020 2728 426c  )',.        '(Bl
-00001b90: 6163 6b42 6572 7279 2920 285c 642b 2927  ackBerry) (\d+)'
-00001ba0: 2c0a 2020 2020 2020 2020 2728 426c 6163  ,.        '(Blac
-00001bb0: 6b42 6572 7279 2927 2c0a 2020 2020 2020  kBerry)',.      
-00001bc0: 2020 2728 4461 7277 696e 2927 2c0a 2020    '(Darwin)',.  
-00001bd0: 2020 2020 2020 2728 4253 4429 2028 4672        '(BSD) (Fr
-00001be0: 6565 4253 447c 4e65 7442 5344 7c4f 7065  eeBSD|NetBSD|Ope
-00001bf0: 6e42 5344 2927 2c0a 2020 2020 2020 2020  nBSD)',.        
-00001c00: 2728 4350 5520 4f53 2920 285c 642b 2927  '(CPU OS) (\d+)'
-00001c10: 2c0a 2020 2020 2020 2020 2728 6950 686f  ,.        '(iPho
-00001c20: 6e65 204f 5329 2028 5c64 2b29 272c 0a20  ne OS) (\d+)',. 
-00001c30: 2020 2020 2020 2027 2869 5068 6f6e 6529         '(iPhone)
-00001c40: 272c 2020 2320 4f70 6572 610a 2020 2020  ',  # Opera.    
-00001c50: 2020 2020 2728 4a32 4d45 5c2f 4d49 4450      '(J2ME\/MIDP
-00001c60: 2927 2c0a 2020 2020 2020 2020 2728 4c69  )',.        '(Li
-00001c70: 6e75 7829 2e2b 2843 656e 744f 537c 4372  nux).+(CentOS|Cr
-00001c80: 4f53 7c44 6562 6961 6e7c 4665 646f 7261  OS|Debian|Fedora
-00001c90: 7c47 656e 746f 6f7c 4d61 6e64 7269 7661  |Gentoo|Mandriva
-00001ca0: 7c4d 6565 476f 7c4d 696e 747c 5265 6420  |MeeGo|Mint|Red 
-00001cb0: 4861 747c 5355 5345 7c55 6275 6e74 757c  Hat|SUSE|Ubuntu|
-00001cc0: 7765 624f 5329 272c 0a20 2020 2020 2020  webOS)',.       
-00001cd0: 2027 2843 656e 744f 537c 4372 4f53 7c44   '(CentOS|CrOS|D
-00001ce0: 6562 6961 6e7c 4665 646f 7261 7c47 656e  ebian|Fedora|Gen
-00001cf0: 746f 6f7c 4d61 6e64 7269 7661 7c4d 6565  too|Mandriva|Mee
-00001d00: 476f 7c4d 696e 747c 5265 6420 4861 747c  Go|Mint|Red Hat|
-00001d10: 5355 5345 7c55 6275 6e74 757c 7765 624f  SUSE|Ubuntu|webO
-00001d20: 5329 2e2b 284c 696e 7578 2927 2c0a 2020  S).+(Linux)',.  
-00001d30: 2020 2020 2020 2728 4c69 6e75 7829 272c        '(Linux)',
-00001d40: 0a20 2020 2020 2020 2027 284d 6163 204f  .        '(Mac O
-00001d50: 5320 5829 2028 3130 2e5c 642b 2927 2c0a  S X) (10.\d+)',.
-00001d60: 2020 2020 2020 2020 2728 4d61 6320 4f53          '(Mac OS
-00001d70: 2058 2927 2c0a 2020 2020 2020 2020 2728   X)',.        '(
-00001d80: 4d61 635f 506f 7765 7250 4329 272c 0a20  Mac_PowerPC)',. 
-00001d90: 2020 2020 2020 2027 284d 6163 5f50 5043         '(Mac_PPC
-00001da0: 2927 2c0a 2020 2020 2020 2020 2728 4d61  )',.        '(Ma
-00001db0: 6369 6e74 6f73 6829 272c 0a20 2020 2020  cintosh)',.     
-00001dc0: 2020 2027 4e69 6e74 656e 646f 2028 5769     'Nintendo (Wi
-00001dd0: 6929 2e2b 4e58 5c2f 285c 642b 2927 2c0a  i).+NX\/(\d+)',.
-00001de0: 2020 2020 2020 2020 2728 504c 4159 5354          '(PLAYST
-00001df0: 4154 494f 4e29 2028 5c64 2b29 272c 0a20  ATION) (\d+)',. 
-00001e00: 2020 2020 2020 2027 2850 6c61 7953 7461         '(PlaySta
-00001e10: 7469 6f6e 2920 5669 7461 2028 5c64 2b29  tion) Vita (\d+)
-00001e20: 272c 0a20 2020 2020 2020 2027 2852 494d  ',.        '(RIM
-00001e30: 2054 6162 6c65 7420 4f53 2920 285c 642b   Tablet OS) (\d+
-00001e40: 2927 2c0a 2020 2020 2020 2020 2728 5329  )',.        '(S)
-00001e50: 2836 3029 3b27 2c0a 2020 2020 2020 2020  (60);',.        
-00001e60: 2728 5365 7269 6573 2920 3f28 3430 7c36  '(Series) ?(40|6
-00001e70: 3029 272c 0a20 2020 2020 2020 2027 2853  0)',.        '(S
-00001e80: 796d 6269 616e 204f 5329 272c 0a20 2020  ymbian OS)',.   
-00001e90: 2020 2020 2027 2853 796d 6269 616e 4f53       '(SymbianOS
-00001ea0: 295c 2f28 5c64 2b29 272c 0a20 2020 2020  )\/(\d+)',.     
-00001eb0: 2020 2027 2853 796d 624f 5329 272c 0a20     '(SymbOS)',. 
-00001ec0: 2020 2020 2020 2027 284f 535c 2f32 2927         '(OS\/2)'
-00001ed0: 2c0a 2020 2020 2020 2020 2728 556e 6978  ,.        '(Unix
-00001ee0: 2920 2841 4958 7c48 502d 5558 7c49 5249  ) (AIX|HP-UX|IRI
-00001ef0: 587c 5375 6e4f 5329 272c 0a20 2020 2020  X|SunOS)',.     
-00001f00: 2020 2027 2855 6e69 7829 272c 0a20 2020     '(Unix)',.   
-00001f10: 2020 2020 2027 2857 696e 646f 7773 2920       '(Windows) 
-00001f20: 284e 5420 5c64 5c2e 5c64 2927 2c0a 2020  (NT \d\.\d)',.  
-00001f30: 2020 2020 2020 2728 5769 6e64 6f77 7320        '(Windows 
-00001f40: 5068 6f6e 6529 2028 5c64 2b29 272c 0a20  Phone) (\d+)',. 
-00001f50: 2020 2020 2020 2027 2857 696e 646f 7773         '(Windows
-00001f60: 2050 686f 6e65 204f 5329 2028 5c64 2b29   Phone OS) (\d+)
-00001f70: 272c 0a20 2020 2020 2020 2027 2857 696e  ',.        '(Win
-00001f80: 646f 7773 2920 2833 5c2e 317c 3935 7c39  dows) (3\.1|95|9
-00001f90: 387c 3230 3030 7c32 3030 337c 4345 7c4d  8|2000|2003|CE|M
-00001fa0: 457c 4d6f 6269 6c65 7c4e 547c 5850 2927  E|Mobile|NT|XP)'
-00001fb0: 2c20 2023 204f 7065 7261 0a20 2020 2020  ,  # Opera.     
-00001fc0: 2020 2027 2857 696e 2920 2839 7820 345c     '(Win) (9x 4\
-00001fd0: 2e39 3029 272c 2020 2320 4669 7265 666f  .90)',  # Firefo
-00001fe0: 780a 2020 2020 2020 2020 2728 5769 6e29  x.        '(Win)
-00001ff0: 2831 3629 272c 2020 2320 4669 7265 666f  (16)',  # Firefo
-00002000: 780a 2020 2020 2020 2020 2728 5769 6e29  x.        '(Win)
-00002010: 2839 5c64 2927 2c20 2023 2046 6972 6566  (9\d)',  # Firef
-00002020: 6f78 0a20 2020 2020 2020 2027 2857 696e  ox.        '(Win
-00002030: 2928 4e54 2927 2c20 2023 2046 6972 6566  )(NT)',  # Firef
-00002040: 6f78 0a20 2020 2020 2020 2027 2857 696e  ox.        '(Win
-00002050: 2928 4e54 345c 2e30 2927 2c20 2023 2046  )(NT4\.0)',  # F
-00002060: 6972 6566 6f78 0a20 2020 2020 2020 2027  irefox.        '
-00002070: 2858 3131 2927 0a20 2020 205d 0a7d 0a55  (X11)'.    ].}.U
-00002080: 415f 5645 5253 494f 4e53 203d 207b 0a20  A_VERSIONS = {. 
-00002090: 2020 2027 6272 6f77 7365 7227 3a20 7b7d     'browser': {}
-000020a0: 2c0a 2020 2020 2772 6f62 6f74 273a 207b  ,.    'robot': {
-000020b0: 7d2c 0a20 2020 2027 7379 7374 656d 273a  },.    'system':
-000020c0: 207b 0a20 2020 2020 2020 2027 3130 2e30   {.        '10.0
-000020d0: 273a 2027 3130 2e30 2028 4368 6565 7461  ': '10.0 (Cheeta
-000020e0: 6829 272c 0a20 2020 2020 2020 2027 3130  h)',.        '10
-000020f0: 2e31 273a 2027 3130 2e31 2028 5075 6d61  .1': '10.1 (Puma
-00002100: 2927 2c0a 2020 2020 2020 2020 2731 302e  )',.        '10.
-00002110: 3227 3a20 2731 302e 3220 284a 6167 7561  2': '10.2 (Jagua
-00002120: 7229 272c 0a20 2020 2020 2020 2027 3130  r)',.        '10
-00002130: 2e33 273a 2027 3130 2e33 2028 5061 6e74  .3': '10.3 (Pant
-00002140: 6865 7229 272c 0a20 2020 2020 2020 2027  her)',.        '
-00002150: 3130 2e34 273a 2027 3130 2e34 2028 5469  10.4': '10.4 (Ti
-00002160: 6765 7229 272c 0a20 2020 2020 2020 2027  ger)',.        '
-00002170: 3130 2e35 273a 2027 3130 2e35 2028 4c65  10.5': '10.5 (Le
-00002180: 6f70 6172 6429 272c 0a20 2020 2020 2020  opard)',.       
-00002190: 2027 3130 2e36 273a 2027 3130 2e36 2028   '10.6': '10.6 (
-000021a0: 536e 6f77 204c 656f 7061 7264 2927 2c0a  Snow Leopard)',.
-000021b0: 2020 2020 2020 2020 2731 302e 3727 3a20          '10.7': 
-000021c0: 2731 302e 3720 284c 696f 6e29 272c 0a20  '10.7 (Lion)',. 
-000021d0: 2020 2020 2020 2027 3130 2e38 273a 2027         '10.8': '
-000021e0: 3130 2e38 2028 4d6f 756e 7461 696e 204c  10.8 (Mountain L
-000021f0: 696f 6e29 272c 0a20 2020 2020 2020 2027  ion)',.        '
-00002200: 3130 2e39 273a 2027 3130 2e39 2028 4d61  10.9': '10.9 (Ma
-00002210: 7665 7269 636b 7329 272c 0a20 2020 2020  vericks)',.     
-00002220: 2020 2027 3130 2e31 3027 3a20 2731 302e     '10.10': '10.
-00002230: 3130 2028 596f 7365 6d69 7465 2927 2c0a  10 (Yosemite)',.
-00002240: 2020 2020 2020 2020 2731 302e 3131 273a          '10.11':
-00002250: 2027 3130 2e31 3120 2845 6c20 4361 7069   '10.11 (El Capi
-00002260: 7461 6e29 272c 0a20 2020 2020 2020 2027  tan)',.        '
-00002270: 3430 273a 2027 5365 7269 6573 2034 3027  40': 'Series 40'
-00002280: 2c0a 2020 2020 2020 2020 2736 3027 3a20  ,.        '60': 
-00002290: 2753 6572 6965 7320 3630 272c 0a20 2020  'Series 60',.   
-000022a0: 2020 2020 2027 4e54 2033 2e31 273a 2027       'NT 3.1': '
-000022b0: 4e54 2033 2e31 2028 332e 3129 272c 0a20  NT 3.1 (3.1)',. 
-000022c0: 2020 2020 2020 2027 4e54 2033 2e35 273a         'NT 3.5':
-000022d0: 2027 4e54 2033 2e35 2028 4e54 2927 2c0a   'NT 3.5 (NT)',.
-000022e0: 2020 2020 2020 2020 274e 5420 342e 3027          'NT 4.0'
-000022f0: 3a20 274e 5420 342e 3020 284e 5429 272c  : 'NT 4.0 (NT)',
-00002300: 0a20 2020 2020 2020 2027 4e54 2034 2e31  .        'NT 4.1
-00002310: 273a 2027 4e54 2034 2e31 2028 3938 2927  ': 'NT 4.1 (98)'
-00002320: 2c0a 2020 2020 2020 2020 2739 7820 342e  ,.        '9x 4.
-00002330: 3930 273a 2027 4e54 2034 2e39 2028 4d45  90': 'NT 4.9 (ME
-00002340: 2927 2c0a 2020 2020 2020 2020 274e 5420  )',.        'NT 
-00002350: 352e 3027 3a20 274e 5420 352e 3020 2832  5.0': 'NT 5.0 (2
-00002360: 3030 3029 272c 0a20 2020 2020 2020 2027  000)',.        '
-00002370: 4e54 2035 2e31 273a 2027 4e54 2035 2e31  NT 5.1': 'NT 5.1
-00002380: 2028 5850 2927 2c0a 2020 2020 2020 2020   (XP)',.        
-00002390: 274e 5420 352e 3227 3a20 274e 5420 352e  'NT 5.2': 'NT 5.
-000023a0: 3220 2832 3030 3329 272c 0a20 2020 2020  2 (2003)',.     
-000023b0: 2020 2027 4e54 2036 2e30 273a 2027 4e54     'NT 6.0': 'NT
-000023c0: 2036 2e30 2028 5669 7374 6129 272c 0a20   6.0 (Vista)',. 
-000023d0: 2020 2020 2020 2027 4e54 2036 2e31 273a         'NT 6.1':
-000023e0: 2027 4e54 2036 2e31 2028 3729 272c 0a20   'NT 6.1 (7)',. 
-000023f0: 2020 2020 2020 2027 4e54 2036 2e32 273a         'NT 6.2':
-00002400: 2027 4e54 2036 2e32 2028 3829 272c 0a20   'NT 6.2 (8)',. 
-00002410: 2020 2020 2020 2027 4e54 2036 2e33 273a         'NT 6.3':
-00002420: 2027 4e54 2036 2e33 2028 382e 3129 272c   'NT 6.3 (8.1)',
-00002430: 0a20 2020 2020 2020 2027 4e54 2036 2e34  .        'NT 6.4
-00002440: 273a 2027 4e54 2036 2e34 2028 3130 2927  ': 'NT 6.4 (10)'
-00002450: 2c0a 2020 2020 2020 2020 2731 3627 3a20  ,.        '16': 
-00002460: 274e 5420 332e 3120 2833 2e31 2927 2c0a  'NT 3.1 (3.1)',.
-00002470: 2020 2020 2020 2020 2733 2e31 273a 2027          '3.1': '
-00002480: 4e54 2033 2e31 2028 332e 3129 272c 0a20  NT 3.1 (3.1)',. 
-00002490: 2020 2020 2020 2027 3935 273a 2027 4e54         '95': 'NT
-000024a0: 2034 2e30 2028 3935 2927 2c0a 2020 2020   4.0 (95)',.    
-000024b0: 2020 2020 274e 5427 3a20 274e 5420 342e      'NT': 'NT 4.
-000024c0: 3020 284e 5429 272c 0a20 2020 2020 2020  0 (NT)',.       
-000024d0: 2027 4e54 342e 3027 3a20 274e 5420 342e   'NT4.0': 'NT 4.
-000024e0: 3020 284e 5429 272c 0a20 2020 2020 2020  0 (NT)',.       
-000024f0: 2027 3938 273a 2027 4e54 2034 2e31 2028   '98': 'NT 4.1 (
-00002500: 3938 2927 2c0a 2020 2020 2020 2020 274d  98)',.        'M
-00002510: 4527 3a20 274e 5420 342e 3920 284d 4529  E': 'NT 4.9 (ME)
-00002520: 272c 0a20 2020 2020 2020 2027 3230 3030  ',.        '2000
-00002530: 273a 2027 4e54 2035 2e30 2028 3230 3030  ': 'NT 5.0 (2000
-00002540: 2927 2c0a 2020 2020 2020 2020 2758 5027  )',.        'XP'
-00002550: 3a20 274e 5420 352e 3120 2858 5029 272c  : 'NT 5.1 (XP)',
-00002560: 0a20 2020 2020 2020 2027 3230 3033 273a  .        '2003':
-00002570: 2027 4e54 2035 2e32 2028 3230 3033 2927   'NT 5.2 (2003)'
-00002580: 0a20 2020 207d 0a7d 0a0a 6465 6620 6765  .    }.}..def ge
-00002590: 745f 736f 7274 5f6e 616d 6528 6e61 6d65  t_sort_name(name
-000025a0: 293a 0a20 2020 2022 2222 0a0a 2020 2020  ):.    """..    
-000025b0: 3e3e 3e20 6765 745f 736f 7274 5f6e 616d  >>> get_sort_nam
-000025c0: 6528 2741 6c66 7265 6420 4869 7463 6863  e('Alfred Hitchc
-000025d0: 6f63 6b27 290a 2020 2020 2748 6974 6368  ock').    'Hitch
-000025e0: 636f 636b 2c20 416c 6672 6564 270a 0a20  cock, Alfred'.. 
-000025f0: 2020 203e 3e3e 2067 6574 5f73 6f72 745f     >>> get_sort_
-00002600: 6e61 6d65 2827 4a65 616e 2d4c 7563 2047  name('Jean-Luc G
-00002610: 6f64 6172 6427 290a 2020 2020 2747 6f64  odard').    'God
-00002620: 6172 642c 204a 6561 6e2d 4c75 6327 0a0a  ard, Jean-Luc'..
-00002630: 2020 2020 3e3e 3e20 6765 745f 736f 7274      >>> get_sort
-00002640: 5f6e 616d 6528 2752 6169 6e65 7220 5765  _name('Rainer We
-00002650: 726e 6572 2046 6173 7362 696e 6465 7227  rner Fassbinder'
-00002660: 290a 2020 2020 2746 6173 7362 696e 6465  ).    'Fassbinde
-00002670: 722c 2052 6169 6e65 7220 5765 726e 6572  r, Rainer Werner
-00002680: 270a 0a20 2020 203e 3e3e 2067 6574 5f73  '..    >>> get_s
-00002690: 6f72 745f 6e61 6d65 2827 4272 6961 6e20  ort_name('Brian 
-000026a0: 4465 2050 616c 6d61 2729 0a20 2020 2027  De Palma').    '
-000026b0: 4465 2050 616c 6d61 2c20 4272 6961 6e27  De Palma, Brian'
-000026c0: 0a0a 2020 2020 3e3e 3e20 6765 745f 736f  ..    >>> get_so
-000026d0: 7274 5f6e 616d 6528 274a 6f68 616e 2076  rt_name('Johan v
-000026e0: 616e 2064 6572 204b 6575 6b65 6e27 290a  an der Keuken').
-000026f0: 2020 2020 2776 616e 2064 6572 204b 6575      'van der Keu
-00002700: 6b65 6e2c 204a 6f68 616e 270a 0a20 2020  ken, Johan'..   
-00002710: 203e 3e3e 2067 6574 5f73 6f72 745f 6e61   >>> get_sort_na
-00002720: 6d65 2827 4564 7761 7264 2044 2e20 576f  me('Edward D. Wo
-00002730: 6f64 204a 722e 2729 0a20 2020 2027 576f  od Jr.').    'Wo
-00002740: 6f64 204a 722e 2c20 4564 7761 7264 2044  od Jr., Edward D
-00002750: 2e27 0a0a 2020 2020 3e3e 3e20 6765 745f  .'..    >>> get_
-00002760: 736f 7274 5f6e 616d 6528 2742 696e 6720  sort_name('Bing 
-00002770: 5761 6e67 2729 0a20 2020 2027 5761 6e67  Wang').    'Wang
-00002780: 2042 696e 6727 0a0a 2020 2020 3e3e 3e20   Bing'..    >>> 
-00002790: 6765 745f 736f 7274 5f6e 616d 6528 2746  get_sort_name('F
-000027a0: 7261 6e6b 2043 6170 7261 2049 4949 2729  rank Capra III')
-000027b0: 0a20 2020 2027 4361 7072 6120 4949 492c  .    'Capra III,
-000027c0: 2046 7261 6e6b 270a 0a20 2020 203e 3e3e   Frank'..    >>>
-000027d0: 2067 6574 5f73 6f72 745f 6e61 6d65 2827   get_sort_name('
-000027e0: 5468 6520 5175 6565 6e20 6f66 2045 6e67  The Queen of Eng
-000027f0: 6c61 6e64 2729 0a20 2020 2027 5175 6565  land').    'Quee
-00002800: 6e20 6f66 2045 6e67 6c61 6e64 2c20 5468  n of England, Th
-00002810: 6527 0a0a 2020 2020 3e3e 3e20 6765 745f  e'..    >>> get_
-00002820: 736f 7274 5f6e 616d 6528 2753 6861 6d20  sort_name('Sham 
-00002830: 3639 2729 0a20 2020 2027 5368 616d 2036  69').    'Sham 6
-00002840: 3927 0a0a 2020 2020 3e3e 3e20 6765 745f  9'..    >>> get_
-00002850: 736f 7274 5f6e 616d 6528 2753 636f 7273  sort_name('Scors
-00002860: 6573 652c 204d 6172 7469 6e27 290a 2020  ese, Martin').  
-00002870: 2020 2753 636f 7273 6573 652c 204d 6172    'Scorsese, Mar
-00002880: 7469 6e27 0a20 2020 2022 2222 0a20 2020  tin'.    """.   
-00002890: 2069 6620 2720 2720 6e6f 7420 696e 206e   if ' ' not in n
-000028a0: 616d 6520 6f72 2027 2c20 2720 696e 206e  ame or ', ' in n
-000028b0: 616d 653a 0a20 2020 2020 2020 2072 6574  ame:.        ret
-000028c0: 7572 6e20 6e61 6d65 0a20 2020 2069 6620  urn name.    if 
-000028d0: 6e61 6d65 2e6c 6f77 6572 2829 2e73 7461  name.lower().sta
-000028e0: 7274 7377 6974 6828 2774 6865 2027 293a  rtswith('the '):
-000028f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00002900: 6765 745f 736f 7274 5f74 6974 6c65 286e  get_sort_title(n
-00002910: 616d 6529 0a0a 2020 2020 6465 6620 6164  ame)..    def ad
-00002920: 645f 6e61 6d65 2829 3a0a 2020 2020 2020  d_name():.      
-00002930: 2020 6966 206c 656e 2866 6972 7374 5f6e    if len(first_n
-00002940: 616d 6573 293a 0a20 2020 2020 2020 2020  ames):.         
-00002950: 2020 206c 6173 745f 6e61 6d65 732e 696e     last_names.in
-00002960: 7365 7274 2830 2c20 6669 7273 745f 6e61  sert(0, first_na
-00002970: 6d65 732e 706f 7028 2929 0a0a 2020 2020  mes.pop())..    
-00002980: 6465 6620 6669 6e64 5f6e 616d 6528 6e61  def find_name(na
-00002990: 6d65 7329 3a0a 2020 2020 2020 2020 7265  mes):.        re
-000029a0: 7475 726e 206c 656e 2866 6972 7374 5f6e  turn len(first_n
-000029b0: 616d 6573 2920 616e 6420 6669 7273 745f  ames) and first_
-000029c0: 6e61 6d65 735b 2d31 5d2e 6c6f 7765 7228  names[-1].lower(
-000029d0: 2920 696e 206e 616d 6573 0a0a 2020 2020  ) in names..    
-000029e0: 6966 2069 735f 6173 6961 6e5f 6e61 6d65  if is_asian_name
-000029f0: 286e 616d 6529 3a0a 2020 2020 2020 2020  (name):.        
-00002a00: 6e61 6d65 7320 3d20 6e61 6d65 2e72 6570  names = name.rep
-00002a10: 6c61 6365 2827 2d27 2c20 2720 2729 2e73  lace('-', ' ').s
-00002a20: 706c 6974 2827 2027 290a 2020 2020 2020  plit(' ').      
-00002a30: 2020 6966 206c 656e 286e 616d 6573 2920    if len(names) 
-00002a40: 3d3d 2032 3a0a 2020 2020 2020 2020 2020  == 2:.          
-00002a50: 2020 6966 206e 616d 6573 5b30 5d2e 6c6f    if names[0].lo
-00002a60: 7765 7228 2920 696e 2041 5349 414e 5f4c  wer() in ASIAN_L
-00002a70: 4153 545f 4e41 4d45 533a 0a20 2020 2020  AST_NAMES:.     
-00002a80: 2020 2020 2020 2020 2020 206c 6173 746e             lastn
-00002a90: 616d 652c 2066 6972 7374 6e61 6d65 203d  ame, firstname =
-00002aa0: 206e 616d 6573 0a20 2020 2020 2020 2020   names.         
-00002ab0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00002ac0: 2020 2020 2020 2020 2066 6972 7374 6e61           firstna
-00002ad0: 6d65 2c20 6c61 7374 6e61 6d65 203d 206e  me, lastname = n
-00002ae0: 616d 6573 0a20 2020 2020 2020 2065 6c73  ames.        els
-00002af0: 653a 0a20 2020 2020 2020 2020 2020 206e  e:.            n
-00002b00: 616d 6573 5f20 3d20 6e61 6d65 2e73 706c  ames_ = name.spl
-00002b10: 6974 2827 2027 290a 2020 2020 2020 2020  it(' ').        
-00002b20: 2020 2020 6966 2027 2d27 2069 6e20 6e61      if '-' in na
-00002b30: 6d65 735f 5b30 5d3a 0a20 2020 2020 2020  mes_[0]:.       
-00002b40: 2020 2020 2020 2020 206c 6173 746e 616d           lastnam
-00002b50: 652c 2066 6972 7374 6e61 6d65 203d 205b  e, firstname = [
-00002b60: 6e61 6d65 735b 325d 2c20 6e61 6d65 735b  names[2], names[
-00002b70: 305d 202b 2027 2d27 202b 206e 616d 6573  0] + '-' + names
-00002b80: 5b31 5d2e 6c6f 7765 7228 295d 0a20 2020  [1].lower()].   
-00002b90: 2020 2020 2020 2020 2065 6c69 6620 272d           elif '-
-00002ba0: 2720 696e 206e 616d 6573 5f5b 315d 3a0a  ' in names_[1]:.
-00002bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bc0: 6c61 7374 6e61 6d65 2c20 6669 7273 746e  lastname, firstn
-00002bd0: 616d 6520 3d20 5b6e 616d 6573 5b30 5d2c  ame = [names[0],
-00002be0: 206e 616d 6573 5b31 5d20 2b20 272d 2720   names[1] + '-' 
-00002bf0: 2b20 6e61 6d65 735b 325d 2e6c 6f77 6572  + names[2].lower
-00002c00: 2829 5d0a 2020 2020 2020 2020 2020 2020  ()].            
-00002c10: 656c 6966 206e 616d 6573 5b30 5d2e 6c6f  elif names[0].lo
-00002c20: 7765 7228 2920 696e 2041 5349 414e 5f46  wer() in ASIAN_F
-00002c30: 4952 5354 5f4e 414d 4553 2061 6e64 206e  IRST_NAMES and n
-00002c40: 616d 6573 5b32 5d2e 6c6f 7765 7228 2920  ames[2].lower() 
-00002c50: 6e6f 7420 696e 2041 5349 414e 5f46 4952  not in ASIAN_FIR
-00002c60: 5354 5f4e 414d 4553 3a0a 2020 2020 2020  ST_NAMES:.      
-00002c70: 2020 2020 2020 2020 2020 6c61 7374 6e61            lastna
-00002c80: 6d65 2c20 6669 7273 746e 616d 6520 3d20  me, firstname = 
-00002c90: 5b6e 616d 6573 5b32 5d2c 206e 616d 6573  [names[2], names
-00002ca0: 5b30 5d20 2b20 2720 2720 2b20 6e61 6d65  [0] + ' ' + name
-00002cb0: 735b 315d 5d0a 2020 2020 2020 2020 2020  s[1]].          
-00002cc0: 2020 656c 6966 206e 616d 6573 5b30 5d2e    elif names[0].
-00002cd0: 6c6f 7765 7228 2920 6e6f 7420 696e 2041  lower() not in A
-00002ce0: 5349 414e 5f46 4952 5354 5f4e 414d 4553  SIAN_FIRST_NAMES
-00002cf0: 2061 6e64 206e 616d 6573 5b32 5d2e 6c6f   and names[2].lo
-00002d00: 7765 7228 2920 696e 2041 5349 414e 5f46  wer() in ASIAN_F
-00002d10: 4952 5354 5f4e 414d 4553 3a0a 2020 2020  IRST_NAMES:.    
-00002d20: 2020 2020 2020 2020 2020 2020 6c61 7374              last
-00002d30: 6e61 6d65 2c20 6669 7273 746e 616d 6520  name, firstname 
-00002d40: 3d20 5b6e 616d 6573 5b30 5d2c 206e 616d  = [names[0], nam
-00002d50: 6573 5b31 5d20 2b20 2720 2720 2b20 6e61  es[1] + ' ' + na
-00002d60: 6d65 735b 325d 5d0a 2020 2020 2020 2020  mes[2]].        
-00002d70: 2020 2020 656c 6966 206e 616d 6573 5b30      elif names[0
-00002d80: 5d2e 6c6f 7765 7228 2920 696e 2041 5349  ].lower() in ASI
-00002d90: 414e 5f4c 4153 545f 4e41 4d45 533a 0a20  AN_LAST_NAMES:. 
-00002da0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00002db0: 6173 746e 616d 652c 2066 6972 7374 6e61  astname, firstna
-00002dc0: 6d65 203d 205b 6e61 6d65 735b 305d 2c20  me = [names[0], 
-00002dd0: 6e61 6d65 735b 315d 202b 2027 2027 202b  names[1] + ' ' +
-00002de0: 206e 616d 6573 5b32 5d5d 0a20 2020 2020   names[2]].     
-00002df0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00002e00: 2020 2020 2020 2020 2020 2020 206c 6173               las
-00002e10: 746e 616d 652c 2066 6972 7374 6e61 6d65  tname, firstname
-00002e20: 203d 205b 6e61 6d65 735b 325d 2c20 6e61   = [names[2], na
-00002e30: 6d65 735b 305d 202b 2027 2027 202b 206e  mes[0] + ' ' + n
-00002e40: 616d 6573 5b31 5d5d 0a20 2020 2020 2020  ames[1]].       
-00002e50: 2072 6574 7572 6e20 6c61 7374 6e61 6d65   return lastname
-00002e60: 202b 2027 2027 202b 2066 6972 7374 6e61   + ' ' + firstna
-00002e70: 6d65 0a0a 2020 2020 6669 7273 745f 6e61  me..    first_na
-00002e80: 6d65 7320 3d20 6e61 6d65 2e73 706c 6974  mes = name.split
-00002e90: 2827 2027 290a 2020 2020 6c61 7374 5f6e  (' ').    last_n
-00002ea0: 616d 6573 203d 205b 5d0a 2020 2020 6966  ames = [].    if
-00002eb0: 2072 652e 7365 6172 6368 2827 5e5b 302d   re.search('^[0-
-00002ec0: 395d 2b24 272c 2066 6972 7374 5f6e 616d  9]+$', first_nam
-00002ed0: 6573 5b2d 315d 293a 0a20 2020 2020 2020  es[-1]):.       
-00002ee0: 2061 6464 5f6e 616d 6528 290a 2020 2020   add_name().    
-00002ef0: 6966 2072 652e 7365 6172 6368 2827 5b28  if re.search('[(
-00002f00: 5c5b 5d2e 2b3f 5b29 5c5d 5d24 272c 2066  \[].+?[)\]]$', f
-00002f10: 6972 7374 5f6e 616d 6573 5b2d 315d 293a  irst_names[-1]):
-00002f20: 0a20 2020 2020 2020 2061 6464 5f6e 616d  .        add_nam
-00002f30: 6528 290a 2020 2020 6966 2066 696e 645f  e().    if find_
-00002f40: 6e61 6d65 2853 5546 4649 5845 5329 3a0a  name(SUFFIXES):.
-00002f50: 2020 2020 2020 2020 6164 645f 6e61 6d65          add_name
-00002f60: 2829 0a20 2020 2061 6464 5f6e 616d 6528  ().    add_name(
-00002f70: 290a 2020 2020 6966 2066 696e 645f 6e61  ).    if find_na
-00002f80: 6d65 284d 4944 4649 5845 5329 3a0a 2020  me(MIDFIXES):.  
-00002f90: 2020 2020 2020 6164 645f 6e61 6d65 2829        add_name()
-00002fa0: 0a20 2020 2020 2020 2061 6464 5f6e 616d  .        add_nam
-00002fb0: 6528 290a 2020 2020 7768 696c 6520 6669  e().    while fi
-00002fc0: 6e64 5f6e 616d 6528 5052 4546 4958 4553  nd_name(PREFIXES
-00002fd0: 293a 0a20 2020 2020 2020 2061 6464 5f6e  ):.        add_n
-00002fe0: 616d 6528 290a 2020 2020 6e61 6d65 203d  ame().    name =
-00002ff0: 2027 2027 2e6a 6f69 6e28 6c61 7374 5f6e   ' '.join(last_n
-00003000: 616d 6573 290a 2020 2020 6966 206c 656e  ames).    if len
-00003010: 2866 6972 7374 5f6e 616d 6573 293a 0a20  (first_names):. 
-00003020: 2020 2020 2020 2073 6570 6172 6174 6f72         separator
-00003030: 203d 2027 2027 2069 6620 6c61 7374 5f6e   = ' ' if last_n
-00003040: 616d 6573 5b30 5d2e 6c6f 7765 7228 2920  ames[0].lower() 
-00003050: 696e 2041 5349 414e 5f4c 4153 545f 4e41  in ASIAN_LAST_NA
-00003060: 4d45 5320 656c 7365 2027 2c20 270a 2020  MES else ', '.  
-00003070: 2020 2020 2020 6e61 6d65 202b 3d20 7365        name += se
-00003080: 7061 7261 746f 7220 2b20 2720 272e 6a6f  parator + ' '.jo
-00003090: 696e 2866 6972 7374 5f6e 616d 6573 290a  in(first_names).
-000030a0: 2020 2020 7265 7475 726e 206e 616d 650a      return name.
-000030b0: 0a64 6566 2067 6574 5f73 6f72 745f 7469  .def get_sort_ti
-000030c0: 746c 6528 7469 746c 6529 3a0a 2020 2020  tle(title):.    
-000030d0: 2222 220a 0a20 2020 203e 3e3e 2067 6574  """..    >>> get
-000030e0: 5f73 6f72 745f 7469 746c 6528 2754 6865  _sort_title('The
-000030f0: 6d72 6f63 2729 0a20 2020 2027 5468 656d  mroc').    'Them
-00003100: 726f 6327 0a0a 2020 2020 3e3e 3e20 6765  roc'..    >>> ge
-00003110: 745f 736f 7274 5f74 6974 6c65 2827 4469  t_sort_title('Di
-00003120: 6520 4861 7264 2729 0a20 2020 2027 4861  e Hard').    'Ha
-00003130: 7264 2c20 4469 6527 0a0a 2020 2020 3e3e  rd, Die'..    >>
-00003140: 3e20 6765 745f 736f 7274 5f74 6974 6c65  > get_sort_title
-00003150: 2822 4c27 6174 616c 616e 7465 2229 0a20  ("L'atalante"). 
-00003160: 2020 2022 6174 616c 616e 7465 2c20 4c27     "atalante, L'
-00003170: 220a 0a20 2020 2022 2222 0a20 2020 2066  "..    """.    f
-00003180: 6f72 2061 7274 6963 6c65 2069 6e20 4152  or article in AR
-00003190: 5449 434c 4553 3a0a 2020 2020 2020 2020  TICLES:.        
-000031a0: 7370 6163 6573 203d 2030 2069 6620 6172  spaces = 0 if ar
-000031b0: 7469 636c 652e 656e 6473 7769 7468 2822  ticle.endswith("
-000031c0: 2722 2920 656c 7365 2031 0a20 2020 2020  '") else 1.     
-000031d0: 2020 2069 6620 7469 746c 652e 6c6f 7765     if title.lowe
-000031e0: 7228 292e 7374 6172 7473 7769 7468 2861  r().startswith(a
-000031f0: 7274 6963 6c65 202b 2027 2027 202a 2073  rticle + ' ' * s
-00003200: 7061 6365 7329 3a0a 2020 2020 2020 2020  paces):.        
-00003210: 2020 2020 6c65 6e67 7468 203d 206c 656e      length = len
-00003220: 2861 7274 6963 6c65 290a 2020 2020 2020  (article).      
-00003230: 2020 2020 2020 7265 7475 726e 2074 6974        return tit
-00003240: 6c65 5b6c 656e 6774 6820 2b20 7370 6163  le[length + spac
-00003250: 6573 3a5d 202b 2027 2c20 2720 2b20 7469  es:] + ', ' + ti
-00003260: 746c 655b 3a6c 656e 6774 685d 0a20 2020  tle[:length].   
-00003270: 2072 6574 7572 6e20 7469 746c 650a 0a64   return title..d
-00003280: 6566 2066 696e 645f 7265 2873 7472 696e  ef find_re(strin
-00003290: 672c 2072 6567 6578 7029 3a0a 2020 2020  g, regexp):.    
-000032a0: 7265 7375 6c74 203d 2072 652e 636f 6d70  result = re.comp
-000032b0: 696c 6528 7265 6765 7870 2c20 7265 2e44  ile(regexp, re.D
-000032c0: 4f54 414c 4c29 2e66 696e 6461 6c6c 2873  OTALL).findall(s
-000032d0: 7472 696e 6729 0a20 2020 2069 6620 7265  tring).    if re
-000032e0: 7375 6c74 3a0a 2020 2020 2020 2020 7265  sult:.        re
-000032f0: 7475 726e 2072 6573 756c 745b 305d 2e73  turn result[0].s
-00003300: 7472 6970 2829 0a20 2020 2072 6574 7572  trip().    retur
-00003310: 6e20 2727 0a0a 6465 6620 6669 6e64 5f73  n ''..def find_s
-00003320: 7472 696e 6728 7374 7269 6e67 2c20 7374  tring(string, st
-00003330: 7269 6e67 303d 2727 2c20 7374 7269 6e67  ring0='', string
-00003340: 313d 2727 293a 0a20 2020 2022 2222 5265  1=''):.    """Re
-00003350: 7475 726e 2074 6865 2073 7472 696e 6720  turn the string 
-00003360: 6265 7477 6565 6e20 7374 7269 6e67 3020  between string0 
-00003370: 616e 6420 7374 7269 6e67 312e 0a0a 2020  and string1...  
-00003380: 2020 4966 2073 7472 696e 6730 206f 7220    If string0 or 
-00003390: 7374 7269 6e67 3120 6973 206c 6566 7420  string1 is left 
-000033a0: 6f75 742c 2062 6567 696e 696e 6720 6f72  out, begining or
-000033b0: 2065 6e64 206f 6620 7374 7269 6e67 2069   end of string i
-000033c0: 7320 7573 6564 2e0a 0a20 2020 203e 3e3e  s used...    >>>
-000033d0: 2066 696e 645f 7374 7269 6e67 2827 6920   find_string('i 
-000033e0: 616d 206e 6f74 2074 6865 7265 272c 2073  am not there', s
-000033f0: 7472 696e 6731 3d27 206e 6f74 2074 6865  tring1=' not the
-00003400: 7265 2729 0a20 2020 2027 6920 616d 270a  re').    'i am'.
-00003410: 0a20 2020 203e 3e3e 2066 696e 645f 7374  .    >>> find_st
-00003420: 7269 6e67 2827 6920 616d 206e 6f74 2074  ring('i am not t
-00003430: 6865 7265 272c 2027 6920 616d 2027 2c20  here', 'i am ', 
-00003440: 2720 7468 6572 6527 290a 2020 2020 276e  ' there').    'n
-00003450: 6f74 270a 0a20 2020 203e 3e3e 2066 696e  ot'..    >>> fin
-00003460: 645f 7374 7269 6e67 2827 6920 616d 206e  d_string('i am n
-00003470: 6f74 2074 6865 7265 272c 2027 6920 616d  ot there', 'i am
-00003480: 206e 6f74 2074 2729 0a20 2020 2027 6865   not t').    'he
-00003490: 7265 270a 0a20 2020 2022 2222 0a20 2020  re'..    """.   
-000034a0: 2069 6620 7374 7269 6e67 303a 0a20 2020   if string0:.   
-000034b0: 2020 2020 2073 7472 696e 6730 203d 2072       string0 = r
-000034c0: 652e 6573 6361 7065 2873 7472 696e 6730  e.escape(string0
-000034d0: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-000034e0: 2020 2020 7374 7269 6e67 3020 3d20 275e      string0 = '^
-000034f0: 270a 2020 2020 6966 2073 7472 696e 6731  '.    if string1
-00003500: 3a0a 2020 2020 2020 2020 7374 7269 6e67  :.        string
-00003510: 3120 3d20 7265 2e65 7363 6170 6528 7374  1 = re.escape(st
-00003520: 7269 6e67 3129 0a20 2020 2065 6c73 653a  ring1).    else:
-00003530: 0a20 2020 2020 2020 2073 7472 696e 6731  .        string1
-00003540: 203d 2027 2427 0a20 2020 2072 6574 7572   = '$'.    retur
-00003550: 6e20 6669 6e64 5f72 6528 7374 7269 6e67  n find_re(string
-00003560: 2c20 7374 7269 6e67 3020 2b20 2728 2e2a  , string0 + '(.*
-00003570: 3f29 2720 2b20 7374 7269 6e67 3129 0a0a  ?)' + string1)..
-00003580: 6465 6620 6973 5f61 7369 616e 5f6e 616d  def is_asian_nam
-00003590: 6528 6e61 6d65 293a 0a20 2020 206e 616d  e(name):.    nam
-000035a0: 6573 203d 206e 616d 652e 7265 706c 6163  es = name.replac
-000035b0: 6528 272d 272c 2027 2027 292e 6c6f 7765  e('-', ' ').lowe
-000035c0: 7228 292e 7370 6c69 7428 2720 2729 0a20  r().split(' '). 
-000035d0: 2020 2072 6574 7572 6e20 286c 656e 286e     return (len(n
-000035e0: 616d 6573 2920 3d3d 2032 2061 6e64 206e  ames) == 2 and n
-000035f0: 6f74 2027 2d27 2069 6e20 6e61 6d65 2061  ot '-' in name a
-00003600: 6e64 2028 0a20 2020 2020 2020 2028 6e61  nd (.        (na
-00003610: 6d65 735b 305d 2069 6e20 4153 4941 4e5f  mes[0] in ASIAN_
-00003620: 4649 5253 545f 4e41 4d45 5320 616e 6420  FIRST_NAMES and 
-00003630: 6e61 6d65 735b 315d 2069 6e20 4153 4941  names[1] in ASIA
-00003640: 4e5f 4c41 5354 5f4e 414d 4553 2920 6f72  N_LAST_NAMES) or
-00003650: 0a20 2020 2020 2020 2028 6e61 6d65 735b  .        (names[
-00003660: 305d 2069 6e20 4153 4941 4e5f 4c41 5354  0] in ASIAN_LAST
-00003670: 5f4e 414d 4553 2061 6e64 206e 616d 6573  _NAMES and names
-00003680: 5b31 5d20 696e 2041 5349 414e 5f46 4952  [1] in ASIAN_FIR
-00003690: 5354 5f4e 414d 4553 290a 2020 2020 2929  ST_NAMES).    ))
-000036a0: 206f 7220 280a 2020 2020 2020 2020 6c65   or (.        le
-000036b0: 6e28 6e61 6d65 7329 203d 3d20 3320 616e  n(names) == 3 an
-000036c0: 6420 6e61 6d65 735b 315d 2069 6e20 4153  d names[1] in AS
-000036d0: 4941 4e5f 4649 5253 545f 4e41 4d45 5320  IAN_FIRST_NAMES 
-000036e0: 616e 6420 280a 2020 2020 2020 2020 2020  and (.          
-000036f0: 2020 6e61 6d65 735b 305d 2069 6e20 4153    names[0] in AS
-00003700: 4941 4e5f 4649 5253 545f 4e41 4d45 5320  IAN_FIRST_NAMES 
-00003710: 6f72 206e 616d 6573 5b32 5d20 696e 2041  or names[2] in A
-00003720: 5349 414e 5f46 4952 5354 5f4e 414d 4553  SIAN_FIRST_NAMES
-00003730: 0a20 2020 2020 2020 2029 0a20 2020 2029  .        ).    )
-00003740: 0a0a 6465 6620 7061 7273 655f 7573 6572  ..def parse_user
-00003750: 6167 656e 7428 7573 6572 6167 656e 7429  agent(useragent)
-00003760: 3a0a 2020 2020 6461 7461 203d 207b 7d0a  :.    data = {}.
-00003770: 2020 2020 666f 7220 6b65 7920 696e 2055      for key in U
-00003780: 415f 5245 4745 5850 533a 0a20 2020 2020  A_REGEXPS:.     
-00003790: 2020 2066 6f72 2061 6c69 6173 2c20 7265     for alias, re
-000037a0: 6765 7870 2069 6e20 5541 5f41 4c49 4153  gexp in UA_ALIAS
-000037b0: 4553 5b6b 6579 5d2e 6974 656d 7328 293a  ES[key].items():
-000037c0: 0a20 2020 2020 2020 2020 2020 2061 6c69  .            ali
-000037d0: 6173 203d 2061 6c69 6173 2069 6620 6b65  as = alias if ke
-000037e0: 7920 3d3d 2027 6272 6f77 7365 7227 2065  y == 'browser' e
-000037f0: 6c73 6520 616c 6961 7320 2b20 2720 5c5c  lse alias + ' \\
-00003800: 3127 0a20 2020 2020 2020 2020 2020 2075  1'.            u
-00003810: 7365 7261 6765 6e74 203d 2072 652e 7375  seragent = re.su
-00003820: 6228 7265 6765 7870 2c20 616c 6961 732c  b(regexp, alias,
-00003830: 2075 7365 7261 6765 6e74 290a 2020 2020   useragent).    
-00003840: 2020 2020 666f 7220 7265 6765 7870 2069      for regexp i
-00003850: 6e20 5541 5f52 4547 4558 5053 5b6b 6579  n UA_REGEXPS[key
-00003860: 5d3a 0a20 2020 2020 2020 2020 2020 2064  ]:.            d
-00003870: 6174 615b 6b65 795d 203d 207b 276e 616d  ata[key] = {'nam
-00003880: 6527 3a20 2727 2c20 2776 6572 7369 6f6e  e': '', 'version
-00003890: 273a 2027 272c 2027 7374 7269 6e67 273a  ': '', 'string':
-000038a0: 2027 277d 0a20 2020 2020 2020 2020 2020   ''}.           
-000038b0: 206d 6174 6368 203d 2072 652e 636f 6d70   match = re.comp
-000038c0: 696c 6528 7265 6765 7870 292e 7365 6172  ile(regexp).sear
-000038d0: 6368 2875 7365 7261 6765 6e74 290a 2020  ch(useragent).  
-000038e0: 2020 2020 2020 2020 2020 6966 206d 6174            if mat
-000038f0: 6368 3a0a 2020 2020 2020 2020 2020 2020  ch:.            
-00003900: 2020 2020 6d61 7463 6865 7320 3d20 6c69      matches = li
-00003910: 7374 286d 6174 6368 2e67 726f 7570 7328  st(match.groups(
-00003920: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00003930: 2020 2069 6620 6c65 6e28 6d61 7463 6865     if len(matche
-00003940: 7329 203d 3d20 313a 0a20 2020 2020 2020  s) == 1:.       
-00003950: 2020 2020 2020 2020 2020 2020 206d 6174               mat
-00003960: 6368 6573 2e61 7070 656e 6428 2727 290a  ches.append('').
+00000040: 706f 7274 2067 7a69 700a 696d 706f 7274  port gzip.import
+00000050: 206d 6174 680a 696d 706f 7274 2072 650a   math.import re.
+00000060: 696d 706f 7274 2075 6e69 636f 6465 6461  import unicodeda
+00000070: 7461 0a66 726f 6d20 696f 2069 6d70 6f72  ta.from io impor
+00000080: 7420 4279 7465 7349 4f0a 0a66 726f 6d20  t BytesIO..from 
+00000090: 6675 6e63 746f 6f6c 7320 696d 706f 7274  functools import
+000000a0: 2072 6564 7563 650a 0a41 5254 4943 4c45   reduce..ARTICLE
+000000b0: 5320 3d20 6c69 7374 2873 6574 285b 0a20  S = list(set([. 
+000000c0: 2020 2023 2064 6566 2073 672c 2064 6566     # def sg, def
+000000d0: 2070 6c2c 2069 6e64 6566 2073 672c 2069   pl, indef sg, i
+000000e0: 6e64 6566 2070 6c20 2865 6163 6820 6d2f  ndef pl (each m/
+000000f0: 662f 6e29 0a20 2020 2027 6465 7227 2c20  f/n).    'der', 
+00000100: 2764 6965 272c 2027 6461 7327 2c20 2765  'die', 'das', 'e
+00000110: 696e 272c 2027 6569 6e65 272c 2020 2320  in', 'eine',  # 
+00000120: 6465 0a20 2020 2027 7468 6527 2c20 2761  de.    'the', 'a
+00000130: 272c 2027 616e 272c 2020 2320 656e 0a20  ', 'an',  # en. 
+00000140: 2020 2027 656c 272c 2027 6c61 272c 2027     'el', 'la', '
+00000150: 6c6f 272c 2027 6c6f 7327 2c20 276c 6173  lo', 'los', 'las
+00000160: 272c 2027 756e 272c 2027 756e 6127 2c20  ', 'un', 'una', 
+00000170: 2775 6e6f 7327 2c20 2775 6e61 7327 2c20  'unos', 'unas', 
+00000180: 2023 2065 730a 2020 2020 276c 6527 2c20   # es.    'le', 
+00000190: 226c 2722 2c20 276c 6127 2c20 276c 6573  "l'", 'la', 'les
+000001a0: 272c 2027 756e 272c 2027 756e 6527 2c20  ', 'un', 'une', 
+000001b0: 2764 6573 272c 2020 2320 6672 0a20 2020  'des',  # fr.   
+000001c0: 2027 696c 272c 2027 6c6f 272c 2022 6c27   'il', 'lo', "l'
+000001d0: 2220 276c 6127 2c20 275f 6927 2c20 2767  " 'la', '_i', 'g
+000001e0: 6c69 272c 2027 6c65 272c 2020 2320 6974  li', 'le',  # it
+000001f0: 0a20 2020 2027 6465 272c 2027 6865 7427  .    'de', 'het'
+00000200: 2c20 2765 656e 272c 2020 2320 6e6c 0a20  , 'een',  # nl. 
+00000210: 2020 2027 6f27 2c20 2761 272c 2027 6f73     'o', 'a', 'os
+00000220: 272c 2027 5f61 7327 2c20 2775 6d27 2c20  ', '_as', 'um', 
+00000230: 2775 6d61 272c 2027 5f75 6e73 272c 2027  'uma', '_uns', '
+00000240: 756d 6173 2720 2023 2070 740a 2020 2020  umas'  # pt.    
+00000250: 2320 736f 6d65 205f 6469 7361 626c 6564  # some _disabled
+00000260: 2062 6563 6175 7365 206f 6620 636f 6c6c   because of coll
+00000270: 6973 696f 6e73 0a5d 2929 0a23 2065 7665  isions.])).# eve
+00000280: 7279 2067 6976 656e 206e 616d 6520 696e  ry given name in
+00000290: 2030 7844 4220 7468 6174 206d 6174 6368   0xDB that match
+000002a0: 6573 2058 7878 782d 7979 7979 204c 6173  es Xxxx-yyyy Las
+000002b0: 746e 616d 650a 4153 4941 4e5f 4649 5253  tname.ASIAN_FIRS
+000002c0: 545f 4e41 4d45 5320 3d20 5b0a 2020 2020  T_NAMES = [.    
+000002d0: 2761 272c 2027 6165 272c 2027 6165 6e67  'a', 'ae', 'aeng
+000002e0: 272c 2027 6168 272c 2027 6169 272c 2027  ', 'ah', 'ai', '
+000002f0: 616e 272c 2027 6261 636b 272c 2027 6261  an', 'back', 'ba
+00000300: 6527 2c20 2762 616e 272c 2027 6261 6e67  e', 'ban', 'bang
+00000310: 272c 2027 6261 6f27 2c20 0a20 2020 2027  ', 'bao', .    '
+00000320: 6265 6f6d 272c 2027 6269 272c 2027 6269  beom', 'bi', 'bi
+00000330: 6e27 2c20 2762 6f27 2c20 2762 6f6b 272c  n', 'bo', 'bok',
+00000340: 2027 626f 6e27 2c20 2762 6f6e 6727 2c20   'bon', 'bong', 
+00000350: 2762 7527 2c20 2762 756d 272c 2027 6279  'bu', 'bum', 'by
+00000360: 656f 6e67 272c 200a 2020 2020 2762 796f  eong', .    'byo
+00000370: 756e 6727 2c20 2762 7975 6e67 272c 2027  ung', 'byung', '
+00000380: 6361 6927 2c20 2763 6861 6527 2c20 2763  cai', 'chae', 'c
+00000390: 6861 6e27 2c20 2763 6861 6e67 272c 2027  han', 'chang', '
+000003a0: 6368 616f 272c 2027 6368 6561 6c27 2c20  chao', 'cheal', 
+000003b0: 2763 6865 6e27 2c20 0a20 2020 2027 6368  'chen', .    'ch
+000003c0: 656e 6727 2c20 2763 6865 6f6c 272c 2027  eng', 'cheol', '
+000003d0: 6368 656f 6e27 2c20 2763 6865 6f6e 6727  cheon', 'cheong'
+000003e0: 2c20 2763 6865 756c 272c 2027 6368 6927  , 'cheul', 'chi'
+000003f0: 2c20 2763 6869 6127 2c20 2763 6869 616f  , 'chia', 'chiao
+00000400: 272c 200a 2020 2020 2763 6869 6568 272c  ', .    'chieh',
+00000410: 2027 6368 6965 6e27 2c20 2763 6869 6827   'chien', 'chih'
+00000420: 2c20 2763 6869 6e27 2c20 2763 6869 6e67  , 'chin', 'ching
+00000430: 272c 2027 6368 6f27 2c20 2763 686f 6927  ', 'cho', 'choi'
+00000440: 2c20 2763 686f 6e67 272c 2027 6368 6f6f  , 'chong', 'choo
+00000450: 272c 200a 2020 2020 2763 6875 272c 2027  ', .    'chu', '
+00000460: 6368 7561 6e27 2c20 2763 6875 656e 272c  chuan', 'chuen',
+00000470: 2027 6368 756c 272c 2027 6368 756e 272c   'chul', 'chun',
+00000480: 2027 6368 756e 6727 2c20 2763 6875 6f27   'chung', 'chuo'
+00000490: 2c20 2763 6879 6927 2c20 2764 6127 2c20  , 'chyi', 'da', 
+000004a0: 0a20 2020 2027 6461 6527 2c20 2764 6168  .    'dae', 'dah
+000004b0: 272c 2027 6461 6c27 2c20 2764 616e 272c  ', 'dal', 'dan',
+000004c0: 2027 6465 6f6b 272c 2027 646f 272c 2027   'deok', 'do', '
+000004d0: 646f 6e67 272c 2027 646f 6f27 2c20 2764  dong', 'doo', 'd
+000004e0: 7565 6b27 2c20 2764 756b 272c 200a 2020  uek', 'duk', .  
+000004f0: 2020 2765 272c 2027 656c 272c 2027 656e    'e', 'el', 'en
+00000500: 272c 2027 6575 6927 2c20 2765 756c 272c  ', 'eui', 'eul',
+00000510: 2027 6575 6e27 2c20 2765 756e 6727 2c20   'eun', 'eung', 
+00000520: 2766 6169 272c 2027 6661 6e27 2c20 2766  'fai', 'fan', 'f
+00000530: 616e 6727 2c20 2766 6569 272c 200a 2020  ang', 'fei', .  
+00000540: 2020 2766 656e 272c 2027 6665 6e67 272c    'fen', 'feng',
+00000550: 2027 666f 272c 2027 666f 6f27 2c20 2766   'fo', 'foo', 'f
+00000560: 7527 2c20 2767 6127 2c20 2767 6165 272c  u', 'ga', 'gae',
+00000570: 2027 6761 6d27 2c20 2767 616e 6727 2c20   'gam', 'gang', 
+00000580: 2767 6527 2c20 2767 656e 272c 200a 2020  'ge', 'gen', .  
+00000590: 2020 2767 656f 6e27 2c20 2767 6575 6e27    'geon', 'geun'
+000005a0: 2c20 2767 6927 2c20 2767 696c 272c 2027  , 'gi', 'gil', '
+000005b0: 6769 6e27 2c20 2767 6e61 6427 2c20 2767  gin', 'gnad', 'g
+000005c0: 6f6b 272c 2027 676f 6f27 2c20 2767 6f6f  ok', 'goo', 'goo
+000005d0: 6b27 2c20 2767 7527 2c20 0a20 2020 2027  k', 'gu', .    '
+000005e0: 6775 6e27 2c20 2767 7761 6e27 2c20 2767  gun', 'gwan', 'g
+000005f0: 7965 272c 2027 6779 656f 6e67 272c 2027  ye', 'gyeong', '
+00000600: 6779 7527 2c20 2767 7975 6e27 2c20 2768  gyu', 'gyun', 'h
+00000610: 6127 2c20 2768 6165 272c 2027 6861 6b27  a', 'hae', 'hak'
+00000620: 2c20 2768 616e 272c 200a 2020 2020 2768  , 'han', .    'h
+00000630: 616e 6727 2c20 2768 616f 272c 2027 6865  ang', 'hao', 'he
+00000640: 272c 2027 6865 6527 2c20 2768 656e 6727  ', 'hee', 'heng'
+00000650: 2c20 2768 656f 6e27 2c20 2768 6965 272c  , 'heon', 'hie',
+00000660: 2027 686f 272c 2027 686f 6927 2c20 2768   'ho', 'hoi', 'h
+00000670: 6f6e 6727 2c20 0a20 2020 2027 686f 6f27  ong', .    'hoo'
+00000680: 2c20 2768 6f6f 6e27 2c20 2768 6f75 272c  , 'hoon', 'hou',
+00000690: 2027 6873 6927 2c20 2768 7369 616e 6727   'hsi', 'hsiang'
+000006a0: 2c20 2768 7369 616f 272c 2027 6873 6965  , 'hsiao', 'hsie
+000006b0: 6827 2c20 2768 7369 656e 272c 2027 6873  h', 'hsien', 'hs
+000006c0: 696e 272c 200a 2020 2020 2768 7369 6e67  in', .    'hsing
+000006d0: 272c 2027 6873 6975 6e67 272c 2027 6875  ', 'hsiung', 'hu
+000006e0: 272c 2027 6875 6127 2c20 2768 7561 6927  ', 'hua', 'huai'
+000006f0: 2c20 2768 7561 6e67 272c 2027 6875 6527  , 'huang', 'hue'
+00000700: 2c20 2768 7569 272c 2027 6875 6e27 2c20  , 'hui', 'hun', 
+00000710: 0a20 2020 2027 6875 6e67 272c 2027 6877  .    'hung', 'hw
+00000720: 6127 2c20 2768 7761 6e27 2c20 2768 7761  a', 'hwan', 'hwa
+00000730: 6e67 272c 2027 6879 6527 2c20 2768 7965  ng', 'hye', 'hye
+00000740: 6f6b 272c 2027 6879 656f 6e27 2c20 2768  ok', 'hyeon', 'h
+00000750: 7965 6f6e 6727 2c20 2768 796f 272c 200a  yeong', 'hyo', .
+00000760: 2020 2020 2768 7975 6b27 2c20 2768 7975      'hyuk', 'hyu
+00000770: 6e27 2c20 2768 7975 6e67 272c 2027 6927  n', 'hyung', 'i'
+00000780: 2c20 2769 6b27 2c20 2769 6c27 2c20 2769  , 'ik', 'il', 'i
+00000790: 6e27 2c20 276a 6127 2c20 276a 6165 272c  n', 'ja', 'jae',
+000007a0: 2027 6a61 6e27 2c20 276a 616e 6727 2c20   'jan', 'jang', 
+000007b0: 0a20 2020 2027 6a65 272c 2027 6a65 6527  .    'je', 'jee'
+000007c0: 2c20 276a 656e 272c 2027 6a65 6f6b 272c  , 'jen', 'jeok',
+000007d0: 2027 6a65 6f6e 6727 2c20 276a 6575 6e67   'jeong', 'jeung
+000007e0: 272c 2027 6a69 272c 2027 6a69 6127 2c20  ', 'ji', 'jia', 
+000007f0: 276a 6961 6e27 2c20 276a 696b 272c 200a  'jian', 'jik', .
+00000800: 2020 2020 276a 696e 272c 2027 6a69 6e67      'jin', 'jing
+00000810: 272c 2027 6a6f 272c 2027 6a6f 6e67 272c  ', 'jo', 'jong',
+00000820: 2027 6a6f 6f27 2c20 276a 6f6f 6e27 2c20   'joo', 'joon', 
+00000830: 276a 7527 2c20 276a 7561 6e27 2c20 276a  'ju', 'juan', 'j
+00000840: 756e 272c 2027 6a75 6e67 272c 200a 2020  un', 'jung', .  
+00000850: 2020 276b 6127 2c20 276b 6169 272c 2027    'ka', 'kai', '
+00000860: 6b61 6d27 2c20 276b 616e 272c 2027 6b61  kam', 'kan', 'ka
+00000870: 6e67 272c 2027 6b61 7027 2c20 276b 6172  ng', 'kap', 'kar
+00000880: 272c 2027 6b65 272c 2027 6b65 6527 2c20  ', 'ke', 'kee', 
+00000890: 276b 6569 272c 200a 2020 2020 276b 656e  'kei', .    'ken
+000008a0: 6727 2c20 276b 6575 6d27 2c20 276b 6575  g', 'keum', 'keu
+000008b0: 6e67 272c 2027 6b69 272c 2027 6b69 6c27  ng', 'ki', 'kil'
+000008c0: 2c20 276b 696e 272c 2027 6b69 7427 2c20  , 'kin', 'kit', 
+000008d0: 276b 6f74 272c 2027 6b75 272c 2027 6b75  'kot', 'ku', 'ku
+000008e0: 6127 2c20 0a20 2020 2027 6b75 616e 272c  a', .    'kuan',
+000008f0: 2027 6b75 616e 6727 2c20 276b 7565 6e27   'kuang', 'kuen'
+00000900: 2c20 276b 756e 272c 2027 6b75 6f27 2c20  , 'kun', 'kuo', 
+00000910: 276b 7761 6e67 272c 2027 6b77 6f6b 272c  'kwang', 'kwok',
+00000920: 2027 6b77 6f6e 272c 2027 6b77 6f6e 6727   'kwon', 'kwong'
+00000930: 2c20 0a20 2020 2027 6b79 656f 6e67 272c  , .    'kyeong',
+00000940: 2027 6b79 6f27 2c20 276b 796f 6f6e 272c   'kyo', 'kyoon',
+00000950: 2027 6b79 6f75 272c 2027 6b79 6f75 6e67   'kyou', 'kyoung
+00000960: 272c 2027 6b79 7527 2c20 276b 7975 6e27  ', 'kyu', 'kyun'
+00000970: 2c20 276b 7975 6e67 272c 2027 6c61 6927  , 'kyung', 'lai'
+00000980: 2c20 0a20 2020 2027 6c61 7527 2c20 276c  , .    'lau', 'l
+00000990: 6565 272c 2027 6c65 6927 2c20 276c 656e  ee', 'lei', 'len
+000009a0: 6727 2c20 276c 6575 6e67 272c 2027 6c69  g', 'leung', 'li
+000009b0: 272c 2027 6c69 616e 6727 2c20 276c 6965  ', 'liang', 'lie
+000009c0: 6e27 2c20 276c 696e 272c 2027 6c69 6e67  n', 'lin', 'ling
+000009d0: 272c 200a 2020 2020 276c 6f63 6b27 2c20  ', .    'lock', 
+000009e0: 276c 6f6e 6727 2c20 276c 756e 272c 2027  'long', 'lun', '
+000009f0: 6c75 6e67 272c 2027 6d61 656e 6727 2c20  lung', 'maeng', 
+00000a00: 276d 616e 272c 2027 6d65 6927 2c20 276d  'man', 'mei', 'm
+00000a10: 6927 2c20 276d 6961 6f27 2c20 276d 696e  i', 'miao', 'min
+00000a20: 272c 200a 2020 2020 276d 696e 6727 2c20  ', .    'ming', 
+00000a30: 276d 6f27 2c20 276d 6f6b 272c 2027 6d6f  'mo', 'mok', 'mo
+00000a40: 6f27 2c20 276d 6f6f 6b27 2c20 276d 6f6f  o', 'mook', 'moo
+00000a50: 6e27 2c20 276d 7527 2c20 276d 756e 272c  n', 'mu', 'mun',
+00000a60: 2027 6d79 656f 6e67 272c 200a 2020 2020   'myeong', .    
+00000a70: 276d 796f 656e 6727 2c20 276d 796f 6e67  'myoeng', 'myong
+00000a80: 272c 2027 6d79 756e 6727 2c20 276e 6127  ', 'myung', 'na'
+00000a90: 2c20 276e 6165 272c 2027 6e61 6927 2c20  , 'nae', 'nai', 
+00000aa0: 276e 616d 272c 2027 6e61 6e27 2c20 276e  'nam', 'nan', 'n
+00000ab0: 6575 6e67 272c 200a 2020 2020 276e 6761  eung', .    'nga
+00000ac0: 7275 272c 2027 6e69 272c 2027 6e6f 272c  ru', 'ni', 'no',
+00000ad0: 2027 6e79 656f 272c 2027 6f68 272c 2027   'nyeo', 'oh', '
+00000ae0: 6f6b 272c 2027 6f75 272c 2027 7061 6927  ok', 'ou', 'pai'
+00000af0: 2c20 2770 6569 272c 2027 7065 6e27 2c20  , 'pei', 'pen', 
+00000b00: 2770 656e 6727 2c20 0a20 2020 2027 7069  'peng', .    'pi
+00000b10: 272c 2027 7069 6c27 2c20 2770 696e 272c  ', 'pil', 'pin',
+00000b20: 2027 7069 6e67 272c 2027 706f 272c 2027   'ping', 'po', '
+00000b30: 7075 6927 2c20 2770 796f 272c 2027 7079  pui', 'pyo', 'py
+00000b40: 756e 6727 2c20 2771 696e 6727 2c20 2771  ung', 'qing', 'q
+00000b50: 756e 272c 200a 2020 2020 2772 6127 2c20  un', .    'ra', 
+00000b60: 2772 616b 272c 2027 7261 6d27 2c20 2772  'rak', 'ram', 'r
+00000b70: 616e 272c 2027 7265 756d 272c 2027 7269  an', 'reum', 'ri
+00000b80: 272c 2027 7269 6d27 2c20 2772 696e 272c  ', 'rim', 'rin',
+00000b90: 2027 726f 6527 2c20 2772 6f6b 272c 2027   'roe', 'rok', '
+00000ba0: 7275 272c 200a 2020 2020 2772 7569 272c  ru', .    'rui',
+00000bb0: 2027 7279 656f 6e27 2c20 2772 796f 6c27   'ryeon', 'ryol'
+00000bc0: 2c20 2772 796f 6e67 272c 2027 7361 272c  , 'ryong', 'sa',
+00000bd0: 2027 7361 6527 2c20 2773 616e 272c 2027   'sae', 'san', '
+00000be0: 7361 6e67 272c 2027 7365 272c 2027 7365  sang', 'se', 'se
+00000bf0: 6f27 2c20 0a20 2020 2027 7365 6f62 272c  o', .    'seob',
+00000c00: 2027 7365 6f6b 272c 2027 7365 6f6c 272c   'seok', 'seol',
+00000c10: 2027 7365 6f6e 272c 2027 7365 6f6e 6727   'seon', 'seong'
+00000c20: 2c20 2773 6575 6e67 272c 2027 7368 616e  , 'seung', 'shan
+00000c30: 272c 2027 7368 656e 272c 2027 7368 656e  ', 'shen', 'shen
+00000c40: 6727 2c20 0a20 2020 2027 7368 6927 2c20  g', .    'shi', 
+00000c50: 2773 6869 6127 2c20 2773 6869 616e 6727  'shia', 'shiang'
+00000c60: 2c20 2773 6869 6827 2c20 2773 6869 6b27  , 'shih', 'shik'
+00000c70: 2c20 2773 6869 6d27 2c20 2773 6869 6e27  , 'shim', 'shin'
+00000c80: 2c20 2773 6869 6e67 272c 2027 7368 6f75  , 'shing', 'shou
+00000c90: 272c 200a 2020 2020 2773 6875 272c 2027  ', .    'shu', '
+00000ca0: 7368 756e 272c 2027 7369 272c 2027 7369  shun', 'si', 'si
+00000cb0: 6b27 2c20 2773 696e 272c 2027 7369 7527  k', 'sin', 'siu'
+00000cc0: 2c20 2773 6f27 2c20 2773 6f6e 6727 2c20  , 'so', 'song', 
+00000cd0: 2773 6f6f 272c 2027 736f 6f6b 272c 200a  'soo', 'sook', .
+00000ce0: 2020 2020 2773 6f6f 6e27 2c20 2773 7527      'soon', 'su'
+00000cf0: 2c20 2773 756b 272c 2027 7375 6e27 2c20  , 'suk', 'sun', 
+00000d00: 2773 756e 6727 2c20 2773 7570 272c 2027  'sung', 'sup', '
+00000d10: 737a 7527 2c20 2274 2769 656e 222c 2027  szu', "t'ien", '
+00000d20: 7461 272c 2027 7461 6527 2c20 0a20 2020  ta', 'tae', .   
+00000d30: 2027 7461 656b 272c 2027 7461 6927 2c20   'taek', 'tai', 
+00000d40: 2774 616b 272c 2027 7465 272c 2027 7469  'tak', 'te', 'ti
+00000d50: 272c 2027 7469 616e 272c 2027 7469 6e67  ', 'tian', 'ting
+00000d60: 272c 2027 746f 272c 2027 746f 6127 2c20  ', 'to', 'toa', 
+00000d70: 2774 7361 6927 2c20 0a20 2020 2027 7473  'tsai', .    'ts
+00000d80: 616e 272c 2027 7473 6527 2c20 2774 736f  an', 'tse', 'tso
+00000d90: 272c 2027 7473 7569 272c 2027 7475 6e67  ', 'tsui', 'tung
+00000da0: 272c 2027 747a 7527 2c20 2775 6127 2c20  ', 'tzu', 'ua', 
+00000db0: 2775 6927 2c20 2775 6e27 2c20 2777 6168  'ui', 'un', 'wah
+00000dc0: 272c 200a 2020 2020 2777 6169 272c 2027  ', .    'wai', '
+00000dd0: 7761 6e27 2c20 2777 6569 272c 2027 7765  wan', 'wei', 'we
+00000de0: 6e27 2c20 2777 656f 6e27 2c20 2777 696e  n', 'weon', 'win
+00000df0: 6727 2c20 2777 6974 272c 2027 776f 6c27  g', 'wit', 'wol'
+00000e00: 2c20 2777 6f6e 272c 2027 776f 6f27 2c20  , 'won', 'woo', 
+00000e10: 0a20 2020 2027 776f 6f6b 272c 2027 776f  .    'wook', 'wo
+00000e20: 6f6e 272c 2027 776f 6f6e 6727 2c20 2777  on', 'woong', 'w
+00000e30: 756b 272c 2027 7869 616f 272c 2027 7961  uk', 'xiao', 'ya
+00000e40: 272c 2027 7961 6e27 2c20 2779 616e 6727  ', 'yan', 'yang'
+00000e50: 2c20 2779 616f 272c 2027 7965 272c 200a  , 'yao', 'ye', .
+00000e60: 2020 2020 2779 6561 272c 2027 7965 6527      'yea', 'yee'
+00000e70: 2c20 2779 6568 272c 2027 7965 6e27 2c20  , 'yeh', 'yen', 
+00000e80: 2779 656f 272c 2027 7965 6f6c 272c 2027  'yeo', 'yeol', '
+00000e90: 7965 6f6e 272c 2027 7965 6f6e 6727 2c20  yeon', 'yeong', 
+00000ea0: 2779 656f 7027 2c20 2779 6927 2c20 0a20  'yeop', 'yi', . 
+00000eb0: 2020 2027 7969 6e27 2c20 2779 696e 6727     'yin', 'ying'
+00000ec0: 2c20 2779 6975 272c 2027 796f 656e 6727  , 'yiu', 'yoeng'
+00000ed0: 2c20 2779 6f6e 6727 2c20 2779 6f6f 272c  , 'yong', 'yoo',
+00000ee0: 2027 796f 6f6e 272c 2027 796f 7527 2c20   'yoon', 'you', 
+00000ef0: 2779 6f75 6e67 272c 2027 7975 272c 200a  'young', 'yu', .
+00000f00: 2020 2020 2779 7561 6e27 2c20 2779 7565      'yuan', 'yue
+00000f10: 272c 2027 7975 656e 272c 2027 7975 6b27  ', 'yuen', 'yuk'
+00000f20: 2c20 2779 756c 6c27 2c20 2779 756e 272c  , 'yull', 'yun',
+00000f30: 2027 7975 6e65 272c 2027 7975 6e67 272c   'yune', 'yung',
+00000f40: 2027 7a68 6927 2c20 0a20 2020 2027 7a68   'zhi', .    'zh
+00000f50: 6f6e 6727 2c20 277a 6875 270a 5d0a 2320  ong', 'zhu'.].# 
+00000f60: 7365 6520 6874 7470 3a2f 2f65 6e2e 7769  see http://en.wi
+00000f70: 6b69 7065 6469 612e 6f72 672f 7769 6b69  kipedia.org/wiki
+00000f80: 2f4c 6973 745f 6f66 5f63 6f6d 6d6f 6e5f  /List_of_common_
+00000f90: 4368 696e 6573 655f 7375 726e 616d 6573  Chinese_surnames
+00000fa0: 0a23 2061 6e64 2068 7474 703a 2f2f 656e  .# and http://en
+00000fb0: 2e77 696b 6970 6564 6961 2e6f 7267 2f77  .wikipedia.org/w
+00000fc0: 696b 692f 4c69 7374 5f6f 665f 4b6f 7265  iki/List_of_Kore
+00000fd0: 616e 5f66 616d 696c 795f 6e61 6d65 730a  an_family_names.
+00000fe0: 4153 4941 4e5f 4c41 5354 5f4e 414d 4553  ASIAN_LAST_NAMES
+00000ff0: 203d 205b 0a20 2020 2027 6368 616e 272c   = [.    'chan',
+00001000: 2027 6368 616e 6727 2c20 2763 6861 6f27   'chang', 'chao'
+00001010: 2c0a 2020 2020 2763 6865 6e27 2c20 2763  ,.    'chen', 'c
+00001020: 6865 6f6e 6727 2c20 2763 6865 756e 6727  heong', 'cheung'
+00001030: 2c0a 2020 2020 2763 686f 6e67 272c 2027  ,.    'chong', '
+00001040: 6368 6f6f 272c 0a20 2020 2027 6368 7527  choo',.    'chu'
+00001050: 2c20 2763 6875 6e27 2c0a 2020 2020 2768  , 'chun',.    'h
+00001060: 6f75 272c 2027 6873 6965 6827 2c20 2768  ou', 'hsieh', 'h
+00001070: 7375 272c 2027 6875 272c 2027 6875 616e  su', 'hu', 'huan
+00001080: 6727 2c0a 2020 2020 276b 756f 272c 0a20  g',.    'kuo',. 
+00001090: 2020 2027 6c69 272c 2027 6c69 616e 6727     'li', 'liang'
+000010a0: 2c20 276c 696e 272c 2027 6c69 7527 2c0a  , 'lin', 'liu',.
+000010b0: 2020 2020 275f 7061 726b 272c 0a20 2020      '_park',.   
+000010c0: 2027 7375 6e27 2c20 2773 756e 6727 2c0a   'sun', 'sung',.
+000010d0: 2020 2020 2774 7361 6f27 2c0a 2020 2020      'tsao',.    
+000010e0: 2777 616e 6727 2c20 2757 6f6e 6727 2c0a  'wang', 'Wong',.
+000010f0: 2020 2020 2779 616e 6727 2c20 2779 656f      'yang', 'yeo
+00001100: 6e67 272c 2027 7965 756e 6727 0a5d 0a50  ng', 'yeung'.].P
+00001110: 5245 4649 5845 5320 3d20 5b0a 2020 2020  REFIXES = [.    
+00001120: 2761 6c27 2c20 2762 696e 272c 2027 6461  'al', 'bin', 'da
+00001130: 272c 2027 6465 272c 2027 6465 6c27 2c20  ', 'de', 'del', 
+00001140: 2764 656d 272c 2027 6465 6e27 2c20 2764  'dem', 'den', 'd
+00001150: 6572 272c 2027 6469 272c 2027 646f 7327  er', 'di', 'dos'
+00001160: 2c20 2764 7527 2c0a 2020 2020 2765 272c  , 'du',.    'e',
+00001170: 2027 656c 272c 2027 6c61 272c 2027 7361   'el', 'la', 'sa
+00001180: 6e27 2c20 2774 6865 272c 2027 7661 6e27  n', 'the', 'van'
+00001190: 2c20 2776 6f6d 272c 2027 766f 6e27 2c20  , 'vom', 'von', 
+000011a0: 2779 272c 2027 7a75 270a 5d0a 4d49 4446  'y', 'zu'.].MIDF
+000011b0: 4958 4553 203d 205b 2775 6e64 275d 0a53  IXES = ['und'].S
+000011c0: 5546 4649 5845 5320 3d20 5b27 6969 272c  UFFIXES = ['ii',
+000011d0: 2027 6969 6927 2c20 276a 7227 2c20 276a   'iii', 'jr', 'j
+000011e0: 722e 272c 2027 7068 2e64 2e27 2c20 2770  r.', 'ph.d.', 'p
+000011f0: 6864 272c 2027 7372 272c 2027 7372 2e27  hd', 'sr', 'sr.'
+00001200: 5d0a 0a55 415f 414c 4941 5345 5320 3d20  ]..UA_ALIASES = 
+00001210: 7b0a 2020 2020 2762 726f 7773 6572 273a  {.    'browser':
+00001220: 207b 0a20 2020 2020 2020 2027 4368 726f   {.        'Chro
+00001230: 6d65 273a 2027 2843 7269 4f53 7c43 724d  me': '(CriOS|CrM
+00001240: 6f29 272c 0a20 2020 2020 2020 2027 4669  o)',.        'Fi
+00001250: 7265 666f 7827 3a20 2728 4665 6e6e 6563  refox': '(Fennec
+00001260: 7c46 6972 6562 6972 647c 4963 6577 6561  |Firebird|Icewea
+00001270: 7365 6c7c 4d69 6e65 6669 656c 647c 4e61  sel|Minefield|Na
+00001280: 6d6f 726f 6b61 7c50 686f 656e 6978 7c53  moroka|Phoenix|S
+00001290: 6561 4d6f 6e6b 6579 7c53 6869 7265 746f  eaMonkey|Shireto
+000012a0: 6b6f 2927 2c0a 2020 2020 2020 2020 274e  ko)',.        'N
+000012b0: 6f6b 6961 2042 726f 7773 6572 273a 2027  okia Browser': '
+000012c0: 284f 7669 4272 6f77 7365 7229 270a 2020  (OviBrowser)'.  
+000012d0: 2020 7d2c 0a20 2020 2027 726f 626f 7427    },.    'robot'
+000012e0: 3a20 7b7d 2c0a 2020 2020 2773 7973 7465  : {},.    'syste
+000012f0: 6d27 3a20 7b0a 2020 2020 2020 2020 2742  m': {.        'B
+00001300: 5344 273a 2027 2846 7265 6542 5344 7c4e  SD': '(FreeBSD|N
+00001310: 6574 4253 447c 4f70 656e 4253 4429 272c  etBSD|OpenBSD)',
+00001320: 0a20 2020 2020 2020 2027 4c69 6e75 7827  .        'Linux'
+00001330: 3a20 2728 4372 4f53 7c4d 6565 476f 7c77  : '(CrOS|MeeGo|w
+00001340: 6562 4f53 2927 2c0a 2020 2020 2020 2020  ebOS)',.        
+00001350: 2755 6e69 7827 3a20 2728 4149 587c 4850  'Unix': '(AIX|HP
+00001360: 2d55 587c 4952 4958 7c53 756e 4f53 2927  -UX|IRIX|SunOS)'
+00001370: 0a20 2020 207d 0a7d 0a55 415f 4e41 4d45  .    }.}.UA_NAME
+00001380: 5320 3d20 7b0a 2020 2020 2762 726f 7773  S = {.    'brows
+00001390: 6572 273a 207b 0a20 2020 2020 2020 2027  er': {.        '
+000013a0: 6368 726f 6d65 6672 616d 6527 3a20 2743  chromeframe': 'C
+000013b0: 6872 6f6d 6520 4672 616d 6527 2c0a 2020  hrome Frame',.  
+000013c0: 2020 2020 2020 2746 4246 6f72 4950 686f        'FBForIPho
+000013d0: 6e65 273a 2027 5765 624b 6974 272c 0a20  ne': 'WebKit',. 
+000013e0: 2020 2020 2020 2027 4765 636b 6f27 3a20         'Gecko': 
+000013f0: 274d 6f7a 696c 6c61 272c 0a20 2020 2020  'Mozilla',.     
+00001400: 2020 2027 4945 4d6f 6269 6c65 273a 2027     'IEMobile': '
+00001410: 496e 7465 726e 6574 2045 7870 6c6f 7265  Internet Explore
+00001420: 7227 2c0a 2020 2020 2020 2020 276b 6f6e  r',.        'kon
+00001430: 7175 6572 6f72 273a 2027 4b6f 6e71 7565  queror': 'Konque
+00001440: 726f 7227 2c0a 2020 2020 2020 2020 274d  ror',.        'M
+00001450: 6f7a 696c 6c61 273a 2027 4e65 7473 6361  ozilla': 'Netsca
+00001460: 7065 272c 0a20 2020 2020 2020 2027 4d53  pe',.        'MS
+00001470: 4945 273a 2027 496e 7465 726e 6574 2045  IE': 'Internet E
+00001480: 7870 6c6f 7265 7227 2c0a 2020 2020 2020  xplorer',.      
+00001490: 2020 274e 6f6b 6961 4272 6f77 7365 7227    'NokiaBrowser'
+000014a0: 3a20 274e 6f6b 6961 2042 726f 7773 6572  : 'Nokia Browser
+000014b0: 272c 0a20 2020 2020 2020 2027 5472 6964  ',.        'Trid
+000014c0: 656e 7427 3a20 2749 6e74 6572 6e65 7420  ent': 'Internet 
+000014d0: 4578 706c 6f72 6572 270a 2020 2020 7d2c  Explorer'.    },
+000014e0: 0a20 2020 2027 726f 626f 7427 3a20 7b7d  .    'robot': {}
+000014f0: 2c0a 2020 2020 2773 7973 7465 6d27 3a20  ,.    'system': 
+00001500: 7b0a 2020 2020 2020 2020 2742 4227 3a20  {.        'BB': 
+00001510: 2742 6c61 636b 4265 7272 7927 2c0a 2020  'BlackBerry',.  
+00001520: 2020 2020 2020 2743 5055 204f 5327 3a20        'CPU OS': 
+00001530: 2769 4f53 272c 0a20 2020 2020 2020 2027  'iOS',.        '
+00001540: 6950 686f 6e65 273a 2027 694f 5327 2c0a  iPhone': 'iOS',.
+00001550: 2020 2020 2020 2020 2769 5068 6f6e 6520          'iPhone 
+00001560: 4f53 273a 2027 694f 5327 2c0a 2020 2020  OS': 'iOS',.    
+00001570: 2020 2020 274a 324d 452f 4d49 4450 273a      'J2ME/MIDP':
+00001580: 2027 4a61 7661 272c 0a20 2020 2020 2020   'Java',.       
+00001590: 2027 4d61 635f 506f 7765 7250 4327 3a20   'Mac_PowerPC': 
+000015a0: 274d 6163 204f 5327 2c0a 2020 2020 2020  'Mac OS',.      
+000015b0: 2020 274d 6163 5f50 5043 273a 2027 4d61    'Mac_PPC': 'Ma
+000015c0: 6320 4f53 272c 0a20 2020 2020 2020 2027  c OS',.        '
+000015d0: 4d61 6369 6e74 6f73 6827 3a20 274d 6163  Macintosh': 'Mac
+000015e0: 204f 5327 2c0a 2020 2020 2020 2020 2750   OS',.        'P
+000015f0: 4c41 5953 5441 5449 4f4e 273a 2027 506c  LAYSTATION': 'Pl
+00001600: 6179 5374 6174 696f 6e27 2c0a 2020 2020  ayStation',.    
+00001610: 2020 2020 2753 273a 2027 4e6f 6b69 6127      'S': 'Nokia'
+00001620: 2c0a 2020 2020 2020 2020 2753 6572 6965  ,.        'Serie
+00001630: 7327 3a20 274e 6f6b 6961 272c 0a20 2020  s': 'Nokia',.   
+00001640: 2020 2020 2027 5769 6e27 3a20 2757 696e       'Win': 'Win
+00001650: 646f 7773 272c 0a20 2020 2020 2020 2027  dows',.        '
+00001660: 5769 6e64 6f77 7320 5068 6f6e 6520 4f53  Windows Phone OS
+00001670: 273a 2027 5769 6e64 6f77 7320 5068 6f6e  ': 'Windows Phon
+00001680: 6527 2c0a 2020 2020 2020 2020 2758 3131  e',.        'X11
+00001690: 273a 2027 4c69 6e75 7827 0a20 2020 207d  ': 'Linux'.    }
+000016a0: 0a7d 0a55 415f 5245 4745 5850 5320 3d20  .}.UA_REGEXPS = 
+000016b0: 7b0a 2020 2020 2762 726f 7773 6572 273a  {.    'browser':
+000016c0: 205b 0a20 2020 2020 2020 2027 2843 616d   [.        '(Cam
+000016d0: 696e 6f29 5c2f 285c 642b 2927 2c0a 2020  ino)\/(\d+)',.  
+000016e0: 2020 2020 2020 2728 4368 696d 6572 6129        '(Chimera)
+000016f0: 5c2f 285c 642b 2927 2c0a 2020 2020 2020  \/(\d+)',.      
+00001700: 2020 2728 6368 726f 6d65 6672 616d 6529    '(chromeframe)
+00001710: 5c2f 285c 642b 2927 2c0a 2020 2020 2020  \/(\d+)',.      
+00001720: 2020 2728 4564 6765 295c 2f28 5c64 2b29    '(Edge)\/(\d+)
+00001730: 272c 0a20 2020 2020 2020 2027 2845 7069  ',.        '(Epi
+00001740: 7068 616e 7929 5c2f 285c 642b 2927 2c20  phany)\/(\d+)', 
+00001750: 2023 2062 6566 6f72 6520 4368 726f 6d65   # before Chrome
+00001760: 2c20 4368 726f 6d69 756d 2061 6e64 2053  , Chromium and S
+00001770: 6166 6172 690a 2020 2020 2020 2020 2728  afari.        '(
+00001780: 4368 726f 6d69 756d 295c 2f28 5c64 2b29  Chromium)\/(\d+)
+00001790: 272c 2020 2320 6265 666f 7265 2043 6872  ',  # before Chr
+000017a0: 6f6d 650a 2020 2020 2020 2020 2728 4368  ome.        '(Ch
+000017b0: 726f 6d65 295c 2f28 5c64 2b29 272c 0a20  rome)\/(\d+)',. 
+000017c0: 2020 2020 2020 2027 2846 4246 6f72 4950         '(FBForIP
+000017d0: 686f 6e65 2927 2c0a 2020 2020 2020 2020  hone)',.        
+000017e0: 2728 4669 7265 666f 7829 5c2f 285c 642b  '(Firefox)\/(\d+
+000017f0: 2927 2c0a 2020 2020 2020 2020 2728 4761  )',.        '(Ga
+00001800: 6c65 6f6e 295c 2f28 5c64 2b29 272c 0a20  leon)\/(\d+)',. 
+00001810: 2020 2020 2020 2027 2849 454d 6f62 696c         '(IEMobil
+00001820: 6529 5c2f 285c 642b 2927 2c0a 2020 2020  e)\/(\d+)',.    
+00001830: 2020 2020 2728 6943 6162 2920 285c 642b      '(iCab) (\d+
+00001840: 2927 2c0a 2020 2020 2020 2020 2728 6943  )',.        '(iC
+00001850: 6162 295c 2f28 5c64 2b29 272c 0a20 2020  ab)\/(\d+)',.   
+00001860: 2020 2020 2027 286b 6f6e 7175 6572 6f72       '(konqueror
+00001870: 295c 2f28 5c64 2b29 272c 0a20 2020 2020  )\/(\d+)',.     
+00001880: 2020 2027 284b 6f6e 7175 6572 6f72 295c     '(Konqueror)\
+00001890: 2f28 5c64 2b29 272c 0a20 2020 2020 2020  /(\d+)',.       
+000018a0: 2027 284c 796e 7829 5c2f 285c 642b 2927   '(Lynx)\/(\d+)'
+000018b0: 2c0a 2020 2020 2020 2020 2728 4e65 7473  ,.        '(Nets
+000018c0: 6361 7065 295c 643f 5c2f 285c 642b 2927  cape)\d?\/(\d+)'
+000018d0: 2c0a 2020 2020 2020 2020 2728 4e6f 6b69  ,.        '(Noki
+000018e0: 6142 726f 7773 6572 295c 2f28 5c64 2b29  aBrowser)\/(\d+)
+000018f0: 272c 0a20 2020 2020 2020 2027 284f 6d6e  ',.        '(Omn
+00001900: 6957 6562 295c 2f28 5c64 2b29 272c 0a20  iWeb)\/(\d+)',. 
+00001910: 2020 2020 2020 2027 284f 7065 7261 295c         '(Opera)\
+00001920: 2f2e 2b56 6572 7369 6f6e 5c2f 285c 642b  /.+Version\/(\d+
+00001930: 2927 2c0a 2020 2020 2020 2020 2728 4f76  )',.        '(Ov
+00001940: 6942 726f 7773 6572 295c 2f28 5c64 2b29  iBrowser)\/(\d+)
+00001950: 272c 0a20 2020 2020 2020 2027 5665 7273  ',.        'Vers
+00001960: 696f 6e5c 2f28 5c64 2b29 2e2b 2853 6166  ion\/(\d+).+(Saf
+00001970: 6172 6929 272c 0a20 2020 2020 2020 2027  ari)',.        '
+00001980: 2857 6562 4b69 7429 5c2f 285c 642b 2927  (WebKit)\/(\d+)'
+00001990: 2c0a 2020 2020 2020 2020 2728 4d53 4945  ,.        '(MSIE
+000019a0: 2920 285c 645c 643f 283f 215c 6429 2927  ) (\d\d?(?!\d))'
+000019b0: 2c20 2023 206c 6173 742c 2073 696e 6365  ,  # last, since
+000019c0: 204f 7065 7261 2075 7365 6420 746f 206d   Opera used to m
+000019d0: 6173 6b20 6173 204d 5349 450a 2020 2020  ask as MSIE.    
+000019e0: 2020 2020 2728 5472 6964 656e 7429 5c2f      '(Trident)\/
+000019f0: 2e2a 3f72 763a 285c 642b 2927 2c0a 2020  .*?rv:(\d+)',.  
+00001a00: 2020 2020 2020 2728 4765 636b 6f29 272c        '(Gecko)',
+00001a10: 0a20 2020 2020 2020 2027 284d 6f7a 696c  .        '(Mozil
+00001a20: 6c61 295c 2f28 337c 3429 270a 2020 2020  la)\/(3|4)'.    
+00001a30: 5d2c 0a20 2020 2027 726f 626f 7427 3a20  ],.    'robot': 
+00001a40: 5b0a 2020 2020 2020 2020 2728 4269 6e67  [.        '(Bing
+00001a50: 5072 6576 6965 7729 5c2f 285c 642b 2927  Preview)\/(\d+)'
+00001a60: 2c0a 2020 2020 2020 2020 2728 476f 6f67  ,.        '(Goog
+00001a70: 6c65 2057 6562 2050 7265 7669 6577 292e  le Web Preview).
+00001a80: 2b43 6872 6f6d 655c 2f28 5c64 2b29 272c  +Chrome\/(\d+)',
+00001a90: 0a20 2020 2020 2020 2027 2847 6f6f 676c  .        '(Googl
+00001aa0: 6562 6f74 295c 2f28 5c64 2b29 272c 0a20  ebot)\/(\d+)',. 
+00001ab0: 2020 2020 2020 2027 2857 6562 4372 6177         '(WebCraw
+00001ac0: 6c65 7229 5c2f 285c 642b 2927 2c0a 2020  ler)\/(\d+)',.  
+00001ad0: 2020 2020 2020 2728 5961 686f 6f21 2053        '(Yahoo! S
+00001ae0: 6c75 7270 295c 2f28 5c64 2b29 272c 0a20  lurp)\/(\d+)',. 
+00001af0: 2020 2020 2020 2027 2859 616e 6465 7842         '(YandexB
+00001b00: 6f74 295c 2f28 5b5c 645c 2e5d 2b29 272c  ot)\/([\d\.]+)',
+00001b10: 0a20 2020 2020 2020 2027 2859 616e 6465  .        '(Yande
+00001b20: 784d 6f62 696c 6542 6f74 295c 2f28 5b5c  xMobileBot)\/([\
+00001b30: 645c 2e5d 2b29 272c 0a20 2020 205d 2c0a  d\.]+)',.    ],.
+00001b40: 2020 2020 2773 7973 7465 6d27 3a20 5b0a      'system': [.
+00001b50: 2020 2020 2020 2020 2728 416e 6472 6f69          '(Androi
+00001b60: 6429 2028 5c64 2b29 272c 0a20 2020 2020  d) (\d+)',.     
+00001b70: 2020 2027 2841 6e64 726f 6964 2927 2c0a     '(Android)',.
+00001b80: 2020 2020 2020 2020 2728 4242 2928 5c64          '(BB)(\d
+00001b90: 2b29 272c 0a20 2020 2020 2020 2027 2842  +)',.        '(B
+00001ba0: 654f 5329 272c 0a20 2020 2020 2020 2027  eOS)',.        '
+00001bb0: 2842 6c61 636b 4265 7272 7929 2028 5c64  (BlackBerry) (\d
+00001bc0: 2b29 272c 0a20 2020 2020 2020 2027 2842  +)',.        '(B
+00001bd0: 6c61 636b 4265 7272 7929 272c 0a20 2020  lackBerry)',.   
+00001be0: 2020 2020 2027 2844 6172 7769 6e29 272c       '(Darwin)',
+00001bf0: 0a20 2020 2020 2020 2027 2842 5344 2920  .        '(BSD) 
+00001c00: 2846 7265 6542 5344 7c4e 6574 4253 447c  (FreeBSD|NetBSD|
+00001c10: 4f70 656e 4253 4429 272c 0a20 2020 2020  OpenBSD)',.     
+00001c20: 2020 2027 2843 5055 204f 5329 2028 5c64     '(CPU OS) (\d
+00001c30: 2b29 272c 0a20 2020 2020 2020 2027 2869  +)',.        '(i
+00001c40: 5068 6f6e 6520 4f53 2920 285c 642b 2927  Phone OS) (\d+)'
+00001c50: 2c0a 2020 2020 2020 2020 2728 6950 686f  ,.        '(iPho
+00001c60: 6e65 2927 2c20 2023 204f 7065 7261 0a20  ne)',  # Opera. 
+00001c70: 2020 2020 2020 2027 284a 324d 455c 2f4d         '(J2ME\/M
+00001c80: 4944 5029 272c 0a20 2020 2020 2020 2027  IDP)',.        '
+00001c90: 284c 696e 7578 292e 2b28 4365 6e74 4f53  (Linux).+(CentOS
+00001ca0: 7c43 724f 537c 4465 6269 616e 7c46 6564  |CrOS|Debian|Fed
+00001cb0: 6f72 617c 4765 6e74 6f6f 7c4d 616e 6472  ora|Gentoo|Mandr
+00001cc0: 6976 617c 4d65 6547 6f7c 4d69 6e74 7c52  iva|MeeGo|Mint|R
+00001cd0: 6564 2048 6174 7c53 5553 457c 5562 756e  ed Hat|SUSE|Ubun
+00001ce0: 7475 7c77 6562 4f53 2927 2c0a 2020 2020  tu|webOS)',.    
+00001cf0: 2020 2020 2728 4365 6e74 4f53 7c43 724f      '(CentOS|CrO
+00001d00: 537c 4465 6269 616e 7c46 6564 6f72 617c  S|Debian|Fedora|
+00001d10: 4765 6e74 6f6f 7c4d 616e 6472 6976 617c  Gentoo|Mandriva|
+00001d20: 4d65 6547 6f7c 4d69 6e74 7c52 6564 2048  MeeGo|Mint|Red H
+00001d30: 6174 7c53 5553 457c 5562 756e 7475 7c77  at|SUSE|Ubuntu|w
+00001d40: 6562 4f53 292e 2b28 4c69 6e75 7829 272c  ebOS).+(Linux)',
+00001d50: 0a20 2020 2020 2020 2027 284c 696e 7578  .        '(Linux
+00001d60: 2927 2c0a 2020 2020 2020 2020 2728 4d61  )',.        '(Ma
+00001d70: 6320 4f53 2058 2920 2831 302e 5c64 2b29  c OS X) (10.\d+)
+00001d80: 272c 0a20 2020 2020 2020 2027 284d 6163  ',.        '(Mac
+00001d90: 204f 5320 5829 272c 0a20 2020 2020 2020   OS X)',.       
+00001da0: 2027 284d 6163 5f50 6f77 6572 5043 2927   '(Mac_PowerPC)'
+00001db0: 2c0a 2020 2020 2020 2020 2728 4d61 635f  ,.        '(Mac_
+00001dc0: 5050 4329 272c 0a20 2020 2020 2020 2027  PPC)',.        '
+00001dd0: 284d 6163 696e 746f 7368 2927 2c0a 2020  (Macintosh)',.  
+00001de0: 2020 2020 2020 274e 696e 7465 6e64 6f20        'Nintendo 
+00001df0: 2857 6969 292e 2b4e 585c 2f28 5c64 2b29  (Wii).+NX\/(\d+)
+00001e00: 272c 0a20 2020 2020 2020 2027 2850 4c41  ',.        '(PLA
+00001e10: 5953 5441 5449 4f4e 2920 285c 642b 2927  YSTATION) (\d+)'
+00001e20: 2c0a 2020 2020 2020 2020 2728 506c 6179  ,.        '(Play
+00001e30: 5374 6174 696f 6e29 2056 6974 6120 285c  Station) Vita (\
+00001e40: 642b 2927 2c0a 2020 2020 2020 2020 2728  d+)',.        '(
+00001e50: 5249 4d20 5461 626c 6574 204f 5329 2028  RIM Tablet OS) (
+00001e60: 5c64 2b29 272c 0a20 2020 2020 2020 2027  \d+)',.        '
+00001e70: 2853 2928 3630 293b 272c 0a20 2020 2020  (S)(60);',.     
+00001e80: 2020 2027 2853 6572 6965 7329 203f 2834     '(Series) ?(4
+00001e90: 307c 3630 2927 2c0a 2020 2020 2020 2020  0|60)',.        
+00001ea0: 2728 5379 6d62 6961 6e20 4f53 2927 2c0a  '(Symbian OS)',.
+00001eb0: 2020 2020 2020 2020 2728 5379 6d62 6961          '(Symbia
+00001ec0: 6e4f 5329 5c2f 285c 642b 2927 2c0a 2020  nOS)\/(\d+)',.  
+00001ed0: 2020 2020 2020 2728 5379 6d62 4f53 2927        '(SymbOS)'
+00001ee0: 2c0a 2020 2020 2020 2020 2728 4f53 5c2f  ,.        '(OS\/
+00001ef0: 3229 272c 0a20 2020 2020 2020 2027 2855  2)',.        '(U
+00001f00: 6e69 7829 2028 4149 587c 4850 2d55 587c  nix) (AIX|HP-UX|
+00001f10: 4952 4958 7c53 756e 4f53 2927 2c0a 2020  IRIX|SunOS)',.  
+00001f20: 2020 2020 2020 2728 556e 6978 2927 2c0a        '(Unix)',.
+00001f30: 2020 2020 2020 2020 2728 5769 6e64 6f77          '(Window
+00001f40: 7329 2028 4e54 205c 645c 2e5c 6429 272c  s) (NT \d\.\d)',
+00001f50: 0a20 2020 2020 2020 2027 2857 696e 646f  .        '(Windo
+00001f60: 7773 2050 686f 6e65 2920 285c 642b 2927  ws Phone) (\d+)'
+00001f70: 2c0a 2020 2020 2020 2020 2728 5769 6e64  ,.        '(Wind
+00001f80: 6f77 7320 5068 6f6e 6520 4f53 2920 285c  ows Phone OS) (\
+00001f90: 642b 2927 2c0a 2020 2020 2020 2020 2728  d+)',.        '(
+00001fa0: 5769 6e64 6f77 7329 2028 335c 2e31 7c39  Windows) (3\.1|9
+00001fb0: 357c 3938 7c32 3030 307c 3230 3033 7c43  5|98|2000|2003|C
+00001fc0: 457c 4d45 7c4d 6f62 696c 657c 4e54 7c58  E|ME|Mobile|NT|X
+00001fd0: 5029 272c 2020 2320 4f70 6572 610a 2020  P)',  # Opera.  
+00001fe0: 2020 2020 2020 2728 5769 6e29 2028 3978        '(Win) (9x
+00001ff0: 2034 5c2e 3930 2927 2c20 2023 2046 6972   4\.90)',  # Fir
+00002000: 6566 6f78 0a20 2020 2020 2020 2027 2857  efox.        '(W
+00002010: 696e 2928 3136 2927 2c20 2023 2046 6972  in)(16)',  # Fir
+00002020: 6566 6f78 0a20 2020 2020 2020 2027 2857  efox.        '(W
+00002030: 696e 2928 395c 6429 272c 2020 2320 4669  in)(9\d)',  # Fi
+00002040: 7265 666f 780a 2020 2020 2020 2020 2728  refox.        '(
+00002050: 5769 6e29 284e 5429 272c 2020 2320 4669  Win)(NT)',  # Fi
+00002060: 7265 666f 780a 2020 2020 2020 2020 2728  refox.        '(
+00002070: 5769 6e29 284e 5434 5c2e 3029 272c 2020  Win)(NT4\.0)',  
+00002080: 2320 4669 7265 666f 780a 2020 2020 2020  # Firefox.      
+00002090: 2020 2728 5831 3129 270a 2020 2020 5d0a    '(X11)'.    ].
+000020a0: 7d0a 5541 5f56 4552 5349 4f4e 5320 3d20  }.UA_VERSIONS = 
+000020b0: 7b0a 2020 2020 2762 726f 7773 6572 273a  {.    'browser':
+000020c0: 207b 7d2c 0a20 2020 2027 726f 626f 7427   {},.    'robot'
+000020d0: 3a20 7b7d 2c0a 2020 2020 2773 7973 7465  : {},.    'syste
+000020e0: 6d27 3a20 7b0a 2020 2020 2020 2020 2731  m': {.        '1
+000020f0: 302e 3027 3a20 2731 302e 3020 2843 6865  0.0': '10.0 (Che
+00002100: 6574 6168 2927 2c0a 2020 2020 2020 2020  etah)',.        
+00002110: 2731 302e 3127 3a20 2731 302e 3120 2850  '10.1': '10.1 (P
+00002120: 756d 6129 272c 0a20 2020 2020 2020 2027  uma)',.        '
+00002130: 3130 2e32 273a 2027 3130 2e32 2028 4a61  10.2': '10.2 (Ja
+00002140: 6775 6172 2927 2c0a 2020 2020 2020 2020  guar)',.        
+00002150: 2731 302e 3327 3a20 2731 302e 3320 2850  '10.3': '10.3 (P
+00002160: 616e 7468 6572 2927 2c0a 2020 2020 2020  anther)',.      
+00002170: 2020 2731 302e 3427 3a20 2731 302e 3420    '10.4': '10.4 
+00002180: 2854 6967 6572 2927 2c0a 2020 2020 2020  (Tiger)',.      
+00002190: 2020 2731 302e 3527 3a20 2731 302e 3520    '10.5': '10.5 
+000021a0: 284c 656f 7061 7264 2927 2c0a 2020 2020  (Leopard)',.    
+000021b0: 2020 2020 2731 302e 3627 3a20 2731 302e      '10.6': '10.
+000021c0: 3620 2853 6e6f 7720 4c65 6f70 6172 6429  6 (Snow Leopard)
+000021d0: 272c 0a20 2020 2020 2020 2027 3130 2e37  ',.        '10.7
+000021e0: 273a 2027 3130 2e37 2028 4c69 6f6e 2927  ': '10.7 (Lion)'
+000021f0: 2c0a 2020 2020 2020 2020 2731 302e 3827  ,.        '10.8'
+00002200: 3a20 2731 302e 3820 284d 6f75 6e74 6169  : '10.8 (Mountai
+00002210: 6e20 4c69 6f6e 2927 2c0a 2020 2020 2020  n Lion)',.      
+00002220: 2020 2731 302e 3927 3a20 2731 302e 3920    '10.9': '10.9 
+00002230: 284d 6176 6572 6963 6b73 2927 2c0a 2020  (Mavericks)',.  
+00002240: 2020 2020 2020 2731 302e 3130 273a 2027        '10.10': '
+00002250: 3130 2e31 3020 2859 6f73 656d 6974 6529  10.10 (Yosemite)
+00002260: 272c 0a20 2020 2020 2020 2027 3130 2e31  ',.        '10.1
+00002270: 3127 3a20 2731 302e 3131 2028 456c 2043  1': '10.11 (El C
+00002280: 6170 6974 616e 2927 2c0a 2020 2020 2020  apitan)',.      
+00002290: 2020 2734 3027 3a20 2753 6572 6965 7320    '40': 'Series 
+000022a0: 3430 272c 0a20 2020 2020 2020 2027 3630  40',.        '60
+000022b0: 273a 2027 5365 7269 6573 2036 3027 2c0a  ': 'Series 60',.
+000022c0: 2020 2020 2020 2020 274e 5420 332e 3127          'NT 3.1'
+000022d0: 3a20 274e 5420 332e 3120 2833 2e31 2927  : 'NT 3.1 (3.1)'
+000022e0: 2c0a 2020 2020 2020 2020 274e 5420 332e  ,.        'NT 3.
+000022f0: 3527 3a20 274e 5420 332e 3520 284e 5429  5': 'NT 3.5 (NT)
+00002300: 272c 0a20 2020 2020 2020 2027 4e54 2034  ',.        'NT 4
+00002310: 2e30 273a 2027 4e54 2034 2e30 2028 4e54  .0': 'NT 4.0 (NT
+00002320: 2927 2c0a 2020 2020 2020 2020 274e 5420  )',.        'NT 
+00002330: 342e 3127 3a20 274e 5420 342e 3120 2839  4.1': 'NT 4.1 (9
+00002340: 3829 272c 0a20 2020 2020 2020 2027 3978  8)',.        '9x
+00002350: 2034 2e39 3027 3a20 274e 5420 342e 3920   4.90': 'NT 4.9 
+00002360: 284d 4529 272c 0a20 2020 2020 2020 2027  (ME)',.        '
+00002370: 4e54 2035 2e30 273a 2027 4e54 2035 2e30  NT 5.0': 'NT 5.0
+00002380: 2028 3230 3030 2927 2c0a 2020 2020 2020   (2000)',.      
+00002390: 2020 274e 5420 352e 3127 3a20 274e 5420    'NT 5.1': 'NT 
+000023a0: 352e 3120 2858 5029 272c 0a20 2020 2020  5.1 (XP)',.     
+000023b0: 2020 2027 4e54 2035 2e32 273a 2027 4e54     'NT 5.2': 'NT
+000023c0: 2035 2e32 2028 3230 3033 2927 2c0a 2020   5.2 (2003)',.  
+000023d0: 2020 2020 2020 274e 5420 362e 3027 3a20        'NT 6.0': 
+000023e0: 274e 5420 362e 3020 2856 6973 7461 2927  'NT 6.0 (Vista)'
+000023f0: 2c0a 2020 2020 2020 2020 274e 5420 362e  ,.        'NT 6.
+00002400: 3127 3a20 274e 5420 362e 3120 2837 2927  1': 'NT 6.1 (7)'
+00002410: 2c0a 2020 2020 2020 2020 274e 5420 362e  ,.        'NT 6.
+00002420: 3227 3a20 274e 5420 362e 3220 2838 2927  2': 'NT 6.2 (8)'
+00002430: 2c0a 2020 2020 2020 2020 274e 5420 362e  ,.        'NT 6.
+00002440: 3327 3a20 274e 5420 362e 3320 2838 2e31  3': 'NT 6.3 (8.1
+00002450: 2927 2c0a 2020 2020 2020 2020 274e 5420  )',.        'NT 
+00002460: 362e 3427 3a20 274e 5420 362e 3420 2831  6.4': 'NT 6.4 (1
+00002470: 3029 272c 0a20 2020 2020 2020 2027 3136  0)',.        '16
+00002480: 273a 2027 4e54 2033 2e31 2028 332e 3129  ': 'NT 3.1 (3.1)
+00002490: 272c 0a20 2020 2020 2020 2027 332e 3127  ',.        '3.1'
+000024a0: 3a20 274e 5420 332e 3120 2833 2e31 2927  : 'NT 3.1 (3.1)'
+000024b0: 2c0a 2020 2020 2020 2020 2739 3527 3a20  ,.        '95': 
+000024c0: 274e 5420 342e 3020 2839 3529 272c 0a20  'NT 4.0 (95)',. 
+000024d0: 2020 2020 2020 2027 4e54 273a 2027 4e54         'NT': 'NT
+000024e0: 2034 2e30 2028 4e54 2927 2c0a 2020 2020   4.0 (NT)',.    
+000024f0: 2020 2020 274e 5434 2e30 273a 2027 4e54      'NT4.0': 'NT
+00002500: 2034 2e30 2028 4e54 2927 2c0a 2020 2020   4.0 (NT)',.    
+00002510: 2020 2020 2739 3827 3a20 274e 5420 342e      '98': 'NT 4.
+00002520: 3120 2839 3829 272c 0a20 2020 2020 2020  1 (98)',.       
+00002530: 2027 4d45 273a 2027 4e54 2034 2e39 2028   'ME': 'NT 4.9 (
+00002540: 4d45 2927 2c0a 2020 2020 2020 2020 2732  ME)',.        '2
+00002550: 3030 3027 3a20 274e 5420 352e 3020 2832  000': 'NT 5.0 (2
+00002560: 3030 3029 272c 0a20 2020 2020 2020 2027  000)',.        '
+00002570: 5850 273a 2027 4e54 2035 2e31 2028 5850  XP': 'NT 5.1 (XP
+00002580: 2927 2c0a 2020 2020 2020 2020 2732 3030  )',.        '200
+00002590: 3327 3a20 274e 5420 352e 3220 2832 3030  3': 'NT 5.2 (200
+000025a0: 3329 270a 2020 2020 7d0a 7d0a 0a64 6566  3)'.    }.}..def
+000025b0: 2067 6574 5f73 6f72 745f 6e61 6d65 286e   get_sort_name(n
+000025c0: 616d 6529 3a0a 2020 2020 2222 220a 0a20  ame):.    """.. 
+000025d0: 2020 203e 3e3e 2067 6574 5f73 6f72 745f     >>> get_sort_
+000025e0: 6e61 6d65 2827 416c 6672 6564 2048 6974  name('Alfred Hit
+000025f0: 6368 636f 636b 2729 0a20 2020 2027 4869  chcock').    'Hi
+00002600: 7463 6863 6f63 6b2c 2041 6c66 7265 6427  tchcock, Alfred'
+00002610: 0a0a 2020 2020 3e3e 3e20 6765 745f 736f  ..    >>> get_so
+00002620: 7274 5f6e 616d 6528 274a 6561 6e2d 4c75  rt_name('Jean-Lu
+00002630: 6320 476f 6461 7264 2729 0a20 2020 2027  c Godard').    '
+00002640: 476f 6461 7264 2c20 4a65 616e 2d4c 7563  Godard, Jean-Luc
+00002650: 270a 0a20 2020 203e 3e3e 2067 6574 5f73  '..    >>> get_s
+00002660: 6f72 745f 6e61 6d65 2827 5261 696e 6572  ort_name('Rainer
+00002670: 2057 6572 6e65 7220 4661 7373 6269 6e64   Werner Fassbind
+00002680: 6572 2729 0a20 2020 2027 4661 7373 6269  er').    'Fassbi
+00002690: 6e64 6572 2c20 5261 696e 6572 2057 6572  nder, Rainer Wer
+000026a0: 6e65 7227 0a0a 2020 2020 3e3e 3e20 6765  ner'..    >>> ge
+000026b0: 745f 736f 7274 5f6e 616d 6528 2742 7269  t_sort_name('Bri
+000026c0: 616e 2044 6520 5061 6c6d 6127 290a 2020  an De Palma').  
+000026d0: 2020 2744 6520 5061 6c6d 612c 2042 7269    'De Palma, Bri
+000026e0: 616e 270a 0a20 2020 203e 3e3e 2067 6574  an'..    >>> get
+000026f0: 5f73 6f72 745f 6e61 6d65 2827 4a6f 6861  _sort_name('Joha
+00002700: 6e20 7661 6e20 6465 7220 4b65 756b 656e  n van der Keuken
+00002710: 2729 0a20 2020 2027 7661 6e20 6465 7220  ').    'van der 
+00002720: 4b65 756b 656e 2c20 4a6f 6861 6e27 0a0a  Keuken, Johan'..
+00002730: 2020 2020 3e3e 3e20 6765 745f 736f 7274      >>> get_sort
+00002740: 5f6e 616d 6528 2745 6477 6172 6420 442e  _name('Edward D.
+00002750: 2057 6f6f 6420 4a72 2e27 290a 2020 2020   Wood Jr.').    
+00002760: 2757 6f6f 6420 4a72 2e2c 2045 6477 6172  'Wood Jr., Edwar
+00002770: 6420 442e 270a 0a20 2020 203e 3e3e 2067  d D.'..    >>> g
+00002780: 6574 5f73 6f72 745f 6e61 6d65 2827 4269  et_sort_name('Bi
+00002790: 6e67 2057 616e 6727 290a 2020 2020 2757  ng Wang').    'W
+000027a0: 616e 6720 4269 6e67 270a 0a20 2020 203e  ang Bing'..    >
+000027b0: 3e3e 2067 6574 5f73 6f72 745f 6e61 6d65  >> get_sort_name
+000027c0: 2827 4672 616e 6b20 4361 7072 6120 4949  ('Frank Capra II
+000027d0: 4927 290a 2020 2020 2743 6170 7261 2049  I').    'Capra I
+000027e0: 4949 2c20 4672 616e 6b27 0a0a 2020 2020  II, Frank'..    
+000027f0: 3e3e 3e20 6765 745f 736f 7274 5f6e 616d  >>> get_sort_nam
+00002800: 6528 2754 6865 2051 7565 656e 206f 6620  e('The Queen of 
+00002810: 456e 676c 616e 6427 290a 2020 2020 2751  England').    'Q
+00002820: 7565 656e 206f 6620 456e 676c 616e 642c  ueen of England,
+00002830: 2054 6865 270a 0a20 2020 203e 3e3e 2067   The'..    >>> g
+00002840: 6574 5f73 6f72 745f 6e61 6d65 2827 5368  et_sort_name('Sh
+00002850: 616d 2036 3927 290a 2020 2020 2753 6861  am 69').    'Sha
+00002860: 6d20 3639 270a 0a20 2020 203e 3e3e 2067  m 69'..    >>> g
+00002870: 6574 5f73 6f72 745f 6e61 6d65 2827 5363  et_sort_name('Sc
+00002880: 6f72 7365 7365 2c20 4d61 7274 696e 2729  orsese, Martin')
+00002890: 0a20 2020 2027 5363 6f72 7365 7365 2c20  .    'Scorsese, 
+000028a0: 4d61 7274 696e 270a 2020 2020 2222 220a  Martin'.    """.
+000028b0: 2020 2020 6966 2027 2027 206e 6f74 2069      if ' ' not i
+000028c0: 6e20 6e61 6d65 206f 7220 272c 2027 2069  n name or ', ' i
+000028d0: 6e20 6e61 6d65 3a0a 2020 2020 2020 2020  n name:.        
+000028e0: 7265 7475 726e 206e 616d 650a 2020 2020  return name.    
+000028f0: 6966 206e 616d 652e 6c6f 7765 7228 292e  if name.lower().
+00002900: 7374 6172 7473 7769 7468 2827 7468 6520  startswith('the 
+00002910: 2729 3a0a 2020 2020 2020 2020 7265 7475  '):.        retu
+00002920: 726e 2067 6574 5f73 6f72 745f 7469 746c  rn get_sort_titl
+00002930: 6528 6e61 6d65 290a 0a20 2020 2064 6566  e(name)..    def
+00002940: 2061 6464 5f6e 616d 6528 293a 0a20 2020   add_name():.   
+00002950: 2020 2020 2069 6620 6c65 6e28 6669 7273       if len(firs
+00002960: 745f 6e61 6d65 7329 3a0a 2020 2020 2020  t_names):.      
+00002970: 2020 2020 2020 6c61 7374 5f6e 616d 6573        last_names
+00002980: 2e69 6e73 6572 7428 302c 2066 6972 7374  .insert(0, first
+00002990: 5f6e 616d 6573 2e70 6f70 2829 290a 0a20  _names.pop()).. 
+000029a0: 2020 2064 6566 2066 696e 645f 6e61 6d65     def find_name
+000029b0: 286e 616d 6573 293a 0a20 2020 2020 2020  (names):.       
+000029c0: 2072 6574 7572 6e20 6c65 6e28 6669 7273   return len(firs
+000029d0: 745f 6e61 6d65 7329 2061 6e64 2066 6972  t_names) and fir
+000029e0: 7374 5f6e 616d 6573 5b2d 315d 2e6c 6f77  st_names[-1].low
+000029f0: 6572 2829 2069 6e20 6e61 6d65 730a 0a20  er() in names.. 
+00002a00: 2020 2069 6620 6973 5f61 7369 616e 5f6e     if is_asian_n
+00002a10: 616d 6528 6e61 6d65 293a 0a20 2020 2020  ame(name):.     
+00002a20: 2020 206e 616d 6573 203d 206e 616d 652e     names = name.
+00002a30: 7265 706c 6163 6528 272d 272c 2027 2027  replace('-', ' '
+00002a40: 292e 7370 6c69 7428 2720 2729 0a20 2020  ).split(' ').   
+00002a50: 2020 2020 2069 6620 6c65 6e28 6e61 6d65       if len(name
+00002a60: 7329 203d 3d20 323a 0a20 2020 2020 2020  s) == 2:.       
+00002a70: 2020 2020 2069 6620 6e61 6d65 735b 305d       if names[0]
+00002a80: 2e6c 6f77 6572 2829 2069 6e20 4153 4941  .lower() in ASIA
+00002a90: 4e5f 4c41 5354 5f4e 414d 4553 3a0a 2020  N_LAST_NAMES:.  
+00002aa0: 2020 2020 2020 2020 2020 2020 2020 6c61                la
+00002ab0: 7374 6e61 6d65 2c20 6669 7273 746e 616d  stname, firstnam
+00002ac0: 6520 3d20 6e61 6d65 730a 2020 2020 2020  e = names.      
+00002ad0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00002ae0: 2020 2020 2020 2020 2020 2020 6669 7273              firs
+00002af0: 746e 616d 652c 206c 6173 746e 616d 6520  tname, lastname 
+00002b00: 3d20 6e61 6d65 730a 2020 2020 2020 2020  = names.        
+00002b10: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00002b20: 2020 6e61 6d65 735f 203d 206e 616d 652e    names_ = name.
+00002b30: 7370 6c69 7428 2720 2729 0a20 2020 2020  split(' ').     
+00002b40: 2020 2020 2020 2069 6620 272d 2720 696e         if '-' in
+00002b50: 206e 616d 6573 5f5b 305d 3a0a 2020 2020   names_[0]:.    
+00002b60: 2020 2020 2020 2020 2020 2020 6c61 7374              last
+00002b70: 6e61 6d65 2c20 6669 7273 746e 616d 6520  name, firstname 
+00002b80: 3d20 5b6e 616d 6573 5b32 5d2c 206e 616d  = [names[2], nam
+00002b90: 6573 5b30 5d20 2b20 272d 2720 2b20 6e61  es[0] + '-' + na
+00002ba0: 6d65 735b 315d 2e6c 6f77 6572 2829 5d0a  mes[1].lower()].
+00002bb0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00002bc0: 2027 2d27 2069 6e20 6e61 6d65 735f 5b31   '-' in names_[1
+00002bd0: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+00002be0: 2020 206c 6173 746e 616d 652c 2066 6972     lastname, fir
+00002bf0: 7374 6e61 6d65 203d 205b 6e61 6d65 735b  stname = [names[
+00002c00: 305d 2c20 6e61 6d65 735b 315d 202b 2027  0], names[1] + '
+00002c10: 2d27 202b 206e 616d 6573 5b32 5d2e 6c6f  -' + names[2].lo
+00002c20: 7765 7228 295d 0a20 2020 2020 2020 2020  wer()].         
+00002c30: 2020 2065 6c69 6620 6e61 6d65 735b 305d     elif names[0]
+00002c40: 2e6c 6f77 6572 2829 2069 6e20 4153 4941  .lower() in ASIA
+00002c50: 4e5f 4649 5253 545f 4e41 4d45 5320 616e  N_FIRST_NAMES an
+00002c60: 6420 6e61 6d65 735b 325d 2e6c 6f77 6572  d names[2].lower
+00002c70: 2829 206e 6f74 2069 6e20 4153 4941 4e5f  () not in ASIAN_
+00002c80: 4649 5253 545f 4e41 4d45 533a 0a20 2020  FIRST_NAMES:.   
+00002c90: 2020 2020 2020 2020 2020 2020 206c 6173               las
+00002ca0: 746e 616d 652c 2066 6972 7374 6e61 6d65  tname, firstname
+00002cb0: 203d 205b 6e61 6d65 735b 325d 2c20 6e61   = [names[2], na
+00002cc0: 6d65 735b 305d 202b 2027 2027 202b 206e  mes[0] + ' ' + n
+00002cd0: 616d 6573 5b31 5d5d 0a20 2020 2020 2020  ames[1]].       
+00002ce0: 2020 2020 2065 6c69 6620 6e61 6d65 735b       elif names[
+00002cf0: 305d 2e6c 6f77 6572 2829 206e 6f74 2069  0].lower() not i
+00002d00: 6e20 4153 4941 4e5f 4649 5253 545f 4e41  n ASIAN_FIRST_NA
+00002d10: 4d45 5320 616e 6420 6e61 6d65 735b 325d  MES and names[2]
+00002d20: 2e6c 6f77 6572 2829 2069 6e20 4153 4941  .lower() in ASIA
+00002d30: 4e5f 4649 5253 545f 4e41 4d45 533a 0a20  N_FIRST_NAMES:. 
+00002d40: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00002d50: 6173 746e 616d 652c 2066 6972 7374 6e61  astname, firstna
+00002d60: 6d65 203d 205b 6e61 6d65 735b 305d 2c20  me = [names[0], 
+00002d70: 6e61 6d65 735b 315d 202b 2027 2027 202b  names[1] + ' ' +
+00002d80: 206e 616d 6573 5b32 5d5d 0a20 2020 2020   names[2]].     
+00002d90: 2020 2020 2020 2065 6c69 6620 6e61 6d65         elif name
+00002da0: 735b 305d 2e6c 6f77 6572 2829 2069 6e20  s[0].lower() in 
+00002db0: 4153 4941 4e5f 4c41 5354 5f4e 414d 4553  ASIAN_LAST_NAMES
+00002dc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00002dd0: 2020 6c61 7374 6e61 6d65 2c20 6669 7273    lastname, firs
+00002de0: 746e 616d 6520 3d20 5b6e 616d 6573 5b30  tname = [names[0
+00002df0: 5d2c 206e 616d 6573 5b31 5d20 2b20 2720  ], names[1] + ' 
+00002e00: 2720 2b20 6e61 6d65 735b 325d 5d0a 2020  ' + names[2]].  
+00002e10: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00002e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e30: 6c61 7374 6e61 6d65 2c20 6669 7273 746e  lastname, firstn
+00002e40: 616d 6520 3d20 5b6e 616d 6573 5b32 5d2c  ame = [names[2],
+00002e50: 206e 616d 6573 5b30 5d20 2b20 2720 2720   names[0] + ' ' 
+00002e60: 2b20 6e61 6d65 735b 315d 5d0a 2020 2020  + names[1]].    
+00002e70: 2020 2020 7265 7475 726e 206c 6173 746e      return lastn
+00002e80: 616d 6520 2b20 2720 2720 2b20 6669 7273  ame + ' ' + firs
+00002e90: 746e 616d 650a 0a20 2020 2066 6972 7374  tname..    first
+00002ea0: 5f6e 616d 6573 203d 206e 616d 652e 7370  _names = name.sp
+00002eb0: 6c69 7428 2720 2729 0a20 2020 206c 6173  lit(' ').    las
+00002ec0: 745f 6e61 6d65 7320 3d20 5b5d 0a20 2020  t_names = [].   
+00002ed0: 2069 6620 7265 2e73 6561 7263 6828 275e   if re.search('^
+00002ee0: 5b30 2d39 5d2b 2427 2c20 6669 7273 745f  [0-9]+$', first_
+00002ef0: 6e61 6d65 735b 2d31 5d29 3a0a 2020 2020  names[-1]):.    
+00002f00: 2020 2020 6164 645f 6e61 6d65 2829 0a20      add_name(). 
+00002f10: 2020 2069 6620 7265 2e73 6561 7263 6828     if re.search(
+00002f20: 275b 285c 5b5d 2e2b 3f5b 295c 5d5d 2427  '[(\[].+?[)\]]$'
+00002f30: 2c20 6669 7273 745f 6e61 6d65 735b 2d31  , first_names[-1
+00002f40: 5d29 3a0a 2020 2020 2020 2020 6164 645f  ]):.        add_
+00002f50: 6e61 6d65 2829 0a20 2020 2069 6620 6669  name().    if fi
+00002f60: 6e64 5f6e 616d 6528 5355 4646 4958 4553  nd_name(SUFFIXES
+00002f70: 293a 0a20 2020 2020 2020 2061 6464 5f6e  ):.        add_n
+00002f80: 616d 6528 290a 2020 2020 6164 645f 6e61  ame().    add_na
+00002f90: 6d65 2829 0a20 2020 2069 6620 6669 6e64  me().    if find
+00002fa0: 5f6e 616d 6528 4d49 4446 4958 4553 293a  _name(MIDFIXES):
+00002fb0: 0a20 2020 2020 2020 2061 6464 5f6e 616d  .        add_nam
+00002fc0: 6528 290a 2020 2020 2020 2020 6164 645f  e().        add_
+00002fd0: 6e61 6d65 2829 0a20 2020 2077 6869 6c65  name().    while
+00002fe0: 2066 696e 645f 6e61 6d65 2850 5245 4649   find_name(PREFI
+00002ff0: 5845 5329 3a0a 2020 2020 2020 2020 6164  XES):.        ad
+00003000: 645f 6e61 6d65 2829 0a20 2020 206e 616d  d_name().    nam
+00003010: 6520 3d20 2720 272e 6a6f 696e 286c 6173  e = ' '.join(las
+00003020: 745f 6e61 6d65 7329 0a20 2020 2069 6620  t_names).    if 
+00003030: 6c65 6e28 6669 7273 745f 6e61 6d65 7329  len(first_names)
+00003040: 3a0a 2020 2020 2020 2020 7365 7061 7261  :.        separa
+00003050: 746f 7220 3d20 2720 2720 6966 206c 6173  tor = ' ' if las
+00003060: 745f 6e61 6d65 735b 305d 2e6c 6f77 6572  t_names[0].lower
+00003070: 2829 2069 6e20 4153 4941 4e5f 4c41 5354  () in ASIAN_LAST
+00003080: 5f4e 414d 4553 2065 6c73 6520 272c 2027  _NAMES else ', '
+00003090: 0a20 2020 2020 2020 206e 616d 6520 2b3d  .        name +=
+000030a0: 2073 6570 6172 6174 6f72 202b 2027 2027   separator + ' '
+000030b0: 2e6a 6f69 6e28 6669 7273 745f 6e61 6d65  .join(first_name
+000030c0: 7329 0a20 2020 2072 6574 7572 6e20 6e61  s).    return na
+000030d0: 6d65 0a0a 6465 6620 6765 745f 736f 7274  me..def get_sort
+000030e0: 5f74 6974 6c65 2874 6974 6c65 293a 0a20  _title(title):. 
+000030f0: 2020 2022 2222 0a0a 2020 2020 3e3e 3e20     """..    >>> 
+00003100: 6765 745f 736f 7274 5f74 6974 6c65 2827  get_sort_title('
+00003110: 5468 656d 726f 6327 290a 2020 2020 2754  Themroc').    'T
+00003120: 6865 6d72 6f63 270a 0a20 2020 203e 3e3e  hemroc'..    >>>
+00003130: 2067 6574 5f73 6f72 745f 7469 746c 6528   get_sort_title(
+00003140: 2744 6965 2048 6172 6427 290a 2020 2020  'Die Hard').    
+00003150: 2748 6172 642c 2044 6965 270a 0a20 2020  'Hard, Die'..   
+00003160: 203e 3e3e 2067 6574 5f73 6f72 745f 7469   >>> get_sort_ti
+00003170: 746c 6528 224c 2761 7461 6c61 6e74 6522  tle("L'atalante"
+00003180: 290a 2020 2020 2261 7461 6c61 6e74 652c  ).    "atalante,
+00003190: 204c 2722 0a0a 2020 2020 2222 220a 2020   L'"..    """.  
+000031a0: 2020 666f 7220 6172 7469 636c 6520 696e    for article in
+000031b0: 2041 5254 4943 4c45 533a 0a20 2020 2020   ARTICLES:.     
+000031c0: 2020 2073 7061 6365 7320 3d20 3020 6966     spaces = 0 if
+000031d0: 2061 7274 6963 6c65 2e65 6e64 7377 6974   article.endswit
+000031e0: 6828 2227 2229 2065 6c73 6520 310a 2020  h("'") else 1.  
+000031f0: 2020 2020 2020 6966 2074 6974 6c65 2e6c        if title.l
+00003200: 6f77 6572 2829 2e73 7461 7274 7377 6974  ower().startswit
+00003210: 6828 6172 7469 636c 6520 2b20 2720 2720  h(article + ' ' 
+00003220: 2a20 7370 6163 6573 293a 0a20 2020 2020  * spaces):.     
+00003230: 2020 2020 2020 206c 656e 6774 6820 3d20         length = 
+00003240: 6c65 6e28 6172 7469 636c 6529 0a20 2020  len(article).   
+00003250: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00003260: 7469 746c 655b 6c65 6e67 7468 202b 2073  title[length + s
+00003270: 7061 6365 733a 5d20 2b20 272c 2027 202b  paces:] + ', ' +
+00003280: 2074 6974 6c65 5b3a 6c65 6e67 7468 5d0a   title[:length].
+00003290: 2020 2020 7265 7475 726e 2074 6974 6c65      return title
+000032a0: 0a0a 6465 6620 6669 6e64 5f72 6528 7374  ..def find_re(st
+000032b0: 7269 6e67 2c20 7265 6765 7870 293a 0a20  ring, regexp):. 
+000032c0: 2020 2072 6573 756c 7420 3d20 7265 2e63     result = re.c
+000032d0: 6f6d 7069 6c65 2872 6567 6578 702c 2072  ompile(regexp, r
+000032e0: 652e 444f 5441 4c4c 292e 6669 6e64 616c  e.DOTALL).findal
+000032f0: 6c28 7374 7269 6e67 290a 2020 2020 6966  l(string).    if
+00003300: 2072 6573 756c 743a 0a20 2020 2020 2020   result:.       
+00003310: 2072 6574 7572 6e20 7265 7375 6c74 5b30   return result[0
+00003320: 5d2e 7374 7269 7028 290a 2020 2020 7265  ].strip().    re
+00003330: 7475 726e 2027 270a 0a64 6566 2066 696e  turn ''..def fin
+00003340: 645f 7374 7269 6e67 2873 7472 696e 672c  d_string(string,
+00003350: 2073 7472 696e 6730 3d27 272c 2073 7472   string0='', str
+00003360: 696e 6731 3d27 2729 3a0a 2020 2020 2222  ing1=''):.    ""
+00003370: 2252 6574 7572 6e20 7468 6520 7374 7269  "Return the stri
+00003380: 6e67 2062 6574 7765 656e 2073 7472 696e  ng between strin
+00003390: 6730 2061 6e64 2073 7472 696e 6731 2e0a  g0 and string1..
+000033a0: 0a20 2020 2049 6620 7374 7269 6e67 3020  .    If string0 
+000033b0: 6f72 2073 7472 696e 6731 2069 7320 6c65  or string1 is le
+000033c0: 6674 206f 7574 2c20 6265 6769 6e69 6e67  ft out, begining
+000033d0: 206f 7220 656e 6420 6f66 2073 7472 696e   or end of strin
+000033e0: 6720 6973 2075 7365 642e 0a0a 2020 2020  g is used...    
+000033f0: 3e3e 3e20 6669 6e64 5f73 7472 696e 6728  >>> find_string(
+00003400: 2769 2061 6d20 6e6f 7420 7468 6572 6527  'i am not there'
+00003410: 2c20 7374 7269 6e67 313d 2720 6e6f 7420  , string1=' not 
+00003420: 7468 6572 6527 290a 2020 2020 2769 2061  there').    'i a
+00003430: 6d27 0a0a 2020 2020 3e3e 3e20 6669 6e64  m'..    >>> find
+00003440: 5f73 7472 696e 6728 2769 2061 6d20 6e6f  _string('i am no
+00003450: 7420 7468 6572 6527 2c20 2769 2061 6d20  t there', 'i am 
+00003460: 272c 2027 2074 6865 7265 2729 0a20 2020  ', ' there').   
+00003470: 2027 6e6f 7427 0a0a 2020 2020 3e3e 3e20   'not'..    >>> 
+00003480: 6669 6e64 5f73 7472 696e 6728 2769 2061  find_string('i a
+00003490: 6d20 6e6f 7420 7468 6572 6527 2c20 2769  m not there', 'i
+000034a0: 2061 6d20 6e6f 7420 7427 290a 2020 2020   am not t').    
+000034b0: 2768 6572 6527 0a0a 2020 2020 2222 220a  'here'..    """.
+000034c0: 2020 2020 6966 2073 7472 696e 6730 3a0a      if string0:.
+000034d0: 2020 2020 2020 2020 7374 7269 6e67 3020          string0 
+000034e0: 3d20 7265 2e65 7363 6170 6528 7374 7269  = re.escape(stri
+000034f0: 6e67 3029 0a20 2020 2065 6c73 653a 0a20  ng0).    else:. 
+00003500: 2020 2020 2020 2073 7472 696e 6730 203d         string0 =
+00003510: 2027 5e27 0a20 2020 2069 6620 7374 7269   '^'.    if stri
+00003520: 6e67 313a 0a20 2020 2020 2020 2073 7472  ng1:.        str
+00003530: 696e 6731 203d 2072 652e 6573 6361 7065  ing1 = re.escape
+00003540: 2873 7472 696e 6731 290a 2020 2020 656c  (string1).    el
+00003550: 7365 3a0a 2020 2020 2020 2020 7374 7269  se:.        stri
+00003560: 6e67 3120 3d20 2724 270a 2020 2020 7265  ng1 = '$'.    re
+00003570: 7475 726e 2066 696e 645f 7265 2873 7472  turn find_re(str
+00003580: 696e 672c 2073 7472 696e 6730 202b 2027  ing, string0 + '
+00003590: 282e 2a3f 2927 202b 2073 7472 696e 6731  (.*?)' + string1
+000035a0: 290a 0a64 6566 2069 735f 6173 6961 6e5f  )..def is_asian_
+000035b0: 6e61 6d65 286e 616d 6529 3a0a 2020 2020  name(name):.    
+000035c0: 6e61 6d65 7320 3d20 6e61 6d65 2e72 6570  names = name.rep
+000035d0: 6c61 6365 2827 2d27 2c20 2720 2729 2e6c  lace('-', ' ').l
+000035e0: 6f77 6572 2829 2e73 706c 6974 2827 2027  ower().split(' '
+000035f0: 290a 2020 2020 7265 7475 726e 2028 6c65  ).    return (le
+00003600: 6e28 6e61 6d65 7329 203d 3d20 3220 616e  n(names) == 2 an
+00003610: 6420 6e6f 7420 272d 2720 696e 206e 616d  d not '-' in nam
+00003620: 6520 616e 6420 280a 2020 2020 2020 2020  e and (.        
+00003630: 286e 616d 6573 5b30 5d20 696e 2041 5349  (names[0] in ASI
+00003640: 414e 5f46 4952 5354 5f4e 414d 4553 2061  AN_FIRST_NAMES a
+00003650: 6e64 206e 616d 6573 5b31 5d20 696e 2041  nd names[1] in A
+00003660: 5349 414e 5f4c 4153 545f 4e41 4d45 5329  SIAN_LAST_NAMES)
+00003670: 206f 720a 2020 2020 2020 2020 286e 616d   or.        (nam
+00003680: 6573 5b30 5d20 696e 2041 5349 414e 5f4c  es[0] in ASIAN_L
+00003690: 4153 545f 4e41 4d45 5320 616e 6420 6e61  AST_NAMES and na
+000036a0: 6d65 735b 315d 2069 6e20 4153 4941 4e5f  mes[1] in ASIAN_
+000036b0: 4649 5253 545f 4e41 4d45 5329 0a20 2020  FIRST_NAMES).   
+000036c0: 2029 2920 6f72 2028 0a20 2020 2020 2020   )) or (.       
+000036d0: 206c 656e 286e 616d 6573 2920 3d3d 2033   len(names) == 3
+000036e0: 2061 6e64 206e 616d 6573 5b31 5d20 696e   and names[1] in
+000036f0: 2041 5349 414e 5f46 4952 5354 5f4e 414d   ASIAN_FIRST_NAM
+00003700: 4553 2061 6e64 2028 0a20 2020 2020 2020  ES and (.       
+00003710: 2020 2020 206e 616d 6573 5b30 5d20 696e       names[0] in
+00003720: 2041 5349 414e 5f46 4952 5354 5f4e 414d   ASIAN_FIRST_NAM
+00003730: 4553 206f 7220 6e61 6d65 735b 325d 2069  ES or names[2] i
+00003740: 6e20 4153 4941 4e5f 4649 5253 545f 4e41  n ASIAN_FIRST_NA
+00003750: 4d45 530a 2020 2020 2020 2020 290a 2020  MES.        ).  
+00003760: 2020 290a 0a64 6566 2070 6172 7365 5f75    )..def parse_u
+00003770: 7365 7261 6765 6e74 2875 7365 7261 6765  seragent(userage
+00003780: 6e74 293a 0a20 2020 2064 6174 6120 3d20  nt):.    data = 
+00003790: 7b7d 0a20 2020 2066 6f72 206b 6579 2069  {}.    for key i
+000037a0: 6e20 5541 5f52 4547 4558 5053 3a0a 2020  n UA_REGEXPS:.  
+000037b0: 2020 2020 2020 666f 7220 616c 6961 732c        for alias,
+000037c0: 2072 6567 6578 7020 696e 2055 415f 414c   regexp in UA_AL
+000037d0: 4941 5345 535b 6b65 795d 2e69 7465 6d73  IASES[key].items
+000037e0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+000037f0: 616c 6961 7320 3d20 616c 6961 7320 6966  alias = alias if
+00003800: 206b 6579 203d 3d20 2762 726f 7773 6572   key == 'browser
+00003810: 2720 656c 7365 2061 6c69 6173 202b 2027  ' else alias + '
+00003820: 205c 5c31 270a 2020 2020 2020 2020 2020   \\1'.          
+00003830: 2020 7573 6572 6167 656e 7420 3d20 7265    useragent = re
+00003840: 2e73 7562 2872 6567 6578 702c 2061 6c69  .sub(regexp, ali
+00003850: 6173 2c20 7573 6572 6167 656e 7429 0a20  as, useragent). 
+00003860: 2020 2020 2020 2066 6f72 2072 6567 6578         for regex
+00003870: 7020 696e 2055 415f 5245 4745 5850 535b  p in UA_REGEXPS[
+00003880: 6b65 795d 3a0a 2020 2020 2020 2020 2020  key]:.          
+00003890: 2020 6461 7461 5b6b 6579 5d20 3d20 7b27    data[key] = {'
+000038a0: 6e61 6d65 273a 2027 272c 2027 7665 7273  name': '', 'vers
+000038b0: 696f 6e27 3a20 2727 2c20 2773 7472 696e  ion': '', 'strin
+000038c0: 6727 3a20 2727 7d0a 2020 2020 2020 2020  g': ''}.        
+000038d0: 2020 2020 6d61 7463 6820 3d20 7265 2e63      match = re.c
+000038e0: 6f6d 7069 6c65 2872 6567 6578 7029 2e73  ompile(regexp).s
+000038f0: 6561 7263 6828 7573 6572 6167 656e 7429  earch(useragent)
+00003900: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00003910: 6d61 7463 683a 0a20 2020 2020 2020 2020  match:.         
+00003920: 2020 2020 2020 206d 6174 6368 6573 203d         matches =
+00003930: 206c 6973 7428 6d61 7463 682e 6772 6f75   list(match.grou
+00003940: 7073 2829 290a 2020 2020 2020 2020 2020  ps()).          
+00003950: 2020 2020 2020 6966 206c 656e 286d 6174        if len(mat
+00003960: 6368 6573 2920 3d3d 2031 3a0a 2020 2020  ches) == 1:.    
 00003970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003980: 7377 6170 203d 2072 652e 6d61 7463 6828  swap = re.match(
-00003990: 275e 5c64 272c 206d 6174 6368 6573 5b30  '^\d', matches[0
-000039a0: 5d29 206f 7220 6d61 7463 6865 735b 315d  ]) or matches[1]
-000039b0: 203d 3d20 274c 696e 7578 270a 2020 2020   == 'Linux'.    
-000039c0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-000039d0: 203d 206d 6174 6368 6573 5b31 2069 6620   = matches[1 if 
-000039e0: 7377 6170 2065 6c73 6520 305d 0a20 2020  swap else 0].   
-000039f0: 2020 2020 2020 2020 2020 2020 2076 6572               ver
-00003a00: 7369 6f6e 203d 206d 6174 6368 6573 5b30  sion = matches[0
-00003a10: 2069 6620 7377 6170 2065 6c73 6520 315d   if swap else 1]
-00003a20: 2e72 6570 6c61 6365 2827 5f27 2c20 272e  .replace('_', '.
-00003a30: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
-00003a40: 2020 206e 616d 6520 3d20 5541 5f4e 414d     name = UA_NAM
-00003a50: 4553 5b6b 6579 5d5b 6e61 6d65 5d20 6966  ES[key][name] if
-00003a60: 206e 616d 6520 696e 2055 415f 4e41 4d45   name in UA_NAME
-00003a70: 535b 6b65 795d 2065 6c73 6520 6e61 6d65  S[key] else name
-00003a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003a90: 2076 6572 7369 6f6e 203d 2055 415f 5645   version = UA_VE
-00003aa0: 5253 494f 4e53 5b6b 6579 5d5b 7665 7273  RSIONS[key][vers
-00003ab0: 696f 6e5d 2069 6620 7665 7273 696f 6e20  ion] if version 
-00003ac0: 696e 2055 415f 5645 5253 494f 4e53 5b6b  in UA_VERSIONS[k
-00003ad0: 6579 5d20 656c 7365 2076 6572 7369 6f6e  ey] else version
-00003ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003af0: 2073 7472 696e 6720 3d20 6e61 6d65 0a20   string = name. 
-00003b00: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00003b10: 6620 7665 7273 696f 6e3a 0a20 2020 2020  f version:.     
-00003b20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00003b30: 7472 696e 6720 3d20 7374 7269 6e67 202b  tring = string +
-00003b40: 2027 2027 202b 2028 0a20 2020 2020 2020   ' ' + (.       
-00003b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b60: 2027 2827 202b 2076 6572 7369 6f6e 202b   '(' + version +
-00003b70: 2027 2927 2069 6620 6e61 6d65 2069 6e20   ')' if name in 
-00003b80: 5b27 4253 4427 2c20 274c 696e 7578 272c  ['BSD', 'Linux',
-00003b90: 2027 556e 6978 275d 2065 6c73 6520 7665   'Unix'] else ve
-00003ba0: 7273 696f 6e0a 2020 2020 2020 2020 2020  rsion.          
-00003bb0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00003bc0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00003bd0: 5b6b 6579 5d20 3d20 7b0a 2020 2020 2020  [key] = {.      
-00003be0: 2020 2020 2020 2020 2020 2020 2020 276e                'n
-00003bf0: 616d 6527 3a20 6e61 6d65 2c0a 2020 2020  ame': name,.    
+00003980: 6d61 7463 6865 732e 6170 7065 6e64 2827  matches.append('
+00003990: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
+000039a0: 2020 2073 7761 7020 3d20 7265 2e6d 6174     swap = re.mat
+000039b0: 6368 2827 5e5c 6427 2c20 6d61 7463 6865  ch('^\d', matche
+000039c0: 735b 305d 2920 6f72 206d 6174 6368 6573  s[0]) or matches
+000039d0: 5b31 5d20 3d3d 2027 4c69 6e75 7827 0a20  [1] == 'Linux'. 
+000039e0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+000039f0: 616d 6520 3d20 6d61 7463 6865 735b 3120  ame = matches[1 
+00003a00: 6966 2073 7761 7020 656c 7365 2030 5d0a  if swap else 0].
+00003a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a20: 7665 7273 696f 6e20 3d20 6d61 7463 6865  version = matche
+00003a30: 735b 3020 6966 2073 7761 7020 656c 7365  s[0 if swap else
+00003a40: 2031 5d2e 7265 706c 6163 6528 275f 272c   1].replace('_',
+00003a50: 2027 2e27 290a 2020 2020 2020 2020 2020   '.').          
+00003a60: 2020 2020 2020 6e61 6d65 203d 2055 415f        name = UA_
+00003a70: 4e41 4d45 535b 6b65 795d 5b6e 616d 655d  NAMES[key][name]
+00003a80: 2069 6620 6e61 6d65 2069 6e20 5541 5f4e   if name in UA_N
+00003a90: 414d 4553 5b6b 6579 5d20 656c 7365 206e  AMES[key] else n
+00003aa0: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
+00003ab0: 2020 2020 7665 7273 696f 6e20 3d20 5541      version = UA
+00003ac0: 5f56 4552 5349 4f4e 535b 6b65 795d 5b76  _VERSIONS[key][v
+00003ad0: 6572 7369 6f6e 5d20 6966 2076 6572 7369  ersion] if versi
+00003ae0: 6f6e 2069 6e20 5541 5f56 4552 5349 4f4e  on in UA_VERSION
+00003af0: 535b 6b65 795d 2065 6c73 6520 7665 7273  S[key] else vers
+00003b00: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+00003b10: 2020 2020 7374 7269 6e67 203d 206e 616d      string = nam
+00003b20: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00003b30: 2020 6966 2076 6572 7369 6f6e 3a0a 2020    if version:.  
+00003b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b50: 2020 7374 7269 6e67 203d 2073 7472 696e    string = strin
+00003b60: 6720 2b20 2720 2720 2b20 280a 2020 2020  g + ' ' + (.    
+00003b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b80: 2020 2020 2728 2720 2b20 7665 7273 696f      '(' + versio
+00003b90: 6e20 2b20 2729 2720 6966 206e 616d 6520  n + ')' if name 
+00003ba0: 696e 205b 2742 5344 272c 2027 4c69 6e75  in ['BSD', 'Linu
+00003bb0: 7827 2c20 2755 6e69 7827 5d20 656c 7365  x', 'Unix'] else
+00003bc0: 2076 6572 7369 6f6e 0a20 2020 2020 2020   version.       
+00003bd0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00003be0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00003bf0: 6174 615b 6b65 795d 203d 207b 0a20 2020  ata[key] = {.   
 00003c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c10: 2776 6572 7369 6f6e 273a 2076 6572 7369  'version': versi
-00003c20: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
-00003c30: 2020 2020 2020 2020 2773 7472 696e 6727          'string'
-00003c40: 3a20 7374 7269 6e67 0a20 2020 2020 2020  : string.       
-00003c50: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00003c60: 2020 2020 2020 2020 2020 2062 7265 616b             break
-00003c70: 0a20 2020 2072 6574 7572 6e20 6461 7461  .    return data
-00003c80: 0a0a 6465 6620 7265 6d6f 7665 5f73 7065  ..def remove_spe
-00003c90: 6369 616c 5f63 6861 7261 6374 6572 7328  cial_characters(
-00003ca0: 7465 7874 293a 0a20 2020 2022 2222 0a20  text):.    """. 
-00003cb0: 2020 2052 656d 6f76 6573 2073 7065 6369     Removes speci
-00003cc0: 616c 2063 6861 7261 6374 6572 7320 696e  al characters in
-00003cd0: 7365 7274 6564 2062 7920 576f 7264 2e0a  serted by Word..
-00003ce0: 2020 2020 2222 220a 2020 2020 7465 7874      """.    text
-00003cf0: 203d 2074 6578 742e 7265 706c 6163 6528   = text.replace(
-00003d00: 7527 5c75 3230 3133 272c 2027 2d27 290a  u'\u2013', '-').
-00003d10: 2020 2020 7465 7874 203d 2074 6578 742e      text = text.
-00003d20: 7265 706c 6163 6528 7527 5c75 3230 3236  replace(u'\u2026
-00003d30: 4f27 2c20 2227 2229 0a20 2020 2074 6578  O', "'").    tex
-00003d40: 7420 3d20 7465 7874 2e72 6570 6c61 6365  t = text.replace
-00003d50: 2875 275c 7532 3031 3927 2c20 2227 2229  (u'\u2019', "'")
-00003d60: 0a20 2020 2074 6578 7420 3d20 7465 7874  .    text = text
-00003d70: 2e72 6570 6c61 6365 2875 2719 272c 2022  .replace(u'.', "
+00003c10: 2027 6e61 6d65 273a 206e 616d 652c 0a20   'name': name,. 
+00003c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c30: 2020 2027 7665 7273 696f 6e27 3a20 7665     'version': ve
+00003c40: 7273 696f 6e2c 0a20 2020 2020 2020 2020  rsion,.         
+00003c50: 2020 2020 2020 2020 2020 2027 7374 7269             'stri
+00003c60: 6e67 273a 2073 7472 696e 670a 2020 2020  ng': string.    
+00003c70: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00003c80: 2020 2020 2020 2020 2020 2020 2020 6272                br
+00003c90: 6561 6b0a 2020 2020 7265 7475 726e 2064  eak.    return d
+00003ca0: 6174 610a 0a64 6566 2072 656d 6f76 655f  ata..def remove_
+00003cb0: 7370 6563 6961 6c5f 6368 6172 6163 7465  special_characte
+00003cc0: 7273 2874 6578 7429 3a0a 2020 2020 2222  rs(text):.    ""
+00003cd0: 220a 2020 2020 5265 6d6f 7665 7320 7370  ".    Removes sp
+00003ce0: 6563 6961 6c20 6368 6172 6163 7465 7273  ecial characters
+00003cf0: 2069 6e73 6572 7465 6420 6279 2057 6f72   inserted by Wor
+00003d00: 642e 0a20 2020 2022 2222 0a20 2020 2074  d..    """.    t
+00003d10: 6578 7420 3d20 7465 7874 2e72 6570 6c61  ext = text.repla
+00003d20: 6365 2875 275c 7532 3031 3327 2c20 272d  ce(u'\u2013', '-
+00003d30: 2729 0a20 2020 2074 6578 7420 3d20 7465  ').    text = te
+00003d40: 7874 2e72 6570 6c61 6365 2875 275c 7532  xt.replace(u'\u2
+00003d50: 3032 364f 272c 2022 2722 290a 2020 2020  026O', "'").    
+00003d60: 7465 7874 203d 2074 6578 742e 7265 706c  text = text.repl
+00003d70: 6163 6528 7527 5c75 3230 3139 272c 2022  ace(u'\u2019', "
 00003d80: 2722 290a 2020 2020 7465 7874 203d 2074  '").    text = t
-00003d90: 6578 742e 7265 706c 6163 6528 7527 1827  ext.replace(u'.'
+00003d90: 6578 742e 7265 706c 6163 6528 7527 1927  ext.replace(u'.'
 00003da0: 2c20 2227 2229 0a20 2020 2074 6578 7420  , "'").    text 
 00003db0: 3d20 7465 7874 2e72 6570 6c61 6365 2875  = text.replace(u
-00003dc0: 2713 272c 2022 2d22 290a 2020 2020 7265  '.', "-").    re
-00003dd0: 7475 726e 2074 6578 740a 0a64 6566 2077  turn text..def w
-00003de0: 7261 7028 7465 7874 2c20 7769 6474 6829  rap(text, width)
-00003df0: 3a0a 2020 2020 2222 220a 2020 2020 4120  :.    """.    A 
-00003e00: 776f 7264 2d77 7261 7020 6675 6e63 7469  word-wrap functi
-00003e10: 6f6e 2074 6861 7420 7072 6573 6572 7665  on that preserve
-00003e20: 7320 6578 6973 7469 6e67 206c 696e 6520  s existing line 
-00003e30: 6272 6561 6b73 2061 6e64 206d 6f73 7420  breaks and most 
-00003e40: 7370 6163 6573 2069 6e0a 2020 2020 7468  spaces in.    th
-00003e50: 6520 7465 7874 2e20 4578 7065 6374 7320  e text. Expects 
-00003e60: 7468 6174 2065 7869 7374 696e 6720 6c69  that existing li
-00003e70: 6e65 2062 7265 616b 7320 6172 6520 706f  ne breaks are po
-00003e80: 7369 7820 6e65 776c 696e 6573 2028 5c6e  six newlines (\n
-00003e90: 292e 0a20 2020 2053 6565 2068 7474 703a  )..    See http:
-00003ea0: 2f2f 6173 706e 2e61 6374 6976 6573 7461  //aspn.activesta
-00003eb0: 7465 2e63 6f6d 2f41 5350 4e2f 436f 6f6b  te.com/ASPN/Cook
-00003ec0: 626f 6f6b 2f50 7974 686f 6e2f 5265 6369  book/Python/Reci
-00003ed0: 7065 2f31 3438 3036 310a 2020 2020 2222  pe/148061.    ""
-00003ee0: 220a 0a20 2020 2064 6566 2072 6564 7563  "..    def reduc
-00003ef0: 655f 6c69 6e65 286c 696e 652c 2077 6f72  e_line(line, wor
-00003f00: 6429 3a0a 2020 2020 2020 2020 7265 7475  d):.        retu
-00003f10: 726e 2027 2573 2573 2573 2720 2520 280a  rn '%s%s%s' % (.
-00003f20: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
-00003f30: 2c0a 2020 2020 2020 2020 2020 2020 2720  ,.            ' 
-00003f40: 5c6e 275b 0a20 2020 2020 2020 2020 2020  \n'[.           
-00003f50: 2020 2020 2028 6c65 6e28 6c69 6e65 5b6c       (len(line[l
-00003f60: 696e 652e 7266 696e 6428 275c 6e27 292b  ine.rfind('\n')+
-00003f70: 313a 5d29 202b 206c 656e 2877 6f72 642e  1:]) + len(word.
-00003f80: 7370 6c69 7428 275c 6e27 2c20 3129 5b30  split('\n', 1)[0
-00003f90: 5d29 203e 3d20 7769 6474 6829 0a20 2020  ]) >= width).   
-00003fa0: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
-00003fb0: 2020 2020 2020 2020 776f 7264 0a20 2020          word.   
-00003fc0: 2020 2020 2029 0a0a 2020 2020 7265 7475       )..    retu
-00003fd0: 726e 2072 6564 7563 6528 7265 6475 6365  rn reduce(reduce
-00003fe0: 5f6c 696e 652c 2074 6578 742e 7370 6c69  _line, text.spli
-00003ff0: 7428 2720 2729 290a 0a64 6566 2077 7261  t(' '))..def wra
-00004000: 705f 7374 7269 6e67 2873 7472 696e 672c  p_string(string,
-00004010: 206c 656e 6774 683d 3830 2c20 7365 7061   length=80, sepa
-00004020: 7261 746f 723d 275c 6e27 2c20 6261 6c61  rator='\n', bala
-00004030: 6e63 653d 4661 6c73 6529 3a0a 2020 2020  nce=False):.    
-00004040: 2727 270a 2020 2020 3e3e 3e20 7772 6170  '''.    >>> wrap
-00004050: 5f73 7472 696e 6728 7522 416e 7469 636f  _string(u"Antico
-00004060: 6e73 7469 7475 7469 6f6e 656c 6c65 6d65  nstitutionelleme
-00004070: 6e74 2c20 5061 7269 7320 7327 6576 6569  nt, Paris s'evei
-00004080: 6c6c 6522 2c20 3136 290a 2020 2020 7522  lle", 16).    u"
-00004090: 416e 7469 636f 6e73 7469 7475 7469 6f6e  Anticonstitution
-000040a0: 5c5c 6e65 6c6c 656d 656e 742c 2050 6172  \\nellement, Par
-000040b0: 6973 205c 5c6e 7327 6576 6569 6c6c 6522  is \\ns'eveille"
-000040c0: 0a20 2020 203e 3e3e 2077 7261 705f 7374  .    >>> wrap_st
-000040d0: 7269 6e67 2875 2741 6c6c 2079 6f75 2063  ring(u'All you c
-000040e0: 616e 2065 6174 272c 2031 322c 2027 5c5c  an eat', 12, '\\
-000040f0: 6e27 2c20 5472 7565 290a 2020 2020 7527  n', True).    u'
-00004100: 416c 6c20 796f 7520 5c5c 6e63 616e 2065  All you \\ncan e
-00004110: 6174 270a 2020 2020 2727 270a 2020 2020  at'.    '''.    
-00004120: 776f 7264 7320 3d20 7374 7269 6e67 2e73  words = string.s
-00004130: 706c 6974 2827 2027 290a 2020 2020 6966  plit(' ').    if
-00004140: 2062 616c 616e 6365 3a0a 2020 2020 2020   balance:.      
-00004150: 2020 2320 6261 6c61 6e63 6520 6c69 6e65    # balance line
-00004160: 733a 2074 6573 7420 6966 2073 616d 6520  s: test if same 
-00004170: 6e75 6d62 6572 206f 6620 6c69 6e65 730a  number of lines.
-00004180: 2020 2020 2020 2020 2320 6361 6e20 6265          # can be
-00004190: 2061 6368 6965 7665 6420 7769 7468 2061   achieved with a
-000041a0: 2073 686f 7274 6572 206c 696e 6520 6c65   shorter line le
-000041b0: 6e67 7468 0a20 2020 2020 2020 206c 696e  ngth.        lin
-000041c0: 6573 203d 2077 7261 705f 7374 7269 6e67  es = wrap_string
-000041d0: 2873 7472 696e 672c 206c 656e 6774 682c  (string, length,
-000041e0: 2073 6570 6172 6174 6f72 2c20 4661 6c73   separator, Fals
-000041f0: 6529 2e73 706c 6974 2873 6570 6172 6174  e).split(separat
-00004200: 6f72 290a 2020 2020 2020 2020 6966 206c  or).        if l
-00004210: 656e 286c 696e 6573 2920 3e20 313a 0a20  en(lines) > 1:. 
-00004220: 2020 2020 2020 2020 2020 2077 6869 6c65             while
-00004230: 206c 656e 6774 6820 3e20 6d61 7828 5b6c   length > max([l
-00004240: 656e 2878 2920 666f 7220 7820 696e 2077  en(x) for x in w
-00004250: 6f72 6473 5d29 3a0a 2020 2020 2020 2020  ords]):.        
-00004260: 2020 2020 2020 2020 6c65 6e67 7468 202d          length -
-00004270: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
-00004280: 2020 2020 6966 206c 656e 2877 7261 705f      if len(wrap_
-00004290: 7374 7269 6e67 2873 7472 696e 672c 206c  string(string, l
-000042a0: 656e 6774 682c 2073 6570 6172 6174 6f72  ength, separator
-000042b0: 2c20 4661 6c73 6529 2e73 706c 6974 2873  , False).split(s
-000042c0: 6570 6172 6174 6f72 2929 203e 206c 656e  eparator)) > len
-000042d0: 286c 696e 6573 293a 0a20 2020 2020 2020  (lines):.       
-000042e0: 2020 2020 2020 2020 2020 2020 206c 656e               len
-000042f0: 6774 6820 2b3d 2031 0a20 2020 2020 2020  gth += 1.       
-00004300: 2020 2020 2020 2020 2020 2020 2062 7265               bre
-00004310: 616b 0a20 2020 206c 696e 6573 203d 205b  ak.    lines = [
-00004320: 2727 5d0a 2020 2020 666f 7220 776f 7264  ''].    for word
-00004330: 2069 6e20 776f 7264 733a 0a20 2020 2020   in words:.     
-00004340: 2020 2069 6620 6c65 6e28 6c69 6e65 735b     if len(lines[
-00004350: 6c65 6e28 6c69 6e65 7329 202d 2031 5d20  len(lines) - 1] 
-00004360: 2b20 776f 7264 202b 2075 2720 2729 203c  + word + u' ') <
-00004370: 3d20 6c65 6e67 7468 202b 2031 3a0a 2020  = length + 1:.  
-00004380: 2020 2020 2020 2020 2020 2320 776f 7264            # word
-00004390: 2066 6974 7320 696e 2063 7572 7265 6e74   fits in current
-000043a0: 206c 696e 650a 2020 2020 2020 2020 2020   line.          
-000043b0: 2020 6c69 6e65 735b 6c65 6e28 6c69 6e65    lines[len(line
-000043c0: 7329 202d 2031 5d20 2b3d 2077 6f72 6420  s) - 1] += word 
-000043d0: 2b20 7527 2027 0a20 2020 2020 2020 2065  + u' '.        e
-000043e0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-000043f0: 2069 6620 6c65 6e28 776f 7264 2920 3c3d   if len(word) <=
-00004400: 206c 656e 6774 683a 0a20 2020 2020 2020   length:.       
-00004410: 2020 2020 2020 2020 2023 2077 6f72 6420           # word 
-00004420: 6669 7473 2069 6e20 6e65 7874 206c 696e  fits in next lin
-00004430: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00004440: 2020 6c69 6e65 732e 6170 7065 6e64 2877    lines.append(w
-00004450: 6f72 6420 2b20 7527 2027 290a 2020 2020  ord + u' ').    
-00004460: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00004470: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00004480: 776f 7264 2069 7320 6c6f 6e67 6572 2074  word is longer t
-00004490: 6861 6e20 6c69 6e65 0a20 2020 2020 2020  han line.       
-000044a0: 2020 2020 2020 2020 2070 6f73 6974 696f           positio
-000044b0: 6e20 3d20 6c65 6e67 7468 202d 206c 656e  n = length - len
-000044c0: 286c 696e 6573 5b6c 656e 286c 696e 6573  (lines[len(lines
-000044d0: 2920 2d20 315d 290a 2020 2020 2020 2020  ) - 1]).        
-000044e0: 2020 2020 2020 2020 6c69 6e65 735b 6c65          lines[le
-000044f0: 6e28 6c69 6e65 7329 202d 2031 5d20 2b3d  n(lines) - 1] +=
-00004500: 2077 6f72 645b 303a 706f 7369 7469 6f6e   word[0:position
-00004510: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00004520: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00004530: 2870 6f73 6974 696f 6e2c 206c 656e 2877  (position, len(w
-00004540: 6f72 6429 2c20 6c65 6e67 7468 293a 0a20  ord), length):. 
-00004550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004560: 2020 206c 696e 6573 2e61 7070 656e 6428     lines.append(
-00004570: 776f 7264 5b69 3a69 2b6c 656e 6774 685d  word[i:i+length]
-00004580: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00004590: 2020 6c69 6e65 735b 6c65 6e28 6c69 6e65    lines[len(line
-000045a0: 7329 202d 2031 5d20 2b3d 2075 2720 270a  s) - 1] += u' '.
-000045b0: 2020 2020 7265 7475 726e 2073 6570 6172      return separ
-000045c0: 6174 6f72 2e6a 6f69 6e28 6c69 6e65 7329  ator.join(lines)
-000045d0: 2e73 7472 6970 2829 0a0a 6465 6620 7472  .strip()..def tr
-000045e0: 756e 6361 7465 5f73 7472 696e 6728 7374  uncate_string(st
-000045f0: 7269 6e67 2c20 6c65 6e67 7468 2c20 7061  ring, length, pa
-00004600: 6464 696e 673d 272e 2e2e 272c 2070 6f73  dding='...', pos
-00004610: 6974 696f 6e3d 2772 6967 6874 2729 3a0a  ition='right'):.
-00004620: 2020 2020 2320 203e 3e3e 2074 7275 6e63      #  >>> trunc
-00004630: 6174 655f 7374 7269 6e67 2827 616e 7469  ate_string('anti
-00004640: 636f 6e73 7469 7475 7469 6f6e 656c 6c65  constitutionelle
-00004650: 6d65 6e74 272c 2031 362c 2027 2e2e 2e27  ment', 16, '...'
-00004660: 2c20 276c 6566 7427 290a 2020 2020 2320  , 'left').    # 
-00004670: 2027 2e2e 2e75 7469 6f6e 656c 6c65 6d65   '...utionelleme
-00004680: 6e74 270a 2020 2020 2320 203e 3e3e 2074  nt'.    #  >>> t
-00004690: 7275 6e63 6174 655f 7374 7269 6e67 2827  runcate_string('
-000046a0: 616e 7469 636f 6e73 7469 7475 7469 6f6e  anticonstitution
-000046b0: 656c 6c65 6d65 6e74 272c 2031 362c 2027  ellement', 16, '
-000046c0: 2e2e 2e27 2c20 2763 656e 7465 7227 290a  ...', 'center').
-000046d0: 2020 2020 2320 2027 616e 7469 636f 6e2e      #  'anticon.
-000046e0: 2e2e 6c65 6d65 6e74 270a 2020 2020 2320  ..lement'.    # 
-000046f0: 203e 3e3e 2074 7275 6e63 6174 655f 7374   >>> truncate_st
-00004700: 7269 6e67 2827 616e 7469 636f 6e73 7469  ring('anticonsti
-00004710: 7475 7469 6f6e 656c 6c65 6d65 6e74 272c  tutionellement',
-00004720: 2031 362c 2027 2e2e 2e27 2c20 2772 6967   16, '...', 'rig
-00004730: 6874 2729 0a20 2020 2023 2020 2761 6e74  ht').    #  'ant
-00004740: 6963 6f6e 7374 6974 7574 2e2e 2e27 0a20  iconstitut...'. 
-00004750: 2020 2073 7472 696e 674c 656e 6774 6820     stringLength 
-00004760: 3d20 6c65 6e28 7374 7269 6e67 290a 2020  = len(string).  
-00004770: 2020 7061 6464 696e 674c 656e 6774 6820    paddingLength 
-00004780: 3d20 6c65 6e28 7061 6464 696e 6729 0a20  = len(padding). 
-00004790: 2020 2069 6620 7374 7269 6e67 4c65 6e67     if stringLeng
-000047a0: 7468 203e 206c 656e 6774 683a 0a20 2020  th > length:.   
-000047b0: 2020 2020 2069 6620 706f 7369 7469 6f6e       if position
-000047c0: 203d 3d20 276c 6566 7427 3a0a 2020 2020   == 'left':.    
-000047d0: 2020 2020 2020 2020 7374 7269 6e67 203d          string =
-000047e0: 2027 2573 2573 2720 2520 2870 6164 6469   '%s%s' % (paddi
-000047f0: 6e67 2c20 7374 7269 6e67 5b73 7472 696e  ng, string[strin
-00004800: 674c 656e 6774 6820 2b20 7061 6464 696e  gLength + paddin
-00004810: 674c 656e 6774 6820 2d20 6c65 6e67 7468  gLength - length
-00004820: 3a5d 290a 2020 2020 2020 2020 656c 6966  :]).        elif
-00004830: 2070 6f73 6974 696f 6e20 3d3d 2027 6365   position == 'ce
-00004840: 6e74 6572 273a 0a20 2020 2020 2020 2020  nter':.         
-00004850: 2020 206c 6566 7420 3d20 696e 7428 6d61     left = int(ma
-00004860: 7468 2e63 6569 6c28 666c 6f61 7428 6c65  th.ceil(float(le
-00004870: 6e67 7468 202d 2070 6164 6469 6e67 4c65  ngth - paddingLe
-00004880: 6e67 7468 2920 2f20 3229 290a 2020 2020  ngth) / 2)).    
-00004890: 2020 2020 2020 2020 7269 6768 7420 3d20          right = 
-000048a0: 696e 7428 7374 7269 6e67 4c65 6e67 7468  int(stringLength
-000048b0: 202d 206d 6174 682e 666c 6f6f 7228 666c   - math.floor(fl
-000048c0: 6f61 7428 6c65 6e67 7468 202d 2070 6164  oat(length - pad
-000048d0: 6469 6e67 4c65 6e67 7468 2920 2f20 3229  dingLength) / 2)
-000048e0: 290a 2020 2020 2020 2020 2020 2020 7374  ).            st
-000048f0: 7269 6e67 203d 2027 2573 2573 2573 2720  ring = '%s%s%s' 
-00004900: 2520 2873 7472 696e 675b 3a6c 6566 745d  % (string[:left]
-00004910: 2c20 7061 6464 696e 672c 2073 7472 696e  , padding, strin
-00004920: 675b 7269 6768 743a 5d29 0a20 2020 2020  g[right:]).     
-00004930: 2020 2065 6c69 6620 706f 7369 7469 6f6e     elif position
-00004940: 203d 3d20 2772 6967 6874 273a 0a20 2020   == 'right':.   
-00004950: 2020 2020 2020 2020 2073 7472 696e 6720           string 
-00004960: 3d20 2725 7325 7327 2025 2028 7374 7269  = '%s%s' % (stri
-00004970: 6e67 5b3a 6c65 6e67 7468 202d 2070 6164  ng[:length - pad
-00004980: 6469 6e67 4c65 6e67 7468 5d2c 2070 6164  dingLength], pad
-00004990: 6469 6e67 290a 2020 2020 7265 7475 726e  ding).    return
-000049a0: 2073 7472 696e 670a 0a64 6566 2074 7275   string..def tru
-000049b0: 6e63 6174 655f 776f 7264 7328 732c 206e  ncate_words(s, n
-000049c0: 756d 293a 0a20 2020 2022 2222 5472 756e  um):.    """Trun
-000049d0: 6361 7465 7320 6120 7374 7269 6e67 2061  cates a string a
-000049e0: 6674 6572 2061 2063 6572 7461 696e 206e  fter a certain n
-000049f0: 756d 6265 7220 6f66 2063 6861 6374 6572  umber of chacter
-00004a00: 732c 2062 7574 2065 6e64 7320 7769 7468  s, but ends with
-00004a10: 2061 2077 6f72 640a 0a20 2020 203e 3e3e   a word..    >>>
-00004a20: 2074 7275 6e63 6174 655f 776f 7264 7328   truncate_words(
-00004a30: 2754 7275 6e63 6174 6573 2061 2073 7472  'Truncates a str
-00004a40: 696e 6720 6166 7465 7220 6120 6365 7274  ing after a cert
-00004a50: 6169 6e20 6e75 6d62 6572 206f 6620 6368  ain number of ch
-00004a60: 6163 7465 7273 2c20 6275 7420 656e 6473  acters, but ends
-00004a70: 2077 6974 6820 6120 776f 7264 272c 2032   with a word', 2
-00004a80: 3329 0a20 2020 2027 5472 756e 6361 7465  3).    'Truncate
-00004a90: 7320 6120 7374 7269 6e67 2e2e 2e27 0a20  s a string...'. 
-00004aa0: 2020 203e 3e3e 2074 7275 6e63 6174 655f     >>> truncate_
-00004ab0: 776f 7264 7328 2754 7275 6e63 6174 6573  words('Truncates
-00004ac0: 2061 2073 7472 696e 6727 2c20 3233 290a   a string', 23).
-00004ad0: 2020 2020 2754 7275 6e63 6174 6573 2061      'Truncates a
-00004ae0: 2073 7472 696e 6727 0a0a 2020 2020 2222   string'..    ""
-00004af0: 220a 2020 2020 6c65 6e67 7468 203d 2069  ".    length = i
-00004b00: 6e74 286e 756d 290a 2020 2020 6966 206c  nt(num).    if l
-00004b10: 656e 2873 2920 3c3d 206c 656e 6774 683a  en(s) <= length:
-00004b20: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00004b30: 730a 2020 2020 776f 7264 7320 3d20 732e  s.    words = s.
-00004b40: 7370 6c69 7428 290a 2020 2020 7473 203d  split().    ts =
-00004b50: 2022 220a 2020 2020 7768 696c 6520 776f   "".    while wo
-00004b60: 7264 7320 616e 6420 6c65 6e28 7473 2920  rds and len(ts) 
-00004b70: 2b20 6c65 6e28 776f 7264 735b 305d 2920  + len(words[0]) 
-00004b80: 3c20 6c65 6e67 7468 3a0a 2020 2020 2020  < length:.      
-00004b90: 2020 7473 202b 3d20 2220 2220 2b20 776f    ts += " " + wo
-00004ba0: 7264 732e 706f 7028 3029 0a20 2020 2069  rds.pop(0).    i
-00004bb0: 6620 776f 7264 733a 0a20 2020 2020 2020  f words:.       
-00004bc0: 2074 7320 2b3d 2022 2e2e 2e22 0a20 2020   ts += "...".   
-00004bd0: 2072 6574 7572 6e20 7473 2e73 7472 6970   return ts.strip
-00004be0: 2829 0a0a 6465 6620 7472 696d 5f73 7472  ()..def trim_str
-00004bf0: 696e 6728 7374 7269 6e67 2c20 6e75 6d29  ing(string, num)
-00004c00: 3a0a 2020 2020 2222 2254 7275 6e63 6174  :.    """Truncat
-00004c10: 6573 2061 2073 7472 696e 6720 6166 7465  es a string afte
-00004c20: 7220 6120 6365 7274 6169 6e20 6e75 6d62  r a certain numb
-00004c30: 6572 206f 6620 6368 6163 7465 7273 2c20  er of chacters, 
-00004c40: 6164 6469 6e67 202e 2e2e 2061 7420 2d31  adding ... at -1
-00004c50: 3020 6368 6172 6163 7465 7273 0a0a 2020  0 characters..  
-00004c60: 2020 3e3e 3e20 7472 696d 5f73 7472 696e    >>> trim_strin
-00004c70: 6728 2754 7275 6e63 6174 6573 2061 2073  g('Truncates a s
-00004c80: 7472 696e 6720 6166 7465 7220 6120 6365  tring after a ce
-00004c90: 7274 6169 6e20 6e75 6d62 6572 206f 6620  rtain number of 
-00004ca0: 6368 6163 7465 7273 272c 2032 3329 0a20  chacters', 23). 
-00004cb0: 2020 2027 5472 756e 6361 7465 7320 2e2e     'Truncates ..
-00004cc0: 2e66 2063 6861 6374 6572 7327 0a20 2020  .f chacters'.   
-00004cd0: 203e 3e3e 2074 7269 6d5f 7374 7269 6e67   >>> trim_string
-00004ce0: 2827 5472 756e 6361 7465 7320 6120 7374  ('Truncates a st
-00004cf0: 7269 6e67 272c 2032 3329 0a20 2020 2027  ring', 23).    '
-00004d00: 5472 756e 6361 7465 7320 6120 7374 7269  Truncates a stri
-00004d10: 6e67 270a 2020 2020 2222 220a 2020 2020  ng'.    """.    
-00004d20: 6966 206c 656e 2873 7472 696e 6729 203e  if len(string) >
-00004d30: 206e 756d 3a0a 2020 2020 2020 2020 7374   num:.        st
-00004d40: 7269 6e67 203d 2073 7472 696e 675b 3a6e  ring = string[:n
-00004d50: 756d 202d 2031 335d 202b 2027 2e2e 2e27  um - 13] + '...'
-00004d60: 202b 2073 7472 696e 675b 2d31 303a 5d0a   + string[-10:].
-00004d70: 2020 2020 7265 7475 726e 2073 7472 696e      return strin
-00004d80: 670a 0a64 6566 2067 6574 5f76 616c 6964  g..def get_valid
-00004d90: 5f66 696c 656e 616d 6528 7329 3a0a 2020  _filename(s):.  
-00004da0: 2020 2222 220a 2020 2020 5265 7475 726e    """.    Return
-00004db0: 7320 7468 6520 6769 7665 6e20 7374 7269  s the given stri
-00004dc0: 6e67 2063 6f6e 7665 7274 6564 2074 6f20  ng converted to 
-00004dd0: 6120 7374 7269 6e67 2074 6861 7420 6361  a string that ca
-00004de0: 6e20 6265 2075 7365 6420 666f 7220 6120  n be used for a 
-00004df0: 636c 6561 6e0a 2020 2020 6669 6c65 6e61  clean.    filena
-00004e00: 6d65 2e20 5370 6563 6966 6963 616c 6c79  me. Specifically
-00004e10: 2c20 6c65 6164 696e 6720 616e 6420 7472  , leading and tr
-00004e20: 6169 6c69 6e67 2073 7061 6365 7320 6172  ailing spaces ar
-00004e30: 6520 7265 6d6f 7665 643b 0a20 2020 2061  e removed;.    a
-00004e40: 6c6c 206e 6f6e 2d66 696c 656e 616d 652d  ll non-filename-
-00004e50: 7361 6665 2063 6861 7261 6374 6572 7320  safe characters 
-00004e60: 6172 6520 7265 6d6f 7665 642e 0a0a 2020  are removed...  
-00004e70: 2020 3e3e 3e20 6765 745f 7661 6c69 645f    >>> get_valid_
-00004e80: 6669 6c65 6e61 6d65 2822 6a6f 686e 2773  filename("john's
-00004e90: 2070 6f72 7472 6169 7420 696e 2032 3030   portrait in 200
-00004ea0: 342e 6a70 6722 290a 2020 2020 276a 6f68  4.jpg").    'joh
-00004eb0: 6e5f 735f 706f 7274 7261 6974 5f69 6e5f  n_s_portrait_in_
-00004ec0: 3230 3034 2e6a 7067 270a 2020 2020 2222  2004.jpg'.    ""
-00004ed0: 220a 2020 2020 7320 3d20 732e 7374 7269  ".    s = s.stri
-00004ee0: 7028 290a 2020 2020 7320 3d20 732e 7265  p().    s = s.re
-00004ef0: 706c 6163 6528 2720 272c 2027 5f27 290a  place(' ', '_').
-00004f00: 2020 2020 7320 3d20 7265 2e73 7562 2872      s = re.sub(r
-00004f10: 275b 5e2d 412d 5a61 2d7a 302d 395f 2e5c  '[^-A-Za-z0-9_.\
-00004f20: 5b5c 5d5c 205d 272c 2027 5f27 2c20 7329  [\]\ ]', '_', s)
-00004f30: 0a20 2020 2073 203d 2073 2e72 6570 6c61  .    s = s.repla
-00004f40: 6365 2827 5f5f 272c 2027 5f27 292e 7265  ce('__', '_').re
-00004f50: 706c 6163 6528 275f 5f27 2c20 275f 2729  place('__', '_')
-00004f60: 0a20 2020 2072 6574 7572 6e20 730a 0a64  .    return s..d
-00004f70: 6566 2067 6574 5f74 6578 745f 6c69 7374  ef get_text_list
-00004f80: 286c 6973 745f 2c20 6c61 7374 5f77 6f72  (list_, last_wor
-00004f90: 643d 276f 7227 293a 0a20 2020 2022 2222  d='or'):.    """
-00004fa0: 0a20 2020 203e 3e3e 2067 6574 5f74 6578  .    >>> get_tex
-00004fb0: 745f 6c69 7374 285b 7527 6127 2c20 7527  t_list([u'a', u'
-00004fc0: 6227 2c20 7527 6327 2c20 7527 6427 5d29  b', u'c', u'd'])
-00004fd0: 0a20 2020 2075 2761 2c20 622c 2063 206f  .    u'a, b, c o
-00004fe0: 7220 6427 0a20 2020 203e 3e3e 2067 6574  r d'.    >>> get
-00004ff0: 5f74 6578 745f 6c69 7374 285b 7527 6127  _text_list([u'a'
-00005000: 2c20 7527 6227 2c20 7527 6327 5d2c 2027  , u'b', u'c'], '
-00005010: 616e 6427 290a 2020 2020 7527 612c 2062  and').    u'a, b
-00005020: 2061 6e64 2063 270a 2020 2020 3e3e 3e20   and c'.    >>> 
-00005030: 6765 745f 7465 7874 5f6c 6973 7428 5b75  get_text_list([u
-00005040: 2761 272c 2075 2762 275d 2c20 2761 6e64  'a', u'b'], 'and
-00005050: 2729 0a20 2020 2075 2761 2061 6e64 2062  ').    u'a and b
-00005060: 270a 2020 2020 3e3e 3e20 6765 745f 7465  '.    >>> get_te
-00005070: 7874 5f6c 6973 7428 5b75 2761 275d 290a  xt_list([u'a']).
-00005080: 2020 2020 7527 6127 0a20 2020 203e 3e3e      u'a'.    >>>
-00005090: 2067 6574 5f74 6578 745f 6c69 7374 285b   get_text_list([
-000050a0: 5d29 0a20 2020 2027 270a 2020 2020 2222  ]).    ''.    ""
-000050b0: 220a 2020 2020 6966 206c 656e 286c 6973  ".    if len(lis
-000050c0: 745f 2920 3d3d 2030 3a0a 2020 2020 2020  t_) == 0:.      
-000050d0: 2020 7265 7475 726e 2027 270a 2020 2020    return ''.    
-000050e0: 6966 206c 656e 286c 6973 745f 2920 3d3d  if len(list_) ==
-000050f0: 2031 3a0a 2020 2020 2020 2020 7265 7475   1:.        retu
-00005100: 726e 206c 6973 745f 5b30 5d0a 2020 2020  rn list_[0].    
-00005110: 7265 7475 726e 2075 2725 7320 2573 2025  return u'%s %s %
-00005120: 7327 2025 2028 7527 2c20 272e 6a6f 696e  s' % (u', '.join
-00005130: 285b 6920 666f 7220 6920 696e 206c 6973  ([i for i in lis
-00005140: 745f 5d5b 3a2d 315d 292c 206c 6173 745f  t_][:-1]), last_
-00005150: 776f 7264 2c20 6c69 7374 5f5b 2d31 5d29  word, list_[-1])
-00005160: 0a0a 6465 6620 6765 745f 6c69 7374 5f74  ..def get_list_t
-00005170: 6578 7428 7465 7874 2c20 6c61 7374 5f77  ext(text, last_w
-00005180: 6f72 643d 276f 7227 293a 0a20 2020 2022  ord='or'):.    "
-00005190: 2222 0a20 2020 203e 3e3e 2067 6574 5f6c  "".    >>> get_l
-000051a0: 6973 745f 7465 7874 2875 2761 2c20 622c  ist_text(u'a, b,
-000051b0: 2063 206f 7220 6427 290a 2020 2020 5b75   c or d').    [u
-000051c0: 2761 272c 2075 2762 272c 2075 2763 272c  'a', u'b', u'c',
-000051d0: 2075 2764 275d 0a20 2020 203e 3e3e 2067   u'd'].    >>> g
-000051e0: 6574 5f6c 6973 745f 7465 7874 2875 2761  et_list_text(u'a
-000051f0: 2c20 6220 616e 6420 6327 2c20 7527 616e  , b and c', u'an
-00005200: 6427 290a 2020 2020 5b75 2761 272c 2075  d').    [u'a', u
-00005210: 2762 272c 2075 2763 275d 0a20 2020 203e  'b', u'c'].    >
-00005220: 3e3e 2067 6574 5f6c 6973 745f 7465 7874  >> get_list_text
-00005230: 2875 2761 2061 6e64 2062 272c 2075 2761  (u'a and b', u'a
-00005240: 6e64 2729 0a20 2020 205b 7527 6127 2c20  nd').    [u'a', 
-00005250: 7527 6227 5d0a 2020 2020 3e3e 3e20 6765  u'b'].    >>> ge
-00005260: 745f 6c69 7374 5f74 6578 7428 7527 6127  t_list_text(u'a'
-00005270: 290a 2020 2020 5b75 2761 275d 0a20 2020  ).    [u'a'].   
-00005280: 203e 3e3e 2067 6574 5f6c 6973 745f 7465   >>> get_list_te
-00005290: 7874 2875 2727 290a 2020 2020 5b5d 0a20  xt(u'').    []. 
-000052a0: 2020 2022 2222 0a20 2020 206c 6973 745f     """.    list_
-000052b0: 203d 205b 5d0a 2020 2020 6966 2074 6578   = [].    if tex
-000052c0: 743a 0a20 2020 2020 2020 206c 6973 745f  t:.        list_
-000052d0: 203d 2074 6578 742e 7370 6c69 7428 7527   = text.split(u'
-000052e0: 2c20 2729 0a20 2020 2020 2020 2069 6620  , ').        if 
-000052f0: 6c69 7374 5f3a 0a20 2020 2020 2020 2020  list_:.         
-00005300: 2020 2069 203d 206c 656e 286c 6973 745f     i = len(list_
-00005310: 292d 310a 2020 2020 2020 2020 2020 2020  )-1.            
-00005320: 6c61 7374 203d 206c 6973 745f 5b69 5d2e  last = list_[i].
-00005330: 7370 6c69 7428 6c61 7374 5f77 6f72 6429  split(last_word)
-00005340: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00005350: 6c65 6e28 6c61 7374 2920 3d3d 2032 3a0a  len(last) == 2:.
-00005360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005370: 6c69 7374 5f5b 695d 203d 206c 6173 745b  list_[i] = last[
-00005380: 305d 2e73 7472 6970 2829 0a20 2020 2020  0].strip().     
-00005390: 2020 2020 2020 2020 2020 206c 6973 745f             list_
-000053a0: 2e61 7070 656e 6428 6c61 7374 5b31 5d2e  .append(last[1].
-000053b0: 7374 7269 7028 2929 0a20 2020 2072 6574  strip()).    ret
-000053c0: 7572 6e20 6c69 7374 5f0a 0a64 6566 206e  urn list_..def n
-000053d0: 6f72 6d61 6c69 7a65 5f6e 6577 6c69 6e65  ormalize_newline
-000053e0: 7328 7465 7874 293a 0a20 2020 2072 6574  s(text):.    ret
-000053f0: 7572 6e20 7265 2e73 7562 2872 275c 725c  urn re.sub(r'\r\
-00005400: 6e7c 5c72 7c5c 6e27 2c20 275c 6e27 2c20  n|\r|\n', '\n', 
-00005410: 7465 7874 290a 0a64 6566 2072 6563 6170  text)..def recap
-00005420: 6974 616c 697a 6528 7465 7874 293a 0a20  italize(text):. 
-00005430: 2020 2022 5265 6361 7069 7461 6c69 7a65     "Recapitalize
-00005440: 7320 7465 7874 2c20 706c 6163 696e 6720  s text, placing 
-00005450: 6361 7073 2061 6674 6572 2065 6e64 2d6f  caps after end-o
-00005460: 662d 7365 6e74 656e 6365 2070 756e 6374  f-sentence punct
-00005470: 7561 7469 6f6e 2e22 0a20 2020 2023 2063  uation.".    # c
-00005480: 6170 776f 7264 7320 3d20 2829 0a20 2020  apwords = ().   
-00005490: 2074 6578 7420 3d20 7465 7874 2e6c 6f77   text = text.low
-000054a0: 6572 2829 0a20 2020 2063 6170 7352 4520  er().    capsRE 
-000054b0: 3d20 7265 2e63 6f6d 7069 6c65 2872 2728  = re.compile(r'(
-000054c0: 3f3a 5e7c 283f 3c3d 5b5c 2e5c 3f5c 215d  ?:^|(?<=[\.\?\!]
-000054d0: 2029 2928 5b61 2d7a 5d29 2729 0a20 2020   ))([a-z])').   
-000054e0: 2074 6578 7420 3d20 6361 7073 5245 2e73   text = capsRE.s
-000054f0: 7562 286c 616d 6264 6120 783a 2078 2e67  ub(lambda x: x.g
-00005500: 726f 7570 2831 292e 7570 7065 7228 292c  roup(1).upper(),
-00005510: 2074 6578 7429 0a20 2020 2023 2066 6f72   text).    # for
-00005520: 2063 6170 776f 7264 2069 6e20 6361 7077   capword in capw
-00005530: 6f72 6473 3a0a 2020 2020 2320 2020 2063  ords:.    #    c
-00005540: 6170 776f 7264 5245 203d 2072 652e 636f  apwordRE = re.co
-00005550: 6d70 696c 6528 7227 5c62 2573 5c62 2720  mpile(r'\b%s\b' 
-00005560: 2520 6361 7077 6f72 642c 2072 652e 4929  % capword, re.I)
-00005570: 0a20 2020 2023 2020 2020 7465 7874 203d  .    #    text =
-00005580: 2063 6170 776f 7264 5245 2e73 7562 2863   capwordRE.sub(c
-00005590: 6170 776f 7264 2c20 7465 7874 290a 2020  apword, text).  
-000055a0: 2020 7265 7475 726e 2074 6578 740a 0a64    return text..d
-000055b0: 6566 2070 686f 6e65 326e 756d 6572 6963  ef phone2numeric
-000055c0: 2870 686f 6e65 293a 0a20 2020 2022 436f  (phone):.    "Co
-000055d0: 6e76 6572 7473 2061 2070 686f 6e65 206e  nverts a phone n
-000055e0: 756d 6265 7220 7769 7468 206c 6574 7465  umber with lette
-000055f0: 7273 2069 6e74 6f20 6974 7320 6e75 6d65  rs into its nume
-00005600: 7269 6320 6571 7569 7661 6c65 6e74 2e22  ric equivalent."
-00005610: 0a20 2020 206c 6574 7465 7273 203d 2072  .    letters = r
-00005620: 652e 636f 6d70 696c 6528 7227 5b41 2d50  e.compile(r'[A-P
-00005630: 522d 595d 272c 2072 652e 4929 0a0a 2020  R-Y]', re.I)..  
-00005640: 2020 6465 6620 6368 6172 326e 756d 6265    def char2numbe
-00005650: 7228 6d29 3a0a 2020 2020 2020 2020 7265  r(m):.        re
-00005660: 7475 726e 207b 0a20 2020 2020 2020 2020  turn {.         
-00005670: 2020 2027 6127 3a20 2732 272c 2027 6327     'a': '2', 'c'
-00005680: 3a20 2732 272c 2027 6227 3a20 2732 272c  : '2', 'b': '2',
-00005690: 2027 6527 3a20 2733 272c 0a20 2020 2020   'e': '3',.     
-000056a0: 2020 2020 2020 2027 6427 3a20 2733 272c         'd': '3',
-000056b0: 2027 6727 3a20 2734 272c 2027 6627 3a20   'g': '4', 'f': 
-000056c0: 2733 272c 2027 6927 3a20 2734 272c 2027  '3', 'i': '4', '
-000056d0: 6827 3a20 2734 272c 2027 6b27 3a20 2735  h': '4', 'k': '5
-000056e0: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
-000056f0: 6a27 3a20 2735 272c 2027 6d27 3a20 2736  j': '5', 'm': '6
-00005700: 272c 2027 6c27 3a20 2735 272c 2027 6f27  ', 'l': '5', 'o'
-00005710: 3a20 2736 272c 2027 6e27 3a20 2736 272c  : '6', 'n': '6',
-00005720: 2027 7027 3a20 2737 272c 0a20 2020 2020   'p': '7',.     
-00005730: 2020 2020 2020 2027 7327 3a20 2737 272c         's': '7',
-00005740: 2027 7227 3a20 2737 272c 2027 7527 3a20   'r': '7', 'u': 
-00005750: 2738 272c 2027 7427 3a20 2738 272c 2027  '8', 't': '8', '
-00005760: 7727 3a20 2739 272c 2027 7627 3a20 2738  w': '9', 'v': '8
-00005770: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
-00005780: 7927 3a20 2739 272c 2027 7827 3a20 2739  y': '9', 'x': '9
-00005790: 270a 2020 2020 2020 2020 7d2e 6765 7428  '.        }.get(
-000057a0: 6d2e 6772 6f75 7028 3029 2e6c 6f77 6572  m.group(0).lower
-000057b0: 2829 290a 2020 2020 7265 7475 726e 206c  ()).    return l
-000057c0: 6574 7465 7273 2e73 7562 2863 6861 7232  etters.sub(char2
-000057d0: 6e75 6d62 6572 2c20 7068 6f6e 6529 0a0a  number, phone)..
-000057e0: 6465 6620 636f 6d70 7265 7373 5f73 7472  def compress_str
-000057f0: 696e 6728 7329 3a0a 2020 2020 696d 706f  ing(s):.    impo
-00005800: 7274 2067 7a69 700a 2020 2020 6672 6f6d  rt gzip.    from
-00005810: 2073 6978 2069 6d70 6f72 7420 4279 7465   six import Byte
-00005820: 7349 4f0a 2020 2020 7a62 7566 203d 2042  sIO.    zbuf = B
-00005830: 7974 6573 494f 2829 0a20 2020 207a 6669  ytesIO().    zfi
-00005840: 6c65 203d 2067 7a69 702e 477a 6970 4669  le = gzip.GzipFi
-00005850: 6c65 286d 6f64 653d 2777 6227 2c20 636f  le(mode='wb', co
-00005860: 6d70 7265 7373 6c65 7665 6c3d 362c 2066  mpresslevel=6, f
-00005870: 696c 656f 626a 3d7a 6275 6629 0a20 2020  ileobj=zbuf).   
-00005880: 207a 6669 6c65 2e77 7269 7465 2873 290a   zfile.write(s).
-00005890: 2020 2020 7a66 696c 652e 636c 6f73 6528      zfile.close(
-000058a0: 290a 2020 2020 7265 7475 726e 207a 6275  ).    return zbu
-000058b0: 662e 6765 7476 616c 7565 2829 0a0a 736d  f.getvalue()..sm
-000058c0: 6172 745f 7370 6c69 745f 7265 203d 2072  art_split_re = r
-000058d0: 652e 636f 6d70 696c 6528 2728 2228 3f3a  e.compile('("(?:
-000058e0: 5b5e 225c 5c5c 5c5d 2a28 3f3a 5c5c 5c5c  [^"\\\\]*(?:\\\\
-000058f0: 2e5b 5e22 5c5c 5c5c 5d2a 292a 2922 7c5c  .[^"\\\\]*)*)"|\
-00005900: 2728 3f3a 5b5e 5c27 5c5c 5c5c 5d2a 283f  '(?:[^\'\\\\]*(?
-00005910: 3a5c 5c5c 5c2e 5b5e 5c27 5c5c 5c5c 5d2a  :\\\\.[^\'\\\\]*
-00005920: 292a 295c 277c 5b5e 5c5c 735d 2b29 2729  )*)\'|[^\\s]+)')
-00005930: 0a0a 6465 6620 736d 6172 745f 7370 6c69  ..def smart_spli
-00005940: 7428 7465 7874 293a 0a20 2020 2022 2222  t(text):.    """
-00005950: 0a20 2020 2047 656e 6572 6174 6f72 2074  .    Generator t
-00005960: 6861 7420 7370 6c69 7473 2061 2073 7472  hat splits a str
-00005970: 696e 6720 6279 2073 7061 6365 732c 206c  ing by spaces, l
-00005980: 6561 7669 6e67 2071 756f 7465 6420 7068  eaving quoted ph
-00005990: 7261 7365 7320 746f 6765 7468 6572 2e0a  rases together..
-000059a0: 2020 2020 5375 7070 6f72 7473 2062 6f74      Supports bot
-000059b0: 6820 7369 6e67 6c65 2061 6e64 2064 6f75  h single and dou
-000059c0: 626c 6520 7175 6f74 6573 2c20 616e 6420  ble quotes, and 
-000059d0: 7375 7070 6f72 7473 2065 7363 6170 696e  supports escapin
-000059e0: 6720 7175 6f74 6573 2077 6974 680a 2020  g quotes with.  
-000059f0: 2020 6261 636b 736c 6173 6865 732e 2049    backslashes. I
-00005a00: 6e20 7468 6520 6f75 7470 7574 2c20 7374  n the output, st
-00005a10: 7269 6e67 7320 7769 6c6c 206b 6565 7020  rings will keep 
-00005a20: 7468 6569 7220 696e 6974 6961 6c20 616e  their initial an
-00005a30: 6420 7472 6169 6c69 6e67 0a20 2020 2071  d trailing.    q
-00005a40: 756f 7465 206d 6172 6b73 2e0a 2020 2020  uote marks..    
-00005a50: 3e3e 3e20 6c69 7374 2873 6d61 7274 5f73  >>> list(smart_s
-00005a60: 706c 6974 2827 5468 6973 2069 7320 2261  plit('This is "a
-00005a70: 2070 6572 736f 6e5c 5c27 7322 2074 6573   person\\'s" tes
-00005a80: 742e 2729 290a 2020 2020 5b27 5468 6973  t.')).    ['This
-00005a90: 272c 2027 6973 272c 2027 2261 2070 6572  ', 'is', '"a per
-00005aa0: 736f 6e5c 5c27 7322 272c 2027 7465 7374  son\\'s"', 'test
-00005ab0: 2e27 5d0a 2020 2020 2222 220a 2020 2020  .'].    """.    
-00005ac0: 666f 7220 6269 7420 696e 2073 6d61 7274  for bit in smart
-00005ad0: 5f73 706c 6974 5f72 652e 6669 6e64 6974  _split_re.findit
-00005ae0: 6572 2874 6578 7429 3a0a 2020 2020 2020  er(text):.      
-00005af0: 2020 6269 7420 3d20 6269 742e 6772 6f75    bit = bit.grou
-00005b00: 7028 3029 0a20 2020 2020 2020 2069 6620  p(0).        if 
-00005b10: 6269 745b 305d 203d 3d20 2722 273a 0a20  bit[0] == '"':. 
-00005b20: 2020 2020 2020 2020 2020 2079 6965 6c64             yield
-00005b30: 2027 2227 202b 2062 6974 5b31 3a2d 315d   '"' + bit[1:-1]
-00005b40: 2e72 6570 6c61 6365 2827 5c5c 2227 2c20  .replace('\\"', 
-00005b50: 2722 2729 2e72 6570 6c61 6365 2827 5c5c  '"').replace('\\
-00005b60: 5c5c 272c 2027 5c5c 2729 202b 2027 2227  \\', '\\') + '"'
-00005b70: 0a20 2020 2020 2020 2065 6c69 6620 6269  .        elif bi
-00005b80: 745b 305d 203d 3d20 2227 223a 0a20 2020  t[0] == "'":.   
-00005b90: 2020 2020 2020 2020 2079 6965 6c64 2022           yield "
-00005ba0: 2722 202b 2062 6974 5b31 3a2d 315d 2e72  '" + bit[1:-1].r
-00005bb0: 6570 6c61 6365 2822 5c5c 2722 2c20 2227  eplace("\\'", "'
-00005bc0: 2229 2e72 6570 6c61 6365 2822 5c5c 5c5c  ").replace("\\\\
-00005bd0: 222c 2022 5c5c 2229 202b 2022 2722 0a20  ", "\\") + "'". 
-00005be0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00005bf0: 2020 2020 2020 2020 2079 6965 6c64 2062           yield b
-00005c00: 6974 0a0a 6465 6620 776f 7264 7328 7465  it..def words(te
-00005c10: 7874 293a 0a20 2020 2022 2222 0a20 2020  xt):.    """.   
-00005c20: 2020 2020 2072 6574 7572 6e73 2077 6f72       returns wor
-00005c30: 6473 2069 6e20 7465 7874 2c20 7265 6d6f  ds in text, remo
-00005c40: 7669 6e67 2070 756e 6374 7561 7469 6f6e  ving punctuation
-00005c50: 0a20 2020 2022 2222 0a20 2020 2074 6578  .    """.    tex
-00005c60: 7420 3d20 7465 7874 2e73 706c 6974 2829  t = text.split()
-00005c70: 0a20 2020 2072 6574 7572 6e20 5b72 652e  .    return [re.
-00005c80: 7375 6228 2228 285b 2e21 3f3a 2d5f 5d7c  sub("(([.!?:-_]|
-00005c90: 2773 2924 2922 2c20 2727 2c20 7829 2066  's)$)", '', x) f
-00005ca0: 6f72 2078 2069 6e20 7465 7874 5d0a 0a64  or x in text]..d
-00005cb0: 6566 2073 6f72 745f 7374 7269 6e67 2873  ef sort_string(s
-00005cc0: 7472 696e 6729 3a0a 2020 2020 7374 7269  tring):.    stri
-00005cd0: 6e67 203d 2073 7472 696e 672e 7265 706c  ng = string.repl
-00005ce0: 6163 6528 7527 c386 272c 2027 4145 2729  ace(u'..', 'AE')
-00005cf0: 2e72 6570 6c61 6365 2875 27c3 9827 2c20  .replace(u'..', 
-00005d00: 274f 2729 2e72 6570 6c61 6365 2875 27c3  'O').replace(u'.
-00005d10: 9e27 2c20 2754 6827 290a 0a20 2020 2023  .', 'Th')..    #
-00005d20: 2070 6164 206e 756d 6265 7265 6420 7469   pad numbered ti
-00005d30: 746c 6573 0a20 2020 2073 7472 696e 6720  tles.    string 
-00005d40: 3d20 7265 2e73 7562 2827 285c 6429 2c28  = re.sub('(\d),(
-00005d50: 5c64 7b33 7d29 272c 2027 5c5c 315c 5c32  \d{3})', '\\1\\2
-00005d60: 272c 2073 7472 696e 6729 0a20 2020 2073  ', string).    s
-00005d70: 7472 696e 6720 3d20 7265 2e73 7562 2827  tring = re.sub('
-00005d80: 285c 642b 2927 2c20 6c61 6d62 6461 2078  (\d+)', lambda x
-00005d90: 3a20 2725 3031 3064 2720 2520 696e 7428  : '%010d' % int(
-00005da0: 782e 6772 6f75 7028 3029 292c 2073 7472  x.group(0)), str
-00005db0: 696e 6729 0a20 2020 2072 6574 7572 6e20  ing).    return 
-00005dc0: 756e 6963 6f64 6564 6174 612e 6e6f 726d  unicodedata.norm
-00005dd0: 616c 697a 6528 274e 464b 4427 2c20 7374  alize('NFKD', st
-00005de0: 7269 6e67 290a 0a64 6566 2073 6f72 7465  ring)..def sorte
-00005df0: 645f 7374 7269 6e67 7328 7374 7269 6e67  d_strings(string
-00005e00: 732c 206b 6579 3d4e 6f6e 6529 3a0a 2020  s, key=None):.  
-00005e10: 2020 6966 206e 6f74 206b 6579 3a0a 2020    if not key:.  
-00005e20: 2020 2020 2020 6b65 7920 3d20 736f 7274        key = sort
-00005e30: 5f73 7472 696e 670a 2020 2020 7265 7475  _string.    retu
-00005e40: 726e 2073 6f72 7465 6428 7374 7269 6e67  rn sorted(string
-00005e50: 732c 206b 6579 3d6b 6579 290a            s, key=key).
+00003dc0: 2718 272c 2022 2722 290a 2020 2020 7465  '.', "'").    te
+00003dd0: 7874 203d 2074 6578 742e 7265 706c 6163  xt = text.replac
+00003de0: 6528 7527 1327 2c20 222d 2229 0a20 2020  e(u'.', "-").   
+00003df0: 2072 6574 7572 6e20 7465 7874 0a0a 6465   return text..de
+00003e00: 6620 7772 6170 2874 6578 742c 2077 6964  f wrap(text, wid
+00003e10: 7468 293a 0a20 2020 2022 2222 0a20 2020  th):.    """.   
+00003e20: 2041 2077 6f72 642d 7772 6170 2066 756e   A word-wrap fun
+00003e30: 6374 696f 6e20 7468 6174 2070 7265 7365  ction that prese
+00003e40: 7276 6573 2065 7869 7374 696e 6720 6c69  rves existing li
+00003e50: 6e65 2062 7265 616b 7320 616e 6420 6d6f  ne breaks and mo
+00003e60: 7374 2073 7061 6365 7320 696e 0a20 2020  st spaces in.   
+00003e70: 2074 6865 2074 6578 742e 2045 7870 6563   the text. Expec
+00003e80: 7473 2074 6861 7420 6578 6973 7469 6e67  ts that existing
+00003e90: 206c 696e 6520 6272 6561 6b73 2061 7265   line breaks are
+00003ea0: 2070 6f73 6978 206e 6577 6c69 6e65 7320   posix newlines 
+00003eb0: 285c 6e29 2e0a 2020 2020 5365 6520 6874  (\n)..    See ht
+00003ec0: 7470 3a2f 2f61 7370 6e2e 6163 7469 7665  tp://aspn.active
+00003ed0: 7374 6174 652e 636f 6d2f 4153 504e 2f43  state.com/ASPN/C
+00003ee0: 6f6f 6b62 6f6f 6b2f 5079 7468 6f6e 2f52  ookbook/Python/R
+00003ef0: 6563 6970 652f 3134 3830 3631 0a20 2020  ecipe/148061.   
+00003f00: 2022 2222 0a0a 2020 2020 6465 6620 7265   """..    def re
+00003f10: 6475 6365 5f6c 696e 6528 6c69 6e65 2c20  duce_line(line, 
+00003f20: 776f 7264 293a 0a20 2020 2020 2020 2072  word):.        r
+00003f30: 6574 7572 6e20 2725 7325 7325 7327 2025  eturn '%s%s%s' %
+00003f40: 2028 0a20 2020 2020 2020 2020 2020 206c   (.            l
+00003f50: 696e 652c 0a20 2020 2020 2020 2020 2020  ine,.           
+00003f60: 2027 205c 6e27 5b0a 2020 2020 2020 2020   ' \n'[.        
+00003f70: 2020 2020 2020 2020 286c 656e 286c 696e          (len(lin
+00003f80: 655b 6c69 6e65 2e72 6669 6e64 2827 5c6e  e[line.rfind('\n
+00003f90: 2729 2b31 3a5d 2920 2b20 6c65 6e28 776f  ')+1:]) + len(wo
+00003fa0: 7264 2e73 706c 6974 2827 5c6e 272c 2031  rd.split('\n', 1
+00003fb0: 295b 305d 2920 3e3d 2077 6964 7468 290a  )[0]) >= width).
+00003fc0: 2020 2020 2020 2020 2020 2020 5d2c 0a20              ],. 
+00003fd0: 2020 2020 2020 2020 2020 2077 6f72 640a             word.
+00003fe0: 2020 2020 2020 2020 290a 0a20 2020 2072          )..    r
+00003ff0: 6574 7572 6e20 7265 6475 6365 2872 6564  eturn reduce(red
+00004000: 7563 655f 6c69 6e65 2c20 7465 7874 2e73  uce_line, text.s
+00004010: 706c 6974 2827 2027 2929 0a0a 6465 6620  plit(' '))..def 
+00004020: 7772 6170 5f73 7472 696e 6728 7374 7269  wrap_string(stri
+00004030: 6e67 2c20 6c65 6e67 7468 3d38 302c 2073  ng, length=80, s
+00004040: 6570 6172 6174 6f72 3d27 5c6e 272c 2062  eparator='\n', b
+00004050: 616c 616e 6365 3d46 616c 7365 293a 0a20  alance=False):. 
+00004060: 2020 2027 2727 0a20 2020 203e 3e3e 2077     '''.    >>> w
+00004070: 7261 705f 7374 7269 6e67 2822 416e 7469  rap_string("Anti
+00004080: 636f 6e73 7469 7475 7469 6f6e 656c 6c65  constitutionelle
+00004090: 6d65 6e74 2c20 5061 7269 7320 7327 6576  ment, Paris s'ev
+000040a0: 6569 6c6c 6522 2c20 3136 290a 2020 2020  eille", 16).    
+000040b0: 2241 6e74 6963 6f6e 7374 6974 7574 696f  "Anticonstitutio
+000040c0: 6e5c 5c6e 656c 6c65 6d65 6e74 2c20 5061  n\\nellement, Pa
+000040d0: 7269 7320 5c5c 6e73 2765 7665 696c 6c65  ris \\ns'eveille
+000040e0: 220a 2020 2020 3e3e 3e20 7772 6170 5f73  ".    >>> wrap_s
+000040f0: 7472 696e 6728 7527 416c 6c20 796f 7520  tring(u'All you 
+00004100: 6361 6e20 6561 7427 2c20 3132 2c20 275c  can eat', 12, '\
+00004110: 5c6e 272c 2054 7275 6529 0a20 2020 2027  \n', True).    '
+00004120: 416c 6c20 796f 7520 5c5c 6e63 616e 2065  All you \\ncan e
+00004130: 6174 270a 2020 2020 2727 270a 2020 2020  at'.    '''.    
+00004140: 776f 7264 7320 3d20 7374 7269 6e67 2e73  words = string.s
+00004150: 706c 6974 2827 2027 290a 2020 2020 6966  plit(' ').    if
+00004160: 2062 616c 616e 6365 3a0a 2020 2020 2020   balance:.      
+00004170: 2020 2320 6261 6c61 6e63 6520 6c69 6e65    # balance line
+00004180: 733a 2074 6573 7420 6966 2073 616d 6520  s: test if same 
+00004190: 6e75 6d62 6572 206f 6620 6c69 6e65 730a  number of lines.
+000041a0: 2020 2020 2020 2020 2320 6361 6e20 6265          # can be
+000041b0: 2061 6368 6965 7665 6420 7769 7468 2061   achieved with a
+000041c0: 2073 686f 7274 6572 206c 696e 6520 6c65   shorter line le
+000041d0: 6e67 7468 0a20 2020 2020 2020 206c 696e  ngth.        lin
+000041e0: 6573 203d 2077 7261 705f 7374 7269 6e67  es = wrap_string
+000041f0: 2873 7472 696e 672c 206c 656e 6774 682c  (string, length,
+00004200: 2073 6570 6172 6174 6f72 2c20 4661 6c73   separator, Fals
+00004210: 6529 2e73 706c 6974 2873 6570 6172 6174  e).split(separat
+00004220: 6f72 290a 2020 2020 2020 2020 6966 206c  or).        if l
+00004230: 656e 286c 696e 6573 2920 3e20 313a 0a20  en(lines) > 1:. 
+00004240: 2020 2020 2020 2020 2020 2077 6869 6c65             while
+00004250: 206c 656e 6774 6820 3e20 6d61 7828 5b6c   length > max([l
+00004260: 656e 2878 2920 666f 7220 7820 696e 2077  en(x) for x in w
+00004270: 6f72 6473 5d29 3a0a 2020 2020 2020 2020  ords]):.        
+00004280: 2020 2020 2020 2020 6c65 6e67 7468 202d          length -
+00004290: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
+000042a0: 2020 2020 6966 206c 656e 2877 7261 705f      if len(wrap_
+000042b0: 7374 7269 6e67 2873 7472 696e 672c 206c  string(string, l
+000042c0: 656e 6774 682c 2073 6570 6172 6174 6f72  ength, separator
+000042d0: 2c20 4661 6c73 6529 2e73 706c 6974 2873  , False).split(s
+000042e0: 6570 6172 6174 6f72 2929 203e 206c 656e  eparator)) > len
+000042f0: 286c 696e 6573 293a 0a20 2020 2020 2020  (lines):.       
+00004300: 2020 2020 2020 2020 2020 2020 206c 656e               len
+00004310: 6774 6820 2b3d 2031 0a20 2020 2020 2020  gth += 1.       
+00004320: 2020 2020 2020 2020 2020 2020 2062 7265               bre
+00004330: 616b 0a20 2020 206c 696e 6573 203d 205b  ak.    lines = [
+00004340: 2727 5d0a 2020 2020 666f 7220 776f 7264  ''].    for word
+00004350: 2069 6e20 776f 7264 733a 0a20 2020 2020   in words:.     
+00004360: 2020 2069 6620 6c65 6e28 6c69 6e65 735b     if len(lines[
+00004370: 6c65 6e28 6c69 6e65 7329 202d 2031 5d20  len(lines) - 1] 
+00004380: 2b20 776f 7264 202b 2027 2027 2920 3c3d  + word + ' ') <=
+00004390: 206c 656e 6774 6820 2b20 313a 0a20 2020   length + 1:.   
+000043a0: 2020 2020 2020 2020 2023 2077 6f72 6420           # word 
+000043b0: 6669 7473 2069 6e20 6375 7272 656e 7420  fits in current 
+000043c0: 6c69 6e65 0a20 2020 2020 2020 2020 2020  line.           
+000043d0: 206c 696e 6573 5b6c 656e 286c 696e 6573   lines[len(lines
+000043e0: 2920 2d20 315d 202b 3d20 776f 7264 202b  ) - 1] += word +
+000043f0: 2027 2027 0a20 2020 2020 2020 2065 6c73   ' '.        els
+00004400: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
+00004410: 6620 6c65 6e28 776f 7264 2920 3c3d 206c  f len(word) <= l
+00004420: 656e 6774 683a 0a20 2020 2020 2020 2020  ength:.         
+00004430: 2020 2020 2020 2023 2077 6f72 6420 6669         # word fi
+00004440: 7473 2069 6e20 6e65 7874 206c 696e 650a  ts in next line.
+00004450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004460: 6c69 6e65 732e 6170 7065 6e64 2877 6f72  lines.append(wor
+00004470: 6420 2b20 2720 2729 0a20 2020 2020 2020  d + ' ').       
+00004480: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00004490: 2020 2020 2020 2020 2020 2023 2077 6f72             # wor
+000044a0: 6420 6973 206c 6f6e 6765 7220 7468 616e  d is longer than
+000044b0: 206c 696e 650a 2020 2020 2020 2020 2020   line.          
+000044c0: 2020 2020 2020 706f 7369 7469 6f6e 203d        position =
+000044d0: 206c 656e 6774 6820 2d20 6c65 6e28 6c69   length - len(li
+000044e0: 6e65 735b 6c65 6e28 6c69 6e65 7329 202d  nes[len(lines) -
+000044f0: 2031 5d29 0a20 2020 2020 2020 2020 2020   1]).           
+00004500: 2020 2020 206c 696e 6573 5b6c 656e 286c       lines[len(l
+00004510: 696e 6573 2920 2d20 315d 202b 3d20 776f  ines) - 1] += wo
+00004520: 7264 5b30 3a70 6f73 6974 696f 6e5d 0a20  rd[0:position]. 
+00004530: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00004540: 6f72 2069 2069 6e20 7261 6e67 6528 706f  or i in range(po
+00004550: 7369 7469 6f6e 2c20 6c65 6e28 776f 7264  sition, len(word
+00004560: 292c 206c 656e 6774 6829 3a0a 2020 2020  ), length):.    
+00004570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004580: 6c69 6e65 732e 6170 7065 6e64 2877 6f72  lines.append(wor
+00004590: 645b 693a 692b 6c65 6e67 7468 5d29 0a20  d[i:i+length]). 
+000045a0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+000045b0: 696e 6573 5b6c 656e 286c 696e 6573 2920  ines[len(lines) 
+000045c0: 2d20 315d 202b 3d20 2720 270a 2020 2020  - 1] += ' '.    
+000045d0: 7265 7475 726e 2073 6570 6172 6174 6f72  return separator
+000045e0: 2e6a 6f69 6e28 6c69 6e65 7329 2e73 7472  .join(lines).str
+000045f0: 6970 2829 0a0a 6465 6620 7472 756e 6361  ip()..def trunca
+00004600: 7465 5f73 7472 696e 6728 7374 7269 6e67  te_string(string
+00004610: 2c20 6c65 6e67 7468 2c20 7061 6464 696e  , length, paddin
+00004620: 673d 272e 2e2e 272c 2070 6f73 6974 696f  g='...', positio
+00004630: 6e3d 2772 6967 6874 2729 3a0a 2020 2020  n='right'):.    
+00004640: 2320 203e 3e3e 2074 7275 6e63 6174 655f  #  >>> truncate_
+00004650: 7374 7269 6e67 2827 616e 7469 636f 6e73  string('anticons
+00004660: 7469 7475 7469 6f6e 656c 6c65 6d65 6e74  titutionellement
+00004670: 272c 2031 362c 2027 2e2e 2e27 2c20 276c  ', 16, '...', 'l
+00004680: 6566 7427 290a 2020 2020 2320 2027 2e2e  eft').    #  '..
+00004690: 2e75 7469 6f6e 656c 6c65 6d65 6e74 270a  .utionellement'.
+000046a0: 2020 2020 2320 203e 3e3e 2074 7275 6e63      #  >>> trunc
+000046b0: 6174 655f 7374 7269 6e67 2827 616e 7469  ate_string('anti
+000046c0: 636f 6e73 7469 7475 7469 6f6e 656c 6c65  constitutionelle
+000046d0: 6d65 6e74 272c 2031 362c 2027 2e2e 2e27  ment', 16, '...'
+000046e0: 2c20 2763 656e 7465 7227 290a 2020 2020  , 'center').    
+000046f0: 2320 2027 616e 7469 636f 6e2e 2e2e 6c65  #  'anticon...le
+00004700: 6d65 6e74 270a 2020 2020 2320 203e 3e3e  ment'.    #  >>>
+00004710: 2074 7275 6e63 6174 655f 7374 7269 6e67   truncate_string
+00004720: 2827 616e 7469 636f 6e73 7469 7475 7469  ('anticonstituti
+00004730: 6f6e 656c 6c65 6d65 6e74 272c 2031 362c  onellement', 16,
+00004740: 2027 2e2e 2e27 2c20 2772 6967 6874 2729   '...', 'right')
+00004750: 0a20 2020 2023 2020 2761 6e74 6963 6f6e  .    #  'anticon
+00004760: 7374 6974 7574 2e2e 2e27 0a20 2020 2073  stitut...'.    s
+00004770: 7472 696e 674c 656e 6774 6820 3d20 6c65  tringLength = le
+00004780: 6e28 7374 7269 6e67 290a 2020 2020 7061  n(string).    pa
+00004790: 6464 696e 674c 656e 6774 6820 3d20 6c65  ddingLength = le
+000047a0: 6e28 7061 6464 696e 6729 0a20 2020 2069  n(padding).    i
+000047b0: 6620 7374 7269 6e67 4c65 6e67 7468 203e  f stringLength >
+000047c0: 206c 656e 6774 683a 0a20 2020 2020 2020   length:.       
+000047d0: 2069 6620 706f 7369 7469 6f6e 203d 3d20   if position == 
+000047e0: 276c 6566 7427 3a0a 2020 2020 2020 2020  'left':.        
+000047f0: 2020 2020 7374 7269 6e67 203d 2027 2573      string = '%s
+00004800: 2573 2720 2520 2870 6164 6469 6e67 2c20  %s' % (padding, 
+00004810: 7374 7269 6e67 5b73 7472 696e 674c 656e  string[stringLen
+00004820: 6774 6820 2b20 7061 6464 696e 674c 656e  gth + paddingLen
+00004830: 6774 6820 2d20 6c65 6e67 7468 3a5d 290a  gth - length:]).
+00004840: 2020 2020 2020 2020 656c 6966 2070 6f73          elif pos
+00004850: 6974 696f 6e20 3d3d 2027 6365 6e74 6572  ition == 'center
+00004860: 273a 0a20 2020 2020 2020 2020 2020 206c  ':.            l
+00004870: 6566 7420 3d20 696e 7428 6d61 7468 2e63  eft = int(math.c
+00004880: 6569 6c28 666c 6f61 7428 6c65 6e67 7468  eil(float(length
+00004890: 202d 2070 6164 6469 6e67 4c65 6e67 7468   - paddingLength
+000048a0: 2920 2f20 3229 290a 2020 2020 2020 2020  ) / 2)).        
+000048b0: 2020 2020 7269 6768 7420 3d20 696e 7428      right = int(
+000048c0: 7374 7269 6e67 4c65 6e67 7468 202d 206d  stringLength - m
+000048d0: 6174 682e 666c 6f6f 7228 666c 6f61 7428  ath.floor(float(
+000048e0: 6c65 6e67 7468 202d 2070 6164 6469 6e67  length - padding
+000048f0: 4c65 6e67 7468 2920 2f20 3229 290a 2020  Length) / 2)).  
+00004900: 2020 2020 2020 2020 2020 7374 7269 6e67            string
+00004910: 203d 2027 2573 2573 2573 2720 2520 2873   = '%s%s%s' % (s
+00004920: 7472 696e 675b 3a6c 6566 745d 2c20 7061  tring[:left], pa
+00004930: 6464 696e 672c 2073 7472 696e 675b 7269  dding, string[ri
+00004940: 6768 743a 5d29 0a20 2020 2020 2020 2065  ght:]).        e
+00004950: 6c69 6620 706f 7369 7469 6f6e 203d 3d20  lif position == 
+00004960: 2772 6967 6874 273a 0a20 2020 2020 2020  'right':.       
+00004970: 2020 2020 2073 7472 696e 6720 3d20 2725       string = '%
+00004980: 7325 7327 2025 2028 7374 7269 6e67 5b3a  s%s' % (string[:
+00004990: 6c65 6e67 7468 202d 2070 6164 6469 6e67  length - padding
+000049a0: 4c65 6e67 7468 5d2c 2070 6164 6469 6e67  Length], padding
+000049b0: 290a 2020 2020 7265 7475 726e 2073 7472  ).    return str
+000049c0: 696e 670a 0a64 6566 2074 7275 6e63 6174  ing..def truncat
+000049d0: 655f 776f 7264 7328 732c 206e 756d 293a  e_words(s, num):
+000049e0: 0a20 2020 2022 2222 5472 756e 6361 7465  .    """Truncate
+000049f0: 7320 6120 7374 7269 6e67 2061 6674 6572  s a string after
+00004a00: 2061 2063 6572 7461 696e 206e 756d 6265   a certain numbe
+00004a10: 7220 6f66 2063 6861 6374 6572 732c 2062  r of chacters, b
+00004a20: 7574 2065 6e64 7320 7769 7468 2061 2077  ut ends with a w
+00004a30: 6f72 640a 0a20 2020 203e 3e3e 2074 7275  ord..    >>> tru
+00004a40: 6e63 6174 655f 776f 7264 7328 2754 7275  ncate_words('Tru
+00004a50: 6e63 6174 6573 2061 2073 7472 696e 6720  ncates a string 
+00004a60: 6166 7465 7220 6120 6365 7274 6169 6e20  after a certain 
+00004a70: 6e75 6d62 6572 206f 6620 6368 6163 7465  number of chacte
+00004a80: 7273 2c20 6275 7420 656e 6473 2077 6974  rs, but ends wit
+00004a90: 6820 6120 776f 7264 272c 2032 3329 0a20  h a word', 23). 
+00004aa0: 2020 2027 5472 756e 6361 7465 7320 6120     'Truncates a 
+00004ab0: 7374 7269 6e67 2e2e 2e27 0a20 2020 203e  string...'.    >
+00004ac0: 3e3e 2074 7275 6e63 6174 655f 776f 7264  >> truncate_word
+00004ad0: 7328 2754 7275 6e63 6174 6573 2061 2073  s('Truncates a s
+00004ae0: 7472 696e 6727 2c20 3233 290a 2020 2020  tring', 23).    
+00004af0: 2754 7275 6e63 6174 6573 2061 2073 7472  'Truncates a str
+00004b00: 696e 6727 0a0a 2020 2020 2222 220a 2020  ing'..    """.  
+00004b10: 2020 6c65 6e67 7468 203d 2069 6e74 286e    length = int(n
+00004b20: 756d 290a 2020 2020 6966 206c 656e 2873  um).    if len(s
+00004b30: 2920 3c3d 206c 656e 6774 683a 0a20 2020  ) <= length:.   
+00004b40: 2020 2020 2072 6574 7572 6e20 730a 2020       return s.  
+00004b50: 2020 776f 7264 7320 3d20 732e 7370 6c69    words = s.spli
+00004b60: 7428 290a 2020 2020 7473 203d 2022 220a  t().    ts = "".
+00004b70: 2020 2020 7768 696c 6520 776f 7264 7320      while words 
+00004b80: 616e 6420 6c65 6e28 7473 2920 2b20 6c65  and len(ts) + le
+00004b90: 6e28 776f 7264 735b 305d 2920 3c20 6c65  n(words[0]) < le
+00004ba0: 6e67 7468 3a0a 2020 2020 2020 2020 7473  ngth:.        ts
+00004bb0: 202b 3d20 2220 2220 2b20 776f 7264 732e   += " " + words.
+00004bc0: 706f 7028 3029 0a20 2020 2069 6620 776f  pop(0).    if wo
+00004bd0: 7264 733a 0a20 2020 2020 2020 2074 7320  rds:.        ts 
+00004be0: 2b3d 2022 2e2e 2e22 0a20 2020 2072 6574  += "...".    ret
+00004bf0: 7572 6e20 7473 2e73 7472 6970 2829 0a0a  urn ts.strip()..
+00004c00: 6465 6620 7472 696d 5f73 7472 696e 6728  def trim_string(
+00004c10: 7374 7269 6e67 2c20 6e75 6d29 3a0a 2020  string, num):.  
+00004c20: 2020 2222 2254 7275 6e63 6174 6573 2061    """Truncates a
+00004c30: 2073 7472 696e 6720 6166 7465 7220 6120   string after a 
+00004c40: 6365 7274 6169 6e20 6e75 6d62 6572 206f  certain number o
+00004c50: 6620 6368 6163 7465 7273 2c20 6164 6469  f chacters, addi
+00004c60: 6e67 202e 2e2e 2061 7420 2d31 3020 6368  ng ... at -10 ch
+00004c70: 6172 6163 7465 7273 0a0a 2020 2020 3e3e  aracters..    >>
+00004c80: 3e20 7472 696d 5f73 7472 696e 6728 2754  > trim_string('T
+00004c90: 7275 6e63 6174 6573 2061 2073 7472 696e  runcates a strin
+00004ca0: 6720 6166 7465 7220 6120 6365 7274 6169  g after a certai
+00004cb0: 6e20 6e75 6d62 6572 206f 6620 6368 6163  n number of chac
+00004cc0: 7465 7273 272c 2032 3329 0a20 2020 2027  ters', 23).    '
+00004cd0: 5472 756e 6361 7465 7320 2e2e 2e66 2063  Truncates ...f c
+00004ce0: 6861 6374 6572 7327 0a20 2020 203e 3e3e  hacters'.    >>>
+00004cf0: 2074 7269 6d5f 7374 7269 6e67 2827 5472   trim_string('Tr
+00004d00: 756e 6361 7465 7320 6120 7374 7269 6e67  uncates a string
+00004d10: 272c 2032 3329 0a20 2020 2027 5472 756e  ', 23).    'Trun
+00004d20: 6361 7465 7320 6120 7374 7269 6e67 270a  cates a string'.
+00004d30: 2020 2020 2222 220a 2020 2020 6966 206c      """.    if l
+00004d40: 656e 2873 7472 696e 6729 203e 206e 756d  en(string) > num
+00004d50: 3a0a 2020 2020 2020 2020 7374 7269 6e67  :.        string
+00004d60: 203d 2073 7472 696e 675b 3a6e 756d 202d   = string[:num -
+00004d70: 2031 335d 202b 2027 2e2e 2e27 202b 2073   13] + '...' + s
+00004d80: 7472 696e 675b 2d31 303a 5d0a 2020 2020  tring[-10:].    
+00004d90: 7265 7475 726e 2073 7472 696e 670a 0a64  return string..d
+00004da0: 6566 2067 6574 5f76 616c 6964 5f66 696c  ef get_valid_fil
+00004db0: 656e 616d 6528 7329 3a0a 2020 2020 2222  ename(s):.    ""
+00004dc0: 220a 2020 2020 5265 7475 726e 7320 7468  ".    Returns th
+00004dd0: 6520 6769 7665 6e20 7374 7269 6e67 2063  e given string c
+00004de0: 6f6e 7665 7274 6564 2074 6f20 6120 7374  onverted to a st
+00004df0: 7269 6e67 2074 6861 7420 6361 6e20 6265  ring that can be
+00004e00: 2075 7365 6420 666f 7220 6120 636c 6561   used for a clea
+00004e10: 6e0a 2020 2020 6669 6c65 6e61 6d65 2e20  n.    filename. 
+00004e20: 5370 6563 6966 6963 616c 6c79 2c20 6c65  Specifically, le
+00004e30: 6164 696e 6720 616e 6420 7472 6169 6c69  ading and traili
+00004e40: 6e67 2073 7061 6365 7320 6172 6520 7265  ng spaces are re
+00004e50: 6d6f 7665 643b 0a20 2020 2061 6c6c 206e  moved;.    all n
+00004e60: 6f6e 2d66 696c 656e 616d 652d 7361 6665  on-filename-safe
+00004e70: 2063 6861 7261 6374 6572 7320 6172 6520   characters are 
+00004e80: 7265 6d6f 7665 642e 0a0a 2020 2020 3e3e  removed...    >>
+00004e90: 3e20 6765 745f 7661 6c69 645f 6669 6c65  > get_valid_file
+00004ea0: 6e61 6d65 2822 6a6f 686e 2773 2070 6f72  name("john's por
+00004eb0: 7472 6169 7420 696e 2032 3030 342e 6a70  trait in 2004.jp
+00004ec0: 6722 290a 2020 2020 276a 6f68 6e5f 735f  g").    'john_s_
+00004ed0: 706f 7274 7261 6974 5f69 6e5f 3230 3034  portrait_in_2004
+00004ee0: 2e6a 7067 270a 2020 2020 2222 220a 2020  .jpg'.    """.  
+00004ef0: 2020 7320 3d20 732e 7374 7269 7028 290a    s = s.strip().
+00004f00: 2020 2020 7320 3d20 732e 7265 706c 6163      s = s.replac
+00004f10: 6528 2720 272c 2027 5f27 290a 2020 2020  e(' ', '_').    
+00004f20: 7320 3d20 7265 2e73 7562 2872 275b 5e2d  s = re.sub(r'[^-
+00004f30: 412d 5a61 2d7a 302d 395f 2e5c 5b5c 5d5c  A-Za-z0-9_.\[\]\
+00004f40: 205d 272c 2027 5f27 2c20 7329 0a20 2020   ]', '_', s).   
+00004f50: 2073 203d 2073 2e72 6570 6c61 6365 2827   s = s.replace('
+00004f60: 5f5f 272c 2027 5f27 292e 7265 706c 6163  __', '_').replac
+00004f70: 6528 275f 5f27 2c20 275f 2729 0a20 2020  e('__', '_').   
+00004f80: 2072 6574 7572 6e20 730a 0a64 6566 2067   return s..def g
+00004f90: 6574 5f74 6578 745f 6c69 7374 286c 6973  et_text_list(lis
+00004fa0: 745f 2c20 6c61 7374 5f77 6f72 643d 276f  t_, last_word='o
+00004fb0: 7227 293a 0a20 2020 2022 2222 0a20 2020  r'):.    """.   
+00004fc0: 203e 3e3e 2067 6574 5f74 6578 745f 6c69   >>> get_text_li
+00004fd0: 7374 285b 2761 272c 2027 6227 2c20 2763  st(['a', 'b', 'c
+00004fe0: 272c 2027 6427 5d29 0a20 2020 2027 612c  ', 'd']).    'a,
+00004ff0: 2062 2c20 6320 6f72 2064 270a 2020 2020   b, c or d'.    
+00005000: 3e3e 3e20 6765 745f 7465 7874 5f6c 6973  >>> get_text_lis
+00005010: 7428 5b27 6127 2c20 2762 272c 2027 6327  t(['a', 'b', 'c'
+00005020: 5d2c 2027 616e 6427 290a 2020 2020 2761  ], 'and').    'a
+00005030: 2c20 6220 616e 6420 6327 0a20 2020 203e  , b and c'.    >
+00005040: 3e3e 2067 6574 5f74 6578 745f 6c69 7374  >> get_text_list
+00005050: 285b 2761 272c 2027 6227 5d2c 2027 616e  (['a', 'b'], 'an
+00005060: 6427 290a 2020 2020 2761 2061 6e64 2062  d').    'a and b
+00005070: 270a 2020 2020 3e3e 3e20 6765 745f 7465  '.    >>> get_te
+00005080: 7874 5f6c 6973 7428 5b27 6127 5d29 0a20  xt_list(['a']). 
+00005090: 2020 2027 6127 0a20 2020 203e 3e3e 2067     'a'.    >>> g
+000050a0: 6574 5f74 6578 745f 6c69 7374 285b 5d29  et_text_list([])
+000050b0: 0a20 2020 2027 270a 2020 2020 2222 220a  .    ''.    """.
+000050c0: 2020 2020 6966 206c 656e 286c 6973 745f      if len(list_
+000050d0: 2920 3d3d 2030 3a0a 2020 2020 2020 2020  ) == 0:.        
+000050e0: 7265 7475 726e 2027 270a 2020 2020 6966  return ''.    if
+000050f0: 206c 656e 286c 6973 745f 2920 3d3d 2031   len(list_) == 1
+00005100: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00005110: 206c 6973 745f 5b30 5d0a 2020 2020 7265   list_[0].    re
+00005120: 7475 726e 2027 2573 2025 7320 2573 2720  turn '%s %s %s' 
+00005130: 2520 2827 2c20 272e 6a6f 696e 285b 6920  % (', '.join([i 
+00005140: 666f 7220 6920 696e 206c 6973 745f 5d5b  for i in list_][
+00005150: 3a2d 315d 292c 206c 6173 745f 776f 7264  :-1]), last_word
+00005160: 2c20 6c69 7374 5f5b 2d31 5d29 0a0a 6465  , list_[-1])..de
+00005170: 6620 6765 745f 6c69 7374 5f74 6578 7428  f get_list_text(
+00005180: 7465 7874 2c20 6c61 7374 5f77 6f72 643d  text, last_word=
+00005190: 276f 7227 293a 0a20 2020 2022 2222 0a20  'or'):.    """. 
+000051a0: 2020 203e 3e3e 2067 6574 5f6c 6973 745f     >>> get_list_
+000051b0: 7465 7874 2827 612c 2062 2c20 6320 6f72  text('a, b, c or
+000051c0: 2064 2729 0a20 2020 205b 2761 272c 2027   d').    ['a', '
+000051d0: 6227 2c20 2763 272c 2027 6427 5d0a 2020  b', 'c', 'd'].  
+000051e0: 2020 3e3e 3e20 6765 745f 6c69 7374 5f74    >>> get_list_t
+000051f0: 6578 7428 2761 2c20 6220 616e 6420 6327  ext('a, b and c'
+00005200: 2c20 2761 6e64 2729 0a20 2020 205b 2761  , 'and').    ['a
+00005210: 272c 2027 6227 2c20 2763 275d 0a20 2020  ', 'b', 'c'].   
+00005220: 203e 3e3e 2067 6574 5f6c 6973 745f 7465   >>> get_list_te
+00005230: 7874 2827 6120 616e 6420 6227 2c20 2761  xt('a and b', 'a
+00005240: 6e64 2729 0a20 2020 205b 2761 272c 2027  nd').    ['a', '
+00005250: 6227 5d0a 2020 2020 3e3e 3e20 6765 745f  b'].    >>> get_
+00005260: 6c69 7374 5f74 6578 7428 2761 2729 0a20  list_text('a'). 
+00005270: 2020 205b 2761 275d 0a20 2020 203e 3e3e     ['a'].    >>>
+00005280: 2067 6574 5f6c 6973 745f 7465 7874 2827   get_list_text('
+00005290: 2729 0a20 2020 205b 5d0a 2020 2020 2222  ').    [].    ""
+000052a0: 220a 2020 2020 6c69 7374 5f20 3d20 5b5d  ".    list_ = []
+000052b0: 0a20 2020 2069 6620 7465 7874 3a0a 2020  .    if text:.  
+000052c0: 2020 2020 2020 6c69 7374 5f20 3d20 7465        list_ = te
+000052d0: 7874 2e73 706c 6974 2827 2c20 2729 0a20  xt.split(', '). 
+000052e0: 2020 2020 2020 2069 6620 6c69 7374 5f3a         if list_:
+000052f0: 0a20 2020 2020 2020 2020 2020 2069 203d  .            i =
+00005300: 206c 656e 286c 6973 745f 292d 310a 2020   len(list_)-1.  
+00005310: 2020 2020 2020 2020 2020 6c61 7374 203d            last =
+00005320: 206c 6973 745f 5b69 5d2e 7370 6c69 7428   list_[i].split(
+00005330: 6c61 7374 5f77 6f72 6429 0a20 2020 2020  last_word).     
+00005340: 2020 2020 2020 2069 6620 6c65 6e28 6c61         if len(la
+00005350: 7374 2920 3d3d 2032 3a0a 2020 2020 2020  st) == 2:.      
+00005360: 2020 2020 2020 2020 2020 6c69 7374 5f5b            list_[
+00005370: 695d 203d 206c 6173 745b 305d 2e73 7472  i] = last[0].str
+00005380: 6970 2829 0a20 2020 2020 2020 2020 2020  ip().           
+00005390: 2020 2020 206c 6973 745f 2e61 7070 656e       list_.appen
+000053a0: 6428 6c61 7374 5b31 5d2e 7374 7269 7028  d(last[1].strip(
+000053b0: 2929 0a20 2020 2072 6574 7572 6e20 6c69  )).    return li
+000053c0: 7374 5f0a 0a64 6566 206e 6f72 6d61 6c69  st_..def normali
+000053d0: 7a65 5f6e 6577 6c69 6e65 7328 7465 7874  ze_newlines(text
+000053e0: 293a 0a20 2020 2072 6574 7572 6e20 7265  ):.    return re
+000053f0: 2e73 7562 2872 275c 725c 6e7c 5c72 7c5c  .sub(r'\r\n|\r|\
+00005400: 6e27 2c20 275c 6e27 2c20 7465 7874 290a  n', '\n', text).
+00005410: 0a64 6566 2072 6563 6170 6974 616c 697a  .def recapitaliz
+00005420: 6528 7465 7874 293a 0a20 2020 2022 5265  e(text):.    "Re
+00005430: 6361 7069 7461 6c69 7a65 7320 7465 7874  capitalizes text
+00005440: 2c20 706c 6163 696e 6720 6361 7073 2061  , placing caps a
+00005450: 6674 6572 2065 6e64 2d6f 662d 7365 6e74  fter end-of-sent
+00005460: 656e 6365 2070 756e 6374 7561 7469 6f6e  ence punctuation
+00005470: 2e22 0a20 2020 2023 2063 6170 776f 7264  .".    # capword
+00005480: 7320 3d20 2829 0a20 2020 2074 6578 7420  s = ().    text 
+00005490: 3d20 7465 7874 2e6c 6f77 6572 2829 0a20  = text.lower(). 
+000054a0: 2020 2063 6170 7352 4520 3d20 7265 2e63     capsRE = re.c
+000054b0: 6f6d 7069 6c65 2872 2728 3f3a 5e7c 283f  ompile(r'(?:^|(?
+000054c0: 3c3d 5b5c 2e5c 3f5c 215d 2029 2928 5b61  <=[\.\?\!] ))([a
+000054d0: 2d7a 5d29 2729 0a20 2020 2074 6578 7420  -z])').    text 
+000054e0: 3d20 6361 7073 5245 2e73 7562 286c 616d  = capsRE.sub(lam
+000054f0: 6264 6120 783a 2078 2e67 726f 7570 2831  bda x: x.group(1
+00005500: 292e 7570 7065 7228 292c 2074 6578 7429  ).upper(), text)
+00005510: 0a20 2020 2023 2066 6f72 2063 6170 776f  .    # for capwo
+00005520: 7264 2069 6e20 6361 7077 6f72 6473 3a0a  rd in capwords:.
+00005530: 2020 2020 2320 2020 2063 6170 776f 7264      #    capword
+00005540: 5245 203d 2072 652e 636f 6d70 696c 6528  RE = re.compile(
+00005550: 7227 5c62 2573 5c62 2720 2520 6361 7077  r'\b%s\b' % capw
+00005560: 6f72 642c 2072 652e 4929 0a20 2020 2023  ord, re.I).    #
+00005570: 2020 2020 7465 7874 203d 2063 6170 776f      text = capwo
+00005580: 7264 5245 2e73 7562 2863 6170 776f 7264  rdRE.sub(capword
+00005590: 2c20 7465 7874 290a 2020 2020 7265 7475  , text).    retu
+000055a0: 726e 2074 6578 740a 0a64 6566 2070 686f  rn text..def pho
+000055b0: 6e65 326e 756d 6572 6963 2870 686f 6e65  ne2numeric(phone
+000055c0: 293a 0a20 2020 2022 436f 6e76 6572 7473  ):.    "Converts
+000055d0: 2061 2070 686f 6e65 206e 756d 6265 7220   a phone number 
+000055e0: 7769 7468 206c 6574 7465 7273 2069 6e74  with letters int
+000055f0: 6f20 6974 7320 6e75 6d65 7269 6320 6571  o its numeric eq
+00005600: 7569 7661 6c65 6e74 2e22 0a20 2020 206c  uivalent.".    l
+00005610: 6574 7465 7273 203d 2072 652e 636f 6d70  etters = re.comp
+00005620: 696c 6528 7227 5b41 2d50 522d 595d 272c  ile(r'[A-PR-Y]',
+00005630: 2072 652e 4929 0a0a 2020 2020 6465 6620   re.I)..    def 
+00005640: 6368 6172 326e 756d 6265 7228 6d29 3a0a  char2number(m):.
+00005650: 2020 2020 2020 2020 7265 7475 726e 207b          return {
+00005660: 0a20 2020 2020 2020 2020 2020 2027 6127  .            'a'
+00005670: 3a20 2732 272c 2027 6327 3a20 2732 272c  : '2', 'c': '2',
+00005680: 2027 6227 3a20 2732 272c 2027 6527 3a20   'b': '2', 'e': 
+00005690: 2733 272c 0a20 2020 2020 2020 2020 2020  '3',.           
+000056a0: 2027 6427 3a20 2733 272c 2027 6727 3a20   'd': '3', 'g': 
+000056b0: 2734 272c 2027 6627 3a20 2733 272c 2027  '4', 'f': '3', '
+000056c0: 6927 3a20 2734 272c 2027 6827 3a20 2734  i': '4', 'h': '4
+000056d0: 272c 2027 6b27 3a20 2735 272c 0a20 2020  ', 'k': '5',.   
+000056e0: 2020 2020 2020 2020 2027 6a27 3a20 2735           'j': '5
+000056f0: 272c 2027 6d27 3a20 2736 272c 2027 6c27  ', 'm': '6', 'l'
+00005700: 3a20 2735 272c 2027 6f27 3a20 2736 272c  : '5', 'o': '6',
+00005710: 2027 6e27 3a20 2736 272c 2027 7027 3a20   'n': '6', 'p': 
+00005720: 2737 272c 0a20 2020 2020 2020 2020 2020  '7',.           
+00005730: 2027 7327 3a20 2737 272c 2027 7227 3a20   's': '7', 'r': 
+00005740: 2737 272c 2027 7527 3a20 2738 272c 2027  '7', 'u': '8', '
+00005750: 7427 3a20 2738 272c 2027 7727 3a20 2739  t': '8', 'w': '9
+00005760: 272c 2027 7627 3a20 2738 272c 0a20 2020  ', 'v': '8',.   
+00005770: 2020 2020 2020 2020 2027 7927 3a20 2739           'y': '9
+00005780: 272c 2027 7827 3a20 2739 270a 2020 2020  ', 'x': '9'.    
+00005790: 2020 2020 7d2e 6765 7428 6d2e 6772 6f75      }.get(m.grou
+000057a0: 7028 3029 2e6c 6f77 6572 2829 290a 2020  p(0).lower()).  
+000057b0: 2020 7265 7475 726e 206c 6574 7465 7273    return letters
+000057c0: 2e73 7562 2863 6861 7232 6e75 6d62 6572  .sub(char2number
+000057d0: 2c20 7068 6f6e 6529 0a0a 6465 6620 636f  , phone)..def co
+000057e0: 6d70 7265 7373 5f73 7472 696e 6728 7329  mpress_string(s)
+000057f0: 3a0a 2020 2020 7a62 7566 203d 2042 7974  :.    zbuf = Byt
+00005800: 6573 494f 2829 0a20 2020 207a 6669 6c65  esIO().    zfile
+00005810: 203d 2067 7a69 702e 477a 6970 4669 6c65   = gzip.GzipFile
+00005820: 286d 6f64 653d 2777 6227 2c20 636f 6d70  (mode='wb', comp
+00005830: 7265 7373 6c65 7665 6c3d 362c 2066 696c  resslevel=6, fil
+00005840: 656f 626a 3d7a 6275 6629 0a20 2020 207a  eobj=zbuf).    z
+00005850: 6669 6c65 2e77 7269 7465 2873 290a 2020  file.write(s).  
+00005860: 2020 7a66 696c 652e 636c 6f73 6528 290a    zfile.close().
+00005870: 2020 2020 7265 7475 726e 207a 6275 662e      return zbuf.
+00005880: 6765 7476 616c 7565 2829 0a0a 736d 6172  getvalue()..smar
+00005890: 745f 7370 6c69 745f 7265 203d 2072 652e  t_split_re = re.
+000058a0: 636f 6d70 696c 6528 2728 2228 3f3a 5b5e  compile('("(?:[^
+000058b0: 225c 5c5c 5c5d 2a28 3f3a 5c5c 5c5c 2e5b  "\\\\]*(?:\\\\.[
+000058c0: 5e22 5c5c 5c5c 5d2a 292a 2922 7c5c 2728  ^"\\\\]*)*)"|\'(
+000058d0: 3f3a 5b5e 5c27 5c5c 5c5c 5d2a 283f 3a5c  ?:[^\'\\\\]*(?:\
+000058e0: 5c5c 5c2e 5b5e 5c27 5c5c 5c5c 5d2a 292a  \\\.[^\'\\\\]*)*
+000058f0: 295c 277c 5b5e 5c5c 735d 2b29 2729 0a0a  )\'|[^\\s]+)')..
+00005900: 6465 6620 736d 6172 745f 7370 6c69 7428  def smart_split(
+00005910: 7465 7874 293a 0a20 2020 2022 2222 0a20  text):.    """. 
+00005920: 2020 2047 656e 6572 6174 6f72 2074 6861     Generator tha
+00005930: 7420 7370 6c69 7473 2061 2073 7472 696e  t splits a strin
+00005940: 6720 6279 2073 7061 6365 732c 206c 6561  g by spaces, lea
+00005950: 7669 6e67 2071 756f 7465 6420 7068 7261  ving quoted phra
+00005960: 7365 7320 746f 6765 7468 6572 2e0a 2020  ses together..  
+00005970: 2020 5375 7070 6f72 7473 2062 6f74 6820    Supports both 
+00005980: 7369 6e67 6c65 2061 6e64 2064 6f75 626c  single and doubl
+00005990: 6520 7175 6f74 6573 2c20 616e 6420 7375  e quotes, and su
+000059a0: 7070 6f72 7473 2065 7363 6170 696e 6720  pports escaping 
+000059b0: 7175 6f74 6573 2077 6974 680a 2020 2020  quotes with.    
+000059c0: 6261 636b 736c 6173 6865 732e 2049 6e20  backslashes. In 
+000059d0: 7468 6520 6f75 7470 7574 2c20 7374 7269  the output, stri
+000059e0: 6e67 7320 7769 6c6c 206b 6565 7020 7468  ngs will keep th
+000059f0: 6569 7220 696e 6974 6961 6c20 616e 6420  eir initial and 
+00005a00: 7472 6169 6c69 6e67 0a20 2020 2071 756f  trailing.    quo
+00005a10: 7465 206d 6172 6b73 2e0a 2020 2020 3e3e  te marks..    >>
+00005a20: 3e20 6c69 7374 2873 6d61 7274 5f73 706c  > list(smart_spl
+00005a30: 6974 2827 5468 6973 2069 7320 2261 2070  it('This is "a p
+00005a40: 6572 736f 6e5c 5c27 7322 2074 6573 742e  erson\\'s" test.
+00005a50: 2729 290a 2020 2020 5b27 5468 6973 272c  ')).    ['This',
+00005a60: 2027 6973 272c 2027 2261 2070 6572 736f   'is', '"a perso
+00005a70: 6e5c 5c27 7322 272c 2027 7465 7374 2e27  n\\'s"', 'test.'
+00005a80: 5d0a 2020 2020 2222 220a 2020 2020 666f  ].    """.    fo
+00005a90: 7220 6269 7420 696e 2073 6d61 7274 5f73  r bit in smart_s
+00005aa0: 706c 6974 5f72 652e 6669 6e64 6974 6572  plit_re.finditer
+00005ab0: 2874 6578 7429 3a0a 2020 2020 2020 2020  (text):.        
+00005ac0: 6269 7420 3d20 6269 742e 6772 6f75 7028  bit = bit.group(
+00005ad0: 3029 0a20 2020 2020 2020 2069 6620 6269  0).        if bi
+00005ae0: 745b 305d 203d 3d20 2722 273a 0a20 2020  t[0] == '"':.   
+00005af0: 2020 2020 2020 2020 2079 6965 6c64 2027           yield '
+00005b00: 2227 202b 2062 6974 5b31 3a2d 315d 2e72  "' + bit[1:-1].r
+00005b10: 6570 6c61 6365 2827 5c5c 2227 2c20 2722  eplace('\\"', '"
+00005b20: 2729 2e72 6570 6c61 6365 2827 5c5c 5c5c  ').replace('\\\\
+00005b30: 272c 2027 5c5c 2729 202b 2027 2227 0a20  ', '\\') + '"'. 
+00005b40: 2020 2020 2020 2065 6c69 6620 6269 745b         elif bit[
+00005b50: 305d 203d 3d20 2227 223a 0a20 2020 2020  0] == "'":.     
+00005b60: 2020 2020 2020 2079 6965 6c64 2022 2722         yield "'"
+00005b70: 202b 2062 6974 5b31 3a2d 315d 2e72 6570   + bit[1:-1].rep
+00005b80: 6c61 6365 2822 5c5c 2722 2c20 2227 2229  lace("\\'", "'")
+00005b90: 2e72 6570 6c61 6365 2822 5c5c 5c5c 222c  .replace("\\\\",
+00005ba0: 2022 5c5c 2229 202b 2022 2722 0a20 2020   "\\") + "'".   
+00005bb0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00005bc0: 2020 2020 2020 2079 6965 6c64 2062 6974         yield bit
+00005bd0: 0a0a 6465 6620 776f 7264 7328 7465 7874  ..def words(text
+00005be0: 293a 0a20 2020 2022 2222 0a20 2020 2020  ):.    """.     
+00005bf0: 2020 2072 6574 7572 6e73 2077 6f72 6473     returns words
+00005c00: 2069 6e20 7465 7874 2c20 7265 6d6f 7669   in text, removi
+00005c10: 6e67 2070 756e 6374 7561 7469 6f6e 0a20  ng punctuation. 
+00005c20: 2020 2022 2222 0a20 2020 2074 6578 7420     """.    text 
+00005c30: 3d20 7465 7874 2e73 706c 6974 2829 0a20  = text.split(). 
+00005c40: 2020 2072 6574 7572 6e20 5b72 652e 7375     return [re.su
+00005c50: 6228 2228 285b 2e21 3f3a 2d5f 5d7c 2773  b("(([.!?:-_]|'s
+00005c60: 2924 2922 2c20 2727 2c20 7829 2066 6f72  )$)", '', x) for
+00005c70: 2078 2069 6e20 7465 7874 5d0a 0a64 6566   x in text]..def
+00005c80: 2073 6f72 745f 7374 7269 6e67 2873 7472   sort_string(str
+00005c90: 696e 6729 3a0a 2020 2020 7374 7269 6e67  ing):.    string
+00005ca0: 203d 2073 7472 696e 672e 7265 706c 6163   = string.replac
+00005cb0: 6528 27c3 8627 2c20 2741 4527 292e 7265  e('..', 'AE').re
+00005cc0: 706c 6163 6528 27c3 9827 2c20 274f 2729  place('..', 'O')
+00005cd0: 2e72 6570 6c61 6365 2827 c39e 272c 2027  .replace('..', '
+00005ce0: 5468 2729 0a0a 2020 2020 2320 7061 6420  Th')..    # pad 
+00005cf0: 6e75 6d62 6572 6564 2074 6974 6c65 730a  numbered titles.
+00005d00: 2020 2020 7374 7269 6e67 203d 2072 652e      string = re.
+00005d10: 7375 6228 2728 5c64 292c 285c 647b 337d  sub('(\d),(\d{3}
+00005d20: 2927 2c20 275c 5c31 5c5c 3227 2c20 7374  )', '\\1\\2', st
+00005d30: 7269 6e67 290a 2020 2020 7374 7269 6e67  ring).    string
+00005d40: 203d 2072 652e 7375 6228 2728 5c64 2b29   = re.sub('(\d+)
+00005d50: 272c 206c 616d 6264 6120 783a 2027 2530  ', lambda x: '%0
+00005d60: 3130 6427 2025 2069 6e74 2878 2e67 726f  10d' % int(x.gro
+00005d70: 7570 2830 2929 2c20 7374 7269 6e67 290a  up(0)), string).
+00005d80: 2020 2020 7265 7475 726e 2075 6e69 636f      return unico
+00005d90: 6465 6461 7461 2e6e 6f72 6d61 6c69 7a65  dedata.normalize
+00005da0: 2827 4e46 4b44 272c 2073 7472 696e 6729  ('NFKD', string)
+00005db0: 0a0a 6465 6620 736f 7274 6564 5f73 7472  ..def sorted_str
+00005dc0: 696e 6773 2873 7472 696e 6773 2c20 6b65  ings(strings, ke
+00005dd0: 793d 4e6f 6e65 293a 0a20 2020 2069 6620  y=None):.    if 
+00005de0: 6e6f 7420 6b65 793a 0a20 2020 2020 2020  not key:.       
+00005df0: 206b 6579 203d 2073 6f72 745f 7374 7269   key = sort_stri
+00005e00: 6e67 0a20 2020 2072 6574 7572 6e20 736f  ng.    return so
+00005e10: 7274 6564 2873 7472 696e 6773 2c20 6b65  rted(strings, ke
+00005e20: 793d 6b65 7929 0a                        y=key).
```

### Comparing `ox-2.3.930/ox/vtt.py` & `ox-3.0.0/ox/vtt.py`

 * *Files identical despite different names*

### Comparing `ox-2.3.930/ox.egg-info/PKG-INFO` & `ox-3.0.0/ox.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 1.1
 Name: ox
-Version: 2.3.930
+Version: 3.0.0
 Summary: python-ox - the web in a dict
 Home-page: https://code.0x2620.org/0x2620/python-ox
 Author: 0x2620
 Author-email: 0x2620@0x2620.org
 License: GPLv3
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `ox-2.3.930/ox.egg-info/SOURCES.txt` & `ox-3.0.0/ox.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 ox/form.py
 ox/format.py
 ox/geo.py
 ox/html.py
 ox/image.py
 ox/iso.py
 ox/js.py
+ox/json_info.py
 ox/jsonc.py
 ox/location.py
 ox/movie.py
 ox/net.py
 ox/normalize.py
 ox/oembed.py
 ox/srt.py
@@ -25,15 +26,14 @@
 ox/vtt.py
 ox.egg-info/PKG-INFO
 ox.egg-info/SOURCES.txt
 ox.egg-info/dependency_links.txt
 ox.egg-info/requires.txt
 ox.egg-info/top_level.txt
 ox/torrent/__init__.py
-ox/torrent/bencode.py
 ox/torrent/bencode3.py
 ox/torrent/makemetafile.py
 ox/web/__init__.py
 ox/web/abebooks.py
 ox/web/allmovie.py
 ox/web/amazon.py
 ox/web/apple.py
```

### Comparing `ox-2.3.930/README.md` & `ox-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ox-2.3.930/setup.py` & `ox-3.0.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 # encoding: utf-8
 
 try:
     from setuptools import setup
 except:
     from distutils.core import setup
 
-def get_revision():
+def get_git_version():
     import subprocess
-    return subprocess.check_output(['git', 'rev-list', 'HEAD', '--count']).decode().strip()
+    version = subprocess.check_output(['git', 'describe', '--tags']).decode().strip().replace('-', '.')
+    return '.'.join((version.split('.') + ['0'])[:3])
 
 def get_version():
-    return '2.3.930' #import os
+    return '3.0.0' #import os
     import re
     _git = os.path.join(os.path.dirname(__file__), '.git')
     __version = os.path.join(os.path.dirname(__file__), 'ox/__version.py')
     changelog = os.path.join(os.path.dirname(__file__), 'debian/changelog')
     if os.path.exists(_git):
-        rev = get_revision()
-        if rev:
-            version = "2.3.%s" % rev
+        version = get_git_version()
+        if version:
             with open(__version, 'w') as fd:
                 fd.write('VERSION="%s"' % version)
             return version
     elif os.path.exists(__version):
         with open(__version) as fd:
             data = fd.read().strip().split('\n')[0]
             version = re.compile('VERSION="(.*)"').findall(data)
@@ -33,35 +33,36 @@
                 return version
     elif os.path.exists(changelog):
         f = open(changelog)
         head = f.read().strip().split('\n')[0]
         f.close()
         rev = re.compile('\d+\.\d+\.(\d+)').findall(head)
         if rev:
-            return '2.3.%s' % rev[0]
-    return '2.3.x'
+            return '3.0.%s' % rev[0]
+    return '3.0.x'
 
 
 setup(
     name="ox",
     version=get_version(),
     description="python-ox - the web in a dict",
     author="0x2620",
     author_email="0x2620@0x2620.org",
     url="https://code.0x2620.org/0x2620/python-ox",
     license="GPLv3",
     packages=['ox', 'ox.torrent', 'ox.web'],
-    install_requires=['six>=1.5.2', 'chardet'],
+    install_requires=['chardet'],
     keywords=[
     ],
     classifiers=[
         'Operating System :: OS Independent',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
 )
```

### Comparing `ox-2.3.930/PKG-INFO` & `ox-3.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 1.1
 Name: ox
-Version: 2.3.930
+Version: 3.0.0
 Summary: python-ox - the web in a dict
 Home-page: https://code.0x2620.org/0x2620/python-ox
 Author: 0x2620
 Author-email: 0x2620@0x2620.org
 License: GPLv3
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

