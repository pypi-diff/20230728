# Comparing `tmp/tkvue-2.1.3-py3-none-any.whl.zip` & `tmp/tkvue-2.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 196322 bytes, number of entries: 10
--rw-r--r--  2.0 unx    32214 b- defN 23-Jul-25 12:19 tkvue/__init__.py
+Zip file size: 196380 bytes, number of entries: 10
+-rw-r--r--  2.0 unx    32446 b- defN 23-Jul-26 17:21 tkvue/__init__.py
 -rw-rw-rw-  2.0 unx   170486 b- defN 23-Jul-12 18:03 tkvue/tests/preloader.gif
 -rw-rw-rw-  2.0 unx      814 b- defN 23-Jul-12 18:03 tkvue/tests/python_icon.png
 -rw-rw-rw-  2.0 unx    23217 b- defN 23-Jul-12 18:18 tkvue/tests/test_tkvue.py
--rw-rw-rw-  2.0 unx    26523 b- defN 23-Jul-25 12:39 tkvue-2.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     6478 b- defN 23-Jul-25 12:39 tkvue-2.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 12:39 tkvue-2.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-Jul-25 12:39 tkvue-2.1.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Jul-25 12:39 tkvue-2.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      794 b- defN 23-Jul-25 12:39 tkvue-2.1.3.dist-info/RECORD
-10 files, 260671 bytes uncompressed, 194978 bytes compressed:  25.2%
+-rw-rw-rw-  2.0 unx    26523 b- defN 23-Jul-28 15:01 tkvue-2.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6478 b- defN 23-Jul-28 15:01 tkvue-2.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-28 15:01 tkvue-2.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-Jul-28 15:01 tkvue-2.1.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-28 15:01 tkvue-2.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      794 b- defN 23-Jul-28 15:01 tkvue-2.1.4.dist-info/RECORD
+10 files, 260903 bytes uncompressed, 195036 bytes compressed:  25.2%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: tkvue/tests/python_icon.png
 Comment: 
 
 Filename: tkvue/tests/test_tkvue.py
 Comment: 
 
-Filename: tkvue-2.1.3.dist-info/LICENSE
+Filename: tkvue-2.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: tkvue-2.1.3.dist-info/METADATA
+Filename: tkvue-2.1.4.dist-info/METADATA
 Comment: 
 
-Filename: tkvue-2.1.3.dist-info/WHEEL
+Filename: tkvue-2.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: tkvue-2.1.3.dist-info/entry_points.txt
+Filename: tkvue-2.1.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: tkvue-2.1.3.dist-info/top_level.txt
+Filename: tkvue-2.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: tkvue-2.1.3.dist-info/RECORD
+Filename: tkvue-2.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tkvue/__init__.py

```diff
@@ -403,21 +403,21 @@
 
     if len(widget.frames) > 1:
         _start_animation()
     else:
         _stop_animation()
 
 
-@attr(ttk.Widget, "wrap")
+@attr(ttk.Label, "wrap")
 def _configure_wrap(widget, wrap):
     # Support Text wrapping
     if wrap.lower() in ["true", "1"]:
         widget.bind(
             "<Configure>",
-            lambda e: widget.configure(wraplen=widget.winfo_width()),
+            lambda e: widget.configure(wraplength=widget.winfo_width()),
             add="+",
         )
 
 
 @attr(tkinter.Tk, "theme")
 def _configure_theme(widget, value):
     # Defined on TopLevel
@@ -667,14 +667,22 @@
 
     def _update_bg(self, event):
         style_name = self.cget('style') or 'TFrame'
         bg = ttk.Style(master=self.master).lookup(style_name, "background")
         self.canvas.configure(bg=bg)
         self.interior.configure(style=style_name)
 
+    def configure(self, cnf=None, **kw):
+        """
+        Ovewrite configure to update style of canvas and interior.
+        """
+        super().configure(cnf, **kw)
+        if 'style' in kw:
+            self._update_bg(None)
+
 
 class TemplateError(Exception):
     """
     Raised when trying to create the component.
     """
 
     pass
```

