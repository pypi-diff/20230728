# Comparing `tmp/numbers_parser-4.1.2.tar.gz` & `tmp/numbers_parser-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numbers_parser-4.1.2.tar", max compression
+gzip compressed data, was "numbers_parser-4.2.0.tar", max compression
```

## Comparing `numbers_parser-4.1.2.tar` & `numbers_parser-4.2.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     1050 2022-06-23 17:13:17.000000 numbers_parser-4.1.2/LICENSE.rst
--rw-r--r--   0        0        0    20092 2023-07-16 14:26:24.846490 numbers_parser-4.1.2/README.md
--rw-r--r--   0        0        0     2112 2023-07-18 20:11:54.382694 numbers_parser-4.1.2/pyproject.toml
--rw-r--r--   0        0        0     2139 2023-07-18 20:05:00.796169 numbers_parser-4.1.2/src/numbers_parser/__init__.py
--rw-r--r--   0        0        0     4350 2023-07-16 15:02:05.843221 numbers_parser-4.1.2/src/numbers_parser/_cat_numbers.py
--rw-r--r--   0        0        0     5826 2023-07-16 15:04:36.595811 numbers_parser-4.1.2/src/numbers_parser/_unpack_numbers.py
--rw-r--r--   0        0        0     2616 2023-05-20 02:42:59.000000 numbers_parser-4.1.2/src/numbers_parser/bullets.py
--rw-r--r--   0        0        0    17992 2023-07-19 18:11:53.756245 numbers_parser-4.1.2/src/numbers_parser/cell.py
--rw-r--r--   0        0        0    29688 2023-07-18 19:05:31.031251 numbers_parser-4.1.2/src/numbers_parser/cell_storage.py
--rw-r--r--   0        0        0     1689 2023-07-16 11:18:31.505310 numbers_parser-4.1.2/src/numbers_parser/constants.py
--rw-r--r--   0        0        0     4239 2023-07-14 19:05:10.687308 numbers_parser-4.1.2/src/numbers_parser/containers.py
--rwxr-xr-x   0        0        0   134819 2022-07-21 08:13:02.000000 numbers_parser-4.1.2/src/numbers_parser/data/empty.numbers
--rw-r--r--   0        0        0    17543 2023-07-20 18:34:33.748901 numbers_parser-4.1.2/src/numbers_parser/document.py
--rw-r--r--   0        0        0      663 2022-10-17 17:39:14.019486 numbers_parser-4.1.2/src/numbers_parser/exceptions.py
--rw-r--r--   0        0        0      374 2023-07-16 14:30:53.391296 numbers_parser-4.1.2/src/numbers_parser/experimental.py
--rw-r--r--   0        0        0     3865 2023-07-14 19:05:10.688785 numbers_parser-4.1.2/src/numbers_parser/file.py
--rw-r--r--   0        0        0    10665 2023-07-14 19:05:10.689467 numbers_parser-4.1.2/src/numbers_parser/formula.py
--rw-r--r--   0        0        0    16007 2023-07-10 11:50:37.380120 numbers_parser-4.1.2/src/numbers_parser/generated/TNArchives_pb2.py
--rw-r--r--   0        0        0     1215 2023-07-10 11:50:37.381233 numbers_parser-4.1.2/src/numbers_parser/generated/TNArchives_sos_pb2.py
--rw-r--r--   0        0        0    18271 2023-07-10 11:50:37.381940 numbers_parser-4.1.2/src/numbers_parser/generated/TNCommandArchives_pb2.py
--rw-r--r--   0        0        0     1857 2023-07-10 11:50:37.383021 numbers_parser-4.1.2/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py
--rw-r--r--   0        0        0    17361 2023-07-10 11:50:37.383432 numbers_parser-4.1.2/src/numbers_parser/generated/TSAArchives_pb2.py
--rw-r--r--   0        0        0     2033 2023-07-10 11:50:37.383703 numbers_parser-4.1.2/src/numbers_parser/generated/TSAArchives_sos_pb2.py
--rw-r--r--   0        0        0     3907 2023-07-10 11:50:37.383945 numbers_parser-4.1.2/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py
--rw-r--r--   0        0        0    64955 2023-07-10 11:50:37.384822 numbers_parser-4.1.2/src/numbers_parser/generated/TSCEArchives_pb2.py
--rw-r--r--   0        0        0    11162 2023-07-10 11:50:37.385161 numbers_parser-4.1.2/src/numbers_parser/generated/TSCH3DArchives_pb2.py
--rw-r--r--   0        0        0     8655 2023-07-10 11:50:37.385944 numbers_parser-4.1.2/src/numbers_parser/generated/TSCHArchives_Common_pb2.py
--rw-r--r--   0        0        0    46323 2023-07-10 11:50:37.386335 numbers_parser-4.1.2/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py
--rw-r--r--   0        0        0    22717 2023-07-10 11:50:37.386667 numbers_parser-4.1.2/src/numbers_parser/generated/TSCHArchives_pb2.py
--rw-r--r--   0        0        0    63730 2023-07-10 11:50:37.387194 numbers_parser-4.1.2/src/numbers_parser/generated/TSCHArchives_sos_pb2.py
--rw-r--r--   0        0        0    27446 2023-07-10 11:50:37.387691 numbers_parser-4.1.2/src/numbers_parser/generated/TSCHCommandArchives_pb2.py
--rw-r--r--   0        0        0    30051 2023-07-10 11:50:37.387967 numbers_parser-4.1.2/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py
--rw-r--r--   0        0        0    40151 2023-07-10 11:50:37.388832 numbers_parser-4.1.2/src/numbers_parser/generated/TSDArchives_pb2.py
--rw-r--r--   0        0        0     6022 2023-07-10 11:50:37.389137 numbers_parser-4.1.2/src/numbers_parser/generated/TSDArchives_sos_pb2.py
--rw-r--r--   0        0        0    29192 2023-07-10 11:50:37.389550 numbers_parser-4.1.2/src/numbers_parser/generated/TSDCommandArchives_pb2.py
--rw-r--r--   0        0        0    53520 2023-07-10 11:50:37.390046 numbers_parser-4.1.2/src/numbers_parser/generated/TSKArchives_pb2.py
--rw-r--r--   0        0        0     1941 2023-07-10 11:50:37.390302 numbers_parser-4.1.2/src/numbers_parser/generated/TSKArchives_sos_pb2.py
--rw-r--r--   0        0        0    18142 2023-07-10 11:50:37.390611 numbers_parser-4.1.2/src/numbers_parser/generated/TSPArchiveMessages_pb2.py
--rw-r--r--   0        0        0     2024 2023-07-10 11:50:37.390860 numbers_parser-4.1.2/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py
--rw-r--r--   0        0        0    12611 2023-07-10 11:50:37.391120 numbers_parser-4.1.2/src/numbers_parser/generated/TSPMessages_pb2.py
--rw-r--r--   0        0        0     9717 2023-07-10 11:50:37.391599 numbers_parser-4.1.2/src/numbers_parser/generated/TSSArchives_pb2.py
--rw-r--r--   0        0        0     2842 2023-07-10 11:50:37.391866 numbers_parser-4.1.2/src/numbers_parser/generated/TSSArchives_sos_pb2.py
--rw-r--r--   0        0        0    88532 2023-07-10 11:50:37.392988 numbers_parser-4.1.2/src/numbers_parser/generated/TSTArchives_pb2.py
--rw-r--r--   0        0        0    12597 2023-07-10 11:50:37.393496 numbers_parser-4.1.2/src/numbers_parser/generated/TSTArchives_sos_pb2.py
--rw-r--r--   0        0        0    59523 2023-07-10 11:50:37.394520 numbers_parser-4.1.2/src/numbers_parser/generated/TSTCommandArchives_pb2.py
--rw-r--r--   0        0        0    12644 2023-07-10 11:50:37.394909 numbers_parser-4.1.2/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py
--rw-r--r--   0        0        0    58663 2023-07-10 11:50:37.396073 numbers_parser-4.1.2/src/numbers_parser/generated/TSWPArchives_pb2.py
--rw-r--r--   0        0        0    28840 2023-07-10 11:50:37.396468 numbers_parser-4.1.2/src/numbers_parser/generated/TSWPArchives_sos_pb2.py
--rw-r--r--   0        0        0    25441 2023-07-10 11:50:37.397211 numbers_parser-4.1.2/src/numbers_parser/generated/TSWPCommandArchives_pb2.py
--rw-r--r--   0        0        0        0 2023-07-10 11:50:37.401529 numbers_parser-4.1.2/src/numbers_parser/generated/__init__.py
--rw-r--r--   0        0        0    22604 2023-07-16 09:02:55.094582 numbers_parser-4.1.2/src/numbers_parser/generated/fontmap.py
--rw-r--r--   0        0        0     6082 2023-07-14 19:05:10.690473 numbers_parser-4.1.2/src/numbers_parser/generated/functionmap.py
--rw-r--r--   0        0        0    12032 2023-07-15 11:47:48.837033 numbers_parser-4.1.2/src/numbers_parser/iwafile.py
--rw-r--r--   0        0        0    32100 2023-07-10 11:51:11.630380 numbers_parser-4.1.2/src/numbers_parser/mapping.py
--rw-r--r--   0        0        0    75677 2023-07-20 18:36:31.553525 numbers_parser-4.1.2/src/numbers_parser/model.py
--rw-r--r--   0        0        0     2690 2023-07-08 11:12:33.356950 numbers_parser-4.1.2/src/numbers_parser/numbers_uuid.py
--rw-r--r--   0        0        0    21269 1970-01-01 00:00:00.000000 numbers_parser-4.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1050 2022-06-23 17:13:17.000000 numbers_parser-4.2.0/LICENSE.rst
+-rw-r--r--   0        0        0    21100 2023-07-21 16:51:45.519938 numbers_parser-4.2.0/README.md
+-rw-r--r--   0        0        0     2112 2023-07-21 16:52:35.915547 numbers_parser-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2081 2023-07-23 15:54:51.138965 numbers_parser-4.2.0/src/numbers_parser/__init__.py
+-rw-r--r--   0        0        0     4336 2023-07-23 15:54:51.161098 numbers_parser-4.2.0/src/numbers_parser/_cat_numbers.py
+-rw-r--r--   0        0        0     5784 2023-07-23 15:54:51.177251 numbers_parser-4.2.0/src/numbers_parser/_unpack_numbers.py
+-rw-r--r--   0        0        0     2616 2023-05-20 02:42:59.000000 numbers_parser-4.2.0/src/numbers_parser/bullets.py
+-rw-r--r--   0        0        0    22973 2023-07-27 06:57:17.175853 numbers_parser-4.2.0/src/numbers_parser/cell.py
+-rw-r--r--   0        0        0    29536 2023-07-23 15:54:51.340254 numbers_parser-4.2.0/src/numbers_parser/cell_storage.py
+-rw-r--r--   0        0        0     1823 2023-07-25 11:49:15.661140 numbers_parser-4.2.0/src/numbers_parser/constants.py
+-rw-r--r--   0        0        0     4239 2023-07-14 19:05:10.687308 numbers_parser-4.2.0/src/numbers_parser/containers.py
+-rwxr-xr-x   0        0        0   134819 2022-07-21 08:13:02.000000 numbers_parser-4.2.0/src/numbers_parser/data/empty.numbers
+-rw-r--r--   0        0        0    18786 2023-07-28 10:14:11.778889 numbers_parser-4.2.0/src/numbers_parser/document.py
+-rw-r--r--   0        0        0      663 2022-10-17 17:39:14.019486 numbers_parser-4.2.0/src/numbers_parser/exceptions.py
+-rw-r--r--   0        0        0      374 2023-07-16 14:30:53.391296 numbers_parser-4.2.0/src/numbers_parser/experimental.py
+-rw-r--r--   0        0        0     3683 2023-07-23 15:54:51.189959 numbers_parser-4.2.0/src/numbers_parser/file.py
+-rw-r--r--   0        0        0    10665 2023-07-14 19:05:10.689467 numbers_parser-4.2.0/src/numbers_parser/formula.py
+-rw-r--r--   0        0        0    16007 2023-07-23 16:06:40.954866 numbers_parser-4.2.0/src/numbers_parser/generated/TNArchives_pb2.py
+-rw-r--r--   0        0        0     1215 2023-07-23 16:06:40.955183 numbers_parser-4.2.0/src/numbers_parser/generated/TNArchives_sos_pb2.py
+-rw-r--r--   0        0        0    18271 2023-07-23 16:06:40.955417 numbers_parser-4.2.0/src/numbers_parser/generated/TNCommandArchives_pb2.py
+-rw-r--r--   0        0        0     1857 2023-07-23 16:06:40.955655 numbers_parser-4.2.0/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py
+-rw-r--r--   0        0        0    17361 2023-07-23 16:06:40.955915 numbers_parser-4.2.0/src/numbers_parser/generated/TSAArchives_pb2.py
+-rw-r--r--   0        0        0     2033 2023-07-23 16:06:40.956132 numbers_parser-4.2.0/src/numbers_parser/generated/TSAArchives_sos_pb2.py
+-rw-r--r--   0        0        0     3907 2023-07-23 16:06:40.956319 numbers_parser-4.2.0/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py
+-rw-r--r--   0        0        0    64955 2023-07-23 16:06:40.956672 numbers_parser-4.2.0/src/numbers_parser/generated/TSCEArchives_pb2.py
+-rw-r--r--   0        0        0    11162 2023-07-23 16:06:40.957188 numbers_parser-4.2.0/src/numbers_parser/generated/TSCH3DArchives_pb2.py
+-rw-r--r--   0        0        0     8655 2023-07-23 16:06:40.957541 numbers_parser-4.2.0/src/numbers_parser/generated/TSCHArchives_Common_pb2.py
+-rw-r--r--   0        0        0    46323 2023-07-23 16:06:40.957794 numbers_parser-4.2.0/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py
+-rw-r--r--   0        0        0    22717 2023-07-23 16:06:40.958066 numbers_parser-4.2.0/src/numbers_parser/generated/TSCHArchives_pb2.py
+-rw-r--r--   0        0        0    63730 2023-07-23 16:06:40.958325 numbers_parser-4.2.0/src/numbers_parser/generated/TSCHArchives_sos_pb2.py
+-rw-r--r--   0        0        0    27446 2023-07-23 16:06:40.958670 numbers_parser-4.2.0/src/numbers_parser/generated/TSCHCommandArchives_pb2.py
+-rw-r--r--   0        0        0    30051 2023-07-23 16:06:40.959087 numbers_parser-4.2.0/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py
+-rw-r--r--   0        0        0    40151 2023-07-23 16:06:40.959435 numbers_parser-4.2.0/src/numbers_parser/generated/TSDArchives_pb2.py
+-rw-r--r--   0        0        0     6022 2023-07-23 16:06:40.959684 numbers_parser-4.2.0/src/numbers_parser/generated/TSDArchives_sos_pb2.py
+-rw-r--r--   0        0        0    29192 2023-07-23 16:06:40.959950 numbers_parser-4.2.0/src/numbers_parser/generated/TSDCommandArchives_pb2.py
+-rw-r--r--   0        0        0    53520 2023-07-23 16:06:40.960332 numbers_parser-4.2.0/src/numbers_parser/generated/TSKArchives_pb2.py
+-rw-r--r--   0        0        0     1941 2023-07-23 16:06:40.960544 numbers_parser-4.2.0/src/numbers_parser/generated/TSKArchives_sos_pb2.py
+-rw-r--r--   0        0        0    18142 2023-07-23 16:06:40.960804 numbers_parser-4.2.0/src/numbers_parser/generated/TSPArchiveMessages_pb2.py
+-rw-r--r--   0        0        0     2024 2023-07-23 16:06:40.961046 numbers_parser-4.2.0/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py
+-rw-r--r--   0        0        0    12611 2023-07-23 16:06:40.961302 numbers_parser-4.2.0/src/numbers_parser/generated/TSPMessages_pb2.py
+-rw-r--r--   0        0        0     9717 2023-07-23 16:06:40.961563 numbers_parser-4.2.0/src/numbers_parser/generated/TSSArchives_pb2.py
+-rw-r--r--   0        0        0     2842 2023-07-23 16:06:40.961856 numbers_parser-4.2.0/src/numbers_parser/generated/TSSArchives_sos_pb2.py
+-rw-r--r--   0        0        0    88532 2023-07-23 16:06:40.962320 numbers_parser-4.2.0/src/numbers_parser/generated/TSTArchives_pb2.py
+-rw-r--r--   0        0        0    12597 2023-07-23 16:06:40.962544 numbers_parser-4.2.0/src/numbers_parser/generated/TSTArchives_sos_pb2.py
+-rw-r--r--   0        0        0    59523 2023-07-23 16:06:40.963108 numbers_parser-4.2.0/src/numbers_parser/generated/TSTCommandArchives_pb2.py
+-rw-r--r--   0        0        0    12644 2023-07-23 16:06:40.963347 numbers_parser-4.2.0/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py
+-rw-r--r--   0        0        0    58663 2023-07-23 16:06:40.963755 numbers_parser-4.2.0/src/numbers_parser/generated/TSWPArchives_pb2.py
+-rw-r--r--   0        0        0    28840 2023-07-23 16:06:40.964041 numbers_parser-4.2.0/src/numbers_parser/generated/TSWPArchives_sos_pb2.py
+-rw-r--r--   0        0        0    25441 2023-07-23 16:06:40.964356 numbers_parser-4.2.0/src/numbers_parser/generated/TSWPCommandArchives_pb2.py
+-rw-r--r--   0        0        0        0 2023-07-23 16:06:40.970289 numbers_parser-4.2.0/src/numbers_parser/generated/__init__.py
+-rw-r--r--   0        0        0    22604 2023-07-23 16:06:33.784957 numbers_parser-4.2.0/src/numbers_parser/generated/fontmap.py
+-rw-r--r--   0        0        0     6082 2023-07-23 16:06:33.032684 numbers_parser-4.2.0/src/numbers_parser/generated/functionmap.py
+-rw-r--r--   0        0        0    11868 2023-07-23 15:54:51.253681 numbers_parser-4.2.0/src/numbers_parser/iwafile.py
+-rw-r--r--   0        0        0    32117 2023-07-23 16:07:16.807745 numbers_parser-4.2.0/src/numbers_parser/mapping.py
+-rw-r--r--   0        0        0    87056 2023-07-28 10:51:47.125210 numbers_parser-4.2.0/src/numbers_parser/model.py
+-rw-r--r--   0        0        0     2642 2023-07-23 15:54:51.198744 numbers_parser-4.2.0/src/numbers_parser/numbers_uuid.py
+-rw-r--r--   0        0        0    22277 1970-01-01 00:00:00.000000 numbers_parser-4.2.0/PKG-INFO
```

### Comparing `numbers_parser-4.1.2/LICENSE.rst` & `numbers_parser-4.2.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/README.md` & `numbers_parser-4.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -180,33 +180,41 @@
 `numbers_parser` currently only supports paragraph styles and cell styles. The following paragraph styles are suppoprted:
 
 * font attributes: bold, italic, underline, strikethrough
 * font selection and size
 * text foreground color
 * horizontal and vertical alignment
 * cell background color
