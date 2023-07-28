# Comparing `tmp/agora_config-1.0.9-py2.py3-none-any.whl.zip` & `tmp/agora_config-1.1.30-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 8647 bytes, number of entries: 13
--rw-r--r--  2.0 fat      105 b- defN 23-Feb-13 17:19 agora_config/__init__.py
--rw-r--r--  2.0 fat     5279 b- defN 23-Mar-16 09:13 agora_config/agora_config.py
--rw-r--r--  2.0 fat      549 b- defN 23-Jan-29 10:17 agora_config/command_line_provider.py
--rw-r--r--  2.0 fat     2771 b- defN 23-Jan-29 13:29 agora_config/dict_of_dict.py
--rw-r--r--  2.0 fat      407 b- defN 23-Jan-29 10:17 agora_config/environment_variable_provider.py
--rw-r--r--  2.0 fat     3689 b- defN 23-Jan-29 13:35 agora_config/events.py
--rw-r--r--  2.0 fat     3438 b- defN 23-Jan-30 13:00 agora_config/file_key_provider.py
--rw-r--r--  2.0 fat     1927 b- defN 23-Jan-30 13:00 agora_config/file_provider.py
--rw-r--r--  2.0 fat       24 b- defN 23-Mar-16 20:19 agora_config/version.py
--rw-r--r--  2.0 fat      139 b- defN 23-Mar-07 09:10 agora_config-1.0.9.dist-info/LICENSE
-?rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_config-1.0.9.dist-info/WHEEL
-?rw-r--r--  2.0 fat      756 b- defN 16-Jan-01 00:00 agora_config-1.0.9.dist-info/METADATA
-?rw-r--r--  2.0 fat     1089 b- defN 16-Jan-01 00:00 agora_config-1.0.9.dist-info/RECORD
-13 files, 20272 bytes uncompressed, 6815 bytes compressed:  66.4%
+Zip file size: 8009 bytes, number of entries: 13
+-rw-r--r--  2.0 fat      105 b- defN 23-May-12 13:38 agora_config/__init__.py
+-rw-r--r--  2.0 fat     5994 b- defN 23-Jun-30 14:21 agora_config/agora_config.py
+-rw-r--r--  2.0 fat      540 b- defN 23-May-12 13:38 agora_config/command_line_provider.py
+-rw-r--r--  2.0 fat     2283 b- defN 23-May-12 13:38 agora_config/dict_of_dict.py
+-rw-r--r--  2.0 fat      410 b- defN 23-May-12 13:38 agora_config/environment_variable_provider.py
+-rw-r--r--  2.0 fat     3164 b- defN 23-May-12 13:38 agora_config/file_key_provider.py
+-rw-r--r--  2.0 fat     1974 b- defN 23-May-18 11:05 agora_config/file_provider.py
+-rw-r--r--  2.0 fat      550 b- defN 23-May-12 13:38 agora_config/last_value_callbacks.py
+-rw-r--r--  2.0 fat       25 b- defN 23-Jul-28 11:19 agora_config/version.py
+-rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_config-1.1.30.dist-info/LICENSE
+-rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_config-1.1.30.dist-info/WHEEL
+-rw-r--r--  2.0 fat     1847 b- defN 16-Jan-01 00:00 agora_config-1.1.30.dist-info/METADATA
+-rw-r--r--  2.0 fat     1107 b- defN 16-Jan-01 00:00 agora_config-1.1.30.dist-info/RECORD
+13 files, 18232 bytes uncompressed, 6141 bytes compressed:  66.3%
```

## zipnote {}

```diff
@@ -9,32 +9,32 @@
 
 Filename: agora_config/dict_of_dict.py
 Comment: 
 
 Filename: agora_config/environment_variable_provider.py
 Comment: 
 
-Filename: agora_config/events.py
-Comment: 
-
 Filename: agora_config/file_key_provider.py
 Comment: 
 
 Filename: agora_config/file_provider.py
 Comment: 
 
+Filename: agora_config/last_value_callbacks.py
+Comment: 
+
 Filename: agora_config/version.py
 Comment: 
 
-Filename: agora_config-1.0.9.dist-info/LICENSE
+Filename: agora_config-1.1.30.dist-info/LICENSE
 Comment: 
 
