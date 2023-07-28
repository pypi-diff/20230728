# Comparing `tmp/emobject-0.7.0b2.tar.gz` & `tmp/emobject-0.7.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emobject-0.7.0b2.tar", last modified: Fri Jul 28 18:21:39 2023, max compression
+gzip compressed data, was "emobject-0.7.0b3.tar", last modified: Fri Jul 28 18:35:36 2023, max compression
```

## Comparing `emobject-0.7.0b2.tar` & `emobject-0.7.0b3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 18:21:39.592228 emobject-0.7.0b2/
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-28 18:21:30.000000 emobject-0.7.0b2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4225 2023-07-28 18:21:39.592228 emobject-0.7.0b2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3826 2023-07-28 18:21:30.000000 emobject-0.7.0b2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 18:21:39.590228 emobject-0.7.0b2/emobject/
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    40016 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/core.py
--rw-rw-rw-   0 root         (0) root         (0)    15643 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/database.py
--rw-rw-rw-   0 root         (0) root         (0)    32512 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/emexperiment.py
--rw-rw-rw-   0 root         (0) root         (0)    14806 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/emimage.py
--rw-rw-rw-   0 root         (0) root         (0)     9750 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/emlayer.py
--rw-rw-rw-   0 root         (0) root         (0)    49374 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/emobject.py
--rw-rw-rw-   0 root         (0) root         (0)     6759 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/empublicaccess.py
--rw-rw-rw-   0 root         (0) root         (0)     9493 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/emroitools.py
--rw-rw-rw-   0 root         (0) root         (0)       96 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 18:21:39.592228 emobject-0.7.0b2/emobject/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3543 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/utils/graph.py
--rw-rw-rw-   0 root         (0) root         (0)     2447 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/utils/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    24229 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/utils/io.py
--rw-rw-rw-   0 root         (0) root         (0)    11201 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/utils/visualization.py
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 18:21:39.591228 emobject-0.7.0b2/emobject.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4225 2023-07-28 18:21:39.000000 emobject-0.7.0b2/emobject.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      559 2023-07-28 18:21:39.000000 emobject-0.7.0b2/emobject.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 18:21:39.000000 emobject-0.7.0b2/emobject.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      229 2023-07-28 18:21:39.000000 emobject-0.7.0b2/emobject.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-28 18:21:39.000000 emobject-0.7.0b2/emobject.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-28 18:21:39.593228 emobject-0.7.0b2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1263 2023-07-28 18:21:30.000000 emobject-0.7.0b2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 18:35:36.153705 emobject-0.7.0b3/
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-28 18:35:26.000000 emobject-0.7.0b3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4225 2023-07-28 18:35:36.153705 emobject-0.7.0b3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3826 2023-07-28 18:35:26.000000 emobject-0.7.0b3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 18:35:36.151705 emobject-0.7.0b3/emobject/
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    39223 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/core.py
+-rw-rw-rw-   0 root         (0) root         (0)    15643 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/database.py
+-rw-rw-rw-   0 root         (0) root         (0)    32512 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/emexperiment.py
+-rw-rw-rw-   0 root         (0) root         (0)    14806 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/emimage.py
+-rw-rw-rw-   0 root         (0) root         (0)     9750 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/emlayer.py
+-rw-rw-rw-   0 root         (0) root         (0)    49374 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/emobject.py
+-rw-rw-rw-   0 root         (0) root         (0)     6759 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/empublicaccess.py
+-rw-rw-rw-   0 root         (0) root         (0)     9493 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/emroitools.py
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 18:35:36.153705 emobject-0.7.0b3/emobject/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3543 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/utils/graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     2447 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/utils/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    24229 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/utils/io.py
+-rw-rw-rw-   0 root         (0) root         (0)    11201 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/utils/visualization.py
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 18:35:36.152705 emobject-0.7.0b3/emobject.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4225 2023-07-28 18:35:36.000000 emobject-0.7.0b3/emobject.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      559 2023-07-28 18:35:36.000000 emobject-0.7.0b3/emobject.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 18:35:36.000000 emobject-0.7.0b3/emobject.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      229 2023-07-28 18:35:36.000000 emobject-0.7.0b3/emobject.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-28 18:35:36.000000 emobject-0.7.0b3/emobject.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-28 18:35:36.153705 emobject-0.7.0b3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1263 2023-07-28 18:35:26.000000 emobject-0.7.0b3/setup.py
```

### Comparing `emobject-0.7.0b2/LICENSE` & `emobject-0.7.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b2/PKG-INFO` & `emobject-0.7.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emobject
-Version: 0.7.0b2
+Version: 0.7.0b3
 Summary: data abstraction and libraries for spatial omics
 Home-page: https://gitlab.com/enable-medicine/rnd-subgroup/emobject/
 Author: Ethan A. G. Baker
 Author-email: ethan.baker@enablemedicine.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7, <4
