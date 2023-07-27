# Comparing `tmp/SBMLDiagrams-1.3.8.tar.gz` & `tmp/SBMLDiagrams-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SBMLDiagrams-1.3.8.tar", last modified: Fri Jul 21 00:28:32 2023, max compression
+gzip compressed data, was "dist\SBMLDiagrams-1.3.9.tar", last modified: Thu Jul 27 22:06:15 2023, max compression
```

## Comparing `SBMLDiagrams-1.3.8.tar` & `SBMLDiagrams-1.3.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 00:28:32.197172 SBMLDiagrams-1.3.8/
--rw-rw-rw-   0        0        0     2653 2023-07-21 00:28:32.198168 SBMLDiagrams-1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     1809 2023-02-23 20:31:51.000000 SBMLDiagrams-1.3.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 00:28:32.182208 SBMLDiagrams-1.3.8/SBMLDiagrams/
--rw-rw-rw-   0        0        0      784 2022-02-24 16:03:36.000000 SBMLDiagrams-1.3.8/SBMLDiagrams/__init__.py
--rw-rw-rw-   0        0        0       71 2023-07-21 00:26:46.000000 SBMLDiagrams-1.3.8/SBMLDiagrams/_version.py
--rw-rw-rw-   0        0        0   122135 2023-05-16 18:57:09.000000 SBMLDiagrams-1.3.8/SBMLDiagrams/drawNetwork.py
--rw-rw-rw-   0        0        0   123007 2023-05-16 21:57:52.000000 SBMLDiagrams-1.3.8/SBMLDiagrams/editSBML.py
--rw-rw-rw-   0        0        0   104713 2023-07-20 22:23:28.000000 SBMLDiagrams-1.3.8/SBMLDiagrams/exportSBML.py
--rw-rw-rw-   0        0        0     1631 2023-05-16 21:58:12.000000 SBMLDiagrams-1.3.8/SBMLDiagrams/point.py
--rw-rw-rw-   0        0        0   348077 2023-07-21 00:25:58.000000 SBMLDiagrams-1.3.8/SBMLDiagrams/processSBML.py
--rw-rw-rw-   0        0        0    10485 2023-05-16 21:58:22.000000 SBMLDiagrams-1.3.8/SBMLDiagrams/styleSBML.py
--rw-rw-rw-   0        0        0     1194 2023-05-16 21:58:30.000000 SBMLDiagrams-1.3.8/SBMLDiagrams/visualizeInfo.py
--rw-rw-rw-   0        0        0   158660 2023-07-20 22:35:30.000000 SBMLDiagrams-1.3.8/SBMLDiagrams/visualizeSBML.py
-drwxrwxrwx   0        0        0        0 2023-07-21 00:28:32.196147 SBMLDiagrams-1.3.8/SBMLDiagrams.egg-info/
--rw-rw-rw-   0        0        0     2653 2023-07-21 00:28:31.000000 SBMLDiagrams-1.3.8/SBMLDiagrams.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      473 2023-07-21 00:28:31.000000 SBMLDiagrams-1.3.8/SBMLDiagrams.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 00:28:31.000000 SBMLDiagrams-1.3.8/SBMLDiagrams.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      136 2023-07-21 00:28:31.000000 SBMLDiagrams-1.3.8/SBMLDiagrams.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-21 00:28:31.000000 SBMLDiagrams-1.3.8/SBMLDiagrams.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-21 00:28:32.198168 SBMLDiagrams-1.3.8/setup.cfg
--rw-rw-rw-   0        0        0     2034 2023-06-08 15:50:51.000000 SBMLDiagrams-1.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 22:06:15.837303 SBMLDiagrams-1.3.9/
+-rw-rw-rw-   0        0        0     2581 2023-07-27 22:06:15.838300 SBMLDiagrams-1.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1737 2023-07-27 19:07:56.000000 SBMLDiagrams-1.3.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 22:06:15.826362 SBMLDiagrams-1.3.9/SBMLDiagrams/
+-rw-rw-rw-   0        0        0      784 2022-02-24 16:03:36.000000 SBMLDiagrams-1.3.9/SBMLDiagrams/__init__.py
+-rw-rw-rw-   0        0        0       71 2023-07-27 22:04:56.000000 SBMLDiagrams-1.3.9/SBMLDiagrams/_version.py
+-rw-rw-rw-   0        0        0   122135 2023-05-16 18:57:09.000000 SBMLDiagrams-1.3.9/SBMLDiagrams/drawNetwork.py
+-rw-rw-rw-   0        0        0   123007 2023-05-16 21:57:52.000000 SBMLDiagrams-1.3.9/SBMLDiagrams/editSBML.py
+-rw-rw-rw-   0        0        0   104713 2023-07-20 22:23:28.000000 SBMLDiagrams-1.3.9/SBMLDiagrams/exportSBML.py
+-rw-rw-rw-   0        0        0     1631 2023-05-16 21:58:12.000000 SBMLDiagrams-1.3.9/SBMLDiagrams/point.py
+-rw-rw-rw-   0        0        0   354834 2023-07-27 21:45:43.000000 SBMLDiagrams-1.3.9/SBMLDiagrams/processSBML.py
+-rw-rw-rw-   0        0        0    10485 2023-05-16 21:58:22.000000 SBMLDiagrams-1.3.9/SBMLDiagrams/styleSBML.py
+-rw-rw-rw-   0        0        0     1194 2023-05-16 21:58:30.000000 SBMLDiagrams-1.3.9/SBMLDiagrams/visualizeInfo.py
+-rw-rw-rw-   0        0        0   158660 2023-07-20 22:35:30.000000 SBMLDiagrams-1.3.9/SBMLDiagrams/visualizeSBML.py
+drwxrwxrwx   0        0        0        0 2023-07-27 22:06:15.836305 SBMLDiagrams-1.3.9/SBMLDiagrams.egg-info/
+-rw-rw-rw-   0        0        0     2581 2023-07-27 22:06:15.000000 SBMLDiagrams-1.3.9/SBMLDiagrams.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      473 2023-07-27 22:06:15.000000 SBMLDiagrams-1.3.9/SBMLDiagrams.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 22:06:15.000000 SBMLDiagrams-1.3.9/SBMLDiagrams.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      136 2023-07-27 22:06:15.000000 SBMLDiagrams-1.3.9/SBMLDiagrams.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-27 22:06:15.000000 SBMLDiagrams-1.3.9/SBMLDiagrams.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-27 22:06:15.839304 SBMLDiagrams-1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     2034 2023-06-08 15:50:51.000000 SBMLDiagrams-1.3.9/setup.py
```

### Comparing `SBMLDiagrams-1.3.8/PKG-INFO` & `SBMLDiagrams-1.3.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SBMLDiagrams
-Version: 1.3.8
+Version: 1.3.9
 Summary: Visualize, edit and write SBML files.
 Home-page: https://github.com/sys-bio/SBMLDiagrams
 Author: Jin Xu, Jessie Jiang, Herbert M. Sauro
 Author-email: jxu2019@uw.edu
 License: MIT License
 Description: # SBMLDiagrams
         [![Coverage](https://codecov.io/gh/sunnyXu/SBMLDiagrams/branch/main/graph/badge.svg)](https://codecov.io/gh/sunnyXu/SBMLDiagrams)
@@ -19,20 +19,20 @@
         
         ## Installation
         
         ``pip install SBMLDiagrams``
         
         ## A Figure Example
         
-        Here is a figure example visualized by SBMLDiagrams below. The Bezier reactions are organized by SBcoyote (https://arxiv.org/abs/2302.09151).
+        Here is a figure example visualized by SBMLDiagrams below. 
         
-        <img src="https://raw.githubusercontent.com/SunnyXu/SBMLDiagrams/main/docs/Figures/Introduction/Jana_WolfGlycolysis.png" width="350" height="450">
+        <img src="https://raw.githubusercontent.com/SunnyXu/SBMLDiagrams/main/docs/Figures/Introduction/Jana_WolfGlycolysis-corrected.png" width="350" height="500">
         
         
-        Its animation is also available at https://youtu.be/zF3_fkDp2Xk. 
+        Its animation is also available at https://youtu.be/6VgjzrXLLoc. 
         Please see more figure examples in the documentation.
         
         ## Documentation
         Please see the documentation at https://sys-bio.github.io/SBMLDiagrams/ for details.
```

### Comparing `SBMLDiagrams-1.3.8/README.md` & `SBMLDiagrams-1.3.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 
 ## Installation
 
 ``pip install SBMLDiagrams``
 
 ## A Figure Example
 
-Here is a figure example visualized by SBMLDiagrams below. The Bezier reactions are organized by SBcoyote (https://arxiv.org/abs/2302.09151).
+Here is a figure example visualized by SBMLDiagrams below. 
 
-<img src="https://raw.githubusercontent.com/SunnyXu/SBMLDiagrams/main/docs/Figures/Introduction/Jana_WolfGlycolysis.png" width="350" height="450">
+<img src="https://raw.githubusercontent.com/SunnyXu/SBMLDiagrams/main/docs/Figures/Introduction/Jana_WolfGlycolysis-corrected.png" width="350" height="500">
 
 
-Its animation is also available at https://youtu.be/zF3_fkDp2Xk. 
+Its animation is also available at https://youtu.be/6VgjzrXLLoc. 
 Please see more figure examples in the documentation.
 
 ## Documentation
 Please see the documentation at https://sys-bio.github.io/SBMLDiagrams/ for details.
```

### Comparing `SBMLDiagrams-1.3.8/SBMLDiagrams/__init__.py` & `SBMLDiagrams-1.3.9/SBMLDiagrams/__init__.py`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.3.8/SBMLDiagrams/drawNetwork.py` & `SBMLDiagrams-1.3.9/SBMLDiagrams/drawNetwork.py`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.3.8/SBMLDiagrams/editSBML.py` & `SBMLDiagrams-1.3.9/SBMLDiagrams/editSBML.py`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.3.8/SBMLDiagrams/exportSBML.py` & `SBMLDiagrams-1.3.9/SBMLDiagrams/exportSBML.py`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.3.8/SBMLDiagrams/point.py` & `SBMLDiagrams-1.3.9/SBMLDiagrams/point.py`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.3.8/SBMLDiagrams/processSBML.py` & `SBMLDiagrams-1.3.9/SBMLDiagrams/processSBML.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import pandas as pd
 from SBMLDiagrams import exportSBML
 from SBMLDiagrams import editSBML
 from SBMLDiagrams import visualizeSBML
 from SBMLDiagrams import styleSBML
 from SBMLDiagrams import point
 import networkx as nx
+from networkx.drawing.nx_agraph import graphviz_layout
 from collections import defaultdict
 import json
 import numpy as np
 
 #create datafames for NodeData, ReactionData, CompartmentData:
 # Column names
 netIdx = 0
@@ -6571,14 +6572,15 @@
         
         """
         if filename:
             out_file = open(filename, "w")
             json.dump(self.color_style.__dict__, out_file, indent=6)
         return json.dumps(self.color_style.__dict__)
 
+    #def autolayout(self, layout="spring", scale=200., k=1., iterations=100, graphvizProgram = "dot"):
     def autolayout(self, layout="spring", scale=200., k=1., iterations=100):
 
         """
         Autolayout the node positions using networkX library.
 
         layout: str-the layout name from networkX, which can be one of the following:
 
@@ -6622,47 +6624,66 @@
             reaction_ids = model.getListOfReactionIds()
 
             width, height = self.color_style.getImageSize()
             if scale == None:
                 scale = max(width, height) // 2
             center = [width // 2, height // 2]
 
+            # # Jessie:
+            # for node in nodes:
+            #     graph.add_node(node)
+            # for edge in edges:
+            #     src = edge[0]
+            #     dests = edge[1:]
+            #     for dest in dests:
+            #         graph.add_edge(src, dest)
+            #         g[src].append(dest)
+
             for node in nodes:
                 graph.add_node(node)
-            for edge in edges:
-                src = edge[0]
-                dests = edge[1:]
-                for dest in dests:
-                    graph.add_edge(src, dest)
-                    g[src].append(dest)
+
+            for rxn in reaction_ids:
+                graph.add_node(rxn) #represent the reaction centroid as a node
+                num_rct = model.getNumReactants(rxn)
+                num_prd = model.getNumProducts(rxn)
+                for i in range(num_rct):
+                    rct = model.getReactant(rxn, i)
+                    graph.add_edge(rct, rxn)
+                for i in range(num_prd):
+                    prd = model.getProduct(rxn, i)
+                    graph.add_edge(rxn, prd)
+
 
             pos = defaultdict(list)
 
             if layout == "spring":
                 pos = nx.spring_layout(graph, scale=scale, center=center, k=k, iterations=iterations)
             elif layout == "spectral":
                 pos = nx.spectral_layout(graph, scale=scale, center=center)
             elif layout == "random":
                 pos = nx.random_layout(graph, center=center)
             elif layout == "circular":
-                pos = nx.circular_layout(graph, scale=scale, center=center)
-                 
+                pos = nx.circular_layout(graph, scale=scale, center=center)              
             # elif layout == "graphviz":
-            #     pos = nx.nx_agraph.graphviz_layout(graph, prog=graphvizProgram)
+            #     pos = graphviz_layout(graph, prog = graphvizProgram)
+
             else:
                 raise Exception("no such layout")
 
             for n, p in pos.items():
                 if layout == "random":
                     p *= scale
                 if type(p) is tuple:
                     p = list(p)
                 else:
                     p = p.tolist()
-                self.setNodeAndTextPosition(n, p)
+                try:#node position
+                    self.setNodeAndTextPosition(n, p)
+                except:#reaction centroid position
+                    self.setReactionCenterPosition(n, p)
 
             center_list = []
             handles_list = []
             line_width_list = []
             for id in reaction_ids:
                 self.setReactionDefaultCenterAndHandlePositions(id)
                 center_position = self.getReactionCenterPosition(id)
@@ -6708,15 +6729,15 @@
             #             theta2 = line_width/radius2
             #             x2 = center_position2[0] - theta2*center_position2[1]
             #             y2 = center_position2[1] + theta2*center_position2[0]
             #             center_position_2_update = [x2, y2]
             #             handles_update2 = [center_position_2_update] + handles2[1:]
             #             self.setReactionCenterPosition(id2, center_position_2_update)
             #             self.setReactionBezierHandles(id2, handles_update2)
-            # #overlap of handles from one reaction
+            #overlap of handles from one reaction
             # for k in range(len(handles_list)):
             #     overlap_handles_idx_list = []
             #     for i in range(len(handles_list[k])):
             #         for j in [x for x in range(len(handles_list[k])) if x != i]:
             #             if [(handles_list[k][i][0]-handles_list[k][j][0])**2+(handles_list[k][i][1]-handles_list[k][j][1])**2]<=2*line_width_list[k]**2:
             #                 if [i,j] not in overlap_handles_idx_list and [j,i] not in overlap_handles_idx_list:
             #                     overlap_handles_idx_list.append([i,j])
@@ -6741,15 +6762,125 @@
             #                 x2 = handle2[0] - theta2*handle2[1]
             #                 y2 = handle2[1] + theta2*handle2[0]
             #                 handle2_update = [x2, y2]
             #                 handles_update = handles_list[k]
             #                 handles_update[idx] = handle_update
             #                 handles_update[idx2] = handle2_update
             #                 self.setReactionBezierHandles(id, handles_update)
-                
+
+    def centroidOverLap(self):
+        sbmlStr = self.export()
+        model = simplesbml.loadSBMLStr(sbmlStr)
+        reaction_ids = model.getListOfReactionIds()
+        center_list = []
+        handles_list = []
+        line_width_list = []
+        for id in reaction_ids:
+            self.setReactionDefaultCenterAndHandlePositions(id)
+            center_position = self.getReactionCenterPosition(id)
+            handles = self.getReactionBezierHandles(id)
+            center_list.append([center_position.x, center_position.y])
+            handles_list_pre = []
+            for i in range(len(handles)):
+                handles_list_pre.append([handles[i].x, handles[i].y])
+            handles_list.append(handles_list_pre)
+            line_width_list.append(self.getReactionLineThickness(id))
+        
+        #overlap of centroids from different reactions
+        overlap_center_idx_list = []
+        for i in range(len(center_list)):
+            for j in [x for x in range(len(center_list)) if x != i]:
+                if [(center_list[i][0]-center_list[j][0])**2+(center_list[i][1]-center_list[j][1])**2]<=2*line_width_list[i]**2:
+                    if [i,j] not in overlap_center_idx_list and [j,i] not in overlap_center_idx_list:
+                        overlap_center_idx_list.append([i,j])
+        
+        for i in range(len(overlap_center_idx_list)):
+            idx = overlap_center_idx_list[i][0]
+            idx2 = overlap_center_idx_list[i][1]
+            id = reaction_ids[idx]
+            id2 = reaction_ids[idx2]
+            center_position = center_list[idx]
+            center_position2 = center_list[idx2]
+            handle_rct1 = handles_list[idx][1]
+            handle_rct1_2 = handles_list[idx2][1]
+            handles = handles_list[idx]
+            handles2 = handles_list[idx2]
+            line_width = line_width_list[idx]
+            radius = math.dist(center_position, handle_rct1)
+            if radius != 0:
+                theta = line_width/radius
+                x = center_position[0] + theta*center_position[1]
+                y = center_position[1] - theta*center_position[0]
+                center_position_update = [x, y]
+                handles_update = [center_position_update] + handles[1:]
+                self.setReactionCenterPosition(id, center_position_update)
+                self.setReactionBezierHandles(id, handles_update)
+                radius2 = math.dist(center_position2, handle_rct1_2)
+                if radius2 !=0 :
+                    theta2 = line_width/radius2
+                    x2 = center_position2[0] - theta2*center_position2[1]
+                    y2 = center_position2[1] + theta2*center_position2[0]
+                    center_position_2_update = [x2, y2]
+                    handles_update2 = [center_position_2_update] + handles2[1:]
+                    self.setReactionCenterPosition(id2, center_position_2_update)
+                    self.setReactionBezierHandles(id2, handles_update2)
+
+    def HandleOverLap(self):
+        sbmlStr = self.export()
+        model = simplesbml.loadSBMLStr(sbmlStr)
+        reaction_ids = model.getListOfReactionIds()
+        center_list = []
+        handles_list = []
+        line_width_list = []
+        for id in reaction_ids:
+            self.setReactionDefaultCenterAndHandlePositions(id)
+            center_position = self.getReactionCenterPosition(id)
+            handles = self.getReactionBezierHandles(id)
+            center_list.append([center_position.x, center_position.y])
+            handles_list_pre = []
+            for i in range(len(handles)):
+                handles_list_pre.append([handles[i].x, handles[i].y])
+            handles_list.append(handles_list_pre)
+            line_width_list.append(self.getReactionLineThickness(id))
+
+        #overlap of handles from one reaction
+        for k in range(len(handles_list)):
+            overlap_handles_idx_list = []
+            for i in range(len(handles_list[k])):
+                for j in [x for x in range(len(handles_list[k])) if x != i]:
+                    if [(handles_list[k][i][0]-handles_list[k][j][0])**2+(handles_list[k][i][1]-handles_list[k][j][1])**2]<=2*line_width_list[k]**2:
+                        if [i,j] not in overlap_handles_idx_list and [j,i] not in overlap_handles_idx_list:
+                            overlap_handles_idx_list.append([i,j])
+            for i in range(len(overlap_handles_idx_list)):
+                idx = overlap_handles_idx_list[i][0]
+                idx2 = overlap_handles_idx_list[i][1]
+                center_position = center_list[k]
+                handle = handles_list[k][idx]
+                handle2 = handles_list[k][idx2]
+                id = reaction_ids[k]
+                line_width = line_width_list[k]
+                #print(center_position, handle, handle2, id, line_width)
+                radius = math.dist(center_position, handle)
+                if radius != 0:
+                    theta = line_width/radius
+                    x = handle[0] + theta*handle[1]
+                    y = handle[1] - theta*handle[0]
+                    handle_update = [x, y]
+                    radius2 = math.dist(center_position, handle2)   
+                    if radius2 != 0:
+                        theta2 = line_width/radius
+                        x2 = handle2[0] - theta2*handle2[1]
+                        y2 = handle2[1] + theta2*handle2[0]
+                        handle2_update = [x2, y2]
+                        handles_update = handles_list[k]
+                        handles_update[idx] = handle_update
+                        handles_update[idx2] = handle2_update
+                        self.setReactionBezierHandles(id, handles_update)
+
+
     def draw(self, setImageSize = [], scale = 1., output_fileName = '', 
         reactionLineType = 'bezier', showBezierHandles = False, 
         showReactionIds = False, showReversible = False, longText = 'auto-font'):
 
         """
         Draw to a PNG/JPG/PDF file.
 
@@ -6991,15 +7122,15 @@
 
         nx.write_graphml_lxml(graph, output_fileName + ".graphml")
 
 if __name__ == '__main__':
     DIR = os.path.dirname(os.path.abspath(__file__))
     TEST_FOLDER = os.path.join(DIR, "test_sbml_files")
     
-    filename = "test.xml" 
+    #filename = "test.xml" 
     #filename = "feedback.xml"
     #filename = "LinearChain.xml"
     #filename = "test_comp.xml"
     #filename = "test_no_comp.xml"
     #filename = "test_modifier.xml"
     #filename = "node_grid.xml"
     #filename = "mass_action_rxn.xml"
@@ -7013,14 +7144,16 @@
     
     #gradient: 
     #filename = "test_suite/test_gradientLinear/test_gradientLinear.xml"
     #filename = "test_suite/test_gradientRadial/test_gradientRadial.xml"
 
     #long text and alias nodes
     #filename = "test_suite/Jana_WolfGlycolysis/Jana_WolfGlycolysis.xml"
+    #filename = "test_suite/Jana_WolfGlycolysis/Jana_WolfGlycolysis-original.xml"
+    #filename = "test_suite/Jana_WolfGlycolysis/Jana_WolfGlycolysis-corrected.xml"
 
     #sbml with errors
     #filename = "test_suite/sbml_error/testbigmodel.xml"
 
     #global render
     #filename = "test_suite/global_render/global_render.xml"
 
@@ -7066,15 +7199,15 @@
 
     #filename = "additional/BrusselatorWithOutJD.xml"
     #filename = "additional/BorisEJB_layoutrender.xml"
     #filename = "additional/m2.xml"
     #filename = "additional/small.xml"
     #filename = "additional/ecoli.xml"
     #filename = "additional/straight_line.xml"
-    #filename = "additional/E_coli_Millard2016.xml"
+    filename = "additional/E_coli_Millard2016.xml"
 
     
 
     f = open(os.path.join(TEST_FOLDER, filename), 'r')
     sbmlStr = f.read()
     f.close()
 
@@ -7351,15 +7484,15 @@
 
     # r = te.loada ('''
     # S1 + S2 -> S2; v;
     # v = 0
     # ''')
 
     # df = load(r.getSBML())
-    # df.autolayout()
+    # df.autolayout(layout = "circular", scale = 500)
     # df.draw(output_fileName = 'output.png')
 
     sbmlStr_layout_render = df.export()
     f = open("output.xml", "w")
     f.write(sbmlStr_layout_render)
     f.close()
```

### Comparing `SBMLDiagrams-1.3.8/SBMLDiagrams/styleSBML.py` & `SBMLDiagrams-1.3.9/SBMLDiagrams/styleSBML.py`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.3.8/SBMLDiagrams/visualizeInfo.py` & `SBMLDiagrams-1.3.9/SBMLDiagrams/visualizeInfo.py`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.3.8/SBMLDiagrams/visualizeSBML.py` & `SBMLDiagrams-1.3.9/SBMLDiagrams/visualizeSBML.py`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.3.8/SBMLDiagrams.egg-info/PKG-INFO` & `SBMLDiagrams-1.3.9/SBMLDiagrams.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SBMLDiagrams
-Version: 1.3.8
+Version: 1.3.9
 Summary: Visualize, edit and write SBML files.
 Home-page: https://github.com/sys-bio/SBMLDiagrams
 Author: Jin Xu, Jessie Jiang, Herbert M. Sauro
 Author-email: jxu2019@uw.edu
 License: MIT License
 Description: # SBMLDiagrams
         [![Coverage](https://codecov.io/gh/sunnyXu/SBMLDiagrams/branch/main/graph/badge.svg)](https://codecov.io/gh/sunnyXu/SBMLDiagrams)
@@ -19,20 +19,20 @@
         
         ## Installation
         
         ``pip install SBMLDiagrams``
         
         ## A Figure Example
         
-        Here is a figure example visualized by SBMLDiagrams below. The Bezier reactions are organized by SBcoyote (https://arxiv.org/abs/2302.09151).
+        Here is a figure example visualized by SBMLDiagrams below. 
         
-        <img src="https://raw.githubusercontent.com/SunnyXu/SBMLDiagrams/main/docs/Figures/Introduction/Jana_WolfGlycolysis.png" width="350" height="450">
+        <img src="https://raw.githubusercontent.com/SunnyXu/SBMLDiagrams/main/docs/Figures/Introduction/Jana_WolfGlycolysis-corrected.png" width="350" height="500">
         
         
-        Its animation is also available at https://youtu.be/zF3_fkDp2Xk. 
+        Its animation is also available at https://youtu.be/6VgjzrXLLoc. 
         Please see more figure examples in the documentation.
         
         ## Documentation
         Please see the documentation at https://sys-bio.github.io/SBMLDiagrams/ for details.
```

### Comparing `SBMLDiagrams-1.3.8/setup.py` & `SBMLDiagrams-1.3.9/setup.py`

 * *Files identical despite different names*

