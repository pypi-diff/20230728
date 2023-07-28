# Comparing `tmp/osmnx-1.5.1.tar.gz` & `tmp/osmnx-1.6.0.tar.gz`

## Comparing `osmnx-1.5.1.tar` & `osmnx-1.6.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/__init__.py
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/_api.py
--rw-r--r--   0        0        0    29173 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/_downloader.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/_errors.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/_version.py
--rw-r--r--   0        0        0    10407 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/bearing.py
--rw-r--r--   0        0        0    18195 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/distance.py
--rw-r--r--   0        0        0     9637 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/elevation.py
--rw-r--r--   0        0        0    41877 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/features.py
--rw-r--r--   0        0        0     6801 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/folium.py
--rw-r--r--   0        0        0     8904 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/geocoder.py
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/geometries.py
--rw-r--r--   0        0        0    30380 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/graph.py
--rw-r--r--   0        0        0    18096 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/io.py
--rw-r--r--   0        0        0    19063 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/osm_xml.py
--rw-r--r--   0        0        0    31934 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/plot.py
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/projection.py
--rw-r--r--   0        0        0     8038 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/settings.py
--rw-r--r--   0        0        0    25731 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/simplification.py
--rw-r--r--   0        0        0     9514 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/speed.py
--rw-r--r--   0        0        0    12680 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/stats.py
--rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/truncate.py
--rw-r--r--   0        0        0    11228 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/utils.py
--rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/utils_geo.py
--rw-r--r--   0        0        0    18223 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/utils_graph.py
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 osmnx-1.5.1/.gitignore
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 osmnx-1.5.1/LICENSE.txt
--rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 osmnx-1.5.1/README.md
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 osmnx-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 osmnx-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 osmnx-1.6.0/osmnx/__init__.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 osmnx-1.6.0/osmnx/_api.py
+-rw-r--r--   0        0        0    10630 2020-02-02 00:00:00.000000 osmnx-1.6.0/osmnx/_downloader.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 osmnx-1.6.0/osmnx/_errors.py
+-rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 osmnx-1.6.0/osmnx/_nominatim.py
+-rw-r--r--   0        0        0    14953 2020-02-02 00:00:00.000000 osmnx-1.6.0/osmnx/_overpass.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 osmnx-1.6.0/osmnx/_version.py
+-rw-r--r--   0        0        0    10540 2020-02-02 00:00:00.000000 osmnx-1.6.0/osmnx/bearing.py
+-rw-r--r--   0        0        0    18381 2020-02-02 00:00:00.000000 osmnx-1.6.0/osmnx/distance.py
+-rw-r--r--   0        0        0    10198 2020-02-02 00:00:00.000000 osmnx-1.6.0/osmnx/elevation.py
+-rw-r--r--   0        0        0    42303 2020-02-02 00:00:00.000000 osmnx-1.6.0/osmnx/features.py
+-rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 osmnx-1.6.0/osmnx/folium.py
+-rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 osmnx-1.6.0/osmnx/geocoder.py
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 osmnx-1.6.0/osmnx/geometries.py
+-rw-r--r--   0        0        0    30398 2020-02-02 00:00:00.000000 osmnx-1.6.0/osmnx/graph.py
+-rw-r--r--   0        0        0    18117 2020-02-02 00:00:00.000000 osmnx-1.6.0/osmnx/io.py
+-rw-r--r--   0        0        0    19070 2020-02-02 00:00:00.000000 osmnx-1.6.0/osmnx/osm_xml.py
+-rw-r--r--   0        0        0    32069 2020-02-02 00:00:00.000000 osmnx-1.6.0/osmnx/plot.py
+-rw-r--r--   0        0        0     6489 2020-02-02 00:00:00.000000 osmnx-1.6.0/osmnx/projection.py
+-rw-r--r--   0        0        0     8054 2020-02-02 00:00:00.000000 osmnx-1.6.0/osmnx/settings.py
+-rw-r--r--   0        0        0    25876 2020-02-02 00:00:00.000000 osmnx-1.6.0/osmnx/simplification.py
+-rw-r--r--   0        0        0     9560 2020-02-02 00:00:00.000000 osmnx-1.6.0/osmnx/speed.py
+-rw-r--r--   0        0        0    12752 2020-02-02 00:00:00.000000 osmnx-1.6.0/osmnx/stats.py
+-rw-r--r--   0        0        0     6760 2020-02-02 00:00:00.000000 osmnx-1.6.0/osmnx/truncate.py
+-rw-r--r--   0        0        0    11322 2020-02-02 00:00:00.000000 osmnx-1.6.0/osmnx/utils.py
+-rw-r--r--   0        0        0    16387 2020-02-02 00:00:00.000000 osmnx-1.6.0/osmnx/utils_geo.py
+-rw-r--r--   0        0        0    18318 2020-02-02 00:00:00.000000 osmnx-1.6.0/osmnx/utils_graph.py
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 osmnx-1.6.0/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 osmnx-1.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 osmnx-1.6.0/README.md
+-rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 osmnx-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 osmnx-1.6.0/PKG-INFO
```

### Comparing `osmnx-1.5.1/osmnx/_api.py` & `osmnx-1.6.0/osmnx/_api.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.5.1/osmnx/bearing.py` & `osmnx-1.6.0/osmnx/bearing.py`

 * *Files 9% similar despite different names*

```diff
@@ -82,15 +82,16 @@
     else:
         warn(
             "the `precision` parameter is deprecated and will be removed in a future release",
             stacklevel=2,
         )
 
     if projection.is_projected(G.graph["crs"]):  # pragma: no cover
-        raise ValueError("graph must be unprojected to add edge bearings")
+        msg = "graph must be unprojected to add edge bearings"
+        raise ValueError(msg)
 
     # extract edge IDs and corresponding coordinates from their nodes
     uvk = [(u, v, k) for u, v, k in G.edges if u != v]
     x = G.nodes(data="x")
     y = G.nodes(data="y")
     coords = np.array([(y[u], x[u], y[v], x[v]) for u, v, k in uvk])
 
@@ -116,15 +117,15 @@
 
     Parameters
     ----------
     Gu : networkx.MultiGraph
         undirected, unprojected graph with `bearing` attributes on each edge
     num_bins : int
         number of bins; for example, if `num_bins=36` is provided, then each
-        bin will represent 10° around the compass
+        bin will represent 10 degrees around the compass
     min_length : float
         ignore edges with `length` attributes less than `min_length`; useful
         to ignore the noise of many very short edges
     weight : string
         if not None, weight edges' bearings by this (non-null) edge attribute.
         for example, if "length" is provided, this will return 1 bearing
         observation per meter per street, which could result in a very large
@@ -133,25 +134,26 @@
     Returns
     -------
     entropy : float
         the graph's orientation entropy
     """
     # check if we were able to import scipy
     if scipy is None:  # pragma: no cover
-        raise ImportError("scipy must be installed to calculate entropy")
+        msg = "scipy must be installed to calculate entropy"
+        raise ImportError(msg)
     bin_counts, _ = _bearings_distribution(Gu, num_bins, min_length, weight)
     return scipy.stats.entropy(bin_counts)
 
 
 def _extract_edge_bearings(Gu, min_length=0, weight=None):
     """
     Extract undirected graph's bidirectional edge bearings.
 
-    For example, if an edge has a bearing of 90° then we will record bearings
-    of both 90° and 270° for this edge.
+    For example, if an edge has a bearing of 90 degrees then we will record
+    bearings of both 90 degrees and 270 degrees for this edge.
 
     Parameters
     ----------
     Gu : networkx.MultiGraph
         undirected, unprojected graph with `bearing` attributes on each edge
     min_length : float
         ignore edges with `length` attributes less than `min_length`; useful
@@ -164,15 +166,16 @@
 
     Returns
     -------
     bearings : numpy.array
         the graph's bidirectional edge bearings
     """
     if nx.is_directed(Gu) or projection.is_projected(Gu.graph["crs"]):  # pragma: no cover
-        raise ValueError("graph must be undirected and unprojected to analyze edge bearings")
+        msg = "graph must be undirected and unprojected to analyze edge bearings"
+        raise ValueError(msg)
     bearings = []
     for u, v, data in Gu.edges(data=True):
         # ignore self-loops and any edges below min_length
         if u != v and data["length"] >= min_length:
             if weight:
                 # weight edges' bearings by some edge attribute value
                 bearings.extend([data["bearing"]] * int(data[weight]))
@@ -187,18 +190,19 @@
     return np.concatenate([bearings, bearings_r])
 
 
 def _bearings_distribution(Gu, num_bins, min_length=0, weight=None):
     """
     Compute distribution of bearings across evenly spaced bins.
 
-    Prevents bin-edge effects around common values like 0° and 90° by
-    initially creating twice as many bins as desired, then merging them in
-    pairs. For example, if `num_bins=36` is provided, then each bin will
-    represent 10° around the compass, with the first bin representing 355°-5°.
+    Prevents bin-edge effects around common values like 0 degrees and 90
+    degrees by initially creating twice as many bins as desired, then merging
+    them in pairs. For example, if `num_bins=36` is provided, then each bin
+    will represent 10 degrees around the compass, with the first bin
+    representing 355 degrees to 5 degrees.
 
     Parameters
     ----------
     Gu : networkx.MultiGraph
         undirected, unprojected graph with `bearing` attributes on each edge
     num_bins : int
         number of bins for the bearings histogram
@@ -218,15 +222,16 @@
     """
     n = num_bins * 2
     bins = np.arange(n + 1) * 360 / n
 
     bearings = _extract_edge_bearings(Gu, min_length, weight)
     count, bin_edges = np.histogram(bearings, bins=bins)
 
-    # move last bin to front, so eg 0.01° and 359.99° will be binned together
+    # move last bin to front, so eg 0.01 degrees and 359.99 degrees will be
+    # binned together
     count = np.roll(count, 1)
     bin_counts = count[::2] + count[1::2]
 
     # because we merged the bins, their edges are now only every other one
     bin_edges = bin_edges[range(0, len(bin_edges), 2)]
     return bin_counts, bin_edges
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `osmnx-1.5.1/osmnx/distance.py` & `osmnx-1.6.0/osmnx/distance.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,17 +155,16 @@
     y = G.nodes(data="y")
     try:
         # two-dimensional array of coordinates: y0, x0, y1, x1
         c = np.array([(y[u], x[u], y[v], x[v]) for u, v, k in uvk])
         # ensure all coordinates can be converted to float and are non-null
         assert not np.isnan(c.astype(float)).any()
     except (AssertionError, KeyError) as e:  # pragma: no cover
-        raise ValueError(
-            "some edges missing nodes, possibly due to input data clipping issue"
-        ) from e
+        msg = "some edges missing nodes, possibly due to input data clipping issue"
+        raise ValueError(msg) from e
 
     # calculate great circle distances, round, and fill nulls with zeros
     dists = great_circle_vec(c[:, 0], c[:, 1], c[:, 2], c[:, 3]).round(precision)
     dists[np.isnan(dists)] = 0
     nx.set_edge_attributes(G, values=dict(zip(uvk, dists)), name="length")
 
     utils.log("Added length attributes to graph edges")
@@ -209,28 +208,31 @@
     if not (hasattr(X, "__iter__") and hasattr(Y, "__iter__")):
         # make coordinates arrays if user passed non-iterable values
         is_scalar = True
         X = np.array([X])
         Y = np.array([Y])
 
     if np.isnan(X).any() or np.isnan(Y).any():  # pragma: no cover
-        raise ValueError("`X` and `Y` cannot contain nulls")
+        msg = "`X` and `Y` cannot contain nulls"
+        raise ValueError(msg)
     nodes = utils_graph.graph_to_gdfs(G, edges=False, node_geometry=False)[["x", "y"]]
 
     if projection.is_projected(G.graph["crs"]):
         # if projected, use k-d tree for euclidean nearest-neighbor search
         if cKDTree is None:  # pragma: no cover
-            raise ImportError("scipy must be installed to search a projected graph")
+            msg = "scipy must be installed to search a projected graph"
+            raise ImportError(msg)
         dist, pos = cKDTree(nodes).query(np.array([X, Y]).T, k=1)
         nn = nodes.index[pos]
 
     else:
         # if unprojected, use ball tree for haversine nearest-neighbor search
         if BallTree is None:  # pragma: no cover
-            raise ImportError("scikit-learn must be installed to search an unprojected graph")
+            msg = "scikit-learn must be installed to search an unprojected graph"
+            raise ImportError(msg)
         # haversine requires lat, lng coords in radians
         nodes_rad = np.deg2rad(nodes[["y", "x"]])
         points_rad = np.deg2rad(np.array([Y, X]).T)
         dist, pos = BallTree(nodes_rad, metric="haversine").query(points_rad, k=1)
         dist = dist[:, 0] * EARTH_RADIUS_M  # convert radians -> meters
         nn = nodes.index[pos[:, 0]]
 
@@ -282,15 +284,16 @@
     if not (hasattr(X, "__iter__") and hasattr(Y, "__iter__")):
         # make coordinates arrays if user passed non-iterable values
         is_scalar = True
         X = np.array([X])
         Y = np.array([Y])
 
     if np.isnan(X).any() or np.isnan(Y).any():  # pragma: no cover
-        raise ValueError("`X` and `Y` cannot contain nulls")
+        msg = "`X` and `Y` cannot contain nulls"
+        raise ValueError(msg)
     geoms = utils_graph.graph_to_gdfs(G, nodes=False)["geometry"]
 
     # if no interpolation distance was provided
     if interpolate is None:
         # build an r-tree spatial index by position for subsequent iloc
         rtree = STRtree(geoms)
 
@@ -316,22 +319,24 @@
             uvk_xy.extend((uvk, xy) for xy in utils_geo.interpolate_points(geom, interpolate))
         labels, xy = zip(*uvk_xy)
         vertices = pd.DataFrame(xy, index=labels, columns=["x", "y"])
 
         if projection.is_projected(G.graph["crs"]):
             # if projected, use k-d tree for euclidean nearest-neighbor search
             if cKDTree is None:  # pragma: no cover
-                raise ImportError("scipy must be installed to search a projected graph")
+                msg = "scipy must be installed to search a projected graph"
+                raise ImportError(msg)
             dist, pos = cKDTree(vertices).query(np.array([X, Y]).T, k=1)
             ne = vertices.index[pos]
 
         else:
             # if unprojected, use ball tree for haversine nearest-neighbor search
             if BallTree is None:  # pragma: no cover
-                raise ImportError("scikit-learn must be installed to search an unprojected graph")
+                msg = "scikit-learn must be installed to search an unprojected graph"
+                raise ImportError(msg)
             # haversine requires lat, lng coords in radians
             vertices_rad = np.deg2rad(vertices[["y", "x"]])
             points_rad = np.deg2rad(np.array([Y, X]).T)
             dist, pos = BallTree(vertices_rad, metric="haversine").query(points_rad, k=1)
             dist = dist[:, 0] * EARTH_RADIUS_M  # convert radians -> meters
             ne = vertices.index[pos[:, 0]]
 
@@ -418,15 +423,16 @@
     # if neither orig nor dest is iterable, just return the shortest path
     if not (hasattr(orig, "__iter__") or hasattr(dest, "__iter__")):
         return _single_shortest_path(G, orig, dest, weight)
 
     # if both orig and dest are iterables, ensure they have same lengths
     elif hasattr(orig, "__iter__") and hasattr(dest, "__iter__"):
         if len(orig) != len(dest):  # pragma: no cover
-            raise ValueError("orig and dest must contain same number of elements")
+            msg = "orig and dest must contain same number of elements"
+            raise ValueError(msg)
 
         if cpus is None:
             cpus = mp.cpu_count()
         cpus = min(cpus, mp.cpu_count())
         utils.log(f"Solving {len(orig)} paths with {cpus} CPUs...")
 
         # if single-threading, calculate each shortest path one at a time
@@ -442,15 +448,16 @@
             pool.close()
             pool.join()
 
         return paths
 
     # if only one of orig or dest is iterable and the other is not
     else:  # pragma: no cover
-        raise ValueError("orig and dest must either both be iterable or neither must be iterable")
+        msg = "orig and dest must either both be iterable or neither must be iterable"
+        raise ValueError(msg)
 
 
 def k_shortest_paths(G, orig, dest, k, weight="length"):
     """
     Solve `k` shortest paths from an origin node to a destination node.
 
     Uses Yen's algorithm. See also `shortest_path` to solve just the one
