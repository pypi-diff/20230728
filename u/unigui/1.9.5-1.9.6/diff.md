# Comparing `tmp/unigui-1.9.5.tar.gz` & `tmp/unigui-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unigui-1.9.5.tar", last modified: Thu Jul 27 17:34:48 2023, max compression
+gzip compressed data, was "dist/unigui-1.9.6.tar", last modified: Fri Jul 28 10:58:33 2023, max compression
```

## Comparing `unigui-1.9.5.tar` & `unigui-1.9.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-27 17:34:48.000000 unigui-1.9.5/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-27 17:34:48.000000 unigui-1.9.5/unigui/
--rw-rw-r--   0 george    (1000) george    (1000)     5250 2023-07-26 02:29:57.000000 unigui-1.9.5/unigui/guielements.py
--rw-rw-r--   0 george    (1000) george    (1000)     3531 2023-07-26 16:18:00.000000 unigui-1.9.5/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)     4299 2023-07-25 09:16:10.000000 unigui-1.9.5/unigui/tables.py
--rw-rw-r--   0 george    (1000) george    (1000)      128 2023-07-25 04:04:00.000000 unigui-1.9.5/unigui/__init__.py
--rw-rw-r--   0 george    (1000) george    (1000)     7370 2023-07-26 17:26:22.000000 unigui-1.9.5/unigui/autotest.py
--rw-r--r--   0 george    (1000) george    (1000)     2642 2023-07-26 17:28:06.000000 unigui-1.9.5/unigui/utils.py
--rw-rw-r--   0 george    (1000) george    (1000)     5573 2023-07-26 17:26:38.000000 unigui-1.9.5/unigui/reloader.py
--rw-rw-r--   0 george    (1000) george    (1000)     8713 2023-07-26 09:11:50.000000 unigui-1.9.5/unigui/users.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-27 17:34:48.000000 unigui-1.9.5/unigui/web/
--rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/favicon.ico
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-27 17:34:48.000000 unigui-1.9.5/unigui/web/css/
--rw-rw-r--   0 george    (1000) george    (1000)        0 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/css/app.31d6cfe0.css
--rw-rw-r--   0 george    (1000) george    (1000)     2750 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/css/982.c7dd083b.css
--rw-rw-r--   0 george    (1000) george    (1000)   220628 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/css/vendor.f747ec02.css
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-27 17:34:48.000000 unigui-1.9.5/unigui/web/icons/
--rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/icons/favicon-96x96.png
--rw-rw-r--   0 george    (1000) george    (1000)      859 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/icons/favicon-16x16.png
--rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/icons/favicon-32x32.png
--rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/icons/favicon-128x128.png
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-27 17:34:48.000000 unigui-1.9.5/unigui/web/fonts/
--rw-rw-r--   0 george    (1000) george    (1000)   128616 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
--rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-27 17:34:48.000000 unigui-1.9.5/unigui/web/js/
--rw-rw-r--   0 george    (1000) george    (1000)  1436034 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/js/vendor.5659ce27.js
--rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/js/430.591e9a73.js
--rw-rw-r--   0 george    (1000) george    (1000)    49159 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/js/982.872ac96a.js
--rw-rw-r--   0 george    (1000) george    (1000)     5923 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/js/app.6805317c.js
--rw-rw-r--   0 george    (1000) george    (1000)      763 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/js/193.283445be.js
--rw-rw-r--   0 george    (1000) george    (1000)      907 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/index.html
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.9.5/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)      642 2023-07-27 17:33:52.000000 unigui-1.9.5/setup.py
--rw-rw-r--   0 george    (1000) george    (1000)    18810 2023-07-27 17:34:48.000000 unigui-1.9.5/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-27 17:34:48.000000 unigui-1.9.5/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)    18505 2023-07-27 09:01:10.000000 unigui-1.9.5/README.md
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.9.5/MANIFEST.in
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-27 17:34:48.000000 unigui-1.9.5/unigui.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)       63 2023-07-27 17:34:48.000000 unigui-1.9.5/unigui.egg-info/requires.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-27 17:34:48.000000 unigui-1.9.5/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)    18810 2023-07-27 17:34:48.000000 unigui-1.9.5/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.9.5/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)     1258 2023-07-27 17:34:48.000000 unigui-1.9.5/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-27 17:34:48.000000 unigui-1.9.5/unigui.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-28 10:58:33.000000 unigui-1.9.6/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-28 10:58:33.000000 unigui-1.9.6/unigui/
+-rw-rw-r--   0 george    (1000) george    (1000)     5553 2023-07-28 10:27:58.000000 unigui-1.9.6/unigui/guielements.py
+-rw-rw-r--   0 george    (1000) george    (1000)     3531 2023-07-26 16:18:00.000000 unigui-1.9.6/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)     4299 2023-07-25 09:16:10.000000 unigui-1.9.6/unigui/tables.py
+-rw-rw-r--   0 george    (1000) george    (1000)      128 2023-07-25 04:04:00.000000 unigui-1.9.6/unigui/__init__.py
+-rw-rw-r--   0 george    (1000) george    (1000)     7589 2023-07-28 09:59:05.000000 unigui-1.9.6/unigui/autotest.py
+-rw-r--r--   0 george    (1000) george    (1000)     2642 2023-07-26 17:28:06.000000 unigui-1.9.6/unigui/utils.py
+-rw-rw-r--   0 george    (1000) george    (1000)     5573 2023-07-26 17:26:38.000000 unigui-1.9.6/unigui/reloader.py
+-rw-rw-r--   0 george    (1000) george    (1000)     8713 2023-07-26 09:11:50.000000 unigui-1.9.6/unigui/users.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-28 10:58:33.000000 unigui-1.9.6/unigui/web/
+-rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-07-28 10:54:44.000000 unigui-1.9.6/unigui/web/favicon.ico
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-28 10:58:33.000000 unigui-1.9.6/unigui/web/css/
+-rw-rw-r--   0 george    (1000) george    (1000)        0 2023-07-28 10:54:44.000000 unigui-1.9.6/unigui/web/css/app.31d6cfe0.css
+-rw-rw-r--   0 george    (1000) george    (1000)   220628 2023-07-28 10:54:44.000000 unigui-1.9.6/unigui/web/css/vendor.f747ec02.css
+-rw-rw-r--   0 george    (1000) george    (1000)     2750 2023-07-28 10:54:44.000000 unigui-1.9.6/unigui/web/css/652.5cfe42ce.css
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-28 10:58:33.000000 unigui-1.9.6/unigui/web/icons/
+-rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-07-28 10:54:44.000000 unigui-1.9.6/unigui/web/icons/favicon-96x96.png
+-rw-rw-r--   0 george    (1000) george    (1000)      859 2023-07-28 10:54:44.000000 unigui-1.9.6/unigui/web/icons/favicon-16x16.png
+-rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-07-28 10:54:44.000000 unigui-1.9.6/unigui/web/icons/favicon-32x32.png
+-rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-07-28 10:54:44.000000 unigui-1.9.6/unigui/web/icons/favicon-128x128.png
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-28 10:58:33.000000 unigui-1.9.6/unigui/web/fonts/
+-rw-rw-r--   0 george    (1000) george    (1000)   128616 2023-07-28 10:54:44.000000 unigui-1.9.6/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
+-rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-07-28 10:54:44.000000 unigui-1.9.6/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-07-28 10:54:44.000000 unigui-1.9.6/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-07-28 10:54:44.000000 unigui-1.9.6/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-07-28 10:54:44.000000 unigui-1.9.6/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-07-28 10:54:44.000000 unigui-1.9.6/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-07-28 10:54:44.000000 unigui-1.9.6/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-07-28 10:54:44.000000 unigui-1.9.6/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-28 10:58:33.000000 unigui-1.9.6/unigui/web/js/
+-rw-rw-r--   0 george    (1000) george    (1000)  1436034 2023-07-28 10:54:44.000000 unigui-1.9.6/unigui/web/js/vendor.5659ce27.js
+-rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-07-28 10:54:44.000000 unigui-1.9.6/unigui/web/js/430.591e9a73.js
+-rw-rw-r--   0 george    (1000) george    (1000)     5923 2023-07-28 10:54:44.000000 unigui-1.9.6/unigui/web/js/app.349c5f1f.js
+-rw-rw-r--   0 george    (1000) george    (1000)    48933 2023-07-28 10:54:44.000000 unigui-1.9.6/unigui/web/js/652.95b9e70c.js
+-rw-rw-r--   0 george    (1000) george    (1000)      763 2023-07-28 10:54:44.000000 unigui-1.9.6/unigui/web/js/193.283445be.js
+-rw-rw-r--   0 george    (1000) george    (1000)      907 2023-07-28 10:54:44.000000 unigui-1.9.6/unigui/web/index.html
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.9.6/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)      642 2023-07-28 10:58:01.000000 unigui-1.9.6/setup.py
+-rw-rw-r--   0 george    (1000) george    (1000)    18788 2023-07-28 10:58:33.000000 unigui-1.9.6/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-28 10:58:33.000000 unigui-1.9.6/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)    18483 2023-07-28 10:50:01.000000 unigui-1.9.6/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.9.6/MANIFEST.in
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-28 10:58:33.000000 unigui-1.9.6/unigui.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)       63 2023-07-28 10:58:33.000000 unigui-1.9.6/unigui.egg-info/requires.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-28 10:58:33.000000 unigui-1.9.6/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)    18788 2023-07-28 10:58:33.000000 unigui-1.9.6/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.9.6/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)     1258 2023-07-28 10:58:33.000000 unigui-1.9.6/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-28 10:58:33.000000 unigui-1.9.6/unigui.egg-info/top_level.txt
```

### Comparing `unigui-1.9.5/unigui/guielements.py` & `unigui-1.9.6/unigui/guielements.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         if hasattr(self, 'changed'):
             self.changed(self, value)
         else:
             self.value = value
 
 Line = Gui("Line", type = 'line')
 
