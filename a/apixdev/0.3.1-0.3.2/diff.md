# Comparing `tmp/apixdev-0.3.1.tar.gz` & `tmp/apixdev-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apixdev-0.3.1.tar", last modified: Mon Jul 24 19:53:44 2023, max compression
+gzip compressed data, was "apixdev-0.3.2.tar", last modified: Thu Jul 27 22:01:48 2023, max compression
```

## Comparing `apixdev-0.3.1.tar` & `apixdev-0.3.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-24 19:53:44.609141 apixdev-0.3.1/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1074 2023-07-23 16:27:29.000000 apixdev-0.3.1/LICENSE
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      662 2023-07-24 19:53:44.609141 apixdev-0.3.1/PKG-INFO
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      864 2023-07-23 16:50:50.000000 apixdev-0.3.1/README.md
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-24 19:53:44.605141 apixdev-0.3.1/apixdev/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       71 2023-07-23 16:27:29.000000 apixdev-0.3.1/apixdev/__init__.py
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-24 19:53:44.609141 apixdev-0.3.1/apixdev/cli/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2022-08-11 15:34:34.000000 apixdev-0.3.1/apixdev/cli/__init__.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      630 2023-07-23 16:32:30.000000 apixdev-0.3.1/apixdev/cli/config.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      287 2023-07-23 16:27:29.000000 apixdev-0.3.1/apixdev/cli/images.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1265 2023-07-24 19:52:26.000000 apixdev-0.3.1/apixdev/cli/main.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     6928 2023-07-24 19:03:21.000000 apixdev-0.3.1/apixdev/cli/project.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      598 2023-07-23 16:27:29.000000 apixdev-0.3.1/apixdev/cli/projects.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      760 2023-07-23 16:27:29.000000 apixdev-0.3.1/apixdev/cli/tools.py
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-24 19:53:44.609141 apixdev-0.3.1/apixdev/core/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2023-07-23 16:27:29.000000 apixdev-0.3.1/apixdev/core/__init__.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      627 2023-07-23 16:27:29.000000 apixdev-0.3.1/apixdev/core/common.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1457 2023-07-24 19:09:56.000000 apixdev-0.3.1/apixdev/core/compose.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     5198 2023-07-24 19:48:50.000000 apixdev-0.3.1/apixdev/core/docker.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      908 2023-07-24 19:31:49.000000 apixdev-0.3.1/apixdev/core/exceptions.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      649 2023-07-23 16:27:29.000000 apixdev-0.3.1/apixdev/core/images.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     2170 2023-07-23 16:27:29.000000 apixdev-0.3.1/apixdev/core/odoo.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     4656 2023-07-24 18:55:18.000000 apixdev-0.3.1/apixdev/core/project.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      561 2023-07-23 16:27:29.000000 apixdev-0.3.1/apixdev/core/projects.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1232 2023-07-23 16:27:29.000000 apixdev-0.3.1/apixdev/core/repository.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     5815 2023-07-24 19:41:43.000000 apixdev-0.3.1/apixdev/core/settings.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     3036 2023-07-24 19:52:26.000000 apixdev-0.3.1/apixdev/core/tools.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1248 2023-07-24 19:52:26.000000 apixdev-0.3.1/apixdev/vars.py
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-24 19:53:44.605141 apixdev-0.3.1/apixdev.egg-info/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      662 2023-07-24 19:53:44.000000 apixdev-0.3.1/apixdev.egg-info/PKG-INFO
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      695 2023-07-24 19:53:44.000000 apixdev-0.3.1/apixdev.egg-info/SOURCES.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        1 2023-07-24 19:53:44.000000 apixdev-0.3.1/apixdev.egg-info/dependency_links.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       46 2023-07-24 19:53:44.000000 apixdev-0.3.1/apixdev.egg-info/entry_points.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      136 2023-07-24 19:53:44.000000 apixdev-0.3.1/apixdev.egg-info/requires.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        8 2023-07-24 19:53:44.000000 apixdev-0.3.1/apixdev.egg-info/top_level.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       38 2023-07-24 19:53:44.609141 apixdev-0.3.1/setup.cfg
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1575 2023-07-24 19:49:56.000000 apixdev-0.3.1/setup.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-27 22:01:48.675858 apixdev-0.3.2/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1074 2023-07-23 16:27:29.000000 apixdev-0.3.2/LICENSE
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      662 2023-07-27 22:01:48.675858 apixdev-0.3.2/PKG-INFO
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      864 2023-07-23 16:50:50.000000 apixdev-0.3.2/README.md
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-27 22:01:48.675858 apixdev-0.3.2/apixdev/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       71 2023-07-23 16:27:29.000000 apixdev-0.3.2/apixdev/__init__.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-27 22:01:48.675858 apixdev-0.3.2/apixdev/cli/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2022-08-11 15:34:34.000000 apixdev-0.3.2/apixdev/cli/__init__.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      630 2023-07-23 16:32:30.000000 apixdev-0.3.2/apixdev/cli/config.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      287 2023-07-23 16:27:29.000000 apixdev-0.3.2/apixdev/cli/images.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1265 2023-07-24 19:52:26.000000 apixdev-0.3.2/apixdev/cli/main.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     6928 2023-07-24 19:03:21.000000 apixdev-0.3.2/apixdev/cli/project.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      598 2023-07-23 16:27:29.000000 apixdev-0.3.2/apixdev/cli/projects.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      760 2023-07-23 16:27:29.000000 apixdev-0.3.2/apixdev/cli/tools.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-27 22:01:48.675858 apixdev-0.3.2/apixdev/core/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2023-07-23 16:27:29.000000 apixdev-0.3.2/apixdev/core/__init__.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      627 2023-07-23 16:27:29.000000 apixdev-0.3.2/apixdev/core/common.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1457 2023-07-24 19:09:56.000000 apixdev-0.3.2/apixdev/core/compose.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     5198 2023-07-24 19:48:50.000000 apixdev-0.3.2/apixdev/core/docker.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      908 2023-07-24 19:31:49.000000 apixdev-0.3.2/apixdev/core/exceptions.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      649 2023-07-23 16:27:29.000000 apixdev-0.3.2/apixdev/core/images.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     2706 2023-07-27 22:01:15.000000 apixdev-0.3.2/apixdev/core/odoo.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     4656 2023-07-24 18:55:18.000000 apixdev-0.3.2/apixdev/core/project.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      561 2023-07-23 16:27:29.000000 apixdev-0.3.2/apixdev/core/projects.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1232 2023-07-23 16:27:29.000000 apixdev-0.3.2/apixdev/core/repository.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     6045 2023-07-27 21:57:47.000000 apixdev-0.3.2/apixdev/core/settings.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     3036 2023-07-24 19:52:26.000000 apixdev-0.3.2/apixdev/core/tools.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1296 2023-07-27 21:52:46.000000 apixdev-0.3.2/apixdev/vars.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-27 22:01:48.675858 apixdev-0.3.2/apixdev.egg-info/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      662 2023-07-27 22:01:48.000000 apixdev-0.3.2/apixdev.egg-info/PKG-INFO
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      695 2023-07-27 22:01:48.000000 apixdev-0.3.2/apixdev.egg-info/SOURCES.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        1 2023-07-27 22:01:48.000000 apixdev-0.3.2/apixdev.egg-info/dependency_links.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       46 2023-07-27 22:01:48.000000 apixdev-0.3.2/apixdev.egg-info/entry_points.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      136 2023-07-27 22:01:48.000000 apixdev-0.3.2/apixdev.egg-info/requires.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        8 2023-07-27 22:01:48.000000 apixdev-0.3.2/apixdev.egg-info/top_level.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       38 2023-07-27 22:01:48.675858 apixdev-0.3.2/setup.cfg
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1575 2023-07-27 21:50:09.000000 apixdev-0.3.2/setup.py
```

### Comparing `apixdev-0.3.1/LICENSE` & `apixdev-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.1/PKG-INFO` & `apixdev-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apixdev
-Version: 0.3.1
+Version: 0.3.2
 Summary: ApiX CLI
 Home-page: https://github.com/apikcloud/apix-cli
 Author: Aurelien ROY
 Author-email: roy.aurelien@gmail.com
 License: MIT
 Keywords: docker odoo development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `apixdev-0.3.1/README.md` & `apixdev-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.1/apixdev/cli/config.py` & `apixdev-0.3.2/apixdev/cli/config.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.1/apixdev/cli/main.py` & `apixdev-0.3.2/apixdev/cli/main.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.1/apixdev/cli/project.py` & `apixdev-0.3.2/apixdev/cli/project.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.1/apixdev/cli/projects.py` & `apixdev-0.3.2/apixdev/cli/projects.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.1/apixdev/cli/tools.py` & `apixdev-0.3.2/apixdev/cli/tools.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.1/apixdev/core/common.py` & `apixdev-0.3.2/apixdev/core/common.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.1/apixdev/core/compose.py` & `apixdev-0.3.2/apixdev/core/compose.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.1/apixdev/core/docker.py` & `apixdev-0.3.2/apixdev/core/docker.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.1/apixdev/core/exceptions.py` & `apixdev-0.3.2/apixdev/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.1/apixdev/core/images.py` & `apixdev-0.3.2/apixdev/core/images.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.1/apixdev/core/project.py` & `apixdev-0.3.2/apixdev/core/project.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.1/apixdev/core/projects.py` & `apixdev-0.3.2/apixdev/core/projects.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.1/apixdev/core/repository.py` & `apixdev-0.3.2/apixdev/core/repository.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.1/apixdev/core/settings.py` & `apixdev-0.3.2/apixdev/core/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,97 +62,103 @@
 
             vals = self._prepare_config()
             vals.update(self._get_default_values())
 
             self.set_vars(vals)
 
         else:
-            _logger.info("Load configuration from {}.".format(self.filepath))
+            _logger.info("Load configuration from %s.", self.filepath)
             self._config.read(self.filepath)
 
     def logout(self):
         values = self._config["apix"]
         self._config["apix"] = {
             k: v for k, v in values.items() if k not in vars.MANDATORY_VALUES
         }
         self.save()
 
     def reload(self):
         self._config = None
         self._load()
 
     def save(self):
-        _logger.info("Save configuration to {}.".format(self.filepath))
+        _logger.info("Save configuration to %s.", self.filepath)
 
         with open(self.filepath, "w") as configfile:
             self._config.write(configfile)
 
     def _get_default_values(self):
         return {
             "apix.port": vars.DEFAULT_PORT,
             "apix.protocol": vars.DEFAULT_PROTOCOL,
             "apix.timeout": vars.DEFAULT_TIMEOUT,
+            "apix.no_verify": vars.DEFAULT_NO_VERIFY,
             "local.default_password": vars.DEFAULT_PASSWORD,
         }
 
     def _prepare_config(self):
         return {
             "apix.url": "",
             "apix.port": "",
             "apix.protocol": "",
             "apix.timeout": "",
+            "apix.no_verify": "",
             "apix.database": "",
             "apix.user": "",
             "apix.password": "",
         }
 
     def split_var(self, key, separator="."):
         section, key = key.split(separator)
         return section, key
 
     def _add_separator(self, items, separator="."):
         return separator.join(items)
 
     def merge_sections(self, vals):
         # [section][key] ==> [section.key]
-        _logger.info("merge sections (before): {}".format(vals))
+        _logger.info("merge sections (before): %s", vals)
         tmp = dict()
         for section in vals.keys():
             tmp.update({self._add_separator([section, k]): v for k, v in vals[section]})
 
-        _logger.info("merge sections: {}".format(tmp))
+        _logger.info("merge sections: %s", tmp)
         return tmp
 
         # {self._add_dot(section, k):v for k,v in vals[section].items()}
 
     def unmerge_sections(self, vals):
         # [section.key] ==> [section][key]
         tmp = dict()
         for k, v in vals.items():
             section, key = self.split_var(k)
             curr = tmp.setdefault(section, dict())
             curr[key] = v
 
-        _logger.info("unmerge_sections: {}".format(tmp))
+        _logger.info("unmerge_sections: %s", tmp)
         return tmp
 
     def set_vars(self, vals):
-        _logger.info("set vars: {}".format(vals))
+        _logger.info("set vars: %s", vals)
         vals = self.unmerge_sections(vals)
         self._config.read_dict(vals)
 
         self.save()
 
     def get_vars(self):
         return {section: self._config[section].items() for section in self._config}
 
     def get_var(self, name):
         section, key = self.split_var(name)
         return self._config.get(section, key)
 
+    def get_boolean(self, name, default=False):
+        section, key = self.split_var(name)
+        return self._config.getboolean(section, key) or default
+
     def get_missing_values(self):
         _logger.error("missing values")
 
         missing_values = dict()
 
         vals = self.get_vars()
         vals = self.merge_sections(vals)
@@ -177,29 +183,32 @@
     @property
     def odoo_options(self):
         return {k: self.get_var("apix.%s" % k) for k in vars.ODOORPC_OPTIONS}
 
     def set_config(self):
         while not self.is_ready:
             vals = dict()
-            for key, value in self.get_missing_values():
+            for key, _ in self.get_missing_values():
                 if "password" in key:
-                    vals[key] = getpass.getpass("{}: ".format(key.capitalize()))
+                    vals[key] = getpass.getpass(f"{key.capitalize()}: ")
                 else:
-                    vals[key] = input("{}: ".format(key.capitalize()))
+                    vals[key] = input(f"{key.capitalize()}: ")
             self.set_vars(vals)
 
     @property
     def is_ready(self):
         return True if len(self.get_missing_values()) == 0 else False
 
     @property
     def workdir(self):
-        # return self._config["local"]["workdir"]
         return self.get_var("local.workdir")
 
     @property
     def env_file(self):
         return os.path.join(self._path, ".env")
 
+    @property
+    def no_verify(self):
+        return self.get_boolean("apix.no_verify", False)
+
 
 settings = Settings(config_dir)
```

