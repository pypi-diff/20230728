# Comparing `tmp/PyModMC-0.2.2a0.tar.gz` & `tmp/PyModMC-1.2.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyModMC-0.2.2a0.tar", last modified: Sun Dec 12 17:18:48 2021, max compression
+gzip compressed data, was "PyModMC-1.2.2a0.tar", last modified: Fri Jul 28 18:52:45 2023, max compression
```

## Comparing `PyModMC-0.2.2a0.tar` & `PyModMC-1.2.2a0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 lukarao    (501) staff       (20)        0 2021-12-12 17:18:48.336802 PyModMC-0.2.2a0/
--rw-r--r--   0 lukarao    (501) staff       (20)      340 2021-12-12 17:18:48.336140 PyModMC-0.2.2a0/PKG-INFO
-drwxr-xr-x   0 lukarao    (501) staff       (20)        0 2021-12-12 17:18:48.331626 PyModMC-0.2.2a0/PyModMC/
--rw-r--r--   0 lukarao    (501) staff       (20)       42 2021-12-11 19:12:18.000000 PyModMC-0.2.2a0/PyModMC/__init__.py
--rw-r--r--   0 lukarao    (501) staff       (20)    18481 2021-12-11 22:10:58.000000 PyModMC-0.2.2a0/PyModMC/main.py
-drwxr-xr-x   0 lukarao    (501) staff       (20)        0 2021-12-12 17:18:48.335391 PyModMC-0.2.2a0/PyModMC.egg-info/
--rw-r--r--   0 lukarao    (501) staff       (20)      340 2021-12-12 17:18:47.000000 PyModMC-0.2.2a0/PyModMC.egg-info/PKG-INFO
--rw-r--r--   0 lukarao    (501) staff       (20)      168 2021-12-12 17:18:47.000000 PyModMC-0.2.2a0/PyModMC.egg-info/SOURCES.txt
--rw-r--r--   0 lukarao    (501) staff       (20)        1 2021-12-12 17:18:47.000000 PyModMC-0.2.2a0/PyModMC.egg-info/dependency_links.txt
--rw-r--r--   0 lukarao    (501) staff       (20)        8 2021-12-12 17:18:47.000000 PyModMC-0.2.2a0/PyModMC.egg-info/top_level.txt
--rw-r--r--   0 lukarao    (501) staff       (20)       38 2021-12-12 17:18:48.337182 PyModMC-0.2.2a0/setup.cfg
--rw-r--r--   0 lukarao    (501) staff       (20)      383 2021-12-12 17:15:47.000000 PyModMC-0.2.2a0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:52:45.016148 PyModMC-1.2.2a0/
+-rw-rw-rw-   0        0        0     1063 2023-07-24 18:22:31.000000 PyModMC-1.2.2a0/LICENSE
+-rw-rw-rw-   0        0        0      311 2023-07-28 18:52:45.016148 PyModMC-1.2.2a0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 18:52:45.000285 PyModMC-1.2.2a0/PyModMC/
+-rw-rw-rw-   0        0        0       60 2023-07-28 18:28:24.000000 PyModMC-1.2.2a0/PyModMC/__init__.py
+-rw-rw-rw-   0        0        0    17601 2023-07-28 17:44:18.000000 PyModMC-1.2.2a0/PyModMC/main.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:52:45.015146 PyModMC-1.2.2a0/PyModMC.egg-info/
+-rw-rw-rw-   0        0        0      311 2023-07-28 18:52:44.000000 PyModMC-1.2.2a0/PyModMC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-07-28 18:52:44.000000 PyModMC-1.2.2a0/PyModMC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 18:52:44.000000 PyModMC-1.2.2a0/PyModMC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-28 18:52:44.000000 PyModMC-1.2.2a0/PyModMC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2674 2023-07-28 18:47:34.000000 PyModMC-1.2.2a0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-28 18:52:45.016148 PyModMC-1.2.2a0/setup.cfg
+-rw-rw-rw-   0        0        0      383 2023-07-28 18:48:37.000000 PyModMC-1.2.2a0/setup.py
```

### Comparing `PyModMC-0.2.2a0/PyModMC/main.py` & `PyModMC-1.2.2a0/PyModMC/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import datetime
 import glob
 import io
 import json
 import locale
 import logging
 import os
 import platform
