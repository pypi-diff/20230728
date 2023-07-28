# Comparing `tmp/meson_vs_gen-0.3.0.tar.gz` & `tmp/meson_vs_gen-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meson_vs_gen-0.3.0.tar", max compression
+gzip compressed data, was "meson_vs_gen-0.4.0.tar", max compression
```

## Comparing `meson_vs_gen-0.3.0.tar` & `meson_vs_gen-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1067 2023-07-26 20:11:03.322478 meson_vs_gen-0.3.0/LICENSE
--rw-r--r--   0        0        0     9649 2023-07-26 20:11:03.322478 meson_vs_gen-0.3.0/README.md
--rw-r--r--   0        0        0     1440 2023-07-26 20:11:03.323479 meson_vs_gen-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-26 20:11:03.348478 meson_vs_gen-0.3.0/vsgen/__init__.py
--rw-r--r--   0        0        0       71 2023-07-26 20:11:03.323479 meson_vs_gen-0.3.0/vsgen/__main__.py
--rw-r--r--   0        0        0     4344 2023-07-26 20:11:03.323479 meson_vs_gen-0.3.0/vsgen/api.py
--rw-r--r--   0        0        0      440 2023-07-26 20:11:03.323479 meson_vs_gen-0.3.0/vsgen/cli/__init__.py
--rw-r--r--   0        0        0     2380 2023-07-26 20:11:03.323479 meson_vs_gen-0.3.0/vsgen/cli/_pathconfig.py
--rw-r--r--   0        0        0     1573 2023-07-26 20:11:03.323479 meson_vs_gen-0.3.0/vsgen/cli/generate.py
--rw-r--r--   0        0        0     1221 2023-07-26 20:11:03.323479 meson_vs_gen-0.3.0/vsgen/cli/project.py
--rw-r--r--   0        0        0     2776 2023-07-26 20:11:03.323479 meson_vs_gen-0.3.0/vsgen/cli/solution.py
--rw-r--r--   0        0        0    10959 2023-07-26 20:11:03.324478 meson_vs_gen-0.3.0/vsgen/configfile.py
--rw-r--r--   0        0        0     1043 2023-07-26 20:11:03.324478 meson_vs_gen-0.3.0/vsgen/configuration.py
--rw-r--r--   0        0        0     8818 2023-07-26 20:11:03.324478 meson_vs_gen-0.3.0/vsgen/introspector.py
--rw-r--r--   0        0        0     3358 2023-07-26 20:11:03.324478 meson_vs_gen-0.3.0/vsgen/runsettings.py
--rw-r--r--   0        0        0     7261 2023-07-26 20:11:03.324478 meson_vs_gen-0.3.0/vsgen/sln.py
--rw-r--r--   0        0        0    12465 2023-07-26 20:11:03.324478 meson_vs_gen-0.3.0/vsgen/vcxproj.py
--rw-r--r--   0        0        0    10837 1970-01-01 00:00:00.000000 meson_vs_gen-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-28 19:28:02.800743 meson_vs_gen-0.4.0/LICENSE
+-rw-r--r--   0        0        0     9649 2023-07-28 19:28:02.800743 meson_vs_gen-0.4.0/README.md
+-rw-r--r--   0        0        0     1440 2023-07-28 19:28:02.800743 meson_vs_gen-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-28 19:28:02.824743 meson_vs_gen-0.4.0/vsgen/__init__.py
+-rw-r--r--   0        0        0       71 2023-07-28 19:28:02.801744 meson_vs_gen-0.4.0/vsgen/__main__.py
+-rw-r--r--   0        0        0     4350 2023-07-28 19:28:02.801744 meson_vs_gen-0.4.0/vsgen/api.py
+-rw-r--r--   0        0        0      440 2023-07-28 19:28:02.801744 meson_vs_gen-0.4.0/vsgen/cli/__init__.py
+-rw-r--r--   0        0        0     2380 2023-07-28 19:28:02.801744 meson_vs_gen-0.4.0/vsgen/cli/_pathconfig.py
+-rw-r--r--   0        0        0     1573 2023-07-28 19:28:02.801744 meson_vs_gen-0.4.0/vsgen/cli/generate.py
+-rw-r--r--   0        0        0     1221 2023-07-28 19:28:02.801744 meson_vs_gen-0.4.0/vsgen/cli/project.py
+-rw-r--r--   0        0        0     2776 2023-07-28 19:28:02.801744 meson_vs_gen-0.4.0/vsgen/cli/solution.py
+-rw-r--r--   0        0        0    10959 2023-07-28 19:28:02.801744 meson_vs_gen-0.4.0/vsgen/configfile.py
+-rw-r--r--   0        0        0     1043 2023-07-28 19:28:02.801744 meson_vs_gen-0.4.0/vsgen/configuration.py
+-rw-r--r--   0        0        0     8818 2023-07-28 19:28:02.801744 meson_vs_gen-0.4.0/vsgen/introspector.py
+-rw-r--r--   0        0        0     3358 2023-07-28 19:28:02.801744 meson_vs_gen-0.4.0/vsgen/runsettings.py
+-rw-r--r--   0        0        0     7261 2023-07-28 19:28:02.801744 meson_vs_gen-0.4.0/vsgen/sln.py
+-rw-r--r--   0        0        0    12398 2023-07-28 19:28:02.801744 meson_vs_gen-0.4.0/vsgen/vcxproj.py
+-rw-r--r--   0        0        0    10837 1970-01-01 00:00:00.000000 meson_vs_gen-0.4.0/PKG-INFO
```

### Comparing `meson_vs_gen-0.3.0/LICENSE` & `meson_vs_gen-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meson_vs_gen-0.3.0/README.md` & `meson_vs_gen-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `meson_vs_gen-0.3.0/pyproject.toml` & `meson_vs_gen-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "meson-vs-gen"
-version = "0.3.0"
+version = "0.4.0"
 description = "Generates Visual Studio solutions and projects for meson projects"
 authors = ["Charles Brunet <charles.brunet@optelgroup.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://gitlab.com/optelgroup-public/meson-vs-gen"
 keywords = ["visualstudio", "meson"]
 classifiers = [
```

