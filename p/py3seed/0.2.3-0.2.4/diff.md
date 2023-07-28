# Comparing `tmp/py3seed-0.2.3.tar.gz` & `tmp/py3seed-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3seed-0.2.3.tar", last modified: Thu Jul 27 13:12:08 2023, max compression
+gzip compressed data, was "py3seed-0.2.4.tar", last modified: Fri Jul 28 10:36:44 2023, max compression
```

## Comparing `py3seed-0.2.3.tar` & `py3seed-0.2.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-27 13:12:08.582430 py3seed-0.2.3/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.2.3/LICENSE
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-27 13:12:08.582744 py3seed-0.2.3/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.2.3/README.md
--rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.2.3/pyproject.toml
--rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-07-27 13:12:08.583961 py3seed-0.2.3/setup.cfg
--rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.2.3/setup.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-27 13:12:08.546386 py3seed-0.2.3/src/
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-27 13:12:08.566645 py3seed-0.2.3/src/py3seed/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.2.3/src/py3seed/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.2.3/src/py3seed/__main__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.2.3/src/py3seed/admin.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     7571 2023-07-21 09:02:47.000000 py3seed-0.2.3/src/py3seed/cachesupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-27 13:12:08.573471 py3seed-0.2.3/src/py3seed/commands/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.2.3/src/py3seed/commands/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    20578 2023-07-26 12:37:30.000000 py3seed-0.2.3/src/py3seed/commands/gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.2.3/src/py3seed/error.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.2.3/src/py3seed/inflection.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.2.3/src/py3seed/log.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.2.3/src/py3seed/merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    57700 2023-07-18 01:28:13.000000 py3seed-0.2.3/src/py3seed/model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.2.3/src/py3seed/mongosupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14651 2023-07-27 13:10:29.000000 py3seed-0.2.3/src/py3seed/utils.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.2.3/src/py3seed/websupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-27 13:12:08.572022 py3seed-0.2.3/src/py3seed.egg-info/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-27 13:12:08.000000 py3seed-0.2.3/src/py3seed.egg-info/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-07-27 13:12:08.000000 py3seed-0.2.3/src/py3seed.egg-info/SOURCES.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-07-27 13:12:08.000000 py3seed-0.2.3/src/py3seed.egg-info/dependency_links.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-07-27 13:12:08.000000 py3seed-0.2.3/src/py3seed.egg-info/entry_points.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-07-27 13:12:08.000000 py3seed-0.2.3/src/py3seed.egg-info/requires.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-07-27 13:12:08.000000 py3seed-0.2.3/src/py3seed.egg-info/top_level.txt
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-27 13:12:08.581156 py3seed-0.2.3/tests/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     4032 2023-07-21 09:03:11.000000 py3seed-0.2.3/tests/test_cachesupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     6589 2023-07-22 05:05:45.000000 py3seed-0.2.3/tests/test_gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.2.3/tests/test_merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.2.3/tests/test_model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.2.3/tests/test_mongosupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-28 10:36:44.795853 py3seed-0.2.4/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.2.4/LICENSE
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-28 10:36:44.796016 py3seed-0.2.4/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.2.4/README.md
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.2.4/pyproject.toml
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-07-28 10:36:44.796732 py3seed-0.2.4/setup.cfg
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.2.4/setup.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-28 10:36:44.773677 py3seed-0.2.4/src/
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-28 10:36:44.787240 py3seed-0.2.4/src/py3seed/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.2.4/src/py3seed/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.2.4/src/py3seed/__main__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.2.4/src/py3seed/admin.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7571 2023-07-21 09:02:47.000000 py3seed-0.2.4/src/py3seed/cachesupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-28 10:36:44.790856 py3seed-0.2.4/src/py3seed/commands/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.2.4/src/py3seed/commands/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    21243 2023-07-28 10:28:30.000000 py3seed-0.2.4/src/py3seed/commands/gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.2.4/src/py3seed/error.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.2.4/src/py3seed/inflection.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.2.4/src/py3seed/log.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.2.4/src/py3seed/merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    57700 2023-07-18 01:28:13.000000 py3seed-0.2.4/src/py3seed/model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.2.4/src/py3seed/mongosupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14651 2023-07-27 13:10:29.000000 py3seed-0.2.4/src/py3seed/utils.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.2.4/src/py3seed/websupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-28 10:36:44.789708 py3seed-0.2.4/src/py3seed.egg-info/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-28 10:36:44.000000 py3seed-0.2.4/src/py3seed.egg-info/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-07-28 10:36:44.000000 py3seed-0.2.4/src/py3seed.egg-info/SOURCES.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-07-28 10:36:44.000000 py3seed-0.2.4/src/py3seed.egg-info/dependency_links.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-07-28 10:36:44.000000 py3seed-0.2.4/src/py3seed.egg-info/entry_points.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-07-28 10:36:44.000000 py3seed-0.2.4/src/py3seed.egg-info/requires.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-07-28 10:36:44.000000 py3seed-0.2.4/src/py3seed.egg-info/top_level.txt
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-28 10:36:44.795354 py3seed-0.2.4/tests/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     4032 2023-07-21 09:03:11.000000 py3seed-0.2.4/tests/test_cachesupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     6731 2023-07-28 10:31:34.000000 py3seed-0.2.4/tests/test_gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.2.4/tests/test_merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.2.4/tests/test_model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.2.4/tests/test_mongosupport.py
```

### Comparing `py3seed-0.2.3/LICENSE` & `py3seed-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.3/PKG-INFO` & `py3seed-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.2.3
+Version: 0.2.4
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.2.3/setup.cfg` & `py3seed-0.2.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py3seed
-version = 0.2.3
+version = 0.2.4
 author = Samuel Feng
 author_email = okosioc@gmail.com
 description = A package that bootstraps your project by simple data models definition and auto api and user interface generation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/okosioc/pyseed
 project_urls =