@@ -20,92 +19,80 @@
 import xml.etree.ElementTree as et
 import zipfile
 
 locale_file = open(os.path.join(os.path.dirname(__file__), 'locale_codes.txt'))
 locale_codes = locale_file.read().split('\n')[1:]
 locale_file.close()
 
-locale.setlocale(locale.LC_ALL, '')
-LOCALE_CODE = str(locale.getlocale()[0]).lower()
+LOCALE_CODE = locale.getdefaultlocale()[0].lower()
 
 if platform.system() == 'Darwin':
-    # Workaround for a bug on OSX where it returns None for the locale
-    # Described/discussed at stackoverflow.com/q/1629699
+    # workaround for a bug on OSX where it returns None for the locale
+    # described/discussed at stackoverflow.com/q/1629699
     if LOCALE_CODE == 'none':
         LOCALE_CODE = 'en_us'
 
 if LOCALE_CODE not in locale_codes:
-    # Attempt to find the closest code to the language
-    # As an example, it will find ar_sa from the locale code ar_eg
+    # attempt to find the closest language to the locale
     for lc in locale_codes:
         if lc.startswith(LOCALE_CODE[:2]):
             LOCALE_CODE = lc
-
-# Makes logs correctly colored in IDLE, PyCharm and other IDEs
-# Adapted from different answers from stackoverflow.com/q/1383254
-class LogFilter(logging.Filter):
-    def __init__(self, level):
-        self.level = level
-
-    def filter(self, record):
-        return record.levelno < self.level
+    if LOCALE_CODE not in locale_codes:
+        LOCALE_CODE = 'en_us'
 
 logger = logging.getLogger()
+logging.basicConfig(format='[%(levelname)s] %(message)s', level=logging.INFO)
 
-info_handler = logging.StreamHandler(sys.stdout)
-info_handler.addFilter(LogFilter(logging.WARNING))
-error_handler = logging.StreamHandler(sys.stderr)
-error_handler.setLevel(logging.WARNING)
-
-logging.basicConfig(format='[%(levelname)s] %(message)s', handlers=[info_handler, error_handler], level=logging.INFO)
+def change_locale(code):
+    global LOCALE_CODE
+    if code in locale_codes:
+        LOCALE_CODE = code
+    else:
+        logger.error('Locale code is not valid.')
+        sys.exit(1)
 
 def run_cmd(command, directory=None):
     '''Used as an internal function to run and log shell commands.'''
     logger.debug(command)
-    process = subprocess.Popen(command, shell=True, stderr=subprocess.PIPE, cwd=directory)
-    error_list = []
+    process = subprocess.Popen(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, cwd=directory)
     while True:
-        error = process.stderr.readline()
+        out, error = process.communicate()
+        logger.debug(out.decode())
 
-        if len(error) > 1:
-            logger.debug(error.decode()[:-1])
-
-        if error:
-            error_list.append(error.decode())
+        if b'error:' in error:
+            for i in re.findall('error: (.*\r\n.*\r\n.*)\r\n', error.decode()):
+                error_str = i.split('\r\n')[0] + '\n'
+                error_str += i.split('\r\n')[1][4:] + '\n'
+                error_str += i.split('\r\n')[2][4:]
+                logger.error(error_str)
+            logger.debug(error.decode())
+            sys.exit(1)
         else:
             break
 