```

### Comparing `emobject-0.7.0b2/README.md` & `emobject-0.7.0b3/README.md`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b2/emobject/core.py` & `emobject-0.7.0b3/emobject/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from logging import warning
 
 from emobject.emobject import EMObject
 from emobject.emimage import EMMask, EMImage
 from emobject.emlayer import BaseLayer
 from emobject.errors import EMObjectException
 from emobject.utils import helpers
-from emobject import emroitools as roi
 from emobject.version import __version__
-import emobject.database as db
+
+from emoaccess.main import run_base_object_queries, run_mask_queries, run_image_queries, run_segmentation_mask_queries, run_metadata_queries
 
 
 class EMObjectConfig:
     '''Object that defines the config
     for an emObject that is interacting with the
     Enable database.
 
@@ -139,15 +139,15 @@
     Args:
         config: EMObjectConfig
 
     Returns:
         BaseLayer
     '''
 
-    cell_df, data_ix, ann_ix = build_base_object_from_enable_db(acquisition_id=config.acquisition_id,
+    bm_df, anno_df, coord_df = build_base_object_from_enable_db(acquisition_id=config.acquisition_id,
                                                                 biomarkers=config.biomarkers,
                                                                 annotations=config.annotations,
                                                                 segmentation_version=config.segmentation_version,
                                                                 biomarker_version=config.biomarker_version,
                                                                 config_mode=True)
 
     if config.include_img:
@@ -173,36 +173,36 @@
         segmentation = f"{segmentation}_1"
 
     # Need to add all the masks to the object's emmask
     if config.masks is not None:
         new_emmask = helpers.merge_emmasks(E.mask, config.masks)
         E.mask = new_emmask
 
-    new_layer = BaseLayer(data=cell_df.iloc[:, data_ix],
-                          obs=cell_df.iloc[:, ann_ix],
+    new_layer = BaseLayer(data=bm_df,
+                          obs=anno_df,
                           var=None,
-                          pos=cell_df.iloc[:, -2:],
+                          pos=coord_df,
                           name=config.acquisition_id,
                           segmentation=segmentation)
 
     E.add(new_layer)
     return E
 
 
-def build_emobject(config: EMObjectConfig) -> EMObject:
+def build_emobject(config: EMObjectConfig) -> EMObject :
     '''Builds a complete EMObject from the Enable database.
 
     Args:
         config: EMObjectConfig
 
     Returns:
         EMObject
     '''
 
-    cell_df, data_ix, ann_ix = build_base_object_from_enable_db(acquisition_id=config.acquisition_id,
+    bm_df, anno_df, coord_df = build_base_object_from_enable_db(acquisition_id=config.acquisition_id,
                                                                 biomarkers=config.biomarkers,
                                                                 annotations=config.annotations,
                                                                 segmentation_version=config.segmentation_version,
                                                                 biomarker_version=config.biomarker_version,
                                                                 config_mode=True)
 
     if config.include_img:
@@ -220,46 +220,66 @@
         config.masks = build_emmask_from_enable_db(acquisition_id=config.acquisition_id,
                                                    study_id=config.study_id,
                                                    include_masks=config.include_masks,
                                                    include_seg_masks=config.include_seg_mask,
                                                    seg_mask_type=config.seg_mask_type,
                                                    segmentation_version=config.segmentation_version,
                                                    biomarker_version=config.biomarker_version)
-    meta = db.get_all_metadata_for_acquisition_id(config.acquisition_id, conn=db.connect_sf())
+    meta = run_metadata_queries(config.acquisition_id)
 
     return EMObject(
-        data=cell_df.iloc[:, data_ix],
-        obs=cell_df.iloc[:, ann_ix],
+        data=bm_df,
+        obs=anno_df,
         var=None,
-        pos=cell_df.iloc[:, -2:],
+        pos=coord_df,
         mask=config.masks,
         img=config.img,
         meta=meta,
         name=config.acquisition_id,
         segmentation=segmentation)
 
 
 def build_base_object_from_enable_db(acquisition_id: Optional[str] = None,
                                      biomarkers: Optional[list] = None,
                                      annotations: Optional[list] = None,
                                      segmentation_version: int = None,
                                      biomarker_version: int = None,
                                      config_mode: Optional[bool] = False
                                      ) -> EMObject:
-    """Builds an EMObject from the Enable Database.
+    """Builds an EMObject from the Enable Database via Diglett.
 
     This is a separate function to allow for future open-sourcing
 
     Args:
         acquisition_id: acquistion ID for the region.
         biomarkers: A subset of biomarkers to include. If None, returns all.
         annotations: A subset of annotations to include.
     """
 
-    return EMObject()
+    bm_df, anno_df, coord_df = run_base_object_queries(
+        acquisition_id=acquisition_id,
+        biomarkers=biomarkers,
+        annotations=annotations,
+        segmentation_version=segmentation_version,
+        biomarker_version=biomarker_version,
+    )
+
+    if config_mode:
+        return bm_df, anno_df, coord_df
+
+    else:
+        return EMObject(
+            data=bm_df,
+            obs=anno_df,
+            var=None,
+            pos=coord_df,
+            mask=None,
+            img=None,
+            meta=None,
+            name=acquisition_id)
 
 
 def build_emmask_from_enable_db(acquisition_id: Optional[str] = None,
                                 study_id: Optional[int] = None,
                                 include_masks: Optional[bool] = None,
                                 include_seg_masks: Optional[bool] = None,
                                 seg_mask_type: Optional[str] = None,
@@ -271,49 +291,39 @@
 
     This needs to follow these steps:
         1. Obtain all story names for the study associated with this acq
         2. Subset the study's story names to the acquisition
         3. stack the masks into an object that can be passed to EMMask
     """
 
-    # Connect to RDS
-    conn = db.connect_rds()
-
-    if study_id is None and acquisition_id is None:
-        raise EMObjectException("Must specify acquisition id and/or study_id")
-
-    elif study_id is None:
-        study_id = db.get_study_id_for_acquisition_id(acquisition_id, conn)
-
     # Need to get the data for each story this is going to be VERY slow
     acquisition_masks = []
     mask_names = []
 
     if include_masks:
-        # START ALTERNATE WORKFLOW FOR 0.4.3
-        roi_df = db.get_roi_df_for_acquisition_id(acquisition_id, conn)
-        mask_dict = roi.roi_df_to_mask_dict(roi_df)
+        mask_dict = run_mask_queries(acquisition_id=acquisition_id)
 
         # TO DO: remove this logic in the future, didn't want to change to test new SQL
         for key in mask_dict.keys():
             acquisition_masks.append(mask_dict[key])
             mask_names.append(key)
 
     # Get the unique segment IDs (exclusive of cell segments)
     t = np.array(acquisition_masks)
     unique_seg_ids = np.sort(np.unique(t))
     del t
 
     if include_seg_masks:
-        seg_mask = db.get_seg_mask(acquisition_id=acquisition_id,
-                                   segmentation_version=segmentation_version,
-                                   biomarker_version=biomarker_version,
-                                   cur=conn,
-                                   b3=db.connect_boto3(),
-                                   mask=seg_mask_type)
+        seg_mask = run_segmentation_mask_queries(
+            acquisition_id=acquisition_id,
+            study_id=study_id,
+            seg_mask_type=seg_mask_type,
+            segmentation_version=segmentation_version,
+            biomarker_version=biomarker_version
+        )
 
         acquisition_masks.append(seg_mask)
         mask_names.append('segmentation_mask')
         max_cell_segment_id = np.max(seg_mask)
 
     # To avoid collisions, make new seg IDs for ROIs, sequentially following the
     # max cell ID.
@@ -346,50 +356,23 @@
         study_id (int): study, placeholder for future functionality
         channels (Union[list, np.ndarray]]): the channels to include, if None includes all.
 
     Returns:
         image (EMImage)
     '''
 
-    conn = db.connect_rds()
-
-    if channels is None:
-        # Get all channels.
-        channels = db.get_all_biomarkers_for_acquisition_id(acquisition_id, conn)
-
-    channel_images = list()
-    for biomarker in channels:
-        channel_images.append(db.get_channel_im(
-            acquisition_id,
-            biomarker,
-            cur=conn,
-            b3=db.connect_boto3(),
-            resolution=resolution))
-
-    channel_images = np.array(channel_images)
+    channel_images = run_image_queries(
+        acquisition_id=acquisition_id,
+        channels=channels,
+        resolution=resolution
+    )
 
     return EMImage(img=channel_images, channels=channels, to_disk=to_disk)
 
 
-def _clean_df_cols(col_names, acquisition_id, conn):
-    # get annotation names
-
-    name_dict = db.get_annotation_names(acquisition_id, conn)
-    updated_names = list()
-    for c in col_names:
-        if c.startswith('ANN'):
-            id = c.split('ANN')[1]
-            name = name_dict[int(id)].replace(' ', '-')
-            c = f"{id}_{name}"
-        elif c.startswith('BM'):
-            c = c.split('BM')[1]
-        updated_names.append(c)
-    return updated_names
-
-
 def save(E: EMObject = None,
          out_dir: Optional[str] = None,
          name: Optional[str] = None) -> None:
     '''Write an EMObject to disk.
 
     Args:
         E (EMObject): EMObject to write to disk
```