-Filename: agora_config-1.0.9.dist-info/WHEEL
+Filename: agora_config-1.1.30.dist-info/WHEEL
 Comment: 
 
-Filename: agora_config-1.0.9.dist-info/METADATA
+Filename: agora_config-1.1.30.dist-info/METADATA
 Comment: 
 
-Filename: agora_config-1.0.9.dist-info/RECORD
+Filename: agora_config-1.1.30.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## agora_config/agora_config.py

```diff
@@ -1,150 +1,177 @@
-
 import threading
 import time
 import sys
 import traceback
+import os
 from inspect import currentframe, getframeinfo
-from concurrent.futures import ThreadPoolExecutor
 from agora_logging import logger
-from .events import Events
 from .file_provider import FileProvider
 from .command_line_provider import CommandLineProvider
 from .environment_variable_provider import EnvironmentVariableProvider
 from .file_key_provider import FileKeyProvider
 from .dict_of_dict import DictOfDict
+from .last_value_callbacks import LastValueCallbacks
+
 
 class ConfigSingleton(DictOfDict):
     _instance = None
 
     def __new__(cls, *args, **kwargs):
         if not cls._instance:
             cls._instance = super().__new__(cls, *args, **kwargs)
         return cls._instance
 
+    def get_main_module_name(self):
+        main_module_spec = sys.argv[0]
+        if main_module_spec is None:
+            return '__main__'
+        else:
+            return main_module_spec
+
     def __init__(self):
         super().__init__()
-        self.events = Events()
+        self.overrides = DictOfDict()
+        self.defaults = DictOfDict()
+        self.callbacks = []
+        self.setting_callbacks = {}
+
+        if "IOTEDGE_MODULEID" in os.environ:
+            self.defaults["Name"] = os.getenv("IOTEDGE_MODULEID")
+        else:
+            self.defaults["Name"] = self.get_main_module_name()
+
+        if "IOTEDGE_DEVICEID" in os.environ:
+            self.defaults["GATEWAY_ID"] = os.getenv("IOTEDGE_DEVICEID")
+        else:
+            self.defaults["GATEWAY_ID"] = "UNKNOWN"
+            
+        if "GROUP_ID" in os.environ:
+            self.defaults["GROUP_ID"] = os.getenv("GROUP_ID")
+        else:
+            self.defaults["GROUP_ID"] = "UNKNOWN"  
 
-        config_defaults["Name"] = __name__
-        config_defaults["DEVICE_ID"] = "UNKNOWN"
-        config_defaults["GROUP_ID"] = "UNKNOWN"
-        config_defaults["GATEWAY_ID"] = "UNKNOWN"
-        
         self.primary_config = FileProvider("AEA.json")
         self.evp = EnvironmentVariableProvider()
-        self.clp = CommandLineProvider()        
+        self.clp = CommandLineProvider()
         self.alt_config = FileProvider("config/AEA.json")
         self.fkp = FileKeyProvider()
 
         self.build()
         self.__start_monitoring()  # start monitoring the providers
 
-    def observe(self,event_string:str,callback):
+    def observe(self, setting: str, callback):
         """
         Creates an observable setting and returns the current value
         """
-        self.events.add_event(event_string,callback)
-        return super().__getitem__(event_string)
-    
-    
-    def observe_config(self,fn):
-        self.events.add_event('##',fn)
-    
-              
+        if setting not in self.setting_callbacks:
+            if setting in self:
+                self.setting_callbacks[setting] = LastValueCallbacks(
+                    super().__getitem__(setting))
+            else:
+                self.setting_callbacks[setting] = LastValueCallbacks("")
+        self.setting_callbacks[setting].append(callback)
+
+    def stop_observing(self, setting: str, callback):
+        if setting in self.setting_callbacks:
+            self.setting_callbacks[setting].remove(callback)
+
+    def observe_config(self, fn):
+        self.callbacks.append(fn)
+
+    def stop_observing_conf(self, fn):
+        if fn in self.callbacks:
+            self.callbacks.remove(fn)
+
     def build(self):
-        print("rebuilding config")
+        # print("rebuilding config")
         super().clear()
-        print (f"build this 0: {super().get_dict()}")
-        print (f"  add defaults: {config_defaults.get_dict()}")
-        if isinstance(config_defaults, DictOfDict):
-            super().merge(config_defaults.get_dict())
-        print (f"build this 1: {super().get_dict()}")
-        print (f"  add primary: {self.primary_config.get_dict()}")
+        # print (f"build this 0: {super()}")
+        # print (f"  add defaults: {config_defaults}")
+        if isinstance(self.defaults, DictOfDict):
+            super().merge(self.defaults)
+        # print (f"build this 1: {super()}")
+        # print (f"  add primary: {self.primary_config}")
         self.primary_config.check_for_updates()
-        super().merge(self.primary_config.get_dict())        
-        print (f"build this 2: {super().get_dict()}")
-        print (f"  add environ: {self.evp.get_dict()}")
-        super().merge(self.evp.get_dict())
-        print (f"build this 3: {super().get_dict()}")
-        print (f"  add commandline: {self.clp.get_dict()}")
-        super().merge(self.clp.get_dict())
-        print (f"build this 4: {super().get_dict()}")
-        print (f"  add alt: {self.alt_config.get_dict()}")
+        super().merge(self.primary_config)
+        # print (f"build this 2: {super()}")
+        # print (f"  add environ: {self.evp}")
+        super().merge(self.evp)
+        # print (f"build this 3: {super()}")
+        # print (f"  add commandline: {self.clp}")
+        super().merge(self.clp)
+        # print (f"build this 4: {super()}")
+        # print (f"  add alt: {self.alt_config}")
         self.alt_config.check_for_updates()
-        super().merge(self.alt_config.get_dict())
-        print (f"build this 5: {super().get_dict()}")
-        print (f"  add fkp: {self.fkp.get_dict()}")
+        super().merge(self.alt_config)
+        # print (f"build this 5: {super()}")
+        # print (f"  add fkp: {self.fkp}")
         self.fkp.check_for_updates()
-        super().merge(self.fkp.get_dict())
-        print (f"build this 6: {super().get_dict()}")
-        print (f"  add overrides: {config_overrides.get_dict()}")
-        if isinstance(config_overrides, DictOfDict):
-            super().merge(config_overrides.get_dict())
-        print (f"final       : {super().get_dict()}")
+        super().merge(self.fkp)
+        # print (f"build this 6: {super()}")
+        # print (f"  add overrides: {config_overrides}")
+        if isinstance(self.overrides, DictOfDict):
+            super().merge(self.overrides)
+        # print (f"final       : {super()}")
         self.__dispatch()
 
-
-    # below are the methods which watch for updates to the AEA.config.json
-
-
     def __dispatch(self):
-        """
-        Dispatch all the callbacks with a threadpool
-        """
-        for event,data in self.events.get_events_to_trigger(self.get_dict()):
-            for subs in self.events.get_event_subs(event):
-                with ThreadPoolExecutor(5) as executor:
-                    handle = executor.submit(subs,data)
-                    if exception := handle.exception():
-                        logger.error(f"""failed to dispatch event for {str(subs)} for event {event}""")
-                        logger.error(str(exception))
-
+        for callback in self.callbacks:
+            callback()
+        for key, value in self.setting_callbacks.items():
+            # print(f"checking key {key}")
+            # print(super())
+            if self.__getitem__(key) != "":
+                # print(f"key in super_dict{key}")
+                value.update(self.__getitem__(key))
+            elif value.last_value != "":
+                value.update("")
 
     def __listen_for_changes(self):
-        while( self.should_run == True \
-              and threading.main_thread().is_alive()):
+        while (self.should_run == True
+               and threading.main_thread().is_alive()):
             time.sleep(1)
-            if ( self.primary_config.check_for_updates() or
-                 self.alt_config.check_for_updates() or
-                 self.fkp.check_for_updates()):
+            if (self.primary_config.check_for_updates() or
+                self.alt_config.check_for_updates() or
+                    self.fkp.check_for_updates()):
                 self.build()
-        
 
     def __start_monitoring(self):
         self.should_run = True
         t = threading.Thread(target=self.__listen_for_changes)
         t.start()
 
-
     def stop(self):
         self.should_run = False
 
 
 def __set_logging_level(level):
     if level != "":
-        logger.debug( f"logging_level changed to {level}")
+        logger.debug(f"logging_level changed to {level}")
         logger.set_level(level)
 
 
-config_overrides = DictOfDict()
-config_defaults = DictOfDict()
+
 
 config = ConfigSingleton()
-config.observe("AEA2:Logging:Verbosity",__set_logging_level)
-__set_logging_level(config["AEA2:Logging:Verbosity"])
+config_overrides = config.overrides
+config_defaults = config.defaults
+config.observe("AEA2:LogLevel", __set_logging_level)
+__set_logging_level(config["AEA2:LogLevel"])
 
 
 def log_except_hook(*exc_info):
     """
     Handles unhandled exceptions
     """
-    exception=exc_info[1]
-    tb_obj=exc_info[2]
-    text="".join(traceback.format_tb(tb_obj))
-
-    frameinfo= getframeinfo(currentframe())
-    logger.write_unhandled_exception(exception,f'''Unhandled exception: {text}''',frameinfo)
+    exception = exc_info[1]
+    tb_obj = exc_info[2]
+    text = "".join(traceback.format_tb(tb_obj))
+
+    frameinfo = getframeinfo(currentframe())
+    logger.write_unhandled_exception(
+        exception, f'''Unhandled exception: {text}''', frameinfo)
 
     config.stop()
 
+
 sys.excepthook = log_except_hook
```