-    if error_list:
-        for error in error_list:
-            if error.startswith('Caused by'):
-                logger.error(error[11:])
-            elif error == error_list[-1]:
-                logger.error([re.sub('^[> ]+|\n', '', i) for i in error_list if '>' in i][-1])
-        sys.exit(1)
-
 def generate_mod(maven_group, modid, mod_name, description, mod_version, minecraft_version, directory, authors, website):
     minecraft_versions = json.loads(urllib.request.urlopen('https://meta.fabricmc.net/v2/versions/game').read())
     minecraft_version_list = [i['version'] for i in minecraft_versions]
     stable_minecraft_versions = [i['version'] for i in minecraft_versions if i['stable']]
     if os.path.exists(os.path.join(os.path.dirname(__file__), 'fabric_versions.json')):
         fabric_versions_file = open(os.path.join(os.path.dirname(__file__), 'fabric_versions.json'), 'r')
         fabric_minecraft_versions = json.load(fabric_versions_file)
         fabric_versions_file.close()
     else:
         fabric_minecraft_versions = {}
 
     # Accounts for unstable Minecraft versions not being recorded in Fabric's Modrinth page
     if not stable_minecraft_versions[1] in fabric_minecraft_versions:
         logger.info('Collecting fabric versions...')
-        fabric_data = urllib.request.urlopen('https://api.modrinth.com/api/v1/mod/P7dR8mSH').read()
+        fabric_data = urllib.request.urlopen('https://api.modrinth.com/v2/project/P7dR8mSH').read()
         modrinth_versions = json.loads(fabric_data)['versions']
 
         fabric_minecraft_versions = {}
         def get_version(modrinth_version, fabric_minecraft_versions):
-            version_url = 'https://api.modrinth.com/api/v1/version/' + modrinth_version
+            version_url = 'https://api.modrinth.com/v2/project/P7dR8mSH/version/' + modrinth_version
             try:
                 game_versions = json.loads(urllib.request.urlopen(version_url).read())['game_versions']
                 fabric_version = json.loads(urllib.request.urlopen(version_url).read())['version_number']
             except urllib.error.HTTPError as e:
                 if e.code == 429:
                     logger.debug('Rate-limited by Modrinth API. Trying again.')
                     time.sleep(0.4)
@@ -115,36 +102,30 @@
 
         threads = []
         for modrinth_version in modrinth_versions:
             threads.append(threading.Thread(target=get_version, args=(modrinth_version, fabric_minecraft_versions)))
 
         for thread in threads:
             thread.start()
-            time.sleep(0.4) # Prevents getting rate-limited by the Modrinth API
+            time.sleep(0.4) # prevents getting rate-limited by the Modrinth API
 
         for thread in threads:
             thread.join()
         fabric_versions_file = open(os.path.join(os.path.dirname(__file__), 'fabric_versions.json'), 'w')
         json.dump(fabric_minecraft_versions, fabric_versions_file, indent=4)
         fabric_versions_file.close()
 
     os.chdir(directory)
 
     logger.info('Cloning example mod...')
 
-    if minecraft_version in minecraft_version_list[:minecraft_version_list.index('1.16.5')]:
-        template_link = 'https://github.com/FabricMC/fabric-example-mod/archive/1.17.zip'
-        template_name = 'fabric-example-mod-1.17'
-    else:
-        template_link = 'https://github.com/FabricMC/fabric-example-mod/archive/master.zip'
-        template_name = 'fabric-example-mod-master'
-
-    template_zip = urllib.request.urlopen(template_link).read()
+    template_branch = json.loads(urllib.request.urlopen('https://api.github.com/repos/FabricMC/fabric-example-mod').read())['default_branch']
+    template_zip = urllib.request.urlopen('https://github.com/FabricMC/fabric-example-mod/archive/' + template_branch + '.zip').read()
     zipfile.ZipFile(io.BytesIO(template_zip), 'r').extractall()
-    os.rename(template_name, mod_name)
+    os.rename('fabric-example-mod-' + template_branch, mod_name)
 
     os.remove(os.path.join(mod_name, 'LICENSE'))
     os.remove(os.path.join(mod_name, 'README.md'))
     shutil.rmtree(os.path.join(mod_name, '.github'))
 
     logger.info('Configuring mod...')
 
@@ -193,15 +174,15 @@
     #json_config['mixins'] = [modid + '.mixins.json']
     json_config['mixins'] = []
     json_config['entrypoints']['main'] = [maven_group + '.' + mod_name.title().replace(' ', '')]
 
     json.dump(json_config, json_file, indent=4)
     json_file.close()
 
