# Comparing `tmp/pipelime_python-1.6.2.tar.gz` & `tmp/pipelime_python-1.7.0.tar.gz`

## Comparing `pipelime_python-1.6.2.tar` & `pipelime_python-1.7.0.tar`

### file list

```diff
@@ -1,120 +1,120 @@
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/__init__.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/choixe/__init__.py
--rw-r--r--   0        0        0    14915 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/choixe/xconfig.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/choixe/ast/__init__.py
--rw-r--r--   0        0        0     9723 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/choixe/ast/nodes.py
--rw-r--r--   0        0        0    13790 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/choixe/ast/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/choixe/utils/__init__.py
--rw-r--r--   0        0        0     3587 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/choixe/utils/common.py
--rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/choixe/utils/imports.py
--rw-r--r--   0        0        0     5314 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/choixe/utils/io.py
--rw-r--r--   0        0        0    13100 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/choixe/utils/rand.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/choixe/visitors/__init__.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/choixe/visitors/decoder.py
--rw-r--r--   0        0        0     7805 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/choixe/visitors/inspector.py
--rw-r--r--   0        0        0    13803 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/choixe/visitors/processor.py
--rw-r--r--   0        0        0     7932 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/choixe/visitors/unparser.py
--rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/choixe/visitors/walker.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/cli/__init__.py
--rw-r--r--   0        0        0    27326 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/cli/main.py
--rw-r--r--   0        0        0     7310 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/cli/parser.py
--rw-r--r--   0        0        0    15208 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/cli/pretty_print.py
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/cli/subcommands.py
--rw-r--r--   0        0        0    22727 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/cli/utils.py
--rw-r--r--   0        0        0    13769 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/cli/wizard.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/cli/tui/__init__.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/cli/tui/tui.css
--rw-r--r--   0        0        0     9900 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/cli/tui/tui.py
--rw-r--r--   0        0        0     7248 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/cli/tui/utils.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/commands/__init__.py
--rw-r--r--   0        0        0    34047 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/commands/general.py
--rw-r--r--   0        0        0    28216 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/commands/interfaces.py
--rw-r--r--   0        0        0    15995 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/commands/piper.py
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/commands/shell.py
--rw-r--r--   0        0        0    13525 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/commands/split_ops.py
--rw-r--r--   0        0        0     9227 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/commands/tempman.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/commands/toy_dataset.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/items/__init__.py
--rw-r--r--   0        0        0    30747 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/items/base.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/items/binary_item.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/items/image_item.py
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/items/metadata_item.py
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/items/model3d_item.py
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/items/numpy_item.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/items/pickle_item.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/__init__.py
--rw-r--r--   0        0        0    18226 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/graph.py
--rw-r--r--   0        0        0    17058 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/drawing/__init__.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/drawing/base.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/drawing/factory.py
--rw-r--r--   0        0        0    10954 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/drawing/graphviz.py
--rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/drawing/mermaid.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/executors/__init__.py
--rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/executors/base.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/executors/factory.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/executors/naive.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/parsers/__init__.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/parsers/base.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/parsers/choixe_parser.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/parsers/factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/progress/__init__.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/progress/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/progress/estimator/__init__.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/progress/estimator/base.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/progress/estimator/factory.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/progress/estimator/naive.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/progress/listener/__init__.py
--rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/progress/listener/base.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/progress/listener/factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/progress/listener/callbacks/__init__.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/progress/listener/callbacks/file.py
--rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/progress/listener/callbacks/rich_table.py
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/progress/listener/callbacks/tqdm_bars.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/progress/listener/receiver/__init__.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/progress/listener/receiver/zmq.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/progress/tracker/__init__.py
--rw-r--r--   0        0        0     6366 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/progress/tracker/base.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/progress/tracker/direct.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/progress/tracker/factory.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/progress/tracker/loguru.py
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/piper/progress/tracker/zmq.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/remotes/__init__.py
--rw-r--r--   0        0        0    12825 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/remotes/base.py
--rw-r--r--   0        0        0     6644 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/remotes/s3_remote.py
--rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/remotes/shared_folder_remote.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/sequences/__init__.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/sequences/direct_access.py
--rw-r--r--   0        0        0     6696 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/sequences/grabber.py
--rw-r--r--   0        0        0     8682 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/sequences/sample.py
--rw-r--r--   0        0        0    23171 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/sequences/samples_sequence.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/sequences/torch.py
--rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/sequences/utils.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/sequences/pipes/__init__.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/sequences/pipes/base.py
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/sequences/pipes/mapping.py
--rw-r--r--   0        0        0    14141 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/sequences/pipes/operations.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/sequences/pipes/validation.py
--rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/sequences/pipes/writers.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/sequences/sources/__init__.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/sequences/sources/from_callable.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/sequences/sources/raw.py
--rw-r--r--   0        0        0     8094 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/sequences/sources/readers.py
--rw-r--r--   0        0        0     8015 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/sequences/sources/toy_dataset.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/stages/__init__.py
--rw-r--r--   0        0        0     9973 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/stages/augmentations.py
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/stages/base.py
--rw-r--r--   0        0        0    13512 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/stages/entities.py
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/stages/item_info.py
--rw-r--r--   0        0        0     5065 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/stages/item_replacement.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/stages/item_sources.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/stages/key_transformations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/utils/__init__.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/utils/context_managers.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/utils/inspection.py
--rw-r--r--   0        0        0    23458 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pipelime/utils/pydantic_types.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/.gitignore
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/LICENSE
--rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/README.md
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/pyproject.toml
--rw-r--r--   0        0        0     8502 2020-02-02 00:00:00.000000 pipelime_python-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/__init__.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/choixe/__init__.py
+-rw-r--r--   0        0        0    14915 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/choixe/xconfig.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/choixe/ast/__init__.py
+-rw-r--r--   0        0        0     9723 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/choixe/ast/nodes.py
+-rw-r--r--   0        0        0    14001 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/choixe/ast/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/choixe/utils/__init__.py
+-rw-r--r--   0        0        0     3587 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/choixe/utils/common.py
+-rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/choixe/utils/imports.py
+-rw-r--r--   0        0        0     5314 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/choixe/utils/io.py
+-rw-r--r--   0        0        0    13100 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/choixe/utils/rand.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/choixe/visitors/__init__.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/choixe/visitors/decoder.py
+-rw-r--r--   0        0        0     7805 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/choixe/visitors/inspector.py
+-rw-r--r--   0        0        0    13803 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/choixe/visitors/processor.py
+-rw-r--r--   0        0        0     7932 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/choixe/visitors/unparser.py
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/choixe/visitors/walker.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/cli/__init__.py
+-rw-r--r--   0        0        0    27326 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/cli/main.py
+-rw-r--r--   0        0        0     7310 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/cli/parser.py
+-rw-r--r--   0        0        0    15208 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/cli/pretty_print.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/cli/subcommands.py
+-rw-r--r--   0        0        0    22727 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/cli/utils.py
+-rw-r--r--   0        0        0    13769 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/cli/wizard.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/cli/tui/__init__.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/cli/tui/tui.css
+-rw-r--r--   0        0        0     9900 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/cli/tui/tui.py
+-rw-r--r--   0        0        0     7248 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/cli/tui/utils.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/commands/__init__.py
+-rw-r--r--   0        0        0    34047 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/commands/general.py
+-rw-r--r--   0        0        0    28216 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/commands/interfaces.py
+-rw-r--r--   0        0        0    18436 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/commands/piper.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/commands/shell.py
+-rw-r--r--   0        0        0    13525 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/commands/split_ops.py
+-rw-r--r--   0        0        0     9227 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/commands/tempman.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/commands/toy_dataset.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/items/__init__.py
+-rw-r--r--   0        0        0    30994 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/items/base.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/items/binary_item.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/items/image_item.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/items/metadata_item.py
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/items/model3d_item.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/items/numpy_item.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/items/pickle_item.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/__init__.py
+-rw-r--r--   0        0        0    18437 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/graph.py
+-rw-r--r--   0        0        0    17058 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/drawing/__init__.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/drawing/base.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/drawing/factory.py
+-rw-r--r--   0        0        0    10954 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/drawing/graphviz.py
+-rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/drawing/mermaid.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/executors/__init__.py
+-rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/executors/base.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/executors/factory.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/executors/naive.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/parsers/__init__.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/parsers/base.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/parsers/choixe_parser.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/parsers/factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/progress/__init__.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/progress/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/progress/estimator/__init__.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/progress/estimator/base.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/progress/estimator/factory.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/progress/estimator/naive.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/progress/listener/__init__.py
+-rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/progress/listener/base.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/progress/listener/factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/progress/listener/callbacks/__init__.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/progress/listener/callbacks/file.py
+-rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/progress/listener/callbacks/rich_table.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/progress/listener/callbacks/tqdm_bars.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/progress/listener/receiver/__init__.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/progress/listener/receiver/zmq.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/progress/tracker/__init__.py
+-rw-r--r--   0        0        0     6366 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/progress/tracker/base.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/progress/tracker/direct.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/progress/tracker/factory.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/progress/tracker/loguru.py
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/piper/progress/tracker/zmq.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/remotes/__init__.py
+-rw-r--r--   0        0        0    12825 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/remotes/base.py
+-rw-r--r--   0        0        0     6644 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/remotes/s3_remote.py
+-rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/remotes/shared_folder_remote.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/sequences/__init__.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/sequences/direct_access.py
+-rw-r--r--   0        0        0     6696 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/sequences/grabber.py
+-rw-r--r--   0        0        0     8682 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/sequences/sample.py
+-rw-r--r--   0        0        0    23171 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/sequences/samples_sequence.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/sequences/torch.py
+-rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/sequences/utils.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/sequences/pipes/__init__.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/sequences/pipes/base.py
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/sequences/pipes/mapping.py
+-rw-r--r--   0        0        0    14141 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/sequences/pipes/operations.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/sequences/pipes/validation.py
+-rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/sequences/pipes/writers.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/sequences/sources/__init__.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/sequences/sources/from_callable.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/sequences/sources/raw.py
+-rw-r--r--   0        0        0     8094 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/sequences/sources/readers.py
+-rw-r--r--   0        0        0     8015 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/sequences/sources/toy_dataset.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/stages/__init__.py
+-rw-r--r--   0        0        0     9973 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/stages/augmentations.py
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/stages/base.py
+-rw-r--r--   0        0        0    13512 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/stages/entities.py
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/stages/item_info.py
+-rw-r--r--   0        0        0     5065 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/stages/item_replacement.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/stages/item_sources.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/stages/key_transformations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/utils/__init__.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/utils/context_managers.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/utils/inspection.py
+-rw-r--r--   0        0        0    23458 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pipelime/utils/pydantic_types.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/.gitignore
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/LICENSE
+-rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/README.md
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     8502 2020-02-02 00:00:00.000000 pipelime_python-1.7.0/PKG-INFO
```

