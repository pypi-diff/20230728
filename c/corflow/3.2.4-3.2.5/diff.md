# Comparing `tmp/corflow-3.2.4.tar.gz` & `tmp/corflow-3.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corflow-3.2.4.tar", last modified: Mon Mar 13 11:26:35 2023, max compression
+gzip compressed data, was "corflow-3.2.5.tar", last modified: Fri Jul 28 12:35:45 2023, max compression
```

## Comparing `corflow-3.2.4.tar` & `corflow-3.2.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-03-13 11:26:35.934256 corflow-3.2.4/
--rw-rw-rw-   0        0        0     5619 2023-03-13 11:26:35.934256 corflow-3.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     4986 2022-08-22 09:32:28.000000 corflow-3.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-03-13 11:26:35.928249 corflow-3.2.4/corflow/
--rw-rw-rw-   0        0        0    52491 2023-02-09 14:25:28.000000 corflow-3.2.4/corflow/Transcription.py
--rw-rw-rw-   0        0        0        0 2022-08-23 06:37:46.000000 corflow-3.2.4/corflow/__init__.py
--rw-rw-rw-   0        0        0    13989 2023-03-13 11:09:59.000000 corflow-3.2.4/corflow/fromElan.py
--rw-rw-rw-   0        0        0    10308 2023-01-25 10:31:26.000000 corflow-3.2.4/corflow/fromExmaralda.py
--rw-rw-rw-   0        0        0    10905 2023-01-25 10:31:26.000000 corflow-3.2.4/corflow/fromPangloss.py
--rw-rw-rw-   0        0        0    15905 2023-01-25 10:31:26.000000 corflow-3.2.4/corflow/fromPraat.py
--rw-rw-rw-   0        0        0    10385 2023-01-25 10:31:26.000000 corflow-3.2.4/corflow/fromTranscriber.py
--rw-rw-rw-   0        0        0    19393 2023-03-13 11:17:55.000000 corflow-3.2.4/corflow/toElan.py
--rw-rw-rw-   0        0        0     9222 2023-01-26 08:34:26.000000 corflow-3.2.4/corflow/toExmaralda.py
--rw-rw-rw-   0        0        0    13448 2023-01-25 10:31:26.000000 corflow-3.2.4/corflow/toPangloss.py
--rw-rw-rw-   0        0        0     8957 2023-01-25 10:31:26.000000 corflow-3.2.4/corflow/toPraat.py
--rw-rw-rw-   0        0        0    11535 2023-01-25 10:31:26.000000 corflow-3.2.4/corflow/toTEI.py
--rw-rw-rw-   0        0        0    10555 2023-01-26 08:45:12.000000 corflow-3.2.4/corflow/toTranscriber.py
-drwxrwxrwx   0        0        0        0 2023-03-13 11:26:35.933256 corflow-3.2.4/corflow.egg-info/
--rw-rw-rw-   0        0        0     5619 2023-03-13 11:26:35.000000 corflow-3.2.4/corflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-03-13 11:26:35.000000 corflow-3.2.4/corflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-13 11:26:35.000000 corflow-3.2.4/corflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-03-13 11:26:35.000000 corflow-3.2.4/corflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      732 2023-03-13 11:25:56.000000 corflow-3.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-13 11:26:35.934256 corflow-3.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 12:35:45.679384 corflow-3.2.5/
+-rw-rw-rw-   0        0        0     5619 2023-07-28 12:35:45.679384 corflow-3.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4986 2022-08-22 09:32:28.000000 corflow-3.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 12:35:45.679384 corflow-3.2.5/corflow/
+-rw-rw-rw-   0        0        0    51722 2023-07-28 12:32:21.000000 corflow-3.2.5/corflow/Transcription.py
+-rw-rw-rw-   0        0        0        0 2022-08-23 06:37:46.000000 corflow-3.2.5/corflow/__init__.py
+-rw-rw-rw-   0        0        0    13989 2023-03-13 11:09:59.000000 corflow-3.2.5/corflow/fromElan.py
+-rw-rw-rw-   0        0        0    10308 2023-01-25 10:31:26.000000 corflow-3.2.5/corflow/fromExmaralda.py
+-rw-rw-rw-   0        0        0    10905 2023-01-25 10:31:26.000000 corflow-3.2.5/corflow/fromPangloss.py
+-rw-rw-rw-   0        0        0    15905 2023-01-25 10:31:26.000000 corflow-3.2.5/corflow/fromPraat.py
+-rw-rw-rw-   0        0        0    10385 2023-01-25 10:31:26.000000 corflow-3.2.5/corflow/fromTranscriber.py
+-rw-rw-rw-   0        0        0    19393 2023-03-13 11:17:55.000000 corflow-3.2.5/corflow/toElan.py
+-rw-rw-rw-   0        0        0     9222 2023-01-26 08:34:26.000000 corflow-3.2.5/corflow/toExmaralda.py
+-rw-rw-rw-   0        0        0    13448 2023-01-25 10:31:26.000000 corflow-3.2.5/corflow/toPangloss.py
+-rw-rw-rw-   0        0        0     8957 2023-01-25 10:31:26.000000 corflow-3.2.5/corflow/toPraat.py
+-rw-rw-rw-   0        0        0    11535 2023-01-25 10:31:26.000000 corflow-3.2.5/corflow/toTEI.py
+-rw-rw-rw-   0        0        0    10555 2023-01-26 08:45:12.000000 corflow-3.2.5/corflow/toTranscriber.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:35:45.679384 corflow-3.2.5/corflow.egg-info/
+-rw-rw-rw-   0        0        0     5619 2023-07-28 12:35:45.000000 corflow-3.2.5/corflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-07-28 12:35:45.000000 corflow-3.2.5/corflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 12:35:45.000000 corflow-3.2.5/corflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-28 12:35:45.000000 corflow-3.2.5/corflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      732 2023-07-28 12:33:51.000000 corflow-3.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-28 12:35:45.679384 corflow-3.2.5/setup.cfg
```

### Comparing `corflow-3.2.4/PKG-INFO` & `corflow-3.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corflow
-Version: 3.2.4
+Version: 3.2.5
 Summary: A conversion/manipulation tool for oral linguistics.
 Author-email: François Delafontaine <francois.delafontaine@unine.ch>
 License: CC-BY-4.0
 Project-URL: repository, https://github.com/DoReCo/corflow
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `corflow-3.2.4/README.md` & `corflow-3.2.5/README.md`

 * *Files identical despite different names*