### Comparing `apixdev-0.3.1/apixdev/core/tools.py` & `apixdev-0.3.2/apixdev/core/tools.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.1/apixdev/vars.py` & `apixdev-0.3.2/apixdev/vars.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from pathlib import Path
 
-VERSION = "0.3.0"
+VERSION = "0.3.2"
 
 HOME_PATH = Path.home()
 
 CONFIG_PATH = ".config/apix"
 CONFIG_FILE = "config.ini"
 
 DEFAULT_TIMEOUT = 60
@@ -14,21 +14,23 @@
 LOGGING_FILE = "apix.log"
 LOGGING_LEVEL = logging.INFO
 
 DEFAULT_PORT = 443
 DEFAULT_PROTOCOL = "jsonrpc+ssl"
 DEFAULT_TIMEOUT = 6000
 DEFAULT_PASSWORD = "admin"
+DEFAULT_NO_VERIFY = False
 
 MANDATORY_VALUES = [
     "apix.database",
     "apix.url",
     "apix.user",
     "apix.password",
     "apix.token",
+    "apix.no_verify",
     "local.workdir",
     "local.default_password",
     "git.remote_url",
     "git.remote_login",
     "git.remote_token",
     "docker.repository",
 ]
```

### Comparing `apixdev-0.3.1/apixdev.egg-info/PKG-INFO` & `apixdev-0.3.2/apixdev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apixdev
-Version: 0.3.1
+Version: 0.3.2
 Summary: ApiX CLI
 Home-page: https://github.com/apikcloud/apix-cli
 Author: Aurelien ROY
 Author-email: roy.aurelien@gmail.com
 License: MIT
 Keywords: docker odoo development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `apixdev-0.3.1/apixdev.egg-info/SOURCES.txt` & `apixdev-0.3.2/apixdev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.1/setup.py` & `apixdev-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="apixdev",
-    version="0.3.1",
+    version="0.3.2",
     description="ApiX CLI",
     keywords="docker odoo development",
     url="https://github.com/apikcloud/apix-cli",
     author="Aurelien ROY",
     author_email="roy.aurelien@gmail.com",
     license="MIT",
     classifiers=[
```

