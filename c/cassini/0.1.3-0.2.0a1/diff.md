# Comparing `tmp/cassini-0.1.3.tar.gz` & `tmp/cassini-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cassini-0.1.3.tar", max compression
+gzip compressed data, was "cassini-0.2.0a1.tar", max compression
```

## Comparing `cassini-0.1.3.tar` & `cassini-0.2.0a1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      250 2020-06-29 20:40:03.744075 cassini-0.1.3/cassini/__init__.py
--rw-r--r--   0        0        0     3905 2020-06-29 20:40:03.745070 cassini-0.1.3/cassini/accessors.py
--rw-r--r--   0        0        0       39 2020-06-29 20:40:03.746080 cassini-0.1.3/cassini/compat/__init__.py
--rw-r--r--   0        0        0     3132 2020-06-29 20:40:03.746080 cassini-0.1.3/cassini/compat/update.py
--rw-r--r--   0        0        0      406 2020-06-29 20:40:03.747065 cassini-0.1.3/cassini/config.py
--rw-r--r--   0        0        0    24224 2021-03-21 16:02:50.862447 cassini-0.1.3/cassini/core.py
--rw-r--r--   0        0        0       82 2020-06-29 20:40:03.749060 cassini-0.1.3/cassini/defaults/__init__.py
--rw-r--r--   0        0        0      940 2020-06-29 20:40:03.750057 cassini-0.1.3/cassini/defaults/templates/Tier.tmplt.ipynb
--rw-r--r--   0        0        0     9080 2021-03-21 16:02:50.868201 cassini-0.1.3/cassini/defaults/tiers.py
--rw-r--r--   0        0        0     8954 2020-06-29 20:40:03.752061 cassini-0.1.3/cassini/environment.py
--rw-r--r--   0        0        0    12841 2020-06-30 11:56:23.589708 cassini-0.1.3/cassini/ipygui.py
--rw-r--r--   0        0        0     2800 2020-06-29 20:40:03.753049 cassini-0.1.3/cassini/magics.py
--rw-r--r--   0        0        0     1581 2020-06-29 20:40:03.754047 cassini-0.1.3/cassini/utils.py
--rw-r--r--   0        0        0      481 2021-03-21 16:04:28.667543 cassini-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      534 2020-06-30 11:56:23.586716 cassini-0.1.3/README.md
--rw-r--r--   0        0        0     1285 2021-03-21 16:06:05.803432 cassini-0.1.3/setup.py
--rw-r--r--   0        0        0     1153 2021-03-21 16:06:05.804430 cassini-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      255 2021-04-07 22:51:55.554459 cassini-0.2.0a1/cassini/__init__.py
+-rw-r--r--   0        0        0     3905 2021-04-07 22:51:43.820271 cassini-0.2.0a1/cassini/accessors.py
+-rw-r--r--   0        0        0       39 2021-04-07 22:51:43.820271 cassini-0.2.0a1/cassini/compat/__init__.py
+-rw-r--r--   0        0        0     3132 2021-04-07 22:51:43.820271 cassini-0.2.0a1/cassini/compat/update.py
+-rw-r--r--   0        0        0      406 2021-04-07 22:51:43.820271 cassini-0.2.0a1/cassini/config.py
+-rw-r--r--   0        0        0    24751 2023-07-28 20:42:20.387018 cassini-0.2.0a1/cassini/core.py
+-rw-r--r--   0        0        0       82 2021-04-07 22:51:43.820271 cassini-0.2.0a1/cassini/defaults/__init__.py
+-rw-r--r--   0        0        0      798 2021-04-07 22:51:55.558420 cassini-0.2.0a1/cassini/defaults/templates/Tier.tmplt.ipynb
+-rw-r--r--   0        0        0     9391 2021-04-07 22:51:55.558420 cassini-0.2.0a1/cassini/defaults/tiers.py
+-rw-r--r--   0        0        0    10146 2021-04-07 22:51:55.562415 cassini-0.2.0a1/cassini/environment.py
+-rw-r--r--   0        0        0    13013 2021-04-07 22:51:55.562415 cassini-0.2.0a1/cassini/ipygui.py
+-rw-r--r--   0        0        0     2800 2021-04-07 22:51:43.824265 cassini-0.2.0a1/cassini/magics.py
+-rw-r--r--   0        0        0     3631 2021-04-07 22:51:55.562415 cassini-0.2.0a1/cassini/utils.py
+-rw-r--r--   0        0        0    35823 2021-04-07 22:51:55.554459 cassini-0.2.0a1/LICENSE.txt
+-rw-r--r--   0        0        0      534 2023-07-28 20:43:38.462312 cassini-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0      922 2021-04-07 22:51:55.554459 cassini-0.2.0a1/README.md
+-rw-r--r--   0        0        0     1677 1970-01-01 00:00:00.000000 cassini-0.2.0a1/PKG-INFO
```

### Comparing `cassini-0.1.3/cassini/accessors.py` & `cassini-0.2.0a1/cassini/accessors.py`

 * *Files identical despite different names*

### Comparing `cassini-0.1.3/cassini/compat/update.py` & `cassini-0.2.0a1/cassini/compat/update.py`

 * *Files identical despite different names*

### Comparing `cassini-0.1.3/cassini/core.py` & `cassini-0.2.0a1/cassini/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from typing import Any, KeysView, List, Type, TypeVar, Tuple, Iterator, Union, Dict, ClassVar, Sequence
 
 import pandas as pd
 
 from .ipygui import BaseTierGui
 from .accessors import MetaAttr, cached_prop, cached_class_prop