-def smart_complete(lst, min_input_length = 0, max_output_length = 10):
+def smart_complete(lst, min_input_length = 0, max_output_length = 20):
     di = {it: it.lower() for it in lst}
     def complete(gui, ustr):
         if len(ustr) < min_input_length:
             return []
         ustr = ustr.lower()
         arr = [(itlow.find(ustr), it) for it, itlow in di.items() if itlow.find(ustr) != -1]
         arr.sort(key=lambda e: e[0])
@@ -43,27 +43,29 @@
             self.type =  'autoedit' if 'complete' in kwargs else 'edit'
         if not hasattr(self,'value'):
             self.value = '' if self.type != 'number' else 0
 
 class Text(Gui):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.value = ''
-        self.edit = False
+        self.value = self.name
+        self.type = 'text'        
 
 class Button(Gui):
     def __init__(self, *args, **kwargs):
         self.name = args[0]
-        if len(args) > 1:
-            self.changed = args[1]        
         self.add(kwargs)
+        if not hasattr(self, 'type'):
+            self.type = 'button'
+        if len(args) > 1 and not hasattr(self, 'changed'):
+            self.changed = args[1]        
             
-
-def CameraButton(name, *args):    
-    return Button(name, *args, type = 'camera')
+def CameraButton(name, *args, **kwargs):    
+    kwargs['type'] = 'camera'
+    return Button(name, *args, **kwargs)
         
 def UploadImageButton(name, handler,**kwargs):    
     kwargs['type'] = 'image_uploader'
     if 'width' not in kwargs:
         kwargs['width'] = 250.0              
     if 'height' not in kwargs:
         kwargs['height'] = 300.0         
@@ -109,27 +111,29 @@
         if not hasattr(self, 'nodes'):
             self.nodes = []
         if not hasattr(self, 'edges'):
             self.edges = []
 
 class Switch(Gui):
     def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)        
         if not hasattr(self,'value'):
             self.value = False
-
-list_types = ['toggles','list','dropdown']
+        if not hasattr(self,'type'):
+            self.type = 'switch'
 
 class Select(Gui):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         if not hasattr(self,'options'):             
             self.options = []
         if not hasattr(self,'value'):
             self.value = None
+        if not hasattr(self, 'type'):
+            self.type = 'select' if len(self.options) > 3 else 'radio'        
 
 class Tree(Gui):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)         
         self.type = 'tree' 
         if not hasattr(self,'options'):
             self.options = {}
```

### Comparing `unigui-1.9.5/unigui/server.py` & `unigui-1.9.6/unigui/server.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.5/unigui/tables.py` & `unigui-1.9.6/unigui/tables.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.5/unigui/autotest.py` & `unigui-1.9.6/unigui/autotest.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,16 +83,17 @@
             user_message = message
         else:
             diff = comparator(obj2pyjson(response), message)
             if diff != NO_DIFF:
                 err = diff.get('_message')
                 if not err:
                     for value in diff.values():
-                        err = value['_message']
+                        err = value['_message']                        
                         print(f"\nTest {filename} is failed on message {user_message}!\n {err}\n")
+                error = True
     return not error
 
 test_name = Edit('Name test file', '', focus = True)
 rewrite = Switch('Overwrite existing', False, type = 'check')
 
 def button_clicked(_,__):
     test_name.value = ''
@@ -118,27 +119,29 @@
 
 button = Button('_Add test', button_clicked, 
         icon='data_saver_on', tooltip='Create autotest')
 
 def check_dialog(self):
     errors = []
     child_names = set()   
-    tt = type(self)   
+    
     if not hasattr(self, 'name') or not self.name:            
         errors.append(f"The block with {[str(type(gui)).split('.')[-1] for gui in flatten(self.value)]} does not contain name!")
         self.name = 'Unknown'          
     if not isinstance(self.name, str):
         errors.append(f"The block with name {self.name} is not a string!")
     for child in flatten(self.value):           
         if not isinstance(child, Gui) or not child:
             errors.append(f'The block {self.name} contains invalid element {child} instead of Gui+ object!') 
         elif isinstance(child, Block):
             errors.append(f'The block {self.name} contains block {child.name}. Blocks cannot contain blocks!')                                                                                                       
         elif child.name in child_names:                        
             errors.append(f'The block {self.name} contains a duplicated element name "{child.name}"!')
+        elif child.type == 'linechart' and not hasattr(child, 'view'):
+            errors.append(f'The block {self.name} contains a chart type "{child.name}", but not "view" option!')
         else:
             child_names.add(child.name)                
     return errors
 
 def check_screen(module):
     self = module.screen
     errors =  []
