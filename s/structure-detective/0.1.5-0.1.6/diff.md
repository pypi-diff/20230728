# Comparing `tmp/structure_detective-0.1.5.tar.gz` & `tmp/structure_detective-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structure_detective-0.1.5.tar", max compression
+gzip compressed data, was "structure_detective-0.1.6.tar", max compression
```

## Comparing `structure_detective-0.1.5.tar` & `structure_detective-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      371 2023-03-30 03:39:36.974233 structure_detective-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       96 2023-03-30 03:39:36.974233 structure_detective-0.1.5/structure_detective/__init__.py
--rw-r--r--   0        0        0      292 2023-03-30 03:39:36.974233 structure_detective-0.1.5/structure_detective/constants.py
--rw-r--r--   0        0        0     3121 2023-03-30 03:39:36.974233 structure_detective-0.1.5/structure_detective/de/structure.py
--rw-r--r--   0        0        0     8863 2023-03-30 03:39:36.974233 structure_detective-0.1.5/structure_detective/de/trans_structure.py
--rw-r--r--   0        0        0     7030 2023-03-30 03:39:36.974233 structure_detective-0.1.5/structure_detective/en/structure.py
--rw-r--r--   0        0        0     6463 2023-03-30 03:39:36.974233 structure_detective-0.1.5/structure_detective/en/trans_structure.py
--rw-r--r--   0        0        0     2223 2023-03-30 03:39:36.974233 structure_detective-0.1.5/structure_detective/es/morph_translation.py
--rw-r--r--   0        0        0     1549 2023-03-30 03:39:36.974233 structure_detective-0.1.5/structure_detective/es/structure.py
--rw-r--r--   0        0        0     1164 2023-03-30 03:39:36.974233 structure_detective-0.1.5/structure_detective/es/trans_structure.py
--rw-r--r--   0        0        0     1681 2023-03-30 03:39:36.974233 structure_detective-0.1.5/structure_detective/lib.py
--rw-r--r--   0        0        0      798 2023-03-30 03:39:36.974233 structure_detective-0.1.5/structure_detective/structure.py
--rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 structure_detective-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      371 2023-07-28 09:31:54.396708 structure_detective-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       96 2023-07-28 09:31:54.396708 structure_detective-0.1.6/structure_detective/__init__.py
+-rw-r--r--   0        0        0      292 2023-07-28 09:31:54.396708 structure_detective-0.1.6/structure_detective/constants.py
+-rw-r--r--   0        0        0     3378 2023-07-28 09:31:54.400708 structure_detective-0.1.6/structure_detective/de/structure.py
+-rw-r--r--   0        0        0     8863 2023-07-28 09:31:54.400708 structure_detective-0.1.6/structure_detective/de/trans_structure.py
+-rw-r--r--   0        0        0     7363 2023-07-28 09:31:54.400708 structure_detective-0.1.6/structure_detective/en/structure.py
+-rw-r--r--   0        0        0     6463 2023-07-28 09:31:54.400708 structure_detective-0.1.6/structure_detective/en/trans_structure.py
+-rw-r--r--   0        0        0     2223 2023-07-28 09:31:54.400708 structure_detective-0.1.6/structure_detective/es/morph_translation.py
+-rw-r--r--   0        0        0     1712 2023-07-28 09:31:54.400708 structure_detective-0.1.6/structure_detective/es/structure.py
+-rw-r--r--   0        0        0     1164 2023-07-28 09:31:54.400708 structure_detective-0.1.6/structure_detective/es/trans_structure.py
+-rw-r--r--   0        0        0     1769 2023-07-28 09:31:54.400708 structure_detective-0.1.6/structure_detective/lib.py
+-rw-r--r--   0        0        0      798 2023-07-28 09:31:54.400708 structure_detective-0.1.6/structure_detective/structure.py
+-rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 structure_detective-0.1.6/PKG-INFO
```

### Comparing `structure_detective-0.1.5/structure_detective/de/structure.py` & `structure_detective-0.1.6/structure_detective/de/structure.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,35 +24,41 @@
     return store
   else:
     for oc in ocs:
       regular_oc_children = get_children_except_xs(oc, ["oc"])
       store.extend(form_children_info(doc, regular_oc_children))
 
       start, end = oc.i, oc.i+1
+      sub = doc[start:end]
       _info = {
         "start": start,
         "end": end,
-        "text": doc[start:end].text,
+        "start_char": sub.start_char,
+        "end_char": sub.end_char,
+        "text": sub.text,
         "element": oc.i,
         "is_root": False,
       }
       store.append(_info)
  
       oc_children = [occ for occ in oc.children if occ.dep_=="oc"]
       store.extend(_handle_backward_ocs(oc_children, doc))
     return store
 
 def _handle_oc(doc: Doc, nlp: Language):
   store = []
   # append ROOT
   root = _get_root(doc)
   start, end = root.i, root.i+1
+  sub = doc[start:end]
   _info = {
     "start": start,
     "end": end,
+    "start_char": sub.start_char,
+    "end_char": sub.end_char,
     "text": doc[start:end].text,
     "element": root.i, 
     "is_root": True,
   }
   store.append(_info)
 
   # No oc
@@ -74,18 +80,21 @@
 
     # handle oc node with/without zu
     zu_children = [t for t in oc.children if t.dep_ in ["pm"] and t.text == "zu" and t.i == oc.i-1]
     if len(zu_children) == 1:
       start, end = oc.i-1, oc.i+1 
     else:
       start, end = oc.i, oc.i+1
