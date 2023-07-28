# Comparing `tmp/tyro-0.5.4.tar.gz` & `tmp/tyro-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tyro-0.5.4.tar", last modified: Wed Jul  5 23:22:33 2023, max compression
+gzip compressed data, was "tyro-0.5.5.tar", last modified: Fri Jul 28 10:19:30 2023, max compression
```

## Comparing `tyro-0.5.4.tar` & `tyro-0.5.5.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:22:33.097649 tyro-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-05 23:20:00.000000 tyro-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-05 23:22:33.097649 tyro-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-05 23:22:27.000000 tyro-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:22:33.053649 tyro-0.5.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:22:33.053649 tyro-0.5.4/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-07-05 23:20:00.000000 tyro-0.5.4/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-07-05 23:20:00.000000 tyro-0.5.4/docs/update_example_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:22:33.053649 tyro-0.5.4/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:22:33.057649 tyro-0.5.4/examples/01_basics/
--rwxr-xr-x   0 runner    (1001) docker     (123)      587 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/01_basics/01_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/01_basics/02_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/01_basics/03_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/01_basics/04_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/01_basics/05_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/01_basics/06_literals.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/01_basics/07_unions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:22:33.061649 tyro-0.5.4/examples/02_nesting/
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/02_nesting/01_nesting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/02_nesting/02_subcommands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/02_nesting/03_multiple_subcommands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/02_nesting/04_nesting_in_containers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:22:33.061649 tyro-0.5.4/examples/03_config_systems/
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/03_config_systems/01_base_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/03_config_systems/02_overriding_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:22:33.065649 tyro-0.5.4/examples/04_additional/
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/04_additional/01_positional_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/04_additional/02_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/04_additional/03_tuples.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/04_additional/04_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/04_additional/05_generics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/04_additional/06_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/04_additional/07_flax.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/04_additional/08_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/04_additional/09_attrs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      420 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/_rename_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-05 23:20:00.000000 tyro-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 23:22:33.097649 tyro-0.5.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:22:33.081649 tyro-0.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_attrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_boolean_optional.py
--rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)    24964 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    17085 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_dcargs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_dict_namedtuple.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_dynamic_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_flax_ignore_py310.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_forward_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11505 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_generics_and_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)    15345 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_helptext.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_initvar_ignore_py37.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_is_nested_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_missing_optional_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_mixed_unions.py
--rw-r--r--   0 runner    (1001) docker     (123)    26765 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     9786 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_nested_in_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_new_style_annotations_above_py39.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_new_style_annotations_only_py310.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_partial.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_positional_ignore_py37.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_union_from_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_unsafe_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_unsupported_but_should_work.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:22:33.093649 tyro-0.5.4/tyro/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22530 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/_argparse_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19335 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/_calling.py
--rw-r--r--   0 runner    (1001) docker     (123)    15722 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)    31032 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    23376 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/_instantiators.py
--rw-r--r--   0 runner    (1001) docker     (123)    21278 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/_singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/_strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/_subcommand_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/_unsafe_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:22:33.093649 tyro-0.5.4/tyro/conf/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/conf/_confstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/conf/_markers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:22:33.097649 tyro-0.5.4/tyro/extras/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/extras/_base_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/extras/_choices_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/extras/_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:22:33.093649 tyro-0.5.4/tyro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-05 23:22:33.000000 tyro-0.5.4/tyro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-05 23:22:33.000000 tyro-0.5.4/tyro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 23:22:33.000000 tyro-0.5.4/tyro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-05 23:22:33.000000 tyro-0.5.4/tyro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-05 23:22:33.000000 tyro-0.5.4/tyro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:19:30.944375 tyro-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-28 10:16:54.000000 tyro-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-28 10:19:30.944375 tyro-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-07-28 10:19:24.000000 tyro-0.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:19:30.916374 tyro-0.5.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:19:30.916374 tyro-0.5.5/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-07-28 10:16:54.000000 tyro-0.5.5/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-07-28 10:16:54.000000 tyro-0.5.5/docs/update_example_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:19:30.916374 tyro-0.5.5/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:19:30.920374 tyro-0.5.5/examples/01_basics/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      587 2023-07-28 10:16:54.000000 tyro-0.5.5/examples/01_basics/01_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-28 10:16:54.000000 tyro-0.5.5/examples/01_basics/02_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-28 10:16:54.000000 tyro-0.5.5/examples/01_basics/03_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-28 10:16:54.000000 tyro-0.5.5/examples/01_basics/04_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-28 10:16:54.000000 tyro-0.5.5/examples/01_basics/05_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-28 10:16:54.000000 tyro-0.5.5/examples/01_basics/06_literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-28 10:16:54.000000 tyro-0.5.5/examples/01_basics/07_unions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:19:30.920374 tyro-0.5.5/examples/02_nesting/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-28 10:16:54.000000 tyro-0.5.5/examples/02_nesting/01_nesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-28 10:16:54.000000 tyro-0.5.5/examples/02_nesting/02_subcommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-28 10:16:54.000000 tyro-0.5.5/examples/02_nesting/03_multiple_subcommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-28 10:16:54.000000 tyro-0.5.5/examples/02_nesting/04_nesting_in_containers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:19:30.924374 tyro-0.5.5/examples/03_config_systems/
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-28 10:16:54.000000 tyro-0.5.5/examples/03_config_systems/01_base_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-28 10:16:54.000000 tyro-0.5.5/examples/03_config_systems/02_overriding_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:19:30.924374 tyro-0.5.5/examples/04_additional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-28 10:16:54.000000 tyro-0.5.5/examples/04_additional/01_positional_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-28 10:16:54.000000 tyro-0.5.5/examples/04_additional/02_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-28 10:16:54.000000 tyro-0.5.5/examples/04_additional/03_tuples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-28 10:16:54.000000 tyro-0.5.5/examples/04_additional/04_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-28 10:16:54.000000 tyro-0.5.5/examples/04_additional/05_generics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-28 10:16:54.000000 tyro-0.5.5/examples/04_additional/06_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-28 10:16:54.000000 tyro-0.5.5/examples/04_additional/07_flax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-28 10:16:54.000000 tyro-0.5.5/examples/04_additional/08_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-28 10:16:54.000000 tyro-0.5.5/examples/04_additional/09_attrs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      420 2023-07-28 10:16:54.000000 tyro-0.5.5/examples/_rename_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-28 10:16:54.000000 tyro-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 10:19:30.944375 tyro-0.5.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:19:30.936374 tyro-0.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-28 10:16:54.000000 tyro-0.5.5/tests/test_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-28 10:16:54.000000 tyro-0.5.5/tests/test_boolean_optional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-07-28 10:16:54.000000 tyro-0.5.5/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-28 10:16:54.000000 tyro-0.5.5/tests/test_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24964 2023-07-28 10:16:54.000000 tyro-0.5.5/tests/test_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17085 2023-07-28 10:16:54.000000 tyro-0.5.5/tests/test_dcargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-07-28 10:16:54.000000 tyro-0.5.5/tests/test_dict_namedtuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-28 10:16:54.000000 tyro-0.5.5/tests/test_dynamic_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-28 10:16:54.000000 tyro-0.5.5/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-28 10:16:54.000000 tyro-0.5.5/tests/test_flax_min_py38.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-28 10:16:54.000000 tyro-0.5.5/tests/test_forward_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-07-28 10:16:54.000000 tyro-0.5.5/tests/test_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11505 2023-07-28 10:16:54.000000 tyro-0.5.5/tests/test_generics_and_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15345 2023-07-28 10:16:54.000000 tyro-0.5.5/tests/test_helptext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-28 10:16:54.000000 tyro-0.5.5/tests/test_initvar_min_py38.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-28 10:16:54.000000 tyro-0.5.5/tests/test_is_nested_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-28 10:16:54.000000 tyro-0.5.5/tests/test_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-28 10:16:54.000000 tyro-0.5.5/tests/test_missing_optional_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-28 10:16:54.000000 tyro-0.5.5/tests/test_mixed_unions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28822 2023-07-28 10:16:54.000000 tyro-0.5.5/tests/test_nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9786 2023-07-28 10:16:54.000000 tyro-0.5.5/tests/test_nested_in_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-28 10:16:54.000000 tyro-0.5.5/tests/test_new_style_annotations_min_py310.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-28 10:16:54.000000 tyro-0.5.5/tests/test_new_style_annotations_min_py39.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-28 10:16:54.000000 tyro-0.5.5/tests/test_partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-28 10:16:54.000000 tyro-0.5.5/tests/test_positional_min_py38.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-07-28 10:16:54.000000 tyro-0.5.5/tests/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-28 10:16:54.000000 tyro-0.5.5/tests/test_strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-28 10:16:54.000000 tyro-0.5.5/tests/test_union_from_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-28 10:16:54.000000 tyro-0.5.5/tests/test_unsafe_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-28 10:16:54.000000 tyro-0.5.5/tests/test_unsupported_but_should_work.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:19:30.940374 tyro-0.5.5/tyro/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-28 10:16:54.000000 tyro-0.5.5/tyro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22530 2023-07-28 10:16:54.000000 tyro-0.5.5/tyro/_argparse_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19291 2023-07-28 10:16:54.000000 tyro-0.5.5/tyro/_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-07-28 10:16:54.000000 tyro-0.5.5/tyro/_calling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15687 2023-07-28 10:16:54.000000 tyro-0.5.5/tyro/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-28 10:16:54.000000 tyro-0.5.5/tyro/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-07-28 10:16:54.000000 tyro-0.5.5/tyro/_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31032 2023-07-28 10:16:54.000000 tyro-0.5.5/tyro/_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23376 2023-07-28 10:16:54.000000 tyro-0.5.5/tyro/_instantiators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20970 2023-07-28 10:16:54.000000 tyro-0.5.5/tyro/_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-07-28 10:16:54.000000 tyro-0.5.5/tyro/_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-28 10:16:54.000000 tyro-0.5.5/tyro/_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-07-28 10:16:54.000000 tyro-0.5.5/tyro/_strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-07-28 10:16:54.000000 tyro-0.5.5/tyro/_subcommand_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-28 10:16:54.000000 tyro-0.5.5/tyro/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-28 10:16:54.000000 tyro-0.5.5/tyro/_unsafe_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:19:30.944375 tyro-0.5.5/tyro/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-28 10:16:54.000000 tyro-0.5.5/tyro/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-28 10:16:54.000000 tyro-0.5.5/tyro/conf/_confstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-28 10:16:54.000000 tyro-0.5.5/tyro/conf/_markers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:19:30.944375 tyro-0.5.5/tyro/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-28 10:16:54.000000 tyro-0.5.5/tyro/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-28 10:16:54.000000 tyro-0.5.5/tyro/extras/_base_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-28 10:16:54.000000 tyro-0.5.5/tyro/extras/_choices_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-07-28 10:16:54.000000 tyro-0.5.5/tyro/extras/_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 10:16:54.000000 tyro-0.5.5/tyro/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:19:30.944375 tyro-0.5.5/tyro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-28 10:19:30.000000 tyro-0.5.5/tyro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-07-28 10:19:30.000000 tyro-0.5.5/tyro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:19:30.000000 tyro-0.5.5/tyro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-28 10:19:30.000000 tyro-0.5.5/tyro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 10:19:30.000000 tyro-0.5.5/tyro.egg-info/top_level.txt
```

### Comparing `tyro-0.5.4/LICENSE` & `tyro-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/PKG-INFO` & `tyro-0.5.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tyro
-Version: 0.5.4
+Version: 0.5.5
 Summary: Strongly typed, zero-effort CLI interfaces
 Author-email: brentyi <brentyi@berkeley.edu>
 License: MIT
 Project-URL: GitHub, https://github.com/brentyi/tyro
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -157,11 +157,11 @@
   distributed training of large language models in JAX.
 - [kevinzakka/obj2mjcf](https://github.com/kevinzakka/obj2mjcf) is an interface
   for processing composite Wavefront OBJ files for Mujoco.
 - [blurgyy/jaxngp](https://github.com/blurgyy/jaxngp) is a CUDA-accelerated
   implementation of [instant-ngp](https://nvlabs.github.io/instant-ngp/),
   implemented in JAX.
 - [NVIDIAGameWorks/kaolin-wisp](https://github.com/NVIDIAGameWorks/kaolin-wisp)
-  is a PyTorch library for working with neural fields.
+  combines `tyro` with [`hydra-zen`](https://github.com/mit-ll-responsible-ai/hydra-zen)
+  for neural fields in PyTorch.
 - [openrlbenchmark/openrlbenchmark](https://github.com/openrlbenchmark/openrlbenchmark)
-  is a comprehensive collection of tracked experiments for reinforcement
-  learning.
+  is a collection of tracked experiments for reinforcement learning.
```

### Comparing `tyro-0.5.4/README.md` & `tyro-0.5.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -137,11 +137,11 @@
   distributed training of large language models in JAX.
 - [kevinzakka/obj2mjcf](https://github.com/kevinzakka/obj2mjcf) is an interface
   for processing composite Wavefront OBJ files for Mujoco.
 - [blurgyy/jaxngp](https://github.com/blurgyy/jaxngp) is a CUDA-accelerated
   implementation of [instant-ngp](https://nvlabs.github.io/instant-ngp/),
   implemented in JAX.
 - [NVIDIAGameWorks/kaolin-wisp](https://github.com/NVIDIAGameWorks/kaolin-wisp)
-  is a PyTorch library for working with neural fields.
+  combines `tyro` with [`hydra-zen`](https://github.com/mit-ll-responsible-ai/hydra-zen)
+  for neural fields in PyTorch.
 - [openrlbenchmark/openrlbenchmark](https://github.com/openrlbenchmark/openrlbenchmark)
-  is a comprehensive collection of tracked experiments for reinforcement
-  learning.
+  is a collection of tracked experiments for reinforcement learning.
```

### Comparing `tyro-0.5.4/docs/source/conf.py` & `tyro-0.5.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/docs/update_example_docs.py` & `tyro-0.5.5/docs/update_example_docs.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/examples/01_basics/01_functions.py` & `tyro-0.5.5/examples/01_basics/01_functions.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/examples/01_basics/02_dataclasses.py` & `tyro-0.5.5/examples/01_basics/02_dataclasses.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/examples/01_basics/03_containers.py` & `tyro-0.5.5/examples/01_basics/03_containers.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/examples/01_basics/04_enums.py` & `tyro-0.5.5/examples/01_basics/04_enums.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/examples/01_basics/05_flags.py` & `tyro-0.5.5/examples/01_basics/05_flags.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/examples/01_basics/06_literals.py` & `tyro-0.5.5/examples/01_basics/06_literals.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/examples/01_basics/07_unions.py` & `tyro-0.5.5/examples/01_basics/07_unions.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/examples/02_nesting/01_nesting.py` & `tyro-0.5.5/examples/02_nesting/01_nesting.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/examples/02_nesting/02_subcommands.py` & `tyro-0.5.5/examples/02_nesting/02_subcommands.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/examples/02_nesting/03_multiple_subcommands.py` & `tyro-0.5.5/examples/02_nesting/03_multiple_subcommands.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/examples/02_nesting/04_nesting_in_containers.py` & `tyro-0.5.5/examples/02_nesting/04_nesting_in_containers.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/examples/03_config_systems/01_base_configs.py` & `tyro-0.5.5/examples/03_config_systems/01_base_configs.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/examples/03_config_systems/02_overriding_yaml.py` & `tyro-0.5.5/examples/03_config_systems/02_overriding_yaml.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/examples/04_additional/01_positional_args.py` & `tyro-0.5.5/examples/04_additional/01_positional_args.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/examples/04_additional/02_dictionaries.py` & `tyro-0.5.5/examples/04_additional/02_dictionaries.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/examples/04_additional/03_tuples.py` & `tyro-0.5.5/examples/04_additional/03_tuples.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/examples/04_additional/04_classes.py` & `tyro-0.5.5/examples/04_additional/04_classes.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/examples/04_additional/05_generics.py` & `tyro-0.5.5/examples/04_additional/05_generics.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/examples/04_additional/06_conf.py` & `tyro-0.5.5/examples/04_additional/06_conf.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/examples/04_additional/07_flax.py` & `tyro-0.5.5/examples/04_additional/07_flax.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/examples/04_additional/08_pydantic.py` & `tyro-0.5.5/examples/04_additional/08_pydantic.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/examples/04_additional/09_attrs.py` & `tyro-0.5.5/examples/04_additional/09_attrs.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/pyproject.toml` & `tyro-0.5.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tyro"
 authors = [
     {name = "brentyi", email = "brentyi@berkeley.edu"},
 ]
-version = "0.5.4"
+version = "0.5.5"
 description = "Strongly typed, zero-effort CLI interfaces"
 readme = "README.md"
 license = { text="MIT" }
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
@@ -39,15 +39,17 @@
     "pytest-cov>=3.0.0",
     "omegaconf>=2.2.2",
     "attrs>=21.4.0",
     "torch>=1.10.0",
     "pyright>=1.1.264",
     "mypy>=0.991",
     "numpy>=1.20.0",
-    "flax>=0.6.0",
+    # As of 7/27/2023, flax install fails for Python 3.7 without pinning to an
+    # old version. But doing so breaks other Python versions.
+    "flax>=0.6.9;python_version>='3.8'", 
     "pydantic>=1.10.2",
     "coverage[toml]>=6.5.0"
 ]
 
 [project.urls]
 "GitHub" = "https://github.com/brentyi/tyro"
```

### Comparing `tyro-0.5.4/tests/test_attrs.py` & `tyro-0.5.5/tests/test_attrs.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tests/test_boolean_optional.py` & `tyro-0.5.5/tests/test_boolean_optional.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tests/test_collections.py` & `tyro-0.5.5/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tests/test_completion.py` & `tyro-0.5.5/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tests/test_conf.py` & `tyro-0.5.5/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tests/test_dcargs.py` & `tyro-0.5.5/tests/test_dcargs.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tests/test_dict_namedtuple.py` & `tyro-0.5.5/tests/test_dict_namedtuple.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tests/test_errors.py` & `tyro-0.5.5/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tests/test_flax_ignore_py310.py` & `tyro-0.5.5/tests/test_flax_min_py38.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tests/test_forward_ref.py` & `tyro-0.5.5/tests/test_forward_ref.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tests/test_functools.py` & `tyro-0.5.5/tests/test_functools.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tests/test_generics_and_serialization.py` & `tyro-0.5.5/tests/test_generics_and_serialization.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tests/test_helptext.py` & `tyro-0.5.5/tests/test_helptext.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tests/test_initvar_ignore_py37.py` & `tyro-0.5.5/tests/test_initvar_min_py38.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tests/test_is_nested_type.py` & `tyro-0.5.5/tests/test_is_nested_type.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tests/test_missing.py` & `tyro-0.5.5/tests/test_missing.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tests/test_missing_optional_packages.py` & `tyro-0.5.5/tests/test_missing_optional_packages.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tests/test_mixed_unions.py` & `tyro-0.5.5/tests/test_mixed_unions.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tests/test_nested.py` & `tyro-0.5.5/tests/test_nested.py`

 * *Files 6% similar despite different names*

```diff
@@ -165,14 +165,75 @@
 
     assert tyro.cli(
         OptionalNested,
         args=["--x", "1", "b:optional-nested-child", "--b.y", "2", "--b.z", "3"],
     ) == OptionalNested(x=1, b=OptionalNestedChild(y=2, z=3))
 
 
+def test_optional_nested_multiple() -> None:
+    """Adapted from: https://github.com/brentyi/tyro/issues/60"""
+
+    @dataclasses.dataclass(frozen=True)
+    class OutputHeadSettings:
+        number_of_outputs: int = 1
+
+    @dataclasses.dataclass(frozen=True)
+    class OptimizerSettings:
+        name: str = "adam"
+
+    @dataclasses.dataclass(frozen=True)
+    class ModelSettings:
+        output_head_settings: Optional[OutputHeadSettings] = None
+        optimizer_settings: Optional[OptimizerSettings] = None
+
+    assert tyro.cli(
+        ModelSettings,
+        args="output-head-settings:None optimizer-settings:None".split(" "),
+    ) == ModelSettings(None, None)
+
+    with pytest.raises(SystemExit):
+        # Order cannot be flipped, unfortunately.
+        tyro.cli(
+            ModelSettings,
+            args="optimizer-settings:None output-head-settings:None".split(" "),
+        )
+
+    assert tyro.cli(
+        ModelSettings,
+        args="output-head-settings:output-head-settings optimizer-settings:None".split(
+            " "
+        ),
+    ) == ModelSettings(OutputHeadSettings(1), None)
+
+    assert tyro.cli(
+        ModelSettings,
+        args="output-head-settings:output-head-settings --output-head-settings.number-of-outputs 5 optimizer-settings:None".split(
+            " "
+        ),
+    ) == ModelSettings(OutputHeadSettings(5), None)
+
+    assert tyro.cli(
+        tyro.conf.OmitSubcommandPrefixes[
+            tyro.conf.ConsolidateSubcommandArgs[ModelSettings]
+        ],
+        args="output-head-settings:output-head-settings optimizer-settings:None --number-of-outputs 5".split(
+            " "
+        ),
+    ) == ModelSettings(OutputHeadSettings(5), None)
+
+    assert tyro.cli(
+        tyro.conf.OmitSubcommandPrefixes[
+            tyro.conf.ConsolidateSubcommandArgs[ModelSettings]
+        ],
+        args="output-head-settings:output-head-settings optimizer-settings:optimizer-settings --name sgd --number-of-outputs 5".split(
+            " "
+        ),
+    ) == ModelSettings(OutputHeadSettings(5), OptimizerSettings("sgd"))
+
+
 def test_subparser() -> None:
     @dataclasses.dataclass
     class HTTPServer:
         y: int
 
     @dataclasses.dataclass
     class SMTPServer:
```

### Comparing `tyro-0.5.4/tests/test_nested_in_containers.py` & `tyro-0.5.5/tests/test_nested_in_containers.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tests/test_new_style_annotations_above_py39.py` & `tyro-0.5.5/tests/test_new_style_annotations_min_py39.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tests/test_new_style_annotations_only_py310.py` & `tyro-0.5.5/tests/test_new_style_annotations_min_py310.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tests/test_partial.py` & `tyro-0.5.5/tests/test_partial.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tests/test_positional_ignore_py37.py` & `tyro-0.5.5/tests/test_positional_min_py38.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tests/test_pydantic.py` & `tyro-0.5.5/tests/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tests/test_strings.py` & `tyro-0.5.5/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tests/test_union_from_mapping.py` & `tyro-0.5.5/tests/test_union_from_mapping.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tests/test_unsupported_but_should_work.py` & `tyro-0.5.5/tests/test_unsupported_but_should_work.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tyro/_argparse_formatter.py` & `tyro-0.5.5/tyro/_argparse_formatter.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tyro/_arguments.py` & `tyro-0.5.5/tyro/_arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -394,17 +394,14 @@
 
     primary_help = arg.field.helptext
 
     if primary_help is None and _markers.Positional in arg.field.markers:
         primary_help = _strings.make_field_name([arg.name_prefix, arg.field.name])
 
     if primary_help is not None and primary_help != "":
-        # Note that the percent symbol needs some extra handling in argparse.
-        # https://stackoverflow.com/questions/21168120/python-argparse-errors-with-in-help-string
-        primary_help = primary_help.replace("%", "%%")
         help_parts.append(_rich_tag_if_enabled(primary_help, "helptext"))
 
     default = lowered.default
     if lowered.is_fixed() or lowered.action == "append":
         # Cases where we'll be missing the lowered default. Use field default instead.
         assert default in _fields.MISSING_SINGLETONS or default is None
         default = arg.field.default
@@ -440,15 +437,17 @@
             default_text = f"(default: {' '.join(default_parts)})"
         else:
             default_text = f"(default: {shlex.quote(str(default))})"
         help_parts.append(_rich_tag_if_enabled(default_text, "helptext_default"))
     else:
         help_parts.append(_rich_tag_if_enabled("(required)", "helptext_required"))
 
-    return dataclasses.replace(lowered, help=" ".join(help_parts))
+    # Note that the percent symbol needs some extra handling in argparse.
+    # https://stackoverflow.com/questions/21168120/python-argparse-errors-with-in-help-string
+    return dataclasses.replace(lowered, help=" ".join(help_parts).replace("%", "%%"))
 
 
 def _rule_set_name_or_flag_and_dest(
     arg: ArgumentDefinition,
     lowered: LoweredArgumentDefinition,
 ) -> LoweredArgumentDefinition:
     name_or_flag = _strings.make_field_name(
```

### Comparing `tyro-0.5.4/tyro/_calling.py` & `tyro-0.5.5/tyro/_calling.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,49 +139,44 @@
                 # No subparser selected -- this should only happen when we have a
                 # default/default_factory set.
                 assert (
                     type(None) in get_args(field_type)
                     or subparser_def.default_instance is not None
                 )
                 value = subparser_def.default_instance
-            elif (
-                subparser_def.can_be_none
-                and subparser_name
-                == _strings.subparser_name_from_type(prefixed_field_name, None)
-            ):
-                # do either
-                # Optional[Union[A, B, ...]] or Union[A, B, None], or have a
-                # default/default_factory set.
-                value = None
             else:
                 options = map(
                     lambda x: _resolver.apply_type_from_typevar(x, type_from_typevar),
                     get_args(_resolver.unwrap_annotated(field_type)[0]),
                 )
                 chosen_f = None
                 for option in options:
                     if (
                         _strings.subparser_name_from_type(prefixed_field_name, option)
                         == subparser_name
                     ):
                         chosen_f = option
                         break
                 assert chosen_f is not None
-                value, consumed_keywords_child = call_from_args(
-                    chosen_f,
-                    subparser_def.parser_from_name[subparser_name],
-                    (
-                        field.default
-                        if type(field.default) is chosen_f
-                        else _fields.MISSING_NONPROP
-                    ),
-                    value_from_prefixed_field_name,
-                    field_name_prefix=prefixed_field_name,
-                )
-                consumed_keywords |= consumed_keywords_child
+
+                if chosen_f is type(None):
+                    value = None
+                else:
+                    value, consumed_keywords_child = call_from_args(
+                        chosen_f,
+                        subparser_def.parser_from_name[subparser_name],
+                        (
+                            field.default
+                            if type(field.default) is chosen_f
+                            else _fields.MISSING_NONPROP
+                        ),
+                        value_from_prefixed_field_name,
+                        field_name_prefix=prefixed_field_name,
+                    )
+                    consumed_keywords |= consumed_keywords_child
 
         if value is _fields.EXCLUDE_FROM_CALL:
             continue
 
         if _markers._UnpackArgsCall in field.markers:
             assert isinstance(value, tuple)
             positional_args.extend(value)
```

### Comparing `tyro-0.5.4/tyro/_cli.py` & `tyro-0.5.5/tyro/_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,24 +283,22 @@
 
     # We wrap our type with a dummy dataclass if it can't be treated as a nested type.
     # For example: passing in f=int will result in a dataclass with a single field
     # typed as int.
     if not _fields.is_nested_type(cast(type, f), default_instance_internal):
         dummy_field = cast(
             dataclasses.Field,
-            dataclasses.field(
-                default_factory=lambda: default
-                if default is not None
-                else dataclasses.MISSING
-            ),
+            dataclasses.field(),
         )
         f = dataclasses.make_dataclass(
             cls_name="",
             fields=[(_strings.dummy_field_name, cast(type, f), dummy_field)],
+            frozen=True,
         )
+        default_instance_internal = f(default_instance_internal)  # type: ignore
         dummy_wrapped = True
     else:
         dummy_wrapped = False
 
     # Read and fix arguments. If the user passes in --field_name instead of
     # --field-name, correct for them.
     args = list(sys.argv[1:]) if args is None else list(args)
```

### Comparing `tyro-0.5.4/tyro/_docstrings.py` & `tyro-0.5.5/tyro/_docstrings.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tyro/_fields.py` & `tyro-0.5.5/tyro/_fields.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tyro/_instantiators.py` & `tyro-0.5.5/tyro/_instantiators.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tyro/_parsers.py` & `tyro-0.5.5/tyro/_parsers.py`

 * *Files 3% similar despite different names*

```diff
@@ -333,62 +333,68 @@
 
     name: str
     description: Optional[str]
     parser_from_name: Dict[str, ParserSpecification]
     prefix: str
     required: bool
     default_instance: Any
-    can_be_none: bool  # If underlying type is Optional[Something].
 
     @staticmethod
     def from_field(
         field: _fields.FieldDefinition,
         type_from_typevar: Dict[TypeVar, TypeForm[Any]],
         parent_classes: Set[Type[Any]],
         prefix: str,
     ) -> Optional[SubparsersSpecification]:
         # Union of classes should create subparsers.
         typ = _resolver.unwrap_annotated(field.typ)[0]
         if get_origin(typ) is not Union:
             return None
 
         # We don't use sets here to retain order of subcommands.
+        options: List[Union[type, Callable]]
         options = [
             _resolver.apply_type_from_typevar(typ, type_from_typevar)
             for typ in get_args(typ)
         ]
-        options_no_none = [o for o in options if o is not type(None)]  # noqa
+        options = [
+            # Cast seems unnecessary but needed in mypy... (1.4.1)
+            cast(Callable, none_proxy) if o is type(None) else o
+            for o in options
+        ]
         if not all(
             [
-                _fields.is_nested_type(o, _fields.MISSING_NONPROP)
-                for o in options_no_none
+                _fields.is_nested_type(cast(type, o), _fields.MISSING_NONPROP)
+                for o in options
             ]
         ):
             return None
 
         # Get subcommand configurations from `tyro.conf.subcommand()`.
         subcommand_config_from_name: Dict[
             str, _confstruct._SubcommandConfiguration
         ] = {}
         subcommand_type_from_name: Dict[str, type] = {}
-        for option in options_no_none:
-            subcommand_name = _strings.subparser_name_from_type(prefix, option)
+        for option in options:
+            subcommand_name = _strings.subparser_name_from_type(
+                prefix, type(None) if option is none_proxy else cast(type, option)
+            )
             option, found_subcommand_configs = _resolver.unwrap_annotated(
                 option, _confstruct._SubcommandConfiguration
             )
             if len(found_subcommand_configs) != 0:
                 # Explicitly annotated default.
                 assert len(found_subcommand_configs) == 1, (
                     f"Expected only one subcommand config, but {subcommand_name} has"
                     f" {len(found_subcommand_configs)}."
                 )
                 subcommand_config_from_name[subcommand_name] = found_subcommand_configs[
                     0
                 ]
-            subcommand_type_from_name[subcommand_name] = option
+            subcommand_type_from_name[subcommand_name] = cast(type, option)
 
         # If a field default is provided, try to find a matching subcommand name.
         if field.default is None or field.default in _fields.MISSING_SINGLETONS:
             default_name = None
         else:
             default_name = _subcommand_matching.match_subcommand(
                 field.default, subcommand_config_from_name, subcommand_type_from_name
@@ -397,22 +403,24 @@
                 # This should really be an error, but we can raise a warning to make
                 # hacking at subcommands easier:
                 # https://github.com/brentyi/tyro/issues/20
                 warnings.warn(
                     f"`{prefix}` was provided a default value of type"
                     f" {type(field.default)} but no matching subcommand was found. A"
                     " type may be missing in the Union type declaration for"
-                    f" `{prefix}`, which currently expects {options_no_none}."
+                    f" `{prefix}`, which currently expects {options}."
                 )
                 return None
 
         # Add subcommands for each option.
         parser_from_name: Dict[str, ParserSpecification] = {}
-        for option in options_no_none:
-            subcommand_name = _strings.subparser_name_from_type(prefix, option)
+        for option in options:
+            subcommand_name = _strings.subparser_name_from_type(
+                prefix, type(None) if option is none_proxy else cast(type, option)
+            )
             option, _ = _resolver.unwrap_annotated(option)
 
             # Get a subcommand config: either pulled from the type annotations or the
             # field default.
             if subcommand_name in subcommand_config_from_name:
                 subcommand_config = subcommand_config_from_name[subcommand_name]
             else:
@@ -491,53 +499,34 @@
             # automatically, as is done for normal fields. But for now we just rely on
             # the user to include it in the docstring.
             description=description,
             parser_from_name=parser_from_name,
             prefix=prefix,
             required=required,
             default_instance=field.default,
-            can_be_none=options != options_no_none,
         )
 
     def apply(
         self, parent_parser: argparse.ArgumentParser
     ) -> Tuple[argparse.ArgumentParser, ...]:
         title = "subcommands"
-        metavar = (
-            "{"
-            + ",".join(
-                (
-                    (_strings.subparser_name_from_type(self.prefix, None),)
-                    if self.can_be_none
-                    else ()
-                )
-                + tuple(self.parser_from_name.keys())
-            )
-            + "}"
-        )
+        metavar = "{" + ",".join(self.parser_from_name.keys()) + "}"
         if not self.required:
             title = "optional " + title
             metavar = f"[{metavar}]"
 
         # Add subparsers to every node in previous level of the tree.
         argparse_subparsers = parent_parser.add_subparsers(
             dest=_strings.make_subparser_dest(self.prefix),
             description=self.description,
             required=self.required,
             title=title,
             metavar=metavar,
         )
 
-        if self.can_be_none:
-            subparser = argparse_subparsers.add_parser(
-                name=_strings.subparser_name_from_type(self.prefix, None),
-                formatter_class=_argparse_formatter.TyroArgparseHelpFormatter,
-                help="",
-            )
-
         subparser_tree_leaves: List[argparse.ArgumentParser] = []
         for name, subparser_def in self.parser_from_name.items():
             helptext = subparser_def.description.replace("%", "%%")
             if len(helptext) > 0:
                 # TODO: calling a private function here.
                 helptext = _arguments._rich_tag_if_enabled(helptext.strip(), "helptext")
 
@@ -564,7 +553,11 @@
             subparsers=add_subparsers_to_leaves(parser.subparsers, leaf),
         )
     return dataclasses.replace(
         root,
         parser_from_name=new_parsers_from_name,
         required=root.required or leaf.required,
     )
+
+
+def none_proxy() -> None:
+    return None
```

### Comparing `tyro-0.5.4/tyro/_resolver.py` & `tyro-0.5.5/tyro/_resolver.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tyro/_strings.py` & `tyro-0.5.5/tyro/_strings.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,17 +103,17 @@
                 [cls] + list(type_from_typevar.values()),
             )
         ),
         prefix_name,
     )
 
 
-def subparser_name_from_type(prefix: str, cls: Union[Type, None]) -> str:
+def subparser_name_from_type(prefix: str, cls: Type) -> str:
     suffix, use_prefix = (
-        _subparser_name_from_type(cls) if cls is not None else ("None", True)
+        _subparser_name_from_type(cls) if cls is not type(None) else ("None", True)
     )
     if len(prefix) == 0 or not use_prefix:
         return suffix
     return f"{prefix}:{suffix}".replace("_", "-")
 
 
 @functools.lru_cache(maxsize=None)
```

### Comparing `tyro-0.5.4/tyro/_subcommand_matching.py` & `tyro-0.5.5/tyro/_subcommand_matching.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tyro/_typing.py` & `tyro-0.5.5/tyro/_typing.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tyro/_unsafe_cache.py` & `tyro-0.5.5/tyro/_unsafe_cache.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tyro/conf/__init__.py` & `tyro-0.5.5/tyro/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tyro/conf/_confstruct.py` & `tyro-0.5.5/tyro/conf/_confstruct.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tyro/conf/_markers.py` & `tyro-0.5.5/tyro/conf/_markers.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tyro/extras/__init__.py` & `tyro-0.5.5/tyro/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tyro/extras/_base_configs.py` & `tyro-0.5.5/tyro/extras/_base_configs.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tyro/extras/_choices_type.py` & `tyro-0.5.5/tyro/extras/_choices_type.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tyro/extras/_serialization.py` & `tyro-0.5.5/tyro/extras/_serialization.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.4/tyro.egg-info/PKG-INFO` & `tyro-0.5.5/tyro.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tyro
-Version: 0.5.4
+Version: 0.5.5
 Summary: Strongly typed, zero-effort CLI interfaces
 Author-email: brentyi <brentyi@berkeley.edu>
 License: MIT
 Project-URL: GitHub, https://github.com/brentyi/tyro
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -157,11 +157,11 @@
   distributed training of large language models in JAX.
 - [kevinzakka/obj2mjcf](https://github.com/kevinzakka/obj2mjcf) is an interface
   for processing composite Wavefront OBJ files for Mujoco.
 - [blurgyy/jaxngp](https://github.com/blurgyy/jaxngp) is a CUDA-accelerated
   implementation of [instant-ngp](https://nvlabs.github.io/instant-ngp/),
   implemented in JAX.
 - [NVIDIAGameWorks/kaolin-wisp](https://github.com/NVIDIAGameWorks/kaolin-wisp)
-  is a PyTorch library for working with neural fields.
+  combines `tyro` with [`hydra-zen`](https://github.com/mit-ll-responsible-ai/hydra-zen)
+  for neural fields in PyTorch.
 - [openrlbenchmark/openrlbenchmark](https://github.com/openrlbenchmark/openrlbenchmark)
-  is a comprehensive collection of tracked experiments for reinforcement
-  learning.
+  is a collection of tracked experiments for reinforcement learning.
```

### Comparing `tyro-0.5.4/tyro.egg-info/SOURCES.txt` & `tyro-0.5.5/tyro.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -31,30 +31,30 @@
 tests/test_collections.py
 tests/test_completion.py
 tests/test_conf.py
 tests/test_dcargs.py
 tests/test_dict_namedtuple.py
 tests/test_dynamic_dataclasses.py
 tests/test_errors.py
-tests/test_flax_ignore_py310.py
+tests/test_flax_min_py38.py
 tests/test_forward_ref.py
 tests/test_functools.py
 tests/test_generics_and_serialization.py
 tests/test_helptext.py
-tests/test_initvar_ignore_py37.py
+tests/test_initvar_min_py38.py
 tests/test_is_nested_type.py
 tests/test_missing.py
 tests/test_missing_optional_packages.py
 tests/test_mixed_unions.py
 tests/test_nested.py
 tests/test_nested_in_containers.py
-tests/test_new_style_annotations_above_py39.py
-tests/test_new_style_annotations_only_py310.py
+tests/test_new_style_annotations_min_py310.py
+tests/test_new_style_annotations_min_py39.py
 tests/test_partial.py
-tests/test_positional_ignore_py37.py
+tests/test_positional_min_py38.py
 tests/test_pydantic.py
 tests/test_strings.py
 tests/test_union_from_mapping.py
 tests/test_unsafe_cache.py
 tests/test_unsupported_but_should_work.py
 tyro/__init__.py
 tyro/_argparse_formatter.py
```