@@ -501,8 +508,9 @@
     """
     try:
         values = np.array(tuple(G.edges(data=attr)))[:, 2]
         values_float = values.astype(float)
         if np.isnan(values_float).any():
             warn(f"The attribute {attr!r} is missing or null on some edges.", stacklevel=2)
     except ValueError as e:
-        raise ValueError(f"The edge attribute {attr!r} contains non-numeric values.") from e
+        msg = f"The edge attribute {attr!r} contains non-numeric values."
+        raise ValueError(msg) from e
```

### Comparing `osmnx-1.5.1/osmnx/elevation.py` & `osmnx-1.6.0/osmnx/elevation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,83 @@
-"""Get node elevations and calculate edge grades."""
-
+"""Add node elevations from raster files or web APIs, and calculate edge grades."""
 import multiprocessing as mp
 import time
 from hashlib import sha1
 from pathlib import Path
 from warnings import warn
 
 import networkx as nx
 import numpy as np
 import pandas as pd
 import requests
 
 from . import _downloader
+from . import settings
 from . import utils
 from . import utils_graph
+from ._errors import InsufficientResponseError
 
 # rasterio and gdal are optional dependencies for raster querying
 try:
     import rasterio
     from osgeo import gdal
 except ImportError:  # pragma: no cover
     rasterio = gdal = None
 
 
+def add_edge_grades(G, add_absolute=True, precision=None):
+    """
+    Add `grade` attribute to each graph edge.
+
+    Vectorized function to calculate the directed grade (ie, rise over run)
+    for each edge in the graph and add it to the edge as an attribute. Nodes
+    must already have `elevation` attributes to use this function.
+
+    See also the `add_node_elevations_raster` and `add_node_elevations_google`
+    functions.
+
+    Parameters
+    ----------
+    G : networkx.MultiDiGraph
+        input graph with `elevation` node attribute
+    add_absolute : bool
+        if True, also add absolute value of grade as `grade_abs` attribute
+    precision : int
+        deprecated, do not use
+
+    Returns
+    -------
+    G : networkx.MultiDiGraph
+        graph with edge `grade` (and optionally `grade_abs`) attributes
+    """
+    if precision is None:
+        precision = 3
+    else:
+        warn(
+            "the `precision` parameter is deprecated and will be removed in a future release",
+            stacklevel=2,
+        )
+
+    elev_lookup = G.nodes(data="elevation")
+    u, v, k, lengths = zip(*G.edges(keys=True, data="length"))
+    uvk = tuple(zip(u, v, k))
+
+    # calculate edges' elevation changes from u to v then divide by lengths
+    elevs = np.array([(elev_lookup[u], elev_lookup[v]) for u, v, k in uvk])
+    grades = ((elevs[:, 1] - elevs[:, 0]) / np.array(lengths)).round(precision)
+    nx.set_edge_attributes(G, dict(zip(uvk, grades)), name="grade")
+
+    # optionally add grade absolute value to the edge attributes
+    if add_absolute:
+        nx.set_edge_attributes(G, dict(zip(uvk, np.abs(grades))), name="grade_abs")
+
+    utils.log("Added grade attributes to all edges.")
+    return G
+
+
 def _query_raster(nodes, filepath, band):
     """
     Query a raster for values at coordinates in a DataFrame's x/y columns.
 
     Parameters
     ----------
     nodes : pandas.DataFrame
@@ -70,15 +121,16 @@
 
     Returns
     -------
     G : networkx.MultiDiGraph
         graph with node elevation attributes
     """
     if rasterio is None or gdal is None:  # pragma: no cover
-        raise ImportError("gdal and rasterio must be installed to query raster files")
+        msg = "gdal and rasterio must be installed to query raster files"
+        raise ImportError(msg)
 
     if cpus is None:
         cpus = mp.cpu_count()
     cpus = min(cpus, mp.cpu_count())
     utils.log(f"Attaching elevations with {cpus} CPUs...")
 
     # if a list of filepaths is passed, compose them all as a virtual raster
@@ -109,15 +161,15 @@
     return G
 
 
 def add_node_elevations_google(
     G,
     api_key=None,
     max_locations_per_batch=350,
-    pause_duration=0,
+    pause=0,
     precision=None,
     url_template="https://maps.googleapis.com/maps/api/elevation/json?locations={}&key={}",
 ):  # pragma: no cover
     """
     Add `elevation` (meters) attribute to each node using a web service.
 
     By default, this uses the Google Maps Elevation API but you can optionally
@@ -134,15 +186,15 @@
         input graph
     api_key : string
         a valid API key, can be None if the API does not require a key
     max_locations_per_batch : int
         max number of coordinate pairs to submit in each API call (if this is
         too high, the server will reject the request because its character
         limit exceeds the max allowed)
-    pause_duration : float
+    pause : float
         time to pause between API calls, which can be increased if you get
         rate limited
     precision : int
         deprecated, do not use
     url_template : string
         a URL string template for the API endpoint, containing exactly two
         parameters: `locations` and `key`; for example, for Open Topo Data:
@@ -164,103 +216,76 @@
     # make a pandas series of all the nodes' coordinates as 'lat,lng'
     # round coordinates to 5 decimal places (approx 1 meter) to be able to fit
     # in more locations per API call
     node_points = pd.Series(
         {node: f'{data["y"]:.5f},{data["x"]:.5f}' for node, data in G.nodes(data=True)}
     )
     n_calls = int(np.ceil(len(node_points) / max_locations_per_batch))
-    utils.log(f"Requesting node elevations from the API in {n_calls} calls")
+    domain = _downloader._hostname_from_url(url_template)
+    utils.log(f"Requesting node elevations from {domain!r} in {n_calls} request(s)")
 
     # break the series of coordinates into chunks of size max_locations_per_batch
     # API format is locations=lat,lng|lat,lng|lat,lng|lat,lng...
     results = []
     for i in range(0, len(node_points), max_locations_per_batch):
         chunk = node_points.iloc[i : i + max_locations_per_batch]
         locations = "|".join(chunk)
         url = url_template.format(locations, api_key)
 
-        # check if this request is already in the cache (if global use_cache=True)
-        cached_response_json = _downloader._retrieve_from_cache(url)
-        if cached_response_json is not None:
-            response_json = cached_response_json
-        else:
-            # request the elevations from the API
-            utils.log(f"Requesting node elevations: {url}")
-            time.sleep(pause_duration)
-            response = requests.get(url)
-            if response.status_code == 200:
-                response_json = response.json()
-                _downloader._save_to_cache(url, response_json, response.status_code)
-            else:
-                raise Exception(
-                    f"Server responded with {response.status_code}: {response.reason} \n{response.json()}"
-                )
-
-        # append these elevation results to the list of all results
+        # download and append these elevation results to list of all results
+        response_json = _elevation_request(url, pause)
         results.extend(response_json["results"])
 
     # sanity check that all our vectors have the same number of elements
+    msg = f"Graph has {len(G):,} nodes and we received {len(results):,} results from {domain!r}"
+    utils.log(msg)
     if not (len(results) == len(G) == len(node_points)):
-        raise Exception(
-            f"Graph has {len(G)} nodes but we received {len(results)} results. \n{response_json}"
-        )
-    else:
-        utils.log(f"Graph has {len(G)} nodes and we received {len(results)} results.")
+        err_msg = f"{msg}\n{response_json}"
+        raise InsufficientResponseError(err_msg)
 
     # add elevation as an attribute to the nodes
     df = pd.DataFrame(node_points, columns=["node_points"])
     df["elevation"] = [result["elevation"] for result in results]
     df["elevation"] = df["elevation"].round(precision)
     nx.set_node_attributes(G, name="elevation", values=df["elevation"].to_dict())
-    utils.log("Added elevation data from API to all nodes.")
+    utils.log(f"Added elevation data from {domain!r} to all nodes.")
 
     return G
 
 
-def add_edge_grades(G, add_absolute=True, precision=None):
+def _elevation_request(url, pause):
     """
-    Add `grade` attribute to each graph edge.
-
-    Vectorized function to calculate the directed grade (ie, rise over run)
-    for each edge in the graph and add it to the edge as an attribute. Nodes
-    must already have `elevation` attributes to use this function.
-
-    See also the `add_node_elevations_raster` and `add_node_elevations_google`
-    functions.
+    Send a HTTP GET request to Google Maps-style Elevation API.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph with `elevation` node attribute
-    add_absolute : bool
-        if True, also add absolute value of grade as `grade_abs` attribute
-    precision : int
-        deprecated, do not use
+    url : string
+        URL for API endpoint populated with request data
+    pause : float
+        how long to pause in seconds before request
 
     Returns
     -------
-    G : networkx.MultiDiGraph
-        graph with edge `grade` (and optionally `grade_abs`) attributes
+    response_json : dict
     """