```

### Comparing `unigui-1.9.5/unigui/utils.py` & `unigui-1.9.6/unigui/utils.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.5/unigui/reloader.py` & `unigui-1.9.6/unigui/reloader.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.5/unigui/users.py` & `unigui-1.9.6/unigui/users.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.5/unigui/web/favicon.ico` & `unigui-1.9.6/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.9.5/unigui/web/css/982.c7dd083b.css` & `unigui-1.9.6/unigui/web/css/652.5cfe42ce.css`

 * *Files 16% similar despite different names*

```diff
@@ -1 +1 @@
-thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-thumb-hover:#2176d2;--scrollbar-thumb-dark:#2176d2;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.chart-container[data-v-12be25e8]{height:400px;width:400px}body[data-v-206674a7]{display:flex;justify-content:center}.custom-caption[data-v-206674a7]{padding:5px!important}.web-camera-container[data-v-206674a7]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-206674a7]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-206674a7]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-206674a7]{opacity:1}.web-camera-container .camera-shoot[data-v-206674a7]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-206674a7]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-206674a7]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-206674a7]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-206674a7]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-206674a7]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-206674a7]{animation:preload-206674a7 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-206674a7]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-206674a7]:nth-child(3){animation-delay:.4s}@keyframes preload-206674a7{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.q-tab__label{font-size:16px;font-weight:700}
+thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-thumb-hover:#2176d2;--scrollbar-thumb-dark:#2176d2;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.chart-container[data-v-1e642992]{height:400px;width:400px}body[data-v-a0d1b89e]{display:flex;justify-content:center}.custom-caption[data-v-a0d1b89e]{padding:5px!important}.web-camera-container[data-v-a0d1b89e]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-a0d1b89e]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-a0d1b89e]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-a0d1b89e]{opacity:1}.web-camera-container .camera-shoot[data-v-a0d1b89e]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-a0d1b89e]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-a0d1b89e]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-a0d1b89e]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-a0d1b89e]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-a0d1b89e]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-a0d1b89e]{animation:preload-a0d1b89e 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-a0d1b89e]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-a0d1b89e]:nth-child(3){animation-delay:.4s}@keyframes preload-a0d1b89e{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.q-tab__label{font-size:16px;font-weight:700}
```

### Comparing `unigui-1.9.5/unigui/web/css/vendor.f747ec02.css` & `unigui-1.9.6/unigui/web/css/vendor.f747ec02.css`

 * *Files identical despite different names*

### Comparing `unigui-1.9.5/unigui/web/icons/favicon-96x96.png` & `unigui-1.9.6/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.5/unigui/web/icons/favicon-16x16.png` & `unigui-1.9.6/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.5/unigui/web/icons/favicon-32x32.png` & `unigui-1.9.6/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.5/unigui/web/icons/favicon-128x128.png` & `unigui-1.9.6/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.5/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2` & `unigui-1.9.6/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.9.5/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-1.9.6/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.5/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-1.9.6/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.5/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-1.9.6/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.5/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-1.9.6/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.5/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-1.9.6/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.5/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-1.9.6/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.5/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-1.9.6/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.5/unigui/web/js/vendor.5659ce27.js` & `unigui-1.9.6/unigui/web/js/vendor.5659ce27.js`

 * *Files identical despite different names*

### Comparing `unigui-1.9.5/unigui/web/js/430.591e9a73.js` & `unigui-1.9.6/unigui/web/js/430.591e9a73.js`

 * *Files identical despite different names*

### Comparing `unigui-1.9.5/unigui/web/js/982.872ac96a.js` & `unigui-1.9.6/unigui/web/js/652.95b9e70c.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 "use strict";
 (globalThis["webpackChunkuniqua"] = globalThis["webpackChunkuniqua"] || []).push([
-    [982], {
-        9982: (e, t, a) => {
+    [652], {
+        4652: (e, t, a) => {
             a.r(t), a.d(t, {
                 default: () => sa
             });
             var s = a(3673),
                 l = a(2323);
             const i = (0, s._)("div", {
                     class: "q-pa-md"
@@ -17,31 +17,31 @@
             function o(e, t, a, o, d, r) {
                 const c = (0, s.up)("q-item-label"),
                     h = (0, s.up)("element"),
                     u = (0, s.up)("q-tab"),
                     p = (0, s.up)("q-tabs"),
                     g = (0, s.up)("q-space"),
                     m = (0, s.up)("q-tooltip"),
-                    f = (0, s.up)("q-btn"),
-                    y = (0, s.up)("q-toolbar"),
+                    y = (0, s.up)("q-btn"),
+                    f = (0, s.up)("q-toolbar"),
                     w = (0, s.up)("q-header"),
                     b = (0, s.up)("zone"),
                     k = (0, s.up)("q-page"),
                     v = (0, s.up)("q-page-container"),
                     x = (0, s.up)("q-layout");
                 return (0, s.wg)(), (0, s.j4)(x, {
                     view: "lHh Lpr lFf"
                 }, {
                     default: (0, s.w5)((() => [(0, s.Wm)(w, {
                         elevated: "",
                         class: (0, l.C_)({
                             "bg-deep-purple-9": e.Dark.isActive
                         })
                     }, {
-                        default: (0, s.w5)((() => [(0, s.Wm)(y, null, {
+                        default: (0, s.w5)((() => [(0, s.Wm)(f, null, {
                             default: (0, s.w5)((() => [(0, s.Wm)(c, {
                                 class: "text-h5"
                             }, {
                                 default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(e.screen.header ? e.screen.header : ""), 1)])),
                                 _: 1
                             }), i, ((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e.screen.toolbar, (t => ((0, s.wg)(), (0, s.j4)(h, {
                                 class: (0, l.C_)(["q-ma-xs", {
@@ -74,16 +74,15 @@
                                     class: "justify-center text-white shadow-2",
                                     "no-caps": "",
                                     name: t.name,
                                     label: t.name,
                                     onClick: a => e.tabclick(t.name)
                                 }, null, 8, ["name", "label", "onClick"]))])))), 256))])),
                                 _: 1
-                            }, 8, ["modelValue"]), (0, s.Wm)(g), (0, s.Wm)(f, {
-                                "no-caps": "",
+                            }, 8, ["modelValue"]), (0, s.Wm)(g), (0, s.Wm)(y, {
                                 dense: "",
                                 round: "",
                                 icon: e.Dark.isActive ? "light_mode" : "dark_mode",
                                 onClick: e.switchTheme
                             }, {
                                 default: (0, s.w5)((() => [(0, s.Wm)(m, {
                                     class: "text-body2"
@@ -146,23 +145,23 @@
             var r = a(698),
                 c = a(8603);
             let h = null,
                 u = {};
             var p;
             const g = !1;
             let m = g;
-            const f = ["graph", "docviewer", "linechart", "block"];
-            const y = window.location.host,
-                w = `${window.location.protocol}//${y}`;
+            const y = ["graph", "docviewer", "linechart", "block"];
+            const f = window.location.host,
+                w = `${window.location.protocol}//${f}`;
             let b = {},
                 k = {},
                 v = {};
 
             function C(e) {
-                p = new WebSocket(g ? "ws://localhost:8000/ws" : `ws://${y}/ws`), p.onopen = () => e.statusConnect = !0, p.onmessage = t => {
+                p = new WebSocket(g ? "ws://localhost:8000/ws" : `ws://${f}/ws`), p.onopen = () => e.statusConnect = !0, p.onmessage = t => {
                     m && console.log("incoming message", t.data), h.designCycle = 0, e.processMessage(JSON.parse(t.data))
                 }, p.onerror = t => e.error(t), p.onclose = t => {
                     t.wasClean ? e.info("Connection was finished by the server.") : e.error("Connection suddenly closed!"), e.statusConnect = !1, m && console.info("close code : " + t.code + " reason: " + t.reason)
                 }, h = e
             }
 
             function _(e) {
@@ -222,15 +221,15 @@
                 for (let s of e) s instanceof Array ? t.push(s) : t.push([s]);
                 let a = t.shift();
                 return t.reduce(((e, t) => e.flatMap((e => t.map((t => e instanceof Array ? [...e, t] : [e, t]))))), a)
             }
 
             function V(e = !1) {
                 for (let t of Object.values(k))
-                    if (t.expanding && (!e || f.includes(t.type))) {
+                    if (t.expanding && (!e || y.includes(t.type))) {
                         t.has_recalc = !0;
                         let e = t.$el;
                         if (e.getBoundingClientRect) {
                             let e = t.$el.getBoundingClientRect();
                             window.innerHeight < e.top + e.height && (t.styleSize = "")
                         }
                     }(0, s.Y3)((() => {
@@ -268,19 +267,19 @@
                             }
                         } else if (e.name == t.data.name) {
                         d = t;
                         break
                     }
                     let p = n;
                     p /= o;
-                    let g = e || f.includes(t.type) || t.has_recalc,
+                    let g = e || y.includes(t.type) || t.has_recalc,
                         m = g ? `width:${Math.ceil(c.clientWidth+p)}px` : "",
-                        y = s.startsWith("_scroll@") ? r.inner.clientHeight : c.clientHeight;
-                    y < 0 && (y = 20);
-                    let w = `height: ${y+l}px; ${m}`;
+                        f = s.startsWith("_scroll@") ? r.inner.clientHeight : c.clientHeight;
+                    f < 0 && (f = 20);
+                    let w = `height: ${f+l}px; ${m}`;
                     w != t.styleSize && (t.styleSize = w), t.has_recalc = !1
                 }
             }
 
             function H(e) {
                 const t = h.screen.blocks;
                 let a = window.innerHeight;
@@ -381,15 +380,15 @@
                     let t = Array.isArray(d) ? d[d.length - 1] : d,
                         a = b[t.name].$el.getBoundingClientRect().right;
                     t = Array.isArray(d) ? d[0] : d;
                     let l = b[t.name].$el.getBoundingClientRect().left,
                         i = s - a + l - 10;
                     const r = [];
                     for (let [s, n] of Object.entries(k))
-                        if (n.expanding_width && (n.fullname.startsWith("_scroll@") || e || f.includes(n.type))) {
+                        if (n.expanding_width && (n.fullname.startsWith("_scroll@") || e || y.includes(n.type))) {
                             let e = s.split("@")[1];
                             if (d.find((t => t.name == e))) {
                                 let e = !0,
                                     t = n.geom().left;
                                 for (let [a, s] of r.entries())
                                     if (s !== n && s.geom().left == t) {
                                         s.geom().scrollWidth < n.geom().scrollWidth ? (r[a] = n, o.set(s.fullname, n.fullname)) : o.set(n.fullname, s.fullname), e = !1;
@@ -450,28 +449,28 @@
                         type: String,
                         default: ""
                     }
                 }
             });
             var U = a(4260),
                 N = a(3414),
-                F = a(2035),
-                T = a(4554),
-                P = a(2350),
-                R = a(7518),
-                I = a.n(R);
+                T = a(2035),
+                F = a(4554),
+                R = a(2350),
+                I = a(7518),
+                P = a.n(I);
             const L = (0, U.Z)(O, [
                     ["render", d]
                 ]),
                 B = L;
-            I()(O, "components", {
+            P()(O, "components", {
                 QItem: N.Z,
-                QItemSection: F.Z,
-                QIcon: T.Z,
-                QItemLabel: P.Z
+                QItemSection: T.Z,
+                QIcon: F.Z,
+                QItemLabel: R.Z
             });
             const Y = {
                     key: 0,
                     class: "row q-col-gutter-xs q-py-xs"
                 },
                 X = {
                     class: "q-col-gutter-xs"
@@ -578,41 +577,41 @@
                         data: t,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"]))], 8, se)))), 256))])),
                     _: 1
                 }, 8, ["style"])
             }
             var ne = a(8880);
-            const oe = e => ((0, s.dD)("data-v-206674a7"), e = e(), (0, s.Cn)(), e),
+            const oe = e => ((0, s.dD)("data-v-a0d1b89e"), e = e(), (0, s.Cn)(), e),
                 de = {
                     key: 4,
                     class: "{'bg-blue-grey-9': Dark.isActive}"
                 },
                 re = ["width", "height"],
                 ce = ["src"],
                 he = {
-                    key: 17,
+                    key: 18,
                     class: "web-camera-container"
                 },
                 ue = {
                     class: "camera-button"
                 },
                 pe = {
                     key: 0
                 },
                 ge = {
                     key: 1
                 },
                 me = {
                     class: "camera-loading"
                 },
-                fe = oe((() => (0, s._)("ul", {
+                ye = oe((() => (0, s._)("ul", {
                     class: "loader-circle"
                 }, [(0, s._)("li"), (0, s._)("li"), (0, s._)("li")], -1))),
-                ye = [fe],
+                fe = [ye],
                 we = ["height"],
                 be = ["height"],
                 ke = {
                     key: 1,
                     class: "camera-shoot"
                 },
                 ve = oe((() => (0, s._)("img", {
@@ -629,16 +628,16 @@
                     r = (0, s.up)("q-img"),
                     c = (0, s.up)("q-badge"),
                     h = (0, s.up)("q-select"),
                     u = (0, s.up)("q-checkbox"),
                     p = (0, s.up)("q-toggle"),
                     g = (0, s.up)("q-btn"),
                     m = (0, s.up)("q-btn-toggle"),
-                    f = (0, s.up)("utable"),
-                    y = (0, s.up)("linechart"),
+                    y = (0, s.up)("utable"),
+                    f = (0, s.up)("linechart"),
                     w = (0, s.up)("q-input"),
                     b = (0, s.up)("q-tree"),
                     k = (0, s.up)("q-scroll-area"),
                     v = (0, s.up)("q-separator"),
                     x = (0, s.up)("q-uploader"),
                     C = (0, s.up)("cgraph"),
                     _ = (0, s.up)("q-tooltip"),
@@ -716,20 +715,20 @@
                         "bg-blue-grey-9": e.Dark.isActive
                     }),
                     "no-caps": "",
                     options: e.data.options.map((e => ({
                         label: e,
                         value: e
                     })))
-                }, null, 8, ["modelValue", "class", "options"])])) : "table" == e.type ? ((0, s.wg)(), (0, s.j4)(f, {
+                }, null, 8, ["modelValue", "class", "options"])])) : "table" == e.type ? ((0, s.wg)(), (0, s.j4)(y, {
                     key: 5,
                     data: e.data,
                     pdata: e.pdata,
                     styleSize: e.styleSize
-                }, null, 8, ["data", "pdata", "styleSize"])) : "linechart" == e.type ? ((0, s.wg)(), (0, s.j4)(y, {
+                }, null, 8, ["data", "pdata", "styleSize"])) : "linechart" == e.type ? ((0, s.wg)(), (0, s.j4)(f, {
                     key: 6,
                     data: e.data,
                     pdata: e.pdata,
                     styleSize: e.styleSize
                 }, null, 8, ["data", "pdata", "styleSize"])) : "edit" == e.type ? ((0, s.wg)(), (0, s.j4)(w, {
                     key: 7,
                     modelValue: e.value,
@@ -773,15 +772,15 @@
                     key: 10,
                     style: (0, l.j5)(e.styleSize),
                     "thumb-style": e.thumbStyle,
                     "bar-style": e.barStyle
                 }, {
                     default: (0, s.w5)((() => [(0, s.Wm)(b, {
                         nodes: e.treeNodes,
-                        "selected-color": e.Dark.isActive ? "cyan-12" : "cyan-10",
+                        "selected-color": e.Dark.isActive ? "blue-3" : "indigo",
                         dense: e.data.dense,
                         selected: e.value,
                         "onUpdate:selected": t[8] || (t[8] = t => e.value = t),
                         expanded: e.expandedKeys,
                         "onUpdate:expanded": t[9] || (t[9] = t => e.expandedKeys = t),
                         "node-key": "label",
                         "default-expand-all": ""
@@ -798,63 +797,69 @@
                     type: "textarea",
                     style: (0, l.j5)(e.elemSize)
                 }, null, 6)), [
                     [ne.nr, e.value]
                 ]) : "line" == e.type ? ((0, s.wg)(), (0, s.j4)(v, {
                     key: 12,
                     color: "green"
-                })) : "video" == e.type ? ((0, s.wg)(), (0, s.iD)("video", {
+                })) : "text" == e.type ? ((0, s.wg)(), (0, s.iD)("p", {
+                    key: 13,
+                    class: (0, l.C_)(["q-ma-sm", {
+                        white: e.Dark.isActive,
+                        black: !e.Dark.isActive
+                    }])
+                }, (0, l.zw)(e.value), 3)) : "video" == e.type ? ((0, s.wg)(), (0, s.iD)("video", {
                     width: e.data.width,
                     height: e.data.height,
                     key: e.data.src,
                     controls: ""
                 }, [(0, s._)("source", {
                     src: e.data.src,
                     type: "video/mp4"
                 }, null, 8, ce)], 8, re)) : "uploader" == e.type ? ((0, s.wg)(), (0, s.j4)(x, {
-                    key: 14,
+                    key: 15,
                     label: e.name,
                     "auto-upload": "",
                     thumbnails: "",
                     url: e.host_path,
                     onUploaded: e.updateDom,
                     onAdded: e.onAdded,
                     style: (0, l.j5)(e.elemSize),
                     ref: "uploaderRef",
                     flat: "",
                     class: (0, l.C_)({
                         "bg-grey-9": e.Dark.isActive
                     })
                 }, null, 8, ["label", "url", "onUploaded", "onAdded", "style", "class"])) : "image_uploader" == e.type ? ((0, s.wg)(), (0, s.j4)(x, {
-                    key: 15,
+                    key: 16,
                     label: e.name,
                     "auto-upload": "",
                     thumbnails: "",
                     url: e.host_path,
                     onUploaded: e.updateDom,
                     onAdded: e.onAdded,
                     ref: "uploaderRef",
                     flat: "",
                     class: (0, l.C_)({
                         "bg-grey-10": e.Dark.isActive
                     }),
                     color: e.Dark.isActive ? "purple-10" : "blue"
                 }, null, 8, ["label", "url", "onUploaded", "onAdded", "class", "color"])) : "graph" == e.type ? ((0, s.wg)(), (0, s.j4)(C, {
-                    key: 16,
+                    key: 17,
                     data: e.data,
                     pdata: e.pdata,
                     styleSize: e.elemSize
                 }, null, 8, ["data", "pdata", "styleSize"])) : "camera" == e.type ? ((0, s.wg)(), (0, s.iD)("div", he, [(0, s._)("div", ue, [(0, s._)("button", {
                     class: (0, l.C_)(["button is-rounded", {
                         "is-primary": !e.isCameraOpen,
                         "is-danger": e.isCameraOpen
                     }]),
                     type: "button",
                     onClick: t[11] || (t[11] = (...t) => e.toggleCamera && e.toggleCamera(...t))
-                }, [e.isCameraOpen ? ((0, s.wg)(), (0, s.iD)("span", ge, "Close Camera")) : ((0, s.wg)(), (0, s.iD)("span", pe, "Open Camera"))], 2)]), (0, s.wy)((0, s._)("div", me, ye, 512), [
+                }, [e.isCameraOpen ? ((0, s.wg)(), (0, s.iD)("span", ge, "Close Camera")) : ((0, s.wg)(), (0, s.iD)("span", pe, "Open Camera"))], 2)]), (0, s.wy)((0, s._)("div", me, fe, 512), [
                     [ne.F8, e.isCameraOpen && e.isLoading]
                 ]), e.isCameraOpen ? (0, s.wy)(((0, s.wg)(), (0, s.iD)("div", {
                     key: 0,
                     class: (0, l.C_)(["camera-box", {
                         flash: e.isShotPhoto
                     }])
                 }, [(0, s._)("div", {
@@ -881,15 +886,15 @@
                     class: "button",
                     type: "button",
                     onClick: t[12] || (t[12] = (...t) => e.takePhoto && e.takePhoto(...t))
                 }, xe)])) : (0, s.kq)("", !0), e.isPhotoTaken && e.isCameraOpen ? ((0, s.wg)(), (0, s.iD)("div", Ce, [(0, s.Wm)(g, {
                     onClick: e.downloadImage,
                     label: "Send"
                 }, null, 8, ["onClick"])])) : (0, s.kq)("", !0)])) : "" != e.showname ? ((0, s.wg)(), (0, s.j4)(g, {
-                    key: 18,
+                    key: 19,
                     "no-caps": "",
                     class: (0, l.C_)({
                         "bg-blue-grey-9": e.Dark.isActive
                     }),
                     label: e.name,
                     icon: e.data.icon,
                     onClick: e.sendValue
@@ -899,15 +904,15 @@
                         class: "text-body2"
                     }, {
                         default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(e.data.tooltip), 1)])),
                         _: 1
                     })) : (0, s.kq)("", !0)])),
                     _: 1
                 }, 8, ["class", "label", "icon", "onClick"])) : e.data.mode ? ((0, s.wg)(), (0, s.j4)(g, {
-                    key: 20,
+                    key: 21,
                     "no-caps": "",
                     dense: "",
                     round: "",
                     class: (0, l.C_)({
                         "bg-grey-9": e.Dark.isActive
                     }),
                     onClick: e.sendValue
@@ -919,15 +924,15 @@
                         class: "text-body2"
                     }, {
                         default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(e.data.tooltip), 1)])),
                         _: 1
                     })) : (0, s.kq)("", !0)])),
                     _: 1
                 }, 8, ["class", "onClick"])) : ((0, s.wg)(), (0, s.j4)(g, {
-                    key: 19,
+                    key: 20,
                     "no-caps": "",
                     dense: "",
                     round: "",
                     class: (0, l.C_)({
                         "bg-grey-9": e.Dark.isActive
                     }),
                     icon: e.data.icon,
@@ -956,17 +961,17 @@
                     r = (0, s.up)("q-tooltip"),
                     c = (0, s.up)("q-input"),
                     h = (0, s.up)("q-btn"),
                     u = (0, s.up)("q-th"),
                     p = (0, s.up)("q-tr"),
                     g = (0, s.up)("q-checkbox"),
                     m = (0, s.up)("q-select"),
-                    f = (0, s.up)("q-td"),
-                    y = (0, s.up)("q-table");
-                return (0, s.wg)(), (0, s.j4)(y, {
+                    y = (0, s.up)("q-td"),
+                    f = (0, s.up)("q-table");
+                return (0, s.wg)(), (0, s.j4)(f, {
                     "virtual-scroll": "",
                     dense: e.data.dense,
                     style: (0, l.j5)(e.styleSize),
                     flat: "",
                     filter: e.search,
                     ref: "table",
                     virtualScrollSliceSize: "100",
@@ -1153,15 +1158,15 @@
                         }, 1032, ["class", "props"])))), 128))])),
                         _: 2
                     }, 1032, ["props"])])),
                     body: (0, s.w5)((t => [(0, s.Wm)(p, {
                         props: t,
                         onClick: e => t.selected = !t.selected
                     }, {
-                        default: (0, s.w5)((() => [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e.columns, ((a, i) => ((0, s.wg)(), (0, s.j4)(f, {
+                        default: (0, s.w5)((() => [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e.columns, ((a, i) => ((0, s.wg)(), (0, s.j4)(y, {
                             key: a.name,
                             props: t
                         }, {
                             default: (0, s.w5)((() => ["boolean" == typeof t.row[a.name] ? ((0, s.wg)(), (0, s.j4)(g, {
                                 key: 0,
                                 modelValue: t.row[a.name],
                                 "onUpdate:modelValue": [e => t.row[a.name] = e, s => e.change_switcher(t.row, a.name, i)],
@@ -1429,40 +1434,40 @@
                 He = a(2414),
                 Qe = a(3884),
                 Oe = a(5735),
                 Ue = a(7208);
             const Ne = (0, U.Z)($e, [
                     ["render", Se]
                 ]),
-                Fe = Ne;
-            I()($e, "components", {
+                Te = Ne;
+            P()($e, "components", {
                 QTable: Me.Z,
                 QInput: We.Z,
-                QIcon: T.Z,
+                QIcon: F.Z,
                 QTooltip: Ve.Z,
                 QBtn: Ee.Z,
                 QTr: Ke.Z,
                 QTh: He.Z,
                 QTd: Qe.Z,
                 QCheckbox: Oe.Z,
                 QSelect: Ue.Z
             });
-            const Te = ["nodes", "edges"];
+            const Fe = ["nodes", "edges"];
 
-            function Pe(e, t, a, i, n, o) {
+            function Re(e, t, a, i, n, o) {
                 return (0, s.wg)(), (0, s.iD)("div", {
                     nodes: e.nodes,
                     edges: e.edges,
                     style: (0, l.j5)(e.styleSize),
                     ref: "cy"
-                }, null, 12, Te)
+                }, null, 12, Fe)
             }
-            var Re = a(2393),
-                Ie = a.n(Re);
-            const Le = Ie().stylesheet().selector("node").css({
+            var Ie = a(2393),
+                Pe = a.n(Ie);
+            const Le = Pe().stylesheet().selector("node").css({
                     content: "data(id)",
                     "background-color": "#4286f4",
                     "font-size": "14px"
                 }).selector(".selected").css({
                     "background-color": "#ff5555",
                     "border-color": "#ff5555",
                     "font-size": "14px"
@@ -1523,15 +1528,15 @@
                         }
                     },
                     beforeUnmount() {
                         window.removeEventListener("keydown", this.handleKeyDown), window.removeEventListener("keyup", this.handleKeyUp)
                     },
                     mounted() {
                         window.addEventListener("keydown", this.handleKeyDown), window.addEventListener("keyup", this.handleKeyUp);
-                        let e = Ie()({
+                        let e = Pe()({
                                 container: this.$refs.cy,
                                 elements: {
                                     nodes: this.nodes,
                                     edges: this.edges
                                 },
                                 style: this.style
                             }),
@@ -1679,26 +1684,27 @@
                         },
                         layoutOptions(e) {
                             this.cy.layout(e).run()
                         }
                     }
                 }),
                 Ge = (0, U.Z)(Xe, [
-                    ["render", Pe]
+                    ["render", Re]
                 ]),
                 Je = Ge;
 
             function et(e, t, a, i, n, o) {
                 const d = (0, s.up)("v-chart");
                 return (0, s.wg)(), (0, s.j4)(d, {
                     ref: "chart",
                     option: n.options,
+                    onClick: o.clicked,
                     style: (0, l.j5)(a.styleSize ? a.styleSize : "width: 300px; height: 200px"),
                     autoresize: !0
-                }, null, 8, ["option", "style"])
+                }, null, 8, ["option", "onClick", "style"])
             }
             var tt = a(7559),
                 at = a(4447),
                 st = a(1006),
                 lt = a(3526),
                 it = a(763),
                 nt = a(546),
@@ -1770,21 +1776,15 @@
                                 }],
                                 series: []
                             }
                         }
                     },
                     computed: {},
                     methods: {
-                        clicked(e) {
-                            alert("!");
-                            var t = [e.offsetX, e.offsetY],
-                                a = myChart.convertFromPixel("grid", t),
-                                s = myChart.getModel().get("xAxis")[0].data[a[0]];
-                            console.log(s)
-                        },
+                        clicked(e) {},
                         calcSeries() {
                             this.options.toolbox.feature.mySwitcher = {
                                 show: !0,
                                 title: "Switch view to the table",
                                 icon: "image:M0 2a2 2 0 0 1 2-2h12a2 2 0 0 1 2 2v12a2 2 0 0 1-2 2H2a2 2 0 0 1-2-2V2zm15 2h-4v3h4V4zm0 4h-4v3h4V8zm0 4h-4v3h3a1 1 0 0 0 1-1v-2zm-5 3v-3H6v3h4zm-5 0v-3H1v2a1 1 0 0 0 1 1h3zm-4-4h4V8H1v3zm0-4h4V4H1v3zm5-3v3h4V4H6zm4 4H6v3h4V8z",
                                 onclick: () => {
                                     let e = this.data;
@@ -1797,50 +1797,50 @@
                             let a = e.split("-"),
                                 s = a[1].split(",");
                             s.unshift(a[0]);
                             let l = [];
                             for (let n = 0; n < s.length; n++) s[n] = "i" == s[n] ? -1 : parseInt(s[n]), l.push([]), n && (this.options.series.push({
                                 name: t[s[n]],
                                 type: "line",
-                                symbol: "none",
+                                symbol: "roundRect",
                                 sampling: "lttb",
                                 itemStyle: {
                                     color: ut[n]
                                 },
                                 data: l[n]
                             }), this.options.legend.data.push(t[s[n]]));
                             this.options.xAxis.data = l[0];
                             let i = this.data.rows;
                             for (let n = 0; n < i.length; n++)
                                 for (let e = 0; e < s.length; e++) l[e].push(-1 == s[e] ? n : i[n][s[e]]);
-                            this.$refs.chart.setOption(this.options), this.$refs.chart.chart.on("click", (e => alert("!")))
+                            this.$refs.chart.setOption(this.options)
                         }
                     },
                     mounted() {
                         this.calcSeries()
                     }
                 },
                 gt = (0, U.Z)(pt, [
                     ["render", et],
-                    ["__scopeId", "data-v-12be25e8"]
+                    ["__scopeId", "data-v-1e642992"]
                 ]),
                 mt = gt;
 
-            function ft(e) {
+            function yt(e) {
                 let t = new FormData;
                 t.append("image", e);
                 let a = new XMLHttpRequest;
                 a.open("POST", w, !0), a.onload = function() {
                     200 === this.status ? console.log(this.response) : console.error(a)
                 }, a.send(t)
             }
-            const yt = (0, s.aZ)({
+            const ft = (0, s.aZ)({
                 name: "element",
                 components: {
-                    utable: Fe,
+                    utable: Te,
                     cgraph: Je,
                     linechart: mt
                 },
                 methods: {
                     log(e) {
                         console.log(e)
                     },
@@ -1904,15 +1904,15 @@
                             }), e)
                         }
                         this.isPhotoTaken = !this.isPhotoTaken;
                         const e = this.$refs.canvas.getContext("2d");
                         e.drawImage(this.$refs.camera, 0, 0, 450, 337.5)
                     },
                     downloadImage() {
-                        document.getElementById("downloadPhoto"), document.getElementById("photoTaken").toBlob(ft, "image/jpeg")
+                        document.getElementById("downloadPhoto"), document.getElementById("photoTaken").toBlob(yt, "image/jpeg")
                     },
                     rect() {
                         let e = "clientHeight" in this.$el ? this.$el : this.$el.nextElementSibling;
                         return e.getBoundingClientRect()
                     },
                     geom() {
                         let e = "clientHeight" in this.$el ? this.$el : this.$el.nextElementSibling;
@@ -2005,19 +2005,15 @@
                     selection() {
                         return this.data.selection
                     },
                     icon() {
                         return this.data.icon
                     },
                     type() {
-                        var e = this.data.type;
-                        if (e) return e;
-                        const t = this.data,
-                            a = t.options;
-                        return a ? a.length > 3 ? "select" : "radio" : t.headers ? "table" : (e = typeof this.value, "number" == e || "string" == e ? void 0 !== t.complete ? "autoedit" : "edit" : "boolean" == e ? "switch" : "button")
+                        return this.data.type
                     },
                     treeNodes() {
                         var e = [];
                         if ("list" == this.type) return this.data.options.map((e => ({
                             label: e,
                             children: []
                         })));
@@ -2069,27 +2065,27 @@
                 kt = a(8886),
                 vt = a(8761),
                 xt = a(1232),
                 Ct = a(5551),
                 _t = a(5869),
                 qt = a(1745),
                 At = a(8430);
-            const Dt = (0, U.Z)(yt, [
+            const Dt = (0, U.Z)(ft, [
                     ["render", _e],
-                    ["__scopeId", "data-v-206674a7"]
+                    ["__scopeId", "data-v-a0d1b89e"]
                 ]),
                 St = Dt;
 
             function jt(e) {
                 let t = e.type;
                 return "tree" == t || "table" == t || "list" == t || "docviewer" == t || "graph" == t || "linechart" == t
             }
-            I()(yt, "components", {
+            P()(ft, "components", {
                 QImg: wt.Z,
-                QIcon: T.Z,
+                QIcon: F.Z,
                 QSelect: Ue.Z,
                 QBadge: bt.Z,
                 QCheckbox: Oe.Z,
                 QToggle: kt.Z,
                 QBtn: Ee.Z,
                 QBtnToggle: vt.Z,
                 QInput: We.Z,
@@ -2214,17 +2210,17 @@
                     requestAnimationFrame((() => {
                         requestAnimationFrame((() => {
                             h.visible(!0)
                         }))
                     }))
                 })))
             }
-            I()(zt, "components", {
+            P()(zt, "components", {
                 QCard: Zt.Z,
-                QIcon: T.Z,
+                QIcon: F.Z,
                 QScrollArea: xt.Z
             });
             const Vt = (0, s.aZ)({
                     name: "zone",
                     components: {
                         block: Mt
                     },
@@ -2271,14 +2267,15 @@
                             class: "text-h6"
                         }, {
                             default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(a.data.text ? a.data.text : ""), 1)])),
                             _: 1
                         }), (0, s._)("div", Ht, [(0, s.Wm)(c), ((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(a.buttons, (e => ((0, s.wg)(), (0, s.j4)(h, {
                             class: "col-md-3",
                             label: e,
+                            "no-caps": "",
                             color: a.buttons[0] == e ? "primary" : "secondary",
                             onClick: t => o.sendMessage(e)
                         }, null, 8, ["label", "color", "onClick"])))), 256))])])),
                         _: 1
                     }, 8, ["style"])])),
                     _: 1
                 }, 8, ["onHide", "onKeyup"])
@@ -2314,31 +2311,31 @@
                     onCancelClick() {
                         this.hide()
                     }
                 }
             };
             var Ut = a(5926),
                 Nt = a(2025);
-            const Ft = (0, U.Z)(Ot, [
+            const Tt = (0, U.Z)(Ot, [
                     ["render", Qt]
                 ]),
-                Tt = Ft;
-            I()(Ot, "components", {
+                Ft = Tt;
+            P()(Ot, "components", {
                 QDialog: Ut.Z,
                 QCard: Zt.Z,
-                QItemLabel: P.Z,
+                QItemLabel: R.Z,
                 QSpace: Nt.Z,
                 QBtn: Ee.Z
             });
-            var Pt = a(589);
-            let Rt = "theme";
+            var Rt = a(589);
+            let It = "theme";
             try {
-                ze.Z.set(Pt.Z.getItem(Rt))
+                ze.Z.set(Rt.Z.getItem(It))
             } catch (la) {}
-            let It = null;
+            let Pt = null;
             const Lt = (0, s.aZ)({
                 name: "MainLayout",
                 data() {
                     return {
                         leftDrawerOpen: !1,
                         Dark: ze.Z,
                         menu: [],
@@ -2364,15 +2361,15 @@
                     C(this)
                 },
                 unmounted() {
                     window.removeEventListener("resize", this.onResize)
                 },
                 methods: {
                     switchTheme() {
-                        ze.Z.set(!ze.Z.isActive), Pt.Z.set(Rt, ze.Z.isActive)
+                        ze.Z.set(!ze.Z.isActive), Rt.Z.set(It, ze.Z.isActive)
                     },
                     toggleLeftDrawer() {
                         this.leftDrawerOpen = !this.leftDrawerOpen
                     },
                     tabclick(e) {
                         _(["root", e])
                     },
@@ -2384,15 +2381,15 @@
                     },
                     lens(e) {
                         let t = {
                                 title: "Photo lens",
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0,
-                                component: Tt
+                                component: Ft
                             },
                             {
                                 height: a,
                                 ...s
                             } = e;
                         s.width = 750;
                         let l = {
@@ -2411,25 +2408,25 @@
                         let a = t,
                             s = {
                                 message: e,
                                 type: t,
                                 position: "top",
                                 icon: a
                             };
-                        "progress" == t ? null == It ? (s = {
+                        "progress" == t ? null == Pt ? (s = {
                             group: !1,
                             timeout: 0,
                             spinner: !0,
                             type: "info",
                             message: e || "Progress..",
                             position: "top",
                             color: "secondary"
-                        }, It = this.$q.notify(s)) : null == e ? (It(), It = null) : (s = {
+                        }, Pt = this.$q.notify(s)) : null == e ? (Pt(), Pt = null) : (s = {
                             caption: e
-                        }, It(s)) : ("error" == t && s.type, this.$q.notify(s))
+                        }, Pt(s)) : ("error" == t && s.type, this.$q.notify(s))
                     },
                     error(e) {
                         this.notify(e, "error")
                     },
                     info(e) {
                         this.notify(e, "info")
                     },
@@ -2442,26 +2439,26 @@
                         else if ("dialog" == e.type) {
                             let t = {
                                 title: e.name,
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0
                             };
-                            t.component = Tt, t.componentProps = {
+                            t.component = Ft, t.componentProps = {
                                 data: e.content ? e.content : e,
                                 buttons: e.buttons
                             }, this.$q.dialog(t)
                         } else if ("answer" == e.type) M(e);
                         else {
                             let t = e.updates && e.updates.length;
                             t && $(e.updates);
                             let a = !1;
                             ["error", "progress", "warning", "info"].includes(e.type) && (this.notify(e.value, e.type), a = !0), a || t || (this.error("Invalid data came from the server! Look the console."), console.log(`Invalid data came from the server! ${e}`))
                         }
-                        It && "progress" != e.type && this.notify(null, "progress")
+                        Pt && "progress" != e.type && this.notify(null, "progress")
                     }
                 },
                 mounted() {
                     window.addEventListener("resize", this.onResize);
                     const e = new ResizeObserver((e => {
                         let t = document.documentElement.scrollWidth > window.innerWidth || document.documentElement.scrollHeight > window.innerHeight;
                         t && V(!0)
@@ -2477,20 +2474,20 @@
                 Jt = a(3269),
                 ea = a(2652),
                 ta = a(4379);
             const aa = (0, U.Z)(Lt, [
                     ["render", o]
                 ]),
                 sa = aa;
-            I()(Lt, "components", {
+            P()(Lt, "components", {
                 QLayout: Bt.Z,
                 QHeader: Yt.Z,
                 QToolbar: Xt.Z,
                 QBtn: Ee.Z,
-                QItemLabel: P.Z,
+                QItemLabel: R.Z,
                 QTabs: Gt.Z,
                 QTab: Jt.Z,
                 QSpace: Nt.Z,
                 QTooltip: Ve.Z,
                 QPageContainer: ea.Z,
                 QPage: ta.Z
             })
```

### Comparing `unigui-1.9.5/unigui/web/js/app.6805317c.js` & `unigui-1.9.6/unigui/web/js/app.349c5f1f.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -22,15 +22,15 @@
                         ["render", l]
                     ]),
                     d = c;
                 var p = r(3340),
                     f = r(8339);
                 const h = [{
                         path: "/",
-                        component: () => Promise.all([r.e(736), r.e(982)]).then(r.bind(r, 9982)),
+                        component: () => Promise.all([r.e(736), r.e(652)]).then(r.bind(r, 4652)),
                         children: [{
                             path: "",
                             component: () => Promise.all([r.e(736), r.e(430)]).then(r.bind(r, 6430))
                         }]
                     }, {
                         path: "/:catchAll(.*)*",
                         component: () => Promise.all([r.e(736), r.e(193)]).then(r.bind(r, 2193))
@@ -164,24 +164,24 @@
         }
     })(), (() => {
         r.f = {}, r.e = e => Promise.all(Object.keys(r.f).reduce(((t, o) => (r.f[o](e, t), t)), []))
     })(), (() => {
         r.u = e => "js/" + e + "." + {
             193: "283445be",
             430: "591e9a73",
-            982: "872ac96a"
+            652: "95b9e70c"
         } [e] + ".js"
     })(), (() => {
         r.miniCssF = e => "css/" + ({
             143: "app",
             736: "vendor"
         } [e] || e) + "." + {
             143: "31d6cfe0",
-            736: "f747ec02",
-            982: "c7dd083b"
+            652: "5cfe42ce",
+            736: "f747ec02"
         } [e] + ".css"
     })(), (() => {
         r.g = function() {
             if ("object" === typeof globalThis) return globalThis;
             try {
                 return this || new Function("return this")()
             } catch (e) {
@@ -264,15 +264,15 @@
                 e(o, l, n, a)
             })),
             n = {
                 143: 0
             };
         r.f.miniCss = (e, t) => {
             var r = {
-                982: 1
+                652: 1
             };
             n[e] ? t.push(n[e]) : 0 !== n[e] && r[e] && t.push(n[e] = o(e).then((() => {
                 n[e] = 0
             }), (t => {
                 throw delete n[e], t
             })))
         }
```

### Comparing `unigui-1.9.5/unigui/web/js/193.283445be.js` & `unigui-1.9.6/unigui/web/js/193.283445be.js`

 * *Files identical despite different names*

### Comparing `unigui-1.9.5/unigui/web/index.html` & `unigui-1.9.6/unigui/web/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.5659ce27.js></script><script defer src=js/app.6805317c.js></script><link href=css/vendor.f747ec02.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
+<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.5659ce27.js></script><script defer src=js/app.349c5f1f.js></script><link href=css/vendor.f747ec02.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
```

### Comparing `unigui-1.9.5/LICENSE` & `unigui-1.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.9.5/setup.py` & `unigui-1.9.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
  
 setup(name='unigui',
-      version='1.9.5',      
+      version='1.9.6',      
       license='MIT',
       author='Georgii Dernovyi',
       author_email='g.dernovoy@gmail.com',
       description='Unigui - Universal GUI Framework and protocol',
       packages=find_packages(exclude=['tests']),
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
```

### Comparing `unigui-1.9.5/PKG-INFO` & `unigui-1.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.9.5
+Version: 1.9.6
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -206,19 +206,19 @@
 handler_when_loading_finish(button_, the_loaded_file_filename) where the_loaded_file_filename is a file name in upload server folder. This folder name is defined in config.py .
 
 ### Edit and Text field. ###
 ```
 Edit('Some field', '') #for string value
 Edit('Number field', 0.9, type = 'number') #changed handler will get a number
 ```
-If set edit = false it will be readonly field or text label.
+If set edit = false it will be readonly field.
 ```
 Edit('Some field', '', edit = false) 
-#is equal to
-Text('Some field')
+#text
+Text('Some text')
 ```
 complete handler is optional function which accepts the current edit value and returns a string list for autocomplete.
 
 ```
 def get_complete_list(gui_element, current_value):
     return [s for s in vocab if current_value in s]
```

### Comparing `unigui-1.9.5/README.md` & `unigui-1.9.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -194,19 +194,19 @@
 handler_when_loading_finish(button_, the_loaded_file_filename) where the_loaded_file_filename is a file name in upload server folder. This folder name is defined in config.py .
 
 ### Edit and Text field. ###
 ```
 Edit('Some field', '') #for string value
 Edit('Number field', 0.9, type = 'number') #changed handler will get a number
 ```
-If set edit = false it will be readonly field or text label.
+If set edit = false it will be readonly field.
 ```
 Edit('Some field', '', edit = false) 
-#is equal to
-Text('Some field')
+#text
+Text('Some text')
 ```
 complete handler is optional function which accepts the current edit value and returns a string list for autocomplete.
 
 ```
 def get_complete_list(gui_element, current_value):
     return [s for s in vocab if current_value in s]
```

### Comparing `unigui-1.9.5/unigui.egg-info/PKG-INFO` & `unigui-1.9.6/unigui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.9.5
+Version: 1.9.6
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -206,19 +206,19 @@
 handler_when_loading_finish(button_, the_loaded_file_filename) where the_loaded_file_filename is a file name in upload server folder. This folder name is defined in config.py .
 
 ### Edit and Text field. ###
 ```
 Edit('Some field', '') #for string value
 Edit('Number field', 0.9, type = 'number') #changed handler will get a number
 ```
-If set edit = false it will be readonly field or text label.
+If set edit = false it will be readonly field.
 ```
 Edit('Some field', '', edit = false) 
-#is equal to
-Text('Some field')
+#text
+Text('Some text')
 ```
 complete handler is optional function which accepts the current edit value and returns a string list for autocomplete.
 
 ```
 def get_complete_list(gui_element, current_value):
     return [s for s in vocab if current_value in s]
```

### Comparing `unigui-1.9.5/unigui.egg-info/SOURCES.txt` & `unigui-1.9.6/unigui.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 unigui.egg-info/SOURCES.txt
 unigui.egg-info/dependency_links.txt
 unigui.egg-info/not-zip-safe
 unigui.egg-info/requires.txt
 unigui.egg-info/top_level.txt
 unigui/web/favicon.ico
 unigui/web/index.html
-unigui/web/css/982.c7dd083b.css
+unigui/web/css/652.5cfe42ce.css
 unigui/web/css/app.31d6cfe0.css
 unigui/web/css/vendor.f747ec02.css
 unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
@@ -31,10 +31,10 @@
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
 unigui/web/icons/favicon-128x128.png
 unigui/web/icons/favicon-16x16.png
 unigui/web/icons/favicon-32x32.png
 unigui/web/icons/favicon-96x96.png
 unigui/web/js/193.283445be.js
 unigui/web/js/430.591e9a73.js
-unigui/web/js/982.872ac96a.js
-unigui/web/js/app.6805317c.js
+unigui/web/js/652.95b9e70c.js
+unigui/web/js/app.349c5f1f.js
 unigui/web/js/vendor.5659ce27.js
```

