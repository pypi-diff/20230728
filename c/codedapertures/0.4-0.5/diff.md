# Comparing `tmp/codedapertures-0.4.tar.gz` & `tmp/codedapertures-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedapertures-0.4.tar", last modified: Tue Jul 25 00:59:06 2023, max compression
+gzip compressed data, was "codedapertures-0.5.tar", last modified: Fri Jul 28 00:11:12 2023, max compression
```

## Comparing `codedapertures-0.4.tar` & `codedapertures-0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-25 00:59:06.202970 codedapertures-0.4/
--rw-r--r--   0 bbudden    (501) staff       (20)     1062 2023-01-26 02:12:38.000000 codedapertures-0.4/LICENSE
--rw-r--r--   0 bbudden    (501) staff       (20)      720 2023-07-25 00:59:06.202849 codedapertures-0.4/PKG-INFO
--rw-r--r--   0 bbudden    (501) staff       (20)     1743 2023-07-25 00:21:35.000000 codedapertures-0.4/README.md
-drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-25 00:59:06.201928 codedapertures-0.4/codedapertures/
--rw-r--r--   0 bbudden    (501) staff       (20)       30 2023-01-26 02:12:38.000000 codedapertures-0.4/codedapertures/__init__.py
--rw-r--r--   0 bbudden    (501) staff       (20)    16567 2023-07-25 00:54:26.000000 codedapertures-0.4/codedapertures/codedapertures.py
-drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-25 00:59:06.202687 codedapertures-0.4/codedapertures.egg-info/
--rw-r--r--   0 bbudden    (501) staff       (20)      720 2023-07-25 00:59:06.000000 codedapertures-0.4/codedapertures.egg-info/PKG-INFO
--rw-r--r--   0 bbudden    (501) staff       (20)      312 2023-07-25 00:59:06.000000 codedapertures-0.4/codedapertures.egg-info/SOURCES.txt
--rw-r--r--   0 bbudden    (501) staff       (20)        1 2023-07-25 00:59:06.000000 codedapertures-0.4/codedapertures.egg-info/dependency_links.txt
--rw-r--r--   0 bbudden    (501) staff       (20)        1 2023-07-06 00:30:22.000000 codedapertures-0.4/codedapertures.egg-info/not-zip-safe
--rw-r--r--   0 bbudden    (501) staff       (20)       26 2023-07-25 00:59:06.000000 codedapertures-0.4/codedapertures.egg-info/requires.txt
--rw-r--r--   0 bbudden    (501) staff       (20)       15 2023-07-25 00:59:06.000000 codedapertures-0.4/codedapertures.egg-info/top_level.txt
--rw-r--r--   0 bbudden    (501) staff       (20)       38 2023-07-25 00:59:06.203002 codedapertures-0.4/setup.cfg
--rw-r--r--   0 bbudden    (501) staff       (20)      891 2023-07-25 00:57:02.000000 codedapertures-0.4/setup.py
+drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-28 00:11:12.507591 codedapertures-0.5/
+-rw-r--r--   0 bbudden    (501) staff       (20)     1062 2023-01-26 02:12:38.000000 codedapertures-0.5/LICENSE
+-rw-r--r--   0 bbudden    (501) staff       (20)      720 2023-07-28 00:11:12.507484 codedapertures-0.5/PKG-INFO
+-rw-r--r--   0 bbudden    (501) staff       (20)     1743 2023-07-25 00:21:35.000000 codedapertures-0.5/README.md
+drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-28 00:11:12.506647 codedapertures-0.5/codedapertures/
+-rw-r--r--   0 bbudden    (501) staff       (20)       30 2023-01-26 02:12:38.000000 codedapertures-0.5/codedapertures/__init__.py
+-rw-r--r--   0 bbudden    (501) staff       (20)    20181 2023-07-27 23:50:09.000000 codedapertures-0.5/codedapertures/codedapertures.py
+drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-28 00:11:12.507354 codedapertures-0.5/codedapertures.egg-info/
+-rw-r--r--   0 bbudden    (501) staff       (20)      720 2023-07-28 00:11:12.000000 codedapertures-0.5/codedapertures.egg-info/PKG-INFO
+-rw-r--r--   0 bbudden    (501) staff       (20)      312 2023-07-28 00:11:12.000000 codedapertures-0.5/codedapertures.egg-info/SOURCES.txt
+-rw-r--r--   0 bbudden    (501) staff       (20)        1 2023-07-28 00:11:12.000000 codedapertures-0.5/codedapertures.egg-info/dependency_links.txt
+-rw-r--r--   0 bbudden    (501) staff       (20)        1 2023-07-06 00:30:22.000000 codedapertures-0.5/codedapertures.egg-info/not-zip-safe
+-rw-r--r--   0 bbudden    (501) staff       (20)       26 2023-07-28 00:11:12.000000 codedapertures-0.5/codedapertures.egg-info/requires.txt
+-rw-r--r--   0 bbudden    (501) staff       (20)       15 2023-07-28 00:11:12.000000 codedapertures-0.5/codedapertures.egg-info/top_level.txt
+-rw-r--r--   0 bbudden    (501) staff       (20)       38 2023-07-28 00:11:12.507624 codedapertures-0.5/setup.cfg
+-rw-r--r--   0 bbudden    (501) staff       (20)      891 2023-07-28 00:08:18.000000 codedapertures-0.5/setup.py
```

### Comparing `codedapertures-0.4/LICENSE` & `codedapertures-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `codedapertures-0.4/PKG-INFO` & `codedapertures-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedapertures
-Version: 0.4
+Version: 0.5
 Summary: a python package for generating coded apertures
 Home-page: https://github.com/bpops/codedapertures
 Author: bpops
 License: MIT
 License-File: LICENSE
 
 CodedApertures is a python package that allows one to easily generate and display common coded aperture patterns. Coded apertures are a spatial encoding technique for straight-line optics, wherein traditional lensing (e.g., visible light) is not possible. Even wherein tradiational lensing is possible, there may be other advantages (infinite depth of field). Coded apertures may therefore be used for hard x-ray and gamma-ray imaging for astrophysics, medical imaging, and homeland security applications.
```

