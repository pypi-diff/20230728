# Comparing `tmp/CTkTable-0.7.tar.gz` & `tmp/CTkTable-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTkTable-0.7.tar", last modified: Sat Jul  8 13:20:53 2023, max compression
+gzip compressed data, was "CTkTable-0.8.tar", last modified: Fri Jul 28 04:57:36 2023, max compression
```

## Comparing `CTkTable-0.7.tar` & `CTkTable-0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 13:20:53.187162 CTkTable-0.7/
-drwxrwxrwx   0        0        0        0 2023-07-08 13:20:53.161012 CTkTable-0.7/CTkTable/
--rw-rw-rw-   0        0        0      227 2023-07-08 13:07:10.000000 CTkTable-0.7/CTkTable/__init__.py
--rw-rw-rw-   0        0        0    16386 2023-07-08 13:06:29.000000 CTkTable-0.7/CTkTable/ctktable.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:20:53.187162 CTkTable-0.7/CTkTable.egg-info/
--rw-rw-rw-   0        0        0     3960 2023-07-08 13:20:53.000000 CTkTable-0.7/CTkTable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-07-08 13:20:53.000000 CTkTable-0.7/CTkTable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       40 2023-07-08 13:20:53.000000 CTkTable-0.7/CTkTable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-08 13:20:53.000000 CTkTable-0.7/CTkTable.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-08 13:20:53.000000 CTkTable-0.7/CTkTable.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1067 2023-06-21 11:17:36.000000 CTkTable-0.7/LICENSE
--rw-rw-rw-   0        0        0     3960 2023-07-08 13:20:53.187162 CTkTable-0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3363 2023-07-08 13:20:33.000000 CTkTable-0.7/README.md
--rw-rw-rw-   0        0        0      519 2023-07-08 13:20:53.187162 CTkTable-0.7/setup.cfg
--rw-rw-rw-   0        0        0     1036 2023-07-08 13:07:27.000000 CTkTable-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:57:36.101854 CTkTable-0.8/
+drwxrwxrwx   0        0        0        0 2023-07-28 04:57:36.079865 CTkTable-0.8/CTkTable/
+-rw-rw-rw-   0        0        0      227 2023-07-28 04:52:08.000000 CTkTable-0.8/CTkTable/__init__.py
+-rw-rw-rw-   0        0        0    16795 2023-07-28 04:51:08.000000 CTkTable-0.8/CTkTable/ctktable.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:57:36.099854 CTkTable-0.8/CTkTable.egg-info/
+-rw-rw-rw-   0        0        0     4005 2023-07-28 04:57:36.000000 CTkTable-0.8/CTkTable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-07-28 04:57:36.000000 CTkTable-0.8/CTkTable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       40 2023-07-28 04:57:36.000000 CTkTable-0.8/CTkTable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-28 04:57:36.000000 CTkTable-0.8/CTkTable.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-28 04:57:36.000000 CTkTable-0.8/CTkTable.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1067 2023-06-21 11:17:36.000000 CTkTable-0.8/LICENSE
+-rw-rw-rw-   0        0        0     4005 2023-07-28 04:57:36.101854 CTkTable-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3407 2023-07-28 04:57:18.000000 CTkTable-0.8/README.md
+-rw-rw-rw-   0        0        0      519 2023-07-28 04:57:36.103854 CTkTable-0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1036 2023-07-28 04:52:46.000000 CTkTable-0.8/setup.py
```

### Comparing `CTkTable-0.7/CTkTable/ctktable.py` & `CTkTable-0.8/CTkTable/ctktable.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         corner_radius: int = 25,
         write: str = False,
         command = None,
         anchor = "c",
         hover_color = None,
         hover = False,
         justify = "center",
+        wraplength: int = 1000,
         **kwargs):
         
         super().__init__(master, fg_color="transparent")
 
         self.master = master # parent widget
         self.rows = row if row else len(values) # number of default rows
         self.columns = column if column else len(values[0])# number of default columns
@@ -51,14 +52,15 @@
         if self.write:
             border_width = border_width=+1
         if hover_color is not None:
             hover=True
         else:
             hover=False
         self.anchor = anchor
