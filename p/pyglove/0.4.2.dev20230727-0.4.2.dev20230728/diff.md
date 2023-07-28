# Comparing `tmp/pyglove-0.4.2.dev20230727.tar.gz` & `tmp/pyglove-0.4.2.dev20230728.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyglove-0.4.2.dev20230727.tar", last modified: Thu Jul 27 08:06:46 2023, max compression
+gzip compressed data, was "pyglove-0.4.2.dev20230728.tar", last modified: Fri Jul 28 08:06:44 2023, max compression
```

## Comparing `pyglove-0.4.2.dev20230727.tar` & `pyglove-0.4.2.dev20230728.tar`

### file list

```diff
@@ -1,196 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:06:46.668518 pyglove-0.4.2.dev20230727/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-27 08:06:46.668518 pyglove-0.4.2.dev20230727/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-27 08:06:44.000000 pyglove-0.4.2.dev20230727/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:06:46.648517 pyglove-0.4.2.dev20230727/pyglove/
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:06:46.648517 pyglove-0.4.2.dev20230727/pyglove/core/
--rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:06:46.648517 pyglove-0.4.2.dev20230727/pyglove/core/detouring/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/detouring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/detouring/class_detour.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/detouring/class_detour_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:06:46.652517 pyglove-0.4.2.dev20230727/pyglove/core/geno/
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/geno/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64370 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/geno/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/geno/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/geno/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/geno/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/geno/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/geno/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/geno/deduping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/geno/deduping_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/geno/dna_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/geno/dna_generator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/geno/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/geno/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/geno/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/geno/random_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/geno/space.py
--rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/geno/space_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/geno/sweeping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/geno/sweeping_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:06:46.652517 pyglove-0.4.2.dev20230727/pyglove/core/hyper/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/hyper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/hyper/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/hyper/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/hyper/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/hyper/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/hyper/derived.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/hyper/derived_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/hyper/dynamic_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/hyper/dynamic_evaluation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/hyper/evolvable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/hyper/evolvable_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/hyper/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/hyper/iter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/hyper/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/hyper/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/hyper/object_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/hyper/object_template_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/logging_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:06:46.656518 pyglove-0.4.2.dev20230727/pyglove/core/object_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/object_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/object_utils/codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/object_utils/codegen_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/object_utils/common_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/object_utils/common_traits_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/object_utils/docstr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/object_utils/docstr_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/object_utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/object_utils/formatting_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/object_utils/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/object_utils/hierarchical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/object_utils/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/object_utils/missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/object_utils/thread_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/object_utils/thread_local_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18160 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/object_utils/value_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/object_utils/value_location_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:06:46.656518 pyglove-0.4.2.dev20230727/pyglove/core/patching/
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/patching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/patching/object_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/patching/object_factory_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/patching/pattern_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/patching/pattern_based_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/patching/rule_based.py
--rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/patching/rule_based_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:06:46.660518 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/
--rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    78519 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/boilerplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/boilerplate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22447 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/class_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/class_wrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10884 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/compounding.py
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/compounding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/contextual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/contextual_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    35745 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    64268 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/dict_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/diff_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/flags_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    23955 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/functor.py
--rw-r--r--   0 runner    (1001) docker     (123)    29174 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/functor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    30269 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    57466 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/list_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    36446 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    84646 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/origin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/origin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/pure_symbolic.py
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/symbolize.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/symbolic/symbolize_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:06:46.660518 pyglove-0.4.2.dev20230727/pyglove/core/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/tuning/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/tuning/backend_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/tuning/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/tuning/local_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/tuning/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/tuning/protocols_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/tuning/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/tuning/sample_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:06:46.664518 pyglove-0.4.2.dev20230727/pyglove/core/typing/
--rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/typing/annotation_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/typing/annotation_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/typing/callable_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/typing/callable_ext_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/typing/callable_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/typing/callable_signature_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    49558 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/typing/class_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/typing/class_schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/typing/class_schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/typing/class_schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/typing/custom_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/typing/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/typing/generic_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/typing/key_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/typing/key_specs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/typing/pytype_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/typing/type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/typing/type_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/typing/typed_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/typing/typed_missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    79809 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/typing/value_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)   105460 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/core/typing/value_specs_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:06:46.664518 pyglove-0.4.2.dev20230727/pyglove/ext/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:06:46.664518 pyglove-0.4.2.dev20230727/pyglove/ext/early_stopping/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/early_stopping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/early_stopping/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/early_stopping/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/early_stopping/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/early_stopping/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:06:46.668518 pyglove-0.4.2.dev20230727/pyglove/ext/evolution/
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/evolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/evolution/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/evolution/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/evolution/hill_climb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/evolution/hill_climb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/evolution/mutators.py
--rw-r--r--   0 runner    (1001) docker     (123)    17975 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/evolution/mutators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/evolution/neat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/evolution/neat_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/evolution/nsga2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/evolution/nsga2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/evolution/recombinators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/evolution/recombinators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/evolution/regularized_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/evolution/regularized_evolution_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/evolution/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/evolution/selectors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/evolution/where.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/evolution/where_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:06:46.668518 pyglove-0.4.2.dev20230727/pyglove/ext/mutfun/
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/mutfun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/mutfun/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/mutfun/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/mutfun/basic_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/mutfun/basic_ops_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:06:46.668518 pyglove-0.4.2.dev20230727/pyglove/ext/scalars/
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/scalars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/scalars/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/scalars/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/scalars/maths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/scalars/maths_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/scalars/randoms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/scalars/randoms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/scalars/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/pyglove/ext/scalars/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:06:46.648517 pyglove-0.4.2.dev20230727/pyglove.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-27 08:06:46.000000 pyglove-0.4.2.dev20230727/pyglove.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-07-27 08:06:46.000000 pyglove-0.4.2.dev20230727/pyglove.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 08:06:46.000000 pyglove-0.4.2.dev20230727/pyglove.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 08:06:46.000000 pyglove-0.4.2.dev20230727/pyglove.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-27 08:06:46.000000 pyglove-0.4.2.dev20230727/pyglove.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 08:06:46.668518 pyglove-0.4.2.dev20230727/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-27 08:06:33.000000 pyglove-0.4.2.dev20230727/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:06:44.075424 pyglove-0.4.2.dev20230728/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-28 08:06:44.075424 pyglove-0.4.2.dev20230728/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-28 08:06:42.000000 pyglove-0.4.2.dev20230728/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:06:44.059424 pyglove-0.4.2.dev20230728/pyglove/
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:06:44.059424 pyglove-0.4.2.dev20230728/pyglove/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:06:44.059424 pyglove-0.4.2.dev20230728/pyglove/core/detouring/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/detouring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/detouring/class_detour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/detouring/class_detour_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:06:44.063423 pyglove-0.4.2.dev20230728/pyglove/core/geno/
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/geno/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64411 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/geno/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/geno/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/geno/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/geno/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/geno/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/geno/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/geno/deduping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/geno/deduping_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/geno/dna_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/geno/dna_generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/geno/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/geno/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/geno/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/geno/random_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/geno/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/geno/space_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/geno/sweeping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/geno/sweeping_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:06:44.063423 pyglove-0.4.2.dev20230728/pyglove/core/hyper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/hyper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/hyper/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/hyper/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/hyper/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/hyper/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/hyper/derived.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/hyper/derived_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/hyper/dynamic_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/hyper/dynamic_evaluation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/hyper/evolvable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/hyper/evolvable_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/hyper/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/hyper/iter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/hyper/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/hyper/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/hyper/object_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/hyper/object_template_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/logging_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:06:44.063423 pyglove-0.4.2.dev20230728/pyglove/core/object_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/object_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/object_utils/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/object_utils/codegen_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15301 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/object_utils/common_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/object_utils/common_traits_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/object_utils/docstr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/object_utils/docstr_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/object_utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/object_utils/formatting_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/object_utils/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/object_utils/hierarchical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/object_utils/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/object_utils/missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/object_utils/thread_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/object_utils/thread_local_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18160 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/object_utils/value_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/object_utils/value_location_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:06:44.063423 pyglove-0.4.2.dev20230728/pyglove/core/patching/
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/patching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/patching/object_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/patching/object_factory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/patching/pattern_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/patching/pattern_based_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/patching/rule_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/patching/rule_based_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:06:44.067424 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78519 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/boilerplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/boilerplate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22715 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/class_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/class_wrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11904 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/compounding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/compounding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/contextual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/contextual_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35745 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64268 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/dict_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/diff_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/flags_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24039 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/functor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29174 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/functor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30269 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57466 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/list_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36989 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84993 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/origin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/origin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/pure_symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/symbolize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/symbolic/symbolize_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:06:44.067424 pyglove-0.4.2.dev20230728/pyglove/core/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/tuning/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/tuning/backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/tuning/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/tuning/local_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/tuning/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/tuning/protocols_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/tuning/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/tuning/sample_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:06:44.071424 pyglove-0.4.2.dev20230728/pyglove/core/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/typing/annotation_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/typing/annotation_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/typing/callable_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/typing/callable_ext_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/typing/callable_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/typing/callable_signature_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49558 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/typing/class_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/typing/class_schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/typing/class_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/typing/class_schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/typing/custom_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/typing/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/typing/generic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/typing/key_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/typing/key_specs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/typing/pytype_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/typing/type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/typing/type_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/typing/typed_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/typing/typed_missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79809 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/typing/value_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105460 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/core/typing/value_specs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:06:44.071424 pyglove-0.4.2.dev20230728/pyglove/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:06:44.071424 pyglove-0.4.2.dev20230728/pyglove/ext/early_stopping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/early_stopping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/early_stopping/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/early_stopping/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/early_stopping/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/early_stopping/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:06:44.075424 pyglove-0.4.2.dev20230728/pyglove/ext/evolution/
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/evolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/evolution/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/evolution/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/evolution/hill_climb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/evolution/hill_climb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/evolution/mutators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17975 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/evolution/mutators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/evolution/neat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/evolution/neat_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/evolution/nsga2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/evolution/nsga2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/evolution/recombinators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/evolution/recombinators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/evolution/regularized_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/evolution/regularized_evolution_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/evolution/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/evolution/selectors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/evolution/where.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/evolution/where_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:06:44.075424 pyglove-0.4.2.dev20230728/pyglove/ext/mutfun/
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/mutfun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/mutfun/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/mutfun/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/mutfun/basic_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/mutfun/basic_ops_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:06:44.075424 pyglove-0.4.2.dev20230728/pyglove/ext/scalars/
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/scalars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/scalars/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/scalars/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/scalars/maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/scalars/maths_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/scalars/randoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/scalars/randoms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/scalars/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/pyglove/ext/scalars/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:06:44.059424 pyglove-0.4.2.dev20230728/pyglove.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-28 08:06:43.000000 pyglove-0.4.2.dev20230728/pyglove.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-07-28 08:06:44.000000 pyglove-0.4.2.dev20230728/pyglove.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:06:43.000000 pyglove-0.4.2.dev20230728/pyglove.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 08:06:43.000000 pyglove-0.4.2.dev20230728/pyglove.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-28 08:06:43.000000 pyglove-0.4.2.dev20230728/pyglove.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 08:06:44.075424 pyglove-0.4.2.dev20230728/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-28 08:06:33.000000 pyglove-0.4.2.dev20230728/setup.py
```

### Comparing `pyglove-0.4.2.dev20230727/LICENSE` & `pyglove-0.4.2.dev20230728/LICENSE`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/PKG-INFO` & `pyglove-0.4.2.dev20230728/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.4.2.dev20230727
+Version: 0.4.2.dev20230728
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.4.2.dev20230727/README.md` & `pyglove-0.4.2.dev20230728/README.md`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/__init__.py` & `pyglove-0.4.2.dev20230728/pyglove/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/__init__.py` & `pyglove-0.4.2.dev20230728/pyglove/core/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -281,14 +281,16 @@
 
 Formattable = object_utils.Formattable
 MaybePartial = object_utils.MaybePartial
 JSONConvertible = object_utils.JSONConvertible
 DocStr = object_utils.DocStr
 
 registered_types = object_utils.registered_types