-    if precision is None:
-        precision = 3
-    else:
-        warn(
-            "the `precision` parameter is deprecated and will be removed in a future release",
-            stacklevel=2,
-        )
-
-    elev_lookup = G.nodes(data="elevation")
-    u, v, k, lengths = zip(*G.edges(keys=True, data="length"))
-    uvk = tuple(zip(u, v, k))
-
-    # calculate edges' elevation changes from u to v then divide by lengths
-    elevs = np.array([(elev_lookup[u], elev_lookup[v]) for u, v, k in uvk])
-    grades = ((elevs[:, 1] - elevs[:, 0]) / np.array(lengths)).round(precision)
-    nx.set_edge_attributes(G, dict(zip(uvk, grades)), name="grade")
-
-    # optionally add grade absolute value to the edge attributes
-    if add_absolute:
-        nx.set_edge_attributes(G, dict(zip(uvk, np.abs(grades))), name="grade_abs")
+    # check if request already exists in cache
+    cached_response_json = _downloader._retrieve_from_cache(url)
+    if cached_response_json is not None:
+        return cached_response_json
+
+    # pause then request this URL
+    domain = _downloader._hostname_from_url(url)
+    utils.log(f"Pausing {pause} second(s) before making HTTP GET request to {domain!r}")
+    time.sleep(pause)
+
+    # transmit the HTTP GET request
+    utils.log(f"Get {url} with timeout={settings.timeout}")
+    response = requests.get(
+        url,
+        timeout=settings.timeout,
+        headers=_downloader._get_http_headers(),
+        **settings.requests_kwargs,
+    )
 
-    utils.log("Added grade attributes to all edges.")
-    return G
+    response_json = _downloader._parse_response(response)
+    _downloader._save_to_cache(url, response_json, response.status_code)
+    return response_json
```

### Comparing `osmnx-1.5.1/osmnx/features.py` & `osmnx-1.6.0/osmnx/features.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,33 +9,35 @@
 
 For more details, see https://wiki.openstreetmap.org/wiki/Map_features and
 https://wiki.openstreetmap.org/wiki/Elements
 """
 
 import logging as lg
 import warnings
+from warnings import warn
 
 import geopandas as gpd
 import pandas as pd
 from shapely.errors import GEOSException
 from shapely.errors import TopologicalError
 from shapely.geometry import LineString
 from shapely.geometry import MultiPolygon
 from shapely.geometry import Point
 from shapely.geometry import Polygon
 from shapely.ops import linemerge
 from shapely.ops import polygonize
 
-from . import _downloader
+from . import _overpass
 from . import geocoder
 from . import osm_xml
 from . import settings
 from . import utils
 from . import utils_geo
-from ._errors import EmptyOverpassResponse
+from ._errors import CacheOnlyInterruptError
+from ._errors import InsufficientResponseError
 
 # dict of tags to determine if closed ways should be polygons, based on JSON
 # from https://wiki.openstreetmap.org/wiki/Overpass_turbo/Polygon_Features
 _POLYGON_FEATURES = {
     "building": {"polygon": "all"},
     "highway": {"polygon": "passlist", "values": ["services", "rest_area", "escape", "elevator"]},
     "natural": {
@@ -112,17 +114,15 @@
     -------
     gdf : geopandas.GeoDataFrame
     """
     # convert bounding box to a polygon
     polygon = utils_geo.bbox_to_poly(north, south, east, west)
 
     # create GeoDataFrame of features within this polygon
-    gdf = features_from_polygon(polygon, tags)
-
-    return gdf
+    return features_from_polygon(polygon, tags)
 
 
 def features_from_point(center_point, tags, dist=1000):
     """
     Create GeoDataFrame of OSM features within some distance N, S, E, W of a point.
 
     You can use the `settings` module to retrieve a snapshot of historical OSM
@@ -157,17 +157,15 @@
     # create bounding box from center point and distance in each direction
     north, south, east, west = utils_geo.bbox_from_point(center_point, dist)
 
     # convert the bounding box to a polygon
     polygon = utils_geo.bbox_to_poly(north, south, east, west)
 
     # create GeoDataFrame of features within this polygon
-    gdf = features_from_polygon(polygon, tags)
-
-    return gdf
+    return features_from_polygon(polygon, tags)
 
 
 def features_from_address(address, tags, dist=1000):
     """
     Create GeoDataFrame of OSM features within some distance N, S, E, W of address.
 
     You can use the `settings` module to retrieve a snapshot of historical OSM
@@ -200,17 +198,15 @@
     -------
     gdf : geopandas.GeoDataFrame
     """
     # geocode the address string to a (lat, lng) point
     center_point = geocoder.geocode(query=address)
 
     # create GeoDataFrame of features around this point
-    gdf = features_from_point(center_point, tags, dist=dist)
-
-    return gdf
+    return features_from_point(center_point, tags, dist=dist)
 
 
 def features_from_place(query, tags, which_result=None, buffer_dist=None):
     """
     Create GeoDataFrame of OSM features within boundaries of some place(s).
 
     The query must be geocodable and OSM must have polygon boundaries for the
@@ -248,41 +244,47 @@
         the area. `tags = {'amenity':True, 'landuse':['retail','commercial'],
         'highway':'bus_stop'}` would return all amenities, landuse=retail,
         landuse=commercial, and highway=bus_stop.
     which_result : int
         which geocoding result to use. if None, auto-select the first
         (Multi)Polygon or raise an error if OSM doesn't return one.
     buffer_dist : float
-        distance to buffer around the place geometry, in meters
+        deprecated, do not use
 
     Returns
     -------
     gdf : geopandas.GeoDataFrame
     """
+    if buffer_dist is not None:
+        warn(
+            "The buffer_dist argument as been deprecated and will be removed "
+            "in a future release. Buffer your query area directly, if desired.",
+            stacklevel=2,
+        )
+
     # create a GeoDataFrame with the spatial boundaries of the place(s)
     if isinstance(query, (str, dict)):
         # if it is a string (place name) or dict (structured place query),
         # then it is a single place
         gdf_place = geocoder.geocode_to_gdf(
             query, which_result=which_result, buffer_dist=buffer_dist
         )
     elif isinstance(query, list):
         # if it is a list, it contains multiple places to get
         gdf_place = geocoder.geocode_to_gdf(query, buffer_dist=buffer_dist)
     else:  # pragma: no cover
-        raise TypeError("query must be dict, string, or list of strings")
+        msg = "query must be dict, string, or list of strings"
+        raise TypeError(msg)
 
     # extract the geometry from the GeoDataFrame to use in API query
     polygon = gdf_place["geometry"].unary_union
     utils.log("Constructed place geometry polygon(s) to query API")
 
     # create GeoDataFrame using this polygon(s) geometry
-    gdf = features_from_polygon(polygon, tags)
-
-    return gdf
+    return features_from_polygon(polygon, tags)
 
 
 def features_from_polygon(polygon, tags):
     """
     Create GeoDataFrame of OSM features within boundaries of a (multi)polygon.
 
     You can use the `settings` module to retrieve a snapshot of historical OSM
@@ -310,30 +312,30 @@
 
     Returns
     -------
     gdf : geopandas.GeoDataFrame
     """
     # verify that the geometry is valid and a Polygon/MultiPolygon
     if not polygon.is_valid:
-        raise ValueError("The geometry of `polygon` is invalid")
+        msg = "The geometry of `polygon` is invalid"
+        raise ValueError(msg)
     if not isinstance(polygon, (Polygon, MultiPolygon)):
-        raise TypeError(
-            "Boundaries must be a shapely Polygon or MultiPolygon. If you requested "
-            "features from place name, make sure your query resolves to a Polygon or "
-            "MultiPolygon, and not some other geometry, like a Point. See OSMnx "
-            "documentation for details."
+        msg = (
+            "Boundaries must be a shapely Polygon or MultiPolygon. If you "
+            "requested features from place name, make sure your query resolves "
+            "to a Polygon or MultiPolygon, and not some other geometry, like a "
+            "Point. See OSMnx documentation for details."
         )
+        raise TypeError(msg)
 
     # download the data from OSM
-    response_jsons = _downloader._osm_features_download(polygon, tags)
+    response_jsons = _overpass._download_overpass_features(polygon, tags)
 
     # create GeoDataFrame from the downloaded data
-    gdf = _create_gdf(response_jsons, polygon, tags)
-
-    return gdf
+    return _create_gdf(response_jsons, polygon, tags)
 
 
 def features_from_xml(filepath, polygon=None, tags=None):
     """
     Create a GeoDataFrame of OSM features in an OSM-formatted XML file.
 
     Because this function creates a GeoDataFrame of features from an
@@ -368,17 +370,15 @@
     -------
     gdf : geopandas.GeoDataFrame
     """
     # transmogrify file of OSM XML data into JSON
     response_jsons = [osm_xml._overpass_json_from_file(filepath)]
 
     # create GeoDataFrame using this response JSON
-    gdf = _create_gdf(response_jsons, polygon=polygon, tags=tags)
-
-    return gdf
+    return _create_gdf(response_jsons, polygon=polygon, tags=tags)
 
 
 def _create_gdf(response_jsons, polygon, tags):
     """
     Parse JSON responses from the Overpass API to a GeoDataFrame.
 
     Note: the `polygon` and `tags` arguments can both be `None` and the
@@ -396,38 +396,37 @@
         dict of tags used for filtering the final GeoDataFrame
 
     Returns
     -------
     gdf : geopandas.GeoDataFrame
         GeoDataFrame of features and their associated tags
     """
-    elements_count = sum(len(rj["elements"]) for rj in response_jsons)
-
-    # make sure we got data back from the server request(s)
-    if elements_count == 0:
-        msg = (
-            "There are no data elements in the server response. Check log and query location/tags."
-        )
-        raise EmptyOverpassResponse(msg)
-
-    # begin processing the elements retrieved from the server
-    utils.log(f"Converting {elements_count} elements in JSON responses to features")
+    response_count = 0
+    if settings.cache_only_mode:
+        # if cache_only_mode, consume response_jsons then interrupt
+        for _ in response_jsons:
+            response_count += 1
+        utils.log(f"Retrieved all data from API in {response_count} request(s)")
+        msg = "Interrupted because `settings.cache_only_mode=True`"
+        raise CacheOnlyInterruptError(msg)
 
     # Dictionaries to hold nodes and complete geometries
     coords = {}
     geometries = {}
 
     # Set to hold the unique IDs of elements that do not have tags
     untagged_element_ids = set()
 
     # identify which relation types to parse to (multi)polygons
     relation_types = {"boundary", "multipolygon"}
 
     # extract geometries from the downloaded osm data
     for response_json in response_jsons:
+        response_count += 1
+
         # Parses the JSON of OSM nodes, ways and (multipolygon) relations
         # to dictionaries of coordinates, Shapely Points, LineStrings,
         # Polygons and MultiPolygons
         for element in response_json["elements"]:
             # id numbers are only unique within element types
             # create unique id from combination of type and id
             unique_id = f"{element['type']}/{element['id']}"
@@ -461,20 +460,25 @@
             ):
                 # parse relations to (multi)polygons
                 multipolygon = _parse_relation_to_multipolygon(
                     element=element, geometries=geometries
                 )
                 geometries[unique_id] = multipolygon
 
-    utils.log(f"{len(geometries)} geometries created in the dict")
+    utils.log(f"Retrieved all data from API in {response_count} request(s)")
+
+    # ensure we got some node/way data back from the server request(s)
+    if len(geometries) == 0:  # pragma: no cover
+        msg = "No data elements in server response. Check log and query location/tags."
+        raise InsufficientResponseError(msg)
 
     # remove untagged elements from the final dict of geometries
+    utils.log(f"{len(geometries)} geometries created in the dict")
     for untagged_element_id in untagged_element_ids:
         geometries.pop(untagged_element_id, None)
-
     utils.log(f"{len(untagged_element_ids)} untagged features removed")
 
     # create GeoDataFrame, ensure it has geometry, then set crs
     gdf = gpd.GeoDataFrame.from_dict(geometries, orient="index")
     if "geometry" not in gdf.columns:
         # if there is no geometry column, create a null column
         gdf = gdf.set_geometry([None] * len(gdf))
@@ -513,16 +517,15 @@
 
     Returns
     -------
     coords : dict
         dict of latitude/longitude coordinates
     """
     # return the coordinate of a single node element
-    coords = {"lat": element["lat"], "lon": element["lon"]}
-    return coords
+    return {"lat": element["lat"], "lon": element["lon"]}
 
 
 def _parse_node_to_point(element):
     """
     Parse point from a tagged node in the overpass response.
 
     The points are geometries in their own right.
@@ -545,29 +548,27 @@
         for tag in element["tags"]:
             point[tag] = element["tags"][tag]
 
     point["geometry"] = Point(element["lon"], element["lat"])
     return point
 
 
-def _parse_way_to_linestring_or_polygon(element, coords, polygon_features=_POLYGON_FEATURES):
+def _parse_way_to_linestring_or_polygon(element, coords):
     """
     Parse open LineString, closed LineString or Polygon from OSM 'way'.
 
     Please see https://wiki.openstreetmap.org/wiki/Overpass_turbo/Polygon_Features
     for more information on which tags should be parsed to polygons
 
     Parameters
     ----------
     element : dict
         element type "way" from overpass response JSON
     coords : dict
         dict of node IDs and their latitude/longitude coordinates
