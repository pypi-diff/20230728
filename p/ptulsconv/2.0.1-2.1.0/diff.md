# Comparing `tmp/ptulsconv-2.0.1.tar.gz` & `tmp/ptulsconv-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptulsconv-2.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ptulsconv-2.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ptulsconv-2.0.1.tar` & `ptulsconv-2.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1068 2023-07-22 20:04:34.183446 ptulsconv-2.0.1/LICENSE
--rw-r--r--   0        0        0     1246 2023-07-22 20:04:34.183446 ptulsconv-2.0.1/README.md
--rw-r--r--   0        0        0      225 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/__init__.py
--rw-r--r--   0        0        0     4074 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/__main__.py
--rw-r--r--   0        0        0     4297 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/broadcast_timecode.py
--rw-r--r--   0        0        0     9319 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/commands.py
--rw-r--r--   0        0        0       68 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/docparser/__init__.py
--rw-r--r--   0        0        0     4641 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/docparser/adr_entity.py
--rw-r--r--   0        0        0     5835 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/docparser/doc_entity.py
--rw-r--r--   0        0        0       36 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/docparser/generic_entity.py
--rw-r--r--   0        0        0    10371 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/docparser/pt_doc_parser.py
--rw-r--r--   0        0        0     7997 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/docparser/tag_compiler.py
--rw-r--r--   0        0        0     2948 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/docparser/tag_mapping.py
--rw-r--r--   0        0        0     2872 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/docparser/tagged_string_parser_visitor.py
--rw-r--r--   0        0        0      754 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/footage.py
--rw-r--r--   0        0        0      477 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/movie_export.py
--rw-r--r--   0        0        0    12703 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/pdf/__init__.py
--rw-r--r--   0        0        0     2102 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/pdf/continuity.py
--rw-r--r--   0        0        0    11362 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/pdf/line_count.py
--rw-r--r--   0        0        0       91 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/pdf/recordist_log.py
--rw-r--r--   0        0        0     5826 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/pdf/summary_log.py
--rw-r--r--   0        0        0    10929 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/pdf/supervisor_1pg.py
--rw-r--r--   0        0        0     3188 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/pdf/talent_sides.py
--rw-r--r--   0        0        0     2244 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/reporting.py
--rw-r--r--   0        0        0     2869 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/validations.py
--rw-r--r--   0        0        0     5909 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/xml/common.py
--rw-r--r--   0        0        0     3275 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/xslt/AvidMarkers.xsl
--rw-r--r--   0        0        0     1529 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/xslt/SRT.xsl
--rw-r--r--   0        0        0     1336 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     2385 1970-01-01 00:00:00.000000 ptulsconv-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-28 06:25:29.237999 ptulsconv-2.1.0/LICENSE
+-rw-r--r--   0        0        0     1246 2023-07-28 06:25:29.237999 ptulsconv-2.1.0/README.md
+-rw-r--r--   0        0        0      225 2023-07-28 06:25:29.245999 ptulsconv-2.1.0/ptulsconv/__init__.py
+-rw-r--r--   0        0        0     4074 2023-07-28 06:25:29.245999 ptulsconv-2.1.0/ptulsconv/__main__.py
+-rw-r--r--   0        0        0     4297 2023-07-28 06:25:29.249999 ptulsconv-2.1.0/ptulsconv/broadcast_timecode.py
+-rw-r--r--   0        0        0     9319 2023-07-28 06:25:29.249999 ptulsconv-2.1.0/ptulsconv/commands.py
+-rw-r--r--   0        0        0       68 2023-07-28 06:25:29.249999 ptulsconv-2.1.0/ptulsconv/docparser/__init__.py
+-rw-r--r--   0        0        0     4641 2023-07-28 06:25:29.249999 ptulsconv-2.1.0/ptulsconv/docparser/adr_entity.py
+-rw-r--r--   0        0        0     6177 2023-07-28 06:25:29.249999 ptulsconv-2.1.0/ptulsconv/docparser/doc_entity.py
+-rw-r--r--   0        0        0       36 2023-07-28 06:25:29.249999 ptulsconv-2.1.0/ptulsconv/docparser/generic_entity.py
+-rw-r--r--   0        0        0    10569 2023-07-28 06:25:29.249999 ptulsconv-2.1.0/ptulsconv/docparser/pt_doc_parser.py
+-rw-r--r--   0        0        0     7997 2023-07-28 06:25:29.249999 ptulsconv-2.1.0/ptulsconv/docparser/tag_compiler.py
+-rw-r--r--   0        0        0     2948 2023-07-28 06:25:29.249999 ptulsconv-2.1.0/ptulsconv/docparser/tag_mapping.py
+-rw-r--r--   0        0        0     2872 2023-07-28 06:25:29.249999 ptulsconv-2.1.0/ptulsconv/docparser/tagged_string_parser_visitor.py
+-rw-r--r--   0        0        0      754 2023-07-28 06:25:29.249999 ptulsconv-2.1.0/ptulsconv/footage.py
+-rw-r--r--   0        0        0      477 2023-07-28 06:25:29.249999 ptulsconv-2.1.0/ptulsconv/movie_export.py
+-rw-r--r--   0        0        0    12703 2023-07-28 06:25:29.249999 ptulsconv-2.1.0/ptulsconv/pdf/__init__.py
+-rw-r--r--   0        0        0     2102 2023-07-28 06:25:29.249999 ptulsconv-2.1.0/ptulsconv/pdf/continuity.py
+-rw-r--r--   0        0        0    11362 2023-07-28 06:25:29.249999 ptulsconv-2.1.0/ptulsconv/pdf/line_count.py
+-rw-r--r--   0        0        0       91 2023-07-28 06:25:29.249999 ptulsconv-2.1.0/ptulsconv/pdf/recordist_log.py
+-rw-r--r--   0        0        0     5826 2023-07-28 06:25:29.249999 ptulsconv-2.1.0/ptulsconv/pdf/summary_log.py
+-rw-r--r--   0        0        0    10929 2023-07-28 06:25:29.249999 ptulsconv-2.1.0/ptulsconv/pdf/supervisor_1pg.py
+-rw-r--r--   0        0        0     3188 2023-07-28 06:25:29.249999 ptulsconv-2.1.0/ptulsconv/pdf/talent_sides.py
+-rw-r--r--   0        0        0     2244 2023-07-28 06:25:29.249999 ptulsconv-2.1.0/ptulsconv/reporting.py
+-rw-r--r--   0        0        0     2869 2023-07-28 06:25:29.249999 ptulsconv-2.1.0/ptulsconv/validations.py
+-rw-r--r--   0        0        0     5909 2023-07-28 06:25:29.249999 ptulsconv-2.1.0/ptulsconv/xml/common.py
+-rw-r--r--   0        0        0     3275 2023-07-28 06:25:29.249999 ptulsconv-2.1.0/ptulsconv/xslt/AvidMarkers.xsl
+-rw-r--r--   0        0        0     1529 2023-07-28 06:25:29.249999 ptulsconv-2.1.0/ptulsconv/xslt/SRT.xsl
+-rw-r--r--   0        0        0     1336 2023-07-28 06:25:29.249999 ptulsconv-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2385 1970-01-01 00:00:00.000000 ptulsconv-2.1.0/PKG-INFO
```

### Comparing `ptulsconv-2.0.1/LICENSE` & `ptulsconv-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.1/README.md` & `ptulsconv-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.1/ptulsconv/__main__.py` & `ptulsconv-2.1.0/ptulsconv/__main__.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.1/ptulsconv/broadcast_timecode.py` & `ptulsconv-2.1.0/ptulsconv/broadcast_timecode.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.1/ptulsconv/commands.py` & `ptulsconv-2.1.0/ptulsconv/commands.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.1/ptulsconv/docparser/adr_entity.py` & `ptulsconv-2.1.0/ptulsconv/docparser/adr_entity.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.1/ptulsconv/docparser/doc_entity.py` & `ptulsconv-2.1.0/ptulsconv/docparser/doc_entity.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,32 +16,41 @@
         self.files = kwargs['files']
         self.clips = kwargs['clips']
         self.plugins = kwargs['plugins']
         self.tracks = kwargs['tracks']
         self.markers = kwargs['markers']
 
     def markers_timed(self) -> Iterator[Tuple['MarkerDescriptor', Fraction]]:
+        """
+        Iterate each marker in the session with its respective time reference.
+        """
         for marker in self.markers:
             marker_time = Fraction(marker.time_reference,
                                    int(self.header.sample_rate))
             # marker_time = self.header.convert_timecode(marker.location)
             yield marker, marker_time
 
     def tracks_clips(self) -> Iterator[Tuple['TrackDescriptor',
                                              'TrackClipDescriptor']]:
+        """
+        Iterate each track clip with its respective owning clip.
+        """
         for track in self.tracks:
             for clip in track.clips:
                 yield track, clip
 
     def track_clips_timed(self) -> Iterator[Tuple["TrackDescriptor",
                                                   "TrackClipDescriptor",
                                                   Fraction, Fraction, Fraction]
                                             ]:
         """
-        :return: A Generator that yields track, clip, start time, finish time,
+        Iterate each track clip with its respective owning clip and timing
+        information.
+
+        :returns: A Generator that yields track, clip, start time, finish time,
         and timestamp
         """
         for track, clip in self.tracks_clips():
             start_time = self.header.convert_timecode(clip.start_timecode)
             finish_time = self.header.convert_timecode(clip.finish_timecode)
             timestamp_time = self.header.convert_timecode(clip.timestamp) \
                 if clip.timestamp is not None else None
@@ -111,22 +120,24 @@
             return frame_rates[self.timecode_fps]
         else:
             raise ValueError("Unrecognized TC rate (%s)" %
                              self.timecode_format)
 
 
 class TrackDescriptor:
+    index: int
     name: str
     comments: str
     user_delay_samples: int
     state: List[str]
     plugins: List[str]
     clips: List["TrackClipDescriptor"]
 
     def __init__(self, **kwargs):
+        self.index = kwargs['index']
         self.name = kwargs['name']
         self.comments = kwargs['comments']
         self.user_delay_samples = kwargs['user_delay_samples']
         self.state = kwargs['state']
         self.plugins = kwargs['plugins']
         self.clips = kwargs['clips']
```

### Comparing `ptulsconv-2.0.1/ptulsconv/docparser/pt_doc_parser.py` & `ptulsconv-2.1.0/ptulsconv/docparser/pt_doc_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,16 +104,20 @@
     """
     ast = protools_text_export_grammar.parse(session_text)
     return DocParserVisitor().visit(ast)
 
 
 class DocParserVisitor(NodeVisitor):
 
-    @staticmethod
-    def visit_document(_, visited_children) -> SessionDescriptor:
+    def __init__(self):
+        self.track_index = 0
+
+    # @staticmethod
+    def visit_document(self, _, visited_children) -> SessionDescriptor:
+        self.track_index = 0
         files = next(iter(visited_children[1]), None)
         clips = next(iter(visited_children[2]), None)
         plugins = next(iter(visited_children[3]), None)
         tracks = next(iter(visited_children[4]), None)
         markers = next(iter(visited_children[5]), None)
 
         return SessionDescriptor(header=visited_children[0],
@@ -162,28 +166,32 @@
                                          plugin_name=child[2],
                                          version=child[4],
                                          format=child[6],
                                          stems=child[8],
                                          count_instances=child[10]),
                         visited_children[2]))
 
-    @staticmethod
-    def visit_track_block(_, visited_children):
+    # @staticmethod
+    def visit_track_block(self, _, visited_children):
         track_header, track_clip_list = visited_children
         clips = []
         for clip in track_clip_list:
             if clip[0] is not None:
                 clips.append(clip[0])
 
         plugins = []
         for plugin_opt in track_header[16]:
             for plugin in plugin_opt[1]:
                 plugins.append(plugin[1])
 
+        this_index = self.track_index
+        self.track_index += 1
+
         return TrackDescriptor(
+            index=this_index,
             name=track_header[2],
             comments=track_header[6],
             user_delay_samples=track_header[10],
             state=track_header[14],
             plugins=plugins,
             clips=clips
         )
```

### Comparing `ptulsconv-2.0.1/ptulsconv/docparser/tag_compiler.py` & `ptulsconv-2.1.0/ptulsconv/docparser/tag_compiler.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.1/ptulsconv/docparser/tag_mapping.py` & `ptulsconv-2.1.0/ptulsconv/docparser/tag_mapping.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.1/ptulsconv/docparser/tagged_string_parser_visitor.py` & `ptulsconv-2.1.0/ptulsconv/docparser/tagged_string_parser_visitor.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.1/ptulsconv/footage.py` & `ptulsconv-2.1.0/ptulsconv/footage.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.1/ptulsconv/pdf/__init__.py` & `ptulsconv-2.1.0/ptulsconv/pdf/__init__.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.1/ptulsconv/pdf/continuity.py` & `ptulsconv-2.1.0/ptulsconv/pdf/continuity.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.1/ptulsconv/pdf/line_count.py` & `ptulsconv-2.1.0/ptulsconv/pdf/line_count.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.1/ptulsconv/pdf/summary_log.py` & `ptulsconv-2.1.0/ptulsconv/pdf/summary_log.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.1/ptulsconv/pdf/supervisor_1pg.py` & `ptulsconv-2.1.0/ptulsconv/pdf/supervisor_1pg.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.1/ptulsconv/pdf/talent_sides.py` & `ptulsconv-2.1.0/ptulsconv/pdf/talent_sides.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.1/ptulsconv/reporting.py` & `ptulsconv-2.1.0/ptulsconv/reporting.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.1/ptulsconv/validations.py` & `ptulsconv-2.1.0/ptulsconv/validations.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.1/ptulsconv/xml/common.py` & `ptulsconv-2.1.0/ptulsconv/xml/common.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.1/ptulsconv/xslt/AvidMarkers.xsl` & `ptulsconv-2.1.0/ptulsconv/xslt/AvidMarkers.xsl`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.1/ptulsconv/xslt/SRT.xsl` & `ptulsconv-2.1.0/ptulsconv/xslt/SRT.xsl`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.1/pyproject.toml` & `ptulsconv-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.1/PKG-INFO` & `ptulsconv-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptulsconv
-Version: 2.0.1
+Version: 2.1.0
 Summary: Parse and convert Pro Tools text exports
 Keywords: text-processing,parsers,film,broadcast,editing,editorial
 Author-email: Jamie Hardt <jamiehardt@me.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Multimedia
```