+* cell indents (first line, left, right, and text inset)
 
 Table styles that allow new tables to adopt a style across the whole table are not planned.
 
+Numbers conflates style attributes that can be stored in paragraph styles (the style menu in the text panel) with the settings that are available on the Style tab of the Text panel. Some attributes in Numbers are not applied to new cells when a style is applied. To keep the API simple, `numbers-parser` packs all styling into a single `Style` object. When a document is saved, the attributes not stored in a paragraph style are applied to each cell that includes it. Attributes behaving in this way are currently `Cell.alignment.vertical` and `Cell.style.text_inset`. The cell background colour `Cell.style.bg_color` also behaves this way, though this is in line with the separation in Numbers.
+
 #### Reading styles
 
 The cell method `style` returns a `Style` object containing all the style information for that cell. Cells with identical style settings contain references to a single style object.
 
-Cell text fonts can be returned using a number of methods.
+Cell style attributes can be returned using a number of methods:
 
 * `Cell.style.alignment`: the horizontal and vertical alignment of the cell as an `Alignment` names tuple
 * `Cell.style.bg_color`: cell background color as an `RGB` named tuple, or a list of `RGB` values for gradients
 * `Cell.style.bold`: `True` if the cell font is bold
 * `Cell.style.font_color`: font color as an `RGB` named tuple
 * `Cell.style.font_size`: font size in points (`float`)
 * `Cell.style.font_name`: font name (`str`)
 * `Cell.style.italic`: `True` if the cell font is italic
 * `Cell.style.name`: cell style (`str`)
 * `Cell.style.underline`: `True` if the cell font is underline
 * `Cell.style.strikethrough`: `True` if the cell font is strikethrough
+* `Cell.style.first_indent`: first line indent in points (`float`)
+* `Cell.style.left_indent`: left indent in points (`float`)
+* `Cell.style.right_indent`: right indent in points (`float`)
+* `Cell.style.text_inset`: text inset in points (`float`)
+
 
 #### Cell images
 
 The methods `style.bg_image.filename` and `style.bg_image.data` return data about the image used for a cell's background, where set. If a cell has no background image, `style.bg_image`  is `None`.
 
 ``` python
 cell = table.cell("B1")
```

### Comparing `numbers_parser-4.1.2/pyproject.toml` & `numbers_parser-4.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 description = "Read and write Apple Numbers spreadsheets"
 documentation = "https://github.com/masaccio/numbers-parser/blob/main/README.md"
 license = "MIT"
 name = "numbers-parser"
 packages = [{include = "numbers_parser", from = "src"}]
 readme = "README.md"
 repository = "https://github.com/masaccio/numbers-parser"
-version = "4.1.2"
+version = "4.2.0"
 
 [tool.poetry.scripts]
 cat-numbers = "numbers_parser._cat_numbers:main"
 unpack-numbers = "numbers_parser._unpack_numbers:main"
 
 [tool.poetry.dependencies]
 compact-json = "^1.1.3"
```

### Comparing `numbers_parser-4.1.2/src/numbers_parser/__init__.py` & `numbers_parser-4.2.0/src/numbers_parser/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,35 +44,29 @@
     "13.1",
 ]
 
 # Don't print the source line
 old_warn_f = warnings.formatwarning
 warnings.formatwarning = (
     # pragma: no cover -- lambda not run by coverage
-    lambda msg, catg, fname, lineno, line=None: old_warn_f(
-        msg, catg, fname, lineno, line=""
-    )
+    lambda msg, catg, fname, lineno, line=None: old_warn_f(msg, catg, fname, lineno, line="")
 )
 
 
 def _get_version():
     return __version__
 
 
 def _check_installed_numbers_version():
     try:
-        fp = open(
-            os.path.join(_DEFAULT_NUMBERS_INSTALL_PATH, _VERSION_PLIST_PATH), "rb"
-        )
+        fp = open(os.path.join(_DEFAULT_NUMBERS_INSTALL_PATH, _VERSION_PLIST_PATH), "rb")
     except IOError:
         return None
     version_dict = plistlib.load(fp)
     installed_version = version_dict["CFBundleShortVersionString"]
     if installed_version not in _SUPPORTED_NUMBERS_VERSIONS:
-        warnings.warn(
-            f"Numbers version {installed_version} not tested with this version"
-        )
+        warnings.warn(f"Numbers version {installed_version} not tested with this version")
     fp.close()
     return installed_version
 
 
 _ = _check_installed_numbers_version()
```

### Comparing `numbers_parser-4.1.2/src/numbers_parser/_cat_numbers.py` & `numbers_parser-4.2.0/src/numbers_parser/_cat_numbers.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,17 +50,15 @@
     parser.add_argument(
         "-s", "--sheet", action="append", help="Names of sheet(s) to include in export"
     )
     parser.add_argument(
         "-t", "--table", action="append", help="Names of table(s) to include in export"
     )
     parser.add_argument("document", nargs="*", help="Document(s) to export")
-    parser.add_argument(
-        "--debug", default=False, action="store_true", help="Enable debug logging"
-    )
+    parser.add_argument("--debug", default=False, action="store_true", help="Enable debug logging")
     parser.add_argument(
         "--experimental", default=False, action="store_true", help=argparse.SUPPRESS
     )
     return parser
 
 
 def print_sheet_names(filename):
```

### Comparing `numbers_parser-4.1.2/src/numbers_parser/_unpack_numbers.py` & `numbers_parser-4.2.0/src/numbers_parser/_unpack_numbers.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,27 +103,21 @@
 
 
 def main():
     parser = ArgumentParser()
     parser.add_argument("document", help="Apple Numbers file(s)", nargs="*")
     parser.add_argument("-V", "--version", action="store_true")
     parser.add_argument("--hex-uuids", action="store_true", help="print UUIDs as hex")
-    parser.add_argument(
-        "--pretty-storage", action="store_true", help="pretty print cell storage"
-    )
+    parser.add_argument("--pretty-storage", action="store_true", help="pretty print cell storage")
     parser.add_argument(
         "--compact-json", action="store_true", help="Format JSON compactly as possible"
     )
-    parser.add_argument(
-        "--pretty", action="store_true", help="Enable all prettifying options"
-    )
+    parser.add_argument("--pretty", action="store_true", help="Enable all prettifying options")
     parser.add_argument("--output", "-o", help="directory name to unpack into")
