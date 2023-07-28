# Comparing `tmp/FontCollector-2.1.1.tar.gz` & `tmp/FontCollector-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FontCollector-2.1.1.tar", last modified: Fri Jun 16 01:13:12 2023, max compression
+gzip compressed data, was "FontCollector-2.1.2.tar", last modified: Fri Jul 28 00:25:19 2023, max compression
```

## Comparing `FontCollector-2.1.1.tar` & `FontCollector-2.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 01:13:12.740296 FontCollector-2.1.1/
-drwxrwxrwx   0        0        0        0 2023-06-16 01:13:12.715363 FontCollector-2.1.1/FontCollector.egg-info/
--rw-rw-rw-   0        0        0     4765 2023-06-16 01:13:12.000000 FontCollector-2.1.1/FontCollector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      745 2023-06-16 01:13:12.000000 FontCollector-2.1.1/FontCollector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 01:13:12.000000 FontCollector-2.1.1/FontCollector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-16 01:13:12.000000 FontCollector-2.1.1/FontCollector.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       82 2023-06-16 01:13:12.000000 FontCollector-2.1.1/FontCollector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-16 01:13:12.000000 FontCollector-2.1.1/FontCollector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2023-03-18 01:24:14.000000 FontCollector-2.1.1/LICENSE
--rw-rw-rw-   0        0        0     4765 2023-06-16 01:13:12.740296 FontCollector-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3876 2023-03-27 00:41:02.000000 FontCollector-2.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 01:13:12.734313 FontCollector-2.1.1/font_collector/
--rw-rw-rw-   0        0        0     1048 2023-06-16 01:05:57.000000 FontCollector-2.1.1/font_collector/__init__.py
--rw-rw-rw-   0        0        0     2936 2023-03-27 00:42:58.000000 FontCollector-2.1.1/font_collector/__main__.py
--rw-rw-rw-   0        0        0       23 2023-06-16 01:01:23.000000 FontCollector-2.1.1/font_collector/_version.py
--rw-rw-rw-   0        0        0     8738 2023-02-26 01:44:56.000000 FontCollector-2.1.1/font_collector/ass_document.py
--rw-rw-rw-   0        0        0     1735 2023-01-02 02:08:59.000000 FontCollector-2.1.1/font_collector/ass_style.py
--rw-rw-rw-   0        0        0      205 2023-03-27 00:40:01.000000 FontCollector-2.1.1/font_collector/exceptions.py
--rw-rw-rw-   0        0        0    10064 2023-06-01 00:26:56.000000 FontCollector-2.1.1/font_collector/font.py
--rw-rw-rw-   0        0        0     5933 2023-06-16 01:01:23.000000 FontCollector-2.1.1/font_collector/font_loader.py
--rw-rw-rw-   0        0        0    22962 2023-06-12 21:16:42.000000 FontCollector-2.1.1/font_collector/font_parser.py
--rw-rw-rw-   0        0        0      510 2023-01-03 18:11:21.000000 FontCollector-2.1.1/font_collector/font_result.py
--rw-rw-rw-   0        0        0     7456 2023-06-16 00:45:55.000000 FontCollector-2.1.1/font_collector/helpers.py
--rw-rw-rw-   0        0        0     5387 2023-02-27 01:22:25.000000 FontCollector-2.1.1/font_collector/mkvpropedit.py
--rw-rw-rw-   0        0        0     3842 2023-01-26 18:34:43.000000 FontCollector-2.1.1/font_collector/parse_arguments.py
--rw-rw-rw-   0        0        0      692 2023-01-03 18:11:21.000000 FontCollector-2.1.1/font_collector/usage_data.py
--rw-rw-rw-   0        0        0       42 2023-06-16 01:13:12.740296 FontCollector-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2762 2023-06-16 01:01:23.000000 FontCollector-2.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 01:13:12.739299 FontCollector-2.1.1/tests/
--rw-rw-rw-   0        0        0      918 2023-01-22 16:04:34.000000 FontCollector-2.1.1/tests/test_ass_document.py
--rw-rw-rw-   0        0        0     8629 2023-06-01 00:26:56.000000 FontCollector-2.1.1/tests/test_font.py
--rw-rw-rw-   0        0        0     1037 2023-03-27 01:07:59.000000 FontCollector-2.1.1/tests/test_font_parser.py
--rw-rw-rw-   0        0        0      902 2023-06-16 01:01:23.000000 FontCollector-2.1.1/tests/test_helpers.py
+drwxrwxrwx   0        0        0        0 2023-07-28 00:25:19.053172 FontCollector-2.1.2/
+drwxrwxrwx   0        0        0        0 2023-07-28 00:25:19.030234 FontCollector-2.1.2/FontCollector.egg-info/
+-rw-rw-rw-   0        0        0     4765 2023-07-28 00:25:18.000000 FontCollector-2.1.2/FontCollector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      745 2023-07-28 00:25:18.000000 FontCollector-2.1.2/FontCollector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 00:25:18.000000 FontCollector-2.1.2/FontCollector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-07-28 00:25:18.000000 FontCollector-2.1.2/FontCollector.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       82 2023-07-28 00:25:18.000000 FontCollector-2.1.2/FontCollector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-28 00:25:18.000000 FontCollector-2.1.2/FontCollector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2023-03-18 01:24:14.000000 FontCollector-2.1.2/LICENSE
+-rw-rw-rw-   0        0        0     4765 2023-07-28 00:25:19.052176 FontCollector-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3876 2023-03-27 00:41:02.000000 FontCollector-2.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 00:25:19.046191 FontCollector-2.1.2/font_collector/
+-rw-rw-rw-   0        0        0     1048 2023-06-16 01:05:57.000000 FontCollector-2.1.2/font_collector/__init__.py
+-rw-rw-rw-   0        0        0     2982 2023-07-28 00:24:41.000000 FontCollector-2.1.2/font_collector/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-07-28 00:24:41.000000 FontCollector-2.1.2/font_collector/_version.py
+-rw-rw-rw-   0        0        0     9789 2023-07-28 00:24:41.000000 FontCollector-2.1.2/font_collector/ass_document.py
+-rw-rw-rw-   0        0        0     1735 2023-01-02 02:08:59.000000 FontCollector-2.1.2/font_collector/ass_style.py
+-rw-rw-rw-   0        0        0      205 2023-03-27 00:40:01.000000 FontCollector-2.1.2/font_collector/exceptions.py
+-rw-rw-rw-   0        0        0    10064 2023-06-01 00:26:56.000000 FontCollector-2.1.2/font_collector/font.py
+-rw-rw-rw-   0        0        0     5933 2023-06-16 01:01:23.000000 FontCollector-2.1.2/font_collector/font_loader.py
+-rw-rw-rw-   0        0        0    22962 2023-06-12 21:16:42.000000 FontCollector-2.1.2/font_collector/font_parser.py
+-rw-rw-rw-   0        0        0      510 2023-01-03 18:11:21.000000 FontCollector-2.1.2/font_collector/font_result.py
+-rw-rw-rw-   0        0        0     7456 2023-06-16 00:45:55.000000 FontCollector-2.1.2/font_collector/helpers.py
+-rw-rw-rw-   0        0        0     5387 2023-02-27 01:22:25.000000 FontCollector-2.1.2/font_collector/mkvpropedit.py
+-rw-rw-rw-   0        0        0     4214 2023-07-28 00:24:41.000000 FontCollector-2.1.2/font_collector/parse_arguments.py
+-rw-rw-rw-   0        0        0      692 2023-01-03 18:11:21.000000 FontCollector-2.1.2/font_collector/usage_data.py
+-rw-rw-rw-   0        0        0       42 2023-07-28 00:25:19.053172 FontCollector-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2762 2023-06-16 01:01:23.000000 FontCollector-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 00:25:19.051178 FontCollector-2.1.2/tests/
+-rw-rw-rw-   0        0        0     1558 2023-07-28 00:24:41.000000 FontCollector-2.1.2/tests/test_ass_document.py
+-rw-rw-rw-   0        0        0     8629 2023-06-01 00:26:56.000000 FontCollector-2.1.2/tests/test_font.py
+-rw-rw-rw-   0        0        0     1037 2023-03-27 01:07:59.000000 FontCollector-2.1.2/tests/test_font_parser.py
+-rw-rw-rw-   0        0        0      902 2023-06-16 01:01:23.000000 FontCollector-2.1.2/tests/test_helpers.py
```

### Comparing `FontCollector-2.1.1/FontCollector.egg-info/PKG-INFO` & `FontCollector-2.1.2/FontCollector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FontCollector
-Version: 2.1.1
+Version: 2.1.2
 Summary: FontCollector for Advanced SubStation Alpha file.
 Home-page: https://github.com/moi15moi/FontCollector/
 Author: moi15moi
 Author-email: moi15moismokerlolilol@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/moi15moi/FontCollector/
 Project-URL: Tracker, https://github.com/moi15moi/FontCollector/issues/