```

### Comparing `py3seed-0.2.3/src/py3seed/__init__.py` & `py3seed-0.2.4/src/py3seed/__init__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.3/src/py3seed/__main__.py` & `py3seed-0.2.4/src/py3seed/__main__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.3/src/py3seed/admin.py` & `py3seed-0.2.4/src/py3seed/admin.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.3/src/py3seed/cachesupport.py` & `py3seed-0.2.4/src/py3seed/cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.3/src/py3seed/commands/gen.py` & `py3seed-0.2.4/src/py3seed/commands/gen.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from werkzeug.urls import url_quote, url_encode
 
 from py3seed import registered_models, BaseModel, TemplateError, LayoutError
 from py3seed.utils import work_in, generate_names, get_layout_fields, parse_layout
 from py3seed.merge3 import Merge3
 
 logger = logging.getLogger('pyseed')
+INCLUDES_FOLDER = '__includes'
 
 
 def _prepare_jinja2_env():
     """ Prepare env for rendering jinja2 templates. """
     #
     # For more env setting, please refer to https://jinja.palletsprojects.com/en/3.0.x/api/#jinja2.Environment
     # - trim_blocks=True, the first newline after a block is removed (block, not variable tag!)
@@ -118,18 +119,28 @@
         """ Get layout fields.
 
         each column in layout can be blank('')/hyphen(-)/group(integer&float)/field(string) suffixed with query and format-span string
         this function will return a list of field names.
         """
         return list(get_layout_fields(layout))
 
+    def exists(path):
+        """ Check if path exists. """
+        # Only support FileSystemLoader which has a searchpath
+        if not isinstance(env.loader, FileSystemLoader):
+            return False
+        #
+        fp = os.path.join(env.loader.searchpath[0], path)
+        return os.path.exists(fp)
+
     env.globals['update_query'] = update_query
     env.globals['new_model'] = new_model
     env.globals['match_field'] = match_field
     env.globals['parse_layout_fields'] = parse_layout_fields
+    env.globals['exists'] = exists
     #
     return env
 
 
 def _gen(ds: str = None):
     """ Gen. """
     include_domains = [d.strip() for d in ds.split(',')] if ds else []
@@ -293,22 +304,21 @@
     """ Render output folder/file, handle names having list/varible syntax.
 
     Supported Syntax:
       {{#blueprints}}
       {{blueprint}}
       {{#views}}
       {{view}}
-      {{#seeds}}
-      {{seed}}
       {{#models}}
       {{model}}
     """
     t_path = os.path.join(t_base, name)
     t_name = ''.join(name.split())  # Remove all the whitespace chars from name
     out_names = [t_name]  # if no matched list or varible syntax, process directly