-    shutil.rmtree(os.path.join('src', 'main', 'java', 'net'))
+    shutil.rmtree(os.path.join('src', 'main', 'java'))
     shutil.rmtree(os.path.join('src', 'main', 'resources', 'assets', 'modid'))
 
     main_entrypoint = os.path.join('src', 'main', 'java', *maven_group.split('.'))
     os.makedirs(main_entrypoint)
     assets = os.path.join('src', 'main', 'resources', 'assets', modid)
     os.makedirs(assets)
 
@@ -254,41 +235,42 @@
         json.dump(model, model_file, indent=4, sort_keys=True)
         model_file.close()
         
     for texture in textures[0]:
         shutil.copy(texture, os.path.join(assets_dir, 'textures', 'item', name + '.png'))
         
 class Mod:
-    '''A class to represent a mod.
+    '''A class to represent a mod.'''
+    def __init__(self, mod_name, mod_version, description, minecraft_version, authors, website='', directory=os.getcwd()):
+        '''
+        Creates a mod.
 
-    Args:
+        Parameters:
         mod_name (str): Name of the mod.
         mod_version (str): Version number of the mod.
         description (str): Description of the mod.
         minecraft_version (str): Minecraft version of the mod.
         authors (list): List of the mod's authors.
         website (str, optional): Website for mod, defaults to None.
         directory (str, optional): Path for the mod folder, defaults to the current working directory.
-    '''
-    def __init__(self, mod_name, mod_version, description, minecraft_version, authors, website='', directory=os.getcwd()):
+        '''
         self.mod_name = mod_name
         self.description = description
         self.minecraft_version = minecraft_version
         self.mod_version = mod_version
         self.directory = directory
         self.authors = authors
         self.website = website
 
         self.mod_folder = os.path.join(directory, mod_name)
 
         self.modid = re.sub('[^a-zA-Z0-9_]', '', self.mod_name).lower()
         self.entrypoint = self.mod_name.title().replace(' ', '')
 
-        self.imports = {'net.fabricmc.api.ModInitializer', 'net.minecraft.util.Identifier',
-                        'net.minecraft.util.registry.Registry'}
+        self.imports = {'net.fabricmc.api.ModInitializer', 'net.minecraft.util.Identifier', 'net.minecraft.registry.Registry', 'net.minecraft.registry.Registries'}
         self.definitions = []
         self.registry = []
 
         self.item_textures = []
         self.item_models = {}
         self.block_textures = []
         self.block_models = {}
@@ -317,49 +299,48 @@
 
 public class {self.entrypoint} implements ModInitializer {{
     {(newline + tab * 2).join(self.definitions)}
     
     @Override
     public void onInitialize() {{
         {(newline + tab * 2).join(self.registry)}
-
     }}
 
 }}'''
         if os.path.isdir(self.mod_folder):
             logger.info('Found existing mod folder.')
             edit_mod(self.mod_folder, java, self.lang, [self.item_models, self.block_models], [self.item_textures, self.block_textures])
         else:
             generate_mod(self.maven_group, self.modid, self.mod_name,
                          self.description, self.mod_version, self.minecraft_version,
                          self.directory, self.authors, self.website)
         
             timer_end = timeit.default_timer()
             elapsed_time = timer_end - timer_start
             time_string = f'{int(divmod(elapsed_time, 60)[0])}m {int(divmod(elapsed_time, 60)[1])}s \
-                            {int(round(divmod(elapsed_time, 60)[1], 3) % 1 * 1000)}ms'
+{int(round(divmod(elapsed_time, 60)[1], 3) % 1 * 1000)}ms'
             logger.info('Finished saving mod in ' + time_string)
         
     def run(self):
         '''Runs the Minecraft client.'''
         self.save()
 
         logger.info('Launching Minecraft client...')
 
         command = 'gradlew runClient'
         if os.name == 'posix':
             command = './' + command
         run_cmd(command, self.mod_folder)
 
     def build(self, directory=os.getcwd()):
-        '''Exports the mod as a jar file.
+        '''
+        Exports the mod as a jar file.
 
-        Args:
-            directory (str): The directory where the jar file is exported to.
-            Defualts to the current working directory.
+        Parameters:
+        directory (str): The directory where the jar file is exported to. Defualts to the current working directory.
         '''
         timer_start = timeit.default_timer()
         
         self.save()
 
         logger.info('Building your mod...')
 