+        self.wraplength = wraplength
         self.hover = hover 
         self.border_width = border_width
         self.hover_color = customtkinter.ThemeManager.theme["CTkButton"]["hover_color"] if hover_color is None else hover_color
         self.orient = orientation
         self.border_color = customtkinter.ThemeManager.theme["CTkButton"]["border_color"] if border_color is None else border_color
         self.text_color = customtkinter.ThemeManager.theme["CTkLabel"]["text_color"] if text_color is None else text_color
         self.font = font
@@ -133,15 +135,15 @@
                         args = copy.deepcopy(kwargs)
                 else:
                     args = copy.deepcopy(kwargs)
                 
                 self.data[i,j] = {"row": i, "column" : j, "value" : value, "args": args}
                 
                 args = self.data[i,j]["args"]
-
+                
                 if "text_color" not in args:
                     args["text_color"] = self.text_color
                 if "border_width" not in args:
                     args["border_width"] = self.border_width
                 if "border_color" not in args:
                     args["border_color"] = self.border_color
                 if "fg_color" not in args:
@@ -171,15 +173,15 @@
                         args["hover"] = self.hover
                     self.frame[i,j] = customtkinter.CTkButton(self, background_corner_colors=corners,
                                                               font=self.font, 
                                                               corner_radius=corner_radius,
                                                               text=value, 
                                                               command=(lambda e=self.data[i,j]: self.command(e)) if self.command else None, **args)
                     self.frame[i,j].grid(column=j, row=i, padx=self.padx, pady=self.pady, sticky="nsew")
-                
+                    self.frame[i,j]._text_label.config(wraplength=self.wraplength)
                 self.rowconfigure(i, weight=1)
                 self.columnconfigure(j, weight=1)
                 
     def manipulate_data(self, row, column):
         """ entry callback """
         self.update_data()
         data = self.data[row,column]
@@ -196,26 +198,30 @@
         self.values = []
         for i in range(self.rows):
             row_data = []
             for j in range(self.columns):
                 row_data.append(self.data[i,j]["value"])
             self.values.append(row_data)
             
-    def edit_row(self, row, **kwargs):
+    def edit_row(self, row, value=None, **kwargs):
         """ edit all parameters of a single row """
         for i in range(self.columns):
             self.frame[row, i].configure(**kwargs)
             self.data[row, i]["args"].update(kwargs)
+            if value:
+                self.insert(row, i, value)
         self.update_data()
         
-    def edit_column(self, column, **kwargs):
+    def edit_column(self, column, value=None, **kwargs):
         """ edit all parameters of a single column """
         for i in range(self.rows):
             self.frame[i, column].configure(**kwargs)
             self.data[i, column]["args"].update(kwargs)
+            if value:
+                self.insert(i, column, value)
         self.update_data()
         
     def update_values(self, values, **kwargs):
         """ update all values at once """
         for i in self.frame.values():
             i.destroy()
         self.frame = {}
@@ -388,15 +394,15 @@
         else:     
             self.frame[row,column].configure(text="", **kwargs)
         if kwargs: self.data[row,column]["args"].update(kwargs)
         self.update_data()
         
     def get(self, row=None, column=None):
         if row and column:
-            return self.data[row,column]["values"]
+            return self.data[row,column]["value"]
         else:
             return self.values
     
     def configure(self, **kwargs):
         """ configure table widget attributes"""
         
         if "colors" in kwargs:
@@ -411,9 +417,11 @@
             self.columns = kwargs.pop("columns")
         if "values" in kwargs:
             self.values = kwargs.pop("values")
         if "padx" in kwargs:
             self.padx = kwargs.pop("padx")
         if "padx" in kwargs:
             self.pady = kwargs.pop("pady")
-        
+        if "wraplength" in kwargs:
+            self.wraplength = kwargs.pop("wraplength")
+            
         self.update_values(self.values, **kwargs)
```

### Comparing `CTkTable-0.7/CTkTable.egg-info/PKG-INFO` & `CTkTable-0.8/CTkTable.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkTable
-Version: 0.7
+Version: 0.8
 Summary: Customtkinter Table widget
 Home-page: https://github.com/Akascape/CTkTable
 Author: Akash Bora
 License: MIT
 Keywords: customtkinter,tkinter,table-widget,table,ctktable,tabular-data,customtkinter-table
 Classifier: License :: OSI Approved :: MIT License 
 Classifier: Programming Language :: Python :: 3
