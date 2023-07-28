# Comparing `tmp/pih-mio-1.48013.tar.gz` & `tmp/pih-mio-1.48014.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-mio-1.48013.tar", last modified: Fri Jul 28 13:42:14 2023, max compression
+gzip compressed data, was "pih-mio-1.48014.tar", last modified: Fri Jul 28 13:50:18 2023, max compression
```

## Comparing `pih-mio-1.48013.tar` & `pih-mio-1.48014.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 13:42:14.467316 pih-mio-1.48013/
-drwxrwxrwx   0        0        0        0 2023-07-28 13:42:14.498580 pih-mio-1.48013/MobileHelperCore/
--rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48013/MobileHelperCore/__init__.py
--rw-rw-rw-   0        0        0      158 2023-07-28 13:41:38.000000 pih-mio-1.48013/MobileHelperCore/__main__.py
--rw-rw-rw-   0        0        0   165201 2023-07-28 09:30:54.000000 pih-mio-1.48013/MobileHelperCore/api.py
--rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-mio-1.48013/MobileHelperCore/service.py
--rw-rw-rw-   0        0        0     9431 2023-07-28 13:39:51.000000 pih-mio-1.48013/MobileHelperCore/service_api.py
--rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-mio-1.48013/MobileHelperCore/tools.py
--rw-rw-rw-   0        0        0      279 2023-07-28 13:42:14.967321 pih-mio-1.48013/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 13:42:14.936080 pih-mio-1.48013/pih_MIO.egg-info/
--rw-rw-rw-   0        0        0      279 2023-07-28 13:42:13.000000 pih-mio-1.48013/pih_MIO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      526 2023-07-28 13:42:14.000000 pih-mio-1.48013/pih_MIO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 13:42:13.000000 pih-mio-1.48013/pih_MIO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-07-28 13:42:13.000000 pih-mio-1.48013/pih_MIO.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-07-28 13:42:13.000000 pih-mio-1.48013/pih_MIO.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-28 13:42:13.000000 pih-mio-1.48013/pih_MIO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1644 2023-07-28 12:42:15.000000 pih-mio-1.48013/pih_mio_setup.py
--rw-rw-rw-   0        0        0       42 2023-07-28 13:42:14.982966 pih-mio-1.48013/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 13:50:17.175657 pih-mio-1.48014/
+drwxrwxrwx   0        0        0        0 2023-07-28 13:50:17.675640 pih-mio-1.48014/MobileHelperCore/
+-rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48014/MobileHelperCore/__init__.py
+-rw-rw-rw-   0        0        0      158 2023-07-28 13:41:38.000000 pih-mio-1.48014/MobileHelperCore/__main__.py
+-rw-rw-rw-   0        0        0   165319 2023-07-28 13:49:12.000000 pih-mio-1.48014/MobileHelperCore/api.py
+-rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-mio-1.48014/MobileHelperCore/service.py
+-rw-rw-rw-   0        0        0     9431 2023-07-28 13:39:51.000000 pih-mio-1.48014/MobileHelperCore/service_api.py
+-rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-mio-1.48014/MobileHelperCore/tools.py
+-rw-rw-rw-   0        0        0      279 2023-07-28 13:50:18.284998 pih-mio-1.48014/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 13:50:18.238127 pih-mio-1.48014/pih_MIO.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-07-28 13:50:16.000000 pih-mio-1.48014/pih_MIO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      526 2023-07-28 13:50:17.000000 pih-mio-1.48014/pih_MIO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 13:50:16.000000 pih-mio-1.48014/pih_MIO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-07-28 13:50:16.000000 pih-mio-1.48014/pih_MIO.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-07-28 13:50:16.000000 pih-mio-1.48014/pih_MIO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-28 13:50:16.000000 pih-mio-1.48014/pih_MIO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1644 2023-07-28 12:42:15.000000 pih-mio-1.48014/pih_mio_setup.py
+-rw-rw-rw-   0        0        0       42 2023-07-28 13:50:18.284998 pih-mio-1.48014/setup.cfg
```

### Comparing `pih-mio-1.48013/MobileHelperCore/api.py` & `pih-mio-1.48014/MobileHelperCore/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1034,15 +1034,15 @@
         #######################
         self.address_as_link_node: CommandNode = self.create_command_link(
             f"link|{LINK_SYMBOL}", LINK_SYMBOL, i("Адресовать ссылку на команду"), MobileHelper.ADM, True)
         self.address_as_link_node.order_value = 3
         additional_nodes.append(self.address_as_link_node)
         #######################
         about_pih_node: CommandNode = CommandNode(
-            "about|o", i("О PIH"), description="\n...", text=f"Я бот-помощник для решения Ваших задач. Моё имя составлено из первых букв нашей организации: *P* acific *I* nternational *H* ospital.\n\n_Автор: {i(b('Караченцев Никита Александрович'))}\nВерсия: {A.V.MIO.local()}", show_in_root_menu=True, wait_for_input=False, show_always=True)
+            "about|o", i("О PIH"), description="\n...", text=f"Я бот-помощник для решения Ваших задач. Моё имя составлено из первых букв нашей организации: {b('P')} acific {b('I')} nternational {b('H')} ospital или {b('П')} асифик {b('И')} нтернейшнл {b('Х')} оспитал.\n\n{i('Автор')}: {i(b('Караченцев Никита Александрович'))} \n{i('Версия')}: {b(A.V.MIO.local())}", show_in_root_menu=True, wait_for_input=False, show_always=True)
         about_pih_node.order_value = 4
         additional_nodes.append(about_pih_node)
         #######################
         self.exit_node: CommandNode = CommandNode(
             "exit", i("Выход"), self.session.exit, show_in_root_menu=True, wait_for_input=False, show_always=True, as_link=True)
         self.exit_node.order_value = 0
         additional_nodes.append(self.exit_node)
```

### Comparing `pih-mio-1.48013/MobileHelperCore/service.py` & `pih-mio-1.48014/MobileHelperCore/service.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48013/MobileHelperCore/service_api.py` & `pih-mio-1.48014/MobileHelperCore/service_api.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48013/MobileHelperCore/tools.py` & `pih-mio-1.48014/MobileHelperCore/tools.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48013/pih_MIO.egg-info/SOURCES.txt` & `pih-mio-1.48014/pih_MIO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48013/pih_mio_setup.py` & `pih-mio-1.48014/pih_mio_setup.py`

 * *Files identical despite different names*