-    polygon_features : dict
-        dict for determining whether closed ways are LineStrings or Polygons
 
     Returns
     -------
     linestring_or_polygon : dict
         dict of OSM ID, OSM element type, nodes, tags and geometry
     """
     nodes = element["nodes"]
@@ -701,20 +702,20 @@
                 elif blocklist_or_passlist == "blocklist":
                     # if the value for that key in the element is not in
                     # the blocklist -> Polygon
                     if key_value not in polygon_features_values:
                         is_polygon = True
 
                 # if the key is for a passlist i.e. specific tags should
-                # become Polygons
-                elif blocklist_or_passlist == "passlist":
-                    # if the value for that key in the element is in the
-                    # passlist -> Polygon
-                    if key_value in polygon_features_values:
-                        is_polygon = True
+                # become Polygons, and if the value for that key in the
+                # element is in the passlist -> Polygon
+                elif (blocklist_or_passlist == "passlist") and (
+                    key_value in polygon_features_values
+                ):
+                    is_polygon = True
 
     return is_polygon
 
 
 def _parse_relation_to_multipolygon(element, geometries):
     """
     Parse multipolygon from OSM relation (type:MultiPolygon).
@@ -879,32 +880,33 @@
     # create a new list to hold the outer polygons with the inner polygons
     # subtracted
     outer_polygons_with_holes = []
 
     # loop through the outer polygons subtracting the inner polygons and
     # appending to the list
     for outer_polygon in outer_polygons:
+        outer_polygon_diff = outer_polygon
         for inner_polygon in inner_polygons:
             if inner_polygon.within(outer_polygon):
                 try:
-                    outer_polygon = outer_polygon.difference(inner_polygon)
+                    outer_polygon_diff = outer_polygon.difference(inner_polygon)
                 except TopologicalError:  # pragma: no cover
                     utils.log(
-                        f"relation https://www.openstreetmap.org/relation/{element['id']} caused"
-                        " a TopologicalError, trying with zero buffer."
+                        f"relation https://www.openstreetmap.org/relation/{element['id']} "
+                        "caused a TopologicalError, trying with zero buffer."
                     )
-                    outer_polygon = outer_polygon.buffer(0).difference(inner_polygon.buffer(0))
+                    outer_polygon_diff = outer_polygon.buffer(0).difference(inner_polygon.buffer(0))
 
         # note: .buffer(0) can return either a Polygon or MultiPolygon
         # if it returns a MultiPolygon we need to extract the component
         # sub Polygons to add to outer_polygons_with_holes
-        if outer_polygon.geom_type == "Polygon":
-            outer_polygons_with_holes.append(outer_polygon)
-        elif outer_polygon.geom_type == "MultiPolygon":
-            outer_polygons_with_holes.extend(list(outer_polygon.geoms))
+        if outer_polygon_diff.geom_type == "Polygon":
+            outer_polygons_with_holes.append(outer_polygon_diff)
+        elif outer_polygon_diff.geom_type == "MultiPolygon":
+            outer_polygons_with_holes.extend(list(outer_polygon_diff.geoms))
 
     # if only one polygon with holes was created, return that single polygon
     if len(outer_polygons_with_holes) == 1:
         geometry = outer_polygons_with_holes[0]
     # otherwise create a multipolygon from list of outer polygons with holes
     else:
         geometry = MultiPolygon(outer_polygons_with_holes)
```

### Comparing `osmnx-1.5.1/osmnx/folium.py` & `osmnx-1.6.0/osmnx/folium.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,16 @@
 
     Returns
     -------
     m : folium.folium.Map
     """
     # check if we were able to import folium successfully
     if folium is None:  # pragma: no cover
-        raise ImportError("folium must be installed to use this optional feature")
+        msg = "folium must be installed to use this optional feature"
+        raise ImportError(msg)
 
     # get centroid
     x, y = gdf.unary_union.centroid.xy
     centroid = (y[0], x[0])
 
     # create the folium web map if one wasn't passed-in
     if m is None:
@@ -209,9 +210,8 @@
     if popup_val is None:
         popup = None
     else:
         # folium doesn't interpret html, so can't do newlines without iframe
         popup = folium.Popup(html=json.dumps(popup_val))
 
     # create a folium polyline with attributes
-    pl = folium.PolyLine(locations=locations, popup=popup, **kwargs)
-    return pl
+    return folium.PolyLine(locations=locations, popup=popup, **kwargs)
```

### Comparing `osmnx-1.5.1/osmnx/geocoder.py` & `osmnx-1.6.0/osmnx/geocoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 This module uses the Nominatim API's "search" and "lookup" endpoints. For more
 details see https://wiki.openstreetmap.org/wiki/Elements and
 https://nominatim.org/.
 """
 
 import logging as lg
 from collections import OrderedDict
+from warnings import warn
 
 import geopandas as gpd
 import pandas as pd
 
-from . import _downloader
+from . import _nominatim
 from . import projection
 from . import settings
 from . import utils
+from ._errors import InsufficientResponseError
 
 
 def geocode(query):
     """
     Geocode place names or addresses to (lat, lng) with the Nominatim API.
 
     This geocodes the query via the Nominatim "search" endpoint.
@@ -36,25 +38,26 @@
     """
     # define the parameters
     params = OrderedDict()
     params["format"] = "json"
     params["limit"] = 1
     params["dedupe"] = 0  # prevent deduping to get precise number of results
     params["q"] = query
-    response_json = _downloader._nominatim_request(params=params)
+    response_json = _nominatim._nominatim_request(params=params)
 
     # if results were returned, parse lat and lng out of the result
     if response_json and "lat" in response_json[0] and "lon" in response_json[0]:
         lat = float(response_json[0]["lat"])
         lng = float(response_json[0]["lon"])
         point = (lat, lng)
         utils.log(f"Geocoded {query!r} to {point}")
         return point
     else:
-        raise ValueError(f"Nominatim could not geocode query {query!r}")
+        msg = f"Nominatim could not geocode query {query!r}"
+        raise InsufficientResponseError(msg)
 
 
 def geocode_to_gdf(query, which_result=None, by_osmid=False, buffer_dist=None):
     """
     Retrieve OSM elements by place name or OSM ID with the Nominatim API.
 
     If searching by place name, the `query` argument can be a string or
@@ -83,43 +86,53 @@
         which search result to return. if None, auto-select the first
         (Multi)Polygon or raise an error if OSM doesn't return one. to get
         the top match regardless of geometry type, set which_result=1.
         ignored if by_osmid=True.
     by_osmid : bool
         if True, treat query as an OSM ID lookup rather than text search
     buffer_dist : float
-        distance to buffer around the place geometry, in meters
+        deprecated, do not use
 
     Returns
     -------
     gdf : geopandas.GeoDataFrame
         a GeoDataFrame with one row for each query
     """
+    if buffer_dist is not None:
+        warn(
+            "The buffer_dist argument as been deprecated and will be removed "
+            "in a future release. Buffer your results directly, if desired.",
+            stacklevel=2,
+        )
+
     if not isinstance(query, (str, dict, list)):  # pragma: no cover
-        raise ValueError("query must be a string or dict or list")
+        msg = "query must be a string or dict or list"
+        raise TypeError(msg)
 
     # if caller passed a list of queries but a scalar which_result value, then
     # turn which_result into a list with same length as query list
     if isinstance(query, list) and (isinstance(which_result, int) or which_result is None):
         which_result = [which_result] * len(query)
 
     # turn query and which_result into lists if they're not already
     if not isinstance(query, list):
         query = [query]
     if not isinstance(which_result, list):
         which_result = [which_result]
 
     # ensure same length
     if len(query) != len(which_result):  # pragma: no cover
-        raise ValueError("which_result length must equal query length")
+        msg = "which_result length must equal query length"
+        raise ValueError(msg)
 
     # ensure query type of each item
     for q in query:
         if not isinstance(q, (str, dict)):  # pragma: no cover
-            raise ValueError("each query must be a dict or a string")
+            msg = "each query must be a dict or a string"
+            raise TypeError(msg)
 
     # geocode each query and add to GeoDataFrame as a new row
     gdf = gpd.GeoDataFrame()
     for q, wr in zip(query, which_result):
         gdf = pd.concat([gdf, _geocode_query_to_gdf(q, wr, by_osmid)])
 
     # reset GeoDataFrame index and set its CRS
@@ -160,37 +173,38 @@
         a GeoDataFrame with one row containing the result of geocoding
     """
     if which_result is None:
         limit = 50
     else:
         limit = which_result
 
-    results = _downloader._retrieve_osm_element(query, by_osmid=by_osmid, limit=limit)
+    results = _nominatim._download_nominatim_element(query, by_osmid=by_osmid, limit=limit)
 
     # choose the right result from the JSON response
     if not results:
         # if no results were returned, raise error
-        raise ValueError(f"Nominatim geocoder returned 0 results for query {query!r}")
+        msg = f"Nominatim geocoder returned 0 results for query {query!r}"
+        raise InsufficientResponseError(msg)
 
-    elif by_osmid:
+    if by_osmid:
         # if searching by OSM ID, always take the first (ie, only) result
         result = results[0]
 
     elif which_result is None:
         # else, if which_result=None, auto-select the first (Multi)Polygon
         result = _get_first_polygon(results, query)
 
     elif len(results) >= which_result:
         # else, if we got at least which_result results, choose that one
         result = results[which_result - 1]
 
     else:  # pragma: no cover
         # else, we got fewer results than which_result, raise error
-        msg = f"Nominatim geocoder only returned {len(results)} result(s) for query {query!r}"
-        raise ValueError(msg)
+        msg = f"Nominatim returned {len(results)} result(s) but which_result={which_result}"
+        raise InsufficientResponseError(msg)
 
     # if we got a non (Multi)Polygon geometry type (like a point), log warning
     geom_type = result["geojson"]["type"]
     if geom_type not in {"Polygon", "MultiPolygon"}:
         msg = f"Nominatim geocoder returned a {geom_type} as the geometry for query {query!r}"
         utils.log(msg, level=lg.WARNING)
 
@@ -237,8 +251,9 @@
     """
     polygon_types = {"Polygon", "MultiPolygon"}
     for result in results:
         if "geojson" in result and result["geojson"]["type"] in polygon_types:
             return result
 
     # if we never found a polygon, throw an error
-    raise ValueError(f"Nominatim could not geocode query {query!r} to polygonal boundaries")
+    msg = f"Nominatim could not geocode query {query!r} to a geometry of type (Multi)Polygon"
+    raise TypeError(msg)
```

### Comparing `osmnx-1.5.1/osmnx/geometries.py` & `osmnx-1.6.0/osmnx/geometries.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.5.1/osmnx/graph.py` & `osmnx-1.6.0/osmnx/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,41 +3,41 @@
 import itertools
 from warnings import warn
 
 import networkx as nx
 from shapely.geometry import MultiPolygon
 from shapely.geometry import Polygon
 
-from . import _downloader
+from . import _overpass
 from . import distance
 from . import geocoder
 from . import osm_xml
 from . import projection
 from . import settings
 from . import simplification
 from . import stats
 from . import truncate
 from . import utils
 from . import utils_geo
 from . import utils_graph
-from ._errors import CacheOnlyModeInterrupt
-from ._errors import EmptyOverpassResponse
+from ._errors import CacheOnlyInterruptError
+from ._errors import InsufficientResponseError
 from ._version import __version__
 
 
 def graph_from_bbox(
     north,
     south,
     east,
     west,
     network_type="all_private",
     simplify=True,
     retain_all=False,
     truncate_by_edge=False,
-    clean_periphery=True,
+    clean_periphery=None,
     custom_filter=None,
 ):
     """
     Download and create a graph within some bounding box.
 
     You can use the `settings` module to retrieve a snapshot of historical OSM
     data as of a certain date, or to configure the Overpass server timeout,
@@ -60,16 +60,15 @@
     retain_all : bool
         if True, return the entire graph even if it is not connected.
         otherwise, retain only the largest weakly connected component.
     truncate_by_edge : bool
         if True, retain nodes outside bounding box if at least one of node's
         neighbors is within the bounding box
     clean_periphery : bool
-        if True, buffer 500m to get a graph larger than requested, then
-        simplify, then truncate it to requested spatial boundaries
+        deprecated, do not use
     custom_filter : string
         a custom ways filter to be used instead of the network_type presets
         e.g., '["power"~"line"]' or '["highway"~"motorway|trunk"]'. Also pass
         in a network_type that is in settings.bidirectional_network_types if
         you want graph to be fully bi-directional.
 
     Returns
@@ -104,15 +103,15 @@
     center_point,
     dist=1000,
     dist_type="bbox",
     network_type="all_private",
     simplify=True,
     retain_all=False,
     truncate_by_edge=False,
-    clean_periphery=True,
+    clean_periphery=None,
     custom_filter=None,
 ):
     """
     Download and create a graph within some distance of a (lat, lng) point.
 
     You can use the `settings` module to retrieve a snapshot of historical OSM
     data as of a certain date, or to configure the Overpass server timeout,
@@ -136,16 +135,15 @@
     retain_all : bool
         if True, return the entire graph even if it is not connected.
         otherwise, retain only the largest weakly connected component.
     truncate_by_edge : bool
         if True, retain nodes outside bounding box if at least one of node's
         neighbors is within the bounding box
     clean_periphery : bool,