+    sub = doc[start:end]
     _info = {
       "start": start,
       "end": end,
-      "text": doc[start:end].text,
+      "start_char": sub.start_char,
+      "end_char": sub.end_char,
+      "text": sub.text,
       "element": oc.i,
       "is_root": False,
     }
     store.append(_info)
 
     # handle forward oc
     oc_forward_children = [t for t in oc.children if t.dep_ == "oc" and t.i>oc.i]
```

### Comparing `structure_detective-0.1.5/structure_detective/de/trans_structure.py` & `structure_detective-0.1.6/structure_detective/de/trans_structure.py`

 * *Files identical despite different names*

### Comparing `structure_detective-0.1.5/structure_detective/en/structure.py` & `structure_detective-0.1.6/structure_detective/en/structure.py`

 * *Files 11% similar despite different names*

```diff
@@ -113,68 +113,80 @@
   _r_range = range(len(roots))
   for index in _r_range:
     if index < len(roots)-1:
       assert(roots[index].i+1 == roots[index+1].i)
   # append ROOT
   root = roots[0] 
   start, end = root.i, roots[-1].i+1
+  sub = doc[start:end]
   _info = {
     "start": start,
     "end": end,
-    "text": doc[start:end].text,
+    "start_char": sub.start_char,
+    "end_char": sub.end_char,
+    "text": sub.text,
     "element": root.i, 
     "is_root": True,
     "semantic_dep": "ROOT"
   }
   store.append(_info)
   return store
 
 def _handle_half_have_to_root(doc:Doc, roots: list):
   store = []
   # append ROOT
   for root in roots:
     start = root.i
     end = root.i+2 if root.dep_== "ROOT" and len(roots)==2 else root.i+1
+    sub = doc[start:end]
     _info = {
       "start": start,
       "end": end,
-      "text": doc[start:end].text,
+      "start_char": sub.start_char,
+      "end_char": sub.end_char,
+      "text": sub.text,
       "element": root.i, 
       "is_root": root.dep_=="ROOT",
       "semantic_dep": "ROOT"
     }
     store.append(_info)
   return store
 
 def _handle_half_have_got_to_root(doc:Doc, roots: list):
   store = []
   # append ROOT
   for root in roots:
     start = root.i
     end = root.i+1
+    sub = doc[start:end]
     _info = {
       "start": start,
       "end": end,
-      "text": doc[start:end].text,
+      "start_char": sub.start_char,
+      "end_char": sub.end_char,
+      "text": sub.text,
       "element": root.i, 
       "is_root": root.dep_=="ROOT",
       "semantic_dep": "ROOT"
     }
     store.append(_info)
   return store
 
 def _handle_half_be_going_to_root(doc:Doc, roots: list):
   store = []
   # append ROOT
   for root in roots:
     start = root.i
     end = root.i+1
+    sub = doc[start:end]
     _info = {
       "start": start,
       "end": end,
+      "start_char": sub.start_char,
+      "end_char": sub.end_char,
       "text": doc[start:end].text,
       "element": root.i, 
       "is_root": root.dep_=="ROOT",
       "semantic_dep": "ROOT"
     }
     store.append(_info)
   return store
```

### Comparing `structure_detective-0.1.5/structure_detective/en/trans_structure.py` & `structure_detective-0.1.6/structure_detective/en/trans_structure.py`

 * *Files identical despite different names*

### Comparing `structure_detective-0.1.5/structure_detective/es/morph_translation.py` & `structure_detective-0.1.6/structure_detective/es/morph_translation.py`

 * *Files identical despite different names*

### Comparing `structure_detective-0.1.5/structure_detective/es/structure.py` & `structure_detective-0.1.6/structure_detective/es/structure.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,31 +25,37 @@
     xs = ["nsubj", "cop", "obl", "punct", "dep", "aux"]
     children = [r for r in root.children if r.dep_ in xs]
     store = form_children_info(doc, children)
 
     copula_tree = get_subtree_except_xs(root, xs)
     copula_ranges = [e.i for e in copula_tree]
     start, end = min(copula_ranges), max(copula_ranges)+1
+    sub = doc[start:end]
     _info = {
       "start": start,
       "end": end,
-      "text": doc[start:end].text,
+      "start_char": sub.start_char,
+      "en_char": sub.end_char,
+      "text": sub.text,
       "element": root.i, 
       "is_root": True,
     }
     store.append(_info)
   elif _is_verb_like(root):
     children = [r for r in root.children]
     store = form_children_info(doc, children)
 
     start, end = root.i, root.i+1
+    sub = doc[start:end]
     _info = {
       "start": start,
       "end": end,
-      "text": doc[start:end].text,
+      "start_char": sub.start_char,
+      "end_char": sub.end_char,
+      "text": sub.text,
       "element": root.i, 
       "is_root": True,
     }
     store.append(_info)
   else:
     store = []
```

### Comparing `structure_detective-0.1.5/structure_detective/es/trans_structure.py` & `structure_detective-0.1.6/structure_detective/es/trans_structure.py`

 * *Files identical despite different names*

### Comparing `structure_detective-0.1.5/structure_detective/lib.py` & `structure_detective-0.1.6/structure_detective/lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,18 +44,21 @@
       tokens = [doc[x] for x in t]
       
       heads = [h for h in tokens if is_top(h, tokens)]
       assert(len(heads)==1)
       head = heads[0]
         
       start, end = min(t), max(t)+1
+      sub = doc[start:end]
       _info = {
         "start": start,
         "end": end,
-        "text": doc[start:end].text,
+        "start_char": sub.start_char,
+        "end_char": sub.end_char,
+        "text": sub.text,
         "element": head.i, 
         "is_root": False,
         "semantic_dep": head.dep_
       }
       store.append(_info)
   return store
```

### Comparing `structure_detective-0.1.5/structure_detective/structure.py` & `structure_detective-0.1.6/structure_detective/structure.py`

 * *Files identical despite different names*