### Comparing `codedapertures-0.4/README.md` & `codedapertures-0.5/README.md`

 * *Files identical despite different names*

### Comparing `codedapertures-0.4/codedapertures/codedapertures.py` & `codedapertures-0.5/codedapertures/codedapertures.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,40 +15,23 @@
 import numpy              as     np
 import matplotlib.pyplot  as     plt
 from   matplotlib.patches import RegularPolygon
 import pyprimes
 import random
 
 
-class mask():
+class mask_sq():
     """
     Mask
 
-    Holds one of several types of coded aperture patterns.
+    Holds one of several types of square coded aperture patterns.
     """
 
     def __init__(self):
         self.A_ij = None
-    
-    def show(self, inverse=False, size=8):
-        """
-        Plots the mask to the screen
-
-        Parameters
-        ----------
-        inverse : bool
-            if True, will invert the array before plotting
-        size : int
-            size of the plot (default 8)
-        """
-        plt.rcParams['figure.figsize'] = [size,size]
-        cmap = "binary_r" if inverse else "binary"
-        plt.imshow(np.transpose(self.A_ij), cmap=cmap, aspect=1)
-        plt.axis('off')
-        plt.show()
 
     def get_pattern(self, inverse=False):
         """
         Returns the pattern as an array
 
         Parameters
         ----------
@@ -77,15 +60,15 @@
         new_height = self.height + width*2
         new_mask   = np.zeros((new_width, new_height))
         if not empty: new_mask = new_mask +1
         new_mask[width:-width,width:-width] = self.A_ij
         self.A_ij  = new_mask
 
 
-class rand_1d(mask):
+class rand_1d(mask_sq):
     """
     Random 1-dimensional Array
 
     Parameters
     ----------
     x : int
         number of 'x' elements in the array