-        if True, buffer 500m to get a graph larger than requested, then
-        simplify, then truncate it to requested spatial boundaries
+        deprecated, do not use
     custom_filter : string
         a custom ways filter to be used instead of the network_type presets
         e.g., '["power"~"line"]' or '["highway"~"motorway|trunk"]'. Also pass
         in a network_type that is in settings.bidirectional_network_types if
         you want graph to be fully bi-directional.
 
     Returns
@@ -155,15 +153,16 @@
     Notes
     -----
     Very large query areas use the `utils_geo._consolidate_subdivide_geometry`
     function to automatically make multiple requests: see that function's
     documentation for caveats.
     """
     if dist_type not in {"bbox", "network"}:  # pragma: no cover
-        raise ValueError('dist_type must be "bbox" or "network"')
+        msg = 'dist_type must be "bbox" or "network"'
+        raise ValueError(msg)
 
     # create bounding box from center point and distance in each direction
     north, south, east, west = utils_geo.bbox_from_point(center_point, dist)
 
     # create a graph from the bounding box
     G = graph_from_bbox(
         north,
@@ -193,15 +192,15 @@
     dist=1000,
     dist_type="bbox",
     network_type="all_private",
     simplify=True,
     retain_all=False,
     truncate_by_edge=False,
     return_coords=False,
-    clean_periphery=True,
+    clean_periphery=None,
     custom_filter=None,
 ):
     """
     Download and create a graph within some distance of an address.
 
     You can use the `settings` module to retrieve a snapshot of historical OSM
     data as of a certain date, or to configure the Overpass server timeout,
@@ -227,17 +226,16 @@
         if True, return the entire graph even if it is not connected.
         otherwise, retain only the largest weakly connected component.
     truncate_by_edge : bool
         if True, retain nodes outside bounding box if at least one of node's
         neighbors is within the bounding box
     return_coords : bool
         optionally also return the geocoded coordinates of the address
-    clean_periphery : bool,
-        if True, buffer 500m to get a graph larger than requested, then
-        simplify, then truncate it to requested spatial boundaries
+    clean_periphery : bool
+        deprecated, do not use
     custom_filter : string
         a custom ways filter to be used instead of the network_type presets
         e.g., '["power"~"line"]' or '["highway"~"motorway|trunk"]'. Also pass
         in a network_type that is in settings.bidirectional_network_types if
         you want graph to be fully bi-directional.
 
     Returns
@@ -277,15 +275,15 @@
     query,
     network_type="all_private",
     simplify=True,
     retain_all=False,
     truncate_by_edge=False,
     which_result=None,
     buffer_dist=None,
-    clean_periphery=True,
+    clean_periphery=None,
     custom_filter=None,
 ):
     """
     Download and create a graph within the boundaries of some place(s).
 
     The query must be geocodable and OSM must have polygon boundaries for the
     geocode result. If OSM does not have a polygon for this place, you can
@@ -317,18 +315,17 @@
     truncate_by_edge : bool
         if True, retain nodes outside boundary polygon if at least one of
         node's neighbors is within the polygon
     which_result : int
         which geocoding result to use. if None, auto-select the first
         (Multi)Polygon or raise an error if OSM doesn't return one.
     buffer_dist : float
-        distance to buffer around the place geometry, in meters
+        deprecated, do not use
     clean_periphery : bool
-        if True, buffer 500m to get a graph larger than requested, then
-        simplify, then truncate it to requested spatial boundaries
+        deprecated, do not use
     custom_filter : string
         a custom ways filter to be used instead of the network_type presets
         e.g., '["power"~"line"]' or '["highway"~"motorway|trunk"]'. Also pass
         in a network_type that is in settings.bidirectional_network_types if
         you want graph to be fully bi-directional.
 
     Returns
@@ -337,26 +334,34 @@
 
     Notes
     -----
     Very large query areas use the `utils_geo._consolidate_subdivide_geometry`
     function to automatically make multiple requests: see that function's
     documentation for caveats.
     """
+    if buffer_dist is not None:
+        warn(
+            "The buffer_dist argument as been deprecated and will be removed "
+            "in a future release. Buffer your query area directly, if desired.",
+            stacklevel=2,
+        )
+
     # create a GeoDataFrame with the spatial boundaries of the place(s)
     if isinstance(query, (str, dict)):
         # if it is a string (place name) or dict (structured place query),
         # then it is a single place
         gdf_place = geocoder.geocode_to_gdf(
             query, which_result=which_result, buffer_dist=buffer_dist
         )
     elif isinstance(query, list):
         # if it is a list, it contains multiple places to get
         gdf_place = geocoder.geocode_to_gdf(query, buffer_dist=buffer_dist)
     else:  # pragma: no cover