### Comparing `emobject-0.7.0b2/emobject/database.py` & `emobject-0.7.0b3/emobject/database.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b2/emobject/emexperiment.py` & `emobject-0.7.0b3/emobject/emexperiment.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b2/emobject/emimage.py` & `emobject-0.7.0b3/emobject/emimage.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b2/emobject/emlayer.py` & `emobject-0.7.0b3/emobject/emlayer.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b2/emobject/emobject.py` & `emobject-0.7.0b3/emobject/emobject.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b2/emobject/empublicaccess.py` & `emobject-0.7.0b3/emobject/empublicaccess.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b2/emobject/emroitools.py` & `emobject-0.7.0b3/emobject/emroitools.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b2/emobject/utils/graph.py` & `emobject-0.7.0b3/emobject/utils/graph.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b2/emobject/utils/helpers.py` & `emobject-0.7.0b3/emobject/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b2/emobject/utils/io.py` & `emobject-0.7.0b3/emobject/utils/io.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b2/emobject/utils/visualization.py` & `emobject-0.7.0b3/emobject/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b2/emobject.egg-info/PKG-INFO` & `emobject-0.7.0b3/emobject.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emobject
-Version: 0.7.0b2
+Version: 0.7.0b3
 Summary: data abstraction and libraries for spatial omics
 Home-page: https://gitlab.com/enable-medicine/rnd-subgroup/emobject/
 Author: Ethan A. G. Baker
 Author-email: ethan.baker@enablemedicine.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7, <4
```

### Comparing `emobject-0.7.0b2/emobject.egg-info/SOURCES.txt` & `emobject-0.7.0b3/emobject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b2/setup.py` & `emobject-0.7.0b3/setup.py`

 * *Files identical despite different names*