```

### Comparing `FontCollector-2.1.1/FontCollector.egg-info/SOURCES.txt` & `FontCollector-2.1.2/FontCollector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FontCollector-2.1.1/LICENSE` & `FontCollector-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FontCollector-2.1.1/PKG-INFO` & `FontCollector-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FontCollector
-Version: 2.1.1
+Version: 2.1.2
 Summary: FontCollector for Advanced SubStation Alpha file.
 Home-page: https://github.com/moi15moi/FontCollector/
 Author: moi15moi
 Author-email: moi15moismokerlolilol@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/moi15moi/FontCollector/
 Project-URL: Tracker, https://github.com/moi15moi/FontCollector/issues/
```

### Comparing `FontCollector-2.1.1/README.md` & `FontCollector-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `FontCollector-2.1.1/font_collector/__init__.py` & `FontCollector-2.1.2/font_collector/__init__.py`

 * *Files identical despite different names*

### Comparing `FontCollector-2.1.1/font_collector/__main__.py` & `FontCollector-2.1.2/font_collector/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,22 +17,23 @@
     (
         ass_files_path,
         output_directory,
         mkv_path,
         delete_fonts,
         additional_fonts,
         use_system_font,
+        collect_draw_fonts
     ) = parse_arguments()
     font_results: List[FontResult] = []
     font_collection = FontLoader(additional_fonts, use_system_font).fonts
 
     for ass_path in ass_files_path:
         subtitle = AssDocument.from_file(ass_path)
         _logger.info(f"Loaded successfully {ass_path}")