@@ -141,15 +124,33 @@
         A_ij : ndarrray
             the 2D (or 1D, if selected) boolean mask
         """
         mask = 1-self.A_ij if inverse else self.A_ij
         if collapse: mask = mask[:,0]
         return mask
 
-class rand_2d(mask):
+    def show(self, inverse=False, size=8):
+        """
+        Plots the mask to the screen
+
+        Parameters
+        ----------
+        inverse : bool
+            if True, will invert the array before plotting
+        size : int
+            size of the plot (default 8)
+        """
+        plt.rcParams['figure.figsize'] = [size,size]
+        cmap = "binary_r" if inverse else "binary"
+        plt.imshow(np.transpose(self.A_ij), cmap=cmap, aspect=1)
+        plt.axis('off')
+        plt.title("Random 1D")
+        plt.show()
+
+class rand_2d(mask_sq):
     """
     Random 2-dimensional Array
 
     Parameters
     ----------
     x : int
         number of 'x' elements in the array
@@ -186,16 +187,33 @@
         Report on the mask information
         """
         print("Random 2D Array")
         print(f"x, y: {self.r}, {self.s}")
         print(f"desired fill factor: {self.fill:.2f}")
         print(f"actual  fill factor: {self.actual_fill:.2f}")
 
+    def show(self, inverse=False, size=8):
+        """
+        Plots the mask to the screen
 
-class ura(mask):
+        Parameters
+        ----------
+        inverse : bool
+            if True, will invert the array before plotting
+        size : int
+            size of the plot (default 8)
+        """
+        plt.rcParams['figure.figsize'] = [size,size]
+        cmap = "binary_r" if inverse else "binary"
+        plt.imshow(np.transpose(self.A_ij), cmap=cmap, aspect=1)
+        plt.axis('off')
+        plt.title("Random 2D")
+        plt.show()
+
+class ura(mask_sq):
     """
     Uniformly Redundant Array
 
     Parameters
     ----------
     rank : int
         the rank of prime pairs to use (0 -> (5,3) 1 -> (13,11) etc.)
@@ -283,16 +301,33 @@
             else:
                 p1 = p2
             if this_rank == rank:
                 break
 
         return p1, p2
 
+    def show(self, inverse=False, size=8):
+        """
+        Plots the mask to the screen
+
+        Parameters
+        ----------
+        inverse : bool
+            if True, will invert the array before plotting
+        size : int
+            size of the plot (default 8)
+        """
+        plt.rcParams['figure.figsize'] = [size,size]
+        cmap = "binary_r" if inverse else "binary"
+        plt.imshow(np.transpose(self.A_ij), cmap=cmap, aspect=1)
+        plt.axis('off')
+        plt.title("URA")
+        plt.show()
 
-class mura(mask):
+class mura(mask_sq):
     """
     Modified Uniformly Redundant Array
 
     Parameters
     ----------
     rank : int
         the rank of prime pairs to use (0 -> (5,3) 1 -> (13,11) etc.)
@@ -370,76 +405,110 @@
             if pyprimes.isprime(L):
                 this_rank += 1
             if this_rank == rank:
                 break
             m += 1
         return L
     
-class shura(mask):
+    def show(self, inverse=False, size=8):
+        """
+        Plots the mask to the screen
+
+        Parameters
+        ----------
+        inverse : bool
+            if True, will invert the array before plotting
+        size : int
+            size of the plot (default 8)
+        """
+        plt.rcParams['figure.figsize'] = [size,size]
+        cmap = "binary_r" if inverse else "binary"
+        plt.imshow(np.transpose(self.A_ij), cmap=cmap, aspect=1)
+        plt.axis('off')
+        plt.title("MURA")
+        plt.show()
+
+class shura():
     """
     Skew-Hadamard Uniformly Redundant Array
 
     Parameters
     ----------
     n : int
         determines the order, v, where v=4n-1 (default 6)
     r : int
         feeds into pattern (default 5)