-from .utils import FileMaker
+from .utils import FileMaker, open_file
 from .environment import env
 from .config import config
 
 
 class Meta:
     """
     Like a dictionary, except linked to a json file on disk. Caches the value of the json in itself.
@@ -431,14 +431,15 @@
         Returns
         -------
         file : Path
             Defaults to self.parent.folder / (self.name + '.ipynb').
         """
         return self.parent.folder / (self.name + '.ipynb')
 
+
     @cached_prop
     def parent(self) -> Union[TierBase, None]:
         """
         Parent of this `Tier` _instance, `None` if has no parent :'(
         """
         if self.parent_cls:
             return self.parent_cls(*self._identifiers[:-1])
@@ -479,14 +480,32 @@
         Returns
         -------
         child : Type[TierBase]
             child `Tier` object.
         """
         return self.child_cls(*self._identifiers, id)
 
+    def serialize(self):
+        data = dict(self.meta)
+        data['identifiers'] = self.identifiers
+        data['name'] = self.name
+        data['file'] = str(self.file)
+        
+        parents = []
+        parent = self.parent
+        
+        while parent:
+            parents.append(parent)
+            parent = parent.parent
+        
+        data['parents'] = [parent.name for parent in parents][::-1]
+        data['children'] = [child.name for child in self]
+        
+        return data
+
     def children_df(self, * , include: Sequence[str] = None, exclude: Sequence[str] = None) -> Union[pd.DataFrame, None]:
         """
         Build an `UnescapedDataFrame` containing rows from each child of this `Tier`. Columns are inferred from contents
         of meta files.
 
         Parameters
         ----------
@@ -586,15 +605,15 @@
         Notes
         -----
         Only works on Windows machines.
 
         Window is opened via the Jupyter server, not the browser, so if you are not accessing jupyter on localhost then
         the window won't open for you!
         """
-        os.startfile(self.folder)
+        open_file(self.folder)
 
     def get_highlights(self) -> Dict[str, List[Dict[str, Dict[str, Any]]]]:
         """
         Get dictionary of highlights for this `Tier` _instance.
 
         This dictionary is in a form that can be rendered in the notebook using `IPython.display.publish_display_data`
         see Examples.
