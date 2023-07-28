# Comparing `tmp/bokehlab-0.2.8.tar.gz` & `tmp/bokehlab-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bokehlab-0.2.8.tar", last modified: Mon Mar 13 09:57:28 2023, max compression
+gzip compressed data, was "bokehlab-0.2.9.tar", last modified: Mon Apr  3 04:49:47 2023, max compression
```

## Comparing `bokehlab-0.2.8.tar` & `bokehlab-0.2.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-03-13 09:57:28.532655 bokehlab-0.2.8/
--rw-rw-rw-   0        0        0     1060 2022-05-21 19:39:24.000000 bokehlab-0.2.8/LICENSE
--rw-rw-rw-   0        0        0     7734 2023-03-13 09:57:28.531654 bokehlab-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     6987 2022-08-30 19:23:39.000000 bokehlab-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-13 09:57:28.486654 bokehlab-0.2.8/bokehlab/
--rw-rw-rw-   0        0        0    51870 2023-03-13 09:56:50.000000 bokehlab-0.2.8/bokehlab/__init__.py
--rw-rw-rw-   0        0        0     1900 2023-03-12 18:13:41.000000 bokehlab-0.2.8/bokehlab/bokehlab_magic.py
--rw-rw-rw-   0        0        0     8267 2023-03-12 16:04:33.000000 bokehlab-0.2.8/bokehlab/config.py
--rw-rw-rw-   0        0        0      856 2023-03-09 16:27:15.000000 bokehlab-0.2.8/bokehlab/fix_copy_paste.py
--rw-rw-rw-   0        0        0      295 2023-03-03 18:47:52.000000 bokehlab-0.2.8/bokehlab/install_magic.py
--rw-rw-rw-   0        0        0      272 2023-03-03 18:47:52.000000 bokehlab-0.2.8/bokehlab/palettes.py
--rw-rw-rw-   0        0        0     6942 2022-09-07 02:45:34.000000 bokehlab-0.2.8/bokehlab/parser.py
-drwxrwxrwx   0        0        0        0 2023-03-13 09:57:28.529661 bokehlab-0.2.8/bokehlab.egg-info/
--rw-rw-rw-   0        0        0     7734 2023-03-13 09:57:28.000000 bokehlab-0.2.8/bokehlab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2023-03-13 09:57:28.000000 bokehlab-0.2.8/bokehlab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-13 09:57:28.000000 bokehlab-0.2.8/bokehlab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-05-22 09:46:56.000000 bokehlab-0.2.8/bokehlab.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       47 2023-03-13 09:57:28.000000 bokehlab-0.2.8/bokehlab.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-13 09:57:28.000000 bokehlab-0.2.8/bokehlab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-13 09:57:28.532655 bokehlab-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0      855 2023-03-13 09:56:42.000000 bokehlab-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-03 04:49:47.250916 bokehlab-0.2.9/
+-rw-rw-rw-   0        0        0     1060 2022-05-21 19:39:24.000000 bokehlab-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0     7734 2023-04-03 04:49:47.249912 bokehlab-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6987 2022-08-30 19:23:39.000000 bokehlab-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-03 04:49:47.200006 bokehlab-0.2.9/bokehlab/
+-rw-rw-rw-   0        0        0    52026 2023-04-03 04:49:05.000000 bokehlab-0.2.9/bokehlab/__init__.py
+-rw-rw-rw-   0        0        0     1900 2023-03-12 18:13:41.000000 bokehlab-0.2.9/bokehlab/bokehlab_magic.py
+-rw-rw-rw-   0        0        0     8292 2023-04-03 04:49:05.000000 bokehlab-0.2.9/bokehlab/config.py
+-rw-rw-rw-   0        0        0      856 2023-03-09 16:27:15.000000 bokehlab-0.2.9/bokehlab/fix_copy_paste.py
+-rw-rw-rw-   0        0        0      295 2023-03-03 18:47:52.000000 bokehlab-0.2.9/bokehlab/install_magic.py
+-rw-rw-rw-   0        0        0      272 2023-03-03 18:47:52.000000 bokehlab-0.2.9/bokehlab/palettes.py
+-rw-rw-rw-   0        0        0     6942 2022-09-07 02:45:34.000000 bokehlab-0.2.9/bokehlab/parser.py
+drwxrwxrwx   0        0        0        0 2023-04-03 04:49:47.246919 bokehlab-0.2.9/bokehlab.egg-info/
+-rw-rw-rw-   0        0        0     7734 2023-04-03 04:49:46.000000 bokehlab-0.2.9/bokehlab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2023-04-03 04:49:46.000000 bokehlab-0.2.9/bokehlab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-03 04:49:46.000000 bokehlab-0.2.9/bokehlab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-05-22 09:46:56.000000 bokehlab-0.2.9/bokehlab.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       68 2023-04-03 04:49:46.000000 bokehlab-0.2.9/bokehlab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-03 04:49:46.000000 bokehlab-0.2.9/bokehlab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-03 04:49:47.250916 bokehlab-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      879 2023-04-03 04:49:05.000000 bokehlab-0.2.9/setup.py
```

### Comparing `bokehlab-0.2.8/LICENSE` & `bokehlab-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bokehlab-0.2.8/PKG-INFO` & `bokehlab-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bokehlab
-Version: 0.2.8
+Version: 0.2.9
 Summary: Interactive plotting with familiar syntax in Jupyter notebooks.
 Home-page: https://github.com/axil/bokehlab
 Author: Lev Maximov
 Author-email: lev.maximov@gmail.com
 License: MIT License
 Keywords: bokeh,jupyter,notebook,plot,interactive
 Platform: UNKNOWN