-    mult : int
-        multiplier (default 10)
     quiet : bool
         if True, will print information about the array upon creation
     """
 
-    def __init__(self, n=6, r=5, mult=4, quiet=False):
+    def __init__(self, n=6, r=5, radius=5, quiet=False):
         self.n    = n
         self.r    = r
-        self.mult = mult
-        
+
+        # calculate mask size
+        self.radius       = radius
+        self.diam         = self.radius*2+1
+        self.side_width   = radius + 1
+
+        # create axial matrix
+        self.axial_matrix = np.zeros((self.diam,self.diam))
+        self.loc_matrix   = np.zeros((2,self.diam,self.diam))
+
         # calculate intermediates
         self.v   = 4*n-1
         self.k   = 2*n-1
         self.lam = n-1
 
         # construct cyclic difference set D
         self.D = np.zeros((int((self.v-1)/2)), dtype=np.int32)
         for i in range(len(self.D)):
             self.D[i] = ((i+1)**2) % self.v
 
         # determine labels
-        rx = r*mult
-        self.l = np.zeros((rx,rx))
-        for i in range(rx):
-            for j in range(rx):
+        self.rx = self.diam
+        self.ry = self.diam
+        self.l = np.zeros((self.rx,self.ry))
+        for i in range(self.rx):
+            for j in range(self.ry):
                 self.l[i,j] = (i + r*j) % self.v
 
         # calculate mask
         self.mask = np.zeros(self.l.shape)
         for i in range(self.mask.shape[0]):
             for j in range(self.mask.shape[1]):
                 if self.l[i,j] in self.D:
                     self.mask[i,j] = 1
 
+        # map to axial matrix
+        for i in range(self.diam):
+            for j in range(self.diam):
+                if (i+j > (self.radius-1)) and (i+j < (self.diam+self.radius)):
+                    # this next line should not work correctly. WHY does it work?
+                    self.axial_matrix[i,j] = self.mask[i,j]
+                else:
+                    self.axial_matrix[i,j] = np.nan
+
         if not quiet: self.report()
 
     def report(self):
         """
         Report the array info
         """
         print("Skew-Hadamard Uniformly Redundant Array")
         print(f"n: {self.n}")
         print(f"order (v): {self.v}")
         print(f"k: {self.k}")
         print(f"lambda: {self.lam}")
         print(f"r: {self.r}")
-        print(f"multiplier: {self.mult}")
-
-    def show(self):
+        print(f"side: {self.side_width}")
+  
+    def show_rhombus(self):
         """