+explicit_method_override = object_utils.explicit_method_override
+
 is_partial = object_utils.is_partial
 format = object_utils.format   # pylint: disable=redefined-builtin
 print = object_utils.print    # pylint: disable=redefined-builtin
 docstr = object_utils.docstr
 
 #
 # Symbols from `logging.py`.
```

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/detouring/__init__.py` & `pyglove-0.4.2.dev20230728/pyglove/core/detouring/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/detouring/class_detour.py` & `pyglove-0.4.2.dev20230728/pyglove/core/detouring/class_detour.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/detouring/class_detour_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/detouring/class_detour_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/geno/__init__.py` & `pyglove-0.4.2.dev20230728/pyglove/core/geno/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/geno/base.py` & `pyglove-0.4.2.dev20230728/pyglove/core/geno/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -491,14 +491,15 @@
     DNA('abc')
   """
   # pylint: enable=line-too-long
 
   # Allow assignment on symbolic attributes.
   allow_symbolic_assignment = True
 
+  @object_utils.explicit_method_override
   def __init__(
       self,
       value: Union[None, int, float, str, List[Any], Tuple[Any]] = None,
       # Set MISSING_VALUE to use default from pg_typing.
       children: Optional[List['DNA']] = None,
       spec: Optional[DNASpec] = None,
       metadata: Optional[Dict[str, Any]] = None,
```

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/geno/base_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/geno/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/geno/categorical.py` & `pyglove-0.4.2.dev20230728/pyglove/core/geno/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/geno/categorical_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/geno/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/geno/custom.py` & `pyglove-0.4.2.dev20230728/pyglove/core/geno/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/geno/custom_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/geno/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/geno/deduping.py` & `pyglove-0.4.2.dev20230728/pyglove/core/geno/deduping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/geno/deduping_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/geno/deduping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/geno/dna_generator.py` & `pyglove-0.4.2.dev20230728/pyglove/core/geno/dna_generator.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/geno/dna_generator_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/geno/dna_generator_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/geno/numerical.py` & `pyglove-0.4.2.dev20230728/pyglove/core/geno/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/geno/numerical_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/geno/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/geno/random.py` & `pyglove-0.4.2.dev20230728/pyglove/core/geno/random.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/geno/random_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/geno/random_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/geno/space.py` & `pyglove-0.4.2.dev20230728/pyglove/core/geno/space.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/geno/space_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/geno/space_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/geno/sweeping.py` & `pyglove-0.4.2.dev20230728/pyglove/core/geno/sweeping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/geno/sweeping_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/geno/sweeping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/hyper/__init__.py` & `pyglove-0.4.2.dev20230728/pyglove/core/hyper/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/hyper/base.py` & `pyglove-0.4.2.dev20230728/pyglove/core/hyper/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/hyper/categorical.py` & `pyglove-0.4.2.dev20230728/pyglove/core/hyper/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/hyper/categorical_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/hyper/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/hyper/custom.py` & `pyglove-0.4.2.dev20230728/pyglove/core/hyper/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/hyper/custom_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/hyper/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/hyper/derived.py` & `pyglove-0.4.2.dev20230728/pyglove/core/hyper/derived.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/hyper/derived_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/hyper/derived_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/hyper/dynamic_evaluation.py` & `pyglove-0.4.2.dev20230728/pyglove/core/hyper/dynamic_evaluation.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/hyper/dynamic_evaluation_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/hyper/dynamic_evaluation_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/hyper/evolvable.py` & `pyglove-0.4.2.dev20230728/pyglove/core/hyper/evolvable.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/hyper/evolvable_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/hyper/evolvable_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/hyper/iter.py` & `pyglove-0.4.2.dev20230728/pyglove/core/hyper/iter.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/hyper/iter_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/hyper/iter_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/hyper/numerical.py` & `pyglove-0.4.2.dev20230728/pyglove/core/hyper/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/hyper/numerical_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/hyper/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/hyper/object_template.py` & `pyglove-0.4.2.dev20230728/pyglove/core/hyper/object_template.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/hyper/object_template_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/hyper/object_template_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/logging.py` & `pyglove-0.4.2.dev20230728/pyglove/core/logging.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/logging_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/logging_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/object_utils/__init__.py` & `pyglove-0.4.2.dev20230728/pyglove/core/object_utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,14 +79,17 @@
 
 from pyglove.core.object_utils.common_traits import Formattable
 from pyglove.core.object_utils.common_traits import MaybePartial
 from pyglove.core.object_utils.common_traits import Functor
 
 from pyglove.core.object_utils.common_traits import registered_types
 