-        styles = subtitle.get_used_style()
+        styles = subtitle.get_used_style(collect_draw_fonts)
 
         nbr_font_not_found = 0
 
         for style, usage_data in styles.items():
 
             font_result = Helpers.get_used_font_by_style(font_collection, style)
```

### Comparing `FontCollector-2.1.1/font_collector/ass_document.py` & `FontCollector-2.1.2/font_collector/ass_document.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 from .ass_style import AssStyle
 from .usage_data import UsageData
 from ass import parse_file, parse_string, Dialogue, Document
 from ass_tag_analyzer import (
+    AssDraw,
     AssInvalidTagBold,
     AssInvalidTagFontName,
     AssInvalidTagItalic,
     AssInvalidTagResetStyle,
     AssInvalidTagWrapStyle,
     AssItem,
     AssTagBold,
@@ -54,25 +55,27 @@
         tags: List[AssItem],
         line_index: int,
         sub_styles: Dict[str, AssStyle],
         original_line_style: AssStyle,
         line_style: AssStyle,
         current_style: AssStyle,
         current_wrap_style: WrapStyle,
+        collect_draw_fonts: bool
     ) -> None:
         """
         Parameters:
             used_styles (Dict[AssStyle, UsageData]): This variable will be modified
             tags (List[AssItem]): List of all tags
             line_index (int): Position of the line in the subtitle
             sub_styles (Dict[str, AssStyle]): Dict of the [V4+ Styles] sections
             original_line_style (AssStyle): Style of the line
             line_style (AssStyle): Style of the line. In general, it will be equal to original_line_style except it there is an \rXXX
             current_style (AssStyle): Real style of the text. It exist since \fn, \b, \i can override the line_style.
             current_wrap_style (WrapStyle): Since \q can override the subtitle WrapStyle, we need it.
+            collect_draw_fonts (bool): If true, then it will also collect the draw style, if false, it will ignore it.
         """
 
         for tag in tags:
             if isinstance(tag, AssTagResetStyle):
                 if isinstance(tag, AssValidTagResetStyle):
                     style = sub_styles.get(tag.style, original_line_style)
 
