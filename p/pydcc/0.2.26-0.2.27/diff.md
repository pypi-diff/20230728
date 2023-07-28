# Comparing `tmp/pydcc-0.2.26.tar.gz` & `tmp/pydcc-0.2.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydcc-0.2.26.tar", last modified: Fri Jul 21 13:35:06 2023, max compression
+gzip compressed data, was "pydcc-0.2.27.tar", last modified: Fri Jul 28 11:19:02 2023, max compression
```

## Comparing `pydcc-0.2.26.tar` & `pydcc-0.2.27.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 13:35:06.710887 pydcc-0.2.26/
--rw-rw-rw-   0        0        0     1057 2023-03-14 11:13:43.000000 pydcc-0.2.26/LICENSE
--rw-rw-rw-   0        0        0       97 2023-04-21 08:04:52.000000 pydcc-0.2.26/MANIFEST.in
--rw-rw-rw-   0        0        0     4793 2023-07-21 13:35:06.710323 pydcc-0.2.26/PKG-INFO
--rw-rw-rw-   0        0        0     4107 2023-07-21 11:07:01.000000 pydcc-0.2.26/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 13:35:06.676042 pydcc-0.2.26/dcc/
--rw-rw-rw-   0        0        0      313 2023-07-10 14:47:54.000000 pydcc-0.2.26/dcc/__init__.py
--rw-rw-rw-   0        0        0    23799 2023-07-10 14:46:54.000000 pydcc-0.2.26/dcc/dcc.py
--rw-rw-rw-   0        0        0    15345 2023-07-12 15:33:45.000000 pydcc-0.2.26/dcc/dcc_xml_validator.py
--rw-rw-rw-   0        0        0        6 2023-07-21 13:34:54.000000 pydcc-0.2.26/next_version.txt
-drwxrwxrwx   0        0        0        0 2023-07-21 13:35:06.706672 pydcc-0.2.26/pydcc.egg-info/
--rw-rw-rw-   0        0        0     4793 2023-07-21 13:35:06.000000 pydcc-0.2.26/pydcc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-07-21 13:35:06.000000 pydcc-0.2.26/pydcc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 13:35:06.000000 pydcc-0.2.26/pydcc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-07-21 13:35:06.000000 pydcc-0.2.26/pydcc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-21 13:35:06.000000 pydcc-0.2.26/pydcc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 13:35:06.711392 pydcc-0.2.26/setup.cfg
--rw-rw-rw-   0        0        0     1413 2023-07-11 09:46:25.000000 pydcc-0.2.26/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:19:02.865615 pydcc-0.2.27/
+-rw-rw-rw-   0        0        0     1057 2023-03-14 11:13:43.000000 pydcc-0.2.27/LICENSE
+-rw-rw-rw-   0        0        0       97 2023-04-21 08:04:52.000000 pydcc-0.2.27/MANIFEST.in
+-rw-rw-rw-   0        0        0     4793 2023-07-28 11:19:02.864615 pydcc-0.2.27/PKG-INFO
+-rw-rw-rw-   0        0        0     4107 2023-07-21 11:07:01.000000 pydcc-0.2.27/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 11:19:02.827514 pydcc-0.2.27/dcc/
+-rw-rw-rw-   0        0        0      313 2023-07-10 14:47:54.000000 pydcc-0.2.27/dcc/__init__.py
+-rw-rw-rw-   0        0        0    24633 2023-07-28 11:12:48.000000 pydcc-0.2.27/dcc/dcc.py
+-rw-rw-rw-   0        0        0    15345 2023-07-12 15:33:45.000000 pydcc-0.2.27/dcc/dcc_xml_validator.py
+-rw-rw-rw-   0        0        0        6 2023-07-28 11:18:48.000000 pydcc-0.2.27/next_version.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 11:19:02.861614 pydcc-0.2.27/pydcc.egg-info/
+-rw-rw-rw-   0        0        0     4793 2023-07-28 11:19:02.000000 pydcc-0.2.27/pydcc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-07-28 11:19:02.000000 pydcc-0.2.27/pydcc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 11:19:02.000000 pydcc-0.2.27/pydcc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-07-28 11:19:02.000000 pydcc-0.2.27/pydcc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-28 11:19:02.000000 pydcc-0.2.27/pydcc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 11:19:02.865615 pydcc-0.2.27/setup.cfg
+-rw-rw-rw-   0        0        0     1413 2023-07-11 09:46:25.000000 pydcc-0.2.27/setup.py
```

### Comparing `pydcc-0.2.26/LICENSE` & `pydcc-0.2.27/LICENSE`

 * *Files identical despite different names*

### Comparing `pydcc-0.2.26/PKG-INFO` & `pydcc-0.2.27/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydcc
-Version: 0.2.26
+Version: 0.2.27
 Summary: Library for handling digital calibration certificates (DCC). 
 Home-page: https://gitlab.com/gemimeg/pydcc
 Author: Andreas Tobola
 Author-email: pydcc.t@siemens.com
 License: MIT License
 Keywords: digital calibration certificate measurement uncertainty precision GUM DCC
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pydcc-0.2.26/README.md` & `pydcc-0.2.27/README.md`

 * *Files identical despite different names*

### Comparing `pydcc-0.2.26/dcc/dcc.py` & `pydcc-0.2.27/dcc/dcc.py`

 * *Files 4% similar despite different names*

```diff
@@ -480,42 +480,57 @@
                     local_res = [quant[2], self.__etree_to_dict(si_node)]
                 else:
                     local_res = [quant[1], self.__etree_to_dict(si_node)]
                 res.append(local_res)
         return res
 
     def __etree_to_dict(self, t):