+    logger.debug(f'Render {t_path} -> {out_names}')
     out_key, out_values = None, []
     #
     # Check list syntax, i.e, {{#name}}
     # This syntax iterate over every item of the list; do not generate anything if empty list and false value
     #
     match_list = re.search('(\\{\\{#[a-zA-Z._]+\\}\\})', t_name)
     if match_list:
@@ -318,38 +328,32 @@
             out_key = '__blueprint'
             out_values = context['blueprints']
             out_names = [t_name.replace(syntax, v['name']) for v in out_values]
         elif key == 'views':
             out_key = '__view'
             out_values = context['__blueprint']['views']  # views under current blueprint
             out_names = [t_name.replace(syntax, v['name']) for v in out_values]
-        elif key == 'seeds':
-            out_key = '__seed'
-            # seeds can be accessed at context level, which means it can be used in different views, there is another way to access seed, that is blueprint->view->seed, we often use it generate backend logic
-            # NOTE: do NOT render the seeds having alphanumeric suffix, e.g, Block-read-features-basic, Block-read-shop-products-grid
-            out_values = [s for s in context['seeds'] if not s.get('suffix')]
-            out_names = [t_name.replace(syntax, v['name']) for v in out_values]
         elif key == 'models':
             out_key = '__model'
             # models can be accessed at context level, NOTE: models is dict, {name: {names, schema}}}, so we use values() here
             out_values = list(context['models'].values())
-            # names of blueprints/views/seeds are kebab formats because them will be used in the url directly, while modal names are always in camel case because of PEP8
+            # names of blueprints/views are kebab formats because them will be used in the url directly, while modal names are always in camel case because of PEP8
             out_names = [t_name.replace(syntax, v['name_kebab']) for v in out_values]
         else:
             raise TemplateError(f'Unsupported list syntax: {syntax}')
     else:
         #
         # Check varible syntax, i.e, {{name}}
         # This syntax return the value of the varible
         #
         match_variable = re.search('(\\{\\{[a-zA-Z._]+\\}\\})', t_name)
         if match_variable:
             syntax = match_list.group(1)
             key = syntax[2:-2]
-            if key in ['blueprint', 'view', 'seed']:
+            if key in ['blueprint', 'view']:
                 out_key == f'__{key}'
                 out_values = [context[f'__{key}']]
                 out_names = [t_name.replace(syntax, v['name']) for v in out_values]
             elif key in ['model']:
                 out_key == f'__{key}'
                 out_values = [context[f'__{key}']]
                 out_names = [t_name.replace(syntax, v['name_kebab']) for v in out_values]
@@ -367,46 +371,60 @@
             #     www/templates/public
             #     www/templates/dash
             #     www/templates/demo
             #     ...
             o_path = os.path.join(o_base, o_name)
             if not os.path.exists(o_path):
                 os.mkdir(o_path)
+            # if output is not the same as template, need to copy includes folder
+            t_includes = os.path.join(t_path, INCLUDES_FOLDER)
+            o_includes = os.path.join(o_path, INCLUDES_FOLDER)
+            if t_path != o_path  and os.path.exists(t_includes):
+                logger.debug(f'Copy {t_includes} -> {o_includes}')
+                shutil.copytree(t_includes, o_includes)
             # Can use this context value in sub folders and files
             if out_values:
                 context[out_key] = out_values[i]
             # Render recursively
-            for d in sorted(os.listdir(t_path)):
-                _recursive_render(t_path, o_path, d, context, env)
+            for f in sorted(os.listdir(t_path)):
+                # Only process files
+                if os.path.isfile(os.path.join(t_path, f)):
+                    _recursive_render(t_path, o_path, f, context, env)
+            #
+            if os.path.exists(o_includes):
+                shutil.rmtree(o_includes)
     #
     # Render file
     #
     else:
         # Only process jinja2 files
         if not t_name.endswith('.jinja2'):
             return
         # Overwrite with template file content firstly
         # e.g,
-        #  1. Files that has list or varible syntax, regenerate each time; The jinjas generated should be removed after generation
-        #  www/templates/public/{{#views}}.html.jinja2
+        # 1. Files that has list or varible syntax, regenerate each time; The jinjas generated should be removed after generation
+        #    www/templates/{{#blueprints}}/{{#views}}.html.jinja2
         #    ->
         #    www/templates/public/user-profile.html.jinja2
         #    www/templates/public/team-members.html.jinja2
         #    ...
