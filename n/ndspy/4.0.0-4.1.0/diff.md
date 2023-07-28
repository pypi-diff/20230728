# Comparing `tmp/ndspy-4.0.0.tar.gz` & `tmp/ndspy-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndspy-4.0.0.tar", last modified: Tue Mar 15 04:57:40 2022, max compression
+gzip compressed data, was "ndspy-4.1.0.tar", last modified: Fri Jul 28 08:08:54 2023, max compression
```

## Comparing `ndspy-4.0.0.tar` & `ndspy-4.1.0.tar`

### file list

```diff
@@ -1,43 +1,56 @@
-drwxrwxr-x   0 user      (1000) user      (1001)        0 2022-03-15 04:57:40.360295 ndspy-4.0.0/
--rw-rw-r--   0 user      (1000) user      (1001)    11326 2022-03-15 04:57:40.360295 ndspy-4.0.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1001)     8893 2022-03-15 04:56:28.000000 ndspy-4.0.0/README.md
-drwxrwxr-x   0 user      (1000) user      (1001)        0 2022-03-15 04:57:40.356295 ndspy-4.0.0/ndspy/
--rw-rw-r--   0 user      (1000) user      (1001)     2465 2022-03-15 04:56:28.000000 ndspy-4.0.0/ndspy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1001)    10518 2022-03-15 04:56:28.000000 ndspy-4.0.0/ndspy/_common.py
--rw-rw-r--   0 user      (1000) user      (1001)     4351 2022-03-15 04:56:28.000000 ndspy-4.0.0/ndspy/_lzCommon.py
--rw-rw-r--   0 user      (1000) user      (1001)    14756 2022-03-15 04:56:28.000000 ndspy-4.0.0/ndspy/bmg.py
--rw-rw-r--   0 user      (1000) user      (1001)     5109 2022-03-15 04:56:28.000000 ndspy-4.0.0/ndspy/bnbl.py
--rw-rw-r--   0 user      (1000) user      (1001)     3332 2022-03-15 04:56:28.000000 ndspy-4.0.0/ndspy/bncl.py
--rw-rw-r--   0 user      (1000) user      (1001)    13995 2022-03-15 04:56:28.000000 ndspy-4.0.0/ndspy/code.py
--rw-rw-r--   0 user      (1000) user      (1001)    12281 2022-03-15 04:56:28.000000 ndspy-4.0.0/ndspy/codeCompression.py
--rw-rw-r--   0 user      (1000) user      (1001)    12691 2022-03-15 04:56:28.000000 ndspy-4.0.0/ndspy/color.py
-drwxrwxr-x   0 user      (1000) user      (1001)        0 2022-03-15 04:57:40.360295 ndspy-4.0.0/ndspy/extras/
--rw-rw-r--   0 user      (1000) user      (1001)        0 2022-03-15 04:56:28.000000 ndspy-4.0.0/ndspy/extras/__init__.py
--rw-rw-r--   0 user      (1000) user      (1001)    30738 2022-03-15 04:56:28.000000 ndspy-4.0.0/ndspy/extras/music.py
--rw-rw-r--   0 user      (1000) user      (1001)        0 2022-03-15 04:56:28.000000 ndspy-4.0.0/ndspy/extras/soundEffect.py
--rw-rw-r--   0 user      (1000) user      (1001)    13244 2022-03-15 04:56:28.000000 ndspy-4.0.0/ndspy/fnt.py
--rw-rw-r--   0 user      (1000) user      (1001)    15848 2022-03-15 04:56:28.000000 ndspy-4.0.0/ndspy/graphics2D.py
--rw-rw-r--   0 user      (1000) user      (1001)     5453 2022-03-15 04:56:28.000000 ndspy-4.0.0/ndspy/lz10.py
--rw-rw-r--   0 user      (1000) user      (1001)    21582 2022-03-15 04:56:28.000000 ndspy-4.0.0/ndspy/model.py
--rw-rw-r--   0 user      (1000) user      (1001)     6842 2022-03-15 04:56:28.000000 ndspy-4.0.0/ndspy/narc.py
--rw-rw-r--   0 user      (1000) user      (1001)    21090 2022-03-15 04:56:28.000000 ndspy-4.0.0/ndspy/rom.py
--rw-rw-r--   0 user      (1000) user      (1001)    31471 2022-03-15 04:56:28.000000 ndspy-4.0.0/ndspy/soundArchive.py
--rw-rw-r--   0 user      (1000) user      (1001)    27323 2022-03-15 04:56:28.000000 ndspy-4.0.0/ndspy/soundBank.py
--rw-rw-r--   0 user      (1000) user      (1001)     4178 2022-03-15 04:56:28.000000 ndspy-4.0.0/ndspy/soundGroup.py
--rw-rw-r--   0 user      (1000) user      (1001)    48487 2022-03-15 04:56:28.000000 ndspy-4.0.0/ndspy/soundSequence.py
--rw-rw-r--   0 user      (1000) user      (1001)    11692 2022-03-15 04:56:28.000000 ndspy-4.0.0/ndspy/soundSequenceArchive.py
--rw-rw-r--   0 user      (1000) user      (1001)     1566 2022-03-15 04:56:28.000000 ndspy-4.0.0/ndspy/soundSequencePlayer.py
--rw-rw-r--   0 user      (1000) user      (1001)    10413 2022-03-15 04:56:28.000000 ndspy-4.0.0/ndspy/soundStream.py
--rw-rw-r--   0 user      (1000) user      (1001)     1337 2022-03-15 04:56:28.000000 ndspy-4.0.0/ndspy/soundStreamPlayer.py
--rw-rw-r--   0 user      (1000) user      (1001)     4931 2022-03-15 04:56:28.000000 ndspy-4.0.0/ndspy/soundWave.py
--rw-rw-r--   0 user      (1000) user      (1001)     5107 2022-03-15 04:56:28.000000 ndspy-4.0.0/ndspy/soundWaveArchive.py
--rw-rw-r--   0 user      (1000) user      (1001)    26474 2022-03-15 04:56:28.000000 ndspy-4.0.0/ndspy/texture.py
-drwxrwxr-x   0 user      (1000) user      (1001)        0 2022-03-15 04:57:40.360295 ndspy-4.0.0/ndspy.egg-info/
--rw-rw-r--   0 user      (1000) user      (1001)    11326 2022-03-15 04:57:40.000000 ndspy-4.0.0/ndspy.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1001)      760 2022-03-15 04:57:40.000000 ndspy-4.0.0/ndspy.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1001)        1 2022-03-15 04:57:40.000000 ndspy-4.0.0/ndspy.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1001)       99 2022-03-15 04:57:40.000000 ndspy-4.0.0/ndspy.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1001)        7 2022-03-15 04:57:40.000000 ndspy-4.0.0/ndspy.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1001)        6 2022-03-15 04:57:40.000000 ndspy-4.0.0/ndspy.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1001)       38 2022-03-15 04:57:40.360295 ndspy-4.0.0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1001)     1196 2022-03-15 04:56:28.000000 ndspy-4.0.0/setup.py
+drwxrwxr-x   0 user      (1000) user      (1001)        0 2023-07-28 08:08:54.390610 ndspy-4.1.0/
+-rw-rw-r--   0 user      (1000) user      (1001)    35148 2019-01-18 06:16:50.000000 ndspy-4.1.0/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1001)     9608 2023-07-28 08:08:54.390610 ndspy-4.1.0/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1001)     8814 2023-04-15 04:35:13.000000 ndspy-4.1.0/README.md
+drwxrwxr-x   0 user      (1000) user      (1001)        0 2023-07-28 08:08:54.382610 ndspy-4.1.0/ndspy/
+-rw-rw-r--   0 user      (1000) user      (1001)     2465 2023-07-28 08:02:12.000000 ndspy-4.1.0/ndspy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1001)    10655 2023-04-15 04:35:13.000000 ndspy-4.1.0/ndspy/_common.py
+-rw-rw-r--   0 user      (1000) user      (1001)     4351 2019-01-18 06:22:19.000000 ndspy-4.1.0/ndspy/_lzCommon.py
+-rw-rw-r--   0 user      (1000) user      (1001)    14756 2020-01-01 01:45:28.000000 ndspy-4.1.0/ndspy/bmg.py
+-rw-rw-r--   0 user      (1000) user      (1001)     5109 2019-02-07 21:55:13.000000 ndspy-4.1.0/ndspy/bnbl.py
+-rw-rw-r--   0 user      (1000) user      (1001)     3332 2019-02-07 21:55:13.000000 ndspy-4.1.0/ndspy/bncl.py
+-rw-rw-r--   0 user      (1000) user      (1001)    13995 2020-09-14 00:06:34.000000 ndspy-4.1.0/ndspy/code.py
+-rw-rw-r--   0 user      (1000) user      (1001)    12281 2022-03-15 04:45:34.000000 ndspy-4.1.0/ndspy/codeCompression.py
+-rw-rw-r--   0 user      (1000) user      (1001)    12691 2022-03-15 04:54:55.000000 ndspy-4.1.0/ndspy/color.py
+drwxrwxr-x   0 user      (1000) user      (1001)        0 2023-07-28 08:08:54.386610 ndspy-4.1.0/ndspy/extras/
+-rw-rw-r--   0 user      (1000) user      (1001)        0 2018-07-02 02:55:01.000000 ndspy-4.1.0/ndspy/extras/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1001)    15977 2019-03-10 22:46:26.000000 ndspy-4.1.0/ndspy/extras/_imageTexeler.py
+-rw-rw-r--   0 user      (1000) user      (1001)    30738 2019-05-30 00:49:09.000000 ndspy-4.1.0/ndspy/extras/music.py
+-rw-rw-r--   0 user      (1000) user      (1001)        0 2018-07-02 02:55:01.000000 ndspy-4.1.0/ndspy/extras/soundEffect.py
+-rw-rw-r--   0 user      (1000) user      (1001)    21460 2019-03-22 01:20:20.000000 ndspy-4.1.0/ndspy/extras/textureEncoding.py
+drwxrwxr-x   0 user      (1000) user      (1001)        0 2023-07-28 08:08:54.386610 ndspy-4.1.0/ndspy/extras/wbmgt/
+-rw-rw-r--   0 user      (1000) user      (1001)     2052 2020-01-20 01:54:23.000000 ndspy-4.1.0/ndspy/extras/wbmgt/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1001)      989 2020-01-01 08:37:29.000000 ndspy-4.1.0/ndspy/extras/wbmgt/_common.py
+-rw-rw-r--   0 user      (1000) user      (1001)    26429 2020-03-16 19:03:47.000000 ndspy-4.1.0/ndspy/extras/wbmgt/_load.py
+-rw-rw-r--   0 user      (1000) user      (1001)    10463 2020-03-15 23:13:05.000000 ndspy-4.1.0/ndspy/extras/wbmgt/_save.py
+-rw-rw-r--   0 user      (1000) user      (1001)    13244 2019-11-24 05:30:48.000000 ndspy-4.1.0/ndspy/fnt.py
+-rw-rw-r--   0 user      (1000) user      (1001)    15872 2023-02-12 00:55:46.000000 ndspy-4.1.0/ndspy/graphics2D.py
+-rw-rw-r--   0 user      (1000) user      (1001)     5453 2020-01-22 02:59:48.000000 ndspy-4.1.0/ndspy/lz10.py
+-rw-rw-r--   0 user      (1000) user      (1001)    21582 2019-02-09 05:18:04.000000 ndspy-4.1.0/ndspy/model.py
+-rw-rw-r--   0 user      (1000) user      (1001)     6842 2019-11-24 04:29:03.000000 ndspy-4.1.0/ndspy/narc.py
+-rw-rw-r--   0 user      (1000) user      (1001)    21090 2020-09-07 09:29:10.000000 ndspy-4.1.0/ndspy/rom.py
+-rw-rw-r--   0 user      (1000) user      (1001)    31471 2019-11-24 04:28:16.000000 ndspy-4.1.0/ndspy/soundArchive.py
+-rw-rw-r--   0 user      (1000) user      (1001)    27323 2019-11-24 04:35:13.000000 ndspy-4.1.0/ndspy/soundBank.py
+-rw-rw-r--   0 user      (1000) user      (1001)     4178 2019-01-18 06:22:59.000000 ndspy-4.1.0/ndspy/soundGroup.py
+-rw-rw-r--   0 user      (1000) user      (1001)    48487 2020-11-15 22:33:58.000000 ndspy-4.1.0/ndspy/soundSequence.py
+-rw-rw-r--   0 user      (1000) user      (1001)    11692 2019-11-24 04:28:34.000000 ndspy-4.1.0/ndspy/soundSequenceArchive.py
+-rw-rw-r--   0 user      (1000) user      (1001)     1566 2019-01-18 06:23:21.000000 ndspy-4.1.0/ndspy/soundSequencePlayer.py
+-rw-rw-r--   0 user      (1000) user      (1001)    10413 2019-11-24 04:36:53.000000 ndspy-4.1.0/ndspy/soundStream.py
+-rw-rw-r--   0 user      (1000) user      (1001)     1337 2019-01-18 06:23:34.000000 ndspy-4.1.0/ndspy/soundStreamPlayer.py
+-rw-rw-r--   0 user      (1000) user      (1001)     4931 2019-11-24 04:49:47.000000 ndspy-4.1.0/ndspy/soundWave.py
+-rw-rw-r--   0 user      (1000) user      (1001)     5107 2019-11-24 04:44:49.000000 ndspy-4.1.0/ndspy/soundWaveArchive.py
+-rw-rw-r--   0 user      (1000) user      (1001)    26474 2019-11-24 04:30:02.000000 ndspy-4.1.0/ndspy/texture.py
+drwxrwxr-x   0 user      (1000) user      (1001)        0 2023-07-28 08:08:54.386610 ndspy-4.1.0/ndspy.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1001)     9608 2023-07-28 08:08:54.000000 ndspy-4.1.0/ndspy.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1001)     1049 2023-07-28 08:08:54.000000 ndspy-4.1.0/ndspy.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1001)        1 2023-07-28 08:08:54.000000 ndspy-4.1.0/ndspy.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1001)       98 2023-07-28 08:08:54.000000 ndspy-4.1.0/ndspy.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1001)        6 2023-07-28 08:08:54.000000 ndspy-4.1.0/ndspy.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1001)       38 2023-07-28 08:08:54.390610 ndspy-4.1.0/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1001)     1198 2023-07-28 08:04:13.000000 ndspy-4.1.0/setup.py
+drwxrwxr-x   0 user      (1000) user      (1001)        0 2023-07-28 08:08:54.390610 ndspy-4.1.0/tests/
+-rw-rw-r--   0 user      (1000) user      (1001)    20817 2020-01-01 09:24:24.000000 ndspy-4.1.0/tests/test_bmg.py
+-rw-rw-r--   0 user      (1000) user      (1001)     9016 2020-03-15 20:42:38.000000 ndspy-4.1.0/tests/test_extras_wbmgt.py
+-rw-rw-r--   0 user      (1000) user      (1001)    18694 2020-03-15 23:02:18.000000 ndspy-4.1.0/tests/test_extras_wbmgt__load.py
+-rw-rw-r--   0 user      (1000) user      (1001)     5871 2020-03-15 23:05:31.000000 ndspy-4.1.0/tests/test_extras_wbmgt__save.py
+-rw-rw-r--   0 user      (1000) user      (1001)     2651 2019-11-24 06:02:09.000000 ndspy-4.1.0/tests/test_main.py
```

### Comparing `ndspy-4.0.0/PKG-INFO` & `ndspy-4.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,227 +1,226 @@
 Metadata-Version: 2.1
 Name: ndspy