### Comparing `corflow-3.2.4/corflow/Transcription.py` & `corflow-3.2.5/corflow/Transcription.py`

 * *Files 1% similar despite different names*

```diff
@@ -782,57 +782,45 @@
         """Sorts the segments by time code.
         Note: let's not reinvent the wheel, we'll rely on 'sort()'."""
         def getStart(el):
             return el.start
         self.elem.sort(key=getStart)
         for a in range(len(self.elem)):
             self.d_elem[self.elem[a]][0] = a
-    def fixOverlaps(self,cont=""):
+    def fixOverlaps(self,cont="",sort=False):
         """Looks for segment overlaps and tries to fix it."""
-        def _addASeg(atier,seg):
-            aseg = atier.create(-1,"",seg.start,seg.end,seg.content)
-            aseg.setMeta("oseg",seg,"tech")
-            return aseg
+        ls = len(self)
+        if ls < 2:
+            return
         atier = self.copy(empty=True)
-        for a in range(len(self.elem)-1,-1,-1):
-            seg = self.elem[a]
-            aseg = atier.findTime(seg.start)
-            if not aseg: # Tier start
-                if not atier.elem: # First segment
-                    _addASeg(atier,seg); continue
-                aseg = atier.elem[0]
-            while aseg.start > seg.end: # All overlapped segments
-                if seg.start < aseg.start and seg.end < aseg.end: # mid-left
-                    if (not cont) or (cont in seg.content):
-                        seg.end = aseg.start
-                    else:
-                        aseg.meta("oseg","tech").start = seg.end
-                    break
-                elif seg.start > aseg.start and seg.end > aseg.end: # mid-right
-                    if (not cont) or (cont in seg.content):
-                        seg.start = aseg.end
-                    else:
-                        aseg.meta("oseg","tech").end = seg.start
-                elif seg.start <= aseg.start and seg.end >= aseg.end: # mid
-                    if (not cont) or (cont in seg.content):
-                        self.pop(a); break
-                    else:
-                        oseg = aseg.meta("oseg","tech")
-                        self.remove(oseg); atier.remove(aseg)
-            _addASeg(atier,seg)
+        if sort:
+            self.sortByTime()
+        for a in range(1,ls): # first pass, no overlap
+            s1,s2 = self.elem[a-1],self.elem[a]
+            if s1.end > s2.start:
+                if cont and re.search(cont,s1.content):
+                    s2.start = s1.end
+                else:
+                    s1.end = s2.start
+        for a in range(ls-1,-1,-1): # second path, only valid segments
+            s = self.elem[a]
+            if s.end <= s.start:
+                continue
+            atier.add(0,s)
+        self.struct.elem[self.index()] = atier # replace
+        self.elem,self.d_elem = atier.elem,atier.d_elem
+        return self._retDet(atier,det)
     def fixGaps(self,sym="_"):
         """Adds segments in gaps."""
-        
         ls = len(self)
         if self.elem and self.elem[-1].end < self.end:      # End
             self.create(ls,"a",self.elem[-1].end,self.end,sym)
         for a in range(ls-1,0,-1):                                  # Middle
             if self.elem[a-1].end < self.elem[a].start:
-                self.create(a,"a",self.elem[a-1].end,
-                            self.elem[a].start,sym)
+                self.create(a,"a",self.elem[a-1].end,self.elem[a].start,sym)
         if self.elem and self.elem[0].start > self.start:   # Start
             self.create(0,"a",self.start,self.elem[0].start,sym)
     def remGaps(self,sym="_"):
         """Removes segments meant to be gaps."""
         
         for a in range(len(self)-1,-1,-1):
             seg = self.elem[a]
```