+from pyglove.core.object_utils.common_traits import explicit_method_override
+from pyglove.core.object_utils.common_traits import ensure_explicit_method_override
+
 # Value location.
 from pyglove.core.object_utils.value_location import KeyPath
 from pyglove.core.object_utils.value_location import StrKey
 
 # Value markers.
 from pyglove.core.object_utils.missing import MissingValue
 from pyglove.core.object_utils.missing import MISSING_VALUE
```

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/object_utils/codegen.py` & `pyglove-0.4.2.dev20230728/pyglove/core/object_utils/codegen.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/object_utils/codegen_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/object_utils/codegen_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/object_utils/common_traits.py` & `pyglove-0.4.2.dev20230728/pyglove/core/object_utils/common_traits.py`

 * *Files 4% similar despite different names*

```diff
@@ -404,7 +404,46 @@
     Args:
       *args: Any positional arguments.
       **kwargs: Any keyword arguments.
 
     Returns:
       Any value.
     """
+
+
+def explicit_method_override(method):
+  """Decorator that marks a member method as explicitly overridden.
+
+  In PyGlove, many methods are managed by the framework - for example -
+  ``pg.Object.__init__``. It's easy for users to override these methods
+  unconsciously. Therefore, we introduce this decorator to catch error at
+  the first place when such overrides incidentally take place, while allowing
+  advanced users to override them.
+
+  Usage::
+
+    class Foo(pg.Object):
+
+      @pg.explicit_method_override
+      def __init__(self, *args, **kwargs):
+       ...
+
+  Args:
+    method: method to explicitly overriden.
+
+  Returns:
+    The original method with an explicit overriden stamp.
+  """
+  setattr(method, '__explicit_override__', True)
+  return method
+
+
+def ensure_explicit_method_override(
+    method, error_message: Optional[str] = None) -> None:
+  """Returns True if a method is explicitly overridden."""
+  if not getattr(method, '__explicit_override__', False):
+    if error_message is None:
+      error_message = (
+          f'{method} is a PyGlove managed method. If you do need to override '
+          'it, please decorate the method with `@pg.explicit_method_override`.')
+    raise TypeError(error_message)
+
```

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/object_utils/common_traits_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/object_utils/common_traits_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -101,9 +101,26 @@
       common_traits.from_json(['__tuple__'])
 
     with self.assertRaisesRegex(
         TypeError, 'Type name .* is not registered'):
       common_traits.from_json({'_type': '__main__.ABC'})
 
 