-    parser.add_argument(
-        "--debug", default=False, action="store_true", help="Enable debug logging"
-    )
+    parser.add_argument("--debug", default=False, action="store_true", help="Enable debug logging")
     args = parser.parse_args()
     if args.version:
         print(_get_version())
     elif args.output is not None and len(args.document) > 1:
         print(
             "unpack-numbers: error: output directory only valid with a single document",
             file=sys.stderr,
```

### Comparing `numbers_parser-4.1.2/src/numbers_parser/bullets.py` & `numbers_parser-4.2.0/src/numbers_parser/bullets.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/cell.py` & `numbers_parser-4.2.0/src/numbers_parser/cell.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import re
 import warnings
 
 from numbers_parser.generated import TSTArchives_pb2 as TSTArchives
 from numbers_parser.generated.TSWPArchives_pb2 import (
     ParagraphStylePropertiesArchive as ParagraphStyle,
 )
-from numbers_parser.exceptions import UnsupportedError
+from numbers_parser.exceptions import UnsupportedError, UnsupportedWarning
 from numbers_parser.cell_storage import CellType, CellStorage
 from numbers_parser.constants import (
     EMPTY_STORAGE_BUFFER,
     DEFAULT_FONT,
     DEFAULT_FONT_SIZE,
     DEFAULT_ALIGNMENT,
+    DEFAULT_TEXT_INSET,
+    DEFAULT_BORDER_WIDTH,
+    DEFAULT_BORDER_COLOR,
+    DEFAULT_BORDER_STYLE,
 )
 
 from dataclasses import dataclass
 from collections import namedtuple
 from enum import IntEnum
 from functools import lru_cache
 from pendulum import duration, Duration, DateTime
@@ -34,19 +38,14 @@
 
     @property
     def filename(self) -> str:
         """The image filename for a cell, or None if no image."""
         return self._filename
 
 
-# Style return types
-_Alignment = namedtuple("Alignment", ["horizontal", "vertical"])
-RGB = namedtuple("RGB", ["r", "g", "b"])
-
-
 class HorizontalJustification(IntEnum):
     LEFT = ParagraphStyle.TextAlignmentType.TATvalue0
     RIGHT = ParagraphStyle.TextAlignmentType.TATvalue1
     CENTER = ParagraphStyle.TextAlignmentType.TATvalue2
     JUSTIFIED = ParagraphStyle.TextAlignmentType.TATvalue3
     AUTO = ParagraphStyle.TextAlignmentType.TATvalue4
 
@@ -67,14 +66,16 @@
 
 VERTICAL_MAP = {
     "top": VerticalJustification.TOP,
     "middle": VerticalJustification.MIDDLE,
     "bottom": VerticalJustification.BOTTOM,
 }
 
+_Alignment = namedtuple("Alignment", ["horizontal", "vertical"])
+
 
 class Alignment(_Alignment):
     def __new__(cls, horizontal=DEFAULT_ALIGNMENT[0], vertical=DEFAULT_ALIGNMENT[1]):
         if isinstance(horizontal, str):
             horizontal = horizontal.lower()
             if horizontal not in HORIZONTAL_MAP:
                 raise TypeError("invalid horizontal alignment")
@@ -88,27 +89,33 @@
 
         self = super(_Alignment, cls).__new__(cls, (horizontal, vertical))
         return self
 
 
 DEFAULT_ALIGNMENT_CLASS = Alignment(*DEFAULT_ALIGNMENT)
 
+RGB = namedtuple("RGB", ["r", "g", "b"])
+
 
 @dataclass
 class Style:
     alignment: Alignment = DEFAULT_ALIGNMENT_CLASS
     bg_image: object = None
     bg_color: Union[RGB, List[RGB]] = None
     font_color: RGB = RGB(0, 0, 0)
     font_size: float = DEFAULT_FONT_SIZE
     font_name: str = DEFAULT_FONT
     bold: bool = False
     italic: bool = False
     strikethrough: bool = False
     underline: bool = False
+    first_indent: float = 0
+    left_indent: float = 0
+    right_indent: float = 0
+    text_inset: float = DEFAULT_TEXT_INSET
     name: str = None
     _text_style_obj_id: int = None
     _cell_style_obj_id: int = None
     _update_cell_style: bool = False
     _update_text_style: bool = False
 
     @staticmethod
@@ -118,14 +125,29 @@
             "font_size",
             "font_name",
             "bold",
             "italic",
             "strikethrough",
             "underline",
             "name",
+            "first_indent",
+            "left_indent",
+            "right_indent",
+            "text_inset",
+        ]
+
+    @staticmethod
+    def _cell_attrs():
+        return [
+            "alignment",
+            "bg_color",
+            "first_indent",
+            "left_indent",
+            "right_indent",
+            "text_inset",
         ]
 
     @classmethod
     def from_storage(cls, cell_storage: object, model: object):
         style = Style()
 
         if cell_storage.image_data is not None:
@@ -140,23 +162,24 @@
             font_size=model.cell_font_size(cell_storage),
             font_name=model.cell_font_name(cell_storage),
             bold=model.cell_is_bold(cell_storage),
             italic=model.cell_is_italic(cell_storage),
             strikethrough=model.cell_is_strikethrough(cell_storage),
             underline=model.cell_is_underline(cell_storage),
             name=model.cell_style_name(cell_storage),
+            first_indent=model.cell_first_indent(cell_storage),
+            left_indent=model.cell_left_indent(cell_storage),
+            right_indent=model.cell_right_indent(cell_storage),
+            text_inset=model.cell_text_inset(cell_storage),
             _text_style_obj_id=model.text_style_object_id(cell_storage),
             _cell_style_obj_id=model.cell_style_object_id(cell_storage),
         )
         return style
 
     def __post_init__(self):
-        if not isinstance(self.alignment, Alignment):
-            raise TypeError("value must be an Alignment class")
-
         self.bg_color = rgb_color(self.bg_color)
         self.font_color = rgb_color(self.font_color)
 
         if not isinstance(self.font_size, float):
             raise TypeError("size must be a float number of points")
         if not isinstance(self.font_name, str):
             raise TypeError("font name must be a string")
@@ -164,33 +187,23 @@
         for field in ["bold", "italic", "underline", "strikethrough"]:
             if not isinstance(getattr(self, field), bool):
                 raise TypeError(f"{field} argument must be boolean")
 
     def __setattr__(self, name: str, value: Any) -> None:
         """Detect changes to cell styles and flag the style for
         possible updates when saving the document"""
-        if name in self.__dict__:
-            # Init has been done
-            if name in ["bg_color", "font_color"]:
-                value = rgb_color(value)
-            if name in ["bg_color"]:
-                self.__dict__["_update_cell_style"] = True
-            elif name in ["alignment"]:
-                self.__dict__["_update_text_style"] = True
-                self.__dict__["_update_cell_style"] = True
-            elif name in Style._text_attrs():
-                self.__dict__["_update_text_style"] = True
-        elif name == "bg_color" and value is not None:
-            self.__dict__["_update_cell_style"] = True
-        elif (
-            name == "alignment"
-            and value is not None
-            and value[1] != DEFAULT_ALIGNMENT_CLASS[1]
-        ):
+        if name in ["bg_color", "font_color"]:
+            value = rgb_color(value)
+        if name == "alignment":
+            value = alignment(value)
+        if name in Style._text_attrs():
+            self.__dict__["_update_text_style"] = True
+        if name in Style._cell_attrs():
             self.__dict__["_update_cell_style"] = True
+
         if name not in ["_update_text_style", "_update_cell_style"]:
             self.__dict__[name] = value
 
 
 def rgb_color(color) -> RGB:
     """Raise a TypeError if a color is not a valid RGB value"""
     if color is None:
@@ -199,31 +212,167 @@
         return color
     if isinstance(color, tuple):
         if not (len(color) == 3 and all([isinstance(x, int) for x in color])):
             raise TypeError("RGB color must be an RGB or a tuple of 3 integers")
         return RGB(*color)
     elif isinstance(color, list):
         return [rgb_color(c) for c in color]
+    raise TypeError("RGB color must be an RGB or a tuple of 3 integers")
+
+
+def alignment(value) -> Alignment:
+    """Raise a TypeError if a alignment is not a valid"""
+    if value is None:
+        return Alignment()
+    if isinstance(value, Alignment):
+        return value
+    if isinstance(value, tuple):
+        if not (len(value) == 2 and all([isinstance(x, (int, str)) for x in value])):
+            raise TypeError("Alignment must be an Alignment or a tuple of 2 integers/strings")
+        return Alignment(*value)
+    raise TypeError("Alignment must be an Alignment or a tuple of 2 integers/strings")
+
+
+BORDER_STYLE_MAP = {"solid": 0, "dashes": 1, "dots": 2, "none": 3}
+
+
+class BorderType(IntEnum):
+    SOLID = BORDER_STYLE_MAP["solid"]
+    DASHES = BORDER_STYLE_MAP["dashes"]
+    DOTS = BORDER_STYLE_MAP["dots"]
+    NONE = BORDER_STYLE_MAP["none"]
+
+
+class Border:
+    def __init__(
+        self,
+        width: float = DEFAULT_BORDER_WIDTH,
+        color: RGB = RGB(*DEFAULT_BORDER_COLOR),
+        style: BorderType = BorderType(BORDER_STYLE_MAP[DEFAULT_BORDER_STYLE]),
+        _order: int = 0,
+    ):
+        if not isinstance(width, float):
+            raise TypeError("width must be a float number of points")
+        self.width = width
+
+        self.color = rgb_color(color)
+
+        if isinstance(style, str):
+            style = style.lower()
+            if style not in BORDER_STYLE_MAP:
+                raise TypeError("invalid border style")
+            self.style = BORDER_STYLE_MAP[style]
+        else:
+            self.style = style
+
+        self._order = _order
+
+    def __repr__(self) -> str:
+        style_name = BorderType(self.style).name.lower()
+        return f"Border(width={self.width}, color={self.color}, style={style_name})"
+
+    def __eq__(self, value: object) -> bool:
+        return all(
+            [self.width == value.width, self.color == value.color, self.style == value.style]
+        )
+
+
+class CellBorder:
+    def __init__(
+        self,
+        top_merged: bool = False,
+        right_merged: bool = False,
+        bottom_merged: bool = False,
+        left_merged: bool = False,
+    ):
+        self._top = None
+        self._right = None
+        self._bottom = None
+        self._left = None
+        self._top_merged = top_merged
+        self._right_merged = right_merged
+        self._bottom_merged = bottom_merged
+        self._left_merged = left_merged
+
+    @property
+    def top(self):
+        if self._top_merged:
+            return None
+        elif self._top is None:
+            return None
+        return self._top
+
+    @top.setter
+    def top(self, value):
+        if self._top is None:
+            self._top = value
+        elif value._order > self.top._order:
+            self._top = value
+
+    @property
+    def right(self):
+        if self._right_merged:
+            return None
+        elif self._right is None:
+            return None
+        return self._right
+
+    @right.setter
+    def right(self, value):
+        if self._right is None:
+            self._right = value
+        elif value._order > self._right._order:
+            self._right = value
+
+    @property
+    def bottom(self):
+        if self._bottom_merged:
+            return None
+        elif self._bottom is None:
+            return None
+        return self._bottom
+
+    @bottom.setter
+    def bottom(self, value):
+        if self._bottom is None:
+            self._bottom = value
+        elif value._order > self._bottom._order:
+            self._bottom = value
+
+    @property
+    def left(self):
+        if self._left_merged:
+            return None
+        elif self._left is None:
+            return None
+        return self._left
+
+    @left.setter
+    def left(self, value):
+        if self._left is None:
+            self._left = value
+        elif value._order > self._left._order:
+            self._left = value
 
 
 class Cell:
     @classmethod
     def empty_cell(cls, table_id: int, row_num: int, col_num: int, model: object):
         row_col = (row_num, col_num)
         merge_cells = model.merge_cell_ranges(table_id)
         is_merged = row_col in merge_cells
 
         if is_merged and merge_cells[row_col]["merge_type"] == "ref":
-            cell = MergedCell(*merge_cells[row_col]["rect"])
+            cell = MergedCell(*merge_cells[row_col]["rect"], row_num, col_num)
         else:
             cell = EmptyCell(row_num, col_num)
         cell.size = None
         cell._model = model
         cell._table_id = table_id
-        cell.style = None
+        cell._style = None
         return cell
 
     @classmethod
     def from_storage(cls, cell_storage: CellStorage):  # noqa: C901
         row_col = (cell_storage.row_num, cell_storage.col_num)
         merge_cells = cell_storage.model.merge_cell_ranges(cell_storage.table_id)
         is_merged = row_col in merge_cells
@@ -256,14 +405,19 @@
         cell._storage = cell_storage
         cell._formula_key = cell_storage.formula_id
         cell._style = None
 
         if is_merged and merge_cells[row_col]["merge_type"] == "source":
             cell.is_merged = True
             cell.size = merge_cells[row_col]["size"]
+            right_merged = cell.size[0] > 1
+            bottom_merged = cell.size[1] > 1
+            cell._border = CellBorder(False, right_merged, bottom_merged, False)
+        else:
+            cell._border = CellBorder()
 
         return cell
 
     def __init__(self, row_num: int, col_num: int, value):
         self._value = value
         self.row = row_num
         self.col = col_num
@@ -331,14 +485,25 @@
             self._style = Style.from_storage(self._storage, self._model)
         return self._style
 
     @style.setter
     def style(self, style):
         self._style = style
 