@@ -123,14 +126,15 @@
                     tag.tags,
                     line_index,
                     sub_styles,
                     original_line_style,
                     line_style,
                     current_style,
                     current_wrap_style,
+                    collect_draw_fonts
                 )
 
             elif isinstance(tag, AssText):
                 # Inspired by
                 #     - https://github.com/libass/libass/blob/a2b39cde4ecb74d5e6fccab4a5f7d8ad52b2b1a4/libass/ass_parse.c#L1039-L1075
                 #     - Aegisub FontCollector ignore \n: https://github.com/arch1t3cht/Aegisub/blob/fad362ec2e2975d8e37893c6dfb3a39452e71d23/src/font_file_lister.cpp#L118-L120
                 text = tag.text.replace("\t", " ")
@@ -152,17 +156,32 @@
                     usage_data.characters_used.update(set(text))
                     usage_data.lines.add(line_index)
 
                 # We need to make an copy of the style since current_style can be modified
                 current_style = AssStyle(
                     current_style.fontname, current_style.weight, current_style.italic
                 )
+            elif collect_draw_fonts and isinstance(tag, AssDraw):
+                usage_data = used_styles.get(current_style, None)
+                if usage_data is None:
+                    usage_data = UsageData(set(), set([line_index]))
+                    used_styles[current_style] = usage_data
+                else:
+                    usage_data.lines.add(line_index)
+
+                # We need to make an copy of the style since current_style can be modified
+                current_style = AssStyle(
+                    current_style.fontname, current_style.weight, current_style.italic
+                )
+
 
-    def get_used_style(self) -> Dict[AssStyle, UsageData]:
+    def get_used_style(self, collect_draw_fonts: bool = False) -> Dict[AssStyle, UsageData]:
         """
+        Parameters:
+            collect_draw_fonts (bool): If true, then it will also collect the draw style, if false, it will ignore it.
         Returns:
             An dictionnary which contain all the used AssStyle and it's UsageData.
         """
         used_styles: Dict[AssStyle, UsageData] = {}
 
         # VSFilter trim:
         #   - *: https://sourceforge.net/p/guliverkli2/code/HEAD/tree/src/subtitles/STS.cpp#l1447
@@ -207,10 +226,11 @@
                     tags,
                     i + 1,
                     sub_styles,
                     original_line_style,
                     line_style,
                     current_style,
                     sub_wrap_style,
+                    collect_draw_fonts
                 )
 
         return used_styles