+        """
+        This method was adapted from a post at Stackoverflow
+        URL: https://stackoverflow.com/a/10077069
+        This method is licensed under a Creative Commons Attribution ShareAlike 3.0 (CC-BY-SA 3.0) License
+        URL: http://creativecommons.org/licenses/by/3.0/deed.en_US
+        """
         # method to recursively traverse the xml tree from a specified point and to return the elemnts in dictionary form
         tkey = t.tag.rpartition('}')[2]
-        d = {tkey: {} if t.attrib else None}
+        tree_dict = {tkey: {} if t.attrib else None}
         children = list(t)
         if children:
-            dd = defaultdict(list)
+            subdict = defaultdict(list)
             for dc in map(self.__etree_to_dict, children):
-                for k, v in dc.items():
-                    dd[k].append(v)
-            d = {tkey: {k: v[0] if len(v) == 1 else v
-                        for k, v in dd.items()}}
+                for key, val in dc.items():
+                    subdict[key].append(val)
+            tree_dict = {tkey: {k: v[0] if len(v) == 1 else v
+                        for k, v in subdict.items()}}
         if t.attrib:
-            d[tkey].update(('@' + k, v)
+            tree_dict[tkey].update(('@' + k, v)
                            for k, v in t.attrib.items())
         if t.text:
             text = t.text.strip()
             if children or t.attrib:
                 if text:
-                    d[tkey]['#text'] = text
+                    tree_dict[tkey]['#text'] = text
             else:
-                d[tkey] = text
-        return d
+                tree_dict[tkey] = text
+        return tree_dict
 
     def item_id(self):
         # Retrieve list of items in DCC and return as a dictionary with identifier type as key
         id_list = self.root.find("dcc:administrativeData/dcc:items/dcc:item/dcc:identifications", self.name_space)
         return self.__etree_to_dict(id_list)
 
+    def item_id_new(self):
+        # Retrieve list of items in DCC and return as a dictionary with identifier type as key
+        id_list = self.root.find("dcc:administrativeData/dcc:items/dcc:item/dcc:identifications", self.name_space)
+        item_id_dict = {'identifications': []}
+        ids = list(id_list)
+        for id in ids:
+            item_id_dict['identifications'].append(self.etree_to_dict(id))
+        return item_id_dict
+
     def get_item_id_by_name(self, searched_name, searched_language = None, searched_issuer = None):
         id_list = self.item_id()['identifications']['identification']
         for id in id_list:
             names = id['name']['content']
             issuer = id['issuer']
             if searched_issuer is not None:
                 if not issuer == searched_issuer:
```

### Comparing `pydcc-0.2.26/dcc/dcc_xml_validator.py` & `pydcc-0.2.27/dcc/dcc_xml_validator.py`

 * *Files identical despite different names*

### Comparing `pydcc-0.2.26/pydcc.egg-info/PKG-INFO` & `pydcc-0.2.27/pydcc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydcc
-Version: 0.2.26
+Version: 0.2.27
 Summary: Library for handling digital calibration certificates (DCC). 
 Home-page: https://gitlab.com/gemimeg/pydcc
 Author: Andreas Tobola
 Author-email: pydcc.t@siemens.com
 License: MIT License
 Keywords: digital calibration certificate measurement uncertainty precision GUM DCC
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pydcc-0.2.26/setup.py` & `pydcc-0.2.27/setup.py`

 * *Files identical despite different names*