+    @property
+    def border(self):
+        self._model.extract_strokes(self._table_id)
+        return self._border
+
+    @border.setter
+    def border(self, _):
+        warnings.warn(
+            "cell border values cannot be set; use Table.add_border() instead", UnsupportedWarning
+        )
+
 
 class NumberCell(Cell):
     def __init__(self, row_num: int, col_num: int, value: float):
         self._type = TSTArchives.numberCellType
         super().__init__(row_num, col_num, value)
 
     @property
@@ -391,16 +556,17 @@
 # Backwards compatibility to earlier class names
 class BulletedTextCell(RichTextCell):
     pass
 
 
 class EmptyCell(Cell):
     def __init__(self, row_num: int, col_num: int):
-        self._type = None
         super().__init__(row_num, col_num, None)
+        self._type = None
+        self._border = CellBorder()
 
     @property
     def value(self):
         return None
 
 
 class BoolCell(Cell):
@@ -440,23 +606,31 @@
         super().__init__(row_num, col_num, None)
 
     @property
     def value(self):
         return None
 
 
-class MergedCell:
-    def __init__(self, row_start: int, col_start: int, row_end: int, col_end: int):
+class MergedCell(Cell):
+    def __init__(
+        self, row_start: int, col_start: int, row_end: int, col_end: int, row_num: int, col_num: int
+    ):
+        super().__init__(row_num, col_num, None)
         self.value = None
-        self.formula = None
         self.row_start = row_start
         self.row_end = row_end
         self.col_start = col_start
         self.col_end = col_end
+        self.is_merged = False
         self.merge_range = xl_range(row_start, col_start, row_end, col_end)
+        top_merged = row_num > row_start
+        right_merged = col_num < col_end
+        bottom_merged = row_num < row_end
+        left_merged = col_num > col_start
+        self._border = CellBorder(top_merged, right_merged, bottom_merged, left_merged)
 
 
 # Cell reference conversion from  https://github.com/jmcnamara/XlsxWriter
 # Copyright (c) 2013-2021, John McNamara <jmcnamara@cpan.org>
 range_parts = re.compile(r"(\$?)([A-Z]{1,3})(\$?)(\d+)")
```

### Comparing `numbers_parser-4.1.2/src/numbers_parser/cell_storage.py` & `numbers_parser-4.2.0/src/numbers_parser/cell_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,17 +118,15 @@
         "text_format_id",
         "bool_format_id",
         # "comment_id",
         # "import_warning_id",
     )
 
     # @profile
-    def __init__(  # noqa: C901
-        self, model: object, table_id: int, buffer, row_num, col_num
-    ):
+    def __init__(self, model: object, table_id: int, buffer, row_num, col_num):  # noqa: C901
         self.buffer = buffer
         self.model = model
         self.table_id = table_id
         self.row_num = row_num
         self.col_num = col_num
 
         self.d128 = None
@@ -301,17 +299,15 @@
         datas = self.model.objects[PACKAGE_ID].datas
         image_file_names = [x.file_name for x in datas if x.identifier == image_id]
         if len(image_file_names) == 0:  # pragma: no cover
             warn(f"No image found with ID {image_id}", UnsupportedWarning)
             return None
 
         image_path_name = [
-            x
-            for x in self.model.objects.file_store.keys()
-            if x == f"Data/{image_file_names[0]}"
+            x for x in self.model.objects.file_store.keys() if x == f"Data/{image_file_names[0]}"
         ][0]
         return (self.model.objects.file_store[image_path_name], image_file_names[0])
 
     def custom_format(self) -> str:
         if self.text_format_id is not None and self.type == CellType.TEXT:
             format = self.model.table_format(self.table_id, self.text_format_id)
         elif self.currency_format_id is not None:
@@ -361,21 +357,17 @@
         format = self.model.table_format(self.table_id, self.date_format_id)
         if format.HasField("custom_uid"):
             format_uuid = NumbersUUID(format.custom_uid).hex
             format_map = self.model.custom_format_map()
             custom_format = format_map[format_uuid].default_format
             custom_format_string = custom_format.custom_format_string
             if custom_format.format_type == FormatType.CUSTOM_DATE:
-                formatted_value = decode_date_format(
-                    custom_format_string, self.datetime
-                )
+                formatted_value = decode_date_format(custom_format_string, self.datetime)
             else:  # pragma: no cover
-                raise UnsupportedError(
-                    f"Unexpected custom format type {custom_format.format_type}"
-                )
+                raise UnsupportedError(f"Unexpected custom format type {custom_format.format_type}")
         else:
             formatted_value = decode_date_format(format.date_time_format, self.datetime)
         return formatted_value
 
     def duration_format(self) -> str:  # noqa: C901
         format = self.model.table_format(self.table_id, self.duration_format_id)
 
@@ -436,17 +428,15 @@
         if unit_smallest >= DurationUnits.MILLISECOND:
             dd = int(round(1000 * d))
             if duration_style == DurationStyle.COMPACT:
                 padding = "0" if dd >= 10 else "00"
                 padding = "" if dd >= 100 else padding
                 dstr.append(f"{padding}{dd}")
             else:
-                dstr.append(
-                    str(dd) + unit_format("millisecond", dd, duration_style, "ms")
-                )
+                dstr.append(str(dd) + unit_format("millisecond", dd, duration_style, "ms"))
         duration_str = (":" if duration_style == 0 else " ").join(dstr)
         if duration_style == DurationStyle.COMPACT:
             duration_str = re.sub(r":(\d\d\d)$", r".\1", duration_str)
 
         return duration_str
```

### Comparing `numbers_parser-4.1.2/src/numbers_parser/constants.py` & `numbers_parser-4.2.0/src/numbers_parser/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,18 +9,23 @@
 DEFAULT_COLUMN_COUNT = 5
 DEFAULT_COLUMN_WIDTH = 98.0
 DEFAULT_PRE_BNC_BYTES = "🤠".encode("utf-8")  # Yes, really!
 DEFAULT_ROW_COUNT = 10
 DEFAULT_ROW_HEIGHT = 20.0
 DEFAULT_TABLE_OFFSET = 80.0
 DEFAULT_TILE_SIZE = 256
+
+# Style defaults
+DEFAULT_ALIGNMENT = ("auto", "top")
+DEFAULT_BORDER_WIDTH = 0.35
+DEFAULT_BORDER_COLOR = (0, 0, 0)
+DEFAULT_BORDER_STYLE = "solid"
 DEFAULT_FONT = "Helvetica Neue"
 DEFAULT_FONT_SIZE = 11.0
-DEFAULT_ALIGNMENT = ("auto", "top")
-
+DEFAULT_TEXT_INSET = 4.0
 EMPTY_STORAGE_BUFFER = b"\x05\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"
 
 # Numbers limits
 MAX_TILE_SIZE = 256
 MAX_ROW_COUNT = 1000000
 MAX_COL_COUNT = 1000
 MAX_HEADER_COUNT = 5
```

### Comparing `numbers_parser-4.1.2/src/numbers_parser/containers.py` & `numbers_parser-4.2.0/src/numbers_parser/containers.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/data/empty.numbers` & `numbers_parser-4.2.0/src/numbers_parser/data/empty.numbers`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/document.py` & `numbers_parser-4.2.0/src/numbers_parser/document.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     DurationCell,
     DateCell,
     Cell,
     MergedCell,
     xl_cell_to_rowcol,
     xl_range,
     Style,
+    Border,
 )
 from numbers_parser.cell_storage import CellStorage
 from numbers_parser.constants import DEFAULT_COLUMN_COUNT, DEFAULT_ROW_COUNT
 
 
 class Document:
     def __init__(self, filename=None):
@@ -154,14 +155,15 @@
         self._model = model
         self._table_id = table_id
         self.num_rows = self._model.number_of_rows(self._table_id)
         self.num_cols = self._model.number_of_columns(self._table_id)
         # Cache all data now to facilite write(). Performance impact
         # of computing all cells is minimal compared to file IO
         self._data = []
+        self._model.set_table_data(table_id, self._data)
         for row_num in range(self.num_rows):
             self._data.append([])
             for col_num in range(self.num_cols):
                 cell_storage = model.table_cell_decode(table_id, row_num, col_num)
                 if cell_storage is None:
                     cell = Cell.empty_cell(table_id, row_num, col_num, model)
                 else:
@@ -203,17 +205,15 @@
     def num_header_cols(self, num_headers: int):
         """Return the number of header columns"""
         if num_headers < 0:
             raise ValueError("Number of headers cannot be negative")
         elif num_headers > self.num_cols:
             raise ValueError("Number of headers cannot exceed the number of columns")
         elif num_headers > MAX_HEADER_COUNT:
-            raise ValueError(
-                f"Number of headers cannot exceed {MAX_HEADER_COUNT} columns"
-            )
+            raise ValueError(f"Number of headers cannot exceed {MAX_HEADER_COUNT} columns")
         return self._model.num_header_cols(self._table_id, num_headers)
 
     @property
     def height(self) -> int:
         """Return the table's height in points"""
         return self._model.table_height(self._table_id)
 
@@ -367,53 +367,49 @@
                 yield tuple(row[col_num] for row in rows[min_row : max_row + 1])
 
     def _validate_cell_coords(self, *args):
         """Check first arguments are value cell references and pad
         the table with empty cells if outside current bounds"""
         if type(args[0]) == str:
             (row_num, col_num) = xl_cell_to_rowcol(args[0])
-            value = args[1]
+            values = args[1:]
         elif len(args) < 2:
             raise IndexError("invalid cell reference " + str(args))
         else:
             (row_num, col_num) = args[0:2]
-            value = args[2]
+            values = args[2:]
 
         if row_num >= MAX_ROW_COUNT:
             raise IndexError(f"{row_num} exceeds maximum row {MAX_ROW_COUNT-1}")
         if col_num >= MAX_COL_COUNT:
             raise IndexError(f"{col_num} exceeds maximum column {MAX_COL_COUNT-1}")
 
         for row in range(self.num_rows, row_num + 1):
             self.add_row()
 
         for row in range(self.num_cols, col_num + 1):
             self.add_column()
 
-        return (row_num, col_num, value)
+        return (row_num, col_num) + tuple(values)
 
     def write(self, *args, style=None):
         (row_num, col_num, value) = self._validate_cell_coords(*args)
 
         if type(value) == str:
             self._data[row_num][col_num] = TextCell(row_num, col_num, value)
         elif type(value) == int or type(value) == float:
             self._data[row_num][col_num] = NumberCell(row_num, col_num, value)
         elif type(value) == bool:
             self._data[row_num][col_num] = BoolCell(row_num, col_num, value)
         elif type(value) == builtin_datetime or type(value) == DateTime:
-            self._data[row_num][col_num] = DateCell(
-                row_num, col_num, pendulum_instance(value)
-            )
+            self._data[row_num][col_num] = DateCell(row_num, col_num, pendulum_instance(value))
         elif type(value) == builtin_timedelta or type(value) == Duration:
             self._data[row_num][col_num] = DurationCell(row_num, col_num, value)
         else:
-            raise ValueError(
-                "Can't determine cell type from type " + type(value).__name__
-            )
+            raise ValueError("Can't determine cell type from type " + type(value).__name__)
         self._data[row_num][col_num]._storage = CellStorage(
             self._model, self._table_id, None, row_num, col_num
         )
         self._data[row_num][col_num]._table_id = self._table_id
         self._data[row_num][col_num]._model = self._model
 
         if style is not None:
@@ -427,17 +423,15 @@
             if style not in self._model.styles:
                 raise IndexError(f"style '{style}' does not exist")
             self._data[row_num][col_num]._style = self._model.styles[style]
         else:
             raise TypeError("style must be a Style object or style name")
 
     def add_row(self, num_rows=1):
-        row = [
-            EmptyCell(self.num_rows - 1, col_num) for col_num in range(self.num_cols)
-        ]
+        row = [EmptyCell(self.num_rows - 1, col_num) for col_num in range(self.num_cols)]
         for _ in range(num_rows):
             self._data.append(row.copy())
             self.num_rows += 1
             self._model.number_of_rows(self._table_id, self.num_rows)
 
     def add_column(self, num_cols=1):
         for _ in range(num_cols):
@@ -465,7 +459,38 @@
             for row_num in range(row_start + 1, row_end + 1):
                 for col_num in range(col_start + 1, col_end + 1):
                     merge_ranges[(row_num, col_num)] = {
                         "merge_type": "ref",
                         "rect": (row_start, col_start, row_end, col_end),
                         "size": (num_rows, num_cols),
                     }
+
+    def add_border(self, *args):
+        (row_num, col_num, *args) = self._validate_cell_coords(*args)
+        if len(args) == 2:
+            (side, border_value) = args
+            length = 1
+        elif len(args) == 3:
+            (side, border_value, length) = args
+        else:
+            raise TypeError("invalid number of arguments to border_value()")
+
+        if not isinstance(border_value, Border):
+            raise TypeError("border value must be a Border object")
+
+        if not isinstance(length, int):
+            raise TypeError("border length must be an int")
+
+        if side == "top" or side == "bottom":
+            for border_col_num in range(col_num, col_num + length):
+                self._model.set_cell_border(
+                    self._table_id, row_num, border_col_num, side, border_value
+                )
+        elif side == "left" or side == "right":
+            for border_row_num in range(row_num, row_num + length):
+                self._model.set_cell_border(
+                    self._table_id, border_row_num, col_num, side, border_value
+                )
+        else:
+            raise TypeError("side must be a valid border segment")
+
+        self._model.add_stroke(self._table_id, row_num, col_num, side, border_value, length)
```

