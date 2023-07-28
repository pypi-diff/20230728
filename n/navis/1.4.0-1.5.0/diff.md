# Comparing `tmp/navis-1.4.0.tar.gz` & `tmp/navis-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/navis-1.4.0.tar", last modified: Wed Dec 21 11:44:47 2022, max compression
+gzip compressed data, was "navis-1.5.0.tar", last modified: Fri Jul 28 08:22:55 2023, max compression
```

## Comparing `navis-1.4.0.tar` & `navis-1.5.0.tar`

### file list

```diff
@@ -1,194 +1,202 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (116)    35141 2022-12-21 11:44:42.000000 navis-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      268 2022-12-21 11:44:42.000000 navis-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     8577 2022-12-21 11:44:47.000000 navis-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     6937 2022-12-21 11:44:42.000000 navis-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/navis/
--rw-r--r--   0 runner    (1001) docker     (116)     1012 2022-12-21 11:44:43.000000 navis-1.4.0/navis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      688 2022-12-21 11:44:43.000000 navis-1.4.0/navis/__version__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4340 2022-12-21 11:44:43.000000 navis-1.4.0/navis/config.py
--rw-r--r--   0 runner    (1001) docker     (116)      762 2022-12-21 11:44:43.000000 navis-1.4.0/navis/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/navis/connectivity/
--rw-r--r--   0 runner    (1001) docker     (116)      940 2022-12-21 11:44:43.000000 navis-1.4.0/navis/connectivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4374 2022-12-21 11:44:43.000000 navis-1.4.0/navis/connectivity/cnmetrics.py
--rw-r--r--   0 runner    (1001) docker     (116)     4858 2022-12-21 11:44:43.000000 navis-1.4.0/navis/connectivity/matrix_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     6691 2022-12-21 11:44:43.000000 navis-1.4.0/navis/connectivity/predict.py
--rw-r--r--   0 runner    (1001) docker     (116)    19869 2022-12-21 11:44:43.000000 navis-1.4.0/navis/connectivity/similarity.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/navis/conversion/
--rw-r--r--   0 runner    (1001) docker     (116)      835 2022-12-21 11:44:43.000000 navis-1.4.0/navis/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    17472 2022-12-21 11:44:43.000000 navis-1.4.0/navis/conversion/converters.py
--rw-r--r--   0 runner    (1001) docker     (116)    18037 2022-12-21 11:44:43.000000 navis-1.4.0/navis/conversion/meshing.py
--rw-r--r--   0 runner    (1001) docker     (116)     6842 2022-12-21 11:44:43.000000 navis-1.4.0/navis/conversion/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/navis/core/
--rw-r--r--   0 runner    (1001) docker     (116)     1169 2022-12-21 11:44:43.000000 navis-1.4.0/navis/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    26391 2022-12-21 11:44:43.000000 navis-1.4.0/navis/core/base.py
--rw-r--r--   0 runner    (1001) docker     (116)    17823 2022-12-21 11:44:43.000000 navis-1.4.0/navis/core/core_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)    22028 2022-12-21 11:44:43.000000 navis-1.4.0/navis/core/dotprop.py
--rw-r--r--   0 runner    (1001) docker     (116)    15350 2022-12-21 11:44:43.000000 navis-1.4.0/navis/core/mesh.py
--rw-r--r--   0 runner    (1001) docker     (116)    34800 2022-12-21 11:44:43.000000 navis-1.4.0/navis/core/neuronlist.py
--rw-r--r--   0 runner    (1001) docker     (116)      895 2022-12-21 11:44:43.000000 navis-1.4.0/navis/core/neurons.py
--rw-r--r--   0 runner    (1001) docker     (116)    46188 2022-12-21 11:44:43.000000 navis-1.4.0/navis/core/skeleton.py
--rw-r--r--   0 runner    (1001) docker     (116)    22037 2022-12-21 11:44:43.000000 navis-1.4.0/navis/core/volumes.py
--rw-r--r--   0 runner    (1001) docker     (116)    13041 2022-12-21 11:44:43.000000 navis-1.4.0/navis/core/voxel.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/navis/data/
--rw-r--r--   0 runner    (1001) docker     (116)      740 2022-12-21 11:44:43.000000 navis-1.4.0/navis/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/navis/data/gml/
--rw-r--r--   0 runner    (1001) docker     (116)   500970 2022-12-21 11:44:43.000000 navis-1.4.0/navis/data/gml/1734350788.gml
--rw-r--r--   0 runner    (1001) docker     (116)   545251 2022-12-21 11:44:43.000000 navis-1.4.0/navis/data/gml/1734350908.gml
--rw-r--r--   0 runner    (1001) docker     (116)   485390 2022-12-21 11:44:43.000000 navis-1.4.0/navis/data/gml/722817260.gml
--rw-r--r--   0 runner    (1001) docker     (116)   528774 2022-12-21 11:44:43.000000 navis-1.4.0/navis/data/gml/754534424.gml
--rw-r--r--   0 runner    (1001) docker     (116)   549154 2022-12-21 11:44:43.000000 navis-1.4.0/navis/data/gml/754538881.gml
--rw-r--r--   0 runner    (1001) docker     (116)     6924 2022-12-21 11:44:43.000000 navis-1.4.0/navis/data/load_data.py
--rw-r--r--   0 runner    (1001) docker     (116)      492 2022-12-21 11:44:43.000000 navis-1.4.0/navis/data/meta.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/navis/data/obj/
--rw-r--r--   0 runner    (1001) docker     (116)   509952 2022-12-21 11:44:43.000000 navis-1.4.0/navis/data/obj/1734350788.obj
--rw-r--r--   0 runner    (1001) docker     (116)   573635 2022-12-21 11:44:43.000000 navis-1.4.0/navis/data/obj/1734350908.obj
--rw-r--r--   0 runner    (1001) docker     (116)   534422 2022-12-21 11:44:43.000000 navis-1.4.0/navis/data/obj/722817260.obj
--rw-r--r--   0 runner    (1001) docker     (116)   533660 2022-12-21 11:44:43.000000 navis-1.4.0/navis/data/obj/754534424.obj
--rw-r--r--   0 runner    (1001) docker     (116)   531212 2022-12-21 11:44:43.000000 navis-1.4.0/navis/data/obj/754538881.obj
--rw-r--r--   0 runner    (1001) docker     (116)      642 2022-12-21 11:44:43.000000 navis-1.4.0/navis/data/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/navis/data/swc/
--rw-r--r--   0 runner    (1001) docker     (116)   186313 2022-12-21 11:44:43.000000 navis-1.4.0/navis/data/swc/1734350788.swc
--rw-r--r--   0 runner    (1001) docker     (116)   202615 2022-12-21 11:44:43.000000 navis-1.4.0/navis/data/swc/1734350908.swc
--rw-r--r--   0 runner    (1001) docker     (116)   180566 2022-12-21 11:44:43.000000 navis-1.4.0/navis/data/swc/722817260.swc
--rw-r--r--   0 runner    (1001) docker     (116)   196153 2022-12-21 11:44:43.000000 navis-1.4.0/navis/data/swc/754534424.swc
--rw-r--r--   0 runner    (1001) docker     (116)   203788 2022-12-21 11:44:43.000000 navis-1.4.0/navis/data/swc/754538881.swc
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/navis/data/synapses/
--rw-r--r--   0 runner    (1001) docker     (116)   124574 2022-12-21 11:44:43.000000 navis-1.4.0/navis/data/synapses/1734350788.csv
--rw-r--r--   0 runner    (1001) docker     (116)   140166 2022-12-21 11:44:43.000000 navis-1.4.0/navis/data/synapses/1734350908.csv
--rw-r--r--   0 runner    (1001) docker     (116)   144503 2022-12-21 11:44:43.000000 navis-1.4.0/navis/data/synapses/722817260.csv
--rw-r--r--   0 runner    (1001) docker     (116)   139110 2022-12-21 11:44:43.000000 navis-1.4.0/navis/data/synapses/754534424.csv
--rw-r--r--   0 runner    (1001) docker     (116)   135951 2022-12-21 11:44:43.000000 navis-1.4.0/navis/data/synapses/754538881.csv
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/navis/data/volumes/
--rw-r--r--   0 runner    (1001) docker     (116)    27418 2022-12-21 11:44:43.000000 navis-1.4.0/navis/data/volumes/lh.obj
--rw-r--r--   0 runner    (1001) docker     (116)   719824 2022-12-21 11:44:43.000000 navis-1.4.0/navis/data/volumes/neuropil.obj
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/navis/graph/
--rw-r--r--   0 runner    (1001) docker     (116)     1859 2022-12-21 11:44:43.000000 navis-1.4.0/navis/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7108 2022-12-21 11:44:43.000000 navis-1.4.0/navis/graph/clinic.py
--rw-r--r--   0 runner    (1001) docker     (116)    24336 2022-12-21 11:44:43.000000 navis-1.4.0/navis/graph/converters.py
--rw-r--r--   0 runner    (1001) docker     (116)    72493 2022-12-21 11:44:43.000000 navis-1.4.0/navis/graph/graph_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/navis/interfaces/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:43.000000 navis-1.4.0/navis/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2939 2022-12-21 11:44:43.000000 navis-1.4.0/navis/interfaces/allen_celltypes.py
--rw-r--r--   0 runner    (1001) docker     (116)    40988 2022-12-21 11:44:43.000000 navis-1.4.0/navis/interfaces/blender.py
--rw-r--r--   0 runner    (1001) docker     (116)     4939 2022-12-21 11:44:43.000000 navis-1.4.0/navis/interfaces/cytoscape.py
--rw-r--r--   0 runner    (1001) docker     (116)    20984 2022-12-21 11:44:43.000000 navis-1.4.0/navis/interfaces/insectbrain_db.py
--rw-r--r--   0 runner    (1001) docker     (116)    13222 2022-12-21 11:44:43.000000 navis-1.4.0/navis/interfaces/microns.py
--rw-r--r--   0 runner    (1001) docker     (116)    20168 2022-12-21 11:44:43.000000 navis-1.4.0/navis/interfaces/neuprint.py
--rw-r--r--   0 runner    (1001) docker     (116)     9254 2022-12-21 11:44:43.000000 navis-1.4.0/navis/interfaces/neuromorpho.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/navis/interfaces/neuron/
--rw-r--r--   0 runner    (1001) docker     (116)       83 2022-12-21 11:44:43.000000 navis-1.4.0/navis/interfaces/neuron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    31672 2022-12-21 11:44:43.000000 navis-1.4.0/navis/interfaces/neuron/comp.py
--rw-r--r--   0 runner    (1001) docker     (116)    27762 2022-12-21 11:44:43.000000 navis-1.4.0/navis/interfaces/neuron/network.py
--rw-r--r--   0 runner    (1001) docker     (116)     1284 2022-12-21 11:44:43.000000 navis-1.4.0/navis/interfaces/neuron/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)    61225 2022-12-21 11:44:43.000000 navis-1.4.0/navis/interfaces/r.py
--rw-r--r--   0 runner    (1001) docker     (116)    11695 2022-12-21 11:44:43.000000 navis-1.4.0/navis/interfaces/vfb.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/navis/intersection/
--rw-r--r--   0 runner    (1001) docker     (116)      821 2022-12-21 11:44:43.000000 navis-1.4.0/navis/intersection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2098 2022-12-21 11:44:43.000000 navis-1.4.0/navis/intersection/convex.py
--rw-r--r--   0 runner    (1001) docker     (116)    17628 2022-12-21 11:44:43.000000 navis-1.4.0/navis/intersection/intersect.py
--rw-r--r--   0 runner    (1001) docker     (116)     4137 2022-12-21 11:44:43.000000 navis-1.4.0/navis/intersection/ray.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/navis/io/
--rw-r--r--   0 runner    (1001) docker     (116)     1306 2022-12-21 11:44:43.000000 navis-1.4.0/navis/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    30437 2022-12-21 11:44:43.000000 navis-1.4.0/navis/io/base.py
--rw-r--r--   0 runner    (1001) docker     (116)    41325 2022-12-21 11:44:43.000000 navis-1.4.0/navis/io/hdf_io.py
--rw-r--r--   0 runner    (1001) docker     (116)     4364 2022-12-21 11:44:43.000000 navis-1.4.0/navis/io/json_io.py
--rw-r--r--   0 runner    (1001) docker     (116)    11421 2022-12-21 11:44:43.000000 navis-1.4.0/navis/io/mesh_io.py
--rw-r--r--   0 runner    (1001) docker     (116)     7135 2022-12-21 11:44:43.000000 navis-1.4.0/navis/io/nmx_io.py
--rw-r--r--   0 runner    (1001) docker     (116)    14530 2022-12-21 11:44:43.000000 navis-1.4.0/navis/io/nrrd_io.py
--rw-r--r--   0 runner    (1001) docker     (116)    22308 2022-12-21 11:44:43.000000 navis-1.4.0/navis/io/precomputed_io.py
--rw-r--r--   0 runner    (1001) docker     (116)     7970 2022-12-21 11:44:43.000000 navis-1.4.0/navis/io/rda_io.py
--rw-r--r--   0 runner    (1001) docker     (116)    25489 2022-12-21 11:44:43.000000 navis-1.4.0/navis/io/swc_io.py
--rw-r--r--   0 runner    (1001) docker     (116)     9974 2022-12-21 11:44:43.000000 navis-1.4.0/navis/io/tiff_io.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/navis/matching/
--rw-r--r--   0 runner    (1001) docker     (116)      766 2022-12-21 11:44:43.000000 navis-1.4.0/navis/matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10115 2022-12-21 11:44:43.000000 navis-1.4.0/navis/matching/bipartite.py
--rw-r--r--   0 runner    (1001) docker     (116)     7624 2022-12-21 11:44:43.000000 navis-1.4.0/navis/matching/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/navis/meshes/
--rw-r--r--   0 runner    (1001) docker     (116)      946 2022-12-21 11:44:43.000000 navis-1.4.0/navis/meshes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5436 2022-12-21 11:44:43.000000 navis-1.4.0/navis/meshes/b3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     2077 2022-12-21 11:44:43.000000 navis-1.4.0/navis/meshes/fqmr.py
--rw-r--r--   0 runner    (1001) docker     (116)    17290 2022-12-21 11:44:43.000000 navis-1.4.0/navis/meshes/mesh_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     4072 2022-12-21 11:44:43.000000 navis-1.4.0/navis/meshes/o3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     9294 2022-12-21 11:44:43.000000 navis-1.4.0/navis/meshes/operations.py
--rw-r--r--   0 runner    (1001) docker     (116)     3697 2022-12-21 11:44:43.000000 navis-1.4.0/navis/meshes/pyml.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/navis/meshes/templates/
--rw-r--r--   0 runner    (1001) docker     (116)     1182 2022-12-21 11:44:43.000000 navis-1.4.0/navis/meshes/templates/blender_decimate.py.template
--rw-r--r--   0 runner    (1001) docker     (116)     1154 2022-12-21 11:44:43.000000 navis-1.4.0/navis/meshes/templates/blender_smooth.py.template
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/navis/models/
--rw-r--r--   0 runner    (1001) docker     (116)      665 2022-12-21 11:44:43.000000 navis-1.4.0/navis/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    22896 2022-12-21 11:44:43.000000 navis-1.4.0/navis/models/network_models.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/navis/morpho/
--rw-r--r--   0 runner    (1001) docker     (116)     2241 2022-12-21 11:44:43.000000 navis-1.4.0/navis/morpho/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3008 2022-12-21 11:44:43.000000 navis-1.4.0/navis/morpho/analyze.py
--rw-r--r--   0 runner    (1001) docker     (116)     5945 2022-12-21 11:44:43.000000 navis-1.4.0/navis/morpho/fq.py
--rw-r--r--   0 runner    (1001) docker     (116)    80124 2022-12-21 11:44:43.000000 navis-1.4.0/navis/morpho/manipulation.py
--rw-r--r--   0 runner    (1001) docker     (116)    61726 2022-12-21 11:44:43.000000 navis-1.4.0/navis/morpho/mmetrics.py
--rw-r--r--   0 runner    (1001) docker     (116)    12435 2022-12-21 11:44:43.000000 navis-1.4.0/navis/morpho/persistence.py
--rw-r--r--   0 runner    (1001) docker     (116)    11671 2022-12-21 11:44:43.000000 navis-1.4.0/navis/morpho/subset.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/navis/nbl/
--rw-r--r--   0 runner    (1001) docker     (116)      944 2022-12-21 11:44:43.000000 navis-1.4.0/navis/nbl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6598 2022-12-21 11:44:43.000000 navis-1.4.0/navis/nbl/base.py
--rw-r--r--   0 runner    (1001) docker     (116)    62723 2022-12-21 11:44:43.000000 navis-1.4.0/navis/nbl/nblast_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/navis/nbl/score_mats/
--rw-r--r--   0 runner    (1001) docker     (116)     3083 2022-12-21 11:44:43.000000 navis-1.4.0/navis/nbl/score_mats/smat_alpha_fcwb.csv
--rw-r--r--   0 runner    (1001) docker     (116)     3979 2022-12-21 11:44:43.000000 navis-1.4.0/navis/nbl/score_mats/smat_fcwb.csv
--rw-r--r--   0 runner    (1001) docker     (116)    40790 2022-12-21 11:44:43.000000 navis-1.4.0/navis/nbl/smat.py
--rw-r--r--   0 runner    (1001) docker     (116)    21255 2022-12-21 11:44:43.000000 navis-1.4.0/navis/nbl/synblast_funcs.py
--rw-r--r--   0 runner    (1001) docker     (116)    12486 2022-12-21 11:44:43.000000 navis-1.4.0/navis/nbl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/navis/plotting/
--rw-r--r--   0 runner    (1001) docker     (116)      904 2022-12-21 11:44:43.000000 navis-1.4.0/navis/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    24972 2022-12-21 11:44:43.000000 navis-1.4.0/navis/plotting/colors.py
--rw-r--r--   0 runner    (1001) docker     (116)     7373 2022-12-21 11:44:43.000000 navis-1.4.0/navis/plotting/d.py
--rw-r--r--   0 runner    (1001) docker     (116)    48337 2022-12-21 11:44:43.000000 navis-1.4.0/navis/plotting/dd.py
--rw-r--r--   0 runner    (1001) docker     (116)    20753 2022-12-21 11:44:43.000000 navis-1.4.0/navis/plotting/ddd.py
--rw-r--r--   0 runner    (1001) docker     (116)    16502 2022-12-21 11:44:43.000000 navis-1.4.0/navis/plotting/flat.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/navis/plotting/k3d/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:43.000000 navis-1.4.0/navis/plotting/k3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      194 2022-12-21 11:44:43.000000 navis-1.4.0/navis/plotting/k3d/conftest.py
--rw-r--r--   0 runner    (1001) docker     (116)    15616 2022-12-21 11:44:43.000000 navis-1.4.0/navis/plotting/k3d/k3d_objects.py
--rw-r--r--   0 runner    (1001) docker     (116)    11012 2022-12-21 11:44:43.000000 navis-1.4.0/navis/plotting/plot_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/navis/plotting/plotly/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:43.000000 navis-1.4.0/navis/plotting/plotly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    24528 2022-12-21 11:44:43.000000 navis-1.4.0/navis/plotting/plotly/graph_objs.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/navis/plotting/vispy/
--rw-r--r--   0 runner    (1001) docker     (116)       44 2022-12-21 11:44:43.000000 navis-1.4.0/navis/plotting/vispy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    48166 2022-12-21 11:44:43.000000 navis-1.4.0/navis/plotting/vispy/viewer.py
--rw-r--r--   0 runner    (1001) docker     (116)    27085 2022-12-21 11:44:43.000000 navis-1.4.0/navis/plotting/vispy/visuals.py
--rw-r--r--   0 runner    (1001) docker     (116)     2373 2022-12-21 11:44:43.000000 navis-1.4.0/navis/plotting/vispy/vputils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/navis/sampling/
--rw-r--r--   0 runner    (1001) docker     (116)      819 2022-12-21 11:44:43.000000 navis-1.4.0/navis/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8875 2022-12-21 11:44:43.000000 navis-1.4.0/navis/sampling/downsampling.py
--rw-r--r--   0 runner    (1001) docker     (116)    18706 2022-12-21 11:44:43.000000 navis-1.4.0/navis/sampling/resampling.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/navis/transforms/
--rw-r--r--   0 runner    (1001) docker     (116)     1184 2022-12-21 11:44:43.000000 navis-1.4.0/navis/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3268 2022-12-21 11:44:43.000000 navis-1.4.0/navis/transforms/affine.py
--rw-r--r--   0 runner    (1001) docker     (116)    11571 2022-12-21 11:44:43.000000 navis-1.4.0/navis/transforms/base.py
--rw-r--r--   0 runner    (1001) docker     (116)    15283 2022-12-21 11:44:43.000000 navis-1.4.0/navis/transforms/cmtk.py
--rw-r--r--   0 runner    (1001) docker     (116)    10109 2022-12-21 11:44:43.000000 navis-1.4.0/navis/transforms/elastix.py
--rw-r--r--   0 runner    (1001) docker     (116)     2989 2022-12-21 11:44:43.000000 navis-1.4.0/navis/transforms/factory.py
--rw-r--r--   0 runner    (1001) docker     (116)    19064 2022-12-21 11:44:43.000000 navis-1.4.0/navis/transforms/h5reg.py
--rw-r--r--   0 runner    (1001) docker     (116)     7544 2022-12-21 11:44:43.000000 navis-1.4.0/navis/transforms/h5reg_java.py
--rw-r--r--   0 runner    (1001) docker     (116)     3922 2022-12-21 11:44:43.000000 navis-1.4.0/navis/transforms/moving_least_squares.py
--rw-r--r--   0 runner    (1001) docker     (116)    49397 2022-12-21 11:44:43.000000 navis-1.4.0/navis/transforms/templates.py
--rw-r--r--   0 runner    (1001) docker     (116)     4803 2022-12-21 11:44:43.000000 navis-1.4.0/navis/transforms/thinplate.py
--rw-r--r--   0 runner    (1001) docker     (116)    20451 2022-12-21 11:44:43.000000 navis-1.4.0/navis/transforms/xfm_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/navis/utils/
--rw-r--r--   0 runner    (1001) docker     (116)     1479 2022-12-21 11:44:43.000000 navis-1.4.0/navis/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4249 2022-12-21 11:44:43.000000 navis-1.4.0/navis/utils/cv.py
--rw-r--r--   0 runner    (1001) docker     (116)    21944 2022-12-21 11:44:43.000000 navis-1.4.0/navis/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (116)    10788 2022-12-21 11:44:43.000000 navis-1.4.0/navis/utils/eval.py
--rw-r--r--   0 runner    (1001) docker     (116)      923 2022-12-21 11:44:43.000000 navis-1.4.0/navis/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     3335 2022-12-21 11:44:43.000000 navis-1.4.0/navis/utils/iterables.py
--rw-r--r--   0 runner    (1001) docker     (116)    12683 2022-12-21 11:44:43.000000 navis-1.4.0/navis/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (116)     5134 2022-12-21 11:44:43.000000 navis-1.4.0/navis/utils/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-21 11:44:47.000000 navis-1.4.0/navis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     8577 2022-12-21 11:44:47.000000 navis-1.4.0/navis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4285 2022-12-21 11:44:47.000000 navis-1.4.0/navis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-21 11:44:47.000000 navis-1.4.0/navis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-21 11:44:47.000000 navis-1.4.0/navis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)     1350 2022-12-21 11:44:47.000000 navis-1.4.0/navis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        6 2022-12-21 11:44:47.000000 navis-1.4.0/navis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       92 2022-12-21 11:44:43.000000 navis-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-12-21 11:44:47.000000 navis-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2587 2022-12-21 11:44:43.000000 navis-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.789556 navis-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-28 08:22:49.000000 navis-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-28 08:22:49.000000 navis-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-07-28 08:22:55.785556 navis-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-07-28 08:22:49.000000 navis-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.725555 navis-1.5.0/navis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-28 08:22:51.000000 navis-1.5.0/navis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-28 08:22:51.000000 navis-1.5.0/navis/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-07-28 08:22:51.000000 navis-1.5.0/navis/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-28 08:22:51.000000 navis-1.5.0/navis/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.729555 navis-1.5.0/navis/connectivity/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-28 08:22:51.000000 navis-1.5.0/navis/connectivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-28 08:22:51.000000 navis-1.5.0/navis/connectivity/cnmetrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-07-28 08:22:51.000000 navis-1.5.0/navis/connectivity/matrix_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-28 08:22:51.000000 navis-1.5.0/navis/connectivity/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19869 2023-07-28 08:22:51.000000 navis-1.5.0/navis/connectivity/similarity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.729555 navis-1.5.0/navis/conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-28 08:22:51.000000 navis-1.5.0/navis/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20355 2023-07-28 08:22:51.000000 navis-1.5.0/navis/conversion/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-07-28 08:22:51.000000 navis-1.5.0/navis/conversion/meshing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-07-28 08:22:51.000000 navis-1.5.0/navis/conversion/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.733555 navis-1.5.0/navis/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-28 08:22:51.000000 navis-1.5.0/navis/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26391 2023-07-28 08:22:51.000000 navis-1.5.0/navis/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18002 2023-07-28 08:22:51.000000 navis-1.5.0/navis/core/core_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22028 2023-07-28 08:22:51.000000 navis-1.5.0/navis/core/dotprop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15350 2023-07-28 08:22:51.000000 navis-1.5.0/navis/core/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38381 2023-07-28 08:22:51.000000 navis-1.5.0/navis/core/neuronlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-28 08:22:51.000000 navis-1.5.0/navis/core/neurons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46188 2023-07-28 08:22:51.000000 navis-1.5.0/navis/core/skeleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22037 2023-07-28 08:22:51.000000 navis-1.5.0/navis/core/volumes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13041 2023-07-28 08:22:51.000000 navis-1.5.0/navis/core/voxel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.733555 navis-1.5.0/navis/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.737555 navis-1.5.0/navis/data/gml/
+-rw-r--r--   0 runner    (1001) docker     (123)   500970 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/gml/1734350788.gml
+-rw-r--r--   0 runner    (1001) docker     (123)   545251 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/gml/1734350908.gml
+-rw-r--r--   0 runner    (1001) docker     (123)   485390 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/gml/722817260.gml
+-rw-r--r--   0 runner    (1001) docker     (123)   528774 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/gml/754534424.gml
+-rw-r--r--   0 runner    (1001) docker     (123)   549154 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/gml/754538881.gml
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/meta.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.741555 navis-1.5.0/navis/data/obj/
+-rw-r--r--   0 runner    (1001) docker     (123)   509952 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/obj/1734350788.obj
+-rw-r--r--   0 runner    (1001) docker     (123)   573635 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/obj/1734350908.obj
+-rw-r--r--   0 runner    (1001) docker     (123)   534422 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/obj/722817260.obj
+-rw-r--r--   0 runner    (1001) docker     (123)   533660 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/obj/754534424.obj
+-rw-r--r--   0 runner    (1001) docker     (123)   531212 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/obj/754538881.obj
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.745555 navis-1.5.0/navis/data/swc/
+-rw-r--r--   0 runner    (1001) docker     (123)   186313 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/swc/1734350788.swc
+-rw-r--r--   0 runner    (1001) docker     (123)   202615 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/swc/1734350908.swc
+-rw-r--r--   0 runner    (1001) docker     (123)   180566 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/swc/722817260.swc
+-rw-r--r--   0 runner    (1001) docker     (123)   196153 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/swc/754534424.swc
+-rw-r--r--   0 runner    (1001) docker     (123)   203788 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/swc/754538881.swc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.745555 navis-1.5.0/navis/data/synapses/
+-rw-r--r--   0 runner    (1001) docker     (123)   124574 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/synapses/1734350788.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   140166 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/synapses/1734350908.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   144503 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/synapses/722817260.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   139110 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/synapses/754534424.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   135951 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/synapses/754538881.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.749555 navis-1.5.0/navis/data/volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)    27418 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/volumes/lh.obj
+-rw-r--r--   0 runner    (1001) docker     (123)   719824 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/volumes/neuropil.obj
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.749555 navis-1.5.0/navis/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-28 08:22:51.000000 navis-1.5.0/navis/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-07-28 08:22:51.000000 navis-1.5.0/navis/graph/clinic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24337 2023-07-28 08:22:51.000000 navis-1.5.0/navis/graph/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72995 2023-07-28 08:22:51.000000 navis-1.5.0/navis/graph/graph_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.753555 navis-1.5.0/navis/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:51.000000 navis-1.5.0/navis/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-28 08:22:51.000000 navis-1.5.0/navis/interfaces/allen_celltypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40988 2023-07-28 08:22:51.000000 navis-1.5.0/navis/interfaces/blender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-28 08:22:51.000000 navis-1.5.0/navis/interfaces/cytoscape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20984 2023-07-28 08:22:51.000000 navis-1.5.0/navis/interfaces/insectbrain_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13317 2023-07-28 08:22:51.000000 navis-1.5.0/navis/interfaces/microns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-07-28 08:22:51.000000 navis-1.5.0/navis/interfaces/neuprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9254 2023-07-28 08:22:51.000000 navis-1.5.0/navis/interfaces/neuromorpho.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.753555 navis-1.5.0/navis/interfaces/neuron/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-28 08:22:51.000000 navis-1.5.0/navis/interfaces/neuron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31672 2023-07-28 08:22:51.000000 navis-1.5.0/navis/interfaces/neuron/comp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30302 2023-07-28 08:22:51.000000 navis-1.5.0/navis/interfaces/neuron/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-28 08:22:51.000000 navis-1.5.0/navis/interfaces/neuron/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61225 2023-07-28 08:22:51.000000 navis-1.5.0/navis/interfaces/r.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11695 2023-07-28 08:22:51.000000 navis-1.5.0/navis/interfaces/vfb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.757556 navis-1.5.0/navis/intersection/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-28 08:22:51.000000 navis-1.5.0/navis/intersection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-28 08:22:51.000000 navis-1.5.0/navis/intersection/convex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-07-28 08:22:51.000000 navis-1.5.0/navis/intersection/intersect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-07-28 08:22:51.000000 navis-1.5.0/navis/intersection/ray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.761556 navis-1.5.0/navis/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-28 08:22:51.000000 navis-1.5.0/navis/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30440 2023-07-28 08:22:51.000000 navis-1.5.0/navis/io/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41325 2023-07-28 08:22:51.000000 navis-1.5.0/navis/io/hdf_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-28 08:22:51.000000 navis-1.5.0/navis/io/json_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-07-28 08:22:51.000000 navis-1.5.0/navis/io/mesh_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-07-28 08:22:51.000000 navis-1.5.0/navis/io/nmx_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14530 2023-07-28 08:22:51.000000 navis-1.5.0/navis/io/nrrd_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22308 2023-07-28 08:22:51.000000 navis-1.5.0/navis/io/precomputed_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-07-28 08:22:51.000000 navis-1.5.0/navis/io/rda_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25489 2023-07-28 08:22:51.000000 navis-1.5.0/navis/io/swc_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-07-28 08:22:51.000000 navis-1.5.0/navis/io/tiff_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.761556 navis-1.5.0/navis/matching/
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-28 08:22:51.000000 navis-1.5.0/navis/matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10115 2023-07-28 08:22:51.000000 navis-1.5.0/navis/matching/bipartite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-07-28 08:22:51.000000 navis-1.5.0/navis/matching/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.765556 navis-1.5.0/navis/meshes/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-28 08:22:51.000000 navis-1.5.0/navis/meshes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-07-28 08:22:51.000000 navis-1.5.0/navis/meshes/b3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-28 08:22:51.000000 navis-1.5.0/navis/meshes/fqmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17290 2023-07-28 08:22:51.000000 navis-1.5.0/navis/meshes/mesh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-07-28 08:22:51.000000 navis-1.5.0/navis/meshes/o3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9294 2023-07-28 08:22:51.000000 navis-1.5.0/navis/meshes/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-28 08:22:51.000000 navis-1.5.0/navis/meshes/pyml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.765556 navis-1.5.0/navis/meshes/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-28 08:22:51.000000 navis-1.5.0/navis/meshes/templates/blender_decimate.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-28 08:22:51.000000 navis-1.5.0/navis/meshes/templates/blender_smooth.py.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.765556 navis-1.5.0/navis/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-28 08:22:51.000000 navis-1.5.0/navis/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23204 2023-07-28 08:22:51.000000 navis-1.5.0/navis/models/network_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.765556 navis-1.5.0/navis/morpho/
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-28 08:22:51.000000 navis-1.5.0/navis/morpho/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-28 08:22:51.000000 navis-1.5.0/navis/morpho/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-07-28 08:22:51.000000 navis-1.5.0/navis/morpho/fq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81191 2023-07-28 08:22:51.000000 navis-1.5.0/navis/morpho/manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61726 2023-07-28 08:22:51.000000 navis-1.5.0/navis/morpho/mmetrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14387 2023-07-28 08:22:51.000000 navis-1.5.0/navis/morpho/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11705 2023-07-28 08:22:51.000000 navis-1.5.0/navis/morpho/subset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.769556 navis-1.5.0/navis/nbl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-28 08:22:51.000000 navis-1.5.0/navis/nbl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25736 2023-07-28 08:22:51.000000 navis-1.5.0/navis/nbl/ablast_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-28 08:22:51.000000 navis-1.5.0/navis/nbl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66298 2023-07-28 08:22:51.000000 navis-1.5.0/navis/nbl/nblast_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.769556 navis-1.5.0/navis/nbl/score_mats/
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-28 08:22:51.000000 navis-1.5.0/navis/nbl/score_mats/smat_alpha_fcwb.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-07-28 08:22:51.000000 navis-1.5.0/navis/nbl/score_mats/smat_fcwb.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    40790 2023-07-28 08:22:51.000000 navis-1.5.0/navis/nbl/smat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21255 2023-07-28 08:22:51.000000 navis-1.5.0/navis/nbl/synblast_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14594 2023-07-28 08:22:51.000000 navis-1.5.0/navis/nbl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.773556 navis-1.5.0/navis/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24991 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48337 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/dd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20753 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/ddd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16502 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/flat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.773556 navis-1.5.0/navis/plotting/k3d/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/k3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/k3d/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15616 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/k3d/k3d_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/plot_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.773556 navis-1.5.0/navis/plotting/plotly/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/plotly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/plotly/graph_objs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.777556 navis-1.5.0/navis/plotting/vispy/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/vispy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48166 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/vispy/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27104 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/vispy/visuals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/vispy/vputils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.777556 navis-1.5.0/navis/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-28 08:22:51.000000 navis-1.5.0/navis/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8875 2023-07-28 08:22:51.000000 navis-1.5.0/navis/sampling/downsampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18706 2023-07-28 08:22:51.000000 navis-1.5.0/navis/sampling/resampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.781556 navis-1.5.0/navis/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-28 08:22:51.000000 navis-1.5.0/navis/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-07-28 08:22:51.000000 navis-1.5.0/navis/transforms/affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-07-28 08:22:51.000000 navis-1.5.0/navis/transforms/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-07-28 08:22:51.000000 navis-1.5.0/navis/transforms/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15283 2023-07-28 08:22:51.000000 navis-1.5.0/navis/transforms/cmtk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-07-28 08:22:51.000000 navis-1.5.0/navis/transforms/elastix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-07-28 08:22:51.000000 navis-1.5.0/navis/transforms/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19064 2023-07-28 08:22:51.000000 navis-1.5.0/navis/transforms/h5reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-07-28 08:22:51.000000 navis-1.5.0/navis/transforms/h5reg_java.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-28 08:22:51.000000 navis-1.5.0/navis/transforms/moving_least_squares.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51158 2023-07-28 08:22:51.000000 navis-1.5.0/navis/transforms/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-07-28 08:22:51.000000 navis-1.5.0/navis/transforms/thinplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20684 2023-07-28 08:22:51.000000 navis-1.5.0/navis/transforms/xfm_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.785556 navis-1.5.0/navis/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-28 08:22:51.000000 navis-1.5.0/navis/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-07-28 08:22:51.000000 navis-1.5.0/navis/utils/cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21944 2023-07-28 08:22:51.000000 navis-1.5.0/navis/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-07-28 08:22:51.000000 navis-1.5.0/navis/utils/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-28 08:22:51.000000 navis-1.5.0/navis/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-28 08:22:51.000000 navis-1.5.0/navis/utils/iterables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12683 2023-07-28 08:22:51.000000 navis-1.5.0/navis/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-07-28 08:22:51.000000 navis-1.5.0/navis/utils/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.729555 navis-1.5.0/navis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-07-28 08:22:55.000000 navis-1.5.0/navis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-07-28 08:22:55.000000 navis-1.5.0/navis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:22:55.000000 navis-1.5.0/navis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:22:55.000000 navis-1.5.0/navis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-28 08:22:55.000000 navis-1.5.0/navis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 08:22:55.000000 navis-1.5.0/navis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 08:22:51.000000 navis-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 08:22:55.789556 navis-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-07-28 08:22:51.000000 navis-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.785556 navis-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-28 08:22:51.000000 navis-1.5.0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-28 08:22:51.000000 navis-1.5.0/tests/test_neurons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-28 08:22:51.000000 navis-1.5.0/tests/test_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-28 08:22:51.000000 navis-1.5.0/tests/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-28 08:22:51.000000 navis-1.5.0/tests/test_transforms.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `navis-1.4.0/LICENSE` & `navis-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/PKG-INFO` & `navis-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: navis
-Version: 1.4.0
+Version: 1.5.0
 Summary: Neuron Analysis and Visualization library
 Home-page: http://navis.readthedocs.io
 Author: Philipp Schlegel
 Author-email: pms70@cam.ac.uk
 License: GNU GPL V3
 Project-URL: Documentation, http://navis.readthedocs.io
 Project-URL: Source, https://github.com/navis-org/navis
 Project-URL: Changelog, https://navis.readthedocs.io/en/latest/source/whats_new.html
-Keywords: Neuron Analysis Visualization Anatomy Connectivity Transform Neuroscience NBLAST Skeletons SWC neuPrint
+Keywords: Neuron Analysis Visualization Morphometrics Morphology Anatomy Connectivity Transform Neuroscience NBLAST Skeletons SWC neuPrint
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: pathos
 Provides-Extra: shapely
 Provides-Extra: r
 Provides-Extra: kdtree
 Provides-Extra: hash
 Provides-Extra: flybrains
@@ -45,15 +45,15 @@
 Provides-Extra: vispy-tk
 License-File: LICENSE
 
 [![Documentation Status](https://readthedocs.org/projects/navis/badge/?version=latest)](http://navis.readthedocs.io/en/latest/?badge=latest) [![Tests](https://github.com/navis-org/navis/actions/workflows/test-package.yml/badge.svg)](https://github.com/navis-org/navis/actions/workflows/test-package.yml) [![Run notebooks](https://github.com/navis-org/navis/actions/workflows/notebooktest-package.yml/badge.svg)](https://github.com/navis-org/navis/actions/workflows/notebooktest-package.yml) [![Coverage Status](https://coveralls.io/repos/github/navis-org/navis/badge.svg?branch=master)](https://coveralls.io/github/navis-org/navis?branch=master) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/navis-org/navis/blob/master/examples/colab.ipynb) [![DOI](https://zenodo.org/badge/168142416.svg)](https://zenodo.org/badge/latestdoi/168142416) [![Downloads](https://pepy.tech/badge/navis)](https://pepy.tech/project/navis)
 
 <img src="https://github.com/navis-org/navis/raw/master/docs/_static/favicon.png" height="60">
 
-NAVis is a Python 3 (3.7 or later) library for **N**euron **A**nalysis and **Vis**ualization.
+NAVis is a Python 3 (3.8 or later) library for **N**euron **A**nalysis and **Vis**ualization.
 
 ## Documentation
 NAVis is on [ReadTheDocs](http://navis.readthedocs.io/ "NAVis ReadTheDocs").
 
 ## Features
 * works as Jupyter notebook, script or from terminal
 * support for various neuron types: **skeletons**, **meshes**, **dotprops**, **voxels**
@@ -103,17 +103,17 @@
 ## NAVis & friends
 <p align="center">
 <img src="https://github.com/navis-org/navis/blob/master/docs/_static/navis_ecosystem.png?raw=true" width="700">
 </p>
 
 NAVis comes with batteries included but is also highly extensible. Some
 libraries built on top of NAVis:
-* [flybrains](https://github.com/navis-org/navis-flybrains) provides templates and transforms to use with navis
+* [flybrains](https://github.com/navis-org/navis-flybrains) provides templates and transforms for *Drosophila* brains to use with navis
 * [pymaid](https://pymaid.readthedocs.io/en/latest/) pulls and pushes data from/to CATMAID servers
-* [fafbseg](https://fafbseg-py.readthedocs.io/en/latest/index.html) contains tools to work with autosegmented data for the FAFB EM dataset
+* [fafbseg](https://fafbseg-py.readthedocs.io/en/latest/index.html) contains tools to work with auto-segmented data for the FAFB EM dataset
 
 ## License
 This code is under GNU GPL V3
 
 ## Acknowledgments
 NAVis is inspired by and inherits much of its design from the excellent
 [natverse](http://natverse.org) R packages by
```