+class ExplicitlyOverrideTest(unittest.TestCase):
+
+  def test_explicitly_override(self):
+    class A:
+
+      @common_traits.explicit_method_override
+      def __init__(self, x, y):
+        pass
+
+      def bar(self):
+        pass
+
+    common_traits.ensure_explicit_method_override(A.__init__)
+    with self.assertRaisesRegex(TypeError, '.* is a PyGlove managed method'):
+      common_traits.ensure_explicit_method_override(A.bar)
+
+
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/object_utils/docstr_utils.py` & `pyglove-0.4.2.dev20230728/pyglove/core/object_utils/docstr_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/object_utils/docstr_utils_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/object_utils/docstr_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/object_utils/formatting.py` & `pyglove-0.4.2.dev20230728/pyglove/core/object_utils/formatting.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/object_utils/formatting_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/object_utils/formatting_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/object_utils/hierarchical.py` & `pyglove-0.4.2.dev20230728/pyglove/core/object_utils/hierarchical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/object_utils/hierarchical_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/object_utils/hierarchical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/object_utils/missing.py` & `pyglove-0.4.2.dev20230728/pyglove/core/object_utils/missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/object_utils/missing_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/object_utils/missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/object_utils/thread_local.py` & `pyglove-0.4.2.dev20230728/pyglove/core/object_utils/thread_local.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/object_utils/thread_local_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/object_utils/thread_local_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/object_utils/value_location.py` & `pyglove-0.4.2.dev20230728/pyglove/core/object_utils/value_location.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/object_utils/value_location_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/object_utils/value_location_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/patching/__init__.py` & `pyglove-0.4.2.dev20230728/pyglove/core/patching/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/patching/object_factory.py` & `pyglove-0.4.2.dev20230728/pyglove/core/patching/object_factory.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/patching/object_factory_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/patching/object_factory_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/patching/pattern_based.py` & `pyglove-0.4.2.dev20230728/pyglove/core/patching/pattern_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/patching/pattern_based_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/patching/pattern_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/patching/rule_based.py` & `pyglove-0.4.2.dev20230728/pyglove/core/patching/rule_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/patching/rule_based_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/patching/rule_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/symbolic/__init__.py` & `pyglove-0.4.2.dev20230728/pyglove/core/symbolic/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/symbolic/base.py` & `pyglove-0.4.2.dev20230728/pyglove/core/symbolic/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/symbolic/base_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/symbolic/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/symbolic/boilerplate.py` & `pyglove-0.4.2.dev20230728/pyglove/core/symbolic/boilerplate.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/symbolic/boilerplate_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/symbolic/boilerplate_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/symbolic/class_wrapper.py` & `pyglove-0.4.2.dev20230728/pyglove/core/symbolic/class_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,15 @@
   # class and __init__ docstrings.
   auto_doc = False
 
   # If True, PyGlove typing will be enabled based on type annotations from
   # the `__init__` method.
   auto_typing = False
 
+  @object_utils.explicit_method_override
   def __init__(self, *args, **kwargs):
     """Overridden __init__ to construct symbolic wrapper only."""
     # NOTE(daiyip): We avoid `__init__` to be called multiple times.
     # This behavior is intended for a use case that detours a source class to
     # a function that returns an instance of the source class' symbolic
     # wrapper. The function may want to pass modified arguments to the
     # symbolic wrapper's `__init__`, but since the symbolic wrapper is a
@@ -95,14 +96,18 @@
   @property
   def wrapped_cls_initialized(self):
     """Returns True if wrapped class is initialized. Otherwise False."""
     return getattr(self, '_wrapped_cls_initialized', False)
 
   @classmethod
   def __init_subclass__(cls):