## agora_config/command_line_provider.py

```diff
@@ -1,18 +1,19 @@
 import sys
 from .dict_of_dict import DictOfDict
 
+
 class CommandLineProvider(DictOfDict):
     def __init__(self):
         super().__init__()
         for arg in sys.argv:
             self._processArg(arg)
 
     # private methods
-            
-    def _processArg(self, arg:str):
+
+    def _processArg(self, arg: str):
         if arg.startswith("-d") and len(arg) > 2:
             first_equals = arg.find("=")
             if first_equals != -1:
                 key = arg[2:first_equals]
                 val = arg[first_equals+1:]
                 super().__setitem__(key, val)
```

## agora_config/dict_of_dict.py

```diff
@@ -1,91 +1,65 @@
-import json
-
-class DictOfDict():
-    '''
-    This class was supposed to encapsulate the dict of dict within all providers... 
-    '''
-    def __init__(self):
-        self.data = dict()
-
-    def __getitem__(self, setting_name:str):
-        keys = setting_name.split(':')
-        ld = self.data
-        for key in keys[:-1]:
-            if isinstance(ld, dict) and key in ld:
-                ld = ld[key]
-            else:
+class DictOfDict(dict):
+    def __getitem__(self, key: str):
+        key = key.replace("__", ":")
+        if isinstance(key, str) and ':' in key:
+            keys = key.split(':')
+            try:
+                value = super().__getitem__(keys[0])
+                for k in keys[1:]:
+                    if isinstance(value, dict):
+                        value = value[k]
+                    else:
+                        return ""
+            except KeyError:
+                return ""
+            return value
+        else:
+            try:
+                value = super().__getitem__(key)
+                return value
+            except KeyError:
                 return ""
-        if keys[-1] in ld:
-            d = ld[keys[-1]]
-            if not isinstance(d, dict):
-                return d
-            elif isinstance(d, dict):
-                if len(d.keys()) == 0:
-                    return ""
-                return json.dumps(ld[keys[-1]])
-        return ""
-    
-    def __setitem__(self, setting_name:str, value:str):
-        #print( f"setting '{setting_name}' = '{value}'")
-        setting_name = setting_name.replace("__", ":")
-        keys = setting_name.split(':')
-        ld = self.data
-        for key in keys[:-1]:
-            if isinstance(ld, dict) and key in ld:
-                if not isinstance(ld[key], dict):
-                    ld[key] = dict()
-                ld = ld[key]
-            else:
-                nd = dict()
-                ld[key] = nd
-                ld = nd
-        if not isinstance(ld, dict):
-            ld = dict()
-        ld[keys[-1]] = value
-        #print(self.data)
-
 
-    def remove(self, setting_name: str):
-        #print( f"removing '{setting_name}'")
-        setting_name = setting_name.replace("__", ":")
-        keys = setting_name.split(':')
-        ld = self.data
-        for key in keys[:-1]:
-            if isinstance(ld, dict) and key in ld:
-                if not isinstance(ld[key], dict):
-                    return
-                ld = ld[key]
-            else:
-                return
-        if isinstance(ld, dict):
-            k = keys[-1]
-            if k in ld:
-                #print( ld )
-                ld.pop(k)
-            return
+    def __setitem__(self, key: str, value: str):
+        key = key.replace("__", ":")
+        if isinstance(key, str) and ':' in key:
+            keys=key.split(':')
+            nested_dict = self
+            for k in keys[:-1]:
+                if k not in nested_dict:
+                    nested_dict[k] = DictOfDict()
+                elif not isinstance(nested_dict[k], dict):
+                    nested_dict[k] = DictOfDict()
+                nested_dict = nested_dict[k]
+            nested_dict[keys[-1]] = value
+        else:
+            super().__setitem__(key,value)
         return
-    
-   
-    def get_dict(self):
-        return self.data
-    
-
-    def merge(self, dict2):
-        self.data = self.__merge(self.data, dict2)
 
-    def __merge(self, dict1, dict2):
-        for key in dict2:
-            if key in dict1 and isinstance(dict1[key], dict) \
-                            and isinstance(dict2[key], dict):
-                self.__merge(dict1[key], dict2[key])
+    def __delitem__(self, key):
+        key = key.replace("__", ":")
+        if isinstance(key, str) and ":" in key:
+            key1, key2 = key.split(":", 1)
+            if key1 in self and isinstance(self[key1], DictOfDict):
+                del self[key1][key2]
+                if not bool(self[key1]):
+                    super().__delitem__(key1)
+        else:
+            if key in self:
+                super().__delitem__(key)
+
+
+    def merge(self, other: dict):
+        merge_nested_dicts(self, other)
+
+def merge_nested_dicts(dict1: dict, dict2: dict):
+    for key, value in dict2.items():
+        if key in dict1 and isinstance(dict1[key], dict) \
+            and isinstance(value, dict):
+            merge_nested_dicts(dict1[key], value)
+        else:
+            if isinstance(value, dict):
+                dict1[key] = DictOfDict()
+                merge_nested_dicts(dict1[key], value)
             else:
-                if( isinstance(dict2[key], dict)):
-                    dict1[key] = dict()
-                    self.__merge(dict1[key], dict2[key])
-                else:
-                    dict1[key] = dict2[key]
-        return dict1
-
-    def clear(self):
-        self.data.clear()
-
+                dict1[key] = value
```