```

### Comparing `cassini-0.1.3/cassini/defaults/templates/Tier.tmplt.ipynb` & `cassini-0.2.0a1/cassini/defaults/templates/Tier.tmplt.ipynb`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333333%*

 * *Differences: {"'metadata'": "{delete: ['pycharm']}"}*

```diff
@@ -30,21 +30,12 @@
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.7.6"
-        },
-        "pycharm": {
-            "stem_cell": {
-                "cell_type": "raw",
-                "metadata": {
-                    "collapsed": false
-                },
-                "source": []
-            }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `cassini-0.1.3/cassini/defaults/tiers.py` & `cassini-0.2.0a1/cassini/defaults/tiers.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,18 +58,29 @@
     @cached_prop
     def folder(self):
         return env.project.project_folder / (self.child_cls.pretty_type + 's')
 
     @cached_prop
     def file(self) -> Path:
         return env.project.project_folder / f"{self.name}.ipynb"
-
+        
     @cached_prop
     def meta_file(self):
         return None
+    
+    def serialize(self) -> dict:
+        data = {}
+        
+        data['identifiers'] = self.name
+        data['name'] = self.name
+        data['file'] = str(self.file)
+        data['parents'] = []
+        data['children'] = [child.name for child in self]
+        
+        return data
 
     def exists(self):
         return self.folder.exists()
 
     def setup_files(self):
         with FileMaker() as maker:
             print(f"Creating {self.child_cls.pretty_type} folder")
```

### Comparing `cassini-0.1.3/cassini/environment.py` & `cassini-0.2.0a1/cassini/environment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from __future__ import annotations
 
 from pathlib import Path
 from warnings import warn
 import re
+import os
+
+from jupyterlab.labapp import LabApp
 
 from typing import Union, Tuple, List
 
 import jinja2
 
 from .accessors import soft_prop
 from .utils import FileMaker
@@ -50,15 +53,15 @@
         env.project = instance
         return instance
 
     def __init__(self, hierarchy: List['BaseTier'], project_folder: Union[str, Path]):
         self.rank_map = {}
         self.hierarchy = hierarchy
 
-        project_folder = Path(project_folder)
+        project_folder = Path(project_folder).resolve()
         self.project_folder = project_folder if project_folder.is_dir() else project_folder.parent
 
         self.template_env = PathLibEnv(autoescape=jinja2.select_autoescape(['html', 'xml']),
                                        loader=jinja2.FileSystemLoader(self.template_folder))
 
         for rank, tier_cls in enumerate(hierarchy):
             tier_cls.rank = rank
@@ -119,14 +122,18 @@
     @soft_prop
     def template_folder(self):
         """
         Overwritable property providing where templates will be stored for this project.
         """
         return self.project_folder / 'templates'
 
+    @soft_prop
+    def caslib_folder(self) -> Path:
+        return self.project_folder / 'caslib'
+
     def setup_files(self):
         """
         Setup files needed for this project.
 
         Will put everything you need in `project_folder` to get going.
         """
         home = self.home
@@ -148,14 +155,42 @@
                 maker.copy_file(config.BASE_TEMPLATE, self.template_folder / tier_cls.default_template)
                 print("Done")
 
         print(f"Setting up Home Tier")
         home.setup_files()
         print("Success")
 
+    def launch(self, app=None, patch_pythonpath=True):
+        """
+        Jump off point for a cassini project.
+
+        Sets up required files for your project, monkeypatches `PYTHONPATH` to make your project available throughout
+        and launches a jupyterlab server.
+
+        This explicitly associates an instance of the Jupyter server with a particular project.
+
+        Parameters
+        ----------
+        app : LabApp
+            A ready made Jupyter Lab app (By defuault will just create a new one).
+        patch_pythonpath : bool
+            Add `self.project_folder` to the `PYTHONPATH`? (defaults to `True`)
+        """
+        self.setup_files()
+
+        if patch_pythonpath:
+            py_path = os.environ.get('PYTHONPATH', '')
+            project_path = str(self.project_folder.resolve())
+            os.environ['PYTHONPATH'] = py_path + os.pathsep + project_path if py_path else project_path
+
+        if app is None:
+            app = LabApp()
+
+        app.launch_instance()
+
     def parse_name(self, name: str) -> Union[Tuple[str], Tuple]:
         """
         Parses a string that corresponds to a `Tier` and returns a list of its identifiers.
 
         returns an empty tuple if not a valid name.
 
         Parameters
```

### Comparing `cassini-0.1.3/cassini/ipygui.py` & `cassini-0.2.0a1/cassini/ipygui.py`

 * *Files 3% similar despite different names*

```diff
@@ -213,15 +213,15 @@
 
 
 class BaseTierGui:
     """
     Mixin to provide nice notebook outputs for Jupyter Notebooks.
     """
     def __init__(self, tier):
-        self.tier : 'BaseTier' = tier
+        self.tier: 'BaseTier' = tier
 
     def _get_header_components(self) -> Dict[str, Callable[[], DOMWidget]]:
         """
         Creates the dictionary that forms the components of the header.
 
         Returns
         -------
@@ -244,15 +244,15 @@
         if child:
             child_name = child.pretty_type
             components[f'{child_name}s'] = self._build_children
             components[f'New {child_name}'] = self.new_child
 
         return components
 
-    def _build_header_title(self) -> DOMWidget:
+    def _build_header_title(self, *, parent=None) -> DOMWidget:
         """
         Creates a widget that displays the title a `Tier` along side clickable links and buttons to its components
         """
         open_btn = Button(description="Folder")
         open_btn.on_click(lambda cb: self.tier.open_folder())
         title = f'<h1 style="display: inline;"><a href="{self.tier.href}">{self.tier.name}</a></h1>'
         parts = []
@@ -265,24 +265,24 @@
 
         if parts:
             text += f"({'->'.join(parts[::-1])})"
 
         text += '</h3>'
         return VBox((widgetify_html(text), open_btn))
 
-    def _build_description(self) -> DOMWidget:
+    def _build_description(self, *, parent=None) -> Union[DOMWidget, None]:
         """
         Creates a widget that displays the motivation for a `Tier`.
         """
         description = self.tier.description
         if not description:
             return None
         return widgetify(Markdown(description))
 
-    def _build_highlights_accordion(self) -> DOMWidget:
+    def _build_highlights_accordion(self, *, parent=None) -> Union[DOMWidget, None]:
         """
         Creates a widget that displays highlights for this `Tier` in an `ipywidgets.Accordion` - which is nice!
         """
         highlights = self.tier.get_highlights()
 
         if not highlights:
             return None
@@ -295,24 +295,24 @@
             with out:
                 for item in highlight:
                     publish_display_data(**item)
             widget.set_title(i, name)
         widget.selected_index = None
         return widget
 
-    def _build_conclusion(self) -> DOMWidget:
+    def _build_conclusion(self, *, parent=None) -> Union[DOMWidget, None]:
         """
         Build widget to display conclusion of this `Tier` object.
         """
         conclusion = self.tier.conclusion
         if not conclusion:
             return None
         return widgetify(Markdown(self.tier.conclusion))
 
-    def _build_children(self) -> DOMWidget:
+    def _build_children(self, *, parent=None) -> DOMWidget:
         """
         Build a widget to display an `UnescapedDataFrame` containing this `Tier`'s children.
         """
         children_df = self.children_df()
         return widgetify(children_df)
 
     def header(self, *, include: Sequence[str] = None, exclude: Sequence[str] = None) -> DOMWidget:
@@ -358,21 +358,21 @@
 
     def display_highlights(self):
         """
         Display an `ipywidgets.Accordian` with this `Tier`'s highlights.
         """
         return display(self._build_highlights_accordion())
 
-    def children_df(self, * , include: Sequence[str] = None, exclude: Sequence[str] = None) -> Union[UnescapedDataFrame, None]:
+    def children_df(self, *, include: Sequence[str] = None, exclude: Sequence[str] = None) -> Union[UnescapedDataFrame, None]:
         """
         Calls `tier.children_df` but returns an `UnescapedDataFrame` instead.
         """
         return UnescapedDataFrame(self.tier.children_df(include=include, exclude=exclude))
 
-    def new_child(self) -> DOMWidget:
+    def new_child(self, *, parent=None) -> DOMWidget:
         """
         Widget for creating new child for this `Tier`.
         """
         child = self.tier.child_cls
         options = child.get_templates()
 
         mapping = {path.name: path for path in options}
@@ -383,14 +383,15 @@
 
         def create(name, template, description):
             with form.status:
                 obj = child(*self.tier.identifiers, name)
                 obj.setup_files(mapping[template])
                 obj.description = description
                 display(widgetify_html(obj._repr_html_()))
+            parent.update('Children')
 
         form = InputSequence(create,
                              Text(description=f'Identifier', placeholder=f'{child.id_regex}'),
                              selection,
                              Textarea(description='Motivation'))
 
         return form.as_widget()
```

### Comparing `cassini-0.1.3/cassini/magics.py` & `cassini-0.2.0a1/cassini/magics.py`

 * *Files identical despite different names*