-Version: 4.0.0
+Version: 4.1.0
 Summary: Python library that can help you read, modify and create many types of files used in Nintendo DS games.
 Home-page: https://github.com/RoadrunnerWMC/ndspy
 Author: RoadrunnerWMC
 Author-email: roadrunnerwmc@gmail.com
-License: UNKNOWN
-Description: ndspy
-        =====
-        
-        [![Discord](https://img.shields.io/discord/534221996230180884.svg?logo=discord&logoColor=white&colorB=7289da)](https://discord.gg/RQhxAxw)
-        [![Documentation](https://img.shields.io/badge/documentation-Read%20the%20Docs-brightgreen.svg?logo=read%20the%20docs&logoColor=white)](http://ndspy.readthedocs.io/)
-        [![PyPI](https://img.shields.io/pypi/v/ndspy.svg?logo=python&logoColor=white)](https://pypi.org/project/ndspy/)
-        [![License: GNU GPL 3.0](https://img.shields.io/github/license/RoadrunnerWMC/ndspy.svg?logo=gnu&logoColor=white)](https://www.gnu.org/licenses/gpl-3.0)
-        
-        **ndspy** ("en-dee-ESS-pie") is a Python library and suite of command-line
-        tools that can help you read, modify and create many types of files used in
-        Nintendo DS games.
-        
-        ndspy follows a few key design principles:
-        
-        -   **Accuracy**: ndspy should be able to open and resave any supported file
-            with byte-for-byte accuracy if it's in its canonical format.
-        -   **Flexibility**: ndspy should be able to read any valid file in a format it
-            supports. In cases where there's a high chance it will be unable to fully
-            interpret some especially complex part of a file, it should still be useful
-            for editing the other parts.
-        -   **Semantic**: ndspy's APIs should closely match the semantics of file
-            structures while hiding their binary-level details.
-        
-        ndspy provides both a Python API and a set of simple command-line tools that
-        make use of it. The command-line tools let you convert files to and from binary
-        formats without having to write any Python code yourself. The API is suitable
-        for use in applications written in Python, and in scripts to do more complex
-        tasks than the command-line tools are capable of.
-        
-        As ndspy is written in pure Python, it is cross-platform and should run on all
-        platforms Python supports. Note that Python doesn't support the Nintendo DS
-        itself; ndspy is intended to be used on your PC.
-        
-        Interested? Read on to see some examples, or check the [API
-        Reference](https://ndspy.readthedocs.io/en/latest/api/index.html) to see the
-        documentation for a specific module. When you're ready to install, head over to
-        the [Installation](#installation) section!
-        
-        
-        
-        A few examples of ndspy in action
-        ---------------------------------
-        
-        Create a *BMG* file containing message strings:
-        
-        ```python
-        >>> import ndspy.bmg
-        >>> message1 = ndspy.bmg.Message(b'', ['Open your eyes...'])
-        >>> message2 = ndspy.bmg.Message(b'', ['Wake up, Link...'])
-        >>> bmg = ndspy.bmg.BMG.fromMessages([message1, message2])
-        >>> bmg.save()
-        b'MESGbmg1\xa0\x00\x00\x00\x02\x00\x00\x00\x02\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00INF1 \x00\x00\x00\x02\x00\x04\x00\x00\x00\x00\x00\x02\x00\x00\x00&\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00DAT1`\x00\x00\x00\x00\x00O\x00p\x00e\x00n\x00 \x00y\x00o\x00u\x00r\x00 \x00e\x00y\x00e\x00s\x00.\x00.\x00.\x00\x00\x00W\x00a\x00k\x00e\x00 \x00u\x00p\x00,\x00 \x00L\x00i\x00n\x00k\x00.\x00.\x00.\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00'
-        >>>
-        ```
-        
-        Change all notes in a *SSEQ* sequenced music file to middle C, similar to [this
-        song](https://youtu.be/cSAp9sBzPbc):
-        
-        ```python
-        >>> import ndspy.soundSequence
-        >>> song = ndspy.soundSequence.SSEQ.fromFile('never-gonna-give-you-up.sseq')
-        >>> song.parse()
-        >>> for event in song.events:
-        ...     if isinstance(event, ndspy.soundSequence.NoteSequenceEvent):
-        ...         event.pitch = 60
-        ...
-        >>> song.saveToFile('never-gonna-give-you-up-but-all-the-notes-are-c.sseq')
-        >>>
-        ```
-        
-        Compress and decompress data using the *LZ10* compression format:
-        
-        ```python
-        >>> import ndspy.lz10
-        >>> compressed = ndspy.lz10.compress(b'This is some data to compress')
-        >>> compressed
-        b'\x10\x1d\x00\x00\x04This \x00\x02so\x00me data \x00to compr\x00ess\x00\x00\x00\x00\x00'
-        >>> ndspy.lz10.decompress(compressed)
-        b'This is some data to compress'
-        >>>
-        ```
-        
-        Search for all files starting with a particular byte sequence in a ROM:
-        
-        ```python
-        >>> import ndspy.rom
-        >>> rom = ndspy.rom.NintendoDSRom.fromFile('nsmb.nds')
-        >>> for i, file in enumerate(rom.files):
-        ...     if file.startswith(b'BMD0'):
-        ...         print(rom.filenames[i] + ' is a NSBMD model')
-        ...
-        demo/end_kp.nsbmd is a NSBMD model
-        demo/staffroll.nsbmd is a NSBMD model
-        demo/staffroll_back.nsbmd is a NSBMD model
-        enemy/A_jiku.nsbmd is a NSBMD model
-        enemy/all_goal_flag.nsbmd is a NSBMD model
-        ...
-        map/world7.nsbmd is a NSBMD model
-        map/world8.nsbmd is a NSBMD model
-        >>>
-        ```
-        
-        
-        Misconceptions
-        --------------
-        
-        Still a little confused about what exactly ndspy is or what it's capable of?
-        This section will try to answer some questions you may have.
-        
-        -   ndspy is a *library*, not a *program.* To use ndspy, you have to write your
-            own Python code; ndspy is essentially a tool your code can use. This may
-            sound daunting -- especially if you're not very familiar with Python -- but
-            the
-            [tutorials](https://ndspy.readthedocs.io/en/latest/tutorials/index.html)
-            walk you through this process step-by-step for some common tasks. In the
-            future, I plan to add some command-line and maybe even GUI tools powered by
-            ndspy, but until then, this is how you use it.
-        -   ndspy runs on your PC, not on the Nintendo DS itself. You use it to create
-            and modify game files, which can then be run on the console. DS games have
-            to be written in a compiled language such as C or C++ to have any hope of
-            being efficient; Python will never be a serious option there,
-            unfortunately.
-        -   ndspy doesn't support every type of file used in every DS game. In fact,
-            for any given game, it's likely that the majority of the game's files
-            *won't* be supported by ndspy. There's a huge amount of variety in video
-            game file formats, and it would be impossible to support them all. ndspy
-            focuses on file formats used in many games, especially first-party ones.
-            Support for formats that are specific to a particular game would best
-            belong in a separate Python library instead.
-        
-            That said, certain parts of ndspy (such as its support for ROM files and
-            raw texture data) have to do with the console's hardware rather than its
-            software, and thus should be relevant to most or all games.
-        
-        
-        <a name="installation"></a>
-        Installation
-        ------------
-        
-        ndspy requires Python 3.6 or newer to run. CPython (the reference
-        implementation of Python) and PyPy are both supported. Python 2, though, is not
-        supported at all.
-        
-        The easiest way to get the latest stable release of ndspy is through PyPI using
-        pip.
-        
-        pip is a command-line application, so you'll need to use the Windows command
-        prompt or bash to do this. The exact command you need to enter depends on your
-        operating system and the settings you chose when you installed Python. One of
-        the following possibilities will probably work for you, though:
-        
-            pip install ndspy
-        
-            python3 -m pip install ndspy
-        
-            py -3 -m pip install ndspy
-        
-        If you want the very latest version of ndspy including features and bugfixes
-        not yet in any official release, you can also download the code from the
-        [GitHub repository](https://github.com/RoadrunnerWMC/ndspy) and install it
-        manually. Note that [crcmod](https://pypi.org/project/crcmod/) is a required
-        dependency.
-        
-        
-        Documentation
-        -------------
-        
-        [ndspy's documentation is hosted on Read the
-        Docs](https://ndspy.readthedocs.io/en/latest/index.html), and the documentation
-        source code can be found in the ``docs/`` folder in this repository. In
-        addition to the [API
-        reference](https://ndspy.readthedocs.io/en/latest/api/index.html), there are
-        also
-        [examples](https://ndspy.readthedocs.io/en/latest/index.html#a-few-examples-of-ndspy-in-action)
-        and [tutorials](https://ndspy.readthedocs.io/en/latest/tutorials/index.html) to
-        help you out!
-        
-        
-        Support
-        -------
-        
-        I spent a long time writing the documentation for ndspy, so first please
-        double-check that your question isn't already answered in the [API
-        reference](https://ndspy.readthedocs.io/en/latest/api/index.html) or
-        [Tutorials](https://ndspy.readthedocs.io/en/latest/tutorials/index.html)
-        sections in the documentation.
-        
-        If that doesn't help, you can ask me (RoadrunnerWMC) your questions via [the
-        ndspy Discord server](https://discord.gg/RQhxAxw). I'll try to get back to
-        you as quickly as I can!
-        
-        If you think you've found a bug in ndspy, please [file an issue on
-        GitHub](https://github.com/RoadrunnerWMC/ndspy/issues/new). Thanks!
-        
-        
-        Versioning
-        ----------
-        
-        ndspy follows [semantic versioning](https://semver.org/) to the best of my
-        ability. If a tool claims to work with ndspy 1.0.2, it should also work with
-        ndspy 1.2.0, but not necessarily 2.0.0. (Please note that not all of those
-        version numbers actually exist!)
-        
-        Undocumented modules are considered exempt from semantic versioning, and are
-        subject to drastic changes at any time. This is also mentioned in the
-        [Undocumented
-        APIs](https://ndspy.readthedocs.io/en/latest/api/index.html#undocumented-apis)
-        section of the documentation.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+ndspy
+=====
+
+[![Discord](https://img.shields.io/discord/534221996230180884.svg?logo=discord&logoColor=white&colorB=7289da)](https://discord.gg/RQhxAxw)
+[![Documentation](https://img.shields.io/badge/documentation-Read%20the%20Docs-brightgreen.svg?logo=read%20the%20docs&logoColor=white)](http://ndspy.readthedocs.io/)
+[![PyPI](https://img.shields.io/pypi/v/ndspy.svg?logo=python&logoColor=white)](https://pypi.org/project/ndspy/)
+[![License: GNU GPL 3.0](https://img.shields.io/github/license/RoadrunnerWMC/ndspy.svg?logo=gnu&logoColor=white)](https://www.gnu.org/licenses/gpl-3.0)
+
+**ndspy** ("en-dee-ESS-pie") is a Python library and suite of command-line
+tools that can help you read, modify and create many types of files used in
+Nintendo DS games.
+
+ndspy follows a few key design principles:
+
+-   **Accuracy**: ndspy should be able to open and resave any supported file
+    with byte-for-byte accuracy if it's in its canonical format.
+-   **Flexibility**: ndspy should be able to read any valid file in a format it
+    supports. In cases where there's a high chance it will be unable to fully
+    interpret some especially complex part of a file, it should still be useful
+    for editing the other parts.
+-   **Semantic**: ndspy's APIs should closely match the semantics of file
+    structures while hiding their binary-level details.
+
+ndspy provides both a Python API and a set of simple command-line tools that
+make use of it. The command-line tools let you convert files to and from binary
+formats without having to write any Python code yourself. The API is suitable
+for use in applications written in Python, and in scripts to do more complex
+tasks than the command-line tools are capable of.
+
+As ndspy is written in pure Python, it is cross-platform and should run on all
+platforms Python supports. Note that Python doesn't support the Nintendo DS
+itself; ndspy is intended to be used on your PC.
+
+Interested? Read on to see some examples, or check the [API
+Reference](https://ndspy.readthedocs.io/en/latest/api/index.html) to see the
+documentation for a specific module. When you're ready to install, head over to
+the [Installation](#installation) section!
+
+
+
+A few examples of ndspy in action
+---------------------------------
+
+Create a *BMG* file containing message strings:
+
+```python
+>>> import ndspy.bmg
+>>> message1 = ndspy.bmg.Message(b'', ['Open your eyes...'])
+>>> message2 = ndspy.bmg.Message(b'', ['Wake up, Link...'])
+>>> bmg = ndspy.bmg.BMG.fromMessages([message1, message2])
+>>> bmg.save()
+b'MESGbmg1\xa0\x00\x00\x00\x02\x00\x00\x00\x02\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00INF1 \x00\x00\x00\x02\x00\x04\x00\x00\x00\x00\x00\x02\x00\x00\x00&\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00DAT1`\x00\x00\x00\x00\x00O\x00p\x00e\x00n\x00 \x00y\x00o\x00u\x00r\x00 \x00e\x00y\x00e\x00s\x00.\x00.\x00.\x00\x00\x00W\x00a\x00k\x00e\x00 \x00u\x00p\x00,\x00 \x00L\x00i\x00n\x00k\x00.\x00.\x00.\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00'
+>>>
+```
+
+Change all notes in a *SSEQ* sequenced music file to middle C, similar to [this
+song](https://youtu.be/cSAp9sBzPbc):
+
+```python
+>>> import ndspy.soundSequence
+>>> song = ndspy.soundSequence.SSEQ.fromFile('never-gonna-give-you-up.sseq')
+>>> song.parse()
+>>> for event in song.events:
+...     if isinstance(event, ndspy.soundSequence.NoteSequenceEvent):
+...         event.pitch = 60
+...
+>>> song.saveToFile('never-gonna-give-you-up-but-all-the-notes-are-c.sseq')
+>>>
+```
+
+Compress and decompress data using the *LZ10* compression format:
+
+```python
+>>> import ndspy.lz10
+>>> compressed = ndspy.lz10.compress(b'This is some data to compress')
+>>> compressed
+b'\x10\x1d\x00\x00\x04This \x00\x02so\x00me data \x00to compr\x00ess\x00\x00\x00\x00\x00'
+>>> ndspy.lz10.decompress(compressed)
+b'This is some data to compress'
+>>>
+```
+
+Search for all files starting with a particular byte sequence in a ROM:
+
+```python
+>>> import ndspy.rom
+>>> rom = ndspy.rom.NintendoDSRom.fromFile('nsmb.nds')
+>>> for i, file in enumerate(rom.files):
+...     if file.startswith(b'BMD0'):
+...         print(rom.filenames[i] + ' is a NSBMD model')
+...
+demo/end_kp.nsbmd is a NSBMD model
+demo/staffroll.nsbmd is a NSBMD model
+demo/staffroll_back.nsbmd is a NSBMD model
+enemy/A_jiku.nsbmd is a NSBMD model
+enemy/all_goal_flag.nsbmd is a NSBMD model
+...
+map/world7.nsbmd is a NSBMD model
+map/world8.nsbmd is a NSBMD model
+>>>
+```
+
+
+Misconceptions
+--------------
+
+Still a little confused about what exactly ndspy is or what it's capable of?
+This section will try to answer some questions you may have.
+
+-   ndspy is a *library*, not a *program.* To use ndspy, you have to write your
+    own Python code; ndspy is essentially a tool your code can use. This may
+    sound daunting -- especially if you're not very familiar with Python -- but
+    the
+    [tutorials](https://ndspy.readthedocs.io/en/latest/tutorials/index.html)
+    walk you through this process step-by-step for some common tasks. In the
+    future, I plan to add some command-line and maybe even GUI tools powered by
+    ndspy, but until then, this is how you use it.
+-   ndspy runs on your PC, not on the Nintendo DS itself. You use it to create
+    and modify game files, which can then be run on the console. DS games have
+    to be written in a compiled language such as C or C++ to have any hope of
+    being efficient; Python will never be a serious option there,
+    unfortunately.
+-   ndspy doesn't support every type of file used in every DS game. In fact,
+    for any given game, it's likely that the majority of the game's files
+    *won't* be supported by ndspy. There's a huge amount of variety in video
+    game file formats, and it would be impossible to support them all. ndspy
+    focuses on file formats used in many games, especially first-party ones.
+    Support for formats that are specific to a particular game would best
+    belong in a separate Python library instead.
+
+    That said, certain parts of ndspy (such as its support for ROM files and
+    raw texture data) have to do with the console's hardware rather than its
+    software, and thus should be relevant to most or all games.
+
+
+<a name="installation"></a>
+Installation
+------------
+
+ndspy requires Python 3.6 or newer to run. CPython (the reference
+implementation of Python) and PyPy are both supported. Python 2, though, is not
+supported at all.
+
+The easiest way to get the latest stable release of ndspy is through PyPI using
+pip.
+
+pip is a command-line application, so you'll need to use the Windows command
+prompt or bash to do this. The exact command you need to enter depends on your
+operating system and the settings you chose when you installed Python. One of
+the following possibilities will probably work for you, though:
+
+    pip install ndspy
+
+    python3 -m pip install ndspy
+
+    py -3 -m pip install ndspy
+
+If you want the very latest version of ndspy including features and bugfixes
+not yet in any official release, you can also download the code from the
+[GitHub repository](https://github.com/RoadrunnerWMC/ndspy) and install it
+manually.
+
+
+Documentation
+-------------
+
+[ndspy's documentation is hosted on Read the
+Docs](https://ndspy.readthedocs.io/en/latest/index.html), and the documentation
+source code can be found in the ``docs/`` folder in this repository. In
+addition to the [API
+reference](https://ndspy.readthedocs.io/en/latest/api/index.html), there are
+also
+[examples](https://ndspy.readthedocs.io/en/latest/index.html#a-few-examples-of-ndspy-in-action)
+and [tutorials](https://ndspy.readthedocs.io/en/latest/tutorials/index.html) to
+help you out!
+
+
+Support
+-------
+
+I spent a long time writing the documentation for ndspy, so first please
+double-check that your question isn't already answered in the [API
+reference](https://ndspy.readthedocs.io/en/latest/api/index.html) or
+[Tutorials](https://ndspy.readthedocs.io/en/latest/tutorials/index.html)
+sections in the documentation.
+
+If that doesn't help, you can ask me (RoadrunnerWMC) your questions via [the
+ndspy Discord server](https://discord.gg/RQhxAxw). I'll try to get back to
+you as quickly as I can!
+
+If you think you've found a bug in ndspy, please [file an issue on
+GitHub](https://github.com/RoadrunnerWMC/ndspy/issues/new). Thanks!
+
+
+Versioning
+----------
+
+ndspy follows [semantic versioning](https://semver.org/) to the best of my
+ability. If a tool claims to work with ndspy 1.0.2, it should also work with
+ndspy 1.2.0, but not necessarily 2.0.0. (Please note that not all of those
+version numbers actually exist!)
+
+Undocumented modules are considered exempt from semantic versioning, and are
+subject to drastic changes at any time. This is also mentioned in the
+[Undocumented
+APIs](https://ndspy.readthedocs.io/en/latest/api/index.html#undocumented-apis)
+section of the documentation.
```

### Comparing `ndspy-4.0.0/README.md` & `ndspy-4.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -154,16 +154,15 @@
     python3 -m pip install ndspy
 
     py -3 -m pip install ndspy
 
 If you want the very latest version of ndspy including features and bugfixes
 not yet in any official release, you can also download the code from the
 [GitHub repository](https://github.com/RoadrunnerWMC/ndspy) and install it
-manually. Note that [crcmod](https://pypi.org/project/crcmod/) is a required
-dependency.
+manually.
 
 
 Documentation
 -------------
 
 [ndspy's documentation is hosted on Read the
 Docs](https://ndspy.readthedocs.io/en/latest/index.html), and the documentation
```

### Comparing `ndspy-4.0.0/ndspy/__init__.py` & `ndspy-4.1.0/ndspy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 """
 
 
 import collections
 import enum
 
 
-VERSION = collections.namedtuple('version', 'major minor patch')(4, 0, 0)
+VERSION = collections.namedtuple('version', 'major minor patch')(4, 1, 0)
 try: VERSION.__class__.__name__ = 'ndspy.version'
 except: pass
 
 
 class Processor(enum.IntEnum):
     """
     An enumeration that can be used to distinguish between the Nintendo
```

### Comparing `ndspy-4.0.0/ndspy/_common.py` & `ndspy-4.1.0/ndspy/_common.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with ndspy.  If not, see <https://www.gnu.org/licenses/>.
 
 
 import struct
 
-import crcmod
-
 HavePIL = True
 try:
     import PIL.Image
 except ImportError:
     HavePIL = False
 
 from . import Alignment
@@ -36,15 +34,23 @@
 # - Version (generally 1)
 # - File size (including this header)
 # - Size of this header (16)
 # - Number of blocks
 
 
 def crc16(data):
-    return crcmod.predefined.mkCrcFun('modbus')(data)
+    crc = 0xFFFF
+    for b in data:
+        crc ^= b
+        for _ in range(8):
+            carry = crc & 1
+            crc >>= 1
+            if carry:
+                crc ^= 0xA001
+    return crc & 0xFFFF
 
 
 def loadNullTerminatedStringFrom(
         data, offset, charWidth=1, encoding='latin-1'):
     """
     Load a null-terminated string from data at offset, with the options
     given
```

### Comparing `ndspy-4.0.0/ndspy/_lzCommon.py` & `ndspy-4.1.0/ndspy/_lzCommon.py`

 * *Files identical despite different names*

### Comparing `ndspy-4.0.0/ndspy/bmg.py` & `ndspy-4.1.0/ndspy/bmg.py`

 * *Files identical despite different names*

### Comparing `ndspy-4.0.0/ndspy/bnbl.py` & `ndspy-4.1.0/ndspy/bnbl.py`

 * *Files identical despite different names*

### Comparing `ndspy-4.0.0/ndspy/bncl.py` & `ndspy-4.1.0/ndspy/bncl.py`

 * *Files identical despite different names*

### Comparing `ndspy-4.0.0/ndspy/code.py` & `ndspy-4.1.0/ndspy/code.py`

 * *Files identical despite different names*

### Comparing `ndspy-4.0.0/ndspy/codeCompression.py` & `ndspy-4.1.0/ndspy/codeCompression.py`

 * *Files identical despite different names*

### Comparing `ndspy-4.0.0/ndspy/color.py` & `ndspy-4.1.0/ndspy/color.py`

 * *Files identical despite different names*

### Comparing `ndspy-4.0.0/ndspy/extras/music.py` & `ndspy-4.1.0/ndspy/extras/music.py`

 * *Files identical despite different names*

### Comparing `ndspy-4.0.0/ndspy/fnt.py` & `ndspy-4.1.0/ndspy/fnt.py`

 * *Files identical despite different names*

### Comparing `ndspy-4.0.0/ndspy/graphics2D.py` & `ndspy-4.1.0/ndspy/graphics2D.py`

 * *Files 1% similar despite different names*

```diff
@@ -470,32 +470,32 @@
     """
     Convenience function: return the tile at (x, y) in the tile list
     given, assuming a row width of `w` (32 by default).
     This can be used with ImageTile.pixels as well (with width 8).
     TODO: maybe rename it somehow to indicate that? Maybe even move it
     into ndspy.__init__ (like the named-list things)?
     """
-    if x >= w or y >= w: return None
+    if x >= width or y >= width: return None
     if x < 0 or y < 0: return None
     try:
-        return tiles[y * w + x]
+        return tiles[y * width + x]
     except IndexError:
         return None
 
 
 def putTile(tiles, x, y, t, *, width=32):
     """
     Convenience function: replace the tile at (x, y) in the tile list
     given with `t`, assuming a row width of `w` (32 by default).
     If (x, y) is not in the tile list, nothing happens.
     This can be used with ImageTile.pixels as well (with width 8).
     TODO: maybe rename it somehow to indicate that? Maybe even move it
     into ndspy.__init__ (like the named-list things)?
     Returns True if the tile was placed, False otherwise (i.e. OOB)
     """
-    if x >= w or y >= w: return False
+    if x >= width or y >= width: return False
     if x < 0 or y < 0: return False
     try:
-        tiles[y * w + x] = t
+        tiles[y * width + x] = t
         return True
     except IndexError:
         return False
```

### Comparing `ndspy-4.0.0/ndspy/lz10.py` & `ndspy-4.1.0/ndspy/lz10.py`

 * *Files identical despite different names*

### Comparing `ndspy-4.0.0/ndspy/model.py` & `ndspy-4.1.0/ndspy/model.py`

 * *Files identical despite different names*

### Comparing `ndspy-4.0.0/ndspy/narc.py` & `ndspy-4.1.0/ndspy/narc.py`

 * *Files identical despite different names*

### Comparing `ndspy-4.0.0/ndspy/rom.py` & `ndspy-4.1.0/ndspy/rom.py`

 * *Files identical despite different names*

### Comparing `ndspy-4.0.0/ndspy/soundArchive.py` & `ndspy-4.1.0/ndspy/soundArchive.py`

 * *Files identical despite different names*

### Comparing `ndspy-4.0.0/ndspy/soundBank.py` & `ndspy-4.1.0/ndspy/soundBank.py`

 * *Files identical despite different names*

### Comparing `ndspy-4.0.0/ndspy/soundGroup.py` & `ndspy-4.1.0/ndspy/soundGroup.py`

 * *Files identical despite different names*

### Comparing `ndspy-4.0.0/ndspy/soundSequence.py` & `ndspy-4.1.0/ndspy/soundSequence.py`

 * *Files identical despite different names*

### Comparing `ndspy-4.0.0/ndspy/soundSequenceArchive.py` & `ndspy-4.1.0/ndspy/soundSequenceArchive.py`

 * *Files identical despite different names*

### Comparing `ndspy-4.0.0/ndspy/soundSequencePlayer.py` & `ndspy-4.1.0/ndspy/soundSequencePlayer.py`

 * *Files identical despite different names*

### Comparing `ndspy-4.0.0/ndspy/soundStream.py` & `ndspy-4.1.0/ndspy/soundStream.py`

 * *Files identical despite different names*

### Comparing `ndspy-4.0.0/ndspy/soundStreamPlayer.py` & `ndspy-4.1.0/ndspy/soundStreamPlayer.py`

 * *Files identical despite different names*

### Comparing `ndspy-4.0.0/ndspy/soundWave.py` & `ndspy-4.1.0/ndspy/soundWave.py`

 * *Files identical despite different names*

### Comparing `ndspy-4.0.0/ndspy/soundWaveArchive.py` & `ndspy-4.1.0/ndspy/soundWaveArchive.py`

 * *Files identical despite different names*

### Comparing `ndspy-4.0.0/ndspy/texture.py` & `ndspy-4.1.0/ndspy/texture.py`

 * *Files identical despite different names*

### Comparing `ndspy-4.0.0/ndspy.egg-info/PKG-INFO` & `ndspy-4.1.0/ndspy.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,227 +1,226 @@
 Metadata-Version: 2.1
 Name: ndspy
-Version: 4.0.0
+Version: 4.1.0
 Summary: Python library that can help you read, modify and create many types of files used in Nintendo DS games.
 Home-page: https://github.com/RoadrunnerWMC/ndspy
 Author: RoadrunnerWMC
 Author-email: roadrunnerwmc@gmail.com
-License: UNKNOWN
-Description: ndspy
-        =====
-        
-        [![Discord](https://img.shields.io/discord/534221996230180884.svg?logo=discord&logoColor=white&colorB=7289da)](https://discord.gg/RQhxAxw)
-        [![Documentation](https://img.shields.io/badge/documentation-Read%20the%20Docs-brightgreen.svg?logo=read%20the%20docs&logoColor=white)](http://ndspy.readthedocs.io/)
-        [![PyPI](https://img.shields.io/pypi/v/ndspy.svg?logo=python&logoColor=white)](https://pypi.org/project/ndspy/)
-        [![License: GNU GPL 3.0](https://img.shields.io/github/license/RoadrunnerWMC/ndspy.svg?logo=gnu&logoColor=white)](https://www.gnu.org/licenses/gpl-3.0)
-        
-        **ndspy** ("en-dee-ESS-pie") is a Python library and suite of command-line
-        tools that can help you read, modify and create many types of files used in
-        Nintendo DS games.
-        
-        ndspy follows a few key design principles:
-        
-        -   **Accuracy**: ndspy should be able to open and resave any supported file
-            with byte-for-byte accuracy if it's in its canonical format.
-        -   **Flexibility**: ndspy should be able to read any valid file in a format it
-            supports. In cases where there's a high chance it will be unable to fully
-            interpret some especially complex part of a file, it should still be useful
-            for editing the other parts.
-        -   **Semantic**: ndspy's APIs should closely match the semantics of file
-            structures while hiding their binary-level details.
-        
-        ndspy provides both a Python API and a set of simple command-line tools that
-        make use of it. The command-line tools let you convert files to and from binary
-        formats without having to write any Python code yourself. The API is suitable
-        for use in applications written in Python, and in scripts to do more complex
-        tasks than the command-line tools are capable of.
-        
-        As ndspy is written in pure Python, it is cross-platform and should run on all
-        platforms Python supports. Note that Python doesn't support the Nintendo DS
-        itself; ndspy is intended to be used on your PC.
-        
-        Interested? Read on to see some examples, or check the [API
-        Reference](https://ndspy.readthedocs.io/en/latest/api/index.html) to see the
-        documentation for a specific module. When you're ready to install, head over to
-        the [Installation](#installation) section!
-        
-        
-        
-        A few examples of ndspy in action
-        ---------------------------------
-        
-        Create a *BMG* file containing message strings:
-        
-        ```python
-        >>> import ndspy.bmg
-        >>> message1 = ndspy.bmg.Message(b'', ['Open your eyes...'])
-        >>> message2 = ndspy.bmg.Message(b'', ['Wake up, Link...'])
-        >>> bmg = ndspy.bmg.BMG.fromMessages([message1, message2])
-        >>> bmg.save()
-        b'MESGbmg1\xa0\x00\x00\x00\x02\x00\x00\x00\x02\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00INF1 \x00\x00\x00\x02\x00\x04\x00\x00\x00\x00\x00\x02\x00\x00\x00&\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00DAT1`\x00\x00\x00\x00\x00O\x00p\x00e\x00n\x00 \x00y\x00o\x00u\x00r\x00 \x00e\x00y\x00e\x00s\x00.\x00.\x00.\x00\x00\x00W\x00a\x00k\x00e\x00 \x00u\x00p\x00,\x00 \x00L\x00i\x00n\x00k\x00.\x00.\x00.\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00'
-        >>>
-        ```
-        
-        Change all notes in a *SSEQ* sequenced music file to middle C, similar to [this
-        song](https://youtu.be/cSAp9sBzPbc):
-        
-        ```python
-        >>> import ndspy.soundSequence
-        >>> song = ndspy.soundSequence.SSEQ.fromFile('never-gonna-give-you-up.sseq')
-        >>> song.parse()
-        >>> for event in song.events:
-        ...     if isinstance(event, ndspy.soundSequence.NoteSequenceEvent):
-        ...         event.pitch = 60
-        ...
-        >>> song.saveToFile('never-gonna-give-you-up-but-all-the-notes-are-c.sseq')
-        >>>
-        ```
-        
-        Compress and decompress data using the *LZ10* compression format:
-        
-        ```python
-        >>> import ndspy.lz10
-        >>> compressed = ndspy.lz10.compress(b'This is some data to compress')
-        >>> compressed
-        b'\x10\x1d\x00\x00\x04This \x00\x02so\x00me data \x00to compr\x00ess\x00\x00\x00\x00\x00'
-        >>> ndspy.lz10.decompress(compressed)
-        b'This is some data to compress'
-        >>>
-        ```
-        
-        Search for all files starting with a particular byte sequence in a ROM:
-        
-        ```python
-        >>> import ndspy.rom
-        >>> rom = ndspy.rom.NintendoDSRom.fromFile('nsmb.nds')
-        >>> for i, file in enumerate(rom.files):
-        ...     if file.startswith(b'BMD0'):
-        ...         print(rom.filenames[i] + ' is a NSBMD model')
-        ...
-        demo/end_kp.nsbmd is a NSBMD model
-        demo/staffroll.nsbmd is a NSBMD model
-        demo/staffroll_back.nsbmd is a NSBMD model
-        enemy/A_jiku.nsbmd is a NSBMD model
-        enemy/all_goal_flag.nsbmd is a NSBMD model
-        ...
-        map/world7.nsbmd is a NSBMD model
-        map/world8.nsbmd is a NSBMD model
-        >>>
-        ```
-        
-        
-        Misconceptions
-        --------------
-        
-        Still a little confused about what exactly ndspy is or what it's capable of?
-        This section will try to answer some questions you may have.
-        
-        -   ndspy is a *library*, not a *program.* To use ndspy, you have to write your
-            own Python code; ndspy is essentially a tool your code can use. This may
-            sound daunting -- especially if you're not very familiar with Python -- but
-            the
-            [tutorials](https://ndspy.readthedocs.io/en/latest/tutorials/index.html)
-            walk you through this process step-by-step for some common tasks. In the
-            future, I plan to add some command-line and maybe even GUI tools powered by
-            ndspy, but until then, this is how you use it.
-        -   ndspy runs on your PC, not on the Nintendo DS itself. You use it to create
-            and modify game files, which can then be run on the console. DS games have
-            to be written in a compiled language such as C or C++ to have any hope of
-            being efficient; Python will never be a serious option there,
-            unfortunately.
-        -   ndspy doesn't support every type of file used in every DS game. In fact,
-            for any given game, it's likely that the majority of the game's files
-            *won't* be supported by ndspy. There's a huge amount of variety in video
-            game file formats, and it would be impossible to support them all. ndspy
-            focuses on file formats used in many games, especially first-party ones.
-            Support for formats that are specific to a particular game would best
-            belong in a separate Python library instead.
-        
-            That said, certain parts of ndspy (such as its support for ROM files and
-            raw texture data) have to do with the console's hardware rather than its
-            software, and thus should be relevant to most or all games.
-        
-        
-        <a name="installation"></a>
-        Installation
-        ------------
-        
-        ndspy requires Python 3.6 or newer to run. CPython (the reference
-        implementation of Python) and PyPy are both supported. Python 2, though, is not
-        supported at all.
-        
-        The easiest way to get the latest stable release of ndspy is through PyPI using
-        pip.
-        
-        pip is a command-line application, so you'll need to use the Windows command
-        prompt or bash to do this. The exact command you need to enter depends on your
-        operating system and the settings you chose when you installed Python. One of
-        the following possibilities will probably work for you, though:
-        
-            pip install ndspy
-        
-            python3 -m pip install ndspy
-        
-            py -3 -m pip install ndspy
-        
-        If you want the very latest version of ndspy including features and bugfixes
-        not yet in any official release, you can also download the code from the
-        [GitHub repository](https://github.com/RoadrunnerWMC/ndspy) and install it
-        manually. Note that [crcmod](https://pypi.org/project/crcmod/) is a required
-        dependency.
-        
-        
-        Documentation
-        -------------
-        
-        [ndspy's documentation is hosted on Read the
-        Docs](https://ndspy.readthedocs.io/en/latest/index.html), and the documentation
-        source code can be found in the ``docs/`` folder in this repository. In
-        addition to the [API
-        reference](https://ndspy.readthedocs.io/en/latest/api/index.html), there are
-        also
-        [examples](https://ndspy.readthedocs.io/en/latest/index.html#a-few-examples-of-ndspy-in-action)
-        and [tutorials](https://ndspy.readthedocs.io/en/latest/tutorials/index.html) to
-        help you out!
-        
-        
-        Support
-        -------
-        
-        I spent a long time writing the documentation for ndspy, so first please
-        double-check that your question isn't already answered in the [API
-        reference](https://ndspy.readthedocs.io/en/latest/api/index.html) or
-        [Tutorials](https://ndspy.readthedocs.io/en/latest/tutorials/index.html)
-        sections in the documentation.
-        
-        If that doesn't help, you can ask me (RoadrunnerWMC) your questions via [the
-        ndspy Discord server](https://discord.gg/RQhxAxw). I'll try to get back to
-        you as quickly as I can!
-        
-        If you think you've found a bug in ndspy, please [file an issue on
-        GitHub](https://github.com/RoadrunnerWMC/ndspy/issues/new). Thanks!
-        
-        
-        Versioning
-        ----------
-        
-        ndspy follows [semantic versioning](https://semver.org/) to the best of my
-        ability. If a tool claims to work with ndspy 1.0.2, it should also work with
-        ndspy 1.2.0, but not necessarily 2.0.0. (Please note that not all of those
-        version numbers actually exist!)
-        
-        Undocumented modules are considered exempt from semantic versioning, and are
-        subject to drastic changes at any time. This is also mentioned in the
-        [Undocumented
-        APIs](https://ndspy.readthedocs.io/en/latest/api/index.html#undocumented-apis)
-        section of the documentation.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+ndspy
+=====
+
+[![Discord](https://img.shields.io/discord/534221996230180884.svg?logo=discord&logoColor=white&colorB=7289da)](https://discord.gg/RQhxAxw)
+[![Documentation](https://img.shields.io/badge/documentation-Read%20the%20Docs-brightgreen.svg?logo=read%20the%20docs&logoColor=white)](http://ndspy.readthedocs.io/)
+[![PyPI](https://img.shields.io/pypi/v/ndspy.svg?logo=python&logoColor=white)](https://pypi.org/project/ndspy/)
+[![License: GNU GPL 3.0](https://img.shields.io/github/license/RoadrunnerWMC/ndspy.svg?logo=gnu&logoColor=white)](https://www.gnu.org/licenses/gpl-3.0)
+
+**ndspy** ("en-dee-ESS-pie") is a Python library and suite of command-line
+tools that can help you read, modify and create many types of files used in
+Nintendo DS games.
+
+ndspy follows a few key design principles:
+
+-   **Accuracy**: ndspy should be able to open and resave any supported file
+    with byte-for-byte accuracy if it's in its canonical format.
+-   **Flexibility**: ndspy should be able to read any valid file in a format it
+    supports. In cases where there's a high chance it will be unable to fully
+    interpret some especially complex part of a file, it should still be useful
+    for editing the other parts.
+-   **Semantic**: ndspy's APIs should closely match the semantics of file
+    structures while hiding their binary-level details.
+
+ndspy provides both a Python API and a set of simple command-line tools that
+make use of it. The command-line tools let you convert files to and from binary
+formats without having to write any Python code yourself. The API is suitable
+for use in applications written in Python, and in scripts to do more complex
+tasks than the command-line tools are capable of.
+
+As ndspy is written in pure Python, it is cross-platform and should run on all
+platforms Python supports. Note that Python doesn't support the Nintendo DS
+itself; ndspy is intended to be used on your PC.
+
+Interested? Read on to see some examples, or check the [API
+Reference](https://ndspy.readthedocs.io/en/latest/api/index.html) to see the
+documentation for a specific module. When you're ready to install, head over to
+the [Installation](#installation) section!
+
+
+
+A few examples of ndspy in action
+---------------------------------
+
+Create a *BMG* file containing message strings:
+
+```python
+>>> import ndspy.bmg
+>>> message1 = ndspy.bmg.Message(b'', ['Open your eyes...'])
+>>> message2 = ndspy.bmg.Message(b'', ['Wake up, Link...'])
+>>> bmg = ndspy.bmg.BMG.fromMessages([message1, message2])
+>>> bmg.save()
+b'MESGbmg1\xa0\x00\x00\x00\x02\x00\x00\x00\x02\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00INF1 \x00\x00\x00\x02\x00\x04\x00\x00\x00\x00\x00\x02\x00\x00\x00&\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00DAT1`\x00\x00\x00\x00\x00O\x00p\x00e\x00n\x00 \x00y\x00o\x00u\x00r\x00 \x00e\x00y\x00e\x00s\x00.\x00.\x00.\x00\x00\x00W\x00a\x00k\x00e\x00 \x00u\x00p\x00,\x00 \x00L\x00i\x00n\x00k\x00.\x00.\x00.\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00'
+>>>
+```
+
+Change all notes in a *SSEQ* sequenced music file to middle C, similar to [this
+song](https://youtu.be/cSAp9sBzPbc):
+
+```python
+>>> import ndspy.soundSequence
+>>> song = ndspy.soundSequence.SSEQ.fromFile('never-gonna-give-you-up.sseq')
+>>> song.parse()
+>>> for event in song.events:
+...     if isinstance(event, ndspy.soundSequence.NoteSequenceEvent):
+...         event.pitch = 60
+...
+>>> song.saveToFile('never-gonna-give-you-up-but-all-the-notes-are-c.sseq')
+>>>
+```
+
+Compress and decompress data using the *LZ10* compression format:
+
+```python
+>>> import ndspy.lz10
+>>> compressed = ndspy.lz10.compress(b'This is some data to compress')
+>>> compressed
+b'\x10\x1d\x00\x00\x04This \x00\x02so\x00me data \x00to compr\x00ess\x00\x00\x00\x00\x00'
+>>> ndspy.lz10.decompress(compressed)
+b'This is some data to compress'
+>>>
+```
+
+Search for all files starting with a particular byte sequence in a ROM:
+
+```python
+>>> import ndspy.rom
+>>> rom = ndspy.rom.NintendoDSRom.fromFile('nsmb.nds')
+>>> for i, file in enumerate(rom.files):
+...     if file.startswith(b'BMD0'):
+...         print(rom.filenames[i] + ' is a NSBMD model')
+...
+demo/end_kp.nsbmd is a NSBMD model
+demo/staffroll.nsbmd is a NSBMD model
+demo/staffroll_back.nsbmd is a NSBMD model
+enemy/A_jiku.nsbmd is a NSBMD model
+enemy/all_goal_flag.nsbmd is a NSBMD model
+...
+map/world7.nsbmd is a NSBMD model
+map/world8.nsbmd is a NSBMD model
+>>>
+```
+
+
+Misconceptions
+--------------
+
+Still a little confused about what exactly ndspy is or what it's capable of?
+This section will try to answer some questions you may have.
+
+-   ndspy is a *library*, not a *program.* To use ndspy, you have to write your
+    own Python code; ndspy is essentially a tool your code can use. This may
+    sound daunting -- especially if you're not very familiar with Python -- but
+    the
+    [tutorials](https://ndspy.readthedocs.io/en/latest/tutorials/index.html)
+    walk you through this process step-by-step for some common tasks. In the
+    future, I plan to add some command-line and maybe even GUI tools powered by
+    ndspy, but until then, this is how you use it.
+-   ndspy runs on your PC, not on the Nintendo DS itself. You use it to create
+    and modify game files, which can then be run on the console. DS games have
+    to be written in a compiled language such as C or C++ to have any hope of
+    being efficient; Python will never be a serious option there,
+    unfortunately.
+-   ndspy doesn't support every type of file used in every DS game. In fact,
+    for any given game, it's likely that the majority of the game's files
+    *won't* be supported by ndspy. There's a huge amount of variety in video
+    game file formats, and it would be impossible to support them all. ndspy
+    focuses on file formats used in many games, especially first-party ones.
+    Support for formats that are specific to a particular game would best
+    belong in a separate Python library instead.
+
+    That said, certain parts of ndspy (such as its support for ROM files and
+    raw texture data) have to do with the console's hardware rather than its
+    software, and thus should be relevant to most or all games.
+
+
+<a name="installation"></a>
+Installation
+------------
+
+ndspy requires Python 3.6 or newer to run. CPython (the reference
+implementation of Python) and PyPy are both supported. Python 2, though, is not
+supported at all.
+
+The easiest way to get the latest stable release of ndspy is through PyPI using
+pip.
+
+pip is a command-line application, so you'll need to use the Windows command
+prompt or bash to do this. The exact command you need to enter depends on your
+operating system and the settings you chose when you installed Python. One of
+the following possibilities will probably work for you, though:
+
+    pip install ndspy
+
+    python3 -m pip install ndspy
+
+    py -3 -m pip install ndspy
+
+If you want the very latest version of ndspy including features and bugfixes
+not yet in any official release, you can also download the code from the
+[GitHub repository](https://github.com/RoadrunnerWMC/ndspy) and install it
+manually.
+
+
+Documentation
+-------------
+
+[ndspy's documentation is hosted on Read the
+Docs](https://ndspy.readthedocs.io/en/latest/index.html), and the documentation
+source code can be found in the ``docs/`` folder in this repository. In
+addition to the [API
+reference](https://ndspy.readthedocs.io/en/latest/api/index.html), there are
+also
+[examples](https://ndspy.readthedocs.io/en/latest/index.html#a-few-examples-of-ndspy-in-action)
+and [tutorials](https://ndspy.readthedocs.io/en/latest/tutorials/index.html) to
+help you out!
+
+
+Support
+-------
+
+I spent a long time writing the documentation for ndspy, so first please
+double-check that your question isn't already answered in the [API
+reference](https://ndspy.readthedocs.io/en/latest/api/index.html) or
+[Tutorials](https://ndspy.readthedocs.io/en/latest/tutorials/index.html)
+sections in the documentation.
+
+If that doesn't help, you can ask me (RoadrunnerWMC) your questions via [the
+ndspy Discord server](https://discord.gg/RQhxAxw). I'll try to get back to
+you as quickly as I can!
+
+If you think you've found a bug in ndspy, please [file an issue on
+GitHub](https://github.com/RoadrunnerWMC/ndspy/issues/new). Thanks!
+
+
+Versioning
+----------
+
+ndspy follows [semantic versioning](https://semver.org/) to the best of my
+ability. If a tool claims to work with ndspy 1.0.2, it should also work with
+ndspy 1.2.0, but not necessarily 2.0.0. (Please note that not all of those
+version numbers actually exist!)
+
+Undocumented modules are considered exempt from semantic versioning, and are
+subject to drastic changes at any time. This is also mentioned in the
+[Undocumented
+APIs](https://ndspy.readthedocs.io/en/latest/api/index.html#undocumented-apis)
+section of the documentation.
```

### Comparing `ndspy-4.0.0/setup.py` & `ndspy-4.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='ndspy',
-    version='4.0.0',
+    version='4.1.0',
     author='RoadrunnerWMC',
     author_email='roadrunnerwmc@gmail.com',
     description='Python library that can help you read, modify and create many types of files used in Nintendo DS games.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/RoadrunnerWMC/ndspy',
     packages=setuptools.find_packages(),
     python_requires='>=3.6',
     entry_points={
         'console_scripts': [
             'ndspy_codeCompression = ndspy.codeCompression:main',
             'ndspy_lz10 = ndspy.lz10:main',
         ],
     },
-    install_requires=[
-        'crcmod',
-    ],
     classifiers=[
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
         'Operating System :: OS Independent',
     ],
 )
```