## agora_config/environment_variable_provider.py

```diff
@@ -1,14 +1,14 @@
 import os
 from .dict_of_dict import DictOfDict
 
+
 class EnvironmentVariableProvider(DictOfDict):
     def __init__(self):
         super().__init__()
         self.my_dict = DictOfDict()
-        for key,val in dict(os.environ).items():
+        for key, val in dict(os.environ).items():
             self._process(key, val)
 
-
     def _process(self, key: str, val: str):
         if key.startswith("AEA__"):
-            super().__setitem__(key[5:], val)
+            super().__setitem__(key[5:], val)
```

## agora_config/file_key_provider.py

```diff
@@ -1,87 +1,79 @@
-import json
 import pathlib
 from agora_logging import logger
 from .dict_of_dict import DictOfDict
 
 
 class FileKeyProvider(DictOfDict):
     def __init__(self):
-        """
-        Uses the c# binary from the sdk, This will be run as a separate process. 
-        To allow configuration changes, root directory of the binary is symlinked to /config of the container 
-        """
         super().__init__()
         self.key_folder = pathlib.Path("config/keys")
         self.last_modified_time = 0
         self.__check_time()
 
-
     def check_for_updates(self) -> bool:
         return self.__check_time()
-    
+
     # private methods
-            
+
     def __read_config(self) -> dict:
-        """
-        Reads the configuration file
-        """
         super().clear()
         if self.key_folder.exists() and self.key_folder.is_dir():
             for file_path in self.key_folder.iterdir():
                 if file_path.is_file():
                     try:
                         with file_path.open() as f:
                             contents = f.read()
                             if len(contents) > 0 and contents[-1] == '\n':
                                 contents = contents[:-1]
-                        #print(f"contents of '{file_path.name}' is '{contents}'")
+                        # print(f"contents of '{file_path.name}' is '{contents}'")
                         self.__set(file_path.name, contents)
                     except Exception as e:
-                        logger.exception(e, f"Could not load config file '{file_path}' : {str(e)}")
-
+                        logger.exception(
+                            e, f"Could not load config file '{file_path}' : {str(e)}")
 
     def __set(self, key, value):
         new_dict = dict()
         current_dict = new_dict
         parts = key.split("__")
         if len(parts) > 0:
             for element in parts[:-1]:
                 current_dict[element] = {}
                 current_dict = current_dict[element]
             current_dict[parts[-1]] = value
         super().merge(new_dict)
-    
-    
+
     def __check_time(self) -> bool:
         """
         Checks if the times of any of the key-files or the key folder itself (i.e. a file create or delete) has changed 
         """
         mtime = 0
         modified = False
         if self.key_folder.exists() and self.key_folder.is_dir():
             try:
                 mtime = self.key_folder.stat().st_mtime
                 if mtime > self.last_modified_time:
                     # print( "key_folder modified" )
                     self.last_modified_time = mtime
                     modified = True
             except Exception as e:
-                logger.exception(e, "Could not get key folder time. 'config/keys'")
+                logger.exception(
+                    e, "Could not get key folder time. 'config/keys'")
 
             for file_path in self.key_folder.iterdir():
                 if file_path.is_file():
                     try:
                         mtime = file_path.stat().st_mtime
-                        #if file_path.name == "DEF":
-                            # print( f"DEF mtime = {mtime}")
+                        # if file_path.name == "DEF":
+                        # print( f"DEF mtime = {mtime}")
                         if mtime > self.last_modified_time:
-                            #print( f"file '{file_path.name}' modified" )
-                            self.last_modified_time =  mtime
-                            modified = True                            
+                            # print( f"file '{file_path.name}' modified" )
+                            self.last_modified_time = mtime
+                            modified = True
                     except Exception as e:
-                        logger.exception(e, f"Could not get config file time. (config_file = '{self.key_folder}')")
+                        logger.exception(
+                            e, f"Could not get config file time. (config_file = '{self.key_folder}')")
 
             if modified == True:
                 self.__read_config()
                 return True
-        return False
+        return False
```