@@ -94,12 +94,13 @@
 | pady | add internal padding in y |
 | colors | set two fg_colors for the table (list), eg: `colors=["yellow", "green"]` |
 | color_phase | set color phase based on rows or columns, eg: `color_phase="vertical"` |
 | orientation | change the orientation of table, `vertical or horizontal` |
 | header_color | define the topmost row color |
 | corner_radius | define the corner roundness of the table |
 | hover_color | enable hover effect on the cells |
+| wraplength | set the width of cell text |
 | **command** | specify a command when a table cell is pressed, [returns row, column, value] |
 | **other button parameters* | all other ctk button parameters can be passed |
 
 Note: This library is at early stage so there can be some performance issues. 
 ### Thanks for visiting! Hope it will help :)
```

### Comparing `CTkTable-0.7/LICENSE` & `CTkTable-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `CTkTable-0.7/PKG-INFO` & `CTkTable-0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkTable
-Version: 0.7
+Version: 0.8
 Summary: Customtkinter Table widget
 Home-page: https://github.com/Akascape/CTkTable
 Author: Akash Bora
 License: MIT
 Keywords: customtkinter,tkinter,table-widget,table,ctktable,tabular-data,customtkinter-table
 Classifier: License :: OSI Approved :: MIT License 
 Classifier: Programming Language :: Python :: 3
@@ -94,12 +94,13 @@
 | pady | add internal padding in y |
 | colors | set two fg_colors for the table (list), eg: `colors=["yellow", "green"]` |
 | color_phase | set color phase based on rows or columns, eg: `color_phase="vertical"` |
 | orientation | change the orientation of table, `vertical or horizontal` |
 | header_color | define the topmost row color |
 | corner_radius | define the corner roundness of the table |
 | hover_color | enable hover effect on the cells |
+| wraplength | set the width of cell text |
 | **command** | specify a command when a table cell is pressed, [returns row, column, value] |
 | **other button parameters* | all other ctk button parameters can be passed |
 
 Note: This library is at early stage so there can be some performance issues. 
 ### Thanks for visiting! Hope it will help :)
```

### Comparing `CTkTable-0.7/README.md` & `CTkTable-0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -79,12 +79,13 @@
 | pady | add internal padding in y |
 | colors | set two fg_colors for the table (list), eg: `colors=["yellow", "green"]` |
 | color_phase | set color phase based on rows or columns, eg: `color_phase="vertical"` |
 | orientation | change the orientation of table, `vertical or horizontal` |
 | header_color | define the topmost row color |
 | corner_radius | define the corner roundness of the table |
 | hover_color | enable hover effect on the cells |
+| wraplength | set the width of cell text |
 | **command** | specify a command when a table cell is pressed, [returns row, column, value] |
 | **other button parameters* | all other ctk button parameters can be passed |
 
 Note: This library is at early stage so there can be some performance issues. 
 ### Thanks for visiting! Hope it will help :)
```

### Comparing `CTkTable-0.7/setup.cfg` & `CTkTable-0.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2043 546b 5461 626c 650d 0a76 6572   = CTkTable..ver
-00000020: 7369 6f6e 203d 2030 2e37 0d0a 6465 7363  sion = 0.7..desc
+00000020: 7369 6f6e 203d 2030 2e38 0d0a 6465 7363  sion = 0.8..desc
 00000030: 7269 7074 696f 6e20 3d20 4375 7374 6f6d  ription = Custom
 00000040: 746b 696e 7465 7220 5461 626c 6520 7769  tkinter Table wi
 00000050: 6467 6574 0d0a 6c6f 6e67 5f64 6573 6372  dget..long_descr
 00000060: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
 00000070: 4541 444d 452e 6d64 0d0a 6c6f 6e67 5f64  EADME.md..long_d
 00000080: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
 00000090: 6e74 5f74 7970 6520 3d20 7465 7874 2f6d  nt_type = text/m
```

### Comparing `CTkTable-0.7/setup.py` & `CTkTable-0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'CTkTable',
-    version = '0.7',
+    version = '0.8',
     description = "Customtkinter Table widget",
     license = "MIT",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akash Bora',
     url = "https://github.com/Akascape/CTkTable",
```