## Comparing `tkvue-2.1.3.dist-info/LICENSE` & `tkvue-2.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tkvue-2.1.3.dist-info/METADATA` & `tkvue-2.1.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkvue
-Version: 2.1.3
+Version: 2.1.4
 Summary: Declarative Tkinter UI using makup language with reactive data binding
 Home-page: https://gitlab.com/ikus-soft/tkvue
 Author: IKUS Software inc.
 Author-email: support@ikus-soft.com
 Maintainer: Patrik Dufresne
 Maintainer-email: patrik@ikus-soft.com
 License: LGPLv3
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tkvue Version: 2.1.3 Summary: Declarative Tkinter
+Metadata-Version: 2.1 Name: tkvue Version: 2.1.4 Summary: Declarative Tkinter
 UI using makup language with reactive data binding Home-page: https://
 gitlab.com/ikus-soft/tkvue Author: IKUS Software inc. Author-email:
 support@ikus-soft.com Maintainer: Patrik Dufresne Maintainer-email:
 patrik@ikus-soft.com License: LGPLv3 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: X11 Applications Classifier: Environment :: Win32
 (MS Windows) Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: End Users/Desktop Classifier: License :: OSI Approved :: GNU Lesser
```

## Comparing `tkvue-2.1.3.dist-info/RECORD` & `tkvue-2.1.4.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-tkvue/__init__.py,sha256=Gwdj9kQkco-465TtfVpDrt--ZnbtFc86jBtDYjO4Kto,32214
+tkvue/__init__.py,sha256=zvV28g4pjnpQ1Ax5JD1dCk5BWy4qNU0hiPP0a3-3vCU,32446
 tkvue/tests/preloader.gif,sha256=4WubudKMAoutzmKtq4PR70A8DoCy5GC_fdVn08FRItc,170486
 tkvue/tests/python_icon.png,sha256=TNB4Jv9uPJYDC9CxCVUv6q5Fu6mlSx2Skuk68ckAcqQ,814
 tkvue/tests/test_tkvue.py,sha256=ou_M6PUEyTeVlPOA0UfTAaW4OyZigxjcXX7m86Cnv7A,23217
-tkvue-2.1.3.dist-info/LICENSE,sha256=wOyDtdXHKbVMd0kW1v8xZvyrYk9MeGP2-70glJMR9nc,26523
-tkvue-2.1.3.dist-info/METADATA,sha256=6aZVSjlx6QXjfTM8DnuAbphKBIIRwwLcrkqjuKlhbhk,6478
-tkvue-2.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-tkvue-2.1.3.dist-info/entry_points.txt,sha256=8VY5M0e9X8hXWRDu4nXU60waEEcTmLS5mRgxCmcVE88,47
-tkvue-2.1.3.dist-info/top_level.txt,sha256=anZORAc3YItPGY-GYRZ9zA_9cHsS-bhOtuYTL0R6ffU,6
-tkvue-2.1.3.dist-info/RECORD,,
+tkvue-2.1.4.dist-info/LICENSE,sha256=wOyDtdXHKbVMd0kW1v8xZvyrYk9MeGP2-70glJMR9nc,26523
+tkvue-2.1.4.dist-info/METADATA,sha256=yP2owdN2fZxpFNbFjOp9jWoRyiF_jY3tRKk-yibp7Fo,6478
+tkvue-2.1.4.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+tkvue-2.1.4.dist-info/entry_points.txt,sha256=8VY5M0e9X8hXWRDu4nXU60waEEcTmLS5mRgxCmcVE88,47
+tkvue-2.1.4.dist-info/top_level.txt,sha256=anZORAc3YItPGY-GYRZ9zA_9cHsS-bhOtuYTL0R6ffU,6
+tkvue-2.1.4.dist-info/RECORD,,
```