```

### Comparing `bokehlab-0.2.8/README.md` & `bokehlab-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `bokehlab-0.2.8/bokehlab/__init__.py` & `bokehlab-0.2.9/bokehlab/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 #    class torch:
 #        class Tensor:
 #            pass
 
 import matplotlib       # for imshow palette
 import matplotlib.cm as cm
 
-__version__ = '0.2.8'
+__version__ = '0.2.9'
 
 SIZING_METHOD = 'policies'        # or 'sizing_mode'
 
 DEBUG_RESOURCES = False
 DEBUG_OUTPUT = False
 
 def load(resources=None):
@@ -598,15 +598,15 @@
 LINE_STYLES = ['-', '--', ':', '-.']
 
 def collect_figure_options(kw):
     res = {}
     for k in ('width', 'height', 'width_policy', 'height_policy', 'sizing_mode',
               'background_fill_color', 'x_range', 'y_range',
               'x_axis_location', 'y_axis_location', 
-              'title', 'title_location', 'legend_location', 'grid',
+              'title', 'title_location', 'legend_location', 'legend_loc', 'grid',
               'toolbar_location', 'toolbar_loc', 'flip_x_range', 'flip_y_range',
               'legend_title'):
         if k in kw:
             res[k] = kw.pop(k)
     return res
 
 def _plot(*args, x=None, y=None, style=None, color=None, label=None, line_width=None, alpha=None,
@@ -651,14 +651,15 @@
             elif mode == 'loglog':
                 figure_opts['x_axis_type'] = figure_opts['y_axis_type'] = 'log'
             if is_dt:
                 if 'x_axis_type' in figure_opts and figure_opts['x_axis_type'] is not None:
                     raise ValueError('datetime x values is incompatible with "%s"' % mode)
                 else:
                     figure_opts['x_axis_type'] = 'datetime'
+            expand_aliases(figure_opts)
             p = Figure(**figure_opts)
             if not (get_p or get_ps):
                 if wrap:
                     FIGURES.append((p, 'wrap'))
                 else:
                     FIGURES.append(p)
             figure_created = True
@@ -782,25 +783,25 @@
                 if marker_style in ANGLES:
                     kw['angle'] = ANGLES[marker_style]
                 p.triangle(x='x', y='y', source=source, **kw)
         sources.append(source)
 
     if isinstance(hline, (int, float, np.number)):
         hline = [hline]
-    if isinstance(hline, (list, tuple)):
+    if isinstance(hline, (list, tuple)) or isinstance(hline, np.ndarray) and hline.ndim==1:
         for y in hline:
             span = Span(location=y, dimension='width', line_color=hline_color, 
                         line_width=1, level='overlay')
             p.renderers.append(span)
     elif hline is not None:
         raise TypeError(f'Unsupported type of hline: {type(hline)}')
 
     if isinstance(vline, (int, float, np.number)):
         vline = [vline]
-    if isinstance(vline, (list, tuple)):
+    if isinstance(vline, (list, tuple)) or isinstance(vline, np.ndarray) and vline.ndim==1:
         for x in vline:
             span = Span(location=x, dimension='height', line_color=vline_color, 
                         line_width=1, level='overlay')
             p.renderers.append(span)
     elif vline is not None:
         raise TypeError(f'Unsupported type of vline: {type(vline)}')
```