-        raise TypeError("query must be dict, string, or list of strings")
+        msg = "query must be dict, string, or list of strings"
+        raise TypeError(msg)
 
     # extract the geometry from the GeoDataFrame to use in API query
     polygon = gdf_place["geometry"].unary_union
     utils.log("Constructed place geometry polygon(s) to query API")
 
     # create graph using this polygon(s) geometry
     G = graph_from_polygon(
@@ -375,15 +380,15 @@
 
 def graph_from_polygon(
     polygon,
     network_type="all_private",
     simplify=True,
     retain_all=False,
     truncate_by_edge=False,
-    clean_periphery=True,
+    clean_periphery=None,
     custom_filter=None,
 ):
     """
     Download and create a graph within the boundaries of a (multi)polygon.
 
     You can use the `settings` module to retrieve a snapshot of historical OSM
     data as of a certain date, or to configure the Overpass server timeout,
@@ -401,16 +406,15 @@
     retain_all : bool
         if True, return the entire graph even if it is not connected.
         otherwise, retain only the largest weakly connected component.
     truncate_by_edge : bool
         if True, retain nodes outside boundary polygon if at least one of
         node's neighbors is within the polygon
     clean_periphery : bool
-        if True, buffer 500m to get a graph larger than requested, then
-        simplify, then truncate it to requested spatial boundaries
+        deprecated, do not use
     custom_filter : string
         a custom ways filter to be used instead of the network_type presets
         e.g., '["power"~"line"]' or '["highway"~"motorway|trunk"]'. Also pass
         in a network_type that is in settings.bidirectional_network_types if
         you want graph to be fully bi-directional.
 
     Returns
@@ -419,35 +423,48 @@
 
     Notes
     -----
     Very large query areas use the `utils_geo._consolidate_subdivide_geometry`
     function to automatically make multiple requests: see that function's
     documentation for caveats.
     """
+    if clean_periphery is None:
+        clean_periphery = True
+    else:
+        warn(
+            "The clean_periphery argument has been deprecated and will be removed in "
+            "a future release. Future behavior will be as though clean_periphery=True.",
+            stacklevel=2,
+        )
+
     # verify that the geometry is valid and is a shapely Polygon/MultiPolygon
     # before proceeding
     if not polygon.is_valid:  # pragma: no cover
-        raise ValueError("The geometry to query within is invalid")
+        msg = "The geometry to query within is invalid"
+        raise ValueError(msg)
     if not isinstance(polygon, (Polygon, MultiPolygon)):  # pragma: no cover
-        raise TypeError(
-            "Geometry must be a shapely Polygon or MultiPolygon. If you requested "
-            "graph from place name, make sure your query resolves to a Polygon or "
-            "MultiPolygon, and not some other geometry, like a Point. See OSMnx "
-            "documentation for details."
+        msg = (
+            "Geometry must be a shapely Polygon or MultiPolygon. If you "
+            "requested graph from place name, make sure your query resolves "
+            "to a Polygon or MultiPolygon, and not some other geometry, like "
+            "a Point. See OSMnx documentation for details."
         )
+        raise TypeError(msg)
 
     if clean_periphery:
         # create a new buffered polygon 0.5km around the desired one
         buffer_dist = 500
         poly_proj, crs_utm = projection.project_geometry(polygon)
         poly_proj_buff = poly_proj.buffer(buffer_dist)
         poly_buff, _ = projection.project_geometry(poly_proj_buff, crs=crs_utm, to_latlong=True)
 
         # download the network data from OSM within buffered polygon
-        response_jsons = _downloader._osm_network_download(poly_buff, network_type, custom_filter)
+        response_jsons = _overpass._download_overpass_network(
+            poly_buff, network_type, custom_filter
+        )
 
         # create buffered graph from the downloaded data
         bidirectional = network_type in settings.bidirectional_network_types
         G_buff = _create_graph(response_jsons, retain_all=True, bidirectional=bidirectional)
 
         # truncate buffered graph to the buffered polygon and retain_all for
         # now. needed because overpass returns entire ways that also include
@@ -471,15 +488,15 @@
         # intersection, even if some of its neighbors are outside the polygon
         spn = stats.count_streets_per_node(G_buff, nodes=G.nodes)
         nx.set_node_attributes(G, values=spn, name="street_count")
 
     # if clean_periphery=False, just use the polygon as provided
     else:
         # download the network data from OSM
-        response_jsons = _downloader._osm_network_download(polygon, network_type, custom_filter)
+        response_jsons = _overpass._download_overpass_network(polygon, network_type, custom_filter)
 
         # create graph from the downloaded data
         bidirectional = network_type in settings.bidirectional_network_types
         G = _create_graph(response_jsons, retain_all=True, bidirectional=bidirectional)
 
         # truncate the graph to the extent of the polygon
         G = truncate.truncate_graph_polygon(G, polygon, retain_all, truncate_by_edge)
@@ -569,33 +586,34 @@
     response_count = 0
     nodes = {}
     paths = {}
 
     # consume response_jsons generator to download data from server
     for response_json in response_jsons:
         response_count += 1
+
+        # if cache_only_mode, consume response_jsons then continue next loop
         if settings.cache_only_mode:  # pragma: no cover
-            # if cache_only_mode, consume response_jsons then continue loop
             continue
-        else:
-            # otherwise, extract nodes and paths from the downloaded OSM data
-            nodes_temp, paths_temp = _parse_nodes_paths(response_json)
-            nodes.update(nodes_temp)
-            paths.update(paths_temp)
+
+        # otherwise, extract nodes and paths from the downloaded OSM data
+        nodes_temp, paths_temp = _parse_nodes_paths(response_json)
+        nodes.update(nodes_temp)
+        paths.update(paths_temp)
 
     utils.log(f"Retrieved all data from API in {response_count} request(s)")
     if settings.cache_only_mode:  # pragma: no cover
         # after consuming all response_jsons in loop, raise exception to catch
-        raise CacheOnlyModeInterrupt("Interrupted because `settings.cache_only_mode=True`")
+        msg = "Interrupted because `settings.cache_only_mode=True`"
+        raise CacheOnlyInterruptError(msg)
 
     # ensure we got some node/way data back from the server request(s)
     if (len(nodes) == 0) and (len(paths) == 0):  # pragma: no cover
-        raise EmptyOverpassResponse(
-            "No data elements in server response. Check query location/filters and log."
-        )
+        msg = "No data elements in server response. Check query location/filters and log."
+        raise InsufficientResponseError(msg)
 
     # create the MultiDiGraph and set its graph-level attributes
     metadata = {
         "created_date": utils.ts(),
         "created_with": f"OSMnx {__version__}",
         "crs": settings.default_crs,
     }
@@ -750,18 +768,15 @@
         the values OSM uses in its 'oneway' tag to denote travel can only
         occur in the opposite direction of the node order
 
     Returns
     -------
     bool
     """
-    if "oneway" in path and path["oneway"] in reversed_values:
-        return True
-    else:
-        return False
+    return "oneway" in path and path["oneway"] in reversed_values
 
 
 def _add_paths(G, paths, bidirectional=False):
     """
     Add a list of paths to the graph as edges.
 
     Parameters
```

### Comparing `osmnx-1.5.1/osmnx/io.py` & `osmnx-1.6.0/osmnx/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Serialize graphs to/from files on disk."""
 
 import ast
+import contextlib
 from pathlib import Path
 from warnings import warn
 
 import networkx as nx
 import pandas as pd
 from shapely import wkt
 
@@ -216,15 +217,16 @@
     Returns
     -------
     G : networkx.MultiDiGraph
     """
     if (filepath is None and graphml_str is None) or (
         filepath is not None and graphml_str is not None
     ):  # pragma: no cover
-        raise ValueError("You must pass one and only one of `filepath` or `graphml_str`.")
+        msg = "You must pass one and only one of `filepath` or `graphml_str`."
+        raise ValueError(msg)
 
     # specify default graph/node/edge attribute values' data types
     default_graph_dtypes = {"simplified": _convert_bool_string}
     default_node_dtypes = {
         "elevation": float,
         "elevation_res": float,
         "lat": float,
@@ -444,18 +446,16 @@
         # remove extraneous "id" attribute added by graphml saving
         data.pop("id", None)
 
         # first, eval stringified lists to convert them to list objects
         # edge attributes might have a single value, or a list if simplified
         for attr, value in data.items():
             if value.startswith("[") and value.endswith("]"):
-                try:
+                with contextlib.suppress(SyntaxError, ValueError):
                     data[attr] = ast.literal_eval(value)
-                except (SyntaxError, ValueError):
-                    pass
 
         # next, convert attribute value types if attribute appears in dtypes
         for attr in data.keys() & dtypes.keys():
             if isinstance(data[attr], list):
                 # if it's a list, eval it then convert each item
                 data[attr] = [dtypes[attr](item) for item in data[attr]]
             else:
@@ -490,15 +490,16 @@
     bool
     """
     if value in {"True", "False"}:
         return value == "True"
     elif isinstance(value, bool):
         return value
     else:  # pragma: no cover
-        raise ValueError(f"invalid literal for boolean: {value!r}")
+        msg = f"invalid literal for boolean: {value!r}"
+        raise ValueError(msg)
 
 
 def _stringify_nonnumeric_cols(gdf):
     """
     Make every non-numeric GeoDataFrame column (besides geometry) a string.
 
     This allows proper serializing via Fiona of GeoDataFrames with mixed types
@@ -511,12 +512,12 @@
 
     Returns
     -------
     gdf : geopandas.GeoDataFrame
         gdf with non-numeric columns stringified
     """
     # stringify every non-numeric column other than geometry column
-    for col in (c for c in gdf.columns if not c == "geometry"):
+    for col in (c for c in gdf.columns if c != "geometry"):
         if not pd.api.types.is_numeric_dtype(gdf[col]):
             gdf[col] = gdf[col].fillna("").astype(str)
 
     return gdf
```

### Comparing `osmnx-1.5.1/osmnx/osm_xml.py` & `osmnx-1.6.0/osmnx/osm_xml.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,20 +311,20 @@
 
     Returns
     -------
     root : ElementTree.Element
         xml tree with nodes appended
     """
     for _, row in gdf_nodes.iterrows():
-        row = row.dropna().astype(str)
-        node = ET.SubElement(root, "node", attrib=row[node_attrs].to_dict())
+        row_str = row.dropna().astype(str)
+        node = ET.SubElement(root, "node", attrib=row_str[node_attrs].to_dict())
 
         for tag in node_tags:
-            if tag in row:
-                ET.SubElement(node, "tag", attrib={"k": tag, "v": row[tag]})
+            if tag in row_str:
+                ET.SubElement(node, "tag", attrib={"k": tag, "v": row_str[tag]})
     return root
 
 
 def _create_way_for_each_edge(root, gdf_edges, edge_attrs, edge_tags):
     """
     Append a new way to an empty XML tree graph for each edge in way.
 
@@ -342,22 +342,21 @@
         GeoDataFrame of graph edges
     edge_attrs : list
         osm way attributes to include in output OSM XML
     edge_tags : list
         osm way tags to include in output OSM XML
     """
     for _, row in gdf_edges.iterrows():
-        row = row.dropna().astype(str)
-        edge = ET.SubElement(root, "way", attrib=row[edge_attrs].to_dict())
-        ET.SubElement(edge, "nd", attrib={"ref": row["u"]})
-        ET.SubElement(edge, "nd", attrib={"ref": row["v"]})
+        row_str = row.dropna().astype(str)
+        edge = ET.SubElement(root, "way", attrib=row_str[edge_attrs].to_dict())
+        ET.SubElement(edge, "nd", attrib={"ref": row_str["u"]})
+        ET.SubElement(edge, "nd", attrib={"ref": row_str["v"]})
         for tag in edge_tags:
-            if tag in row:
-                ET.SubElement(edge, "tag", attrib={"k": tag, "v": row[tag]})
-    return
+            if tag in row_str:
+                ET.SubElement(edge, "tag", attrib={"k": tag, "v": row_str[tag]})
 
 
 def _append_merged_edge_attrs(xml_edge, sample_edge, all_edges_df, edge_tags, edge_tag_aggs):
     """
     Extract edge attributes and append to XML edge.
 
     Parameters
@@ -396,15 +395,14 @@
                     xml_edge,
                     "tag",
                     attrib={
                         "k": tag,
                         "v": str(all_edges_df[tag].aggregate(agg)),
                     },
                 )
-    return
 
 
 def _append_nodes_as_edge_attrs(xml_edge, sample_edge, all_edges_df):
     """
     Extract list of ordered nodes and append as attributes of XML edge.
 
     Parameters
@@ -425,15 +423,14 @@
             ordered_nodes = _get_unique_nodes_ordered_from_way(all_edges_df)
         except nx.NetworkXUnfeasible:
             first_node = all_edges_df.iloc[0]["u"]
             ordered_nodes = _get_unique_nodes_ordered_from_way(all_edges_df.iloc[1:])
             ordered_nodes = [first_node] + ordered_nodes
         for node in ordered_nodes:
             ET.SubElement(xml_edge, "nd", attrib={"ref": str(node)})
-    return
 
 
 def _append_edges_xml_tree(root, gdf_edges, edge_attrs, edge_tags, edge_tag_aggs, merge_edges):
     """
     Append edges to an XML tree.
 
     Parameters
```

### Comparing `osmnx-1.5.1/osmnx/plot.py` & `osmnx-1.6.0/osmnx/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 from . import simplification
 from . import utils
 from . import utils_geo
 from . import utils_graph
 
 # matplotlib is an optional dependency needed for visualization
 try:
-    import matplotlib.cm as cm
-    import matplotlib.colors as colors
     import matplotlib.pyplot as plt
+    from matplotlib import cm
     from matplotlib import colormaps
+    from matplotlib import colors
 except ImportError:  # pragma: no cover
     cm = colors = plt = colormaps = None
 
 
 def get_colors(n, cmap="viridis", start=0.0, stop=1.0, alpha=1.0, return_hex=False):
     """
     Get `n` evenly-spaced colors from a matplotlib colormap.
@@ -204,15 +204,16 @@
     fig, ax : tuple
         matplotlib figure, axis
     """
     _verify_mpl()
     max_node_size = max(node_size) if hasattr(node_size, "__iter__") else node_size
     max_edge_lw = max(edge_linewidth) if hasattr(edge_linewidth, "__iter__") else edge_linewidth
     if max_node_size <= 0 and max_edge_lw <= 0:  # pragma: no cover
-        raise ValueError("Either node_size or edge_linewidth must be > 0 to plot something.")
+        msg = "Either node_size or edge_linewidth must be > 0 to plot something."
+        raise ValueError(msg)
 
     # create fig, ax as needed
     utils.log("Begin plotting the graph...")
     if ax is None:
         fig, ax = plt.subplots(figsize=figsize, facecolor=bgcolor, frameon=False)
         ax.set_facecolor(bgcolor)
     else:
@@ -353,25 +354,29 @@
     fig, ax : tuple
         matplotlib figure, axis
     """
     _verify_mpl()
 
     # check for valid arguments
     if not all(isinstance(r, list) for r in routes):  # pragma: no cover
-        raise ValueError("routes must be a list of route lists")
-    if len(routes) < 2:  # pragma: no cover
-        raise ValueError("You must pass more than 1 route")
+        msg = "routes must be a list of route lists"
+        raise ValueError(msg)
+    if len(routes) <= 1:  # pragma: no cover
+        msg = "You must pass more than 1 route"
+        raise ValueError(msg)
     if isinstance(route_colors, str):
         route_colors = [route_colors] * len(routes)
     if len(routes) != len(route_colors):  # pragma: no cover
-        raise ValueError("route_colors list must have same length as routes")
+        msg = "route_colors list must have same length as routes"
+        raise ValueError(msg)
     if isinstance(route_linewidths, int):
         route_linewidths = [route_linewidths] * len(routes)
     if len(routes) != len(route_linewidths):  # pragma: no cover
-        raise ValueError("route_linewidths list must have same length as routes")
+        msg = "route_linewidths list must have same length as routes"
+        raise ValueError(msg)
 
     # plot the graph and the first route
     override = {"route", "route_color", "route_linewidth", "show", "save", "close"}
     kwargs = {k: v for k, v in pgr_kwargs.items() if k not in override}
     fig, ax = plot_graph_route(
         G,
         route=routes[0],
@@ -496,15 +501,16 @@
             dist_type="bbox",
             network_type=network_type,
             simplify=False,
             truncate_by_edge=True,
         )
         G = simplification.simplify_graph(G, strict=False)
     else:  # pragma: no cover
-        raise ValueError("You must pass an address or lat-lng point or graph.")
+        msg = "You must pass an address or lat-lng point or graph."
+        raise ValueError(msg)
 
     # we need an undirected graph to find every edge incident on a node
     Gu = utils_graph.get_undirected(G)
 
     # for each edge, get a linewidth according to street type
     edge_linewidths = []
     for _, _, d in Gu.edges(keys=False, data=True):
@@ -681,15 +687,15 @@
 
     Parameters
     ----------
     Gu : networkx.MultiGraph
         undirected, unprojected graph with `bearing` attributes on each edge
     num_bins : int
         number of bins; for example, if `num_bins=36` is provided, then each
-        bin will represent 10° around the compass
+        bin will represent 10 degrees around the compass
     min_length : float
         ignore edges with `length` attributes less than `min_length`
     weight : string
         if not None, weight edges' bearings by this (non-null) edge attribute
     ax : matplotlib.axes.PolarAxesSubplot
         if not None, plot on this preexisting axis; must have projection=polar
     figsize : tuple
@@ -732,15 +738,15 @@
             "zorder": 3,
         }
 
     # get the bearings' distribution's bin counts and edges
     bin_counts, bin_edges = bearing._bearings_distribution(Gu, num_bins, min_length, weight)
 
     # positions: where to center each bar. ignore the last bin edge, because
-    # it's the same as the first (i.e., 0° = 360°)
+    # it's the same as the first (i.e., 0 degrees = 360 degrees)
     positions = np.radians(bin_edges[:-1])
 
     # width: make bars fill the circumference without gaps or overlaps
     width = 2 * np.pi / num_bins
 
     # radius: how long to make each bar
     bin_frequency = bin_counts / bin_counts.sum()
@@ -815,15 +821,16 @@
 
     Returns
     -------
     color_series : pandas.Series
         series labels are node/edge IDs and values are colors
     """
     if len(vals) == 0:
-        raise ValueError("There are no attribute values.")
+        msg = "There are no attribute values."
+        raise ValueError(msg)
 
     if num_bins is None:
         # calculate min/max values based on start/stop and data range
         vals_min = vals.dropna().min()
         vals_max = vals.dropna().max()
         full_range = (vals_max - vals_min) / (stop - start)
         full_min = vals_min - full_range * start
@@ -970,10 +977,9 @@
     Verify that matplotlib is installed and successfully imported.
 
     Returns
     -------
     None
     """
     if cm is None or colors is None or plt is None or colormaps is None:  # pragma: no cover
-        raise ImportError(
-            "matplotlib must be installed as an optional dependency for visualization"
-        )
+        msg = "matplotlib must be installed as an optional dependency for visualization"
+        raise ImportError(msg)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `osmnx-1.5.1/osmnx/projection.py` & `osmnx-1.6.0/osmnx/projection.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,30 +84,32 @@
 
     Returns
     -------
     gdf_proj : geopandas.GeoDataFrame
         the projected GeoDataFrame
     """
     if gdf.crs is None or len(gdf) < 1:  # pragma: no cover
-        raise ValueError("GeoDataFrame must have a valid CRS and cannot be empty")
+        msg = "GeoDataFrame must have a valid CRS and cannot be empty"
+        raise ValueError(msg)
 
     # if to_latlong is True, project the gdf to latlong
     if to_latlong:
         gdf_proj = gdf.to_crs(settings.default_crs)
         utils.log(f"Projected GeoDataFrame to {settings.default_crs}")
 
     # else if to_crs was passed-in, project gdf to this CRS
     elif to_crs is not None:
         gdf_proj = gdf.to_crs(to_crs)
         utils.log(f"Projected GeoDataFrame to {to_crs}")
 
     # otherwise, automatically project the gdf to UTM
     else:
         if is_projected(gdf.crs):  # pragma: no cover
-            raise ValueError("Geometry must be unprojected to calculate UTM zone")
+            msg = "Geometry must be unprojected to calculate UTM zone"
+            raise ValueError(msg)
 
         # calculate approximate longitude of centroid of union of all geometries in gdf
         avg_lng = gdf["geometry"].representative_point().x.mean()
 
         # calculate UTM zone from avg longitude to define CRS to project to
         utm_zone = int(np.floor((avg_lng + 180) / 6) + 1)
         utm_crs = f"+proj=utm +zone={utm_zone} +ellps=WGS84 +datum=WGS84 +units=m +no_defs"
```

### Comparing `osmnx-1.5.1/osmnx/settings.py` & `osmnx-1.6.0/osmnx/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,16 +108,16 @@
 requests_kwargs : dict
     Optional keyword args to pass to the requests package when connecting
     to APIs, for example to configure authentication or provide a path to
     a local certificate file. More info on options such as auth, cert,
     verify, and proxies can be found in the requests package advanced docs.
     Default is `{}`.
 timeout : int
-    The timeout interval in seconds for the HTTP request and for API to use
-    while running the query. Default is `180`.
+    The timeout interval in seconds for HTTP requests, and (when applicable)
+    for API to use while running the query. Default is `180`.
 use_cache : bool
     If True, cache HTTP responses locally instead of calling API repeatedly
     for the same request. Default is `True`.
 useful_tags_node : list
     OSM "node" tags to add as graph node attributes, when present in the data
     retrieved from OSM. Default is `["ref", "highway"]`.
 useful_tags_way : list
```

### Comparing `osmnx-1.5.1/osmnx/simplification.py` & `osmnx-1.6.0/osmnx/simplification.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from shapely.geometry import MultiPolygon
 from shapely.geometry import Point
 from shapely.geometry import Polygon
 
 from . import stats
 from . import utils
 from . import utils_graph
+from ._errors import GraphSimplificationError
 
 
 def _is_endpoint(G, node, strict=True):
     """
     Is node a true endpoint of an edge.
 
     Return True if the node is a "real" endpoint of an edge in the network,
@@ -53,15 +54,15 @@
 
     # rule 2
     elif G.out_degree(node) == 0 or G.in_degree(node) == 0:
         # if node has no incoming edges or no outgoing edges, it is an endpoint
         return True
 
     # rule 3
-    elif not (n == 2 and (d == 2 or d == 4)):
+    elif not ((n == 2) and (d in {2, 4})):  # noqa: PLR2004
         # else, if it does NOT have 2 neighbors AND either 2 or 4 directed
         # edges, it is an endpoint. either it has 1 or 3+ neighbors, in which
         # case it is a dead-end or an intersection of multiple streets or it has
         # 2 neighbors but 3 degree (indicating a change from oneway to twoway)
         # or more than 4 degree (indicating a parallel edge) and thus is an
         # endpoint
         return True
@@ -113,15 +114,16 @@
         nodes, and all other items are interstitial nodes that can be removed
         subsequently
     """
     # start building path from endpoint node through its successor
     path = [endpoint, endpoint_successor]
 
     # for each successor of the endpoint's successor
-    for successor in G.successors(endpoint_successor):
+    for this_successor in G.successors(endpoint_successor):
+        successor = this_successor
         if successor not in path:
             # if this successor is already in the path, ignore it, otherwise add
             # it to the path
             path.append(successor)
             while successor not in endpoints:
                 # find successors (of current successor) not in path
                 successors = [n for n in G.successors(successor) if n not in path]
@@ -145,15 +147,16 @@
                             f"Unexpected simplify pattern handled near {successor}", level=lg.WARN
                         )
                         return path
                 else:  # pragma: no cover
                     # if successor has >1 successors, then successor must have
                     # been an endpoint because you can go in 2 new directions.
                     # this should never occur in practice
-                    raise Exception(f"Unexpected simplify pattern failed near {successor}")
+                    msg = f"Unexpected simplify pattern failed near {successor}"
+                    raise GraphSimplificationError(msg)
 
             # if this successor is an endpoint, we've completed the path
             return path
 
     # if endpoint_successor has no successors not already in the path, return
     # the current path: this is usually due to a digitization quirk on OSM
     return path
@@ -250,15 +253,16 @@
     Returns
     -------
     G : networkx.MultiDiGraph
         topologically simplified graph, with a new `geometry` attribute on
         each simplified edge
     """
     if "simplified" in G.graph and G.graph["simplified"]:  # pragma: no cover
-        raise Exception("This graph has already been simplified, cannot simplify it again.")
+        msg = "This graph has already been simplified, cannot simplify it again."
+        raise GraphSimplificationError(msg)
 
     utils.log("Begin topologically simplifying the graph...")
 
     # define edge segment attributes to sum upon edge simplification
     attrs_to_sum = {"length", "travel_time"}
 
     # make a copy to not mutate original graph object caller passed in
@@ -425,22 +429,20 @@
 
     if rebuild_graph:
         if not G or not G.edges:
             # cannot rebuild a graph with no nodes or no edges, just return it
             return G
         else:
             return _consolidate_intersections_rebuild_graph(G, tolerance, reconnect_edges)
-
+    elif not G:
+        # if graph has no nodes, just return empty GeoSeries
+        return gpd.GeoSeries(crs=G.graph["crs"])
     else:
-        if not G:
-            # if graph has no nodes, just return empty GeoSeries
-            return gpd.GeoSeries(crs=G.graph["crs"])
-        else:
-            # return the centroids of the merged intersection polygons
-            return _merge_nodes_geometric(G, tolerance).centroid
+        # return the centroids of the merged intersection polygons
+        return _merge_nodes_geometric(G, tolerance).centroid
 
 
 def _merge_nodes_geometric(G, tolerance):
     """
     Geometrically merge nodes within some distance of each other.
 
     Parameters
```

### Comparing `osmnx-1.5.1/osmnx/speed.py` & `osmnx-1.6.0/osmnx/speed.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,19 +111,19 @@
     speed_kph = (
         edges[["highway", "speed_kph"]].set_index("highway").iloc[:, 0].fillna(hwy_speed_avg)
     )
 
     # all speeds will be null if edges had no preexisting maxspeed data and
     # caller did not pass in hwy_speeds or fallback arguments
     if pd.isnull(speed_kph).all():
-        raise ValueError(
-            "this graph's edges have no preexisting `maxspeed` "
-            "attribute values so you must pass `hwy_speeds` or "
-            "`fallback` arguments."
+        msg = (
+            "this graph's edges have no preexisting `maxspeed` attribute "
+            "values so you must pass `hwy_speeds` or `fallback` arguments."
         )
+        raise ValueError(msg)
 
     # add speed kph attribute to graph edges
     edges["speed_kph"] = speed_kph.round(precision).values
     nx.set_edge_attributes(G, values=edges["speed_kph"], name="speed_kph")
 
     return G
 
@@ -155,22 +155,23 @@
         warn(
             "the `precision` parameter is deprecated and will be removed in a future release",
             stacklevel=2,
         )
 
     edges = utils_graph.graph_to_gdfs(G, nodes=False)
 
-    # verify edge length and speed_kph attributes exist and contain no nulls
+    # verify edge length and speed_kph attributes exist
     if not ("length" in edges.columns and "speed_kph" in edges.columns):  # pragma: no cover
-        raise KeyError("all edges must have `length` and `speed_kph` attributes.")
-    else:
-        if (
-            pd.isnull(edges["length"]).any() or pd.isnull(edges["speed_kph"]).any()
-        ):  # pragma: no cover
-            raise ValueError("edge `length` and `speed_kph` values must be non-null.")
+        msg = "all edges must have `length` and `speed_kph` attributes."
+        raise KeyError(msg)
+
+    # verify edge length and speed_kph attributes contain no nulls
+    if pd.isnull(edges["length"]).any() or pd.isnull(edges["speed_kph"]).any():  # pragma: no cover
+        msg = "edge `length` and `speed_kph` values must be non-null."
+        raise ValueError(msg)
 
     # convert distance meters to km, and speed km per hour to km per second
     distance_km = edges["length"] / 1000
     speed_km_sec = edges["speed_kph"] / (60 * 60)
 
     # calculate edge travel time in seconds
     travel_time = distance_km / speed_km_sec
```

### Comparing `osmnx-1.5.1/osmnx/stats.py` & `osmnx-1.6.0/osmnx/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,16 @@
 
     Returns
     -------
     count : int
         count of street segments in graph
     """
     if nx.is_directed(Gu):  # pragma: no cover
-        raise ValueError("`Gu` must be undirected")
+        msg = "`Gu` must be undirected"
+        raise ValueError(msg)
     return len(Gu.edges)
 
 
 def street_length_total(Gu):
     """
     Calculate graph's total street segment length.
 
@@ -158,15 +159,16 @@
 
     Returns
     -------
     length : float
         total length (meters) of streets in graph
     """
     if nx.is_directed(Gu):  # pragma: no cover
-        raise ValueError("`Gu` must be undirected")
+        msg = "`Gu` must be undirected"
+        raise ValueError(msg)
     return sum(d["length"] for u, v, d in Gu.edges(data=True))
 
 
 def edge_length_total(G):
     """
     Calculate graph's total edge length.
 
@@ -196,15 +198,16 @@
 
     Returns
     -------
     proportion : float
         proportion of graph edges that are self-loops
     """
     if nx.is_directed(Gu):  # pragma: no cover
-        raise ValueError("`Gu` must be undirected")
+        msg = "`Gu` must be undirected"
+        raise ValueError(msg)
     return sum(u == v for u, v, k in Gu.edges) / len(Gu.edges)
 
 
 def circuity_avg(Gu):
     """
     Calculate average street circuity using edges of undirected graph.
 
@@ -219,15 +222,16 @@
 
     Returns
     -------
     circuity_avg : float
         the graph's average undirected edge circuity
     """
     if nx.is_directed(Gu):  # pragma: no cover
-        raise ValueError("`Gu` must be undirected")
+        msg = "`Gu` must be undirected"
+        raise ValueError(msg)
 
     # extract the edges' endpoint nodes' coordinates
     coords = np.array(
         [
             (Gu.nodes[u]["y"], Gu.nodes[u]["x"], Gu.nodes[v]["y"], Gu.nodes[v]["x"])
             for u, v, _ in Gu.edges
         ]
```

### Comparing `osmnx-1.5.1/osmnx/truncate.py` & `osmnx-1.6.0/osmnx/truncate.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,16 @@
 
     # first identify all nodes whose point geometries lie within the polygon
     gs_nodes = utils_graph.graph_to_gdfs(G, edges=False)[["geometry"]]
     to_keep = utils_geo._intersect_index_quadrats(gs_nodes, polygon, quadrat_width, min_num)
 
     if not to_keep:
         # no graph nodes within the polygon: can't create a graph from that
-        raise ValueError("Found no graph nodes within the requested polygon")
+        msg = "Found no graph nodes within the requested polygon"
+        raise ValueError(msg)
 
     # now identify all nodes whose point geometries lie outside the polygon
     gs_nodes_outside_poly = gs_nodes[~gs_nodes.index.isin(to_keep)]
     nodes_outside_poly = set(gs_nodes_outside_poly.index)
 
     if truncate_by_edge:
         # retain nodes outside boundary polygon if at least one of node's
```

### Comparing `osmnx-1.5.1/osmnx/utils.py` & `osmnx-1.6.0/osmnx/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,75 +27,78 @@
         citation format, either APA or BibTeX or IEEE
 
     Returns
     -------
     None
     """
     if style == "apa":
-        print(
+        msg = (
             "Boeing, G. (2017). OSMnx: New Methods for Acquiring, Constructing, "
             "Analyzing, and Visualizing Complex Street Networks. Computers, "
             "Environment and Urban Systems, 65, 126-139. "
             "https://doi.org/10.1016/j.compenvurbsys.2017.05.004"
         )
     elif style == "bibtex":
-        print(
+        msg = (
             "@article{boeing_osmnx_2017,\n"
             "    title = {{OSMnx}: {New} {Methods} for {Acquiring}, "
             "{Constructing}, {Analyzing}, and {Visualizing} {Complex} "
             "{Street} {Networks}},\n"
             "    volume = {65},\n"
             "    doi = {10.1016/j.compenvurbsys.2017.05.004},\n"
             "    number = {126-139},\n"
             "    journal = {Computers, Environment and Urban Systems},\n"
             "    author = {Boeing, Geoff},\n"
             "    year = {2017},\n"
             "    pages = {126--139}\n"
             "}"
         )
     elif style == "ieee":
-        print(
+        msg = (
             'G. Boeing, "OSMnx: New Methods for Acquiring, Constructing, '
             'Analyzing, and Visualizing Complex Street Networks," Computers, '
             "Environment and Urban Systems, vol. 65, pp. 126-139, 2017, "
             "doi: 10.1016/j.compenvurbsys.2017.05.004."
         )
     else:  # pragma: no cover
-        raise ValueError(f"unrecognized citation style {style!r}")
+        err_msg = f"unrecognized citation style {style!r}"
+        raise ValueError(err_msg)
+
+    print(msg)  # noqa: T201
 
 
 def ts(style="datetime", template=None):
     """
-    Return current timestamp as a string.
+    Return current local timestamp as a string.
 
     Parameters
     ----------
     style : string {"datetime", "date", "time"}
         format the timestamp with this built-in style
     template : string
         if not None, format the timestamp with this format string instead of
         one of the built-in styles
 
     Returns
     -------
     ts : string
-        timestamp string
+        local timestamp string
     """
     if template is None:
         if style == "datetime":
             template = "{:%Y-%m-%d %H:%M:%S}"
         elif style == "date":
             template = "{:%Y-%m-%d}"
         elif style == "time":
             template = "{:%H:%M:%S}"
         else:  # pragma: no cover
-            raise ValueError(f"unrecognized timestamp style {style!r}")
+            msg = f"unrecognized timestamp style {style!r}"
+            raise ValueError(msg)
 
-    ts = template.format(dt.datetime.now())
-    return ts
+    return template.format(dt.datetime.now().astimezone())
 
 
 def config(
     all_oneway=settings.all_oneway,
     bidirectional_network_types=settings.bidirectional_network_types,
     cache_folder=settings.cache_folder,
     cache_only_mode=settings.cache_only_mode,
```

### Comparing `osmnx-1.5.1/osmnx/utils_geo.py` & `osmnx-1.6.0/osmnx/utils_geo.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,16 @@
     """
     if isinstance(geom, LineString):
         num_vert = max(round(geom.length / dist), 1)
         for n in range(num_vert + 1):
             point = geom.interpolate(n / num_vert, normalized=True)
             yield point.x, point.y
     else:  # pragma: no cover
-        raise TypeError(f"unhandled geometry type {geom.geom_type}")
+        msg = f"unhandled geometry type {geom.geom_type}"
+        raise TypeError(msg)
 
 
 def _round_polygon_coords(p, precision):
     """
     Round the coordinates of a shapely Polygon to some decimal precision.
 
     Parameters
@@ -230,15 +231,16 @@
     elif isinstance(geom, Polygon):
         return _round_polygon_coords(geom, precision)
 
     elif isinstance(geom, MultiPolygon):
         return _round_multipolygon_coords(geom, precision)
 
     else:  # pragma: no cover
-        raise TypeError(f"cannot round coordinates of unhandled geometry type: {type(geom)}")
+        msg = f"cannot round coordinates of unhandled geometry type: {type(geom)}"
+        raise TypeError(msg)
 
 
 def _consolidate_subdivide_geometry(geometry, max_query_area_size=None):
     """
     Consolidate and subdivide some geometry.
 
     Consolidate a geometry into a convex hull, then subdivide it into smaller
@@ -267,15 +269,16 @@
         max_query_area_size = settings.max_query_area_size
 
     # let the linear length of the quadrats (with which to subdivide the
     # geometry) be the square root of max area size
     quadrat_width = np.sqrt(max_query_area_size)
 
     if not isinstance(geometry, (Polygon, MultiPolygon)):  # pragma: no cover
-        raise TypeError("Geometry must be a shapely Polygon or MultiPolygon")
+        msg = "Geometry must be a shapely Polygon or MultiPolygon"
+        raise TypeError(msg)
 
     # if geometry is either 1) a Polygon whose area exceeds the max size, or
     # 2) a MultiPolygon, then get the convex hull around the geometry
     if isinstance(geometry, MultiPolygon) or (
         isinstance(geometry, Polygon) and geometry.area > max_query_area_size
     ):
         geometry = geometry.convex_hull
@@ -302,15 +305,16 @@
         the geometry to extract exterior coordinates from
 
     Returns
     -------
     polygon_coord_strs : list
     """
     if not isinstance(geometry, MultiPolygon):  # pragma: no cover
-        raise TypeError("Geometry must be a shapely MultiPolygon")
+        msg = "Geometry must be a shapely MultiPolygon"
+        raise TypeError(msg)
 
     # extract geometry's exterior coords
     polygons_coords = []
     for polygon in geometry.geoms:
         x, y = polygon.exterior.xy
         polygons_coords.append(list(zip(x, y)))
 
@@ -405,19 +409,19 @@
     multipoly = _quadrat_cut_geometry(polygon, quadrat_width=quadrat_width, min_num=min_num)
     geoms_in_poly = set()
 
     # loop through each chunk of the polygon to find intersecting geometries
     for poly in multipoly.geoms:
         # first find approximate matches with spatial index, then precise
         # matches from those approximate ones
-        poly = poly.buffer(0)
-        if poly.is_valid and poly.area > 0:
-            possible_matches_iloc = sindex.intersection(poly.bounds)
+        poly_buff = poly.buffer(0)
+        if poly_buff.is_valid and poly_buff.area > 0:
+            possible_matches_iloc = sindex.intersection(poly_buff.bounds)
             possible_matches = geometries.iloc[list(possible_matches_iloc)]
-            precise_matches = possible_matches[possible_matches.intersects(poly)]
+            precise_matches = possible_matches[possible_matches.intersects(poly_buff)]
             geoms_in_poly.update(precise_matches.index)
 
     utils.log(f"Identified {len(geoms_in_poly):,} geometries inside polygon")
     return geoms_in_poly
 
 
 def bbox_from_point(point, dist=1000, project_utm=False, return_crs=False):
```

### Comparing `osmnx-1.5.1/osmnx/utils_graph.py` & `osmnx-1.6.0/osmnx/utils_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,16 @@
         is indexed by osmid and gdf_edges is multi-indexed by u, v, key
         following normal MultiDiGraph structure.
     """
     crs = G.graph["crs"]
 
     if nodes:
         if not G.nodes:  # pragma: no cover
-            raise ValueError("graph contains no nodes")
+            msg = "graph contains no nodes"
+            raise ValueError(msg)
 
         nodes, data = zip(*G.nodes(data=True))
 
         if node_geometry:
             # convert node x/y attributes to Points for geometry column
             geom = (Point(d["x"], d["y"]) for d in data)
             gdf_nodes = gpd.GeoDataFrame(data, index=nodes, crs=crs, geometry=list(geom))
@@ -54,15 +55,16 @@
             gdf_nodes = gpd.GeoDataFrame(data, index=nodes)
 
         gdf_nodes.index.rename("osmid", inplace=True)
         utils.log("Created nodes GeoDataFrame from graph")
 
     if edges:
         if not G.edges:  # pragma: no cover
-            raise ValueError("graph contains no edges")
+            msg = "graph contains no edges"
+            raise ValueError(msg)
 
         u, v, k, data = zip(*G.edges(keys=True, data=True))
 
         if fill_edge_geometry:
             # subroutine to get geometry for every edge: if edge already has
             # geometry return it, otherwise create it using the incident nodes
             x_lookup = nx.get_node_attributes(G, "x")
@@ -95,15 +97,16 @@
     if nodes and edges:
         return gdf_nodes, gdf_edges
     elif nodes:
         return gdf_nodes
     elif edges:
         return gdf_edges
     else:  # pragma: no cover
-        raise ValueError("you must request nodes or edges or both")
+        msg = "you must request nodes or edges or both"
+        raise ValueError(msg)
 
 
 def graph_from_gdfs(gdf_nodes, gdf_edges, graph_attrs=None):
     """
     Convert node and edge GeoDataFrames to a MultiDiGraph.
 
     This function is the inverse of `graph_to_gdfs` and is designed to work in
@@ -129,24 +132,26 @@
         only graph-level attribute (gdf_edges must have crs attribute set)
 
     Returns
     -------
     G : networkx.MultiDiGraph
     """
     if not ("x" in gdf_nodes.columns and "y" in gdf_nodes.columns):  # pragma: no cover
-        raise ValueError("gdf_nodes must contain x and y columns")
+        msg = "gdf_nodes must contain x and y columns"
+        raise ValueError(msg)
 
     # if gdf_nodes has a geometry attribute set, drop that column (as we use x
     # and y for geometry information) and warn the user if the geometry values
     # differ from the coordinates in the x and y columns
     if hasattr(gdf_nodes, "geometry"):
         try:
             all_x_match = (gdf_nodes.geometry.x == gdf_nodes["x"]).all()
             all_y_match = (gdf_nodes.geometry.y == gdf_nodes["y"]).all()
-            assert all_x_match and all_y_match
+            assert all_x_match
+            assert all_y_match
         except (AssertionError, ValueError):  # pragma: no cover
             # AssertionError if x/y coords don't match geometry column
             # ValueError if geometry column contains non-point geometry types
             warn(
                 "discarding the gdf_nodes geometry column, though its "
                 "values differ from the coordinates in the x and y columns",
                 stacklevel=2,
```

### Comparing `osmnx-1.5.1/.gitignore` & `osmnx-1.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `osmnx-1.5.1/LICENSE.txt` & `osmnx-1.6.0/LICENSE.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2016–2023 Geoff Boeing https://geoffboeing.com/
+Copyright (c) 2016-2023 Geoff Boeing https://geoffboeing.com/
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `osmnx-1.5.1/README.md` & `osmnx-1.6.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 
 **OSMnx** is a Python package to download, model, analyze, and visualize street networks and other geospatial features from OpenStreetMap. You can download and model walking, driving, or biking networks with a single line of code then easily analyze and visualize them. You can just as easily work with urban amenities/points of interest, building footprints, transit stops, elevation data, street orientations, speed/travel time, and routing.
 
 ## Citation
 
 If you use OSMnx in your work, please cite the journal article:
 
-Boeing, G. 2017. "[OSMnx: New Methods for Acquiring, Constructing, Analyzing, and Visualizing Complex Street Networks](https://geoffboeing.com/publications/osmnx-complex-street-networks/)." *Computers, Environment and Urban Systems* 65, 126–139.
+Boeing, G. 2017. "[OSMnx: New Methods for Acquiring, Constructing, Analyzing, and Visualizing Complex Street Networks](https://geoffboeing.com/publications/osmnx-complex-street-networks/)." _Computers, Environment and Urban Systems_ 65, 126-139.
 
 ## Getting Started
 
-Read the [Getting Started](https://osmnx.readthedocs.io/en/stable/getting-started.html) guide for an introduction to the package, then work through the [OSMnx Examples](https://github.com/gboeing/osmnx-examples) gallery for step-by-step tutorials and sample code.
+Read the [Getting Started](https://osmnx.readthedocs.io/en/stable/getting-started.html) guide for an introduction to the package and FAQ, then work through the [OSMnx Examples](https://github.com/gboeing/osmnx-examples) gallery for step-by-step tutorials and sample code.
 
 ## Installation
 
 Follow the [Installation](https://osmnx.readthedocs.io/en/stable/installation.html) guide to install OSMnx.
 
 ## Support
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `osmnx-1.5.1/PKG-INFO` & `osmnx-1.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osmnx
-Version: 1.5.1
+Version: 1.6.0
 Summary: Download, model, analyze, and visualize street networks and other geospatial features from OpenStreetMap
 Project-URL: Documentation, https://osmnx.readthedocs.io
 Project-URL: Repository, https://github.com/gboeing/osmnx
 Author-email: Geoff Boeing <boeing@usc.edu>
 Maintainer: OSMnx contributors
 License: MIT License
 License-File: LICENSE.txt
@@ -27,15 +27,15 @@
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.8
 Requires-Dist: geopandas>=0.12
 Requires-Dist: networkx>=2.5
 Requires-Dist: numpy>=1.20
 Requires-Dist: pandas>=1.1
-Requires-Dist: requests>=2.25
+Requires-Dist: requests>=2.27
 Requires-Dist: shapely>=2.0
 Provides-Extra: entropy
 Requires-Dist: scipy>=1.5; extra == 'entropy'
 Provides-Extra: neighbors
 Requires-Dist: scikit-learn>=0.23; extra == 'neighbors'
 Requires-Dist: scipy>=1.5; extra == 'neighbors'
 Provides-Extra: raster
@@ -56,19 +56,19 @@
 
 **OSMnx** is a Python package to download, model, analyze, and visualize street networks and other geospatial features from OpenStreetMap. You can download and model walking, driving, or biking networks with a single line of code then easily analyze and visualize them. You can just as easily work with urban amenities/points of interest, building footprints, transit stops, elevation data, street orientations, speed/travel time, and routing.
 
 ## Citation
 
 If you use OSMnx in your work, please cite the journal article:
 
-Boeing, G. 2017. "[OSMnx: New Methods for Acquiring, Constructing, Analyzing, and Visualizing Complex Street Networks](https://geoffboeing.com/publications/osmnx-complex-street-networks/)." *Computers, Environment and Urban Systems* 65, 126–139.
+Boeing, G. 2017. "[OSMnx: New Methods for Acquiring, Constructing, Analyzing, and Visualizing Complex Street Networks](https://geoffboeing.com/publications/osmnx-complex-street-networks/)." _Computers, Environment and Urban Systems_ 65, 126-139.
 
 ## Getting Started
 
-Read the [Getting Started](https://osmnx.readthedocs.io/en/stable/getting-started.html) guide for an introduction to the package, then work through the [OSMnx Examples](https://github.com/gboeing/osmnx-examples) gallery for step-by-step tutorials and sample code.
+Read the [Getting Started](https://osmnx.readthedocs.io/en/stable/getting-started.html) guide for an introduction to the package and FAQ, then work through the [OSMnx Examples](https://github.com/gboeing/osmnx-examples) gallery for step-by-step tutorials and sample code.
 
 ## Installation
 
 Follow the [Installation](https://osmnx.readthedocs.io/en/stable/installation.html) guide to install OSMnx.
 
 ## Support
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