```

### Comparing `FontCollector-2.1.1/font_collector/ass_style.py` & `FontCollector-2.1.2/font_collector/ass_style.py`

 * *Files identical despite different names*

### Comparing `FontCollector-2.1.1/font_collector/font.py` & `FontCollector-2.1.2/font_collector/font.py`

 * *Files identical despite different names*

### Comparing `FontCollector-2.1.1/font_collector/font_loader.py` & `FontCollector-2.1.2/font_collector/font_loader.py`

 * *Files identical despite different names*

### Comparing `FontCollector-2.1.1/font_collector/font_parser.py` & `FontCollector-2.1.2/font_collector/font_parser.py`

 * *Files identical despite different names*

### Comparing `FontCollector-2.1.1/font_collector/helpers.py` & `FontCollector-2.1.2/font_collector/helpers.py`

 * *Files identical despite different names*

### Comparing `FontCollector-2.1.1/font_collector/mkvpropedit.py` & `FontCollector-2.1.2/font_collector/mkvpropedit.py`

 * *Files identical despite different names*

### Comparing `FontCollector-2.1.1/font_collector/parse_arguments.py` & `FontCollector-2.1.2/font_collector/parse_arguments.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 def parse_arguments() -> Tuple[
     List[Path],
     Path,
     Union[Path, None],
     bool,
     Set[Path],
     bool,
+    bool
 ]:
     """
     Returns:
         ass_files_path, output_directory, mkv_path, delete_fonts, additional_fonts, use_system_fonts
     """
     parser = ArgumentParser(
         description="FontCollector for Advanced SubStation Alpha file."
@@ -98,14 +99,21 @@
     parser.add_argument(
         "--exclude-system-fonts",
         action="store_false",
         help="""
     If specified, FontCollector won't use the system font to find the font used by an .ass file.
     """,
     )
+    parser.add_argument(
+        "--collect-draw-fonts",
+        action="store_true",
+        help="""
+    If specified, FontCollector will collect the font used by the draw. For more detail when this is usefull, see: https://github.com/libass/libass/issues/617
+    """,
+    )
 
     args = parser.parse_args()
 
     # Parse args
     ass_files_path = _parse_input_file(args.input)
 
     output_directory = args.output
@@ -119,16 +127,18 @@
 
     if args.additional_fonts is not None:
         additional_fonts = args.additional_fonts
     else:
         additional_fonts = set()
 
     use_system_fonts = args.exclude_system_fonts
+    collect_draw_fonts = args.collect_draw_fonts
 
     return (
         ass_files_path,
         output_directory,
         mkv_path,
         delete_fonts,
         additional_fonts,
         use_system_fonts,
+        collect_draw_fonts
     )
```

### Comparing `FontCollector-2.1.1/font_collector/usage_data.py` & `FontCollector-2.1.2/font_collector/usage_data.py`

 * *Files identical despite different names*

### Comparing `FontCollector-2.1.1/setup.py` & `FontCollector-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `FontCollector-2.1.1/tests/test_ass_document.py` & `FontCollector-2.1.2/tests/test_ass_document.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,42 @@
 import os
 from font_collector import AssDocument, AssStyle, UsageData
 
 # Get ass path used for tests
 dir_path = os.path.dirname(os.path.realpath(__file__))
-path_ass = os.path.join(dir_path, "ass", "Untitled.ass")
-
-subtitle = AssDocument.from_file(path_ass)
 
 
 def test_get_style_used():
+    path_ass = os.path.join(dir_path, "ass", "Style test.ass")
+    subtitle = AssDocument.from_file(path_ass)
+
     styles = subtitle.get_used_style()
 
     expected_results = {
         AssStyle("Sunny Spells", 700, True): UsageData(set("example"), {1}),
         AssStyle("Akashi", 700, True): UsageData(set("Multiple \\t"), {2}),
         AssStyle("Bodo Amat", 400, True): UsageData(set("Italic"), {3}),
         AssStyle("Bodo Amat", 400, False): UsageData(set("Regular"), {3}),
         AssStyle("Avenir LT 65 Medium", 400, False): UsageData(
             set("Don't match with style"), {4}
         ),
         AssStyle("Asap", 400, True): UsageData(set("\\r override"), {5}),
     }
 
     assert styles == expected_results
+
+def test_get_style_used_with_and_without_collect_draw_fonts():
+    path_ass = os.path.join(dir_path, "ass", "Collect Draw Style test.ass")
+    subtitle = AssDocument.from_file(path_ass)
+
+    styles = subtitle.get_used_style()
+    expected_results = {
+        AssStyle("Jester", 700, False): UsageData(set("Test"), {1}),
+    }
+    assert styles == expected_results
+
+    styles = subtitle.get_used_style(True)
+    expected_results = {
+        AssStyle("Jester", 700, False): UsageData(set("Test"), {1}),
+        AssStyle("testgmail", 700, False): UsageData(set(), {2}),
+    }
+    assert styles == expected_results
```

### Comparing `FontCollector-2.1.1/tests/test_font.py` & `FontCollector-2.1.2/tests/test_font.py`

 * *Files identical despite different names*

### Comparing `FontCollector-2.1.1/tests/test_font_parser.py` & `FontCollector-2.1.2/tests/test_font_parser.py`

 * *Files identical despite different names*

### Comparing `FontCollector-2.1.1/tests/test_helpers.py` & `FontCollector-2.1.2/tests/test_helpers.py`

 * *Files identical despite different names*

