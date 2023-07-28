# Comparing `tmp/RSFlib-0.1.3.tar.gz` & `tmp/RSFlib-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RSFlib-0.1.3.tar", last modified: Tue Jul 11 20:00:18 2023, max compression
+gzip compressed data, was "RSFlib-0.1.4.tar", last modified: Fri Jul 28 20:54:47 2023, max compression
```

## Comparing `RSFlib-0.1.3.tar` & `RSFlib-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 radimslovak   (501) staff       (20)        0 2023-07-11 20:00:18.652740 RSFlib-0.1.3/
--rw-r--r--   0 radimslovak   (501) staff       (20)      619 2023-07-11 20:00:18.652620 RSFlib-0.1.3/PKG-INFO
--rw-r--r--   0 radimslovak   (501) staff       (20)       82 2023-06-26 03:03:38.000000 RSFlib-0.1.3/README.md
-drwxr-xr-x   0 radimslovak   (501) staff       (20)        0 2023-07-11 20:00:18.651944 RSFlib-0.1.3/RSFlib/
--rw-r--r--   0 radimslovak   (501) staff       (20)     2192 2023-07-03 17:47:36.000000 RSFlib-0.1.3/RSFlib/CalcFunctions.py
--rw-r--r--   0 radimslovak   (501) staff       (20)      477 2023-07-03 18:52:23.000000 RSFlib-0.1.3/RSFlib/Constants.py
--rw-r--r--   0 radimslovak   (501) staff       (20)     1159 2023-07-11 19:54:14.000000 RSFlib-0.1.3/RSFlib/DataManagement.py
--rw-r--r--   0 radimslovak   (501) staff       (20)     3239 2023-07-11 19:59:08.000000 RSFlib-0.1.3/RSFlib/TkinterExtension.py
--rw-r--r--   0 radimslovak   (501) staff       (20)        0 2023-03-09 22:15:22.000000 RSFlib-0.1.3/RSFlib/__init__.py
-drwxr-xr-x   0 radimslovak   (501) staff       (20)        0 2023-07-11 20:00:18.652421 RSFlib-0.1.3/RSFlib.egg-info/
--rw-r--r--   0 radimslovak   (501) staff       (20)      619 2023-07-11 20:00:18.000000 RSFlib-0.1.3/RSFlib.egg-info/PKG-INFO
--rw-r--r--   0 radimslovak   (501) staff       (20)      253 2023-07-11 20:00:18.000000 RSFlib-0.1.3/RSFlib.egg-info/SOURCES.txt
--rw-r--r--   0 radimslovak   (501) staff       (20)        1 2023-07-11 20:00:18.000000 RSFlib-0.1.3/RSFlib.egg-info/dependency_links.txt
--rw-r--r--   0 radimslovak   (501) staff       (20)        7 2023-07-11 20:00:18.000000 RSFlib-0.1.3/RSFlib.egg-info/top_level.txt
--rw-r--r--   0 radimslovak   (501) staff       (20)       38 2023-07-11 20:00:18.652790 RSFlib-0.1.3/setup.cfg
--rw-r--r--   0 radimslovak   (501) staff       (20)     1068 2023-07-11 19:59:54.000000 RSFlib-0.1.3/setup.py
+drwxr-xr-x   0 radimslovak   (501) staff       (20)        0 2023-07-28 20:54:47.353443 RSFlib-0.1.4/
+-rw-r--r--   0 radimslovak   (501) staff       (20)      617 2023-07-28 20:54:47.353322 RSFlib-0.1.4/PKG-INFO
+-rw-r--r--   0 radimslovak   (501) staff       (20)       82 2023-06-26 03:03:38.000000 RSFlib-0.1.4/README.md
+drwxr-xr-x   0 radimslovak   (501) staff       (20)        0 2023-07-28 20:54:47.352654 RSFlib-0.1.4/RSFlib/
+-rw-r--r--   0 radimslovak   (501) staff       (20)     2192 2023-07-03 17:47:36.000000 RSFlib-0.1.4/RSFlib/CalcFunctions.py
+-rw-r--r--   0 radimslovak   (501) staff       (20)     1676 2023-07-28 20:49:24.000000 RSFlib-0.1.4/RSFlib/ColorSearch.py
+-rw-r--r--   0 radimslovak   (501) staff       (20)      477 2023-07-03 18:52:23.000000 RSFlib-0.1.4/RSFlib/Constants.py
+-rw-r--r--   0 radimslovak   (501) staff       (20)     1163 2023-07-28 20:50:09.000000 RSFlib-0.1.4/RSFlib/DataManagement.py
+-rw-r--r--   0 radimslovak   (501) staff       (20)     4580 2023-07-28 19:16:42.000000 RSFlib-0.1.4/RSFlib/TkinterExtension.py
+-rw-r--r--   0 radimslovak   (501) staff       (20)        0 2023-03-09 22:15:22.000000 RSFlib-0.1.4/RSFlib/__init__.py
+drwxr-xr-x   0 radimslovak   (501) staff       (20)        0 2023-07-28 20:54:47.353134 RSFlib-0.1.4/RSFlib.egg-info/
+-rw-r--r--   0 radimslovak   (501) staff       (20)      617 2023-07-28 20:54:47.000000 RSFlib-0.1.4/RSFlib.egg-info/PKG-INFO
+-rw-r--r--   0 radimslovak   (501) staff       (20)      275 2023-07-28 20:54:47.000000 RSFlib-0.1.4/RSFlib.egg-info/SOURCES.txt
+-rw-r--r--   0 radimslovak   (501) staff       (20)        1 2023-07-28 20:54:47.000000 RSFlib-0.1.4/RSFlib.egg-info/dependency_links.txt
+-rw-r--r--   0 radimslovak   (501) staff       (20)        7 2023-07-28 20:54:47.000000 RSFlib-0.1.4/RSFlib.egg-info/top_level.txt
+-rw-r--r--   0 radimslovak   (501) staff       (20)       38 2023-07-28 20:54:47.353490 RSFlib-0.1.4/setup.cfg
+-rw-r--r--   0 radimslovak   (501) staff       (20)     1066 2023-07-28 20:54:32.000000 RSFlib-0.1.4/setup.py
```

### Comparing `RSFlib-0.1.3/RSFlib/CalcFunctions.py` & `RSFlib-0.1.4/RSFlib/CalcFunctions.py`

 * *Files identical despite different names*

### Comparing `RSFlib-0.1.3/RSFlib/DataManagement.py` & `RSFlib-0.1.4/RSFlib/DataManagement.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-''' Methods for data management '''
+''' Functions for data management '''
 import os
 
 def fileName(path):