+    # Class wrappers inherit `__init__` from the user class. Therefore, we mark
+    # all of them as explicitly overridden.
+    object_utils.explicit_method_override(cls.__init__)
+
     super().__init_subclass__()
     if cls.__init__ is _SubclassedWrapperBase.__init__:
       # Symbolized class inherits __init__ from ClassWrapper, meaning that
       # neither it defines its own __init__ nor inherits __init__ from any
       # non-symbolic bases. In such case we use object.__init__ as the original
       # __init__ method.
       cls.__init__ = object.__init__
@@ -121,14 +126,16 @@
       # This means the class is either wrapped from a user class
       # or subclassing a symbolic wrapper with its own __init__.
       # In both cases, we need to generate an __init__ wrapper for
       # calling the symbolic initialization.
       setattr(cls, '__orig_init__', cls.__init__)
       description, init_arg_list, arg_fields = _extract_init_signature(
           cls, auto_doc=cls.auto_doc, auto_typing=cls.auto_typing)
+
+      @object_utils.explicit_method_override
       @functools.wraps(cls.__init__)
       def _sym_init(self, *args, **kwargs):
         _SubclassedWrapperBase.__init__(self, *args, **kwargs)
 
         # The following code is to deal with call to `super().__init__()`.
         # In such case, we need to invoke the original __init__ instead of
         # the symbolic init, which can be told by the