### Comparing `meson_vs_gen-0.3.0/vsgen/api.py` & `meson_vs_gen-0.4.0/vsgen/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         if subdir is True:
             project_path /= name
         elif subdir:
             project_path /= subdir
 
         vcxproj = VcxProj(name, project_path)
         if update:
-            vcxproj.load_configs()
+            vcxproj.load(required=False)
         else:
             vcxproj.remove_user_file()
 
         vcxproj.add_config(self.config)
 
         if target:
             if target is True:
```

### Comparing `meson_vs_gen-0.3.0/vsgen/cli/_pathconfig.py` & `meson_vs_gen-0.4.0/vsgen/cli/_pathconfig.py`

 * *Files identical despite different names*

### Comparing `meson_vs_gen-0.3.0/vsgen/cli/generate.py` & `meson_vs_gen-0.4.0/vsgen/cli/generate.py`

 * *Files identical despite different names*

### Comparing `meson_vs_gen-0.3.0/vsgen/cli/project.py` & `meson_vs_gen-0.4.0/vsgen/cli/project.py`

 * *Files identical despite different names*

### Comparing `meson_vs_gen-0.3.0/vsgen/cli/solution.py` & `meson_vs_gen-0.4.0/vsgen/cli/solution.py`

 * *Files identical despite different names*

### Comparing `meson_vs_gen-0.3.0/vsgen/configfile.py` & `meson_vs_gen-0.4.0/vsgen/configfile.py`

 * *Files identical despite different names*

### Comparing `meson_vs_gen-0.3.0/vsgen/configuration.py` & `meson_vs_gen-0.4.0/vsgen/configuration.py`

 * *Files identical despite different names*

### Comparing `meson_vs_gen-0.3.0/vsgen/introspector.py` & `meson_vs_gen-0.4.0/vsgen/introspector.py`

 * *Files identical despite different names*

### Comparing `meson_vs_gen-0.3.0/vsgen/runsettings.py` & `meson_vs_gen-0.4.0/vsgen/runsettings.py`

 * *Files identical despite different names*

### Comparing `meson_vs_gen-0.3.0/vsgen/sln.py` & `meson_vs_gen-0.4.0/vsgen/sln.py`

 * *Files identical despite different names*

### Comparing `meson_vs_gen-0.3.0/vsgen/vcxproj.py` & `meson_vs_gen-0.4.0/vsgen/vcxproj.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,21 +37,14 @@
     def filterspath(self) -> Path:
         return self.path / (self.name + self.FILTER_EXT)
 
     @property
     def userpath(self) -> Path:
         return self.path / (self.name + self.USER_EXT)
 
-    def load_configs(self) -> None:
-        if not self.filepath.exists():
-            return
-
-        project_xml = ET.parse(self.filepath).getroot()
-        self._load_configs(project_xml)
-
     def _load_configs(self, project_xml: ET.Element):
         self.uuid = project_xml.find(f'.//{{{self.NS}}}ProjectGuid').text
 
         for config_node in project_xml.iterfind(f'.//{{{self.NS}}}ProjectConfiguration'):
             config = config_node.findtext(f"{{{self.NS}}}Configuration")
             arch = config_node.findtext(f"{{{self.NS}}}Platform")
 
@@ -95,19 +88,22 @@
                 build_cmd = self._read_opt_node(config_node, 'NMakeBuildCommandLine', '')
                 m = re.fullmatch(r'ninja -C (\S+) (\S+)', build_cmd)
                 params.output = m[2] if m else None
 
     def _load_files(self, project_xml: ET.Element):
         for filetype in ("ClCompile", "ClInclude", "None"):
             for file_node in project_xml.iterfind(f'.//{{{self.NS}}}{filetype}'):
-                self._files[Path(file_node.get("Include"))] = filetype
+                self._files[Path(self.filepath.parent, file_node.get("Include")).resolve()] = filetype
 
-    def load(self):
+    def load(self, required=True) -> None:
         if not self.filepath.exists():
-            raise FileNotFoundError(f'{self.filepath} does not exist')
+            if required:
+                raise FileNotFoundError(f'{self.filepath} does not exist')
+            else:
+                return
 
         project_xml = ET.parse(self.filepath).getroot()
         self._load_configs(project_xml)
         self._load_files(project_xml)
 
     def _read_opt_node(self, parent: ET.Element, name: str, default: Optional[str] = None) -> str | None:
         node = parent.find(f'{{{self.NS}}}{name}')
```

### Comparing `meson_vs_gen-0.3.0/PKG-INFO` & `meson_vs_gen-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meson-vs-gen
-Version: 0.3.0
+Version: 0.4.0
 Summary: Generates Visual Studio solutions and projects for meson projects
 Home-page: https://gitlab.com/optelgroup-public/meson-vs-gen
 License: MIT
 Keywords: visualstudio,meson
 Author: Charles Brunet
 Author-email: charles.brunet@optelgroup.com
 Requires-Python: >=3.9,<4.0
```