@@ -376,85 +357,69 @@
 
         timer_end = timeit.default_timer()
         elapsed_time = timer_end - timer_start
         time_string = f'{int(divmod(elapsed_time, 60)[0])}m {int(divmod(elapsed_time, 60)[1])}s \
                         {int(round(divmod(elapsed_time, 60)[1], 3) % 1 * 1000)}ms'
         logger.info('Finished building in ' + time_string)
 
-    def Item(self, name, itemgroup='misc', image=None):
-        '''Creates an item.
-
-        Args:
-            name (str): Name of the item.
-
-            itemgroup (str, optional): The item's category, used for creative tabs - one
-            of the following: brewing, building blocks, combat, decorations,
-            food, materials, misc, redstone, tools or transportation. Defaults
-            to misc.
+class Item:
+    '''A class to represent an item.'''
+    def __init__(self, mod, name, itemgroup, image=None):
+        '''
+        Creates an item.
 
-            image (str, optional): Path to the item's image. If no path is
-            specified, it will look in the working directory for an image.
+        Parameters:
+        mod (Mod): The mod class.
+        name (str): Name of the item.
+        itemgroup (str): The item's category, used for creative tabs - one of the following: COLORED_BLOCKS, NATURAL, FUNCTIONAL, REDSTONE, HOTBAR, SEARCH, TOOLS, COMBAT, FOOD_AND_DRINK, INGREDIENTS, SPAWN_EGGS, OPERATOR, or INVENTORY.
+        image (str, optional): Path to the item's image. If no path is specified, it will look in the working directory for an image.
         '''
 
         texture = glob.glob('**/' + name.lower().replace(' ', '_') + '.png', recursive=True)
         
         if image:
             texture_file = image
         elif texture:
             texture_file = os.path.join(os.getcwd(), texture[0])
         else:
             logger.error('Could not find a texture for \'' + name + '\'')
             sys.exit()
 
-        self.item_models[name.lower().replace(' ', '_')] = {'parent': 'minecraft:item/generated', 'textures': {'layer0': f'{self.modid}:item/{name.lower().replace(" ", "_")}'}}
+        mod.item_models[name.lower().replace(' ', '_')] = {'parent': 'minecraft:item/generated', 'textures': {'layer0': f'{mod.modid}:item/{name.lower().replace(" ", "_")}'}}
 
-        self.item_textures.append(texture_file)
+        mod.item_textures.append(texture_file)
         
-        self.definitions.append(f'public static final Item {name.upper().replace(" ", "_")} = new Item(new Item.Settings().group(ItemGroup.{itemgroup.upper().replace(" ", "_")}));')
-        self.imports.add('net.minecraft.item.Item')
-        self.imports.add('net.minecraft.item.ItemGroup')
-        self.registry.append(f'Registry.register(Registry.ITEM, new Identifier("{self.modid}", "{name.lower().replace(" ", "_")}"), {name.upper().replace(" ", "_")});')
+        mod.imports.add('net.minecraft.item.Item')
+        mod.imports.add('net.minecraft.item.ItemGroups')
+        mod.imports.add('net.fabricmc.fabric.api.item.v1.FabricItemSettings')
+        mod.imports.add('net.fabricmc.fabric.api.itemgroup.v1.ItemGroupEvents')
+        mod.registry.append(f'Registry.register(Registries.ITEM, new Identifier("{mod.modid}", "{name.lower().replace(" ", "_")}"), {name.upper().replace(" ", "_")});')
+        mod.registry.append(f'ItemGroupEvents.modifyEntriesEvent(ItemGroups.{itemgroup}).register(entries -> entries.add({name.upper().replace(" ", "_")}));')
         
-        self.lang[f'item.{self.modid}.{name.lower().replace(" ", "_")}'] = name
+        mod.lang[f'item.{mod.modid}.{name.lower().replace(" ", "_")}'] = name
 
-    def FoodItem(self, name, hunger, saturation, itemgroup='food', image=None):
-        '''Creates a food item.
+        self.definition(mod, name, itemgroup)
 
