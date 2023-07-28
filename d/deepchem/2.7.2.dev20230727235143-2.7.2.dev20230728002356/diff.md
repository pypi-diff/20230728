# Comparing `tmp/deepchem-2.7.2.dev20230727235143.tar.gz` & `tmp/deepchem-2.7.2.dev20230728002356.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepchem-2.7.2.dev20230727235143.tar", last modified: Thu Jul 27 23:51:44 2023, max compression
+gzip compressed data, was "deepchem-2.7.2.dev20230728002356.tar", last modified: Fri Jul 28 00:23:57 2023, max compression
```

## Comparing `deepchem-2.7.2.dev20230727235143.tar` & `deepchem-2.7.2.dev20230728002356.tar`

### file list

```diff
@@ -1,298 +1,298 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:44.153483 deepchem-2.7.2.dev20230727235143/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1047 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-27 23:51:44.153483 deepchem-2.7.2.dev20230727235143/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:44.113483 deepchem-2.7.2.dev20230727235143/deepchem/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:44.113483 deepchem-2.7.2.dev20230727235143/deepchem/data/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67994 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/data/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)   118009 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/data/pytorch_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/data/supports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:44.113483 deepchem-2.7.2.dev20230727235143/deepchem/dock/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/dock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/dock/binding_pocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/dock/docking.py
--rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/dock/pose_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/dock/pose_scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:44.117483 deepchem-2.7.2.dev20230727235143/deepchem/feat/
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/atomic_conformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19458 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/bert_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/binding_pocket_features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:44.117483 deepchem-2.7.2.dev20230727235143/deepchem/feat/complex_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/complex_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/complex_featurizers/contact_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/complex_featurizers/grid_featurizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/complex_featurizers/splif_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/dft_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    22111 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/graph_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    38890 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/graph_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/huggingface_featurizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:44.117483 deepchem-2.7.2.dev20230727235143/deepchem/feat/material_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/material_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/material_featurizers/cgcnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/material_featurizers/element_property_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/material_featurizers/elemnet_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    28058 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/material_featurizers/lcnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/material_featurizers/sine_coulomb_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    14808 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/mol_graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:44.121483 deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/atomic_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/circular_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/conformer_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/coulomb_matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/grover_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/mat_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/molgan_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/mordred_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/mxmnet_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/one_hot_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/raw_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9881 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/rdkit_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/smiles_to_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/smiles_to_seq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/snap_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/reaction_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/roberta_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:44.121483 deepchem-2.7.2.dev20230727235143/deepchem/feat/sequence_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/sequence_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/smiles_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:44.121483 deepchem-2.7.2.dev20230727235143/deepchem/feat/vocabulary_builders/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/vocabulary_builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18726 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/vocabulary_builders/grover_vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/vocabulary_builders/hf_vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/feat/vocabulary_builders/vocabulary_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:44.121483 deepchem-2.7.2.dev20230727235143/deepchem/hyper/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/hyper/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    17151 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/hyper/gaussian_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/hyper/grid_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/hyper/random_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:44.121483 deepchem-2.7.2.dev20230727235143/deepchem/metalearning/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/metalearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/metalearning/maml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:44.121483 deepchem-2.7.2.dev20230727235143/deepchem/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/metrics/genomic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    31620 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/metrics/score_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:44.125483 deepchem-2.7.2.dev20230727235143/deepchem/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/IRV.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/atomic_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/chemnet_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/chemnet_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:44.125483 deepchem-2.7.2.dev20230727235143/deepchem/models/dft/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/dft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/dft/dftxc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14020 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/dft/nnxc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/dft/scf.py
--rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/fcnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/gan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:44.125483 deepchem-2.7.2.dev20230727235143/deepchem/models/gbdt_models/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/gbdt_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/gbdt_models/gbdt_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    57408 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/graph_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:44.125483 deepchem-2.7.2.dev20230727235143/deepchem/models/jax_models/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/jax_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28179 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/jax_models/jax_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/jax_models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/jax_models/pinns_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    56522 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/keras_model.py
--rw-r--r--   0 runner    (1001) docker     (123)   144759 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:44.125483 deepchem-2.7.2.dev20230727235143/deepchem/models/lightning/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/lightning/dc_lightning_dataset_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/lightning/dc_lightning_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    61903 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/molgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/normalizing_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/progressive_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)    17830 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/robust_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/scscore.py
--rw-r--r--   0 runner    (1001) docker     (123)    25969 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/seqtoseq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:44.129483 deepchem-2.7.2.dev20230727235143/deepchem/models/sklearn_models/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/sklearn_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/sklearn_models/sklearn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/text_cnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:44.129483 deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/attentivefp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/cgcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/chemberta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/dmpnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/ferminet.py
--rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/gat.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/gcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    51159 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/gnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    24969 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/gnn3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    38126 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/grover.py
--rw-r--r--   0 runner    (1001) docker     (123)    38432 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/grover_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    22942 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/hf_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30077 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/infograph.py
--rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/kfac_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)   167672 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18575 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/lcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/mat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/megnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/modular.py
--rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/mpnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/normalizing_flows_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/pagtn.py
--rw-r--r--   0 runner    (1001) docker     (123)    23016 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/pna_gnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/readout.py
--rw-r--r--   0 runner    (1001) docker     (123)    52726 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/torch_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/models/wandblogger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:44.133483 deepchem-2.7.2.dev20230727235143/deepchem/molnet/
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/check_availability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/dnasim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:44.141483 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/bace_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/bace_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/bbbc_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/bbbp_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/cell_counting_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/chembl25_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/chembl_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/chembl_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/clearance_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/clintox_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/delaney_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/factors_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/freesolv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/hiv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/hopv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/hppb_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/kaggle_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)   165414 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/kaggle_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/kinase_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/lipo_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/load_dataset_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:44.145483 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/material_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/material_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/material_datasets/load_bandgap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/material_datasets/load_perovskite.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/molnet_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/muv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/nci_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/pcba_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/pdbbind_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/ppb_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/qm7_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/qm8_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/qm9_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/sampl_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/sider_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/sweetlead_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/thermosol_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/tox21_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    18900 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/toxcast_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/uspto_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/uv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/uv_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/zinc15_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/preset_hyper_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/run_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/run_benchmark_low_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    36564 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/molnet/run_benchmark_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:44.145483 deepchem-2.7.2.dev20230727235143/deepchem/rl/
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/rl/a2c.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:44.145483 deepchem-2.7.2.dev20230727235143/deepchem/rl/envs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/rl/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/rl/envs/test_tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/rl/envs/tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/rl/ppo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:44.145483 deepchem-2.7.2.dev20230727235143/deepchem/splits/
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/splits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63895 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/splits/splitters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/splits/task_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:44.145483 deepchem-2.7.2.dev20230727235143/deepchem/trans/
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/trans/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)    91191 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/trans/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:44.149483 deepchem-2.7.2.dev20230727235143/deepchem/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/conformers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/coordinate_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20923 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/debug_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/dftutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/docking_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/electron_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19454 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/fake_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/fragment_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/genomics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/grover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/molecule_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/noncovalent_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/pdbqt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/pytorch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    65672 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/sequence_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:44.153483 deepchem-2.7.2.dev20230727235143/deepchem/utils/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_coordinate_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_dftutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_docking_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_electron_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_fake_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_fragment_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_generator_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_genomics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_grover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_molecule_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_noncovalent_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_pdbqt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_pytorch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_updated_scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_voxel_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/vina_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-07-27 23:51:28.000000 deepchem-2.7.2.dev20230727235143/deepchem/utils/voxel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:51:44.113483 deepchem-2.7.2.dev20230727235143/deepchem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-27 23:51:44.000000 deepchem-2.7.2.dev20230727235143/deepchem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-07-27 23:51:44.000000 deepchem-2.7.2.dev20230727235143/deepchem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 23:51:44.000000 deepchem-2.7.2.dev20230727235143/deepchem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-27 23:51:44.000000 deepchem-2.7.2.dev20230727235143/deepchem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 23:51:44.000000 deepchem-2.7.2.dev20230727235143/deepchem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-27 23:51:44.153483 deepchem-2.7.2.dev20230727235143/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-27 23:51:29.000000 deepchem-2.7.2.dev20230727235143/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.175554 deepchem-2.7.2.dev20230728002356/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1047 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-28 00:23:57.175554 deepchem-2.7.2.dev20230728002356/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.151554 deepchem-2.7.2.dev20230728002356/deepchem/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.151554 deepchem-2.7.2.dev20230728002356/deepchem/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67994 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/data/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118009 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/data/pytorch_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/data/supports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.151554 deepchem-2.7.2.dev20230728002356/deepchem/dock/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/dock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/dock/binding_pocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/dock/docking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/dock/pose_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/dock/pose_scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.155554 deepchem-2.7.2.dev20230728002356/deepchem/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/atomic_conformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19458 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/bert_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/binding_pocket_features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.155554 deepchem-2.7.2.dev20230728002356/deepchem/feat/complex_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/complex_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/complex_featurizers/contact_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/complex_featurizers/grid_featurizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/complex_featurizers/splif_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/dft_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22111 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/graph_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38890 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/graph_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/huggingface_featurizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.155554 deepchem-2.7.2.dev20230728002356/deepchem/feat/material_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/material_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/material_featurizers/cgcnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/material_featurizers/element_property_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/material_featurizers/elemnet_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28058 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/material_featurizers/lcnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/material_featurizers/sine_coulomb_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14808 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/mol_graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.155554 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/atomic_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/circular_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/conformer_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/coulomb_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/grover_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/mat_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/molgan_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/mordred_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/mxmnet_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/one_hot_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/raw_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9881 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/rdkit_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/smiles_to_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/smiles_to_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/snap_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/reaction_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/roberta_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.159554 deepchem-2.7.2.dev20230728002356/deepchem/feat/sequence_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/sequence_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/smiles_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.159554 deepchem-2.7.2.dev20230728002356/deepchem/feat/vocabulary_builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/vocabulary_builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18726 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/vocabulary_builders/grover_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/vocabulary_builders/hf_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/feat/vocabulary_builders/vocabulary_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.159554 deepchem-2.7.2.dev20230728002356/deepchem/hyper/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/hyper/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17151 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/hyper/gaussian_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/hyper/grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/hyper/random_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.159554 deepchem-2.7.2.dev20230728002356/deepchem/metalearning/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/metalearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/metalearning/maml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.159554 deepchem-2.7.2.dev20230728002356/deepchem/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/metrics/genomic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31620 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/metrics/score_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.159554 deepchem-2.7.2.dev20230728002356/deepchem/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/IRV.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/atomic_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/chemnet_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/chemnet_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.163554 deepchem-2.7.2.dev20230728002356/deepchem/models/dft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/dft/dftxc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14020 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/dft/nnxc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/dft/scf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/fcnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/gan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.163554 deepchem-2.7.2.dev20230728002356/deepchem/models/gbdt_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/gbdt_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/gbdt_models/gbdt_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57408 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/graph_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.163554 deepchem-2.7.2.dev20230728002356/deepchem/models/jax_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/jax_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28179 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/jax_models/jax_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/jax_models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/jax_models/pinns_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56522 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/keras_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144759 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.163554 deepchem-2.7.2.dev20230728002356/deepchem/models/lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/lightning/dc_lightning_dataset_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/lightning/dc_lightning_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61903 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/molgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/normalizing_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/progressive_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17830 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/robust_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/scscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25969 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/seqtoseq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.163554 deepchem-2.7.2.dev20230728002356/deepchem/models/sklearn_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/sklearn_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/sklearn_models/sklearn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/text_cnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.167554 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/attentivefp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/cgcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/chemberta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/dmpnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/ferminet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/gat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/gcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51159 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/gnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24969 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/gnn3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38126 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38432 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/grover_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22942 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/hf_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30077 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/infograph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/kfac_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   172379 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18575 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/lcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/megnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/modular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/mpnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/normalizing_flows_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/pagtn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23016 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/pna_gnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52726 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/torch_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/models/wandblogger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.167554 deepchem-2.7.2.dev20230728002356/deepchem/molnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/check_availability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/dnasim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.171554 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/bace_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/bace_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/bbbc_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/bbbp_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/cell_counting_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/chembl25_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/chembl_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/chembl_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/clearance_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/clintox_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/delaney_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/factors_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/freesolv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/hiv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/hopv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/hppb_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/kaggle_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)   165414 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/kaggle_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/kinase_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/lipo_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/load_dataset_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.171554 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/material_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/material_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/material_datasets/load_bandgap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/material_datasets/load_perovskite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/molnet_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/muv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/nci_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/pcba_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/pdbbind_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/ppb_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/qm7_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/qm8_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/qm9_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/sampl_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/sider_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/sweetlead_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/thermosol_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/tox21_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18900 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/toxcast_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/uspto_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/uv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/uv_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/zinc15_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/preset_hyper_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/run_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/run_benchmark_low_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36564 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/molnet/run_benchmark_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.171554 deepchem-2.7.2.dev20230728002356/deepchem/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/rl/a2c.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.171554 deepchem-2.7.2.dev20230728002356/deepchem/rl/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/rl/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/rl/envs/test_tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/rl/envs/tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/rl/ppo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.171554 deepchem-2.7.2.dev20230728002356/deepchem/splits/
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/splits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63895 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/splits/splitters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/splits/task_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.171554 deepchem-2.7.2.dev20230728002356/deepchem/trans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/trans/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91191 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/trans/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.175554 deepchem-2.7.2.dev20230728002356/deepchem/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/conformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/coordinate_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20923 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/debug_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/dftutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/docking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/electron_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19454 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/fake_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/fragment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/genomics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/molecule_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/noncovalent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/pdbqt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/pytorch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65672 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/sequence_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.175554 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_coordinate_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_dftutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_docking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_electron_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_fake_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_fragment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_generator_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_genomics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_molecule_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_noncovalent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_pdbqt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_pytorch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_updated_scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_voxel_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/vina_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/deepchem/utils/voxel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:57.151554 deepchem-2.7.2.dev20230728002356/deepchem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-28 00:23:57.000000 deepchem-2.7.2.dev20230728002356/deepchem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-07-28 00:23:57.000000 deepchem-2.7.2.dev20230728002356/deepchem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 00:23:57.000000 deepchem-2.7.2.dev20230728002356/deepchem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-28 00:23:57.000000 deepchem-2.7.2.dev20230728002356/deepchem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-28 00:23:57.000000 deepchem-2.7.2.dev20230728002356/deepchem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-28 00:23:57.175554 deepchem-2.7.2.dev20230728002356/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-28 00:23:40.000000 deepchem-2.7.2.dev20230728002356/setup.py
```

### Comparing `deepchem-2.7.2.dev20230727235143/LICENSE` & `deepchem-2.7.2.dev20230728002356/LICENSE`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/PKG-INFO` & `deepchem-2.7.2.dev20230728002356/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepchem
-Version: 2.7.2.dev20230727235143
+Version: 2.7.2.dev20230728002356
 Summary: Deep learning models for drug discovery,         quantum chemistry, and the life sciences.
 Home-page: https://github.com/deepchem/deepchem
 Maintainer: DeepChem contributors
 License: MIT
 Project-URL: Documentation, https://deepchem.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/deepchem/deepchem
 Keywords: deepchem,chemistry,biology,materials-science,life-science,drug-discovery
```

### Comparing `deepchem-2.7.2.dev20230727235143/README.md` & `deepchem-2.7.2.dev20230728002356/README.md`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/data/__init__.py` & `deepchem-2.7.2.dev20230728002356/deepchem/data/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/data/data_loader.py` & `deepchem-2.7.2.dev20230728002356/deepchem/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/data/datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/data/datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/data/pytorch_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/data/pytorch_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/data/supports.py` & `deepchem-2.7.2.dev20230728002356/deepchem/data/supports.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/dock/binding_pocket.py` & `deepchem-2.7.2.dev20230728002356/deepchem/dock/binding_pocket.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/dock/docking.py` & `deepchem-2.7.2.dev20230728002356/deepchem/dock/docking.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/dock/pose_generation.py` & `deepchem-2.7.2.dev20230728002356/deepchem/dock/pose_generation.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/dock/pose_scoring.py` & `deepchem-2.7.2.dev20230728002356/deepchem/dock/pose_scoring.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/__init__.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/atomic_conformation.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/atomic_conformation.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/base_classes.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/base_classes.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/bert_tokenizer.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/binding_pocket_features.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/binding_pocket_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/complex_featurizers/__init__.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/complex_featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/complex_featurizers/contact_fingerprints.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/complex_featurizers/contact_fingerprints.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/complex_featurizers/grid_featurizers.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/complex_featurizers/grid_featurizers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/complex_featurizers/splif_fingerprints.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/complex_featurizers/splif_fingerprints.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/dft_data.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/dft_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/graph_data.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/graph_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/graph_features.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/graph_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/huggingface_featurizer.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/huggingface_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/material_featurizers/cgcnn_featurizer.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/material_featurizers/cgcnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/material_featurizers/element_property_fingerprint.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/material_featurizers/element_property_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/material_featurizers/elemnet_featurizer.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/material_featurizers/elemnet_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/material_featurizers/lcnn_featurizer.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/material_featurizers/lcnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/material_featurizers/sine_coulomb_matrix.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/material_featurizers/sine_coulomb_matrix.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/mol_graphs.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/mol_graphs.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/__init__.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/atomic_coordinates.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/atomic_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/circular_fingerprint.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/circular_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/conformer_featurizer.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/conformer_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/coulomb_matrices.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/coulomb_matrices.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/grover_featurizer.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/grover_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/mat_featurizer.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/mat_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/molgan_featurizer.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/molgan_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/mordred_descriptors.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/mordred_descriptors.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/mxmnet_featurizer.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/mxmnet_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/one_hot_featurizer.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/one_hot_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/raw_featurizer.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/raw_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/rdkit_descriptors.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/rdkit_descriptors.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/smiles_to_image.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/smiles_to_image.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/smiles_to_seq.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/smiles_to_seq.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/snap_featurizer.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/snap_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/reaction_featurizer.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/reaction_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/roberta_tokenizer.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/roberta_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/smiles_tokenizer.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/smiles_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/vocabulary_builders/grover_vocab.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/vocabulary_builders/grover_vocab.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/vocabulary_builders/hf_vocab.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/vocabulary_builders/hf_vocab.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/feat/vocabulary_builders/vocabulary_builder.py` & `deepchem-2.7.2.dev20230728002356/deepchem/feat/vocabulary_builders/vocabulary_builder.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/hyper/base_classes.py` & `deepchem-2.7.2.dev20230728002356/deepchem/hyper/base_classes.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/hyper/gaussian_process.py` & `deepchem-2.7.2.dev20230728002356/deepchem/hyper/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/hyper/grid_search.py` & `deepchem-2.7.2.dev20230728002356/deepchem/hyper/grid_search.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/hyper/random_search.py` & `deepchem-2.7.2.dev20230728002356/deepchem/hyper/random_search.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/metalearning/maml.py` & `deepchem-2.7.2.dev20230728002356/deepchem/metalearning/maml.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/metrics/__init__.py` & `deepchem-2.7.2.dev20230728002356/deepchem/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/metrics/genomic_metrics.py` & `deepchem-2.7.2.dev20230728002356/deepchem/metrics/genomic_metrics.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/metrics/metric.py` & `deepchem-2.7.2.dev20230728002356/deepchem/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/metrics/score_function.py` & `deepchem-2.7.2.dev20230728002356/deepchem/metrics/score_function.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/IRV.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/IRV.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/__init__.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/atomic_conv.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/atomic_conv.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/callbacks.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/callbacks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/chemnet_layers.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/chemnet_layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/chemnet_models.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/chemnet_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/dft/dftxc.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/dft/dftxc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/dft/nnxc.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/dft/nnxc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/dft/scf.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/dft/scf.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/fcnet.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/fcnet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/gan.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/gan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/gbdt_models/gbdt_model.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/gbdt_models/gbdt_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/graph_models.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/graph_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/jax_models/jax_model.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/jax_models/jax_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/jax_models/layers.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/jax_models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/jax_models/pinns_model.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/jax_models/pinns_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/keras_model.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/keras_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/layers.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/lightning/dc_lightning_dataset_module.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/lightning/dc_lightning_dataset_module.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/lightning/dc_lightning_module.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/lightning/dc_lightning_module.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/losses.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/losses.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/models.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/molgan.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/molgan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/multitask.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/normalizing_flows.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/normalizing_flows.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/optimizers.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/optimizers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/progressive_multitask.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/progressive_multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/robust_multitask.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/robust_multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/scscore.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/scscore.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/seqtoseq.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/seqtoseq.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/sklearn_models/sklearn_model.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/sklearn_models/sklearn_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/text_cnn.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/text_cnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/__init__.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from deepchem.models.torch_models.infograph import InfoGraphStar, InfoGraphStarModel, InfoGraphEncoder, GINEncoder, InfoGraph, InfoGraphModel, InfoGraphEncoder
 from deepchem.models.torch_models.mpnn import MPNN, MPNNModel
 from deepchem.models.torch_models.lcnn import LCNN, LCNNModel
 from deepchem.models.torch_models.pagtn import Pagtn, PagtnModel
 from deepchem.models.torch_models.mat import MAT, MATModel
 from deepchem.models.torch_models.megnet import MEGNetModel
 from deepchem.models.torch_models.normalizing_flows_pytorch import NormalizingFlow
-from deepchem.models.torch_models.layers import MultilayerPerceptron, CNNModule, CombineMeanStd, WeightedLinearCombo, AtomicConvolution, NeighborList, SetGather, EdgeNetwork, WeaveLayer, WeaveGather, MolGANConvolutionLayer, MolGANAggregationLayer, MolGANMultiConvolutionLayer
+from deepchem.models.torch_models.layers import MultilayerPerceptron, CNNModule, CombineMeanStd, WeightedLinearCombo, AtomicConvolution, NeighborList, SetGather, EdgeNetwork, WeaveLayer, WeaveGather, MolGANConvolutionLayer, MolGANAggregationLayer, MolGANMultiConvolutionLayer, MolGANEncoderLayer
 from deepchem.models.torch_models.cnn import CNN
 from deepchem.models.torch_models.attention import ScaledDotProductAttention, SelfAttention
 from deepchem.models.torch_models.grover import GroverModel, GroverPretrain, GroverFinetune
 from deepchem.models.torch_models.readout import GroverReadout
 try:
     from deepchem.models.torch_models.dmpnn import DMPNN, DMPNNModel
     from deepchem.models.torch_models.gnn import GNN, GNNHead, GNNModular
```

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/attention.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/attention.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/attentivefp.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/attentivefp.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/cgcnn.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/cgcnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/chemberta.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/chemberta.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/cnn.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/cnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/dmpnn.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/dmpnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/ferminet.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/ferminet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/gat.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/gat.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/gcn.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/gcn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/gnn.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/gnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/gnn3d.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/gnn3d.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/grover.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/grover_layers.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/grover_layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/hf_models.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/hf_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/infograph.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/infograph.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/kfac_optimizer.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/kfac_optimizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/layers.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -7846,2635 +7846,2929 @@
 0001ea50: 2020 2020 2020 2020 2020 6163 7469 7661            activa
 0001ea60: 7469 6f6e 3d74 6f72 6368 2e74 616e 682c  tion=torch.tanh,
 0001ea70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0001ea80: 2020 6472 6f70 6f75 745f 7261 7465 3a20    dropout_rate: 
 0001ea90: 666c 6f61 7420 3d20 302e 302c 0a20 2020  float = 0.0,.   
 0001eaa0: 2020 2020 2020 2020 2020 2020 2020 6e61                na
 0001eab0: 6d65 3a20 7374 7220 3d20 2222 2c0a 2020  me: str = "",.  
-0001eac0: 2020 2020 2020 2020 2020 2020 2020 202a                 *
-0001ead0: 2a6b 7761 7267 7329 3a0a 2020 2020 2020  *kwargs):.      
-0001eae0: 2020 2222 220a 2020 2020 2020 2020 496e    """.        In
-0001eaf0: 6974 6961 6c69 7a65 2074 6865 206c 6179  itialize the lay
-0001eb00: 6572 0a0a 2020 2020 2020 2020 5061 7261  er..        Para
-0001eb10: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-0001eb20: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-0001eb30: 2075 6e69 7473 3a20 696e 742c 206f 7074   units: int, opt
-0001eb40: 696f 6e61 6c20 2864 6566 6175 6c74 3d31  ional (default=1
-0001eb50: 3238 290a 2020 2020 2020 2020 2020 2020  28).            
-0001eb60: 4469 6d65 7369 6f6e 206f 6620 6465 6e73  Dimesion of dens
-0001eb70: 6520 6c61 7965 7273 2075 7365 6420 666f  e layers used fo
-0001eb80: 7220 6167 6772 6567 6174 696f 6e0a 2020  r aggregation.  
-0001eb90: 2020 2020 2020 6163 7469 7661 7469 6f6e        activation
-0001eba0: 3a20 6675 6e63 7469 6f6e 2c20 6f70 7469  : function, opti
-0001ebb0: 6f6e 616c 2028 6465 6661 756c 743d 5461  onal (default=Ta
-0001ebc0: 6e68 290a 2020 2020 2020 2020 2020 2020  nh).            
-0001ebd0: 6163 7469 7661 7469 6f6e 2066 756e 6374  activation funct
-0001ebe0: 696f 6e20 7573 6564 2061 6372 6f73 7320  ion used across 
-0001ebf0: 6d6f 6465 6c2c 2064 6566 6175 6c74 2069  model, default i
-0001ec00: 7320 5461 6e68 0a20 2020 2020 2020 2064  s Tanh.        d
-0001ec10: 726f 706f 7574 5f72 6174 653a 2066 6c6f  ropout_rate: flo
-0001ec20: 6174 2c20 6f70 7469 6f6e 616c 2028 6465  at, optional (de
-0001ec30: 6661 756c 743d 302e 3029 0a20 2020 2020  fault=0.0).     
-0001ec40: 2020 2020 2020 2055 7365 6420 6279 2064         Used by d
-0001ec50: 726f 706f 7574 206c 6179 6572 0a20 2020  ropout layer.   
-0001ec60: 2020 2020 206e 616d 653a 2073 7472 696e       name: strin
-0001ec70: 672c 206f 7074 696f 6e61 6c20 2864 6566  g, optional (def
-0001ec80: 6175 6c74 3d22 2229 0a20 2020 2020 2020  ault="").       
-0001ec90: 2020 2020 204e 616d 6520 6f66 2074 6865       Name of the
-0001eca0: 206c 6179 6572 0a20 2020 2020 2020 2022   layer.        "
-0001ecb0: 2222 0a0a 2020 2020 2020 2020 7375 7065  ""..        supe
-0001ecc0: 7228 4d6f 6c47 414e 4167 6772 6567 6174  r(MolGANAggregat
-0001ecd0: 696f 6e4c 6179 6572 2c20 7365 6c66 292e  ionLayer, self).
-0001ece0: 5f5f 696e 6974 5f5f 2829 0a20 2020 2020  __init__().     
-0001ecf0: 2020 2073 656c 662e 756e 6974 733a 2069     self.units: i
-0001ed00: 6e74 203d 2075 6e69 7473 0a20 2020 2020  nt = units.     
-0001ed10: 2020 2073 656c 662e 6163 7469 7661 7469     self.activati
-0001ed20: 6f6e 203d 2061 6374 6976 6174 696f 6e0a  on = activation.
-0001ed30: 2020 2020 2020 2020 7365 6c66 2e64 726f          self.dro
-0001ed40: 706f 7574 5f72 6174 653a 2066 6c6f 6174  pout_rate: float
-0001ed50: 203d 2064 726f 706f 7574 5f72 6174 650a   = dropout_rate.
-0001ed60: 2020 2020 2020 2020 7365 6c66 2e6e 616d          self.nam
-0001ed70: 653a 2073 7472 203d 206e 616d 650a 0a20  e: str = name.. 
-0001ed80: 2020 2020 2020 2073 656c 662e 6431 203d         self.d1 =
-0001ed90: 206e 6e2e 4c69 6e65 6172 2873 656c 662e   nn.Linear(self.
-0001eda0: 756e 6974 732c 2073 656c 662e 756e 6974  units, self.unit
-0001edb0: 7329 0a20 2020 2020 2020 2073 656c 662e  s).        self.
-0001edc0: 6432 203d 206e 6e2e 4c69 6e65 6172 2873  d2 = nn.Linear(s
-0001edd0: 656c 662e 756e 6974 732c 2073 656c 662e  elf.units, self.
-0001ede0: 756e 6974 7329 0a20 2020 2020 2020 2073  units).        s
-0001edf0: 656c 662e 6472 6f70 6f75 745f 6c61 7965  elf.dropout_laye
-0001ee00: 7220 3d20 6e6e 2e44 726f 706f 7574 2864  r = nn.Dropout(d
-0001ee10: 726f 706f 7574 5f72 6174 6529 0a0a 2020  ropout_rate)..  
-0001ee20: 2020 6465 6620 5f5f 7265 7072 5f5f 2873    def __repr__(s
-0001ee30: 656c 6629 202d 3e20 7374 723a 0a20 2020  elf) -> str:.   
-0001ee40: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0001ee50: 2053 7472 696e 6720 7265 7072 6573 656e   String represen
-0001ee60: 7461 7469 6f6e 206f 6620 7468 6520 6c61  tation of the la
-0001ee70: 7965 720a 2020 2020 2020 2020 0a20 2020  yer.        .   
-0001ee80: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
-0001ee90: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
-0001eea0: 2020 2020 2073 7472 696e 670a 2020 2020       string.    
-0001eeb0: 2020 2020 2020 2020 5374 7269 6e67 2072          String r
-0001eec0: 6570 7265 7365 6e74 6174 696f 6e20 6f66  epresentation of
-0001eed0: 2074 6865 206c 6179 6572 2020 2020 0a20   the layer    . 
-0001eee0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0001eef0: 2020 2072 6574 7572 6e20 6622 7b73 656c     return f"{sel
-0001ef00: 662e 5f5f 636c 6173 735f 5f2e 5f5f 6e61  f.__class__.__na
-0001ef10: 6d65 5f5f 7d28 756e 6974 733d 7b73 656c  me__}(units={sel
-0001ef20: 662e 756e 6974 737d 2c20 6163 7469 7661  f.units}, activa
-0001ef30: 7469 6f6e 3d7b 7365 6c66 2e61 6374 6976  tion={self.activ
-0001ef40: 6174 696f 6e7d 2c20 6472 6f70 6f75 745f  ation}, dropout_
-0001ef50: 7261 7465 3d7b 7365 6c66 2e64 726f 706f  rate={self.dropo
-0001ef60: 7574 5f72 6174 657d 2922 0a0a 2020 2020  ut_rate})"..    
-0001ef70: 6465 6620 666f 7277 6172 6428 7365 6c66  def forward(self
-0001ef80: 2c20 696e 7075 7473 3a20 4c69 7374 2920  , inputs: List) 
-0001ef90: 2d3e 2074 6f72 6368 2e54 656e 736f 723a  -> torch.Tensor:
-0001efa0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0001efb0: 2020 2020 2049 6e76 6f6b 6520 7468 6973       Invoke this
-0001efc0: 206c 6179 6572 0a0a 2020 2020 2020 2020   layer..        
-0001efd0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-0001efe0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-0001eff0: 2020 2020 2020 696e 7075 7473 3a20 4c69        inputs: Li
-0001f000: 7374 0a20 2020 2020 2020 2020 2020 2053  st.            S
-0001f010: 696e 676c 6520 7465 6e73 6f72 2072 6573  ingle tensor res
-0001f020: 756c 7469 6e67 2066 726f 6d20 6772 6170  ulting from grap
-0001f030: 6820 636f 6e76 6f6c 7574 696f 6e20 6c61  h convolution la
-0001f040: 7965 720a 0a20 2020 2020 2020 2052 6574  yer..        Ret
-0001f050: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-0001f060: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6167  -----.        ag
-0001f070: 6772 6567 6174 696f 6e20 7465 6e73 6f72  gregation tensor
-0001f080: 3a20 746f 7263 682e 5465 6e73 6f72 0a20  : torch.Tensor. 
-0001f090: 2020 2020 2020 2020 2052 6573 756c 7420           Result 
-0001f0a0: 6f66 2061 6767 7265 6761 7469 6f6e 2066  of aggregation f
-0001f0b0: 756e 6374 696f 6e20 6f6e 2069 6e70 7574  unction on input
-0001f0c0: 2063 6f6e 766f 6c75 7469 6f6e 2074 656e   convolution ten
-0001f0d0: 736f 722e 0a20 2020 2020 2020 2022 2222  sor..        """
-0001f0e0: 0a0a 2020 2020 2020 2020 6920 3d20 746f  ..        i = to
-0001f0f0: 7263 682e 7369 676d 6f69 6428 7365 6c66  rch.sigmoid(self
-0001f100: 2e64 3128 696e 7075 7473 2929 0a20 2020  .d1(inputs)).   
-0001f110: 2020 2020 206a 203d 2073 656c 662e 6163       j = self.ac
-0001f120: 7469 7661 7469 6f6e 2873 656c 662e 6432  tivation(self.d2
-0001f130: 2869 6e70 7574 7329 290a 2020 2020 2020  (inputs)).      
-0001f140: 2020 6f75 7470 7574 203d 2074 6f72 6368    output = torch
-0001f150: 2e73 756d 2869 202a 206a 2c20 6469 6d3d  .sum(i * j, dim=
-0001f160: 3129 0a20 2020 2020 2020 206f 7574 7075  1).        outpu
-0001f170: 7420 3d20 7365 6c66 2e61 6374 6976 6174  t = self.activat
-0001f180: 696f 6e28 6f75 7470 7574 290a 2020 2020  ion(output).    
-0001f190: 2020 2020 6f75 7470 7574 203d 2073 656c      output = sel
-0001f1a0: 662e 6472 6f70 6f75 745f 6c61 7965 7228  f.dropout_layer(
-0001f1b0: 6f75 7470 7574 290a 2020 2020 2020 2020  output).        
-0001f1c0: 7265 7475 726e 206f 7574 7075 740a 0a0a  return output...
-0001f1d0: 636c 6173 7320 4d6f 6c47 414e 4d75 6c74  class MolGANMult
-0001f1e0: 6943 6f6e 766f 6c75 7469 6f6e 4c61 7965  iConvolutionLaye
-0001f1f0: 7228 6e6e 2e4d 6f64 756c 6529 3a0a 2020  r(nn.Module):.  
-0001f200: 2020 2222 220a 2020 2020 4d75 6c74 6970    """.    Multip
-0001f210: 6c65 2070 6173 7320 636f 6e76 6f6c 7574  le pass convolut
-0001f220: 696f 6e20 6c61 7965 7220 7573 6564 2069  ion layer used i
-0001f230: 6e20 4d6f 6c47 414e 206d 6f64 656c 2e0a  n MolGAN model..
-0001f240: 2020 2020 4d6f 6c47 414e 2069 7320 6120      MolGAN is a 
-0001f250: 5747 414e 2074 7970 6520 6d6f 6465 6c20  WGAN type model 
-0001f260: 666f 7220 6765 6e65 7261 7469 6f6e 206f  for generation o
-0001f270: 6620 736d 616c 6c20 6d6f 6c65 6375 6c65  f small molecule
-0001f280: 732e 0a20 2020 2049 7420 7461 6b65 7320  s..    It takes 
-0001f290: 6f75 7470 7574 7320 6f66 2070 7265 7669  outputs of previ
-0001f2a0: 6f75 7320 636f 6e76 6f6c 7574 696f 6e20  ous convolution 
-0001f2b0: 6c61 7965 7220 616e 6420 7573 6573 0a20  layer and uses. 
-0001f2c0: 2020 2074 6865 6d20 6173 2069 6e70 7574     them as input
-0001f2d0: 7320 666f 7220 7468 6520 6e65 7874 206f  s for the next o
-0001f2e0: 6e65 2e0a 2020 2020 4974 2073 696d 706c  ne..    It simpl
-0001f2f0: 6966 6965 7320 7468 6520 6f76 6572 616c  ifies the overal
-0001f300: 6c20 6672 616d 6577 6f72 6b2c 2062 7574  l framework, but
-0001f310: 206d 6967 6874 2062 6520 6d6f 7665 6420   might be moved 
-0001f320: 746f 0a20 2020 204d 6f6c 4741 4e45 6e63  to.    MolGANEnc
-0001f330: 6f64 6572 4c61 7965 7220 696e 2074 6865  oderLayer in the
-0001f340: 2066 7574 7572 6520 696e 206f 7264 6572   future in order
-0001f350: 2074 6f20 7265 6475 6365 206e 756d 6265   to reduce numbe
-0001f360: 7220 6f66 206c 6179 6572 732e 0a0a 2020  r of layers...  
-0001f370: 2020 4578 616d 706c 650a 2020 2020 2d2d    Example.    --
-0001f380: 2d2d 2d2d 2d0a 2020 2020 3e3e 3e20 696d  -----.    >>> im
-0001f390: 706f 7274 2074 6f72 6368 0a20 2020 203e  port torch.    >
-0001f3a0: 3e3e 2069 6d70 6f72 7420 746f 7263 682e  >> import torch.
-0001f3b0: 6e6e 2061 7320 6e6e 0a20 2020 203e 3e3e  nn as nn.    >>>
-0001f3c0: 2069 6d70 6f72 7420 746f 7263 682e 6e6e   import torch.nn
-0001f3d0: 2e66 756e 6374 696f 6e61 6c20 6173 2046  .functional as F
-0001f3e0: 0a20 2020 203e 3e3e 2076 6572 7469 6365  .    >>> vertice
-0001f3f0: 7320 3d20 390a 2020 2020 3e3e 3e20 6e6f  s = 9.    >>> no
-0001f400: 6465 7320 3d20 350a 2020 2020 3e3e 3e20  des = 5.    >>> 
-0001f410: 6564 6765 7320 3d20 350a 2020 2020 3e3e  edges = 5.    >>
-0001f420: 3e20 756e 6974 7320 3d20 2831 3238 2c36  > units = (128,6
-0001f430: 3429 0a0a 2020 2020 3e3e 3e20 6c61 7965  4)..    >>> laye
-0001f440: 725f 3120 3d20 4d6f 6c47 414e 4d75 6c74  r_1 = MolGANMult
-0001f450: 6943 6f6e 766f 6c75 7469 6f6e 4c61 7965  iConvolutionLaye
-0001f460: 7228 756e 6974 733d 756e 6974 732c 206e  r(units=units, n
-0001f470: 6f64 6573 3d6e 6f64 6573 2c20 6564 6765  odes=nodes, edge
-0001f480: 733d 6564 6765 732c 206e 616d 653d 276c  s=edges, name='l
-0001f490: 6179 6572 3127 290a 2020 2020 3e3e 3e20  ayer1').    >>> 
-0001f4a0: 6164 6a61 6365 6e63 795f 7465 6e73 6f72  adjacency_tensor
-0001f4b0: 203d 2074 6f72 6368 2e72 616e 646e 2828   = torch.randn((
-0001f4c0: 312c 2076 6572 7469 6365 732c 2076 6572  1, vertices, ver
-0001f4d0: 7469 6365 732c 2065 6467 6573 2929 0a20  tices, edges)). 
-0001f4e0: 2020 203e 3e3e 206e 6f64 655f 7465 6e73     >>> node_tens
-0001f4f0: 6f72 203d 2074 6f72 6368 2e72 616e 646e  or = torch.randn
-0001f500: 2828 312c 2076 6572 7469 6365 732c 206e  ((1, vertices, n
-0001f510: 6f64 6573 2929 0a20 2020 203e 3e3e 206f  odes)).    >>> o
-0001f520: 7574 7075 7420 3d20 6c61 7965 725f 3128  utput = layer_1(
-0001f530: 5b61 646a 6163 656e 6379 5f74 656e 736f  [adjacency_tenso
-0001f540: 722c 206e 6f64 655f 7465 6e73 6f72 5d29  r, node_tensor])
-0001f550: 0a0a 2020 2020 5265 6665 7265 6e63 6573  ..    References
-0001f560: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
-0001f570: 2020 2020 2e2e 205b 315d 204e 6963 6f6c      .. [1] Nicol
-0001f580: 6120 4465 2043 616f 2065 7420 616c 2e20  a De Cao et al. 
-0001f590: 224d 6f6c 4741 4e3a 2041 6e20 696d 706c  "MolGAN: An impl
-0001f5a0: 6963 6974 2067 656e 6572 6174 6976 6520  icit generative 
-0001f5b0: 6d6f 6465 6c0a 2020 2020 2020 2020 666f  model.        fo
-0001f5c0: 7220 736d 616c 6c20 6d6f 6c65 6375 6c61  r small molecula
-0001f5d0: 7220 6772 6170 6873 222c 2068 7474 7073  r graphs", https
-0001f5e0: 3a2f 2f61 7278 6976 2e6f 7267 2f61 6273  ://arxiv.org/abs
-0001f5f0: 2f31 3830 352e 3131 3937 330a 2020 2020  /1805.11973.    
-0001f600: 2222 220a 0a20 2020 2064 6566 205f 5f69  """..    def __i
-0001f610: 6e69 745f 5f28 7365 6c66 2c0a 2020 2020  nit__(self,.    
-0001f620: 2020 2020 2020 2020 2020 2020 2075 6e69               uni
-0001f630: 7473 3a20 5475 706c 6520 3d20 2831 3238  ts: Tuple = (128
-0001f640: 2c20 3634 292c 0a20 2020 2020 2020 2020  , 64),.         
-0001f650: 2020 2020 2020 2020 6e6f 6465 733a 2069          nodes: i
-0001f660: 6e74 203d 2035 2c0a 2020 2020 2020 2020  nt = 5,.        
-0001f670: 2020 2020 2020 2020 2061 6374 6976 6174           activat
-0001f680: 696f 6e3d 746f 7263 682e 7461 6e68 2c0a  ion=torch.tanh,.
-0001f690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f6a0: 2064 726f 706f 7574 5f72 6174 653a 2066   dropout_rate: f
-0001f6b0: 6c6f 6174 203d 2030 2e30 2c0a 2020 2020  loat = 0.0,.    
-0001f6c0: 2020 2020 2020 2020 2020 2020 2065 6467               edg
-0001f6d0: 6573 3a20 696e 7420 3d20 352c 0a20 2020  es: int = 5,.   
-0001f6e0: 2020 2020 2020 2020 2020 2020 2020 6e61                na
-0001f6f0: 6d65 3a20 7374 7220 3d20 2222 2c0a 2020  me: str = "",.  
-0001f700: 2020 2020 2020 2020 2020 2020 2020 202a                 *
-0001f710: 2a6b 7761 7267 7329 3a0a 2020 2020 2020  *kwargs):.      
-0001f720: 2020 2222 220a 2020 2020 2020 2020 496e    """.        In
-0001f730: 6974 6961 6c69 7a65 2074 6865 206c 6179  itialize the lay
-0001f740: 6572 0a0a 2020 2020 2020 2020 5061 7261  er..        Para
-0001f750: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-0001f760: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-0001f770: 2075 6e69 7473 3a20 5475 706c 652c 206f   units: Tuple, o
-0001f780: 7074 696f 6e61 6c20 2864 6566 6175 6c74  ptional (default
-0001f790: 3d28 3132 382c 3634 2929 2c20 6d69 6e5f  =(128,64)), min_
-0001f7a0: 6c65 6e67 7468 3d32 0a20 2020 2020 2020  length=2.       
-0001f7b0: 2020 2020 2069 7374 206f 6620 6469 6d65       ist of dime
-0001f7c0: 6e73 696f 6e73 2075 7365 6420 6279 2063  nsions used by c
-0001f7d0: 6f6e 7365 6375 7469 7665 2063 6f6e 766f  onsecutive convo
-0001f7e0: 6c75 7469 6f6e 206c 6179 6572 732e 0a20  lution layers.. 
-0001f7f0: 2020 2020 2020 2020 2020 2054 6865 206d             The m
-0001f800: 6f72 6520 7661 6c75 6573 2074 6865 206d  ore values the m
-0001f810: 6f72 6520 636f 6e76 6f6c 7574 696f 6e20  ore convolution 
-0001f820: 6c61 7965 7273 2069 6e76 6f6b 6564 2e0a  layers invoked..
-0001f830: 2020 2020 2020 2020 6e6f 6465 733a 2069          nodes: i
-0001f840: 6e74 2c20 6f70 7469 6f6e 616c 2028 6465  nt, optional (de
-0001f850: 6661 756c 743d 3529 0a20 2020 2020 2020  fault=5).       
-0001f860: 2020 2020 204e 756d 6265 7220 6f66 2066       Number of f
-0001f870: 6561 7475 7265 7320 696e 206e 6f64 6520  eatures in node 
-0001f880: 7465 6e73 6f72 0a20 2020 2020 2020 2061  tensor.        a
-0001f890: 6374 6976 6174 696f 6e3a 2066 756e 6374  ctivation: funct
-0001f8a0: 696f 6e2c 206f 7074 696f 6e61 6c20 2864  ion, optional (d
-0001f8b0: 6566 6175 6c74 3d54 616e 6829 0a20 2020  efault=Tanh).   
-0001f8c0: 2020 2020 2020 2020 2061 6374 6976 6174           activat
-0001f8d0: 696f 6e20 6675 6e63 7469 6f6e 2075 7365  ion function use
-0001f8e0: 6420 6163 726f 7373 206d 6f64 656c 2c20  d across model, 
-0001f8f0: 6465 6661 756c 7420 6973 2054 616e 680a  default is Tanh.
-0001f900: 2020 2020 2020 2020 6472 6f70 6f75 745f          dropout_
-0001f910: 7261 7465 3a20 666c 6f61 742c 206f 7074  rate: float, opt
-0001f920: 696f 6e61 6c20 2864 6566 6175 6c74 3d30  ional (default=0
-0001f930: 2e30 290a 2020 2020 2020 2020 2020 2020  .0).            
-0001f940: 5573 6564 2062 7920 6472 6f70 6f75 7420  Used by dropout 
-0001f950: 6c61 7965 720a 2020 2020 2020 2020 6564  layer.        ed
-0001f960: 6765 733a 2069 6e74 2c20 6f70 7469 6f6e  ges: int, option
-0001f970: 616c 2028 6465 6661 756c 743d 3529 0a20  al (default=5). 
-0001f980: 2020 2020 2020 2020 2020 2043 6f6e 7472             Contr
-0001f990: 6f6c 7320 686f 7720 6d61 6e79 2064 656e  ols how many den
-0001f9a0: 7365 206c 6179 6572 7320 7573 6520 666f  se layers use fo
-0001f9b0: 7220 7369 6e67 6c65 2063 6f6e 766f 6c75  r single convolu
-0001f9c0: 7469 6f6e 2075 6e69 742e 0a20 2020 2020  tion unit..     
-0001f9d0: 2020 2020 2020 2054 7970 6963 616c 6c79         Typically
-0001f9e0: 206d 6174 6368 6573 206e 756d 6265 7220   matches number 
-0001f9f0: 6f66 2062 6f6e 6420 7479 7065 7320 7573  of bond types us
-0001fa00: 6564 2069 6e20 7468 6520 6d6f 6c65 6375  ed in the molecu
-0001fa10: 6c65 2e0a 2020 2020 2020 2020 6e61 6d65  le..        name
-0001fa20: 3a20 7374 7269 6e67 2c20 6f70 7469 6f6e  : string, option
-0001fa30: 616c 2028 6465 6661 756c 743d 2222 290a  al (default="").
-0001fa40: 2020 2020 2020 2020 2020 2020 4e61 6d65              Name
-0001fa50: 206f 6620 7468 6520 6c61 7965 720a 2020   of the layer.  
-0001fa60: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-0001fa70: 2020 2073 7570 6572 284d 6f6c 4741 4e4d     super(MolGANM
-0001fa80: 756c 7469 436f 6e76 6f6c 7574 696f 6e4c  ultiConvolutionL
-0001fa90: 6179 6572 2c20 7365 6c66 292e 5f5f 696e  ayer, self).__in
-0001faa0: 6974 5f5f 2829 0a20 2020 2020 2020 2069  it__().        i
-0001fab0: 6620 6c65 6e28 756e 6974 7329 203c 2032  f len(units) < 2
-0001fac0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-0001fad0: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
-0001fae0: 756e 6974 7320 7061 7261 6d65 7465 7220  units parameter 
-0001faf0: 6d75 7374 2063 6f6e 7461 696e 2061 7420  must contain at 
-0001fb00: 6c65 6173 7420 7477 6f20 7661 6c75 6573  least two values
-0001fb10: 2229 0a0a 2020 2020 2020 2020 7365 6c66  ")..        self
-0001fb20: 2e6e 6f64 6573 3a20 696e 7420 3d20 6e6f  .nodes: int = no
-0001fb30: 6465 730a 2020 2020 2020 2020 7365 6c66  des.        self
-0001fb40: 2e75 6e69 7473 3a20 5475 706c 6520 3d20  .units: Tuple = 
-0001fb50: 756e 6974 730a 2020 2020 2020 2020 7365  units.        se
-0001fb60: 6c66 2e61 6374 6976 6174 696f 6e20 3d20  lf.activation = 
-0001fb70: 6163 7469 7661 7469 6f6e 0a20 2020 2020  activation.     
-0001fb80: 2020 2073 656c 662e 6472 6f70 6f75 745f     self.dropout_
-0001fb90: 7261 7465 3a20 666c 6f61 7420 3d20 6472  rate: float = dr
-0001fba0: 6f70 6f75 745f 7261 7465 0a20 2020 2020  opout_rate.     
-0001fbb0: 2020 2073 656c 662e 6564 6765 733a 2069     self.edges: i
-0001fbc0: 6e74 203d 2065 6467 6573 0a20 2020 2020  nt = edges.     
-0001fbd0: 2020 2073 656c 662e 6e61 6d65 3a20 7374     self.name: st
-0001fbe0: 7220 3d20 6e61 6d65 0a0a 2020 2020 2020  r = name..      
-0001fbf0: 2020 7365 6c66 2e66 6972 7374 5f63 6f6e    self.first_con
-0001fc00: 766f 6c75 7469 6f6e 203d 204d 6f6c 4741  volution = MolGA
-0001fc10: 4e43 6f6e 766f 6c75 7469 6f6e 4c61 7965  NConvolutionLaye
-0001fc20: 7228 0a20 2020 2020 2020 2020 2020 2075  r(.            u
-0001fc30: 6e69 7473 3d73 656c 662e 756e 6974 735b  nits=self.units[
-0001fc40: 305d 2c0a 2020 2020 2020 2020 2020 2020  0],.            
-0001fc50: 6e6f 6465 733d 7365 6c66 2e6e 6f64 6573  nodes=self.nodes
-0001fc60: 2c0a 2020 2020 2020 2020 2020 2020 6163  ,.            ac
-0001fc70: 7469 7661 7469 6f6e 3d73 656c 662e 6163  tivation=self.ac
-0001fc80: 7469 7661 7469 6f6e 2c0a 2020 2020 2020  tivation,.      
-0001fc90: 2020 2020 2020 6472 6f70 6f75 745f 7261        dropout_ra
-0001fca0: 7465 3d73 656c 662e 6472 6f70 6f75 745f  te=self.dropout_
-0001fcb0: 7261 7465 2c0a 2020 2020 2020 2020 2020  rate,.          
-0001fcc0: 2020 6564 6765 733d 7365 6c66 2e65 6467    edges=self.edg
-0001fcd0: 6573 290a 2020 2020 2020 2020 7365 6c66  es).        self
-0001fce0: 2e67 636c 203d 206e 6e2e 4d6f 6475 6c65  .gcl = nn.Module
-0001fcf0: 4c69 7374 285b 0a20 2020 2020 2020 2020  List([.         
-0001fd00: 2020 204d 6f6c 4741 4e43 6f6e 766f 6c75     MolGANConvolu
-0001fd10: 7469 6f6e 4c61 7965 7228 756e 6974 733d  tionLayer(units=
-0001fd20: 752c 0a20 2020 2020 2020 2020 2020 2020  u,.             
-0001fd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fd40: 2020 2020 2020 6e6f 6465 733d 7365 6c66        nodes=self
-0001fd50: 2e6e 6f64 6573 2c0a 2020 2020 2020 2020  .nodes,.        
-0001fd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fd70: 2020 2020 2020 2020 2020 2061 6374 6976             activ
-0001fd80: 6174 696f 6e3d 7365 6c66 2e61 6374 6976  ation=self.activ
-0001fd90: 6174 696f 6e2c 0a20 2020 2020 2020 2020  ation,.         
-0001fda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fdb0: 2020 2020 2020 2020 2020 6472 6f70 6f75            dropou
-0001fdc0: 745f 7261 7465 3d73 656c 662e 6472 6f70  t_rate=self.drop
-0001fdd0: 6f75 745f 7261 7465 2c0a 2020 2020 2020  out_rate,.      
-0001fde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fdf0: 2020 2020 2020 2020 2020 2020 2065 6467               edg
-0001fe00: 6573 3d73 656c 662e 6564 6765 732c 0a20  es=self.edges,. 
-0001fe10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eac0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0001ead0: 7265 765f 7368 6170 653a 2069 6e74 203d  rev_shape: int =
+0001eae0: 2030 293a 0a20 2020 2020 2020 2022 2222   0):.        """
+0001eaf0: 0a20 2020 2020 2020 2049 6e69 7469 616c  .        Initial
+0001eb00: 697a 6520 7468 6520 6c61 7965 720a 0a20  ize the layer.. 
+0001eb10: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+0001eb20: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+0001eb30: 2d2d 2d0a 2020 2020 2020 2020 756e 6974  ---.        unit
+0001eb40: 733a 2069 6e74 2c20 6f70 7469 6f6e 616c  s: int, optional
+0001eb50: 2028 6465 6661 756c 743d 3132 3829 0a20   (default=128). 
+0001eb60: 2020 2020 2020 2020 2020 2044 696d 6573             Dimes
+0001eb70: 696f 6e20 6f66 2064 656e 7365 206c 6179  ion of dense lay
+0001eb80: 6572 7320 7573 6564 2066 6f72 2061 6767  ers used for agg
+0001eb90: 7265 6761 7469 6f6e 0a20 2020 2020 2020  regation.       
+0001eba0: 2061 6374 6976 6174 696f 6e3a 2066 756e   activation: fun
+0001ebb0: 6374 696f 6e2c 206f 7074 696f 6e61 6c20  ction, optional 
+0001ebc0: 2864 6566 6175 6c74 3d54 616e 6829 0a20  (default=Tanh). 
+0001ebd0: 2020 2020 2020 2020 2020 2061 6374 6976             activ
+0001ebe0: 6174 696f 6e20 6675 6e63 7469 6f6e 2075  ation function u
+0001ebf0: 7365 6420 6163 726f 7373 206d 6f64 656c  sed across model
+0001ec00: 2c20 6465 6661 756c 7420 6973 2054 616e  , default is Tan
+0001ec10: 680a 2020 2020 2020 2020 6472 6f70 6f75  h.        dropou
+0001ec20: 745f 7261 7465 3a20 666c 6f61 742c 206f  t_rate: float, o
+0001ec30: 7074 696f 6e61 6c20 2864 6566 6175 6c74  ptional (default
+0001ec40: 3d30 2e30 290a 2020 2020 2020 2020 2020  =0.0).          
+0001ec50: 2020 5573 6564 2062 7920 6472 6f70 6f75    Used by dropou
+0001ec60: 7420 6c61 7965 720a 2020 2020 2020 2020  t layer.        
+0001ec70: 6e61 6d65 3a20 7374 7269 6e67 2c20 6f70  name: string, op
+0001ec80: 7469 6f6e 616c 2028 6465 6661 756c 743d  tional (default=
+0001ec90: 2222 290a 2020 2020 2020 2020 2020 2020  "").            
+0001eca0: 4e61 6d65 206f 6620 7468 6520 6c61 7965  Name of the laye
+0001ecb0: 720a 2020 2020 2020 2020 7072 6576 5f73  r.        prev_s
+0001ecc0: 6861 7065 3a20 696e 742c 206f 7074 696f  hape: int, optio
+0001ecd0: 6e61 6c20 2864 6566 6175 6c74 3d30 290a  nal (default=0).
+0001ece0: 2020 2020 2020 2020 2020 2020 5368 6170              Shap
+0001ecf0: 6520 6f66 2074 6865 2069 6e70 7574 2074  e of the input t
+0001ed00: 656e 736f 720a 2020 2020 2020 2020 2222  ensor.        ""
+0001ed10: 220a 0a20 2020 2020 2020 2073 7570 6572  "..        super
+0001ed20: 284d 6f6c 4741 4e41 6767 7265 6761 7469  (MolGANAggregati
+0001ed30: 6f6e 4c61 7965 722c 2073 656c 6629 2e5f  onLayer, self)._
+0001ed40: 5f69 6e69 745f 5f28 290a 2020 2020 2020  _init__().      
+0001ed50: 2020 7365 6c66 2e75 6e69 7473 3a20 696e    self.units: in
+0001ed60: 7420 3d20 756e 6974 730a 2020 2020 2020  t = units.      
+0001ed70: 2020 7365 6c66 2e61 6374 6976 6174 696f    self.activatio
+0001ed80: 6e20 3d20 6163 7469 7661 7469 6f6e 0a20  n = activation. 
+0001ed90: 2020 2020 2020 2073 656c 662e 6472 6f70         self.drop
+0001eda0: 6f75 745f 7261 7465 3a20 666c 6f61 7420  out_rate: float 
+0001edb0: 3d20 6472 6f70 6f75 745f 7261 7465 0a20  = dropout_rate. 
+0001edc0: 2020 2020 2020 2073 656c 662e 6e61 6d65         self.name
+0001edd0: 3a20 7374 7220 3d20 6e61 6d65 0a0a 2020  : str = name..  
+0001ede0: 2020 2020 2020 6966 2070 7265 765f 7368        if prev_sh
+0001edf0: 6170 653a 0a20 2020 2020 2020 2020 2020  ape:.           
+0001ee00: 2073 656c 662e 6431 203d 206e 6e2e 4c69   self.d1 = nn.Li
+0001ee10: 6e65 6172 2870 7265 765f 7368 6170 652c  near(prev_shape,
+0001ee20: 2073 656c 662e 756e 6974 7329 0a20 2020   self.units).   
+0001ee30: 2020 2020 2020 2020 2073 656c 662e 6432           self.d2
+0001ee40: 203d 206e 6e2e 4c69 6e65 6172 2870 7265   = nn.Linear(pre
+0001ee50: 765f 7368 6170 652c 2073 656c 662e 756e  v_shape, self.un
+0001ee60: 6974 7329 0a20 2020 2020 2020 2065 6c73  its).        els
+0001ee70: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0001ee80: 656c 662e 6431 203d 206e 6e2e 4c69 6e65  elf.d1 = nn.Line
+0001ee90: 6172 2873 656c 662e 756e 6974 732c 2073  ar(self.units, s
+0001eea0: 656c 662e 756e 6974 7329 0a20 2020 2020  elf.units).     
+0001eeb0: 2020 2020 2020 2073 656c 662e 6432 203d         self.d2 =
+0001eec0: 206e 6e2e 4c69 6e65 6172 2873 656c 662e   nn.Linear(self.
+0001eed0: 756e 6974 732c 2073 656c 662e 756e 6974  units, self.unit
+0001eee0: 7329 0a20 2020 2020 2020 2073 656c 662e  s).        self.
+0001eef0: 6472 6f70 6f75 745f 6c61 7965 7220 3d20  dropout_layer = 
+0001ef00: 6e6e 2e44 726f 706f 7574 2864 726f 706f  nn.Dropout(dropo
+0001ef10: 7574 5f72 6174 6529 0a0a 2020 2020 6465  ut_rate)..    de
+0001ef20: 6620 5f5f 7265 7072 5f5f 2873 656c 6629  f __repr__(self)
+0001ef30: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
+0001ef40: 2022 2222 0a20 2020 2020 2020 2053 7472   """.        Str
+0001ef50: 696e 6720 7265 7072 6573 656e 7461 7469  ing representati
+0001ef60: 6f6e 206f 6620 7468 6520 6c61 7965 720a  on of the layer.
+0001ef70: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+0001ef80: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+0001ef90: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+0001efa0: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
+0001efb0: 2020 2020 5374 7269 6e67 2072 6570 7265      String repre
+0001efc0: 7365 6e74 6174 696f 6e20 6f66 2074 6865  sentation of the
+0001efd0: 206c 6179 6572 2020 2020 0a20 2020 2020   layer    .     
+0001efe0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+0001eff0: 6574 7572 6e20 6622 7b73 656c 662e 5f5f  eturn f"{self.__
+0001f000: 636c 6173 735f 5f2e 5f5f 6e61 6d65 5f5f  class__.__name__
+0001f010: 7d28 756e 6974 733d 7b73 656c 662e 756e  }(units={self.un
+0001f020: 6974 737d 2c20 6163 7469 7661 7469 6f6e  its}, activation
+0001f030: 3d7b 7365 6c66 2e61 6374 6976 6174 696f  ={self.activatio
+0001f040: 6e7d 2c20 6472 6f70 6f75 745f 7261 7465  n}, dropout_rate
+0001f050: 3d7b 7365 6c66 2e64 726f 706f 7574 5f72  ={self.dropout_r
+0001f060: 6174 657d 2922 0a0a 2020 2020 6465 6620  ate})"..    def 
+0001f070: 666f 7277 6172 6428 7365 6c66 2c20 696e  forward(self, in
+0001f080: 7075 7473 3a20 4c69 7374 2920 2d3e 2074  puts: List) -> t
+0001f090: 6f72 6368 2e54 656e 736f 723a 0a20 2020  orch.Tensor:.   
+0001f0a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0001f0b0: 2049 6e76 6f6b 6520 7468 6973 206c 6179   Invoke this lay
+0001f0c0: 6572 0a0a 2020 2020 2020 2020 5061 7261  er..        Para
+0001f0d0: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
+0001f0e0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+0001f0f0: 2020 696e 7075 7473 3a20 4c69 7374 0a20    inputs: List. 
+0001f100: 2020 2020 2020 2020 2020 2053 696e 676c             Singl
+0001f110: 6520 7465 6e73 6f72 2072 6573 756c 7469  e tensor resulti
+0001f120: 6e67 2066 726f 6d20 6772 6170 6820 636f  ng from graph co
+0001f130: 6e76 6f6c 7574 696f 6e20 6c61 7965 720a  nvolution layer.
+0001f140: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+0001f150: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+0001f160: 2d0a 2020 2020 2020 2020 6167 6772 6567  -.        aggreg
+0001f170: 6174 696f 6e20 7465 6e73 6f72 3a20 746f  ation tensor: to
+0001f180: 7263 682e 5465 6e73 6f72 0a20 2020 2020  rch.Tensor.     
+0001f190: 2020 2020 2052 6573 756c 7420 6f66 2061       Result of a
+0001f1a0: 6767 7265 6761 7469 6f6e 2066 756e 6374  ggregation funct
+0001f1b0: 696f 6e20 6f6e 2069 6e70 7574 2063 6f6e  ion on input con
+0001f1c0: 766f 6c75 7469 6f6e 2074 656e 736f 722e  volution tensor.
+0001f1d0: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
+0001f1e0: 2020 2020 2020 6920 3d20 746f 7263 682e        i = torch.
+0001f1f0: 7369 676d 6f69 6428 7365 6c66 2e64 3128  sigmoid(self.d1(
+0001f200: 696e 7075 7473 2929 0a20 2020 2020 2020  inputs)).       
+0001f210: 206a 203d 2073 656c 662e 6163 7469 7661   j = self.activa
+0001f220: 7469 6f6e 2873 656c 662e 6432 2869 6e70  tion(self.d2(inp
+0001f230: 7574 7329 290a 2020 2020 2020 2020 6f75  uts)).        ou
+0001f240: 7470 7574 203d 2074 6f72 6368 2e73 756d  tput = torch.sum
+0001f250: 2869 202a 206a 2c20 6469 6d3d 3129 0a20  (i * j, dim=1). 
+0001f260: 2020 2020 2020 206f 7574 7075 7420 3d20         output = 
+0001f270: 7365 6c66 2e61 6374 6976 6174 696f 6e28  self.activation(
+0001f280: 6f75 7470 7574 290a 2020 2020 2020 2020  output).        
+0001f290: 6f75 7470 7574 203d 2073 656c 662e 6472  output = self.dr
+0001f2a0: 6f70 6f75 745f 6c61 7965 7228 6f75 7470  opout_layer(outp
+0001f2b0: 7574 290a 2020 2020 2020 2020 7265 7475  ut).        retu
+0001f2c0: 726e 206f 7574 7075 740a 0a0a 636c 6173  rn output...clas
+0001f2d0: 7320 4d6f 6c47 414e 4d75 6c74 6943 6f6e  s MolGANMultiCon
+0001f2e0: 766f 6c75 7469 6f6e 4c61 7965 7228 6e6e  volutionLayer(nn
+0001f2f0: 2e4d 6f64 756c 6529 3a0a 2020 2020 2222  .Module):.    ""
+0001f300: 220a 2020 2020 4d75 6c74 6970 6c65 2070  ".    Multiple p
+0001f310: 6173 7320 636f 6e76 6f6c 7574 696f 6e20  ass convolution 
+0001f320: 6c61 7965 7220 7573 6564 2069 6e20 4d6f  layer used in Mo
+0001f330: 6c47 414e 206d 6f64 656c 2e0a 2020 2020  lGAN model..    
+0001f340: 4d6f 6c47 414e 2069 7320 6120 5747 414e  MolGAN is a WGAN
+0001f350: 2074 7970 6520 6d6f 6465 6c20 666f 7220   type model for 
+0001f360: 6765 6e65 7261 7469 6f6e 206f 6620 736d  generation of sm
+0001f370: 616c 6c20 6d6f 6c65 6375 6c65 732e 0a20  all molecules.. 
+0001f380: 2020 2049 7420 7461 6b65 7320 6f75 7470     It takes outp
+0001f390: 7574 7320 6f66 2070 7265 7669 6f75 7320  uts of previous 
+0001f3a0: 636f 6e76 6f6c 7574 696f 6e20 6c61 7965  convolution laye
+0001f3b0: 7220 616e 6420 7573 6573 0a20 2020 2074  r and uses.    t
+0001f3c0: 6865 6d20 6173 2069 6e70 7574 7320 666f  hem as inputs fo
+0001f3d0: 7220 7468 6520 6e65 7874 206f 6e65 2e0a  r the next one..
+0001f3e0: 2020 2020 4974 2073 696d 706c 6966 6965      It simplifie
+0001f3f0: 7320 7468 6520 6f76 6572 616c 6c20 6672  s the overall fr
+0001f400: 616d 6577 6f72 6b2c 2062 7574 206d 6967  amework, but mig
+0001f410: 6874 2062 6520 6d6f 7665 6420 746f 0a20  ht be moved to. 
+0001f420: 2020 204d 6f6c 4741 4e45 6e63 6f64 6572     MolGANEncoder
+0001f430: 4c61 7965 7220 696e 2074 6865 2066 7574  Layer in the fut
+0001f440: 7572 6520 696e 206f 7264 6572 2074 6f20  ure in order to 
+0001f450: 7265 6475 6365 206e 756d 6265 7220 6f66  reduce number of
+0001f460: 206c 6179 6572 732e 0a0a 2020 2020 4578   layers...    Ex
+0001f470: 616d 706c 650a 2020 2020 2d2d 2d2d 2d2d  ample.    ------
+0001f480: 2d0a 2020 2020 3e3e 3e20 696d 706f 7274  -.    >>> import
+0001f490: 2074 6f72 6368 0a20 2020 203e 3e3e 2069   torch.    >>> i
+0001f4a0: 6d70 6f72 7420 746f 7263 682e 6e6e 2061  mport torch.nn a
+0001f4b0: 7320 6e6e 0a20 2020 203e 3e3e 2069 6d70  s nn.    >>> imp
+0001f4c0: 6f72 7420 746f 7263 682e 6e6e 2e66 756e  ort torch.nn.fun
+0001f4d0: 6374 696f 6e61 6c20 6173 2046 0a20 2020  ctional as F.   
+0001f4e0: 203e 3e3e 2076 6572 7469 6365 7320 3d20   >>> vertices = 
+0001f4f0: 390a 2020 2020 3e3e 3e20 6e6f 6465 7320  9.    >>> nodes 
+0001f500: 3d20 350a 2020 2020 3e3e 3e20 6564 6765  = 5.    >>> edge
+0001f510: 7320 3d20 350a 2020 2020 3e3e 3e20 756e  s = 5.    >>> un
+0001f520: 6974 7320 3d20 2831 3238 2c36 3429 0a0a  its = (128,64)..
+0001f530: 2020 2020 3e3e 3e20 6c61 7965 725f 3120      >>> layer_1 
+0001f540: 3d20 4d6f 6c47 414e 4d75 6c74 6943 6f6e  = MolGANMultiCon
+0001f550: 766f 6c75 7469 6f6e 4c61 7965 7228 756e  volutionLayer(un
+0001f560: 6974 733d 756e 6974 732c 206e 6f64 6573  its=units, nodes
+0001f570: 3d6e 6f64 6573 2c20 6564 6765 733d 6564  =nodes, edges=ed
+0001f580: 6765 732c 206e 616d 653d 276c 6179 6572  ges, name='layer
+0001f590: 3127 290a 2020 2020 3e3e 3e20 6164 6a61  1').    >>> adja
+0001f5a0: 6365 6e63 795f 7465 6e73 6f72 203d 2074  cency_tensor = t
+0001f5b0: 6f72 6368 2e72 616e 646e 2828 312c 2076  orch.randn((1, v
+0001f5c0: 6572 7469 6365 732c 2076 6572 7469 6365  ertices, vertice
+0001f5d0: 732c 2065 6467 6573 2929 0a20 2020 203e  s, edges)).    >
+0001f5e0: 3e3e 206e 6f64 655f 7465 6e73 6f72 203d  >> node_tensor =
+0001f5f0: 2074 6f72 6368 2e72 616e 646e 2828 312c   torch.randn((1,
+0001f600: 2076 6572 7469 6365 732c 206e 6f64 6573   vertices, nodes
+0001f610: 2929 0a20 2020 203e 3e3e 206f 7574 7075  )).    >>> outpu
+0001f620: 7420 3d20 6c61 7965 725f 3128 5b61 646a  t = layer_1([adj
+0001f630: 6163 656e 6379 5f74 656e 736f 722c 206e  acency_tensor, n
+0001f640: 6f64 655f 7465 6e73 6f72 5d29 0a0a 2020  ode_tensor])..  
+0001f650: 2020 5265 6665 7265 6e63 6573 0a20 2020    References.   
+0001f660: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+0001f670: 2e2e 205b 315d 204e 6963 6f6c 6120 4465  .. [1] Nicola De
+0001f680: 2043 616f 2065 7420 616c 2e20 224d 6f6c   Cao et al. "Mol
+0001f690: 4741 4e3a 2041 6e20 696d 706c 6963 6974  GAN: An implicit
+0001f6a0: 2067 656e 6572 6174 6976 6520 6d6f 6465   generative mode
+0001f6b0: 6c0a 2020 2020 2020 2020 666f 7220 736d  l.        for sm
+0001f6c0: 616c 6c20 6d6f 6c65 6375 6c61 7220 6772  all molecular gr
+0001f6d0: 6170 6873 222c 2068 7474 7073 3a2f 2f61  aphs", https://a
+0001f6e0: 7278 6976 2e6f 7267 2f61 6273 2f31 3830  rxiv.org/abs/180
+0001f6f0: 352e 3131 3937 330a 2020 2020 2222 220a  5.11973.    """.
+0001f700: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+0001f710: 5f28 7365 6c66 2c0a 2020 2020 2020 2020  _(self,.        
+0001f720: 2020 2020 2020 2020 2075 6e69 7473 3a20           units: 
+0001f730: 5475 706c 6520 3d20 2831 3238 2c20 3634  Tuple = (128, 64
+0001f740: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0001f750: 2020 2020 6e6f 6465 733a 2069 6e74 203d      nodes: int =
+0001f760: 2035 2c0a 2020 2020 2020 2020 2020 2020   5,.            
+0001f770: 2020 2020 2061 6374 6976 6174 696f 6e3d       activation=
+0001f780: 746f 7263 682e 7461 6e68 2c0a 2020 2020  torch.tanh,.    
+0001f790: 2020 2020 2020 2020 2020 2020 2064 726f               dro
+0001f7a0: 706f 7574 5f72 6174 653a 2066 6c6f 6174  pout_rate: float
+0001f7b0: 203d 2030 2e30 2c0a 2020 2020 2020 2020   = 0.0,.        
+0001f7c0: 2020 2020 2020 2020 2065 6467 6573 3a20           edges: 
+0001f7d0: 696e 7420 3d20 352c 0a20 2020 2020 2020  int = 5,.       
+0001f7e0: 2020 2020 2020 2020 2020 6e61 6d65 3a20            name: 
+0001f7f0: 7374 7220 3d20 2222 2c0a 2020 2020 2020  str = "",.      
+0001f800: 2020 2020 2020 2020 2020 202a 2a6b 7761             **kwa
+0001f810: 7267 7329 3a0a 2020 2020 2020 2020 2222  rgs):.        ""
+0001f820: 220a 2020 2020 2020 2020 496e 6974 6961  ".        Initia
+0001f830: 6c69 7a65 2074 6865 206c 6179 6572 0a0a  lize the layer..
+0001f840: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+0001f850: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+0001f860: 2d2d 2d2d 0a20 2020 2020 2020 2075 6e69  ----.        uni
+0001f870: 7473 3a20 5475 706c 652c 206f 7074 696f  ts: Tuple, optio
+0001f880: 6e61 6c20 2864 6566 6175 6c74 3d28 3132  nal (default=(12
+0001f890: 382c 3634 2929 2c20 6d69 6e5f 6c65 6e67  8,64)), min_leng
+0001f8a0: 7468 3d32 0a20 2020 2020 2020 2020 2020  th=2.           
+0001f8b0: 2069 7374 206f 6620 6469 6d65 6e73 696f   ist of dimensio
+0001f8c0: 6e73 2075 7365 6420 6279 2063 6f6e 7365  ns used by conse
+0001f8d0: 6375 7469 7665 2063 6f6e 766f 6c75 7469  cutive convoluti
+0001f8e0: 6f6e 206c 6179 6572 732e 0a20 2020 2020  on layers..     
+0001f8f0: 2020 2020 2020 2054 6865 206d 6f72 6520         The more 
+0001f900: 7661 6c75 6573 2074 6865 206d 6f72 6520  values the more 
+0001f910: 636f 6e76 6f6c 7574 696f 6e20 6c61 7965  convolution laye
+0001f920: 7273 2069 6e76 6f6b 6564 2e0a 2020 2020  rs invoked..    
+0001f930: 2020 2020 6e6f 6465 733a 2069 6e74 2c20      nodes: int, 
+0001f940: 6f70 7469 6f6e 616c 2028 6465 6661 756c  optional (defaul
+0001f950: 743d 3529 0a20 2020 2020 2020 2020 2020  t=5).           
+0001f960: 204e 756d 6265 7220 6f66 2066 6561 7475   Number of featu
+0001f970: 7265 7320 696e 206e 6f64 6520 7465 6e73  res in node tens
+0001f980: 6f72 0a20 2020 2020 2020 2061 6374 6976  or.        activ
+0001f990: 6174 696f 6e3a 2066 756e 6374 696f 6e2c  ation: function,
+0001f9a0: 206f 7074 696f 6e61 6c20 2864 6566 6175   optional (defau
+0001f9b0: 6c74 3d54 616e 6829 0a20 2020 2020 2020  lt=Tanh).       
+0001f9c0: 2020 2020 2061 6374 6976 6174 696f 6e20       activation 
+0001f9d0: 6675 6e63 7469 6f6e 2075 7365 6420 6163  function used ac
+0001f9e0: 726f 7373 206d 6f64 656c 2c20 6465 6661  ross model, defa
+0001f9f0: 756c 7420 6973 2054 616e 680a 2020 2020  ult is Tanh.    
+0001fa00: 2020 2020 6472 6f70 6f75 745f 7261 7465      dropout_rate
+0001fa10: 3a20 666c 6f61 742c 206f 7074 696f 6e61  : float, optiona
+0001fa20: 6c20 2864 6566 6175 6c74 3d30 2e30 290a  l (default=0.0).
+0001fa30: 2020 2020 2020 2020 2020 2020 5573 6564              Used
+0001fa40: 2062 7920 6472 6f70 6f75 7420 6c61 7965   by dropout laye
+0001fa50: 720a 2020 2020 2020 2020 6564 6765 733a  r.        edges:
+0001fa60: 2069 6e74 2c20 6f70 7469 6f6e 616c 2028   int, optional (
+0001fa70: 6465 6661 756c 743d 3529 0a20 2020 2020  default=5).     
+0001fa80: 2020 2020 2020 2043 6f6e 7472 6f6c 7320         Controls 
+0001fa90: 686f 7720 6d61 6e79 2064 656e 7365 206c  how many dense l
+0001faa0: 6179 6572 7320 7573 6520 666f 7220 7369  ayers use for si
+0001fab0: 6e67 6c65 2063 6f6e 766f 6c75 7469 6f6e  ngle convolution
+0001fac0: 2075 6e69 742e 0a20 2020 2020 2020 2020   unit..         
+0001fad0: 2020 2054 7970 6963 616c 6c79 206d 6174     Typically mat
+0001fae0: 6368 6573 206e 756d 6265 7220 6f66 2062  ches number of b
+0001faf0: 6f6e 6420 7479 7065 7320 7573 6564 2069  ond types used i
+0001fb00: 6e20 7468 6520 6d6f 6c65 6375 6c65 2e0a  n the molecule..
+0001fb10: 2020 2020 2020 2020 6e61 6d65 3a20 7374          name: st
+0001fb20: 7269 6e67 2c20 6f70 7469 6f6e 616c 2028  ring, optional (
+0001fb30: 6465 6661 756c 743d 2222 290a 2020 2020  default="").    
+0001fb40: 2020 2020 2020 2020 4e61 6d65 206f 6620          Name of 
+0001fb50: 7468 6520 6c61 7965 720a 2020 2020 2020  the layer.      
+0001fb60: 2020 2222 220a 0a20 2020 2020 2020 2073    """..        s
+0001fb70: 7570 6572 284d 6f6c 4741 4e4d 756c 7469  uper(MolGANMulti
+0001fb80: 436f 6e76 6f6c 7574 696f 6e4c 6179 6572  ConvolutionLayer
+0001fb90: 2c20 7365 6c66 292e 5f5f 696e 6974 5f5f  , self).__init__
+0001fba0: 2829 0a20 2020 2020 2020 2069 6620 6c65  ().        if le
+0001fbb0: 6e28 756e 6974 7329 203c 2032 3a0a 2020  n(units) < 2:.  
+0001fbc0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0001fbd0: 5661 6c75 6545 7272 6f72 2822 756e 6974  ValueError("unit
+0001fbe0: 7320 7061 7261 6d65 7465 7220 6d75 7374  s parameter must
+0001fbf0: 2063 6f6e 7461 696e 2061 7420 6c65 6173   contain at leas
+0001fc00: 7420 7477 6f20 7661 6c75 6573 2229 0a0a  t two values")..
+0001fc10: 2020 2020 2020 2020 7365 6c66 2e6e 6f64          self.nod
+0001fc20: 6573 3a20 696e 7420 3d20 6e6f 6465 730a  es: int = nodes.
+0001fc30: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+0001fc40: 7473 3a20 5475 706c 6520 3d20 756e 6974  ts: Tuple = unit
+0001fc50: 730a 2020 2020 2020 2020 7365 6c66 2e61  s.        self.a
+0001fc60: 6374 6976 6174 696f 6e20 3d20 6163 7469  ctivation = acti
+0001fc70: 7661 7469 6f6e 0a20 2020 2020 2020 2073  vation.        s
+0001fc80: 656c 662e 6472 6f70 6f75 745f 7261 7465  elf.dropout_rate
+0001fc90: 3a20 666c 6f61 7420 3d20 6472 6f70 6f75  : float = dropou
+0001fca0: 745f 7261 7465 0a20 2020 2020 2020 2073  t_rate.        s
+0001fcb0: 656c 662e 6564 6765 733a 2069 6e74 203d  elf.edges: int =
+0001fcc0: 2065 6467 6573 0a20 2020 2020 2020 2073   edges.        s
+0001fcd0: 656c 662e 6e61 6d65 3a20 7374 7220 3d20  elf.name: str = 
+0001fce0: 6e61 6d65 0a0a 2020 2020 2020 2020 7365  name..        se
+0001fcf0: 6c66 2e66 6972 7374 5f63 6f6e 766f 6c75  lf.first_convolu
+0001fd00: 7469 6f6e 203d 204d 6f6c 4741 4e43 6f6e  tion = MolGANCon
+0001fd10: 766f 6c75 7469 6f6e 4c61 7965 7228 0a20  volutionLayer(. 
+0001fd20: 2020 2020 2020 2020 2020 2075 6e69 7473             units
+0001fd30: 3d73 656c 662e 756e 6974 735b 305d 2c0a  =self.units[0],.
+0001fd40: 2020 2020 2020 2020 2020 2020 6e6f 6465              node
+0001fd50: 733d 7365 6c66 2e6e 6f64 6573 2c0a 2020  s=self.nodes,.  
+0001fd60: 2020 2020 2020 2020 2020 6163 7469 7661            activa
+0001fd70: 7469 6f6e 3d73 656c 662e 6163 7469 7661  tion=self.activa
+0001fd80: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
+0001fd90: 2020 6472 6f70 6f75 745f 7261 7465 3d73    dropout_rate=s
+0001fda0: 656c 662e 6472 6f70 6f75 745f 7261 7465  elf.dropout_rate
+0001fdb0: 2c0a 2020 2020 2020 2020 2020 2020 6564  ,.            ed
+0001fdc0: 6765 733d 7365 6c66 2e65 6467 6573 290a  ges=self.edges).
+0001fdd0: 2020 2020 2020 2020 7365 6c66 2e67 636c          self.gcl
+0001fde0: 203d 206e 6e2e 4d6f 6475 6c65 4c69 7374   = nn.ModuleList
+0001fdf0: 285b 0a20 2020 2020 2020 2020 2020 204d  ([.            M
+0001fe00: 6f6c 4741 4e43 6f6e 766f 6c75 7469 6f6e  olGANConvolution
+0001fe10: 4c61 7965 7228 756e 6974 733d 752c 0a20  Layer(units=u,. 
 0001fe20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fe30: 2020 7072 6576 5f73 6861 7065 3d73 656c    prev_shape=sel
-0001fe40: 662e 756e 6974 735b 636f 756e 745d 290a  f.units[count]).
-0001fe50: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0001fe60: 636f 756e 742c 2075 2069 6e20 656e 756d  count, u in enum
-0001fe70: 6572 6174 6528 7365 6c66 2e75 6e69 7473  erate(self.units
-0001fe80: 5b31 3a5d 290a 2020 2020 2020 2020 5d29  [1:]).        ])
-0001fe90: 0a0a 2020 2020 6465 6620 5f5f 7265 7072  ..    def __repr
-0001fea0: 5f5f 2873 656c 6629 202d 3e20 7374 723a  __(self) -> str:
-0001feb0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0001fec0: 2020 2020 2053 7472 696e 6720 7265 7072       String repr
-0001fed0: 6573 656e 7461 7469 6f6e 206f 6620 7468  esentation of th
-0001fee0: 6520 6c61 7965 720a 2020 2020 2020 2020  e layer.        
-0001fef0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-0001ff00: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-0001ff10: 0a20 2020 2020 2020 2073 7472 696e 670a  .        string.
-0001ff20: 2020 2020 2020 2020 2020 2020 5374 7269              Stri
-0001ff30: 6e67 2072 6570 7265 7365 6e74 6174 696f  ng representatio
-0001ff40: 6e20 6f66 2074 6865 206c 6179 6572 0a20  n of the layer. 
-0001ff50: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0001ff60: 2020 2072 6574 7572 6e20 6622 7b73 656c     return f"{sel
-0001ff70: 662e 5f5f 636c 6173 735f 5f2e 5f5f 6e61  f.__class__.__na
-0001ff80: 6d65 5f5f 7d28 756e 6974 733d 7b73 656c  me__}(units={sel
-0001ff90: 662e 756e 6974 737d 2c20 6163 7469 7661  f.units}, activa
-0001ffa0: 7469 6f6e 3d7b 7365 6c66 2e61 6374 6976  tion={self.activ
-0001ffb0: 6174 696f 6e7d 2c20 6472 6f70 6f75 745f  ation}, dropout_
-0001ffc0: 7261 7465 3d7b 7365 6c66 2e64 726f 706f  rate={self.dropo
-0001ffd0: 7574 5f72 6174 657d 292c 2065 6467 6573  ut_rate}), edges
-0001ffe0: 3d7b 7365 6c66 2e65 6467 6573 7d29 220a  ={self.edges})".
-0001fff0: 0a20 2020 2064 6566 2066 6f72 7761 7264  .    def forward
-00020000: 2873 656c 662c 2069 6e70 7574 733a 204c  (self, inputs: L
-00020010: 6973 7429 202d 3e20 746f 7263 682e 5465  ist) -> torch.Te
-00020020: 6e73 6f72 3a0a 2020 2020 2020 2020 2222  nsor:.        ""
-00020030: 220a 2020 2020 2020 2020 496e 766f 6b65  ".        Invoke
-00020040: 2074 6869 7320 6c61 7965 720a 0a20 2020   this layer..   
-00020050: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00020060: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00020070: 2d2d 0a20 2020 2020 2020 2069 6e70 7574  --.        input
-00020080: 733a 206c 6973 740a 2020 2020 2020 2020  s: list.        
-00020090: 2020 2020 4c69 7374 206f 6620 7477 6f20      List of two 
-000200a0: 696e 7075 7420 6d61 7472 6963 6573 2c20  input matrices, 
-000200b0: 6164 6a61 6365 6e63 7920 7465 6e73 6f72  adjacency tensor
-000200c0: 2061 6e64 206e 6f64 6520 6665 6174 7572   and node featur
-000200d0: 6573 2074 656e 736f 7273 0a20 2020 2020  es tensors.     
-000200e0: 2020 2020 2020 2069 6e20 6f6e 652d 686f         in one-ho
-000200f0: 7420 656e 636f 6469 6e67 2066 6f72 6d61  t encoding forma
-00020100: 742e 0a0a 2020 2020 2020 2020 5265 7475  t...        Retu
-00020110: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
-00020120: 2d2d 2d2d 0a20 2020 2020 2020 2063 6f6e  ----.        con
-00020130: 766f 6c75 7469 6f6e 2074 656e 736f 723a  volution tensor:
-00020140: 2074 6f72 6368 2e54 656e 736f 720a 2020   torch.Tensor.  
-00020150: 2020 2020 2020 2020 2020 5265 7375 6c74            Result
-00020160: 206f 6620 696e 7075 7420 7465 6e73 6f72   of input tensor
-00020170: 7320 676f 696e 6720 7468 726f 7567 6820  s going through 
-00020180: 636f 6e76 6f6c 7574 696f 6e20 6120 6e75  convolution a nu
-00020190: 6d62 6572 206f 6620 7469 6d65 732e 0a20  mber of times.. 
-000201a0: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-000201b0: 2020 2020 6164 6a61 6365 6e63 795f 7465      adjacency_te
-000201c0: 6e73 6f72 203d 2069 6e70 7574 735b 305d  nsor = inputs[0]
-000201d0: 0a20 2020 2020 2020 206e 6f64 655f 7465  .        node_te
-000201e0: 6e73 6f72 203d 2069 6e70 7574 735b 315d  nsor = inputs[1]
-000201f0: 0a0a 2020 2020 2020 2020 7465 6e73 6f72  ..        tensor
-00020200: 7320 3d20 7365 6c66 2e66 6972 7374 5f63  s = self.first_c
-00020210: 6f6e 766f 6c75 7469 6f6e 285b 6164 6a61  onvolution([adja
-00020220: 6365 6e63 795f 7465 6e73 6f72 2c20 6e6f  cency_tensor, no
-00020230: 6465 5f74 656e 736f 725d 290a 0a20 2020  de_tensor])..   
-00020240: 2020 2020 2023 204c 6f6f 7020 6f76 6572       # Loop over
-00020250: 2074 6865 2072 656d 6169 6e69 6e67 2063   the remaining c
-00020260: 6f6e 766f 6c75 7469 6f6e 206c 6179 6572  onvolution layer
-00020270: 730a 2020 2020 2020 2020 666f 7220 6c61  s.        for la
-00020280: 7965 7220 696e 2073 656c 662e 6763 6c3a  yer in self.gcl:
-00020290: 0a20 2020 2020 2020 2020 2020 2023 2041  .            # A
-000202a0: 7070 6c79 2074 6865 2063 7572 7265 6e74  pply the current
-000202b0: 206c 6179 6572 2074 6f20 7468 6520 6f75   layer to the ou
-000202c0: 7470 7574 7320 6672 6f6d 2074 6865 2070  tputs from the p
-000202d0: 7265 7669 6f75 7320 6c61 7965 720a 2020  revious layer.  
-000202e0: 2020 2020 2020 2020 2020 7465 6e73 6f72            tensor
-000202f0: 7320 3d20 6c61 7965 7228 7465 6e73 6f72  s = layer(tensor
-00020300: 7329 0a0a 2020 2020 2020 2020 5f2c 205f  s)..        _, _
-00020310: 2c20 6869 6464 656e 5f74 656e 736f 7220  , hidden_tensor 
-00020320: 3d20 7465 6e73 6f72 730a 0a20 2020 2020  = tensors..     
-00020330: 2020 2072 6574 7572 6e20 6869 6464 656e     return hidden
-00020340: 5f74 656e 736f 720a 0a0a 636c 6173 7320  _tensor...class 
-00020350: 4454 4e4e 5374 6570 286e 6e2e 4d6f 6475  DTNNStep(nn.Modu
-00020360: 6c65 293a 0a20 2020 2022 2222 4454 4e4e  le):.    """DTNN
-00020370: 5374 6570 204c 6179 6572 2066 6f72 2044  Step Layer for D
-00020380: 544e 4e20 6d6f 6465 6c2e 0a0a 2020 2020  TNN model...    
-00020390: 456e 636f 6465 7320 7468 6520 6174 6f6d  Encodes the atom
-000203a0: 2773 2069 6e74 6572 6163 7469 6f6e 2077  's interaction w
-000203b0: 6974 6820 6f74 6865 7220 6174 6f6d 7320  ith other atoms 
-000203c0: 6163 636f 7264 696e 6720 746f 2064 6973  according to dis
-000203d0: 7461 6e63 6520 7265 6c61 7469 6f6e 7368  tance relationsh
-000203e0: 6970 732e 205b 315d 5f0a 0a20 2020 2054  ips. [1]_..    T
-000203f0: 6869 7320 4c61 7965 7220 696d 706c 656d  his Layer implem
-00020400: 656e 7473 2074 6865 2045 7120 2837 2920  ents the Eq (7) 
-00020410: 6672 6f6d 2044 544e 4e20 5061 7065 722e  from DTNN Paper.
-00020420: 2054 6865 6e20 7375 6d73 2074 6865 6d20   Then sums them 
-00020430: 7570 2074 6f20 6765 7420 7468 6520 6669  up to get the fi
-00020440: 6e61 6c20 6f75 7470 7574 2075 7369 6e67  nal output using
-00020450: 2045 7120 2836 2920 6672 6f6d 2044 544e   Eq (6) from DTN
-00020460: 4e20 5061 7065 722e 0a0a 2020 2020 4571  N Paper...    Eq
-00020470: 2028 3729 3a20 565f 696a 203d 2074 616e   (7): V_ij = tan
-00020480: 685b 575f 6663 202e 2028 2857 5f63 6620  h[W_fc . ((W_cf 
-00020490: 2e20 435f 6a20 2b20 625f 6366 2920 2a20  . C_j + b_cf) * 
-000204a0: 2857 5f64 6620 2e20 645f 696a 202b 2062  (W_df . d_ij + b
-000204b0: 5f64 6629 295d 0a0a 2020 2020 4571 2028  _df))]..    Eq (
-000204c0: 3629 3a20 435f 6920 3d20 435f 6920 2b20  6): C_i = C_i + 
-000204d0: 7375 6d28 565f 696a 290a 0a20 2020 2048  sum(V_ij)..    H
-000204e0: 6572 6520 3a20 272e 273d 4d61 7472 6978  ere : '.'=Matrix
-000204f0: 204d 756c 7469 706c 6963 6174 696f 6e20   Multiplication 
-00020500: 2c20 272a 273d 4d75 6c74 6970 6c69 6361  , '*'=Multiplica
-00020510: 7469 6f6e 0a0a 2020 2020 5265 6665 7265  tion..    Refere
-00020520: 6e63 6573 0a20 2020 202d 2d2d 2d2d 2d2d  nces.    -------
-00020530: 2d2d 2d0a 2020 2020 5b31 5d20 5363 68c3  ---.    [1] Sch.
-00020540: bc74 742c 204b 7269 7374 6f66 2054 2e2c  .tt, Kristof T.,
-00020550: 2065 7420 616c 2e20 2251 7561 6e74 756d   et al. "Quantum
-00020560: 2d63 6865 6d69 6361 6c20 696e 7369 6768  -chemical insigh
-00020570: 7473 2066 726f 6d20 6465 6570 0a20 2020  ts from deep.   
-00020580: 2020 2020 2074 656e 736f 7220 6e65 7572       tensor neur
-00020590: 616c 206e 6574 776f 726b 732e 2220 4e61  al networks." Na
-000205a0: 7475 7265 2063 6f6d 6d75 6e69 6361 7469  ture communicati
-000205b0: 6f6e 7320 382e 3120 2832 3031 3729 3a20  ons 8.1 (2017): 
-000205c0: 312d 382e 0a0a 2020 2020 4578 616d 706c  1-8...    Exampl
-000205d0: 6573 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a  es.    --------.
-000205e0: 2020 2020 3e3e 3e20 6672 6f6d 2064 6565      >>> from dee
-000205f0: 7063 6865 6d2e 6d6f 6465 6c73 2e74 6f72  pchem.models.tor
-00020600: 6368 5f6d 6f64 656c 7320 696d 706f 7274  ch_models import
-00020610: 206c 6179 6572 730a 2020 2020 3e3e 3e20   layers.    >>> 
-00020620: 696d 706f 7274 2074 6f72 6368 0a20 2020  import torch.   
-00020630: 203e 3e3e 2065 6d62 6564 6469 6e67 5f6c   >>> embedding_l
-00020640: 6179 6572 203d 206c 6179 6572 732e 4454  ayer = layers.DT
-00020650: 4e4e 456d 6265 6464 696e 6728 342c 2034  NNEmbedding(4, 4
-00020660: 290a 2020 2020 3e3e 3e20 656d 6220 3d20  ).    >>> emb = 
-00020670: 656d 6265 6464 696e 675f 6c61 7965 7228  embedding_layer(
-00020680: 746f 7263 682e 5465 6e73 6f72 285b 302c  torch.Tensor([0,
-00020690: 312c 322c 335d 292e 746f 2874 6f72 6368  1,2,3]).to(torch
-000206a0: 2e69 6e74 3634 2929 0a20 2020 203e 3e3e  .int64)).    >>>
-000206b0: 2073 7465 705f 6c61 7965 7220 3d20 6c61   step_layer = la
-000206c0: 7965 7273 2e44 544e 4e53 7465 7028 342c  yers.DTNNStep(4,
-000206d0: 2036 2c20 3829 0a20 2020 203e 3e3e 206f   6, 8).    >>> o
-000206e0: 7574 7075 745f 746f 7263 6820 3d20 7374  utput_torch = st
-000206f0: 6570 5f6c 6179 6572 285b 0a20 2020 202e  ep_layer([.    .
-00020700: 2e2e 2020 2020 2074 6f72 6368 2e54 656e  ..     torch.Ten
-00020710: 736f 7228 656d 6229 2c0a 2020 2020 2e2e  sor(emb),.    ..
-00020720: 2e20 2020 2020 746f 7263 682e 5465 6e73  .     torch.Tens
-00020730: 6f72 285b 302c 2031 2c20 322c 2033 2c20  or([0, 1, 2, 3, 
-00020740: 342c 2035 5d29 2e74 6f28 746f 7263 682e  4, 5]).to(torch.
-00020750: 666c 6f61 7433 3229 2c0a 2020 2020 2e2e  float32),.    ..
-00020760: 2e20 2020 2020 746f 7263 682e 5465 6e73  .     torch.Tens
-00020770: 6f72 285b 315d 292e 746f 2874 6f72 6368  or([1]).to(torch
-00020780: 2e69 6e74 3634 292c 0a20 2020 202e 2e2e  .int64),.    ...
-00020790: 2020 2020 2074 6f72 6368 2e54 656e 736f       torch.Tenso
-000207a0: 7228 5b5b 315d 5d29 2e74 6f28 746f 7263  r([[1]]).to(torc
-000207b0: 682e 696e 7436 3429 0a20 2020 202e 2e2e  h.int64).    ...
-000207c0: 205d 290a 2020 2020 3e3e 3e20 6f75 7470   ]).    >>> outp
-000207d0: 7574 5f74 6f72 6368 2e73 6861 7065 0a20  ut_torch.shape. 
-000207e0: 2020 2074 6f72 6368 2e53 697a 6528 5b32     torch.Size([2
-000207f0: 2c20 342c 2034 5d29 0a0a 2020 2020 2222  , 4, 4])..    ""
-00020800: 220a 0a20 2020 2064 6566 205f 5f69 6e69  "..    def __ini
-00020810: 745f 5f28 7365 6c66 2c0a 2020 2020 2020  t__(self,.      
-00020820: 2020 2020 2020 2020 2020 206e 5f65 6d62             n_emb
-00020830: 6564 6469 6e67 3a20 696e 7420 3d20 3330  edding: int = 30
-00020840: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00020850: 2020 206e 5f64 6973 7461 6e63 653a 2069     n_distance: i
-00020860: 6e74 203d 2031 3030 2c0a 2020 2020 2020  nt = 100,.      
-00020870: 2020 2020 2020 2020 2020 206e 5f68 6964             n_hid
-00020880: 6465 6e3a 2069 6e74 203d 2036 302c 0a20  den: int = 60,. 
-00020890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000208a0: 696e 6974 6961 6c69 7a65 723a 2073 7472  initializer: str
-000208b0: 203d 2027 7861 7669 6572 5f75 6e69 666f   = 'xavier_unifo
-000208c0: 726d 5f27 2c0a 2020 2020 2020 2020 2020  rm_',.          
-000208d0: 2020 2020 2020 2061 6374 6976 6174 696f         activatio
-000208e0: 6e3d 2774 616e 6827 2c0a 2020 2020 2020  n='tanh',.      
-000208f0: 2020 2020 2020 2020 2020 202a 2a6b 7761             **kwa
-00020900: 7267 7329 3a0a 2020 2020 2020 2020 2222  rgs):.        ""
-00020910: 220a 2020 2020 2020 2020 5061 7261 6d65  ".        Parame
-00020920: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-00020930: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00020940: 6e5f 656d 6265 6464 696e 673a 2069 6e74  n_embedding: int
-00020950: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-00020960: 2020 2020 2020 204e 756d 6265 7220 6f66         Number of
-00020970: 2066 6561 7475 7265 7320 666f 7220 6561   features for ea
-00020980: 6368 2061 746f 6d0a 2020 2020 2020 2020  ch atom.        
-00020990: 6e5f 6469 7374 616e 6365 3a20 696e 742c  n_distance: int,
-000209a0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-000209b0: 2020 2020 2020 6772 616e 756c 6172 6974        granularit
-000209c0: 7920 6f66 2064 6973 7461 6e63 6520 6d61  y of distance ma
-000209d0: 7472 6978 0a20 2020 2020 2020 206e 5f68  trix.        n_h
-000209e0: 6964 6465 6e3a 2069 6e74 2c20 6f70 7469  idden: int, opti
-000209f0: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
-00020a00: 204e 756d 6265 7220 6f66 206e 6f64 6573   Number of nodes
-00020a10: 2069 6e20 6869 6464 656e 206c 6179 6572   in hidden layer
-00020a20: 0a20 2020 2020 2020 2069 6e69 7469 616c  .        initial
-00020a30: 697a 6572 3a20 7374 722c 206f 7074 696f  izer: str, optio
-00020a40: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
-00020a50: 5765 6967 6874 2069 6e69 7469 616c 697a  Weight initializ
-00020a60: 6174 696f 6e20 666f 7220 6669 6c74 6572  ation for filter
-00020a70: 732e 0a20 2020 2020 2020 2020 2020 204f  s..            O
-00020a80: 7074 696f 6e73 3a20 7b78 6176 6965 725f  ptions: {xavier_
-00020a90: 756e 6966 6f72 6d5f 2c20 7861 7669 6572  uniform_, xavier
-00020aa0: 5f6e 6f72 6d61 6c5f 2c20 6b61 696d 696e  _normal_, kaimin
-00020ab0: 675f 756e 6966 6f72 6d5f 2c20 6b61 696d  g_uniform_, kaim
-00020ac0: 696e 675f 6e6f 726d 616c 5f2c 2074 7275  ing_normal_, tru
-00020ad0: 6e63 5f6e 6f72 6d61 6c5f 7d0a 2020 2020  nc_normal_}.    
-00020ae0: 2020 2020 6163 7469 7661 7469 6f6e 3a20      activation: 
-00020af0: 7374 722c 206f 7074 696f 6e61 6c0a 2020  str, optional.  
-00020b00: 2020 2020 2020 2020 2020 4163 7469 7661            Activa
-00020b10: 7469 6f6e 2066 756e 6374 696f 6e20 6170  tion function ap
-00020b20: 706c 6965 640a 0a20 2020 2020 2020 2022  plied..        "
-00020b30: 2222 0a20 2020 2020 2020 2073 7570 6572  "".        super
-00020b40: 2844 544e 4e53 7465 702c 2073 656c 6629  (DTNNStep, self)
-00020b50: 2e5f 5f69 6e69 745f 5f28 2a2a 6b77 6172  .__init__(**kwar
-00020b60: 6773 290a 2020 2020 2020 2020 7365 6c66  gs).        self
-00020b70: 2e6e 5f65 6d62 6564 6469 6e67 203d 206e  .n_embedding = n
-00020b80: 5f65 6d62 6564 6469 6e67 0a20 2020 2020  _embedding.     
-00020b90: 2020 2073 656c 662e 6e5f 6469 7374 616e     self.n_distan
-00020ba0: 6365 203d 206e 5f64 6973 7461 6e63 650a  ce = n_distance.
-00020bb0: 2020 2020 2020 2020 7365 6c66 2e6e 5f68          self.n_h
-00020bc0: 6964 6465 6e20 3d20 6e5f 6869 6464 656e  idden = n_hidden
-00020bd0: 0a20 2020 2020 2020 2073 656c 662e 696e  .        self.in
-00020be0: 6974 6961 6c69 7a65 7220 3d20 696e 6974  itializer = init
-00020bf0: 6961 6c69 7a65 7220 2023 2053 6574 2077  ializer  # Set w
-00020c00: 6569 6768 7420 696e 6974 6961 6c69 7a61  eight initializa
-00020c10: 7469 6f6e 0a20 2020 2020 2020 2073 656c  tion.        sel
-00020c20: 662e 6163 7469 7661 7469 6f6e 203d 2061  f.activation = a
-00020c30: 6374 6976 6174 696f 6e20 2023 2047 6574  ctivation  # Get
-00020c40: 2061 6374 6976 6174 696f 6e73 0a20 2020   activations.   
-00020c50: 2020 2020 2073 656c 662e 6163 7469 7661       self.activa
-00020c60: 7469 6f6e 5f66 6e20 3d20 6765 745f 6163  tion_fn = get_ac
-00020c70: 7469 7661 7469 6f6e 2873 656c 662e 6163  tivation(self.ac
-00020c80: 7469 7661 7469 6f6e 290a 0a20 2020 2020  tivation)..     
-00020c90: 2020 2069 6e69 745f 6675 6e63 3a20 4361     init_func: Ca
-00020ca0: 6c6c 6162 6c65 203d 2067 6574 6174 7472  llable = getattr
-00020cb0: 2869 6e69 7469 616c 697a 6572 732c 2073  (initializers, s
-00020cc0: 656c 662e 696e 6974 6961 6c69 7a65 7229  elf.initializer)
-00020cd0: 0a0a 2020 2020 2020 2020 7365 6c66 2e57  ..        self.W
-00020ce0: 5f63 6620 3d20 6e6e 2e50 6172 616d 6574  _cf = nn.Paramet
-00020cf0: 6572 280a 2020 2020 2020 2020 2020 2020  er(.            
-00020d00: 696e 6974 5f66 756e 6328 746f 7263 682e  init_func(torch.
-00020d10: 656d 7074 7928 5b73 656c 662e 6e5f 656d  empty([self.n_em
-00020d20: 6265 6464 696e 672c 2073 656c 662e 6e5f  bedding, self.n_
-00020d30: 6869 6464 656e 5d29 2929 0a20 2020 2020  hidden]))).     
-00020d40: 2020 2073 656c 662e 575f 6466 203d 206e     self.W_df = n
-00020d50: 6e2e 5061 7261 6d65 7465 7228 0a20 2020  n.Parameter(.   
-00020d60: 2020 2020 2020 2020 2069 6e69 745f 6675           init_fu
-00020d70: 6e63 2874 6f72 6368 2e65 6d70 7479 285b  nc(torch.empty([
-00020d80: 7365 6c66 2e6e 5f64 6973 7461 6e63 652c  self.n_distance,
-00020d90: 2073 656c 662e 6e5f 6869 6464 656e 5d29   self.n_hidden])
-00020da0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00020db0: 575f 6663 203d 206e 6e2e 5061 7261 6d65  W_fc = nn.Parame
-00020dc0: 7465 7228 0a20 2020 2020 2020 2020 2020  ter(.           
-00020dd0: 2069 6e69 745f 6675 6e63 2874 6f72 6368   init_func(torch
-00020de0: 2e65 6d70 7479 285b 7365 6c66 2e6e 5f68  .empty([self.n_h
-00020df0: 6964 6465 6e2c 2073 656c 662e 6e5f 656d  idden, self.n_em
-00020e00: 6265 6464 696e 675d 2929 290a 2020 2020  bedding]))).    
-00020e10: 2020 2020 7365 6c66 2e62 5f63 6620 3d20      self.b_cf = 
-00020e20: 6e6e 2e50 6172 616d 6574 6572 2874 6f72  nn.Parameter(tor
-00020e30: 6368 2e7a 6572 6f73 2873 697a 653d 5b0a  ch.zeros(size=[.
-00020e40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00020e50: 2e6e 5f68 6964 6465 6e2c 0a20 2020 2020  .n_hidden,.     
-00020e60: 2020 205d 2929 0a20 2020 2020 2020 2073     ])).        s
-00020e70: 656c 662e 625f 6466 203d 206e 6e2e 5061  elf.b_df = nn.Pa
-00020e80: 7261 6d65 7465 7228 746f 7263 682e 7a65  rameter(torch.ze
-00020e90: 726f 7328 7369 7a65 3d5b 0a20 2020 2020  ros(size=[.     
-00020ea0: 2020 2020 2020 2073 656c 662e 6e5f 6869         self.n_hi
-00020eb0: 6464 656e 2c0a 2020 2020 2020 2020 5d29  dden,.        ])
-00020ec0: 290a 0a20 2020 2064 6566 205f 5f72 6570  )..    def __rep
-00020ed0: 725f 5f28 7365 6c66 293a 0a20 2020 2020  r__(self):.     
-00020ee0: 2020 2022 2222 5265 7475 726e 7320 6120     """Returns a 
-00020ef0: 7374 7269 6e67 2072 6570 7265 7365 6e74  string represent
-00020f00: 696e 6720 7468 6520 636f 6e66 6967 7572  ing the configur
-00020f10: 6174 696f 6e20 6f66 2074 6865 206c 6179  ation of the lay
-00020f20: 6572 2e0a 0a20 2020 2020 2020 2052 6574  er...        Ret
-00020f30: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-00020f40: 2d2d 2d2d 0a20 2020 2020 2020 206e 5f65  ----.        n_e
-00020f50: 6d62 6564 6469 6e67 3a20 696e 742c 206f  mbedding: int, o
-00020f60: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-00020f70: 2020 2020 4e75 6d62 6572 206f 6620 6665      Number of fe
-00020f80: 6174 7572 6573 2066 6f72 2065 6163 6820  atures for each 
-00020f90: 6174 6f6d 0a20 2020 2020 2020 206e 5f64  atom.        n_d
-00020fa0: 6973 7461 6e63 653a 2069 6e74 2c20 6f70  istance: int, op
-00020fb0: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
-00020fc0: 2020 2067 7261 6e75 6c61 7269 7479 206f     granularity o
-00020fd0: 6620 6469 7374 616e 6365 206d 6174 7269  f distance matri
-00020fe0: 780a 2020 2020 2020 2020 6e5f 6869 6464  x.        n_hidd
-00020ff0: 656e 3a20 696e 742c 206f 7074 696f 6e61  en: int, optiona
-00021000: 6c0a 2020 2020 2020 2020 2020 2020 4e75  l.            Nu
-00021010: 6d62 6572 206f 6620 6e6f 6465 7320 696e  mber of nodes in
-00021020: 2068 6964 6465 6e20 6c61 7965 720a 2020   hidden layer.  
-00021030: 2020 2020 2020 696e 6974 6961 6c69 7a65        initialize
-00021040: 723a 2073 7472 2c20 6f70 7469 6f6e 616c  r: str, optional
-00021050: 0a20 2020 2020 2020 2020 2020 2057 6569  .            Wei
-00021060: 6768 7420 696e 6974 6961 6c69 7a61 7469  ght initializati
-00021070: 6f6e 2066 6f72 2066 696c 7465 7273 2e0a  on for filters..
-00021080: 2020 2020 2020 2020 2020 2020 4f70 7469              Opti
-00021090: 6f6e 733a 207b 7861 7669 6572 5f75 6e69  ons: {xavier_uni
-000210a0: 666f 726d 5f2c 2078 6176 6965 725f 6e6f  form_, xavier_no
-000210b0: 726d 616c 5f2c 206b 6169 6d69 6e67 5f75  rmal_, kaiming_u
-000210c0: 6e69 666f 726d 5f2c 206b 6169 6d69 6e67  niform_, kaiming
-000210d0: 5f6e 6f72 6d61 6c5f 2c20 7472 756e 635f  _normal_, trunc_
-000210e0: 6e6f 726d 616c 5f7d 0a20 2020 2020 2020  normal_}.       
-000210f0: 2061 6374 6976 6174 696f 6e3a 2073 7472   activation: str
-00021100: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-00021110: 2020 2020 2020 2041 6374 6976 6174 696f         Activatio
-00021120: 6e20 6675 6e63 7469 6f6e 2061 7070 6c69  n function appli
-00021130: 6564 0a0a 2020 2020 2020 2020 2222 220a  ed..        """.
-00021140: 2020 2020 2020 2020 7265 7475 726e 2066          return f
-00021150: 277b 7365 6c66 2e5f 5f63 6c61 7373 5f5f  '{self.__class__
-00021160: 2e5f 5f6e 616d 655f 5f7d 286e 5f65 6d62  .__name__}(n_emb
-00021170: 6564 6469 6e67 3d7b 7365 6c66 2e6e 5f65  edding={self.n_e
-00021180: 6d62 6564 6469 6e67 7d2c 206e 5f64 6973  mbedding}, n_dis
-00021190: 7461 6e63 653d 7b73 656c 662e 6e5f 6469  tance={self.n_di
-000211a0: 7374 616e 6365 7d2c 206e 5f68 6964 6465  stance}, n_hidde
-000211b0: 6e3d 7b73 656c 662e 6e5f 6869 6464 656e  n={self.n_hidden
-000211c0: 7d2c 2069 6e69 7469 616c 697a 6572 3d7b  }, initializer={
-000211d0: 7365 6c66 2e69 6e69 7469 616c 697a 6572  self.initializer
-000211e0: 7d2c 2061 6374 6976 6174 696f 6e3d 7b73  }, activation={s
-000211f0: 656c 662e 6163 7469 7661 7469 6f6e 7d29  elf.activation})
-00021200: 270a 0a20 2020 2064 6566 2066 6f72 7761  '..    def forwa
-00021210: 7264 2873 656c 662c 2069 6e70 7574 7329  rd(self, inputs)
-00021220: 3a0a 2020 2020 2020 2020 2222 2245 7865  :.        """Exe
-00021230: 6375 7465 7320 7468 6520 6571 7561 7469  cutes the equati
-00021240: 6f6e 7320 616e 6420 5265 7475 726e 7320  ons and Returns 
-00021250: 7468 6520 696e 7472 6163 7469 6f6e 2076  the intraction v
-00021260: 6563 746f 7220 6f66 2074 6865 2061 746f  ector of the ato
-00021270: 6d20 7769 7468 206f 7468 6572 2061 746f  m with other ato
-00021280: 6d73 2e0a 0a20 2020 2020 2020 2050 6172  ms...        Par
-00021290: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-000212a0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-000212b0: 2020 2069 6e70 7574 733a 2074 6f72 6368     inputs: torch
-000212c0: 2e54 656e 736f 720a 2020 2020 2020 2020  .Tensor.        
-000212d0: 2020 2020 4c69 7374 206f 6620 5465 6e73      List of Tens
-000212e0: 6f72 7320 6861 7669 6e67 2061 746f 6d5f  ors having atom_
-000212f0: 6665 6174 7572 6573 2c20 6469 7374 616e  features, distan
-00021300: 6365 2c20 6469 7374 616e 6365 5f6d 656d  ce, distance_mem
-00021310: 6265 7273 6869 705f 692c 2064 6973 7461  bership_i, dista
-00021320: 6e63 655f 6d65 6d62 6572 7368 6970 5f6a  nce_membership_j
-00021330: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00021340: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
-00021350: 2d2d 0a20 2020 2020 2020 2069 6e74 6572  --.        inter
-00021360: 6163 7469 6f6e 5f76 6563 746f 723a 2074  action_vector: t
-00021370: 6f72 6368 2e54 656e 736f 720a 2020 2020  orch.Tensor.    
-00021380: 2020 2020 2020 2020 696e 7465 7261 6374          interact
-00021390: 696f 6e20 6f66 2074 6865 2061 746f 6d20  ion of the atom 
-000213a0: 7769 7468 206f 7468 6572 2061 746f 6d73  with other atoms
-000213b0: 2062 6173 6564 206f 6e20 6469 7374 616e   based on distan
-000213c0: 6365 2061 6e64 2064 6973 7461 6e63 655f  ce and distance_
-000213d0: 6d65 6d62 6572 7368 6970 2e0a 0a20 2020  membership...   
-000213e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000213f0: 2061 746f 6d5f 6665 6174 7572 6573 203d   atom_features =
-00021400: 2069 6e70 7574 735b 305d 0a20 2020 2020   inputs[0].     
-00021410: 2020 2064 6973 7461 6e63 6520 3d20 696e     distance = in
-00021420: 7075 7473 5b31 5d0a 2020 2020 2020 2020  puts[1].        
-00021430: 6469 7374 616e 6365 5f6d 656d 6265 7273  distance_members
-00021440: 6869 705f 6920 3d20 696e 7075 7473 5b32  hip_i = inputs[2
-00021450: 5d0a 2020 2020 2020 2020 6469 7374 616e  ].        distan
-00021460: 6365 5f6d 656d 6265 7273 6869 705f 6a20  ce_membership_j 
-00021470: 3d20 696e 7075 7473 5b33 5d0a 2020 2020  = inputs[3].    
-00021480: 2020 2020 6469 7374 616e 6365 5f68 6964      distance_hid
-00021490: 6465 6e20 3d20 746f 7263 682e 6d61 746d  den = torch.matm
-000214a0: 756c 2864 6973 7461 6e63 652c 2073 656c  ul(distance, sel
-000214b0: 662e 575f 6466 2920 2b20 7365 6c66 2e62  f.W_df) + self.b
-000214c0: 5f64 660a 2020 2020 2020 2020 6174 6f6d  _df.        atom
-000214d0: 5f66 6561 7475 7265 735f 6869 6464 656e  _features_hidden
-000214e0: 203d 2074 6f72 6368 2e6d 6174 6d75 6c28   = torch.matmul(
-000214f0: 6174 6f6d 5f66 6561 7475 7265 732c 0a20  atom_features,. 
-00021500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021520: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00021530: 575f 6366 2920 2b20 7365 6c66 2e62 5f63  W_cf) + self.b_c
-00021540: 660a 2020 2020 2020 2020 6f75 7470 7574  f.        output
-00021550: 7320 3d20 746f 7263 682e 6d75 6c28 0a20  s = torch.mul(. 
-00021560: 2020 2020 2020 2020 2020 2064 6973 7461             dista
-00021570: 6e63 655f 6869 6464 656e 2c0a 2020 2020  nce_hidden,.    
-00021580: 2020 2020 2020 2020 746f 7263 682e 656d          torch.em
-00021590: 6265 6464 696e 6728 6174 6f6d 5f66 6561  bedding(atom_fea
-000215a0: 7475 7265 735f 6869 6464 656e 2c20 6469  tures_hidden, di
-000215b0: 7374 616e 6365 5f6d 656d 6265 7273 6869  stance_membershi
-000215c0: 705f 6a29 290a 0a20 2020 2020 2020 2023  p_j))..        #
-000215d0: 2066 6f72 2061 746f 6d20 6920 696e 2061   for atom i in a
-000215e0: 206d 6f6c 6563 756c 6520 6d2c 2074 6869   molecule m, thi
-000215f0: 7320 7374 6570 206d 756c 7469 706c 6965  s step multiplie
-00021600: 7320 746f 6765 7468 6572 2064 6973 7461  s together dista
-00021610: 6e63 6520 696e 666f 206f 6620 6174 6f6d  nce info of atom
-00021620: 2070 6169 7228 692c 6a29 0a20 2020 2020   pair(i,j).     
-00021630: 2020 2023 2061 6e64 2065 6d62 6564 6469     # and embeddi
-00021640: 6e67 7320 6f66 2061 746f 6d20 6a28 626f  ngs of atom j(bo
-00021650: 7468 2067 6f6e 6520 7468 726f 7567 6820  th gone through 
-00021660: 6120 6869 6464 656e 206c 6179 6572 290a  a hidden layer).
-00021670: 2020 2020 2020 2020 6f75 7470 7574 7320          outputs 
-00021680: 3d20 746f 7263 682e 6d61 746d 756c 286f  = torch.matmul(o
-00021690: 7574 7075 7473 2c20 7365 6c66 2e57 5f66  utputs, self.W_f
-000216a0: 6329 0a20 2020 2020 2020 206f 7574 7075  c).        outpu
-000216b0: 7473 203d 2073 656c 662e 6163 7469 7661  ts = self.activa
-000216c0: 7469 6f6e 5f66 6e28 6f75 7470 7574 7329  tion_fn(outputs)
-000216d0: 0a0a 2020 2020 2020 2020 6f75 7470 7574  ..        output
-000216e0: 5f69 6920 3d20 746f 7263 682e 6d75 6c28  _ii = torch.mul(
-000216f0: 7365 6c66 2e62 5f64 662c 2061 746f 6d5f  self.b_df, atom_
-00021700: 6665 6174 7572 6573 5f68 6964 6465 6e29  features_hidden)
-00021710: 0a20 2020 2020 2020 206f 7574 7075 745f  .        output_
-00021720: 6969 203d 2074 6f72 6368 2e6d 6174 6d75  ii = torch.matmu
-00021730: 6c28 6f75 7470 7574 5f69 692c 2073 656c  l(output_ii, sel
-00021740: 662e 575f 6663 290a 2020 2020 2020 2020  f.W_fc).        
-00021750: 6f75 7470 7574 5f69 6920 3d20 7365 6c66  output_ii = self
-00021760: 2e61 6374 6976 6174 696f 6e5f 666e 286f  .activation_fn(o
-00021770: 7574 7075 745f 6969 290a 0a20 2020 2020  utput_ii)..     
-00021780: 2020 2023 2066 6f72 2061 746f 6d20 692c     # for atom i,
-00021790: 2073 756d 2074 6865 2069 6e66 6c75 656e   sum the influen
-000217a0: 6365 2066 726f 6d20 616c 6c20 6f74 6865  ce from all othe
-000217b0: 7220 6174 6f6d 206a 2069 6e20 7468 6520  r atom j in the 
-000217c0: 6d6f 6c65 6375 6c65 0a20 2020 2020 2020  molecule.       
-000217d0: 2069 6e74 7261 6374 696f 6e5f 7665 6374   intraction_vect
-000217e0: 6f72 203d 2073 6361 7474 6572 286f 7574  or = scatter(out
-000217f0: 7075 7473 2c20 6469 7374 616e 6365 5f6d  puts, distance_m
-00021800: 656d 6265 7273 6869 705f 692c 0a20 2020  embership_i,.   
-00021810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021830: 2064 696d 3d30 2920 2d20 6f75 7470 7574   dim=0) - output
-00021840: 5f69 6920 2b20 6174 6f6d 5f66 6561 7475  _ii + atom_featu
-00021850: 7265 730a 2020 2020 2020 2020 7265 7475  res.        retu
-00021860: 726e 2069 6e74 7261 6374 696f 6e5f 7665  rn intraction_ve
-00021870: 6374 6f72 0a0a 0a63 6c61 7373 2044 544e  ctor...class DTN
-00021880: 4e47 6174 6865 7228 6e6e 2e4d 6f64 756c  NGather(nn.Modul
-00021890: 6529 3a0a 2020 2020 2222 2244 544e 4e47  e):.    """DTNNG
-000218a0: 6174 6865 7220 4c61 7965 7220 666f 7220  ather Layer for 
-000218b0: 4454 4e4e 204d 6f64 656c 2e0a 0a20 2020  DTNN Model...   
-000218c0: 2050 7265 6469 6374 204d 6f6c 6563 756c   Predict Molecul
-000218d0: 6172 2045 6e65 7267 7920 7573 696e 6720  ar Energy using 
-000218e0: 6174 6f6d 5f66 6561 7475 7265 7320 616e  atom_features an
-000218f0: 6420 6174 6f6d 5f6d 656d 6265 7273 6869  d atom_membershi
-00021900: 702e 205b 315d 5f0a 0a20 2020 2054 6869  p. [1]_..    Thi
-00021910: 7320 4c61 7965 7220 6761 7468 6572 7320  s Layer gathers 
-00021920: 7468 6520 696e 7075 7473 2067 6f74 2066  the inputs got f
-00021930: 726f 6d20 7468 6520 7374 6570 206c 6179  rom the step lay
-00021940: 6572 2061 6363 6f72 6469 6e67 2074 6f20  er according to 
-00021950: 6174 6f6d 5f6d 656d 6265 7273 6869 7020  atom_membership 
-00021960: 616e 6420 6361 6c75 6c61 7465 7320 7468  and calulates th
-00021970: 6520 746f 7461 6c20 4d6f 6c65 6375 6c61  e total Molecula
-00021980: 7220 456e 6572 6779 2e0a 0a20 2020 2052  r Energy...    R
-00021990: 6566 6572 656e 6365 730a 2020 2020 2d2d  eferences.    --
-000219a0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 205b 315d  --------.    [1]
-000219b0: 2053 6368 c3bc 7474 2c20 4b72 6973 746f   Sch..tt, Kristo
-000219c0: 6620 542e 2c20 6574 2061 6c2e 2022 5175  f T., et al. "Qu
-000219d0: 616e 7475 6d2d 6368 656d 6963 616c 2069  antum-chemical i
-000219e0: 6e73 6967 6874 7320 6672 6f6d 2064 6565  nsights from dee
-000219f0: 700a 2020 2020 2020 2020 7465 6e73 6f72  p.        tensor
-00021a00: 206e 6575 7261 6c20 6e65 7477 6f72 6b73   neural networks
-00021a10: 2e22 204e 6174 7572 6520 636f 6d6d 756e  ." Nature commun
-00021a20: 6963 6174 696f 6e73 2038 2e31 2028 3230  ications 8.1 (20
-00021a30: 3137 293a 2031 2d38 2e0a 0a20 2020 2045  17): 1-8...    E
-00021a40: 7861 6d70 6c65 730a 2020 2020 2d2d 2d2d  xamples.    ----
-00021a50: 2d2d 2d2d 0a20 2020 203e 3e3e 2066 726f  ----.    >>> fro
-00021a60: 6d20 6465 6570 6368 656d 2e6d 6f64 656c  m deepchem.model
-00021a70: 732e 746f 7263 685f 6d6f 6465 6c73 2069  s.torch_models i
-00021a80: 6d70 6f72 7420 6c61 7965 7273 2061 7320  mport layers as 
-00021a90: 6c61 7965 7273 5f74 6f72 6368 0a20 2020  layers_torch.   
-00021aa0: 203e 3e3e 2069 6d70 6f72 7420 746f 7263   >>> import torc
-00021ab0: 680a 2020 2020 3e3e 3e20 6761 7468 6572  h.    >>> gather
-00021ac0: 5f6c 6179 6572 5f74 6f72 6368 203d 206c  _layer_torch = l
-00021ad0: 6179 6572 735f 746f 7263 682e 4454 4e4e  ayers_torch.DTNN
-00021ae0: 4761 7468 6572 2833 2c20 332c 205b 3130  Gather(3, 3, [10
-00021af0: 5d29 0a20 2020 203e 3e3e 2072 6573 756c  ]).    >>> resul
-00021b00: 7420 3d20 6761 7468 6572 5f6c 6179 6572  t = gather_layer
-00021b10: 5f74 6f72 6368 285b 746f 7263 682e 5465  _torch([torch.Te
-00021b20: 6e73 6f72 285b 5b33 2c20 322c 2031 5d5d  nsor([[3, 2, 1]]
-00021b30: 292e 746f 2874 6f72 6368 2e66 6c6f 6174  ).to(torch.float
-00021b40: 3332 292c 2074 6f72 6368 2e54 656e 736f  32), torch.Tenso
-00021b50: 7228 5b30 5d29 2e74 6f28 746f 7263 682e  r([0]).to(torch.
-00021b60: 696e 7436 3429 5d29 0a20 2020 203e 3e3e  int64)]).    >>>
-00021b70: 2072 6573 756c 742e 7368 6170 650a 2020   result.shape.  
-00021b80: 2020 746f 7263 682e 5369 7a65 285b 312c    torch.Size([1,
-00021b90: 2033 5d29 0a0a 2020 2020 2222 220a 0a20   3])..    """.. 
-00021ba0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00021bb0: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
-00021bc0: 2020 2020 2020 206e 5f65 6d62 6564 6469         n_embeddi
-00021bd0: 6e67 3d33 302c 0a20 2020 2020 2020 2020  ng=30,.         
-00021be0: 2020 2020 2020 2020 6e5f 6f75 7470 7574          n_output
-00021bf0: 733d 3130 302c 0a20 2020 2020 2020 2020  s=100,.         
-00021c00: 2020 2020 2020 2020 6c61 7965 725f 7369          layer_si
-00021c10: 7a65 733d 5b31 3030 5d2c 0a20 2020 2020  zes=[100],.     
-00021c20: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
-00021c30: 7574 5f61 6374 6976 6174 696f 6e3d 5472  ut_activation=Tr
-00021c40: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00021c50: 2020 2020 2069 6e69 7469 616c 697a 6572       initializer
-00021c60: 3d27 7861 7669 6572 5f75 6e69 666f 726d  ='xavier_uniform
-00021c70: 5f27 2c0a 2020 2020 2020 2020 2020 2020  _',.            
-00021c80: 2020 2020 2061 6374 6976 6174 696f 6e3d       activation=
-00021c90: 2774 616e 6827 2c0a 2020 2020 2020 2020  'tanh',.        
-00021ca0: 2020 2020 2020 2020 202a 2a6b 7761 7267           **kwarg
-00021cb0: 7329 3a0a 2020 2020 2020 2020 2222 220a  s):.        """.
-00021cc0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00021cd0: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-00021ce0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6e5f  -----.        n_
-00021cf0: 656d 6265 6464 696e 673a 2069 6e74 2c20  embedding: int, 
-00021d00: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-00021d10: 2020 2020 204e 756d 6265 7220 6f66 2066       Number of f
-00021d20: 6561 7475 7265 7320 666f 7220 6561 6368  eatures for each
-00021d30: 2061 746f 6d0a 2020 2020 2020 2020 6e5f   atom.        n_
-00021d40: 6f75 7470 7574 733a 2069 6e74 2c20 6f70  outputs: int, op
-00021d50: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
-00021d60: 2020 204e 756d 6265 7220 6f66 2066 6561     Number of fea
-00021d70: 7475 7265 7320 666f 7220 6561 6368 206d  tures for each m
-00021d80: 6f6c 6563 756c 6528 6f75 7470 7574 290a  olecule(output).
-00021d90: 2020 2020 2020 2020 6c61 7965 725f 7369          layer_si
-00021da0: 7a65 733a 206c 6973 7420 6f66 2069 6e74  zes: list of int
-00021db0: 2c20 6f70 7469 6f6e 616c 2864 6566 6175  , optional(defau
-00021dc0: 6c74 3d5b 3130 3030 5d29 0a20 2020 2020  lt=[1000]).     
-00021dd0: 2020 2020 2020 2053 7472 7563 7475 7265         Structure
-00021de0: 206f 6620 6869 6464 656e 206c 6179 6572   of hidden layer
-00021df0: 2873 290a 2020 2020 2020 2020 696e 6974  (s).        init
-00021e00: 6961 6c69 7a65 723a 2073 7472 2c20 6f70  ializer: str, op
-00021e10: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
-00021e20: 2020 2057 6569 6768 7420 696e 6974 6961     Weight initia
-00021e30: 6c69 7a61 7469 6f6e 2066 6f72 2066 696c  lization for fil
-00021e40: 7465 7273 2e0a 2020 2020 2020 2020 6163  ters..        ac
-00021e50: 7469 7661 7469 6f6e 3a20 7374 722c 206f  tivation: str, o
-00021e60: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-00021e70: 2020 2020 4163 7469 7661 7469 6f6e 2066      Activation f
-00021e80: 756e 6374 696f 6e20 6170 706c 6965 640a  unction applied.
-00021e90: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
-00021ea0: 2020 2020 2020 7375 7065 7228 4454 4e4e        super(DTNN
-00021eb0: 4761 7468 6572 2c20 7365 6c66 292e 5f5f  Gather, self).__
-00021ec0: 696e 6974 5f5f 282a 2a6b 7761 7267 7329  init__(**kwargs)
-00021ed0: 0a20 2020 2020 2020 2073 656c 662e 6e5f  .        self.n_
-00021ee0: 656d 6265 6464 696e 6720 3d20 6e5f 656d  embedding = n_em
-00021ef0: 6265 6464 696e 670a 2020 2020 2020 2020  bedding.        
-00021f00: 7365 6c66 2e6e 5f6f 7574 7075 7473 203d  self.n_outputs =
-00021f10: 206e 5f6f 7574 7075 7473 0a20 2020 2020   n_outputs.     
-00021f20: 2020 2073 656c 662e 6c61 7965 725f 7369     self.layer_si
-00021f30: 7a65 7320 3d20 6c61 7965 725f 7369 7a65  zes = layer_size
-00021f40: 730a 2020 2020 2020 2020 7365 6c66 2e6f  s.        self.o
-00021f50: 7574 7075 745f 6163 7469 7661 7469 6f6e  utput_activation
-00021f60: 203d 206f 7574 7075 745f 6163 7469 7661   = output_activa
-00021f70: 7469 6f6e 0a20 2020 2020 2020 2073 656c  tion.        sel
-00021f80: 662e 696e 6974 6961 6c69 7a65 7220 3d20  f.initializer = 
-00021f90: 696e 6974 6961 6c69 7a65 7220 2023 2053  initializer  # S
-00021fa0: 6574 2077 6569 6768 7420 696e 6974 6961  et weight initia
-00021fb0: 6c69 7a61 7469 6f6e 0a20 2020 2020 2020  lization.       
-00021fc0: 2073 656c 662e 6163 7469 7661 7469 6f6e   self.activation
-00021fd0: 203d 2061 6374 6976 6174 696f 6e20 2023   = activation  #
-00021fe0: 2047 6574 2061 6374 6976 6174 696f 6e73   Get activations
-00021ff0: 0a20 2020 2020 2020 2073 656c 662e 6163  .        self.ac
-00022000: 7469 7661 7469 6f6e 5f66 6e20 3d20 6765  tivation_fn = ge
-00022010: 745f 6163 7469 7661 7469 6f6e 2873 656c  t_activation(sel
-00022020: 662e 6163 7469 7661 7469 6f6e 290a 0a20  f.activation).. 
-00022030: 2020 2020 2020 2073 656c 662e 575f 6c69         self.W_li
-00022040: 7374 203d 206e 6e2e 5061 7261 6d65 7465  st = nn.Paramete
-00022050: 724c 6973 7428 290a 2020 2020 2020 2020  rList().        
-00022060: 7365 6c66 2e62 5f6c 6973 7420 3d20 6e6e  self.b_list = nn
-00022070: 2e50 6172 616d 6574 6572 4c69 7374 2829  .ParameterList()
-00022080: 0a0a 2020 2020 2020 2020 696e 6974 5f66  ..        init_f
-00022090: 756e 633a 2043 616c 6c61 626c 6520 3d20  unc: Callable = 
-000220a0: 6765 7461 7474 7228 696e 6974 6961 6c69  getattr(initiali
-000220b0: 7a65 7273 2c20 7365 6c66 2e69 6e69 7469  zers, self.initi
-000220c0: 616c 697a 6572 290a 0a20 2020 2020 2020  alizer)..       
-000220d0: 2070 7265 765f 6c61 7965 725f 7369 7a65   prev_layer_size
-000220e0: 203d 2073 656c 662e 6e5f 656d 6265 6464   = self.n_embedd
-000220f0: 696e 670a 2020 2020 2020 2020 666f 7220  ing.        for 
-00022100: 692c 206c 6179 6572 5f73 697a 6520 696e  i, layer_size in
-00022110: 2065 6e75 6d65 7261 7465 2873 656c 662e   enumerate(self.
-00022120: 6c61 7965 725f 7369 7a65 7329 3a0a 2020  layer_sizes):.  
-00022130: 2020 2020 2020 2020 2020 7365 6c66 2e57            self.W
-00022140: 5f6c 6973 742e 6170 7065 6e64 280a 2020  _list.append(.  
-00022150: 2020 2020 2020 2020 2020 2020 2020 6e6e                nn
-00022160: 2e50 6172 616d 6574 6572 280a 2020 2020  .Parameter(.    
-00022170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022180: 696e 6974 5f66 756e 6328 746f 7263 682e  init_func(torch.
-00022190: 656d 7074 7928 5b70 7265 765f 6c61 7965  empty([prev_laye
-000221a0: 725f 7369 7a65 2c20 6c61 7965 725f 7369  r_size, layer_si
-000221b0: 7a65 5d29 2929 290a 2020 2020 2020 2020  ze])))).        
-000221c0: 2020 2020 7365 6c66 2e62 5f6c 6973 742e      self.b_list.
-000221d0: 6170 7065 6e64 286e 6e2e 5061 7261 6d65  append(nn.Parame
-000221e0: 7465 7228 746f 7263 682e 7a65 726f 7328  ter(torch.zeros(
-000221f0: 7369 7a65 3d5b 0a20 2020 2020 2020 2020  size=[.         
-00022200: 2020 2020 2020 206c 6179 6572 5f73 697a         layer_siz
-00022210: 652c 0a20 2020 2020 2020 2020 2020 205d  e,.            ]
-00022220: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
-00022230: 7072 6576 5f6c 6179 6572 5f73 697a 6520  prev_layer_size 
-00022240: 3d20 6c61 7965 725f 7369 7a65 0a20 2020  = layer_size.   
-00022250: 2020 2020 2073 656c 662e 575f 6c69 7374       self.W_list
-00022260: 2e61 7070 656e 6428 0a20 2020 2020 2020  .append(.       
-00022270: 2020 2020 206e 6e2e 5061 7261 6d65 7465       nn.Paramete
-00022280: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-00022290: 2020 2069 6e69 745f 6675 6e63 2874 6f72     init_func(tor
-000222a0: 6368 2e65 6d70 7479 285b 7072 6576 5f6c  ch.empty([prev_l
-000222b0: 6179 6572 5f73 697a 652c 2073 656c 662e  ayer_size, self.
-000222c0: 6e5f 6f75 7470 7574 735d 2929 2929 0a20  n_outputs])))). 
-000222d0: 2020 2020 2020 2073 656c 662e 625f 6c69         self.b_li
-000222e0: 7374 2e61 7070 656e 6428 6e6e 2e50 6172  st.append(nn.Par
-000222f0: 616d 6574 6572 2874 6f72 6368 2e7a 6572  ameter(torch.zer
-00022300: 6f73 2873 697a 653d 5b0a 2020 2020 2020  os(size=[.      
-00022310: 2020 2020 2020 7365 6c66 2e6e 5f6f 7574        self.n_out
-00022320: 7075 7473 2c0a 2020 2020 2020 2020 5d29  puts,.        ])
-00022330: 2929 0a0a 2020 2020 6465 6620 5f5f 7265  ))..    def __re
-00022340: 7072 5f5f 2873 656c 6629 3a0a 2020 2020  pr__(self):.    
-00022350: 2020 2020 2222 2252 6574 7572 6e73 2061      """Returns a
-00022360: 2073 7472 696e 6720 7265 7072 6573 656e   string represen
-00022370: 7469 6e67 2074 6865 2063 6f6e 6669 6775  ting the configu
-00022380: 7261 7469 6f6e 206f 6620 7468 6520 6c61  ration of the la
-00022390: 7965 722e 0a0a 2020 2020 2020 2020 5265  yer...        Re
-000223a0: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
-000223b0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-000223c0: 206e 5f65 6d62 6564 6469 6e67 3a20 696e   n_embedding: in
-000223d0: 742c 206f 7074 696f 6e61 6c0a 2020 2020  t, optional.    
-000223e0: 2020 2020 2020 2020 4e75 6d62 6572 206f          Number o
-000223f0: 6620 6665 6174 7572 6573 2066 6f72 2065  f features for e
-00022400: 6163 6820 6174 6f6d 0a20 2020 2020 2020  ach atom.       
-00022410: 206e 5f6f 7574 7075 7473 3a20 696e 742c   n_outputs: int,
-00022420: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-00022430: 2020 2020 2020 4e75 6d62 6572 206f 6620        Number of 
-00022440: 6665 6174 7572 6573 2066 6f72 2065 6163  features for eac
-00022450: 6820 6d6f 6c65 6375 6c65 286f 7574 7075  h molecule(outpu
-00022460: 7429 0a20 2020 2020 2020 206c 6179 6572  t).        layer
-00022470: 5f73 697a 6573 3a20 6c69 7374 206f 6620  _sizes: list of 
-00022480: 696e 742c 206f 7074 696f 6e61 6c28 6465  int, optional(de
-00022490: 6661 756c 743d 5b31 3030 305d 290a 2020  fault=[1000]).  
-000224a0: 2020 2020 2020 2020 2020 5374 7275 6374            Struct
-000224b0: 7572 6520 6f66 2068 6964 6465 6e20 6c61  ure of hidden la
-000224c0: 7965 7228 7329 0a20 2020 2020 2020 2069  yer(s).        i
-000224d0: 6e69 7469 616c 697a 6572 3a20 7374 722c  nitializer: str,
-000224e0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-000224f0: 2020 2020 2020 5765 6967 6874 2069 6e69        Weight ini
-00022500: 7469 616c 697a 6174 696f 6e20 666f 7220  tialization for 
-00022510: 6669 6c74 6572 732e 0a20 2020 2020 2020  filters..       
-00022520: 2061 6374 6976 6174 696f 6e3a 2073 7472   activation: str
-00022530: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-00022540: 2020 2020 2020 2041 6374 6976 6174 696f         Activatio
-00022550: 6e20 6675 6e63 7469 6f6e 2061 7070 6c69  n function appli
-00022560: 6564 0a0a 2020 2020 2020 2020 2222 220a  ed..        """.
-00022570: 2020 2020 2020 2020 7265 7475 726e 2066          return f
-00022580: 277b 7365 6c66 2e5f 5f63 6c61 7373 5f5f  '{self.__class__
-00022590: 2e5f 5f6e 616d 655f 5f7d 286e 5f65 6d62  .__name__}(n_emb
-000225a0: 6564 6469 6e67 3d7b 7365 6c66 2e6e 5f65  edding={self.n_e
-000225b0: 6d62 6564 6469 6e67 7d2c 206e 5f6f 7574  mbedding}, n_out
-000225c0: 7075 7473 3d7b 7365 6c66 2e6e 5f6f 7574  puts={self.n_out
-000225d0: 7075 7473 7d2c 206c 6179 6572 5f73 697a  puts}, layer_siz
-000225e0: 6573 3d7b 7365 6c66 2e6c 6179 6572 5f73  es={self.layer_s
-000225f0: 697a 6573 7d2c 206f 7574 7075 745f 6163  izes}, output_ac
-00022600: 7469 7661 7469 6f6e 3d7b 7365 6c66 2e6f  tivation={self.o
-00022610: 7574 7075 745f 6163 7469 7661 7469 6f6e  utput_activation
-00022620: 7d2c 2069 6e69 7469 616c 697a 6572 3d7b  }, initializer={
-00022630: 7365 6c66 2e69 6e69 7469 616c 697a 6572  self.initializer
-00022640: 7d2c 2061 6374 6976 6174 696f 6e3d 7b73  }, activation={s
-00022650: 656c 662e 6163 7469 7661 7469 6f6e 7d29  elf.activation})
-00022660: 270a 0a20 2020 2064 6566 2066 6f72 7761  '..    def forwa
-00022670: 7264 2873 656c 662c 2069 6e70 7574 7329  rd(self, inputs)
-00022680: 3a0a 2020 2020 2020 2020 2222 2245 7865  :.        """Exe
-00022690: 6375 7465 7320 7468 6520 6571 7561 7469  cutes the equati
-000226a0: 6f6e 2061 6e64 2052 6574 7572 6e73 204d  on and Returns M
-000226b0: 6f6c 6563 756c 6172 2045 6e65 7267 6965  olecular Energie
-000226c0: 7320 6163 636f 7264 696e 6720 746f 2061  s according to a
-000226d0: 746f 6d5f 6d65 6d62 6572 7368 6970 2e0a  tom_membership..
-000226e0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-000226f0: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-00022700: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2069  ------.        i
-00022710: 6e70 7574 733a 2074 6f72 6368 2e54 656e  nputs: torch.Ten
-00022720: 736f 720a 2020 2020 2020 2020 2020 2020  sor.            
-00022730: 4c69 7374 206f 6620 5465 6e73 6f72 2063  List of Tensor c
-00022740: 6f6e 7461 696e 696e 6720 6174 6f6d 5f66  ontaining atom_f
-00022750: 6561 7475 7265 7320 616e 6420 6174 6f6d  eatures and atom
-00022760: 5f6d 656d 6265 7273 6869 700a 0a20 2020  _membership..   
-00022770: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
-00022780: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
-00022790: 2020 2020 206d 6f6c 6563 756c 6172 5f65       molecular_e
-000227a0: 6e65 7267 6965 733a 2074 6f72 6368 2e54  nergies: torch.T
-000227b0: 656e 736f 720a 2020 2020 2020 2020 2020  ensor.          
-000227c0: 2020 5465 6e73 6f72 2063 6f6e 7461 696e    Tensor contain
-000227d0: 696e 6720 7468 6520 4d6f 6c65 6375 6c61  ing the Molecula
-000227e0: 7220 456e 6572 6769 6573 2061 6363 6f72  r Energies accor
-000227f0: 6469 6e67 2074 6f20 6174 6f6d 5f6d 656d  ding to atom_mem
-00022800: 6265 7273 6869 702e 0a0a 2020 2020 2020  bership...      
-00022810: 2020 2222 220a 2020 2020 2020 2020 6f75    """.        ou
-00022820: 7470 7574 203d 2069 6e70 7574 735b 305d  tput = inputs[0]
-00022830: 0a20 2020 2020 2020 2061 746f 6d5f 6d65  .        atom_me
-00022840: 6d62 6572 7368 6970 203d 2069 6e70 7574  mbership = input
-00022850: 735b 315d 0a0a 2020 2020 2020 2020 666f  s[1]..        fo
-00022860: 7220 692c 2057 2069 6e20 656e 756d 6572  r i, W in enumer
-00022870: 6174 6528 7365 6c66 2e57 5f6c 6973 745b  ate(self.W_list[
-00022880: 3a2d 315d 293a 0a20 2020 2020 2020 2020  :-1]):.         
-00022890: 2020 206f 7574 7075 7420 3d20 746f 7263     output = torc
-000228a0: 682e 6d61 746d 756c 286f 7574 7075 742c  h.matmul(output,
-000228b0: 2057 2920 2b20 7365 6c66 2e62 5f6c 6973   W) + self.b_lis
-000228c0: 745b 695d 0a20 2020 2020 2020 2020 2020  t[i].           
-000228d0: 206f 7574 7075 7420 3d20 7365 6c66 2e61   output = self.a
-000228e0: 6374 6976 6174 696f 6e5f 666e 286f 7574  ctivation_fn(out
-000228f0: 7075 7429 0a20 2020 2020 2020 206f 7574  put).        out
-00022900: 7075 7420 3d20 746f 7263 682e 6d61 746d  put = torch.matm
-00022910: 756c 286f 7574 7075 742c 2073 656c 662e  ul(output, self.
-00022920: 575f 6c69 7374 5b2d 315d 2920 2b20 7365  W_list[-1]) + se
-00022930: 6c66 2e62 5f6c 6973 745b 2d31 5d0a 2020  lf.b_list[-1].  
-00022940: 2020 2020 2020 6966 2073 656c 662e 6f75        if self.ou
-00022950: 7470 7574 5f61 6374 6976 6174 696f 6e3a  tput_activation:
-00022960: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
-00022970: 7075 7420 3d20 7365 6c66 2e61 6374 6976  put = self.activ
-00022980: 6174 696f 6e5f 666e 286f 7574 7075 7429  ation_fn(output)
-00022990: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000229a0: 7363 6174 7465 7228 6f75 7470 7574 2c20  scatter(output, 
-000229b0: 6174 6f6d 5f6d 656d 6265 7273 6869 7029  atom_membership)
-000229c0: 0a0a 0a63 6c61 7373 2045 6467 654e 6574  ...class EdgeNet
-000229d0: 776f 726b 286e 6e2e 4d6f 6475 6c65 293a  work(nn.Module):
-000229e0: 0a20 2020 2022 2222 5468 6520 4564 6765  .    """The Edge
-000229f0: 4e65 7477 6f72 6b20 6d6f 6475 6c65 2069  Network module i
-00022a00: 7320 6120 5079 546f 7263 6820 7375 626d  s a PyTorch subm
-00022a10: 6f64 756c 6520 6465 7369 676e 6564 2066  odule designed f
-00022a20: 6f72 206d 6573 7361 6765 2070 6173 7369  or message passi
-00022a30: 6e67 2069 6e20 6772 6170 6820 6e65 7572  ng in graph neur
-00022a40: 616c 206e 6574 776f 726b 732e 0a0a 2020  al networks...  
-00022a50: 2020 4578 616d 706c 6573 0a20 2020 202d    Examples.    -
-00022a60: 2d2d 2d2d 2d2d 2d0a 2020 2020 3e3e 3e20  -------.    >>> 
-00022a70: 7061 6972 5f66 6561 7475 7265 7320 3d20  pair_features = 
-00022a80: 746f 7263 682e 7261 6e64 2828 342c 2032  torch.rand((4, 2
-00022a90: 292c 2064 7479 7065 3d74 6f72 6368 2e66  ), dtype=torch.f
-00022aa0: 6c6f 6174 3332 290a 2020 2020 3e3e 3e20  loat32).    >>> 
-00022ab0: 6174 6f6d 5f66 6561 7475 7265 7320 3d20  atom_features = 
-00022ac0: 746f 7263 682e 7261 6e64 2828 352c 2032  torch.rand((5, 2
-00022ad0: 292c 2064 7479 7065 3d74 6f72 6368 2e66  ), dtype=torch.f
-00022ae0: 6c6f 6174 3332 290a 2020 2020 3e3e 3e20  loat32).    >>> 
-00022af0: 6174 6f6d 5f74 6f5f 7061 6972 203d 205b  atom_to_pair = [
-00022b00: 5d0a 2020 2020 3e3e 3e20 6e5f 6174 6f6d  ].    >>> n_atom
-00022b10: 7320 3d20 320a 2020 2020 3e3e 3e20 7374  s = 2.    >>> st
-00022b20: 6172 7420 3d20 300a 2020 2020 3e3e 3e20  art = 0.    >>> 
-00022b30: 4330 2c20 4331 203d 206e 702e 6d65 7368  C0, C1 = np.mesh
-00022b40: 6772 6964 286e 702e 6172 616e 6765 286e  grid(np.arange(n
-00022b50: 5f61 746f 6d73 292c 206e 702e 6172 616e  _atoms), np.aran
-00022b60: 6765 286e 5f61 746f 6d73 2929 0a20 2020  ge(n_atoms)).   
-00022b70: 203e 3e3e 2061 746f 6d5f 746f 5f70 6169   >>> atom_to_pai
-00022b80: 722e 6170 7065 6e64 286e 702e 7472 616e  r.append(np.tran
-00022b90: 7370 6f73 6528 6e70 2e61 7272 6179 285b  spose(np.array([
-00022ba0: 4331 2e66 6c61 7474 656e 2829 202b 2073  C1.flatten() + s
-00022bb0: 7461 7274 2c20 4330 2e66 6c61 7474 656e  tart, C0.flatten
-00022bc0: 2829 202b 2073 7461 7274 5d29 2929 0a20  () + start]))). 
-00022bd0: 2020 203e 3e3e 2061 746f 6d5f 746f 5f70     >>> atom_to_p
-00022be0: 6169 7220 3d20 746f 7263 682e 5465 6e73  air = torch.Tens
-00022bf0: 6f72 2861 746f 6d5f 746f 5f70 6169 7229  or(atom_to_pair)
-00022c00: 0a20 2020 203e 3e3e 2061 746f 6d5f 746f  .    >>> atom_to
-00022c10: 5f70 6169 7220 3d20 746f 7263 682e 7371  _pair = torch.sq
-00022c20: 7565 657a 6528 6174 6f6d 5f74 6f5f 7061  ueeze(atom_to_pa
-00022c30: 6972 2e74 6f28 746f 7263 682e 696e 7436  ir.to(torch.int6
-00022c40: 3429 2c20 6469 6d3d 3029 0a20 2020 203e  4), dim=0).    >
-00022c50: 3e3e 2069 6e70 7574 7320 3d20 5b70 6169  >> inputs = [pai
-00022c60: 725f 6665 6174 7572 6573 2c20 6174 6f6d  r_features, atom
-00022c70: 5f66 6561 7475 7265 732c 2061 746f 6d5f  _features, atom_
-00022c80: 746f 5f70 6169 725d 0a20 2020 203e 3e3e  to_pair].    >>>
-00022c90: 206e 5f70 6169 725f 6665 6174 7572 6573   n_pair_features
-00022ca0: 203d 2032 0a20 2020 203e 3e3e 206e 5f68   = 2.    >>> n_h
-00022cb0: 6964 6465 6e20 3d20 320a 2020 2020 3e3e  idden = 2.    >>
-00022cc0: 3e20 696e 6974 203d 2027 7861 7669 6572  > init = 'xavier
-00022cd0: 5f75 6e69 666f 726d 5f27 0a20 2020 203e  _uniform_'.    >
-00022ce0: 3e3e 206c 6179 6572 203d 2045 6467 654e  >> layer = EdgeN
-00022cf0: 6574 776f 726b 286e 5f70 6169 725f 6665  etwork(n_pair_fe
-00022d00: 6174 7572 6573 2c20 6e5f 6869 6464 656e  atures, n_hidden
-00022d10: 2c20 696e 6974 290a 2020 2020 3e3e 3e20  , init).    >>> 
-00022d20: 7265 7375 6c74 203d 206c 6179 6572 2869  result = layer(i
-00022d30: 6e70 7574 7329 0a20 2020 203e 3e3e 2072  nputs).    >>> r
-00022d40: 6573 756c 742e 7368 6170 655b 315d 0a20  esult.shape[1]. 
-00022d50: 2020 2032 0a20 2020 2022 2222 0a0a 2020     2.    """..  
-00022d60: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00022d70: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
-00022d80: 2020 2020 2020 6e5f 7061 6972 5f66 6561        n_pair_fea
-00022d90: 7475 7265 733a 2069 6e74 203d 2038 2c0a  tures: int = 8,.
-00022da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022db0: 206e 5f68 6964 6465 6e3a 2069 6e74 203d   n_hidden: int =
-00022dc0: 2031 3030 2c0a 2020 2020 2020 2020 2020   100,.          
-00022dd0: 2020 2020 2020 2069 6e69 743a 2073 7472         init: str
-00022de0: 203d 2027 7861 7669 6572 5f75 6e69 666f   = 'xavier_unifo
-00022df0: 726d 5f27 2c0a 2020 2020 2020 2020 2020  rm_',.          
-00022e00: 2020 2020 2020 202a 2a6b 7761 7267 7329         **kwargs)
-00022e10: 3a0a 2020 2020 2020 2020 2222 2249 6e69  :.        """Ini
-00022e20: 7461 6c69 7365 7320 6120 4564 6765 4e65  talises a EdgeNe
-00022e30: 7477 6f72 6b20 4c61 7965 720a 0a20 2020  twork Layer..   
-00022e40: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00022e50: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00022e60: 2d2d 0a20 2020 2020 2020 206e 5f70 6169  --.        n_pai
-00022e70: 725f 6665 6174 7572 6573 3a20 696e 742c  r_features: int,
-00022e80: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-00022e90: 2020 2020 2020 5468 6520 6c65 6e67 7468        The length
-00022ea0: 206f 6620 7468 6520 7061 6972 2066 6561   of the pair fea
-00022eb0: 7475 7265 7320 7665 6374 6f72 2e0a 2020  tures vector..  
-00022ec0: 2020 2020 2020 6e5f 6869 6464 656e 3a20        n_hidden: 
-00022ed0: 696e 742c 206f 7074 696f 6e61 6c0a 2020  int, optional.  
-00022ee0: 2020 2020 2020 2020 2020 6e75 6d62 6572            number
-00022ef0: 206f 6620 6869 6464 656e 2075 6e69 7473   of hidden units
-00022f00: 2069 6e20 7468 6520 7061 7373 696e 6720   in the passing 
-00022f10: 7068 6173 650a 2020 2020 2020 2020 696e  phase.        in
-00022f20: 6974 3a20 7374 722c 206f 7074 696f 6e61  it: str, optiona
-00022f30: 6c0a 2020 2020 2020 2020 2020 2020 496e  l.            In
-00022f40: 6974 6961 6c69 7a61 7469 6f6e 2066 756e  itialization fun
-00022f50: 6374 696f 6e20 746f 2062 6520 7573 6564  ction to be used
-00022f60: 2069 6e20 7468 6520 6d65 7373 6167 6520   in the message 
-00022f70: 7061 7373 696e 6720 6c61 7965 722e 0a20  passing layer.. 
-00022f80: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-00022f90: 2020 2020 7375 7065 7228 4564 6765 4e65      super(EdgeNe
-00022fa0: 7477 6f72 6b2c 2073 656c 6629 2e5f 5f69  twork, self).__i
-00022fb0: 6e69 745f 5f28 2a2a 6b77 6172 6773 290a  nit__(**kwargs).
-00022fc0: 2020 2020 2020 2020 7365 6c66 2e6e 5f70          self.n_p
-00022fd0: 6169 725f 6665 6174 7572 6573 3a20 696e  air_features: in
-00022fe0: 7420 3d20 6e5f 7061 6972 5f66 6561 7475  t = n_pair_featu
-00022ff0: 7265 730a 2020 2020 2020 2020 7365 6c66  res.        self
-00023000: 2e6e 5f68 6964 6465 6e3a 2069 6e74 203d  .n_hidden: int =
-00023010: 206e 5f68 6964 6465 6e0a 2020 2020 2020   n_hidden.      
-00023020: 2020 7365 6c66 2e69 6e69 743a 2073 7472    self.init: str
-00023030: 203d 2069 6e69 740a 0a20 2020 2020 2020   = init..       
-00023040: 2069 6e69 745f 6675 6e63 3a20 4361 6c6c   init_func: Call
-00023050: 6162 6c65 203d 2067 6574 6174 7472 2869  able = getattr(i
-00023060: 6e69 7469 616c 697a 6572 732c 2073 656c  nitializers, sel
-00023070: 662e 696e 6974 290a 2020 2020 2020 2020  f.init).        
-00023080: 7365 6c66 2e57 3a20 746f 7263 682e 5465  self.W: torch.Te
-00023090: 6e73 6f72 203d 2069 6e69 745f 6675 6e63  nsor = init_func
-000230a0: 280a 2020 2020 2020 2020 2020 2020 746f  (.            to
-000230b0: 7263 682e 656d 7074 7928 5b73 656c 662e  rch.empty([self.
-000230c0: 6e5f 7061 6972 5f66 6561 7475 7265 732c  n_pair_features,
-000230d0: 2073 656c 662e 6e5f 6869 6464 656e 202a   self.n_hidden *
-000230e0: 2073 656c 662e 6e5f 6869 6464 656e 5d29   self.n_hidden])
-000230f0: 290a 2020 2020 2020 2020 7365 6c66 2e62  ).        self.b
-00023100: 3a20 746f 7263 682e 5465 6e73 6f72 203d  : torch.Tensor =
-00023110: 2074 6f72 6368 2e7a 6572 6f73 2828 7365   torch.zeros((se
-00023120: 6c66 2e6e 5f68 6964 6465 6e20 2a20 7365  lf.n_hidden * se
-00023130: 6c66 2e6e 5f68 6964 6465 6e2c 2929 0a20  lf.n_hidden,)). 
-00023140: 2020 2020 2020 2073 656c 662e 6275 696c         self.buil
-00023150: 743a 2062 6f6f 6c20 3d20 5472 7565 0a0a  t: bool = True..
-00023160: 2020 2020 6465 6620 5f5f 7265 7072 5f5f      def __repr__
-00023170: 2873 656c 6629 202d 3e20 7374 723a 0a20  (self) -> str:. 
-00023180: 2020 2020 2020 2072 6574 7572 6e20 280a         return (.
-00023190: 2020 2020 2020 2020 2020 2020 6627 7b73              f'{s
-000231a0: 656c 662e 5f5f 636c 6173 735f 5f2e 5f5f  elf.__class__.__
-000231b0: 6e61 6d65 5f5f 7d28 6e5f 7061 6972 5f66  name__}(n_pair_f
-000231c0: 6561 7475 7265 733a 7b73 656c 662e 6e5f  eatures:{self.n_
-000231d0: 7061 6972 5f66 6561 7475 7265 737d 2c6e  pair_features},n
-000231e0: 5f68 6964 6465 6e3a 7b73 656c 662e 6e5f  _hidden:{self.n_
-000231f0: 6869 6464 656e 7d2c 696e 6974 3a7b 7365  hidden},init:{se
-00023200: 6c66 2e69 6e69 747d 2927 0a20 2020 2020  lf.init})'.     
-00023210: 2020 2029 0a0a 2020 2020 6465 6620 666f     )..    def fo
-00023220: 7277 6172 6428 7365 6c66 2c20 696e 7075  rward(self, inpu
-00023230: 7473 3a20 4c69 7374 5b74 6f72 6368 2e54  ts: List[torch.T
-00023240: 656e 736f 725d 2920 2d3e 2074 6f72 6368  ensor]) -> torch
-00023250: 2e54 656e 736f 723a 0a20 2020 2020 2020  .Tensor:.       
-00023260: 2022 2222 0a20 2020 2020 2020 2050 6172   """.        Par
-00023270: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-00023280: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-00023290: 2020 2069 6e70 7574 733a 204c 6973 745b     inputs: List[
-000232a0: 746f 7263 682e 5465 6e73 6f72 5d0a 2020  torch.Tensor].  
-000232b0: 2020 2020 2020 2020 2020 5468 6520 6c65            The le
-000232c0: 6e67 7468 206f 6620 6174 6f6d 5f74 6f5f  ngth of atom_to_
-000232d0: 7061 6972 2073 686f 756c 6420 6265 2073  pair should be s
-000232e0: 616d 6520 6173 206e 5f70 6169 725f 6665  ame as n_pair_fe
-000232f0: 6174 7572 6573 2e0a 2020 2020 2020 2020  atures..        
-00023300: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
-00023310: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00023320: 7265 7375 6c74 3a20 746f 7263 682e 5465  result: torch.Te
-00023330: 6e73 6f72 0a20 2020 2020 2020 2020 2020  nsor.           
-00023340: 2054 656e 736f 7220 636f 6e74 6169 6e69   Tensor containi
-00023350: 6e67 2074 6865 206d 6170 7069 6e67 206f  ng the mapping o
-00023360: 6620 7468 6520 6564 6765 2076 6563 746f  f the edge vecto
-00023370: 7220 746f 2061 2064 20c3 9720 6420 6d61  r to a d .. d ma
-00023380: 7472 6978 2c20 7768 6572 6520 6420 6465  trix, where d de
-00023390: 6e6f 7465 7320 7468 6520 6469 6d65 6e73  notes the dimens
-000233a0: 696f 6e20 6f66 2074 6865 2069 6e74 6572  ion of the inter
-000233b0: 6e61 6c20 6869 6464 656e 2072 6570 7265  nal hidden repre
-000233c0: 7365 6e74 6174 696f 6e20 6f66 2065 6163  sentation of eac
-000233d0: 6820 6e6f 6465 2069 6e20 7468 6520 6772  h node in the gr
-000233e0: 6170 682e 0a20 2020 2020 2020 2022 2222  aph..        """
-000233f0: 0a20 2020 2020 2020 2070 6169 725f 6665  .        pair_fe
-00023400: 6174 7572 6573 3a20 746f 7263 682e 5465  atures: torch.Te
-00023410: 6e73 6f72 0a20 2020 2020 2020 2061 746f  nsor.        ato
-00023420: 6d5f 6665 6174 7572 6573 3a20 746f 7263  m_features: torc
-00023430: 682e 5465 6e73 6f72 0a20 2020 2020 2020  h.Tensor.       
-00023440: 2061 746f 6d5f 746f 5f70 6169 723a 2074   atom_to_pair: t
-00023450: 6f72 6368 2e54 656e 736f 720a 2020 2020  orch.Tensor.    
-00023460: 2020 2020 7061 6972 5f66 6561 7475 7265      pair_feature
-00023470: 732c 2061 746f 6d5f 6665 6174 7572 6573  s, atom_features
-00023480: 2c20 6174 6f6d 5f74 6f5f 7061 6972 203d  , atom_to_pair =
-00023490: 2069 6e70 7574 730a 0a20 2020 2020 2020   inputs..       
-000234a0: 2041 3a20 746f 7263 682e 5465 6e73 6f72   A: torch.Tensor
-000234b0: 203d 2074 6f72 6368 2e61 6464 2874 6f72   = torch.add(tor
-000234c0: 6368 2e6d 6174 6d75 6c28 7061 6972 5f66  ch.matmul(pair_f
-000234d0: 6561 7475 7265 732c 2073 656c 662e 5729  eatures, self.W)
-000234e0: 2c20 7365 6c66 2e62 290a 2020 2020 2020  , self.b).      
-000234f0: 2020 4120 3d20 746f 7263 682e 7265 7368    A = torch.resh
-00023500: 6170 6528 412c 2028 2d31 2c20 7365 6c66  ape(A, (-1, self
-00023510: 2e6e 5f68 6964 6465 6e2c 2073 656c 662e  .n_hidden, self.
-00023520: 6e5f 6869 6464 656e 2929 0a20 2020 2020  n_hidden)).     
-00023530: 2020 206f 7574 3a20 746f 7263 682e 5465     out: torch.Te
-00023540: 6e73 6f72 203d 2074 6f72 6368 2e75 6e73  nsor = torch.uns
-00023550: 7175 6565 7a65 2861 746f 6d5f 6665 6174  queeze(atom_feat
-00023560: 7572 6573 5b61 746f 6d5f 746f 5f70 6169  ures[atom_to_pai
-00023570: 725b 3a2c 2031 5d5d 2c0a 2020 2020 2020  r[:, 1]],.      
-00023580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000235a0: 2020 2020 2020 6469 6d3d 3229 0a20 2020        dim=2).   
-000235b0: 2020 2020 206f 7574 5f73 7175 6565 7a65       out_squeeze
-000235c0: 3a20 746f 7263 682e 5465 6e73 6f72 203d  : torch.Tensor =
-000235d0: 2074 6f72 6368 2e73 7175 6565 7a65 2874   torch.squeeze(t
-000235e0: 6f72 6368 2e6d 6174 6d75 6c28 412c 206f  orch.matmul(A, o
-000235f0: 7574 292c 2064 696d 3d32 290a 2020 2020  ut), dim=2).    
-00023600: 2020 2020 696e 643a 2074 6f72 6368 2e54      ind: torch.T
-00023610: 656e 736f 7220 3d20 6174 6f6d 5f74 6f5f  ensor = atom_to_
-00023620: 7061 6972 5b3a 2c20 305d 0a0a 2020 2020  pair[:, 0]..    
-00023630: 2020 2020 7265 7375 6c74 3a20 746f 7263      result: torc
-00023640: 682e 5465 6e73 6f72 203d 2073 6567 6d65  h.Tensor = segme
-00023650: 6e74 5f73 756d 286f 7574 5f73 7175 6565  nt_sum(out_squee
-00023660: 7a65 2c20 696e 6429 0a0a 2020 2020 2020  ze, ind)..      
-00023670: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-00023680: 0a0a 636c 6173 7320 5765 6176 654c 6179  ..class WeaveLay
-00023690: 6572 286e 6e2e 4d6f 6475 6c65 293a 0a20  er(nn.Module):. 
-000236a0: 2020 2022 2222 5468 6973 2063 6c61 7373     """This class
-000236b0: 2069 6d70 6c65 6d65 6e74 7320 7468 6520   implements the 
-000236c0: 636f 7265 2057 6561 7665 2063 6f6e 766f  core Weave convo
-000236d0: 6c75 7469 6f6e 2066 726f 6d20 7468 6520  lution from the 
-000236e0: 476f 6f67 6c65 2067 7261 7068 2063 6f6e  Google graph con
-000236f0: 766f 6c75 7469 6f6e 2070 6170 6572 205b  volution paper [
-00023700: 315d 5f0a 2020 5468 6973 2069 7320 7468  1]_.  This is th
-00023710: 6520 546f 7263 6820 6571 7569 7661 6c65  e Torch equivale
-00023720: 6e74 206f 6620 7468 6520 6f72 6967 696e  nt of the origin
-00023730: 616c 2069 6d70 6c65 6d65 6e74 6174 696f  al implementatio
-00023740: 6e20 7573 696e 6720 4b65 7261 732e 0a0a  n using Keras...
-00023750: 2020 5468 6973 206d 6f64 656c 2063 6f6e    This model con
-00023760: 7461 696e 7320 6174 6f6d 2066 6561 7475  tains atom featu
-00023770: 7265 7320 616e 6420 626f 6e64 2066 6561  res and bond fea
-00023780: 7475 7265 730a 2020 7365 7061 7261 7465  tures.  separate
-00023790: 6c79 2e48 6572 652c 2062 6f6e 6420 6665  ly.Here, bond fe
-000237a0: 6174 7572 6573 2061 7265 2061 6c73 6f20  atures are also 
-000237b0: 6361 6c6c 6564 2070 6169 7220 6665 6174  called pair feat
-000237c0: 7572 6573 2e0a 2020 5468 6572 6520 6172  ures..  There ar
-000237d0: 6520 3220 7479 7065 7320 6f66 2074 7261  e 2 types of tra
-000237e0: 6e73 666f 726d 6174 696f 6e2c 2061 746f  nsformation, ato
-000237f0: 6d2d 3e61 746f 6d2c 2061 746f 6d2d 3e70  m->atom, atom->p
-00023800: 6169 722c 2070 6169 722d 3e61 746f 6d2c  air, pair->atom,
-00023810: 2070 6169 722d 3e70 6169 7220 7468 6174   pair->pair that
-00023820: 2074 6869 7320 6d6f 6465 6c20 696d 706c   this model impl
-00023830: 656d 656e 7473 2e0a 0a20 2045 7861 6d70  ements...  Examp
-00023840: 6c65 730a 2020 2d2d 2d2d 2d2d 2d2d 0a20  les.  --------. 
-00023850: 2054 6869 7320 6c61 7965 7220 6578 7065   This layer expe
-00023860: 6374 7320 3420 696e 7075 7473 2069 6e20  cts 4 inputs in 
-00023870: 6120 6c69 7374 206f 6620 7468 6520 666f  a list of the fo
-00023880: 726d 2060 5b61 746f 6d5f 6665 6174 7572  rm `[atom_featur
-00023890: 6573 2c0a 2020 7061 6972 5f66 6561 7475  es,.  pair_featu
-000238a0: 7265 732c 2070 6169 725f 7370 6c69 742c  res, pair_split,
-000238b0: 2061 746f 6d5f 746f 5f70 6169 725d 602e   atom_to_pair]`.
-000238c0: 2057 6527 6c6c 2077 616c 6b20 7468 726f   We'll walk thro
-000238d0: 7567 6820 7468 6520 7374 7275 6374 7572  ugh the structur
-000238e0: 6520 6f66 2074 6865 7365 2069 6e70 7574  e of these input
-000238f0: 732e 204c 6574 2773 2073 7461 7274 2077  s. Let's start w
-00023900: 6974 6820 736f 6d65 2062 6173 6963 2064  ith some basic d
-00023910: 6566 696e 6974 696f 6e73 2e0a 2020 3e3e  efinitions..  >>
-00023920: 3e20 696d 706f 7274 2064 6565 7063 6865  > import deepche
-00023930: 6d20 6173 2064 630a 2020 3e3e 3e20 696d  m as dc.  >>> im
-00023940: 706f 7274 206e 756d 7079 2061 7320 6e70  port numpy as np
-00023950: 0a20 203e 3e3e 2073 6d69 6c65 7320 3d20  .  >>> smiles = 
-00023960: 5b22 4343 4322 2c20 2243 225d 0a0a 2020  ["CCC", "C"]..  
-00023970: 4e6f 7465 2074 6861 7420 7468 6572 6520  Note that there 
-00023980: 6172 6520 3420 6174 6f6d 7320 696e 2074  are 4 atoms in t
-00023990: 6f74 616c 2069 6e20 7468 6973 2073 7973  otal in this sys
-000239a0: 7465 6d2e 2054 6869 7320 6c61 7965 7220  tem. This layer 
-000239b0: 6578 7065 6374 7320 6974 7320 696e 7075  expects its inpu
-000239c0: 7420 6d6f 6c65 6375 6c65 7320 746f 2062  t molecules to b
-000239d0: 6520 6261 7463 6865 6420 746f 6765 7468  e batched togeth
-000239e0: 6572 2e0a 0a20 203e 3e3e 2074 6f74 616c  er...  >>> total
-000239f0: 5f6e 5f61 746f 6d73 203d 2034 0a0a 2020  _n_atoms = 4..  
-00023a00: 4c65 7427 7320 7375 7070 6f73 6520 7468  Let's suppose th
-00023a10: 6174 2077 6520 6861 7665 2061 2066 6561  at we have a fea
-00023a20: 7475 7269 7a65 7220 7468 6174 2063 6f6d  turizer that com
-00023a30: 7075 7465 7320 606e 5f61 746f 6d5f 6665  putes `n_atom_fe
-00023a40: 6174 6020 6665 6174 7572 6573 2070 6572  at` features per
-00023a50: 2061 746f 6d2e 0a0a 2020 3e3e 3e20 6e5f   atom...  >>> n_
-00023a60: 6174 6f6d 5f66 6561 7420 3d20 3735 0a0a  atom_feat = 75..
-00023a70: 2020 5468 656e 2063 6f6e 6365 7074 7561    Then conceptua
-00023a80: 6c6c 792c 2060 6174 6f6d 5f66 6561 7460  lly, `atom_feat`
-00023a90: 2069 7320 7468 6520 6172 7261 7920 6f66   is the array of
-00023aa0: 2073 6861 7065 2060 2874 6f74 616c 5f6e   shape `(total_n
-00023ab0: 5f61 746f 6d73 2c0a 2020 6e5f 6174 6f6d  _atoms,.  n_atom
-00023ac0: 5f66 6561 7429 6020 6f66 2061 746f 6d69  _feat)` of atomi
-00023ad0: 6320 6665 6174 7572 6573 2e20 466f 7220  c features. For 
-00023ae0: 7369 6d70 6c69 6369 7479 2c20 6c65 7427  simplicity, let'
-00023af0: 7320 6a75 7374 2067 6f20 7769 7468 2061  s just go with a
-00023b00: 0a20 2072 616e 646f 6d20 7375 6368 206d  .  random such m
-00023b10: 6174 7269 782e 0a0a 2020 3e3e 3e20 6174  atrix...  >>> at
-00023b20: 6f6d 5f66 6561 7420 3d20 6e70 2e72 616e  om_feat = np.ran
-00023b30: 646f 6d2e 7261 6e64 2874 6f74 616c 5f6e  dom.rand(total_n
-00023b40: 5f61 746f 6d73 2c20 6e5f 6174 6f6d 5f66  _atoms, n_atom_f
-00023b50: 6561 7429 0a0a 2020 4c65 7427 7320 7375  eat)..  Let's su
-00023b60: 7070 6f73 6520 7765 2068 6176 6520 606e  ppose we have `n
-00023b70: 5f70 6169 725f 6665 6174 6020 7061 6972  _pair_feat` pair
-00023b80: 7769 7365 2066 6561 7475 7265 730a 0a20  wise features.. 
-00023b90: 203e 3e3e 206e 5f70 6169 725f 6665 6174   >>> n_pair_feat
-00023ba0: 203d 2031 340a 0a20 2046 6f72 2065 6163   = 14..  For eac
-00023bb0: 6820 6d6f 6c65 6375 6c65 2c20 7765 2063  h molecule, we c
-00023bc0: 6f6d 7075 7465 2061 206d 6174 7269 7820  ompute a matrix 
-00023bd0: 6f66 2073 6861 7065 2060 286e 5f61 746f  of shape `(n_ato
-00023be0: 6d73 2a6e 5f61 746f 6d73 2c0a 2020 6e5f  ms*n_atoms,.  n_
-00023bf0: 7061 6972 5f66 6561 7429 6020 6f66 2070  pair_feat)` of p
-00023c00: 6169 7277 6973 6520 6665 6174 7572 6573  airwise features
-00023c10: 2066 6f72 2065 6163 6820 7061 6972 206f   for each pair o
-00023c20: 6620 6174 6f6d 7320 696e 2074 6865 206d  f atoms in the m
-00023c30: 6f6c 6563 756c 652e 0a20 204c 6574 2773  olecule..  Let's
-00023c40: 2063 6f6e 7374 7275 6374 2074 6869 7320   construct this 
-00023c50: 636f 6e63 6570 7475 616c 6c79 2066 6f72  conceptually for
-00023c60: 206f 7572 2065 7861 6d70 6c65 2e0a 0a20   our example... 
-00023c70: 203e 3e3e 2070 6169 725f 6665 6174 203d   >>> pair_feat =
-00023c80: 205b 6e70 2e72 616e 646f 6d2e 7261 6e64   [np.random.rand
-00023c90: 2833 2a33 2c20 6e5f 7061 6972 5f66 6561  (3*3, n_pair_fea
-00023ca0: 7429 2c20 6e70 2e72 616e 646f 6d2e 7261  t), np.random.ra
-00023cb0: 6e64 2831 2a31 2c6e 5f70 6169 725f 6665  nd(1*1,n_pair_fe
-00023cc0: 6174 295d 0a20 203e 3e3e 2070 6169 725f  at)].  >>> pair_
-00023cd0: 6665 6174 203d 206e 702e 636f 6e63 6174  feat = np.concat
-00023ce0: 656e 6174 6528 7061 6972 5f66 6561 742c  enate(pair_feat,
-00023cf0: 2061 7869 733d 3029 0a20 203e 3e3e 2070   axis=0).  >>> p
-00023d00: 6169 725f 6665 6174 2e73 6861 7065 0a20  air_feat.shape. 
-00023d10: 2028 3130 2c20 3134 290a 0a20 2060 7061   (10, 14)..  `pa
-00023d20: 6972 5f73 706c 6974 6020 6973 2061 6e20  ir_split` is an 
-00023d30: 696e 6465 7820 696e 746f 2060 7061 6972  index into `pair
-00023d40: 5f66 6561 7460 2077 6869 6368 2074 656c  _feat` which tel
-00023d50: 6c73 2075 7320 7768 6963 6820 6174 6f6d  ls us which atom
-00023d60: 2065 6163 6820 726f 7720 6265 6c6f 6e67   each row belong
-00023d70: 7320 746f 2e20 496e 206f 7572 2063 6173  s to. In our cas
-00023d80: 652c 2077 6520 6876 650a 0a20 203e 3e3e  e, we hve..  >>>
-00023d90: 2070 6169 725f 7370 6c69 7420 3d20 6e70   pair_split = np
-00023da0: 2e61 7272 6179 285b 302c 2030 2c20 302c  .array([0, 0, 0,
-00023db0: 2031 2c20 312c 2031 2c20 322c 2032 2c20   1, 1, 1, 2, 2, 
-00023dc0: 322c 2033 5d29 0a0a 2020 5468 6174 2069  2, 3])..  That i
-00023dd0: 732c 2074 6865 2066 6972 7374 2039 2065  s, the first 9 e
-00023de0: 6e74 7269 6573 2062 656c 6f6e 6720 746f  ntries belong to
-00023df0: 2022 4343 4322 2061 6e64 2074 6865 206c   "CCC" and the l
-00023e00: 6173 7420 656e 7472 7920 746f 2022 4322  ast entry to "C"
-00023e10: 2e20 5468 650a 2020 6669 6e61 6c20 656e  . The.  final en
-00023e20: 7472 7920 6061 746f 6d5f 746f 5f70 6169  try `atom_to_pai
-00023e30: 7260 2067 6f65 7320 696e 2061 206c 6974  r` goes in a lit
-00023e40: 746c 6520 6d6f 7265 2069 6e2d 6465 7074  tle more in-dept
-00023e50: 6820 7468 616e 2060 7061 6972 5f73 706c  h than `pair_spl
-00023e60: 6974 600a 2020 616e 6420 7465 6c6c 7320  it`.  and tells 
-00023e70: 7573 2074 6865 2070 7265 6369 7365 2070  us the precise p
-00023e80: 6169 7220 6561 6368 2070 6169 7220 6665  air each pair fe
-00023e90: 6174 7572 6520 6265 6c6f 6e67 7320 746f  ature belongs to
-00023ea0: 2e20 496e 206f 7572 2063 6173 650a 0a20  . In our case.. 
-00023eb0: 203e 3e3e 2061 746f 6d5f 746f 5f70 6169   >>> atom_to_pai
-00023ec0: 7220 3d20 6e70 2e61 7272 6179 285b 5b30  r = np.array([[0
-00023ed0: 2c20 305d 2c0a 2020 2e2e 2e20 2020 2020  , 0],.  ...     
-00023ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023ef0: 2020 2020 205b 302c 2031 5d2c 0a20 202e       [0, 1],.  .
-00023f00: 2e2e 2020 2020 2020 2020 2020 2020 2020  ..              
-00023f10: 2020 2020 2020 2020 2020 2020 5b30 2c20              [0, 
-00023f20: 325d 2c0a 2020 2e2e 2e20 2020 2020 2020  2],.  ...       
-00023f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023f40: 2020 205b 312c 2030 5d2c 0a20 202e 2e2e     [1, 0],.  ...
-00023f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023f60: 2020 2020 2020 2020 2020 5b31 2c20 315d            [1, 1]
-00023f70: 2c0a 2020 2e2e 2e20 2020 2020 2020 2020  ,.  ...         
-00023f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023f90: 205b 312c 2032 5d2c 0a20 202e 2e2e 2020   [1, 2],.  ...  
-00023fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023fb0: 2020 2020 2020 2020 5b32 2c20 305d 2c0a          [2, 0],.
-00023fc0: 2020 2e2e 2e20 2020 2020 2020 2020 2020    ...           
-00023fd0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-00023fe0: 322c 2031 5d2c 0a20 202e 2e2e 2020 2020  2, 1],.  ...    
-00023ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024000: 2020 2020 2020 5b32 2c20 325d 2c0a 2020        [2, 2],.  
-00024010: 2e2e 2e20 2020 2020 2020 2020 2020 2020  ...             
-00024020: 2020 2020 2020 2020 2020 2020 205b 332c               [3,
-00024030: 2033 5d5d 290a 0a20 204c 6574 2773 206e   3]])..  Let's n
-00024040: 6f77 2064 6566 696e 6520 7468 6520 6163  ow define the ac
-00024050: 7475 616c 206c 6179 6572 0a0a 2020 3e3e  tual layer..  >>
-00024060: 3e20 6c61 7965 7220 3d20 5765 6176 654c  > layer = WeaveL
-00024070: 6179 6572 2829 0a0a 2020 416e 6420 696e  ayer()..  And in
-00024080: 766f 6b65 2069 740a 0a20 203e 3e3e 205b  voke it..  >>> [
-00024090: 412c 2050 5d20 3d20 6c61 7965 7228 5b61  A, P] = layer([a
-000240a0: 746f 6d5f 6665 6174 2c20 7061 6972 5f66  tom_feat, pair_f
-000240b0: 6561 742c 2070 6169 725f 7370 6c69 742c  eat, pair_split,
-000240c0: 2061 746f 6d5f 746f 5f70 6169 725d 290a   atom_to_pair]).
-000240d0: 0a20 2054 6865 2077 6561 7665 206c 6179  .  The weave lay
-000240e0: 6572 2070 726f 6475 6365 7320 6e65 7720  er produces new 
-000240f0: 6174 6f6d 2f70 6169 7220 6665 6174 7572  atom/pair featur
-00024100: 6573 2e20 4c65 7427 7320 6368 6563 6b20  es. Let's check 
-00024110: 7468 6569 7220 7368 6170 6573 0a0a 2020  their shapes..  
-00024120: 3e3e 3e20 4120 3d20 412e 6465 7461 6368  >>> A = A.detach
-00024130: 2829 2e6e 756d 7079 2829 0a20 203e 3e3e  ().numpy().  >>>
-00024140: 2041 2e73 6861 7065 0a20 2028 342c 2035   A.shape.  (4, 5
-00024150: 3029 0a20 203e 3e3e 2050 203d 2050 2e64  0).  >>> P = P.d
-00024160: 6574 6163 6828 292e 6e75 6d70 7928 290a  etach().numpy().
-00024170: 2020 3e3e 3e20 502e 7368 6170 650a 2020    >>> P.shape.  
-00024180: 2831 302c 2035 3029 0a0a 2020 5468 6520  (10, 50)..  The 
-00024190: 3420 6973 2060 746f 7461 6c5f 6e75 6d5f  4 is `total_num_
-000241a0: 6174 6f6d 7360 2061 6e64 2074 6865 2031  atoms` and the 1
-000241b0: 3020 6973 2074 6865 2074 6f74 616c 206e  0 is the total n
-000241c0: 756d 6265 7220 6f66 2070 6169 7273 2e20  umber of pairs. 
-000241d0: 5768 6572 650a 2020 646f 6573 2060 3530  Where.  does `50
-000241e0: 6020 636f 6d65 2066 726f 6d3f 2049 7427  ` come from? It'
-000241f0: 7320 6672 6f6d 2074 6865 2064 6566 6175  s from the defau
-00024200: 6c74 2061 7267 756d 656e 7473 2060 6e5f  lt arguments `n_
-00024210: 6174 6f6d 5f69 6e70 7574 5f66 6561 7460  atom_input_feat`
-00024220: 2061 6e64 0a20 2060 6e5f 7061 6972 5f69   and.  `n_pair_i
-00024230: 6e70 7574 5f66 6561 7460 2e0a 0a20 2052  nput_feat`...  R
-00024240: 6566 6572 656e 6365 730a 2020 2d2d 2d2d  eferences.  ----
-00024250: 2d2d 2d2d 2d2d 0a20 202e 2e20 5b31 5d20  ------.  .. [1] 
-00024260: 4b65 6172 6e65 732c 2053 7465 7665 6e2c  Kearnes, Steven,
-00024270: 2065 7420 616c 2e20 224d 6f6c 6563 756c   et al. "Molecul
-00024280: 6172 2067 7261 7068 2063 6f6e 766f 6c75  ar graph convolu
-00024290: 7469 6f6e 733a 206d 6f76 696e 6720 6265  tions: moving be
-000242a0: 796f 6e64 0a20 2020 2020 2020 2066 696e  yond.        fin
-000242b0: 6765 7270 7269 6e74 732e 2220 4a6f 7572  gerprints." Jour
-000242c0: 6e61 6c20 6f66 2063 6f6d 7075 7465 722d  nal of computer-
-000242d0: 6169 6465 6420 6d6f 6c65 6375 6c61 7220  aided molecular 
-000242e0: 6465 7369 676e 2033 302e 3820 2832 3031  design 30.8 (201
-000242f0: 3629 3a0a 2020 2020 2020 2020 3539 352d  6):.        595-
-00024300: 3630 382e 0a20 2022 2222 0a0a 2020 2020  608..  """..    
-00024310: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00024320: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
-00024330: 2020 2020 6e5f 6174 6f6d 5f69 6e70 7574      n_atom_input
-00024340: 5f66 6561 743a 2069 6e74 203d 2037 352c  _feat: int = 75,
-00024350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024360: 2020 6e5f 7061 6972 5f69 6e70 7574 5f66    n_pair_input_f
-00024370: 6561 743a 2069 6e74 203d 2031 342c 0a20  eat: int = 14,. 
-00024380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024390: 6e5f 6174 6f6d 5f6f 7574 7075 745f 6665  n_atom_output_fe
-000243a0: 6174 3a20 696e 7420 3d20 3530 2c0a 2020  at: int = 50,.  
-000243b0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-000243c0: 5f70 6169 725f 6f75 7470 7574 5f66 6561  _pair_output_fea
-000243d0: 743a 2069 6e74 203d 2035 302c 0a20 2020  t: int = 50,.   
-000243e0: 2020 2020 2020 2020 2020 2020 2020 6e5f                n_
-000243f0: 6869 6464 656e 5f41 413a 2069 6e74 203d  hidden_AA: int =
-00024400: 2035 302c 0a20 2020 2020 2020 2020 2020   50,.           
-00024410: 2020 2020 2020 6e5f 6869 6464 656e 5f50        n_hidden_P
-00024420: 413a 2069 6e74 203d 2035 302c 0a20 2020  A: int = 50,.   
-00024430: 2020 2020 2020 2020 2020 2020 2020 6e5f                n_
-00024440: 6869 6464 656e 5f41 503a 2069 6e74 203d  hidden_AP: int =
-00024450: 2035 302c 0a20 2020 2020 2020 2020 2020   50,.           
-00024460: 2020 2020 2020 6e5f 6869 6464 656e 5f50        n_hidden_P
-00024470: 503a 2069 6e74 203d 2035 302c 0a20 2020  P: int = 50,.   
-00024480: 2020 2020 2020 2020 2020 2020 2020 7570                up
-00024490: 6461 7465 5f70 6169 723a 2062 6f6f 6c20  date_pair: bool 
-000244a0: 3d20 5472 7565 2c0a 2020 2020 2020 2020  = True,.        
-000244b0: 2020 2020 2020 2020 2069 6e69 745f 3a20           init_: 
-000244c0: 7374 7220 3d20 2778 6176 6965 725f 756e  str = 'xavier_un
-000244d0: 6966 6f72 6d5f 272c 0a20 2020 2020 2020  iform_',.       
-000244e0: 2020 2020 2020 2020 2020 6163 7469 7661            activa
-000244f0: 7469 6f6e 3a20 7374 7220 3d20 2772 656c  tion: str = 'rel
-00024500: 7527 2c0a 2020 2020 2020 2020 2020 2020  u',.            
-00024510: 2020 2020 2062 6174 6368 5f6e 6f72 6d61       batch_norma
-00024520: 6c69 7a65 3a20 626f 6f6c 203d 2054 7275  lize: bool = Tru
-00024530: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00024540: 2020 2020 2a2a 6b77 6172 6773 293a 0a20      **kwargs):. 
-00024550: 2020 2020 2020 2022 2222 0a20 2020 2050         """.    P
-00024560: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-00024570: 2d2d 2d2d 2d2d 2d2d 0a20 2020 206e 5f61  --------.    n_a
-00024580: 746f 6d5f 696e 7075 745f 6665 6174 3a20  tom_input_feat: 
-00024590: 696e 742c 206f 7074 696f 6e61 6c20 2864  int, optional (d
-000245a0: 6566 6175 6c74 2037 3529 0a20 2020 2020  efault 75).     
-000245b0: 204e 756d 6265 7220 6f66 2066 6561 7475   Number of featu
-000245c0: 7265 7320 666f 7220 6561 6368 2061 746f  res for each ato
-000245d0: 6d20 696e 2069 6e70 7574 2e0a 2020 2020  m in input..    
-000245e0: 6e5f 7061 6972 5f69 6e70 7574 5f66 6561  n_pair_input_fea
-000245f0: 743a 2069 6e74 2c20 6f70 7469 6f6e 616c  t: int, optional
-00024600: 2028 6465 6661 756c 7420 3134 290a 2020   (default 14).  
-00024610: 2020 2020 4e75 6d62 6572 206f 6620 6665      Number of fe
-00024620: 6174 7572 6573 2066 6f72 2065 6163 6820  atures for each 
-00024630: 7061 6972 206f 6620 6174 6f6d 7320 696e  pair of atoms in
-00024640: 2069 6e70 7574 2e0a 2020 2020 6e5f 6174   input..    n_at
-00024650: 6f6d 5f6f 7574 7075 745f 6665 6174 3a20  om_output_feat: 
-00024660: 696e 742c 206f 7074 696f 6e61 6c20 2864  int, optional (d
-00024670: 6566 6175 6c74 2035 3029 0a20 2020 2020  efault 50).     
-00024680: 204e 756d 6265 7220 6f66 2066 6561 7475   Number of featu
-00024690: 7265 7320 666f 7220 6561 6368 2061 746f  res for each ato
-000246a0: 6d20 696e 206f 7574 7075 742e 0a20 2020  m in output..   
-000246b0: 206e 5f70 6169 725f 6f75 7470 7574 5f66   n_pair_output_f
-000246c0: 6561 743a 2069 6e74 2c20 6f70 7469 6f6e  eat: int, option
-000246d0: 616c 2028 6465 6661 756c 7420 3530 290a  al (default 50).
-000246e0: 2020 2020 2020 4e75 6d62 6572 206f 6620        Number of 
-000246f0: 6665 6174 7572 6573 2066 6f72 2065 6163  features for eac
-00024700: 6820 7061 6972 206f 6620 6174 6f6d 7320  h pair of atoms 
-00024710: 696e 206f 7574 7075 742e 0a20 2020 206e  in output..    n
-00024720: 5f68 6964 6465 6e5f 4141 3a20 696e 742c  _hidden_AA: int,
-00024730: 206f 7074 696f 6e61 6c20 2864 6566 6175   optional (defau
-00024740: 6c74 2035 3029 0a20 2020 2020 204e 756d  lt 50).      Num
-00024750: 6265 7220 6f66 2075 6e69 7473 2863 6f6e  ber of units(con
-00024760: 766f 6c75 7469 6f6e 2064 6570 7468 7329  volution depths)
-00024770: 2069 6e20 636f 7272 6573 706f 6e64 696e   in correspondin
-00024780: 6720 6869 6464 656e 206c 6179 6572 0a20  g hidden layer. 
-00024790: 2020 206e 5f68 6964 6465 6e5f 5041 3a20     n_hidden_PA: 
-000247a0: 696e 742c 206f 7074 696f 6e61 6c20 2864  int, optional (d
-000247b0: 6566 6175 6c74 2035 3029 0a20 2020 2020  efault 50).     
-000247c0: 204e 756d 6265 7220 6f66 2075 6e69 7473   Number of units
-000247d0: 2863 6f6e 766f 6c75 7469 6f6e 2064 6570  (convolution dep
-000247e0: 7468 7329 2069 6e20 636f 7272 6573 706f  ths) in correspo
-000247f0: 6e64 696e 6720 6869 6464 656e 206c 6179  nding hidden lay
-00024800: 6572 0a20 2020 206e 5f68 6964 6465 6e5f  er.    n_hidden_
-00024810: 4150 3a20 696e 742c 206f 7074 696f 6e61  AP: int, optiona
-00024820: 6c20 2864 6566 6175 6c74 2035 3029 0a20  l (default 50). 
-00024830: 2020 2020 204e 756d 6265 7220 6f66 2075       Number of u
-00024840: 6e69 7473 2863 6f6e 766f 6c75 7469 6f6e  nits(convolution
-00024850: 2064 6570 7468 7329 2069 6e20 636f 7272   depths) in corr
-00024860: 6573 706f 6e64 696e 6720 6869 6464 656e  esponding hidden
-00024870: 206c 6179 6572 0a20 2020 206e 5f68 6964   layer.    n_hid
-00024880: 6465 6e5f 5050 3a20 696e 742c 206f 7074  den_PP: int, opt
-00024890: 696f 6e61 6c20 2864 6566 6175 6c74 2035  ional (default 5
-000248a0: 3029 0a20 2020 2020 204e 756d 6265 7220  0).      Number 
-000248b0: 6f66 2075 6e69 7473 2863 6f6e 766f 6c75  of units(convolu
-000248c0: 7469 6f6e 2064 6570 7468 7329 2069 6e20  tion depths) in 
-000248d0: 636f 7272 6573 706f 6e64 696e 6720 6869  corresponding hi
-000248e0: 6464 656e 206c 6179 6572 0a20 2020 2075  dden layer.    u
-000248f0: 7064 6174 655f 7061 6972 3a20 626f 6f6c  pdate_pair: bool
-00024900: 2c20 6f70 7469 6f6e 616c 2028 6465 6661  , optional (defa
-00024910: 756c 7420 5472 7565 290a 2020 2020 2020  ult True).      
-00024920: 5768 6574 6865 7220 746f 2063 616c 6375  Whether to calcu
-00024930: 6c61 7465 2066 6f72 2070 6169 7220 6665  late for pair fe
-00024940: 6174 7572 6573 2c0a 2020 2020 2020 636f  atures,.      co
-00024950: 756c 6420 6265 2074 7572 6e65 6420 6f66  uld be turned of
-00024960: 6620 666f 7220 6c61 7374 206c 6179 6572  f for last layer
-00024970: 0a20 2020 2069 6e69 743a 2073 7472 2c20  .    init: str, 
-00024980: 6f70 7469 6f6e 616c 2028 6465 6661 756c  optional (defaul
-00024990: 7420 2778 6176 6965 725f 756e 6966 6f72  t 'xavier_unifor
-000249a0: 6d5f 2729 0a20 2020 2020 2057 6569 6768  m_').      Weigh
-000249b0: 7420 696e 6974 6961 6c69 7a61 7469 6f6e  t initialization
-000249c0: 2066 6f72 2066 696c 7465 7273 2e0a 2020   for filters..  
-000249d0: 2020 6163 7469 7661 7469 6f6e 3a20 7374    activation: st
-000249e0: 722c 206f 7074 696f 6e61 6c20 2864 6566  r, optional (def
-000249f0: 6175 6c74 2027 7265 6c75 2729 0a20 2020  ault 'relu').   
-00024a00: 2020 2041 6374 6976 6174 696f 6e20 6675     Activation fu
-00024a10: 6e63 7469 6f6e 2061 7070 6c69 6564 0a20  nction applied. 
-00024a20: 2020 2062 6174 6368 5f6e 6f72 6d61 6c69     batch_normali
-00024a30: 7a65 3a20 626f 6f6c 2c20 6f70 7469 6f6e  ze: bool, option
-00024a40: 616c 2028 6465 6661 756c 7420 5472 7565  al (default True
-00024a50: 290a 2020 2020 2020 4966 2074 6869 7320  ).      If this 
-00024a60: 6973 2074 7572 6e65 6420 6f6e 2c20 6170  is turned on, ap
-00024a70: 706c 7920 6261 7463 6820 6e6f 726d 616c  ply batch normal
-00024a80: 697a 6174 696f 6e20 6265 666f 7265 2061  ization before a
-00024a90: 7070 6c79 696e 670a 2020 2020 2020 6163  pplying.      ac
-00024aa0: 7469 7661 7469 6f6e 2066 756e 6374 696f  tivation functio
-00024ab0: 6e73 206f 6e20 636f 6e76 6f6c 7574 696f  ns on convolutio
-00024ac0: 6e61 6c20 6c61 7965 7273 2e0a 2020 2020  nal layers..    
-00024ad0: 2222 220a 2020 2020 2020 2020 7375 7065  """.        supe
-00024ae0: 7228 5765 6176 654c 6179 6572 2c20 7365  r(WeaveLayer, se
-00024af0: 6c66 292e 5f5f 696e 6974 5f5f 282a 2a6b  lf).__init__(**k
-00024b00: 7761 7267 7329 0a20 2020 2020 2020 2073  wargs).        s
-00024b10: 656c 662e 696e 6974 3a20 7374 7220 3d20  elf.init: str = 
-00024b20: 696e 6974 5f20 2023 2053 6574 2077 6569  init_  # Set wei
-00024b30: 6768 7420 696e 6974 6961 6c69 7a61 7469  ght initializati
-00024b40: 6f6e 0a20 2020 2020 2020 2073 656c 662e  on.        self.
-00024b50: 6163 7469 7661 7469 6f6e 3a20 7374 7220  activation: str 
-00024b60: 3d20 6163 7469 7661 7469 6f6e 2020 2320  = activation  # 
-00024b70: 4765 7420 6163 7469 7661 7469 6f6e 730a  Get activations.
-00024b80: 2020 2020 2020 2020 7365 6c66 2e61 6374          self.act
-00024b90: 6976 6174 696f 6e5f 666e 3a20 746f 7263  ivation_fn: torc
-00024ba0: 682e 6e6e 2e4d 6f64 756c 6520 3d20 6765  h.nn.Module = ge
-00024bb0: 745f 6163 7469 7661 7469 6f6e 2861 6374  t_activation(act
-00024bc0: 6976 6174 696f 6e29 0a20 2020 2020 2020  ivation).       
-00024bd0: 2073 656c 662e 7570 6461 7465 5f70 6169   self.update_pai
-00024be0: 723a 2062 6f6f 6c20 3d20 7570 6461 7465  r: bool = update
-00024bf0: 5f70 6169 7220 2023 206c 6173 7420 7765  _pair  # last we
-00024c00: 6176 6520 6c61 7965 7220 646f 6573 206e  ave layer does n
-00024c10: 6f74 206e 6565 6420 746f 2075 7064 6174  ot need to updat
-00024c20: 650a 2020 2020 2020 2020 7365 6c66 2e6e  e.        self.n
-00024c30: 5f68 6964 6465 6e5f 4141 3a20 696e 7420  _hidden_AA: int 
-00024c40: 3d20 6e5f 6869 6464 656e 5f41 410a 2020  = n_hidden_AA.  
-00024c50: 2020 2020 2020 7365 6c66 2e6e 5f68 6964        self.n_hid
-00024c60: 6465 6e5f 5041 3a20 696e 7420 3d20 6e5f  den_PA: int = n_
-00024c70: 6869 6464 656e 5f50 410a 2020 2020 2020  hidden_PA.      
-00024c80: 2020 7365 6c66 2e6e 5f68 6964 6465 6e5f    self.n_hidden_
-00024c90: 4150 3a20 696e 7420 3d20 6e5f 6869 6464  AP: int = n_hidd
-00024ca0: 656e 5f41 500a 2020 2020 2020 2020 7365  en_AP.        se
-00024cb0: 6c66 2e6e 5f68 6964 6465 6e5f 5050 3a20  lf.n_hidden_PP: 
-00024cc0: 696e 7420 3d20 6e5f 6869 6464 656e 5f50  int = n_hidden_P
-00024cd0: 500a 2020 2020 2020 2020 7365 6c66 2e6e  P.        self.n
-00024ce0: 5f68 6964 6465 6e5f 413a 2069 6e74 203d  _hidden_A: int =
-00024cf0: 206e 5f68 6964 6465 6e5f 4141 202b 206e   n_hidden_AA + n
-00024d00: 5f68 6964 6465 6e5f 5041 0a20 2020 2020  _hidden_PA.     
-00024d10: 2020 2073 656c 662e 6e5f 6869 6464 656e     self.n_hidden
-00024d20: 5f50 3a20 696e 7420 3d20 6e5f 6869 6464  _P: int = n_hidd
-00024d30: 656e 5f41 5020 2b20 6e5f 6869 6464 656e  en_AP + n_hidden
-00024d40: 5f50 500a 2020 2020 2020 2020 7365 6c66  _PP.        self
-00024d50: 2e62 6174 6368 5f6e 6f72 6d61 6c69 7a65  .batch_normalize
-00024d60: 3a20 626f 6f6c 203d 2062 6174 6368 5f6e  : bool = batch_n
-00024d70: 6f72 6d61 6c69 7a65 0a0a 2020 2020 2020  ormalize..      
-00024d80: 2020 7365 6c66 2e6e 5f61 746f 6d5f 696e    self.n_atom_in
-00024d90: 7075 745f 6665 6174 3a20 696e 7420 3d20  put_feat: int = 
-00024da0: 6e5f 6174 6f6d 5f69 6e70 7574 5f66 6561  n_atom_input_fea
-00024db0: 740a 2020 2020 2020 2020 7365 6c66 2e6e  t.        self.n
-00024dc0: 5f70 6169 725f 696e 7075 745f 6665 6174  _pair_input_feat
-00024dd0: 3a20 696e 7420 3d20 6e5f 7061 6972 5f69  : int = n_pair_i
-00024de0: 6e70 7574 5f66 6561 740a 2020 2020 2020  nput_feat.      
-00024df0: 2020 7365 6c66 2e6e 5f61 746f 6d5f 6f75    self.n_atom_ou
-00024e00: 7470 7574 5f66 6561 743a 2069 6e74 203d  tput_feat: int =
-00024e10: 206e 5f61 746f 6d5f 6f75 7470 7574 5f66   n_atom_output_f
-00024e20: 6561 740a 2020 2020 2020 2020 7365 6c66  eat.        self
-00024e30: 2e6e 5f70 6169 725f 6f75 7470 7574 5f66  .n_pair_output_f
-00024e40: 6561 743a 2069 6e74 203d 206e 5f70 6169  eat: int = n_pai
-00024e50: 725f 6f75 7470 7574 5f66 6561 740a 0a20  r_output_feat.. 
-00024e60: 2020 2020 2020 2023 2043 6f6e 7374 7275         # Constru
-00024e70: 6374 2069 6e74 6572 6e61 6c20 7472 6169  ct internal trai
-00024e80: 6e61 626c 6520 7765 6967 6874 730a 2020  nable weights.  
-00024e90: 2020 2020 2020 696e 6974 203d 2067 6574        init = get
-00024ea0: 6174 7472 2869 6e69 7469 616c 697a 6572  attr(initializer
-00024eb0: 732c 2073 656c 662e 696e 6974 290a 2020  s, self.init).  
-00024ec0: 2020 2020 2020 2320 5765 6967 6874 206d        # Weight m
-00024ed0: 6174 7269 7820 616e 6420 6269 6173 206d  atrix and bias m
-00024ee0: 6174 7269 7820 7265 7175 6972 6564 2074  atrix required t
-00024ef0: 6f20 636f 6d70 7574 6520 6e65 7720 6174  o compute new at
-00024f00: 6f6d 206c 6179 6572 2066 726f 6d20 7468  om layer from th
-00024f10: 6520 7072 6576 696f 7573 2061 746f 6d20  e previous atom 
-00024f20: 6c61 7965 720a 2020 2020 2020 2020 7365  layer.        se
-00024f30: 6c66 2e57 5f41 413a 2074 6f72 6368 2e54  lf.W_AA: torch.T
-00024f40: 656e 736f 7220 3d20 696e 6974 280a 2020  ensor = init(.  
-00024f50: 2020 2020 2020 2020 2020 746f 7263 682e            torch.
-00024f60: 656d 7074 7928 7365 6c66 2e6e 5f61 746f  empty(self.n_ato
-00024f70: 6d5f 696e 7075 745f 6665 6174 2c20 7365  m_input_feat, se
-00024f80: 6c66 2e6e 5f68 6964 6465 6e5f 4141 2929  lf.n_hidden_AA))
-00024f90: 0a20 2020 2020 2020 2073 656c 662e 625f  .        self.b_
-00024fa0: 4141 3a20 746f 7263 682e 5465 6e73 6f72  AA: torch.Tensor
-00024fb0: 203d 2074 6f72 6368 2e7a 6572 6f73 2828   = torch.zeros((
-00024fc0: 7365 6c66 2e6e 5f68 6964 6465 6e5f 4141  self.n_hidden_AA
-00024fd0: 2c29 290a 2020 2020 2020 2020 7365 6c66  ,)).        self
-00024fe0: 2e41 415f 626e 3a20 6e6e 2e42 6174 6368  .AA_bn: nn.Batch
-00024ff0: 4e6f 726d 3164 203d 206e 6e2e 4261 7463  Norm1d = nn.Batc
-00025000: 684e 6f72 6d31 6428 0a20 2020 2020 2020  hNorm1d(.       
-00025010: 2020 2020 206e 756d 5f66 6561 7475 7265       num_feature
-00025020: 733d 7365 6c66 2e6e 5f68 6964 6465 6e5f  s=self.n_hidden_
-00025030: 4141 2c0a 2020 2020 2020 2020 2020 2020  AA,.            
-00025040: 6570 733d 3165 2d33 2c0a 2020 2020 2020  eps=1e-3,.      
-00025050: 2020 2020 2020 6d6f 6d65 6e74 756d 3d30        momentum=0
-00025060: 2e39 392c 0a20 2020 2020 2020 2020 2020  .99,.           
-00025070: 2061 6666 696e 653d 5472 7565 2c0a 2020   affine=True,.  
-00025080: 2020 2020 2020 2020 2020 7472 6163 6b5f            track_
-00025090: 7275 6e6e 696e 675f 7374 6174 733d 5472  running_stats=Tr
-000250a0: 7565 290a 0a20 2020 2020 2020 2023 2057  ue)..        # W
-000250b0: 6569 6768 7420 6d61 7472 6978 2061 6e64  eight matrix and
-000250c0: 2062 6961 7320 6d61 7472 6978 2072 6571   bias matrix req
-000250d0: 7569 7265 6420 746f 2063 6f6d 7075 7465  uired to compute
-000250e0: 206e 6577 2061 746f 6d20 6c61 7965 7220   new atom layer 
-000250f0: 6672 6f6d 2074 6865 2070 7265 7669 6f75  from the previou
-00025100: 7320 7061 6972 206c 6179 6572 0a20 2020  s pair layer.   
-00025110: 2020 2020 2073 656c 662e 575f 5041 3a20       self.W_PA: 
-00025120: 746f 7263 682e 5465 6e73 6f72 203d 2069  torch.Tensor = i
-00025130: 6e69 7428 0a20 2020 2020 2020 2020 2020  nit(.           
-00025140: 2074 6f72 6368 2e65 6d70 7479 2873 656c   torch.empty(sel
-00025150: 662e 6e5f 7061 6972 5f69 6e70 7574 5f66  f.n_pair_input_f
-00025160: 6561 742c 2073 656c 662e 6e5f 6869 6464  eat, self.n_hidd
-00025170: 656e 5f50 4129 290a 2020 2020 2020 2020  en_PA)).        
-00025180: 7365 6c66 2e62 5f50 413a 2074 6f72 6368  self.b_PA: torch
-00025190: 2e54 656e 736f 7220 3d20 746f 7263 682e  .Tensor = torch.
-000251a0: 7a65 726f 7328 2873 656c 662e 6e5f 6869  zeros((self.n_hi
-000251b0: 6464 656e 5f50 412c 2929 0a20 2020 2020  dden_PA,)).     
-000251c0: 2020 2073 656c 662e 5041 5f62 6e3a 206e     self.PA_bn: n
-000251d0: 6e2e 4261 7463 684e 6f72 6d31 6420 3d20  n.BatchNorm1d = 
-000251e0: 6e6e 2e42 6174 6368 4e6f 726d 3164 280a  nn.BatchNorm1d(.
-000251f0: 2020 2020 2020 2020 2020 2020 6e75 6d5f              num_
-00025200: 6665 6174 7572 6573 3d73 656c 662e 6e5f  features=self.n_
-00025210: 6869 6464 656e 5f50 412c 0a20 2020 2020  hidden_PA,.     
-00025220: 2020 2020 2020 2065 7073 3d31 652d 332c         eps=1e-3,
-00025230: 0a20 2020 2020 2020 2020 2020 206d 6f6d  .            mom
-00025240: 656e 7475 6d3d 302e 3939 2c0a 2020 2020  entum=0.99,.    
-00025250: 2020 2020 2020 2020 6166 6669 6e65 3d54          affine=T
-00025260: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-00025270: 2074 7261 636b 5f72 756e 6e69 6e67 5f73   track_running_s
-00025280: 7461 7473 3d54 7275 6529 0a0a 2020 2020  tats=True)..    
-00025290: 2020 2020 7365 6c66 2e57 5f41 3a20 746f      self.W_A: to
-000252a0: 7263 682e 5465 6e73 6f72 203d 2069 6e69  rch.Tensor = ini
-000252b0: 7428 0a20 2020 2020 2020 2020 2020 2074  t(.            t
-000252c0: 6f72 6368 2e65 6d70 7479 2873 656c 662e  orch.empty(self.
-000252d0: 6e5f 6869 6464 656e 5f41 2c20 7365 6c66  n_hidden_A, self
-000252e0: 2e6e 5f61 746f 6d5f 6f75 7470 7574 5f66  .n_atom_output_f
-000252f0: 6561 7429 290a 2020 2020 2020 2020 7365  eat)).        se
-00025300: 6c66 2e62 5f41 3a20 746f 7263 682e 5465  lf.b_A: torch.Te
-00025310: 6e73 6f72 203d 2074 6f72 6368 2e7a 6572  nsor = torch.zer
-00025320: 6f73 2828 7365 6c66 2e6e 5f61 746f 6d5f  os((self.n_atom_
-00025330: 6f75 7470 7574 5f66 6561 742c 2929 0a20  output_feat,)). 
-00025340: 2020 2020 2020 2073 656c 662e 415f 626e         self.A_bn
-00025350: 3a20 6e6e 2e42 6174 6368 4e6f 726d 3164  : nn.BatchNorm1d
-00025360: 203d 206e 6e2e 4261 7463 684e 6f72 6d31   = nn.BatchNorm1
-00025370: 6428 0a20 2020 2020 2020 2020 2020 206e  d(.            n
-00025380: 756d 5f66 6561 7475 7265 733d 7365 6c66  um_features=self
-00025390: 2e6e 5f61 746f 6d5f 6f75 7470 7574 5f66  .n_atom_output_f
-000253a0: 6561 742c 0a20 2020 2020 2020 2020 2020  eat,.           
-000253b0: 2065 7073 3d31 652d 332c 0a20 2020 2020   eps=1e-3,.     
-000253c0: 2020 2020 2020 206d 6f6d 656e 7475 6d3d         momentum=
-000253d0: 302e 3939 2c0a 2020 2020 2020 2020 2020  0.99,.          
-000253e0: 2020 6166 6669 6e65 3d54 7275 652c 0a20    affine=True,. 
-000253f0: 2020 2020 2020 2020 2020 2074 7261 636b             track
-00025400: 5f72 756e 6e69 6e67 5f73 7461 7473 3d54  _running_stats=T
-00025410: 7275 6529 0a0a 2020 2020 2020 2020 6966  rue)..        if
-00025420: 2073 656c 662e 7570 6461 7465 5f70 6169   self.update_pai
-00025430: 723a 0a20 2020 2020 2020 2020 2020 2023  r:.            #
-00025440: 2057 6569 6768 7420 6d61 7472 6978 2061   Weight matrix a
-00025450: 6e64 2062 6961 7320 6d61 7472 6978 2072  nd bias matrix r
-00025460: 6571 7569 7265 6420 746f 2063 6f6d 7075  equired to compu
-00025470: 7465 206e 6577 2070 6169 7220 6c61 7965  te new pair laye
-00025480: 7220 6672 6f6d 2074 6865 2070 7265 7669  r from the previ
-00025490: 6f75 7320 6174 6f6d 206c 6179 6572 0a20  ous atom layer. 
-000254a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000254b0: 575f 4150 3a20 746f 7263 682e 5465 6e73  W_AP: torch.Tens
-000254c0: 6f72 203d 2069 6e69 7428 0a20 2020 2020  or = init(.     
-000254d0: 2020 2020 2020 2020 2020 2074 6f72 6368             torch
-000254e0: 2e65 6d70 7479 2873 656c 662e 6e5f 6174  .empty(self.n_at
-000254f0: 6f6d 5f69 6e70 7574 5f66 6561 7420 2a20  om_input_feat * 
-00025500: 322c 2073 656c 662e 6e5f 6869 6464 656e  2, self.n_hidden
-00025510: 5f41 5029 290a 2020 2020 2020 2020 2020  _AP)).          
-00025520: 2020 7365 6c66 2e62 5f41 503a 2074 6f72    self.b_AP: tor
-00025530: 6368 2e54 656e 736f 7220 3d20 746f 7263  ch.Tensor = torc
-00025540: 682e 7a65 726f 7328 2873 656c 662e 6e5f  h.zeros((self.n_
-00025550: 6869 6464 656e 5f41 502c 2929 0a20 2020  hidden_AP,)).   
-00025560: 2020 2020 2020 2020 2073 656c 662e 4150           self.AP
-00025570: 5f62 6e3a 206e 6e2e 4261 7463 684e 6f72  _bn: nn.BatchNor
-00025580: 6d31 6420 3d20 6e6e 2e42 6174 6368 4e6f  m1d = nn.BatchNo
-00025590: 726d 3164 280a 2020 2020 2020 2020 2020  rm1d(.          
-000255a0: 2020 2020 2020 6e75 6d5f 6665 6174 7572        num_featur
-000255b0: 6573 3d73 656c 662e 6e5f 6869 6464 656e  es=self.n_hidden
-000255c0: 5f41 502c 0a20 2020 2020 2020 2020 2020  _AP,.           
-000255d0: 2020 2020 2065 7073 3d31 652d 332c 0a20       eps=1e-3,. 
-000255e0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000255f0: 6f6d 656e 7475 6d3d 302e 3939 2c0a 2020  omentum=0.99,.  
-00025600: 2020 2020 2020 2020 2020 2020 2020 6166                af
-00025610: 6669 6e65 3d54 7275 652c 0a20 2020 2020  fine=True,.     
-00025620: 2020 2020 2020 2020 2020 2074 7261 636b             track
-00025630: 5f72 756e 6e69 6e67 5f73 7461 7473 3d54  _running_stats=T
-00025640: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
-00025650: 2023 2057 6569 6768 7420 6d61 7472 6978   # Weight matrix
-00025660: 2061 6e64 2062 6961 7320 6d61 7472 6978   and bias matrix
-00025670: 2072 6571 7569 7265 6420 746f 2063 6f6d   required to com
-00025680: 7075 7465 206e 6577 2070 6169 7220 6c61  pute new pair la
-00025690: 7965 7220 6672 6f6d 2074 6865 2070 7265  yer from the pre
-000256a0: 7669 6f75 7320 7061 6972 206c 6179 6572  vious pair layer
-000256b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000256c0: 662e 575f 5050 3a20 746f 7263 682e 5465  f.W_PP: torch.Te
-000256d0: 6e73 6f72 203d 2069 6e69 7428 0a20 2020  nsor = init(.   
-000256e0: 2020 2020 2020 2020 2020 2020 2074 6f72               tor
-000256f0: 6368 2e65 6d70 7479 2873 656c 662e 6e5f  ch.empty(self.n_
-00025700: 7061 6972 5f69 6e70 7574 5f66 6561 742c  pair_input_feat,
-00025710: 2073 656c 662e 6e5f 6869 6464 656e 5f50   self.n_hidden_P
-00025720: 5029 290a 2020 2020 2020 2020 2020 2020  P)).            
-00025730: 7365 6c66 2e62 5f50 503a 2074 6f72 6368  self.b_PP: torch
-00025740: 2e54 656e 736f 7220 3d20 746f 7263 682e  .Tensor = torch.
-00025750: 7a65 726f 7328 2873 656c 662e 6e5f 6869  zeros((self.n_hi
-00025760: 6464 656e 5f50 502c 2929 0a20 2020 2020  dden_PP,)).     
-00025770: 2020 2020 2020 2073 656c 662e 5050 5f62         self.PP_b
-00025780: 6e3a 206e 6e2e 4261 7463 684e 6f72 6d31  n: nn.BatchNorm1
-00025790: 6420 3d20 6e6e 2e42 6174 6368 4e6f 726d  d = nn.BatchNorm
-000257a0: 3164 280a 2020 2020 2020 2020 2020 2020  1d(.            
-000257b0: 2020 2020 6e75 6d5f 6665 6174 7572 6573      num_features
-000257c0: 3d73 656c 662e 6e5f 6869 6464 656e 5f50  =self.n_hidden_P
-000257d0: 502c 0a20 2020 2020 2020 2020 2020 2020  P,.             
-000257e0: 2020 2065 7073 3d31 652d 332c 0a20 2020     eps=1e-3,.   
-000257f0: 2020 2020 2020 2020 2020 2020 206d 6f6d               mom
-00025800: 656e 7475 6d3d 302e 3939 2c0a 2020 2020  entum=0.99,.    
-00025810: 2020 2020 2020 2020 2020 2020 6166 6669              affi
-00025820: 6e65 3d54 7275 652c 0a20 2020 2020 2020  ne=True,.       
-00025830: 2020 2020 2020 2020 2074 7261 636b 5f72           track_r
-00025840: 756e 6e69 6e67 5f73 7461 7473 3d54 7275  unning_stats=Tru
-00025850: 6529 0a0a 2020 2020 2020 2020 2020 2020  e)..            
-00025860: 7365 6c66 2e57 5f50 3a20 746f 7263 682e  self.W_P: torch.
-00025870: 5465 6e73 6f72 203d 2069 6e69 7428 0a20  Tensor = init(. 
-00025880: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00025890: 6f72 6368 2e65 6d70 7479 2873 656c 662e  orch.empty(self.
-000258a0: 6e5f 6869 6464 656e 5f50 2c20 7365 6c66  n_hidden_P, self
-000258b0: 2e6e 5f70 6169 725f 6f75 7470 7574 5f66  .n_pair_output_f
-000258c0: 6561 7429 290a 2020 2020 2020 2020 2020  eat)).          
-000258d0: 2020 7365 6c66 2e62 5f50 3a20 746f 7263    self.b_P: torc
-000258e0: 682e 5465 6e73 6f72 203d 2074 6f72 6368  h.Tensor = torch
-000258f0: 2e7a 6572 6f73 2828 7365 6c66 2e6e 5f70  .zeros((self.n_p
-00025900: 6169 725f 6f75 7470 7574 5f66 6561 742c  air_output_feat,
-00025910: 2929 0a20 2020 2020 2020 2020 2020 2073  )).            s
-00025920: 656c 662e 505f 626e 3a20 6e6e 2e42 6174  elf.P_bn: nn.Bat
-00025930: 6368 4e6f 726d 3164 203d 206e 6e2e 4261  chNorm1d = nn.Ba
-00025940: 7463 684e 6f72 6d31 6428 0a20 2020 2020  tchNorm1d(.     
-00025950: 2020 2020 2020 2020 2020 206e 756d 5f66             num_f
-00025960: 6561 7475 7265 733d 7365 6c66 2e6e 5f70  eatures=self.n_p
-00025970: 6169 725f 6f75 7470 7574 5f66 6561 742c  air_output_feat,
-00025980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00025990: 2065 7073 3d31 652d 332c 0a20 2020 2020   eps=1e-3,.     
-000259a0: 2020 2020 2020 2020 2020 206d 6f6d 656e             momen
-000259b0: 7475 6d3d 302e 3939 2c0a 2020 2020 2020  tum=0.99,.      
-000259c0: 2020 2020 2020 2020 2020 6166 6669 6e65            affine
-000259d0: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
-000259e0: 2020 2020 2020 2074 7261 636b 5f72 756e         track_run
-000259f0: 6e69 6e67 5f73 7461 7473 3d54 7275 6529  ning_stats=True)
-00025a00: 0a20 2020 2020 2020 2073 656c 662e 6275  .        self.bu
-00025a10: 696c 7420 3d20 5472 7565 0a0a 2020 2020  ilt = True..    
-00025a20: 6465 6620 5f5f 7265 7072 5f5f 2873 656c  def __repr__(sel
-00025a30: 6629 202d 3e20 7374 723a 0a20 2020 2020  f) -> str:.     
-00025a40: 2020 2022 2222 0a20 2020 2052 6574 7572     """.    Retur
-00025a50: 6e73 2061 2073 7472 696e 6720 7265 7072  ns a string repr
-00025a60: 6573 656e 7461 7469 6f6e 206f 6620 7468  esentation of th
-00025a70: 6520 6f62 6a65 6374 2e0a 0a20 2020 2052  e object...    R
-00025a80: 6574 7572 6e73 3a0a 2020 2020 2d2d 2d2d  eturns:.    ----
-00025a90: 2d2d 2d0a 2020 2020 7374 723a 2041 2073  ---.    str: A s
-00025aa0: 7472 696e 6720 7468 6174 2063 6f6e 7461  tring that conta
-00025ab0: 696e 7320 7468 6520 636c 6173 7320 6e61  ins the class na
-00025ac0: 6d65 2066 6f6c 6c6f 7765 6420 6279 2074  me followed by t
-00025ad0: 6865 2076 616c 7565 7320 6f66 2069 7473  he values of its
-00025ae0: 2069 6e73 7461 6e63 6520 7661 7269 6162   instance variab
-00025af0: 6c65 2e0a 2020 2020 2222 220a 2020 2020  le..    """.    
-00025b00: 2020 2020 2320 666c 616b 6538 3a20 6e6f      # flake8: no
-00025b10: 7161 0a20 2020 2020 2020 2072 6574 7572  qa.        retur
-00025b20: 6e20 280a 2020 2020 2020 2020 2020 2020  n (.            
-00025b30: 6627 7b73 656c 662e 5f5f 636c 6173 735f  f'{self.__class_
-00025b40: 5f2e 5f5f 6e61 6d65 5f5f 7d28 6e5f 6174  _.__name__}(n_at
-00025b50: 6f6d 5f69 6e70 7574 5f66 6561 743a 7b73  om_input_feat:{s
-00025b60: 656c 662e 6e5f 6174 6f6d 5f69 6e70 7574  elf.n_atom_input
-00025b70: 5f66 6561 747d 2c6e 5f70 6169 725f 696e  _feat},n_pair_in
-00025b80: 7075 745f 6665 6174 3a7b 7365 6c66 2e6e  put_feat:{self.n
-00025b90: 5f70 6169 725f 696e 7075 745f 6665 6174  _pair_input_feat
-00025ba0: 7d2c 6e5f 6174 6f6d 5f6f 7574 7075 745f  },n_atom_output_
-00025bb0: 6665 6174 3a7b 7365 6c66 2e6e 5f61 746f  feat:{self.n_ato
-00025bc0: 6d5f 6f75 7470 7574 5f66 6561 747d 2c6e  m_output_feat},n
-00025bd0: 5f70 6169 725f 6f75 7470 7574 5f66 6561  _pair_output_fea
-00025be0: 743a 7b73 656c 662e 6e5f 7061 6972 5f6f  t:{self.n_pair_o
-00025bf0: 7574 7075 745f 6665 6174 7d2c 6e5f 6869  utput_feat},n_hi
-00025c00: 6464 656e 5f41 413a 7b73 656c 662e 6e5f  dden_AA:{self.n_
-00025c10: 6869 6464 656e 5f41 417d 2c6e 5f68 6964  hidden_AA},n_hid
-00025c20: 6465 6e5f 5041 3a7b 7365 6c66 2e6e 5f68  den_PA:{self.n_h
-00025c30: 6964 6465 6e5f 5041 7d2c 6e5f 6869 6464  idden_PA},n_hidd
-00025c40: 656e 5f41 503a 7b73 656c 662e 6e5f 6869  en_AP:{self.n_hi
-00025c50: 6464 656e 5f41 507d 2c6e 5f68 6964 6465  dden_AP},n_hidde
-00025c60: 6e5f 5050 3a7b 7365 6c66 2e6e 5f68 6964  n_PP:{self.n_hid
-00025c70: 6465 6e5f 5050 7d2c 6261 7463 685f 6e6f  den_PP},batch_no
-00025c80: 726d 616c 697a 653a 7b73 656c 662e 6261  rmalize:{self.ba
-00025c90: 7463 685f 6e6f 726d 616c 697a 657d 2c75  tch_normalize},u
-00025ca0: 7064 6174 655f 7061 6972 3a7b 7365 6c66  pdate_pair:{self
-00025cb0: 2e75 7064 6174 655f 7061 6972 7d2c 696e  .update_pair},in
-00025cc0: 6974 3a7b 7365 6c66 2e69 6e69 747d 2c61  it:{self.init},a
-00025cd0: 6374 6976 6174 696f 6e3a 7b73 656c 662e  ctivation:{self.
-00025ce0: 6163 7469 7661 7469 6f6e 7d29 270a 2020  activation})'.  
-00025cf0: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
-00025d00: 2066 6f72 7761 7264 280a 2020 2020 2020   forward(.      
-00025d10: 2020 7365 6c66 2c20 696e 7075 7473 3a20    self, inputs: 
-00025d20: 4c69 7374 5b55 6e69 6f6e 5b6e 702e 6e64  List[Union[np.nd
-00025d30: 6172 7261 792c 206e 702e 6e64 6172 7261  array, np.ndarra
-00025d40: 792c 206e 702e 6e64 6172 7261 792c 0a20  y, np.ndarray,. 
-00025d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025d70: 6e70 2e6e 6461 7272 6179 5d5d 0a20 2020  np.ndarray]].   
-00025d80: 2029 202d 3e20 4c69 7374 5b55 6e69 6f6e   ) -> List[Union
-00025d90: 5b74 6f72 6368 2e54 656e 736f 722c 2074  [torch.Tensor, t
-00025da0: 6f72 6368 2e54 656e 736f 725d 5d3a 0a20  orch.Tensor]]:. 
-00025db0: 2020 2020 2020 2022 2222 0a20 2020 2043         """.    C
-00025dc0: 7265 6174 6573 2077 6561 7665 2074 656e  reates weave ten
-00025dd0: 736f 7273 2e0a 0a20 2020 2050 6172 616d  sors...    Param
-00025de0: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
-00025df0: 2d2d 2d2d 0a20 2020 2069 6e70 7574 733a  ----.    inputs:
-00025e00: 204c 6973 745b 556e 696f 6e5b 6e70 2e6e   List[Union[np.n
-00025e10: 6461 7272 6179 2c20 6e70 2e6e 6461 7272  darray, np.ndarr
-00025e20: 6179 2c20 6e70 2e6e 6461 7272 6179 2c20  ay, np.ndarray, 
-00025e30: 6e70 2e6e 6461 7272 6179 5d5d 0a20 2020  np.ndarray]].   
-00025e40: 2053 686f 756c 6420 636f 6e74 6169 6e20   Should contain 
-00025e50: 3420 7465 6e73 6f72 7320 5b61 746f 6d5f  4 tensors [atom_
-00025e60: 6665 6174 7572 6573 2c20 7061 6972 5f66  features, pair_f
-00025e70: 6561 7475 7265 732c 2070 6169 725f 7370  eatures, pair_sp
-00025e80: 6c69 742c 0a20 2020 2061 746f 6d5f 746f  lit,.    atom_to
-00025e90: 5f70 6169 725d 0a0a 2020 2020 5265 7475  _pair]..    Retu
-00025ea0: 726e 733a 0a20 2020 202d 2d2d 2d2d 2d2d  rns:.    -------
-00025eb0: 0a20 2020 204c 6973 745b 556e 696f 6e5b  .    List[Union[
-00025ec0: 746f 7263 682e 5465 6e73 6f72 2c20 746f  torch.Tensor, to
-00025ed0: 7263 682e 5465 6e73 6f72 5d5d 0a20 2020  rch.Tensor]].   
-00025ee0: 2020 2041 3a20 4174 6f6d 2066 6561 7475     A: Atom featu
-00025ef0: 7265 7320 7465 6e73 6f72 2077 6974 6820  res tensor with 
-00025f00: 7368 6170 655b 746f 7461 6c5f 6e75 6d5f  shape[total_num_
-00025f10: 6174 6f6d 732c 6174 6f6d 2066 6561 7475  atoms,atom featu
-00025f20: 7265 2073 697a 655d 0a20 2020 2020 2050  re size].      P
-00025f30: 3a20 5061 6972 2066 6561 7475 7265 7320  : Pair features 
-00025f40: 7465 6e73 6f72 2077 6974 6820 7368 6170  tensor with shap
-00025f50: 655b 746f 7461 6c20 6e75 6d20 6f66 2070  e[total num of p
-00025f60: 6169 7273 2c62 6f6e 6420 6665 6174 7572  airs,bond featur
-00025f70: 6520 7369 7a65 5d0a 2020 2020 2222 220a  e size].    """.
-00025f80: 2020 2020 2020 2020 2320 436f 6e76 6572          # Conver
-00025f90: 7469 6e67 2074 6865 2069 6e70 7574 2074  ting the input t
-00025fa0: 6f20 746f 7263 6820 7465 6e73 6f72 730a  o torch tensors.
-00025fb0: 2020 2020 2020 2020 6174 6f6d 5f66 6561          atom_fea
-00025fc0: 7475 7265 733a 2074 6f72 6368 2e54 656e  tures: torch.Ten
-00025fd0: 736f 7220 3d20 746f 7263 682e 7465 6e73  sor = torch.tens
-00025fe0: 6f72 2869 6e70 7574 735b 305d 290a 2020  or(inputs[0]).  
-00025ff0: 2020 2020 2020 7061 6972 5f66 6561 7475        pair_featu
-00026000: 7265 733a 2074 6f72 6368 2e54 656e 736f  res: torch.Tenso
-00026010: 7220 3d20 746f 7263 682e 7465 6e73 6f72  r = torch.tensor
-00026020: 2869 6e70 7574 735b 315d 290a 0a20 2020  (inputs[1])..   
-00026030: 2020 2020 2070 6169 725f 7370 6c69 743a       pair_split:
-00026040: 2074 6f72 6368 2e54 656e 736f 7220 3d20   torch.Tensor = 
-00026050: 746f 7263 682e 7465 6e73 6f72 2869 6e70  torch.tensor(inp
-00026060: 7574 735b 325d 290a 2020 2020 2020 2020  uts[2]).        
-00026070: 6174 6f6d 5f74 6f5f 7061 6972 3a20 746f  atom_to_pair: to
-00026080: 7263 682e 5465 6e73 6f72 203d 2074 6f72  rch.Tensor = tor
-00026090: 6368 2e74 656e 736f 7228 696e 7075 7473  ch.tensor(inputs
-000260a0: 5b33 5d29 0a0a 2020 2020 2020 2020 6163  [3])..        ac
-000260b0: 7469 7661 7469 6f6e 203d 2073 656c 662e  tivation = self.
-000260c0: 6163 7469 7661 7469 6f6e 5f66 6e0a 0a20  activation_fn.. 
-000260d0: 2020 2020 2020 2023 2041 4120 6973 2061         # AA is a
-000260e0: 2074 656e 736f 7220 7769 7468 2073 6861   tensor with sha
-000260f0: 7065 5b74 6f74 616c 5f6e 756d 5f61 746f  pe[total_num_ato
-00026100: 6d73 2c6e 5f68 6964 6465 6e5f 4141 5d0a  ms,n_hidden_AA].
-00026110: 2020 2020 2020 2020 4141 3a20 746f 7263          AA: torc
-00026120: 682e 5465 6e73 6f72 203d 2074 6f72 6368  h.Tensor = torch
-00026130: 2e6d 6174 6d75 6c28 6174 6f6d 5f66 6561  .matmul(atom_fea
-00026140: 7475 7265 732e 7479 7065 2874 6f72 6368  tures.type(torch
-00026150: 2e66 6c6f 6174 3332 292c 0a20 2020 2020  .float32),.     
-00026160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026180: 2020 2073 656c 662e 575f 4141 2920 2b20     self.W_AA) + 
-00026190: 7365 6c66 2e62 5f41 410a 2020 2020 2020  self.b_AA.      
-000261a0: 2020 6966 2073 656c 662e 6261 7463 685f    if self.batch_
-000261b0: 6e6f 726d 616c 697a 653a 0a20 2020 2020  normalize:.     
-000261c0: 2020 2020 2020 2073 656c 662e 4141 5f62         self.AA_b
-000261d0: 6e2e 6576 616c 2829 0a20 2020 2020 2020  n.eval().       
-000261e0: 2020 2020 2041 4120 3d20 7365 6c66 2e41       AA = self.A
-000261f0: 415f 626e 2841 4129 0a20 2020 2020 2020  A_bn(AA).       
-00026200: 2041 4120 3d20 6163 7469 7661 7469 6f6e   AA = activation
-00026210: 2841 4129 0a20 2020 2020 2020 2023 2050  (AA).        # P
-00026220: 4120 6973 2061 2074 656e 736f 7220 7769  A is a tensor wi
-00026230: 7468 2073 6861 7065 5b74 6f74 616c 206e  th shape[total n
-00026240: 756d 6265 7220 6f66 2070 6169 7273 2c6e  umber of pairs,n
-00026250: 5f68 6964 6465 6e5f 5041 5d0a 2020 2020  _hidden_PA].    
-00026260: 2020 2020 5041 3a20 746f 7263 682e 5465      PA: torch.Te
-00026270: 6e73 6f72 203d 2074 6f72 6368 2e6d 6174  nsor = torch.mat
-00026280: 6d75 6c28 7061 6972 5f66 6561 7475 7265  mul(pair_feature
-00026290: 732e 7479 7065 2874 6f72 6368 2e66 6c6f  s.type(torch.flo
-000262a0: 6174 3332 292c 0a20 2020 2020 2020 2020  at32),.         
-000262b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000262c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000262d0: 656c 662e 575f 5041 2920 2b20 7365 6c66  elf.W_PA) + self
-000262e0: 2e62 5f50 410a 2020 2020 2020 2020 6966  .b_PA.        if
-000262f0: 2073 656c 662e 6261 7463 685f 6e6f 726d   self.batch_norm
-00026300: 616c 697a 653a 0a20 2020 2020 2020 2020  alize:.         
-00026310: 2020 2073 656c 662e 5041 5f62 6e2e 6576     self.PA_bn.ev
-00026320: 616c 2829 0a20 2020 2020 2020 2020 2020  al().           
-00026330: 2050 4120 3d20 7365 6c66 2e50 415f 626e   PA = self.PA_bn
-00026340: 2850 4129 0a20 2020 2020 2020 2050 4120  (PA).        PA 
-00026350: 3d20 6163 7469 7661 7469 6f6e 2850 4129  = activation(PA)
-00026360: 0a0a 2020 2020 2020 2020 2320 5370 6c69  ..        # Spli
-00026370: 7420 7468 6520 5041 2074 656e 736f 7220  t the PA tensor 
-00026380: 6163 636f 7264 696e 6720 746f 2074 6865  according to the
-00026390: 2027 7061 6972 5f73 706c 6974 2720 7465   'pair_split' te
-000263a0: 6e73 6f72 0a20 2020 2020 2020 2074 5f67  nsor.        t_g
-000263b0: 7270 3a20 4469 6374 5b54 656e 736f 722c  rp: Dict[Tensor,
-000263c0: 2054 656e 736f 725d 203d 207b 7d0a 2020   Tensor] = {}.  
-000263d0: 2020 2020 2020 6964 783a 2069 6e74 203d        idx: int =
-000263e0: 2030 0a20 2020 2020 2020 2066 6f72 2069   0.        for i
-000263f0: 2c20 735f 6964 2069 6e20 656e 756d 6572  , s_id in enumer
-00026400: 6174 6528 7061 6972 5f73 706c 6974 293a  ate(pair_split):
-00026410: 0a20 2020 2020 2020 2020 2020 2073 5f69  .            s_i
-00026420: 6420 3d20 735f 6964 2e69 7465 6d28 290a  d = s_id.item().
-00026430: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00026440: 5f69 6420 696e 2074 5f67 7270 3a0a 2020  _id in t_grp:.  
-00026450: 2020 2020 2020 2020 2020 2020 2020 745f                t_
-00026460: 6772 705b 735f 6964 5d20 3d20 745f 6772  grp[s_id] = t_gr
-00026470: 705b 735f 6964 5d20 2b20 5041 5b69 6478  p[s_id] + PA[idx
-00026480: 5d0a 2020 2020 2020 2020 2020 2020 656c  ].            el
-00026490: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000264a0: 2020 2020 745f 6772 705b 735f 6964 5d20      t_grp[s_id] 
-000264b0: 3d20 5041 5b69 6478 5d0a 2020 2020 2020  = PA[idx].      
-000264c0: 2020 2020 2020 6964 7820 3d20 6920 2b20        idx = i + 
-000264d0: 310a 0a20 2020 2020 2020 2020 2020 206c  1..            l
-000264e0: 7374 203d 206c 6973 7428 745f 6772 702e  st = list(t_grp.
-000264f0: 7661 6c75 6573 2829 290a 2020 2020 2020  values()).      
-00026500: 2020 2020 2020 7465 6e73 6f72 203d 2074        tensor = t
-00026510: 6f72 6368 2e73 7461 636b 286c 7374 290a  orch.stack(lst).
-00026520: 2020 2020 2020 2020 5041 203d 2074 656e          PA = ten
-00026530: 736f 720a 0a20 2020 2020 2020 2041 3a20  sor..        A: 
-00026540: 746f 7263 682e 5465 6e73 6f72 203d 2074  torch.Tensor = t
-00026550: 6f72 6368 2e6d 6174 6d75 6c28 746f 7263  orch.matmul(torc
-00026560: 682e 636f 6e63 6174 285b 4141 2c20 5041  h.concat([AA, PA
-00026570: 5d2c 2031 292c 0a20 2020 2020 2020 2020  ], 1),.         
-00026580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026590: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000265a0: 6c66 2e57 5f41 2920 2b20 7365 6c66 2e62  lf.W_A) + self.b
-000265b0: 5f41 0a20 2020 2020 2020 2069 6620 7365  _A.        if se
-000265c0: 6c66 2e62 6174 6368 5f6e 6f72 6d61 6c69  lf.batch_normali
-000265d0: 7a65 3a0a 2020 2020 2020 2020 2020 2020  ze:.            
-000265e0: 7365 6c66 2e41 5f62 6e2e 6576 616c 2829  self.A_bn.eval()
-000265f0: 0a20 2020 2020 2020 2020 2020 2041 203d  .            A =
-00026600: 2073 656c 662e 415f 626e 2841 290a 2020   self.A_bn(A).  
-00026610: 2020 2020 2020 4120 3d20 6163 7469 7661        A = activa
-00026620: 7469 6f6e 2841 290a 0a20 2020 2020 2020  tion(A)..       
-00026630: 2069 6620 7365 6c66 2e75 7064 6174 655f   if self.update_
-00026640: 7061 6972 3a0a 2020 2020 2020 2020 2020  pair:.          
-00026650: 2020 2320 4e6f 7465 2074 6861 7420 4150    # Note that AP
-00026660: 5f69 6a20 616e 6420 4150 5f6a 6920 7368  _ij and AP_ji sh
-00026670: 6172 6520 7468 6520 7361 6d65 2073 656c  are the same sel
-00026680: 662e 4150 5f62 6e20 6261 7463 680a 2020  f.AP_bn batch.  
-00026690: 2020 2020 2020 2020 2020 2320 6e6f 726d            # norm
-000266a0: 616c 697a 6174 696f 6e0a 2020 2020 2020  alization.      
-000266b0: 2020 2020 2020 4150 5f69 6a3a 2074 6f72        AP_ij: tor
-000266c0: 6368 2e54 656e 736f 7220 3d20 746f 7263  ch.Tensor = torc
-000266d0: 682e 6d61 746d 756c 280a 2020 2020 2020  h.matmul(.      
-000266e0: 2020 2020 2020 2020 2020 746f 7263 682e            torch.
-000266f0: 7265 7368 6170 6528 6174 6f6d 5f66 6561  reshape(atom_fea
-00026700: 7475 7265 735b 6174 6f6d 5f74 6f5f 7061  tures[atom_to_pa
-00026710: 6972 5d2c 0a20 2020 2020 2020 2020 2020  ir],.           
-00026720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026730: 2020 205b 2d31 2c20 3220 2a20 7365 6c66     [-1, 2 * self
-00026740: 2e6e 5f61 746f 6d5f 696e 7075 745f 6665  .n_atom_input_fe
-00026750: 6174 5d29 2e74 7970 6528 0a20 2020 2020  at]).type(.     
-00026760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026770: 2020 2020 2020 2020 2020 2020 2074 6f72               tor
-00026780: 6368 2e66 6c6f 6174 3332 292c 2073 656c  ch.float32), sel
-00026790: 662e 575f 4150 2920 2b20 7365 6c66 2e62  f.W_AP) + self.b
-000267a0: 5f41 500a 2020 2020 2020 2020 2020 2020  _AP.            
-000267b0: 6966 2073 656c 662e 6261 7463 685f 6e6f  if self.batch_no
-000267c0: 726d 616c 697a 653a 0a20 2020 2020 2020  rmalize:.       
-000267d0: 2020 2020 2020 2020 2073 656c 662e 4150           self.AP
-000267e0: 5f62 6e2e 6576 616c 2829 0a20 2020 2020  _bn.eval().     
-000267f0: 2020 2020 2020 2020 2020 2041 505f 696a             AP_ij
-00026800: 203d 2073 656c 662e 4150 5f62 6e28 4150   = self.AP_bn(AP
-00026810: 5f69 6a29 0a20 2020 2020 2020 2020 2020  _ij).           
-00026820: 2041 505f 696a 203d 2061 6374 6976 6174   AP_ij = activat
-00026830: 696f 6e28 4150 5f69 6a29 0a20 2020 2020  ion(AP_ij).     
-00026840: 2020 2020 2020 2041 505f 6a69 3a20 746f         AP_ji: to
-00026850: 7263 682e 5465 6e73 6f72 203d 2074 6f72  rch.Tensor = tor
-00026860: 6368 2e6d 6174 6d75 6c28 0a20 2020 2020  ch.matmul(.     
-00026870: 2020 2020 2020 2020 2020 2074 6f72 6368             torch
-00026880: 2e72 6573 6861 7065 2861 746f 6d5f 6665  .reshape(atom_fe
-00026890: 6174 7572 6573 5b74 6f72 6368 2e66 6c69  atures[torch.fli
-000268a0: 7028 6174 6f6d 5f74 6f5f 7061 6972 2c20  p(atom_to_pair, 
-000268b0: 5b31 5d29 5d2c 0a20 2020 2020 2020 2020  [1])],.         
-000268c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000268d0: 2020 2020 205b 2d31 2c20 3220 2a20 7365       [-1, 2 * se
-000268e0: 6c66 2e6e 5f61 746f 6d5f 696e 7075 745f  lf.n_atom_input_
-000268f0: 6665 6174 5d29 2e74 7970 6528 0a20 2020  feat]).type(.   
-00026900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026910: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00026920: 6f72 6368 2e66 6c6f 6174 3332 292c 2073  orch.float32), s
-00026930: 656c 662e 575f 4150 2920 2b20 7365 6c66  elf.W_AP) + self
-00026940: 2e62 5f41 500a 2020 2020 2020 2020 2020  .b_AP.          
-00026950: 2020 6966 2073 656c 662e 6261 7463 685f    if self.batch_
-00026960: 6e6f 726d 616c 697a 653a 0a20 2020 2020  normalize:.     
-00026970: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00026980: 4150 5f62 6e2e 6576 616c 2829 0a20 2020  AP_bn.eval().   
-00026990: 2020 2020 2020 2020 2020 2020 2041 505f               AP_
-000269a0: 6a69 203d 2073 656c 662e 4150 5f62 6e28  ji = self.AP_bn(
-000269b0: 4150 5f6a 6929 0a20 2020 2020 2020 2020  AP_ji).         
-000269c0: 2020 2041 505f 6a69 203d 2061 6374 6976     AP_ji = activ
-000269d0: 6174 696f 6e28 4150 5f6a 6929 0a20 2020  ation(AP_ji).   
-000269e0: 2020 2020 2020 2020 2023 2050 5020 6973           # PP is
-000269f0: 2061 2074 656e 736f 7220 7769 7468 2073   a tensor with s
-00026a00: 6861 7065 205b 746f 7461 6c20 6e75 6d62  hape [total numb
-00026a10: 6572 206f 6620 7061 6972 732c 6e5f 6869  er of pairs,n_hi
-00026a20: 6464 656e 5f50 505d 0a20 2020 2020 2020  dden_PP].       
-00026a30: 2020 2020 2050 503a 2074 6f72 6368 2e54       PP: torch.T
-00026a40: 656e 736f 7220 3d20 746f 7263 682e 6d61  ensor = torch.ma
-00026a50: 746d 756c 2870 6169 725f 6665 6174 7572  tmul(pair_featur
-00026a60: 6573 2e74 7970 6528 746f 7263 682e 666c  es.type(torch.fl
-00026a70: 6f61 7433 3229 2c0a 2020 2020 2020 2020  oat32),.        
-00026a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026aa0: 2020 2020 7365 6c66 2e57 5f50 5029 202b      self.W_PP) +
-00026ab0: 2073 656c 662e 625f 5050 0a20 2020 2020   self.b_PP.     
-00026ac0: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-00026ad0: 6174 6368 5f6e 6f72 6d61 6c69 7a65 3a0a  atch_normalize:.
-00026ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026af0: 7365 6c66 2e50 505f 626e 2e65 7661 6c28  self.PP_bn.eval(
-00026b00: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00026b10: 2020 5050 203d 2073 656c 662e 5050 5f62    PP = self.PP_b
-00026b20: 6e28 5050 290a 2020 2020 2020 2020 2020  n(PP).          
-00026b30: 2020 5050 203d 2061 6374 6976 6174 696f    PP = activatio
-00026b40: 6e28 5050 290a 2020 2020 2020 2020 2020  n(PP).          
-00026b50: 2020 503a 2074 6f72 6368 2e54 656e 736f    P: torch.Tenso
-00026b60: 7220 3d20 746f 7263 682e 6d61 746d 756c  r = torch.matmul
-00026b70: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00026b80: 2020 746f 7263 682e 636f 6e63 6174 285b    torch.concat([
-00026b90: 4150 5f69 6a20 2b20 4150 5f6a 692c 2050  AP_ij + AP_ji, P
-00026ba0: 505d 2c20 3129 2e74 7970 6528 746f 7263  P], 1).type(torc
-00026bb0: 682e 666c 6f61 7433 3229 2c0a 2020 2020  h.float32),.    
-00026bc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00026bd0: 2e57 5f50 2920 2b20 7365 6c66 2e62 5f50  .W_P) + self.b_P
-00026be0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00026bf0: 7365 6c66 2e62 6174 6368 5f6e 6f72 6d61  self.batch_norma
-00026c00: 6c69 7a65 3a0a 2020 2020 2020 2020 2020  lize:.          
-00026c10: 2020 2020 2020 7365 6c66 2e50 5f62 6e2e        self.P_bn.
-00026c20: 6576 616c 2829 0a20 2020 2020 2020 2020  eval().         
-00026c30: 2020 2020 2020 2050 203d 2073 656c 662e         P = self.
-00026c40: 505f 626e 2850 290a 2020 2020 2020 2020  P_bn(P).        
-00026c50: 2020 2020 5020 3d20 6163 7469 7661 7469      P = activati
-00026c60: 6f6e 2850 290a 2020 2020 2020 2020 656c  on(P).        el
-00026c70: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00026c80: 5020 3d20 7061 6972 5f66 6561 7475 7265  P = pair_feature
-00026c90: 730a 0a20 2020 2020 2020 2072 6574 7572  s..        retur
-00026ca0: 6e20 5b41 2c20 505d 0a0a 0a63 6c61 7373  n [A, P]...class
-00026cb0: 2057 6561 7665 4761 7468 6572 286e 6e2e   WeaveGather(nn.
-00026cc0: 4d6f 6475 6c65 293a 0a20 2020 2022 2222  Module):.    """
-00026cd0: 496d 706c 656d 656e 7473 2074 6865 2077  Implements the w
-00026ce0: 6561 7665 2d67 6174 6865 7269 6e67 2073  eave-gathering s
-00026cf0: 6563 7469 6f6e 206f 6620 7765 6176 6520  ection of weave 
-00026d00: 636f 6e76 6f6c 7574 696f 6e73 2e0a 2020  convolutions..  
-00026d10: 2020 5468 6973 2069 7320 7468 6520 546f    This is the To
-00026d20: 7263 6820 6571 7569 7661 6c65 6e74 206f  rch equivalent o
-00026d30: 6620 7468 6520 6f72 6967 696e 616c 2069  f the original i
-00026d40: 6d70 6c65 6d65 6e74 6174 696f 6e20 7573  mplementation us
-00026d50: 696e 6720 4b65 7261 732e 0a0a 2020 2020  ing Keras...    
-00026d60: 496d 706c 656d 656e 7473 2074 6865 2067  Implements the g
-00026d70: 6174 6865 7269 6e67 206c 6179 6572 2066  athering layer f
-00026d80: 726f 6d20 5b31 5d5f 2e20 5468 6520 7765  rom [1]_. The we
-00026d90: 6176 6520 6761 7468 6572 696e 6720 6c61  ave gathering la
-00026da0: 7965 7220 6761 7468 6572 730a 2020 2020  yer gathers.    
-00026db0: 7065 722d 6174 6f6d 2066 6561 7475 7265  per-atom feature
-00026dc0: 7320 746f 2063 7265 6174 6520 6120 6d6f  s to create a mo
-00026dd0: 6c65 6375 6c65 2d6c 6576 656c 2066 696e  lecule-level fin
-00026de0: 6765 7270 7269 6e74 2069 6e20 6120 7765  gerprint in a we
-00026df0: 6176 650a 2020 2020 636f 6e76 6f6c 7574  ave.    convolut
-00026e00: 696f 6e61 6c20 6e65 7477 6f72 6b2e 2054  ional network. T
-00026e10: 6869 7320 6c61 7965 7220 6361 6e20 616c  his layer can al
-00026e20: 736f 2070 6572 666f 726d 7320 4761 7573  so performs Gaus
-00026e30: 7369 616e 2068 6973 746f 6772 616d 0a20  sian histogram. 
-00026e40: 2020 2065 7870 616e 7369 6f6e 2061 7320     expansion as 
-00026e50: 6465 7461 696c 6564 2069 6e20 5b31 5d5f  detailed in [1]_
-00026e60: 2e20 4e6f 7465 2074 6861 7420 7468 6520  . Note that the 
-00026e70: 6761 7468 6572 696e 6720 6675 6e63 7469  gathering functi
-00026e80: 6f6e 2068 6572 6520 6973 0a20 2020 2073  on here is.    s
-00026e90: 696d 706c 7920 6164 6469 7469 6f6e 2061  imply addition a
-00026ea0: 7320 696e 205b 315d 5f3e 0a0a 2020 2020  s in [1]_>..    
-00026eb0: 4578 616d 706c 6573 0a20 2020 202d 2d2d  Examples.    ---
-00026ec0: 2d2d 2d2d 2d0a 2020 2020 5468 6973 206c  -----.    This l
-00026ed0: 6179 6572 2065 7870 6563 7473 2032 2069  ayer expects 2 i
-00026ee0: 6e70 7574 7320 696e 2061 206c 6973 7420  nputs in a list 
-00026ef0: 6f66 2074 6865 2066 6f72 6d20 605b 6174  of the form `[at
-00026f00: 6f6d 5f66 6561 7475 7265 732c 0a20 2020  om_features,.   
-00026f10: 2070 6169 725f 6665 6174 7572 6573 5d60   pair_features]`
-00026f20: 2e20 5765 276c 6c20 7761 6c6b 2074 6872  . We'll walk thr
-00026f30: 6f75 6768 2074 6865 2073 7472 7563 7475  ough the structu
-00026f40: 7265 0a20 2020 206f 6620 7468 6573 6520  re.    of these 
-00026f50: 696e 7075 7473 2e20 4c65 7427 7320 7374  inputs. Let's st
-00026f60: 6172 7420 7769 7468 2073 6f6d 6520 6261  art with some ba
-00026f70: 7369 6320 6465 6669 6e69 7469 6f6e 732e  sic definitions.
-00026f80: 0a0a 2020 2020 3e3e 3e20 696d 706f 7274  ..    >>> import
-00026f90: 2064 6565 7063 6865 6d20 6173 2064 630a   deepchem as dc.
-00026fa0: 2020 2020 3e3e 3e20 696d 706f 7274 206e      >>> import n
-00026fb0: 756d 7079 2061 7320 6e70 0a0a 2020 2020  umpy as np..    
-00026fc0: 5375 7070 6f73 6520 796f 7520 6861 7665  Suppose you have
-00026fd0: 2061 2062 6174 6368 206f 6620 6d6f 6c65   a batch of mole
-00026fe0: 6375 6c65 730a 0a20 2020 203e 3e3e 2073  cules..    >>> s
-00026ff0: 6d69 6c65 7320 3d20 5b22 4343 4322 2c20  miles = ["CCC", 
-00027000: 2243 225d 0a0a 2020 2020 4e6f 7465 2074  "C"]..    Note t
-00027010: 6861 7420 7468 6572 6520 6172 6520 3420  hat there are 4 
-00027020: 6174 6f6d 7320 696e 2074 6f74 616c 2069  atoms in total i
-00027030: 6e20 7468 6973 2073 7973 7465 6d2e 2054  n this system. T
-00027040: 6869 7320 6c61 7965 7220 6578 7065 6374  his layer expect
-00027050: 7320 6974 730a 2020 2020 696e 7075 7420  s its.    input 
-00027060: 6d6f 6c65 6375 6c65 7320 746f 2062 6520  molecules to be 
-00027070: 6261 7463 6865 6420 746f 6765 7468 6572  batched together
-00027080: 2e0a 0a20 2020 203e 3e3e 2074 6f74 616c  ...    >>> total
-00027090: 5f6e 5f61 746f 6d73 203d 2034 0a0a 2020  _n_atoms = 4..  
-000270a0: 2020 4c65 7427 7320 7375 7070 6f73 6520    Let's suppose 
-000270b0: 7468 6174 2077 6520 6861 7665 2060 6e5f  that we have `n_
-000270c0: 6174 6f6d 5f66 6561 7460 2066 6561 7475  atom_feat` featu
-000270d0: 7265 7320 7065 7220 6174 6f6d 2e0a 0a20  res per atom... 
-000270e0: 2020 203e 3e3e 206e 5f61 746f 6d5f 6665     >>> n_atom_fe
-000270f0: 6174 203d 2037 350a 0a20 2020 2054 6865  at = 75..    The
-00027100: 6e20 636f 6e63 6570 7475 616c 6c79 2c20  n conceptually, 
-00027110: 6061 746f 6d5f 6665 6174 6020 6973 2074  `atom_feat` is t
-00027120: 6865 2061 7272 6179 206f 6620 7368 6170  he array of shap
-00027130: 6520 6028 746f 7461 6c5f 6e5f 6174 6f6d  e `(total_n_atom
-00027140: 732c 0a20 2020 206e 5f61 746f 6d5f 6665  s,.    n_atom_fe
-00027150: 6174 2960 206f 6620 6174 6f6d 6963 2066  at)` of atomic f
-00027160: 6561 7475 7265 732e 2046 6f72 2073 696d  eatures. For sim
-00027170: 706c 6963 6974 792c 206c 6574 2773 206a  plicity, let's j
-00027180: 7573 7420 676f 2077 6974 6820 610a 2020  ust go with a.  
-00027190: 2020 7261 6e64 6f6d 2073 7563 6820 6d61    random such ma
-000271a0: 7472 6978 2e0a 0a20 2020 203e 3e3e 2061  trix...    >>> a
-000271b0: 746f 6d5f 6665 6174 203d 206e 702e 7261  tom_feat = np.ra
-000271c0: 6e64 6f6d 2e72 616e 6428 746f 7461 6c5f  ndom.rand(total_
-000271d0: 6e5f 6174 6f6d 732c 206e 5f61 746f 6d5f  n_atoms, n_atom_
-000271e0: 6665 6174 290a 0a20 2020 2057 6520 7468  feat)..    We th
-000271f0: 656e 206e 6565 6420 746f 2070 726f 7669  en need to provi
-00027200: 6465 2061 206d 6170 7069 6e67 206f 6620  de a mapping of 
-00027210: 696e 6469 6365 7320 746f 2074 6865 2061  indices to the a
-00027220: 746f 6d73 2074 6865 7920 6265 6c6f 6e67  toms they belong
-00027230: 2074 6f2e 2049 6e0a 2020 2020 6f75 7273   to. In.    ours
-00027240: 2063 6173 6520 7468 6973 2077 6f75 6c64   case this would
-00027250: 2062 650a 0a20 2020 203e 3e3e 2061 746f   be..    >>> ato
-00027260: 6d5f 7370 6c69 7420 3d20 6e70 2e61 7272  m_split = np.arr
-00027270: 6179 285b 302c 2030 2c20 302c 2031 5d29  ay([0, 0, 0, 1])
-00027280: 0a0a 2020 2020 4c65 7427 7320 6e6f 7720  ..    Let's now 
-00027290: 6465 6669 6e65 2074 6865 2061 6374 7561  define the actua
-000272a0: 6c20 6c61 7965 720a 0a20 2020 203e 3e3e  l layer..    >>>
-000272b0: 2067 6174 6865 7220 3d20 5765 6176 6547   gather = WeaveG
-000272c0: 6174 6865 7228 6261 7463 685f 7369 7a65  ather(batch_size
-000272d0: 3d32 2c20 6e5f 696e 7075 743d 6e5f 6174  =2, n_input=n_at
-000272e0: 6f6d 5f66 6561 7429 0a20 2020 203e 3e3e  om_feat).    >>>
-000272f0: 206f 7574 7075 745f 6d6f 6c65 6375 6c65   output_molecule
-00027300: 7320 3d20 6761 7468 6572 285b 6174 6f6d  s = gather([atom
-00027310: 5f66 6561 742c 2061 746f 6d5f 7370 6c69  _feat, atom_spli
-00027320: 745d 290a 2020 2020 3e3e 3e20 6c65 6e28  t]).    >>> len(
-00027330: 6f75 7470 7574 5f6d 6f6c 6563 756c 6573  output_molecules
-00027340: 290a 2020 2020 320a 0a20 2020 2052 6566  ).    2..    Ref
-00027350: 6572 656e 6365 730a 2020 2020 2d2d 2d2d  erences.    ----
-00027360: 2d2d 2d2d 2d2d 0a20 2020 202e 2e20 5b31  ------.    .. [1
-00027370: 5d20 4b65 6172 6e65 732c 2053 7465 7665  ] Kearnes, Steve
-00027380: 6e2c 2065 7420 616c 2e20 224d 6f6c 6563  n, et al. "Molec
-00027390: 756c 6172 2067 7261 7068 2063 6f6e 766f  ular graph convo
-000273a0: 6c75 7469 6f6e 733a 206d 6f76 696e 6720  lutions: moving 
-000273b0: 6265 796f 6e64 0a20 2020 2020 2020 2066  beyond.        f
-000273c0: 696e 6765 7270 7269 6e74 732e 2220 4a6f  ingerprints." Jo
-000273d0: 7572 6e61 6c20 6f66 2063 6f6d 7075 7465  urnal of compute
-000273e0: 722d 6169 6465 6420 6d6f 6c65 6375 6c61  r-aided molecula
-000273f0: 7220 6465 7369 676e 2033 302e 3820 2832  r design 30.8 (2
-00027400: 3031 3629 3a0a 2020 2020 2020 2020 3539  016):.        59
-00027410: 352d 3630 382e 0a20 2020 2022 2222 0a0a  5-608..    """..
-00027420: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00027430: 2873 656c 662c 0a20 2020 2020 2020 2020  (self,.         
-00027440: 2020 2020 2020 2020 6261 7463 685f 7369          batch_si
-00027450: 7a65 3a20 696e 742c 0a20 2020 2020 2020  ze: int,.       
-00027460: 2020 2020 2020 2020 2020 6e5f 696e 7075            n_inpu
-00027470: 743a 2069 6e74 203d 2031 3238 2c0a 2020  t: int = 128,.  
-00027480: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-00027490: 6175 7373 6961 6e5f 6578 7061 6e64 3a20  aussian_expand: 
-000274a0: 626f 6f6c 203d 2054 7275 652c 0a20 2020  bool = True,.   
-000274b0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-000274c0: 6d70 7265 7373 5f70 6f73 745f 6761 7573  mpress_post_gaus
-000274d0: 7369 616e 5f65 7870 616e 7369 6f6e 3a20  sian_expansion: 
-000274e0: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
-000274f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00027500: 6e69 745f 3a20 7374 7220 3d20 2778 6176  nit_: str = 'xav
-00027510: 6965 725f 756e 6966 6f72 6d5f 272c 0a20  ier_uniform_',. 
+0001fe30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fe40: 2020 6e6f 6465 733d 7365 6c66 2e6e 6f64    nodes=self.nod
+0001fe50: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+0001fe60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fe70: 2020 2020 2020 2061 6374 6976 6174 696f         activatio
+0001fe80: 6e3d 7365 6c66 2e61 6374 6976 6174 696f  n=self.activatio
+0001fe90: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
+0001fea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001feb0: 2020 2020 2020 6472 6f70 6f75 745f 7261        dropout_ra
+0001fec0: 7465 3d73 656c 662e 6472 6f70 6f75 745f  te=self.dropout_
+0001fed0: 7261 7465 2c0a 2020 2020 2020 2020 2020  rate,.          
+0001fee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fef0: 2020 2020 2020 2020 2065 6467 6573 3d73           edges=s
+0001ff00: 656c 662e 6564 6765 732c 0a20 2020 2020  elf.edges,.     
+0001ff10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ff20: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+0001ff30: 6576 5f73 6861 7065 3d73 656c 662e 756e  ev_shape=self.un
+0001ff40: 6974 735b 636f 756e 745d 290a 2020 2020  its[count]).    
+0001ff50: 2020 2020 2020 2020 666f 7220 636f 756e          for coun
+0001ff60: 742c 2075 2069 6e20 656e 756d 6572 6174  t, u in enumerat
+0001ff70: 6528 7365 6c66 2e75 6e69 7473 5b31 3a5d  e(self.units[1:]
+0001ff80: 290a 2020 2020 2020 2020 5d29 0a0a 2020  ).        ])..  
+0001ff90: 2020 6465 6620 5f5f 7265 7072 5f5f 2873    def __repr__(s
+0001ffa0: 656c 6629 202d 3e20 7374 723a 0a20 2020  elf) -> str:.   
+0001ffb0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0001ffc0: 2053 7472 696e 6720 7265 7072 6573 656e   String represen
+0001ffd0: 7461 7469 6f6e 206f 6620 7468 6520 6c61  tation of the la
+0001ffe0: 7965 720a 2020 2020 2020 2020 0a20 2020  yer.        .   
+0001fff0: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
+00020000: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
+00020010: 2020 2020 2073 7472 696e 670a 2020 2020       string.    
+00020020: 2020 2020 2020 2020 5374 7269 6e67 2072          String r
+00020030: 6570 7265 7365 6e74 6174 696f 6e20 6f66  epresentation of
+00020040: 2074 6865 206c 6179 6572 0a20 2020 2020   the layer.     
+00020050: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+00020060: 6574 7572 6e20 6622 7b73 656c 662e 5f5f  eturn f"{self.__
+00020070: 636c 6173 735f 5f2e 5f5f 6e61 6d65 5f5f  class__.__name__
+00020080: 7d28 756e 6974 733d 7b73 656c 662e 756e  }(units={self.un
+00020090: 6974 737d 2c20 6163 7469 7661 7469 6f6e  its}, activation
+000200a0: 3d7b 7365 6c66 2e61 6374 6976 6174 696f  ={self.activatio
+000200b0: 6e7d 2c20 6472 6f70 6f75 745f 7261 7465  n}, dropout_rate
+000200c0: 3d7b 7365 6c66 2e64 726f 706f 7574 5f72  ={self.dropout_r
+000200d0: 6174 657d 292c 2065 6467 6573 3d7b 7365  ate}), edges={se
+000200e0: 6c66 2e65 6467 6573 7d29 220a 0a20 2020  lf.edges})"..   
+000200f0: 2064 6566 2066 6f72 7761 7264 2873 656c   def forward(sel
+00020100: 662c 2069 6e70 7574 733a 204c 6973 7429  f, inputs: List)
+00020110: 202d 3e20 746f 7263 682e 5465 6e73 6f72   -> torch.Tensor
+00020120: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00020130: 2020 2020 2020 496e 766f 6b65 2074 6869        Invoke thi
+00020140: 7320 6c61 7965 720a 0a20 2020 2020 2020  s layer..       
+00020150: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00020160: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00020170: 2020 2020 2020 2069 6e70 7574 733a 206c         inputs: l
+00020180: 6973 740a 2020 2020 2020 2020 2020 2020  ist.            
+00020190: 4c69 7374 206f 6620 7477 6f20 696e 7075  List of two inpu
+000201a0: 7420 6d61 7472 6963 6573 2c20 6164 6a61  t matrices, adja
+000201b0: 6365 6e63 7920 7465 6e73 6f72 2061 6e64  cency tensor and
+000201c0: 206e 6f64 6520 6665 6174 7572 6573 2074   node features t
+000201d0: 656e 736f 7273 0a20 2020 2020 2020 2020  ensors.         
+000201e0: 2020 2069 6e20 6f6e 652d 686f 7420 656e     in one-hot en
+000201f0: 636f 6469 6e67 2066 6f72 6d61 742e 0a0a  coding format...
+00020200: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+00020210: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00020220: 0a20 2020 2020 2020 2063 6f6e 766f 6c75  .        convolu
+00020230: 7469 6f6e 2074 656e 736f 723a 2074 6f72  tion tensor: tor
+00020240: 6368 2e54 656e 736f 720a 2020 2020 2020  ch.Tensor.      
+00020250: 2020 2020 2020 5265 7375 6c74 206f 6620        Result of 
+00020260: 696e 7075 7420 7465 6e73 6f72 7320 676f  input tensors go
+00020270: 696e 6720 7468 726f 7567 6820 636f 6e76  ing through conv
+00020280: 6f6c 7574 696f 6e20 6120 6e75 6d62 6572  olution a number
+00020290: 206f 6620 7469 6d65 732e 0a20 2020 2020   of times..     
+000202a0: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+000202b0: 6164 6a61 6365 6e63 795f 7465 6e73 6f72  adjacency_tensor
+000202c0: 203d 2069 6e70 7574 735b 305d 0a20 2020   = inputs[0].   
+000202d0: 2020 2020 206e 6f64 655f 7465 6e73 6f72       node_tensor
+000202e0: 203d 2069 6e70 7574 735b 315d 0a0a 2020   = inputs[1]..  
+000202f0: 2020 2020 2020 7465 6e73 6f72 7320 3d20        tensors = 
+00020300: 7365 6c66 2e66 6972 7374 5f63 6f6e 766f  self.first_convo
+00020310: 6c75 7469 6f6e 285b 6164 6a61 6365 6e63  lution([adjacenc
+00020320: 795f 7465 6e73 6f72 2c20 6e6f 6465 5f74  y_tensor, node_t
+00020330: 656e 736f 725d 290a 0a20 2020 2020 2020  ensor])..       
+00020340: 2023 204c 6f6f 7020 6f76 6572 2074 6865   # Loop over the
+00020350: 2072 656d 6169 6e69 6e67 2063 6f6e 766f   remaining convo
+00020360: 6c75 7469 6f6e 206c 6179 6572 730a 2020  lution layers.  
+00020370: 2020 2020 2020 666f 7220 6c61 7965 7220        for layer 
+00020380: 696e 2073 656c 662e 6763 6c3a 0a20 2020  in self.gcl:.   
+00020390: 2020 2020 2020 2020 2023 2041 7070 6c79           # Apply
+000203a0: 2074 6865 2063 7572 7265 6e74 206c 6179   the current lay
+000203b0: 6572 2074 6f20 7468 6520 6f75 7470 7574  er to the output
+000203c0: 7320 6672 6f6d 2074 6865 2070 7265 7669  s from the previ
+000203d0: 6f75 7320 6c61 7965 720a 2020 2020 2020  ous layer.      
+000203e0: 2020 2020 2020 7465 6e73 6f72 7320 3d20        tensors = 
+000203f0: 6c61 7965 7228 7465 6e73 6f72 7329 0a0a  layer(tensors)..
+00020400: 2020 2020 2020 2020 5f2c 205f 2c20 6869          _, _, hi
+00020410: 6464 656e 5f74 656e 736f 7220 3d20 7465  dden_tensor = te
+00020420: 6e73 6f72 730a 0a20 2020 2020 2020 2072  nsors..        r
+00020430: 6574 7572 6e20 6869 6464 656e 5f74 656e  eturn hidden_ten
+00020440: 736f 720a 0a0a 636c 6173 7320 4d6f 6c47  sor...class MolG
+00020450: 414e 456e 636f 6465 724c 6179 6572 286e  ANEncoderLayer(n
+00020460: 6e2e 4d6f 6475 6c65 293a 0a20 2020 2022  n.Module):.    "
+00020470: 2222 0a20 2020 204d 6169 6e20 6c65 6172  "".    Main lear
+00020480: 6e69 6e67 206c 6179 6572 2075 7365 6420  ning layer used 
+00020490: 6279 204d 6f6c 4741 4e20 6d6f 6465 6c2e  by MolGAN model.
+000204a0: 0a20 2020 204d 6f6c 4741 4e20 6973 2061  .    MolGAN is a
+000204b0: 2057 4741 4e20 7479 7065 206d 6f64 656c   WGAN type model
+000204c0: 2066 6f72 2067 656e 6572 6174 696f 6e20   for generation 
+000204d0: 6f66 2073 6d61 6c6c 206d 6f6c 6563 756c  of small molecul
+000204e0: 6573 2e0a 2020 2020 4974 2072 6f6c 6520  es..    It role 
+000204f0: 6973 2074 6f20 6675 7274 6865 7220 7369  is to further si
+00020500: 6d70 6c69 6679 206d 6f64 656c 2e0a 2020  mplify model..  
+00020510: 2020 5468 6973 206c 6179 6572 2063 616e    This layer can
+00020520: 2062 6520 6d61 6e75 616c 6c79 2062 7569   be manually bui
+00020530: 6c74 2062 7920 7374 6163 6b69 6e67 2067  lt by stacking g
+00020540: 7261 7068 2063 6f6e 766f 6c75 7469 6f6e  raph convolution
+00020550: 206c 6179 6572 730a 2020 2020 666f 6c6c   layers.    foll
+00020560: 6f77 6564 2062 7920 6772 6170 6820 6167  owed by graph ag
+00020570: 6772 6567 6174 696f 6e2e 0a20 2020 200a  gregation..    .
+00020580: 2020 2020 4578 616d 706c 650a 2020 2020      Example.    
+00020590: 2d2d 2d2d 2d2d 2d0a 2020 2020 3e3e 3e20  -------.    >>> 
+000205a0: 696d 706f 7274 2074 6f72 6368 0a20 2020  import torch.   
+000205b0: 203e 3e3e 2069 6d70 6f72 7420 746f 7263   >>> import torc
+000205c0: 682e 6e6e 2061 7320 6e6e 0a20 2020 203e  h.nn as nn.    >
+000205d0: 3e3e 2069 6d70 6f72 7420 746f 7263 682e  >> import torch.
+000205e0: 6e6e 2e66 756e 6374 696f 6e61 6c20 6173  nn.functional as
+000205f0: 2046 0a20 2020 203e 3e3e 2076 6572 7469   F.    >>> verti
+00020600: 6365 7320 3d20 390a 2020 2020 3e3e 3e20  ces = 9.    >>> 
+00020610: 6e6f 6465 7320 3d20 350a 2020 2020 3e3e  nodes = 5.    >>
+00020620: 3e20 6564 6765 7320 3d20 350a 2020 2020  > edges = 5.    
+00020630: 3e3e 3e20 6472 6f70 6f75 745f 7261 7465  >>> dropout_rate
+00020640: 203d 2030 2e30 0a20 2020 203e 3e3e 2061   = 0.0.    >>> a
+00020650: 646a 6163 656e 6379 5f74 656e 736f 7220  djacency_tensor 
+00020660: 3d20 746f 7263 682e 7261 6e64 6e28 2831  = torch.randn((1
+00020670: 2c20 7665 7274 6963 6573 2c20 7665 7274  , vertices, vert
+00020680: 6963 6573 2c20 6564 6765 7329 290a 2020  ices, edges)).  
+00020690: 2020 3e3e 3e20 6e6f 6465 5f74 656e 736f    >>> node_tenso
+000206a0: 7220 3d20 746f 7263 682e 7261 6e64 6e28  r = torch.randn(
+000206b0: 2831 2c20 7665 7274 6963 6573 2c20 6e6f  (1, vertices, no
+000206c0: 6465 7329 290a 2020 2020 0a20 2020 203e  des)).    .    >
+000206d0: 3e3e 2067 7261 7068 203d 204d 6f6c 4741  >> graph = MolGA
+000206e0: 4e45 6e63 6f64 6572 4c61 7965 7228 756e  NEncoderLayer(un
+000206f0: 6974 7320 3d20 5b28 3132 382c 3634 292c  its = [(128,64),
+00020700: 3132 385d 2c20 6472 6f70 6f75 745f 7261  128], dropout_ra
+00020710: 7465 3d20 6472 6f70 6f75 745f 7261 7465  te= dropout_rate
+00020720: 2c20 6564 6765 733d 6564 6765 732c 206e  , edges=edges, n
+00020730: 6f64 6573 3d6e 6f64 6573 2928 5b61 646a  odes=nodes)([adj
+00020740: 6163 656e 6379 5f74 656e 736f 722c 6e6f  acency_tensor,no
+00020750: 6465 5f74 656e 736f 725d 290a 2020 2020  de_tensor]).    
+00020760: 3e3e 3e20 6465 6e73 6520 3d20 6e6e 2e4c  >>> dense = nn.L
+00020770: 696e 6561 7228 3132 382c 3132 3829 2867  inear(128,128)(g
+00020780: 7261 7068 290a 2020 2020 3e3e 3e20 6465  raph).    >>> de
+00020790: 6e73 6520 3d20 746f 7263 682e 7461 6e68  nse = torch.tanh
+000207a0: 2864 656e 7365 290a 2020 2020 3e3e 3e20  (dense).    >>> 
+000207b0: 6465 6e73 6520 3d20 6e6e 2e44 726f 706f  dense = nn.Dropo
+000207c0: 7574 2864 726f 706f 7574 5f72 6174 6529  ut(dropout_rate)
+000207d0: 2864 656e 7365 290a 2020 2020 3e3e 3e20  (dense).    >>> 
+000207e0: 6465 6e73 6520 3d20 6e6e 2e4c 696e 6561  dense = nn.Linea
+000207f0: 7228 3132 382c 3634 2928 6465 6e73 6529  r(128,64)(dense)
+00020800: 0a20 2020 203e 3e3e 2064 656e 7365 203d  .    >>> dense =
+00020810: 2074 6f72 6368 2e74 616e 6828 6465 6e73   torch.tanh(dens
+00020820: 6529 0a20 2020 203e 3e3e 2064 656e 7365  e).    >>> dense
+00020830: 203d 206e 6e2e 4472 6f70 6f75 7428 6472   = nn.Dropout(dr
+00020840: 6f70 6f75 745f 7261 7465 2928 6465 6e73  opout_rate)(dens
+00020850: 6529 0a20 2020 203e 3e3e 206f 7574 7075  e).    >>> outpu
+00020860: 7420 3d20 6e6e 2e4c 696e 6561 7228 3634  t = nn.Linear(64
+00020870: 2c31 2928 6465 6e73 6529 0a20 2020 200a  ,1)(dense).    .
+00020880: 2020 2020 5265 6665 7265 6e63 6573 0a20      References. 
+00020890: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+000208a0: 2020 2e2e 205b 315d 204e 6963 6f6c 6120    .. [1] Nicola 
+000208b0: 4465 2043 616f 2065 7420 616c 2e20 224d  De Cao et al. "M
+000208c0: 6f6c 4741 4e3a 2041 6e20 696d 706c 6963  olGAN: An implic
+000208d0: 6974 2067 656e 6572 6174 6976 6520 6d6f  it generative mo
+000208e0: 6465 6c0a 2020 2020 2020 2020 666f 7220  del.        for 
+000208f0: 736d 616c 6c20 6d6f 6c65 6375 6c61 7220  small molecular 
+00020900: 6772 6170 6873 222c 2068 7474 7073 3a2f  graphs", https:/
+00020910: 2f61 7278 6976 2e6f 7267 2f61 6273 2f31  /arxiv.org/abs/1
+00020920: 3830 352e 3131 3937 330a 2020 2020 2222  805.11973.    ""
+00020930: 220a 0a20 2020 2064 6566 205f 5f69 6e69  "..    def __ini
+00020940: 745f 5f28 7365 6c66 2c0a 2020 2020 2020  t__(self,.      
+00020950: 2020 2020 2020 2020 2020 2075 6e69 7473             units
+00020960: 3a20 4c69 7374 203d 205b 2831 3238 2c20  : List = [(128, 
+00020970: 3634 292c 2031 3238 5d2c 0a20 2020 2020  64), 128],.     
+00020980: 2020 2020 2020 2020 2020 2020 6163 7469              acti
+00020990: 7661 7469 6f6e 3a20 4361 6c6c 6162 6c65  vation: Callable
+000209a0: 203d 2074 6f72 6368 2e74 616e 682c 0a20   = torch.tanh,. 
+000209b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000209c0: 6472 6f70 6f75 745f 7261 7465 3a20 666c  dropout_rate: fl
+000209d0: 6f61 7420 3d20 302e 302c 0a20 2020 2020  oat = 0.0,.     
+000209e0: 2020 2020 2020 2020 2020 2020 6564 6765              edge
+000209f0: 733a 2069 6e74 203d 2035 2c0a 2020 2020  s: int = 5,.    
+00020a00: 2020 2020 2020 2020 2020 2020 206e 6f64               nod
+00020a10: 6573 3a20 696e 7420 3d20 352c 0a20 2020  es: int = 5,.   
+00020a20: 2020 2020 2020 2020 2020 2020 2020 6e61                na
+00020a30: 6d65 3a20 7374 7220 3d20 2222 293a 0a20  me: str = ""):. 
+00020a40: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00020a50: 2020 2049 6e69 7469 616c 697a 6520 7468     Initialize th
+00020a60: 6520 6c61 7965 720a 2020 2020 2020 2020  e layer.        
+00020a70: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00020a80: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+00020a90: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2075  ------.        u
+00020aa0: 6e69 7473 3a20 4c69 7374 2c20 6f70 7469  nits: List, opti
+00020ab0: 6f6e 616c 2028 6465 6661 756c 743d 5b28  onal (default=[(
+00020ac0: 3132 382c 3634 292c 3132 385d 290a 2020  128,64),128]).  
+00020ad0: 2020 2020 2020 2020 2020 4c69 7374 206f            List o
+00020ae0: 6620 6469 6d65 6e73 696f 6e73 2075 7365  f dimensions use
+00020af0: 6420 6279 2063 6f6e 7365 6375 7469 7665  d by consecutive
+00020b00: 2063 6f6e 766f 6c75 7469 6f6e 206c 6179   convolution lay
+00020b10: 6572 732e 0a20 2020 2020 2020 2020 2020  ers..           
+00020b20: 2054 6865 206d 6f72 6520 7661 6c75 6573   The more values
+00020b30: 2074 6865 206d 6f72 6520 636f 6e76 6f6c   the more convol
+00020b40: 7574 696f 6e20 6c61 7965 7273 2069 6e76  ution layers inv
+00020b50: 6f6b 6564 2e0a 2020 2020 2020 2020 6163  oked..        ac
+00020b60: 7469 7661 7469 6f6e 3a20 6675 6e63 7469  tivation: functi
+00020b70: 6f6e 2c20 6f70 7469 6f6e 616c 2028 6465  on, optional (de
+00020b80: 6661 756c 743d 5461 6e68 290a 2020 2020  fault=Tanh).    
+00020b90: 2020 2020 2020 2020 6163 7469 7661 7469          activati
+00020ba0: 6f6e 2066 756e 6374 696f 6e20 7573 6564  on function used
+00020bb0: 2061 6372 6f73 7320 6d6f 6465 6c2c 2064   across model, d
+00020bc0: 6566 6175 6c74 2069 7320 5461 6e68 0a20  efault is Tanh. 
+00020bd0: 2020 2020 2020 2064 726f 706f 7574 5f72         dropout_r
+00020be0: 6174 653a 2066 6c6f 6174 2c20 6f70 7469  ate: float, opti
+00020bf0: 6f6e 616c 2028 6465 6661 756c 743d 302e  onal (default=0.
+00020c00: 3029 0a20 2020 2020 2020 2020 2020 2055  0).            U
+00020c10: 7365 6420 6279 2064 726f 706f 7574 206c  sed by dropout l
+00020c20: 6179 6572 0a20 2020 2020 2020 2065 6467  ayer.        edg
+00020c30: 6573 3a20 696e 742c 206f 7074 696f 6e61  es: int, optiona
+00020c40: 6c20 2864 6566 6175 6c74 3d35 290a 2020  l (default=5).  
+00020c50: 2020 2020 2020 2020 2020 436f 6e74 726f            Contro
+00020c60: 6c73 2068 6f77 206d 616e 7920 6465 6e73  ls how many dens
+00020c70: 6520 6c61 7965 7273 2075 7365 2066 6f72  e layers use for
+00020c80: 2073 696e 676c 6520 636f 6e76 6f6c 7574   single convolut
+00020c90: 696f 6e20 756e 6974 2e0a 2020 2020 2020  ion unit..      
+00020ca0: 2020 2020 2020 5479 7069 6361 6c6c 7920        Typically 
+00020cb0: 6d61 7463 6865 7320 6e75 6d62 6572 206f  matches number o
+00020cc0: 6620 626f 6e64 2074 7970 6573 2075 7365  f bond types use
+00020cd0: 6420 696e 2074 6865 206d 6f6c 6563 756c  d in the molecul
+00020ce0: 652e 0a20 2020 2020 2020 206e 6f64 6573  e..        nodes
+00020cf0: 3a20 696e 742c 206f 7074 696f 6e61 6c20  : int, optional 
+00020d00: 2864 6566 6175 6c74 3d35 290a 2020 2020  (default=5).    
+00020d10: 2020 2020 2020 2020 4e75 6d62 6572 206f          Number o
+00020d20: 6620 6665 6174 7572 6573 2069 6e20 6e6f  f features in no
+00020d30: 6465 2074 656e 736f 720a 2020 2020 2020  de tensor.      
+00020d40: 2020 6e61 6d65 3a20 7374 7269 6e67 2c20    name: string, 
+00020d50: 6f70 7469 6f6e 616c 2028 6465 6661 756c  optional (defaul
+00020d60: 743d 2222 290a 2020 2020 2020 2020 2020  t="").          
+00020d70: 2020 4e61 6d65 206f 6620 7468 6520 6c61    Name of the la
+00020d80: 7965 720a 2020 2020 2020 2020 2222 220a  yer.        """.
+00020d90: 0a20 2020 2020 2020 2073 7570 6572 284d  .        super(M
+00020da0: 6f6c 4741 4e45 6e63 6f64 6572 4c61 7965  olGANEncoderLaye
+00020db0: 722c 2073 656c 6629 2e5f 5f69 6e69 745f  r, self).__init_
+00020dc0: 5f28 290a 2020 2020 2020 2020 6966 206c  _().        if l
+00020dd0: 656e 2875 6e69 7473 2920 213d 2032 3a0a  en(units) != 2:.
+00020de0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00020df0: 6520 5661 6c75 6545 7272 6f72 2822 756e  e ValueError("un
+00020e00: 6974 7320 7061 7261 6d65 7465 7220 6d75  its parameter mu
+00020e10: 7374 2063 6f6e 7461 696e 2074 776f 2076  st contain two v
+00020e20: 616c 7565 7322 290a 2020 2020 2020 2020  alues").        
+00020e30: 7365 6c66 2e67 7261 7068 5f63 6f6e 766f  self.graph_convo
+00020e40: 6c75 7469 6f6e 5f75 6e69 7473 2c20 7365  lution_units, se
+00020e50: 6c66 2e61 7578 696c 6961 7279 5f75 6e69  lf.auxiliary_uni
+00020e60: 7473 203d 2075 6e69 7473 0a20 2020 2020  ts = units.     
+00020e70: 2020 2073 656c 662e 6163 7469 7661 7469     self.activati
+00020e80: 6f6e 203d 2061 6374 6976 6174 696f 6e0a  on = activation.
+00020e90: 2020 2020 2020 2020 7365 6c66 2e64 726f          self.dro
+00020ea0: 706f 7574 5f72 6174 6520 3d20 6472 6f70  pout_rate = drop
+00020eb0: 6f75 745f 7261 7465 0a20 2020 2020 2020  out_rate.       
+00020ec0: 2073 656c 662e 6564 6765 7320 3d20 6564   self.edges = ed
+00020ed0: 6765 730a 0a20 2020 2020 2020 2073 656c  ges..        sel
+00020ee0: 662e 6d75 6c74 695f 6772 6170 685f 636f  f.multi_graph_co
+00020ef0: 6e76 6f6c 7574 696f 6e5f 6c61 7965 7220  nvolution_layer 
+00020f00: 3d20 4d6f 6c47 414e 4d75 6c74 6943 6f6e  = MolGANMultiCon
+00020f10: 766f 6c75 7469 6f6e 4c61 7965 7228 0a20  volutionLayer(. 
+00020f20: 2020 2020 2020 2020 2020 2075 6e69 7473             units
+00020f30: 3d73 656c 662e 6772 6170 685f 636f 6e76  =self.graph_conv
+00020f40: 6f6c 7574 696f 6e5f 756e 6974 732c 0a20  olution_units,. 
+00020f50: 2020 2020 2020 2020 2020 206e 6f64 6573             nodes
+00020f60: 3d6e 6f64 6573 2c0a 2020 2020 2020 2020  =nodes,.        
+00020f70: 2020 2020 6163 7469 7661 7469 6f6e 3d73      activation=s
+00020f80: 656c 662e 6163 7469 7661 7469 6f6e 2c0a  elf.activation,.
+00020f90: 2020 2020 2020 2020 2020 2020 6472 6f70              drop
+00020fa0: 6f75 745f 7261 7465 3d73 656c 662e 6472  out_rate=self.dr
+00020fb0: 6f70 6f75 745f 7261 7465 2c0a 2020 2020  opout_rate,.    
+00020fc0: 2020 2020 2020 2020 6564 6765 733d 7365          edges=se
+00020fd0: 6c66 2e65 6467 6573 290a 2020 2020 2020  lf.edges).      
+00020fe0: 2020 7365 6c66 2e67 7261 7068 5f61 6767    self.graph_agg
+00020ff0: 7265 6761 7469 6f6e 5f6c 6179 6572 203d  regation_layer =
+00021000: 204d 6f6c 4741 4e41 6767 7265 6761 7469   MolGANAggregati
+00021010: 6f6e 4c61 7965 7228 0a20 2020 2020 2020  onLayer(.       
+00021020: 2020 2020 2075 6e69 7473 3d73 656c 662e       units=self.
+00021030: 6175 7869 6c69 6172 795f 756e 6974 732c  auxiliary_units,
+00021040: 0a20 2020 2020 2020 2020 2020 2061 6374  .            act
+00021050: 6976 6174 696f 6e3d 7365 6c66 2e61 6374  ivation=self.act
+00021060: 6976 6174 696f 6e2c 0a20 2020 2020 2020  ivation,.       
+00021070: 2020 2020 2064 726f 706f 7574 5f72 6174       dropout_rat
+00021080: 653d 7365 6c66 2e64 726f 706f 7574 5f72  e=self.dropout_r
+00021090: 6174 652c 0a20 2020 2020 2020 2020 2020  ate,.           
+000210a0: 2070 7265 765f 7368 6170 653d 7365 6c66   prev_shape=self
+000210b0: 2e67 7261 7068 5f63 6f6e 766f 6c75 7469  .graph_convoluti
+000210c0: 6f6e 5f75 6e69 7473 5b2d 315d 202b 206e  on_units[-1] + n
+000210d0: 6f64 6573 290a 0a20 2020 2064 6566 205f  odes)..    def _
+000210e0: 5f72 6570 725f 5f28 7365 6c66 2920 2d3e  _repr__(self) ->
+000210f0: 2073 7472 3a0a 2020 2020 2020 2020 2222   str:.        ""
+00021100: 220a 2020 2020 2020 2020 5374 7269 6e67  ".        String
+00021110: 2072 6570 7265 7365 6e74 6174 696f 6e20   representation 
+00021120: 6f66 2074 6865 206c 6179 6572 0a20 2020  of the layer.   
+00021130: 2020 2020 200a 2020 2020 2020 2020 5265       .        Re
+00021140: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
+00021150: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7374  -----.        st
+00021160: 7269 6e67 0a20 2020 2020 2020 2020 2020  ring.           
+00021170: 2053 7472 696e 6720 7265 7072 6573 656e   String represen
+00021180: 7461 7469 6f6e 206f 6620 7468 6520 6c61  tation of the la
+00021190: 7965 720a 2020 2020 2020 2020 2222 220a  yer.        """.
+000211a0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+000211b0: 227b 7365 6c66 2e5f 5f63 6c61 7373 5f5f  "{self.__class__
+000211c0: 2e5f 5f6e 616d 655f 5f7d 2875 6e69 7473  .__name__}(units
+000211d0: 3d7b 7365 6c66 2e75 6e69 7473 7d2c 2061  ={self.units}, a
+000211e0: 6374 6976 6174 696f 6e3d 7b73 656c 662e  ctivation={self.
+000211f0: 6163 7469 7661 7469 6f6e 7d2c 2064 726f  activation}, dro
+00021200: 706f 7574 5f72 6174 653d 7b73 656c 662e  pout_rate={self.
+00021210: 6472 6f70 6f75 745f 7261 7465 7d29 2c20  dropout_rate}), 
+00021220: 6564 6765 733d 7b73 656c 662e 6564 6765  edges={self.edge
+00021230: 737d 2922 0a0a 2020 2020 6465 6620 666f  s})"..    def fo
+00021240: 7277 6172 6428 7365 6c66 2c20 696e 7075  rward(self, inpu
+00021250: 7473 3a20 4c69 7374 2920 2d3e 2074 6f72  ts: List) -> tor
+00021260: 6368 2e54 656e 736f 723a 0a20 2020 2020  ch.Tensor:.     
+00021270: 2020 2022 2222 0a20 2020 2020 2020 2049     """.        I
+00021280: 6e76 6f6b 6520 7468 6973 206c 6179 6572  nvoke this layer
+00021290: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+000212a0: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+000212b0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+000212c0: 696e 7075 7473 3a20 6c69 7374 0a20 2020  inputs: list.   
+000212d0: 2020 2020 2020 2020 204c 6973 7420 6f66           List of
+000212e0: 2074 776f 2069 6e70 7574 206d 6174 7269   two input matri
+000212f0: 6365 732c 2061 646a 6163 656e 6379 2074  ces, adjacency t
+00021300: 656e 736f 7220 616e 6420 6e6f 6465 2066  ensor and node f
+00021310: 6561 7475 7265 7320 7465 6e73 6f72 730a  eatures tensors.
+00021320: 2020 2020 2020 2020 2020 2020 696e 206f              in o
+00021330: 6e65 2d68 6f74 2065 6e63 6f64 696e 6720  ne-hot encoding 
+00021340: 666f 726d 6174 2e0a 0a20 2020 2020 2020  format...       
+00021350: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+00021360: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020   --------.      
+00021370: 2020 656e 636f 6465 7220 7465 6e73 6f72    encoder tensor
+00021380: 3a20 7466 2e54 656e 736f 720a 2020 2020  : tf.Tensor.    
+00021390: 2020 2020 2020 2020 5465 6e73 6f72 2074          Tensor t
+000213a0: 6861 7420 6265 656e 2074 6872 6f75 6768  hat been through
+000213b0: 206e 756d 6265 7220 6f66 2063 6f6e 766f   number of convo
+000213c0: 6c75 7469 6f6e 7320 666f 6c6c 6f77 6564  lutions followed
+000213d0: 0a20 2020 2020 2020 2020 2020 2062 7920  .            by 
+000213e0: 6167 6772 6567 6174 696f 6e2e 0a20 2020  aggregation..   
+000213f0: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+00021400: 2020 6f75 7470 7574 203d 2073 656c 662e    output = self.
+00021410: 6d75 6c74 695f 6772 6170 685f 636f 6e76  multi_graph_conv
+00021420: 6f6c 7574 696f 6e5f 6c61 7965 7228 696e  olution_layer(in
+00021430: 7075 7473 290a 0a20 2020 2020 2020 206e  puts)..        n
+00021440: 6f64 655f 7465 6e73 6f72 203d 2069 6e70  ode_tensor = inp
+00021450: 7574 735b 315d 0a0a 2020 2020 2020 2020  uts[1]..        
+00021460: 6966 206c 656e 2869 6e70 7574 7329 203e  if len(inputs) >
+00021470: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
+00021480: 6869 6464 656e 5f74 656e 736f 7220 3d20  hidden_tensor = 
+00021490: 696e 7075 7473 5b32 5d0a 2020 2020 2020  inputs[2].      
+000214a0: 2020 2020 2020 616e 6e6f 7461 7469 6f6e        annotation
+000214b0: 7320 3d20 746f 7263 682e 6361 7428 286f  s = torch.cat((o
+000214c0: 7574 7075 742c 2068 6964 6465 6e5f 7465  utput, hidden_te
+000214d0: 6e73 6f72 2c20 6e6f 6465 5f74 656e 736f  nsor, node_tenso
+000214e0: 7229 2c20 2d31 290a 2020 2020 2020 2020  r), -1).        
+000214f0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00021500: 2020 5f2c 206e 6f64 655f 7465 6e73 6f72    _, node_tensor
+00021510: 203d 2069 6e70 7574 730a 2020 2020 2020   = inputs.      
+00021520: 2020 2020 2020 616e 6e6f 7461 7469 6f6e        annotation
+00021530: 7320 3d20 746f 7263 682e 6361 7428 286f  s = torch.cat((o
+00021540: 7574 7075 742c 206e 6f64 655f 7465 6e73  utput, node_tens
+00021550: 6f72 292c 202d 3129 0a0a 2020 2020 2020  or), -1)..      
+00021560: 2020 6f75 7470 7574 203d 2073 656c 662e    output = self.
+00021570: 6772 6170 685f 6167 6772 6567 6174 696f  graph_aggregatio
+00021580: 6e5f 6c61 7965 7228 616e 6e6f 7461 7469  n_layer(annotati
+00021590: 6f6e 7329 0a20 2020 2020 2020 2072 6574  ons).        ret
+000215a0: 7572 6e20 6f75 7470 7574 0a0a 0a63 6c61  urn output...cla
+000215b0: 7373 2044 544e 4e53 7465 7028 6e6e 2e4d  ss DTNNStep(nn.M
+000215c0: 6f64 756c 6529 3a0a 2020 2020 2222 2244  odule):.    """D
+000215d0: 544e 4e53 7465 7020 4c61 7965 7220 666f  TNNStep Layer fo
+000215e0: 7220 4454 4e4e 206d 6f64 656c 2e0a 0a20  r DTNN model... 
+000215f0: 2020 2045 6e63 6f64 6573 2074 6865 2061     Encodes the a
+00021600: 746f 6d27 7320 696e 7465 7261 6374 696f  tom's interactio
+00021610: 6e20 7769 7468 206f 7468 6572 2061 746f  n with other ato
+00021620: 6d73 2061 6363 6f72 6469 6e67 2074 6f20  ms according to 
+00021630: 6469 7374 616e 6365 2072 656c 6174 696f  distance relatio
+00021640: 6e73 6869 7073 2e20 5b31 5d5f 0a0a 2020  nships. [1]_..  
+00021650: 2020 5468 6973 204c 6179 6572 2069 6d70    This Layer imp
+00021660: 6c65 6d65 6e74 7320 7468 6520 4571 2028  lements the Eq (
+00021670: 3729 2066 726f 6d20 4454 4e4e 2050 6170  7) from DTNN Pap
+00021680: 6572 2e20 5468 656e 2073 756d 7320 7468  er. Then sums th
+00021690: 656d 2075 7020 746f 2067 6574 2074 6865  em up to get the
+000216a0: 2066 696e 616c 206f 7574 7075 7420 7573   final output us
+000216b0: 696e 6720 4571 2028 3629 2066 726f 6d20  ing Eq (6) from 
+000216c0: 4454 4e4e 2050 6170 6572 2e0a 0a20 2020  DTNN Paper...   
+000216d0: 2045 7120 2837 293a 2056 5f69 6a20 3d20   Eq (7): V_ij = 
+000216e0: 7461 6e68 5b57 5f66 6320 2e20 2828 575f  tanh[W_fc . ((W_
+000216f0: 6366 202e 2043 5f6a 202b 2062 5f63 6629  cf . C_j + b_cf)
+00021700: 202a 2028 575f 6466 202e 2064 5f69 6a20   * (W_df . d_ij 
+00021710: 2b20 625f 6466 2929 5d0a 0a20 2020 2045  + b_df))]..    E
+00021720: 7120 2836 293a 2043 5f69 203d 2043 5f69  q (6): C_i = C_i
+00021730: 202b 2073 756d 2856 5f69 6a29 0a0a 2020   + sum(V_ij)..  
+00021740: 2020 4865 7265 203a 2027 2e27 3d4d 6174    Here : '.'=Mat
+00021750: 7269 7820 4d75 6c74 6970 6c69 6361 7469  rix Multiplicati
+00021760: 6f6e 202c 2027 2a27 3d4d 756c 7469 706c  on , '*'=Multipl
+00021770: 6963 6174 696f 6e0a 0a20 2020 2052 6566  ication..    Ref
+00021780: 6572 656e 6365 730a 2020 2020 2d2d 2d2d  erences.    ----
+00021790: 2d2d 2d2d 2d2d 0a20 2020 205b 315d 2053  ------.    [1] S
+000217a0: 6368 c3bc 7474 2c20 4b72 6973 746f 6620  ch..tt, Kristof 
+000217b0: 542e 2c20 6574 2061 6c2e 2022 5175 616e  T., et al. "Quan
+000217c0: 7475 6d2d 6368 656d 6963 616c 2069 6e73  tum-chemical ins
+000217d0: 6967 6874 7320 6672 6f6d 2064 6565 700a  ights from deep.
+000217e0: 2020 2020 2020 2020 7465 6e73 6f72 206e          tensor n
+000217f0: 6575 7261 6c20 6e65 7477 6f72 6b73 2e22  eural networks."
+00021800: 204e 6174 7572 6520 636f 6d6d 756e 6963   Nature communic
+00021810: 6174 696f 6e73 2038 2e31 2028 3230 3137  ations 8.1 (2017
+00021820: 293a 2031 2d38 2e0a 0a20 2020 2045 7861  ): 1-8...    Exa
+00021830: 6d70 6c65 730a 2020 2020 2d2d 2d2d 2d2d  mples.    ------
+00021840: 2d2d 0a20 2020 203e 3e3e 2066 726f 6d20  --.    >>> from 
+00021850: 6465 6570 6368 656d 2e6d 6f64 656c 732e  deepchem.models.
+00021860: 746f 7263 685f 6d6f 6465 6c73 2069 6d70  torch_models imp
+00021870: 6f72 7420 6c61 7965 7273 0a20 2020 203e  ort layers.    >
+00021880: 3e3e 2069 6d70 6f72 7420 746f 7263 680a  >> import torch.
+00021890: 2020 2020 3e3e 3e20 656d 6265 6464 696e      >>> embeddin
+000218a0: 675f 6c61 7965 7220 3d20 6c61 7965 7273  g_layer = layers
+000218b0: 2e44 544e 4e45 6d62 6564 6469 6e67 2834  .DTNNEmbedding(4
+000218c0: 2c20 3429 0a20 2020 203e 3e3e 2065 6d62  , 4).    >>> emb
+000218d0: 203d 2065 6d62 6564 6469 6e67 5f6c 6179   = embedding_lay
+000218e0: 6572 2874 6f72 6368 2e54 656e 736f 7228  er(torch.Tensor(
+000218f0: 5b30 2c31 2c32 2c33 5d29 2e74 6f28 746f  [0,1,2,3]).to(to
+00021900: 7263 682e 696e 7436 3429 290a 2020 2020  rch.int64)).    
+00021910: 3e3e 3e20 7374 6570 5f6c 6179 6572 203d  >>> step_layer =
+00021920: 206c 6179 6572 732e 4454 4e4e 5374 6570   layers.DTNNStep
+00021930: 2834 2c20 362c 2038 290a 2020 2020 3e3e  (4, 6, 8).    >>
+00021940: 3e20 6f75 7470 7574 5f74 6f72 6368 203d  > output_torch =
+00021950: 2073 7465 705f 6c61 7965 7228 5b0a 2020   step_layer([.  
+00021960: 2020 2e2e 2e20 2020 2020 746f 7263 682e    ...     torch.
+00021970: 5465 6e73 6f72 2865 6d62 292c 0a20 2020  Tensor(emb),.   
+00021980: 202e 2e2e 2020 2020 2074 6f72 6368 2e54   ...     torch.T
+00021990: 656e 736f 7228 5b30 2c20 312c 2032 2c20  ensor([0, 1, 2, 
+000219a0: 332c 2034 2c20 355d 292e 746f 2874 6f72  3, 4, 5]).to(tor
+000219b0: 6368 2e66 6c6f 6174 3332 292c 0a20 2020  ch.float32),.   
+000219c0: 202e 2e2e 2020 2020 2074 6f72 6368 2e54   ...     torch.T
+000219d0: 656e 736f 7228 5b31 5d29 2e74 6f28 746f  ensor([1]).to(to
+000219e0: 7263 682e 696e 7436 3429 2c0a 2020 2020  rch.int64),.    
+000219f0: 2e2e 2e20 2020 2020 746f 7263 682e 5465  ...     torch.Te
+00021a00: 6e73 6f72 285b 5b31 5d5d 292e 746f 2874  nsor([[1]]).to(t
+00021a10: 6f72 6368 2e69 6e74 3634 290a 2020 2020  orch.int64).    
+00021a20: 2e2e 2e20 5d29 0a20 2020 203e 3e3e 206f  ... ]).    >>> o
+00021a30: 7574 7075 745f 746f 7263 682e 7368 6170  utput_torch.shap
+00021a40: 650a 2020 2020 746f 7263 682e 5369 7a65  e.    torch.Size
+00021a50: 285b 322c 2034 2c20 345d 290a 0a20 2020  ([2, 4, 4])..   
+00021a60: 2022 2222 0a0a 2020 2020 6465 6620 5f5f   """..    def __
+00021a70: 696e 6974 5f5f 2873 656c 662c 0a20 2020  init__(self,.   
+00021a80: 2020 2020 2020 2020 2020 2020 2020 6e5f                n_
+00021a90: 656d 6265 6464 696e 673a 2069 6e74 203d  embedding: int =
+00021aa0: 2033 302c 0a20 2020 2020 2020 2020 2020   30,.           
+00021ab0: 2020 2020 2020 6e5f 6469 7374 616e 6365        n_distance
+00021ac0: 3a20 696e 7420 3d20 3130 302c 0a20 2020  : int = 100,.   
+00021ad0: 2020 2020 2020 2020 2020 2020 2020 6e5f                n_
+00021ae0: 6869 6464 656e 3a20 696e 7420 3d20 3630  hidden: int = 60
+00021af0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00021b00: 2020 2069 6e69 7469 616c 697a 6572 3a20     initializer: 
+00021b10: 7374 7220 3d20 2778 6176 6965 725f 756e  str = 'xavier_un
+00021b20: 6966 6f72 6d5f 272c 0a20 2020 2020 2020  iform_',.       
+00021b30: 2020 2020 2020 2020 2020 6163 7469 7661            activa
+00021b40: 7469 6f6e 3d27 7461 6e68 272c 0a20 2020  tion='tanh',.   
+00021b50: 2020 2020 2020 2020 2020 2020 2020 2a2a                **
+00021b60: 6b77 6172 6773 293a 0a20 2020 2020 2020  kwargs):.       
+00021b70: 2022 2222 0a20 2020 2020 2020 2050 6172   """.        Par
+00021b80: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+00021b90: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00021ba0: 2020 206e 5f65 6d62 6564 6469 6e67 3a20     n_embedding: 
+00021bb0: 696e 742c 206f 7074 696f 6e61 6c0a 2020  int, optional.  
+00021bc0: 2020 2020 2020 2020 2020 4e75 6d62 6572            Number
+00021bd0: 206f 6620 6665 6174 7572 6573 2066 6f72   of features for
+00021be0: 2065 6163 6820 6174 6f6d 0a20 2020 2020   each atom.     
+00021bf0: 2020 206e 5f64 6973 7461 6e63 653a 2069     n_distance: i
+00021c00: 6e74 2c20 6f70 7469 6f6e 616c 0a20 2020  nt, optional.   
+00021c10: 2020 2020 2020 2020 2067 7261 6e75 6c61           granula
+00021c20: 7269 7479 206f 6620 6469 7374 616e 6365  rity of distance
+00021c30: 206d 6174 7269 780a 2020 2020 2020 2020   matrix.        
+00021c40: 6e5f 6869 6464 656e 3a20 696e 742c 206f  n_hidden: int, o
+00021c50: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+00021c60: 2020 2020 4e75 6d62 6572 206f 6620 6e6f      Number of no
+00021c70: 6465 7320 696e 2068 6964 6465 6e20 6c61  des in hidden la
+00021c80: 7965 720a 2020 2020 2020 2020 696e 6974  yer.        init
+00021c90: 6961 6c69 7a65 723a 2073 7472 2c20 6f70  ializer: str, op
+00021ca0: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
+00021cb0: 2020 2057 6569 6768 7420 696e 6974 6961     Weight initia
+00021cc0: 6c69 7a61 7469 6f6e 2066 6f72 2066 696c  lization for fil
+00021cd0: 7465 7273 2e0a 2020 2020 2020 2020 2020  ters..          
+00021ce0: 2020 4f70 7469 6f6e 733a 207b 7861 7669    Options: {xavi
+00021cf0: 6572 5f75 6e69 666f 726d 5f2c 2078 6176  er_uniform_, xav
+00021d00: 6965 725f 6e6f 726d 616c 5f2c 206b 6169  ier_normal_, kai
+00021d10: 6d69 6e67 5f75 6e69 666f 726d 5f2c 206b  ming_uniform_, k
+00021d20: 6169 6d69 6e67 5f6e 6f72 6d61 6c5f 2c20  aiming_normal_, 
+00021d30: 7472 756e 635f 6e6f 726d 616c 5f7d 0a20  trunc_normal_}. 
+00021d40: 2020 2020 2020 2061 6374 6976 6174 696f         activatio
+00021d50: 6e3a 2073 7472 2c20 6f70 7469 6f6e 616c  n: str, optional
+00021d60: 0a20 2020 2020 2020 2020 2020 2041 6374  .            Act
+00021d70: 6976 6174 696f 6e20 6675 6e63 7469 6f6e  ivation function
+00021d80: 2061 7070 6c69 6564 0a0a 2020 2020 2020   applied..      
+00021d90: 2020 2222 220a 2020 2020 2020 2020 7375    """.        su
+00021da0: 7065 7228 4454 4e4e 5374 6570 2c20 7365  per(DTNNStep, se
+00021db0: 6c66 292e 5f5f 696e 6974 5f5f 282a 2a6b  lf).__init__(**k
+00021dc0: 7761 7267 7329 0a20 2020 2020 2020 2073  wargs).        s
+00021dd0: 656c 662e 6e5f 656d 6265 6464 696e 6720  elf.n_embedding 
+00021de0: 3d20 6e5f 656d 6265 6464 696e 670a 2020  = n_embedding.  
+00021df0: 2020 2020 2020 7365 6c66 2e6e 5f64 6973        self.n_dis
+00021e00: 7461 6e63 6520 3d20 6e5f 6469 7374 616e  tance = n_distan
+00021e10: 6365 0a20 2020 2020 2020 2073 656c 662e  ce.        self.
+00021e20: 6e5f 6869 6464 656e 203d 206e 5f68 6964  n_hidden = n_hid
+00021e30: 6465 6e0a 2020 2020 2020 2020 7365 6c66  den.        self
+00021e40: 2e69 6e69 7469 616c 697a 6572 203d 2069  .initializer = i
+00021e50: 6e69 7469 616c 697a 6572 2020 2320 5365  nitializer  # Se
+00021e60: 7420 7765 6967 6874 2069 6e69 7469 616c  t weight initial
+00021e70: 697a 6174 696f 6e0a 2020 2020 2020 2020  ization.        
+00021e80: 7365 6c66 2e61 6374 6976 6174 696f 6e20  self.activation 
+00021e90: 3d20 6163 7469 7661 7469 6f6e 2020 2320  = activation  # 
+00021ea0: 4765 7420 6163 7469 7661 7469 6f6e 730a  Get activations.
+00021eb0: 2020 2020 2020 2020 7365 6c66 2e61 6374          self.act
+00021ec0: 6976 6174 696f 6e5f 666e 203d 2067 6574  ivation_fn = get
+00021ed0: 5f61 6374 6976 6174 696f 6e28 7365 6c66  _activation(self
+00021ee0: 2e61 6374 6976 6174 696f 6e29 0a0a 2020  .activation)..  
+00021ef0: 2020 2020 2020 696e 6974 5f66 756e 633a        init_func:
+00021f00: 2043 616c 6c61 626c 6520 3d20 6765 7461   Callable = geta
+00021f10: 7474 7228 696e 6974 6961 6c69 7a65 7273  ttr(initializers
+00021f20: 2c20 7365 6c66 2e69 6e69 7469 616c 697a  , self.initializ
+00021f30: 6572 290a 0a20 2020 2020 2020 2073 656c  er)..        sel
+00021f40: 662e 575f 6366 203d 206e 6e2e 5061 7261  f.W_cf = nn.Para
+00021f50: 6d65 7465 7228 0a20 2020 2020 2020 2020  meter(.         
+00021f60: 2020 2069 6e69 745f 6675 6e63 2874 6f72     init_func(tor
+00021f70: 6368 2e65 6d70 7479 285b 7365 6c66 2e6e  ch.empty([self.n
+00021f80: 5f65 6d62 6564 6469 6e67 2c20 7365 6c66  _embedding, self
+00021f90: 2e6e 5f68 6964 6465 6e5d 2929 290a 2020  .n_hidden]))).  
+00021fa0: 2020 2020 2020 7365 6c66 2e57 5f64 6620        self.W_df 
+00021fb0: 3d20 6e6e 2e50 6172 616d 6574 6572 280a  = nn.Parameter(.
+00021fc0: 2020 2020 2020 2020 2020 2020 696e 6974              init
+00021fd0: 5f66 756e 6328 746f 7263 682e 656d 7074  _func(torch.empt
+00021fe0: 7928 5b73 656c 662e 6e5f 6469 7374 616e  y([self.n_distan
+00021ff0: 6365 2c20 7365 6c66 2e6e 5f68 6964 6465  ce, self.n_hidde
+00022000: 6e5d 2929 290a 2020 2020 2020 2020 7365  n]))).        se
+00022010: 6c66 2e57 5f66 6320 3d20 6e6e 2e50 6172  lf.W_fc = nn.Par
+00022020: 616d 6574 6572 280a 2020 2020 2020 2020  ameter(.        
+00022030: 2020 2020 696e 6974 5f66 756e 6328 746f      init_func(to
+00022040: 7263 682e 656d 7074 7928 5b73 656c 662e  rch.empty([self.
+00022050: 6e5f 6869 6464 656e 2c20 7365 6c66 2e6e  n_hidden, self.n
+00022060: 5f65 6d62 6564 6469 6e67 5d29 2929 0a20  _embedding]))). 
+00022070: 2020 2020 2020 2073 656c 662e 625f 6366         self.b_cf
+00022080: 203d 206e 6e2e 5061 7261 6d65 7465 7228   = nn.Parameter(
+00022090: 746f 7263 682e 7a65 726f 7328 7369 7a65  torch.zeros(size
+000220a0: 3d5b 0a20 2020 2020 2020 2020 2020 2073  =[.            s
+000220b0: 656c 662e 6e5f 6869 6464 656e 2c0a 2020  elf.n_hidden,.  
+000220c0: 2020 2020 2020 5d29 290a 2020 2020 2020        ])).      
+000220d0: 2020 7365 6c66 2e62 5f64 6620 3d20 6e6e    self.b_df = nn
+000220e0: 2e50 6172 616d 6574 6572 2874 6f72 6368  .Parameter(torch
+000220f0: 2e7a 6572 6f73 2873 697a 653d 5b0a 2020  .zeros(size=[.  
+00022100: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00022110: 5f68 6964 6465 6e2c 0a20 2020 2020 2020  _hidden,.       
+00022120: 205d 2929 0a0a 2020 2020 6465 6620 5f5f   ]))..    def __
+00022130: 7265 7072 5f5f 2873 656c 6629 3a0a 2020  repr__(self):.  
+00022140: 2020 2020 2020 2222 2252 6574 7572 6e73        """Returns
+00022150: 2061 2073 7472 696e 6720 7265 7072 6573   a string repres
+00022160: 656e 7469 6e67 2074 6865 2063 6f6e 6669  enting the confi
+00022170: 6775 7261 7469 6f6e 206f 6620 7468 6520  guration of the 
+00022180: 6c61 7965 722e 0a0a 2020 2020 2020 2020  layer...        
+00022190: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+000221a0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+000221b0: 6e5f 656d 6265 6464 696e 673a 2069 6e74  n_embedding: int
+000221c0: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+000221d0: 2020 2020 2020 204e 756d 6265 7220 6f66         Number of
+000221e0: 2066 6561 7475 7265 7320 666f 7220 6561   features for ea
+000221f0: 6368 2061 746f 6d0a 2020 2020 2020 2020  ch atom.        
+00022200: 6e5f 6469 7374 616e 6365 3a20 696e 742c  n_distance: int,
+00022210: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+00022220: 2020 2020 2020 6772 616e 756c 6172 6974        granularit
+00022230: 7920 6f66 2064 6973 7461 6e63 6520 6d61  y of distance ma
+00022240: 7472 6978 0a20 2020 2020 2020 206e 5f68  trix.        n_h
+00022250: 6964 6465 6e3a 2069 6e74 2c20 6f70 7469  idden: int, opti
+00022260: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
+00022270: 204e 756d 6265 7220 6f66 206e 6f64 6573   Number of nodes
+00022280: 2069 6e20 6869 6464 656e 206c 6179 6572   in hidden layer
+00022290: 0a20 2020 2020 2020 2069 6e69 7469 616c  .        initial
+000222a0: 697a 6572 3a20 7374 722c 206f 7074 696f  izer: str, optio
+000222b0: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
+000222c0: 5765 6967 6874 2069 6e69 7469 616c 697a  Weight initializ
+000222d0: 6174 696f 6e20 666f 7220 6669 6c74 6572  ation for filter
+000222e0: 732e 0a20 2020 2020 2020 2020 2020 204f  s..            O
+000222f0: 7074 696f 6e73 3a20 7b78 6176 6965 725f  ptions: {xavier_
+00022300: 756e 6966 6f72 6d5f 2c20 7861 7669 6572  uniform_, xavier
+00022310: 5f6e 6f72 6d61 6c5f 2c20 6b61 696d 696e  _normal_, kaimin
+00022320: 675f 756e 6966 6f72 6d5f 2c20 6b61 696d  g_uniform_, kaim
+00022330: 696e 675f 6e6f 726d 616c 5f2c 2074 7275  ing_normal_, tru
+00022340: 6e63 5f6e 6f72 6d61 6c5f 7d0a 2020 2020  nc_normal_}.    
+00022350: 2020 2020 6163 7469 7661 7469 6f6e 3a20      activation: 
+00022360: 7374 722c 206f 7074 696f 6e61 6c0a 2020  str, optional.  
+00022370: 2020 2020 2020 2020 2020 4163 7469 7661            Activa
+00022380: 7469 6f6e 2066 756e 6374 696f 6e20 6170  tion function ap
+00022390: 706c 6965 640a 0a20 2020 2020 2020 2022  plied..        "
+000223a0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+000223b0: 6e20 6627 7b73 656c 662e 5f5f 636c 6173  n f'{self.__clas
+000223c0: 735f 5f2e 5f5f 6e61 6d65 5f5f 7d28 6e5f  s__.__name__}(n_
+000223d0: 656d 6265 6464 696e 673d 7b73 656c 662e  embedding={self.
+000223e0: 6e5f 656d 6265 6464 696e 677d 2c20 6e5f  n_embedding}, n_
+000223f0: 6469 7374 616e 6365 3d7b 7365 6c66 2e6e  distance={self.n
+00022400: 5f64 6973 7461 6e63 657d 2c20 6e5f 6869  _distance}, n_hi
+00022410: 6464 656e 3d7b 7365 6c66 2e6e 5f68 6964  dden={self.n_hid
+00022420: 6465 6e7d 2c20 696e 6974 6961 6c69 7a65  den}, initialize
+00022430: 723d 7b73 656c 662e 696e 6974 6961 6c69  r={self.initiali
+00022440: 7a65 727d 2c20 6163 7469 7661 7469 6f6e  zer}, activation
+00022450: 3d7b 7365 6c66 2e61 6374 6976 6174 696f  ={self.activatio
+00022460: 6e7d 2927 0a0a 2020 2020 6465 6620 666f  n})'..    def fo
+00022470: 7277 6172 6428 7365 6c66 2c20 696e 7075  rward(self, inpu
+00022480: 7473 293a 0a20 2020 2020 2020 2022 2222  ts):.        """
+00022490: 4578 6563 7574 6573 2074 6865 2065 7175  Executes the equ
+000224a0: 6174 696f 6e73 2061 6e64 2052 6574 7572  ations and Retur
+000224b0: 6e73 2074 6865 2069 6e74 7261 6374 696f  ns the intractio
+000224c0: 6e20 7665 6374 6f72 206f 6620 7468 6520  n vector of the 
+000224d0: 6174 6f6d 2077 6974 6820 6f74 6865 7220  atom with other 
+000224e0: 6174 6f6d 732e 0a0a 2020 2020 2020 2020  atoms...        
+000224f0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+00022500: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00022510: 2020 2020 2020 696e 7075 7473 3a20 746f        inputs: to
+00022520: 7263 682e 5465 6e73 6f72 0a20 2020 2020  rch.Tensor.     
+00022530: 2020 2020 2020 204c 6973 7420 6f66 2054         List of T
+00022540: 656e 736f 7273 2068 6176 696e 6720 6174  ensors having at
+00022550: 6f6d 5f66 6561 7475 7265 732c 2064 6973  om_features, dis
+00022560: 7461 6e63 652c 2064 6973 7461 6e63 655f  tance, distance_
+00022570: 6d65 6d62 6572 7368 6970 5f69 2c20 6469  membership_i, di
+00022580: 7374 616e 6365 5f6d 656d 6265 7273 6869  stance_membershi
+00022590: 705f 6a2e 0a0a 2020 2020 2020 2020 5265  p_j...        Re
+000225a0: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
+000225b0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 696e  -----.        in
+000225c0: 7465 7261 6374 696f 6e5f 7665 6374 6f72  teraction_vector
+000225d0: 3a20 746f 7263 682e 5465 6e73 6f72 0a20  : torch.Tensor. 
+000225e0: 2020 2020 2020 2020 2020 2069 6e74 6572             inter
+000225f0: 6163 7469 6f6e 206f 6620 7468 6520 6174  action of the at
+00022600: 6f6d 2077 6974 6820 6f74 6865 7220 6174  om with other at
+00022610: 6f6d 7320 6261 7365 6420 6f6e 2064 6973  oms based on dis
+00022620: 7461 6e63 6520 616e 6420 6469 7374 616e  tance and distan
+00022630: 6365 5f6d 656d 6265 7273 6869 702e 0a0a  ce_membership...
+00022640: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00022650: 2020 2020 6174 6f6d 5f66 6561 7475 7265      atom_feature
+00022660: 7320 3d20 696e 7075 7473 5b30 5d0a 2020  s = inputs[0].  
+00022670: 2020 2020 2020 6469 7374 616e 6365 203d        distance =
+00022680: 2069 6e70 7574 735b 315d 0a20 2020 2020   inputs[1].     
+00022690: 2020 2064 6973 7461 6e63 655f 6d65 6d62     distance_memb
+000226a0: 6572 7368 6970 5f69 203d 2069 6e70 7574  ership_i = input
+000226b0: 735b 325d 0a20 2020 2020 2020 2064 6973  s[2].        dis
+000226c0: 7461 6e63 655f 6d65 6d62 6572 7368 6970  tance_membership
+000226d0: 5f6a 203d 2069 6e70 7574 735b 335d 0a20  _j = inputs[3]. 
+000226e0: 2020 2020 2020 2064 6973 7461 6e63 655f         distance_
+000226f0: 6869 6464 656e 203d 2074 6f72 6368 2e6d  hidden = torch.m
+00022700: 6174 6d75 6c28 6469 7374 616e 6365 2c20  atmul(distance, 
+00022710: 7365 6c66 2e57 5f64 6629 202b 2073 656c  self.W_df) + sel
+00022720: 662e 625f 6466 0a20 2020 2020 2020 2061  f.b_df.        a
+00022730: 746f 6d5f 6665 6174 7572 6573 5f68 6964  tom_features_hid
+00022740: 6465 6e20 3d20 746f 7263 682e 6d61 746d  den = torch.matm
+00022750: 756c 2861 746f 6d5f 6665 6174 7572 6573  ul(atom_features
+00022760: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00022770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022780: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00022790: 6c66 2e57 5f63 6629 202b 2073 656c 662e  lf.W_cf) + self.
+000227a0: 625f 6366 0a20 2020 2020 2020 206f 7574  b_cf.        out
+000227b0: 7075 7473 203d 2074 6f72 6368 2e6d 756c  puts = torch.mul
+000227c0: 280a 2020 2020 2020 2020 2020 2020 6469  (.            di
+000227d0: 7374 616e 6365 5f68 6964 6465 6e2c 0a20  stance_hidden,. 
+000227e0: 2020 2020 2020 2020 2020 2074 6f72 6368             torch
+000227f0: 2e65 6d62 6564 6469 6e67 2861 746f 6d5f  .embedding(atom_
+00022800: 6665 6174 7572 6573 5f68 6964 6465 6e2c  features_hidden,
+00022810: 2064 6973 7461 6e63 655f 6d65 6d62 6572   distance_member
+00022820: 7368 6970 5f6a 2929 0a0a 2020 2020 2020  ship_j))..      
+00022830: 2020 2320 666f 7220 6174 6f6d 2069 2069    # for atom i i
+00022840: 6e20 6120 6d6f 6c65 6375 6c65 206d 2c20  n a molecule m, 
+00022850: 7468 6973 2073 7465 7020 6d75 6c74 6970  this step multip
+00022860: 6c69 6573 2074 6f67 6574 6865 7220 6469  lies together di
+00022870: 7374 616e 6365 2069 6e66 6f20 6f66 2061  stance info of a
+00022880: 746f 6d20 7061 6972 2869 2c6a 290a 2020  tom pair(i,j).  
+00022890: 2020 2020 2020 2320 616e 6420 656d 6265        # and embe
+000228a0: 6464 696e 6773 206f 6620 6174 6f6d 206a  ddings of atom j
+000228b0: 2862 6f74 6820 676f 6e65 2074 6872 6f75  (both gone throu
+000228c0: 6768 2061 2068 6964 6465 6e20 6c61 7965  gh a hidden laye
+000228d0: 7229 0a20 2020 2020 2020 206f 7574 7075  r).        outpu
+000228e0: 7473 203d 2074 6f72 6368 2e6d 6174 6d75  ts = torch.matmu
+000228f0: 6c28 6f75 7470 7574 732c 2073 656c 662e  l(outputs, self.
+00022900: 575f 6663 290a 2020 2020 2020 2020 6f75  W_fc).        ou
+00022910: 7470 7574 7320 3d20 7365 6c66 2e61 6374  tputs = self.act
+00022920: 6976 6174 696f 6e5f 666e 286f 7574 7075  ivation_fn(outpu
+00022930: 7473 290a 0a20 2020 2020 2020 206f 7574  ts)..        out
+00022940: 7075 745f 6969 203d 2074 6f72 6368 2e6d  put_ii = torch.m
+00022950: 756c 2873 656c 662e 625f 6466 2c20 6174  ul(self.b_df, at
+00022960: 6f6d 5f66 6561 7475 7265 735f 6869 6464  om_features_hidd
+00022970: 656e 290a 2020 2020 2020 2020 6f75 7470  en).        outp
+00022980: 7574 5f69 6920 3d20 746f 7263 682e 6d61  ut_ii = torch.ma
+00022990: 746d 756c 286f 7574 7075 745f 6969 2c20  tmul(output_ii, 
+000229a0: 7365 6c66 2e57 5f66 6329 0a20 2020 2020  self.W_fc).     
+000229b0: 2020 206f 7574 7075 745f 6969 203d 2073     output_ii = s
+000229c0: 656c 662e 6163 7469 7661 7469 6f6e 5f66  elf.activation_f
+000229d0: 6e28 6f75 7470 7574 5f69 6929 0a0a 2020  n(output_ii)..  
+000229e0: 2020 2020 2020 2320 666f 7220 6174 6f6d        # for atom
+000229f0: 2069 2c20 7375 6d20 7468 6520 696e 666c   i, sum the infl
+00022a00: 7565 6e63 6520 6672 6f6d 2061 6c6c 206f  uence from all o
+00022a10: 7468 6572 2061 746f 6d20 6a20 696e 2074  ther atom j in t
+00022a20: 6865 206d 6f6c 6563 756c 650a 2020 2020  he molecule.    
+00022a30: 2020 2020 696e 7472 6163 7469 6f6e 5f76      intraction_v
+00022a40: 6563 746f 7220 3d20 7363 6174 7465 7228  ector = scatter(
+00022a50: 6f75 7470 7574 732c 2064 6973 7461 6e63  outputs, distanc
+00022a60: 655f 6d65 6d62 6572 7368 6970 5f69 2c0a  e_membership_i,.
+00022a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022a90: 2020 2020 6469 6d3d 3029 202d 206f 7574      dim=0) - out
+00022aa0: 7075 745f 6969 202b 2061 746f 6d5f 6665  put_ii + atom_fe
+00022ab0: 6174 7572 6573 0a20 2020 2020 2020 2072  atures.        r
+00022ac0: 6574 7572 6e20 696e 7472 6163 7469 6f6e  eturn intraction
+00022ad0: 5f76 6563 746f 720a 0a0a 636c 6173 7320  _vector...class 
+00022ae0: 4454 4e4e 4761 7468 6572 286e 6e2e 4d6f  DTNNGather(nn.Mo
+00022af0: 6475 6c65 293a 0a20 2020 2022 2222 4454  dule):.    """DT
+00022b00: 4e4e 4761 7468 6572 204c 6179 6572 2066  NNGather Layer f
+00022b10: 6f72 2044 544e 4e20 4d6f 6465 6c2e 0a0a  or DTNN Model...
+00022b20: 2020 2020 5072 6564 6963 7420 4d6f 6c65      Predict Mole
+00022b30: 6375 6c61 7220 456e 6572 6779 2075 7369  cular Energy usi
+00022b40: 6e67 2061 746f 6d5f 6665 6174 7572 6573  ng atom_features
+00022b50: 2061 6e64 2061 746f 6d5f 6d65 6d62 6572   and atom_member
+00022b60: 7368 6970 2e20 5b31 5d5f 0a0a 2020 2020  ship. [1]_..    
+00022b70: 5468 6973 204c 6179 6572 2067 6174 6865  This Layer gathe
+00022b80: 7273 2074 6865 2069 6e70 7574 7320 676f  rs the inputs go
+00022b90: 7420 6672 6f6d 2074 6865 2073 7465 7020  t from the step 
+00022ba0: 6c61 7965 7220 6163 636f 7264 696e 6720  layer according 
+00022bb0: 746f 2061 746f 6d5f 6d65 6d62 6572 7368  to atom_membersh
+00022bc0: 6970 2061 6e64 2063 616c 756c 6174 6573  ip and calulates
+00022bd0: 2074 6865 2074 6f74 616c 204d 6f6c 6563   the total Molec
+00022be0: 756c 6172 2045 6e65 7267 792e 0a0a 2020  ular Energy...  
+00022bf0: 2020 5265 6665 7265 6e63 6573 0a20 2020    References.   
+00022c00: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00022c10: 5b31 5d20 5363 68c3 bc74 742c 204b 7269  [1] Sch..tt, Kri
+00022c20: 7374 6f66 2054 2e2c 2065 7420 616c 2e20  stof T., et al. 
+00022c30: 2251 7561 6e74 756d 2d63 6865 6d69 6361  "Quantum-chemica
+00022c40: 6c20 696e 7369 6768 7473 2066 726f 6d20  l insights from 
+00022c50: 6465 6570 0a20 2020 2020 2020 2074 656e  deep.        ten
+00022c60: 736f 7220 6e65 7572 616c 206e 6574 776f  sor neural netwo
+00022c70: 726b 732e 2220 4e61 7475 7265 2063 6f6d  rks." Nature com
+00022c80: 6d75 6e69 6361 7469 6f6e 7320 382e 3120  munications 8.1 
+00022c90: 2832 3031 3729 3a20 312d 382e 0a0a 2020  (2017): 1-8...  
+00022ca0: 2020 4578 616d 706c 6573 0a20 2020 202d    Examples.    -
+00022cb0: 2d2d 2d2d 2d2d 2d0a 2020 2020 3e3e 3e20  -------.    >>> 
+00022cc0: 6672 6f6d 2064 6565 7063 6865 6d2e 6d6f  from deepchem.mo
+00022cd0: 6465 6c73 2e74 6f72 6368 5f6d 6f64 656c  dels.torch_model
+00022ce0: 7320 696d 706f 7274 206c 6179 6572 7320  s import layers 
+00022cf0: 6173 206c 6179 6572 735f 746f 7263 680a  as layers_torch.
+00022d00: 2020 2020 3e3e 3e20 696d 706f 7274 2074      >>> import t
+00022d10: 6f72 6368 0a20 2020 203e 3e3e 2067 6174  orch.    >>> gat
+00022d20: 6865 725f 6c61 7965 725f 746f 7263 6820  her_layer_torch 
+00022d30: 3d20 6c61 7965 7273 5f74 6f72 6368 2e44  = layers_torch.D
+00022d40: 544e 4e47 6174 6865 7228 332c 2033 2c20  TNNGather(3, 3, 
+00022d50: 5b31 305d 290a 2020 2020 3e3e 3e20 7265  [10]).    >>> re
+00022d60: 7375 6c74 203d 2067 6174 6865 725f 6c61  sult = gather_la
+00022d70: 7965 725f 746f 7263 6828 5b74 6f72 6368  yer_torch([torch
+00022d80: 2e54 656e 736f 7228 5b5b 332c 2032 2c20  .Tensor([[3, 2, 
+00022d90: 315d 5d29 2e74 6f28 746f 7263 682e 666c  1]]).to(torch.fl
+00022da0: 6f61 7433 3229 2c20 746f 7263 682e 5465  oat32), torch.Te
+00022db0: 6e73 6f72 285b 305d 292e 746f 2874 6f72  nsor([0]).to(tor
+00022dc0: 6368 2e69 6e74 3634 295d 290a 2020 2020  ch.int64)]).    
+00022dd0: 3e3e 3e20 7265 7375 6c74 2e73 6861 7065  >>> result.shape
+00022de0: 0a20 2020 2074 6f72 6368 2e53 697a 6528  .    torch.Size(
+00022df0: 5b31 2c20 335d 290a 0a20 2020 2022 2222  [1, 3])..    """
+00022e00: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+00022e10: 5f5f 2873 656c 662c 0a20 2020 2020 2020  __(self,.       
+00022e20: 2020 2020 2020 2020 2020 6e5f 656d 6265            n_embe
+00022e30: 6464 696e 673d 3330 2c0a 2020 2020 2020  dding=30,.      
+00022e40: 2020 2020 2020 2020 2020 206e 5f6f 7574             n_out
+00022e50: 7075 7473 3d31 3030 2c0a 2020 2020 2020  puts=100,.      
+00022e60: 2020 2020 2020 2020 2020 206c 6179 6572             layer
+00022e70: 5f73 697a 6573 3d5b 3130 305d 2c0a 2020  _sizes=[100],.  
+00022e80: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00022e90: 7574 7075 745f 6163 7469 7661 7469 6f6e  utput_activation
+00022ea0: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
+00022eb0: 2020 2020 2020 2020 696e 6974 6961 6c69          initiali
+00022ec0: 7a65 723d 2778 6176 6965 725f 756e 6966  zer='xavier_unif
+00022ed0: 6f72 6d5f 272c 0a20 2020 2020 2020 2020  orm_',.         
+00022ee0: 2020 2020 2020 2020 6163 7469 7661 7469          activati
+00022ef0: 6f6e 3d27 7461 6e68 272c 0a20 2020 2020  on='tanh',.     
+00022f00: 2020 2020 2020 2020 2020 2020 2a2a 6b77              **kw
+00022f10: 6172 6773 293a 0a20 2020 2020 2020 2022  args):.        "
+00022f20: 2222 0a20 2020 2020 2020 2050 6172 616d  "".        Param
+00022f30: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+00022f40: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+00022f50: 206e 5f65 6d62 6564 6469 6e67 3a20 696e   n_embedding: in
+00022f60: 742c 206f 7074 696f 6e61 6c0a 2020 2020  t, optional.    
+00022f70: 2020 2020 2020 2020 4e75 6d62 6572 206f          Number o
+00022f80: 6620 6665 6174 7572 6573 2066 6f72 2065  f features for e
+00022f90: 6163 6820 6174 6f6d 0a20 2020 2020 2020  ach atom.       
+00022fa0: 206e 5f6f 7574 7075 7473 3a20 696e 742c   n_outputs: int,
+00022fb0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+00022fc0: 2020 2020 2020 4e75 6d62 6572 206f 6620        Number of 
+00022fd0: 6665 6174 7572 6573 2066 6f72 2065 6163  features for eac
+00022fe0: 6820 6d6f 6c65 6375 6c65 286f 7574 7075  h molecule(outpu
+00022ff0: 7429 0a20 2020 2020 2020 206c 6179 6572  t).        layer
+00023000: 5f73 697a 6573 3a20 6c69 7374 206f 6620  _sizes: list of 
+00023010: 696e 742c 206f 7074 696f 6e61 6c28 6465  int, optional(de
+00023020: 6661 756c 743d 5b31 3030 305d 290a 2020  fault=[1000]).  
+00023030: 2020 2020 2020 2020 2020 5374 7275 6374            Struct
+00023040: 7572 6520 6f66 2068 6964 6465 6e20 6c61  ure of hidden la
+00023050: 7965 7228 7329 0a20 2020 2020 2020 2069  yer(s).        i
+00023060: 6e69 7469 616c 697a 6572 3a20 7374 722c  nitializer: str,
+00023070: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+00023080: 2020 2020 2020 5765 6967 6874 2069 6e69        Weight ini
+00023090: 7469 616c 697a 6174 696f 6e20 666f 7220  tialization for 
+000230a0: 6669 6c74 6572 732e 0a20 2020 2020 2020  filters..       
+000230b0: 2061 6374 6976 6174 696f 6e3a 2073 7472   activation: str
+000230c0: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+000230d0: 2020 2020 2020 2041 6374 6976 6174 696f         Activatio
+000230e0: 6e20 6675 6e63 7469 6f6e 2061 7070 6c69  n function appli
+000230f0: 6564 0a0a 2020 2020 2020 2020 2222 220a  ed..        """.
+00023100: 0a20 2020 2020 2020 2073 7570 6572 2844  .        super(D
+00023110: 544e 4e47 6174 6865 722c 2073 656c 6629  TNNGather, self)
+00023120: 2e5f 5f69 6e69 745f 5f28 2a2a 6b77 6172  .__init__(**kwar
+00023130: 6773 290a 2020 2020 2020 2020 7365 6c66  gs).        self
+00023140: 2e6e 5f65 6d62 6564 6469 6e67 203d 206e  .n_embedding = n
+00023150: 5f65 6d62 6564 6469 6e67 0a20 2020 2020  _embedding.     
+00023160: 2020 2073 656c 662e 6e5f 6f75 7470 7574     self.n_output
+00023170: 7320 3d20 6e5f 6f75 7470 7574 730a 2020  s = n_outputs.  
+00023180: 2020 2020 2020 7365 6c66 2e6c 6179 6572        self.layer
+00023190: 5f73 697a 6573 203d 206c 6179 6572 5f73  _sizes = layer_s
+000231a0: 697a 6573 0a20 2020 2020 2020 2073 656c  izes.        sel
+000231b0: 662e 6f75 7470 7574 5f61 6374 6976 6174  f.output_activat
+000231c0: 696f 6e20 3d20 6f75 7470 7574 5f61 6374  ion = output_act
+000231d0: 6976 6174 696f 6e0a 2020 2020 2020 2020  ivation.        
+000231e0: 7365 6c66 2e69 6e69 7469 616c 697a 6572  self.initializer
+000231f0: 203d 2069 6e69 7469 616c 697a 6572 2020   = initializer  
+00023200: 2320 5365 7420 7765 6967 6874 2069 6e69  # Set weight ini
+00023210: 7469 616c 697a 6174 696f 6e0a 2020 2020  tialization.    
+00023220: 2020 2020 7365 6c66 2e61 6374 6976 6174      self.activat
+00023230: 696f 6e20 3d20 6163 7469 7661 7469 6f6e  ion = activation
+00023240: 2020 2320 4765 7420 6163 7469 7661 7469    # Get activati
+00023250: 6f6e 730a 2020 2020 2020 2020 7365 6c66  ons.        self
+00023260: 2e61 6374 6976 6174 696f 6e5f 666e 203d  .activation_fn =
+00023270: 2067 6574 5f61 6374 6976 6174 696f 6e28   get_activation(
+00023280: 7365 6c66 2e61 6374 6976 6174 696f 6e29  self.activation)
+00023290: 0a0a 2020 2020 2020 2020 7365 6c66 2e57  ..        self.W
+000232a0: 5f6c 6973 7420 3d20 6e6e 2e50 6172 616d  _list = nn.Param
+000232b0: 6574 6572 4c69 7374 2829 0a20 2020 2020  eterList().     
+000232c0: 2020 2073 656c 662e 625f 6c69 7374 203d     self.b_list =
+000232d0: 206e 6e2e 5061 7261 6d65 7465 724c 6973   nn.ParameterLis
+000232e0: 7428 290a 0a20 2020 2020 2020 2069 6e69  t()..        ini
+000232f0: 745f 6675 6e63 3a20 4361 6c6c 6162 6c65  t_func: Callable
+00023300: 203d 2067 6574 6174 7472 2869 6e69 7469   = getattr(initi
+00023310: 616c 697a 6572 732c 2073 656c 662e 696e  alizers, self.in
+00023320: 6974 6961 6c69 7a65 7229 0a0a 2020 2020  itializer)..    
+00023330: 2020 2020 7072 6576 5f6c 6179 6572 5f73      prev_layer_s
+00023340: 697a 6520 3d20 7365 6c66 2e6e 5f65 6d62  ize = self.n_emb
+00023350: 6564 6469 6e67 0a20 2020 2020 2020 2066  edding.        f
+00023360: 6f72 2069 2c20 6c61 7965 725f 7369 7a65  or i, layer_size
+00023370: 2069 6e20 656e 756d 6572 6174 6528 7365   in enumerate(se
+00023380: 6c66 2e6c 6179 6572 5f73 697a 6573 293a  lf.layer_sizes):
+00023390: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000233a0: 662e 575f 6c69 7374 2e61 7070 656e 6428  f.W_list.append(
+000233b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000233c0: 206e 6e2e 5061 7261 6d65 7465 7228 0a20   nn.Parameter(. 
+000233d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000233e0: 2020 2069 6e69 745f 6675 6e63 2874 6f72     init_func(tor
+000233f0: 6368 2e65 6d70 7479 285b 7072 6576 5f6c  ch.empty([prev_l
+00023400: 6179 6572 5f73 697a 652c 206c 6179 6572  ayer_size, layer
+00023410: 5f73 697a 655d 2929 2929 0a20 2020 2020  _size])))).     
+00023420: 2020 2020 2020 2073 656c 662e 625f 6c69         self.b_li
+00023430: 7374 2e61 7070 656e 6428 6e6e 2e50 6172  st.append(nn.Par
+00023440: 616d 6574 6572 2874 6f72 6368 2e7a 6572  ameter(torch.zer
+00023450: 6f73 2873 697a 653d 5b0a 2020 2020 2020  os(size=[.      
+00023460: 2020 2020 2020 2020 2020 6c61 7965 725f            layer_
+00023470: 7369 7a65 2c0a 2020 2020 2020 2020 2020  size,.          
+00023480: 2020 5d29 2929 0a20 2020 2020 2020 2020    ]))).         
+00023490: 2020 2070 7265 765f 6c61 7965 725f 7369     prev_layer_si
+000234a0: 7a65 203d 206c 6179 6572 5f73 697a 650a  ze = layer_size.
+000234b0: 2020 2020 2020 2020 7365 6c66 2e57 5f6c          self.W_l
+000234c0: 6973 742e 6170 7065 6e64 280a 2020 2020  ist.append(.    
+000234d0: 2020 2020 2020 2020 6e6e 2e50 6172 616d          nn.Param
+000234e0: 6574 6572 280a 2020 2020 2020 2020 2020  eter(.          
+000234f0: 2020 2020 2020 696e 6974 5f66 756e 6328        init_func(
+00023500: 746f 7263 682e 656d 7074 7928 5b70 7265  torch.empty([pre
+00023510: 765f 6c61 7965 725f 7369 7a65 2c20 7365  v_layer_size, se
+00023520: 6c66 2e6e 5f6f 7574 7075 7473 5d29 2929  lf.n_outputs])))
+00023530: 290a 2020 2020 2020 2020 7365 6c66 2e62  ).        self.b
+00023540: 5f6c 6973 742e 6170 7065 6e64 286e 6e2e  _list.append(nn.
+00023550: 5061 7261 6d65 7465 7228 746f 7263 682e  Parameter(torch.
+00023560: 7a65 726f 7328 7369 7a65 3d5b 0a20 2020  zeros(size=[.   
+00023570: 2020 2020 2020 2020 2073 656c 662e 6e5f           self.n_
+00023580: 6f75 7470 7574 732c 0a20 2020 2020 2020  outputs,.       
+00023590: 205d 2929 290a 0a20 2020 2064 6566 205f   ])))..    def _
+000235a0: 5f72 6570 725f 5f28 7365 6c66 293a 0a20  _repr__(self):. 
+000235b0: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
+000235c0: 7320 6120 7374 7269 6e67 2072 6570 7265  s a string repre
+000235d0: 7365 6e74 696e 6720 7468 6520 636f 6e66  senting the conf
+000235e0: 6967 7572 6174 696f 6e20 6f66 2074 6865  iguration of the
+000235f0: 206c 6179 6572 2e0a 0a20 2020 2020 2020   layer...       
+00023600: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+00023610: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00023620: 2020 2020 6e5f 656d 6265 6464 696e 673a      n_embedding:
+00023630: 2069 6e74 2c20 6f70 7469 6f6e 616c 0a20   int, optional. 
+00023640: 2020 2020 2020 2020 2020 204e 756d 6265             Numbe
+00023650: 7220 6f66 2066 6561 7475 7265 7320 666f  r of features fo
+00023660: 7220 6561 6368 2061 746f 6d0a 2020 2020  r each atom.    
+00023670: 2020 2020 6e5f 6f75 7470 7574 733a 2069      n_outputs: i
+00023680: 6e74 2c20 6f70 7469 6f6e 616c 0a20 2020  nt, optional.   
+00023690: 2020 2020 2020 2020 204e 756d 6265 7220           Number 
+000236a0: 6f66 2066 6561 7475 7265 7320 666f 7220  of features for 
+000236b0: 6561 6368 206d 6f6c 6563 756c 6528 6f75  each molecule(ou
+000236c0: 7470 7574 290a 2020 2020 2020 2020 6c61  tput).        la
+000236d0: 7965 725f 7369 7a65 733a 206c 6973 7420  yer_sizes: list 
+000236e0: 6f66 2069 6e74 2c20 6f70 7469 6f6e 616c  of int, optional
+000236f0: 2864 6566 6175 6c74 3d5b 3130 3030 5d29  (default=[1000])
+00023700: 0a20 2020 2020 2020 2020 2020 2053 7472  .            Str
+00023710: 7563 7475 7265 206f 6620 6869 6464 656e  ucture of hidden
+00023720: 206c 6179 6572 2873 290a 2020 2020 2020   layer(s).      
+00023730: 2020 696e 6974 6961 6c69 7a65 723a 2073    initializer: s
+00023740: 7472 2c20 6f70 7469 6f6e 616c 0a20 2020  tr, optional.   
+00023750: 2020 2020 2020 2020 2057 6569 6768 7420           Weight 
+00023760: 696e 6974 6961 6c69 7a61 7469 6f6e 2066  initialization f
+00023770: 6f72 2066 696c 7465 7273 2e0a 2020 2020  or filters..    
+00023780: 2020 2020 6163 7469 7661 7469 6f6e 3a20      activation: 
+00023790: 7374 722c 206f 7074 696f 6e61 6c0a 2020  str, optional.  
+000237a0: 2020 2020 2020 2020 2020 4163 7469 7661            Activa
+000237b0: 7469 6f6e 2066 756e 6374 696f 6e20 6170  tion function ap
+000237c0: 706c 6965 640a 0a20 2020 2020 2020 2022  plied..        "
+000237d0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+000237e0: 6e20 6627 7b73 656c 662e 5f5f 636c 6173  n f'{self.__clas
+000237f0: 735f 5f2e 5f5f 6e61 6d65 5f5f 7d28 6e5f  s__.__name__}(n_
+00023800: 656d 6265 6464 696e 673d 7b73 656c 662e  embedding={self.
+00023810: 6e5f 656d 6265 6464 696e 677d 2c20 6e5f  n_embedding}, n_
+00023820: 6f75 7470 7574 733d 7b73 656c 662e 6e5f  outputs={self.n_
+00023830: 6f75 7470 7574 737d 2c20 6c61 7965 725f  outputs}, layer_
+00023840: 7369 7a65 733d 7b73 656c 662e 6c61 7965  sizes={self.laye
+00023850: 725f 7369 7a65 737d 2c20 6f75 7470 7574  r_sizes}, output
+00023860: 5f61 6374 6976 6174 696f 6e3d 7b73 656c  _activation={sel
+00023870: 662e 6f75 7470 7574 5f61 6374 6976 6174  f.output_activat
+00023880: 696f 6e7d 2c20 696e 6974 6961 6c69 7a65  ion}, initialize
+00023890: 723d 7b73 656c 662e 696e 6974 6961 6c69  r={self.initiali
+000238a0: 7a65 727d 2c20 6163 7469 7661 7469 6f6e  zer}, activation
+000238b0: 3d7b 7365 6c66 2e61 6374 6976 6174 696f  ={self.activatio
+000238c0: 6e7d 2927 0a0a 2020 2020 6465 6620 666f  n})'..    def fo
+000238d0: 7277 6172 6428 7365 6c66 2c20 696e 7075  rward(self, inpu
+000238e0: 7473 293a 0a20 2020 2020 2020 2022 2222  ts):.        """
+000238f0: 4578 6563 7574 6573 2074 6865 2065 7175  Executes the equ
+00023900: 6174 696f 6e20 616e 6420 5265 7475 726e  ation and Return
+00023910: 7320 4d6f 6c65 6375 6c61 7220 456e 6572  s Molecular Ener
+00023920: 6769 6573 2061 6363 6f72 6469 6e67 2074  gies according t
+00023930: 6f20 6174 6f6d 5f6d 656d 6265 7273 6869  o atom_membershi
+00023940: 702e 0a0a 2020 2020 2020 2020 5061 7261  p...        Para
+00023950: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
+00023960: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+00023970: 2020 696e 7075 7473 3a20 746f 7263 682e    inputs: torch.
+00023980: 5465 6e73 6f72 0a20 2020 2020 2020 2020  Tensor.         
+00023990: 2020 204c 6973 7420 6f66 2054 656e 736f     List of Tenso
+000239a0: 7220 636f 6e74 6169 6e69 6e67 2061 746f  r containing ato
+000239b0: 6d5f 6665 6174 7572 6573 2061 6e64 2061  m_features and a
+000239c0: 746f 6d5f 6d65 6d62 6572 7368 6970 0a0a  tom_membership..
+000239d0: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+000239e0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+000239f0: 2020 2020 2020 2020 6d6f 6c65 6375 6c61          molecula
+00023a00: 725f 656e 6572 6769 6573 3a20 746f 7263  r_energies: torc
+00023a10: 682e 5465 6e73 6f72 0a20 2020 2020 2020  h.Tensor.       
+00023a20: 2020 2020 2054 656e 736f 7220 636f 6e74       Tensor cont
+00023a30: 6169 6e69 6e67 2074 6865 204d 6f6c 6563  aining the Molec
+00023a40: 756c 6172 2045 6e65 7267 6965 7320 6163  ular Energies ac
+00023a50: 636f 7264 696e 6720 746f 2061 746f 6d5f  cording to atom_
+00023a60: 6d65 6d62 6572 7368 6970 2e0a 0a20 2020  membership...   
+00023a70: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00023a80: 206f 7574 7075 7420 3d20 696e 7075 7473   output = inputs
+00023a90: 5b30 5d0a 2020 2020 2020 2020 6174 6f6d  [0].        atom
+00023aa0: 5f6d 656d 6265 7273 6869 7020 3d20 696e  _membership = in
+00023ab0: 7075 7473 5b31 5d0a 0a20 2020 2020 2020  puts[1]..       
+00023ac0: 2066 6f72 2069 2c20 5720 696e 2065 6e75   for i, W in enu
+00023ad0: 6d65 7261 7465 2873 656c 662e 575f 6c69  merate(self.W_li
+00023ae0: 7374 5b3a 2d31 5d29 3a0a 2020 2020 2020  st[:-1]):.      
+00023af0: 2020 2020 2020 6f75 7470 7574 203d 2074        output = t
+00023b00: 6f72 6368 2e6d 6174 6d75 6c28 6f75 7470  orch.matmul(outp
+00023b10: 7574 2c20 5729 202b 2073 656c 662e 625f  ut, W) + self.b_
+00023b20: 6c69 7374 5b69 5d0a 2020 2020 2020 2020  list[i].        
+00023b30: 2020 2020 6f75 7470 7574 203d 2073 656c      output = sel
+00023b40: 662e 6163 7469 7661 7469 6f6e 5f66 6e28  f.activation_fn(
+00023b50: 6f75 7470 7574 290a 2020 2020 2020 2020  output).        
+00023b60: 6f75 7470 7574 203d 2074 6f72 6368 2e6d  output = torch.m
+00023b70: 6174 6d75 6c28 6f75 7470 7574 2c20 7365  atmul(output, se
+00023b80: 6c66 2e57 5f6c 6973 745b 2d31 5d29 202b  lf.W_list[-1]) +
+00023b90: 2073 656c 662e 625f 6c69 7374 5b2d 315d   self.b_list[-1]
+00023ba0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00023bb0: 2e6f 7574 7075 745f 6163 7469 7661 7469  .output_activati
+00023bc0: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
+00023bd0: 6f75 7470 7574 203d 2073 656c 662e 6163  output = self.ac
+00023be0: 7469 7661 7469 6f6e 5f66 6e28 6f75 7470  tivation_fn(outp
+00023bf0: 7574 290a 2020 2020 2020 2020 7265 7475  ut).        retu
+00023c00: 726e 2073 6361 7474 6572 286f 7574 7075  rn scatter(outpu
+00023c10: 742c 2061 746f 6d5f 6d65 6d62 6572 7368  t, atom_membersh
+00023c20: 6970 290a 0a0a 636c 6173 7320 4564 6765  ip)...class Edge
+00023c30: 4e65 7477 6f72 6b28 6e6e 2e4d 6f64 756c  Network(nn.Modul
+00023c40: 6529 3a0a 2020 2020 2222 2254 6865 2045  e):.    """The E
+00023c50: 6467 654e 6574 776f 726b 206d 6f64 756c  dgeNetwork modul
+00023c60: 6520 6973 2061 2050 7954 6f72 6368 2073  e is a PyTorch s
+00023c70: 7562 6d6f 6475 6c65 2064 6573 6967 6e65  ubmodule designe
+00023c80: 6420 666f 7220 6d65 7373 6167 6520 7061  d for message pa
+00023c90: 7373 696e 6720 696e 2067 7261 7068 206e  ssing in graph n
+00023ca0: 6575 7261 6c20 6e65 7477 6f72 6b73 2e0a  eural networks..
+00023cb0: 0a20 2020 2045 7861 6d70 6c65 730a 2020  .    Examples.  
+00023cc0: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 203e    --------.    >
+00023cd0: 3e3e 2070 6169 725f 6665 6174 7572 6573  >> pair_features
+00023ce0: 203d 2074 6f72 6368 2e72 616e 6428 2834   = torch.rand((4
+00023cf0: 2c20 3229 2c20 6474 7970 653d 746f 7263  , 2), dtype=torc
+00023d00: 682e 666c 6f61 7433 3229 0a20 2020 203e  h.float32).    >
+00023d10: 3e3e 2061 746f 6d5f 6665 6174 7572 6573  >> atom_features
+00023d20: 203d 2074 6f72 6368 2e72 616e 6428 2835   = torch.rand((5
+00023d30: 2c20 3229 2c20 6474 7970 653d 746f 7263  , 2), dtype=torc
+00023d40: 682e 666c 6f61 7433 3229 0a20 2020 203e  h.float32).    >
+00023d50: 3e3e 2061 746f 6d5f 746f 5f70 6169 7220  >> atom_to_pair 
+00023d60: 3d20 5b5d 0a20 2020 203e 3e3e 206e 5f61  = [].    >>> n_a
+00023d70: 746f 6d73 203d 2032 0a20 2020 203e 3e3e  toms = 2.    >>>
+00023d80: 2073 7461 7274 203d 2030 0a20 2020 203e   start = 0.    >
+00023d90: 3e3e 2043 302c 2043 3120 3d20 6e70 2e6d  >> C0, C1 = np.m
+00023da0: 6573 6867 7269 6428 6e70 2e61 7261 6e67  eshgrid(np.arang
+00023db0: 6528 6e5f 6174 6f6d 7329 2c20 6e70 2e61  e(n_atoms), np.a
+00023dc0: 7261 6e67 6528 6e5f 6174 6f6d 7329 290a  range(n_atoms)).
+00023dd0: 2020 2020 3e3e 3e20 6174 6f6d 5f74 6f5f      >>> atom_to_
+00023de0: 7061 6972 2e61 7070 656e 6428 6e70 2e74  pair.append(np.t
+00023df0: 7261 6e73 706f 7365 286e 702e 6172 7261  ranspose(np.arra
+00023e00: 7928 5b43 312e 666c 6174 7465 6e28 2920  y([C1.flatten() 
+00023e10: 2b20 7374 6172 742c 2043 302e 666c 6174  + start, C0.flat
+00023e20: 7465 6e28 2920 2b20 7374 6172 745d 2929  ten() + start]))
+00023e30: 290a 2020 2020 3e3e 3e20 6174 6f6d 5f74  ).    >>> atom_t
+00023e40: 6f5f 7061 6972 203d 2074 6f72 6368 2e54  o_pair = torch.T
+00023e50: 656e 736f 7228 6174 6f6d 5f74 6f5f 7061  ensor(atom_to_pa
+00023e60: 6972 290a 2020 2020 3e3e 3e20 6174 6f6d  ir).    >>> atom
+00023e70: 5f74 6f5f 7061 6972 203d 2074 6f72 6368  _to_pair = torch
+00023e80: 2e73 7175 6565 7a65 2861 746f 6d5f 746f  .squeeze(atom_to
+00023e90: 5f70 6169 722e 746f 2874 6f72 6368 2e69  _pair.to(torch.i
+00023ea0: 6e74 3634 292c 2064 696d 3d30 290a 2020  nt64), dim=0).  
+00023eb0: 2020 3e3e 3e20 696e 7075 7473 203d 205b    >>> inputs = [
+00023ec0: 7061 6972 5f66 6561 7475 7265 732c 2061  pair_features, a
+00023ed0: 746f 6d5f 6665 6174 7572 6573 2c20 6174  tom_features, at
+00023ee0: 6f6d 5f74 6f5f 7061 6972 5d0a 2020 2020  om_to_pair].    
+00023ef0: 3e3e 3e20 6e5f 7061 6972 5f66 6561 7475  >>> n_pair_featu
+00023f00: 7265 7320 3d20 320a 2020 2020 3e3e 3e20  res = 2.    >>> 
+00023f10: 6e5f 6869 6464 656e 203d 2032 0a20 2020  n_hidden = 2.   
+00023f20: 203e 3e3e 2069 6e69 7420 3d20 2778 6176   >>> init = 'xav
+00023f30: 6965 725f 756e 6966 6f72 6d5f 270a 2020  ier_uniform_'.  
+00023f40: 2020 3e3e 3e20 6c61 7965 7220 3d20 4564    >>> layer = Ed
+00023f50: 6765 4e65 7477 6f72 6b28 6e5f 7061 6972  geNetwork(n_pair
+00023f60: 5f66 6561 7475 7265 732c 206e 5f68 6964  _features, n_hid
+00023f70: 6465 6e2c 2069 6e69 7429 0a20 2020 203e  den, init).    >
+00023f80: 3e3e 2072 6573 756c 7420 3d20 6c61 7965  >> result = laye
+00023f90: 7228 696e 7075 7473 290a 2020 2020 3e3e  r(inputs).    >>
+00023fa0: 3e20 7265 7375 6c74 2e73 6861 7065 5b31  > result.shape[1
+00023fb0: 5d0a 2020 2020 320a 2020 2020 2222 220a  ].    2.    """.
+00023fc0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00023fd0: 5f28 7365 6c66 2c0a 2020 2020 2020 2020  _(self,.        
+00023fe0: 2020 2020 2020 2020 206e 5f70 6169 725f           n_pair_
+00023ff0: 6665 6174 7572 6573 3a20 696e 7420 3d20  features: int = 
+00024000: 382c 0a20 2020 2020 2020 2020 2020 2020  8,.             
+00024010: 2020 2020 6e5f 6869 6464 656e 3a20 696e      n_hidden: in
+00024020: 7420 3d20 3130 302c 0a20 2020 2020 2020  t = 100,.       
+00024030: 2020 2020 2020 2020 2020 696e 6974 3a20            init: 
+00024040: 7374 7220 3d20 2778 6176 6965 725f 756e  str = 'xavier_un
+00024050: 6966 6f72 6d5f 272c 0a20 2020 2020 2020  iform_',.       
+00024060: 2020 2020 2020 2020 2020 2a2a 6b77 6172            **kwar
+00024070: 6773 293a 0a20 2020 2020 2020 2022 2222  gs):.        """
+00024080: 496e 6974 616c 6973 6573 2061 2045 6467  Initalises a Edg
+00024090: 654e 6574 776f 726b 204c 6179 6572 0a0a  eNetwork Layer..
+000240a0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+000240b0: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+000240c0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6e5f  -----.        n_
+000240d0: 7061 6972 5f66 6561 7475 7265 733a 2069  pair_features: i
+000240e0: 6e74 2c20 6f70 7469 6f6e 616c 0a20 2020  nt, optional.   
+000240f0: 2020 2020 2020 2020 2054 6865 206c 656e           The len
+00024100: 6774 6820 6f66 2074 6865 2070 6169 7220  gth of the pair 
+00024110: 6665 6174 7572 6573 2076 6563 746f 722e  features vector.
+00024120: 0a20 2020 2020 2020 206e 5f68 6964 6465  .        n_hidde
+00024130: 6e3a 2069 6e74 2c20 6f70 7469 6f6e 616c  n: int, optional
+00024140: 0a20 2020 2020 2020 2020 2020 206e 756d  .            num
+00024150: 6265 7220 6f66 2068 6964 6465 6e20 756e  ber of hidden un
+00024160: 6974 7320 696e 2074 6865 2070 6173 7369  its in the passi
+00024170: 6e67 2070 6861 7365 0a20 2020 2020 2020  ng phase.       
+00024180: 2069 6e69 743a 2073 7472 2c20 6f70 7469   init: str, opti
+00024190: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
+000241a0: 2049 6e69 7469 616c 697a 6174 696f 6e20   Initialization 
+000241b0: 6675 6e63 7469 6f6e 2074 6f20 6265 2075  function to be u
+000241c0: 7365 6420 696e 2074 6865 206d 6573 7361  sed in the messa
+000241d0: 6765 2070 6173 7369 6e67 206c 6179 6572  ge passing layer
+000241e0: 2e0a 2020 2020 2020 2020 2222 220a 0a20  ..        """.. 
+000241f0: 2020 2020 2020 2073 7570 6572 2845 6467         super(Edg
+00024200: 654e 6574 776f 726b 2c20 7365 6c66 292e  eNetwork, self).
+00024210: 5f5f 696e 6974 5f5f 282a 2a6b 7761 7267  __init__(**kwarg
+00024220: 7329 0a20 2020 2020 2020 2073 656c 662e  s).        self.
+00024230: 6e5f 7061 6972 5f66 6561 7475 7265 733a  n_pair_features:
+00024240: 2069 6e74 203d 206e 5f70 6169 725f 6665   int = n_pair_fe
+00024250: 6174 7572 6573 0a20 2020 2020 2020 2073  atures.        s
+00024260: 656c 662e 6e5f 6869 6464 656e 3a20 696e  elf.n_hidden: in
+00024270: 7420 3d20 6e5f 6869 6464 656e 0a20 2020  t = n_hidden.   
+00024280: 2020 2020 2073 656c 662e 696e 6974 3a20       self.init: 
+00024290: 7374 7220 3d20 696e 6974 0a0a 2020 2020  str = init..    
+000242a0: 2020 2020 696e 6974 5f66 756e 633a 2043      init_func: C
+000242b0: 616c 6c61 626c 6520 3d20 6765 7461 7474  allable = getatt
+000242c0: 7228 696e 6974 6961 6c69 7a65 7273 2c20  r(initializers, 
+000242d0: 7365 6c66 2e69 6e69 7429 0a20 2020 2020  self.init).     
+000242e0: 2020 2073 656c 662e 573a 2074 6f72 6368     self.W: torch
+000242f0: 2e54 656e 736f 7220 3d20 696e 6974 5f66  .Tensor = init_f
+00024300: 756e 6328 0a20 2020 2020 2020 2020 2020  unc(.           
+00024310: 2074 6f72 6368 2e65 6d70 7479 285b 7365   torch.empty([se
+00024320: 6c66 2e6e 5f70 6169 725f 6665 6174 7572  lf.n_pair_featur
+00024330: 6573 2c20 7365 6c66 2e6e 5f68 6964 6465  es, self.n_hidde
+00024340: 6e20 2a20 7365 6c66 2e6e 5f68 6964 6465  n * self.n_hidde
+00024350: 6e5d 2929 0a20 2020 2020 2020 2073 656c  n])).        sel
+00024360: 662e 623a 2074 6f72 6368 2e54 656e 736f  f.b: torch.Tenso
+00024370: 7220 3d20 746f 7263 682e 7a65 726f 7328  r = torch.zeros(
+00024380: 2873 656c 662e 6e5f 6869 6464 656e 202a  (self.n_hidden *
+00024390: 2073 656c 662e 6e5f 6869 6464 656e 2c29   self.n_hidden,)
+000243a0: 290a 2020 2020 2020 2020 7365 6c66 2e62  ).        self.b
+000243b0: 7569 6c74 3a20 626f 6f6c 203d 2054 7275  uilt: bool = Tru
+000243c0: 650a 0a20 2020 2064 6566 205f 5f72 6570  e..    def __rep
+000243d0: 725f 5f28 7365 6c66 2920 2d3e 2073 7472  r__(self) -> str
+000243e0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+000243f0: 2028 0a20 2020 2020 2020 2020 2020 2066   (.            f
+00024400: 277b 7365 6c66 2e5f 5f63 6c61 7373 5f5f  '{self.__class__
+00024410: 2e5f 5f6e 616d 655f 5f7d 286e 5f70 6169  .__name__}(n_pai
+00024420: 725f 6665 6174 7572 6573 3a7b 7365 6c66  r_features:{self
+00024430: 2e6e 5f70 6169 725f 6665 6174 7572 6573  .n_pair_features
+00024440: 7d2c 6e5f 6869 6464 656e 3a7b 7365 6c66  },n_hidden:{self
+00024450: 2e6e 5f68 6964 6465 6e7d 2c69 6e69 743a  .n_hidden},init:
+00024460: 7b73 656c 662e 696e 6974 7d29 270a 2020  {self.init})'.  
+00024470: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+00024480: 2066 6f72 7761 7264 2873 656c 662c 2069   forward(self, i
+00024490: 6e70 7574 733a 204c 6973 745b 746f 7263  nputs: List[torc
+000244a0: 682e 5465 6e73 6f72 5d29 202d 3e20 746f  h.Tensor]) -> to
+000244b0: 7263 682e 5465 6e73 6f72 3a0a 2020 2020  rch.Tensor:.    
+000244c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000244d0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+000244e0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+000244f0: 2020 2020 2020 696e 7075 7473 3a20 4c69        inputs: Li
+00024500: 7374 5b74 6f72 6368 2e54 656e 736f 725d  st[torch.Tensor]
+00024510: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+00024520: 206c 656e 6774 6820 6f66 2061 746f 6d5f   length of atom_
+00024530: 746f 5f70 6169 7220 7368 6f75 6c64 2062  to_pair should b
+00024540: 6520 7361 6d65 2061 7320 6e5f 7061 6972  e same as n_pair
+00024550: 5f66 6561 7475 7265 732e 0a20 2020 2020  _features..     
+00024560: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+00024570: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+00024580: 2020 2072 6573 756c 743a 2074 6f72 6368     result: torch
+00024590: 2e54 656e 736f 720a 2020 2020 2020 2020  .Tensor.        
+000245a0: 2020 2020 5465 6e73 6f72 2063 6f6e 7461      Tensor conta
+000245b0: 696e 696e 6720 7468 6520 6d61 7070 696e  ining the mappin
+000245c0: 6720 6f66 2074 6865 2065 6467 6520 7665  g of the edge ve
+000245d0: 6374 6f72 2074 6f20 6120 6420 c397 2064  ctor to a d .. d
+000245e0: 206d 6174 7269 782c 2077 6865 7265 2064   matrix, where d
+000245f0: 2064 656e 6f74 6573 2074 6865 2064 696d   denotes the dim
+00024600: 656e 7369 6f6e 206f 6620 7468 6520 696e  ension of the in
+00024610: 7465 726e 616c 2068 6964 6465 6e20 7265  ternal hidden re
+00024620: 7072 6573 656e 7461 7469 6f6e 206f 6620  presentation of 
+00024630: 6561 6368 206e 6f64 6520 696e 2074 6865  each node in the
+00024640: 2067 7261 7068 2e0a 2020 2020 2020 2020   graph..        
+00024650: 2222 220a 2020 2020 2020 2020 7061 6972  """.        pair
+00024660: 5f66 6561 7475 7265 733a 2074 6f72 6368  _features: torch
+00024670: 2e54 656e 736f 720a 2020 2020 2020 2020  .Tensor.        
+00024680: 6174 6f6d 5f66 6561 7475 7265 733a 2074  atom_features: t
+00024690: 6f72 6368 2e54 656e 736f 720a 2020 2020  orch.Tensor.    
+000246a0: 2020 2020 6174 6f6d 5f74 6f5f 7061 6972      atom_to_pair
+000246b0: 3a20 746f 7263 682e 5465 6e73 6f72 0a20  : torch.Tensor. 
+000246c0: 2020 2020 2020 2070 6169 725f 6665 6174         pair_feat
+000246d0: 7572 6573 2c20 6174 6f6d 5f66 6561 7475  ures, atom_featu
+000246e0: 7265 732c 2061 746f 6d5f 746f 5f70 6169  res, atom_to_pai
+000246f0: 7220 3d20 696e 7075 7473 0a0a 2020 2020  r = inputs..    
+00024700: 2020 2020 413a 2074 6f72 6368 2e54 656e      A: torch.Ten
+00024710: 736f 7220 3d20 746f 7263 682e 6164 6428  sor = torch.add(
+00024720: 746f 7263 682e 6d61 746d 756c 2870 6169  torch.matmul(pai
+00024730: 725f 6665 6174 7572 6573 2c20 7365 6c66  r_features, self
+00024740: 2e57 292c 2073 656c 662e 6229 0a20 2020  .W), self.b).   
+00024750: 2020 2020 2041 203d 2074 6f72 6368 2e72       A = torch.r
+00024760: 6573 6861 7065 2841 2c20 282d 312c 2073  eshape(A, (-1, s
+00024770: 656c 662e 6e5f 6869 6464 656e 2c20 7365  elf.n_hidden, se
+00024780: 6c66 2e6e 5f68 6964 6465 6e29 290a 2020  lf.n_hidden)).  
+00024790: 2020 2020 2020 6f75 743a 2074 6f72 6368        out: torch
+000247a0: 2e54 656e 736f 7220 3d20 746f 7263 682e  .Tensor = torch.
+000247b0: 756e 7371 7565 657a 6528 6174 6f6d 5f66  unsqueeze(atom_f
+000247c0: 6561 7475 7265 735b 6174 6f6d 5f74 6f5f  eatures[atom_to_
+000247d0: 7061 6972 5b3a 2c20 315d 5d2c 0a20 2020  pair[:, 1]],.   
+000247e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000247f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024800: 2020 2020 2020 2020 2064 696d 3d32 290a           dim=2).
+00024810: 2020 2020 2020 2020 6f75 745f 7371 7565          out_sque
+00024820: 657a 653a 2074 6f72 6368 2e54 656e 736f  eze: torch.Tenso
+00024830: 7220 3d20 746f 7263 682e 7371 7565 657a  r = torch.squeez
+00024840: 6528 746f 7263 682e 6d61 746d 756c 2841  e(torch.matmul(A
+00024850: 2c20 6f75 7429 2c20 6469 6d3d 3229 0a20  , out), dim=2). 
+00024860: 2020 2020 2020 2069 6e64 3a20 746f 7263         ind: torc
+00024870: 682e 5465 6e73 6f72 203d 2061 746f 6d5f  h.Tensor = atom_
+00024880: 746f 5f70 6169 725b 3a2c 2030 5d0a 0a20  to_pair[:, 0].. 
+00024890: 2020 2020 2020 2072 6573 756c 743a 2074         result: t
+000248a0: 6f72 6368 2e54 656e 736f 7220 3d20 7365  orch.Tensor = se
+000248b0: 676d 656e 745f 7375 6d28 6f75 745f 7371  gment_sum(out_sq
+000248c0: 7565 657a 652c 2069 6e64 290a 0a20 2020  ueeze, ind)..   
+000248d0: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+000248e0: 6c74 0a0a 0a63 6c61 7373 2057 6561 7665  lt...class Weave
+000248f0: 4c61 7965 7228 6e6e 2e4d 6f64 756c 6529  Layer(nn.Module)
+00024900: 3a0a 2020 2020 2222 2254 6869 7320 636c  :.    """This cl
+00024910: 6173 7320 696d 706c 656d 656e 7473 2074  ass implements t
+00024920: 6865 2063 6f72 6520 5765 6176 6520 636f  he core Weave co
+00024930: 6e76 6f6c 7574 696f 6e20 6672 6f6d 2074  nvolution from t
+00024940: 6865 2047 6f6f 676c 6520 6772 6170 6820  he Google graph 
+00024950: 636f 6e76 6f6c 7574 696f 6e20 7061 7065  convolution pape
+00024960: 7220 5b31 5d5f 0a20 2054 6869 7320 6973  r [1]_.  This is
+00024970: 2074 6865 2054 6f72 6368 2065 7175 6976   the Torch equiv
+00024980: 616c 656e 7420 6f66 2074 6865 206f 7269  alent of the ori
+00024990: 6769 6e61 6c20 696d 706c 656d 656e 7461  ginal implementa
+000249a0: 7469 6f6e 2075 7369 6e67 204b 6572 6173  tion using Keras
+000249b0: 2e0a 0a20 2054 6869 7320 6d6f 6465 6c20  ...  This model 
+000249c0: 636f 6e74 6169 6e73 2061 746f 6d20 6665  contains atom fe
+000249d0: 6174 7572 6573 2061 6e64 2062 6f6e 6420  atures and bond 
+000249e0: 6665 6174 7572 6573 0a20 2073 6570 6172  features.  separ
+000249f0: 6174 656c 792e 4865 7265 2c20 626f 6e64  ately.Here, bond
+00024a00: 2066 6561 7475 7265 7320 6172 6520 616c   features are al
+00024a10: 736f 2063 616c 6c65 6420 7061 6972 2066  so called pair f
+00024a20: 6561 7475 7265 732e 0a20 2054 6865 7265  eatures..  There
+00024a30: 2061 7265 2032 2074 7970 6573 206f 6620   are 2 types of 
+00024a40: 7472 616e 7366 6f72 6d61 7469 6f6e 2c20  transformation, 
+00024a50: 6174 6f6d 2d3e 6174 6f6d 2c20 6174 6f6d  atom->atom, atom
+00024a60: 2d3e 7061 6972 2c20 7061 6972 2d3e 6174  ->pair, pair->at
+00024a70: 6f6d 2c20 7061 6972 2d3e 7061 6972 2074  om, pair->pair t
+00024a80: 6861 7420 7468 6973 206d 6f64 656c 2069  hat this model i
+00024a90: 6d70 6c65 6d65 6e74 732e 0a0a 2020 4578  mplements...  Ex
+00024aa0: 616d 706c 6573 0a20 202d 2d2d 2d2d 2d2d  amples.  -------
+00024ab0: 2d0a 2020 5468 6973 206c 6179 6572 2065  -.  This layer e
+00024ac0: 7870 6563 7473 2034 2069 6e70 7574 7320  xpects 4 inputs 
+00024ad0: 696e 2061 206c 6973 7420 6f66 2074 6865  in a list of the
+00024ae0: 2066 6f72 6d20 605b 6174 6f6d 5f66 6561   form `[atom_fea
+00024af0: 7475 7265 732c 0a20 2070 6169 725f 6665  tures,.  pair_fe
+00024b00: 6174 7572 6573 2c20 7061 6972 5f73 706c  atures, pair_spl
+00024b10: 6974 2c20 6174 6f6d 5f74 6f5f 7061 6972  it, atom_to_pair
+00024b20: 5d60 2e20 5765 276c 6c20 7761 6c6b 2074  ]`. We'll walk t
+00024b30: 6872 6f75 6768 2074 6865 2073 7472 7563  hrough the struc
+00024b40: 7475 7265 206f 6620 7468 6573 6520 696e  ture of these in
+00024b50: 7075 7473 2e20 4c65 7427 7320 7374 6172  puts. Let's star
+00024b60: 7420 7769 7468 2073 6f6d 6520 6261 7369  t with some basi
+00024b70: 6320 6465 6669 6e69 7469 6f6e 732e 0a20  c definitions.. 
+00024b80: 203e 3e3e 2069 6d70 6f72 7420 6465 6570   >>> import deep
+00024b90: 6368 656d 2061 7320 6463 0a20 203e 3e3e  chem as dc.  >>>
+00024ba0: 2069 6d70 6f72 7420 6e75 6d70 7920 6173   import numpy as
+00024bb0: 206e 700a 2020 3e3e 3e20 736d 696c 6573   np.  >>> smiles
+00024bc0: 203d 205b 2243 4343 222c 2022 4322 5d0a   = ["CCC", "C"].
+00024bd0: 0a20 204e 6f74 6520 7468 6174 2074 6865  .  Note that the
+00024be0: 7265 2061 7265 2034 2061 746f 6d73 2069  re are 4 atoms i
+00024bf0: 6e20 746f 7461 6c20 696e 2074 6869 7320  n total in this 
+00024c00: 7379 7374 656d 2e20 5468 6973 206c 6179  system. This lay
+00024c10: 6572 2065 7870 6563 7473 2069 7473 2069  er expects its i
+00024c20: 6e70 7574 206d 6f6c 6563 756c 6573 2074  nput molecules t
+00024c30: 6f20 6265 2062 6174 6368 6564 2074 6f67  o be batched tog
+00024c40: 6574 6865 722e 0a0a 2020 3e3e 3e20 746f  ether...  >>> to
+00024c50: 7461 6c5f 6e5f 6174 6f6d 7320 3d20 340a  tal_n_atoms = 4.
+00024c60: 0a20 204c 6574 2773 2073 7570 706f 7365  .  Let's suppose
+00024c70: 2074 6861 7420 7765 2068 6176 6520 6120   that we have a 
+00024c80: 6665 6174 7572 697a 6572 2074 6861 7420  featurizer that 
+00024c90: 636f 6d70 7574 6573 2060 6e5f 6174 6f6d  computes `n_atom
+00024ca0: 5f66 6561 7460 2066 6561 7475 7265 7320  _feat` features 
+00024cb0: 7065 7220 6174 6f6d 2e0a 0a20 203e 3e3e  per atom...  >>>
+00024cc0: 206e 5f61 746f 6d5f 6665 6174 203d 2037   n_atom_feat = 7
+00024cd0: 350a 0a20 2054 6865 6e20 636f 6e63 6570  5..  Then concep
+00024ce0: 7475 616c 6c79 2c20 6061 746f 6d5f 6665  tually, `atom_fe
+00024cf0: 6174 6020 6973 2074 6865 2061 7272 6179  at` is the array
+00024d00: 206f 6620 7368 6170 6520 6028 746f 7461   of shape `(tota
+00024d10: 6c5f 6e5f 6174 6f6d 732c 0a20 206e 5f61  l_n_atoms,.  n_a
+00024d20: 746f 6d5f 6665 6174 2960 206f 6620 6174  tom_feat)` of at
+00024d30: 6f6d 6963 2066 6561 7475 7265 732e 2046  omic features. F
+00024d40: 6f72 2073 696d 706c 6963 6974 792c 206c  or simplicity, l
+00024d50: 6574 2773 206a 7573 7420 676f 2077 6974  et's just go wit
+00024d60: 6820 610a 2020 7261 6e64 6f6d 2073 7563  h a.  random suc
+00024d70: 6820 6d61 7472 6978 2e0a 0a20 203e 3e3e  h matrix...  >>>
+00024d80: 2061 746f 6d5f 6665 6174 203d 206e 702e   atom_feat = np.
+00024d90: 7261 6e64 6f6d 2e72 616e 6428 746f 7461  random.rand(tota
+00024da0: 6c5f 6e5f 6174 6f6d 732c 206e 5f61 746f  l_n_atoms, n_ato
+00024db0: 6d5f 6665 6174 290a 0a20 204c 6574 2773  m_feat)..  Let's
+00024dc0: 2073 7570 706f 7365 2077 6520 6861 7665   suppose we have
+00024dd0: 2060 6e5f 7061 6972 5f66 6561 7460 2070   `n_pair_feat` p
+00024de0: 6169 7277 6973 6520 6665 6174 7572 6573  airwise features
+00024df0: 0a0a 2020 3e3e 3e20 6e5f 7061 6972 5f66  ..  >>> n_pair_f
+00024e00: 6561 7420 3d20 3134 0a0a 2020 466f 7220  eat = 14..  For 
+00024e10: 6561 6368 206d 6f6c 6563 756c 652c 2077  each molecule, w
+00024e20: 6520 636f 6d70 7574 6520 6120 6d61 7472  e compute a matr
+00024e30: 6978 206f 6620 7368 6170 6520 6028 6e5f  ix of shape `(n_
+00024e40: 6174 6f6d 732a 6e5f 6174 6f6d 732c 0a20  atoms*n_atoms,. 
+00024e50: 206e 5f70 6169 725f 6665 6174 2960 206f   n_pair_feat)` o
+00024e60: 6620 7061 6972 7769 7365 2066 6561 7475  f pairwise featu
+00024e70: 7265 7320 666f 7220 6561 6368 2070 6169  res for each pai
+00024e80: 7220 6f66 2061 746f 6d73 2069 6e20 7468  r of atoms in th
+00024e90: 6520 6d6f 6c65 6375 6c65 2e0a 2020 4c65  e molecule..  Le
+00024ea0: 7427 7320 636f 6e73 7472 7563 7420 7468  t's construct th
+00024eb0: 6973 2063 6f6e 6365 7074 7561 6c6c 7920  is conceptually 
+00024ec0: 666f 7220 6f75 7220 6578 616d 706c 652e  for our example.
+00024ed0: 0a0a 2020 3e3e 3e20 7061 6972 5f66 6561  ..  >>> pair_fea
+00024ee0: 7420 3d20 5b6e 702e 7261 6e64 6f6d 2e72  t = [np.random.r
+00024ef0: 616e 6428 332a 332c 206e 5f70 6169 725f  and(3*3, n_pair_
+00024f00: 6665 6174 292c 206e 702e 7261 6e64 6f6d  feat), np.random
+00024f10: 2e72 616e 6428 312a 312c 6e5f 7061 6972  .rand(1*1,n_pair
+00024f20: 5f66 6561 7429 5d0a 2020 3e3e 3e20 7061  _feat)].  >>> pa
+00024f30: 6972 5f66 6561 7420 3d20 6e70 2e63 6f6e  ir_feat = np.con
+00024f40: 6361 7465 6e61 7465 2870 6169 725f 6665  catenate(pair_fe
+00024f50: 6174 2c20 6178 6973 3d30 290a 2020 3e3e  at, axis=0).  >>
+00024f60: 3e20 7061 6972 5f66 6561 742e 7368 6170  > pair_feat.shap
+00024f70: 650a 2020 2831 302c 2031 3429 0a0a 2020  e.  (10, 14)..  
+00024f80: 6070 6169 725f 7370 6c69 7460 2069 7320  `pair_split` is 
+00024f90: 616e 2069 6e64 6578 2069 6e74 6f20 6070  an index into `p
+00024fa0: 6169 725f 6665 6174 6020 7768 6963 6820  air_feat` which 
+00024fb0: 7465 6c6c 7320 7573 2077 6869 6368 2061  tells us which a
+00024fc0: 746f 6d20 6561 6368 2072 6f77 2062 656c  tom each row bel
+00024fd0: 6f6e 6773 2074 6f2e 2049 6e20 6f75 7220  ongs to. In our 
+00024fe0: 6361 7365 2c20 7765 2068 7665 0a0a 2020  case, we hve..  
+00024ff0: 3e3e 3e20 7061 6972 5f73 706c 6974 203d  >>> pair_split =
+00025000: 206e 702e 6172 7261 7928 5b30 2c20 302c   np.array([0, 0,
+00025010: 2030 2c20 312c 2031 2c20 312c 2032 2c20   0, 1, 1, 1, 2, 
+00025020: 322c 2032 2c20 335d 290a 0a20 2054 6861  2, 2, 3])..  Tha
+00025030: 7420 6973 2c20 7468 6520 6669 7273 7420  t is, the first 
+00025040: 3920 656e 7472 6965 7320 6265 6c6f 6e67  9 entries belong
+00025050: 2074 6f20 2243 4343 2220 616e 6420 7468   to "CCC" and th
+00025060: 6520 6c61 7374 2065 6e74 7279 2074 6f20  e last entry to 
+00025070: 2243 222e 2054 6865 0a20 2066 696e 616c  "C". The.  final
+00025080: 2065 6e74 7279 2060 6174 6f6d 5f74 6f5f   entry `atom_to_
+00025090: 7061 6972 6020 676f 6573 2069 6e20 6120  pair` goes in a 
+000250a0: 6c69 7474 6c65 206d 6f72 6520 696e 2d64  little more in-d
+000250b0: 6570 7468 2074 6861 6e20 6070 6169 725f  epth than `pair_
+000250c0: 7370 6c69 7460 0a20 2061 6e64 2074 656c  split`.  and tel
+000250d0: 6c73 2075 7320 7468 6520 7072 6563 6973  ls us the precis
+000250e0: 6520 7061 6972 2065 6163 6820 7061 6972  e pair each pair
+000250f0: 2066 6561 7475 7265 2062 656c 6f6e 6773   feature belongs
+00025100: 2074 6f2e 2049 6e20 6f75 7220 6361 7365   to. In our case
+00025110: 0a0a 2020 3e3e 3e20 6174 6f6d 5f74 6f5f  ..  >>> atom_to_
+00025120: 7061 6972 203d 206e 702e 6172 7261 7928  pair = np.array(
+00025130: 5b5b 302c 2030 5d2c 0a20 202e 2e2e 2020  [[0, 0],.  ...  
+00025140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025150: 2020 2020 2020 2020 5b30 2c20 315d 2c0a          [0, 1],.
+00025160: 2020 2e2e 2e20 2020 2020 2020 2020 2020    ...           
+00025170: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+00025180: 302c 2032 5d2c 0a20 202e 2e2e 2020 2020  0, 2],.  ...    
+00025190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000251a0: 2020 2020 2020 5b31 2c20 305d 2c0a 2020        [1, 0],.  
+000251b0: 2e2e 2e20 2020 2020 2020 2020 2020 2020  ...             
+000251c0: 2020 2020 2020 2020 2020 2020 205b 312c               [1,
+000251d0: 2031 5d2c 0a20 202e 2e2e 2020 2020 2020   1],.  ...      
+000251e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000251f0: 2020 2020 5b31 2c20 325d 2c0a 2020 2e2e      [1, 2],.  ..
+00025200: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
+00025210: 2020 2020 2020 2020 2020 205b 322c 2030             [2, 0
+00025220: 5d2c 0a20 202e 2e2e 2020 2020 2020 2020  ],.  ...        
+00025230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025240: 2020 5b32 2c20 315d 2c0a 2020 2e2e 2e20    [2, 1],.  ... 
+00025250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025260: 2020 2020 2020 2020 205b 322c 2032 5d2c           [2, 2],
+00025270: 0a20 202e 2e2e 2020 2020 2020 2020 2020  .  ...          
+00025280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025290: 5b33 2c20 335d 5d29 0a0a 2020 4c65 7427  [3, 3]])..  Let'
+000252a0: 7320 6e6f 7720 6465 6669 6e65 2074 6865  s now define the
+000252b0: 2061 6374 7561 6c20 6c61 7965 720a 0a20   actual layer.. 
+000252c0: 203e 3e3e 206c 6179 6572 203d 2057 6561   >>> layer = Wea
+000252d0: 7665 4c61 7965 7228 290a 0a20 2041 6e64  veLayer()..  And
+000252e0: 2069 6e76 6f6b 6520 6974 0a0a 2020 3e3e   invoke it..  >>
+000252f0: 3e20 5b41 2c20 505d 203d 206c 6179 6572  > [A, P] = layer
+00025300: 285b 6174 6f6d 5f66 6561 742c 2070 6169  ([atom_feat, pai
+00025310: 725f 6665 6174 2c20 7061 6972 5f73 706c  r_feat, pair_spl
+00025320: 6974 2c20 6174 6f6d 5f74 6f5f 7061 6972  it, atom_to_pair
+00025330: 5d29 0a0a 2020 5468 6520 7765 6176 6520  ])..  The weave 
+00025340: 6c61 7965 7220 7072 6f64 7563 6573 206e  layer produces n
+00025350: 6577 2061 746f 6d2f 7061 6972 2066 6561  ew atom/pair fea
+00025360: 7475 7265 732e 204c 6574 2773 2063 6865  tures. Let's che
+00025370: 636b 2074 6865 6972 2073 6861 7065 730a  ck their shapes.
+00025380: 0a20 203e 3e3e 2041 203d 2041 2e64 6574  .  >>> A = A.det
+00025390: 6163 6828 292e 6e75 6d70 7928 290a 2020  ach().numpy().  
+000253a0: 3e3e 3e20 412e 7368 6170 650a 2020 2834  >>> A.shape.  (4
+000253b0: 2c20 3530 290a 2020 3e3e 3e20 5020 3d20  , 50).  >>> P = 
+000253c0: 502e 6465 7461 6368 2829 2e6e 756d 7079  P.detach().numpy
+000253d0: 2829 0a20 203e 3e3e 2050 2e73 6861 7065  ().  >>> P.shape
+000253e0: 0a20 2028 3130 2c20 3530 290a 0a20 2054  .  (10, 50)..  T
+000253f0: 6865 2034 2069 7320 6074 6f74 616c 5f6e  he 4 is `total_n
+00025400: 756d 5f61 746f 6d73 6020 616e 6420 7468  um_atoms` and th
+00025410: 6520 3130 2069 7320 7468 6520 746f 7461  e 10 is the tota
+00025420: 6c20 6e75 6d62 6572 206f 6620 7061 6972  l number of pair
+00025430: 732e 2057 6865 7265 0a20 2064 6f65 7320  s. Where.  does 
+00025440: 6035 3060 2063 6f6d 6520 6672 6f6d 3f20  `50` come from? 
+00025450: 4974 2773 2066 726f 6d20 7468 6520 6465  It's from the de
+00025460: 6661 756c 7420 6172 6775 6d65 6e74 7320  fault arguments 
+00025470: 606e 5f61 746f 6d5f 696e 7075 745f 6665  `n_atom_input_fe
+00025480: 6174 6020 616e 640a 2020 606e 5f70 6169  at` and.  `n_pai
+00025490: 725f 696e 7075 745f 6665 6174 602e 0a0a  r_input_feat`...
+000254a0: 2020 5265 6665 7265 6e63 6573 0a20 202d    References.  -
+000254b0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2e2e 205b  ---------.  .. [
+000254c0: 315d 204b 6561 726e 6573 2c20 5374 6576  1] Kearnes, Stev
+000254d0: 656e 2c20 6574 2061 6c2e 2022 4d6f 6c65  en, et al. "Mole
+000254e0: 6375 6c61 7220 6772 6170 6820 636f 6e76  cular graph conv
+000254f0: 6f6c 7574 696f 6e73 3a20 6d6f 7669 6e67  olutions: moving
+00025500: 2062 6579 6f6e 640a 2020 2020 2020 2020   beyond.        
+00025510: 6669 6e67 6572 7072 696e 7473 2e22 204a  fingerprints." J
+00025520: 6f75 726e 616c 206f 6620 636f 6d70 7574  ournal of comput
+00025530: 6572 2d61 6964 6564 206d 6f6c 6563 756c  er-aided molecul
+00025540: 6172 2064 6573 6967 6e20 3330 2e38 2028  ar design 30.8 (
+00025550: 3230 3136 293a 0a20 2020 2020 2020 2035  2016):.        5
+00025560: 3935 2d36 3038 2e0a 2020 2222 220a 0a20  95-608..  """.. 
+00025570: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00025580: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+00025590: 2020 2020 2020 206e 5f61 746f 6d5f 696e         n_atom_in
+000255a0: 7075 745f 6665 6174 3a20 696e 7420 3d20  put_feat: int = 
+000255b0: 3735 2c0a 2020 2020 2020 2020 2020 2020  75,.            
+000255c0: 2020 2020 206e 5f70 6169 725f 696e 7075       n_pair_inpu
+000255d0: 745f 6665 6174 3a20 696e 7420 3d20 3134  t_feat: int = 14
+000255e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000255f0: 2020 206e 5f61 746f 6d5f 6f75 7470 7574     n_atom_output
+00025600: 5f66 6561 743a 2069 6e74 203d 2035 302c  _feat: int = 50,
+00025610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025620: 2020 6e5f 7061 6972 5f6f 7574 7075 745f    n_pair_output_
+00025630: 6665 6174 3a20 696e 7420 3d20 3530 2c0a  feat: int = 50,.
+00025640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025650: 206e 5f68 6964 6465 6e5f 4141 3a20 696e   n_hidden_AA: in
+00025660: 7420 3d20 3530 2c0a 2020 2020 2020 2020  t = 50,.        
+00025670: 2020 2020 2020 2020 206e 5f68 6964 6465           n_hidde
+00025680: 6e5f 5041 3a20 696e 7420 3d20 3530 2c0a  n_PA: int = 50,.
+00025690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000256a0: 206e 5f68 6964 6465 6e5f 4150 3a20 696e   n_hidden_AP: in
+000256b0: 7420 3d20 3530 2c0a 2020 2020 2020 2020  t = 50,.        
+000256c0: 2020 2020 2020 2020 206e 5f68 6964 6465           n_hidde
+000256d0: 6e5f 5050 3a20 696e 7420 3d20 3530 2c0a  n_PP: int = 50,.
+000256e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000256f0: 2075 7064 6174 655f 7061 6972 3a20 626f   update_pair: bo
+00025700: 6f6c 203d 2054 7275 652c 0a20 2020 2020  ol = True,.     
+00025710: 2020 2020 2020 2020 2020 2020 696e 6974              init
+00025720: 5f3a 2073 7472 203d 2027 7861 7669 6572  _: str = 'xavier
+00025730: 5f75 6e69 666f 726d 5f27 2c0a 2020 2020  _uniform_',.    
+00025740: 2020 2020 2020 2020 2020 2020 2061 6374               act
+00025750: 6976 6174 696f 6e3a 2073 7472 203d 2027  ivation: str = '
+00025760: 7265 6c75 272c 0a20 2020 2020 2020 2020  relu',.         
+00025770: 2020 2020 2020 2020 6261 7463 685f 6e6f          batch_no
+00025780: 726d 616c 697a 653a 2062 6f6f 6c20 3d20  rmalize: bool = 
+00025790: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+000257a0: 2020 2020 2020 202a 2a6b 7761 7267 7329         **kwargs)
+000257b0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+000257c0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+000257d0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+000257e0: 6e5f 6174 6f6d 5f69 6e70 7574 5f66 6561  n_atom_input_fea
+000257f0: 743a 2069 6e74 2c20 6f70 7469 6f6e 616c  t: int, optional
+00025800: 2028 6465 6661 756c 7420 3735 290a 2020   (default 75).  
+00025810: 2020 2020 4e75 6d62 6572 206f 6620 6665      Number of fe
+00025820: 6174 7572 6573 2066 6f72 2065 6163 6820  atures for each 
+00025830: 6174 6f6d 2069 6e20 696e 7075 742e 0a20  atom in input.. 
+00025840: 2020 206e 5f70 6169 725f 696e 7075 745f     n_pair_input_
+00025850: 6665 6174 3a20 696e 742c 206f 7074 696f  feat: int, optio
+00025860: 6e61 6c20 2864 6566 6175 6c74 2031 3429  nal (default 14)
+00025870: 0a20 2020 2020 204e 756d 6265 7220 6f66  .      Number of
+00025880: 2066 6561 7475 7265 7320 666f 7220 6561   features for ea
+00025890: 6368 2070 6169 7220 6f66 2061 746f 6d73  ch pair of atoms
+000258a0: 2069 6e20 696e 7075 742e 0a20 2020 206e   in input..    n
+000258b0: 5f61 746f 6d5f 6f75 7470 7574 5f66 6561  _atom_output_fea
+000258c0: 743a 2069 6e74 2c20 6f70 7469 6f6e 616c  t: int, optional
+000258d0: 2028 6465 6661 756c 7420 3530 290a 2020   (default 50).  
+000258e0: 2020 2020 4e75 6d62 6572 206f 6620 6665      Number of fe
+000258f0: 6174 7572 6573 2066 6f72 2065 6163 6820  atures for each 
+00025900: 6174 6f6d 2069 6e20 6f75 7470 7574 2e0a  atom in output..
+00025910: 2020 2020 6e5f 7061 6972 5f6f 7574 7075      n_pair_outpu
+00025920: 745f 6665 6174 3a20 696e 742c 206f 7074  t_feat: int, opt
+00025930: 696f 6e61 6c20 2864 6566 6175 6c74 2035  ional (default 5
+00025940: 3029 0a20 2020 2020 204e 756d 6265 7220  0).      Number 
+00025950: 6f66 2066 6561 7475 7265 7320 666f 7220  of features for 
+00025960: 6561 6368 2070 6169 7220 6f66 2061 746f  each pair of ato
+00025970: 6d73 2069 6e20 6f75 7470 7574 2e0a 2020  ms in output..  
+00025980: 2020 6e5f 6869 6464 656e 5f41 413a 2069    n_hidden_AA: i
+00025990: 6e74 2c20 6f70 7469 6f6e 616c 2028 6465  nt, optional (de
+000259a0: 6661 756c 7420 3530 290a 2020 2020 2020  fault 50).      
+000259b0: 4e75 6d62 6572 206f 6620 756e 6974 7328  Number of units(
+000259c0: 636f 6e76 6f6c 7574 696f 6e20 6465 7074  convolution dept
+000259d0: 6873 2920 696e 2063 6f72 7265 7370 6f6e  hs) in correspon
+000259e0: 6469 6e67 2068 6964 6465 6e20 6c61 7965  ding hidden laye
+000259f0: 720a 2020 2020 6e5f 6869 6464 656e 5f50  r.    n_hidden_P
+00025a00: 413a 2069 6e74 2c20 6f70 7469 6f6e 616c  A: int, optional
+00025a10: 2028 6465 6661 756c 7420 3530 290a 2020   (default 50).  
+00025a20: 2020 2020 4e75 6d62 6572 206f 6620 756e      Number of un
+00025a30: 6974 7328 636f 6e76 6f6c 7574 696f 6e20  its(convolution 
+00025a40: 6465 7074 6873 2920 696e 2063 6f72 7265  depths) in corre
+00025a50: 7370 6f6e 6469 6e67 2068 6964 6465 6e20  sponding hidden 
+00025a60: 6c61 7965 720a 2020 2020 6e5f 6869 6464  layer.    n_hidd
+00025a70: 656e 5f41 503a 2069 6e74 2c20 6f70 7469  en_AP: int, opti
+00025a80: 6f6e 616c 2028 6465 6661 756c 7420 3530  onal (default 50
+00025a90: 290a 2020 2020 2020 4e75 6d62 6572 206f  ).      Number o
+00025aa0: 6620 756e 6974 7328 636f 6e76 6f6c 7574  f units(convolut
+00025ab0: 696f 6e20 6465 7074 6873 2920 696e 2063  ion depths) in c
+00025ac0: 6f72 7265 7370 6f6e 6469 6e67 2068 6964  orresponding hid
+00025ad0: 6465 6e20 6c61 7965 720a 2020 2020 6e5f  den layer.    n_
+00025ae0: 6869 6464 656e 5f50 503a 2069 6e74 2c20  hidden_PP: int, 
+00025af0: 6f70 7469 6f6e 616c 2028 6465 6661 756c  optional (defaul
+00025b00: 7420 3530 290a 2020 2020 2020 4e75 6d62  t 50).      Numb
+00025b10: 6572 206f 6620 756e 6974 7328 636f 6e76  er of units(conv
+00025b20: 6f6c 7574 696f 6e20 6465 7074 6873 2920  olution depths) 
+00025b30: 696e 2063 6f72 7265 7370 6f6e 6469 6e67  in corresponding
+00025b40: 2068 6964 6465 6e20 6c61 7965 720a 2020   hidden layer.  
+00025b50: 2020 7570 6461 7465 5f70 6169 723a 2062    update_pair: b
+00025b60: 6f6f 6c2c 206f 7074 696f 6e61 6c20 2864  ool, optional (d
+00025b70: 6566 6175 6c74 2054 7275 6529 0a20 2020  efault True).   
+00025b80: 2020 2057 6865 7468 6572 2074 6f20 6361     Whether to ca
+00025b90: 6c63 756c 6174 6520 666f 7220 7061 6972  lculate for pair
+00025ba0: 2066 6561 7475 7265 732c 0a20 2020 2020   features,.     
+00025bb0: 2063 6f75 6c64 2062 6520 7475 726e 6564   could be turned
+00025bc0: 206f 6666 2066 6f72 206c 6173 7420 6c61   off for last la
+00025bd0: 7965 720a 2020 2020 696e 6974 3a20 7374  yer.    init: st
+00025be0: 722c 206f 7074 696f 6e61 6c20 2864 6566  r, optional (def
+00025bf0: 6175 6c74 2027 7861 7669 6572 5f75 6e69  ault 'xavier_uni
+00025c00: 666f 726d 5f27 290a 2020 2020 2020 5765  form_').      We
+00025c10: 6967 6874 2069 6e69 7469 616c 697a 6174  ight initializat
+00025c20: 696f 6e20 666f 7220 6669 6c74 6572 732e  ion for filters.
+00025c30: 0a20 2020 2061 6374 6976 6174 696f 6e3a  .    activation:
+00025c40: 2073 7472 2c20 6f70 7469 6f6e 616c 2028   str, optional (
+00025c50: 6465 6661 756c 7420 2772 656c 7527 290a  default 'relu').
+00025c60: 2020 2020 2020 4163 7469 7661 7469 6f6e        Activation
+00025c70: 2066 756e 6374 696f 6e20 6170 706c 6965   function applie
+00025c80: 640a 2020 2020 6261 7463 685f 6e6f 726d  d.    batch_norm
+00025c90: 616c 697a 653a 2062 6f6f 6c2c 206f 7074  alize: bool, opt
+00025ca0: 696f 6e61 6c20 2864 6566 6175 6c74 2054  ional (default T
+00025cb0: 7275 6529 0a20 2020 2020 2049 6620 7468  rue).      If th
+00025cc0: 6973 2069 7320 7475 726e 6564 206f 6e2c  is is turned on,
+00025cd0: 2061 7070 6c79 2062 6174 6368 206e 6f72   apply batch nor
+00025ce0: 6d61 6c69 7a61 7469 6f6e 2062 6566 6f72  malization befor
+00025cf0: 6520 6170 706c 7969 6e67 0a20 2020 2020  e applying.     
+00025d00: 2061 6374 6976 6174 696f 6e20 6675 6e63   activation func
+00025d10: 7469 6f6e 7320 6f6e 2063 6f6e 766f 6c75  tions on convolu
+00025d20: 7469 6f6e 616c 206c 6179 6572 732e 0a20  tional layers.. 
+00025d30: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
+00025d40: 7570 6572 2857 6561 7665 4c61 7965 722c  uper(WeaveLayer,
+00025d50: 2073 656c 6629 2e5f 5f69 6e69 745f 5f28   self).__init__(
+00025d60: 2a2a 6b77 6172 6773 290a 2020 2020 2020  **kwargs).      
+00025d70: 2020 7365 6c66 2e69 6e69 743a 2073 7472    self.init: str
+00025d80: 203d 2069 6e69 745f 2020 2320 5365 7420   = init_  # Set 
+00025d90: 7765 6967 6874 2069 6e69 7469 616c 697a  weight initializ
+00025da0: 6174 696f 6e0a 2020 2020 2020 2020 7365  ation.        se
+00025db0: 6c66 2e61 6374 6976 6174 696f 6e3a 2073  lf.activation: s
+00025dc0: 7472 203d 2061 6374 6976 6174 696f 6e20  tr = activation 
+00025dd0: 2023 2047 6574 2061 6374 6976 6174 696f   # Get activatio
+00025de0: 6e73 0a20 2020 2020 2020 2073 656c 662e  ns.        self.
+00025df0: 6163 7469 7661 7469 6f6e 5f66 6e3a 2074  activation_fn: t
+00025e00: 6f72 6368 2e6e 6e2e 4d6f 6475 6c65 203d  orch.nn.Module =
+00025e10: 2067 6574 5f61 6374 6976 6174 696f 6e28   get_activation(
+00025e20: 6163 7469 7661 7469 6f6e 290a 2020 2020  activation).    
+00025e30: 2020 2020 7365 6c66 2e75 7064 6174 655f      self.update_
+00025e40: 7061 6972 3a20 626f 6f6c 203d 2075 7064  pair: bool = upd
+00025e50: 6174 655f 7061 6972 2020 2320 6c61 7374  ate_pair  # last
+00025e60: 2077 6561 7665 206c 6179 6572 2064 6f65   weave layer doe
+00025e70: 7320 6e6f 7420 6e65 6564 2074 6f20 7570  s not need to up
+00025e80: 6461 7465 0a20 2020 2020 2020 2073 656c  date.        sel
+00025e90: 662e 6e5f 6869 6464 656e 5f41 413a 2069  f.n_hidden_AA: i
+00025ea0: 6e74 203d 206e 5f68 6964 6465 6e5f 4141  nt = n_hidden_AA
+00025eb0: 0a20 2020 2020 2020 2073 656c 662e 6e5f  .        self.n_
+00025ec0: 6869 6464 656e 5f50 413a 2069 6e74 203d  hidden_PA: int =
+00025ed0: 206e 5f68 6964 6465 6e5f 5041 0a20 2020   n_hidden_PA.   
+00025ee0: 2020 2020 2073 656c 662e 6e5f 6869 6464       self.n_hidd
+00025ef0: 656e 5f41 503a 2069 6e74 203d 206e 5f68  en_AP: int = n_h
+00025f00: 6964 6465 6e5f 4150 0a20 2020 2020 2020  idden_AP.       
+00025f10: 2073 656c 662e 6e5f 6869 6464 656e 5f50   self.n_hidden_P
+00025f20: 503a 2069 6e74 203d 206e 5f68 6964 6465  P: int = n_hidde
+00025f30: 6e5f 5050 0a20 2020 2020 2020 2073 656c  n_PP.        sel
+00025f40: 662e 6e5f 6869 6464 656e 5f41 3a20 696e  f.n_hidden_A: in
+00025f50: 7420 3d20 6e5f 6869 6464 656e 5f41 4120  t = n_hidden_AA 
+00025f60: 2b20 6e5f 6869 6464 656e 5f50 410a 2020  + n_hidden_PA.  
+00025f70: 2020 2020 2020 7365 6c66 2e6e 5f68 6964        self.n_hid
+00025f80: 6465 6e5f 503a 2069 6e74 203d 206e 5f68  den_P: int = n_h
+00025f90: 6964 6465 6e5f 4150 202b 206e 5f68 6964  idden_AP + n_hid
+00025fa0: 6465 6e5f 5050 0a20 2020 2020 2020 2073  den_PP.        s
+00025fb0: 656c 662e 6261 7463 685f 6e6f 726d 616c  elf.batch_normal
+00025fc0: 697a 653a 2062 6f6f 6c20 3d20 6261 7463  ize: bool = batc
+00025fd0: 685f 6e6f 726d 616c 697a 650a 0a20 2020  h_normalize..   
+00025fe0: 2020 2020 2073 656c 662e 6e5f 6174 6f6d       self.n_atom
+00025ff0: 5f69 6e70 7574 5f66 6561 743a 2069 6e74  _input_feat: int
+00026000: 203d 206e 5f61 746f 6d5f 696e 7075 745f   = n_atom_input_
+00026010: 6665 6174 0a20 2020 2020 2020 2073 656c  feat.        sel
+00026020: 662e 6e5f 7061 6972 5f69 6e70 7574 5f66  f.n_pair_input_f
+00026030: 6561 743a 2069 6e74 203d 206e 5f70 6169  eat: int = n_pai
+00026040: 725f 696e 7075 745f 6665 6174 0a20 2020  r_input_feat.   
+00026050: 2020 2020 2073 656c 662e 6e5f 6174 6f6d       self.n_atom
+00026060: 5f6f 7574 7075 745f 6665 6174 3a20 696e  _output_feat: in
+00026070: 7420 3d20 6e5f 6174 6f6d 5f6f 7574 7075  t = n_atom_outpu
+00026080: 745f 6665 6174 0a20 2020 2020 2020 2073  t_feat.        s
+00026090: 656c 662e 6e5f 7061 6972 5f6f 7574 7075  elf.n_pair_outpu
+000260a0: 745f 6665 6174 3a20 696e 7420 3d20 6e5f  t_feat: int = n_
+000260b0: 7061 6972 5f6f 7574 7075 745f 6665 6174  pair_output_feat
+000260c0: 0a0a 2020 2020 2020 2020 2320 436f 6e73  ..        # Cons
+000260d0: 7472 7563 7420 696e 7465 726e 616c 2074  truct internal t
+000260e0: 7261 696e 6162 6c65 2077 6569 6768 7473  rainable weights
+000260f0: 0a20 2020 2020 2020 2069 6e69 7420 3d20  .        init = 
+00026100: 6765 7461 7474 7228 696e 6974 6961 6c69  getattr(initiali
+00026110: 7a65 7273 2c20 7365 6c66 2e69 6e69 7429  zers, self.init)
+00026120: 0a20 2020 2020 2020 2023 2057 6569 6768  .        # Weigh
+00026130: 7420 6d61 7472 6978 2061 6e64 2062 6961  t matrix and bia
+00026140: 7320 6d61 7472 6978 2072 6571 7569 7265  s matrix require
+00026150: 6420 746f 2063 6f6d 7075 7465 206e 6577  d to compute new
+00026160: 2061 746f 6d20 6c61 7965 7220 6672 6f6d   atom layer from
+00026170: 2074 6865 2070 7265 7669 6f75 7320 6174   the previous at
+00026180: 6f6d 206c 6179 6572 0a20 2020 2020 2020  om layer.       
+00026190: 2073 656c 662e 575f 4141 3a20 746f 7263   self.W_AA: torc
+000261a0: 682e 5465 6e73 6f72 203d 2069 6e69 7428  h.Tensor = init(
+000261b0: 0a20 2020 2020 2020 2020 2020 2074 6f72  .            tor
+000261c0: 6368 2e65 6d70 7479 2873 656c 662e 6e5f  ch.empty(self.n_
+000261d0: 6174 6f6d 5f69 6e70 7574 5f66 6561 742c  atom_input_feat,
+000261e0: 2073 656c 662e 6e5f 6869 6464 656e 5f41   self.n_hidden_A
+000261f0: 4129 290a 2020 2020 2020 2020 7365 6c66  A)).        self
+00026200: 2e62 5f41 413a 2074 6f72 6368 2e54 656e  .b_AA: torch.Ten
+00026210: 736f 7220 3d20 746f 7263 682e 7a65 726f  sor = torch.zero
+00026220: 7328 2873 656c 662e 6e5f 6869 6464 656e  s((self.n_hidden
+00026230: 5f41 412c 2929 0a20 2020 2020 2020 2073  _AA,)).        s
+00026240: 656c 662e 4141 5f62 6e3a 206e 6e2e 4261  elf.AA_bn: nn.Ba
+00026250: 7463 684e 6f72 6d31 6420 3d20 6e6e 2e42  tchNorm1d = nn.B
+00026260: 6174 6368 4e6f 726d 3164 280a 2020 2020  atchNorm1d(.    
+00026270: 2020 2020 2020 2020 6e75 6d5f 6665 6174          num_feat
+00026280: 7572 6573 3d73 656c 662e 6e5f 6869 6464  ures=self.n_hidd
+00026290: 656e 5f41 412c 0a20 2020 2020 2020 2020  en_AA,.         
+000262a0: 2020 2065 7073 3d31 652d 332c 0a20 2020     eps=1e-3,.   
+000262b0: 2020 2020 2020 2020 206d 6f6d 656e 7475           momentu
+000262c0: 6d3d 302e 3939 2c0a 2020 2020 2020 2020  m=0.99,.        
+000262d0: 2020 2020 6166 6669 6e65 3d54 7275 652c      affine=True,
+000262e0: 0a20 2020 2020 2020 2020 2020 2074 7261  .            tra
+000262f0: 636b 5f72 756e 6e69 6e67 5f73 7461 7473  ck_running_stats
+00026300: 3d54 7275 6529 0a0a 2020 2020 2020 2020  =True)..        
+00026310: 2320 5765 6967 6874 206d 6174 7269 7820  # Weight matrix 
+00026320: 616e 6420 6269 6173 206d 6174 7269 7820  and bias matrix 
+00026330: 7265 7175 6972 6564 2074 6f20 636f 6d70  required to comp
+00026340: 7574 6520 6e65 7720 6174 6f6d 206c 6179  ute new atom lay
+00026350: 6572 2066 726f 6d20 7468 6520 7072 6576  er from the prev
+00026360: 696f 7573 2070 6169 7220 6c61 7965 720a  ious pair layer.
+00026370: 2020 2020 2020 2020 7365 6c66 2e57 5f50          self.W_P
+00026380: 413a 2074 6f72 6368 2e54 656e 736f 7220  A: torch.Tensor 
+00026390: 3d20 696e 6974 280a 2020 2020 2020 2020  = init(.        
+000263a0: 2020 2020 746f 7263 682e 656d 7074 7928      torch.empty(
+000263b0: 7365 6c66 2e6e 5f70 6169 725f 696e 7075  self.n_pair_inpu
+000263c0: 745f 6665 6174 2c20 7365 6c66 2e6e 5f68  t_feat, self.n_h
+000263d0: 6964 6465 6e5f 5041 2929 0a20 2020 2020  idden_PA)).     
+000263e0: 2020 2073 656c 662e 625f 5041 3a20 746f     self.b_PA: to
+000263f0: 7263 682e 5465 6e73 6f72 203d 2074 6f72  rch.Tensor = tor
+00026400: 6368 2e7a 6572 6f73 2828 7365 6c66 2e6e  ch.zeros((self.n
+00026410: 5f68 6964 6465 6e5f 5041 2c29 290a 2020  _hidden_PA,)).  
+00026420: 2020 2020 2020 7365 6c66 2e50 415f 626e        self.PA_bn
+00026430: 3a20 6e6e 2e42 6174 6368 4e6f 726d 3164  : nn.BatchNorm1d
+00026440: 203d 206e 6e2e 4261 7463 684e 6f72 6d31   = nn.BatchNorm1
+00026450: 6428 0a20 2020 2020 2020 2020 2020 206e  d(.            n
+00026460: 756d 5f66 6561 7475 7265 733d 7365 6c66  um_features=self
+00026470: 2e6e 5f68 6964 6465 6e5f 5041 2c0a 2020  .n_hidden_PA,.  
+00026480: 2020 2020 2020 2020 2020 6570 733d 3165            eps=1e
+00026490: 2d33 2c0a 2020 2020 2020 2020 2020 2020  -3,.            
+000264a0: 6d6f 6d65 6e74 756d 3d30 2e39 392c 0a20  momentum=0.99,. 
+000264b0: 2020 2020 2020 2020 2020 2061 6666 696e             affin
+000264c0: 653d 5472 7565 2c0a 2020 2020 2020 2020  e=True,.        
+000264d0: 2020 2020 7472 6163 6b5f 7275 6e6e 696e      track_runnin
+000264e0: 675f 7374 6174 733d 5472 7565 290a 0a20  g_stats=True).. 
+000264f0: 2020 2020 2020 2073 656c 662e 575f 413a         self.W_A:
+00026500: 2074 6f72 6368 2e54 656e 736f 7220 3d20   torch.Tensor = 
+00026510: 696e 6974 280a 2020 2020 2020 2020 2020  init(.          
+00026520: 2020 746f 7263 682e 656d 7074 7928 7365    torch.empty(se
+00026530: 6c66 2e6e 5f68 6964 6465 6e5f 412c 2073  lf.n_hidden_A, s
+00026540: 656c 662e 6e5f 6174 6f6d 5f6f 7574 7075  elf.n_atom_outpu
+00026550: 745f 6665 6174 2929 0a20 2020 2020 2020  t_feat)).       
+00026560: 2073 656c 662e 625f 413a 2074 6f72 6368   self.b_A: torch
+00026570: 2e54 656e 736f 7220 3d20 746f 7263 682e  .Tensor = torch.
+00026580: 7a65 726f 7328 2873 656c 662e 6e5f 6174  zeros((self.n_at
+00026590: 6f6d 5f6f 7574 7075 745f 6665 6174 2c29  om_output_feat,)
+000265a0: 290a 2020 2020 2020 2020 7365 6c66 2e41  ).        self.A
+000265b0: 5f62 6e3a 206e 6e2e 4261 7463 684e 6f72  _bn: nn.BatchNor
+000265c0: 6d31 6420 3d20 6e6e 2e42 6174 6368 4e6f  m1d = nn.BatchNo
+000265d0: 726d 3164 280a 2020 2020 2020 2020 2020  rm1d(.          
+000265e0: 2020 6e75 6d5f 6665 6174 7572 6573 3d73    num_features=s
+000265f0: 656c 662e 6e5f 6174 6f6d 5f6f 7574 7075  elf.n_atom_outpu
+00026600: 745f 6665 6174 2c0a 2020 2020 2020 2020  t_feat,.        
+00026610: 2020 2020 6570 733d 3165 2d33 2c0a 2020      eps=1e-3,.  
+00026620: 2020 2020 2020 2020 2020 6d6f 6d65 6e74            moment
+00026630: 756d 3d30 2e39 392c 0a20 2020 2020 2020  um=0.99,.       
+00026640: 2020 2020 2061 6666 696e 653d 5472 7565       affine=True
+00026650: 2c0a 2020 2020 2020 2020 2020 2020 7472  ,.            tr
+00026660: 6163 6b5f 7275 6e6e 696e 675f 7374 6174  ack_running_stat
+00026670: 733d 5472 7565 290a 0a20 2020 2020 2020  s=True)..       
+00026680: 2069 6620 7365 6c66 2e75 7064 6174 655f   if self.update_
+00026690: 7061 6972 3a0a 2020 2020 2020 2020 2020  pair:.          
+000266a0: 2020 2320 5765 6967 6874 206d 6174 7269    # Weight matri
+000266b0: 7820 616e 6420 6269 6173 206d 6174 7269  x and bias matri
+000266c0: 7820 7265 7175 6972 6564 2074 6f20 636f  x required to co
+000266d0: 6d70 7574 6520 6e65 7720 7061 6972 206c  mpute new pair l
+000266e0: 6179 6572 2066 726f 6d20 7468 6520 7072  ayer from the pr
+000266f0: 6576 696f 7573 2061 746f 6d20 6c61 7965  evious atom laye
+00026700: 720a 2020 2020 2020 2020 2020 2020 7365  r.            se
+00026710: 6c66 2e57 5f41 503a 2074 6f72 6368 2e54  lf.W_AP: torch.T
+00026720: 656e 736f 7220 3d20 696e 6974 280a 2020  ensor = init(.  
+00026730: 2020 2020 2020 2020 2020 2020 2020 746f                to
+00026740: 7263 682e 656d 7074 7928 7365 6c66 2e6e  rch.empty(self.n
+00026750: 5f61 746f 6d5f 696e 7075 745f 6665 6174  _atom_input_feat
+00026760: 202a 2032 2c20 7365 6c66 2e6e 5f68 6964   * 2, self.n_hid
+00026770: 6465 6e5f 4150 2929 0a20 2020 2020 2020  den_AP)).       
+00026780: 2020 2020 2073 656c 662e 625f 4150 3a20       self.b_AP: 
+00026790: 746f 7263 682e 5465 6e73 6f72 203d 2074  torch.Tensor = t
+000267a0: 6f72 6368 2e7a 6572 6f73 2828 7365 6c66  orch.zeros((self
+000267b0: 2e6e 5f68 6964 6465 6e5f 4150 2c29 290a  .n_hidden_AP,)).
+000267c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000267d0: 2e41 505f 626e 3a20 6e6e 2e42 6174 6368  .AP_bn: nn.Batch
+000267e0: 4e6f 726d 3164 203d 206e 6e2e 4261 7463  Norm1d = nn.Batc
+000267f0: 684e 6f72 6d31 6428 0a20 2020 2020 2020  hNorm1d(.       
+00026800: 2020 2020 2020 2020 206e 756d 5f66 6561           num_fea
+00026810: 7475 7265 733d 7365 6c66 2e6e 5f68 6964  tures=self.n_hid
+00026820: 6465 6e5f 4150 2c0a 2020 2020 2020 2020  den_AP,.        
+00026830: 2020 2020 2020 2020 6570 733d 3165 2d33          eps=1e-3
+00026840: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00026850: 2020 6d6f 6d65 6e74 756d 3d30 2e39 392c    momentum=0.99,
+00026860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00026870: 2061 6666 696e 653d 5472 7565 2c0a 2020   affine=True,.  
+00026880: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00026890: 6163 6b5f 7275 6e6e 696e 675f 7374 6174  ack_running_stat
+000268a0: 733d 5472 7565 290a 2020 2020 2020 2020  s=True).        
+000268b0: 2020 2020 2320 5765 6967 6874 206d 6174      # Weight mat
+000268c0: 7269 7820 616e 6420 6269 6173 206d 6174  rix and bias mat
+000268d0: 7269 7820 7265 7175 6972 6564 2074 6f20  rix required to 
+000268e0: 636f 6d70 7574 6520 6e65 7720 7061 6972  compute new pair
+000268f0: 206c 6179 6572 2066 726f 6d20 7468 6520   layer from the 
+00026900: 7072 6576 696f 7573 2070 6169 7220 6c61  previous pair la
+00026910: 7965 720a 2020 2020 2020 2020 2020 2020  yer.            
+00026920: 7365 6c66 2e57 5f50 503a 2074 6f72 6368  self.W_PP: torch
+00026930: 2e54 656e 736f 7220 3d20 696e 6974 280a  .Tensor = init(.
+00026940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026950: 746f 7263 682e 656d 7074 7928 7365 6c66  torch.empty(self
+00026960: 2e6e 5f70 6169 725f 696e 7075 745f 6665  .n_pair_input_fe
+00026970: 6174 2c20 7365 6c66 2e6e 5f68 6964 6465  at, self.n_hidde
+00026980: 6e5f 5050 2929 0a20 2020 2020 2020 2020  n_PP)).         
+00026990: 2020 2073 656c 662e 625f 5050 3a20 746f     self.b_PP: to
+000269a0: 7263 682e 5465 6e73 6f72 203d 2074 6f72  rch.Tensor = tor
+000269b0: 6368 2e7a 6572 6f73 2828 7365 6c66 2e6e  ch.zeros((self.n
+000269c0: 5f68 6964 6465 6e5f 5050 2c29 290a 2020  _hidden_PP,)).  
+000269d0: 2020 2020 2020 2020 2020 7365 6c66 2e50            self.P
+000269e0: 505f 626e 3a20 6e6e 2e42 6174 6368 4e6f  P_bn: nn.BatchNo
+000269f0: 726d 3164 203d 206e 6e2e 4261 7463 684e  rm1d = nn.BatchN
+00026a00: 6f72 6d31 6428 0a20 2020 2020 2020 2020  orm1d(.         
+00026a10: 2020 2020 2020 206e 756d 5f66 6561 7475         num_featu
+00026a20: 7265 733d 7365 6c66 2e6e 5f68 6964 6465  res=self.n_hidde
+00026a30: 6e5f 5050 2c0a 2020 2020 2020 2020 2020  n_PP,.          
+00026a40: 2020 2020 2020 6570 733d 3165 2d33 2c0a        eps=1e-3,.
+00026a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026a60: 6d6f 6d65 6e74 756d 3d30 2e39 392c 0a20  momentum=0.99,. 
+00026a70: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00026a80: 6666 696e 653d 5472 7565 2c0a 2020 2020  ffine=True,.    
+00026a90: 2020 2020 2020 2020 2020 2020 7472 6163              trac
+00026aa0: 6b5f 7275 6e6e 696e 675f 7374 6174 733d  k_running_stats=
+00026ab0: 5472 7565 290a 0a20 2020 2020 2020 2020  True)..         
+00026ac0: 2020 2073 656c 662e 575f 503a 2074 6f72     self.W_P: tor
+00026ad0: 6368 2e54 656e 736f 7220 3d20 696e 6974  ch.Tensor = init
+00026ae0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00026af0: 2020 746f 7263 682e 656d 7074 7928 7365    torch.empty(se
+00026b00: 6c66 2e6e 5f68 6964 6465 6e5f 502c 2073  lf.n_hidden_P, s
+00026b10: 656c 662e 6e5f 7061 6972 5f6f 7574 7075  elf.n_pair_outpu
+00026b20: 745f 6665 6174 2929 0a20 2020 2020 2020  t_feat)).       
+00026b30: 2020 2020 2073 656c 662e 625f 503a 2074       self.b_P: t
+00026b40: 6f72 6368 2e54 656e 736f 7220 3d20 746f  orch.Tensor = to
+00026b50: 7263 682e 7a65 726f 7328 2873 656c 662e  rch.zeros((self.
+00026b60: 6e5f 7061 6972 5f6f 7574 7075 745f 6665  n_pair_output_fe
+00026b70: 6174 2c29 290a 2020 2020 2020 2020 2020  at,)).          
+00026b80: 2020 7365 6c66 2e50 5f62 6e3a 206e 6e2e    self.P_bn: nn.
+00026b90: 4261 7463 684e 6f72 6d31 6420 3d20 6e6e  BatchNorm1d = nn
+00026ba0: 2e42 6174 6368 4e6f 726d 3164 280a 2020  .BatchNorm1d(.  
+00026bb0: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
+00026bc0: 6d5f 6665 6174 7572 6573 3d73 656c 662e  m_features=self.
+00026bd0: 6e5f 7061 6972 5f6f 7574 7075 745f 6665  n_pair_output_fe
+00026be0: 6174 2c0a 2020 2020 2020 2020 2020 2020  at,.            
+00026bf0: 2020 2020 6570 733d 3165 2d33 2c0a 2020      eps=1e-3,.  
+00026c00: 2020 2020 2020 2020 2020 2020 2020 6d6f                mo
+00026c10: 6d65 6e74 756d 3d30 2e39 392c 0a20 2020  mentum=0.99,.   
+00026c20: 2020 2020 2020 2020 2020 2020 2061 6666               aff
+00026c30: 696e 653d 5472 7565 2c0a 2020 2020 2020  ine=True,.      
+00026c40: 2020 2020 2020 2020 2020 7472 6163 6b5f            track_
+00026c50: 7275 6e6e 696e 675f 7374 6174 733d 5472  running_stats=Tr
+00026c60: 7565 290a 2020 2020 2020 2020 7365 6c66  ue).        self
+00026c70: 2e62 7569 6c74 203d 2054 7275 650a 0a20  .built = True.. 
+00026c80: 2020 2064 6566 205f 5f72 6570 725f 5f28     def __repr__(
+00026c90: 7365 6c66 2920 2d3e 2073 7472 3a0a 2020  self) -> str:.  
+00026ca0: 2020 2020 2020 2222 220a 2020 2020 5265        """.    Re
+00026cb0: 7475 726e 7320 6120 7374 7269 6e67 2072  turns a string r
+00026cc0: 6570 7265 7365 6e74 6174 696f 6e20 6f66  epresentation of
+00026cd0: 2074 6865 206f 626a 6563 742e 0a0a 2020   the object...  
+00026ce0: 2020 5265 7475 726e 733a 0a20 2020 202d    Returns:.    -
+00026cf0: 2d2d 2d2d 2d2d 0a20 2020 2073 7472 3a20  ------.    str: 
+00026d00: 4120 7374 7269 6e67 2074 6861 7420 636f  A string that co
+00026d10: 6e74 6169 6e73 2074 6865 2063 6c61 7373  ntains the class
+00026d20: 206e 616d 6520 666f 6c6c 6f77 6564 2062   name followed b
+00026d30: 7920 7468 6520 7661 6c75 6573 206f 6620  y the values of 
+00026d40: 6974 7320 696e 7374 616e 6365 2076 6172  its instance var
+00026d50: 6961 626c 652e 0a20 2020 2022 2222 0a20  iable..    """. 
+00026d60: 2020 2020 2020 2023 2066 6c61 6b65 383a         # flake8:
+00026d70: 206e 6f71 610a 2020 2020 2020 2020 7265   noqa.        re
+00026d80: 7475 726e 2028 0a20 2020 2020 2020 2020  turn (.         
+00026d90: 2020 2066 277b 7365 6c66 2e5f 5f63 6c61     f'{self.__cla
+00026da0: 7373 5f5f 2e5f 5f6e 616d 655f 5f7d 286e  ss__.__name__}(n
+00026db0: 5f61 746f 6d5f 696e 7075 745f 6665 6174  _atom_input_feat
+00026dc0: 3a7b 7365 6c66 2e6e 5f61 746f 6d5f 696e  :{self.n_atom_in
+00026dd0: 7075 745f 6665 6174 7d2c 6e5f 7061 6972  put_feat},n_pair
+00026de0: 5f69 6e70 7574 5f66 6561 743a 7b73 656c  _input_feat:{sel
+00026df0: 662e 6e5f 7061 6972 5f69 6e70 7574 5f66  f.n_pair_input_f
+00026e00: 6561 747d 2c6e 5f61 746f 6d5f 6f75 7470  eat},n_atom_outp
+00026e10: 7574 5f66 6561 743a 7b73 656c 662e 6e5f  ut_feat:{self.n_
+00026e20: 6174 6f6d 5f6f 7574 7075 745f 6665 6174  atom_output_feat
+00026e30: 7d2c 6e5f 7061 6972 5f6f 7574 7075 745f  },n_pair_output_
+00026e40: 6665 6174 3a7b 7365 6c66 2e6e 5f70 6169  feat:{self.n_pai
+00026e50: 725f 6f75 7470 7574 5f66 6561 747d 2c6e  r_output_feat},n
+00026e60: 5f68 6964 6465 6e5f 4141 3a7b 7365 6c66  _hidden_AA:{self
+00026e70: 2e6e 5f68 6964 6465 6e5f 4141 7d2c 6e5f  .n_hidden_AA},n_
+00026e80: 6869 6464 656e 5f50 413a 7b73 656c 662e  hidden_PA:{self.
+00026e90: 6e5f 6869 6464 656e 5f50 417d 2c6e 5f68  n_hidden_PA},n_h
+00026ea0: 6964 6465 6e5f 4150 3a7b 7365 6c66 2e6e  idden_AP:{self.n
+00026eb0: 5f68 6964 6465 6e5f 4150 7d2c 6e5f 6869  _hidden_AP},n_hi
+00026ec0: 6464 656e 5f50 503a 7b73 656c 662e 6e5f  dden_PP:{self.n_
+00026ed0: 6869 6464 656e 5f50 507d 2c62 6174 6368  hidden_PP},batch
+00026ee0: 5f6e 6f72 6d61 6c69 7a65 3a7b 7365 6c66  _normalize:{self
+00026ef0: 2e62 6174 6368 5f6e 6f72 6d61 6c69 7a65  .batch_normalize
+00026f00: 7d2c 7570 6461 7465 5f70 6169 723a 7b73  },update_pair:{s
+00026f10: 656c 662e 7570 6461 7465 5f70 6169 727d  elf.update_pair}
+00026f20: 2c69 6e69 743a 7b73 656c 662e 696e 6974  ,init:{self.init
+00026f30: 7d2c 6163 7469 7661 7469 6f6e 3a7b 7365  },activation:{se
+00026f40: 6c66 2e61 6374 6976 6174 696f 6e7d 2927  lf.activation})'
+00026f50: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00026f60: 6465 6620 666f 7277 6172 6428 0a20 2020  def forward(.   
+00026f70: 2020 2020 2073 656c 662c 2069 6e70 7574       self, input
+00026f80: 733a 204c 6973 745b 556e 696f 6e5b 6e70  s: List[Union[np
+00026f90: 2e6e 6461 7272 6179 2c20 6e70 2e6e 6461  .ndarray, np.nda
+00026fa0: 7272 6179 2c20 6e70 2e6e 6461 7272 6179  rray, np.ndarray
+00026fb0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00026fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026fd0: 2020 206e 702e 6e64 6172 7261 795d 5d0a     np.ndarray]].
+00026fe0: 2020 2020 2920 2d3e 204c 6973 745b 556e      ) -> List[Un
+00026ff0: 696f 6e5b 746f 7263 682e 5465 6e73 6f72  ion[torch.Tensor
+00027000: 2c20 746f 7263 682e 5465 6e73 6f72 5d5d  , torch.Tensor]]
+00027010: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00027020: 2020 4372 6561 7465 7320 7765 6176 6520    Creates weave 
+00027030: 7465 6e73 6f72 732e 0a0a 2020 2020 5061  tensors...    Pa
+00027040: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
+00027050: 2d2d 2d2d 2d2d 2d0a 2020 2020 696e 7075  -------.    inpu
+00027060: 7473 3a20 4c69 7374 5b55 6e69 6f6e 5b6e  ts: List[Union[n
+00027070: 702e 6e64 6172 7261 792c 206e 702e 6e64  p.ndarray, np.nd
+00027080: 6172 7261 792c 206e 702e 6e64 6172 7261  array, np.ndarra
+00027090: 792c 206e 702e 6e64 6172 7261 795d 5d0a  y, np.ndarray]].
+000270a0: 2020 2020 5368 6f75 6c64 2063 6f6e 7461      Should conta
+000270b0: 696e 2034 2074 656e 736f 7273 205b 6174  in 4 tensors [at
+000270c0: 6f6d 5f66 6561 7475 7265 732c 2070 6169  om_features, pai
+000270d0: 725f 6665 6174 7572 6573 2c20 7061 6972  r_features, pair
+000270e0: 5f73 706c 6974 2c0a 2020 2020 6174 6f6d  _split,.    atom
+000270f0: 5f74 6f5f 7061 6972 5d0a 0a20 2020 2052  _to_pair]..    R
+00027100: 6574 7572 6e73 3a0a 2020 2020 2d2d 2d2d  eturns:.    ----
+00027110: 2d2d 2d0a 2020 2020 4c69 7374 5b55 6e69  ---.    List[Uni
+00027120: 6f6e 5b74 6f72 6368 2e54 656e 736f 722c  on[torch.Tensor,
+00027130: 2074 6f72 6368 2e54 656e 736f 725d 5d0a   torch.Tensor]].
+00027140: 2020 2020 2020 413a 2041 746f 6d20 6665        A: Atom fe
+00027150: 6174 7572 6573 2074 656e 736f 7220 7769  atures tensor wi
+00027160: 7468 2073 6861 7065 5b74 6f74 616c 5f6e  th shape[total_n
+00027170: 756d 5f61 746f 6d73 2c61 746f 6d20 6665  um_atoms,atom fe
+00027180: 6174 7572 6520 7369 7a65 5d0a 2020 2020  ature size].    
+00027190: 2020 503a 2050 6169 7220 6665 6174 7572    P: Pair featur
+000271a0: 6573 2074 656e 736f 7220 7769 7468 2073  es tensor with s
+000271b0: 6861 7065 5b74 6f74 616c 206e 756d 206f  hape[total num o
+000271c0: 6620 7061 6972 732c 626f 6e64 2066 6561  f pairs,bond fea
+000271d0: 7475 7265 2073 697a 655d 0a20 2020 2022  ture size].    "
+000271e0: 2222 0a20 2020 2020 2020 2023 2043 6f6e  "".        # Con
+000271f0: 7665 7274 696e 6720 7468 6520 696e 7075  verting the inpu
+00027200: 7420 746f 2074 6f72 6368 2074 656e 736f  t to torch tenso
+00027210: 7273 0a20 2020 2020 2020 2061 746f 6d5f  rs.        atom_
+00027220: 6665 6174 7572 6573 3a20 746f 7263 682e  features: torch.
+00027230: 5465 6e73 6f72 203d 2074 6f72 6368 2e74  Tensor = torch.t
+00027240: 656e 736f 7228 696e 7075 7473 5b30 5d29  ensor(inputs[0])
+00027250: 0a20 2020 2020 2020 2070 6169 725f 6665  .        pair_fe
+00027260: 6174 7572 6573 3a20 746f 7263 682e 5465  atures: torch.Te
+00027270: 6e73 6f72 203d 2074 6f72 6368 2e74 656e  nsor = torch.ten
+00027280: 736f 7228 696e 7075 7473 5b31 5d29 0a0a  sor(inputs[1])..
+00027290: 2020 2020 2020 2020 7061 6972 5f73 706c          pair_spl
+000272a0: 6974 3a20 746f 7263 682e 5465 6e73 6f72  it: torch.Tensor
+000272b0: 203d 2074 6f72 6368 2e74 656e 736f 7228   = torch.tensor(
+000272c0: 696e 7075 7473 5b32 5d29 0a20 2020 2020  inputs[2]).     
+000272d0: 2020 2061 746f 6d5f 746f 5f70 6169 723a     atom_to_pair:
+000272e0: 2074 6f72 6368 2e54 656e 736f 7220 3d20   torch.Tensor = 
+000272f0: 746f 7263 682e 7465 6e73 6f72 2869 6e70  torch.tensor(inp
+00027300: 7574 735b 335d 290a 0a20 2020 2020 2020  uts[3])..       
+00027310: 2061 6374 6976 6174 696f 6e20 3d20 7365   activation = se
+00027320: 6c66 2e61 6374 6976 6174 696f 6e5f 666e  lf.activation_fn
+00027330: 0a0a 2020 2020 2020 2020 2320 4141 2069  ..        # AA i
+00027340: 7320 6120 7465 6e73 6f72 2077 6974 6820  s a tensor with 
+00027350: 7368 6170 655b 746f 7461 6c5f 6e75 6d5f  shape[total_num_
+00027360: 6174 6f6d 732c 6e5f 6869 6464 656e 5f41  atoms,n_hidden_A
+00027370: 415d 0a20 2020 2020 2020 2041 413a 2074  A].        AA: t
+00027380: 6f72 6368 2e54 656e 736f 7220 3d20 746f  orch.Tensor = to
+00027390: 7263 682e 6d61 746d 756c 2861 746f 6d5f  rch.matmul(atom_
+000273a0: 6665 6174 7572 6573 2e74 7970 6528 746f  features.type(to
+000273b0: 7263 682e 666c 6f61 7433 3229 2c0a 2020  rch.float32),.  
+000273c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000273d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000273e0: 2020 2020 2020 7365 6c66 2e57 5f41 4129        self.W_AA)
+000273f0: 202b 2073 656c 662e 625f 4141 0a20 2020   + self.b_AA.   
+00027400: 2020 2020 2069 6620 7365 6c66 2e62 6174       if self.bat
+00027410: 6368 5f6e 6f72 6d61 6c69 7a65 3a0a 2020  ch_normalize:.  
+00027420: 2020 2020 2020 2020 2020 7365 6c66 2e41            self.A
+00027430: 415f 626e 2e65 7661 6c28 290a 2020 2020  A_bn.eval().    
+00027440: 2020 2020 2020 2020 4141 203d 2073 656c          AA = sel
+00027450: 662e 4141 5f62 6e28 4141 290a 2020 2020  f.AA_bn(AA).    
+00027460: 2020 2020 4141 203d 2061 6374 6976 6174      AA = activat
+00027470: 696f 6e28 4141 290a 2020 2020 2020 2020  ion(AA).        
+00027480: 2320 5041 2069 7320 6120 7465 6e73 6f72  # PA is a tensor
+00027490: 2077 6974 6820 7368 6170 655b 746f 7461   with shape[tota
+000274a0: 6c20 6e75 6d62 6572 206f 6620 7061 6972  l number of pair
+000274b0: 732c 6e5f 6869 6464 656e 5f50 415d 0a20  s,n_hidden_PA]. 
+000274c0: 2020 2020 2020 2050 413a 2074 6f72 6368         PA: torch
+000274d0: 2e54 656e 736f 7220 3d20 746f 7263 682e  .Tensor = torch.
+000274e0: 6d61 746d 756c 2870 6169 725f 6665 6174  matmul(pair_feat
+000274f0: 7572 6573 2e74 7970 6528 746f 7263 682e  ures.type(torch.
+00027500: 666c 6f61 7433 3229 2c0a 2020 2020 2020  float32),.      
+00027510: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00027520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027530: 6163 7469 7661 7469 6f6e 3a20 7374 7220  activation: str 
-00027540: 3d20 2774 616e 6827 2c0a 2020 2020 2020  = 'tanh',.      
-00027550: 2020 2020 2020 2020 2020 202a 2a6b 7761             **kwa
-00027560: 7267 7329 3a0a 2020 2020 2020 2020 2222  rgs):.        ""
-00027570: 220a 2020 2020 2020 2020 5061 7261 6d65  ".        Parame
-00027580: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-00027590: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-000275a0: 6261 7463 685f 7369 7a65 3a20 696e 740a  batch_size: int.
-000275b0: 2020 2020 2020 2020 2020 2020 6e75 6d62              numb
-000275c0: 6572 206f 6620 6d6f 6c65 6375 6c65 7320  er of molecules 
-000275d0: 696e 2061 2062 6174 6368 0a20 2020 2020  in a batch.     
-000275e0: 2020 206e 5f69 6e70 7574 3a20 696e 742c     n_input: int,
-000275f0: 206f 7074 696f 6e61 6c20 2864 6566 6175   optional (defau
-00027600: 6c74 2031 3238 290a 2020 2020 2020 2020  lt 128).        
-00027610: 2020 2020 6e75 6d62 6572 206f 6620 6665      number of fe
-00027620: 6174 7572 6573 2066 6f72 2065 6163 6820  atures for each 
-00027630: 696e 7075 7420 6d6f 6c65 6375 6c65 0a20  input molecule. 
-00027640: 2020 2020 2020 2067 6175 7373 6961 6e5f         gaussian_
-00027650: 6578 7061 6e64 3a20 626f 6f6c 6561 6e2c  expand: boolean,
-00027660: 206f 7074 696f 6e61 6c20 2864 6566 6175   optional (defau
-00027670: 6c74 2054 7275 6529 0a20 2020 2020 2020  lt True).       
-00027680: 2020 2020 2057 6865 7468 6572 2074 6f20       Whether to 
-00027690: 6578 7061 6e64 2065 6163 6820 6469 6d65  expand each dime
-000276a0: 6e73 696f 6e20 6f66 2061 746f 6d69 6320  nsion of atomic 
-000276b0: 6665 6174 7572 6573 2062 7920 6761 7573  features by gaus
-000276c0: 7369 616e 2068 6973 746f 6772 616d 0a20  sian histogram. 
-000276d0: 2020 2020 2020 2063 6f6d 7072 6573 735f         compress_
-000276e0: 706f 7374 5f67 6175 7373 6961 6e5f 6578  post_gaussian_ex
-000276f0: 7061 6e73 696f 6e3a 2062 6f6f 6c2c 206f  pansion: bool, o
-00027700: 7074 696f 6e61 6c20 2864 6566 6175 6c74  ptional (default
-00027710: 2046 616c 7365 290a 2020 2020 2020 2020   False).        
-00027720: 2020 2020 4966 2054 7275 652c 2063 6f6d      If True, com
-00027730: 7072 6573 7320 7468 6520 7265 7375 6c74  press the result
-00027740: 7320 6f66 2074 6865 2047 6175 7373 6961  s of the Gaussia
-00027750: 6e20 6578 7061 6e73 696f 6e20 6261 636b  n expansion back
-00027760: 2074 6f20 7468 650a 2020 2020 2020 2020   to the.        
-00027770: 2020 2020 6f72 6967 696e 616c 2064 696d      original dim
-00027780: 656e 7369 6f6e 7320 6f66 2074 6865 2069  ensions of the i
-00027790: 6e70 7574 2062 7920 7573 696e 6720 6120  nput by using a 
-000277a0: 6c69 6e65 6172 206c 6179 6572 2077 6974  linear layer wit
-000277b0: 6820 7370 6563 6966 6965 640a 2020 2020  h specified.    
-000277c0: 2020 2020 2020 2020 6163 7469 7661 7469          activati
-000277d0: 6f6e 2066 756e 6374 696f 6e2e 204e 6f74  on function. Not
-000277e0: 6520 7468 6174 2074 6869 7320 636f 6d70  e that this comp
-000277f0: 7265 7373 696f 6e20 7761 7320 6e6f 7420  ression was not 
-00027800: 696e 2074 6865 206f 7269 6769 6e61 6c0a  in the original.
-00027810: 2020 2020 2020 2020 2020 2020 7061 7065              pape
-00027820: 722c 2062 7574 2077 6173 2070 7265 7365  r, but was prese
-00027830: 6e74 2069 6e20 7468 6520 6f72 6967 696e  nt in the origin
-00027840: 616c 2044 6565 7043 6865 6d20 696d 706c  al DeepChem impl
-00027850: 656d 656e 7461 7469 6f6e 2073 6f20 6973  ementation so is
-00027860: 0a20 2020 2020 2020 2020 2020 206c 6566  .            lef
-00027870: 7420 7072 6573 656e 7420 666f 7220 6261  t present for ba
-00027880: 636b 7761 7264 7320 636f 6d70 6174 6962  ckwards compatib
-00027890: 696c 6974 792e 0a20 2020 2020 2020 2069  ility..        i
-000278a0: 6e69 743a 2073 7472 2c20 6f70 7469 6f6e  nit: str, option
-000278b0: 616c 2028 6465 6661 756c 7420 2778 6176  al (default 'xav
-000278c0: 6965 725f 756e 6966 6f72 6d5f 2729 0a20  ier_uniform_'). 
-000278d0: 2020 2020 2020 2020 2020 2057 6569 6768             Weigh
-000278e0: 7420 696e 6974 6961 6c69 7a61 7469 6f6e  t initialization
-000278f0: 2066 6f72 2066 696c 7465 7273 2069 6620   for filters if 
-00027900: 6063 6f6d 7072 6573 735f 706f 7374 5f67  `compress_post_g
-00027910: 6175 7373 6961 6e5f 6578 7061 6e73 696f  aussian_expansio
-00027920: 6e60 0a20 2020 2020 2020 2020 2020 2069  n`.            i
-00027930: 7320 5472 7565 2e0a 2020 2020 2020 2020  s True..        
-00027940: 6163 7469 7661 7469 6f6e 3a20 7374 722c  activation: str,
-00027950: 206f 7074 696f 6e61 6c20 2864 6566 6175   optional (defau
-00027960: 6c74 2027 7461 6e68 2729 0a20 2020 2020  lt 'tanh').     
-00027970: 2020 2020 2020 2041 6374 6976 6174 696f         Activatio
-00027980: 6e20 6675 6e63 7469 6f6e 2061 7070 6c69  n function appli
-00027990: 6564 2066 6f72 2066 696c 7465 7273 2069  ed for filters i
-000279a0: 660a 2020 2020 2020 2020 2020 2020 6063  f.            `c
-000279b0: 6f6d 7072 6573 735f 706f 7374 5f67 6175  ompress_post_gau
-000279c0: 7373 6961 6e5f 6578 7061 6e73 696f 6e60  ssian_expansion`
-000279d0: 2069 7320 5472 7565 2e0a 2020 2020 2020   is True..      
-000279e0: 2020 2222 220a 2020 2020 2020 2020 7375    """.        su
-000279f0: 7065 7228 5765 6176 6547 6174 6865 722c  per(WeaveGather,
-00027a00: 2073 656c 6629 2e5f 5f69 6e69 745f 5f28   self).__init__(
-00027a10: 2a2a 6b77 6172 6773 290a 2020 2020 2020  **kwargs).      
-00027a20: 2020 7365 6c66 2e6e 5f69 6e70 7574 3a20    self.n_input: 
-00027a30: 696e 7420 3d20 6e5f 696e 7075 740a 2020  int = n_input.  
-00027a40: 2020 2020 2020 7365 6c66 2e62 6174 6368        self.batch
-00027a50: 5f73 697a 653a 2069 6e74 203d 2062 6174  _size: int = bat
-00027a60: 6368 5f73 697a 650a 2020 2020 2020 2020  ch_size.        
-00027a70: 7365 6c66 2e67 6175 7373 6961 6e5f 6578  self.gaussian_ex
-00027a80: 7061 6e64 3a20 626f 6f6c 203d 2067 6175  pand: bool = gau
-00027a90: 7373 6961 6e5f 6578 7061 6e64 0a20 2020  ssian_expand.   
-00027aa0: 2020 2020 2073 656c 662e 636f 6d70 7265       self.compre
-00027ab0: 7373 5f70 6f73 745f 6761 7573 7369 616e  ss_post_gaussian
-00027ac0: 5f65 7870 616e 7369 6f6e 3a20 626f 6f6c  _expansion: bool
-00027ad0: 203d 2063 6f6d 7072 6573 735f 706f 7374   = compress_post
-00027ae0: 5f67 6175 7373 6961 6e5f 6578 7061 6e73  _gaussian_expans
-00027af0: 696f 6e0a 2020 2020 2020 2020 7365 6c66  ion.        self
-00027b00: 2e69 6e69 743a 2073 7472 203d 2069 6e69  .init: str = ini
-00027b10: 745f 2020 2320 5365 7420 7765 6967 6874  t_  # Set weight
-00027b20: 2069 6e69 7469 616c 697a 6174 696f 6e0a   initialization.
-00027b30: 2020 2020 2020 2020 7365 6c66 2e61 6374          self.act
-00027b40: 6976 6174 696f 6e3a 2073 7472 203d 2061  ivation: str = a
-00027b50: 6374 6976 6174 696f 6e20 2023 2047 6574  ctivation  # Get
-00027b60: 2061 6374 6976 6174 696f 6e73 0a20 2020   activations.   
-00027b70: 2020 2020 2073 656c 662e 6163 7469 7661       self.activa
-00027b80: 7469 6f6e 5f66 6e3a 2074 6f72 6368 2e6e  tion_fn: torch.n
-00027b90: 6e2e 4d6f 6475 6c65 203d 2067 6574 5f61  n.Module = get_a
-00027ba0: 6374 6976 6174 696f 6e28 6163 7469 7661  ctivation(activa
-00027bb0: 7469 6f6e 290a 0a20 2020 2020 2020 2069  tion)..        i
-00027bc0: 6620 7365 6c66 2e63 6f6d 7072 6573 735f  f self.compress_
-00027bd0: 706f 7374 5f67 6175 7373 6961 6e5f 6578  post_gaussian_ex
-00027be0: 7061 6e73 696f 6e3a 0a20 2020 2020 2020  pansion:.       
-00027bf0: 2020 2020 2069 6e69 7420 3d20 6765 7461       init = geta
-00027c00: 7474 7228 696e 6974 6961 6c69 7a65 7273  ttr(initializers
-00027c10: 2c20 7365 6c66 2e69 6e69 7429 0a20 2020  , self.init).   
-00027c20: 2020 2020 2020 2020 2073 656c 662e 573a           self.W:
-00027c30: 2074 6f72 6368 2e54 656e 736f 7220 3d20   torch.Tensor = 
-00027c40: 696e 6974 280a 2020 2020 2020 2020 2020  init(.          
-00027c50: 2020 2020 2020 746f 7263 682e 656d 7074        torch.empt
-00027c60: 7928 5b73 656c 662e 6e5f 696e 7075 7420  y([self.n_input 
-00027c70: 2a20 3131 2c20 7365 6c66 2e6e 5f69 6e70  * 11, self.n_inp
-00027c80: 7574 5d29 290a 2020 2020 2020 2020 2020  ut])).          
-00027c90: 2020 7365 6c66 2e62 3a20 746f 7263 682e    self.b: torch.
-00027ca0: 5465 6e73 6f72 203d 2074 6f72 6368 2e7a  Tensor = torch.z
-00027cb0: 6572 6f73 2828 7365 6c66 2e6e 5f69 6e70  eros((self.n_inp
-00027cc0: 7574 2c29 290a 2020 2020 2020 2020 7365  ut,)).        se
-00027cd0: 6c66 2e62 7569 6c74 203d 2054 7275 650a  lf.built = True.
-00027ce0: 0a20 2020 2064 6566 205f 5f72 6570 725f  .    def __repr_
-00027cf0: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
-00027d00: 2022 2222 0a20 2020 2020 2020 2052 6574   """.        Ret
-00027d10: 7572 6e73 2061 2073 7472 696e 6720 7265  urns a string re
-00027d20: 7072 6573 656e 7461 7469 6f6e 206f 6620  presentation of 
-00027d30: 7468 6520 6f62 6a65 6374 2e0a 0a20 2020  the object...   
-00027d40: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00027d50: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
-00027d60: 2020 2020 2020 7374 723a 2041 2073 7472        str: A str
-00027d70: 696e 6720 7468 6174 2063 6f6e 7461 696e  ing that contain
-00027d80: 7320 7468 6520 636c 6173 7320 6e61 6d65  s the class name
-00027d90: 2066 6f6c 6c6f 7765 6420 6279 2074 6865   followed by the
-00027da0: 2076 616c 7565 7320 6f66 2069 7473 2069   values of its i
-00027db0: 6e73 7461 6e63 6520 7661 7269 6162 6c65  nstance variable
-00027dc0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00027dd0: 2020 2020 2020 7265 7475 726e 2028 0a20        return (. 
-00027de0: 2020 2020 2020 2020 2020 2066 277b 7365             f'{se
-00027df0: 6c66 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e  lf.__class__.__n
-00027e00: 616d 655f 5f7d 2862 6174 6368 5f73 697a  ame__}(batch_siz
-00027e10: 653a 7b73 656c 662e 6261 7463 685f 7369  e:{self.batch_si
-00027e20: 7a65 7d2c 6e5f 696e 7075 743a 7b73 656c  ze},n_input:{sel
-00027e30: 662e 6e5f 696e 7075 747d 2c67 6175 7373  f.n_input},gauss
-00027e40: 6961 6e5f 6578 7061 6e64 3a7b 7365 6c66  ian_expand:{self
-00027e50: 2e67 6175 7373 6961 6e5f 6578 7061 6e64  .gaussian_expand
-00027e60: 7d2c 696e 6974 3a7b 7365 6c66 2e69 6e69  },init:{self.ini
-00027e70: 747d 2c61 6374 6976 6174 696f 6e3a 7b73  t},activation:{s
-00027e80: 656c 662e 6163 7469 7661 7469 6f6e 7d2c  elf.activation},
-00027e90: 636f 6d70 7265 7373 5f70 6f73 745f 6761  compress_post_ga
-00027ea0: 7573 7369 616e 5f65 7870 616e 7369 6f6e  ussian_expansion
-00027eb0: 3a7b 7365 6c66 2e63 6f6d 7072 6573 735f  :{self.compress_
-00027ec0: 706f 7374 5f67 6175 7373 6961 6e5f 6578  post_gaussian_ex
-00027ed0: 7061 6e73 696f 6e7d 2927 0a20 2020 2020  pansion})'.     
-00027ee0: 2020 2029 0a0a 2020 2020 6465 6620 666f     )..    def fo
-00027ef0: 7277 6172 6428 7365 6c66 2c20 696e 7075  rward(self, inpu
-00027f00: 7473 3a20 4c69 7374 5b55 6e69 6f6e 5b6e  ts: List[Union[n
-00027f10: 702e 6e64 6172 7261 792c 0a20 2020 2020  p.ndarray,.     
-00027f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027f40: 2020 2020 6e70 2e6e 6461 7272 6179 5d5d      np.ndarray]]
-00027f50: 2920 2d3e 2074 6f72 6368 2e54 656e 736f  ) -> torch.Tenso
-00027f60: 723a 0a20 2020 2020 2020 2022 2222 4372  r:.        """Cr
-00027f70: 6561 7465 7320 7765 6176 6520 7465 6e73  eates weave tens
-00027f80: 6f72 732e 0a0a 2020 2020 2020 2020 5061  ors...        Pa
-00027f90: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-00027fa0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00027fb0: 2020 2020 696e 7075 7473 3a20 4c69 7374      inputs: List
-00027fc0: 5b55 6e69 6f6e 5b6e 702e 6e64 6172 7261  [Union[np.ndarra
-00027fd0: 792c 6e70 2e6e 6461 7272 6179 5d5d 0a20  y,np.ndarray]]. 
-00027fe0: 2020 2020 2020 2020 2020 2053 686f 756c             Shoul
-00027ff0: 6420 636f 6e74 6169 6e20 3220 7465 6e73  d contain 2 tens
-00028000: 6f72 7320 5b61 746f 6d5f 6665 6174 7572  ors [atom_featur
-00028010: 6573 2c20 6174 6f6d 5f73 706c 6974 5d0a  es, atom_split].
-00028020: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00028030: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00028040: 0a20 2020 2020 2020 206f 7574 7075 745f  .        output_
-00028050: 6d6f 6c65 6375 6c65 733a 2074 6f72 6368  molecules: torch
-00028060: 2e54 656e 736f 720a 2020 2020 2020 2020  .Tensor.        
-00028070: 2020 2020 4561 6368 2065 6e74 7279 2069      Each entry i
-00028080: 6e20 7468 6973 206c 6973 7420 6973 206f  n this list is o
-00028090: 6620 7368 6170 6520 6028 7365 6c66 2e6e  f shape `(self.n
-000280a0: 5f69 6e70 7574 732c 2960 0a0a 2020 2020  _inputs,)`..    
-000280b0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000280c0: 6f75 7470 7574 733a 2074 6f72 6368 2e54  outputs: torch.T
-000280d0: 656e 736f 7220 3d20 746f 7263 682e 7465  ensor = torch.te
-000280e0: 6e73 6f72 2869 6e70 7574 735b 305d 290a  nsor(inputs[0]).
-000280f0: 2020 2020 2020 2020 6174 6f6d 5f73 706c          atom_spl
-00028100: 6974 3a20 746f 7263 682e 5465 6e73 6f72  it: torch.Tensor
-00028110: 203d 2074 6f72 6368 2e74 656e 736f 7228   = torch.tensor(
-00028120: 696e 7075 7473 5b31 5d29 0a0a 2020 2020  inputs[1])..    
-00028130: 2020 2020 6966 2073 656c 662e 6761 7573      if self.gaus
-00028140: 7369 616e 5f65 7870 616e 643a 0a20 2020  sian_expand:.   
-00028150: 2020 2020 2020 2020 206f 7574 7075 7473           outputs
-00028160: 203d 2073 656c 662e 6761 7573 7369 616e   = self.gaussian
-00028170: 5f68 6973 746f 6772 616d 286f 7574 7075  _histogram(outpu
-00028180: 7473 290a 0a20 2020 2020 2020 2074 5f67  ts)..        t_g
-00028190: 7270 3a20 4469 6374 5b54 656e 736f 722c  rp: Dict[Tensor,
-000281a0: 2054 656e 736f 725d 203d 207b 7d0a 2020   Tensor] = {}.  
-000281b0: 2020 2020 2020 6964 783a 2069 6e74 203d        idx: int =
-000281c0: 2030 0a20 2020 2020 2020 2066 6f72 2069   0.        for i
-000281d0: 2c20 735f 6964 2069 6e20 656e 756d 6572  , s_id in enumer
-000281e0: 6174 6528 6174 6f6d 5f73 706c 6974 293a  ate(atom_split):
-000281f0: 0a20 2020 2020 2020 2020 2020 2073 5f69  .            s_i
-00028200: 6420 3d20 735f 6964 2e69 7465 6d28 290a  d = s_id.item().
-00028210: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00028220: 5f69 6420 696e 2074 5f67 7270 3a0a 2020  _id in t_grp:.  
-00028230: 2020 2020 2020 2020 2020 2020 2020 745f                t_
-00028240: 6772 705b 735f 6964 5d20 3d20 745f 6772  grp[s_id] = t_gr
-00028250: 705b 735f 6964 5d20 2b20 6f75 7470 7574  p[s_id] + output
-00028260: 735b 6964 785d 0a20 2020 2020 2020 2020  s[idx].         
-00028270: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00028280: 2020 2020 2020 2020 2074 5f67 7270 5b73           t_grp[s
-00028290: 5f69 645d 203d 206f 7574 7075 7473 5b69  _id] = outputs[i
-000282a0: 6478 5d0a 2020 2020 2020 2020 2020 2020  dx].            
-000282b0: 6964 7820 3d20 6920 2b20 310a 0a20 2020  idx = i + 1..   
-000282c0: 2020 2020 2020 2020 206c 7374 203d 206c           lst = l
-000282d0: 6973 7428 745f 6772 702e 7661 6c75 6573  ist(t_grp.values
-000282e0: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
-000282f0: 7465 6e73 6f72 203d 2074 6f72 6368 2e73  tensor = torch.s
-00028300: 7461 636b 286c 7374 290a 2020 2020 2020  tack(lst).      
-00028310: 2020 6f75 7470 7574 5f6d 6f6c 6563 756c    output_molecul
-00028320: 6573 3a20 746f 7263 682e 5465 6e73 6f72  es: torch.Tensor
-00028330: 203d 2074 656e 736f 720a 0a20 2020 2020   = tensor..     
-00028340: 2020 2069 6620 7365 6c66 2e63 6f6d 7072     if self.compr
-00028350: 6573 735f 706f 7374 5f67 6175 7373 6961  ess_post_gaussia
-00028360: 6e5f 6578 7061 6e73 696f 6e3a 0a20 2020  n_expansion:.   
-00028370: 2020 2020 2020 2020 206f 7574 7075 745f           output_
-00028380: 6d6f 6c65 6375 6c65 7320 3d20 746f 7263  molecules = torc
-00028390: 682e 6d61 746d 756c 280a 2020 2020 2020  h.matmul(.      
-000283a0: 2020 2020 2020 2020 2020 6f75 7470 7574            output
-000283b0: 5f6d 6f6c 6563 756c 6573 2e74 7970 6528  _molecules.type(
-000283c0: 746f 7263 682e 666c 6f61 7433 3229 2c20  torch.float32), 
-000283d0: 7365 6c66 2e57 2920 2b20 7365 6c66 2e62  self.W) + self.b
-000283e0: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
-000283f0: 7075 745f 6d6f 6c65 6375 6c65 7320 3d20  put_molecules = 
-00028400: 7365 6c66 2e61 6374 6976 6174 696f 6e5f  self.activation_
-00028410: 666e 286f 7574 7075 745f 6d6f 6c65 6375  fn(output_molecu
-00028420: 6c65 7329 0a0a 2020 2020 2020 2020 7265  les)..        re
-00028430: 7475 726e 206f 7574 7075 745f 6d6f 6c65  turn output_mole
-00028440: 6375 6c65 730a 0a20 2020 2064 6566 2067  cules..    def g
-00028450: 6175 7373 6961 6e5f 6869 7374 6f67 7261  aussian_histogra
-00028460: 6d28 7365 6c66 2c20 783a 2074 6f72 6368  m(self, x: torch
-00028470: 2e54 656e 736f 7229 202d 3e20 746f 7263  .Tensor) -> torc
-00028480: 682e 5465 6e73 6f72 3a0a 2020 2020 2020  h.Tensor:.      
-00028490: 2020 2222 2245 7870 616e 6473 2069 6e70    """Expands inp
-000284a0: 7574 2069 6e74 6f20 6120 7365 7420 6f66  ut into a set of
-000284b0: 2067 6175 7373 6961 6e20 6869 7374 6f67   gaussian histog
-000284c0: 7261 6d20 6269 6e73 2e0a 0a20 2020 2020  ram bins...     
-000284d0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-000284e0: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-000284f0: 0a20 2020 2020 2020 2078 3a20 746f 7263  .        x: torc
-00028500: 682e 5465 6e73 6f72 0a20 2020 2020 2020  h.Tensor.       
-00028510: 2020 2020 204f 6620 7368 6170 6520 6028       Of shape `(
-00028520: 4e2c 206e 5f66 6561 7429 600a 0a20 2020  N, n_feat)`..   
-00028530: 2020 2020 2045 7861 6d70 6c65 730a 2020       Examples.  
-00028540: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20        --------. 
-00028550: 2020 2020 2020 2054 6869 7320 6d65 7468         This meth
-00028560: 6f64 2075 7365 7320 3131 2062 696e 7320  od uses 11 bins 
-00028570: 7370 616e 6e69 6e67 2070 6f72 7469 6f6e  spanning portion
-00028580: 7320 6f66 2061 2047 6175 7373 6961 6e20  s of a Gaussian 
-00028590: 7769 7468 207a 6572 6f20 6d65 616e 0a20  with zero mean. 
-000285a0: 2020 2020 2020 2061 6e64 2075 6e69 7420         and unit 
-000285b0: 7374 616e 6461 7264 2064 6576 6961 7469  standard deviati
-000285c0: 6f6e 2e0a 0a20 2020 2020 2020 203e 3e3e  on...        >>>
-000285d0: 2067 6175 7373 6961 6e5f 6d65 6d62 6572   gaussian_member
-000285e0: 7368 6970 7320 3d20 5b28 2d31 2e36 3435  ships = [(-1.645
-000285f0: 2c20 302e 3238 3329 2c20 282d 312e 3038  , 0.283), (-1.08
-00028600: 302c 2030 2e31 3730 292c 0a20 2020 2020  0, 0.170),.     
-00028610: 2020 202e 2e2e 2020 2020 2020 2020 2020     ...          
-00028620: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-00028630: 2d30 2e37 3339 2c20 302e 3133 3429 2c20  -0.739, 0.134), 
-00028640: 282d 302e 3436 382c 2030 2e31 3138 292c  (-0.468, 0.118),
-00028650: 0a20 2020 2020 2020 202e 2e2e 2020 2020  .        ...    
-00028660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028670: 2020 2020 2028 2d30 2e32 3238 2c20 302e       (-0.228, 0.
-00028680: 3131 3429 2c20 2830 2e2c 2030 2e31 3134  114), (0., 0.114
-00028690: 292c 0a20 2020 2020 2020 202e 2e2e 2020  ),.        ...  
-000286a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000286b0: 2020 2020 2020 2028 302e 3232 382c 2030         (0.228, 0
-000286c0: 2e31 3134 292c 2028 302e 3436 382c 2030  .114), (0.468, 0
-000286d0: 2e31 3138 292c 0a20 2020 2020 2020 202e  .118),.        .
-000286e0: 2e2e 2020 2020 2020 2020 2020 2020 2020  ..              
-000286f0: 2020 2020 2020 2020 2020 2028 302e 3733             (0.73
-00028700: 392c 2030 2e31 3334 292c 2028 312e 3038  9, 0.134), (1.08
-00028710: 302c 2030 2e31 3730 292c 0a20 2020 2020  0, 0.170),.     
-00028720: 2020 202e 2e2e 2020 2020 2020 2020 2020     ...          
-00028730: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-00028740: 312e 3634 352c 2030 2e32 3833 295d 0a0a  1.645, 0.283)]..
-00028750: 2020 2020 2020 2020 5765 2063 6f6e 7374          We const
-00028760: 7275 6374 2061 2047 6175 7373 6961 6e20  ruct a Gaussian 
-00028770: 6174 2060 6761 7573 7369 616e 5f6d 656d  at `gaussian_mem
-00028780: 6265 7273 6869 7073 5b69 5d5b 305d 6020  berships[i][0]` 
-00028790: 7769 7468 2073 7461 6e64 6172 640a 2020  with standard.  
-000287a0: 2020 2020 2020 6465 7669 6174 696f 6e20        deviation 
-000287b0: 6067 6175 7373 6961 6e5f 6d65 6d62 6572  `gaussian_member
-000287c0: 7368 6970 735b 695d 5b31 5d60 2e20 4561  ships[i][1]`. Ea
-000287d0: 6368 2066 6561 7475 7265 2069 6e20 6078  ch feature in `x
-000287e0: 6020 6973 2061 7373 6967 6e65 640a 2020  ` is assigned.  
-000287f0: 2020 2020 2020 7468 6520 7072 6f62 6162        the probab
-00028800: 696c 6974 7920 6f66 2066 616c 6c69 6e67  ility of falling
-00028810: 2069 6e20 6561 6368 2047 6175 7373 6961   in each Gaussia
-00028820: 6e2c 2061 6e64 2070 726f 6261 6269 6c69  n, and probabili
-00028830: 7469 6573 2061 7265 0a20 2020 2020 2020  ties are.       
-00028840: 206e 6f72 6d61 6c69 7a65 6420 6163 726f   normalized acro
-00028850: 7373 2074 6865 2031 3120 6469 6666 6572  ss the 11 differ
-00028860: 656e 7420 4761 7573 7369 616e 732e 0a0a  ent Gaussians...
-00028870: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-00028880: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-00028890: 2020 2020 2020 2020 6f75 7470 7574 733a          outputs:
-000288a0: 2074 6f72 6368 2e54 656e 736f 720a 2020   torch.Tensor.  
-000288b0: 2020 2020 2020 2020 2020 4f66 2073 6861            Of sha
-000288c0: 7065 2060 284e 2c20 3131 2a6e 5f66 6561  pe `(N, 11*n_fea
-000288d0: 7429 600a 2020 2020 2020 2020 2222 220a  t)`.        """.
-000288e0: 2020 2020 2020 2020 696d 706f 7274 2074          import t
-000288f0: 6f72 6368 2e64 6973 7472 6962 7574 696f  orch.distributio
-00028900: 6e73 2061 7320 6469 7374 0a20 2020 2020  ns as dist.     
-00028910: 2020 2067 6175 7373 6961 6e5f 6d65 6d62     gaussian_memb
-00028920: 6572 7368 6970 733a 204c 6973 745b 5475  erships: List[Tu
-00028930: 706c 655b 666c 6f61 742c 2066 6c6f 6174  ple[float, float
-00028940: 5d5d 203d 205b 282d 312e 3634 352c 2030  ]] = [(-1.645, 0
-00028950: 2e32 3833 292c 0a20 2020 2020 2020 2020  .283),.         
-00028960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028990: 2020 282d 312e 3038 302c 2030 2e31 3730    (-1.080, 0.170
-000289a0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-000289b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000289c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000289d0: 2020 2020 2020 2020 2020 2020 2020 282d                (-
-000289e0: 302e 3733 392c 2030 2e31 3334 292c 0a20  0.739, 0.134),. 
-000289f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028a20: 2020 2020 2020 2020 2020 282d 302e 3436            (-0.46
-00028a30: 382c 2030 2e31 3138 292c 0a20 2020 2020  8, 0.118),.     
-00028a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028a70: 2020 2020 2020 282d 302e 3232 382c 2030        (-0.228, 0
-00028a80: 2e31 3134 292c 0a20 2020 2020 2020 2020  .114),.         
-00028a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028ac0: 2020 2830 2e2c 2030 2e31 3134 292c 0a20    (0., 0.114),. 
-00028ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028b00: 2020 2020 2020 2020 2020 2830 2e32 3238            (0.228
-00028b10: 2c20 302e 3131 3429 2c0a 2020 2020 2020  , 0.114),.      
-00028b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028b50: 2020 2020 2028 302e 3436 382c 2030 2e31       (0.468, 0.1
-00028b60: 3138 292c 0a20 2020 2020 2020 2020 2020  18),.           
-00028b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028ba0: 2830 2e37 3339 2c20 302e 3133 3429 2c0a  (0.739, 0.134),.
-00028bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028be0: 2020 2020 2020 2020 2020 2028 312e 3038             (1.08
-00028bf0: 302c 2030 2e31 3730 292c 0a20 2020 2020  0, 0.170),.     
-00028c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028c30: 2020 2020 2020 2831 2e36 3435 2c20 302e        (1.645, 0.
-00028c40: 3238 3329 5d0a 0a20 2020 2020 2020 2064  283)]..        d
-00028c50: 6973 7472 6962 7574 696f 6e73 3a20 4c69  istributions: Li
-00028c60: 7374 5b64 6973 742e 4e6f 726d 616c 5d20  st[dist.Normal] 
-00028c70: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
-00028c80: 6469 7374 2e4e 6f72 6d61 6c28 746f 7263  dist.Normal(torc
-00028c90: 682e 7465 6e73 6f72 2870 5b30 5d29 2c20  h.tensor(p[0]), 
-00028ca0: 746f 7263 682e 7465 6e73 6f72 2870 5b31  torch.tensor(p[1
-00028cb0: 5d29 290a 2020 2020 2020 2020 2020 2020  ])).            
-00028cc0: 666f 7220 7020 696e 2067 6175 7373 6961  for p in gaussia
-00028cd0: 6e5f 6d65 6d62 6572 7368 6970 730a 2020  n_memberships.  
-00028ce0: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
-00028cf0: 6469 7374 5f6d 6178 3a20 4c69 7374 5b74  dist_max: List[t
-00028d00: 6f72 6368 2e54 656e 736f 725d 203d 205b  orch.Tensor] = [
-00028d10: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
-00028d20: 7472 6962 7574 696f 6e73 5b69 5d2e 6c6f  tributions[i].lo
-00028d30: 675f 7072 6f62 2874 6f72 6368 2e74 656e  g_prob(torch.ten
-00028d40: 736f 7228 0a20 2020 2020 2020 2020 2020  sor(.           
-00028d50: 2020 2020 2067 6175 7373 6961 6e5f 6d65       gaussian_me
-00028d60: 6d62 6572 7368 6970 735b 695d 5b30 5d29  mberships[i][0])
-00028d70: 292e 6578 7028 2920 666f 7220 6920 696e  ).exp() for i in
-00028d80: 2072 616e 6765 2831 3129 0a20 2020 2020   range(11).     
-00028d90: 2020 205d 0a0a 2020 2020 2020 2020 6f75     ]..        ou
-00028da0: 7470 7574 733a 204c 6973 745b 746f 7263  tputs: List[torc
-00028db0: 682e 5465 6e73 6f72 5d20 3d20 5b0a 2020  h.Tensor] = [.  
-00028dc0: 2020 2020 2020 2020 2020 6469 7374 7269            distri
-00028dd0: 6275 7469 6f6e 735b 695d 2e6c 6f67 5f70  butions[i].log_p
-00028de0: 726f 6228 746f 7263 682e 7465 6e73 6f72  rob(torch.tensor
-00028df0: 2878 2929 2e65 7870 2829 202f 2064 6973  (x)).exp() / dis
-00028e00: 745f 6d61 785b 695d 0a20 2020 2020 2020  t_max[i].       
-00028e10: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-00028e20: 6e67 6528 3131 290a 2020 2020 2020 2020  nge(11).        
-00028e30: 5d0a 2020 2020 2020 2020 6f75 7470 7574  ].        output
-00028e40: 3a20 746f 7263 682e 5465 6e73 6f72 203d  : torch.Tensor =
-00028e50: 2074 6f72 6368 2e73 7461 636b 286f 7574   torch.stack(out
-00028e60: 7075 7473 2c20 6469 6d3d 3229 0a20 2020  puts, dim=2).   
-00028e70: 2020 2020 206f 7574 7075 7420 3d20 6f75       output = ou
-00028e80: 7470 7574 202f 2074 6f72 6368 2e73 756d  tput / torch.sum
-00028e90: 286f 7574 7075 742c 2064 696d 3d32 2c20  (output, dim=2, 
-00028ea0: 6b65 6570 6469 6d3d 5472 7565 290a 2020  keepdim=True).  
-00028eb0: 2020 2020 2020 6f75 7470 7574 203d 206f        output = o
-00028ec0: 7574 7075 742e 7669 6577 282d 312c 2073  utput.view(-1, s
-00028ed0: 656c 662e 6e5f 696e 7075 7420 2a20 3131  elf.n_input * 11
-00028ee0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00028ef0: 206f 7574 7075 740a                       output.
+00027530: 2020 7365 6c66 2e57 5f50 4129 202b 2073    self.W_PA) + s
+00027540: 656c 662e 625f 5041 0a20 2020 2020 2020  elf.b_PA.       
+00027550: 2069 6620 7365 6c66 2e62 6174 6368 5f6e   if self.batch_n
+00027560: 6f72 6d61 6c69 7a65 3a0a 2020 2020 2020  ormalize:.      
+00027570: 2020 2020 2020 7365 6c66 2e50 415f 626e        self.PA_bn
+00027580: 2e65 7661 6c28 290a 2020 2020 2020 2020  .eval().        
+00027590: 2020 2020 5041 203d 2073 656c 662e 5041      PA = self.PA
+000275a0: 5f62 6e28 5041 290a 2020 2020 2020 2020  _bn(PA).        
+000275b0: 5041 203d 2061 6374 6976 6174 696f 6e28  PA = activation(
+000275c0: 5041 290a 0a20 2020 2020 2020 2023 2053  PA)..        # S
+000275d0: 706c 6974 2074 6865 2050 4120 7465 6e73  plit the PA tens
+000275e0: 6f72 2061 6363 6f72 6469 6e67 2074 6f20  or according to 
+000275f0: 7468 6520 2770 6169 725f 7370 6c69 7427  the 'pair_split'
+00027600: 2074 656e 736f 720a 2020 2020 2020 2020   tensor.        
+00027610: 745f 6772 703a 2044 6963 745b 5465 6e73  t_grp: Dict[Tens
+00027620: 6f72 2c20 5465 6e73 6f72 5d20 3d20 7b7d  or, Tensor] = {}
+00027630: 0a20 2020 2020 2020 2069 6478 3a20 696e  .        idx: in
+00027640: 7420 3d20 300a 2020 2020 2020 2020 666f  t = 0.        fo
+00027650: 7220 692c 2073 5f69 6420 696e 2065 6e75  r i, s_id in enu
+00027660: 6d65 7261 7465 2870 6169 725f 7370 6c69  merate(pair_spli
+00027670: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+00027680: 735f 6964 203d 2073 5f69 642e 6974 656d  s_id = s_id.item
+00027690: 2829 0a20 2020 2020 2020 2020 2020 2069  ().            i
+000276a0: 6620 735f 6964 2069 6e20 745f 6772 703a  f s_id in t_grp:
+000276b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000276c0: 2074 5f67 7270 5b73 5f69 645d 203d 2074   t_grp[s_id] = t
+000276d0: 5f67 7270 5b73 5f69 645d 202b 2050 415b  _grp[s_id] + PA[
+000276e0: 6964 785d 0a20 2020 2020 2020 2020 2020  idx].           
+000276f0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00027700: 2020 2020 2020 2074 5f67 7270 5b73 5f69         t_grp[s_i
+00027710: 645d 203d 2050 415b 6964 785d 0a20 2020  d] = PA[idx].   
+00027720: 2020 2020 2020 2020 2069 6478 203d 2069           idx = i
+00027730: 202b 2031 0a0a 2020 2020 2020 2020 2020   + 1..          
+00027740: 2020 6c73 7420 3d20 6c69 7374 2874 5f67    lst = list(t_g
+00027750: 7270 2e76 616c 7565 7328 2929 0a20 2020  rp.values()).   
+00027760: 2020 2020 2020 2020 2074 656e 736f 7220           tensor 
+00027770: 3d20 746f 7263 682e 7374 6163 6b28 6c73  = torch.stack(ls
+00027780: 7429 0a20 2020 2020 2020 2050 4120 3d20  t).        PA = 
+00027790: 7465 6e73 6f72 0a0a 2020 2020 2020 2020  tensor..        
+000277a0: 413a 2074 6f72 6368 2e54 656e 736f 7220  A: torch.Tensor 
+000277b0: 3d20 746f 7263 682e 6d61 746d 756c 2874  = torch.matmul(t
+000277c0: 6f72 6368 2e63 6f6e 6361 7428 5b41 412c  orch.concat([AA,
+000277d0: 2050 415d 2c20 3129 2c0a 2020 2020 2020   PA], 1),.      
+000277e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000277f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027800: 2073 656c 662e 575f 4129 202b 2073 656c   self.W_A) + sel
+00027810: 662e 625f 410a 2020 2020 2020 2020 6966  f.b_A.        if
+00027820: 2073 656c 662e 6261 7463 685f 6e6f 726d   self.batch_norm
+00027830: 616c 697a 653a 0a20 2020 2020 2020 2020  alize:.         
+00027840: 2020 2073 656c 662e 415f 626e 2e65 7661     self.A_bn.eva
+00027850: 6c28 290a 2020 2020 2020 2020 2020 2020  l().            
+00027860: 4120 3d20 7365 6c66 2e41 5f62 6e28 4129  A = self.A_bn(A)
+00027870: 0a20 2020 2020 2020 2041 203d 2061 6374  .        A = act
+00027880: 6976 6174 696f 6e28 4129 0a0a 2020 2020  ivation(A)..    
+00027890: 2020 2020 6966 2073 656c 662e 7570 6461      if self.upda
+000278a0: 7465 5f70 6169 723a 0a20 2020 2020 2020  te_pair:.       
+000278b0: 2020 2020 2023 204e 6f74 6520 7468 6174       # Note that
+000278c0: 2041 505f 696a 2061 6e64 2041 505f 6a69   AP_ij and AP_ji
+000278d0: 2073 6861 7265 2074 6865 2073 616d 6520   share the same 
+000278e0: 7365 6c66 2e41 505f 626e 2062 6174 6368  self.AP_bn batch
+000278f0: 0a20 2020 2020 2020 2020 2020 2023 206e  .            # n
+00027900: 6f72 6d61 6c69 7a61 7469 6f6e 0a20 2020  ormalization.   
+00027910: 2020 2020 2020 2020 2041 505f 696a 3a20           AP_ij: 
+00027920: 746f 7263 682e 5465 6e73 6f72 203d 2074  torch.Tensor = t
+00027930: 6f72 6368 2e6d 6174 6d75 6c28 0a20 2020  orch.matmul(.   
+00027940: 2020 2020 2020 2020 2020 2020 2074 6f72               tor
+00027950: 6368 2e72 6573 6861 7065 2861 746f 6d5f  ch.reshape(atom_
+00027960: 6665 6174 7572 6573 5b61 746f 6d5f 746f  features[atom_to
+00027970: 5f70 6169 725d 2c0a 2020 2020 2020 2020  _pair],.        
+00027980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027990: 2020 2020 2020 5b2d 312c 2032 202a 2073        [-1, 2 * s
+000279a0: 656c 662e 6e5f 6174 6f6d 5f69 6e70 7574  elf.n_atom_input
+000279b0: 5f66 6561 745d 292e 7479 7065 280a 2020  _feat]).type(.  
+000279c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000279d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000279e0: 746f 7263 682e 666c 6f61 7433 3229 2c20  torch.float32), 
+000279f0: 7365 6c66 2e57 5f41 5029 202b 2073 656c  self.W_AP) + sel
+00027a00: 662e 625f 4150 0a20 2020 2020 2020 2020  f.b_AP.         
+00027a10: 2020 2069 6620 7365 6c66 2e62 6174 6368     if self.batch
+00027a20: 5f6e 6f72 6d61 6c69 7a65 3a0a 2020 2020  _normalize:.    
+00027a30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00027a40: 2e41 505f 626e 2e65 7661 6c28 290a 2020  .AP_bn.eval().  
+00027a50: 2020 2020 2020 2020 2020 2020 2020 4150                AP
+00027a60: 5f69 6a20 3d20 7365 6c66 2e41 505f 626e  _ij = self.AP_bn
+00027a70: 2841 505f 696a 290a 2020 2020 2020 2020  (AP_ij).        
+00027a80: 2020 2020 4150 5f69 6a20 3d20 6163 7469      AP_ij = acti
+00027a90: 7661 7469 6f6e 2841 505f 696a 290a 2020  vation(AP_ij).  
+00027aa0: 2020 2020 2020 2020 2020 4150 5f6a 693a            AP_ji:
+00027ab0: 2074 6f72 6368 2e54 656e 736f 7220 3d20   torch.Tensor = 
+00027ac0: 746f 7263 682e 6d61 746d 756c 280a 2020  torch.matmul(.  
+00027ad0: 2020 2020 2020 2020 2020 2020 2020 746f                to
+00027ae0: 7263 682e 7265 7368 6170 6528 6174 6f6d  rch.reshape(atom
+00027af0: 5f66 6561 7475 7265 735b 746f 7263 682e  _features[torch.
+00027b00: 666c 6970 2861 746f 6d5f 746f 5f70 6169  flip(atom_to_pai
+00027b10: 722c 205b 315d 295d 2c0a 2020 2020 2020  r, [1])],.      
+00027b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027b30: 2020 2020 2020 2020 5b2d 312c 2032 202a          [-1, 2 *
+00027b40: 2073 656c 662e 6e5f 6174 6f6d 5f69 6e70   self.n_atom_inp
+00027b50: 7574 5f66 6561 745d 292e 7479 7065 280a  ut_feat]).type(.
+00027b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027b80: 2020 746f 7263 682e 666c 6f61 7433 3229    torch.float32)
+00027b90: 2c20 7365 6c66 2e57 5f41 5029 202b 2073  , self.W_AP) + s
+00027ba0: 656c 662e 625f 4150 0a20 2020 2020 2020  elf.b_AP.       
+00027bb0: 2020 2020 2069 6620 7365 6c66 2e62 6174       if self.bat
+00027bc0: 6368 5f6e 6f72 6d61 6c69 7a65 3a0a 2020  ch_normalize:.  
+00027bd0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00027be0: 6c66 2e41 505f 626e 2e65 7661 6c28 290a  lf.AP_bn.eval().
+00027bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027c00: 4150 5f6a 6920 3d20 7365 6c66 2e41 505f  AP_ji = self.AP_
+00027c10: 626e 2841 505f 6a69 290a 2020 2020 2020  bn(AP_ji).      
+00027c20: 2020 2020 2020 4150 5f6a 6920 3d20 6163        AP_ji = ac
+00027c30: 7469 7661 7469 6f6e 2841 505f 6a69 290a  tivation(AP_ji).
+00027c40: 2020 2020 2020 2020 2020 2020 2320 5050              # PP
+00027c50: 2069 7320 6120 7465 6e73 6f72 2077 6974   is a tensor wit
+00027c60: 6820 7368 6170 6520 5b74 6f74 616c 206e  h shape [total n
+00027c70: 756d 6265 7220 6f66 2070 6169 7273 2c6e  umber of pairs,n
+00027c80: 5f68 6964 6465 6e5f 5050 5d0a 2020 2020  _hidden_PP].    
+00027c90: 2020 2020 2020 2020 5050 3a20 746f 7263          PP: torc
+00027ca0: 682e 5465 6e73 6f72 203d 2074 6f72 6368  h.Tensor = torch
+00027cb0: 2e6d 6174 6d75 6c28 7061 6972 5f66 6561  .matmul(pair_fea
+00027cc0: 7475 7265 732e 7479 7065 2874 6f72 6368  tures.type(torch
+00027cd0: 2e66 6c6f 6174 3332 292c 0a20 2020 2020  .float32),.     
+00027ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027d00: 2020 2020 2020 2073 656c 662e 575f 5050         self.W_PP
+00027d10: 2920 2b20 7365 6c66 2e62 5f50 500a 2020  ) + self.b_PP.  
+00027d20: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00027d30: 662e 6261 7463 685f 6e6f 726d 616c 697a  f.batch_normaliz
+00027d40: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00027d50: 2020 2073 656c 662e 5050 5f62 6e2e 6576     self.PP_bn.ev
+00027d60: 616c 2829 0a20 2020 2020 2020 2020 2020  al().           
+00027d70: 2020 2020 2050 5020 3d20 7365 6c66 2e50       PP = self.P
+00027d80: 505f 626e 2850 5029 0a20 2020 2020 2020  P_bn(PP).       
+00027d90: 2020 2020 2050 5020 3d20 6163 7469 7661       PP = activa
+00027da0: 7469 6f6e 2850 5029 0a20 2020 2020 2020  tion(PP).       
+00027db0: 2020 2020 2050 3a20 746f 7263 682e 5465       P: torch.Te
+00027dc0: 6e73 6f72 203d 2074 6f72 6368 2e6d 6174  nsor = torch.mat
+00027dd0: 6d75 6c28 0a20 2020 2020 2020 2020 2020  mul(.           
+00027de0: 2020 2020 2074 6f72 6368 2e63 6f6e 6361       torch.conca
+00027df0: 7428 5b41 505f 696a 202b 2041 505f 6a69  t([AP_ij + AP_ji
+00027e00: 2c20 5050 5d2c 2031 292e 7479 7065 2874  , PP], 1).type(t
+00027e10: 6f72 6368 2e66 6c6f 6174 3332 292c 0a20  orch.float32),. 
+00027e20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00027e30: 656c 662e 575f 5029 202b 2073 656c 662e  elf.W_P) + self.
+00027e40: 625f 500a 2020 2020 2020 2020 2020 2020  b_P.            
+00027e50: 6966 2073 656c 662e 6261 7463 685f 6e6f  if self.batch_no
+00027e60: 726d 616c 697a 653a 0a20 2020 2020 2020  rmalize:.       
+00027e70: 2020 2020 2020 2020 2073 656c 662e 505f           self.P_
+00027e80: 626e 2e65 7661 6c28 290a 2020 2020 2020  bn.eval().      
+00027e90: 2020 2020 2020 2020 2020 5020 3d20 7365            P = se
+00027ea0: 6c66 2e50 5f62 6e28 5029 0a20 2020 2020  lf.P_bn(P).     
+00027eb0: 2020 2020 2020 2050 203d 2061 6374 6976         P = activ
+00027ec0: 6174 696f 6e28 5029 0a20 2020 2020 2020  ation(P).       
+00027ed0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00027ee0: 2020 2050 203d 2070 6169 725f 6665 6174     P = pair_feat
+00027ef0: 7572 6573 0a0a 2020 2020 2020 2020 7265  ures..        re
+00027f00: 7475 726e 205b 412c 2050 5d0a 0a0a 636c  turn [A, P]...cl
+00027f10: 6173 7320 5765 6176 6547 6174 6865 7228  ass WeaveGather(
+00027f20: 6e6e 2e4d 6f64 756c 6529 3a0a 2020 2020  nn.Module):.    
+00027f30: 2222 2249 6d70 6c65 6d65 6e74 7320 7468  """Implements th
+00027f40: 6520 7765 6176 652d 6761 7468 6572 696e  e weave-gatherin
+00027f50: 6720 7365 6374 696f 6e20 6f66 2077 6561  g section of wea
+00027f60: 7665 2063 6f6e 766f 6c75 7469 6f6e 732e  ve convolutions.
+00027f70: 0a20 2020 2054 6869 7320 6973 2074 6865  .    This is the
+00027f80: 2054 6f72 6368 2065 7175 6976 616c 656e   Torch equivalen
+00027f90: 7420 6f66 2074 6865 206f 7269 6769 6e61  t of the origina
+00027fa0: 6c20 696d 706c 656d 656e 7461 7469 6f6e  l implementation
+00027fb0: 2075 7369 6e67 204b 6572 6173 2e0a 0a20   using Keras... 
+00027fc0: 2020 2049 6d70 6c65 6d65 6e74 7320 7468     Implements th
+00027fd0: 6520 6761 7468 6572 696e 6720 6c61 7965  e gathering laye
+00027fe0: 7220 6672 6f6d 205b 315d 5f2e 2054 6865  r from [1]_. The
+00027ff0: 2077 6561 7665 2067 6174 6865 7269 6e67   weave gathering
+00028000: 206c 6179 6572 2067 6174 6865 7273 0a20   layer gathers. 
+00028010: 2020 2070 6572 2d61 746f 6d20 6665 6174     per-atom feat
+00028020: 7572 6573 2074 6f20 6372 6561 7465 2061  ures to create a
+00028030: 206d 6f6c 6563 756c 652d 6c65 7665 6c20   molecule-level 
+00028040: 6669 6e67 6572 7072 696e 7420 696e 2061  fingerprint in a
+00028050: 2077 6561 7665 0a20 2020 2063 6f6e 766f   weave.    convo
+00028060: 6c75 7469 6f6e 616c 206e 6574 776f 726b  lutional network
+00028070: 2e20 5468 6973 206c 6179 6572 2063 616e  . This layer can
+00028080: 2061 6c73 6f20 7065 7266 6f72 6d73 2047   also performs G
+00028090: 6175 7373 6961 6e20 6869 7374 6f67 7261  aussian histogra
+000280a0: 6d0a 2020 2020 6578 7061 6e73 696f 6e20  m.    expansion 
+000280b0: 6173 2064 6574 6169 6c65 6420 696e 205b  as detailed in [
+000280c0: 315d 5f2e 204e 6f74 6520 7468 6174 2074  1]_. Note that t
+000280d0: 6865 2067 6174 6865 7269 6e67 2066 756e  he gathering fun
+000280e0: 6374 696f 6e20 6865 7265 2069 730a 2020  ction here is.  
+000280f0: 2020 7369 6d70 6c79 2061 6464 6974 696f    simply additio
+00028100: 6e20 6173 2069 6e20 5b31 5d5f 3e0a 0a20  n as in [1]_>.. 
+00028110: 2020 2045 7861 6d70 6c65 730a 2020 2020     Examples.    
+00028120: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2054 6869  --------.    Thi
+00028130: 7320 6c61 7965 7220 6578 7065 6374 7320  s layer expects 
+00028140: 3220 696e 7075 7473 2069 6e20 6120 6c69  2 inputs in a li
+00028150: 7374 206f 6620 7468 6520 666f 726d 2060  st of the form `
+00028160: 5b61 746f 6d5f 6665 6174 7572 6573 2c0a  [atom_features,.
+00028170: 2020 2020 7061 6972 5f66 6561 7475 7265      pair_feature
+00028180: 735d 602e 2057 6527 6c6c 2077 616c 6b20  s]`. We'll walk 
+00028190: 7468 726f 7567 6820 7468 6520 7374 7275  through the stru
+000281a0: 6374 7572 650a 2020 2020 6f66 2074 6865  cture.    of the
+000281b0: 7365 2069 6e70 7574 732e 204c 6574 2773  se inputs. Let's
+000281c0: 2073 7461 7274 2077 6974 6820 736f 6d65   start with some
+000281d0: 2062 6173 6963 2064 6566 696e 6974 696f   basic definitio
+000281e0: 6e73 2e0a 0a20 2020 203e 3e3e 2069 6d70  ns...    >>> imp
+000281f0: 6f72 7420 6465 6570 6368 656d 2061 7320  ort deepchem as 
+00028200: 6463 0a20 2020 203e 3e3e 2069 6d70 6f72  dc.    >>> impor
+00028210: 7420 6e75 6d70 7920 6173 206e 700a 0a20  t numpy as np.. 
+00028220: 2020 2053 7570 706f 7365 2079 6f75 2068     Suppose you h
+00028230: 6176 6520 6120 6261 7463 6820 6f66 206d  ave a batch of m
+00028240: 6f6c 6563 756c 6573 0a0a 2020 2020 3e3e  olecules..    >>
+00028250: 3e20 736d 696c 6573 203d 205b 2243 4343  > smiles = ["CCC
+00028260: 222c 2022 4322 5d0a 0a20 2020 204e 6f74  ", "C"]..    Not
+00028270: 6520 7468 6174 2074 6865 7265 2061 7265  e that there are
+00028280: 2034 2061 746f 6d73 2069 6e20 746f 7461   4 atoms in tota
+00028290: 6c20 696e 2074 6869 7320 7379 7374 656d  l in this system
+000282a0: 2e20 5468 6973 206c 6179 6572 2065 7870  . This layer exp
+000282b0: 6563 7473 2069 7473 0a20 2020 2069 6e70  ects its.    inp
+000282c0: 7574 206d 6f6c 6563 756c 6573 2074 6f20  ut molecules to 
+000282d0: 6265 2062 6174 6368 6564 2074 6f67 6574  be batched toget
+000282e0: 6865 722e 0a0a 2020 2020 3e3e 3e20 746f  her...    >>> to
+000282f0: 7461 6c5f 6e5f 6174 6f6d 7320 3d20 340a  tal_n_atoms = 4.
+00028300: 0a20 2020 204c 6574 2773 2073 7570 706f  .    Let's suppo
+00028310: 7365 2074 6861 7420 7765 2068 6176 6520  se that we have 
+00028320: 606e 5f61 746f 6d5f 6665 6174 6020 6665  `n_atom_feat` fe
+00028330: 6174 7572 6573 2070 6572 2061 746f 6d2e  atures per atom.
+00028340: 0a0a 2020 2020 3e3e 3e20 6e5f 6174 6f6d  ..    >>> n_atom
+00028350: 5f66 6561 7420 3d20 3735 0a0a 2020 2020  _feat = 75..    
+00028360: 5468 656e 2063 6f6e 6365 7074 7561 6c6c  Then conceptuall
+00028370: 792c 2060 6174 6f6d 5f66 6561 7460 2069  y, `atom_feat` i
+00028380: 7320 7468 6520 6172 7261 7920 6f66 2073  s the array of s
+00028390: 6861 7065 2060 2874 6f74 616c 5f6e 5f61  hape `(total_n_a
+000283a0: 746f 6d73 2c0a 2020 2020 6e5f 6174 6f6d  toms,.    n_atom
+000283b0: 5f66 6561 7429 6020 6f66 2061 746f 6d69  _feat)` of atomi
+000283c0: 6320 6665 6174 7572 6573 2e20 466f 7220  c features. For 
+000283d0: 7369 6d70 6c69 6369 7479 2c20 6c65 7427  simplicity, let'
+000283e0: 7320 6a75 7374 2067 6f20 7769 7468 2061  s just go with a
+000283f0: 0a20 2020 2072 616e 646f 6d20 7375 6368  .    random such
+00028400: 206d 6174 7269 782e 0a0a 2020 2020 3e3e   matrix...    >>
+00028410: 3e20 6174 6f6d 5f66 6561 7420 3d20 6e70  > atom_feat = np
+00028420: 2e72 616e 646f 6d2e 7261 6e64 2874 6f74  .random.rand(tot
+00028430: 616c 5f6e 5f61 746f 6d73 2c20 6e5f 6174  al_n_atoms, n_at
+00028440: 6f6d 5f66 6561 7429 0a0a 2020 2020 5765  om_feat)..    We
+00028450: 2074 6865 6e20 6e65 6564 2074 6f20 7072   then need to pr
+00028460: 6f76 6964 6520 6120 6d61 7070 696e 6720  ovide a mapping 
+00028470: 6f66 2069 6e64 6963 6573 2074 6f20 7468  of indices to th
+00028480: 6520 6174 6f6d 7320 7468 6579 2062 656c  e atoms they bel
+00028490: 6f6e 6720 746f 2e20 496e 0a20 2020 206f  ong to. In.    o
+000284a0: 7572 7320 6361 7365 2074 6869 7320 776f  urs case this wo
+000284b0: 756c 6420 6265 0a0a 2020 2020 3e3e 3e20  uld be..    >>> 
+000284c0: 6174 6f6d 5f73 706c 6974 203d 206e 702e  atom_split = np.
+000284d0: 6172 7261 7928 5b30 2c20 302c 2030 2c20  array([0, 0, 0, 
+000284e0: 315d 290a 0a20 2020 204c 6574 2773 206e  1])..    Let's n
+000284f0: 6f77 2064 6566 696e 6520 7468 6520 6163  ow define the ac
+00028500: 7475 616c 206c 6179 6572 0a0a 2020 2020  tual layer..    
+00028510: 3e3e 3e20 6761 7468 6572 203d 2057 6561  >>> gather = Wea
+00028520: 7665 4761 7468 6572 2862 6174 6368 5f73  veGather(batch_s
+00028530: 697a 653d 322c 206e 5f69 6e70 7574 3d6e  ize=2, n_input=n
+00028540: 5f61 746f 6d5f 6665 6174 290a 2020 2020  _atom_feat).    
+00028550: 3e3e 3e20 6f75 7470 7574 5f6d 6f6c 6563  >>> output_molec
+00028560: 756c 6573 203d 2067 6174 6865 7228 5b61  ules = gather([a
+00028570: 746f 6d5f 6665 6174 2c20 6174 6f6d 5f73  tom_feat, atom_s
+00028580: 706c 6974 5d29 0a20 2020 203e 3e3e 206c  plit]).    >>> l
+00028590: 656e 286f 7574 7075 745f 6d6f 6c65 6375  en(output_molecu
+000285a0: 6c65 7329 0a20 2020 2032 0a0a 2020 2020  les).    2..    
+000285b0: 5265 6665 7265 6e63 6573 0a20 2020 202d  References.    -
+000285c0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2e2e  ---------.    ..
+000285d0: 205b 315d 204b 6561 726e 6573 2c20 5374   [1] Kearnes, St
+000285e0: 6576 656e 2c20 6574 2061 6c2e 2022 4d6f  even, et al. "Mo
+000285f0: 6c65 6375 6c61 7220 6772 6170 6820 636f  lecular graph co
+00028600: 6e76 6f6c 7574 696f 6e73 3a20 6d6f 7669  nvolutions: movi
+00028610: 6e67 2062 6579 6f6e 640a 2020 2020 2020  ng beyond.      
+00028620: 2020 6669 6e67 6572 7072 696e 7473 2e22    fingerprints."
+00028630: 204a 6f75 726e 616c 206f 6620 636f 6d70   Journal of comp
+00028640: 7574 6572 2d61 6964 6564 206d 6f6c 6563  uter-aided molec
+00028650: 756c 6172 2064 6573 6967 6e20 3330 2e38  ular design 30.8
+00028660: 2028 3230 3136 293a 0a20 2020 2020 2020   (2016):.       
+00028670: 2035 3935 2d36 3038 2e0a 2020 2020 2222   595-608..    ""
+00028680: 220a 0a20 2020 2064 6566 205f 5f69 6e69  "..    def __ini
+00028690: 745f 5f28 7365 6c66 2c0a 2020 2020 2020  t__(self,.      
+000286a0: 2020 2020 2020 2020 2020 2062 6174 6368             batch
+000286b0: 5f73 697a 653a 2069 6e74 2c0a 2020 2020  _size: int,.    
+000286c0: 2020 2020 2020 2020 2020 2020 206e 5f69               n_i
+000286d0: 6e70 7574 3a20 696e 7420 3d20 3132 382c  nput: int = 128,
+000286e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000286f0: 2020 6761 7573 7369 616e 5f65 7870 616e    gaussian_expan
+00028700: 643a 2062 6f6f 6c20 3d20 5472 7565 2c0a  d: bool = True,.
+00028710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028720: 2063 6f6d 7072 6573 735f 706f 7374 5f67   compress_post_g
+00028730: 6175 7373 6961 6e5f 6578 7061 6e73 696f  aussian_expansio
+00028740: 6e3a 2062 6f6f 6c20 3d20 4661 6c73 652c  n: bool = False,
+00028750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00028760: 2020 696e 6974 5f3a 2073 7472 203d 2027    init_: str = '
+00028770: 7861 7669 6572 5f75 6e69 666f 726d 5f27  xavier_uniform_'
+00028780: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00028790: 2020 2061 6374 6976 6174 696f 6e3a 2073     activation: s
+000287a0: 7472 203d 2027 7461 6e68 272c 0a20 2020  tr = 'tanh',.   
+000287b0: 2020 2020 2020 2020 2020 2020 2020 2a2a                **
+000287c0: 6b77 6172 6773 293a 0a20 2020 2020 2020  kwargs):.       
+000287d0: 2022 2222 0a20 2020 2020 2020 2050 6172   """.        Par
+000287e0: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+000287f0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00028800: 2020 2062 6174 6368 5f73 697a 653a 2069     batch_size: i
+00028810: 6e74 0a20 2020 2020 2020 2020 2020 206e  nt.            n
+00028820: 756d 6265 7220 6f66 206d 6f6c 6563 756c  umber of molecul
+00028830: 6573 2069 6e20 6120 6261 7463 680a 2020  es in a batch.  
+00028840: 2020 2020 2020 6e5f 696e 7075 743a 2069        n_input: i
+00028850: 6e74 2c20 6f70 7469 6f6e 616c 2028 6465  nt, optional (de
+00028860: 6661 756c 7420 3132 3829 0a20 2020 2020  fault 128).     
+00028870: 2020 2020 2020 206e 756d 6265 7220 6f66         number of
+00028880: 2066 6561 7475 7265 7320 666f 7220 6561   features for ea
+00028890: 6368 2069 6e70 7574 206d 6f6c 6563 756c  ch input molecul
+000288a0: 650a 2020 2020 2020 2020 6761 7573 7369  e.        gaussi
+000288b0: 616e 5f65 7870 616e 643a 2062 6f6f 6c65  an_expand: boole
+000288c0: 616e 2c20 6f70 7469 6f6e 616c 2028 6465  an, optional (de
+000288d0: 6661 756c 7420 5472 7565 290a 2020 2020  fault True).    
+000288e0: 2020 2020 2020 2020 5768 6574 6865 7220          Whether 
+000288f0: 746f 2065 7870 616e 6420 6561 6368 2064  to expand each d
+00028900: 696d 656e 7369 6f6e 206f 6620 6174 6f6d  imension of atom
+00028910: 6963 2066 6561 7475 7265 7320 6279 2067  ic features by g
+00028920: 6175 7373 6961 6e20 6869 7374 6f67 7261  aussian histogra
+00028930: 6d0a 2020 2020 2020 2020 636f 6d70 7265  m.        compre
+00028940: 7373 5f70 6f73 745f 6761 7573 7369 616e  ss_post_gaussian
+00028950: 5f65 7870 616e 7369 6f6e 3a20 626f 6f6c  _expansion: bool
+00028960: 2c20 6f70 7469 6f6e 616c 2028 6465 6661  , optional (defa
+00028970: 756c 7420 4661 6c73 6529 0a20 2020 2020  ult False).     
+00028980: 2020 2020 2020 2049 6620 5472 7565 2c20         If True, 
+00028990: 636f 6d70 7265 7373 2074 6865 2072 6573  compress the res
+000289a0: 756c 7473 206f 6620 7468 6520 4761 7573  ults of the Gaus
+000289b0: 7369 616e 2065 7870 616e 7369 6f6e 2062  sian expansion b
+000289c0: 6163 6b20 746f 2074 6865 0a20 2020 2020  ack to the.     
+000289d0: 2020 2020 2020 206f 7269 6769 6e61 6c20         original 
+000289e0: 6469 6d65 6e73 696f 6e73 206f 6620 7468  dimensions of th
+000289f0: 6520 696e 7075 7420 6279 2075 7369 6e67  e input by using
+00028a00: 2061 206c 696e 6561 7220 6c61 7965 7220   a linear layer 
+00028a10: 7769 7468 2073 7065 6369 6669 6564 0a20  with specified. 
+00028a20: 2020 2020 2020 2020 2020 2061 6374 6976             activ
+00028a30: 6174 696f 6e20 6675 6e63 7469 6f6e 2e20  ation function. 
+00028a40: 4e6f 7465 2074 6861 7420 7468 6973 2063  Note that this c
+00028a50: 6f6d 7072 6573 7369 6f6e 2077 6173 206e  ompression was n
+00028a60: 6f74 2069 6e20 7468 6520 6f72 6967 696e  ot in the origin
+00028a70: 616c 0a20 2020 2020 2020 2020 2020 2070  al.            p
+00028a80: 6170 6572 2c20 6275 7420 7761 7320 7072  aper, but was pr
+00028a90: 6573 656e 7420 696e 2074 6865 206f 7269  esent in the ori
+00028aa0: 6769 6e61 6c20 4465 6570 4368 656d 2069  ginal DeepChem i
+00028ab0: 6d70 6c65 6d65 6e74 6174 696f 6e20 736f  mplementation so
+00028ac0: 2069 730a 2020 2020 2020 2020 2020 2020   is.            
+00028ad0: 6c65 6674 2070 7265 7365 6e74 2066 6f72  left present for
+00028ae0: 2062 6163 6b77 6172 6473 2063 6f6d 7061   backwards compa
+00028af0: 7469 6269 6c69 7479 2e0a 2020 2020 2020  tibility..      
+00028b00: 2020 696e 6974 3a20 7374 722c 206f 7074    init: str, opt
+00028b10: 696f 6e61 6c20 2864 6566 6175 6c74 2027  ional (default '
+00028b20: 7861 7669 6572 5f75 6e69 666f 726d 5f27  xavier_uniform_'
+00028b30: 290a 2020 2020 2020 2020 2020 2020 5765  ).            We
+00028b40: 6967 6874 2069 6e69 7469 616c 697a 6174  ight initializat
+00028b50: 696f 6e20 666f 7220 6669 6c74 6572 7320  ion for filters 
+00028b60: 6966 2060 636f 6d70 7265 7373 5f70 6f73  if `compress_pos
+00028b70: 745f 6761 7573 7369 616e 5f65 7870 616e  t_gaussian_expan
+00028b80: 7369 6f6e 600a 2020 2020 2020 2020 2020  sion`.          
+00028b90: 2020 6973 2054 7275 652e 0a20 2020 2020    is True..     
+00028ba0: 2020 2061 6374 6976 6174 696f 6e3a 2073     activation: s
+00028bb0: 7472 2c20 6f70 7469 6f6e 616c 2028 6465  tr, optional (de
+00028bc0: 6661 756c 7420 2774 616e 6827 290a 2020  fault 'tanh').  
+00028bd0: 2020 2020 2020 2020 2020 4163 7469 7661            Activa
+00028be0: 7469 6f6e 2066 756e 6374 696f 6e20 6170  tion function ap
+00028bf0: 706c 6965 6420 666f 7220 6669 6c74 6572  plied for filter
+00028c00: 7320 6966 0a20 2020 2020 2020 2020 2020  s if.           
+00028c10: 2060 636f 6d70 7265 7373 5f70 6f73 745f   `compress_post_
+00028c20: 6761 7573 7369 616e 5f65 7870 616e 7369  gaussian_expansi
+00028c30: 6f6e 6020 6973 2054 7275 652e 0a20 2020  on` is True..   
+00028c40: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00028c50: 2073 7570 6572 2857 6561 7665 4761 7468   super(WeaveGath
+00028c60: 6572 2c20 7365 6c66 292e 5f5f 696e 6974  er, self).__init
+00028c70: 5f5f 282a 2a6b 7761 7267 7329 0a20 2020  __(**kwargs).   
+00028c80: 2020 2020 2073 656c 662e 6e5f 696e 7075       self.n_inpu
+00028c90: 743a 2069 6e74 203d 206e 5f69 6e70 7574  t: int = n_input
+00028ca0: 0a20 2020 2020 2020 2073 656c 662e 6261  .        self.ba
+00028cb0: 7463 685f 7369 7a65 3a20 696e 7420 3d20  tch_size: int = 
+00028cc0: 6261 7463 685f 7369 7a65 0a20 2020 2020  batch_size.     
+00028cd0: 2020 2073 656c 662e 6761 7573 7369 616e     self.gaussian
+00028ce0: 5f65 7870 616e 643a 2062 6f6f 6c20 3d20  _expand: bool = 
+00028cf0: 6761 7573 7369 616e 5f65 7870 616e 640a  gaussian_expand.
+00028d00: 2020 2020 2020 2020 7365 6c66 2e63 6f6d          self.com
+00028d10: 7072 6573 735f 706f 7374 5f67 6175 7373  press_post_gauss
+00028d20: 6961 6e5f 6578 7061 6e73 696f 6e3a 2062  ian_expansion: b
+00028d30: 6f6f 6c20 3d20 636f 6d70 7265 7373 5f70  ool = compress_p
+00028d40: 6f73 745f 6761 7573 7369 616e 5f65 7870  ost_gaussian_exp
+00028d50: 616e 7369 6f6e 0a20 2020 2020 2020 2073  ansion.        s
+00028d60: 656c 662e 696e 6974 3a20 7374 7220 3d20  elf.init: str = 
+00028d70: 696e 6974 5f20 2023 2053 6574 2077 6569  init_  # Set wei
+00028d80: 6768 7420 696e 6974 6961 6c69 7a61 7469  ght initializati
+00028d90: 6f6e 0a20 2020 2020 2020 2073 656c 662e  on.        self.
+00028da0: 6163 7469 7661 7469 6f6e 3a20 7374 7220  activation: str 
+00028db0: 3d20 6163 7469 7661 7469 6f6e 2020 2320  = activation  # 
+00028dc0: 4765 7420 6163 7469 7661 7469 6f6e 730a  Get activations.
+00028dd0: 2020 2020 2020 2020 7365 6c66 2e61 6374          self.act
+00028de0: 6976 6174 696f 6e5f 666e 3a20 746f 7263  ivation_fn: torc
+00028df0: 682e 6e6e 2e4d 6f64 756c 6520 3d20 6765  h.nn.Module = ge
+00028e00: 745f 6163 7469 7661 7469 6f6e 2861 6374  t_activation(act
+00028e10: 6976 6174 696f 6e29 0a0a 2020 2020 2020  ivation)..      
+00028e20: 2020 6966 2073 656c 662e 636f 6d70 7265    if self.compre
+00028e30: 7373 5f70 6f73 745f 6761 7573 7369 616e  ss_post_gaussian
+00028e40: 5f65 7870 616e 7369 6f6e 3a0a 2020 2020  _expansion:.    
+00028e50: 2020 2020 2020 2020 696e 6974 203d 2067          init = g
+00028e60: 6574 6174 7472 2869 6e69 7469 616c 697a  etattr(initializ
+00028e70: 6572 732c 2073 656c 662e 696e 6974 290a  ers, self.init).
+00028e80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00028e90: 2e57 3a20 746f 7263 682e 5465 6e73 6f72  .W: torch.Tensor
+00028ea0: 203d 2069 6e69 7428 0a20 2020 2020 2020   = init(.       
+00028eb0: 2020 2020 2020 2020 2074 6f72 6368 2e65           torch.e
+00028ec0: 6d70 7479 285b 7365 6c66 2e6e 5f69 6e70  mpty([self.n_inp
+00028ed0: 7574 202a 2031 312c 2073 656c 662e 6e5f  ut * 11, self.n_
+00028ee0: 696e 7075 745d 2929 0a20 2020 2020 2020  input])).       
+00028ef0: 2020 2020 2073 656c 662e 623a 2074 6f72       self.b: tor
+00028f00: 6368 2e54 656e 736f 7220 3d20 746f 7263  ch.Tensor = torc
+00028f10: 682e 7a65 726f 7328 2873 656c 662e 6e5f  h.zeros((self.n_
+00028f20: 696e 7075 742c 2929 0a20 2020 2020 2020  input,)).       
+00028f30: 2073 656c 662e 6275 696c 7420 3d20 5472   self.built = Tr
+00028f40: 7565 0a0a 2020 2020 6465 6620 5f5f 7265  ue..    def __re
+00028f50: 7072 5f5f 2873 656c 6629 3a0a 2020 2020  pr__(self):.    
+00028f60: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00028f70: 5265 7475 726e 7320 6120 7374 7269 6e67  Returns a string
+00028f80: 2072 6570 7265 7365 6e74 6174 696f 6e20   representation 
+00028f90: 6f66 2074 6865 206f 626a 6563 742e 0a0a  of the object...
+00028fa0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00028fb0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00028fc0: 0a20 2020 2020 2020 2073 7472 3a20 4120  .        str: A 
+00028fd0: 7374 7269 6e67 2074 6861 7420 636f 6e74  string that cont
+00028fe0: 6169 6e73 2074 6865 2063 6c61 7373 206e  ains the class n
+00028ff0: 616d 6520 666f 6c6c 6f77 6564 2062 7920  ame followed by 
+00029000: 7468 6520 7661 6c75 6573 206f 6620 6974  the values of it
+00029010: 7320 696e 7374 616e 6365 2076 6172 6961  s instance varia
+00029020: 626c 652e 0a20 2020 2020 2020 2022 2222  ble..        """
+00029030: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00029040: 280a 2020 2020 2020 2020 2020 2020 6627  (.            f'
+00029050: 7b73 656c 662e 5f5f 636c 6173 735f 5f2e  {self.__class__.
+00029060: 5f5f 6e61 6d65 5f5f 7d28 6261 7463 685f  __name__}(batch_
+00029070: 7369 7a65 3a7b 7365 6c66 2e62 6174 6368  size:{self.batch
+00029080: 5f73 697a 657d 2c6e 5f69 6e70 7574 3a7b  _size},n_input:{
+00029090: 7365 6c66 2e6e 5f69 6e70 7574 7d2c 6761  self.n_input},ga
+000290a0: 7573 7369 616e 5f65 7870 616e 643a 7b73  ussian_expand:{s
+000290b0: 656c 662e 6761 7573 7369 616e 5f65 7870  elf.gaussian_exp
+000290c0: 616e 647d 2c69 6e69 743a 7b73 656c 662e  and},init:{self.
+000290d0: 696e 6974 7d2c 6163 7469 7661 7469 6f6e  init},activation
+000290e0: 3a7b 7365 6c66 2e61 6374 6976 6174 696f  :{self.activatio
+000290f0: 6e7d 2c63 6f6d 7072 6573 735f 706f 7374  n},compress_post
+00029100: 5f67 6175 7373 6961 6e5f 6578 7061 6e73  _gaussian_expans
+00029110: 696f 6e3a 7b73 656c 662e 636f 6d70 7265  ion:{self.compre
+00029120: 7373 5f70 6f73 745f 6761 7573 7369 616e  ss_post_gaussian
+00029130: 5f65 7870 616e 7369 6f6e 7d29 270a 2020  _expansion})'.  
+00029140: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+00029150: 2066 6f72 7761 7264 2873 656c 662c 2069   forward(self, i
+00029160: 6e70 7574 733a 204c 6973 745b 556e 696f  nputs: List[Unio
+00029170: 6e5b 6e70 2e6e 6461 7272 6179 2c0a 2020  n[np.ndarray,.  
+00029180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000291a0: 2020 2020 2020 206e 702e 6e64 6172 7261         np.ndarra
+000291b0: 795d 5d29 202d 3e20 746f 7263 682e 5465  y]]) -> torch.Te
+000291c0: 6e73 6f72 3a0a 2020 2020 2020 2020 2222  nsor:.        ""
+000291d0: 2243 7265 6174 6573 2077 6561 7665 2074  "Creates weave t
+000291e0: 656e 736f 7273 2e0a 0a20 2020 2020 2020  ensors...       
+000291f0: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00029200: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00029210: 2020 2020 2020 2069 6e70 7574 733a 204c         inputs: L
+00029220: 6973 745b 556e 696f 6e5b 6e70 2e6e 6461  ist[Union[np.nda
+00029230: 7272 6179 2c6e 702e 6e64 6172 7261 795d  rray,np.ndarray]
+00029240: 5d0a 2020 2020 2020 2020 2020 2020 5368  ].            Sh
+00029250: 6f75 6c64 2063 6f6e 7461 696e 2032 2074  ould contain 2 t
+00029260: 656e 736f 7273 205b 6174 6f6d 5f66 6561  ensors [atom_fea
+00029270: 7475 7265 732c 2061 746f 6d5f 7370 6c69  tures, atom_spli
+00029280: 745d 0a0a 2020 2020 2020 2020 5265 7475  t]..        Retu
+00029290: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
+000292a0: 2d2d 2d0a 2020 2020 2020 2020 6f75 7470  ---.        outp
+000292b0: 7574 5f6d 6f6c 6563 756c 6573 3a20 746f  ut_molecules: to
+000292c0: 7263 682e 5465 6e73 6f72 0a20 2020 2020  rch.Tensor.     
+000292d0: 2020 2020 2020 2045 6163 6820 656e 7472         Each entr
+000292e0: 7920 696e 2074 6869 7320 6c69 7374 2069  y in this list i
+000292f0: 7320 6f66 2073 6861 7065 2060 2873 656c  s of shape `(sel
+00029300: 662e 6e5f 696e 7075 7473 2c29 600a 0a20  f.n_inputs,)`.. 
+00029310: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00029320: 2020 206f 7574 7075 7473 3a20 746f 7263     outputs: torc
+00029330: 682e 5465 6e73 6f72 203d 2074 6f72 6368  h.Tensor = torch
+00029340: 2e74 656e 736f 7228 696e 7075 7473 5b30  .tensor(inputs[0
+00029350: 5d29 0a20 2020 2020 2020 2061 746f 6d5f  ]).        atom_
+00029360: 7370 6c69 743a 2074 6f72 6368 2e54 656e  split: torch.Ten
+00029370: 736f 7220 3d20 746f 7263 682e 7465 6e73  sor = torch.tens
+00029380: 6f72 2869 6e70 7574 735b 315d 290a 0a20  or(inputs[1]).. 
+00029390: 2020 2020 2020 2069 6620 7365 6c66 2e67         if self.g
+000293a0: 6175 7373 6961 6e5f 6578 7061 6e64 3a0a  aussian_expand:.
+000293b0: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
+000293c0: 7574 7320 3d20 7365 6c66 2e67 6175 7373  uts = self.gauss
+000293d0: 6961 6e5f 6869 7374 6f67 7261 6d28 6f75  ian_histogram(ou
+000293e0: 7470 7574 7329 0a0a 2020 2020 2020 2020  tputs)..        
+000293f0: 745f 6772 703a 2044 6963 745b 5465 6e73  t_grp: Dict[Tens
+00029400: 6f72 2c20 5465 6e73 6f72 5d20 3d20 7b7d  or, Tensor] = {}
+00029410: 0a20 2020 2020 2020 2069 6478 3a20 696e  .        idx: in
+00029420: 7420 3d20 300a 2020 2020 2020 2020 666f  t = 0.        fo
+00029430: 7220 692c 2073 5f69 6420 696e 2065 6e75  r i, s_id in enu
+00029440: 6d65 7261 7465 2861 746f 6d5f 7370 6c69  merate(atom_spli
+00029450: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+00029460: 735f 6964 203d 2073 5f69 642e 6974 656d  s_id = s_id.item
+00029470: 2829 0a20 2020 2020 2020 2020 2020 2069  ().            i
+00029480: 6620 735f 6964 2069 6e20 745f 6772 703a  f s_id in t_grp:
+00029490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000294a0: 2074 5f67 7270 5b73 5f69 645d 203d 2074   t_grp[s_id] = t
+000294b0: 5f67 7270 5b73 5f69 645d 202b 206f 7574  _grp[s_id] + out
+000294c0: 7075 7473 5b69 6478 5d0a 2020 2020 2020  puts[idx].      
+000294d0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000294e0: 2020 2020 2020 2020 2020 2020 745f 6772              t_gr
+000294f0: 705b 735f 6964 5d20 3d20 6f75 7470 7574  p[s_id] = output
+00029500: 735b 6964 785d 0a20 2020 2020 2020 2020  s[idx].         
+00029510: 2020 2069 6478 203d 2069 202b 2031 0a0a     idx = i + 1..
+00029520: 2020 2020 2020 2020 2020 2020 6c73 7420              lst 
+00029530: 3d20 6c69 7374 2874 5f67 7270 2e76 616c  = list(t_grp.val
+00029540: 7565 7328 2929 0a20 2020 2020 2020 2020  ues()).         
+00029550: 2020 2074 656e 736f 7220 3d20 746f 7263     tensor = torc
+00029560: 682e 7374 6163 6b28 6c73 7429 0a20 2020  h.stack(lst).   
+00029570: 2020 2020 206f 7574 7075 745f 6d6f 6c65       output_mole
+00029580: 6375 6c65 733a 2074 6f72 6368 2e54 656e  cules: torch.Ten
+00029590: 736f 7220 3d20 7465 6e73 6f72 0a0a 2020  sor = tensor..  
+000295a0: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
+000295b0: 6d70 7265 7373 5f70 6f73 745f 6761 7573  mpress_post_gaus
+000295c0: 7369 616e 5f65 7870 616e 7369 6f6e 3a0a  sian_expansion:.
+000295d0: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
+000295e0: 7574 5f6d 6f6c 6563 756c 6573 203d 2074  ut_molecules = t
+000295f0: 6f72 6368 2e6d 6174 6d75 6c28 0a20 2020  orch.matmul(.   
+00029600: 2020 2020 2020 2020 2020 2020 206f 7574               out
+00029610: 7075 745f 6d6f 6c65 6375 6c65 732e 7479  put_molecules.ty
+00029620: 7065 2874 6f72 6368 2e66 6c6f 6174 3332  pe(torch.float32
+00029630: 292c 2073 656c 662e 5729 202b 2073 656c  ), self.W) + sel
+00029640: 662e 620a 2020 2020 2020 2020 2020 2020  f.b.            
+00029650: 6f75 7470 7574 5f6d 6f6c 6563 756c 6573  output_molecules
+00029660: 203d 2073 656c 662e 6163 7469 7661 7469   = self.activati
+00029670: 6f6e 5f66 6e28 6f75 7470 7574 5f6d 6f6c  on_fn(output_mol
+00029680: 6563 756c 6573 290a 0a20 2020 2020 2020  ecules)..       
+00029690: 2072 6574 7572 6e20 6f75 7470 7574 5f6d   return output_m
+000296a0: 6f6c 6563 756c 6573 0a0a 2020 2020 6465  olecules..    de
+000296b0: 6620 6761 7573 7369 616e 5f68 6973 746f  f gaussian_histo
+000296c0: 6772 616d 2873 656c 662c 2078 3a20 746f  gram(self, x: to
+000296d0: 7263 682e 5465 6e73 6f72 2920 2d3e 2074  rch.Tensor) -> t
+000296e0: 6f72 6368 2e54 656e 736f 723a 0a20 2020  orch.Tensor:.   
+000296f0: 2020 2020 2022 2222 4578 7061 6e64 7320       """Expands 
+00029700: 696e 7075 7420 696e 746f 2061 2073 6574  input into a set
+00029710: 206f 6620 6761 7573 7369 616e 2068 6973   of gaussian his
+00029720: 746f 6772 616d 2062 696e 732e 0a0a 2020  togram bins...  
+00029730: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+00029740: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00029750: 2d2d 2d0a 2020 2020 2020 2020 783a 2074  ---.        x: t
+00029760: 6f72 6368 2e54 656e 736f 720a 2020 2020  orch.Tensor.    
+00029770: 2020 2020 2020 2020 4f66 2073 6861 7065          Of shape
+00029780: 2060 284e 2c20 6e5f 6665 6174 2960 0a0a   `(N, n_feat)`..
+00029790: 2020 2020 2020 2020 4578 616d 706c 6573          Examples
+000297a0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+000297b0: 2d0a 2020 2020 2020 2020 5468 6973 206d  -.        This m
+000297c0: 6574 686f 6420 7573 6573 2031 3120 6269  ethod uses 11 bi
+000297d0: 6e73 2073 7061 6e6e 696e 6720 706f 7274  ns spanning port
+000297e0: 696f 6e73 206f 6620 6120 4761 7573 7369  ions of a Gaussi
+000297f0: 616e 2077 6974 6820 7a65 726f 206d 6561  an with zero mea
+00029800: 6e0a 2020 2020 2020 2020 616e 6420 756e  n.        and un
+00029810: 6974 2073 7461 6e64 6172 6420 6465 7669  it standard devi
+00029820: 6174 696f 6e2e 0a0a 2020 2020 2020 2020  ation...        
+00029830: 3e3e 3e20 6761 7573 7369 616e 5f6d 656d  >>> gaussian_mem
+00029840: 6265 7273 6869 7073 203d 205b 282d 312e  berships = [(-1.
+00029850: 3634 352c 2030 2e32 3833 292c 2028 2d31  645, 0.283), (-1
+00029860: 2e30 3830 2c20 302e 3137 3029 2c0a 2020  .080, 0.170),.  
+00029870: 2020 2020 2020 2e2e 2e20 2020 2020 2020        ...       
+00029880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029890: 2020 282d 302e 3733 392c 2030 2e31 3334    (-0.739, 0.134
+000298a0: 292c 2028 2d30 2e34 3638 2c20 302e 3131  ), (-0.468, 0.11
+000298b0: 3829 2c0a 2020 2020 2020 2020 2e2e 2e20  8),.        ... 
+000298c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000298d0: 2020 2020 2020 2020 282d 302e 3232 382c          (-0.228,
+000298e0: 2030 2e31 3134 292c 2028 302e 2c20 302e   0.114), (0., 0.
+000298f0: 3131 3429 2c0a 2020 2020 2020 2020 2e2e  114),.        ..
+00029900: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
+00029910: 2020 2020 2020 2020 2020 2830 2e32 3238            (0.228
+00029920: 2c20 302e 3131 3429 2c20 2830 2e34 3638  , 0.114), (0.468
+00029930: 2c20 302e 3131 3829 2c0a 2020 2020 2020  , 0.118),.      
+00029940: 2020 2e2e 2e20 2020 2020 2020 2020 2020    ...           
+00029950: 2020 2020 2020 2020 2020 2020 2020 2830                (0
+00029960: 2e37 3339 2c20 302e 3133 3429 2c20 2831  .739, 0.134), (1
+00029970: 2e30 3830 2c20 302e 3137 3029 2c0a 2020  .080, 0.170),.  
+00029980: 2020 2020 2020 2e2e 2e20 2020 2020 2020        ...       
+00029990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000299a0: 2020 2831 2e36 3435 2c20 302e 3238 3329    (1.645, 0.283)
+000299b0: 5d0a 0a20 2020 2020 2020 2057 6520 636f  ]..        We co
+000299c0: 6e73 7472 7563 7420 6120 4761 7573 7369  nstruct a Gaussi
+000299d0: 616e 2061 7420 6067 6175 7373 6961 6e5f  an at `gaussian_
+000299e0: 6d65 6d62 6572 7368 6970 735b 695d 5b30  memberships[i][0
+000299f0: 5d60 2077 6974 6820 7374 616e 6461 7264  ]` with standard
+00029a00: 0a20 2020 2020 2020 2064 6576 6961 7469  .        deviati
+00029a10: 6f6e 2060 6761 7573 7369 616e 5f6d 656d  on `gaussian_mem
+00029a20: 6265 7273 6869 7073 5b69 5d5b 315d 602e  berships[i][1]`.
+00029a30: 2045 6163 6820 6665 6174 7572 6520 696e   Each feature in
+00029a40: 2060 7860 2069 7320 6173 7369 676e 6564   `x` is assigned
+00029a50: 0a20 2020 2020 2020 2074 6865 2070 726f  .        the pro
+00029a60: 6261 6269 6c69 7479 206f 6620 6661 6c6c  bability of fall
+00029a70: 696e 6720 696e 2065 6163 6820 4761 7573  ing in each Gaus
+00029a80: 7369 616e 2c20 616e 6420 7072 6f62 6162  sian, and probab
+00029a90: 696c 6974 6965 7320 6172 650a 2020 2020  ilities are.    
+00029aa0: 2020 2020 6e6f 726d 616c 697a 6564 2061      normalized a
+00029ab0: 6372 6f73 7320 7468 6520 3131 2064 6966  cross the 11 dif
+00029ac0: 6665 7265 6e74 2047 6175 7373 6961 6e73  ferent Gaussians
+00029ad0: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00029ae0: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
+00029af0: 2d2d 0a20 2020 2020 2020 206f 7574 7075  --.        outpu
+00029b00: 7473 3a20 746f 7263 682e 5465 6e73 6f72  ts: torch.Tensor
+00029b10: 0a20 2020 2020 2020 2020 2020 204f 6620  .            Of 
+00029b20: 7368 6170 6520 6028 4e2c 2031 312a 6e5f  shape `(N, 11*n_
+00029b30: 6665 6174 2960 0a20 2020 2020 2020 2022  feat)`.        "
+00029b40: 2222 0a20 2020 2020 2020 2069 6d70 6f72  "".        impor
+00029b50: 7420 746f 7263 682e 6469 7374 7269 6275  t torch.distribu
+00029b60: 7469 6f6e 7320 6173 2064 6973 740a 2020  tions as dist.  
+00029b70: 2020 2020 2020 6761 7573 7369 616e 5f6d        gaussian_m
+00029b80: 656d 6265 7273 6869 7073 3a20 4c69 7374  emberships: List
+00029b90: 5b54 7570 6c65 5b66 6c6f 6174 2c20 666c  [Tuple[float, fl
+00029ba0: 6f61 745d 5d20 3d20 5b28 2d31 2e36 3435  oat]] = [(-1.645
+00029bb0: 2c20 302e 3238 3329 2c0a 2020 2020 2020  , 0.283),.      
+00029bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029bf0: 2020 2020 2028 2d31 2e30 3830 2c20 302e       (-1.080, 0.
+00029c00: 3137 3029 2c0a 2020 2020 2020 2020 2020  170),.          
+00029c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029c40: 2028 2d30 2e37 3339 2c20 302e 3133 3429   (-0.739, 0.134)
+00029c50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00029c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029c80: 2020 2020 2020 2020 2020 2020 2028 2d30               (-0
+00029c90: 2e34 3638 2c20 302e 3131 3829 2c0a 2020  .468, 0.118),.  
+00029ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029cd0: 2020 2020 2020 2020 2028 2d30 2e32 3238           (-0.228
+00029ce0: 2c20 302e 3131 3429 2c0a 2020 2020 2020  , 0.114),.      
+00029cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029d20: 2020 2020 2028 302e 2c20 302e 3131 3429       (0., 0.114)
+00029d30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00029d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029d60: 2020 2020 2020 2020 2020 2020 2028 302e               (0.
+00029d70: 3232 382c 2030 2e31 3134 292c 0a20 2020  228, 0.114),.   
+00029d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029db0: 2020 2020 2020 2020 2830 2e34 3638 2c20          (0.468, 
+00029dc0: 302e 3131 3829 2c0a 2020 2020 2020 2020  0.118),.        
+00029dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029e00: 2020 2028 302e 3733 392c 2030 2e31 3334     (0.739, 0.134
+00029e10: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00029e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029e40: 2020 2020 2020 2020 2020 2020 2020 2831                (1
+00029e50: 2e30 3830 2c20 302e 3137 3029 2c0a 2020  .080, 0.170),.  
+00029e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029e90: 2020 2020 2020 2020 2028 312e 3634 352c           (1.645,
+00029ea0: 2030 2e32 3833 295d 0a0a 2020 2020 2020   0.283)]..      
+00029eb0: 2020 6469 7374 7269 6275 7469 6f6e 733a    distributions:
+00029ec0: 204c 6973 745b 6469 7374 2e4e 6f72 6d61   List[dist.Norma
+00029ed0: 6c5d 203d 205b 0a20 2020 2020 2020 2020  l] = [.         
+00029ee0: 2020 2064 6973 742e 4e6f 726d 616c 2874     dist.Normal(t
+00029ef0: 6f72 6368 2e74 656e 736f 7228 705b 305d  orch.tensor(p[0]
+00029f00: 292c 2074 6f72 6368 2e74 656e 736f 7228  ), torch.tensor(
+00029f10: 705b 315d 2929 0a20 2020 2020 2020 2020  p[1])).         
+00029f20: 2020 2066 6f72 2070 2069 6e20 6761 7573     for p in gaus
+00029f30: 7369 616e 5f6d 656d 6265 7273 6869 7073  sian_memberships
+00029f40: 0a20 2020 2020 2020 205d 0a20 2020 2020  .        ].     
+00029f50: 2020 2064 6973 745f 6d61 783a 204c 6973     dist_max: Lis
+00029f60: 745b 746f 7263 682e 5465 6e73 6f72 5d20  t[torch.Tensor] 
+00029f70: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
+00029f80: 6469 7374 7269 6275 7469 6f6e 735b 695d  distributions[i]
+00029f90: 2e6c 6f67 5f70 726f 6228 746f 7263 682e  .log_prob(torch.
+00029fa0: 7465 6e73 6f72 280a 2020 2020 2020 2020  tensor(.        
+00029fb0: 2020 2020 2020 2020 6761 7573 7369 616e          gaussian
+00029fc0: 5f6d 656d 6265 7273 6869 7073 5b69 5d5b  _memberships[i][
+00029fd0: 305d 2929 2e65 7870 2829 2066 6f72 2069  0])).exp() for i
+00029fe0: 2069 6e20 7261 6e67 6528 3131 290a 2020   in range(11).  
+00029ff0: 2020 2020 2020 5d0a 0a20 2020 2020 2020        ]..       
+0002a000: 206f 7574 7075 7473 3a20 4c69 7374 5b74   outputs: List[t
+0002a010: 6f72 6368 2e54 656e 736f 725d 203d 205b  orch.Tensor] = [
+0002a020: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
+0002a030: 7472 6962 7574 696f 6e73 5b69 5d2e 6c6f  tributions[i].lo
+0002a040: 675f 7072 6f62 2874 6f72 6368 2e74 656e  g_prob(torch.ten
+0002a050: 736f 7228 7829 292e 6578 7028 2920 2f20  sor(x)).exp() / 
+0002a060: 6469 7374 5f6d 6178 5b69 5d0a 2020 2020  dist_max[i].    
+0002a070: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+0002a080: 2072 616e 6765 2831 3129 0a20 2020 2020   range(11).     
+0002a090: 2020 205d 0a20 2020 2020 2020 206f 7574     ].        out
+0002a0a0: 7075 743a 2074 6f72 6368 2e54 656e 736f  put: torch.Tenso
+0002a0b0: 7220 3d20 746f 7263 682e 7374 6163 6b28  r = torch.stack(
+0002a0c0: 6f75 7470 7574 732c 2064 696d 3d32 290a  outputs, dim=2).
+0002a0d0: 2020 2020 2020 2020 6f75 7470 7574 203d          output =
+0002a0e0: 206f 7574 7075 7420 2f20 746f 7263 682e   output / torch.
+0002a0f0: 7375 6d28 6f75 7470 7574 2c20 6469 6d3d  sum(output, dim=
+0002a100: 322c 206b 6565 7064 696d 3d54 7275 6529  2, keepdim=True)
+0002a110: 0a20 2020 2020 2020 206f 7574 7075 7420  .        output 
+0002a120: 3d20 6f75 7470 7574 2e76 6965 7728 2d31  = output.view(-1
+0002a130: 2c20 7365 6c66 2e6e 5f69 6e70 7574 202a  , self.n_input *
+0002a140: 2031 3129 0a20 2020 2020 2020 2072 6574   11).        ret
+0002a150: 7572 6e20 6f75 7470 7574 0a              urn output.
```

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/lcnn.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/lcnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/mat.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/mat.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/megnet.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/megnet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/modular.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/modular.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/mpnn.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/mpnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/normalizing_flows_pytorch.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/normalizing_flows_pytorch.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/pagtn.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/pagtn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/pna_gnn.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/pna_gnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/readout.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/readout.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/torch_models/torch_model.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/torch_models/torch_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/models/wandblogger.py` & `deepchem-2.7.2.dev20230728002356/deepchem/models/wandblogger.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/__init__.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/check_availability.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/check_availability.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/defaults.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/defaults.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/dnasim.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/dnasim.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/bace_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/bace_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/bace_features.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/bace_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/bbbc_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/bbbc_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/bbbp_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/bbbp_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/cell_counting_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/cell_counting_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/chembl25_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/chembl25_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/chembl_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/chembl_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/chembl_tasks.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/chembl_tasks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/clearance_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/clearance_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/clintox_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/clintox_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/delaney_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/delaney_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/factors_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/factors_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/freesolv_dataset.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/freesolv_dataset.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/hiv_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/hiv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/hopv_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/hopv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/hppb_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/hppb_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/kaggle_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/kaggle_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/kaggle_features.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/kaggle_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/kinase_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/kinase_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/lipo_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/lipo_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/load_dataset_template.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/load_dataset_template.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/material_datasets/load_bandgap.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/material_datasets/load_bandgap.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/material_datasets/load_perovskite.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/material_datasets/load_perovskite.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/molnet_loader.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/molnet_loader.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/muv_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/muv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/nci_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/nci_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/pcba_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/pcba_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/pdbbind_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/pdbbind_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/ppb_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/ppb_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/qm7_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/qm7_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/qm8_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/qm8_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/qm9_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/qm9_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/sampl_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/sampl_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/sider_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/sider_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/sweetlead_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/sweetlead_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/thermosol_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/thermosol_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/tox21_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/tox21_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/toxcast_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/toxcast_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/uspto_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/uspto_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/uv_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/uv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/uv_tasks.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/uv_tasks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/load_function/zinc15_datasets.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/load_function/zinc15_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/preset_hyper_parameters.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/preset_hyper_parameters.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/run_benchmark.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/run_benchmark_low_data.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/run_benchmark_low_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/molnet/run_benchmark_models.py` & `deepchem-2.7.2.dev20230728002356/deepchem/molnet/run_benchmark_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/rl/__init__.py` & `deepchem-2.7.2.dev20230728002356/deepchem/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/rl/a2c.py` & `deepchem-2.7.2.dev20230728002356/deepchem/rl/a2c.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/rl/envs/test_tictactoe.py` & `deepchem-2.7.2.dev20230728002356/deepchem/rl/envs/test_tictactoe.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/rl/envs/tictactoe.py` & `deepchem-2.7.2.dev20230728002356/deepchem/rl/envs/tictactoe.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/rl/ppo.py` & `deepchem-2.7.2.dev20230728002356/deepchem/rl/ppo.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/splits/__init__.py` & `deepchem-2.7.2.dev20230728002356/deepchem/splits/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/splits/splitters.py` & `deepchem-2.7.2.dev20230728002356/deepchem/splits/splitters.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/splits/task_splitter.py` & `deepchem-2.7.2.dev20230728002356/deepchem/splits/task_splitter.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/trans/__init__.py` & `deepchem-2.7.2.dev20230728002356/deepchem/trans/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/trans/duplicate.py` & `deepchem-2.7.2.dev20230728002356/deepchem/trans/duplicate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/trans/transformers.py` & `deepchem-2.7.2.dev20230728002356/deepchem/trans/transformers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/__init__.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/conformers.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/conformers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/coordinate_box_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/coordinate_box_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/data_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/debug_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/debug_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/dftutils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/dftutils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/docking_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/docking_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/electron_sampler.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/electron_sampler.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/evaluate.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/evaluate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/fake_data_generator.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/fake_data_generator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/fragment_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/fragment_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/genomics_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/genomics_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/geometry_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/graph_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/grover.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/hash_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/molecule_feature_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/molecule_feature_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/noncovalent_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/noncovalent_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/pdbqt_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/pdbqt_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/pytorch_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/rdkit_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/save.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/save.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/sequence_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_coordinate_box_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_coordinate_box_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_data_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_dftutils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_dftutils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_docking_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_docking_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_electron_sampler.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_electron_sampler.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_evaluate.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_fake_data_generator.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_fake_data_generator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_fragment_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_fragment_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_generator_evaluator.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_generator_evaluator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_genomics_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_genomics_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_geometry_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_geometry_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_graph_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_graph_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_grover.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_hash_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_hash_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_molecule_feature_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_molecule_feature_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_noncovalent_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_noncovalent_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_pdbqt_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_pdbqt_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_pytorch_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_rdkit_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_sequence_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_sequence_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/test/test_voxel_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/test/test_voxel_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/typing.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/typing.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/vina_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/vina_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem/utils/voxel_utils.py` & `deepchem-2.7.2.dev20230728002356/deepchem/utils/voxel_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem.egg-info/PKG-INFO` & `deepchem-2.7.2.dev20230728002356/deepchem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepchem
-Version: 2.7.2.dev20230727235143
+Version: 2.7.2.dev20230728002356
 Summary: Deep learning models for drug discovery,         quantum chemistry, and the life sciences.
 Home-page: https://github.com/deepchem/deepchem
 Maintainer: DeepChem contributors
 License: MIT
 Project-URL: Documentation, https://deepchem.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/deepchem/deepchem
 Keywords: deepchem,chemistry,biology,materials-science,life-science,drug-discovery
```

### Comparing `deepchem-2.7.2.dev20230727235143/deepchem.egg-info/SOURCES.txt` & `deepchem-2.7.2.dev20230728002356/deepchem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/setup.cfg` & `deepchem-2.7.2.dev20230728002356/setup.cfg`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230727235143/setup.py` & `deepchem-2.7.2.dev20230728002356/setup.py`

 * *Files identical despite different names*