### Comparing `numbers_parser-4.1.2/src/numbers_parser/exceptions.py` & `numbers_parser-4.2.0/src/numbers_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/file.py` & `numbers_parser-4.2.0/src/numbers_parser/file.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,45 +12,39 @@
 debug = logger.debug
 
 
 def read_numbers_file(path, file_handler, object_handler=None):
     debug("read_numbers_file: path=%s", path)
     if os.path.isdir(path):
         if os.path.isfile(os.path.join(path, "Index.zip")):
-            get_objects_from_zip_file(
-                os.path.join(path, "Index.zip"), file_handler, object_handler
-            )
+            get_objects_from_zip_file(os.path.join(path, "Index.zip"), file_handler, object_handler)
         else:
             for filename in os.listdir(path):
                 filepath = os.path.join(path, filename)
                 if os.path.isdir(filepath):
                     read_numbers_file(filepath, file_handler, object_handler)
                 else:
                     f = open(filepath, "rb")
                     if filename.endswith(".iwa"):
                         blob = f.read()
-                        extract_iwa_archives(
-                            blob, filepath, file_handler, object_handler
-                        )
+                        extract_iwa_archives(blob, filepath, file_handler, object_handler)
                     blob = f.read()
                     file_handler(os.path.join(path, filename), blob)
     else:
         try:
             zipf = ZipFile(path)
         except BadZipFile:
             raise FileError("Invalid Numbers file")
         except FileNotFoundError:
             raise FileError("No such file or directory")
 
         index_zip = [f for f in zipf.namelist() if f.lower().endswith("index.zip")]
         if len(index_zip) > 0:
             index_data = BytesIO(zipf.read(index_zip[0]))
-            get_objects_from_zip_stream(
-                ZipFile(index_data), file_handler, object_handler
-            )
+            get_objects_from_zip_stream(ZipFile(index_data), file_handler, object_handler)
         else:
             get_objects_from_zip_stream(zipf, file_handler, object_handler)
 
 
 def write_numbers_file(filename, file_store):
     zipf = ZipFile(filename, "w")
     for filename, blob in file_store.items():
@@ -88,22 +82,18 @@
         debug("extract_iwa_archives: filename=%s", filename)
         iwaf = IWAFile.from_buffer(blob, filename)
     except Exception as e:  # pragma: no cover
         raise FileFormatError(f"{filename}: invalid IWA file {filename}") from e
 
     if object_handler is not None:
         if len(iwaf.chunks) != 1:
-            raise FileFormatError(
-                f"{filename}: chunk count != 1 in {filename}"
-            )  # pragma: no cover
+            raise FileFormatError(f"{filename}: chunk count != 1 in {filename}")  # pragma: no cover
         for archive in iwaf.chunks[0].archives:
             if len(archive.objects) == 0:
-                raise FileFormatError(
-                    f"{filename}: no objects in {filename}"
-                )  # pragma: no cover
+                raise FileFormatError(f"{filename}: no objects in {filename}")  # pragma: no cover
 
             identifier = archive.header.identifier
             if len(archive.objects) > 1:
                 # TODO: what should we do for len(archive.objects) > 1?
                 pass
             object_handler(identifier, archive.objects[0], filename)
```

### Comparing `numbers_parser-4.1.2/src/numbers_parser/formula.py` & `numbers_parser-4.2.0/src/numbers_parser/formula.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TNArchives_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TNArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TNArchives_sos_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TNArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TNCommandArchives_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TNCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TSAArchives_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TSAArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TSAArchives_sos_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TSAArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TSCEArchives_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TSCEArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TSCH3DArchives_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TSCH3DArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TSCHArchives_Common_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TSCHArchives_Common_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TSCHArchives_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TSCHArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TSCHArchives_sos_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TSCHArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TSCHCommandArchives_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TSCHCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TSDArchives_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TSDArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TSDArchives_sos_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TSDArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TSDCommandArchives_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TSDCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TSKArchives_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TSKArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TSKArchives_sos_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TSKArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TSPArchiveMessages_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TSPArchiveMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TSPMessages_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TSPMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TSSArchives_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TSSArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TSSArchives_sos_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TSSArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TSTArchives_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TSTArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TSTArchives_sos_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TSTArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TSTCommandArchives_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TSTCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TSWPArchives_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TSWPArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TSWPArchives_sos_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TSWPArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/TSWPCommandArchives_pb2.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/TSWPCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/fontmap.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/fontmap.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/generated/functionmap.py` & `numbers_parser-4.2.0/src/numbers_parser/generated/functionmap.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.2/src/numbers_parser/iwafile.py` & `numbers_parser-4.2.0/src/numbers_parser/iwafile.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,18 +109,15 @@
     def to_buffer(self):
         uncompressed = b"".join([archive.to_buffer() for archive in self.archives])
         payloads = []
         while uncompressed:
             payloads.append(snappy.compress(uncompressed[:65536]))
             uncompressed = uncompressed[65536:]
         return b"".join(
-            [
-                b"\x00" + struct.pack("<I", len(payload))[:3] + payload
-                for payload in payloads
-            ]
+            [b"\x00" + struct.pack("<I", len(payload))[:3] + payload for payload in payloads]
         )
 
 
 class ProtobufPatch(object):
     def __init__(self, data):
         self.data = data
 
@@ -146,17 +143,15 @@
 
 class IWAArchiveSegment(object):
     def __init__(self, header, objects):
         self.header = header
         self.objects = objects
 
     def __eq__(self, other):
-        return (
-            self.header == other.header and self.objects == other.objects
-        )  # pragma: no cover
+        return self.header == other.header and self.objects == other.objects  # pragma: no cover
 
     def __repr__(self):
         return "<%s identifier=%s objects=%s>" % (  # pragma: no cover
             self.__class__.__name__,
             self.header.identifier,
             repr(self.objects).replace("\n", " ").replace("  ", " "),
         )
@@ -171,28 +166,25 @@
 
         payloads = []
 
         n = 0
         for message_info in archive_info.message_infos:
             try:
                 if message_info.type == 0 and archive_info.should_merge and payloads:
-                    base_message = archive_info.message_infos[
-                        message_info.base_message_index
-                    ]
+                    base_message = archive_info.message_infos[message_info.base_message_index]
                     klass = partial(
                         ProtobufPatch.FromString,
                         message_info,
                         ID_NAME_MAP[base_message.type],
                     )
                 else:
                     klass = ID_NAME_MAP[message_info.type]
             except KeyError:  # pragma: no cover
                 raise NotImplementedError(
-                    "Don't know how to parse Protobuf message type "
-                    + str(message_info.type)
+                    "Don't know how to parse Protobuf message type " + str(message_info.type)
                 )
             try:
                 message_payload = payload[n : n + message_info.length]
                 if hasattr(klass, "FromString"):
                     output = klass.FromString(message_payload)
                 else:
                     output = klass(message_payload)
@@ -340,18 +332,14 @@
         segment_length = unpack("<I", bytes(header[1:]) + b"\x00")[0]
         length += segment_length + 4
         data = data[4 + segment_length :]
     return length == data_length
 
 
 def extensions(obj) -> List[object]:
-    return [
-        obj.Extensions[field] for field, _ in obj.ListFields() if field.is_extension
-    ]
+    return [obj.Extensions[field] for field, _ in obj.ListFields() if field.is_extension]
 
 
 def find_extension(obj, name: str) -> object:
     all_extensions = extensions(obj)
-    filtered = [
-        getattr(x, name) for x in all_extensions if getattr(x, name, None) is not None
-    ]
+    filtered = [getattr(x, name) for x in all_extensions if getattr(x, name, None) is not None]
     return filtered[0]
```

### Comparing `numbers_parser-4.1.2/src/numbers_parser/mapping.py` & `numbers_parser-4.2.0/src/numbers_parser/mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from numbers_parser.generated import TNArchives_pb2 as TNArchives
 from numbers_parser.generated import TSTArchives_pb2 as TSTArchives
 from numbers_parser.generated import TSCH3DArchives_pb2 as TSCH3DArchives
 from numbers_parser.generated import TSSArchives_pb2 as TSSArchives
 from numbers_parser.generated import TSAArchives_sos_pb2 as TSAArchives_sos
 from numbers_parser.generated import TSCHArchives_GEN_pb2 as TSCHArchives_GEN
 from numbers_parser.generated import TSTStylePropertyArchiving_pb2 as TSTStylePropertyArchiving
@@ -28,15 +27,14 @@
 from numbers_parser.generated import TSCHArchives_pb2 as TSCHArchives
 from numbers_parser.generated import TSACommandArchives_sos_pb2 as TSACommandArchives_sos
 from numbers_parser.generated import TSTArchives_sos_pb2 as TSTArchives_sos
 from numbers_parser.generated import TSAArchives_pb2 as TSAArchives
 from numbers_parser.generated import TSCEArchives_pb2 as TSCEArchives
 from numbers_parser.generated import TSCHArchives_Common_pb2 as TSCHArchives_Common
 
-
 PROTO_FILES = [
     TNArchives,
     TSTArchives,
     TSCH3DArchives,
     TSSArchives,
     TSAArchives_sos,
     TSCHArchives_GEN,
@@ -62,15 +60,14 @@
     TSTCommandArchives,
     TSCHArchives,
     TSACommandArchives_sos,
     TSTArchives_sos,
     TSAArchives,
     TSCEArchives,
     TSCHArchives_Common,
-
 ]
 
 TSPRegistryMapping = {
     "1": "TN.DocumentArchive",
     "2": "TN.SheetArchive",
     "3": "TN.FormBasedSheetArchive",
     "7": "TN.PlaceholderArchive",
@@ -647,15 +644,14 @@
     "12053": "TN.FormBuilderSelectionArchive",
     "12054": "TN.FormTableChooserSelectionArchive",
     "12055": "TN.FormTableChooserSelectionTransformerArchive",
     "12056": "TN.FormBuilderSelectionTransformerArchive",
     "12057": "TN.FormViewerSelectionTransformerArchive",
     "12058": "TN.FormSheetSelectionTransformerArchive",
     "12059": "TN.FormCommandActivityBehaviorArchive",
-
 }
 
 
 def compute_maps():
     name_class_map = {}
 
     def add_nested_types(message_type):
@@ -669,15 +665,15 @@
             message_type = getattr(file, message_name)
             name_class_map[message_type.DESCRIPTOR.full_name] = message_type
             add_nested_types(message_type)
 
     id_name_map = {}
     name_id_map = {}
     for k, v in list(TSPRegistryMapping.items()):
-        if v in name_class_map:
+        if v in name_class_map:  # pragma: no branch
             id_name_map[int(k)] = name_class_map[v]
             if v not in name_id_map:
                 name_id_map[v] = int(k)
 
     return name_class_map, id_name_map, name_id_map
```

### Comparing `numbers_parser-4.1.2/src/numbers_parser/model.py` & `numbers_parser-4.2.0/src/numbers_parser/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     EPOCH,
     DEFAULT_COLUMN_WIDTH,
     DEFAULT_DOCUMENT,
     DEFAULT_PRE_BNC_BYTES,
     DEFAULT_ROW_HEIGHT,
     DEFAULT_TABLE_OFFSET,
     DEFAULT_TILE_SIZE,