-    ''' method that takes path as input and returns unique path if input
+    ''' function that takes path as input and returns unique path if input
     path already exist (prevent data unique data overwrite) '''
     name, suffix = os.path.splitext(path)
     num = ""
     while True:
         new_path = f"{name}{num}{suffix}"
         if not os.path.exists(new_path):
             break
```

### Comparing `RSFlib-0.1.3/RSFlib/TkinterExtension.py` & `RSFlib-0.1.4/RSFlib/TkinterExtension.py`

 * *Files 24% similar despite different names*

```diff
@@ -61,17 +61,17 @@
         self.lock_checkbutton.grid(row=0, column=1)
 
     def update_state(self):
         self.entry.config(state=tk.DISABLED if self.locked.get() == False else tk.NORMAL)
 
 class EntryWithPlaceholder(tk.Entry):
     ''' Entry that has grey text as background. '''
-    def __init__(self, master=None, placeholder="", background=None, width=None):
+    def __init__(self, master=None, text="", background=None, width=None):
         super().__init__(master)
-        self.placeholder = placeholder
+        self.placeholder = text
         self.placeholder_color = "grey"
         self.default_color = self["fg"]
 
         if background:
             self.configure(bg=background)
 
         if width:
@@ -89,8 +89,38 @@
     def on_focus_in(self, event):
         if self.get() == self.placeholder:
             self.delete(0, "end")
             self.config(fg=self.default_color)
 
     def on_focus_out(self, event):
         if not self.get():
-            self.add_placeholder()
+            self.add_placeholder()
+
+class InfoCircleLabel(tk.Label):
+    ''' Label with question mark that show info when cursor hover above it '''
+    def __init__(self, master, info_text):
+        super().__init__(master)
+        self.info_text = info_text
+        self.info_window = None
+        self.create_circle_icon()
+        self.bind("<Enter>", self.show_info)
+        self.bind("<Leave>", self.hide_info)
+
+    def create_circle_icon(self):
+        size = 24  # Adjust the size of the circle
+        self.circle_icon = tk.Canvas(self, width=size, height=size, bg=None, highlightthickness=0)
+        self.circle_icon.create_oval(4, 4, size-4, size-4, outline="gray", width=2)
+        self.circle_icon.create_text(size // 2, size // 2, text="?", fill="gray", font=("Helvetica", 12, "bold"))
+        self.circle_icon.pack()
+
+    def show_info(self, event):
+        if not self.info_window:
+            self.info_window = tk.Toplevel(self.master)
+            self.info_window.wm_overrideredirect(True)
+            self.info_window.wm_geometry("+{}+{}".format(event.x_root, event.y_root))
+            self.info_window_label = tk.Label(self.info_window, text=self.info_text, bg="lightgray")
+            self.info_window_label.pack(ipadx=10, ipady=5)
+
+    def hide_info(self, event):
+        if self.info_window:
+            self.info_window.destroy()
+            self.info_window = None
```

### Comparing `RSFlib-0.1.3/setup.py` & `RSFlib-0.1.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.3'
-DESCRIPTION = 'Useful methods and constants for Fyzing struggle'
+VERSION = '0.1.4'
+DESCRIPTION = 'Useful functions and constants for Fyzing struggle'
 LONG_DESCRIPTION = 'A package that helped me at University - Radim Slovák, VUT.'
 
 # Setting up
 setup(
     name="RSFlib",
     version=VERSION,
     author="Radzym (Radim Slovák)",
@@ -20,15 +20,15 @@
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     install_requires=[],
     keywords=['python', 'data analysis', "physics"],
     classifiers=[
-        "Development Status :: 1 - Planning",
+        "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
 )
```