### Comparing `bokehlab-0.2.8/bokehlab/bokehlab_magic.py` & `bokehlab-0.2.9/bokehlab/bokehlab_magic.py`

 * *Files identical despite different names*

### Comparing `bokehlab-0.2.8/bokehlab/config.py` & `bokehlab-0.2.9/bokehlab/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,14 @@
                         config[section][key] = v
                 else:
                     print(f'Unknown section: {section}. Available sections: {CONFIG_SECTIONS}')
         else:
             print(f'Unknown key: {k}')
 
 def read_config():
-    from bokehlab import CONFIG_DIR, CONFIG_FILE
     if not CONFIG_DIR.exists():
         CONFIG_DIR.mkdir()
     if CONFIG_FILE.exists():
         on_disk = yaml.load(CONFIG_FILE.open().read(), yaml.SafeLoader)
     else:
         on_disk = {}
     return on_disk
@@ -155,25 +154,29 @@
                     print("Available output modes: 'notebook', 'file'. For 'file' mode you can specify filename by setting output.file")
                     break
                 elif part == 'resources.mode':
                     print('Available resource modes: ' + ', '.join(f'"{m}"' for m in RESOURCE_MODES))
                     break
             else:
                 print(textwrap.dedent(configure.__doc__.strip('\n')))
+        if '-g' in parts or '--global' in parts:
+            _global = True
+            print(f'Editing global settings in {CONFIG_FILE}')
+        else:
+            _global = False
         if '--clear' in parts:
             if '--force' in parts or input('Are you sure you want to delete the configuration file (y/n)? ') == 'y':
                 os.unlink(CONFIG_FILE)
                 print('Config file deleted')
         elif '-d' in parts or '--delete' in parts:
             _global = False
             keys = []
             for part in parts:
                 if part in ('-g', '--global'):
-                    _global = True
-                    print(f'Editing global settings in {CONFIG_FILE}')
+                    pass
                 elif part in ('-d', '--delete'):
                     pass
                 else:
                     if '.' in part:
                         section, key = part.split('.', 1)
                         if section in CONFIG:
                             if key in CONFIG[section]:
@@ -200,15 +203,14 @@
                             if not on_disk[section]:
                                 del on_disk[section]
                     else:
                         on_disk.pop(part, None)
                 CONFIG_FILE.open('w').write(yaml.dump(on_disk))
                 print('Settings saved')
         else:
-            _global = False
             config = defaultdict(dict)   # items to save to global config
             parse_config_line(parts, CONFIG, config)
             if _global:
                 on_disk = read_config()
                 for k, v in config.items():
                     if k in on_disk and isinstance(v, dict):
                         for kk, vv in v.items():
```

### Comparing `bokehlab-0.2.8/bokehlab/fix_copy_paste.py` & `bokehlab-0.2.9/bokehlab/fix_copy_paste.py`

 * *Files identical despite different names*

### Comparing `bokehlab-0.2.8/bokehlab/parser.py` & `bokehlab-0.2.9/bokehlab/parser.py`

 * *Files identical despite different names*

### Comparing `bokehlab-0.2.8/bokehlab.egg-info/PKG-INFO` & `bokehlab-0.2.9/bokehlab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bokehlab
-Version: 0.2.8
+Version: 0.2.9
 Summary: Interactive plotting with familiar syntax in Jupyter notebooks.
 Home-page: https://github.com/axil/bokehlab
 Author: Lev Maximov
 Author-email: lev.maximov@gmail.com
 License: MIT License
 Keywords: bokeh,jupyter,notebook,plot,interactive
 Platform: UNKNOWN
```

### Comparing `bokehlab-0.2.8/setup.py` & `bokehlab-0.2.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="bokehlab",
-    version="0.2.8",
+    version="0.2.9",
     author='Lev Maximov',
     author_email='lev.maximov@gmail.com',
     url='https://github.com/axil/bokehlab',
     description="Interactive plotting with familiar syntax in Jupyter notebooks.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=['bokeh<3', 'matplotlib', 'pyyaml', 'jupyter_bokeh', 'pandas'],
+    install_requires=['bokeh<3', 'jupyter-bokeh<=3.0.4', 'matplotlib', 'pyyaml', 'jupyter_bokeh', 'pandas'],
     packages=['bokehlab'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     license="MIT License",
```