### Comparing `corflow-3.2.4/corflow/fromElan.py` & `corflow-3.2.5/corflow/fromElan.py`

 * *Files identical despite different names*

### Comparing `corflow-3.2.4/corflow/fromExmaralda.py` & `corflow-3.2.5/corflow/fromExmaralda.py`

 * *Files identical despite different names*

### Comparing `corflow-3.2.4/corflow/fromPangloss.py` & `corflow-3.2.5/corflow/fromPangloss.py`

 * *Files identical despite different names*

### Comparing `corflow-3.2.4/corflow/fromPraat.py` & `corflow-3.2.5/corflow/fromPraat.py`

 * *Files identical despite different names*

### Comparing `corflow-3.2.4/corflow/fromTranscriber.py` & `corflow-3.2.5/corflow/fromTranscriber.py`

 * *Files identical despite different names*

### Comparing `corflow-3.2.4/corflow/toElan.py` & `corflow-3.2.5/corflow/toElan.py`

 * *Files identical despite different names*

### Comparing `corflow-3.2.4/corflow/toExmaralda.py` & `corflow-3.2.5/corflow/toExmaralda.py`

 * *Files identical despite different names*

### Comparing `corflow-3.2.4/corflow/toPangloss.py` & `corflow-3.2.5/corflow/toPangloss.py`

 * *Files identical despite different names*

### Comparing `corflow-3.2.4/corflow/toPraat.py` & `corflow-3.2.5/corflow/toPraat.py`

 * *Files identical despite different names*

### Comparing `corflow-3.2.4/corflow/toTEI.py` & `corflow-3.2.5/corflow/toTEI.py`

 * *Files identical despite different names*

### Comparing `corflow-3.2.4/corflow/toTranscriber.py` & `corflow-3.2.5/corflow/toTranscriber.py`

 * *Files identical despite different names*

### Comparing `corflow-3.2.4/corflow.egg-info/PKG-INFO` & `corflow-3.2.5/corflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corflow
-Version: 3.2.4
+Version: 3.2.5
 Summary: A conversion/manipulation tool for oral linguistics.
 Author-email: François Delafontaine <francois.delafontaine@unine.ch>
 License: CC-BY-4.0
 Project-URL: repository, https://github.com/DoReCo/corflow
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `corflow-3.2.4/pyproject.toml` & `corflow-3.2.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "corflow"
-version = "3.2.4"
+version = "3.2.5"
 description = "A conversion/manipulation tool for oral linguistics."
 authors = [
 	{name = "François Delafontaine", email = "francois.delafontaine@unine.ch"},
 ]
 readme = "README.md"
 requires-python = ">= 3.10"
 license = {text = "CC-BY-4.0"}
```

