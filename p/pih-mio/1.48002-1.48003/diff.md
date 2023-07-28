# Comparing `tmp/pih_mio-1.48002.tar.gz` & `tmp/pih_mio-1.48003.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih_mio-1.48002.tar", last modified: Fri Jul 28 09:21:24 2023, max compression
+gzip compressed data, was "pih_mio-1.48003.tar", last modified: Fri Jul 28 09:31:16 2023, max compression
```

## Comparing `pih_mio-1.48002.tar` & `pih_mio-1.48003.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 09:21:23.585389 pih_mio-1.48002/
-drwxrwxrwx   0        0        0        0 2023-07-28 09:21:23.929136 pih_mio-1.48002/MobileHelperCore/
--rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih_mio-1.48002/MobileHelperCore/__init__.py
--rw-rw-rw-   0        0        0   165168 2023-07-28 09:19:10.000000 pih_mio-1.48002/MobileHelperCore/api.py
--rw-rw-rw-   0        0        0      686 2023-07-17 12:20:25.000000 pih_mio-1.48002/MobileHelperCore/service.py
--rw-rw-rw-   0        0        0     9200 2023-07-23 04:55:02.000000 pih_mio-1.48002/MobileHelperCore/service_api.py
--rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih_mio-1.48002/MobileHelperCore/tools.py
--rw-rw-rw-   0        0        0      279 2023-07-28 09:21:24.335509 pih_mio-1.48002/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 09:21:23.991636 pih_mio-1.48002/pih_MIO.egg-info/
--rw-rw-rw-   0        0        0      279 2023-07-28 09:21:22.000000 pih_mio-1.48002/pih_MIO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      463 2023-07-28 09:21:23.000000 pih_mio-1.48002/pih_MIO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 09:21:22.000000 pih_mio-1.48002/pih_MIO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-28 09:21:23.000000 pih_mio-1.48002/pih_MIO.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-28 09:21:23.000000 pih_mio-1.48002/pih_MIO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1501 2023-07-28 09:13:59.000000 pih_mio-1.48002/pih_mio_setup.py
--rw-rw-rw-   0        0        0       42 2023-07-28 09:21:24.335509 pih_mio-1.48002/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 09:31:16.208093 pih_mio-1.48003/
+drwxrwxrwx   0        0        0        0 2023-07-28 09:31:16.473712 pih_mio-1.48003/MobileHelperCore/
+-rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih_mio-1.48003/MobileHelperCore/__init__.py
+-rw-rw-rw-   0        0        0   165201 2023-07-28 09:30:54.000000 pih_mio-1.48003/MobileHelperCore/api.py
+-rw-rw-rw-   0        0        0      686 2023-07-17 12:20:25.000000 pih_mio-1.48003/MobileHelperCore/service.py
+-rw-rw-rw-   0        0        0     9200 2023-07-23 04:55:02.000000 pih_mio-1.48003/MobileHelperCore/service_api.py
+-rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih_mio-1.48003/MobileHelperCore/tools.py
+-rw-rw-rw-   0        0        0      279 2023-07-28 09:31:16.708106 pih_mio-1.48003/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 09:31:16.629944 pih_mio-1.48003/pih_MIO.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-07-28 09:31:15.000000 pih_mio-1.48003/pih_MIO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2023-07-28 09:31:16.000000 pih_mio-1.48003/pih_MIO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 09:31:15.000000 pih_mio-1.48003/pih_MIO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-28 09:31:15.000000 pih_mio-1.48003/pih_MIO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-28 09:31:15.000000 pih_mio-1.48003/pih_MIO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1501 2023-07-28 09:13:59.000000 pih_mio-1.48003/pih_mio_setup.py
+-rw-rw-rw-   0        0        0       42 2023-07-28 09:31:16.724055 pih_mio-1.48003/setup.cfg
```

### Comparing `pih_mio-1.48002/MobileHelperCore/api.py` & `pih_mio-1.48003/MobileHelperCore/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1034,15 +1034,15 @@
         #######################
         self.address_as_link_node: CommandNode = self.create_command_link(
             f"link|{LINK_SYMBOL}", LINK_SYMBOL, i("Адресовать ссылку на команду"), MobileHelper.ADM, True)
         self.address_as_link_node.order_value = 3
         additional_nodes.append(self.address_as_link_node)
         #######################
         about_pih_node: CommandNode = CommandNode(
-            "about|o", i("О PIH"), description="\n...", text=f"Я бот-помощник для решения Ваших задач. Моё имя составлено из первых букв нашей организации: *P* acific *I* nternational *H* ospital.\n\n_Автор: {i(b('Караченцев Никита Александрович'))}", show_in_root_menu=True, wait_for_input=False, show_always=True)
+            "about|o", i("О PIH"), description="\n...", text=f"Я бот-помощник для решения Ваших задач. Моё имя составлено из первых букв нашей организации: *P* acific *I* nternational *H* ospital.\n\n_Автор: {i(b('Караченцев Никита Александрович'))}\nВерсия: {A.V.MIO.local()}", show_in_root_menu=True, wait_for_input=False, show_always=True)
         about_pih_node.order_value = 4
         additional_nodes.append(about_pih_node)
         #######################
         self.exit_node: CommandNode = CommandNode(
             "exit", i("Выход"), self.session.exit, show_in_root_menu=True, wait_for_input=False, show_always=True, as_link=True)
         self.exit_node.order_value = 0
         additional_nodes.append(self.exit_node)
```

### Comparing `pih_mio-1.48002/MobileHelperCore/service.py` & `pih_mio-1.48003/MobileHelperCore/service.py`

 * *Files identical despite different names*

### Comparing `pih_mio-1.48002/MobileHelperCore/service_api.py` & `pih_mio-1.48003/MobileHelperCore/service_api.py`

 * *Files identical despite different names*

### Comparing `pih_mio-1.48002/MobileHelperCore/tools.py` & `pih_mio-1.48003/MobileHelperCore/tools.py`

 * *Files identical despite different names*

### Comparing `pih_mio-1.48002/pih_mio_setup.py` & `pih_mio-1.48003/pih_mio_setup.py`

 * *Files identical despite different names*