-        Plot the mask
+        Plot the mask rhombus
         """
 
         # determine open/closed pixels
         pix_close  = np.where(self.mask == 1)
         pix_open   = np.where(self.mask == 0)
         
         # determine open/closed pixels
@@ -458,15 +527,15 @@
         for x, y in zip (x_closed, y_closed):
 
             # determine patch origin
             x += y * 0.5
             y *= 1/hex_vert
 
             # recenter
-            x -= (self.mask.shape[0] + self.mask.shape[1]/2.0)/2.0
+            x -= (self.mask.shape[0] + self.mask.shape[1]/2.0)/2.0 -1/hex_vert
             y -= (self.mask.shape[1] * 1/hex_vert)/2.0
 
             # add hexagon
             hex = RegularPolygon((x, y), numVertices=6, radius=hex_radius, 
                                     orientation=np.radians(60), 
                                     facecolor='k', alpha=0.6, edgecolor='k')
             ax.add_patch(hex)
@@ -475,27 +544,60 @@
         for x, y in zip (x_opened, y_opened):
 
             # determine patch origin
             x += y * 0.5
             y *= np.sqrt(3)/2
 
             # recenter
-            x -= (self.mask.shape[0] + self.mask.shape[1]/2.0)/2.0
+            x -= (self.mask.shape[0] + self.mask.shape[1]/2.0)/2.0 -1/hex_vert
             y -= (self.mask.shape[1] * 1/hex_vert)/2.0
 
             # add hexagon
             hex = RegularPolygon((x, y), numVertices=6, radius=hex_radius, 
                                     orientation=np.radians(60), 
                                     facecolor='w', alpha=0.2, edgecolor='k')
             ax.add_patch(hex)
 
-        plt.xlim(-self.mask.shape[0]/3.0,self.mask.shape[0]/3.0)
-        plt.ylim(-self.mask.shape[0]/3.0,self.mask.shape[1]/3.0)
-        plt.title(f"SHURA [o:{self.v}, r:{self.r}, x:{self.mult}]")
+        plt.xlim(-self.rx,self.rx)
+        plt.ylim(-self.ry,self.ry)
+        #plt.xlim(-10,10)
+        #plt.ylim(-10,10)
+        plt.title(f"SHURA rhombus [o:{self.v}, r:{self.r}]")
+        plt.show()
 
+    def show(self):
+        """
+        Plot the mask
+        """
+
+        # set up plot parameters
+        fig, ax = plt.subplots(1)
+        ax.set_aspect('equal')
+        hex_width = 1.0 # face-to-face distance
+        hex_vert  = (hex_width)*(2.0/np.sqrt(3))
+
+        # draw hexagon array
+        for y in range(self.diam):
+            row_width = self.diam - abs(self.radius-y)
+            start_i   = np.max((self.radius-y,0))
+            for x in range(row_width):
+                facecolor = 'k' if self.axial_matrix[x+start_i,y] == 1 else 'w'
+                alpha     = 0.6 if self.axial_matrix[x+start_i,y] == 1 else 0.3
+                hex = RegularPolygon((x+0.5*abs(y-self.radius)-self.radius,
+                                      ((y-self.radius)*((3/2)*hex_vert/2.0))),
+                                     numVertices=6, radius=hex_vert/2.0, 
+                                     orientation=np.radians(60), 
+                                     facecolor=facecolor, alpha=alpha, edgecolor='k')
+                ax.add_patch(hex)
+
+        # set axis limits
+        plt.xlim(-self.radius*hex_vert,self.radius*hex_vert)
+        plt.ylim(-self.radius,self.radius)
+        plt.title(f"SHURA [o:{self.v}, r:{self.r}]")
+        plt.show()
 
 class rand_hex():
     """
     Random Hexagonal Array
 
     Parameters
     ----------
@@ -573,7 +675,8 @@
                                      facecolor=facecolor, alpha=alpha, edgecolor='k')
                 ax.add_patch(hex)
 
         # set axis limits
         plt.xlim(-self.radius*hex_vert,self.radius*hex_vert)
         plt.ylim(-self.radius,self.radius)
         plt.title(f"Random Hex Array [diam: {self.diam}, fill: {self.actual_fill:.2f}]")
+        plt.show()
```

### Comparing `codedapertures-0.4/codedapertures.egg-info/PKG-INFO` & `codedapertures-0.5/codedapertures.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedapertures
-Version: 0.4
+Version: 0.5
 Summary: a python package for generating coded apertures
 Home-page: https://github.com/bpops/codedapertures
 Author: bpops
 License: MIT
 License-File: LICENSE
 
 CodedApertures is a python package that allows one to easily generate and display common coded aperture patterns. Coded apertures are a spatial encoding technique for straight-line optics, wherein traditional lensing (e.g., visible light) is not possible. Even wherein tradiational lensing is possible, there may be other advantages (infinite depth of field). Coded apertures may therefore be used for hard x-ray and gamma-ray imaging for astrophysics, medical imaging, and homeland security applications.
```

### Comparing `codedapertures-0.4/setup.py` & `codedapertures-0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 setuptools.setup(name='codedapertures',
-      version='0.4',
+      version='0.5',
       description='a python package for generating coded apertures',
       long_description='CodedApertures is a python package that allows one to easily generate and display common coded aperture patterns. Coded apertures are a spatial encoding technique for straight-line optics, wherein traditional lensing (e.g., visible light) is not possible. Even wherein tradiational lensing is possible, there may be other advantages (infinite depth of field). Coded apertures may therefore be used for hard x-ray and gamma-ray imaging for astrophysics, medical imaging, and homeland security applications.',
       url='https://github.com/bpops/codedapertures',
       author='bpops',
       license='MIT',
       install_requires=['pyprimes',
                 'numpy',
```

