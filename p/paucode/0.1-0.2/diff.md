# Comparing `tmp/paucode-0.1.tar.gz` & `tmp/paucode-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paucode-0.1.tar", last modified: Thu Jul 20 01:43:40 2023, max compression
+gzip compressed data, was "paucode-0.2.tar", last modified: Fri Jul 28 18:16:40 2023, max compression
```

## Comparing `paucode-0.1.tar` & `paucode-0.2.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 01:43:40.352674 paucode-0.1/
--rw-rw-rw-   0        0        0      399 2023-07-20 01:43:40.350593 paucode-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-07-20 00:43:08.000000 paucode-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 01:43:40.268362 paucode-0.1/paucode/
--rw-rw-rw-   0        0        0        0 2023-07-19 04:35:44.000000 paucode-0.1/paucode/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-19 13:14:52.000000 paucode-0.1/paucode/ds.py
--rw-rw-rw-   0        0        0      796 2023-07-20 01:17:51.000000 paucode-0.1/paucode/eco.py
--rw-rw-rw-   0        0        0     1101 2023-07-19 13:14:52.000000 paucode-0.1/paucode/tsp.py
-drwxrwxrwx   0        0        0        0 2023-07-20 01:43:40.345590 paucode-0.1/paucode.egg-info/
--rw-rw-rw-   0        0        0      399 2023-07-20 01:43:39.000000 paucode-0.1/paucode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-07-20 01:43:40.000000 paucode-0.1/paucode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 01:43:39.000000 paucode-0.1/paucode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-20 01:43:39.000000 paucode-0.1/paucode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-20 01:43:40.352674 paucode-0.1/setup.cfg
--rw-rw-rw-   0        0        0      545 2023-07-20 01:33:24.000000 paucode-0.1/setup.py
+drwxrwxr-x   0 choque    (1000) choque    (1000)        0 2023-07-28 18:16:40.685483 paucode-0.2/
+-rw-rw-r--   0 choque    (1000) choque    (1000)     1065 2023-07-24 04:26:30.000000 paucode-0.2/LICENSE
+-rw-rw-r--   0 choque    (1000) choque    (1000)      635 2023-07-28 18:16:40.685483 paucode-0.2/PKG-INFO
+-rw-rw-r--   0 choque    (1000) choque    (1000)      313 2023-07-24 04:27:02.000000 paucode-0.2/README.md
+drwxrwxr-x   0 choque    (1000) choque    (1000)        0 2023-07-28 18:16:40.685483 paucode-0.2/paucode/
+-rw-rw-r--   0 choque    (1000) choque    (1000)       46 2023-07-28 18:11:14.000000 paucode-0.2/paucode/__init__.py
+-rw-rw-r--   0 choque    (1000) choque    (1000)        0 2023-07-24 04:26:30.000000 paucode-0.2/paucode/ds.py
+-rw-rw-r--   0 choque    (1000) choque    (1000)      587 2023-07-28 17:51:54.000000 paucode-0.2/paucode/eco.py
+-rw-rw-r--   0 choque    (1000) choque    (1000)     4505 2023-07-28 17:45:38.000000 paucode-0.2/paucode/ing.py
+-rw-rw-r--   0 choque    (1000) choque    (1000)     1077 2023-07-24 04:26:30.000000 paucode-0.2/paucode/tsp.py
+drwxrwxr-x   0 choque    (1000) choque    (1000)        0 2023-07-28 18:16:40.685483 paucode-0.2/paucode.egg-info/
+-rw-rw-r--   0 choque    (1000) choque    (1000)      635 2023-07-28 18:16:40.000000 paucode-0.2/paucode.egg-info/PKG-INFO
+-rw-rw-r--   0 choque    (1000) choque    (1000)      229 2023-07-28 18:16:40.000000 paucode-0.2/paucode.egg-info/SOURCES.txt
+-rw-rw-r--   0 choque    (1000) choque    (1000)        1 2023-07-28 18:16:40.000000 paucode-0.2/paucode.egg-info/dependency_links.txt
+-rw-rw-r--   0 choque    (1000) choque    (1000)        8 2023-07-28 18:16:40.000000 paucode-0.2/paucode.egg-info/top_level.txt
+-rw-rw-r--   0 choque    (1000) choque    (1000)       38 2023-07-28 18:16:40.685483 paucode-0.2/setup.cfg
+-rw-rw-r--   0 choque    (1000) choque    (1000)      528 2023-07-28 18:11:01.000000 paucode-0.2/setup.py
```

### Comparing `paucode-0.1/paucode/tsp.py` & `paucode-0.2/paucode/tsp.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import matplotlib.pyplot as plt
-
-def trasparente(color:str):
-    """Para sacar los graficos en trasparente que puede ser util en cualquier caso. Solo funciona con matplotlib
-    Args:
-        color (str): Escoge el color que deseas, pero siempre utilizando las convenciones de python
-    """
-    #crea un figura con fondo trasparente
-    fig=plt.figure(facecolor="none")
-    
-    #crear ejes dentro de la figura
-    ax=fig.add_subplot(111, facecolor="none")
-    
-    ax=plt.gca()
-    # Cambiar el color de los ejes, los números y el marco
-    ax.spines['bottom'].set_color(color)   # Eje x
-    ax.spines['left'].set_color(color)    # Eje y
-    ax.spines['top'].set_color(color)     # Remover borde superior
-    ax.spines['right'].set_color(color)   # Remover borde derecho
-    
-    ax.xaxis.label.set_color(color)   # color de la etiqueta del eje x
-    ax.yaxis.label.set_color(color)   # color de la etiqueta del eje y
-    
-    ax.tick_params(axis='x', colors=color)   # Color de los ticks del eje x
+import matplotlib.pyplot as plt
+
+def trasparente(color:str):
+    """Para sacar los graficos en trasparente que puede ser util en cualquier caso. Solo funciona con matplotlib
+    Args:
+        color (str): Escoge el color que deseas, pero siempre utilizando las convenciones de python
+    """
+    #crea un figura con fondo trasparente
+    fig=plt.figure(facecolor="none")
+    
+    #crear ejes dentro de la figura
+    ax=fig.add_subplot(111, facecolor="none")
+    
+    ax=plt.gca()
+    # Cambiar el color de los ejes, los números y el marco
+    ax.spines['bottom'].set_color(color)   # Eje x
+    ax.spines['left'].set_color(color)    # Eje y
+    ax.spines['top'].set_color(color)     # Remover borde superior
+    ax.spines['right'].set_color(color)   # Remover borde derecho
+    
+    ax.xaxis.label.set_color(color)   # color de la etiqueta del eje x
+    ax.yaxis.label.set_color(color)   # color de la etiqueta del eje y
+    
+    ax.tick_params(axis='x', colors=color)   # Color de los ticks del eje x
     ax.tick_params(axis='y', colors=color)   # Color de los ticks del eje y
```