### Comparing `pipelime_python-1.6.2/pipelime/choixe/xconfig.py` & `pipelime_python-1.7.0/pipelime/choixe/xconfig.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/choixe/ast/nodes.py` & `pipelime_python-1.7.0/pipelime/choixe/ast/nodes.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/choixe/ast/parser.py` & `pipelime_python-1.7.0/pipelime/choixe/ast/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import ast
 import re
 from dataclasses import dataclass
-from typing import Any, Dict, List, Optional, OrderedDict, Tuple, Type, Union
+from typing import Any, Callable, Dict, List, Optional, OrderedDict, Tuple, Type, Union
 
 import astunparse
 import schema as S
 
 import pipelime.choixe.ast.nodes as c_ast
 
 DIRECTIVE_PREFIX = "$"
@@ -138,15 +138,15 @@
 
 
 class Parser:
     """Choixe parser for all kind of python objects."""
 
     def __init__(self) -> None:
         self._scanner = Scanner()
-        self._type_map = {
+        self._type_map: Dict[Type, Callable[[Any], c_ast.Node]] = {
             dict: self._parse_dict,
             list: self._parse_list,
             tuple: self._parse_list,
             str: self._parse_str,
         }
 
         self._call_forms = {
@@ -295,15 +295,16 @@
             for schema, fn in self._key_value_forms.items():
                 if schema.is_valid({k: v}):
                     parsed_keyvalues.append(fn(k, v))
                     any_valid = True
                     break
 
             if not any_valid:
-                parsed_other[self._parse_str(k)] = self.parse(v)
+                parsed_key = self._type_map.get(type(k), self._parse_value)(k)
+                parsed_other[parsed_key] = self.parse(v)
 
         # Parse the remaining entries as a DictNode.
         parsed_other = c_ast.DictNode(nodes=parsed_other)
 
         # If no key_value form was found, return the DictNode.
         if len(parsed_keyvalues) == 0:
             return parsed_other
@@ -329,14 +330,17 @@
                     node = fn(*args, **kwargs)
                     return node
         except TypeError:
             raise ChoixeStructValidationError(token)
 
         raise ChoixeTokenValidationError(token)
 
+    def _parse_value(self, data: Any) -> c_ast.LiteralNode:
+        return c_ast.LiteralNode(data=data)
+
     def _parse_str(self, data: str) -> c_ast.Node:
         nodes = []
         for token in self._scanner.scan(data):
             nodes.append(self._parse_token(token))
 
         if len(nodes) == 0:
             return c_ast.LiteralNode(data="")
@@ -351,20 +355,20 @@
         Args:
             data (Any): The object to parse.
 
         Returns:
             Node: The parsed Choixe AST node.
         """
         try:
-            fn = c_ast.LiteralNode
+            fn = self._parse_value
             for type_, parse_fn in self._type_map.items():
                 if isinstance(data, type_):
                     fn = parse_fn
                     break
-            res = fn(data)  # type: ignore
+            res = fn(data)
             return res
 
         except (ChoixeSyntaxError, SyntaxError) as e:
             code = e.args[0]
             raise ChoixeParsingError(
                 f'Error when parsing code "{code}" found in "{data}", expected either '
                 "a compact form like $DIRECTIVE, or a call form like "
```

### Comparing `pipelime_python-1.6.2/pipelime/choixe/utils/common.py` & `pipelime_python-1.7.0/pipelime/choixe/utils/common.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/choixe/utils/imports.py` & `pipelime_python-1.7.0/pipelime/choixe/utils/imports.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/choixe/utils/io.py` & `pipelime_python-1.7.0/pipelime/choixe/utils/io.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/choixe/utils/rand.py` & `pipelime_python-1.7.0/pipelime/choixe/utils/rand.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/choixe/visitors/decoder.py` & `pipelime_python-1.7.0/pipelime/choixe/visitors/decoder.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/choixe/visitors/inspector.py` & `pipelime_python-1.7.0/pipelime/choixe/visitors/inspector.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/choixe/visitors/processor.py` & `pipelime_python-1.7.0/pipelime/choixe/visitors/processor.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/choixe/visitors/unparser.py` & `pipelime_python-1.7.0/pipelime/choixe/visitors/unparser.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/choixe/visitors/walker.py` & `pipelime_python-1.7.0/pipelime/choixe/visitors/walker.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/cli/__init__.py` & `pipelime_python-1.7.0/pipelime/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/cli/main.py` & `pipelime_python-1.7.0/pipelime/cli/main.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/cli/parser.py` & `pipelime_python-1.7.0/pipelime/cli/parser.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/cli/pretty_print.py` & `pipelime_python-1.7.0/pipelime/cli/pretty_print.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/cli/subcommands.py` & `pipelime_python-1.7.0/pipelime/cli/subcommands.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/cli/utils.py` & `pipelime_python-1.7.0/pipelime/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/cli/wizard.py` & `pipelime_python-1.7.0/pipelime/cli/wizard.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/cli/tui/tui.py` & `pipelime_python-1.7.0/pipelime/cli/tui/tui.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/cli/tui/utils.py` & `pipelime_python-1.7.0/pipelime/cli/tui/utils.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/commands/__init__.py` & `pipelime_python-1.7.0/pipelime/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/commands/general.py` & `pipelime_python-1.7.0/pipelime/commands/general.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/commands/interfaces.py` & `pipelime_python-1.7.0/pipelime/commands/interfaces.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/commands/piper.py` & `pipelime_python-1.7.0/pipelime/commands/piper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typing as t
-from abc import abstractmethod
+from abc import ABC, abstractmethod
 from enum import Enum
 from pathlib import Path
 
 from loguru import logger
-from pydantic import BaseModel, Field, PositiveInt, PrivateAttr
+from pydantic import BaseModel, Field, PositiveInt, PrivateAttr, create_model
 
 from pipelime.choixe.utils.io import PipelimeTemporaryDirectory
 from pipelime.piper import PipelimeCommand, PiperPortType
 
 if t.TYPE_CHECKING:
     from pipelime.piper.graph import DAGNodesGraph
 
@@ -31,18 +31,18 @@
         }[self]
 
 
 class PiperGraphCommandBase(PipelimeCommand):
     """Base class for piper-aware commands."""
 
     include: t.Union[str, t.Sequence[str], None] = Field(
-        None, alias="in", description="Nodes not in this list are not run."
+        None, alias="i", description="Nodes not in this list are not run."
     )
     exclude: t.Union[str, t.Sequence[str], None] = Field(
-        None, alias="ex", description="Nodes in this list are not run."
+        None, alias="e", description="Nodes in this list are not run."
     )
 
     _piper_graph: t.Optional["DAGNodesGraph"] = PrivateAttr(None)
 
     @property
     @abstractmethod
     def nodes_graph(self) -> T_NODES:
@@ -111,15 +111,15 @@
             for x in self.piper_graph.output_data_nodes
         }
 
 
 class RunCommandBase(GraphPortForwardingCommand):
     token: t.Optional[str] = Field(
         None,
-        alias="tk",
+        alias="t",
         description=(
             "The execution token. If not specified, a new token will be generated."
         ),
     )
     watch: t.Union[bool, WatcherBackend, Path, None] = Field(
         None,
         description=(
@@ -451,15 +451,14 @@
     @abstractmethod
     def create_graph(self) -> T_NODES:
         """Creates the graph nodes.
 
         Returns:
             T_NODES: a dictionary containing the mapping between node names and nodes.
         """
-        pass
 
     @property
     def nodes_graph(self) -> T_NODES:
         if self._nodes is None:
             self._nodes = self.create_graph()
         return self._nodes
 
@@ -468,7 +467,84 @@
         if self.draw:
             output = self.draw if isinstance(self.draw, Path) else None
             self.draw_graph(
                 output, **(self.draw if isinstance(self.draw, t.Mapping) else {})
             )
             return
         return super().run()
+
+
+class PiperDAG(
+    BaseModel,
+    ABC,
+    allow_population_by_field_name=True,
+    extra="forbid",
+    copy_on_model_validation="none",
+):
+    """Base class to ease the creation of Python DAG Object.
+
+    Derived classes should add custom properties as pydantic fields and implement
+    at least the `create_graph` method. Then, use the `piper_dag` decorator to create
+    a full-fledged command class.
+
+    Example:
+
+        @piper_dag
+        class MyGrandDAG(PiperDAG, title="mgd"):
+            '''My Grand DAG'''
+
+            aparam: str = Field(..., alias="a", description="a param")
+            bparam: int = Field(12, alias="b", description="b param")
+
+            def create_graph(self, folder_debug):
+                ...
+    """
+
+    @property
+    def input_mapping(self) -> t.Optional[t.Mapping[str, str]]:
+        """Optional mapping from graph input data keys and desired keys."""
+        return None
+
+    @property
+    def output_mapping(self) -> t.Optional[t.Mapping[str, str]]:
+        """Optional mapping from graph output data keys and desired keys."""
+        return None
+
+    @abstractmethod
+    def create_graph(self, folder_debug: Path) -> T_NODES:
+        """Creates the graph nodes.
+
+        Args:
+            folder_debug (Path): The path to the folder for debug data.
+
+        Returns:
+            T_NODES: a dictionary containing the mapping between node names and nodes.
+        """
+
+
+def piper_dag(cls: t.Type[PiperDAG]):
+    """A decorator to create a full-fledged command class from a PiperDAG class."""
+
+    class _PiperDagCommandHelper(DagBaseCommand):
+        properties: cls = Field(..., alias="p")
+
+        @property
+        def input_mapping(self) -> t.Optional[t.Mapping[str, str]]:
+            """Optional mapping from graph input data keys and desired keys."""
+            return self.properties.input_mapping
+
+        @property
+        def output_mapping(self) -> t.Optional[t.Mapping[str, str]]:
+            """Optional mapping from graph output data keys and desired keys."""
+            return self.properties.output_mapping
+
+        def create_graph(self) -> T_NODES:
+            return self.properties.create_graph(self.folder_debug)
+
+    dag_command = create_model(
+        cls.__name__,
+        __base__=_PiperDagCommandHelper,
+        __module__=cls.__module__,
+        __cls_kwargs__={"title": cls.schema()["title"]},
+    )
+    dag_command.__doc__ = cls.__doc__
+    return dag_command
```

### Comparing `pipelime_python-1.6.2/pipelime/commands/shell.py` & `pipelime_python-1.7.0/pipelime/commands/shell.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/commands/split_ops.py` & `pipelime_python-1.7.0/pipelime/commands/split_ops.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/commands/tempman.py` & `pipelime_python-1.7.0/pipelime/commands/tempman.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/commands/toy_dataset.py` & `pipelime_python-1.7.0/pipelime/commands/toy_dataset.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/items/__init__.py` & `pipelime_python-1.7.0/pipelime/items/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,20 @@
     no_data_cache,
     data_cache,
 )
 
 # import and register all items
 from pipelime.items.binary_item import BinaryItem
 from pipelime.items.pickle_item import PickleItem
-from pipelime.items.numpy_item import NumpyItem, NpyNumpyItem, TxtNumpyItem
+from pipelime.items.numpy_item import (
+    NumpyItem,
+    NumpyRawItem,
+    NpyNumpyItem,
+    TxtNumpyItem,
+)
 from pipelime.items.image_item import (
     ImageItem,
     BmpImageItem,
     PngImageItem,
     JpegImageItem,
     TiffImageItem,
 )
```

### Comparing `pipelime_python-1.6.2/pipelime/items/base.py` & `pipelime_python-1.7.0/pipelime/items/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -658,14 +658,20 @@
             data_source = (
                 self._serialize_to_local_file(trg)
                 if isinstance(trg, Path)
                 else self._serialize_to_remote(trg)
             )
             if data_source is not None:
                 self._add_data_source(data_source)
+                if (
+                    self.cache_data is None
+                    and Item.is_cache_enabled(self.__class__) is False
+                    or self.cache_data is False
+                ):
+                    self._data_cache = None
 
     def remove_data_source(
         self: DerivedItemTp, *sources: _item_data_source
     ) -> DerivedItemTp:
         def _normalize_source(src: _item_data_source) -> t.List[_item_data_source]:
             if isinstance(src, Path):
                 src = src.resolve().absolute()
```

### Comparing `pipelime_python-1.6.2/pipelime/items/binary_item.py` & `pipelime_python-1.7.0/pipelime/items/binary_item.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/items/image_item.py` & `pipelime_python-1.7.0/pipelime/items/image_item.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/items/metadata_item.py` & `pipelime_python-1.7.0/pipelime/items/metadata_item.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/items/model3d_item.py` & `pipelime_python-1.7.0/pipelime/items/model3d_item.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/items/numpy_item.py` & `pipelime_python-1.7.0/pipelime/items/numpy_item.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/piper/graph.py` & `pipelime_python-1.7.0/pipelime/piper/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -445,20 +445,26 @@
                 return str(x)
             if isinstance(x, Path):
                 return x.resolve().absolute().as_posix()
             return repr(x)
 
         if io_map is not None:
             for name, value in io_map.items():
-                if isinstance(value, (str, bytes)) or not isinstance(value, Sequence):
-                    value = [value]
+                if isinstance(value, (str, bytes)):
+                    values = [value]
+                elif isinstance(value, Sequence):
+                    values = value
+                elif isinstance(value, Mapping):
+                    values = list(value.values())
+                else:
+                    values = [value]
 
                 port_basename = f"{node_name}.{node_cmd.command_name}.{name}"
                 attrs = {}
-                for idx, x in enumerate(value):
+                for idx, x in enumerate(values):
                     if x:  # discard empty strings and None
                         x_name = _to_str(x)
                         n0 = GraphNodeData(
                             x_name, x_name, data_max_width, ellipsis_position
                         )
                         n1 = GraphNodeOperation(node_name, node_cmd, show_command_name)
                         if is_input:
@@ -470,15 +476,15 @@
                             n0, n1 = n1, n0
 
                         di_graph.add_edge(n0, n1)
                         attrs.update(
                             {
                                 (n0, n1): {
                                     port_attr: f"{port_basename}[{idx}]"
-                                    if len(value) > 1
+                                    if len(values) > 1
                                     else port_basename,
                                     DAGNodesGraph.GraphAttrs.EDGE_TYPE: edge_attr,
                                 }
                             }
                         )
                 nx.set_edge_attributes(di_graph, attrs)
```

### Comparing `pipelime_python-1.6.2/pipelime/piper/model.py` & `pipelime_python-1.7.0/pipelime/piper/model.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/piper/drawing/base.py` & `pipelime_python-1.7.0/pipelime/piper/drawing/base.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/piper/drawing/factory.py` & `pipelime_python-1.7.0/pipelime/piper/drawing/factory.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/piper/drawing/graphviz.py` & `pipelime_python-1.7.0/pipelime/piper/drawing/graphviz.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/piper/drawing/mermaid.py` & `pipelime_python-1.7.0/pipelime/piper/drawing/mermaid.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/piper/executors/base.py` & `pipelime_python-1.7.0/pipelime/piper/executors/base.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/piper/executors/factory.py` & `pipelime_python-1.7.0/pipelime/piper/executors/factory.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/piper/executors/naive.py` & `pipelime_python-1.7.0/pipelime/piper/executors/naive.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/piper/parsers/base.py` & `pipelime_python-1.7.0/pipelime/piper/parsers/base.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/piper/parsers/choixe_parser.py` & `pipelime_python-1.7.0/pipelime/piper/parsers/choixe_parser.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/piper/parsers/factory.py` & `pipelime_python-1.7.0/pipelime/piper/parsers/factory.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/piper/progress/model.py` & `pipelime_python-1.7.0/pipelime/piper/progress/model.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/piper/progress/estimator/base.py` & `pipelime_python-1.7.0/pipelime/piper/progress/estimator/base.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/piper/progress/estimator/naive.py` & `pipelime_python-1.7.0/pipelime/piper/progress/estimator/naive.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/piper/progress/listener/base.py` & `pipelime_python-1.7.0/pipelime/piper/progress/listener/base.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/piper/progress/listener/factory.py` & `pipelime_python-1.7.0/pipelime/piper/progress/listener/factory.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/piper/progress/listener/callbacks/file.py` & `pipelime_python-1.7.0/pipelime/piper/progress/listener/callbacks/file.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/piper/progress/listener/callbacks/rich_table.py` & `pipelime_python-1.7.0/pipelime/piper/progress/listener/callbacks/rich_table.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/piper/progress/listener/callbacks/tqdm_bars.py` & `pipelime_python-1.7.0/pipelime/piper/progress/listener/callbacks/tqdm_bars.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/piper/progress/listener/receiver/zmq.py` & `pipelime_python-1.7.0/pipelime/piper/progress/listener/receiver/zmq.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/piper/progress/tracker/base.py` & `pipelime_python-1.7.0/pipelime/piper/progress/tracker/base.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/piper/progress/tracker/direct.py` & `pipelime_python-1.7.0/pipelime/piper/progress/tracker/direct.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/piper/progress/tracker/factory.py` & `pipelime_python-1.7.0/pipelime/piper/progress/tracker/factory.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/piper/progress/tracker/loguru.py` & `pipelime_python-1.7.0/pipelime/piper/progress/tracker/loguru.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/piper/progress/tracker/zmq.py` & `pipelime_python-1.7.0/pipelime/piper/progress/tracker/zmq.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/remotes/base.py` & `pipelime_python-1.7.0/pipelime/remotes/base.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/remotes/s3_remote.py` & `pipelime_python-1.7.0/pipelime/remotes/s3_remote.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/remotes/shared_folder_remote.py` & `pipelime_python-1.7.0/pipelime/remotes/shared_folder_remote.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/sequences/direct_access.py` & `pipelime_python-1.7.0/pipelime/sequences/direct_access.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/sequences/grabber.py` & `pipelime_python-1.7.0/pipelime/sequences/grabber.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/sequences/sample.py` & `pipelime_python-1.7.0/pipelime/sequences/sample.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/sequences/samples_sequence.py` & `pipelime_python-1.7.0/pipelime/sequences/samples_sequence.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/sequences/utils.py` & `pipelime_python-1.7.0/pipelime/sequences/utils.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/sequences/pipes/base.py` & `pipelime_python-1.7.0/pipelime/sequences/pipes/base.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/sequences/pipes/mapping.py` & `pipelime_python-1.7.0/pipelime/sequences/pipes/mapping.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/sequences/pipes/operations.py` & `pipelime_python-1.7.0/pipelime/sequences/pipes/operations.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/sequences/pipes/validation.py` & `pipelime_python-1.7.0/pipelime/sequences/pipes/validation.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/sequences/pipes/writers.py` & `pipelime_python-1.7.0/pipelime/sequences/pipes/writers.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/sequences/sources/from_callable.py` & `pipelime_python-1.7.0/pipelime/sequences/sources/from_callable.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/sequences/sources/raw.py` & `pipelime_python-1.7.0/pipelime/sequences/sources/raw.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/sequences/sources/readers.py` & `pipelime_python-1.7.0/pipelime/sequences/sources/readers.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/sequences/sources/toy_dataset.py` & `pipelime_python-1.7.0/pipelime/sequences/sources/toy_dataset.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/stages/__init__.py` & `pipelime_python-1.7.0/pipelime/stages/__init__.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/stages/augmentations.py` & `pipelime_python-1.7.0/pipelime/stages/augmentations.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/stages/base.py` & `pipelime_python-1.7.0/pipelime/stages/base.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/stages/entities.py` & `pipelime_python-1.7.0/pipelime/stages/entities.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/stages/item_info.py` & `pipelime_python-1.7.0/pipelime/stages/item_info.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/stages/item_replacement.py` & `pipelime_python-1.7.0/pipelime/stages/item_replacement.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/stages/item_sources.py` & `pipelime_python-1.7.0/pipelime/stages/item_sources.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/stages/key_transformations.py` & `pipelime_python-1.7.0/pipelime/stages/key_transformations.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/utils/context_managers.py` & `pipelime_python-1.7.0/pipelime/utils/context_managers.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/utils/inspection.py` & `pipelime_python-1.7.0/pipelime/utils/inspection.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pipelime/utils/pydantic_types.py` & `pipelime_python-1.7.0/pipelime/utils/pydantic_types.py`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/.gitignore` & `pipelime_python-1.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/LICENSE` & `pipelime_python-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/README.md` & `pipelime_python-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/pyproject.toml` & `pipelime_python-1.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pipelime_python-1.6.2/PKG-INFO` & `pipelime_python-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipelime-python
-Version: 1.6.2
+Version: 1.7.0
 Summary: Data workflows, cli and dataflow automation.
 Project-URL: Source, https://github.com/eyecan-ai/pipelime-python
 Project-URL: Issues, https://github.com/eyecan-ai/pipelime-python/issues
 Project-URL: Documentation, http://pipelime-python.readthedocs.io/
 Author-email: "Eyecan.ai" <info@eyecan.ai>
 License: GNU General Public License v3 (GPLv3)
 License-File: LICENSE
```