```

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/symbolic/class_wrapper_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/symbolic/class_wrapper_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/symbolic/compounding.py` & `pyglove-0.4.2.dev20230728/pyglove/core/symbolic/compounding.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,18 +11,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Compounding symbolic classes."""
 
 import abc
 import inspect
+import sys
 import types
 from typing import Any, List, Optional, Tuple, Type, Union
 
+from pyglove.core import object_utils
 from pyglove.core.symbolic import schema_utils
+from pyglove.core.symbolic.base import Symbolic
 from pyglove.core.symbolic.object import Object
 import pyglove.core.typing as pg_typing
 
 
 class Compound(Object):
   """Base class for compound objects."""
 
@@ -33,14 +36,15 @@
 
   def __init_subclass__(cls):
     # Bypass other classes' `__init_subclass__` method when `Compound`
     # is inherited as the first base class. This is to avoid side-effect
     # from the user class to compound with.
     Object.__init_subclass__(cls)
 
+  @object_utils.explicit_method_override
   def __init__(self, *args, **kwargs):
     # `explicit_init` allows the `__init__` of the other classes that sit after
     # `Compound` to be bypassed.
     Object.__init__(self, *args, explicit_init=True, **kwargs)
 
 
 _COMPOUND_OWNED_ATTR_NAMES = frozenset(dir(Compound))
@@ -165,50 +169,69 @@
         _ = self.decomposed
 
     @property
     def decomposed(self):
       if self._sym_decomposed is None:
         # Build the compound object.
         self._sym_decomposed = factory_fn(**self.sym_init_args)
+
+        # This allows the decomposed symbolic object to access the parent chain
+        # for value retrieval of contextual attributes.
+        if isinstance(self._sym_decomposed, Symbolic):
+          self._sym_decomposed.sym_setparent(self.sym_parent)
       return self._sym_decomposed
 
+    def _on_parent_change(self, old_parent, new_parent):
+      """Override to allow decomposed object to follow parent chain change."""
+      super()._on_parent_change(old_parent, new_parent)
+      if isinstance(self._sym_decomposed, Symbolic):
+        self._sym_decomposed.sym_setparent(new_parent)
+
+    def sym_value(self, name: str) -> Any:
+      # Bypass the user base' `sym_value` if it's overriden.
+      return Compound.sym_value(self, name)
+
     def __getattribute__(self, name: str):
       if (
           name.startswith('_')
           or name in _COMPOUND_OWNED_ATTR_NAMES
           or name in self.sym_init_args
       ):
-        return super().__getattribute__(name)
+        return Compound.__getattribute__(self, name)
       # Redirect attribute to the compound object.
       return getattr(self.decomposed, name)
 
   cls = _Compound
   cls.__name__ = factory_fn.__name__
   cls.__qualname__ = factory_fn.__qualname__
   cls.__module__ = factory_fn.__module__
   cls.__doc__ = factory_fn.__doc__
 
   # Enable automatic registration of subclass.
   cls.auto_register = True
   cls.apply_schema(schema)
 
-  # NOTE(daiyip): Override abstract methods as non-ops, so `cls` could have an
-  # abstract class as its base. We don't need to worry about the implementation
-  # of the abstract method, since it will be detoured to the decomposed object
-  # at runtime via `__getattribute__`.
-  for key in dir(cls):
-    attr = getattr(cls, key)
-    if getattr(attr, '__isabstractmethod__', False):
-      noop = lambda self, *args, **kwargs: None
-      if isinstance(attr, property):
-        noop = property(noop)
-      else:
-        assert inspect.isfunction(attr), (key, attr)
-      setattr(cls, key, noop)
-  abc.update_abstractmethods(cls)
+  # Supporting abstract class as compound base class.
+  # This is a feature supported for Python 3.10 and above.
+  if sys.version_info >= (3, 10):
+
+    # NOTE(daiyip): Override abstract methods as non-ops, so `cls` could
+    # have an abstract class as its base. We don't need to worry about the
+    # implementation of the abstract method, since it will be detoured to the
+    # decomposed object at runtime via `__getattribute__`.
+    for key in dir(cls):
+      attr = getattr(cls, key)
+      if getattr(attr, '__isabstractmethod__', False):
+        noop = lambda self, *args, **kwargs: None
+        if isinstance(attr, property):
+          noop = property(noop)
+        else:
+          assert inspect.isfunction(attr), (key, attr)
+        setattr(cls, key, noop)
+    abc.update_abstractmethods(cls)
 
   if add_to_registry:
     cls.register_for_deserialization(serialization_key, additional_keys)
   return cls
 
 
 def compound(
@@ -251,15 +274,15 @@
 
     # We can access symbolic attributes of the compound object.
     assert f.v == 1
 
     # We can also access the public APIs of the decomposed object.
     assert f.x == 1
     assert f.y == 1
-    assert f.sum() == 2     
+    assert f.sum() == 2
 
     # Or explicit access the decomposed object.
     assert f.decomposed == Foo(1, 1)
 
     # Moreover, symbolic power is fully unleashed to the compound class.
     f.rebind(v=2)
     assert f.x == 2
```

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/symbolic/compounding_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/symbolic/compounding_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,23 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for pyglove.compounding."""
 
 import abc
 import dataclasses
+import sys
 import unittest
 
+from pyglove.core import object_utils
 from pyglove.core import typing as pg_typing
+from pyglove.core.symbolic.base import ContextualValue
 from pyglove.core.symbolic.compounding import compound as pg_compound
 from pyglove.core.symbolic.compounding import compound_class as pg_compound_class
+from pyglove.core.symbolic.dict import Dict
 from pyglove.core.symbolic.object import Object
 
 
 class BasicTest(unittest.TestCase):
 
   def test_basics(self):
     @dataclasses.dataclass
@@ -59,62 +63,14 @@
         'Cannot inference the base class from return value annotation',
     ):
 
       @pg_compound
       def bar(unused_x):
         pass
 
-  def test_on_bound_side_effect_free(self):
-
-    class Foo(Object):
-      x: int
-
-      def _on_bound(self):
-        # Side effect.
-        super()._on_bound()
-        assert type(self) is Foo   # pylint: disable=unidiomatic-typecheck
-
-      def hello(self):
-        return self.x
-
-    @pg_compound(Foo)
-    def foo(x):
-      return Foo(x)
-
-    # This does not trigger assertion.
-    self.assertEqual(foo(1).hello(), 1)
-
-  def test_use_abstract_base(self):
-
-    class Foo(metaclass=abc.ABCMeta):
-      @abc.abstractmethod
-      def foo(self, x):
-        pass
-
-      @property
-      @abc.abstractmethod
-      def bar(self):
-        pass
-
-    class Bar(Foo):
-      def foo(self, x):
-        return x
-
-      @property
-      def bar(self):
-        return 1
-
-    @pg_compound(Foo)
-    def bar():
-      return Bar()
-
-    b = bar()
-    self.assertEqual(b.bar, 1)
-    self.assertEqual(b.foo(1), 1)
-
   def test_lazy_build(self):
     count = dict(x=0)
 
     class Foo:
       def __init__(self, y):
         self.y = y
         self.z = y
@@ -185,14 +141,15 @@
     self.assertEqual(ca.value(), 2)
     self.assertIs(type(ca.decomposed), A)
 
   def test_user_class_with_side_effect_init(self):
     class A(Object):
       x: int
 
+      @object_utils.explicit_method_override
       def __init__(self, x):
         super().__init__(x=x)
         assert type(self) is A  # pylint: disable=unidiomatic-typecheck
 
       def value(self):
         return self.x
 
@@ -218,14 +175,88 @@
       def foo(self):
         return 'bar'
 
     CompoundA = pg_compound_class(lambda: A(), A)  # pylint: disable=invalid-name, unnecessary-lambda
     self.assertTrue(issubclass(CompoundA, A))
     self.assertEqual(CompoundA().foo(), 'bar')
 
+  def test_on_bound_side_effect_free(self):
+    class Foo(Object):
+      x: int
+
+      def _on_bound(self):
+        # Side effect.
+        super()._on_bound()
+        assert type(self) is Foo  # pylint: disable=unidiomatic-typecheck
+
+      def hello(self):
+        return self.x
+
+    @pg_compound(Foo)
+    def foo(x):
+      return Foo(x)
+
+    # This does not trigger assertion.
+    self.assertEqual(foo(1).hello(), 1)
+
+  @unittest.skipIf(
+      sys.version_info < (3, 10),
+      'This feature is only supported on Python 3.10 and above.',
+  )
+  def test_use_abstract_base(self):
+    class Foo(metaclass=abc.ABCMeta):
+
+      @abc.abstractmethod
+      def foo(self, x):
+        pass
+
+      @property
+      @abc.abstractmethod
+      def bar(self):
+        pass
+
+    class Bar(Foo):
+
+      def foo(self, x):
+        return x
+
+      @property
+      def bar(self):
+        return 1
+
+    @pg_compound(Foo)
+    def bar():
+      return Bar()
+
+    b = bar()
+    self.assertEqual(b.bar, 1)
+    self.assertEqual(b.foo(1), 1)
+
+  def test_contextual_attr_access(self):
+    class Foo(Object):
+      x: int = ContextualValue()
+
+    @pg_compound(Foo)
+    def foo():
+      return Foo()
+
+    f = foo()
+    d = Dict(x=1, y=f)
+    self.assertEqual(f.x, 1)
+    d.y = None
+    self.assertIsNone(f.sym_parent)
+
+    with self.assertRaisesRegex(
+        AttributeError, '.* is not found under its context'
+    ):
+      _ = f.x
+
+    _ = Dict(x=2, y=f)
+    self.assertEqual(f.x, 2)
+
 
 class TypingTest(unittest.TestCase):
 
   def test_no_typing(self):
     @dataclasses.dataclass
     class Foo:
       x: int
```

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/symbolic/contextual.py` & `pyglove-0.4.2.dev20230728/pyglove/core/symbolic/contextual.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/symbolic/contextual_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/symbolic/contextual_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/symbolic/dict.py` & `pyglove-0.4.2.dev20230728/pyglove/core/symbolic/dict.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/symbolic/dict_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/symbolic/dict_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/symbolic/diff.py` & `pyglove-0.4.2.dev20230728/pyglove/core/symbolic/diff.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/symbolic/diff_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/symbolic/diff_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/symbolic/flags.py` & `pyglove-0.4.2.dev20230728/pyglove/core/symbolic/flags.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/symbolic/flags_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/symbolic/flags_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/symbolic/functor.py` & `pyglove-0.4.2.dev20230728/pyglove/core/symbolic/functor.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,15 @@
         name='__init__',
         module_name=cls.__module__,
         qualname=cls.__qualname__,
     )
 
     pseudo_init = init_signature.make_function(['pass'])
 
+    @object_utils.explicit_method_override
     @functools.wraps(pseudo_init)
     def _init(self, *args, **kwargs):
       Functor.__init__(self, *args, **kwargs)
 
     setattr(cls, '__init__', _init)
 
     # Update __call__ signature.
@@ -116,14 +117,15 @@
   def __new__(cls, *args, **kwargs):
     instance = object.__new__(cls)
     if flags.should_call_functors_during_init():
       instance.__init__(*args, **kwargs)
       return instance()
     return instance
 
+  @object_utils.explicit_method_override
   def __init__(
       self,
       *args,
       root_path: Optional[object_utils.KeyPath] = None,
       override_args: bool = False,
       ignore_extra_args: bool = False,
       **kwargs):
```

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/symbolic/functor_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/symbolic/functor_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/symbolic/list.py` & `pyglove-0.4.2.dev20230728/pyglove/core/symbolic/list.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/symbolic/list_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/symbolic/list_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/symbolic/object.py` & `pyglove-0.4.2.dev20230728/pyglove/core/symbolic/object.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,14 +270,23 @@
         def __init_subclass__(cls):
           # This bypasses UserClass.__init_subclass__
           pg.Object.__init_subclass__(cls)
 
     Args:
       user_cls: The source class that calls this class method.
     """