-        Args:
-            name (str): Name of the food.
-            
-            hunger (int): Amount of hunger points your item fills. Each hunger
-            point is half a hunger shank.
-            
-            saturation (float): Saturation modifier for the item. The saturation
-            modifier is equvalent to saturation restored / hunger points * 0.5.
+    def definition(self, mod, name, itemgroup):
+        mod.definitions.append(f'public static final Item {name.upper().replace(" ", "_")} = new Item(new FabricItemSettings());')
 
-            itemgroup (str, optional): The item's category, used for creative
-            tabs - one of the following: brewing, building blocks, combat,
-            decorations, food, materials, misc, redstone, tools or
-            transportation. Defaults to misc.
-            
-            image (str, optional): Path to the item's image. If no path is
-            specified, it will look in the working directory for an image.
+class FoodItem(Item):
+    '''A class to represent a food item.'''
+    def __init__(self, mod, name, hunger, saturation, itemgroup='FOOD_AND_DRINK', image=None):
         '''
-        texture = glob.glob('**/' + name.lower().replace(' ', '_') + '.png', recursive=True)
-        
-        if image:
-            texture_file = image
-        elif texture:
-            texture_file = os.path.join(os.getcwd(), texture[0])
-        else:
-            logger.error('Could not find a texture for \'' + name + '\'')
-            sys.exit()
-
-        self.item_models[name.lower().replace(' ', '_')] = {'parent': 'minecraft:item/generated', 'textures': {'layer0': f'{self.modid}:item/{name.lower().replace(" ", "_")}'}}
-
-        self.item_textures.append(texture_file)
-        
-        self.definitions.append(f'public static final Item {name.upper().replace(" ", "_")} = new Item.Settings().group(ItemGroup.{itemgroup.upper().replace(" ", "_")}).food(new FoodComponent.Builder().hunger({hunger}).saturationModifier({saturation}f).build())')
-        self.imports.add('net.minecraft.item.Item')
-        self.imports.add('net.minecraft.item.ItemGroup')
-        self.imports.add('net.minecraft.item.FoodComponent')
+        Creates a food item.
 
-        self.registry.append(f'Registry.register(Registry.ITEM, new Identifier("{self.modid}", "{name.lower().replace(" ", "_")}"), {name.upper().replace(" ", "_")});')
-        
-        self.lang[f'item.{self.modid}.{name.lower().replace(" ", "_")}'] = name
+        Args:
+        mod (Mod): The mod class.
+        name (str): Name of the food.
+        hunger (int): Amount of hunger points your item fills. Each hunger point is half a hunger shank.
+        saturation (float): Saturation modifier for the item. The saturation modifier is equvalent to saturation restored / hunger points * 0.5.
+        itemgroup (str, optional): The item's category, used for creative tabs - one of the following: COLORED_BLOCKS, NATURAL, FUNCTIONAL, REDSTONE, HOTBAR, SEARCH, TOOLS, COMBAT, FOOD_AND_DRINK, INGREDIENTS, SPAWN_EGGS, OPERATOR, or INVENTORY. Defaults to FOOD_AND_DRINK.
+        image (str, optional): Path to the item's image. If no path is specified, it will look in the working directory for an image.
+        '''
+        self.hunger = hunger
+        self.saturation = saturation
+        super().__init__(mod, name, itemgroup, image)
+    
+    def definition(self, mod, name, itemgroup):
+        mod.definitions.append(f'public static final Item {name.upper().replace(" ", "_")} = new Item(new FabricItemSettings().food(new FoodComponent.Builder().hunger({self.hunger}).saturationModifier({self.saturation}f).build()));')
+        mod.imports.add('net.minecraft.item.FoodComponent')
```