-        #  2. Files that is just a jinja, no need to overwrite just render directly; The jinja file should NOT be removed after generation
-        #  www/static/js/enums.js.jinja2
+        # 2. Files that is just a jinja, no need to overwrite just render directly; The jinja file should NOT be removed after generation
+        #    www/static/js/enums.js.jinja2
         for o_name in out_names:
             o_path = os.path.join(o_base, o_name)
-            if out_key:  # out_key is not None means it has list or varible syntax
+            # Only two cases
+            # - name has list/var syntax, e.g, www/views/public/{{#views}}.html.jinja2
+            # - name has not list/var syntax but parent folder has, e.g, www/templates/{{#blueprints}}/env.txt.jinja2
+            if t_path != o_path:
+                logger.debug(f'Copy {t_path} to {o_path}')
                 shutil.copyfile(t_path, o_path)
-                shutil.copymode(t_path, o_path)
         # Change working folder to ., so that jinja2 works ok
-        o_base = os.path.abspath(o_base)
-        with work_in(o_base):
-            logger.info(f'Working at {o_base}')
+        abs_o_base = os.path.abspath(o_base)
+        with work_in(abs_o_base):
+            logger.info(f'Working at {abs_o_base}')
             # Set jinja2's path
             env.loader = FileSystemLoader('.')
             o_context = {k: v for k, v in context.items() if not k.startswith('__')}
             #
             for i, o_name in enumerate(out_names):
                 o_file_raw = o_name.replace('.jinja2', '')
                 #
@@ -482,15 +500,15 @@
                         logger.warning(f'Please solve merging conflicts of {o_file_raw}')
                     else:
                         # Rename .111 to .1 for next merging
                         os.rename(o_file_111, o_file_1)
                         # Remove .11
                         os.remove(o_file_11)
                 # Remove template file
-                if out_key:
+                if t_path != os.path.join(o_base, o_name):
                     os.remove(o_name)
 
 
 def main(args: List[str]) -> bool:
     """ Main. """
     parser = argparse.ArgumentParser(prog="pyseed gen")
     parser.add_argument(
```

### Comparing `py3seed-0.2.3/src/py3seed/error.py` & `py3seed-0.2.4/src/py3seed/error.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.3/src/py3seed/inflection.py` & `py3seed-0.2.4/src/py3seed/inflection.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.3/src/py3seed/log.py` & `py3seed-0.2.4/src/py3seed/log.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.3/src/py3seed/merge3.py` & `py3seed-0.2.4/src/py3seed/merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.3/src/py3seed/model.py` & `py3seed-0.2.4/src/py3seed/model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.3/src/py3seed/mongosupport.py` & `py3seed-0.2.4/src/py3seed/mongosupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.3/src/py3seed/utils.py` & `py3seed-0.2.4/src/py3seed/utils.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.3/src/py3seed/websupport.py` & `py3seed-0.2.4/src/py3seed/websupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.3/src/py3seed.egg-info/PKG-INFO` & `py3seed-0.2.4/src/py3seed.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.2.3
+Version: 0.2.4
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.2.3/src/py3seed.egg-info/SOURCES.txt` & `py3seed-0.2.4/src/py3seed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.3/tests/test_cachesupport.py` & `py3seed-0.2.4/tests/test_cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.3/tests/test_gen.py` & `py3seed-0.2.4/tests/test_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,7 +219,10 @@
 //
 
 var global_enums = {
 UserStatus: {'normal': 'Normal', 'rejected': 'Rejected'},
 UserRole: {1: 'Member', 2: 'Editor', 9: 'Admin'},
 }
 '''
+    # global functions
+    env_txt = open('www/templates/public/env.txt', encoding='utf-8').read()
+    assert 'iamhere.html: True' in env_txt
```

### Comparing `py3seed-0.2.3/tests/test_merge3.py` & `py3seed-0.2.4/tests/test_merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.3/tests/test_model.py` & `py3seed-0.2.4/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.3/tests/test_mongosupport.py` & `py3seed-0.2.4/tests/test_mongosupport.py`

 * *Files identical despite different names*