### Comparing `navis-1.4.0/README.md` & `navis-1.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [![Documentation Status](https://readthedocs.org/projects/navis/badge/?version=latest)](http://navis.readthedocs.io/en/latest/?badge=latest) [![Tests](https://github.com/navis-org/navis/actions/workflows/test-package.yml/badge.svg)](https://github.com/navis-org/navis/actions/workflows/test-package.yml) [![Run notebooks](https://github.com/navis-org/navis/actions/workflows/notebooktest-package.yml/badge.svg)](https://github.com/navis-org/navis/actions/workflows/notebooktest-package.yml) [![Coverage Status](https://coveralls.io/repos/github/navis-org/navis/badge.svg?branch=master)](https://coveralls.io/github/navis-org/navis?branch=master) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/navis-org/navis/blob/master/examples/colab.ipynb) [![DOI](https://zenodo.org/badge/168142416.svg)](https://zenodo.org/badge/latestdoi/168142416) [![Downloads](https://pepy.tech/badge/navis)](https://pepy.tech/project/navis)
 
 <img src="https://github.com/navis-org/navis/raw/master/docs/_static/favicon.png" height="60">
 
-NAVis is a Python 3 (3.7 or later) library for **N**euron **A**nalysis and **Vis**ualization.
+NAVis is a Python 3 (3.8 or later) library for **N**euron **A**nalysis and **Vis**ualization.
 
 ## Documentation
 NAVis is on [ReadTheDocs](http://navis.readthedocs.io/ "NAVis ReadTheDocs").
 
 ## Features
 * works as Jupyter notebook, script or from terminal
 * support for various neuron types: **skeletons**, **meshes**, **dotprops**, **voxels**
@@ -56,17 +56,17 @@
 ## NAVis & friends
 <p align="center">
 <img src="https://github.com/navis-org/navis/blob/master/docs/_static/navis_ecosystem.png?raw=true" width="700">
 </p>
 
 NAVis comes with batteries included but is also highly extensible. Some
 libraries built on top of NAVis:
-* [flybrains](https://github.com/navis-org/navis-flybrains) provides templates and transforms to use with navis
+* [flybrains](https://github.com/navis-org/navis-flybrains) provides templates and transforms for *Drosophila* brains to use with navis
 * [pymaid](https://pymaid.readthedocs.io/en/latest/) pulls and pushes data from/to CATMAID servers
-* [fafbseg](https://fafbseg-py.readthedocs.io/en/latest/index.html) contains tools to work with autosegmented data for the FAFB EM dataset
+* [fafbseg](https://fafbseg-py.readthedocs.io/en/latest/index.html) contains tools to work with auto-segmented data for the FAFB EM dataset
 
 ## License
 This code is under GNU GPL V3
 
 ## Acknowledgments
 NAVis is inspired by and inherits much of its design from the excellent
 [natverse](http://natverse.org) R packages by
```

### Comparing `navis-1.4.0/navis/__init__.py` & `navis-1.5.0/navis/__init__.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/__version__.py` & `navis-1.5.0/navis/__version__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 #    (at your option) any later version.
 #
 #    This program is distributed in the hope that it will be useful,
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 
-__version__ = "1.4.0"
-__version_vector__ = (1, 4, 0)
+__version__ = "1.5.0"
+__version_vector__ = (1, 5, 0)
```

### Comparing `navis-1.4.0/navis/config.py` & `navis-1.5.0/navis/config.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/conftest.py` & `navis-1.5.0/navis/conftest.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/connectivity/__init__.py` & `navis-1.5.0/navis/connectivity/__init__.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/connectivity/cnmetrics.py` & `navis-1.5.0/navis/connectivity/cnmetrics.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/connectivity/matrix_utils.py` & `navis-1.5.0/navis/connectivity/matrix_utils.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/connectivity/predict.py` & `navis-1.5.0/navis/connectivity/predict.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/connectivity/similarity.py` & `navis-1.5.0/navis/connectivity/similarity.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/conversion/__init__.py` & `navis-1.5.0/navis/conversion/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,12 +7,12 @@
 #    (at your option) any later version.
 #
 #    This program is distributed in the hope that it will be useful,
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 
-from .converters import tree2meshneuron, neuron2voxels, mesh2skeleton
+from .converters import tree2meshneuron, neuron2voxels, mesh2skeleton, points2skeleton
 from .meshing import voxels2mesh
 from .wrappers import skeletonize, voxelize, mesh
 
 __all__ = ['skeletonize', 'voxelize', 'mesh']
```

### Comparing `navis-1.4.0/navis/conversion/converters.py` & `navis-1.5.0/navis/conversion/converters.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,25 +10,115 @@
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 
 import numpy as np
 import skeletor as sk
 import trimesh as tm
+import networkx as nx
 
 from numbers import Number
 from scipy.ndimage import gaussian_filter
 from typing import Union, Optional
 
 from .. import core, config, utils, morpho, graph
 
 logger = config.get_logger(__name__)
 
 
 @utils.map_neuronlist(desc='Skeletonizing', allow_parallel=True)
+def points2skeleton(x: Union['core.Dotprops', np.ndarray],
+                    k: int = 10,
+                    max_dist: Optional[float] = None):
+    """Turn points into skeleton.
+
+    This function works by:
+     1. Compute the ``k`` nearest neighbors for each point
+     2. Generate a graph from the nearest-neighbor edges
+     3. Extract a minimum-spanning tree (MST) from the graph
+     4. Process the MST into a skeleton
+
+    Parameters
+    ----------
+    x :         (N, 3) array | Dotprops
+                Points to skeletonize.
+    k :         int
+                Number of nearest neighbors to consider. Too low values of `k`
+                can lead to disconnected skeletons.
+    max_dist :  float, optional
+                Edges longer than this will be ignored. This can lead to a
+                fragmented (i.e. multi-root) skeleton!
+
+    Returns
+    -------
+    skeleton :  navis.TreeNeuron
+
+    Examples
+    --------
+    >>> import navis
+    >>> # Get a mesh neuron
+    >>> n = navis.example_neurons(1)
+    >>> # Get the points
+    >>> pts = n.nodes[['x', 'y', 'z']].values
+    >>> # Convert points back into skeleton
+    >>> sk = navis.conversion.points2skeleton(pts)
+
+    """
+    utils.eval_param(x, name='x', allowed_types=(core.Dotprops, np.ndarray))
+
+    if isinstance(x, core.Dotprops):
+        pts = x.points
+    else:
+        if (x.ndim != 2) and (x.shape[1] != 3):
+            raise ValueError(f'Points must be shape (N, 3), got {x.shape}')
+        pts = x
+
+    # Get the list of nearest neighbours
+    tree = core.dotprop.KDTree(pts)
+
+    defaults = {}
+    if max_dist is not None:
+        # We have to avoid passing `None` because scipy's KDTree does not like
+        # that (pykdtree does not care)
+        defaults['distance_upper_bound'] = max_dist
+    dists, NN = tree.query(pts, k=k + 1, **defaults)
+
+    # Drop self-hits
+    dists, NN = dists[:, 1:], NN[:, 1:]
+
+    # Turn into edges
+    edges = []
+    ix1 = np.arange(len(dists))
+    for i in range(k):
+        ix2 = NN[:, i]
+        le = dists[:, i]
+        # If a max dist was set we have to remove NN that have dist np.inf
+        if max_dist is None:
+            edges += list(zip(ix1, ix2, le))
+        else:
+            not_inf = le != np.inf
+            edges += list(zip(ix1[not_inf], ix2[not_inf], le[not_inf]))
+
+    # Generate graph
+    G = nx.Graph()
+    G.add_nodes_from(ix1)
+    G.add_weighted_edges_from(edges)
+
+    # Extract minimum spanning tree
+    G_mst = nx.minimum_spanning_tree(G)
+
+    # Add the coordinates as node properties
+    nx.set_node_attributes(G_mst, dict(zip(G.nodes, pts[:, 0])), name='x')
+    nx.set_node_attributes(G_mst, dict(zip(G.nodes, pts[:, 1])), name='y')
+    nx.set_node_attributes(G_mst, dict(zip(G.nodes, pts[:, 2])), name='z')
+
+    return graph.nx2neuron(G_mst)
+
+
+@utils.map_neuronlist(desc='Skeletonizing', allow_parallel=True)
 def mesh2skeleton(x: 'core.MeshNeuron',
                   method: str = 'wavefront',
                   fix_mesh: bool = False,
                   shave: bool = True,
                   heal: bool = False,
                   connectors: bool = False,
                   inv_dist: Union[int, float] = None,
```

### Comparing `navis-1.4.0/navis/conversion/meshing.py` & `navis-1.5.0/navis/conversion/meshing.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/conversion/wrappers.py` & `navis-1.5.0/navis/conversion/wrappers.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,68 +14,87 @@
 import trimesh as tm
 import numpy as np
 
 from typing import Union, Optional
 from typing_extensions import Literal
 
 from .. import core, config, utils
-from .converters import neuron2voxels, mesh2skeleton, tree2meshneuron
+from .converters import (neuron2voxels, mesh2skeleton, tree2meshneuron,
+                         points2skeleton)
 from .meshing import voxels2mesh
 
 logger = config.get_logger(__name__)
 
 
 @utils.map_neuronlist(desc='Skeletonizing', allow_parallel=True)
-def skeletonize(x: 'core.MeshNeuron',
+def skeletonize(x: Union['core.MeshNeuron', 'core.Dotprops', np.ndarray],
                 **kwargs):
     """Turn neuron into skeleton.
 
-    Currently, we can only skeletonize meshes but are looking into ways to do
-    the same for VoxelNeuron.
+    Currently, we can only skeletonize meshes, dotprops and point clouds but
+    are looking into ways to also do it for ``VoxelNeurons``.
 
-    This function is a thin-wrapper for `skeletor`. It uses sensible defaults
-    for neurons but if you want to fine-tune your skeletons you should look
-    into using `skeletor` directly.
+    For meshes, this function is a thin-wrapper for `skeletor`. It uses sensible
+    defaults for neurons but if you want to fine-tune your skeletons you should
+    look into using `skeletor` directly.
 
     Parameters
     ----------
-    x :         MeshNeuron | trimesh.Trimesh
+    x :         MeshNeuron | trimesh.Trimesh | Dotprops
                 Mesh(es) to skeletonize. Note that the quality of the results
                 very much depends on the mesh, so it might be worth doing some
                 pre-processing (see below).
     **kwargs
                 Keyword arguments are passed through to the respective
-                converters: currently only :func:`navis.conversion.mesh2skeleton`.
+                converters:
+                    - meshes: :func:`navis.conversion.mesh2skeleton`
+                    - dotprops and point clouds: :func:`navis.conversion.points2skeleton`
 
     Returns
     -------
     skeleton :  navis.TreeNeuron
-                Has a `.vertex_map` attribute that maps each vertex in the
-                input mesh to a skeleton node ID.
+                For meshes, this has a `.vertex_map` attribute that maps each
+                vertex in the input mesh to a skeleton node ID.
 
     See Also
     --------
     :func:`navis.drop_fluff`
                 Use this if your mesh has lots of tiny free floating bits to
                 reduce noise and speed up skeletonization.
 
     Examples
     --------
+    # Skeletonize a mesh
     >>> import navis
     >>> # Get a mesh neuron
     >>> n = navis.example_neurons(1, kind='mesh')
     >>> # Convert to skeleton
     >>> sk = navis.skeletonize(n)
     >>> # Mesh vertex indices to node IDs map
     >>> sk.vertex_map                                           # doctest: +SKIP
     array([938, 990, 990, ...,  39, 234, 234])
 
+    # Skeletonize dotprops (i.e. point-clouds)
+    >>> import navis
+    >>> # Get a skeleton and turn into dotprops
+    >>> dp = navis.make_dotprops(navis.example_neurons(1))
+    >>> # Turn back into a skeleton
+    >>> sk = navis.skeletonize(dp)
+
     """
     if isinstance(x, (core.MeshNeuron, tm.Trimesh)):
         return mesh2skeleton(x, **kwargs)
+    elif isinstance(x, (core.Dotprops, )):
+        sk = points2skeleton(x.points, **kwargs)
+        for attr in ('id', 'units', 'name'):
+            if hasattr(x, attr):
+                setattr(sk, attr, getattr(x, attr))
+        return sk
+    elif isinstance(x, np.ndarray):
+        return points2skeleton(x.points, **kwargs)
 
     raise TypeError(f'Unable to skeletonize data of type {type(x)}')
 
 
 @utils.map_neuronlist(desc='Voxelizing', allow_parallel=True)
 def voxelize(x: 'core.BaseNeuron',
              pitch: Union[list, tuple, float],
```

### Comparing `navis-1.4.0/navis/core/__init__.py` & `navis-1.5.0/navis/core/__init__.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/core/base.py` & `navis-1.5.0/navis/core/base.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/core/core_utils.py` & `navis-1.5.0/navis/core/core_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,15 +65,15 @@
                   threshold: float = None) -> Union['core.Dotprops', 'core.NeuronList']:
     """Produce dotprops from neurons or x/y/z points.
 
     This is following the implementation in R's `nat` library.
 
     Parameters
     ----------
-    x :         TreeNeuron | MeshNeuron | VoxelNeuron | NeuronList | pandas.DataFrame | numpy.ndarray
+    x :         Neuron | NeuronList | pandas.DataFrame | numpy.ndarray
                 Data/object to generate dotprops from. DataFrame must have
                 'x', 'y' and 'z' columns.
     k :         int (> 1), optional
                 Number of nearest neighbours to use for tangent vector
                 calculation:
 
                   - ``k=0`` or ``k=None`` is possible but only for
@@ -145,14 +145,19 @@
 
         x = x.nodes[['x', 'y', 'z']].values
     elif isinstance(x, core.MeshNeuron):
         properties.update({'units': x.units, 'name': x.name, 'id': x.id})
         x = x.vertices
         if resample:
             x, _ = tm.points.remove_close(x, resample)
+    elif isinstance(x, core.Dotprops):
+        properties.update({'units': x.units, 'name': x.name, 'id': x.id})
+        x = x.points
+        if resample:
+            x, _ = tm.points.remove_close(x, resample)
     elif isinstance(x, core.VoxelNeuron):
         properties.update({'name': x.name, 'id': x.id})
         if not x.units.dimensionless:
             # We are scaling the units - hence all are set to 1
             properties['units'] = [f'1 {u.units}' for u in x.units_xyz]
 
         if threshold:
```

### Comparing `navis-1.4.0/navis/core/dotprop.py` & `navis-1.5.0/navis/core/dotprop.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/core/mesh.py` & `navis-1.5.0/navis/core/mesh.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/core/neuronlist.py` & `navis-1.5.0/navis/core/neuronlist.py`

 * *Files 6% similar despite different names*

```diff
@@ -105,21 +105,24 @@
         if isinstance(x, NeuronList):
             # We can't simply say self.neurons = x.neurons b/c that way
             # changes in the list would backpropagate
             self.neurons = [n for n in x.neurons]
         elif utils.is_iterable(x):
             # If x is a list of mixed objects we need to unpack/flatten that
             # E.g. x = [NeuronList, NeuronList, core.TreeNeuron]
-            to_unpack = [e for e in x if isinstance(e, NeuronList)]
-            x = [e for e in x if not isinstance(e, NeuronList)]
-            x += [n for ob in to_unpack for n in ob.neurons]
-
-            # We have to convert from numpy ndarray to list
-            # Do NOT remove list() here!
-            self.neurons = list(x)  # type: ignore
+            # We need to make sure the order is retained though (important for
+            # e.g. plotting)
+            self.neurons = []
+            for n in x:
+                # Unpack neuronlists
+                if isinstance(n, NeuronList):
+                    self.neurons += n.neurons
+                # Everything else is just appended - will throw error later
+                else:
+                    self.neurons.append(n)
         elif isinstance(x, type(None)):
             # Empty Neuronlist
             self.neurons = []
         else:
             # Any other datatype will simply be assumed to be accepted by
             # core.Neuron() - if not this will throw an error
             self.neurons = [x]  # type: ignore
@@ -377,17 +380,19 @@
             self.__dict__.clear()
             for k, v in value.items():
                 self.__dict__[k] = v
             return
 
         # Check if this attribute exists in the neurons
         if any([hasattr(n, key) for n in self.neurons]):
-            logger.warning('It looks like you are trying to add a Neuron '
-                           f'attribute to a NeuronList. "{key}" will not '
-                           'propagated to the neurons it contains!')
+            logger.warning('It looks like you are trying to add a neuron '
+                           'attribute to a NeuronList. Setting the attribute '
+                           f'"{key}" on the NeuronList will not propagated to '
+                           'the neurons it contains! To set neuron attributes '
+                           'use the `NeuronList.set_neuron_attributes()` method.')
 
         self.__dict__[key] = value
 
     def __getstate__(self):
         """Get state (used e.g. for pickling)."""
         # We have to implement this to make sure that we don't accidentally
         # call __getstate__ of each neuron via the NeuronProcessor
@@ -410,16 +415,16 @@
         return self.copy(deepcopy=True)
 
     def __getitem__(self, key):
         if utils.is_iterable(key):
             if all([isinstance(k, (bool, np.bool_)) for k in key]):
                 if len(key) != len(self.neurons):
                     raise IndexError('boolean index did not match indexed '
-                                     f'NeuronList; dimension is {len(self.neurons)}'
-                                     ' but corresponding boolean dimension is'
+                                     f'NeuronList; dimension is {len(self.neurons)} '
+                                     'but corresponding boolean dimension is '
                                      f'{len(key)}')
                 subset = [n for i, n in enumerate(self.neurons) if key[i]]
             else:
                 subset = [self[i] for i in key]
         elif isinstance(key, str):
             subset = [n for n in self.neurons if re.fullmatch(key, getattr(n, 'name', ''))]
 
@@ -761,14 +766,88 @@
                                                        disable=not progress)],
                             columns=props)
 
     def itertuples(self):
         """Helper to mimic ``pandas.DataFrame.itertuples()``."""
         return self.neurons
 
+    def set_neuron_attributes(self, x, name, register=False, na='raise'):
+        """Set attributes of neurons contained in the NeuronList.
+
+        Parameters
+        ----------
+        x :         any | list | np.ndarray | dict | function
+                    Value of the property:
+                      - lists and arrays are expected to contain a value for
+                        each neuron and hence have to match the length of the
+                        NeuronList
+                      - dict is expected to map ``{neuron.id: value}``
+                      - a function is expected to take ``neuron.id`` as input
+                        and return a value
+        name :      str
+                    Name of the property to set.
+        register :  bool
+                    If True, will also register the attribute(s) as properties
+                    that should show up in the summary.
+        na :        'raise' | 'propagate' | 'skip'
+                    What to do if `x` is a dictionary and does not contain a
+                    value for a neuron:
+                     - 'raise' will raise a KeyError
+                     - 'propagate' will set the attribute to `None`
+                     - 'skip' will not set the attribute
+
+        Examples
+        --------
+        >>> import navis
+        >>> nl = navis.example_neurons(5)
+        >>> # Set a single value
+        >>> nl.set_neuron_attributes('some_value', name='my_attr')
+        >>> nl[0].my_attr
+        'some_value'
+        >>> # Set individual values as iterable
+        >>> nl.set_neuron_attributes([1, 2, 3, 4, 5], name='my_attr')
+        >>> nl[0].my_attr
+        1
+        >>> nl.my_attr
+        array([1, 2, 3, 4, 5])
+        >>> # Set individual values using a dictionary
+        >>> val_dict = dict(zip(nl.id, ['test', 2, 2.2, 4, 'test2']))
+        >>> nl.set_neuron_attributes(val_dict, name='my_attr')
+        >>> nl[0].my_attr
+        'test'
+
+        """
+        utils.eval_param(na, name='na',
+                         allowed_values=('raise', 'propagate', 'skip'))
+        utils.eval_param(name, name='name', allowed_types=(str, ))
+
+        if isinstance(x, dict):
+            if na == 'raise':
+                miss = ~np.isin(self.id, list(x))
+                if any(miss):
+                    raise KeyError('Dictionary `x` is missing entries for IDs: '
+                                   f'{self.id[miss]}')
+            for n in self.neurons:
+                v = x.get(n.id, None)
+                if (v is None) and (na == 'skip'):
+                    continue
+                n._register_attr(name, v, summary=register)
+        elif isinstance(x, (list, np.ndarray)):
+            if len(x) != len(self):
+                raise ValueError(f'Got {len(x)} values for the{len(self)} '
+                                 'neurons in the NeuronList.')
+            for n, v in zip(self.neurons, x):
+                n._register_attr(name, v, summary=register)
+        elif callable(x):
+            for n in self.neurons:
+                n._register_attr(name, x(n.id), summary=register)
+        else:
+            for n in self.neurons:
+                n._register_attr(name, x, summary=register)
+
     def sort_values(self, key: str, ascending: bool = False):
         """Sort neurons by given key.
 
         Needs to be an attribute of all neurons: for example ``name``.
         Also works with custom attributes.
         """
         self.neurons = sorted(self.neurons,
@@ -802,24 +881,27 @@
 
     def tail(self, N: int = 5) -> pd.DataFrame:
         """Return summary for bottom N neurons."""
         return self.summary(N=slice(-N, len(self)))
 
     def remove_duplicates(self,
                           key: str = 'name',
+                          keep: str = 'first',
                           inplace: bool = False
                           ) -> Optional['NeuronList']:
         """Remove duplicate neurons from list.
 
         Parameters
         ----------
         key :       str | list, optional
                     Attribute(s) by which to identify duplicates. In case of
                     multiple, all attributes must match to flag a neuron as
                     duplicate.
+        keep :      str
+                    Which of the duplicated neurons to keep.
         inplace :   bool, optional
                     If False will return a copy of the original with
                     duplicates removed.
 
         """
         if inplace:
             x = self
@@ -829,18 +911,18 @@
         key = utils.make_iterable(key)
 
         # Generate pandas DataFrame
         df = pd.DataFrame([[getattr(n, at) for at in key] for n in x],
                           columns=key)
 
         # Find out which neurons to keep
-        keep = ~df.duplicated(keep='first').values
+        to_keep = ~df.duplicated(keep=keep).values
 
         # Reassign neurons
-        x.neurons = x[keep].neurons
+        x.neurons = x[to_keep].neurons
 
         if not inplace:
             return x
         return None
 
     def unmix(self):
         """Split into NeuronLists of the same neuron type.
```

### Comparing `navis-1.4.0/navis/core/neurons.py` & `navis-1.5.0/navis/core/neurons.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/core/skeleton.py` & `navis-1.5.0/navis/core/skeleton.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/core/volumes.py` & `navis-1.5.0/navis/core/volumes.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/core/voxel.py` & `navis-1.5.0/navis/core/voxel.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/data/__init__.py` & `navis-1.5.0/navis/data/__init__.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/data/gml/1734350788.gml` & `navis-1.5.0/navis/data/gml/1734350788.gml`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/data/gml/1734350908.gml` & `navis-1.5.0/navis/data/gml/1734350908.gml`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/data/gml/722817260.gml` & `navis-1.5.0/navis/data/gml/722817260.gml`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/data/gml/754534424.gml` & `navis-1.5.0/navis/data/gml/754534424.gml`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/data/gml/754538881.gml` & `navis-1.5.0/navis/data/gml/754538881.gml`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/data/load_data.py` & `navis-1.5.0/navis/data/load_data.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/data/obj/1734350788.obj` & `navis-1.5.0/navis/data/obj/1734350788.obj`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/data/obj/1734350908.obj` & `navis-1.5.0/navis/data/obj/1734350908.obj`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/data/obj/722817260.obj` & `navis-1.5.0/navis/data/obj/722817260.obj`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/data/obj/754534424.obj` & `navis-1.5.0/navis/data/obj/754534424.obj`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/data/obj/754538881.obj` & `navis-1.5.0/navis/data/obj/754538881.obj`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/data/readme.md` & `navis-1.5.0/navis/data/readme.md`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/data/swc/1734350788.swc` & `navis-1.5.0/navis/data/swc/1734350788.swc`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/data/swc/1734350908.swc` & `navis-1.5.0/navis/data/swc/1734350908.swc`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/data/swc/722817260.swc` & `navis-1.5.0/navis/data/swc/722817260.swc`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/data/swc/754534424.swc` & `navis-1.5.0/navis/data/swc/754534424.swc`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/data/swc/754538881.swc` & `navis-1.5.0/navis/data/swc/754538881.swc`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/data/synapses/1734350788.csv` & `navis-1.5.0/navis/data/synapses/1734350788.csv`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/data/synapses/1734350908.csv` & `navis-1.5.0/navis/data/synapses/1734350908.csv`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/data/synapses/722817260.csv` & `navis-1.5.0/navis/data/synapses/722817260.csv`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/data/synapses/754534424.csv` & `navis-1.5.0/navis/data/synapses/754534424.csv`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/data/synapses/754538881.csv` & `navis-1.5.0/navis/data/synapses/754538881.csv`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/data/volumes/lh.obj` & `navis-1.5.0/navis/data/volumes/lh.obj`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/data/volumes/neuropil.obj` & `navis-1.5.0/navis/data/volumes/neuropil.obj`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/graph/__init__.py` & `navis-1.5.0/navis/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/graph/clinic.py` & `navis-1.5.0/navis/graph/clinic.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/graph/converters.py` & `navis-1.5.0/navis/graph/converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -444,15 +444,15 @@
               root: Optional[Union[int, str]] = None,
               break_cycles: bool = False,
               **kwargs
               ) -> pd.DataFrame:
     """Generate node table from NetworkX Graph.
 
     This function will try to generate a neuron-like tree structure from
-    the Graph. Therefore the graph may not contain loops!
+    the Graph. Therefore the graph must not contain loops!
 
     Node attributes (e.g. ``x``, ``y``, ``z``, ``radius``) need
     to be properties of the graph's nodes. All node property will be added to
     the neuron's ``.nodes`` table.
 
     Parameters
     ----------
@@ -471,15 +471,15 @@
     Returns
     -------
     TreeNeuron
 
     """
     # First some sanity checks
     if not isinstance(g, nx.Graph):
-        raise TypeError(f'`g` must be NetworkX Graph, not "{type(g)}"')
+        raise TypeError(f'`g` must be NetworkX Graph, got "{type(g)}"')
 
     # We need an undirected Graph
     if isinstance(g, nx.DiGraph):
         g = g.to_undirected(as_view=True)
 
     if not nx.is_forest(g):
         if not break_cycles:
```

### Comparing `navis-1.4.0/navis/graph/graph_utils.py` & `navis-1.5.0/navis/graph/graph_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -658,16 +658,20 @@
             nodeList = np.arange(len(x.igraph.vs))
 
         # Matrix is ordered by vertex number
         m = _igraph_to_sparse(x.igraph, weight_attr=weight)
     else:
         nodeList = np.array(x.graph.nodes())
 
-        m = nx.to_scipy_sparse_matrix(x.graph, nodeList,
-                                      weight=weight)
+        if hasattr(nx, 'to_scipy_sparse_matrix'):
+            m = nx.to_scipy_sparse_matrix(x.graph, nodeList,
+                                          weight=weight)
+        else:
+            m = nx.to_scipy_sparse_array(x.graph, nodeList,
+                                         weight=weight)
 
     if not isinstance(from_, type(None)):
         from_ = np.unique(utils.make_iterable(from_))
 
         miss = from_[~np.isin(from_, nodeList)].astype(str)
         if any(miss):
             raise ValueError(f'Node/vertex IDs not present: {", ".join(miss)}')
@@ -1035,14 +1039,15 @@
 
 @utils.map_neuronlist(desc='Pruning', allow_parallel=True)
 @utils.meshneuron_skeleton(method='subset')
 def longest_neurite(x: 'core.NeuronObject',
                     n: int = 1,
                     reroot_soma: bool = False,
                     from_root: bool = True,
+                    inverse: bool = False,
                     inplace: bool = False) -> 'core.NeuronObject':
     """Return a neuron consisting of only the longest neurite(s).
 
     Based on geodesic distances.
 
     Parameters
     ----------
@@ -1055,14 +1060,16 @@
                          - ``n=slice(1, None)`` removes the longest neurite
     reroot_soma :       bool
                         If True, neuron will be rerooted to soma.
     from_root :         bool
                         If True, will look for longest neurite from root.
                         If False, will look for the longest neurite between any
                         two tips.
+    inverse :           bool
+                        If True, will instead *remove* the longest neurite.
     inplace :           bool
                         If False, copy of the neuron will be trimmed down to
                         longest neurite and returned.
 
     Returns
     -------
     TreeNeuron/List
@@ -1116,15 +1123,19 @@
     if isinstance(n, (int, np.integer)):
         tn_to_preserve: List[int] = [tn for s in segments[:n] for tn in s]
     elif isinstance(n, slice):
         tn_to_preserve = [tn for s in segments[n] for tn in s]
     else:
         raise TypeError(f'Unable to use N of type "{type(n)}"')
 
-    _ = morpho.subset_neuron(x, tn_to_preserve, inplace=True)
+    if not inverse:
+        _ = morpho.subset_neuron(x, tn_to_preserve, inplace=True)
+    else:
+        _ = morpho.subset_neuron(x, ~np.isin(x.nodes.node_id.values, tn_to_preserve),
+                                 inplace=True)
 
     return x
 
 
 @utils.lock_neuron
 def reroot_skeleton(x: 'core.NeuronObject',
                     new_root: Union[int, str],
@@ -2019,15 +2030,15 @@
 
     Parameters
     ----------
     x :         TreeNeuron
                 Neuron to be rewired.
     g :         networkx.Graph
                 Graph to use for rewiring. Please note that directionality (if
-                present) is note taken into account. Nodes not included in the
+                present) is not taken into account. Nodes not included in the
                 graph will be disconnected (i.e. won't have a parent). Nodes
                 in the graph but not in the table are ignored!
     root :      int
                 Node ID for the new root. If not given, will try to use the
                 current root.
     inplace :   bool
                 If True, will rewire the neuron inplace. If False, will return
```

### Comparing `navis-1.4.0/navis/interfaces/allen_celltypes.py` & `navis-1.5.0/navis/interfaces/allen_celltypes.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/interfaces/blender.py` & `navis-1.5.0/navis/interfaces/blender.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/interfaces/cytoscape.py` & `navis-1.5.0/navis/interfaces/cytoscape.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/interfaces/insectbrain_db.py` & `navis-1.5.0/navis/interfaces/insectbrain_db.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/interfaces/microns.py` & `navis-1.5.0/navis/interfaces/microns.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,15 +287,16 @@
     ----------
     x :             int
                     A single root ID.
     mip :           int
                     Scale at which to fetch voxels.
     bounds :        list, optional
                     Bounding box [xmin, xmax, ymin, ymax, zmin, zmax] in voxel
-                    space.
+                    space. For example, the voxel resolution for mip 0
+                    segmentation is 8 x 8 x 40 nm.
     datastack :     "cortex65" | "cortex35" | "layer 2/3"
                     Which dataset to use. Internally these are mapped to the
                     corresponding sources (e.g. "minnie65_public_v117" for
                     "cortex65").
 
     Returns
     -------
```

### Comparing `navis-1.4.0/navis/interfaces/neuprint.py` & `navis-1.5.0/navis/interfaces/neuprint.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,15 +258,18 @@
 
         # Meshes come out in units (e.g. nanometers) but most other data (synapses,
         # skeletons, etc) come out in voxels, we will therefore scale meshes to voxels
         n.vertices /= np.array(client.meta['voxelSize']).reshape(1, 3)
         n.units=f'{client.meta["voxelSize"][0]} {client.meta["voxelUnits"]}'
 
         if n.somaLocation:
-            n.soma_radius = radii[n.id] / n.units.to('nm').magnitude
+            if radii[n.id]:
+                n.soma_radius = radii[n.id] / n.units.to('nm').magnitude
+            else:
+                n.soma_radius = None
             n.soma = n.somaLocation
 
     if with_synapses:
         # Fetch synapses
         syn = fetch_synapses(meta.bodyId.values,
                              synapse_criteria=SynapseCriteria(primary_only=True),
                              client=client)
@@ -420,14 +423,15 @@
     try:
         data = client.fetch_skeleton(r.bodyId, format='pandas', heal=heal)
     except HTTPError as err:
         if err.response.status_code == 400:
             if missing_swc in ['warn', 'skip']:
                 if missing_swc == 'warn':
                     logger.warning(f'No SWC found for {r.bodyId}')
+                    return
             else:
                 raise
         else:
             raise
 
     # Generate neuron
     # Note that we are currently assuming that the x/y/z data is isotropic
```

### Comparing `navis-1.4.0/navis/interfaces/neuromorpho.py` & `navis-1.5.0/navis/interfaces/neuromorpho.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/interfaces/neuron/comp.py` & `navis-1.5.0/navis/interfaces/neuron/comp.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/interfaces/neuron/network.py` & `navis-1.5.0/navis/interfaces/neuron/network.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,19 +43,32 @@
 __all__ = []
 
 # It looks like there can only ever be one reference to the time
 # If we have multiple models, we will each reference them to this variable
 main_t = None
 
 Stimulus = namedtuple('Stimulus', ['start', 'stop', 'frequency', 'randomness',
-                                   'neurons', 'netstim', 'netcon'])
+                                   'neurons', 'netstim', 'netcon', 'label'])
 
 
+"""
+Note to self: it would best best if PointNetwork would not actually
+build the model until it's executed. That way we can run the entire
+simulation in a separate thread (or multiple cores).
+"""
+
 class PointNetwork:
-    """A Network in which all neurons are represented as LIF point processes."""
+    """A Network of Leaky-Integrate-and-Fire (LIF) point processes.
+
+    Examples
+    --------
+    >>> import navis.interfaces.neuron as nrn
+    >>> N = nrn.PointNetwork()
+    >>>
+    """
 
     def __init__(self):
         self._neurons = []
         self._neurons_dict = {}
         self._edges = []
         self._stimuli = []
         self._ids = []
@@ -126,15 +139,18 @@
         model :         "IntFire1" | "IntFire2" | "IntFire4"
                         The model to use for the integrate-and-fire point processes.
         source_col :    str
                         Name of the column with the source IDs.
         target_col :    str
                         Name of the column with the target IDs.
         weight_col :    str
-                        Name of the column with the weights.
+                        Name of the column with the weights. The important thing
+                        to note here is that weight is expected to be in the 0-1
+                        range with 1 effectively guaranteeing that a presynaptic
+                        spike triggers a postsynaptic spike.
         **props
                         Keyword arguments are passed through to ``add_neurons``.
                         Use to set e.g. labels, threshold or additional
                         model parameters.
 
         """
         assert isinstance(edges, pd.DataFrame)
@@ -227,15 +243,15 @@
 
         """
         self.add_stimulus(ids=ids, start=0, stop=9999999999,
                           frequency=frequency, randomness=randomness,
                           independent=independent)
 
     def add_stimulus(self, ids, start, frequency, stop=None, duration=None,
-                     randomness=.5, independent=True, weight=1):
+                     randomness=.5, independent=True, label=None, weight=1):
         """Add stimulus to given neurons.
 
         Important
         ---------
         Stimuli are implemented via a NetStim object which provides the
         specified stimulation (i.e. start, stop, frequency). This NetStim is
         then connected to the neuron(s) via a NetCon. The response of the
@@ -260,14 +276,16 @@
                         Frequency [Hz] of background noise . If iterable must
                         match length of `ids`. Values <= 0 are silently skipped.
         randomness :    float [0-1]
                         Randomness of spike timings.
         independent :   bool
                         If True (default), each neuron will get its own
                         independent stimulus.
+        label :         str, optional
+                        A label to identify the stimulus.
         weight :        float
                         Weight for the connection between the stimulator and
                         the neuron. This really should be 1 to make sure each
                         spike in the stimulus elicits a spike in the target.
 
         """
         ids = utils.make_iterable(ids)
@@ -314,31 +332,47 @@
                 ns.number = int(duration / 1000 * f)
                 ns.start = start
 
             nc = neuron.h.NetCon(ns, proc)
             nc.weight[0] = weight
             nc.delay = 0
 
-            self._stimuli.append(Stimulus(start, stop, f, randomness, i, ns, nc))
+            self._stimuli.append(Stimulus(start, stop, f, randomness, i, ns, nc, label))
 
     def connect(self, source, target, weight, delay=5):
-        """Connect two neurons."""
+        """Connect two neurons.
+
+        Parameters
+        ----------
+        source :    int | str
+                    ID of the source.
+        target :    int | str
+                    ID of the target
+        weight :    float
+                    Weight of the edge. The important thing to note here is that
+                    the weight is expected to be in the 0-1 range with 1
+                    effectively guaranteeing that a presynaptic spike triggers
+                    a postsynaptic spike.
+        delay :     int
+                    Delay in ms between a pre- and a postsynaptic spike.
+
+        """
         # Get the point processes corresponding to source and target
         pre = self.idx[source]
         post = self.idx[target]
 
         # Connect
         nc = neuron.h.NetCon(pre.process, post.process)
         nc.weight[0] = weight
         nc.delay = delay
 
         # Keep track
         self._edges.append([source, target, weight, nc])
 
-    def plot_raster(self, subset=None, group=False, ax=None, label=False,
+    def plot_raster(self, subset=None, group=False, stimuli=True, ax=None, label=False,
                     backend='auto', **kwargs):
         """Raster plot of spike timings.
 
         Parameters
         ----------
         subset :        list-like
                         Subset of IDs to plot. You can also use this to
@@ -388,15 +422,19 @@
                 backend = 'plotly'
             else:
                 backend = 'matplotlib'
 
         if backend == 'plotly':
             return _plot_raster_plotly(x, y, ids, fig=ax, labels=labels, **kwargs)
         elif backend == 'matplotlib':
-            return _plot_raster_mpl(x, y, ids, ax=ax, labels=labels, **kwargs)
+            ax = _plot_raster_mpl(x, y, ids, ax=ax, labels=labels,
+                                  stimuli=self._stimuli if stimuli else None,
+                                  **kwargs)
+            ax.set_xlim(0, neuron.h.t)
+            return ax
         else:
             raise ValueError(f'Unknown backend "{backend}"')
 
     def plot_traces(self, bin_size=100, subset=None, rolling_window=None,
                     group=False, stimuli=True, ax=None, backend='auto', **kwargs):
         """Plot mean firing rate.
 
@@ -434,41 +472,41 @@
         # Collect spike frequencies
         spks = self.get_spike_counts(bin_size=bin_size, subset=subset,
                                      rolling_window=rolling_window)
         freq = spks * 1000 / bin_size
 
         if self.labels:
             ld = dict(zip(self._ids, self._labels))
-            labels = [ld[i] for i in ids]
+            labels = [f'{i} ({ld[i]})' for i in ids]
         else:
             labels = None
 
         if backend == 'auto':
             if utils.is_jupyter():
                 backend = 'plotly'
             else:
                 backend = 'matplotlib'
 
         if isinstance(group, bool) and group:
-            std = freq.groupby(dict(zip(self._ids, self._labels))).sem()
+            sem = freq.groupby(dict(zip(self._ids, self._labels))).sem()
             freq = freq.groupby(dict(zip(self._ids, self._labels))).mean()
             labels = freq.index.values.tolist()
         elif not isinstance(group, bool):
-            std = freq.groupby(group).sem()
+            sem = freq.groupby(group).sem()
             freq = freq.groupby(group).mean()
             labels = freq.index.values.tolist()
         else:
-            std = None
+            sem = None
 
         if backend == 'plotly':
             return _plot_traces_plotly(freq, fig=ax, labels=labels,
                                        stimuli=self._stimuli if stimuli else None,
-                                       std=std, **kwargs)
+                                       env=sem, **kwargs)
         elif backend == 'matplotlib':
-            return _plot_traces_mpl(freq, ax=ax, std=std,
+            return _plot_traces_mpl(freq, ax=ax, env=sem,
                                     stimuli=self._stimuli if stimuli else None,
                                     **kwargs)
         else:
             raise ValueError(f'Unknown backend "{backend}"')
 
     def set_labels(self, labels):
         """Set labels for neurons.
@@ -493,24 +531,28 @@
     def run_simulation(self, duration=25 * ms, v_init=-65 * mV):
         """Run the simulation."""
 
         # This resets the entire model space not just this neuron!
         neuron.h.finitialize(v_init)
         neuron.h.continuerun(duration)
 
-    def get_spike_counts(self, bin_size=50, subset=None, rolling_window=None):
+    def get_spike_counts(self, bin_size=50, subset=None, rolling_window=None,
+                         group=False):
         """Get matrix of spike counts.
 
         Parameters
         ----------
         bin_size :          int | None
                             Size [ms] of the bins over which to count spikes.
                             If None, will simply return total counts.
         rolling_window :    int, optional
                             Average spike counts in a rolling window.
+        group :             bool
+                            If True, will return the spike counts per unique
+                            label.
 
         Returns
         -------
         pd.DataFrame
 
         """
         if not isinstance(subset, type(None)):
@@ -532,15 +574,20 @@
         for i, id in enumerate(ids):
             pp = self.idx[id]
             timings = list(pp.spk_timings)
             if timings:
                 hist, _ = np.histogram(timings, bins)
                 counts[i, :] = hist
 
-        counts = pd.DataFrame(counts, index=ids, columns=bins[:-1])
+        counts = pd.DataFrame(counts, index=ids, columns=bins[1:])
+
+        if group:
+            if not self._labels:
+                raise ValueError('Unable to group: Network has no labels.')
+            counts = counts.groupby(counts.index.map(dict(zip(self.ids, self._labels)))).sum()
 
         if rolling_window:
             avg = sliding_window_view(counts, rolling_window, axis=1).mean(axis=2)
             counts.iloc[:, :-(rolling_window - 1)] = avg
 
         return counts
 
@@ -581,15 +628,15 @@
         neurons = self.network._neurons_dict
         if utils.is_iterable(id):
             return [neurons[i] for i in id]
         else:
             return neurons[id]
 
 
-def _plot_raster_mpl(x, y, ids, ax=None, labels=None, **kwargs):
+def _plot_raster_mpl(x, y, ids, ax=None, labels=None, stimuli=None, **kwargs):
     if not ax:
         fig, ax = plt.subplots(figsize=kwargs.pop('figsize', (12, min(20, len(ids)))))
 
     DEFAULTS = dict(alpha=.9, rasterized=False, lw=1)
     DEFAULTS.update(kwargs)
 
     ax.plot(x, y, **DEFAULTS)
@@ -599,18 +646,30 @@
     if not isinstance(labels, type(None)):
         ax.set_yticks(np.arange(0, len(ids), 1) + .5)
         ax.set_yticklabels(labels)
     else:
         ax.set_yticks([])
         ax.set_yticklabels([])
 
+    if stimuli:
+        y = len(ids) + max(1, len(ids) / 100)
+        stimuli = np.unique([(s.start, s.stop) for s in stimuli], axis=0)
+        for st in stimuli:
+            # Skip background noise
+            if st[1] >= 999_999_999:
+                continue
+            ax.plot([st[0], st[1]], [y, y], lw=4,
+                    color=kwargs.get('color', (.5, .5, .5)))
+
+        ax.set_ylim(top=y + 1)
+
     return ax
 
 
-def _plot_traces_mpl(freq, ax=None, show=True, std=None, stimuli=None, **kwargs):
+def _plot_traces_mpl(freq, ax=None, show=True, env=None, stimuli=None, **kwargs):
     if not ax:
         fig, ax = plt.subplots(figsize=kwargs.pop('figsize', (12, 7)))
 
     if 'color' in kwargs:
         c = kwargs.pop('color')
         if utils.is_iterable(c) and len(c) == freq.shape[0]:
             colors = np.array([mcl.to_rgb(c) for c in c])
@@ -630,23 +689,23 @@
 
     DEFAULTS = dict(alpha=.9, rasterized=False, lw=1)
     DEFAULTS.update(kwargs)
 
     lc = LineCollection(segs, **DEFAULTS, colors=colors)
     ax.add_collection(lc)
 
-    if not isinstance(std, type(None)):
-        for i, s in enumerate(std.index.values):
-            # If no std (single neuron)
-            if not std.loc[s].any():
+    if not isinstance(env, type(None)):
+        for i, s in enumerate(env.index.values):
+            # If no envelope (single neuron)
+            if not env.loc[s].any():
                 continue
 
-            y1 = freq.loc[s].values + std.loc[s].values
-            y2 = freq.loc[s].values - std.loc[s].values
-            ax.fill_between(std.columns.values, y1, y2,
+            y1 = freq.loc[s].values + env.loc[s].values
+            y2 = freq.loc[s].values - env.loc[s].values
+            ax.fill_between(env.columns.values, y1, y2,
                             facecolor=colors[i],
                             alpha=0.5)
 
     if stimuli:
         y = freq.max().max() + 20
         stimuli = np.unique([(s.start, s.stop) for s in stimuli], axis=0)
         for st in stimuli:
@@ -691,15 +750,15 @@
     if show:
         fig.show()
 
     return fig
 
 
 def _plot_traces_plotly(freq, fig=None, labels=None, show=True, stimuli=None,
-                        std=None, **kwargs):
+                        env=None, **kwargs):
     if not fig:
         fig = go.Figure()
 
     if 'color' in kwargs:
         c = kwargs['color']
         if utils.is_iterable(c) and len(c) == freq.shape[0]:
             colors = np.array([mcl.to_rgb(c) for c in c])
@@ -730,39 +789,44 @@
                                    hovertext=labels[i] if labels else None,
                                    hoverinfo='text' if labels else 'x+y',
                                    name=labels[i] if labels else freq.index[i],
                                    legendgroup=labels[i] if labels else freq.index[i],
                                    line=dict(color=color_str,
                                              width=kwargs.get('width', 1.5))))
 
-        if not isinstance(std, type(None)):
-            y = (freq.iloc[i].values + std.iloc[i].values).tolist()
-            y += (freq.iloc[i].values - std.iloc[i].values).tolist()[::-1]
+        if not isinstance(env, type(None)):
+            y = (freq.iloc[i].values + env.iloc[i].values).tolist()
+            y += (freq.iloc[i].values - env.iloc[i].values).tolist()[::-1]
             fig.add_trace(go.Scattergl(x=x.tolist() + x.tolist()[::-1],
                                        y=y,
                                        fill='toself',
                                        fillcolor=fill_color_str,
                                        name=labels[i] if labels else freq.index[i],
                                        showlegend=False,
                                        hoverinfo='skip',
                                        legendgroup=labels[i] if labels else freq.index[i],
                                        line=dict(color="rgba(255,255,255,0)",
                                                  width=kwargs.get('width', 1.5))))
 
     if stimuli:
+        timings = [(st.start, st.stop) for st in stimuli]
+        to_plot = np.unique(timings, axis=0, return_index=True)[1]
         y = freq.max().max() + 20
-        stimuli = np.unique([(s.start, s.stop) for s in stimuli], axis=0)
-        for i, st in enumerate(stimuli):
+        for i, ix in enumerate(to_plot):
+            st = stimuli[ix]
             # Skip background noise
-            if st[1] >= 999_999_999:
+            if st.stop >= 999_999_999:
                 continue
-            fig.add_trace(go.Scattergl(x=[st[0], st[1]], y=[y, y],
+            fig.add_trace(go.Scattergl(x=[st.start, st.stop], y=[y+i, y+i],
                                        mode='lines',
                                        line=dict(color='rgb(155,155,155)',
                                                  width=4),
+                                       name=st.label,
+                                       hovertext=st.label,
+                                       hoverinfo='text',
                                        showlegend=False))
 
     fig.update_layout(paper_bgcolor='rgba(0,0,0,0)',
                       height=kwargs.get('height', 500),
                       xaxis_title="time [ms]",
                       yaxis_title="spike rate [Hz]",
                       yaxis_gridwidth=.25,
```

### Comparing `navis-1.4.0/navis/interfaces/neuron/utils.py` & `navis-1.5.0/navis/interfaces/neuron/utils.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/interfaces/r.py` & `navis-1.5.0/navis/interfaces/r.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/interfaces/vfb.py` & `navis-1.5.0/navis/interfaces/vfb.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/intersection/__init__.py` & `navis-1.5.0/navis/intersection/__init__.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/intersection/convex.py` & `navis-1.5.0/navis/intersection/convex.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/intersection/intersect.py` & `navis-1.5.0/navis/intersection/intersect.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/intersection/ray.py` & `navis-1.5.0/navis/intersection/ray.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/io/__init__.py` & `navis-1.5.0/navis/io/__init__.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/io/base.py` & `navis-1.5.0/navis/io/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -589,15 +589,15 @@
         obj :               sequence
                             Sequence of anything readable by read_any_single or
                             directory path(s).
         include_subdirs :   bool
                             Whether to include subdirectories of a given
                             directory.
         parallel :          str | bool | int | None
-                            "auto" or True for n_cores - 2, otherwise int for
+                            "auto" or True for n_cores // 2, otherwise int for
                             number of jobs, or False for serial.
         attrs :             dict or None
                             Arbitrary attributes to include in each TreeNeuron
                             of the NeuronList.
 
         Returns
         -------
@@ -824,15 +824,15 @@
                     are interpreted as looking for filenames without extension.
                     To include all files use `'*'`. Can also be callable that
                     accepts a filename and returns True or False depending on
                     if it should be included.
     limit :         int, optional
                     Limit the number of files read from this directory.
     parallel :      str | bool | int
-                    "auto" or True for n_cores - 2, otherwise int for number of
+                    "auto" or True for n_cores // 2, otherwise int for number of
                     jobs, or false for serial.
     ignore_hidden : bool
                     Archives zipped on OSX can end up containing a
                     `__MACOSX` folder with files that mirror the name of other
                     files. For example if there is a `123456.swc` in the archive
                     you might also find a `__MACOSX/._123456.swc`. Reading the
                     latter will result in an error. If ignore_hidden=True
@@ -878,15 +878,15 @@
         and len(to_read) < 200
     ):
         parallel = False
 
     if parallel:
         # Do not swap this as ``isinstance(True, int)`` returns ``True``
         if isinstance(parallel, (bool, str)):
-            n_cores = max(1, os.cpu_count() - 2)
+            n_cores = max(1, os.cpu_count() // 2)
         else:
             n_cores = int(parallel)
 
         with mp.Pool(processes=n_cores) as pool:
             results = pool.imap(read_fn, to_read)
             neurons = list(prog(results))
     else:
```

### Comparing `navis-1.4.0/navis/io/hdf_io.py` & `navis-1.5.0/navis/io/hdf_io.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/io/json_io.py` & `navis-1.5.0/navis/io/json_io.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/io/mesh_io.py` & `navis-1.5.0/navis/io/mesh_io.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/io/nmx_io.py` & `navis-1.5.0/navis/io/nmx_io.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/io/nrrd_io.py` & `navis-1.5.0/navis/io/nrrd_io.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/io/precomputed_io.py` & `navis-1.5.0/navis/io/precomputed_io.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/io/rda_io.py` & `navis-1.5.0/navis/io/rda_io.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/io/swc_io.py` & `navis-1.5.0/navis/io/swc_io.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/io/tiff_io.py` & `navis-1.5.0/navis/io/tiff_io.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/matching/__init__.py` & `navis-1.5.0/navis/matching/__init__.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/matching/bipartite.py` & `navis-1.5.0/navis/matching/bipartite.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/matching/pipeline.py` & `navis-1.5.0/navis/matching/pipeline.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/meshes/__init__.py` & `navis-1.5.0/navis/meshes/__init__.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/meshes/b3d.py` & `navis-1.5.0/navis/meshes/b3d.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/meshes/fqmr.py` & `navis-1.5.0/navis/meshes/fqmr.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/meshes/mesh_utils.py` & `navis-1.5.0/navis/meshes/mesh_utils.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/meshes/o3d.py` & `navis-1.5.0/navis/meshes/o3d.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/meshes/operations.py` & `navis-1.5.0/navis/meshes/operations.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/meshes/pyml.py` & `navis-1.5.0/navis/meshes/pyml.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/meshes/templates/blender_decimate.py.template` & `navis-1.5.0/navis/meshes/templates/blender_decimate.py.template`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/meshes/templates/blender_smooth.py.template` & `navis-1.5.0/navis/meshes/templates/blender_smooth.py.template`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/models/__init__.py` & `navis-1.5.0/navis/models/__init__.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/models/network_models.py` & `navis-1.5.0/navis/models/network_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -411,51 +411,58 @@
     def make_summary(self) -> pd.DataFrame:
         """Generate summary."""
         if not self.has_results:
             logger.error('Must run simulation first.')
 
         cmfs = np.stack(self.results.cmf)
         layer_min = (cmfs != 0).argmax(axis=1)
+        valid = np.any(cmfs != 0, axis=1)
         layer_max = (cmfs == 1.).argmax(axis=1)
-        layer_median = (cmfs >= .5).argmax(axis=1)
+        layer_max[~np.any(cmfs == 1., axis=1)] = cmfs.shape[1]
+        layer_median = (cmfs >= .5).argmax(axis=1).astype(float)
         pmfs = np.diff(cmfs, axis=1, prepend=0.)
         layer_pmfs = pmfs * np.arange(pmfs.shape[1])
         layer_mean = np.sum(layer_pmfs, axis=1)
 
         summary = pd.DataFrame({
                 'layer_min': layer_min + 1,
                 'layer_max': layer_max + 1,
                 'layer_mean': layer_mean + 1,
                 'layer_median': layer_median + 1,
             }, index=self.results.node)
 
+        # Discard nodes that are never activated
+        summary = summary[valid]
+
         self._summary = summary
         return self._summary
 
     def run(self, **kwargs) -> pd.DataFrame:
         """Run model (single process)."""
 
         # For some reason this is required for progress bars in Jupyter to show
         print(' ', end='', flush=True)
         # For faster access, use the raw array
         edges = self.edges[[self.source, self.target, self.weights]].values
+        id_type = self.edges[self.source].dtype
         # Transform weights to traversal probabilities
         edges[:, 2] = self.traversal_func(edges[:, 2])
 
         # Change node IDs into indices in [0, len(nodes))
         ids, edges_idx = np.unique(edges[:, :2], return_inverse=True)
+        ids = ids.astype(id_type)
         edges_idx = edges_idx.reshape((edges.shape[0], 2))
         edges_idx = np.concatenate(
             (edges_idx, np.expand_dims(edges[:, 2], axis=1)),
             axis=1)
 
         cmfs = np.zeros((len(ids), self.max_steps), dtype=np.float64)
         seed_idx = np.searchsorted(ids, self.seeds)
         cmfs[seed_idx, :] = 1.
-        changed = set(edges_idx[seed_idx, 1].astype(np.int64))
+        changed = set(edges_idx[np.isin(edges_idx[:, 0], seed_idx), 1].astype(id_type))
 
         with config.tqdm(
                 total=0,
                 disable=config.pbar_hide,
                 leave=config.pbar_leave,
                 position=kwargs.get('position', 0)) as pbar:
             while len(changed):
@@ -482,15 +489,15 @@
 
                     if np.allclose(cmf, new_cmf):
                         continue
 
                     cmfs[idx, :] = new_cmf
 
                     # Notify downstream nodes that they have changed next iteration.
-                    post_idx = edges_idx[edges_idx[:, 0] == idx, 1].astype(np.int64)
+                    post_idx = edges_idx[edges_idx[:, 0] == idx, 1].astype(id_type)
                     next_changed.extend(list(post_idx))
 
                 pbar.update(len(changed))
                 changed = set(next_changed)
 
         self.iterations = 1
         self.results = pd.DataFrame({'node': ids, 'cmf': list(cmfs)})
```

### Comparing `navis-1.4.0/navis/morpho/__init__.py` & `navis-1.5.0/navis/morpho/__init__.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/morpho/analyze.py` & `navis-1.5.0/navis/morpho/analyze.py`

 * *Files 7% similar despite different names*

```diff
@@ -79,10 +79,14 @@
                     is_large = soma_nodes.radius.values * soma_radius.units >= soma_radius
             else:
                 is_large = soma_nodes.radius >= soma_radius
 
             soma_nodes = soma_nodes[is_large]
 
     if not isinstance(soma_label, type(None)) and 'label' in soma_nodes.columns:
-        soma_nodes = soma_nodes[soma_nodes.label.astype(str) == str(soma_label)]
+        # Important: we need to use np.asarray here because the `label` column
+        # can be categorical in which case a `soma_nodes.label.astype(str)` might
+        # throw annoying runtime warnings
+        labels = np.asarray(soma_nodes.label).astype(str)
+        soma_nodes = soma_nodes[labels == str(soma_label)]
 
     return soma_nodes.node_id.values
```

### Comparing `navis-1.4.0/navis/morpho/fq.py` & `navis-1.5.0/navis/morpho/fq.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 #
 #    This program is distributed in the hope that it will be useful,
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 
 
-""" This module contains functions to analyse neuron's form factors.
-"""
+""" This module contains functions to analyse neuron's form factors."""
+
 import os
 import scipy
 
 import pandas as pd
 import multiprocessing as mp
 import numpy as np
```

### Comparing `navis-1.4.0/navis/morpho/manipulation.py` & `navis-1.5.0/navis/morpho/manipulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 @utils.meshneuron_skeleton(method='subset')
 def cell_body_fiber(x: NeuronObject,
                     method: Union[Literal['longest_neurite'],
                                   Literal['betweenness']] = 'betweenness',
                     reroot_soma: bool = True,
                     heal: bool = True,
                     threshold: float = 0.95,
+                    inverse: bool = False,
                     inplace: bool = False):
     """Prune neuron to its cell body fiber.
 
     Here, "cell body fiber" (CBF) refers to the tract connecting the soma to the
     backbone in unipolar neuron (common in e.g. insects). This function works
     best for typical neurons with clean skeletons.
 
@@ -73,14 +74,16 @@
                     rerooted to its soma.
     heal :          bool
                     If True (recommended), will heal fragmented neurons.
                     Fragmented neurons are not guaranteed to have correct CBFs.
     threshold :     float [0-1]
                     For method "betweenness" only: threshold at which to cut the
                     cell body fiber. Lower thresholds produce longer CBFs.
+    inverse :       bool
+                    If True, will instead *remove* the cell body fiber.
     inplace :       bool, optional
                     If False, pruning is performed on copy of original neuron
                     which is then returned.
 
     Returns
     -------
     TreeNeuron/List
@@ -136,15 +139,20 @@
             path = nx.shortest_path(x.graph, target=r, source=cut)
             break
         except nx.NetworkXNoPath:
             continue
         except BaseException:
             raise
 
-    _ = subset.subset_neuron(x, path, inplace=True)
+    if not inverse:
+        keep = path
+    else:
+        keep = x.nodes.node_id.values[~np.isin(x.nodes.node_id, path)]
+
+    _ = subset.subset_neuron(x, keep, inplace=True)
 
     return x
 
 
 @utils.map_neuronlist(desc='Pruning', allow_parallel=True)
 @utils.meshneuron_skeleton(method='subset')
 def prune_by_strahler(x: NeuronObject,
@@ -1399,15 +1407,15 @@
             C = this_C[['x', 'y', 'z']].values
 
             # Calculate euclidian distances A->B and A->C
             dist_AB = np.linalg.norm(A - B, axis=1)
             dist_AC = np.linalg.norm(A - C, axis=1)
 
             # Get the spikes
-            spikes_ix = np.where((dist_AB / dist_AC) > sigma)[0]
+            spikes_ix = np.where(np.divide(dist_AB, dist_AC, where=dist_AC != 0) > sigma)[0]
             spikes = this_B.iloc[spikes_ix]
 
             if not spikes.empty:
                 # Interpolate new position(s) between A and C
                 new_positions = A[spikes_ix] + (C[spikes_ix] - A[spikes_ix]) / 2
 
                 this_nodes.loc[spikes.index, ['x', 'y', 'z']] = new_positions
@@ -1745,15 +1753,15 @@
 @utils.map_neuronlist(desc='Healing', allow_parallel=True)
 def heal_skeleton(x: 'core.NeuronList',
                   method: Union[Literal['LEAFS'],
                                 Literal['ALL']] = 'ALL',
                   max_dist: Optional[float] = None,
                   min_size: Optional[float] = None,
                   drop_disc: float = False,
-                  use_radii: bool = False,
+                  mask: Optional[Sequence] = None,
                   inplace: bool = False) -> Optional[NeuronObject]:
     """Heal fragmented skeleton(s).
 
     Tries to heal a fragmented skeleton (i.e. a neuron with multiple roots)
     using a minimum spanning tree.
 
     Parameters
@@ -1776,14 +1784,17 @@
                 smaller than ``min_size`` will be ignored during stitching and
                 hence remain disconnected.
     drop_disc : bool
                 If True and the neuron remains fragmented after healing (i.e.
                 ``max_dist`` or ``min_size`` prevented a full connect), we will
                 keep only the largest (by number of nodes) connected component
                 and discard all other fragments.
+    mask :      list-like, optional
+                Either a boolean mask or a list of node IDs. If provided will
+                only heal breaks between these nodes.
     inplace :   bool, optional
                 If False, will perform healing on and return a copy.
 
     Returns
     -------
     None
                 If ``inplace=True``.
@@ -1811,15 +1822,15 @@
     >>> healed = navis.heal_skeleton(n)
     >>> len(healed.root)
     1
 
     """
     method = str(method).upper()
 
-    if method not in ['LEAFS', 'ALL']:
+    if method not in ('LEAFS', 'ALL'):
         raise ValueError(f'Unknown method "{method}"')
 
     # The decorator makes sure that at this point we have single neurons
     if not isinstance(x, core.TreeNeuron):
         raise TypeError(f'Expected TreeNeuron(s), got "{type(x)}"')
 
     if not isinstance(max_dist, type(None)):
@@ -1828,14 +1839,15 @@
     if not inplace:
         x = x.copy()
 
     _ = _stitch_mst(x,
                     nodes=method,
                     max_dist=max_dist,
                     min_size=min_size,
+                    mask=mask,
                     inplace=True)
 
     # See if we need to drop remaining disconnected fragments
     if drop_disc:
         # Compute this property only once
         trees = x.subtrees
         if len(trees) > 1:
@@ -1847,32 +1859,36 @@
 
 def _stitch_mst(x: 'core.TreeNeuron',
                 nodes:  Union[Literal['LEAFS'],
                               Literal['ALL'],
                               list] = 'ALL',
                 max_dist: Optional[float] = np.inf,
                 min_size: Optional[float] = None,
+                mask: Optional[Sequence] = None,
                 inplace: bool = False) -> Optional['core.TreeNeuron']:
     """Stitch disconnected neuron using a minimum spanning tree.
 
     Parameters
     ----------
     x :             TreeNeuron
                     Neuron to stitch.
     nodes :         "ALL" | "LEAFS" | list of IDs
                     Nodes that can be used to stitch the neuron. Can be "ALL"
-                    nodes, just "LEAFS" or a list of node IDs.
+                    nodes, just "LEAFS".
     max_dist :      int | float | str
                     If given, will only connect fragments if they are within
                     ``max_distance``. Use this to prevent the creation of
                     unrealistic edges.
     min_size :      int, optional
                     Minimum size in nodes for fragments to be reattached.
                     Fragments smaller than ``min_size`` will be ignored during
                     stitching and hence remain disconnected.
+    mask :          list-like, optional
+                    Either a boolean mask or a list of node IDs. If provided
+                    will only heal breaks between these nodes.
     inplace :       bool
                     If True, will stitch the original neuron in place.
 
     Return
     ------
     TreeNeuron
                     Only if ``inplace=True``.
@@ -1880,14 +1896,22 @@
     """
     assert isinstance(x, core.TreeNeuron)
     # Code modified from neuprint-python:
     # https://github.com/connectome-neuprint/neuprint-python
     if max_dist is True or not max_dist:
         max_dist = np.inf
 
+    if not isinstance(mask, type(None)):
+        mask = np.asarray(mask)
+        if mask.dtype == bool:
+            if len(mask) != len(x.nodes):
+                raise ValueError("Length of boolean mask must match number of "
+                                 "nodes in the neuron")
+            mask = x.nodes.node_id.values[mask]
+
     g = x.graph.to_undirected()
 
     # Extract each fragment's rows and construct a KD-Tree
     Fragment = namedtuple('Fragment', ['frag_id', 'df', 'kd'])
     fragments = []
     for frag_id, cc in enumerate(nx.connected_components(g)):
         if len(cc) == len(g.nodes):
@@ -1897,19 +1921,21 @@
         # Skip if fragment is smaller than threshold
         if not isinstance(min_size, type(None)):
             if len(cc) < min_size:
                 continue
 
         df = x.nodes.query('node_id in @cc')
 
+        # If mask, drop everything that is masked out
+        if not isinstance(mask, type(None)):
+            df = df[df.node_id.isin(mask)]
+
         # Filter to leaf nodes if applicable
-        if isinstance(nodes, str) and nodes == 'LEAFS':
+        if nodes == 'LEAFS':
             df = df[df['type'].isin(['end', 'root'])]
-        if utils.is_iterable(nodes):
-            df = df[df['node_id'].isin(nodes)]
 
         if not df.empty:
             kd = cKDTree(df[[*'xyz']].values)
             fragments.append(Fragment(frag_id, df, kd))
 
     # Sort from big-to-small, so the calculations below use a
     # KD tree for the larger point set in every fragment pair.
```

### Comparing `navis-1.4.0/navis/morpho/mmetrics.py` & `navis-1.5.0/navis/morpho/mmetrics.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/morpho/persistence.py` & `navis-1.5.0/navis/morpho/persistence.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 #    This script is part of navis (http://www.github.com/navis-org/navis).
 #    Copyright (C) 2018 Philipp Schlegel
 #
 #    This program is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
@@ -36,15 +35,15 @@
 
 @utils.map_neuronlist(desc='Calc. persistence', allow_parallel=True)
 def persistence_points(x: 'core.NeuronObject',
                        descriptor: Union[
                                          Literal['root_dist']
                                          ] = 'root_dist',
                        remove_cbf: bool = False
-                       ) -> 'core.NeuronObject':
+                       ) -> pd.DataFrame:
     """Calculate points for a persistence diagram.
 
     Based on Li et al., PLoS One (2017). Briefly, this cuts the neuron into
     linear segments, the start (birth) and end (death) of which are assigned a
     value (see ``descriptor`` parameter). In combination, these points represent
     a fingerprint for the topology of the neuron.
 
@@ -135,18 +134,16 @@
     pers['death'] = death
 
     return pers
 
 
 def persistence_distances(q: 'core.NeuronObject',
                           t: Optional['core.NeuronObject'] = None,
-                          scores: Union[Literal['forward'],
-                                        Literal['reverse'],
-                                        Literal['mean']] = 'mean',
                           augment: bool = True,
+                          normalize: bool = True,
                           bw: float = .2,
                           **persistence_kwargs):
     """Calculate morphological similarity using persistence diagrams.
 
     This works by:
       1. Generate persistence points for each neuron.
       2. Create a weighted Gaussian from persistence points and sample 100
@@ -155,16 +152,17 @@
 
     Parameters
     ----------
     q/t :       NeuronList
                 Queries and targets, respectively. If ``t=None`` will run
                 queries against queries. Neurons should have the same units,
                 ideally nanometers.
-    scores :    "forward" | "reverse" | "mean"
-
+    normalize : bool
+                If True, will normalized the vector for each neuron to be within
+                0-1. Set to False if the total number of linear segments matter.
     bw :        float
                 Bandwidth for Gaussian kernel: larger = smoother, smaller =
                 more detailed.
     augment :   bool
                 Whether to augment the persistence vectors with other neuron
                 properties (number of branch points & leafs and cable length).
     **persistence_kwargs
@@ -214,15 +212,18 @@
     # Get persistence points for each skeleton
     pers = persistence_points(all_n, **persistence_kwargs)
 
     # Get the vectors
     vectors, samples = persistence_vectors(pers, samples=100, bw=bw)
 
     # Normalizing the vectors will produce more useful distances
-    vectors = vectors / vectors.max(axis=1).reshape(-1, 1)
+    if normalize:
+        vectors = vectors / vectors.max(axis=1).reshape(-1, 1)
+    else:
+        vectors = vectors / vectors.max()
 
     if augment:
         # Collect extra data. Note that this adds only 3 more to the existing
         # 100 observations
         vec_aug = np.vstack((all_n.cable_length,
                              all_n.n_leafs,
                              all_n.n_branches)).T
@@ -241,27 +242,28 @@
         q_vec = vectors[:len(q)]
         t_vec = vectors[len(q):]
         return pd.DataFrame(cdist(q_vec, t_vec), index=q.id, columns=t.id)
     else:
         return pd.DataFrame(squareform(pdist(vectors)), index=q.id, columns=q.id)
 
 
-def persistence_vectors(pers,
+def persistence_vectors(x,
                         threshold: Optional[float] = None,
                         samples: int = 100,
                         bw: float = .2,
-                        center: bool = False):
+                        center: bool = False,
+                        **kwargs):
     """Produce vectors from persistence points.
 
     Works by creating a Gaussian and sampling ``samples`` evenly spaced
     points across it.
 
     Parameters
     ----------
-    pers :      pd.DataFrame | list thereof
+    x :         navis.NeuronList | pd.DataFrame | list thereof
                 The persistence points (see :func:`navis.persistence_points`).
                 For vectors for multiple neurons, provide either a list of
                 persistence points DataFrames or a single DataFrame with a
                 "neuron_id" column.
     threshold : float, optional
                 If provided, segments shorter (death - birth) than this will not
                 be used to create the Gaussian.
@@ -293,14 +295,29 @@
     --------
     :func:`navis.persistence_points`
                 The function to calculate the persistence points.
     :func:`navis.persistence_distances`
                 Get distances based on (augmented) persistence vectors.
 
     """
+    if isinstance(x, core.BaseNeuron):
+        x = core.NeuronList(x)
+
+    if isinstance(x, pd.DataFrame):
+        pers = [x]
+    elif isinstance(x, core.NeuronList):
+        pers = [persistence_points(n, **kwargs) for n in x]
+    elif isinstance(x, list):
+        if not all([isinstance(l, pd.DataFrame) for l in x]):
+            raise ValueError('Expected lists to contain only DataFrames')
+        pers = x
+    else:
+        raise TypeError('Unable to work extract persistence vectors from data '
+                        f'of type "{x}"')
+
     # Get the max distance
     max_pdist = max([p.birth.max() for p in pers])
     samples = np.linspace(0, max_pdist * 1.05, samples)
 
     # Now get a persistence vector
     vectors = []
     for p in pers:
@@ -325,38 +342,83 @@
         for i in range(len(vectors)):
             vectors[i] = np.roll(vectors[i],
                                  -np.argmax(vectors[i]) + len(samples) // 2)
 
     return vectors, samples
 
 
-def persistence_diagram(pers, ax=None):
+def persistence_diagram(pers, ax=None, **kwargs):
     """Plot a persistence diagram.
 
     Parameters
     ----------
     pers :      pd.DataFrame
                 Persistent points from :func:`navis.persistence_points`.
     ax :        matplotlib ax, optional
                 Ax to plot on.
+    **kwargs
+                Keyword arguments are passed to `LineCollection`.
 
     Returns
     -------
     ax :        matplotlib ax
 
     """
+    if not isinstance(pers, pd.DataFrame):
+        raise TypeError(f'Expected DataFrame, got "{type(pers)}"')
+
     if not ax:
         fig, ax = plt.subplots()
 
     segs = []
     for i, (b, d) in enumerate(zip(pers.birth.values, pers.death.values)):
         segs.append([[b, i], [d, i]])
-    lc = LineCollection(segs)
+    lc = LineCollection(segs, **kwargs)
     ax.add_collection(lc)
 
     ax.set_xlim(-5, pers.death.max())
     ax.set_ylim(-5, pers.shape[0])
 
     ax.set_ylabel('segments')
     ax.set_xlabel('time')
 
     return ax
+
+
+def persistence_vector_plot(x, normalize=True, ax=None,
+                            persistence_kwargs={}, vector_kwargs={}):
+    """Plot persistence vectors.
+
+    Parameters
+    ----------
+    x :         TreeNeuron | MeshNeuron | NeuronList
+                Neuron(s) to calculate persistence points for. For MeshNeurons,
+                we will use the skeleton produced by/associated with its
+                ``.skeleton`` property.
+
+    Returns
+    -------
+    ax
+
+    """
+    if not isinstance(x, core.NeuronList):
+        x = core.NeuronList(x)
+
+    # Get persistence points for each skeleton
+    pers = persistence_points(x, **persistence_kwargs)
+
+    # Get the vectors
+    vectors, samples = persistence_vectors(pers, **vector_kwargs)
+
+    # Normalizing the vectors will produce more useful distances
+    if normalize:
+        vectors = vectors / vectors.max(axis=1).reshape(-1, 1)
+    else:
+        vectors = vectors / vectors.max()
+
+    if not ax:
+        fig, ax = plt.subplots()
+
+    for n, v in zip(x, vectors):
+        ax.plot(samples, v, label=n.label)
+
+    return ax
```

### Comparing `navis-1.4.0/navis/morpho/subset.py` & `navis-1.5.0/navis/morpho/subset.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,16 @@
     # Mask vectors
     # This will also trigger re-calculation which is necessary for two reasons:
     # 1. Vectors will change if they have to be recalculated from
     #    the downsampled dotprops.
     # 2. There might not be enough points left after downsampling given the
     #    original k.
     if isinstance(x._vect, type(None)) and x.k:
-        x.recalculate_tangents(k=x.k, inplace=True)
+        if x.n_points >= x.k:
+            x.recalculate_tangents(k=x.k, inplace=True)
     x._vect = x._vect[mask]
 
     # Mask alphas if exists
     if not isinstance(x._alpha, type(None)):
         x._alpha = x._alpha[mask]
 
     # Finally mask points
```

### Comparing `navis-1.4.0/navis/nbl/__init__.py` & `navis-1.5.0/navis/nbl/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,10 +11,12 @@
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 
 """Module containing a Python implementation of NBLAST."""
 
 from .nblast_funcs import nblast, nblast_allbyall, nblast_smart
 from .synblast_funcs import synblast
-from .utils import (extract_matches, update_scores, dendrogram, make_clusters)
+from .ablast_funcs import nblast_align
+from .utils import (extract_matches, update_scores, dendrogram, make_clusters, compress_scores)
 
-__all__ = ['nblast', 'nblast_allbyall', 'nblast_smart', 'synblast']
+__all__ = ['nblast', 'nblast_allbyall', 'nblast_smart', 'synblast',
+           'nblast_align']
```

### Comparing `navis-1.4.0/navis/nbl/base.py` & `navis-1.5.0/navis/nbl/base.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/nbl/nblast_funcs.py` & `navis-1.5.0/navis/nbl/nblast_funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,18 @@
 
 # This multiplier controls job size for NBLASTs (only relevant for
 # multiprocessing and if progress=True).
 # Larger multiplier = larger job sizes = fewer jobs = slower updates & less overhead
 # Smaller multiplier = smaller job sizes = more jobs = faster updates & more overhead
 JOB_SIZE_MULTIPLIER = 1
 
+# This controls how many threads we allow pykdtree to use during multi-core
+# NBLAST
+OMP_NUM_THREADS_LIMIT = 1
+
 
 class NBlaster(Blaster):
     """Implements version 2 of the NBLAST algorithm.
 
     Please note that some properties are computed on initialization and
     changing parameters (e.g. ``use_alpha``) at a later stage will mess things
     up!
@@ -62,36 +66,35 @@
                     If True, the dotproduct of nearest neighbor vectors will
                     be scaled by ``sqrt(alpha1 * alpha2)``.
     normalized :    bool
                     If True, will normalize scores by the best possible score
                     (i.e. self-self) of the query neuron.
     smat :          navis.nbl.smat.Lookup2d | pd.DataFrame | str | Callable
                     How to convert the point match pairs into an NBLAST score,
-                    usually by a lookup table.
-                    If 'auto' (default), will use scoring matrices
-                    from FCWB. Same behaviour as in R's nat.nblast
-                    implementation.
-                    If ``smat='v1'`` it uses the analytic formulation of the
-                    NBLAST scoring from Kohl et. al (2013). You can adjust parameter
-                    ``sigma_scaling`` (default to 10) using ``smat_kwargs``.
-                    Dataframes will be used to build a ``Lookup2d``.
-                    If ``limit_dist`` is not given,
-                    will attempt to infer from the first axis of the lookup table.
-                    If ``Callable`` given, it passes distance and dot products as
-                    first and second argument respectively.
-                    If ``smat=None`` the scores will be
-                    generated as the product of the distances and the dotproduct
-                    of the vectors of nearest-neighbor pairs.
+                    usually by a lookup table:
+                     - if 'auto' (default), will use the "official" NBLAST scoring
+                       matrices based on FCWB data. Same behaviour as in R's
+                       nat.nblast implementation.
+                     - if ``smat='v1'`` it uses the analytic formulation of the
+                       NBLAST scoring from Kohl et. al (2013). You can adjust parameter
+                       ``sigma_scaling`` (default to 10) using ``smat_kwargs``.
+                     - DataFrames will be used to build a ``Lookup2d``
+                     - if ``Callable`` given, it passes distance and dot products as
+                       first and second argument respectively
+                     - if ``smat=None`` the scores will be generated as the
+                       product of the distances and the dotproduct of the vectors
+                       of nearest-neighbor pairs
     smat_kwargs:    Dictionary with additional parameters passed to scoring
                     functions. For example: ``smat_kwargs["sigma_scoring"] = 10``.
     limit_dist :    float | "auto" | None
                     Sets the max distance for the nearest neighbor search
                     (`distance_upper_bound`). Typically this should be the
                     highest distance considered by the scoring function. If
-                    "auto", will extract that value from the scoring matrix.
+                    "auto", will extract that value from the first axis of the
+                    scoring matrix.
     progress :      bool
                     If True, will show a progress bar.
 
     """
 
     def __init__(self, use_alpha=False, normalized=True, smat='auto',
                  limit_dist=None, approx_nn=False, dtype=np.float64,
@@ -435,93 +438,95 @@
                   dtype=precision,
                   approx_nn=approx_nn,
                   progress=progress,
                   smat_kwargs=smat_kwargs)
     query_self_hits = np.array([nb.calc_self_hit(n) for n in query_dps_simp])
     target_self_hits = np.array([nb.calc_self_hit(n) for n in target_dps_simp])
 
-    # Initialize a pool of workers
-    # Note that we're forcing "spawn" instead of "fork" (default on linux)!
-    # This is to reduce the memory footprint since "fork" appears to inherit all
-    # variables (including all neurons) while "spawn" appears to get only
-    # what's required to run the job?
-    with ProcessPoolExecutor(max_workers=n_cores,
-                             mp_context=mp.get_context('spawn')) as pool:
-        with config.tqdm(desc='Prep. pre-NBLAST',
-                         total=n_rows * n_cols,
-                         leave=False,
-                         disable=not progress) as pbar:
-            futures = {}
-            nblasters = []
-            for qix in np.array_split(np.arange(len(query_dps_simp)), n_rows):
-                for tix in np.array_split(np.arange(len(target_dps_simp)), n_cols):
-                    # Initialize NBlaster
-                    this = NBlaster(use_alpha=use_alpha,
-                                    normalized=normalized,
-                                    smat=smat,
-                                    limit_dist=limit_dist,
-                                    dtype=precision,
-                                    approx_nn=approx_nn,
-                                    progress=progress,
-                                    smat_kwargs=smat_kwargs)
-
-                    # Add queries and targets
-                    for i, ix in enumerate(qix):
-                        this.append(query_dps_simp[ix], query_self_hits[ix])
-                    for i, ix in enumerate(tix):
-                        this.append(target_dps_simp[ix], target_self_hits[ix])
-
-                    # Keep track of indices of queries and targets
-                    this.queries = np.arange(len(qix))
-                    this.targets = np.arange(len(tix)) + len(qix)
-                    this.queries_ix = qix  # this facilitates filling in the big matrix later
-                    this.targets_ix = tix  # this facilitates filling in the big matrix later
-                    this.pbar_position = len(nblasters) if not utils.is_jupyter() else None
-
-                    nblasters.append(this)
-                    pbar.update()
-
-                    # If multiple cores requested, submit job to the pool right away
-                    if n_cores and n_cores > 1 and (n_cols > 1 or n_rows > 1):
-                        this.progress=False  # no progress bar for individual NBLASTERs
-                        futures[pool.submit(this.multi_query_target,
-                                            q_idx=this.queries,
-                                            t_idx=this.targets,
-                                            scores=scores)] = this
-
-        # Collect results
-        if futures and len(futures) > 1:
-            # Prepare empty score matrix
-            scr = pd.DataFrame(np.empty((len(query_dps_simp),
-                                         len(target_dps_simp)),
-                                        dtype=this.dtype),
-                                  index=query_dps_simp.id,
-                                  columns=target_dps_simp.id)
-            scr.index.name = 'query'
-            scr.columns.name = 'target'
+    # This makes sure we don't run into multiple layers of concurrency
+    with set_omp_flag(limits=OMP_NUM_THREADS_LIMIT if n_cores and (n_cores > 1) else None):
+        # Initialize a pool of workers
+        # Note that we're forcing "spawn" instead of "fork" (default on linux)!
+        # This is to reduce the memory footprint since "fork" appears to inherit all
+        # variables (including all neurons) while "spawn" appears to get only
+        # what's required to run the job?
+        with ProcessPoolExecutor(max_workers=n_cores,
+                                 mp_context=mp.get_context('spawn')) as pool:
+            with config.tqdm(desc='Prep. pre-NBLAST',
+                             total=n_rows * n_cols,
+                             leave=False,
+                             disable=not progress) as pbar:
+                futures = {}
+                nblasters = []
+                for qix in np.array_split(np.arange(len(query_dps_simp)), n_rows):
+                    for tix in np.array_split(np.arange(len(target_dps_simp)), n_cols):
+                        # Initialize NBlaster
+                        this = NBlaster(use_alpha=use_alpha,
+                                        normalized=normalized,
+                                        smat=smat,
+                                        limit_dist=limit_dist,
+                                        dtype=precision,
+                                        approx_nn=approx_nn,
+                                        progress=progress,
+                                        smat_kwargs=smat_kwargs)
+
+                        # Add queries and targets
+                        for i, ix in enumerate(qix):
+                            this.append(query_dps_simp[ix], query_self_hits[ix])
+                        for i, ix in enumerate(tix):
+                            this.append(target_dps_simp[ix], target_self_hits[ix])
+
+                        # Keep track of indices of queries and targets
+                        this.queries = np.arange(len(qix))
+                        this.targets = np.arange(len(tix)) + len(qix)
+                        this.queries_ix = qix  # this facilitates filling in the big matrix later
+                        this.targets_ix = tix  # this facilitates filling in the big matrix later
+                        this.pbar_position = len(nblasters) if not utils.is_jupyter() else None
+
+                        nblasters.append(this)
+                        pbar.update()
+
+                        # If multiple cores requested, submit job to the pool right away
+                        if n_cores and n_cores > 1 and (n_cols > 1 or n_rows > 1):
+                            this.progress=False  # no progress bar for individual NBLASTERs
+                            futures[pool.submit(this.multi_query_target,
+                                                q_idx=this.queries,
+                                                t_idx=this.targets,
+                                                scores=pre_scores)] = this
 
             # Collect results
-            # We're dropping the "N / N_total" bit from the progress bar because
-            # it's not helpful here
-            fmt = ('{desc}: {percentage:3.0f}%|{bar}| [{elapsed}<{remaining}]')
-            for f in config.tqdm(as_completed(futures),
-                                 desc='Pre-NBLASTs',
-                                 bar_format=fmt,
-                                 total=len(futures),
-                                 smoothing=0,
-                                 disable=not progress,
-                                 leave=False):
-                res = f.result()
-                this = futures[f]
-                # Fill-in big score matrix
-                scr.iloc[this.queries_ix, this.targets_ix] = res.values
-        else:
-            scr = this.multi_query_target(this.queries,
-                                          this.targets,
-                                          scores=scores)
+            if futures and len(futures) > 1:
+                # Prepare empty score matrix
+                scr = pd.DataFrame(np.empty((len(query_dps_simp),
+                                             len(target_dps_simp)),
+                                            dtype=this.dtype),
+                                      index=query_dps_simp.id,
+                                      columns=target_dps_simp.id)
+                scr.index.name = 'query'
+                scr.columns.name = 'target'
+
+                # Collect results
+                # We're dropping the "N / N_total" bit from the progress bar because
+                # it's not helpful here
+                fmt = ('{desc}: {percentage:3.0f}%|{bar}| [{elapsed}<{remaining}]')
+                for f in config.tqdm(as_completed(futures),
+                                     desc='Pre-NBLASTs',
+                                     bar_format=fmt,
+                                     total=len(futures),
+                                     smoothing=0,
+                                     disable=not progress,
+                                     leave=False):
+                    res = f.result()
+                    this = futures[f]
+                    # Fill-in big score matrix
+                    scr.iloc[this.queries_ix, this.targets_ix] = res.values
+            else:
+                scr = this.multi_query_target(this.queries,
+                                              this.targets,
+                                              scores=scores)
 
     # If this is an all-by-all and we would have computed only forward scores
     # during pre-NBLAST
     if aba and scores == 'mean':
         scr = (scr + scr.T.values) / 2
 
     # Now select targets of interest for each query
@@ -543,92 +548,94 @@
         for N in range(t):
             mask.values[_, srt[:, N]] = True
 
     # Calculate self-hits for full neurons
     query_self_hits = np.array([nb.calc_self_hit(n) for n in query_dps])
     target_self_hits = np.array([nb.calc_self_hit(n) for n in target_dps])
 
-    # Initialize a pool of workers
-    # Note that we're forcing "spawn" instead of "fork" (default on linux)!
-    # This is to reduce the memory footprint since "fork" appears to inherit all
-    # variables (including all neurons) while "spawn" appears to get only
-    # what's required to run the job?
-    with ProcessPoolExecutor(max_workers=n_cores,
-                             mp_context=mp.get_context('spawn')) as pool:
-        with config.tqdm(desc='Prep. full NBLAST',
-                         total=n_rows * n_cols,
-                         leave=False,
-                         disable=not progress) as pbar:
-            futures = {}
-            nblasters = []
-            for qix in np.array_split(np.arange(len(query_dps)), n_rows):
-                for tix in np.array_split(np.arange(len(target_dps)), n_cols):
-                    # Initialize NBlaster
-                    this = NBlaster(use_alpha=use_alpha,
-                                    normalized=normalized,
-                                    smat=smat,
-                                    limit_dist=limit_dist,
-                                    dtype=precision,
-                                    approx_nn=approx_nn,
-                                    progress=progress,
-                                    smat_kwargs=smat_kwargs)
-
-                    # Add queries and targets
-                    for i, ix in enumerate(qix):
-                        this.append(query_dps[ix], query_self_hits[ix])
-                    for i, ix in enumerate(tix):
-                        this.append(target_dps[ix], target_self_hits[ix])
-
-                    # Find the pairs to NBLAST in this part of the matrix
-                    submask = mask.loc[query_dps[qix].id,
-                                       target_dps[tix].id]
-                    # `pairs` is an array of `[[query, target], [...]]` pairs
-                    this.pairs = np.vstack(np.where(submask)).T
-
-                    # Offset the query indices
-                    this.pairs[:, 1] += len(qix)
-
-                    # Track this NBLASTER's mask relative to the original big one
-                    this.mask = np.zeros(mask.shape, dtype=bool)
-                    this.mask[qix[0]:qix[-1]+1, tix[0]:tix[-1]+1] = submask
-
-                    # Make sure position of progress bar checks out
-                    this.pbar_position = len(nblasters) if not utils.is_jupyter() else None
-                    this.desc = 'Full NBLAST'
-
-                    nblasters.append(this)
-                    pbar.update()
-
-                    # If multiple cores requested, submit job to the pool right away
-                    if n_cores and n_cores > 1 and (n_cols > 1 or n_rows > 1):
-                        this.progress=False  # no progress bar for individual NBLASTERs
-                        futures[pool.submit(this.pair_query_target,
-                                            pairs=this.pairs,
-                                            scores=scores)] = this
+    # This makes sure we don't run into multiple layers of concurrency
+    with set_omp_flag(limits=OMP_NUM_THREADS_LIMIT if n_cores and (n_cores > 1) else None):
+        # Initialize a pool of workers
+        # Note that we're forcing "spawn" instead of "fork" (default on linux)!
+        # This is to reduce the memory footprint since "fork" appears to inherit all
+        # variables (including all neurons) while "spawn" appears to get only
+        # what's required to run the job?
+        with ProcessPoolExecutor(max_workers=n_cores,
+                                 mp_context=mp.get_context('spawn')) as pool:
+            with config.tqdm(desc='Prep. full NBLAST',
+                             total=n_rows * n_cols,
+                             leave=False,
+                             disable=not progress) as pbar:
+                futures = {}
+                nblasters = []
+                for qix in np.array_split(np.arange(len(query_dps)), n_rows):
+                    for tix in np.array_split(np.arange(len(target_dps)), n_cols):
+                        # Initialize NBlaster
+                        this = NBlaster(use_alpha=use_alpha,
+                                        normalized=normalized,
+                                        smat=smat,
+                                        limit_dist=limit_dist,
+                                        dtype=precision,
+                                        approx_nn=approx_nn,
+                                        progress=progress,
+                                        smat_kwargs=smat_kwargs)
+
+                        # Add queries and targets
+                        for i, ix in enumerate(qix):
+                            this.append(query_dps[ix], query_self_hits[ix])
+                        for i, ix in enumerate(tix):
+                            this.append(target_dps[ix], target_self_hits[ix])
+
+                        # Find the pairs to NBLAST in this part of the matrix
+                        submask = mask.loc[query_dps[qix].id,
+                                           target_dps[tix].id]
+                        # `pairs` is an array of `[[query, target], [...]]` pairs
+                        this.pairs = np.vstack(np.where(submask)).T
+
+                        # Offset the query indices
+                        this.pairs[:, 1] += len(qix)
+
+                        # Track this NBLASTER's mask relative to the original big one
+                        this.mask = np.zeros(mask.shape, dtype=bool)
+                        this.mask[qix[0]:qix[-1]+1, tix[0]:tix[-1]+1] = submask
+
+                        # Make sure position of progress bar checks out
+                        this.pbar_position = len(nblasters) if not utils.is_jupyter() else None
+                        this.desc = 'Full NBLAST'
+
+                        nblasters.append(this)
+                        pbar.update()
+
+                        # If multiple cores requested, submit job to the pool right away
+                        if n_cores and n_cores > 1 and (n_cols > 1 or n_rows > 1):
+                            this.progress=False  # no progress bar for individual NBLASTERs
+                            futures[pool.submit(this.pair_query_target,
+                                                pairs=this.pairs,
+                                                scores=scores)] = this
 
-        # Collect results
-        if futures and len(futures) > 1:
             # Collect results
-            # We're dropping the "N / N_total" bit from the progress bar because
-            # it's not helpful here
-            fmt = ('{desc}: {percentage:3.0f}%|{bar}| [{elapsed}<{remaining}]')
-            for f in config.tqdm(as_completed(futures),
-                                 desc='NBLASTing',
-                                 bar_format=fmt,
-                                 total=len(futures),
-                                 smoothing=0,
-                                 disable=not progress,
-                                 leave=False):
-                res = f.result()
-                this = futures[f]
-
-                # Fill-in big score matrix
-                scr[this.mask] = res
-        else:
-            scr[mask] = this.pair_query_target(this.pairs, scores=scores)
+            if futures and len(futures) > 1:
+                # Collect results
+                # We're dropping the "N / N_total" bit from the progress bar because
+                # it's not helpful here
+                fmt = ('{desc}: {percentage:3.0f}%|{bar}| [{elapsed}<{remaining}]')
+                for f in config.tqdm(as_completed(futures),
+                                     desc='NBLASTing',
+                                     bar_format=fmt,
+                                     total=len(futures),
+                                     smoothing=0,
+                                     disable=not progress,
+                                     leave=False):
+                    res = f.result()
+                    this = futures[f]
+
+                    # Fill-in big score matrix
+                    scr[this.mask] = res
+            else:
+                scr[mask] = this.pair_query_target(this.pairs, scores=scores)
 
     if return_mask:
         return scr, mask
 
     return scr
 
 
@@ -785,16 +792,18 @@
             # from spawning and sending results between processes slows things
             # down dramatically. Hence we want to make sure that each job runs
             # for >10s. The run time depends on the system and how big the neurons
             # are. Here, we run a quick test and try to extrapolate from there
             n_rows, n_cols = find_batch_partition(query_dps, target_dps,
                                                   T=10 * JOB_SIZE_MULTIPLIER)
         else:
-            # If no progress bar needed, we can just split neurons evenly across
-            # all available cores
+            # If no progress bar needed, we could just split neurons evenly across
+            # all available cores but that can lead to one core lagging behind
+            # and finishing much later than all the others. To avoid this, we
+            # should probably
             n_rows, n_cols = find_optimal_partition(n_cores, query_dps, target_dps)
     else:
         n_rows = n_cols = 1
 
     # Calculate self-hits once for all neurons
     nb = NBlaster(use_alpha=use_alpha,
                   normalized=normalized,
@@ -803,91 +812,93 @@
                   dtype=precision,
                   approx_nn=approx_nn,
                   progress=progress,
                   smat_kwargs=smat_kwargs)
     query_self_hits = np.array([nb.calc_self_hit(n) for n in query_dps])
     target_self_hits = np.array([nb.calc_self_hit(n) for n in target_dps])
 
-    # Initialize a pool of workers
-    # Note that we're forcing "spawn" instead of "fork" (default on linux)!
-    # This is to reduce the memory footprint since "fork" appears to inherit all
-    # variables (including all neurons) while "spawn" appears to get only
-    # what's required to run the job?
-    with ProcessPoolExecutor(max_workers=n_cores,
-                             mp_context=mp.get_context('spawn')) as pool:
-        with config.tqdm(desc='Preparing',
-                         total=n_rows * n_cols,
-                         leave=False,
-                         disable=not progress) as pbar:
-            futures = {}
-            nblasters = []
-            for qix in np.array_split(np.arange(len(query_dps)), n_rows):
-                for tix in np.array_split(np.arange(len(target_dps)), n_cols):
-                    # Initialize NBlaster
-                    this = NBlaster(use_alpha=use_alpha,
-                                    normalized=normalized,
-                                    smat=smat,
-                                    limit_dist=limit_dist,
-                                    dtype=precision,
-                                    approx_nn=approx_nn,
-                                    progress=progress,
-                                    smat_kwargs=smat_kwargs)
-
-                    # Add queries and targets
-                    for i, ix in enumerate(qix):
-                        this.append(query_dps[ix], query_self_hits[ix])
-                    for i, ix in enumerate(tix):
-                        this.append(target_dps[ix], target_self_hits[ix])
-
-                    # Keep track of indices of queries and targets
-                    this.queries = np.arange(len(qix))
-                    this.targets = np.arange(len(tix)) + len(qix)
-                    this.queries_ix = qix  # this facilitates filling in the big matrix later
-                    this.targets_ix = tix  # this facilitates filling in the big matrix later
-                    this.pbar_position = len(nblasters) if not utils.is_jupyter() else None
-
-                    nblasters.append(this)
-                    pbar.update()
-
-                    # If multiple cores requested, submit job to the pool right away
-                    if n_cores and n_cores > 1 and (n_cols > 1 or n_rows > 1):
-                        this.progress=False  # no progress bar for individual NBLASTERs
-                        futures[pool.submit(this.multi_query_target,
-                                            q_idx=this.queries,
-                                            t_idx=this.targets,
-                                            scores=scores)] = this
-
-        # Collect results
-        if futures and len(futures) > 1:
-            # Prepare empty score matrix
-            scores = pd.DataFrame(np.empty((len(query_dps), len(target_dps)),
-                                           dtype=this.dtype),
-                                  index=query_dps.id, columns=target_dps.id)
-            scores.index.name = 'query'
-            scores.columns.name = 'target'
+    # This makes sure we don't run into multiple layers of concurrency
+    with set_omp_flag(limits=OMP_NUM_THREADS_LIMIT if n_cores and (n_cores > 1) else None):
+        # Initialize a pool of workers
+        # Note that we're forcing "spawn" instead of "fork" (default on linux)!
+        # This is to reduce the memory footprint since "fork" appears to inherit all
+        # variables (including all neurons) while "spawn" appears to get only
+        # what's required to run the job?
+        with ProcessPoolExecutor(max_workers=n_cores,
+                                 mp_context=mp.get_context('spawn')) as pool:
+            with config.tqdm(desc='Preparing',
+                             total=n_rows * n_cols,
+                             leave=False,
+                             disable=not progress) as pbar:
+                futures = {}
+                nblasters = []
+                for qix in np.array_split(np.arange(len(query_dps)), n_rows):
+                    for tix in np.array_split(np.arange(len(target_dps)), n_cols):
+                        # Initialize NBlaster
+                        this = NBlaster(use_alpha=use_alpha,
+                                        normalized=normalized,
+                                        smat=smat,
+                                        limit_dist=limit_dist,
+                                        dtype=precision,
+                                        approx_nn=approx_nn,
+                                        progress=progress,
+                                        smat_kwargs=smat_kwargs)
+
+                        # Add queries and targets
+                        for i, ix in enumerate(qix):
+                            this.append(query_dps[ix], query_self_hits[ix])
+                        for i, ix in enumerate(tix):
+                            this.append(target_dps[ix], target_self_hits[ix])
+
+                        # Keep track of indices of queries and targets
+                        this.queries = np.arange(len(qix))
+                        this.targets = np.arange(len(tix)) + len(qix)
+                        this.queries_ix = qix  # this facilitates filling in the big matrix later
+                        this.targets_ix = tix  # this facilitates filling in the big matrix later
+                        this.pbar_position = len(nblasters) if not utils.is_jupyter() else None
+
+                        nblasters.append(this)
+                        pbar.update()
+
+                        # If multiple cores requested, submit job to the pool right away
+                        if n_cores and n_cores > 1 and (n_cols > 1 or n_rows > 1):
+                            this.progress=False  # no progress bar for individual NBLASTERs
+                            futures[pool.submit(this.multi_query_target,
+                                                q_idx=this.queries,
+                                                t_idx=this.targets,
+                                                scores=scores)] = this
 
             # Collect results
-            # We're dropping the "N / N_total" bit from the progress bar because
-            # it's not helpful here
-            fmt = ('{desc}: {percentage:3.0f}%|{bar}| [{elapsed}<{remaining}]')
-            for f in config.tqdm(as_completed(futures),
-                                 desc='NBLASTing',
-                                 bar_format=fmt,
-                                 total=len(futures),
-                                 smoothing=0,
-                                 disable=not progress,
-                                 leave=False):
-                res = f.result()
-                this = futures[f]
-                # Fill-in big score matrix
-                scores.iloc[this.queries_ix, this.targets_ix] = res.values
-        else:
-            scores = this.multi_query_target(this.queries,
-                                             this.targets,
-                                             scores=scores)
+            if futures and len(futures) > 1:
+                # Prepare empty score matrix
+                scores = pd.DataFrame(np.empty((len(query_dps), len(target_dps)),
+                                               dtype=this.dtype),
+                                      index=query_dps.id, columns=target_dps.id)
+                scores.index.name = 'query'
+                scores.columns.name = 'target'
+
+                # Collect results
+                # We're dropping the "N / N_total" bit from the progress bar because
+                # it's not helpful here
+                fmt = ('{desc}: {percentage:3.0f}%|{bar}| [{elapsed}<{remaining}]')
+                for f in config.tqdm(as_completed(futures),
+                                     desc='NBLASTing',
+                                     bar_format=fmt,
+                                     total=len(futures),
+                                     smoothing=0,
+                                     disable=not progress,
+                                     leave=False):
+                    res = f.result()
+                    this = futures[f]
+                    # Fill-in big score matrix
+                    scores.iloc[this.queries_ix, this.targets_ix] = res.values
+            else:
+                scores = this.multi_query_target(this.queries,
+                                                 this.targets,
+                                                 scores=scores)
 
     return scores
 
 
 def nblast_allbyall(x: NeuronList,
                     normalized: bool = True,
                     use_alpha: bool = False,
@@ -989,16 +1000,16 @@
     See Also
     --------
     :func:`navis.nblast`
                 For generic query -> target nblasts.
 
     """
     # Check if pykdtree flag needed to be set
-    if n_cores and n_cores > 1:
-        check_pykdtree_flag()
+    #if n_cores and n_cores > 1:
+    #    check_pykdtree_flag()
 
     # Make sure we're working on NeuronLists
     dps = NeuronList(x)
 
     # Run NBLAST preflight checks
     # Note that we are passing the same dotprops twice to avoid having to
     # change the function's signature. Should have little to no overhead.
@@ -1032,93 +1043,95 @@
                   limit_dist=limit_dist,
                   dtype=precision,
                   approx_nn=approx_nn,
                   progress=progress,
                   smat_kwargs=smat_kwargs)
     self_hits = np.array([nb.calc_self_hit(n) for n in dps])
 
-    # Initialize a pool of workers
-    # Note that we're forcing "spawn" instead of "fork" (default on linux)!
-    # This is to reduce the memory footprint since "fork" appears to inherit all
-    # variables (including all neurons) while "spawn" appears to get only
-    # what's required to run the job?
-    with ProcessPoolExecutor(max_workers=n_cores,
-                             mp_context=mp.get_context('spawn')) as pool:
-        with config.tqdm(desc='Preparing',
-                         total=n_rows * n_cols,
-                         leave=False,
-                         disable=not progress) as pbar:
-            futures = {}
-            nblasters = []
-            for qix in np.array_split(np.arange(len(dps)), n_rows):
-                for tix in np.array_split(np.arange(len(dps)), n_cols):
-                    # Initialize NBlaster
-                    this = NBlaster(use_alpha=use_alpha,
-                                    normalized=normalized,
-                                    smat=smat,
-                                    limit_dist=limit_dist,
-                                    dtype=precision,
-                                    approx_nn=approx_nn,
-                                    progress=progress,
-                                    smat_kwargs=smat_kwargs)
-
-                    # Make sure we don't add the same neuron twice
-                    # Map indices to neurons
-                    to_add = list(set(qix) | set(tix))
-
-                    # Add neurons
-                    ixmap = {}
-                    for i, ix in enumerate(to_add):
-                        this.append(dps[ix], self_hits[ix])
-                        ixmap[ix] = i
-
-                    # Keep track of indices of queries and targets
-                    this.queries = [ixmap[ix] for ix in qix]
-                    this.targets = [ixmap[ix] for ix in tix]
-                    this.queries_ix = qix  # this facilitates filling in the big matrix later
-                    this.targets_ix = tix  # this facilitates filling in the big matrix later
-                    this.pbar_position = len(nblasters) if not utils.is_jupyter() else None
-
-                    nblasters.append(this)
-                    pbar.update()
-
-                    # If multiple cores requested, submit job to the pool right away
-                    if n_cores and n_cores > 1 and (n_cols > 1 or n_rows > 1):
-                        this.progress=False  # no progress bar for individual NBLASTERs
-                        futures[pool.submit(this.multi_query_target,
-                                            q_idx=this.queries,
-                                            t_idx=this.targets,
-                                            scores='forward')] = this
-
-        # Collect results
-        if futures and len(futures) > 1:
-            # Prepare empty score matrix
-            scores = pd.DataFrame(np.empty((len(dps), len(dps)),
-                                           dtype=this.dtype),
-                                  index=dps.id, columns=dps.id)
-            scores.index.name = 'query'
-            scores.columns.name = 'target'
+    # This makes sure we don't run into multiple layers of concurrency
+    with set_omp_flag(limits=OMP_NUM_THREADS_LIMIT if n_cores and (n_cores > 1) else None):
+        # Initialize a pool of workers
+        # Note that we're forcing "spawn" instead of "fork" (default on linux)!
+        # This is to reduce the memory footprint since "fork" appears to inherit all
+        # variables (including all neurons) while "spawn" appears to get only
+        # what's required to run the job?
+        with ProcessPoolExecutor(max_workers=n_cores,
+                                 mp_context=mp.get_context('spawn')) as pool:
+            with config.tqdm(desc='Preparing',
+                             total=n_rows * n_cols,
+                             leave=False,
+                             disable=not progress) as pbar:
+                futures = {}
+                nblasters = []
+                for qix in np.array_split(np.arange(len(dps)), n_rows):
+                    for tix in np.array_split(np.arange(len(dps)), n_cols):
+                        # Initialize NBlaster
+                        this = NBlaster(use_alpha=use_alpha,
+                                        normalized=normalized,
+                                        smat=smat,
+                                        limit_dist=limit_dist,
+                                        dtype=precision,
+                                        approx_nn=approx_nn,
+                                        progress=progress,
+                                        smat_kwargs=smat_kwargs)
+
+                        # Make sure we don't add the same neuron twice
+                        # Map indices to neurons
+                        to_add = list(set(qix) | set(tix))
+
+                        # Add neurons
+                        ixmap = {}
+                        for i, ix in enumerate(to_add):
+                            this.append(dps[ix], self_hits[ix])
+                            ixmap[ix] = i
+
+                        # Keep track of indices of queries and targets
+                        this.queries = [ixmap[ix] for ix in qix]
+                        this.targets = [ixmap[ix] for ix in tix]
+                        this.queries_ix = qix  # this facilitates filling in the big matrix later
+                        this.targets_ix = tix  # this facilitates filling in the big matrix later
+                        this.pbar_position = len(nblasters) if not utils.is_jupyter() else None
+
+                        nblasters.append(this)
+                        pbar.update()
+
+                        # If multiple cores requested, submit job to the pool right away
+                        if n_cores and n_cores > 1 and (n_cols > 1 or n_rows > 1):
+                            this.progress=False  # no progress bar for individual NBLASTERs
+                            futures[pool.submit(this.multi_query_target,
+                                                q_idx=this.queries,
+                                                t_idx=this.targets,
+                                                scores='forward')] = this
 
             # Collect results
-            # We're dropping the "N / N_total" bit from the progress bar because
-            # it's not helpful here
-            fmt = ('{desc}: {percentage:3.0f}%|{bar}| [{elapsed}<{remaining}]')
-            for f in config.tqdm(as_completed(futures),
-                                 desc='NBLASTing',
-                                 bar_format=fmt,
-                                 total=len(futures),
-                                 smoothing=0,
-                                 disable=not progress,
-                                 leave=False):
-                res = f.result()
-                this = futures[f]
-                # Fill-in big score matrix
-                scores.iloc[this.queries_ix, this.targets_ix] = res.values
-        else:
-            scores = this.all_by_all()
+            if futures and len(futures) > 1:
+                # Prepare empty score matrix
+                scores = pd.DataFrame(np.empty((len(dps), len(dps)),
+                                               dtype=this.dtype),
+                                      index=dps.id, columns=dps.id)
+                scores.index.name = 'query'
+                scores.columns.name = 'target'
+
+                # Collect results
+                # We're dropping the "N / N_total" bit from the progress bar because
+                # it's not helpful here
+                fmt = ('{desc}: {percentage:3.0f}%|{bar}| [{elapsed}<{remaining}]')
+                for f in config.tqdm(as_completed(futures),
+                                     desc='NBLASTing',
+                                     bar_format=fmt,
+                                     total=len(futures),
+                                     smoothing=0,
+                                     disable=not progress,
+                                     leave=False):
+                    res = f.result()
+                    this = futures[f]
+                    # Fill-in big score matrix
+                    scores.iloc[this.queries_ix, this.targets_ix] = res.values
+            else:
+                scores = this.all_by_all()
 
     return scores
 
 
 def find_batch_partition(q, t, T=10):
     """Find partitions such that each batch takes about `T` seconds."""
     # Get a median-sized query and target
@@ -1343,26 +1356,36 @@
     else:
         mx = x.max()
 
     return (x - mx) * -1
 
 
 def nblast_preflight(query, target, n_cores, batch_size=None,
-                     req_unique_ids=False, req_dotprops=True,
+                     req_unique_ids=False, req_dotprops=True, req_points=True,
                      req_microns=True):
     """Run preflight checks for NBLAST."""
     if req_dotprops:
         if query.types != (Dotprops, ):
             raise TypeError(f'`query` must be Dotprop(s), got "{query.types}". '
                             'Use `navis.make_dotprops` to convert neurons.')
 
         if target.types != (Dotprops, ):
             raise TypeError(f'`target` must be Dotprop(s), got "{target.types}". '
                             'Use `navis.make_dotprops` to convert neurons.')
 
+        if req_points:
+            no_points = query.n_points == 0
+            if any(no_points):
+                raise ValueError('Some query dotprops appear to have no points: '
+                                 f'{query.id[no_points]}')
+            no_points = target.n_points == 0
+            if any(no_points):
+                raise ValueError('Some target dotprops appear to have no points: '
+                                 f'{target.id[no_points]}')
+
     if req_unique_ids:
         # At the moment, neurons need to have a unique ID for things to work
         if query.is_degenerated:
             raise ValueError('Queries have non-unique IDs.')
         if target.is_degenerated:
             raise ValueError('Targets have non-unique IDs.')
 
@@ -1422,12 +1445,46 @@
         import pykdtree
     except ImportError:
         # If not present, just return
         return
 
     import os
     if os.environ.get('OMP_NUM_THREADS', None) != "1":
-        msg = ('`OMP_NUM_THREADS` environment variable not set to "1". '
-               'This may cause multiple layers of concurrency which in turn will'
+        msg = ('`OMP_NUM_THREADS` environment variable not set to 1. This may '
+               'result in multiple layers of concurrency which in turn will '
                'slow down NBLAST when using multiple cores. '
                'See also https://github.com/navis-org/navis/issues/49')
         logger.warning(msg)
+
+
+def set_omp_flag(limits=1):
+    """Set OMP_NUM_THREADS flag to given value.
+
+    This is to avoid pykdtree causing multiple layers of concurrency which
+    will over-subcribe and slow down NBLAST on multi-core systems.
+
+    Use as context manager!
+    """
+    class OMPSetter:
+        def __init__(self, num_threads):
+            assert isinstance(num_threads, (int, type(None)))
+            self.num_threads = num_threads
+
+        def __enter__(self):
+            if self.num_threads is None:
+                return
+            # Track old value (if there is one)
+            self.old_value = os.environ.get('OMP_NUM_THREADS', None)
+            # Set flag
+            os.environ['OMP_NUM_THREADS'] = str(self.num_threads)
+
+        def __exit__(self, *args, **kwargs):
+            if self.num_threads is None:
+                return
+
+            # Reset flag
+            if self.old_value:
+                os.environ['OMP_NUM_THREADS'] = str(self.old_value)
+            else:
+                os.environ.pop('OMP_NUM_THREADS', None)
+
+    return OMPSetter(limits)
```

### Comparing `navis-1.4.0/navis/nbl/score_mats/smat_alpha_fcwb.csv` & `navis-1.5.0/navis/nbl/score_mats/smat_alpha_fcwb.csv`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/nbl/score_mats/smat_fcwb.csv` & `navis-1.5.0/navis/nbl/score_mats/smat_fcwb.csv`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/nbl/smat.py` & `navis-1.5.0/navis/nbl/smat.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/nbl/synblast_funcs.py` & `navis-1.5.0/navis/nbl/synblast_funcs.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/nbl/utils.py` & `navis-1.5.0/navis/nbl/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,23 +7,21 @@
 #    (at your option) any later version.
 #
 #    This program is distributed in the hope that it will be useful,
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 
-"""Module containing base classes for BLASTING."""
+"""Module containing utility functions for BLASTING."""
 
 import numpy as np
 import pandas as pd
 import scipy.cluster.hierarchy as sch
 
-from abc import ABC, abstractmethod
-from typing import Union, List
-from scipy.spatial.distance import squareform
+from scipy.spatial.distance import squareform, pdist
 
 from .. import config
 
 logger = config.logger
 
 
 def extract_matches(scores, N=None, threshold=None, percentage=None,
@@ -55,19 +53,14 @@
 
     Returns
     -------
     pd.DataFrame
                     Note that the format is slightly different depending on
                     the criterion.
 
-    See Also
-    --------
-    :func:navis.nbl.extract_matches_threshold`
-                If you all matches above a given threshold.
-
     """
     assert axis in (0, 1), '`axis` must be 0 or 1'
 
     if N is None and threshold is None and percentage is None:
         raise ValueError('Must provide either `N` or `threshold` or '
                          '`percentage` as criterion for match extraction.')
     elif len({N, threshold, percentage}) > 2:
@@ -133,30 +126,18 @@
     """Extract all matches above a given threshold from score matrix."""
     if not distances:
         ind, cols = np.where(scores.values >= threshold)
     else:
         ind, cols = np.where(scores.values <= threshold)
 
     matches = pd.DataFrame()
-    matches.index = scores.index
-
-    match_str = []
-    scores_str = []
-    for i in range(len(matches)):
-        this = cols[ind == i]
-        sc = scores.iloc[i].values[this]
-        srt = np.argsort(sc)[::-1]
-        m = scores.columns[this][srt]
-        sc = sc[srt]
-
-        match_str.append(','.join(m.astype(str)))
-        scores_str.append(','.join(sc.round(3).astype(str)))
-
-    matches['matches'] = match_str
-    matches['scores'] = scores_str
+    matches['query'] = scores.index[ind]
+    matches['match'] = scores.columns[cols]
+    matches['score'] = scores.values[ind, cols]
+    matches = matches.sort_values(['query', 'match', 'score']).set_index(['query', 'match'])
 
     return matches
 
 
 def _extract_matches_perc(scores, perc=.05, distances=False):
     """Extract all matches within a given percentage of the top match."""
     if not distances:
@@ -171,15 +152,15 @@
     matches = pd.DataFrame()
     matches.index = scores.index
 
     match_str = []
     scores_str = []
     for i in range(len(matches)):
         this = cols[ind == i]
-        sc = scores.iloc[i].values[this]
+        sc = scores.values[i, this]
         srt = np.argsort(sc)[::-1]
         m = scores.columns[this][srt]
         sc = sc[srt]
 
         match_str.append(','.join(m.astype(str)))
         scores_str.append(','.join(sc.round(3).astype(str)))
 
@@ -255,14 +236,44 @@
         logger.info(f'Updating old queries -> new targets scores')
         tq = nblast_func(queries[~is_new_q], targets[is_new_t], **kwargs)
         scores.loc[tq.index, tq.columns] = tq.values
 
     return scores
 
 
+def compress_scores(scores, threshold=None, digits=None):
+    """Compress scores.
+
+    This will not necessarily reduce the in-memory footprint but will lead to
+    much smaller file sizes when saved to disk.
+
+    Parameters
+    ----------
+    scores :        pandas.DataFrame
+    threshold :     float, optional
+                    Scores lower than this will be capped at `threshold`.
+    digits :        int, optional
+                    Round scores to the Nth digit.
+
+    Returns
+    -------
+    scores_comp :   pandas.DataFrame
+                    Copy of the original dataframe with the data cast to 32bit
+                    floats and the optional filters (see `threshold` and
+                    `digits`) applied.
+
+    """
+    scores = scores.astype(np.float32)
+    if digits is not None:
+        scores = scores.round(digits)
+    if threshold is not None:
+        scores.clip(lower=threshold, inplace=True)
+    return scores
+
+
 def make_linkage(x, method='single', optimal_ordering=False):
     """Make linkage from input. If input looks like linkage it is passed through."""
     if isinstance(x, pd.DataFrame):
         # Make sure it is symmetric
         if x.shape[0] != x.shape[1]:
             raise ValueError(f'Scores must be symmetric, got shape {x.shape}')
         # A cheap check for whether these are mean scores
@@ -351,7 +362,56 @@
         cl = sch.cut_tree(Z, n_clusters=t, **kwargs).flatten()
     elif criterion == 'height':
         cl = sch.cut_tree(Z, height=t, **kwargs).flatten()
     else:
         cl = sch.fcluster(Z, t=t, criterion=criterion, **kwargs)
 
     return cl
+
+
+def nblast_prime(scores, n_dim=.2, metric='euclidean'):
+    """Generate a smoothed version of the NBLAST scores.
+
+    In brief:
+     1. Run PCA on the NBLAST scores and extract the first N components.
+     2. From that calulate a new similarity matrix.
+
+    Requires scikit-learn.
+
+    Parameters
+    ----------
+    scores :    pandas.DataFrame
+                The all-by-all NBLAST scores.
+    n_dim :     float | int
+                The number of dimensions to use. If float (0 < n_dim < 1) will
+                use `scores.shape[0] * n_dim`.
+    metric :    str
+                Which distance metric to use. Directly passed through to the
+                `scipy.spatial.distance.pdist` function.
+
+    Returns
+    -------
+    scores_new
+
+    """
+    try:
+        from sklearn.decomposition import PCA
+    except ImportError:
+        raise ImportError('Please install scikit-learn to use `nblast_prime`:\n'
+                          '  pip3 install scikit-learn -U')
+
+    if not isinstance(scores, pd.DataFrame):
+        raise TypeError(f'`scores` must be pandas DataFrame, got "{type(scores)}"')
+
+    if (scores.shape[0] != scores.shape[1]) or ~np.all(scores.columns == scores.index):
+        logger.warning('NBLAST matrix is not symmetric - are you sure this is '
+                       'an all-by-all matrix?')
+
+    if n_dim < 1:
+        n_dim = int(scores.shape[1] * n_dim)
+
+    pca = PCA(n_components=n_dim)
+    X_new = pca.fit_transform(scores.values)
+
+    dist = pdist(X_new, metric=metric)
+
+    return pd.DataFrame(1 - squareform(dist), index=scores.index, columns=scores.columns)
```

### Comparing `navis-1.4.0/navis/plotting/__init__.py` & `navis-1.5.0/navis/plotting/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 from .ddd import *
 from .flat import *
 from .vispy import *
 
 from .colors import vary_colors
 
 __all__ = ['plot1d', 'plot2d', 'plot3d', 'plot_flat', 'vary_colors', 'Viewer',
-           'get_viewer', 'clear3d', 'close3d', 'screenshot']
+           'get_viewer', 'clear3d', 'close3d', 'pop3d', 'screenshot']
```

### Comparing `navis-1.4.0/navis/plotting/colors.py` & `navis-1.5.0/navis/plotting/colors.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,15 +310,15 @@
                 na = mcl.to_rgba(na, alpha=alpha)
             except ValueError:
                 raise ValueError('`na` must be either "raise" or a valid color '
                                  f'to replace NA values. Unable to convert {na}'
                                  ' to a color.')
 
     # First check if data is numerical or categorical
-    is_num = [utils.is_numeric(a, bool_numeric=False) for a in values]
+    is_num = [utils.is_numeric(a, bool_numeric=False, try_convert=False) for a in values]
     # If numerical
     if all(is_num):
         # Get min/max values
         if not vmin:
             vmin = [np.nanmin(v) for v in values]
 
             if norm_global:
```

### Comparing `navis-1.4.0/navis/plotting/d.py` & `navis-1.5.0/navis/plotting/d.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/plotting/dd.py` & `navis-1.5.0/navis/plotting/dd.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/plotting/ddd.py` & `navis-1.5.0/navis/plotting/ddd.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/plotting/flat.py` & `navis-1.5.0/navis/plotting/flat.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/plotting/k3d/k3d_objects.py` & `navis-1.5.0/navis/plotting/k3d/k3d_objects.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/plotting/plot_utils.py` & `navis-1.5.0/navis/plotting/plot_utils.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/plotting/plotly/graph_objs.py` & `navis-1.5.0/navis/plotting/plotly/graph_objs.py`

 * *Files 0% similar despite different names*

```diff
@@ -460,15 +460,15 @@
 
         if not isinstance(scatter, np.ndarray):
             scatter = np.array(scatter)
 
         trace_data.append(go.Scatter3d(x=scatter[:, 0],
                                        y=scatter[:, 1],
                                        z=scatter[:, 2],
-                                       mode='markers',
+                                       mode=kwargs.get('mode', 'markers'),
                                        marker=dict(color='rgb%s' % str(c),
                                                    size=s,
                                                    opacity=kwargs.get('opacity', 1)),
                                        name=name,
                                        showlegend=True,
                                        hoverinfo='none'))
     return trace_data
```

### Comparing `navis-1.4.0/navis/plotting/vispy/viewer.py` & `navis-1.5.0/navis/plotting/vispy/viewer.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/plotting/vispy/visuals.py` & `navis-1.5.0/navis/plotting/vispy/visuals.py`

 * *Files 0% similar despite different names*

```diff
@@ -507,15 +507,15 @@
                         soma_color = neuron_color[s_ix]
                     else:
                         soma_color = neuron_color
 
                     n = neuron.nodes.set_index('node_id').loc[s]
                     r = getattr(n, neuron.soma_radius) if isinstance(neuron.soma_radius, str) else neuron.soma_radius
                     sp = create_sphere(7, 7, radius=r)
-                    verts = sp.get_vertices() + n[['x', 'y', 'z']].values
+                    verts = sp.get_vertices() + n[['x', 'y', 'z']].values.astype(np.float32)
                     s = scene.visuals.Mesh(vertices=verts,
                                            shading='smooth',
                                            faces=sp.get_faces(),
                                            color=soma_color)
                     # Vispy 0.7.0 uses a new shading filter
                     if int(vispy.__version__.split('.')[1]) >= 7:
                         s.shading_filter.ambient_light = vispy.color.Color('white')
```

### Comparing `navis-1.4.0/navis/plotting/vispy/vputils.py` & `navis-1.5.0/navis/plotting/vispy/vputils.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 import png
 import warnings
 
 from ... import config
 
-__all__ = ['get_viewer', 'clear3d', 'close3d', 'screenshot']
+__all__ = ['get_viewer', 'clear3d', 'close3d', 'screenshot', 'pop3d']
 
 
 def get_viewer():
     """Grab active 3D viewer.
 
     Returns
     -------
@@ -59,14 +59,20 @@
         viewer.close()
         globals().pop('viewer')
         del viewer
     except BaseException:
         pass
 
 
+def pop3d():
+    """Remove the last item added to the 3D canvas."""
+    viewer = get_viewer()
+    viewer.pop()
+
+
 def screenshot(file='screenshot.png', alpha=True):
     """Save a screenshot of active vispy 3D canvas.
 
     Parameters
     ----------
     file :      str, optional
                 Filename
```

### Comparing `navis-1.4.0/navis/sampling/__init__.py` & `navis-1.5.0/navis/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/sampling/downsampling.py` & `navis-1.5.0/navis/sampling/downsampling.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/sampling/resampling.py` & `navis-1.5.0/navis/sampling/resampling.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/transforms/__init__.py` & `navis-1.5.0/navis/transforms/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,9 +17,11 @@
 from .affine import AffineTransform
 from .elastix import ElastixTransform
 from .thinplate import TPStransform
 from .h5reg import H5transform
 from .cmtk import CMTKtransform
 from .moving_least_squares import MovingLeastSquaresTransform
 
+from .import align
+
 # Make sure that only these functions are avaialable at top level
-__all__ = ['xform_brain', 'mirror_brain', 'xform', 'mirror', 'symmetrize_brain']
+__all__ = ['xform_brain', 'mirror_brain', 'xform', 'mirror', 'symmetrize_brain', 'align']
```

### Comparing `navis-1.4.0/navis/transforms/affine.py` & `navis-1.5.0/navis/transforms/affine.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/transforms/base.py` & `navis-1.5.0/navis/transforms/base.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/transforms/cmtk.py` & `navis-1.5.0/navis/transforms/cmtk.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/transforms/elastix.py` & `navis-1.5.0/navis/transforms/elastix.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/transforms/factory.py` & `navis-1.5.0/navis/transforms/factory.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/transforms/h5reg.py` & `navis-1.5.0/navis/transforms/h5reg.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/transforms/h5reg_java.py` & `navis-1.5.0/navis/transforms/h5reg_java.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/transforms/moving_least_squares.py` & `navis-1.5.0/navis/transforms/moving_least_squares.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/transforms/templates.py` & `navis-1.5.0/navis/transforms/templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #    This program is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
 #
 #    This program is distributed in the hope that it will be useful,
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
-#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 #    GNU General Public License for more details.
 
 """Functions to work with templates."""
 
 import functools
 import math
 import numbers
@@ -53,35 +53,34 @@
 
 # Defines entry the registry needs to register a transform
 transform_reg = namedtuple('Transform',
                            ['source', 'target', 'transform', 'type',
                             'invertible', 'weight'])
 
 # Check for environment variable pointing to registries
-_os_transpaths = os.environ.get('NAVIS_TRANSFORMS', '')
+_OS_TRANSPATHS = os.environ.get('NAVIS_TRANSFORMS', '')
 try:
-    _os_transpaths = [i for i in _os_transpaths.split(';') if len(i) > 0]
+    _OS_TRANSPATHS = [i for i in _OS_TRANSPATHS.split(';') if len(i) > 0]
 except BaseException:
     logger.error('Error parsing the `NAVIS_TRANSFORMS` environment variable')
-    _os_transpaths = []
+    _OS_TRANSPATHS = []
 
 
 class TemplateRegistry:
     """Tracks template brains, available transforms and produces bridging sequences.
 
     Parameters
     ----------
     scan_paths :    bool
                     If True will scan paths on initialization.
 
     """
-
     def __init__(self, scan_paths: bool = True):
         # Paths to scan for transforms
-        self._transpaths = _os_transpaths
+        self._transpaths = _OS_TRANSPATHS.copy()
         # Transforms
         self._transforms = []
         # Template brains
         self._templates = []
 
         if scan_paths:
             self.scan_paths()
@@ -683,56 +682,59 @@
 
 def xform_brain(x: Union['core.NeuronObject', 'pd.DataFrame', 'np.ndarray'],
                 source: str,
                 target: str,
                 via: Optional[str] = None,
                 affine_fallback: bool = True,
                 caching: bool = True,
-                verbose = True) -> Union['core.NeuronObject',
-                                         'pd.DataFrame',
-                                         'np.ndarray']:
+                verbose: bool = True) -> Union['core.NeuronObject',
+                                               'pd.DataFrame',
+                                               'np.ndarray']:
     """Transform 3D data between template brains.
 
     This requires the appropriate transforms to be registered with ``navis``.
-    See the docs for details.
+    See the docs/tutorials for details.
 
     Notes
     -----
-    For Neurons only: whether there is a change in units during transformation
-    (e.g. nm -> um) is inferred by comparing distances between x/y/z coordinates
-    before and after transform. This guesstimate is then used to convert
-    ``.units`` and node/soma radii. This works reasonably well with base 10
-    increments (e.g. nm -> um) but may be off with odd changes in units (e.g.
-    physical -> voxel space).
+    For Neurons only: transforms can introduce a change in the units (e.g. if
+    the transform goes from micron to nanometer space). Some template brains have
+    their units hard-coded in their meta data (as ``_navis_units``). If that's
+    not the case we fall-back to trying to infer any change in units by comparing
+    distances between x/y/z coordinate before and after the transform. That
+    approach works reasonably well with base 10 increments (e.g. nm -> um) but
+    may be off with odd changes in units (e.g. physical -> voxel space).
+    Regardless of whether hard-coded or inferred, any change in units is used to
+    update the ``.units`` property and node/soma radii for TreeNeurons.
 
     Parameters
     ----------
     x :                 Neuron/List | numpy.ndarray | pandas.DataFrame
                         Data to transform. Dataframe must contain ``['x', 'y', 'z']``
                         columns. Numpy array must be shape ``(N, 3)``.
     source :            str
                         Source template brain that the data currently is in.
     target :            str
                         Target template brain that the data should be
                         transformed into.
     via :               str, optional
-                        Optional define an intermediate template. This can be
+                        Optionally set an intermediate template. This can be
                         helpful to force a specific transformation sequence.
     affine_fallback :   bool
-                        In same cases the non-rigid transformation of points
+                        In some cases the non-rigid transformation of points
                         can fail - for example if points are outside the
                         deformation field. If that happens, they will be
-                        returned as ``NaN``. Unless ``affine_fallback`` is
-                        ``True``, in which case we will apply only the rigid
-                        affine  part of the transformation to at least get close
-                        to the correct coordinates.
+                        returned as ``NaN``. If ``affine_fallback=True``
+                        we will apply only the rigid affine part of the
+                        transformation to those points to get as close as
+                        possible to the correct coordinates.
     caching :           bool
                         If True, will (pre-)cache data for transforms whenever
                         possible. Depending on the data and the type of
-                        transforms this can tremendously speed things up at the
+                        transforms this can speed things up significantly at the
                         cost of increased memory usage:
                           - ``False`` = no upfront cost, lower memory footprint
                           - ``True`` = higher upfront cost, most definitely faster
                         Only applies if input is NeuronList and if transforms
                         include H5 transform.
     verbose :           bool
                         If True, will print some useful info on transform.
@@ -765,14 +767,17 @@
     >>> xf = navis.xform_brain(n, source='JRCFIB2018Fraw', target='FAFB14') # doctest: +SKIP
 
     See Also
     --------
     :func:`navis.xform`
                     Lower level entry point that takes data and applies a given
                     transform or sequence thereof.
+    :func:`navis.mirror_brain`
+                    Uses non-rigid transforms to mirror neurons from the left
+                    to the right side of given template brain and vice versa.
 
     """
     if not isinstance(source, str):
         TypeError(f'Expected source of type str, got "{type(source)}"')
 
     if not isinstance(target, str):
         TypeError(f'Expected target of type str, got "{type(target)}"')
@@ -791,16 +796,38 @@
 
         print('Transform path:', path_str)
 
     # Combine into transform sequence
     trans_seq = TransformSequence(*transforms)
 
     # Apply transform and returned xformed points
-    return xform(x, transform=trans_seq, caching=caching,
-                 affine_fallback=affine_fallback)
+    xf = xform(x, transform=trans_seq, caching=caching,
+               affine_fallback=affine_fallback)
+
+    # We might be able to set the correct units based on the target template's
+    # meta data (the "guessed" new units can be off if the transform is
+    # not base 10 which happens for e.g. voxels -> physical space)
+    if isinstance(xf, (core.NeuronList, core.BaseNeuron)):
+        # First we need to find the last non-alias template space
+        for tmp, tr in zip(path[::-1], transforms[::-1]):
+            if not isinstance(tr, AliasTransform):
+                # There is a chance that there is no meta data for this template
+                try:
+                    last_temp = registry.find_template(tmp)
+                except ValueError:
+                    break
+                except BaseException:
+                    raise
+                # If this template brain has a property for navis units
+                if hasattr(last_temp, '_navis_units'):
+                    for n in core.NeuronList(xf):
+                        n.units = last_temp._navis_units
+                break
+
+    return xf
 
 
 def _guess_change(xyz_before: np.ndarray,
                   xyz_after: np.ndarray,
                   sample: float = .1) -> tuple:
     """Guess change in units during xforming."""
     if isinstance(xyz_before, pd.DataFrame):
@@ -858,14 +885,16 @@
     template :      str | TemplateBrain
                     Source template brain space that the data is in. If string
                     will be searched against registered template brains.
     via :           "auto" | str
                     By default ("auto") it will find and apply the closest
                     mirror transform. You can also specify a template that
                     should be used. That template must have a mirror transform!
+    verbose :       bool
+                    If True, will print some useful info on the transform(s).
 
     Returns
     -------
     xs
                     Same object type as input (array, neurons, etc) but
                     hopefully symmetrical.
 
@@ -1026,23 +1055,26 @@
                     Source template brain space that the data is in. If string
                     will be searched against registered template brains.
                     Alternatively check out :func:`navis.transforms.mirror`
                     for a lower level interface.
     mirror_axis :   'x' | 'y' | 'z', optional
                     Axis to mirror. Defaults to `x`.
     warp :          bool | "auto" | Transform, optional
-                    If 'auto', will check if a mirror transformation exists
-                    for the given ``template`` and apply it after the flipping.
-                    You can also just pass a Transform or TransformSequence.
+                    If 'auto', will check if a non-rigi mirror transformation
+                    exists for the given ``template`` and apply it after the
+                    flipping. Alternatively, you can also pass a Transform or
+                    TransformSequence directly.
     via :           str | None
                     If provided, (e.g. "FCWB") will first transform coordinates
                     into that space, then mirror and transform back.
                     Use this if there is no mirror registration for the original
                     template, or to transform to a symmetrical template in which
                     flipping is sufficient.
+    verbose :       bool
+                    If True, will print some useful info on the transform(s).
 
     Returns
     -------
     xf
                     Same object type as input (array, neurons, etc) but with
                     transformed coordinates.
 
@@ -1250,16 +1282,16 @@
     """Generic base class for template brains.
 
     Minimally, a template should have a `name` and `label` property. For
     mirroring, it also needs a `boundingbox`.
 
     See `navis-flybrains <https://github.com/navis-org/navis-flybrains>`_ for
     an example of how to use template brains.
-    """
 
+    """
     def __init__(self, **properties):
         """Initialize class."""
         for k, v in properties.items():
             setattr(self, k, v)
 
     @property
     def mesh(self):
```

### Comparing `navis-1.4.0/navis/transforms/thinplate.py` & `navis-1.5.0/navis/transforms/thinplate.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/transforms/xfm_funcs.py` & `navis-1.5.0/navis/transforms/xfm_funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #    This program is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
 #
 #    This program is distributed in the hope that it will be useful,
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
-#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 #    GNU General Public License for more details.
 
 import math
 import numbers
 
 import numpy as np
 import pandas as pd
@@ -165,15 +165,20 @@
 
         # Do the xform of all spatial data
         xyz_xf = xform(xyz,
                        transform=transform,
                        affine_fallback=affine_fallback)
 
         # Guess change in spatial units
-        change, magnitude = _guess_change(xyz, xyz_xf, sample=1000)
+        if xyz.shape[0] > 1:
+            change, magnitude = _guess_change(xyz, xyz_xf, sample=1000)
+        else:
+            change, magnitude = 1, 0
+            logger.warning(f'Unable to assess change of units for neuron {x.id}: '
+                           'must have at least two nodes/points.')
 
         # Round change -> this rounds to the first non-zero digit
         # change = np.around(change, decimals=-magnitude)
 
         # Map xformed coordinates back
         if isinstance(xf, core.TreeNeuron):
             xf.nodes.loc[:, ['x', 'y', 'z']] = xyz_xf[:xf.n_nodes]
```

### Comparing `navis-1.4.0/navis/utils/__init__.py` & `navis-1.5.0/navis/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/utils/cv.py` & `navis-1.5.0/navis/utils/cv.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/utils/decorators.py` & `navis-1.5.0/navis/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/utils/eval.py` & `navis-1.5.0/navis/utils/eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,39 +73,43 @@
                    f'Allowed value(s): {", ".join([str(t) for t in allowed_values])}')
             if on_error == 'raise':
                 raise ValueError(msg)
             elif on_error == 'warn':
                 logger.warning(msg)
 
 
-def is_numeric(array: np.ndarray, bool_numeric: bool = True) -> bool:
+def is_numeric(array: np.ndarray,
+               bool_numeric: bool = True,
+               try_convert: bool = False) -> bool:
     """Determine whether the argument has a numeric datatype.
 
     Booleans, unsigned integers, signed integers, floats and complex
     numbers are the kinds of numeric datatype.
 
     Arrays with "dtype=object" will return True if data can be cast to floats.
 
     Parameters
     ----------
     array :         array-like
                     The array to check.
     bool_numeric :  bool
                     If True (default), we count booleans as numeric data types.
+    try_convert :   bool
+                    If True, will try to convert array to floats.
 
     Returns
     -------
     is_numeric :    `bool`
                     True if the array has a numeric datatype, False if not.
 
     """
     array = np.asarray(array)
 
     # If array
-    if array.dtype.kind == 'O':
+    if array.dtype.kind == 'O' and try_convert:
         try:
             array = array.astype(float)
         except ValueError:
             pass
 
     if not bool_numeric:
         _NUMERIC_KINDS_NO_BOOL = _NUMERIC_KINDS.copy()
```

### Comparing `navis-1.4.0/navis/utils/exceptions.py` & `navis-1.5.0/navis/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/utils/iterables.py` & `navis-1.5.0/navis/utils/iterables.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/utils/misc.py` & `navis-1.5.0/navis/utils/misc.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis/utils/validate.py` & `navis-1.5.0/navis/utils/validate.py`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/navis.egg-info/PKG-INFO` & `navis-1.5.0/navis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: navis
-Version: 1.4.0
+Version: 1.5.0
 Summary: Neuron Analysis and Visualization library
 Home-page: http://navis.readthedocs.io
 Author: Philipp Schlegel
 Author-email: pms70@cam.ac.uk
 License: GNU GPL V3
 Project-URL: Documentation, http://navis.readthedocs.io
 Project-URL: Source, https://github.com/navis-org/navis
 Project-URL: Changelog, https://navis.readthedocs.io/en/latest/source/whats_new.html
-Keywords: Neuron Analysis Visualization Anatomy Connectivity Transform Neuroscience NBLAST Skeletons SWC neuPrint
+Keywords: Neuron Analysis Visualization Morphometrics Morphology Anatomy Connectivity Transform Neuroscience NBLAST Skeletons SWC neuPrint
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: pathos
 Provides-Extra: shapely
 Provides-Extra: r
 Provides-Extra: kdtree
 Provides-Extra: hash
 Provides-Extra: flybrains
@@ -45,15 +45,15 @@
 Provides-Extra: vispy-tk
 License-File: LICENSE
 
 [![Documentation Status](https://readthedocs.org/projects/navis/badge/?version=latest)](http://navis.readthedocs.io/en/latest/?badge=latest) [![Tests](https://github.com/navis-org/navis/actions/workflows/test-package.yml/badge.svg)](https://github.com/navis-org/navis/actions/workflows/test-package.yml) [![Run notebooks](https://github.com/navis-org/navis/actions/workflows/notebooktest-package.yml/badge.svg)](https://github.com/navis-org/navis/actions/workflows/notebooktest-package.yml) [![Coverage Status](https://coveralls.io/repos/github/navis-org/navis/badge.svg?branch=master)](https://coveralls.io/github/navis-org/navis?branch=master) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/navis-org/navis/blob/master/examples/colab.ipynb) [![DOI](https://zenodo.org/badge/168142416.svg)](https://zenodo.org/badge/latestdoi/168142416) [![Downloads](https://pepy.tech/badge/navis)](https://pepy.tech/project/navis)
 
 <img src="https://github.com/navis-org/navis/raw/master/docs/_static/favicon.png" height="60">
 
-NAVis is a Python 3 (3.7 or later) library for **N**euron **A**nalysis and **Vis**ualization.
+NAVis is a Python 3 (3.8 or later) library for **N**euron **A**nalysis and **Vis**ualization.
 
 ## Documentation
 NAVis is on [ReadTheDocs](http://navis.readthedocs.io/ "NAVis ReadTheDocs").
 
 ## Features
 * works as Jupyter notebook, script or from terminal
 * support for various neuron types: **skeletons**, **meshes**, **dotprops**, **voxels**
@@ -103,17 +103,17 @@
 ## NAVis & friends
 <p align="center">
 <img src="https://github.com/navis-org/navis/blob/master/docs/_static/navis_ecosystem.png?raw=true" width="700">
 </p>
 
 NAVis comes with batteries included but is also highly extensible. Some
 libraries built on top of NAVis:
-* [flybrains](https://github.com/navis-org/navis-flybrains) provides templates and transforms to use with navis
+* [flybrains](https://github.com/navis-org/navis-flybrains) provides templates and transforms for *Drosophila* brains to use with navis
 * [pymaid](https://pymaid.readthedocs.io/en/latest/) pulls and pushes data from/to CATMAID servers
-* [fafbseg](https://fafbseg-py.readthedocs.io/en/latest/index.html) contains tools to work with autosegmented data for the FAFB EM dataset
+* [fafbseg](https://fafbseg-py.readthedocs.io/en/latest/index.html) contains tools to work with auto-segmented data for the FAFB EM dataset
 
 ## License
 This code is under GNU GPL V3
 
 ## Acknowledgments
 NAVis is inspired by and inherits much of its design from the excellent
 [natverse](http://natverse.org) R packages by
```

### Comparing `navis-1.4.0/navis.egg-info/SOURCES.txt` & `navis-1.5.0/navis.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -109,14 +109,15 @@
 navis/morpho/analyze.py
 navis/morpho/fq.py
 navis/morpho/manipulation.py
 navis/morpho/mmetrics.py
 navis/morpho/persistence.py
 navis/morpho/subset.py
 navis/nbl/__init__.py
+navis/nbl/ablast_funcs.py
 navis/nbl/base.py
 navis/nbl/nblast_funcs.py
 navis/nbl/smat.py
 navis/nbl/synblast_funcs.py
 navis/nbl/utils.py
 navis/nbl/score_mats/smat_alpha_fcwb.csv
 navis/nbl/score_mats/smat_fcwb.csv
@@ -137,14 +138,15 @@
 navis/plotting/vispy/visuals.py
 navis/plotting/vispy/vputils.py
 navis/sampling/__init__.py
 navis/sampling/downsampling.py
 navis/sampling/resampling.py
 navis/transforms/__init__.py
 navis/transforms/affine.py
+navis/transforms/align.py
 navis/transforms/base.py
 navis/transforms/cmtk.py
 navis/transforms/elastix.py
 navis/transforms/factory.py
 navis/transforms/h5reg.py
 navis/transforms/h5reg_java.py
 navis/transforms/moving_least_squares.py
@@ -154,8 +156,13 @@
 navis/utils/__init__.py
 navis/utils/cv.py
 navis/utils/decorators.py
 navis/utils/eval.py
 navis/utils/exceptions.py
 navis/utils/iterables.py
 navis/utils/misc.py
-navis/utils/validate.py
+navis/utils/validate.py
+tests/test_io.py
+tests/test_neurons.py
+tests/test_notebooks.py
+tests/test_parallel.py
+tests/test_transforms.py
```

### Comparing `navis-1.4.0/navis.egg-info/requires.txt` & `navis-1.5.0/navis.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `navis-1.4.0/setup.py` & `navis-1.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,32 +52,31 @@
     project_urls={
      "Documentation": "http://navis.readthedocs.io",
      "Source": "https://github.com/navis-org/navis",
      "Changelog": "https://navis.readthedocs.io/en/latest/source/whats_new.html",
     },
     author='Philipp Schlegel',
     author_email='pms70@cam.ac.uk',
-    keywords='Neuron Analysis Visualization Anatomy Connectivity Transform Neuroscience NBLAST Skeletons SWC neuPrint',
+    keywords='Neuron Analysis Visualization Morphometrics Morphology Anatomy Connectivity Transform Neuroscience NBLAST Skeletons SWC neuPrint',
     classifiers=[
         'Development Status :: 4 - Beta',
 
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
 
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
 
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
     ],
     install_requires=install_requires,
     extras_require=dict(extras_require),
     tests_require=extras_require["dev"],
-    # CI runs against >=3.7
-    # but R-Python interface ships with 3.6 so this is necessary
-    python_requires='>=3.6',
+    # CI runs against >=3.8
+    python_requires='>=3.8',
     zip_safe=False,
 
     include_package_data=True
 
 )
```