+    object_utils.ensure_explicit_method_override(
+        cls.__init__,
+        (
+            '`pg.Object.__init__` is a PyGlove managed method. For setting up '
+            'the class initialization logic, please override `_on_bound()` or '
+            '`_on_init()`. If you do have a need to override `__init__` and '
+            'know the implications, please decorate your overridden method '
+            'with `@pg.explicit_method_override`.'
+        ))
     super().__init_subclass__()
 
     user_cls = user_cls or cls
     if user_cls.auto_schema:
       # Inherit schema from base classes that have schema
       # in the ordered of inheritance.
       # TODO(daiyip): size of base_schema_list can be reduced
@@ -339,14 +348,15 @@
         cls.schema, cls.__module__, '__init__', f'{cls.__name__}.__init__'
     )
     pseudo_init = signature.make_function(['pass'])
 
     # Create a new `__init__` that passes through all the arguments to
     # in `pg.Object.__init__`. This is needed for each class to use different
     # signature.
+    @object_utils.explicit_method_override
     @functools.wraps(pseudo_init)
     def _init(self, *args, **kwargs):
       # We pass through the arguments to `Object.__init__` instead of
       # `super()` since the parent class uses a generated `__init__` will
       # be delegated to `Object.__init__` eventually. Therefore, directly
       # calling `Object.__init__` is equivalent to calling `super().__init__`.
       Object.__init__(self, *args, **kwargs)