## agora_config/file_provider.py

```diff
@@ -1,57 +1,61 @@
 import json
 import pathlib
-from concurrent.futures import ThreadPoolExecutor
 from agora_logging import logger
 from .dict_of_dict import DictOfDict
 
 
 class FileProvider(DictOfDict):
     def __init__(self, filename):
-        """
-        Uses the c# binary from the sdk, This will be run as a separate process. 
-        To allow configuration changes, root directory of the binary is symlinked to /config of the container 
-        """
         super().__init__()
-        self.config_file = pathlib.Path(filename) 
+        self.config_file = pathlib.Path(filename)
+        if filename == "AEA.json":
+            self.primary = True
+        else:
+            self.primary = False
         self.last_modified_time = 0
         self.__check_time()
 
-
     def check_for_updates(self) -> bool:
         return self.__check_time()
-    
+
+    def get_config_file_type(self) -> str:
+        if self.primary:
+            return 'PRIMARY'
+        return 'ALTERNATE'
+
     # private methods
-            
+
     def __read_config(self) -> dict:
         """
         Reads the configuration file
         """
-        super().clear()
+        self.clear()
         if self.config_file.exists():
             data = self.config_file.read_text()
             try:
                 self.merge(json.loads(data))
             except Exception as e:
-                logger.exception(e, f"Could not load config file '{self.config_file}' : {str(e)}")
-                super().clear()
-    
-    
+                logger.exception(
+                    e, f"Could not load {self.get_config_file_type()} config file '{self.config_file}' : {str(e)}")
+                self.clear()
+
     def __check_time(self) -> bool:
         """
         Checks if the time on the configuration file has changed
         """
         mtime = 0
         if self.config_file.exists():
             try:
                 mtime = self.config_file.stat().st_mtime
             except Exception as e:
-                logger.exception(e, f"Could not get config file time. (config_file = '{self.config_file}')")
+                logger.exception(
+                    e, f"Could not get {self.get_config_file_type()} config file time. (config_file = '{self.config_file}')")
                 return False
             if mtime != self.last_modified_time:
                 self.__read_config()
                 self.last_modified_time = mtime
                 return True
         else:
             # print( f"file = '{self.config_file.absolute()}' - does not exist")
             super().clear()
-        return False
+        return False
```

## agora_config/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.0.9'
+__version__ = '1.1.30'
```