+    DEFAULT_TEXT_INSET,
     DOCUMENT_ID,
     PACKAGE_ID,
     MAX_TILE_SIZE,
 )
 from numbers_parser.cell import (
     xl_rowcol_to_cell,
     xl_col_to_name,
@@ -32,14 +33,16 @@
     NumberCell,
     TextCell,
     Style,
     Alignment,
     HorizontalJustification,
     VerticalJustification,
     RGB,
+    Border,
+    BorderType,
 )
 from numbers_parser.exceptions import UnsupportedError, UnsupportedWarning
 from numbers_parser.formula import TableFormulas
 from numbers_parser.bullets import (
     BULLET_PREFIXES,
     BULLET_CONVERTION,
     BULLET_SUFFIXES,
@@ -55,14 +58,17 @@
 from numbers_parser.generated import TSTArchives_pb2 as TSTArchives
 from numbers_parser.generated import TSCEArchives_pb2 as TSCEArchives
 from numbers_parser.generated import TSWPArchives_pb2 as TSWPArchives
 from numbers_parser.generated import TSSArchives_pb2 as TSSArchives
 from numbers_parser.generated.TSWPArchives_pb2 import (
     CharacterStylePropertiesArchive as CharacterStyle,
 )
+from numbers_parser.generated.TSDArchives_pb2 import (
+    StrokePatternArchive as StrokePattern,
+)
 
 
 def create_font_name_map(font_map: dict) -> dict:
     new_font_map = {}
     for k, v in font_map.items():
         if v not in new_font_map:
             new_font_map[v] = k
@@ -123,17 +129,15 @@
         clear_field_container(self._datalists[table_id]["datalist"].entries)
 
     def lookup_key(self, table_id: int, value) -> int:
         """Return the key associated with a value for a particular table entry.
         If the value is not in the datalist, allocate a new entry with the
         next available key"""
         self.add_table(table_id)
-        value_key = (
-            value.identifier if isinstance(value, TSPMessages.Reference) else value
-        )
+        value_key = value.identifier if isinstance(value, TSPMessages.Reference) else value
         if value_key not in self._datalists[table_id]["by_value"]:
             key = self._datalists[table_id]["next_key"]
             self._datalists[table_id]["next_key"] += 1
             self._datalists[table_id]["datalist"].nextListID += 1
             attrs = {"key": key, self._value_attr: value, "refcount": 1}
             entry = TSTArchives.TableDataList.ListEntry(**attrs)
             self._datalists[table_id]["datalist"].entries.append(entry)
@@ -163,15 +167,17 @@
         self.objects = ObjectStore(filename)
         self._merge_cells = {}
         self._row_heights = {}
         self._col_widths = {}
         self._table_formats = DataLists(self, "format_table")
         self._table_styles = DataLists(self, "styleTable", "reference")
         self._table_strings = DataLists(self, "stringTable", "string")
+        self._table_data = {}
         self._styles = None
+        self._max_stroke_order = 0
 
     @property
     def file_store(self):
         return self.objects.file_store
 
     def find_refs(self, ref: str) -> list:
         return self.objects.find_refs(ref)
@@ -181,14 +187,17 @@
 
     def sheet_name(self, sheet_id, value=None):
         if value is None:
             return self.objects[sheet_id].name
         else:
             self.objects[sheet_id].name = value
 
+    def set_table_data(self, table_id: int, data: List):
+        self._table_data[table_id] = data
+
     # Don't cache: new tables can be added at runtime
     def table_ids(self, sheet_id: int) -> list:
         """Return a list of table IDs for a given sheet ID"""
         table_info_ids = self.find_refs("TableInfoArchive")
         return [
             self.objects[t_id].tableModel.identifier
             for t_id in table_info_ids
@@ -246,17 +255,15 @@
         #
         #  {
         #      "hiding_state": 0,
         #      "index": 0,
         #      "number_of_cells": 3,
         #      "size": 0.0
         #  },
-        col_bucket_map = {
-            i: None for i in range(self.objects[table_id].number_of_columns)
-        }
+        col_bucket_map = {i: None for i in range(self.objects[table_id].number_of_columns)}
         bds = self.objects[table_id].base_data_store
         buckets = self.objects[bds.columnHeaders.identifier].headers
         for i, bucket in enumerate(buckets):
             col_bucket_map[bucket.index] = i
         return col_bucket_map
 
     def table_name(self, table_id, value=None):
@@ -268,17 +275,15 @@
     @lru_cache(maxsize=None)
     def table_tiles(self, table_id):
         bds = self.objects[table_id].base_data_store
         return [self.objects[t.tile.identifier] for t in bds.tiles.tiles]
 
     @lru_cache(maxsize=None)
     def custom_format_map(self):
-        custom_format_list_id = self.objects[
-            DOCUMENT_ID
-        ].super.custom_format_list.identifier
+        custom_format_list_id = self.objects[DOCUMENT_ID].super.custom_format_list.identifier
         custom_format_list = self.objects[custom_format_list_id]
         custom_format_map = {
             NumbersUUID(u).hex: custom_format_list.custom_formats[i]
             for i, u in enumerate(custom_format_list.uuids)
         }
         return custom_format_map
 
@@ -468,17 +473,15 @@
         for sheet_id in self.sheet_ids():  # pragma: no branch
             for table_id in self.table_ids(sheet_id):
                 if table_uuid == self.table_base_id(table_id):
                     return table_id
 
     def node_to_ref(self, this_table_id: int, row_num: int, col_num: int, node):
         if node.HasField("AST_cross_table_reference_extra_info"):
-            table_uuid = NumbersUUID(
-                node.AST_cross_table_reference_extra_info.table_id
-            ).hex
+            table_uuid = NumbersUUID(node.AST_cross_table_reference_extra_info.table_id).hex
             other_table_id = self.table_uuids_to_id(table_uuid)
             other_table_name = self.table_name(other_table_id)
         else:
             other_table_id = None
             other_table_name = None
 
         if other_table_id is not None:
@@ -617,27 +620,23 @@
 
         merge_map_id, merge_map = self.objects.create_object_from_dict(
             "CalculationEngine", {}, TSTArchives.MergeRegionMapArchive
         )
 
         for merge_cell, merge_data in merge_cells.items():
             if merge_data["merge_type"] == "source":
-                cell_id = TSTArchives.CellID(
-                    packedData=(merge_cell[1] << 16 | merge_cell[0])
-                )
+                cell_id = TSTArchives.CellID(packedData=(merge_cell[1] << 16 | merge_cell[0]))
                 table_size = TSTArchives.TableSize(
                     packedData=(merge_data["size"][1] << 16 | merge_data["size"][0])
                 )
                 cell_range = TSTArchives.CellRange(origin=cell_id, size=table_size)
                 merge_map.cell_range.append(cell_range)
 
         base_data_store = self.objects[table_id].base_data_store
-        base_data_store.merge_region_map.CopyFrom(
-            TSPMessages.Reference(identifier=merge_map_id)
-        )
+        base_data_store.merge_region_map.CopyFrom(TSPMessages.Reference(identifier=merge_map_id))
 
     def recalculate_row_info(
         self, table_id: int, data: List, tile_row_offset: int, row_num: int
     ) -> TSTArchives.TileRowInfo:
         row_info = TSTArchives.TileRowInfo()
         row_info.storage_version = 5
         row_info.tile_row_index = row_num - tile_row_offset
@@ -666,22 +665,18 @@
 
     @lru_cache(maxsize=None)
     def metadata_component(self, reference: Union[str, int] = None) -> int:
         """Return the ID of an object in the document metadata given it's name or ID"""
         component_map = {c.identifier: c for c in self.objects[PACKAGE_ID].components}
         if isinstance(reference, str):
             component_ids = [
-                id
-                for id, c in component_map.items()
-                if c.preferred_locator == reference
+                id for id, c in component_map.items() if c.preferred_locator == reference
             ]
         else:
-            component_ids = [
-                id for id, c in component_map.items() if c.identifier == reference
-            ]
+            component_ids = [id for id, c in component_map.items() if c.identifier == reference]
         return component_map[component_ids[0]]
 
     def add_component_metadata(self, object_id: int, parent: str, locator: str):
         """Add a new ComponentInfo record to the parent object in the document metadata"""
         locator = locator.format(object_id)
         preferred_locator = re.sub(r"\-\d+.*", "", locator)
         component_info = TSPArchiveMessages.ComponentInfo(
@@ -776,17 +771,15 @@
 
     def create_string_table(self):
         table_strings_id, table_strings = self.objects.create_object_from_dict(
             "Index/Tables/DataList-{}",
             {"listType": TSTArchives.TableDataList.ListType.STRING, "nextListID": 1},
             TSTArchives.TableDataList,
         )
-        self.add_component_metadata(
-            table_strings_id, "CalculationEngine", "Tables/DataList-{}"
-        )
+        self.add_component_metadata(table_strings_id, "CalculationEngine", "Tables/DataList-{}")
         return table_strings_id, table_strings
 
     def table_height(self, table_id: int) -> int:
         """Return the height of a table in points"""
         table_model = self.objects[table_id]
         bds = self.objects[table_id].base_data_store
         buckets = self.objects[bds.rowHeaders.buckets[0].identifier].headers
@@ -963,17 +956,15 @@
         )
 
         style_table_id, _ = self.objects.create_object_from_dict(
             "Index/Tables/DataList-{}",
             {"listType": TSTArchives.TableDataList.ListType.STYLE, "nextListID": 1},
             TSTArchives.TableDataList,
         )
-        self.add_component_metadata(
-            style_table_id, "CalculationEngine", "Tables/DataList-{}"
-        )
+        self.add_component_metadata(style_table_id, "CalculationEngine", "Tables/DataList-{}")
 
         formula_table_id, _ = self.objects.create_object_from_dict(
             "Index/Tables/TableDataList-{}",
             {"listType": TSTArchives.TableDataList.ListType.FORMULA, "nextListID": 1},
             TSTArchives.TableDataList,
         )
         self.add_component_metadata(
@@ -992,17 +983,15 @@
         )
 
         data_store_refs = field_references(from_table.base_data_store)
         data_store_refs["stringTable"] = {"identifier": table_strings_id}
         data_store_refs["columnHeaders"] = {"identifier": column_headers_id}
         data_store_refs["styleTable"] = {"identifier": style_table_id}
         data_store_refs["formula_table"] = {"identifier": formula_table_id}
-        data_store_refs["format_table_pre_bnc"] = {
-            "identifier": format_table_pre_bnc_id
-        }
+        data_store_refs["format_table_pre_bnc"] = {"identifier": format_table_pre_bnc_id}
         table_model.base_data_store.MergeFrom(
             TSTArchives.DataStore(
                 rowHeaders=TSTArchives.HeaderStorage(bucketHashFunction=1),
                 nextRowStripID=1,
                 nextColumnStripID=0,
                 rowTileTree=TSTArchives.TableRBTree(),
                 columnTileTree=TSTArchives.TableRBTree(),
@@ -1034,17 +1023,15 @@
         self.recalculate_table_data(table_model_id, data)
 
         table_info_id, table_info = self.objects.create_object_from_dict(
             "CalculationEngine",
             {},
             TSTArchives.TableInfoArchive,
         )
-        table_info.tableModel.MergeFrom(
-            TSPMessages.Reference(identifier=table_model_id)
-        )
+        table_info.tableModel.MergeFrom(TSPMessages.Reference(identifier=table_model_id))
         table_info.super.MergeFrom(self.create_drawable(sheet_id, x, y))
         self.add_component_reference(table_info_id, "Document", self.calc_engine_id())
 
         self.add_formula_owner(
             table_info_id,
             num_rows,
             num_cols,
@@ -1135,44 +1122,37 @@
 
     def add_sheet(self, sheet_name: str) -> int:
         """Add a new sheet with a copy of a table from another sheet"""
         sheet_id, _ = self.objects.create_object_from_dict(
             "Document", {"name": sheet_name}, TNArchives.SheetArchive
         )
 
-        self.add_component_reference(
-            sheet_id, "CalculationEngine", DOCUMENT_ID, is_weak=True
-        )
+        self.add_component_reference(sheet_id, "CalculationEngine", DOCUMENT_ID, is_weak=True)
 
-        self.objects[DOCUMENT_ID].sheets.append(
-            TSPMessages.Reference(identifier=sheet_id)
-        )
+        self.objects[DOCUMENT_ID].sheets.append(TSPMessages.Reference(identifier=sheet_id))
 
         return sheet_id
 
     @property
     def styles(self):
         if self._styles is None:
             self._styles = self.available_paragraph_styles()
         return self._styles
 
     @lru_cache(maxsize=None)
     def available_paragraph_styles(self) -> List[Style]:
         theme_id = self.objects[DOCUMENT_ID].theme.identifier
-        presets = find_extension(
-            self.objects[theme_id].super, "paragraph_style_presets"
-        )
+        presets = find_extension(self.objects[theme_id].super, "paragraph_style_presets")
         presets_map = {
             self.objects[x.identifier].super.name: {
                 "id": x.identifier,
                 "obj": self.objects[x.identifier],
             }
             for x in presets
         }
-        # HorizontalJustification(cell_style.para_properties.alignment)
         return {
             k: Style(
                 alignment=Alignment(
                     HorizontalJustification(v["obj"].para_properties.alignment),
                     VerticalJustification(0),
                 ),
                 font_color=self.cell_font_color(v["obj"]),
@@ -1231,36 +1211,33 @@
                             "a": 1.0,
                             "rgbspace": "srgb",
                         },
                     },
                 },
                 "para_properties": {
                     "alignment": style.alignment.horizontal,
+                    "first_line_indent": style.first_indent,
+                    "left_indent": style.left_indent,
+                    "right_indent": style.right_indent,
                 },
             },
             TSWPArchives.ParagraphStyleArchive,
         )
         stylesheet_id = self.objects[DOCUMENT_ID].stylesheet.identifier
-        para_style.super.stylesheet.MergeFrom(
-            TSPMessages.Reference(identifier=stylesheet_id)
-        )
-        self.objects[stylesheet_id].styles.append(
-            TSPMessages.Reference(identifier=para_style_id)
-        )
+        para_style.super.stylesheet.MergeFrom(TSPMessages.Reference(identifier=stylesheet_id))
+        self.objects[stylesheet_id].styles.append(TSPMessages.Reference(identifier=para_style_id))
         self.objects[stylesheet_id].identifier_to_style_map.append(
             TSSArchives.StylesheetArchive.IdentifiedStyleEntry(
                 identifier=style_id_name,
                 style=TSPMessages.Reference(identifier=para_style_id),
             )
         )
 
         theme_id = self.objects[DOCUMENT_ID].theme.identifier
-        presets = find_extension(
-            self.objects[theme_id].super, "paragraph_style_presets"
-        )
+        presets = find_extension(self.objects[theme_id].super, "paragraph_style_presets")
         presets.append(TSPMessages.Reference(identifier=para_style_id))
         self._styles[style.name] = style
         return para_style_id
 
     def update_paragraph_style(self, style: Style):
         if style.underline:
             underline = CharacterStyle.UnderlineType.kSingleUnderline
@@ -1280,14 +1257,17 @@
         style_obj.char_properties.strikethru = strikethru
         style_obj.char_properties.font_size = style.font_size
         style_obj.char_properties.font_name = FONT_FAMILY_TO_NAME[style.font_name]
         style_obj.char_properties.tsd_fill.color.r = style.font_color.r / 255
         style_obj.char_properties.tsd_fill.color.g = style.font_color.g / 255
         style_obj.char_properties.tsd_fill.color.b = style.font_color.b / 255
         style_obj.para_properties.alignment = style.alignment.horizontal
+        style_obj.para_properties.first_line_indent = style.first_indent
+        style_obj.para_properties.left_indent = style.left_indent
+        style_obj.para_properties.right_indent = style.right_indent
 
     def update_paragraph_styles(self):
         """Create new paragraph style archives for any new styles that
         have been created for this document"""
         new_styles = [x for x in self.styles.values() if x._text_style_obj_id is None]
         updated_styles = [
             x
@@ -1304,22 +1284,26 @@
     def update_cell_styles(self, table_id: int, data: List):
         """Create new cell style archives for any cells whose styles
         have changes that require a cell style"""
         cell_styles = {}
         for row_num, row in enumerate(data):
             for col_num, cell in enumerate(row):
                 if cell._style is not None and cell._style._update_cell_style:
-                    if cell._style.bg_color is None:
-                        fingerprint = str(cell.style.alignment.vertical)
-                    else:
-                        fingerprint = "{0}-{1}-{2}-{3}".format(
-                            cell.style.alignment.vertical,
-                            cell.style.bg_color.r,
-                            cell.style.bg_color.g,
-                            cell.style.bg_color.b,
+                    fingerprint = (
+                        str(cell.style.alignment.vertical)
+                        + str(cell.style.first_indent)
+                        + str(cell.style.left_indent)
+                        + str(cell.style.right_indent)
+                        + str(cell.style.text_inset)
+                    )
+                    if cell._style.bg_color is not None:
+                        fingerprint = fingerprint + (
+                            str(cell.style.bg_color.r)
+                            + str(cell.style.bg_color.g)
+                            + str(cell.style.bg_color.b)
                         )
                     if fingerprint not in cell_styles:
                         cell_styles[fingerprint] = self.add_cell_style(cell._style)
                     cell._style._cell_style_obj_id = cell_styles[fingerprint]
 
     def add_cell_style(self, style: Style) -> int:
         if style.bg_color is not None:
@@ -1343,61 +1327,57 @@
                 "super": {
                     "name": style.name,
                     "style_identifier": "",
                 },
                 "override_count": 1,
                 "cell_properties": {
                     **color_attrs,
+                    "padding": {
+                        "left": style.text_inset,
+                        "top": style.text_inset,
+                        "right": style.text_inset,
+                        "bottom": style.text_inset,
+                    },
                     "vertical_alignment": style.alignment.vertical,
                 },
             },
             TSTArchives.CellStyleArchive,
         )
         style_id_name = f"numbers-parser-custom-{cell_style_id}"
         cell_style.super.style_identifier = style_id_name
 
         stylesheet_id = self.objects[DOCUMENT_ID].stylesheet.identifier
-        cell_style.super.stylesheet.MergeFrom(
-            TSPMessages.Reference(identifier=stylesheet_id)
-        )
-        self.objects[stylesheet_id].styles.append(
-            TSPMessages.Reference(identifier=cell_style_id)
-        )
+        cell_style.super.stylesheet.MergeFrom(TSPMessages.Reference(identifier=stylesheet_id))
+        self.objects[stylesheet_id].styles.append(TSPMessages.Reference(identifier=cell_style_id))
         self.objects[stylesheet_id].identifier_to_style_map.append(
             TSSArchives.StylesheetArchive.IdentifiedStyleEntry(
                 identifier=style_id_name,
                 style=TSPMessages.Reference(identifier=cell_style_id),
             )
         )
         return cell_style_id
 
     def text_style_object_id(self, cell_storage) -> int:
         if cell_storage.text_style_id is None:
             return None
-        entry = self._table_styles.lookup_value(
-            cell_storage.table_id, cell_storage.text_style_id
-        )
+        entry = self._table_styles.lookup_value(cell_storage.table_id, cell_storage.text_style_id)
         return entry.reference.identifier
 
     def cell_style_object_id(self, cell_storage) -> int:
         if cell_storage.cell_style_id is None:
             return None
-        entry = self._table_styles.lookup_value(
-            cell_storage.table_id, cell_storage.cell_style_id
-        )
+        entry = self._table_styles.lookup_value(cell_storage.table_id, cell_storage.cell_style_id)
         return entry.reference.identifier
 
     def custom_style_name(self) -> Tuple[str, str]:
         """Find custom styles in the current document and return the next
         highest numbered style"""
         stylesheet_id = self.objects[DOCUMENT_ID].stylesheet.identifier
         current_styles = self.styles.keys()
-        custom_styles = [
-            x for x in current_styles if re.fullmatch(r"Custom Style \d+", x)
-        ]
+        custom_styles = [x for x in current_styles if re.fullmatch(r"Custom Style \d+", x)]
         for style_entry in self.objects[stylesheet_id].identifier_to_style_map:
             style_id = style_entry.style.identifier
             style_name = getattr(self.objects[style_id].super, "name", "")
             if re.fullmatch(r"Custom Style \d+", style_name):
                 custom_styles.append(style_name)
 
         if len(custom_styles) > 0:
@@ -1519,17 +1499,15 @@
         return storage[0:length]
 
     @lru_cache(maxsize=None)
     def table_formulas(self, table_id: int):
         return TableFormulas(self, table_id)
 
     @lru_cache(maxsize=None)
-    def table_cell_decode(  # noqa: C901
-        self, table_id: int, row_num: int, col_num: int
-    ) -> Dict:
+    def table_cell_decode(self, table_id: int, row_num: int, col_num: int) -> Dict:  # noqa: C901
         buffer = self.storage_buffer(table_id, row_num, col_num)
         if buffer is None:
             return None
 
         cell = CellStorage(self, table_id, buffer, row_num, col_num)
         return cell
 
@@ -1638,50 +1616,36 @@
 
         table_model = self.objects[cell_storage.table_id]
         if cell_storage.row_num in range(0, table_model.number_of_header_rows):
             return self.objects[table_model.header_row_text_style.identifier]
         elif cell_storage.col_num in range(0, table_model.number_of_header_columns):
             return self.objects[table_model.header_column_text_style.identifier]
         elif table_model.number_of_footer_rows > 0:
-            start_row_num = (
-                table_model.number_of_rows - table_model.number_of_footer_rows
-            )
-            if cell_storage.row_num in range(
-                start_row_num, table_model.number_of_header_rows
-            ):
+            start_row_num = table_model.number_of_rows - table_model.number_of_footer_rows
+            if cell_storage.row_num in range(start_row_num, table_model.number_of_header_rows):
                 return self.objects[table_model.footer_row_text_style.identifier]
         return self.objects[table_model.body_text_style.identifier]
 
     def cell_alignment(self, cell_storage: object) -> Alignment:
-        cell_style = self.cell_text_style(cell_storage)
-        if cell_style.para_properties.HasField("alignment"):
-            horizontal = HorizontalJustification(cell_style.para_properties.alignment)
-        else:
-            parent_obj_id = cell_style.super.parent.identifier
-            horizontal = HorizontalJustification(
-                self.objects[parent_obj_id].para_properties.alignment
-            )
+        style = self.cell_text_style(cell_storage)
+        horizontal = HorizontalJustification(self.para_property(style, "alignment"))
 
         if cell_storage.cell_style_id is None:
             vertical = VerticalJustification.TOP
         else:
-            cell_style = self.table_style(
-                cell_storage.table_id, cell_storage.cell_style_id
-            )
-            vertical = VerticalJustification(
-                cell_style.cell_properties.vertical_alignment
-            )
+            style = self.table_style(cell_storage.table_id, cell_storage.cell_style_id)
+            vertical = VerticalJustification(self.cell_property(style, "vertical_alignment"))
         return Alignment(horizontal, vertical)
 
     def cell_bg_color(self, cell_storage: object) -> Union[Tuple, List[Tuple]]:
         if cell_storage.cell_style_id is None:
             return None
 
-        cell_style = self.table_style(cell_storage.table_id, cell_storage.cell_style_id)
-        cell_properties = cell_style.cell_properties.cell_fill
+        style = self.table_style(cell_storage.table_id, cell_storage.cell_style_id)
+        cell_properties = style.cell_properties.cell_fill
 
         if cell_properties.HasField("color"):
             return rgb(cell_properties.color)
         elif cell_properties.HasField("gradient"):
             return [(rgb(s.color)) for s in cell_properties.gradient.stops]
 
     def char_property(self, style: object, field: str):
@@ -1689,14 +1653,36 @@
         in the style, or from the parent if not"""
         if not style.char_properties.HasField(field):
             parent = self.objects[style.super.parent.identifier]
             return getattr(parent.char_properties, field)
         else:
             return getattr(style.char_properties, field)
 
+    def para_property(self, style: object, field: str) -> float:
+        """Return a para_property field from a style if present
+        in the style, or from the parent if not"""
+        if not style.para_properties.HasField(field):
+            if not style.super.parent.identifier:
+                return 0.0
+            parent = self.objects[style.super.parent.identifier]
+            return getattr(parent.para_properties, field)
+        else:
+            return getattr(style.para_properties, field)
+
+    def cell_property(self, style: object, field: str) -> float:
+        """Return a cell_property field from a style if present
+        in the style, or from the parent if not"""
+        if not style.cell_properties.HasField(field):
+            if not style.super.parent.identifier:
+                return 0.0
+            parent = self.objects[style.super.parent.identifier]
+            return getattr(parent.cell_properties, field)
+        else:
+            return getattr(style.cell_properties, field)
+
     def cell_is_bold(self, obj: object) -> bool:
         style = self.cell_text_style(obj) if isinstance(obj, CellStorage) else obj
         return self.char_property(style, "bold")
 
     def cell_is_italic(self, obj: object) -> bool:
         style = self.cell_text_style(obj) if isinstance(obj, CellStorage) else obj
         return self.char_property(style, "italic")
@@ -1724,14 +1710,251 @@
         return self.char_property(style, "font_size")
 
     def cell_font_name(self, obj: object) -> str:
         style = self.cell_text_style(obj) if isinstance(obj, CellStorage) else obj
         font_name = self.char_property(style, "font_name")
         return FONT_NAME_TO_FAMILY[font_name]
 
+    def cell_first_indent(self, obj: object) -> float:
+        style = self.cell_text_style(obj) if isinstance(obj, CellStorage) else obj
+        return self.para_property(style, "first_line_indent")
+
+    def cell_left_indent(self, obj: object) -> float:
+        style = self.cell_text_style(obj) if isinstance(obj, CellStorage) else obj
+        return self.para_property(style, "left_indent")
+
+    def cell_right_indent(self, obj: object) -> float:
+        style = self.cell_text_style(obj) if isinstance(obj, CellStorage) else obj
+        return self.para_property(style, "right_indent")
+
+    def cell_text_inset(self, cell_storage: CellStorage) -> float:
+        if cell_storage.cell_style_id is None:
+            return DEFAULT_TEXT_INSET
+        else:
+            style = self.table_style(cell_storage.table_id, cell_storage.cell_style_id)
+            padding = self.cell_property(style, "padding")
+            # Padding is always identical (only one UI setting)
+            text_inset = padding.left
+            return text_inset
+
+    def stroke_type(self, stroke_run: object) -> str:
+        """Return the stroke type for a stroke run"""
+        stroke_type = stroke_run.stroke.pattern.type
+        if stroke_type == StrokePattern.StrokePatternType.TSDSolidPattern:
+            return "solid"
+        elif stroke_type == StrokePattern.StrokePatternType.TSDPattern:
+            if stroke_run.stroke.pattern.pattern[0] < 1.0:
+                return "dots"
+            else:
+                return "dashes"
+        else:
+            return "none"
+
+    def cell_for_stroke(self, table_id: int, side: str, row_num: int, col_num: int) -> object:
+        data = self._table_data[table_id]
+        if row_num < 0 or col_num < 0:
+            return None
+        if row_num >= len(data) or col_num >= len(data[row_num]):
+            return None
+        cell = self._table_data[table_id][row_num][col_num]
+        if isinstance(cell, MergedCell):
+            if side == "top":
+                if row_num == cell.row_start:
+                    return cell
+                else:
+                    return None
+            elif side == "right":
+                if col_num == cell.col_end:
+                    return cell
+                else:
+                    return None
+            elif side == "bottom":
+                if row_num == cell.row_end:
+                    return cell
+                else:
+                    return None
+            else:  # left
+                if col_num == cell.col_start:
+                    return cell
+                else:
+                    return None
+        return cell
+
+    def set_cell_border(
+        self, table_id: int, row_num: int, col_num: int, side: str, border_value: Border
+    ):
+        """Set the 2 borders adjacent to a stroke if within the table range"""
+        if side == "top":
+            if (cell := self.cell_for_stroke(table_id, "top", row_num, col_num)) is not None:
+                cell._border.top = border_value
+            if (cell := self.cell_for_stroke(table_id, "bottom", row_num - 1, col_num)) is not None:
+                cell._border.bottom = border_value
+        elif side == "right":
+            if (cell := self.cell_for_stroke(table_id, "right", row_num, col_num)) is not None:
+                cell._border.right = border_value
+            if (cell := self.cell_for_stroke(table_id, "left", row_num, col_num + 1)) is not None:
+                cell._border.left = border_value
+        elif side == "bottom":
+            if (cell := self.cell_for_stroke(table_id, "bottom", row_num, col_num)) is not None:
+                cell._border.bottom = border_value
+            if (cell := self.cell_for_stroke(table_id, "top", row_num + 1, col_num)) is not None:
+                cell._border.top = border_value
+        else:  # left border
+            if (cell := self.cell_for_stroke(table_id, "left", row_num, col_num)) is not None:
+                cell._border.left = border_value
+            if (cell := self.cell_for_stroke(table_id, "right", row_num, col_num - 1)) is not None:
+                cell._border.right = border_value
+
+    def extract_strokes_in_layers(self, table_id: int, layer_ids: List, side: str):
+        for layer_id in layer_ids:
+            stroke_layer = self.objects[layer_id.identifier]
+            for stroke_run in stroke_layer.stroke_runs:
+                if stroke_run.order > self._max_stroke_order:
+                    self._max_stroke_order = stroke_run.order
+                border_value = Border(
+                    width=round(stroke_run.stroke.width, 2),
+                    color=rgb(stroke_run.stroke.color),
+                    style=self.stroke_type(stroke_run),
+                    _order=stroke_run.order,
+                )
+                if side in ["top", "bottom"]:
+                    start_row = stroke_layer.row_column_index
+                    start_column = stroke_run.origin
+                    for col_num in range(start_column, start_column + stroke_run.length):
+                        self.set_cell_border(table_id, start_row, col_num, side, border_value)
+                else:
+                    start_row = stroke_run.origin
+                    start_column = stroke_layer.row_column_index
+                    for row_num in range(start_row, start_row + stroke_run.length):
+                        self.set_cell_border(table_id, row_num, start_column, side, border_value)
+
+    @lru_cache(maxsize=None)
+    def extract_strokes(self, table_id: int):
+        table_obj = self.objects[table_id]
+        sidecar_obj = self.objects[table_obj.stroke_sidecar.identifier]
+        self.extract_strokes_in_layers(table_id, sidecar_obj.top_row_stroke_layers, "top")
+        self.extract_strokes_in_layers(table_id, sidecar_obj.left_column_stroke_layers, "left")
+        self.extract_strokes_in_layers(table_id, sidecar_obj.right_column_stroke_layers, "right")
+        self.extract_strokes_in_layers(table_id, sidecar_obj.bottom_row_stroke_layers, "bottom")
+
+    def create_stroke(self, origin: int, length: int, border_value: Border):
+        self._max_stroke_order += 1
+        line_cap = TSDArchives.StrokeArchive.LineCap.ButtCap
+        line_join = TSDArchives.LineJoin.MiterJoin
+        if border_value.style == BorderType.SOLID:
+            pattern = TSDArchives.StrokePatternArchive(
+                type=StrokePattern.StrokePatternType.TSDSolidPattern,
+                phase=0.0,
+                count=0,
+                pattern=[0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
+            )
+        elif border_value.style == BorderType.DASHES:
+            pattern = TSDArchives.StrokePatternArchive(
+                type=StrokePattern.StrokePatternType.TSDPattern,
+                phase=0.0,
+                count=2,
+                pattern=[2.0, 2.0, 0.0, 0.0, 0.0, 0.0],
+            )
+        elif border_value.style == BorderType.DOTS:
+            pattern = TSDArchives.StrokePatternArchive(
+                type=StrokePattern.StrokePatternType.TSDPattern,
+                phase=0.0,
+                count=2,
+                pattern=[0.0001, 2.0, 0.0, 0.0, 0.0, 0.0],
+            )
+            line_cap = TSDArchives.StrokeArchive.LineCap.RoundCap
+            line_join = TSDArchives.LineJoin.RoundJoin
+        else:
+            pattern = TSDArchives.StrokePatternArchive(
+                type=StrokePattern.StrokePatternType.TSDEmptyPattern,
+                phase=0.0,
+                count=0,
+                pattern=[0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
+            )
+
+        if border_value is None:
+            color = TSPMessages.Color(
+                model=TSPMessages.Color.rgb,
+                rgbspace=TSPMessages.Color.srgb,
+                r=0.0,
+                g=0.0,
+                b=0.0,
+                a=1.0,
+            )
+            width = 0.0
+        else:
+            color = TSPMessages.Color(
+                model=TSPMessages.Color.rgb,
+                rgbspace=TSPMessages.Color.srgb,
+                r=border_value.color.r / 255,
+                g=border_value.color.g / 255,
+                b=border_value.color.b / 255,
+                a=1.0,
+            )
+            width = border_value.width
+        return TSTArchives.StrokeLayerArchive.StrokeRunArchive(
+            origin=origin,
+            length=length,
+            order=self._max_stroke_order,
+            stroke=TSDArchives.StrokeArchive(
+                color=color,
+                width=width,
+                cap=line_cap,
+                join=line_join,
+                miter_limit=4.0,
+                pattern=pattern,
+            ),
+        )
+
+    def add_stroke(
+        self,
+        table_id: int,
+        row_num: int,
+        col_num: int,
+        side: str,
+        border_value: Border,
+        length: int,
+    ):
+        table_obj = self.objects[table_id]
+        sidecar_obj = self.objects[table_obj.stroke_sidecar.identifier]
+
+        if side == "top":
+            layer_ids = sidecar_obj.top_row_stroke_layers
+            row_column_index = row_num
+            origin = col_num
+        elif side == "right":
+            layer_ids = sidecar_obj.right_column_stroke_layers
+            row_column_index = col_num
+            origin = row_num
+        elif side == "bottom":
+            layer_ids = sidecar_obj.bottom_row_stroke_layers
+            row_column_index = row_num
+            origin = col_num
+        else:  # left border
+            layer_ids = sidecar_obj.left_column_stroke_layers
+            row_column_index = col_num
+            origin = row_num
+
+        stroke_layer = None
+        for layer_id in layer_ids:
+            if self.objects[layer_id.identifier].row_column_index == row_column_index:
+                stroke_layer = self.objects[layer_id.identifier]
+        if stroke_layer is not None:
+            stroke_layer.append(self.create_stroke(origin, length, border_value))
+        else:
+            stroke_layer_id, stroke_layer = self.objects.create_object_from_dict(
+                "CalculationEngine",
+                {
+                    "row_column_index": row_column_index,
+                },
+                TSTArchives.StrokeLayerArchive,
+            )
+            stroke_layer.stroke_runs.append(self.create_stroke(origin, length, border_value))
+            layer_ids.append(TSPMessages.Reference(identifier=stroke_layer_id))
+
 
 def rgb(obj) -> RGB:
     """Convert a TSPArchives.Color into an RGB tuple"""
     return RGB(round(obj.r * 255), round(obj.g * 255), round(obj.b * 255))
 
 
 def range_end(obj):
@@ -1760,17 +1983,15 @@
     col_name = xl_col_to_name(col, node.AST_column.absolute)
     if table_name is not None:
         return f"{table_name}::{col_name}"
     else:
         return col_name
 
 
-def node_to_row_col_ref(
-    node: object, table_name: str, row_num: int, col_num: int
-) -> str:
+def node_to_row_col_ref(node: object, table_name: str, row_num: int, col_num: int) -> str:
     if node.AST_row.absolute:
         row = node.AST_row.row
     else:
         row = row_num + node.AST_row.row
     if node.AST_column.absolute:
         col = node.AST_column.column
     else:
```

### Comparing `numbers_parser-4.1.2/src/numbers_parser/numbers_uuid.py` & `numbers_parser-4.2.0/src/numbers_parser/numbers_uuid.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,15 @@
         elif type(uuid) == str:
             super().__init__(hex=uuid)
         elif type(uuid) == TSPMessages.UUID:
             uuid_int = uuid.upper << 64 | uuid.lower
             super().__init__(int=uuid_int)
         elif type(uuid) == TSPMessages.CFUUIDArchive:
             uuid_int = (
-                (uuid.uuid_w3 << 96)
-                | (uuid.uuid_w2 << 64)
-                | (uuid.uuid_w1 << 32)
-                | uuid.uuid_w0
+                (uuid.uuid_w3 << 96) | (uuid.uuid_w2 << 64) | (uuid.uuid_w1 << 32) | uuid.uuid_w0
             )
             super().__init__(int=uuid_int)
         elif type(uuid) == dict:
             if "uuid_w0" in uuid and "uuid_w1" in uuid:
                 uuid_int = (
                     (int(uuid["uuid_w3"]) << 96)
                     | (int(uuid["uuid_w2"]) << 64)
```

### Comparing `numbers_parser-4.1.2/PKG-INFO` & `numbers_parser-4.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numbers-parser
-Version: 4.1.2
+Version: 4.2.0
 Summary: Read and write Apple Numbers spreadsheets
 Home-page: https://github.com/masaccio/numbers-parser
 License: MIT
 Author: Jon Connell
 Author-email: python@figsandfudge.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -208,33 +208,41 @@
 `numbers_parser` currently only supports paragraph styles and cell styles. The following paragraph styles are suppoprted:
 
 * font attributes: bold, italic, underline, strikethrough
 * font selection and size
 * text foreground color
 * horizontal and vertical alignment
 * cell background color
+* cell indents (first line, left, right, and text inset)
 
 Table styles that allow new tables to adopt a style across the whole table are not planned.
 
+Numbers conflates style attributes that can be stored in paragraph styles (the style menu in the text panel) with the settings that are available on the Style tab of the Text panel. Some attributes in Numbers are not applied to new cells when a style is applied. To keep the API simple, `numbers-parser` packs all styling into a single `Style` object. When a document is saved, the attributes not stored in a paragraph style are applied to each cell that includes it. Attributes behaving in this way are currently `Cell.alignment.vertical` and `Cell.style.text_inset`. The cell background colour `Cell.style.bg_color` also behaves this way, though this is in line with the separation in Numbers.
+
 #### Reading styles
 
 The cell method `style` returns a `Style` object containing all the style information for that cell. Cells with identical style settings contain references to a single style object.
 
-Cell text fonts can be returned using a number of methods.
+Cell style attributes can be returned using a number of methods:
 
 * `Cell.style.alignment`: the horizontal and vertical alignment of the cell as an `Alignment` names tuple
 * `Cell.style.bg_color`: cell background color as an `RGB` named tuple, or a list of `RGB` values for gradients
 * `Cell.style.bold`: `True` if the cell font is bold
 * `Cell.style.font_color`: font color as an `RGB` named tuple
 * `Cell.style.font_size`: font size in points (`float`)
 * `Cell.style.font_name`: font name (`str`)
 * `Cell.style.italic`: `True` if the cell font is italic
 * `Cell.style.name`: cell style (`str`)
 * `Cell.style.underline`: `True` if the cell font is underline
 * `Cell.style.strikethrough`: `True` if the cell font is strikethrough
+* `Cell.style.first_indent`: first line indent in points (`float`)
+* `Cell.style.left_indent`: left indent in points (`float`)
+* `Cell.style.right_indent`: right indent in points (`float`)
+* `Cell.style.text_inset`: text inset in points (`float`)
+
 
 #### Cell images
 
 The methods `style.bg_image.filename` and `style.bg_image.data` return data about the image used for a cell's background, where set. If a cell has no background image, `style.bg_image`  is `None`.
 
 ``` python
 cell = table.cell("B1")
```