@@ -444,14 +454,15 @@
       root_path: KeyPath of loaded object in its object tree.
 
     Returns:
       A symbolic Object instance.
     """
     return cls(allow_partial=allow_partial, root_path=root_path, **json_value)
 
+  @object_utils.explicit_method_override
   def __init__(
       self,
       *args,
       allow_partial: bool = False,
       sealed: Optional[bool] = None,
       root_path: Optional[object_utils.KeyPath] = None,
       explicit_init: bool = False,
```

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/symbolic/object_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/symbolic/object_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,30 +198,39 @@
   def test_override_init(self):
 
     @pg_members([
         ('x', pg_typing.Int())
     ])
     class A(Object):
 
+      @object_utils.explicit_method_override
       def __init__(self, x):
         super().__init__(int(x))
 
     a = A(1.1)
     self.assertEqual(a.x, 1)
 
     class B(A):
 
+      @object_utils.explicit_method_override
       def __init__(self, x):  # pylint: disable=super-init-not-called
         # Forgot to call super().__init__ will trigger error.
         self.x = x
 
     with self.assertRaisesRegex(
         ValueError, '.* should call `super.*__init__`'):
       _ = B(1)
 
+    with self.assertRaisesRegex(
+        TypeError, '.* is a PyGlove managed method.'
+    ):
+      class C(A):  # pylint: disable=unused-variable
+        def __init__(self, x):
+          super().__init__(x + 1)
+
   def test_symbolic_fields_from_annotations(self):
 
     class X(Object):
       pass
 
     self.assertEqual(X.init_arg_list, [])
 
@@ -1909,14 +1918,15 @@
     ], init_arg_list=['y', '*z'])
     class B(Object):
       pass
 
     class C(B):
       """Custom __init__."""
 
+      @object_utils.explicit_method_override
       def __init__(self, a, b):
         super().__init__(b, x=a)
 
     signature = inspect.signature(C.__init__)
     self.assertEqual(
         list(signature.parameters.keys()), ['self', 'a', 'b'])
```

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/symbolic/origin.py` & `pyglove-0.4.2.dev20230728/pyglove/core/symbolic/origin.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/symbolic/origin_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/symbolic/origin_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/symbolic/pure_symbolic.py` & `pyglove-0.4.2.dev20230728/pyglove/core/symbolic/pure_symbolic.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/symbolic/schema_utils.py` & `pyglove-0.4.2.dev20230728/pyglove/core/symbolic/schema_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/symbolic/schema_utils_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/symbolic/schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/symbolic/symbolize.py` & `pyglove-0.4.2.dev20230728/pyglove/core/symbolic/symbolize.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/symbolic/symbolize_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/symbolic/symbolize_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/tuning/__init__.py` & `pyglove-0.4.2.dev20230728/pyglove/core/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/tuning/backend.py` & `pyglove-0.4.2.dev20230728/pyglove/core/tuning/backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/tuning/backend_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/tuning/backend_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/tuning/early_stopping.py` & `pyglove-0.4.2.dev20230728/pyglove/core/tuning/early_stopping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/tuning/local_backend.py` & `pyglove-0.4.2.dev20230728/pyglove/core/tuning/local_backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/tuning/protocols.py` & `pyglove-0.4.2.dev20230728/pyglove/core/tuning/protocols.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/tuning/protocols_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/tuning/protocols_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/tuning/sample.py` & `pyglove-0.4.2.dev20230728/pyglove/core/tuning/sample.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/tuning/sample_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/tuning/sample_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/typing/__init__.py` & `pyglove-0.4.2.dev20230728/pyglove/core/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/typing/annotation_conversion.py` & `pyglove-0.4.2.dev20230728/pyglove/core/typing/annotation_conversion.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/typing/annotation_conversion_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/typing/annotation_conversion_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/typing/callable_ext.py` & `pyglove-0.4.2.dev20230728/pyglove/core/typing/callable_ext.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/typing/callable_ext_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/typing/callable_ext_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/typing/callable_signature.py` & `pyglove-0.4.2.dev20230728/pyglove/core/typing/callable_signature.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/typing/callable_signature_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/typing/callable_signature_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/typing/class_schema.py` & `pyglove-0.4.2.dev20230728/pyglove/core/typing/class_schema.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/typing/class_schema_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/typing/class_schema_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/typing/class_schema_utils.py` & `pyglove-0.4.2.dev20230728/pyglove/core/typing/class_schema_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/typing/class_schema_utils_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/typing/class_schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/typing/custom_typing.py` & `pyglove-0.4.2.dev20230728/pyglove/core/typing/custom_typing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/typing/generic.py` & `pyglove-0.4.2.dev20230728/pyglove/core/typing/generic.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/typing/generic_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/typing/generic_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/typing/key_specs.py` & `pyglove-0.4.2.dev20230728/pyglove/core/typing/key_specs.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/typing/key_specs_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/typing/key_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/typing/pytype_support.py` & `pyglove-0.4.2.dev20230728/pyglove/core/typing/pytype_support.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/typing/type_conversion.py` & `pyglove-0.4.2.dev20230728/pyglove/core/typing/type_conversion.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/typing/type_conversion_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/typing/type_conversion_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/typing/typed_missing.py` & `pyglove-0.4.2.dev20230728/pyglove/core/typing/typed_missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/typing/typed_missing_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/typing/typed_missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/typing/value_specs.py` & `pyglove-0.4.2.dev20230728/pyglove/core/typing/value_specs.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/core/typing/value_specs_test.py` & `pyglove-0.4.2.dev20230728/pyglove/core/typing/value_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/__init__.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/early_stopping/__init__.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/early_stopping/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/early_stopping/base.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/early_stopping/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/early_stopping/base_test.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/early_stopping/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/early_stopping/step_wise.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/early_stopping/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/early_stopping/step_wise_test.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/early_stopping/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/evolution/__init__.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/evolution/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/evolution/base.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/evolution/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/evolution/base_test.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/evolution/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/evolution/hill_climb.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/evolution/hill_climb.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/evolution/hill_climb_test.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/evolution/hill_climb_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/evolution/mutators.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/evolution/mutators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/evolution/mutators_test.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/evolution/mutators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/evolution/neat.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/evolution/neat.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/evolution/neat_test.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/evolution/neat_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/evolution/nsga2.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/evolution/nsga2.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/evolution/nsga2_test.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/evolution/nsga2_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/evolution/recombinators.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/evolution/recombinators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/evolution/recombinators_test.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/evolution/recombinators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/evolution/regularized_evolution.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/evolution/regularized_evolution.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/evolution/regularized_evolution_test.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/evolution/regularized_evolution_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/evolution/selectors.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/evolution/selectors.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/evolution/selectors_test.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/evolution/selectors_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/evolution/where.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/evolution/where.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/evolution/where_test.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/evolution/where_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/mutfun/__init__.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/mutfun/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/mutfun/base.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/mutfun/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/mutfun/base_test.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/mutfun/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/mutfun/basic_ops.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/mutfun/basic_ops.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/mutfun/basic_ops_test.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/mutfun/basic_ops_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/scalars/__init__.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/scalars/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/scalars/base.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/scalars/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/scalars/base_test.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/scalars/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/scalars/maths.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/scalars/maths.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/scalars/maths_test.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/scalars/maths_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/scalars/randoms.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/scalars/randoms.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/scalars/randoms_test.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/scalars/randoms_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/scalars/step_wise.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/scalars/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove/ext/scalars/step_wise_test.py` & `pyglove-0.4.2.dev20230728/pyglove/ext/scalars/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/pyglove.egg-info/PKG-INFO` & `pyglove-0.4.2.dev20230728/pyglove.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.4.2.dev20230727
+Version: 0.4.2.dev20230728
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.4.2.dev20230727/pyglove.egg-info/SOURCES.txt` & `pyglove-0.4.2.dev20230728/pyglove.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.2.dev20230727/setup.py` & `pyglove-0.4.2.dev20230728/setup.py`

 * *Files identical despite different names*

