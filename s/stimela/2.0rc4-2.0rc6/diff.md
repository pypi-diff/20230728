# Comparing `tmp/stimela-2.0rc4.tar.gz` & `tmp/stimela-2.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stimela-2.0rc4.tar", max compression
+gzip compressed data, was "stimela-2.0rc6.tar", max compression
```

## Comparing `stimela-2.0rc4.tar` & `stimela-2.0rc6.tar`

### file list

```diff
@@ -1,151 +1,97 @@
--rw-r--r--   0        0        0    18047 2023-03-28 14:27:45.913525 stimela-2.0rc4/LICENSE
--rw-r--r--   0        0        0      642 2023-03-28 14:27:45.913525 stimela-2.0rc4/README.rst
--rw-r--r--   0        0        0     1086 2023-03-28 14:27:45.913525 stimela-2.0rc4/pyproject.toml
--rw-r--r--   0        0        0     1605 2023-03-28 14:27:45.913525 stimela-2.0rc4/scabha/__init__.py
--rw-r--r--   0        0        0     1622 2023-03-28 14:27:45.913525 stimela-2.0rc4/scabha/basetypes.py
--rw-r--r--   0        0        0      161 2023-03-28 14:27:45.913525 stimela-2.0rc4/scabha/cab_utils.py
--rw-r--r--   0        0        0    20610 2023-03-28 14:27:45.917525 stimela-2.0rc4/scabha/cargo.py
--rw-r--r--   0        0        0    11458 2023-03-28 14:27:45.917525 stimela-2.0rc4/scabha/configuratt/__init__.py
--rw-r--r--   0        0        0    10076 2023-03-28 14:27:45.917525 stimela-2.0rc4/scabha/configuratt/cache.py
--rw-r--r--   0        0        0      501 2023-03-28 14:27:45.917525 stimela-2.0rc4/scabha/configuratt/common.py
--rw-r--r--   0        0        0     9385 2023-03-28 14:27:45.917525 stimela-2.0rc4/scabha/configuratt/deps.py
--rw-r--r--   0        0        0    15499 2023-03-28 14:27:45.917525 stimela-2.0rc4/scabha/configuratt/resolvers.py
--rw-r--r--   0        0        0    19111 2023-03-28 14:27:45.917525 stimela-2.0rc4/scabha/evaluator.py
--rw-r--r--   0        0        0     2990 2023-03-28 14:27:45.917525 stimela-2.0rc4/scabha/exceptions.py
--rw-r--r--   0        0        0     3110 2023-03-28 14:27:45.917525 stimela-2.0rc4/scabha/logging_utils.py
--rw-r--r--   0        0        0      423 2023-03-28 14:27:45.917525 stimela-2.0rc4/scabha/proc_utils.py
--rw-r--r--   0        0        0     6402 2023-03-28 14:27:45.917525 stimela-2.0rc4/scabha/schema_utils.py
--rw-r--r--   0        0        0    20309 2023-03-28 14:27:45.917525 stimela-2.0rc4/scabha/substitutions.py
--rw-r--r--   0        0        0    12152 2023-03-28 14:27:45.917525 stimela-2.0rc4/scabha/validate.py
--rw-r--r--   0        0        0      662 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/__init__.py
--rw-r--r--   0        0        0     3565 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/backends/__init__.py
--rw-r--r--   0        0        0    10808 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/backends/docker.py
--rw-r--r--   0        0        0     4216 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/backends/flavours/__init__.py
--rw-r--r--   0        0        0      919 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/backends/flavours/binary.py
--rw-r--r--   0        0        0     3221 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/backends/flavours/casa.py
--rw-r--r--   0        0        0     8118 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/backends/flavours/python_flavours.py
--rw-r--r--   0        0        0      306 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/backends/kubernetes/__init__.py
--rw-r--r--   0        0        0    17289 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/backends/kubernetes/run_kube.py
--rw-r--r--   0        0        0       59 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/backends/native/__init__.py
--rw-r--r--   0        0        0     3396 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/backends/native/run_native.py
--rw-r--r--   0        0        0     7563 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/backends/podman.py
--rw-r--r--   0        0        0     4230 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/backends/singularity.py
--rw-r--r--   0        0        0      249 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/__init__.py
--rw-r--r--   0        0        0       56 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/21cmfast/Dockerfile
--rw-r--r--   0        0        0        0 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/__init__.py
--rw-r--r--   0        0        0       86 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/aegean/Dockerfile
--rw-r--r--   0        0        0      170 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/aimfast/Dockerfile
--rw-r--r--   0        0        0       57 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/aoflagger/Dockerfile
--rw-r--r--   0        0        0      180 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/astropy/Dockerfile
--rw-r--r--   0        0        0      538 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/base/Dockerfile
--rw-r--r--   0        0        0     1036 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/casa/Dockerfile
--rw-r--r--   0        0        0      987 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/casa/casa.yaml
--rw-r--r--   0        0        0        0 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/casa/casa.yml
--rw-r--r--   0        0        0      108 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/casarest/Dockerfile
--rw-r--r--   0        0        0      118 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/catdagger/Dockerfile
--rw-r--r--   0        0        0      993 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/chgcentre/Dockerfile
--rw-r--r--   0        0        0      266 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/codex-africanus/Dockerfile
--rw-r--r--   0        0        0      280 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/cubical/Dockerfile
--rw-r--r--   0        0        0      385 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/cubical_ddf/Dockerfile
--rw-r--r--   0        0        0       52 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/curl/Dockerfile
--rw-r--r--   0        0        0      420 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/ddfacet/Dockerfile
--rw-r--r--   0        0        0       98 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/eidos/Dockerfile
--rw-r--r--   0        0        0      490 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/group.template
--rw-r--r--   0        0        0      257 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/katdal/Dockerfile
--rw-r--r--   0        0        0      102 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/lofar/Dockerfile
--rw-r--r--   0        0        0      109 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/meqtrees/Dockerfile
--rw-r--r--   0        0        0      194 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/montage/Dockerfile
--rw-r--r--   0        0        0       51 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/moresane/Dockerfile
--rw-r--r--   0        0        0      125 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/msutils/Dockerfile
--rw-r--r--   0        0        0      294 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/owlcat/Dockerfile
--rw-r--r--   0        0        0      979 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/passwd.template
--rw-r--r--   0        0        0      217 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/politsiyakat/Dockerfile
--rw-r--r--   0        0        0      103 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/pybdsf/Dockerfile
--rw-r--r--   0        0        0      116 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/pyddi/Dockerfile
--rw-r--r--   0        0        0      508 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/quartical/Dockerfile
--rw-r--r--   0        0        0      381 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/ragavi/Dockerfile
--rw-r--r--   0        0        0      352 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/rfimasker/Dockerfile
--rw-r--r--   0        0        0      285 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/rfinder/Dockerfile
--rw-r--r--   0        0        0       55 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/sagecal/Dockerfile
--rw-r--r--   0        0        0      231 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/shadems/Dockerfile
--rw-r--r--   0        0        0      266 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/shadems/Dockerfile.v040
--rw-r--r--   0        0        0      529 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/shadems/shadems.yaml
--rw-r--r--   0        0        0      236 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/sharpener/Dockerfile
--rw-r--r--   0        0        0      797 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/sofia/Dockerfile
--rw-r--r--   0        0        0      136 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/sourcery/Dockerfile
--rw-r--r--   0        0        0      189 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/sunblocker/Dockerfile
--rw-r--r--   0        0        0      193 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/tigger/Dockerfile
--rw-r--r--   0        0        0      678 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/tricolour/Dockerfile
--rw-r--r--   0        0        0      859 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/base/wsclean/Dockerfile
--rw-r--r--   0        0        0     1592 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/cab/casa_applycal.yaml
--rw-r--r--   0        0        0      614 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/cab/fitstool_stack.yaml
--rw-r--r--   0        0        0     5920 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/cab/shadems.yaml
--rw-r--r--   0        0        0      983 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/cab/simms.yaml
--rw-r--r--   0        0        0     2319 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/cab/tricolour.yaml
--rw-r--r--   0        0        0     1548 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/cab/wsclean.yaml
--rw-r--r--   0        0        0     2182 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/cab/wsclean_pol.yaml
--rw-r--r--   0        0        0     1197 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/lib/params/casa.yaml
--rw-r--r--   0        0        0     2559 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/cargo/lib/params/wsclean.yaml
--rw-r--r--   0        0        0        0 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/commands/__init__.py
--rw-r--r--   0        0        0     2249 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/commands/build.py
--rw-r--r--   0        0        0      832 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/commands/cabs.py
--rw-r--r--   0        0        0      896 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/commands/clean.py
--rw-r--r--   0        0        0      643 2023-03-28 14:27:45.917525 stimela-2.0rc4/stimela/commands/containers.py
--rw-r--r--   0        0        0     5847 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/commands/doc.py
--rw-r--r--   0        0        0     1681 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/commands/images.py
--rw-r--r--   0        0        0      371 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/commands/kill.py
--rw-r--r--   0        0        0      640 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/commands/ps.py
--rw-r--r--   0        0        0     1338 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/commands/pull.py
--rw-r--r--   0        0        0     1856 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/commands/push.py
--rw-r--r--   0        0        0    13131 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/commands/run.py
--rw-r--r--   0        0        0     2627 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/commands/save_config.py
--rw-r--r--   0        0        0    13171 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/config.py
--rw-r--r--   0        0        0     1761 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/kitchen/__init__.py
--rw-r--r--   0        0        0      533 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/kitchen/batch.py
--rw-r--r--   0        0        0    18688 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/kitchen/cab.py
--rw-r--r--   0        0        0    62522 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/kitchen/recipe.py
--rw-r--r--   0        0        0     1036 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/kitchen/runners.py
--rw-r--r--   0        0        0    26463 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/kitchen/step.py
--rw-r--r--   0        0        0    11379 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/kitchen/wranglers.py
--rw-r--r--   0        0        0     4876 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/main.py
--rw-r--r--   0        0        0       29 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/schedulers/__init__.py
--rw-r--r--   0        0        0     2274 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/schedulers/slurm.py
--rw-r--r--   0        0        0    14999 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/stimelogging.py
--rw-r--r--   0        0        0    10741 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/task_stats.py
--rw-r--r--   0        0        0      254 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/utils/__init__.py
--rw-r--r--   0        0        0     7314 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/utils/xrun_asyncio.py
--rw-r--r--   0        0        0     9181 2023-03-28 14:27:45.921525 stimela-2.0rc4/stimela/utils/xrun_poll.py
--rw-r--r--   0        0        0        0 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/scabha_tests/__init__.py
--rw-r--r--   0        0        0     1965 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/scabha_tests/test_configuratt.py
--rw-r--r--   0        0        0      540 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/scabha_tests/test_dynschema.py
--rw-r--r--   0        0        0       70 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/scabha_tests/test_include.yaml
--rw-r--r--   0        0        0       46 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/scabha_tests/test_include2.yaml
--rw-r--r--   0        0        0       21 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/scabha_tests/test_nest_a.yml
--rw-r--r--   0        0        0       21 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/scabha_tests/test_nest_b.yml
--rw-r--r--   0        0        0       25 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/scabha_tests/test_nest_c.yml
--rw-r--r--   0        0        0     1659 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/scabha_tests/test_parsing.py
--rw-r--r--   0        0        0      658 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/scabha_tests/test_schema.py
--rw-r--r--   0        0        0       55 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/scabha_tests/test_schema.yaml
--rw-r--r--   0        0        0     5805 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/scabha_tests/test_substitutions.py
--rw-r--r--   0        0        0      924 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/scabha_tests/testconf.yaml
--rw-r--r--   0        0        0        0 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/__init__.py
--rw-r--r--   0        0        0      240 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/example_callable.py
--rw-r--r--   0        0        0      541 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/example_dynschema.py
--rw-r--r--   0        0        0     1428 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_aliasing.yml
--rw-r--r--   0        0        0      554 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_callables.py
--rw-r--r--   0        0        0     2033 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_callables.yml
--rw-r--r--   0        0        0      756 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_casa.yml
--rw-r--r--   0        0        0      172 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_dask_storage_options.yaml
--rw-r--r--   0        0        0     2228 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_kube.yml
--rw-r--r--   0        0        0     2033 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_loop_recipe.yml
--rw-r--r--   0        0        0     2154 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_loop_recipe_slurm.yml
--rw-r--r--   0        0        0     4408 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_nesting.yml
--rw-r--r--   0        0        0     3441 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_recipe.py
--rw-r--r--   0        0        0     4023 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_recipe.yml
--rw-r--r--   0        0        0     1390 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_scatter.yml
--rw-r--r--   0        0        0     1882 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_wranglers.py
--rw-r--r--   0        0        0      205 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_wranglers.txt
--rw-r--r--   0        0        0     3010 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_wranglers.yml
--rw-r--r--   0        0        0     1273 2023-03-28 14:27:45.921525 stimela-2.0rc4/tests/stimela_tests/test_xrun.yml
--rw-r--r--   0        0        0     1586 1970-01-01 00:00:00.000000 stimela-2.0rc4/PKG-INFO
+-rw-r--r--   0        0        0    18047 2023-07-28 09:06:32.201342 stimela-2.0rc6/LICENSE
+-rw-r--r--   0        0        0      642 2023-07-28 09:06:32.201342 stimela-2.0rc6/README.rst
+-rw-r--r--   0        0        0     1086 2023-07-28 09:06:32.205343 stimela-2.0rc6/pyproject.toml
+-rw-r--r--   0        0        0     1605 2023-07-28 09:06:32.205343 stimela-2.0rc6/scabha/__init__.py
+-rw-r--r--   0        0        0     1622 2023-07-28 09:06:32.205343 stimela-2.0rc6/scabha/basetypes.py
+-rw-r--r--   0        0        0      161 2023-07-28 09:06:32.205343 stimela-2.0rc6/scabha/cab_utils.py
+-rw-r--r--   0        0        0    24429 2023-07-28 09:06:32.205343 stimela-2.0rc6/scabha/cargo.py
+-rw-r--r--   0        0        0    11458 2023-07-28 09:06:32.205343 stimela-2.0rc6/scabha/configuratt/__init__.py
+-rw-r--r--   0        0        0    10076 2023-07-28 09:06:32.205343 stimela-2.0rc6/scabha/configuratt/cache.py
+-rw-r--r--   0        0        0      501 2023-07-28 09:06:32.205343 stimela-2.0rc6/scabha/configuratt/common.py
+-rw-r--r--   0        0        0     9385 2023-07-28 09:06:32.205343 stimela-2.0rc6/scabha/configuratt/deps.py
+-rw-r--r--   0        0        0    16209 2023-07-28 09:06:32.205343 stimela-2.0rc6/scabha/configuratt/resolvers.py
+-rw-r--r--   0        0        0    20250 2023-07-28 09:06:32.205343 stimela-2.0rc6/scabha/evaluator.py
+-rw-r--r--   0        0        0     2990 2023-07-28 09:06:32.205343 stimela-2.0rc6/scabha/exceptions.py
+-rw-r--r--   0        0        0     3110 2023-07-28 09:06:32.205343 stimela-2.0rc6/scabha/logging_utils.py
+-rw-r--r--   0        0        0      423 2023-07-28 09:06:32.205343 stimela-2.0rc6/scabha/proc_utils.py
+-rw-r--r--   0        0        0     6487 2023-07-28 09:06:32.205343 stimela-2.0rc6/scabha/schema_utils.py
+-rw-r--r--   0        0        0    20331 2023-07-28 09:06:32.205343 stimela-2.0rc6/scabha/substitutions.py
+-rw-r--r--   0        0        0    12506 2023-07-28 09:06:32.205343 stimela-2.0rc6/scabha/validate.py
+-rw-r--r--   0        0        0      798 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/__init__.py
+-rw-r--r--   0        0        0     6036 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/backends/__init__.py
+-rw-r--r--   0        0        0    12929 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/backends/docker.py
+-rw-r--r--   0        0        0     4575 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/backends/flavours/__init__.py
+-rw-r--r--   0        0        0     1252 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/backends/flavours/binary.py
+-rw-r--r--   0        0        0     3339 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/backends/flavours/casa.py
+-rw-r--r--   0        0        0     8742 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/backends/flavours/python_flavours.py
+-rw-r--r--   0        0        0     2010 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/backends/kubernetes/__init__.py
+-rw-r--r--   0        0        0    15850 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/backends/kubernetes/run_kube.py
+-rw-r--r--   0        0        0      309 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/backends/native/__init__.py
+-rw-r--r--   0        0        0     4065 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/backends/native/run_native.py
+-rw-r--r--   0        0        0     7653 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/backends/podman.py
+-rw-r--r--   0        0        0     2193 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/backends/runner.py
+-rw-r--r--   0        0        0    13218 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/backends/singularity.py
+-rw-r--r--   0        0        0      249 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/cargo/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/commands/__init__.py
+-rw-r--r--   0        0        0     2249 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/commands/build.py
+-rw-r--r--   0        0        0      832 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/commands/cabs.py
+-rw-r--r--   0        0        0      896 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/commands/clean.py
+-rw-r--r--   0        0        0      643 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/commands/containers.py
+-rw-r--r--   0        0        0     5847 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/commands/doc.py
+-rw-r--r--   0        0        0     1681 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/commands/images.py
+-rw-r--r--   0        0        0      371 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/commands/kill.py
+-rw-r--r--   0        0        0      640 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/commands/ps.py
+-rw-r--r--   0        0        0     1338 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/commands/pull.py
+-rw-r--r--   0        0        0     1856 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/commands/push.py
+-rw-r--r--   0        0        0    13616 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/commands/run.py
+-rw-r--r--   0        0        0     2627 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/commands/save_config.py
+-rw-r--r--   0        0        0    10644 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/config.py
+-rw-r--r--   0        0        0     1826 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-28 09:06:32.205343 stimela-2.0rc6/stimela/kitchen/__init__.py
+-rw-r--r--   0        0        0      555 2023-07-28 09:06:32.209343 stimela-2.0rc6/stimela/kitchen/batch.py
+-rw-r--r--   0        0        0    19996 2023-07-28 09:06:32.209343 stimela-2.0rc6/stimela/kitchen/cab.py
+-rw-r--r--   0        0        0    62988 2023-07-28 09:06:32.209343 stimela-2.0rc6/stimela/kitchen/recipe.py
+-rw-r--r--   0        0        0    28994 2023-07-28 09:06:32.209343 stimela-2.0rc6/stimela/kitchen/step.py
+-rw-r--r--   0        0        0    11381 2023-07-28 09:06:32.209343 stimela-2.0rc6/stimela/kitchen/wranglers.py
+-rw-r--r--   0        0        0     4744 2023-07-28 09:06:32.209343 stimela-2.0rc6/stimela/main.py
+-rw-r--r--   0        0        0       29 2023-07-28 09:06:32.209343 stimela-2.0rc6/stimela/schedulers/__init__.py
+-rw-r--r--   0        0        0     2238 2023-07-28 09:06:32.209343 stimela-2.0rc6/stimela/schedulers/slurm.py
+-rw-r--r--   0        0        0      114 2023-07-28 09:06:32.209343 stimela-2.0rc6/stimela/stimela.conf
+-rw-r--r--   0        0        0    14999 2023-07-28 09:06:32.209343 stimela-2.0rc6/stimela/stimelogging.py
+-rw-r--r--   0        0        0    10741 2023-07-28 09:06:32.209343 stimela-2.0rc6/stimela/task_stats.py
+-rw-r--r--   0        0        0      254 2023-07-28 09:06:32.209343 stimela-2.0rc6/stimela/utils/__init__.py
+-rw-r--r--   0        0        0     7349 2023-07-28 09:06:32.209343 stimela-2.0rc6/stimela/utils/xrun_asyncio.py
+-rw-r--r--   0        0        0     9181 2023-07-28 09:06:32.209343 stimela-2.0rc6/stimela/utils/xrun_poll.py
+-rw-r--r--   0        0        0        0 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/scabha_tests/__init__.py
+-rw-r--r--   0        0        0     1965 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/scabha_tests/test_configuratt.py
+-rw-r--r--   0        0        0      540 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/scabha_tests/test_dynschema.py
+-rw-r--r--   0        0        0       70 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/scabha_tests/test_include.yaml
+-rw-r--r--   0        0        0       46 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/scabha_tests/test_include2.yaml
+-rw-r--r--   0        0        0       21 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/scabha_tests/test_nest_a.yml
+-rw-r--r--   0        0        0       21 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/scabha_tests/test_nest_b.yml
+-rw-r--r--   0        0        0       25 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/scabha_tests/test_nest_c.yml
+-rw-r--r--   0        0        0     1659 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/scabha_tests/test_parsing.py
+-rw-r--r--   0        0        0      658 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/scabha_tests/test_schema.py
+-rw-r--r--   0        0        0       55 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/scabha_tests/test_schema.yaml
+-rw-r--r--   0        0        0     5805 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/scabha_tests/test_substitutions.py
+-rw-r--r--   0        0        0      924 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/scabha_tests/testconf.yaml
+-rw-r--r--   0        0        0        0 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/stimela_tests/__init__.py
+-rw-r--r--   0        0        0      240 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/stimela_tests/example_callable.py
+-rw-r--r--   0        0        0      541 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/stimela_tests/example_dynschema.py
+-rw-r--r--   0        0        0     1428 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/stimela_tests/test_aliasing.yml
+-rw-r--r--   0        0        0      554 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/stimela_tests/test_callables.py
+-rw-r--r--   0        0        0     2033 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/stimela_tests/test_callables.yml
+-rw-r--r--   0        0        0     1136 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/stimela_tests/test_casa.yml
+-rw-r--r--   0        0        0      172 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/stimela_tests/test_dask_storage_options.yaml
+-rw-r--r--   0        0        0     2228 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/stimela_tests/test_kube.yml
+-rw-r--r--   0        0        0     2033 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/stimela_tests/test_loop_recipe.yml
+-rw-r--r--   0        0        0     2154 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/stimela_tests/test_loop_recipe_slurm.yml
+-rw-r--r--   0        0        0     4408 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/stimela_tests/test_nesting.yml
+-rw-r--r--   0        0        0     3441 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/stimela_tests/test_recipe.py
+-rw-r--r--   0        0        0     4136 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/stimela_tests/test_recipe.yml
+-rw-r--r--   0        0        0     1390 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/stimela_tests/test_scatter.yml
+-rw-r--r--   0        0        0     1882 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/stimela_tests/test_wranglers.py
+-rw-r--r--   0        0        0      205 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/stimela_tests/test_wranglers.txt
+-rw-r--r--   0        0        0     3010 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/stimela_tests/test_wranglers.yml
+-rw-r--r--   0        0        0     1273 2023-07-28 09:06:32.209343 stimela-2.0rc6/tests/stimela_tests/test_xrun.yml
+-rw-r--r--   0        0        0     1586 1970-01-01 00:00:00.000000 stimela-2.0rc6/PKG-INFO
```

### Comparing `stimela-2.0rc4/LICENSE` & `stimela-2.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/README.rst` & `stimela-2.0rc6/README.rst`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/pyproject.toml` & `stimela-2.0rc6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stimela"
-version = "2.0rc4"
+version = "2.0rc6"
 description = "Framework for system agnostic pipelines for radio interferometry arrays"
 authors = ["Sphesihle Makhathini <sphemakh@gmail.com>", "Oleg Smirnov and RATT <osmirnov@gmail.com>"]
 readme = "README.rst"
 license = "GNU GPL v2"
 include = [{ path = "tests" }]
 packages = [
     {include = "stimela"},
```

### Comparing `stimela-2.0rc4/scabha/__init__.py` & `stimela-2.0rc6/scabha/__init__.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/scabha/basetypes.py` & `stimela-2.0rc6/scabha/basetypes.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/scabha/cargo.py` & `stimela-2.0rc6/scabha/cargo.py`

 * *Files 16% similar despite different names*

```diff
@@ -127,14 +127,17 @@
     # if true, treat parameter as a path, and ensure that the parent directories it refers to exist
     mkdir: bool = False
 
     # for file and dir-type parameters: if True, the file(s)/dir(s) must exist. If False, they can be missing.
     # if None, then the default logic applies: inputs must exist, and outputs don't
     must_exist: Optional[bool] = None
 
+    # for file and dir-type parameters: if True, ignore them when making processing logic decisions based on file freshness
+    skip_freshness_checks: Optional[bool] = None
+
     # For output File-type parameters. If True, and the output exists, remove before running
     remove_if_exists: bool = False
 
     # if command-line option for underlying binary has a different name, specify it here
     nom_de_guerre: Optional[str] = None
 
     # policies object, specifying a non-default way to handle this parameter
@@ -150,14 +153,16 @@
 
     # abbreviated option name for this parameter.  Used when constructing command-line interfaces
     abbreviation: Optional[str] = None
 
     # arbitrary metadata associated with parameter
     metadata: Dict[str, Any] = EmptyDictDefault()
 
+    _file_types = (File, MS, Directory)
+
     def __post_init__(self):
         def natify(value):
             # convert OmegaConf lists and dicts to native types
             if type(value) in (list, ListConfig):
                 return [natify(x) for x in value]
             elif type(value) in (dict, OrderedDict, DictConfig):
                 return OrderedDict([(name, natify(value)) for name, value in value.items()])
@@ -169,14 +174,17 @@
 
         # converts string dtype into proper type object
         # yes I know eval() is naughty but this is the best we can do for now
         # see e.g. https://stackoverflow.com/questions/67500755/python-convert-type-hint-string-representation-from-docstring-to-actual-type-t
         # The alternative is a non-standard API call i.e. typing._eval_type()
         self._dtype = eval(self.dtype, globals())
 
+        self._is_file_type = any(self._dtype == t for t in self._file_types)
+        self._is_file_list_type = any(self._dtype == List[t] for t in self._file_types)
+
         self._is_input = True
 
     def get_category(self):
         """Returns category of parameter, auto-setting it if not already preset"""
         if self.category is None:
             if self.required:
                 self.category = ParameterCategory.Required
@@ -190,20 +198,23 @@
     def is_input(self):
         return self._is_input
 
     @property 
     def is_output(self):
         return not self._is_input
 
-    _filename_types = (File, MS, Directory, "File", "MS", "Directory")
-
     @property
     def is_file_type(self):
         """True if parameter is a file or directory type"""
-        return self.dtype in self._filename_types
+        return self._is_file_type 
+
+    @property
+    def is_file_list_type(self):
+        """True if parameter is a file or directory type"""
+        return self._is_file_list_type
 
     @property
     def is_named_output(self):
         """True if parameter is a named file or directory output"""
         return self.is_output and self.is_file_type and not self.implicit
 
 ParameterSchema = OmegaConf.structured(Parameter)
@@ -211,15 +222,17 @@
 ParameterFields = set(f.name for f in dataclasses.fields(Parameter))
 
 @dataclass
 class Cargo(object):
     name: Optional[str] = None                    # cab name (if None, use image or command name)
     fqname: Optional[str] = None                  # fully-qualified name (recipe_name.step_label.etc.etc.)
 
-    info: Optional[str] = None                    # description
+    info: Optional[str] = None                    # help string
+
+    extra_info: Dict[str, str] = EmptyDictDefault() # optional, additional help sections
 
     # schemas are postentially nested (dicts of dicts), which omegaconf doesn't quite recognize,
     # (or in my ignorance I can't specify it -- in any case Union support is weak), so do a dict to Any
     # "Leaf" elements of the nested dict must be Parameters
     inputs: Dict[str, Any]   = EmptyDictDefault()
     outputs: Dict[str, Any]  = EmptyDictDefault()
     defaults: Dict[str, Any] = EmptyDictDefault()
@@ -231,25 +244,51 @@
     @staticmethod
     def flatten_schemas(io_dest, io, label, prefix=""):
         for name, value in io.items():
             if name == "subsection":
                 continue
             name = f"{prefix}{name}"
             if not isinstance(value, Parameter):
-                if not isinstance(value, (DictConfig, dict)):
-                    raise SchemaError(f"{label}.{name} is not a valid schema")
-                # try to treat as Parameter based on field names
-                if not (set(value.keys()) - ParameterFields):
-                    try:
-                        value = OmegaConf.unsafe_merge(ParameterSchema.copy(), value)
-                        io_dest[name] = Parameter(**value)
-                    except Exception as exc0:
-                        raise SchemaError(f"{label}.{name} is not a valid parameter definition", exc0)
+                if isinstance(value, str):
+                    schema = {}
+                    value = value.strip()
+                    # if value ends with a double-quoted string, parse out the docstring
+                    if value.endswith('"') and '"' in value[:-1]:
+                        value, info, _ = value.rsplit('"', 2)
+                        value = value.strip()
+                        schema['info'] = info
+                    # does value contain "="? Parse it as "type = default" then
+                    if "=" in value:
+                        value, default  = value.split("=", 1)
+                        value = value.strip()
+                        default = default.strip()
+                        if (default.startswith('"') and default.endswith('"')) or \
+                           (default.startswith("'") and default.endswith("'")): 
+                           default = default[1:-1]
+                        schema['default'] = default
+                    # does value end with "*"? Mark as required
+                    elif value.endswith("*"):
+                        schema['required'] = True
+                        value = value[:-1]
+                    schema['dtype'] = value
+                    io_dest[name] = Parameter(**schema)
+                # else proper dict schema, or subsection
                 else:
-                    Cargo.flatten_schemas(io_dest, value, label=label, prefix=f"{name}.")
+                    if not isinstance(value, (DictConfig, dict)):
+                        raise SchemaError(f"{label}.{name} is not a valid schema")
+                    # try to treat as Parameter based on field names
+                    if not (set(value.keys()) - ParameterFields):
+                        try:
+                            value = OmegaConf.unsafe_merge(ParameterSchema.copy(), value)
+                            io_dest[name] = Parameter(**value)
+                        except Exception as exc0:
+                            raise SchemaError(f"{label}.{name} is not a valid parameter definition", exc0)
+                    # else assume subsection and recurse in
+                    else:
+                        Cargo.flatten_schemas(io_dest, value, label=label, prefix=f"{name}.")
         return io_dest
 
     def flatten_param_dict(self, output_params, input_params, prefix=""):
         for name, value in input_params.items():
             name = f"{prefix}{name}"
             if isinstance(value, (dict, DictConfig)):
                 # if prefix.name. is present in schemas, treat as nested mapping
@@ -303,15 +342,15 @@
         return self.config is not None
 
     def unresolved_params(self, params):
         """Returns list of unresolved parameters"""
         return [name for name, value in params.items() if isinstance(value, Unresolved)]
 
 
-    def finalize(self, config=None, log=None, fqname=None, nesting=0):
+    def finalize(self, config=None, log=None, fqname=None, backend=None, nesting=0):
         if not self.finalized:
             if fqname is not None:
                 self.fqname = fqname
             self.config = config
             self.nesting = nesting
             self.log = log
             self.logopts = config.opts.log.copy()
@@ -328,76 +367,101 @@
                 for name, schema in list(io.items()):
                     if isinstance(schema, DictConfig):
                         try:
                             schema = OmegaConf.unsafe_merge(ParameterSchema.copy(), schema)
                         except Exception  as exc:
                             raise SchemaError(f"error in dynamic schema for parameter 'name'", exc)
                         io[name] = Parameter(**schema)
+            # new outputs may have been added
+            for schema in self.outputs.values():
+                schema._is_input = False
+            # re-resolve implicits
+            self._resolve_implicit_parameters(params)
 
-    def prevalidate(self, params: Optional[Dict[str, Any]], subst: Optional[SubstitutionNS]=None, root=False):
-        """Does pre-validation.
-        No parameter substitution is done, but will check for missing params and such.
-        A dynamic schema, if defined, is applied at this point."""
-        self.finalize()
-        # add implicits, if resolved
+    def _resolve_implicit_parameters(self, params):
+        self._implicit_params = set()
         for name, schema in self.inputs_outputs.items():
             if schema.implicit is not None and type(schema.implicit) is not Unresolved:
-                if name in params and name not in self._implicit_params:
+                if name in params and name not in self._implicit_params and params[name] != schema.implicit:
                     raise ParameterValidationError(f"implicit parameter {name} was supplied explicitly")
                 if name in self.defaults:
                    raise SchemaError(f"implicit parameter {name} also has a default value")
                 params[name] = schema.implicit
                 self._implicit_params.add(name)
+
+
+    def prevalidate(self, params: Optional[Dict[str, Any]], subst: Optional[SubstitutionNS]=None, root=False):
+        """Does pre-validation.
+        No parameter substitution is done, but will check for missing params and such.
+        A dynamic schema, if defined, is applied at this point."""
+        self.finalize()
+        # add implicits, if resolved
+        self._resolve_implicit_parameters(params)
         # assign unset categories
         for name, schema in self.inputs_outputs.items():
             schema.get_category()
 
         params = validate_parameters(params, self.inputs_outputs, defaults=self.defaults, subst=subst, fqname=self.fqname,
-                                          check_unknowns=True, check_required=False, check_exist=False,
+                                          check_unknowns=True, check_required=False, 
+                                          check_inputs_exist=False, check_outputs_exist=False,
                                           create_dirs=False, ignore_subst_errors=True)
 
         return params
 
     def validate_inputs(self, params: Dict[str, Any], subst: Optional[SubstitutionNS]=None, loosely=False):
         """Validates inputs.
         If loosely is True, then doesn't check for required parameters, and doesn't check for files to exist etc.
         This is used when skipping a step.
         """
         assert(self.finalized)
+        self._resolve_implicit_parameters(params)
 
         # check inputs
         params1 = validate_parameters(params, self.inputs, defaults=self.defaults, subst=subst, fqname=self.fqname,
-                                                check_unknowns=False, check_required=not loosely, check_exist=not loosely,
+                                                check_unknowns=False, check_required=not loosely, 
+                                                check_inputs_exist=not loosely, check_outputs_exist=False,
                                                 create_dirs=not loosely)
         # check outputs
         params1.update(**validate_parameters(params, self.outputs, defaults=self.defaults, subst=subst, fqname=self.fqname,
-                                                check_unknowns=False, check_required=False, check_exist=False,
+                                                check_unknowns=False, check_required=False, 
+                                                check_inputs_exist=not loosely, check_outputs_exist=False,
                                                 create_dirs=not loosely))
         return params1
 
     def validate_outputs(self, params: Dict[str, Any], subst: Optional[SubstitutionNS]=None, loosely=False):
         """Validates outputs. Parameter substitution is done.
         If loosely is True, then doesn't check for required parameters, and doesn't check for files to exist etc.
         """
         assert(self.finalized)
         # update implicits that weren't marked as unresolved
         for name in self._implicit_params:
             impl = self.inputs_outputs[name].implicit
             if type(impl) is not Unresolved:
                 params[name] = self.inputs_outputs[name].implicit
         params.update(**validate_parameters(params, self.outputs, defaults=self.defaults, subst=subst, fqname=self.fqname,
-                                                check_unknowns=False, check_required=not loosely, check_exist=not loosely))
+                                                check_unknowns=False, check_required=not loosely, 
+                                                check_inputs_exist=not loosely, check_outputs_exist=not loosely,
+                                                ))
         return params
 
     def rich_help(self, tree, max_category=ParameterCategory.Optional):
         """Generates help into a rich.tree.Tree object"""
         if self.info:
             tree.add("Description:").add(Markdown(self.info))
+        # extra documentation?
+        for section, content in self.extra_info.items():
+            if not section.lower().endswith("inputs") and not section.lower().endswith("outputs"):
+                tree.add(f"{section}:").add(Markdown(content))
         # adds tables for inputs and outputs
         for io, title in (self.inputs, "inputs"), (self.outputs, "outputs"):
+            # add extra help sections
+            for section, content in self.extra_info.items():
+                if section.lower().endswith(title):
+                    tree.add(f"{section}:").add(Markdown(content))
+            # add parameters by category
             for cat in ParameterCategory:
                 schemas = [(name, schema) for name, schema in io.items() if schema.get_category() == cat]
                 if not schemas:
                     continue
                 if cat > max_category:
                     subtree = tree.add(f"[dim]{cat.name} {title}: omitting {len(schemas)}[/dim]")
                     continue
@@ -423,7 +487,16 @@
     def assign_value(self, key: str, value: Any, override: bool = False):
         """assigns a parameter value to the cargo. 
         Recipe will override this to handle nested assignments. Cabs can't be assigned to
         (it will be handled by the wraping step)
         """
         raise AssignmentError(f"{self.name}: invalid assignment {key}={value}")
 
+    @staticmethod
+    def add_parameter_summary(params: Dict[str, Any], lines: List[str] = []):
+        for name, value in params.items():
+            if isinstance(value, (list, tuple)) and len(value) > 10:
+                sep1, sep2 = "()" if isinstance(value, tuple) else "[]" 
+                lines.append(f"  {name} = {sep1}{value[0]}, {value[1]}, ..., {value[-1]}{sep2}")
+            else:
+                lines.append(f"  {name} = {value}")
+        return lines
```

### Comparing `stimela-2.0rc4/scabha/configuratt/__init__.py` & `stimela-2.0rc6/scabha/configuratt/__init__.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/scabha/configuratt/cache.py` & `stimela-2.0rc6/scabha/configuratt/cache.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/scabha/configuratt/deps.py` & `stimela-2.0rc6/scabha/configuratt/deps.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/scabha/configuratt/resolvers.py` & `stimela-2.0rc6/scabha/configuratt/resolvers.py`

 * *Files 4% similar despite different names*

```diff
@@ -182,37 +182,47 @@
             # check for infinite recursion
             recurse += 1
             if recurse > 20:
                 raise ConfigurattError(f"{errloc}: recursion limit exceeded, check your _use and _include statements")
 
             # handle _include entries
             if includes:
-                include_files = pop_conf(conf, "_include", None)
-                if include_files:
+                include_directive = pop_conf(conf, "_include", None)
+                if include_directive:
                     updated = True
-                    if isinstance(include_files, str):
-                        include_files = [include_files]
-                    elif not isinstance(include_files, (tuple, list, ListConfig)) or not all(isinstance(x, str) for x in include_files):
-                        raise ConfigurattError(f"{errloc}: _include: must be a string or a list of strings")
+                    include_files = []
+                    # process includes recursively
+                    def process_include_directive(directive: str, subpath=None):
+                        if isinstance(directive, str):
+                            include_files.append(directive if subpath is None else f"{subpath}/{directive}")
+                        elif isinstance(directive, (tuple, list, ListConfig)):
+                            for dir1 in directive:
+                                process_include_directive(dir1, subpath)
+                        elif isinstance(directive, DictConfig):
+                            for key, value in directive.items_ex():
+                                process_include_directive(value, subpath=key if subpath is None else f"{subpath}/{key}")
+                        else:
+                            raise ConfigurattError(f"{errloc}: _include contains invalid entry of type {type(directive)}")
+                    process_include_directive(include_directive)
 
                     # load includes
                     accum_incl_conf = OmegaConf.create()
                     for incl in include_files:
                         if not incl:
                             raise ConfigurattError(f"{errloc}: empty _include specifier")
-                        # check for flags
+                        # check for [flags] at end of specifier
                         match = re.match("^(.*)\[(.*)\]$", incl)
                         if match:
                             incl = match.group(1)
                             flags = set([x.strip().lower() for x in match.group(2).split(",")])
                         else:
                             flags = {}
 
-                        # check for (module)filename.yaml style
-                        match = re.match("^\\((.+)\\)(.+)$", incl)
+                        # check for (module)filename.yaml or (module)/filename.yaml style
+                        match = re.match("^\\((.+)\\)/?(.+)$", incl)
                         if match:
                             modulename, filename = match.groups()
                             try:
                                 mod = importlib.import_module(modulename)
                             except ImportError as exc:
                                 if 'optional' in flags:
                                     dependencies.add_fail(FailRecord(incl, pathname, modulename=modulename, fname=filename))
```

### Comparing `stimela-2.0rc4/scabha/evaluator.py` & `stimela-2.0rc6/scabha/evaluator.py`

 * *Files 7% similar despite different names*

```diff
@@ -147,14 +147,19 @@
         return callable(*eval_args)
 
     def LIST(self, evaluator, args):
         def make_list(*x):
             return list(x)
         return self.evaluate_generic_callable(evaluator, "LIST", make_list, args)
 
+    def RANGE(self, evaluator, args):
+        def make_range(*x):
+            return list(range(*x))
+        return self.evaluate_generic_callable(evaluator, "RANGE", make_range, args, min_args=1, max_args=3)
+
     def MIN(self, evaluator, args):
         return self.evaluate_generic_callable(evaluator, "MIN", min, args, min_args=1)
 
     def MAX(self, evaluator, args):
         return self.evaluate_generic_callable(evaluator, "MAX", max, args, min_args=1)
 
     def IF(self, evaluator, args):
@@ -208,39 +213,52 @@
 
     def DIRNAME(self, evaluator, args):
         if len(args) != 1:
             raise FormulaError(f"{'.'.join(evaluator.location)}: DIRNAME() expects 1 argument, got {len(args)}")
         path = evaluator._evaluate_result(args[0])
         if type(path) is UNSET:
             return path
-        return os.path.dirname(str(path))
+        if not isinstance(path, str):
+            raise FormulaError(f"DIRNAME() expects a string, got a {str(type(path))}") 
+        return os.path.dirname(path)
 
     def BASENAME(self, evaluator, args):
         if len(args) != 1:
             raise FormulaError(f"{'.'.join(evaluator.location)}: BASENAME() expects 1 argument, got {len(args)}")
         path = evaluator._evaluate_result(args[0])
         if type(path) is UNSET:
             return path
-        return os.path.basename(str(path))
+        if not isinstance(path, str):
+            raise FormulaError(f"BASENAME() expects a string, got a {str(type(path))}") 
+        return os.path.basename(path)
 
     def EXTENSION(self, evaluator, args):
         if len(args) != 1:
             raise FormulaError(f"{'.'.join(evaluator.location)}: EXTENSION() expects 1 argument, got {len(args)}")
         path = evaluator._evaluate_result(args[0])
         if type(path) is UNSET:
             return path
-        return os.path.splitext(str(path))[1]
+        if not isinstance(path, str):
+            raise FormulaError(f"EXTENSION() expects a string, got a {str(type(path))}") 
+        return os.path.splitext(path)[1]
 
     def STRIPEXT(self, evaluator, args):
         if len(args) != 1:
             raise FormulaError(f"{'.'.join(evaluator.location)}: STRIPEXT() expects 1 argument, got {len(args)}")
         path = evaluator._evaluate_result(args[0])
         if type(path) is UNSET:
             return path
-        return os.path.splitext(str(path))[0]
+        if not isinstance(path, str):
+            raise FormulaError(f"STRIPEXT() expects a string, got a {str(type(path))}") 
+        return os.path.splitext(path)[0]
+
+    def NOSUBST(self, evaluator, args):
+        if len(args) != 1:
+            raise FormulaError(f"{'.'.join(evaluator.location)}: NOSUBST() expects 1 argument, got {len(args)}")
+        return evaluator._evaluate_result(args[0], subst=False)
 
 def construct_parser():
     lparen = Literal("(").suppress()
     rparen = Literal(")").suppress()
     lbrack = Keyword("[").suppress()
     rbrack = Keyword("]").suppress()
     comma = Literal(",").suppress()
@@ -260,15 +278,15 @@
     anyseq = CharsNotIn(",)")("constant")
 
     # allow expression to be used recursively
     expr = Forward()
     
     # functions
     functions = reduce(operator.or_, map(Keyword, ["IF", "IFSET", "GLOB", "EXISTS", "LIST", 
-        "BASENAME", "DIRNAME", "EXTENSION", "STRIPEXT", "MIN", "MAX"]))
+        "BASENAME", "DIRNAME", "EXTENSION", "STRIPEXT", "MIN", "MAX", "RANGE", "NOSUBST"]))
     # these functions take one argument, which could also be a sequence
     anyseq_functions = reduce(operator.or_, map(Keyword, ["GLOB", "EXISTS"]))
 
     atomic_value = (boolean | UNSET | EMPTY | nested_field | string | number)
 
     function_call_anyseq = Group(anyseq_functions + lparen + anyseq + rparen).setParseAction(FunctionHandler.pa)
     function_call = Group(functions + lparen + 
@@ -341,45 +359,45 @@
                         allow_unresolved: bool = False,
                         location: List[str] = []):
         self.ns = ns
         self.subst_context = subst_context
         self.location = location
         self.allow_unresolved = allow_unresolved
 
-    def _resolve(self, value, in_formula=True):
+    def _resolve(self, value, in_formula=True, subst=True):
         if type(value) is str:
             if in_formula and value == "SELF":
                 return SELF
             elif in_formula and value == "UNSET":
                 return UNSET
-            elif self.subst_context is not None:
+            elif self.subst_context is not None and subst:
                 try:
                     value = self.subst_context.evaluate(value, location=self.location)
                 except (KeyError, AttributeError) as exc:
                     raise SubstitutionError(f"{value}: invalid key {exc}")
                 except Exception as exc:
                     raise SubstitutionError(f"{value}: {exc}")
         return value
 
-    def empty(self, *args):
+    def empty(self, *args, **kw):
         return ""
 
-    def unset(self, *args):
+    def unset(self, *args, **kw):
         return UNSET
 
-    def self_value(self, *args):
+    def self_value(self, *args, **kw):
         return SELF
 
-    def constant(self, value):
-        return self._resolve(value)
+    def constant(self, value, subst=True, **kw):
+        return self._resolve(value, subst=subst)
 
-    def subexpression(self, value):
-        return self._evaluate_result(value, allow_unset=True)
+    def subexpression(self, value, subst=True):
+        return self._evaluate_result(value, allow_unset=True, subst=subst)
     
-    def namespace_lookup(self, *args):
+    def namespace_lookup(self, *args, subst=True):
         if len(args) == 1 and type(args[0]) is ParseResults:
             args = args[0]
             assert args._name == "namespace_lookup"
         value = self.ns
         fields = list(args)
         while fields:
             fld = fields.pop(0)
@@ -392,38 +410,38 @@
             if fld not in value:
                 if fields:
                     raise SubstitutionError(f"{'.'.join(self.location)}: '{fld}' undefined (in '{'.'.join(args)}')")
                 else:
                     return UNSET('.'.join(args))
             # this can still throw an error if a nested interpolation is invoked
             try:
-                value = value[fld]
+                value = value.get(fld, subst=subst)
             except (KeyError, AttributeError) as exc:
                 raise SubstitutionError(f"{'.'.join(self.location)}: '{'.'.join(args)}' unresolved (at '{exc}')")
-        return self._resolve(value)
+        return self._resolve(value, subst=subst)
 
-    def _evaluate_result(self, parse_result, allow_unset=False):
+    def _evaluate_result(self, parse_result, allow_unset=False, subst=True):
         allow_unset = allow_unset or self.allow_unresolved
         # if result is a handler, use evaluate
         if isinstance(parse_result, ResultsHandler):
             value = parse_result.evaluate(self)
 
         # if result is already a constant, resolve it
         elif type(parse_result) is not ParseResults:
-            return self._resolve(parse_result)
+            return self._resolve(parse_result, subst=subst)
         
         # lookup processing method based on name
         else:
             method = parse_result.getName()
             assert method is not None
             if not hasattr(self, method):
                 raise ParserError(f"{'.'.join(self.location)}: don't know how to deal with an element of type '{method}'")
 
             try:
-                value = getattr(self, method)(*parse_result)
+                value = getattr(self, method)(*parse_result, subst=subst)
             except SubstitutionError as exc:
                 if allow_unset:
                     return UNSET("", [exc])
                 raise
 
         if type(value) is UNSET and not allow_unset:
             raise UnsetError(f"'{value.value}' undefined")
```

### Comparing `stimela-2.0rc4/scabha/exceptions.py` & `stimela-2.0rc6/scabha/exceptions.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/scabha/logging_utils.py` & `stimela-2.0rc6/scabha/logging_utils.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/scabha/schema_utils.py` & `stimela-2.0rc6/scabha/schema_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,27 +118,30 @@
 
     decorator_chain = None
     for io in schemas.inputs, schemas.outputs:
         for name, schema in io.items():
 
             name = name.replace("_", "-")
             optname = f"--{name}"
+            dtype = schema.dtype
 
             # sort out option type
-            if schema.dtype == "bool":
+            if dtype == "bool":
                 optname = f"{optname}/--no-{name}"
                 dtype = bool
-            elif schema.dtype == "str":
+            elif dtype == "str":
                 dtype = str
-            elif schema.dtype == "int":
+            elif dtype == "int":
                 dtype = int
-            elif schema.dtype == "float":
+            elif dtype == "float":
                 dtype = float
-            elif schema.dtype == "MS":
-                dtype = click.Path(exists=True)
+            elif dtype in ("MS", "File", "Directory"):
+                dtype = click.Path(exists=(io is schemas.inputs))
+            else:
+                dtype = str
 
             # choices?
             if schema.choices:
                 dtype = click.Choice(schema.choices)
 
             # aliases?
             optnames = [optname]
```

### Comparing `stimela-2.0rc4/scabha/substitutions.py` & `stimela-2.0rc6/scabha/substitutions.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 
     def __setattr__(self, name: str, value: Any) -> None:
         SubstitutionNS._add_(self, name, value)
 
     def __setitem__(self, k: str, v: Any) -> None:
         SubstitutionNS._add_(self, k, v)
 
-    def get(self, name, default=None):
+    def get(self, name, default=None, subst=True):
         context = SubstitutionContext.current()
         # keep track of nested lookups, if doing substitutions
         nestloc = context.nested_location if context else None
         value = None # set to None, in case exception handler is invoked before value is set
         try:
             if nestloc is not None:
                 nestloc.append(name)
@@ -158,15 +158,15 @@
                     name = names[-1]
             # now look up again
             if name in self:
                 value = super().get(name)
                 if context:
                     if context.raise_errors and type(value) is Unresolved:
                         raise SubstitutionError(f"unresolved substitution for {name} ({value})")
-                    if not self._nosubst_:
+                    if subst and not self._nosubst_:
                         # recursive=False will invoke substitution on strings, but will return containers as is
                         value = context.evaluate(value, location=nestloc, recursive=False)
                 return value
             elif default in (KeyError, AttributeError):
                 raise default(name)
             else:
                 return default
```

### Comparing `stimela-2.0rc4/scabha/validate.py` & `stimela-2.0rc6/scabha/validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,16 @@
 
 def validate_parameters(params: Dict[str, Any], schemas: Dict[str, Any], 
                         defaults: Optional[Dict[str, Any]] = None,
                         subst: Optional[SubstitutionNS] = None,
                         fqname: str = "",
                         check_unknowns=True,    
                         check_required=True,
-                        check_exist=True,
+                        check_inputs_exist=True,
+                        check_outputs_exist=True,
                         create_dirs=False,
                         ignore_subst_errors=False,
                         ) -> Dict[str, Any]:
     """Validates a dict of parameter values against a given schema 
 
     Args:
         params (Dict[str, Any]):   map of input parameter values
@@ -86,16 +87,18 @@
         defaults (Dict[str, Any], optional): dictionary of default values to be used when a value is missing
         subst (SubsititionNS, optional): namespace to do {}-substitutions on parameter values
         fqname: fully-qualified name of the parameter set (e.g. "recipe_name.step_name"), used in error messages. If not given,
                 errors will report parameter names only
 
         check_unknowns (bool): if True, unknown parameters (not in schema) raise an error
         check_required (bool): if True, missing parameters with required=True will raise an error
-        check_exist (bool): if True, files with must_exist={None,True} in schema must exist, or will raise an error. 
-                            If False, only files with must_exist=True must exist.
+        check_inputs_exist (bool): if True, input files with must_exist={None,True} in schema must exist, or will raise an error. 
+                                   If False, doesn't check.
+        check_outputs_exist (bool): if True, output files with must_exist=True in schema must exist, or will raise an error. 
+                                   If False, doesn't check.
         create_dirs (bool): if True, non-existing directories in filenames (and parameters with mkdir=True in schema) 
                             will be created.
         ignore_subst_errors (bool): if True, substitution errors will be ignored
 
 
     Raises:
         ParameterValidationError: parameter fails validation
@@ -191,15 +194,18 @@
             continue
         dtype = schema._dtype
 
         is_file = is_file_type(dtype)
         is_file_list = is_filelist_type(dtype)
 
         # must this file exist? Schema may force this check, otherwise follow the default check_exist policy
-        must_exist = check_exist if schema.must_exist is None else schema.must_exist
+        if schema.is_input:
+            must_exist = check_inputs_exist and schema.must_exist is not False
+        elif schema.is_output:
+            must_exist = check_outputs_exist and schema.must_exist
 
         if is_file or is_file_list:
             # match to existing file(s)
             if type(value) is str:
                 # try to interpret string as a formatted list (a list substituted in would come out like that)
                 try:
                     files = yaml.safe_load(value)
```

### Comparing `stimela-2.0rc4/stimela/__init__.py` & `stimela-2.0rc6/stimela/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 from pathlib import Path
-
-__author__ = """Sphesihle Makhathini, Oleg Smirnov and RATT"""
-__email__ = "sphemakh@gmail.com"
-__version__ = "2.0rc2"
+#-----------
+# knicked from https://github.com/python-poetry/poetry/issues/273#issuecomment-1103812336
+from importlib import metadata
+__version__ = metadata.version(__package__)
+del metadata  # optional, avoids polluting the results of dir()
+#------------
 
 CONFIG = None
 
 UID = os.getuid()
 GID = os.getgid()
 
 root = os.path.dirname(__file__)
```

### Comparing `stimela-2.0rc4/stimela/backends/flavours/__init__.py` & `stimela-2.0rc6/stimela/backends/flavours/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,22 +17,28 @@
     # if true, full command line is logged, else just command name
     log_full_command: bool = True
 
     def finalize(self, cab: "stimela.kitchen.cab.Cab"):
         """Finalizes flavour definition, given a cab"""
         self.command_name = cab.command.split()[0]
 
-    def get_arguments(self, cab: "stimela.kitchen.cab.Cab", params: Dict[str, Any], subst: Dict[str, Any]):
+    def get_arguments(self, cab: "stimela.kitchen.cab.Cab", 
+                            params: Dict[str, Any], 
+                            subst: Dict[str, Any],
+                            virtual_env: Optional[str]=None,
+                            check_executable: bool = True):
         """Returns command line arguments for running this flavour of task, given
         a cab and a set of parameters. 
 
         Args:
             cab (Cab):               cab definition
             params (Dict[str, Any]): parameter dict
             subst (Dict[str, Any]):  substitution namespace 
+            virtual_env (Optional[str]): virtual environment to run in
+            check_executable:        if True, cab may check for the executable to exist (but doesn't have to)
         """
         pass
 
 
 @dataclass
 class _CallableFlavour(_BaseFlavour):
     """
```

### Comparing `stimela-2.0rc4/stimela/backends/flavours/binary.py` & `stimela-2.0rc6/stimela/backends/flavours/binary.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,27 +5,31 @@
 from stimela.exceptions import CabValidationError
 from stimela.kitchen.cab import Cab
 from scabha.cab_utils import CAB_OUTPUT_PREFIX
 from stimela.kitchen import wranglers
 from scabha.substitutions import substitutions_from
 
 from . import _CallableFlavour, _BaseFlavour
-
+import stimela
 
 @dataclass
 class BinaryFlavour(_BaseFlavour):
     """
     Represents a cab flavour that is a command run via the shell
     """
     kind: str = "binary"
 
-    def get_arguments(self, cab: Cab, params: Dict[str, Any], subst: Dict[str, Any]):
+    def get_arguments(self, cab: Cab, params: Dict[str, Any], subst: Dict[str, Any], 
+                      virtual_env: Optional[str]=None, check_executable: bool = True):
 
         # build command line from parameters
-        args, venv = cab.build_command_line(params, subst)
+        args = cab.build_command_line(params, subst, virtual_env=virtual_env, check_executable=check_executable)
 
         # prepend virtual env invocation, if asked
-        if venv:
-            args = ["/bin/bash", "--rcfile", f"{venv}/bin/activate", "-c", " ".join(shlex.quote(arg) for arg in args)]
+        if virtual_env:
+            args = ["/bin/bash", "--rcfile", f"{virtual_env}/bin/activate", "-c", " ".join(shlex.quote(arg) for arg in args)]
 
         return args
+    
+    def get_image_name(self, cab: Cab, backend: 'stimela.backend.StimelaBackendOptions'):
+        return cab.image.to_string(backend.default_registry)
```

### Comparing `stimela-2.0rc4/stimela/backends/flavours/casa.py` & `stimela-2.0rc6/stimela/backends/flavours/casa.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,29 +12,14 @@
 from stimela.kitchen import wranglers
 from scabha.substitutions import substitutions_from
 
 from . import _CallableFlavour, _BaseFlavour
 from .python_flavours import form_python_function_call
 
 
-def get_python_interpreter_args(cab: Cab, subst: Dict[str, Any]):
-    # get virtual env, if specified
-    with substitutions_from(subst, raise_errors=True) as context:
-        venv = context.evaluate(cab.virtual_env, location=["virtual_env"])
-
-    if venv:
-        venv = os.path.expanduser(venv)
-        interpreter = f"{venv}/bin/python"
-        if not os.path.isfile(interpreter):
-            raise CabValidationError(f"virtual environment {venv} doesn't exist")
-    else:
-        interpreter = "python"
-
-    return [interpreter]
-
 
 @dataclass
 class CasaTaskFlavour(_CallableFlavour):
     kind: str = "casa-task"
     casa: Optional[str] = None
     casa_opts: Optional[str] = None
 
@@ -44,15 +29,21 @@
         err_patt = re.compile("(?P<content>(\tSEVERE\t|ABORTING|\*\*\* Error \*\*\*)(.*))$")
         cab._wranglers.append((
             err_patt, [
                 wranglers.DeclareError(err_patt, "ERROR", message="CASA error: {content}" )
             ]
         ))
 
-    def get_arguments(self, cab: Cab, params: Dict[str, Any], subst: Dict[str, Any]):
+    def get_image_name(self, cab: Cab, backend: 'stimela.backend.StimelaBackendOptions'):
+        from stimela import CONFIG
+        return cab.image.to_string(backend.default_registry) if cab.image else CONFIG.images['default-casa']
+
+    def get_arguments(self, cab: Cab, params: Dict[str, Any], subst: Dict[str, Any], 
+                              virtual_env: Optional[str]=None, check_executable: bool = True):
+
         with substitutions_from(subst, raise_errors=True) as context:
             try:
                 command = context.evaluate(cab.command, location=["command"])
             except Exception as exc:
                 raise SubstitutionError(f"error substituting casa task '{cab.command}'", exc)
             if self.casa:
                 try:
@@ -65,23 +56,44 @@
                 try:
                     casa_opts = context.evaluate(self.casa_opts, location=["casa_opts"])
                 except Exception as exc:
                     raise SubstitutionError(f"error substituting casa options '{casa_opts}'", exc)
             else:
                 casa_opts = stimela.CONFIG.opts.runtime.get('casa_opts', "--log2term --nologger --nologfile")
 
+        # check for virtual_env
+        if virtual_env and "/" not in command:
+            command = f"{virtual_env}/bin/{command}"
+
         self.command_name = command
         # convert inputs into a JSON string
         pass_params = cab.filter_input_params(params)
         params_string = json.dumps(pass_params)
 
+        # unicode instance only exists in python2, python3 bytes
         code = f"""
-import sys, json;
-kw=json.loads(sys.argv[-1]);
+import sys, json
+kw = json.loads(sys.argv[-1])
+
+try:
+    utype = unicode
+except NameError:
+    utype = bytes
+
 def stringify(x):
-    return str(x) if type(x) is unicode else ([stringify(y) for y in x] if type(x) is list else x);
-kw={{key: stringify(value) for key, value in kw.items()}}; {command}(**kw);"""
+    if isinstance(x, (utype, str)):
+        return str(x)
+    elif isinstance(x, list):
+        return [stringify(y) for y in x]
+    else:
+        return x
+
+kw = {{key: stringify(value) for key, value in kw.items()}}
+
+{command}(**kw)
+
+"""
 
         args =  casa.strip().split() + casa_opts.strip().split() + ["-c", code, params_string]
         return args
```

### Comparing `stimela-2.0rc4/stimela/backends/flavours/python_flavours.py` & `stimela-2.0rc6/stimela/backends/flavours/python_flavours.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     """
     arguments = []
     for key, value in cab.filter_input_params(params).items():
         arguments.append(f"{key}={repr(value)}")
     return f"{function}({', '.join(arguments)})"
 
 
-def get_python_interpreter_args(cab: Cab, subst: Dict[str, Any]):
+def get_python_interpreter_args(cab: Cab, subst: Dict[str, Any], virtual_env: Optional[str]=None):
     """
     Helper. Given a cab definition, forms up appropriate argument list to
     invoke the interpreter. Invokes a virtual environment as appropriate.
 
     Args:
         cab (Cab):              cab definition 
         subst (Dict[str, Any]): substitution namespace
@@ -45,22 +45,19 @@
     Raises:
         CabValidationError: on errors
 
     Returns:
         List[str]: [command, arguments, ...] needed to invoke the interpreter
     """    
     # get virtual env, if specified
-    with substitutions_from(subst, raise_errors=True) as context:
-        venv = context.evaluate(cab.virtual_env, location=["virtual_env"])
-
-    if venv:
-        venv = os.path.expanduser(venv)
-        interpreter = f"{venv}/bin/python"
+    if virtual_env:
+        virtual_env = os.path.expanduser(virtual_env)
+        interpreter = f"{virtual_env}/bin/python"
         if not os.path.isfile(interpreter):
-            raise CabValidationError(f"virtual environment {venv} doesn't exist")
+            raise CabValidationError(f"virtual environment {virtual_env} doesn't exist")
     else:
         interpreter = "python"
 
     return [interpreter, "-u"]
 
 
 @dataclass
@@ -86,15 +83,20 @@
             wrangs = [wrangler]
             if not stimela.VERBOSE:
                 wrangs.append(wranglers.Suppress(pattern, "SUPPRESS"))
             cab._wranglers.append((pattern, wrangs))
         else:
             self._yield_output = ""
 
-    def get_arguments(self, cab: Cab, params: Dict[str, Any], subst: Dict[str, Any]):
+    def get_image_name(self, cab: Cab, backend: 'stimela.backend.StimelaBackendOptions'):
+        from stimela import CONFIG
+        return cab.image.to_string(backend.default_registry) if cab.image else CONFIG.images['default-python']
+
+    def get_arguments(self, cab: Cab, params: Dict[str, Any], subst: Dict[str, Any], 
+                      virtual_env: Optional[str]=None, check_executable: bool = True):
         # substitute command and split into module/function
         with substitutions_from(subst, raise_errors=True) as context:
             try:
                 command = context.evaluate(cab.command, location=["command"])
             except Exception as exc:
                 raise SubstitutionError(f"error substituting Python callable '{cab.command}'", exc)
 
@@ -127,15 +129,15 @@
     {py_function} = {py_function}.callback
 else:
     print("invoking callable {command}() using external interpreter")
 _result = {py_function}(**_inputs)
 {self._yield_output}
         """
 
-        args = get_python_interpreter_args(cab, subst)
+        args = get_python_interpreter_args(cab, subst, virtual_env=virtual_env)
         args += ["-c", code, params_string]
         return args
 
 
 @dataclass
 class PythonCodeFlavour(_BaseFlavour):
     """
@@ -159,15 +161,20 @@
         pattern = re.compile(f"{CAB_OUTPUT_PREFIX}(.*)")
         wrangs = [wranglers.ParseJSONOutputDict(pattern, "PARSE_JSON")]
         if not stimela.VERBOSE:
             wrangs.append(wranglers.Suppress(pattern, "SUPPRESS"))
         cab._wranglers.append((pattern, wrangs))
         self.command_name = "[python]"
 
-    def get_arguments(self, cab: Cab, params: Dict[str, Any], subst: Dict[str, Any]):
+    def get_image_name(self, cab: Cab, backend: 'stimela.backend.StimelaBackendOptions'):
+        from stimela import CONFIG
+        return cab.image.to_string(backend.default_registry) if cab.image else CONFIG.images['default-python']
+
+    def get_arguments(self, cab: Cab, params: Dict[str, Any], subst: Dict[str, Any], 
+                      virtual_env: Optional[str]=None, check_executable: bool = True):
         # do substitutions on command, if necessary
         if self.subst:
             with substitutions_from(subst, raise_errors=True) as context:
                 try:
                     command = context.evaluate(cab.command, location=["command"])
                 except Exception as exc:
                     raise SubstitutionError("error substituting inline Python code", exc)
@@ -197,10 +204,10 @@
             post_command += "from scabha.cab_utils import yield_output\n"
             if self.output_vars:
                 for name in pass_outputs:
                     var_name = name.replace("-", "_").replace(".", "__")
                     post_command += f"yield_output(**{{'{name}': {var_name}}})\n"                
 
         # form up interpreter invocation
-        args = get_python_interpreter_args(cab, subst)
+        args = get_python_interpreter_args(cab, subst, virtual_env=virtual_env)
         args += ["-c", pre_command + command + post_command, params_arg]
         return args
```

### Comparing `stimela-2.0rc4/stimela/backends/kubernetes/run_kube.py` & `stimela-2.0rc6/stimela/backends/kubernetes/run_kube.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,74 +1,31 @@
 from dataclasses import dataclass
 import logging, time, json, datetime, yaml, os.path, uuid, pathlib
 
 from typing import Dict, List, Optional, Any
-from enum import Enum
-from collections import OrderedDict
 
 from omegaconf import OmegaConf, DictConfig, ListConfig
 from scabha.basetypes import EmptyDictDefault, EmptyListDefault
 
 import stimela
 from stimela.kitchen.cab import Cab
-from stimela.kitchen.step import Step
-from stimela.utils.xrun_asyncio import xrun, dispatch_to_log
+from stimela.utils.xrun_asyncio import dispatch_to_log
 from stimela.exceptions import StimelaCabParameterError, StimelaCabRuntimeError, CabValidationError
 from stimela.stimelogging import log_exception
 from stimela.backends import resolve_required_mounts
 # these are used to drive the status bar
 from stimela.stimelogging import declare_subcommand, declare_subtask, update_process_status
 
 import kubernetes
 from kubernetes.client.api import core_v1_api
 from kubernetes.client.rest import ApiException
 from kubernetes.stream import stream
 from dask_kubernetes import make_pod_spec, KubeCluster
 
-@dataclass
-class KubernetesDaskRuntime(object):
-    num_workers: int = 0
-    cpu_limit: int = 1
-    memory_limit: Optional[str] = None
-    threads_per_worker: int = 1
-    name: Optional[str] = None
-    persist: bool = False
-
-# dict of methods for converting an object to text format
-_InjectedFileFormatters = dict(
-    yaml = yaml.dump,
-    json = json.dumps,
-    txt = str
-)
-
-InjectedFileFormats = Enum("InjectedFileFormats", " ".join(_InjectedFileFormatters.keys()), module=__name__)
-
-@dataclass
-class KubernetesFileInjection(object):
-    format: InjectedFileFormats = "txt"
-    content: Any = ""
-
-@dataclass
-class KubernetesLocalMount(object):
-    path: str
-    dest: str = ""              # destination path -- same as local if empty
-    readonly: bool = False      # mount as readonly, but it doesn't work (yet?)
-    mkdir: bool = False         # create dir, if it is missing
-
-@dataclass
-class KubernetesRuntime(object):
-    namespace: str
-    dask_cluster: KubernetesDaskRuntime = KubernetesDaskRuntime()
-    inject_files: Dict[str, KubernetesFileInjection] = EmptyDictDefault()
-    pre_commands: List[str] = EmptyListDefault()
-    local_mounts: Dict[str, KubernetesLocalMount] = EmptyDictDefault()
-    env: Dict[str, str] = EmptyDictDefault()
-    run_dir: str = "."          # directory to run in inside container
-
-KubernetesRuntimeSchema = OmegaConf.structured(KubernetesRuntime)
+from . import KubernetesRuntimeSchema, _InjectedFileFormatters
 
 _kube_client = _kube_config = None
 
 def get_kube_api():
     global _kube_client
     global _kube_config
 
@@ -77,15 +34,15 @@
         kubernetes.config.load_kube_config()
 
     return core_v1_api.CoreV1Api()
 
 
 
 def run(cab: Cab, params: Dict[str, Any], runtime: Dict[str, Any], fqname: str,
-        log: logging.Logger, subst: Optional[Dict[str, Any]] = None, batch=None):
+        log: logging.Logger, subst: Optional[Dict[str, Any]] = None):
     """Runs cab contents
 
     Args:
         cab (Cab): cab object
         log (logger): logger to use
         subst (Optional[Dict[str, Any]]): Substitution dict for commands etc., if any.
```

### Comparing `stimela-2.0rc4/stimela/backends/native/run_native.py` & `stimela-2.0rc6/stimela/backends/native/run_native.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,72 +1,81 @@
-import logging, datetime, resource
+import logging, datetime, resource, os.path
 
-from typing import Dict, Optional, Any
+from typing import Dict, Optional, Any, List
 
 import stimela
-from stimela.kitchen.cab import Cab
+import stimela.kitchen
 from stimela.utils.xrun_asyncio import xrun
-from stimela.schedulers.slurm import SlurmBatch
-from stimela.schedulers import SlurmBatch
-from stimela.exceptions import StimelaProcessRuntimeError
+from stimela.exceptions import StimelaProcessRuntimeError, BackendSpecificationError
+from scabha.substitutions import substitutions_from
 
 
 def update_rlimits(rlimits: Dict[str, Any], log: logging.Logger):
     for name, limit in rlimits.items():
         rname = f"RLIMIT_{name}"
         if not hasattr(resource, rname):
-            raise StimelaProcessRuntimeError(f"unknown resource limit 'opts.rlimits.{name}'")
+            raise StimelaProcessRuntimeError(f"unknown resource limit 'backend.rlimits.{name}'")
         rconst = getattr(resource, rname)
         # get current limits
         soft, hard = resource.getrlimit(rconst)
         # check for unlimited
         if limit is None:
             limit = resource.RLIM_INFINITY
             if hard != resource.RLIM_INFINITY:
-                raise StimelaProcessRuntimeError(f"can't set opts.rlimits.{name}=unlimited: hard limit is {hard}")
+                raise StimelaProcessRuntimeError(f"can't set backend.rlimits.{name}=unlimited: hard limit is {hard}")
         else:
             if limit > hard:
-                raise StimelaProcessRuntimeError(f"can't set opts.rlimits.{name}={limit}: hard limit is {hard}")
+                raise StimelaProcessRuntimeError(f"can't set backend.rlimits.{name}={limit}: hard limit is {hard}")
         resource.setrlimit(rconst, (limit, hard))
         log.debug(f"setting soft limit {name}={limit} (hard limit is {hard})")
 
 
-def run(cab: Cab, params: Dict[str, Any], runtime: Dict[str, Any], fqname: str,
-        log: logging.Logger, subst: Optional[Dict[str, Any]] = None, batch=None):
+
+def build_command_line(cab: 'stimela.kitchen.cab.Cab', params: Dict[str, Any], subst: Optional[Dict[str, Any]] = None,
+                        virtual_env: Optional[str] = None):
+    return cab.flavour.get_arguments(cab, params, subst, virtual_env=virtual_env)
+
+
+def run(cab: 'stimela.kitchen.cab.Cab', params: Dict[str, Any], fqname: str,
+        backend: 'stimela.backend.StimelaBackendOptions',
+        log: logging.Logger, subst: Optional[Dict[str, Any]] = None):
     """Runs cab contents
 
     Args:
         cab (Cab): cab object
         log (logger): logger to use
         subst (Optional[Dict[str, Any]]): Substitution dict for commands etc., if any.
 
     Returns:
         Any: return value (e.g. exit code) of content
     """
-    update_rlimits(stimela.CONFIG.opts.rlimits, log)
+    update_rlimits(backend.rlimits, log)
 
-    args = cab.flavour.get_arguments(cab, params, subst)
+    venv = search = None
+    if backend.native and backend.native.virtual_env:
+        try:
+            with substitutions_from(subst, raise_errors=True) as context:
+                venv = context.evaluate(backend.native.virtual_env, 
+                                        location=["backend.native.virtual_env"])
+        except Exception as exc:
+            raise BackendSpecificationError(f"error evaluating backend.native.virtual_env", exc)
+        if venv:
+            venv = os.path.expanduser(venv)
+            if not os.path.isfile(f"{venv}/bin/activate"):
+                raise BackendSpecificationError(f"virtual environment {venv} doesn't exist")
+            log.debug(f"virtual environment is {venv}")
+
+    args = build_command_line(cab, params, subst, virtual_env=venv)
 
     log.debug(f"command line is {args}")
 
     cabstat = cab.reset_status()
 
     command_name = cab.flavour.command_name
 
-    if batch:
-        batch = SlurmBatch(**batch)
-        batch.__init_cab__(cabstat.cab, params, subst, log)
-        runcmd = "/bin/bash -c" + " ".join(args)
-        jobfile = "foo-bar.job"
-        batch.name = "foo-bar"
-        batch.submit(jobfile=jobfile, runcmd=runcmd)
-
-        return
-
-    #-------------------------------------------------------
     # run command
     start_time = datetime.datetime.now()
     def elapsed(since=None):
         """Returns string representing elapsed time"""
         return str(datetime.datetime.now() - (since or start_time)).split('.', 1)[0]
 
     # log.info(f"argument lengths are {[len(a) for a in args]}")
```

### Comparing `stimela-2.0rc4/stimela/backends/podman.py` & `stimela-2.0rc6/stimela/backends/podman.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 from stimela import utils
 import json
 import stimela
 import time
 import datetime
 import tempfile
 
+def is_available():
+    return False
+
+def get_status():
+    return "not yet implemented"
+
 
 class DockerError(Exception):
     pass
 
 
 def build(image, build_path, tag=None, build_args=None, fromline=None, args=[]):
     """ build a podman image"""
```

### Comparing `stimela-2.0rc4/stimela/commands/build.py` & `stimela-2.0rc6/stimela/commands/build.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/stimela/commands/cabs.py` & `stimela-2.0rc6/stimela/commands/cabs.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/stimela/commands/clean.py` & `stimela-2.0rc6/stimela/commands/clean.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/stimela/commands/containers.py` & `stimela-2.0rc6/stimela/commands/containers.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/stimela/commands/doc.py` & `stimela-2.0rc6/stimela/commands/doc.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/stimela/commands/images.py` & `stimela-2.0rc6/stimela/commands/images.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/stimela/commands/ps.py` & `stimela-2.0rc6/stimela/commands/ps.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/stimela/commands/pull.py` & `stimela-2.0rc6/stimela/commands/pull.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/stimela/commands/push.py` & `stimela-2.0rc6/stimela/commands/push.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/stimela/commands/run.py` & `stimela-2.0rc6/stimela/commands/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from scabha import configuratt
 from scabha.basetypes import UNSET
 from scabha.exceptions import ScabhaBaseException
 from stimela import stimelogging
 import stimela.config
 from stimela.config import ConfigExceptionTypes
 from stimela import logger, log_exception
-from stimela.exceptions import RecipeValidationError, StimelaRuntimeError, StepSelectionError
+from stimela.exceptions import RecipeValidationError, StimelaRuntimeError, StepSelectionError, StimelaBaseException
 from stimela.main import cli
 from stimela.kitchen.recipe import Recipe, Step, RecipeSchema, join_quote
 from stimela import task_stats
 
 def load_recipe_file(filename: str):
     dependencies = stimela.config.get_initial_deps()
 
@@ -199,15 +199,15 @@
             if recipe_name not in conf:
                 log_exception(f"{what} does not contain recipe '{recipe_name}'")
                 sys.exit(2)
         elif last_recipe or len(all_recipe_names) == 1:
             recipe_name = all_recipe_names[-1]
         else:
             print(f"This file contains the following recipes: {', '.join(all_recipe_names)}")
-            log_exception(f"multiple recipes found, please specify one on the command line")
+            log_exception(f"multiple recipes found, please specify one on the command line, or use -l/--last-recipe")
             sys.exit(2)
         
         log.info(f"selected recipe is '{recipe_name}'")
 
         # create recipe object from the config
         kwargs = dict(**stimela.CONFIG.lib.recipes[recipe_name])
         kwargs.setdefault('name', recipe_name)
@@ -220,18 +220,28 @@
 
         # force name, if not set
         if not recipe.name:
             recipe.name = recipe_name
 
         # wrap it in an outer step and prevalidate (to set up loggers etc.)
         recipe.fqname = recipe_name
-        recipe.finalize()
+        try:
+            recipe.finalize()
+        except Exception as exc:
+            log_exception(RecipeValidationError(f"error validating recipe '{recipe_name}'", exc))
+            for line in traceback.format_exc().split("\n"):
+                log.debug(line)
+            sys.exit(1)        
         
         for key, value in params.items():
-            recipe.assign_value(key, value, override=True)
+            try:
+                recipe.assign_value(key, value, override=True)
+            except ScabhaBaseException as exc:
+                log_exception(exc)
+                sys.exit(1)
 
         # split out parameters
         params = {key: value for key, value in params.items() if key in recipe.inputs_outputs}
 
         stimelogging.declare_chapter("prevalidation")
         log.info("pre-validating the recipe")
         outer_step = Step(recipe=recipe, name=f"{recipe_name}", info=what, params=params)
@@ -274,15 +284,15 @@
         sys.exit(0)
 
     start_time = datetime.now()
     def elapsed():
         return str(datetime.now() - start_time).split('.', 1)[0]
 
     try:
-        outputs = outer_step.run()
+        outputs = outer_step.run(backend=stimela.CONFIG.opts.backend)
     except Exception as exc:
         task_stats.save_profiling_stats(outer_step.log, 
             print_depth=profile if profile is not None else stimela.CONFIG.opts.profile.print_depth,
             unroll_loops=stimela.CONFIG.opts.profile.unroll_loops)
         if not isinstance(exc, ScabhaBaseException) or not exc.logged:
             log_exception(StimelaRuntimeError(f"run failed after {elapsed()}", exc, 
                 tb=not isinstance(exc, ScabhaBaseException)))
```

### Comparing `stimela-2.0rc4/stimela/commands/save_config.py` & `stimela-2.0rc6/stimela/commands/save_config.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/stimela/config.py` & `stimela-2.0rc6/stimela/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,38 +12,15 @@
 from stimela.exceptions import *
 from stimela import log_exception
 
 CONFIG_FILE = os.path.expanduser("~/.config/stimela.conf")
 
 from scabha import configuratt
 from scabha.cargo import ListOrString, EmptyDictDefault, EmptyListDefault
-from stimela.kitchen.cab import CabManagement 
-
-
-## schema for a stimela image
-
-@dataclass
-class ImageBuildInfo:
-    info: Optional[str] = ""
-    dockerfile: Optional[str] = "Dockerfile"
-    production: Optional[bool] = True          # False can be used to mark test (non-production) images 
-
-
-@dataclass
-class StimelaImage:
-    name: str = MISSING
-    info: str = "image description"
-    images: Dict[str, ImageBuildInfo] = MISSING
-    _path: Optional[str] = None   # path to image definition yaml file, if any
-
-    # optional library of common parameter sets
-    params: Dict[str, Any] = EmptyDictDefault()
-
-    # optional library of common management settings
-    management: Dict[str, CabManagement] = EmptyDictDefault()
+from stimela.backends import StimelaBackendOptions
 
 
 @dataclass 
 class StimelaLogConfig(object):
     enable: bool = True                          
     name: str = "log-{info.fqname}"          # Default name for log file. info dict and {config.x.y} is substituted.
     ext: str = ".txt"                        # Default extension for log file.
@@ -60,67 +37,41 @@
 
 
 
 ## overall Stimela config schema
 
 import stimela.backends
 
-Backend = Enum("Backend", "docker singularity podman kubernetes native", module=__name__)
-
-SUPPORTED_BACKENDS = set(Backend.__members__)
-AVAILABLE_BACKENDS = {}
-BACKEND_STATUS = {}
-
-for _name in SUPPORTED_BACKENDS:
-    backend = __import__(f"stimela.backends.{_name}", fromlist=[_name])
-    if getattr(backend, 'AVAILABLE', None):
-        AVAILABLE_BACKENDS[_name] = backend
-        BACKEND_STATUS[_name] = backend.STATUS
-    else:
-        if hasattr(backend, 'STATUS'):
-            BACKEND_STATUS[_name] = backend.STATUS
-        else:
-            BACKEND_STATUS[_name] = "not implemented"
-
-def get_backend_status(name):
-    return BACKEND_STATUS.get(name, "unknown status")
-
 
 @dataclass
 class StimelaProfilingOptions(object):
     print_depth: int = 9999
     unroll_loops: bool = False
 
 @dataclass
 class StimelaOptions(object):
-    backend: Backend = "native" #TODO(Sphe):: Maybe docker/singularity makes more sense
-    registry: str = "quay.io"
-    basename: str = "stimela/v2-"
-    singularity_image_dir: str = "~/.singularity"
+    backend: StimelaBackendOptions = StimelaBackendOptions()
     log: StimelaLogConfig = StimelaLogConfig()
     ## list of paths to search with _include
     include: List[str] = EmptyListDefault()
-    ## For distributed computes and cpu allocation
-    dist: Dict[str, Any] = EmptyDictDefault()  
-    ## Resource limits -- see resource module
-    rlimits: Dict[str, Any] = EmptyDictDefault()
     ## Miscellaneous runtime option 
     runtime: Dict[str, Any] = EmptyDictDefault()
     ## Profiling options
     profile: StimelaProfilingOptions = StimelaProfilingOptions()
 
 
 def DefaultDirs():
     return field(default_factory=lambda:dict(indir='.', outdir='.'))
 
 _CONFIG_BASENAME = "stimela.conf"
 _STIMELA_CONFDIR = os.path.os.path.expanduser("~/.stimela")
 
 # dict of config file locations to check, in order of preference
 CONFIG_LOCATIONS = OrderedDict(
+    package = os.path.join(os.path.dirname(__file__), _CONFIG_BASENAME),
     local   = _CONFIG_BASENAME,
     venv    = os.environ.get('VIRTUAL_ENV', None) and os.path.join(os.environ['VIRTUAL_ENV'], _CONFIG_BASENAME),
     stimela = os.path.isdir(_STIMELA_CONFDIR) and os.path.join(_STIMELA_CONFDIR, _CONFIG_BASENAME),
     user    = os.path.join(os.path.expanduser("~/.config"), _CONFIG_BASENAME),
 )
 
 # set to the config file that was actually found
@@ -204,28 +155,22 @@
         recipes: Dict[str, Any] = EmptyDictDefault()
         steps: Dict[str, Any] = EmptyDictDefault()
         misc: Dict[str, Any] = EmptyDictDefault()
         wisdom: Dict[str, Any] = EmptyDictDefault()
 
     @dataclass 
     class StimelaConfig:
-        base: Dict[str, StimelaImage] = EmptyDictDefault()
+        images: Dict[str, str] = EmptyDictDefault()
         lib: StimelaLibrary = StimelaLibrary()
         cabs: Dict[str, Cab] = EmptyDictDefault()
         opts: StimelaOptions = StimelaOptions()
         vars: Dict[str, Any] = EmptyDictDefault()
         run:  Dict[str, Any] = EmptyDictDefault()
 
-    base_configs_glob = f"{STIMELA_DIR}/cargo/base/*/*.yaml"
-    lib_configs_glob = f"{STIMELA_DIR}/cargo/lib/params/*.yaml"
-    cab_configs_glob = f"{STIMELA_DIR}/cargo/cab/*.yaml"
-
-    base_configs = glob.glob(base_configs_glob)
-    lib_configs = glob.glob(lib_configs_glob)
-    cab_configs = glob.glob(cab_configs_glob)
+    base_configs = lib_configs = cab_configs = []
 
     if use_sys_config:
         sys_configs = [config_file for config_file in CONFIG_LOCATIONS.values()
                         if config_file and os.path.exists(config_file)]
     else:
         sys_configs = []
 
@@ -236,32 +181,21 @@
     if conf is not None:
         log.info("loaded full configuration from cache")
     else:
         log.info("loading configuration")
         dependencies = get_initial_deps()
 
         # start with empty structured config containing schema
-        base_schema = OmegaConf.structured(StimelaImage) 
         cab_schema = OmegaConf.structured(Cab)
         opts_schema = OmegaConf.structured(StimelaOptions)
 
         StimelaConfigSchema = OmegaConf.structured(StimelaConfig)
 
         conf = StimelaConfigSchema.copy()
 
-        # merge base/*/*yaml files into the config, under base.imagename
-        try:
-            conf.base, deps = configuratt.load_nested(base_configs, use_sources=[conf], structured=base_schema, 
-                                                        nameattr='name', include_path='_path', location='base', 
-                                                        use_cache=False, verbose=verbose)
-            dependencies.update(deps)
-        except Exception as exc:
-            log_exception(ConfigError(f"error loading base configuration", exc))
-            return None
-
         # merge lib/params/*yaml files into the config
         try:
             conf.lib.params, deps = configuratt.load_nested(lib_configs,  use_sources=[conf], 
                                                                 location='lib.params', include_path='_path') 
             dependencies.update(deps)
         except Exception as exc:
             if verbose:
@@ -305,15 +239,15 @@
         # add local configs
         for path in extra_configs:
             conf = _load(conf, path)
 
         if not CONFIG_LOADED:
             log.info("no user-supplied configuration files given, using defaults")
 
-        dependencies.replace((base_configs_glob, cab_configs_glob, lib_configs_glob), STIMELA_DIR)
+        # dependencies.replace((base_configs_glob, cab_configs_glob, lib_configs_glob), STIMELA_DIR)
 
         configuratt.save_cache(all_configs, conf, dependencies, extra_keys=extra_cache_keys, verbose=verbose)
 
     # add dotlist settings
     if extra_dotlist:
         try:
             dotlist_conf = OmegaConf.from_dotlist(extra_dotlist)
```

### Comparing `stimela-2.0rc4/stimela/exceptions.py` & `stimela-2.0rc6/stimela/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 class BackendError(StimelaBaseException):
     pass
 
 class CabValidationError(StimelaBaseException):
     pass
 
+class BackendSpecificationError(StimelaBaseException):
+    pass
+
 class SchemaError(StimelaBaseException):
     pass
 
 class DefinitionError(StimelaBaseException):
     pass
 
 class StepValidationError(StimelaBaseException):
```

### Comparing `stimela-2.0rc4/stimela/kitchen/batch.py` & `stimela-2.0rc6/stimela/kitchen/batch.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from typing import Any, List, Dict, Optional, Union
 from dataclasses import dataclass
 
 from scabha.basetypes import EmptyDictDefault, EmptyListDefault
-
-from .cab import Cab
-
+import stimela.kitchen
 
 @dataclass
 class Batch:
     scheduler: str = "slurm"
     cpus: int = 4
     mem: str = "128gb"
     email: Optional[str] = None
 
-    def __init_cab__(self, cab: Cab, params: Dict[str, Any], subst: Optional[Dict[str, Any]], log: Any=None):
+    def __init_cab__(self, cab: 'stimela.kitchen.cab.Cab', params: Dict[str, Any], subst: Optional[Dict[str, Any]], log: Any=None):
         self.cab = cab
         self.log = log
         self.args, self.venv = self.cab.build_command_line(params, subst)
```

### Comparing `stimela-2.0rc4/stimela/kitchen/cab.py` & `stimela-2.0rc6/stimela/kitchen/cab.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,66 @@
 import os.path, re, stat, itertools, logging, yaml, shlex
 from typing import Any, List, Dict, Optional, Union
 from collections import OrderedDict
 from enum import Enum, IntEnum
 from dataclasses import dataclass
-from omegaconf import MISSING, OmegaConf
+from omegaconf import MISSING, OmegaConf, DictConfig
+from omegaconf.errors import OmegaConfBaseException
 import rich.markup
 
 from scabha.cargo import Parameter, Cargo, ListOrString, ParameterPolicies, ParameterCategory
 from stimela.exceptions import CabValidationError, StimelaCabRuntimeError
 from scabha.exceptions import SchemaError
 from scabha.basetypes import EmptyDictDefault, EmptyListDefault
-from stimela.backends import flavours
+from stimela.backends import flavours, StimelaBackendSchema
 import stimela
 from . import wranglers
 from scabha.substitutions import substitutions_from
 
 ParameterPassingMechanism = Enum("ParameterPassingMechanism", "args yaml", module=__name__)
 
 
 @dataclass 
-class CabManagement:        # defines common cab management behaviours
+class CabManagement(object):        # defines common cab management behaviours
     environment: Optional[Dict[str, str]] = EmptyDictDefault()
     cleanup: Optional[Dict[str, ListOrString]]     = EmptyDictDefault()   
     wranglers: Optional[Dict[str, ListOrString]]   = EmptyDictDefault()   
 
+@dataclass
+class ImageInfo(object):
+    name: str                           # image name
+    registry: Optional[str] = None      # registry/org or org (for Dockerhub)
+    version: str = "latest"
+
+    @staticmethod
+    def from_string(spec: str):
+        """Creates ImageInfo from string"""
+        # get version specs
+        if ":" in spec:
+            spec, version = spec.rsplit(":", 1)
+        else:
+            version = "latest"
+        # get registry
+        if "/" in spec:
+            registry, name = spec.rsplit("/", 1)
+        else:
+            registry, name = None, spec
+        return ImageInfo(name, registry, version)
+    
+    def to_string(self, default_registry=None):
+        registry = self.registry or default_registry
+        if registry:
+            return f"{self.registry}/{self.name}:{self.version}"
+        else:        
+            return f"{self.name}:{self.version}"
+        
+    def __str__(self):
+        return self.to_string()
+
+ImageInfoSchema = OmegaConf.structured(ImageInfo)
 
 @dataclass
 class Cab(Cargo):
     """Represents a cab i.e. an atomic task in a recipe.
     See dataclass fields below for documentation of fields.
 
     Additional attributes available after validation with arguments:
@@ -36,129 +69,132 @@
         self.missing_params:    dict (name to Parameter) of required parameters that have not been specified
     
     Raises:
         CabValidationError: [description]
     """
     # if set, the cab is run in a container, and this is the image name
     # if not set, commands are run by the native runner
-    image: Optional[str] = None                   
+    image: Optional[Any] = None                   
 
     # command to run, inside the container or natively
     command: str = MISSING
 
-    # if set, activates this virtual environment first before running the command (not much sense doing this inside the container)
-    virtual_env: Optional[str] = None
+    ## moved to backend: native
+    # # if set, activates this virtual environment first before running the command (not much sense doing this inside the container)
+    # virtual_env: Optional[str] = None
 
     # cab flavour. Default will run the command as a binary (inside image or virtual_env). Otherwise specify
     # a string flavour, or a mapping to specify options (see backends.flavours)
     flavour: Optional[Any] = None
 
+    # overrides backend options
+    backend: Optional[Dict[str, Any]] = None
+
     # controls how params are passed. args: via command line argument, yml: via a single yml string
     parameter_passing: ParameterPassingMechanism = ParameterPassingMechanism.args
 
     # cab management and cleanup definitions
     management: CabManagement = CabManagement()
 
     # default parameter conversion policies
     policies: ParameterPolicies = ParameterPolicies()
 
-    # For callable-type cabs, determines how the return value is treated.
-    # None to ignore, "{}" to treat it as a dict of outputs, else an output name to 
-    # treat it as a single output
-    return_outputs: Optional[str] = "{}" 
-
-    # runtime settings
-    backend: Optional['stimela.config.Backend']
-    runtime: Dict[str, Any] = EmptyDictDefault()
-
-    _path: Optional[str] = None   # path to image definition yaml file, if any
-
     def __post_init__ (self):
         if self.name is None:
-            self.name = self.image or self.command.split()[0]
+            self.name = self.command.split()[0] or self.image
         Cargo.__post_init__(self)
         for param in self.inputs.keys():
             if param in self.outputs:
                 raise CabValidationError(f"cab {self.name}: parameter '{param}' appears in both inputs and outputs")
+            
+        # check image setting
+        if self.image:
+            if type(self.image) is str:
+                self.image = ImageInfo.from_string(self.image)
+            elif isinstance(self.image, DictConfig):
+                try:
+                    self.image = OmegaConf.to_container(OmegaConf.merge(ImageInfoSchema, self.image))
+                except OmegaConfBaseException as exc:
+                    raise CabValidationError(f"cab {self.name}: invalid image setting", exc)
+            else:
+                raise CabValidationError(f"cab {self.name}: invalid image setting")
+            
+        # check backend setting
+        if self.backend:
+            try:
+                OmegaConf.merge(StimelaBackendSchema, self.backend)
+            except OmegaConfBaseException as exc:
+                raise CabValidationError(f"cab {self.name}: invalid backend setting", exc)
 
         # setup wranglers
         self._wranglers = []
         for pattern, actions in self.management.wranglers.items():
             self._wranglers.append(wranglers.create_list(pattern, actions))
 
         # check flavours
         self.flavour = flavours.init_cab_flavour(self)
 
 
     def summary(self, params=None, recursive=True, ignore_missing=False):
         lines = [f"cab {self.name}:"] 
         if params is not None:
-            for name, value in params.items():
-                # if type(value) is validate.Error:
-                #     lines.append(f"  {name} = ERR: {value}")
-                # else:
-                lines.append(f"  {name} = {value}")
+            Cargo.add_parameter_summary(params, lines)
             lines += [f"  {name} = ???" for name, schema in self.inputs_outputs.items()
                         if name not in params and (not ignore_missing or schema.required)]
         return lines
 
     def rich_help(self, tree, max_category=ParameterCategory.Optional):
         tree.add(f"command: {self.command}")
         if self.image:
             tree.add(f"image: {self.image}")
-        if self.virtual_env:
-            tree.add(f"virtual environment: {self.virtual_env}")
+        ## moved to backend.native options
+        # if self.virtual_env:
+        #     tree.add(f"virtual environment: {self.virtual_env}")
         Cargo.rich_help(self, tree, max_category=max_category)
 
     def get_schema_policy(self, schema, policy, default=None):
         """Resolves a policy setting. If the policy is set here, returns it. If None and set in the cab,
         returns that. Else returns default value.
         """
         if getattr(schema.policies, policy) is not None:
             return getattr(schema.policies, policy)
         elif getattr(self.policies, policy) is not None:
             return getattr(self.policies, policy)
         else:
             return default
 
-    def build_command_line(self, params: Dict[str, Any], subst: Optional[Dict[str, Any]] = None, search=True):
-
+    def build_command_line(self, params: Dict[str, Any], 
+                           subst: Optional[Dict[str, Any]] = None, 
+                           virtual_env: Optional[str] = None,
+                           check_executable: bool = True):
+        
         try:
             with substitutions_from(subst, raise_errors=True) as context:
-                venv = context.evaluate(self.virtual_env, location=["virtual_env"])
                 command = context.evaluate(self.command, location=["command"])
         except Exception as exc:
             raise CabValidationError(f"error constructing cab command", exc)
 
-        if venv:
-            venv = os.path.expanduser(venv)
-            if not os.path.isfile(f"{venv}/bin/activate"):
-                raise CabValidationError(f"virtual environment {venv} doesn't exist")
-            self.log.debug(f"virtual environment is {venv}")
-        else:
-            venv = None
-
         command_line = shlex.split(os.path.expanduser(command))
         command = command_line[0]
         args = command_line[1:]
         # collect command
-        if search:
+        if check_executable:
             if "/" not in command:
                 from scabha.proc_utils import which
                 command0 = command
-                command = which(command, extra_paths=venv and [f"{venv}/bin"])
+                command = which(command, extra_paths=virtual_env and [f"{virtual_env}/bin"])
                 if command is None:
                     raise CabValidationError(f"{command0}: not found", log=self.log)
             else:
                 if not os.path.isfile(command) or not os.stat(command).st_mode & stat.S_IXUSR:
                     raise CabValidationError(f"{command} doesn't exist or is not executable")
 
         self.log.debug(f"command is {command}")
 
-        return ([command] + args + self.build_argument_list(params)), venv
+        return [command] + args + self.build_argument_list(params)
 
     def update_environment(self, subst):
         try:
             with substitutions_from(subst, raise_errors=True) as context:
                 environ = CabManagement().environment
                 for key,val in self.management.environment.items():
                     environ[key] = context.evaluate(val,
```

### Comparing `stimela-2.0rc4/stimela/kitchen/recipe.py` & `stimela-2.0rc6/stimela/kitchen/recipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import os, os.path, re, fnmatch, copy, traceback
 from typing import Any, Tuple, List, Dict, Optional, Union
 from dataclasses import dataclass
 from omegaconf import MISSING, OmegaConf, DictConfig, ListConfig
+from omegaconf.errors import OmegaConfBaseException
 from collections import OrderedDict
 from collections.abc import Mapping
 import rich.table
 
 from concurrent.futures import ProcessPoolExecutor
 
 from stimela.config import EmptyDictDefault, EmptyListDefault
 import stimela
 from stimela import log_exception, stimelogging
 from stimela.exceptions import *
-from scabha.basetypes import SkippedOutput
+from stimela.backends import StimelaBackendSchema
 from scabha.validate import evaluate_and_substitute, Unresolved, join_quote
 from scabha.substitutions import SubstitutionNS
 from scabha.cargo import Parameter, Cargo, ParameterCategory
 from scabha.basetypes import File, Directory, MS, UNSET, Placeholder
 from .cab import Cab
 from .batch import Batch
 from .step import Step
 from stimela import task_stats 
+from stimela.backends import StimelaBackendSchema
 
 
 class DeferredAlias(Unresolved):
     """Class used as placeholder for deferred alias lookup (i.e. before an aliased value is available)"""
     pass
 
 
@@ -61,29 +63,40 @@
     assign: Dict[str, Any] = EmptyDictDefault()     # assigns variables
 
     assign_based_on: Dict[str, Any] = EmptyDictDefault()
                                                     # assigns variables based on values of other variables
 
     aliases: Dict[str, Any] = EmptyDictDefault()
 
+    # overrides backend options
+    backend: Optional[Dict[str, Any]] = None
+
     # make recipe a for_loop-gather (i.e. parallel for loop)
     for_loop: Optional[ForLoopClause] = None
 
     # logging control, overrides opts.log.init_logname and opts.log.logname 
     init_logname: Optional[str] = None
     logname: Optional[str] = None
     batch: Optional[Batch] = None
+
+    #
     
     # # if not None, do a while loop with the conditional
     # _while: Conditional = None
     # # if not None, do an until loop with the conditional
     # _until: Conditional = None
 
     def __post_init__ (self):
         Cargo.__post_init__(self)
+        # check backend setting
+        if self.backend:
+            try:
+                OmegaConf.merge(StimelaBackendSchema, self.backend)
+            except OmegaConfBaseException as exc:
+                raise RecipeValidationError(f"recipe '{self.name}': invalid backend setting", exc)
         # flatten aliases and assignments
         self.aliases = self.flatten_param_dict(OrderedDict(), self.aliases)
         # check that schemas are valid
         for io in self.inputs, self.outputs:
             for name, schema in io.items():
                 if not schema:
                     raise RecipeValidationError(f"recipe '{self.name}': '{name}' does not define a valid schema")
@@ -588,18 +601,20 @@
             # the original schema forces a required value
             if schema.required and not have_step_param and (orig_schema is None or orig_schema.required is None):
                 alias_schema.required = True
 
             self._alias_map[step_label, step_param_name] = alias_name, orig_schema
             self._alias_list.setdefault(alias_name, []).append(Recipe.AliasInfo(step_label, step, step_param_name, io))
 
-    def finalize(self, config=None, log=None, name=None, fqname=None, nesting=0):
+    def finalize(self, config=None, log=None, name=None, fqname=None, backend=None, nesting=0):
         if not self.finalized:
             config = config or stimela.CONFIG
 
+            backend = OmegaConf.merge(backend or config.opts.backend, self.backend or {})
+
             # fully qualified name, i.e. recipe_name.step_name.step_name etc.
             self.fqname = fqname = fqname or self.fqname or self.name
 
             # if logger is not provided, then init one
             if log is None:
                 log = stimela.logger().getChild(self.fqname)
                 log.propagate = True
@@ -615,15 +630,15 @@
             super().finalize(config, log=log, fqname=fqname, nesting=nesting)
 
             # finalize steps
             for label, step in self.steps.items():
                 step_log = log.getChild(label)
                 step_log.propagate = False
                 try:
-                    step.finalize(config, log=step_log, fqname=f"{fqname}.{label}", nesting=nesting+1)
+                    step.finalize(config, log=step_log, fqname=f"{fqname}.{label}", backend=backend, nesting=nesting+1)
                     # check that per-step assignments don't clash with i/o parameters
                     step.assign = self.flatten_param_dict(OrderedDict(), step.assign)
                     self.validate_assignments(step.assign, step.assign_based_on, f"{fqname}.{label}")
                 except Exception as exc:
                     raise StepValidationError(f"error validating step '{label}'", exc, 
                                 tb=not isinstance(exc, ScabhaBaseException))
 
@@ -971,15 +986,15 @@
     #         elif i == N-1:
     #             step.next_step = None
     #             step.previous_step = steps[i-2]
 
     def summary(self, params: Dict[str, Any], recursive=True, ignore_missing=False):
         """Returns list of lines with a summary of the recipe state
         """
-        lines = [f"recipe '{self.name}':"] + [f"  {name} = {value}" for name, value in params.items()]
+        lines = [f"recipe '{self.name}':"] + Cargo.add_parameter_summary(params)
         if not ignore_missing:
             lines += [f"  {name} = ???" for name in self.inputs_outputs if name not in params]
         if recursive:
             lines.append("  steps:")
             for name, step in self.steps.items():
                 stepsum = step.summary()
                 lines.append(f"    {name}: {stepsum[0]}")
@@ -1020,15 +1035,15 @@
             value (Any): value
         """
         for alias in self._alias_list.get(name, []):
             if alias.from_recipe:
                 alias.step.update_parameter(alias.param, value)
 
 
-    def _iterate_loop_worker(self, params, info, subst, count, iter_var, raise_exc=True):
+    def _iterate_loop_worker(self, params, info, subst, backend, count, iter_var, raise_exc=True):
         """"
         Needed for concurrency
         """
         outputs = {}
         exception = tb = None
         try:
             # if for-loop, assign new value
@@ -1075,15 +1090,15 @@
                     self.log.debug(f"step '{label}' will be explicitly skipped")
                 else:
                     self.log.info(f"processing step '{label}'")
                     if step.info:
                         self.log.info(f"  ({step.info})", extra=dict(color="GREEN", boldface=True))
                 try:
                     #step_params = step.run(subst=subst.copy(), batch=batch)  # make a copy of the subst dict since recipe might modify
-                    step_params = step.run(subst=subst.copy(), parent_log=self.log)  # make a copy of the subst dict since recipe might modify
+                    step_params = step.run(backend=backend, subst=subst.copy(), parent_log=self.log)  # make a copy of the subst dict since recipe might modify
                 except ScabhaBaseException as exc:
                     newexc = StimelaStepExecutionError(f"step '{step.fqname}' has failed, aborting the recipe", exc)
                     if not exc.logged:
                         log_exception(newexc, log=step.log)
                     raise newexc
 
                 # put step parameters into previous and steps[label] again, as they may have changed based on outputs)
@@ -1109,29 +1124,31 @@
                 raise
             # else will be returned
             exception = exc
             tb = FormattedTraceback(sys.exc_info()[2])
 
         return task_stats.collect_stats(), outputs, exception, tb
 
-    def _run(self, params, subst=None) -> Dict[str, Any]:
+    def _run(self, params, subst=None, backend={}) -> Dict[str, Any]:
         """Internal recipe run method. Meant to be called from a wrapper Step object (which validates the parameters, etc.)
 
         Parameters
         ----------
 
         Returns
         -------
         Dict[str, Any]
             Dictionary of formal outputs
 
         Raises
         ------
         RecipeValidationError
         """
+        # set up backend
+        backend = OmegaConf.merge(backend, self.backend or {})
 
         # set up substitution namespace
         subst_outer = subst
         if subst is None:
             subst = SubstitutionNS()
 
         info = SubstitutionNS(fqname=self.fqname, label='', label_parts=[], suffix='')
@@ -1176,15 +1193,15 @@
                     self._update_aliases(name, value)
                 elif schema.required and (self.for_loop is None or name != self.for_loop.var): 
                         raise RecipeValidationError(f"recipe '{self.name}' is missing required input '{name}'", log=self.log)
 
             # form list of arguments for each invocation of the loop worker
             loop_worker_args = []
             for count, iter_var in enumerate(self._for_loop_values):
-                loop_worker_args.append((params, info, subst, count, iter_var))
+                loop_worker_args.append((params, info, subst, backend, count, iter_var))
 
             # if scatter is enabled, use a process pool
             if self._for_loop_scatter:
                 num_workers = self._for_loop_scatter if self._for_loop_scatter > 0 else len(loop_worker_args)
                 with ProcessPoolExecutor(num_workers) as pool:
                     # submit each iterant to pool
                     futures = [pool.submit(self._iterate_loop_worker, *args, raise_exc=False) for args in loop_worker_args]
@@ -1211,18 +1228,14 @@
             
             # either way, outputs contains output aliases from the last iteration
             params.update(**outputs)
 
             # current namespace becomes recipe again
             subst.current = subst.recipe
             
-            # # evaluate implicit outputs
-            # implicits = {name: schema.implcit for name, schema in self.outputs if schema.implicit}
-            # params.update(**evaluate_and_substitute(implicits, subst, subst.current, location=self.fqname))
-
             self.log.info(f"recipe '{self.name}' executed successfully")
             return OrderedDict((name, value) for name, value in params.items() if name in self.outputs)
         finally:
             steps = subst.steps
             subst.update(subst_copy)
             subst.current.steps = steps
```

### Comparing `stimela-2.0rc4/stimela/kitchen/step.py` & `stimela-2.0rc6/stimela/kitchen/step.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from typing import Any, Tuple, List, Dict, Optional, Union
 from dataclasses import dataclass
 from omegaconf import MISSING, OmegaConf, DictConfig, ListConfig
 from omegaconf.errors import OmegaConfBaseException
 from collections import OrderedDict
 from contextlib import nullcontext
 
-from stimela import config
 from stimela.config import EmptyDictDefault, EmptyListDefault
 import stimela
 from stimela import log_exception, stimelogging
+from stimela.backends import StimelaBackendSchema, runner
 from stimela.exceptions import *
 import scabha.exceptions
 from scabha.exceptions import SubstitutionError, SubstitutionErrorList
 from scabha.validate import evaluate_and_substitute, Unresolved, join_quote
 from scabha.substitutions import SubstitutionNS, substitutions_from 
 from scabha.basetypes import UNSET, Placeholder, MS, File, Directory, SkippedOutput
 from .cab import Cab, get_cab_schema
@@ -52,38 +52,40 @@
     cab: Optional[Any] = None                       # if not None, this step is a cab and this is the cab name
     recipe: Optional[Any] = None                    # if not None, this step is a nested recipe
     params: Dict[str, Any] = EmptyDictDefault()     # assigns parameter values
     info: Optional[str] = None                      # comment or info
     skip: Optional[str] = None                      # if this evaluates to True, step is skipped.  
     skip_if_outputs: Optional[str] = None           # skip if outputs "exist' or "fresh"
     tags: List[str] = EmptyListDefault()
-    backend: Optional["stimela.config.Backend"] = None                   # backend setting, overrides opts.config.backend if set
 
     name: str = ''                                  # step's internal name
     fqname: str = ''                                # fully-qualified name e.g. recipe_name.step_label
 
     assign: Dict[str, Any] = EmptyDictDefault()     # assigns recipe-level variables when step is executed
 
     assign_based_on: Dict[str, Any] = EmptyDictDefault()
                                                     # assigns recipe-level variables when step is executed based on value of another variable
 
-    # runtime settings
-    runtime: Dict[str, Any] = EmptyDictDefault()
-
-    # _skip: Conditional = None                       # skip this step if conditional evaluates to true
-    # _break_on: Conditional = None                   # break out (of parent recipe) if conditional evaluates to true
+    # optional backend settings
+    backend: Optional[Dict[str, Any]] = None
 
     def __post_init__(self):
         self.fqname = self.fqname or self.name
         if not bool(self.cab) and not bool(self.recipe):
             raise StepValidationError(f"step '{self.name}': step must specify either a cab or a nested recipe")
         if bool(self.cab) == bool(self.recipe):
             raise StepValidationError(f"step '{self.name}': step can't specify both a cab and a nested recipe")
         self.cargo = self.config = None
         self.tags = set(self.tags)
+        # check backend setting
+        if self.backend:
+            try:
+                OmegaConf.merge(StimelaBackendSchema, self.backend)
+            except OmegaConfBaseException as exc:
+                raise StepValidationError(f"step '{self.name}': invalid backend setting", exc)
         # convert params into standard dict, else lousy stuff happens when we insert non-standard objects
         if isinstance(self.params, DictConfig):
             self.params = OmegaConf.to_container(self.params)
         # after (pre)validation, this contains parameter values
         self.validated_params = None
         # parameters protected from assignment (because they've been set on the command line, presumably)
         self._assignment_overrides = set()
@@ -169,15 +171,15 @@
                 raise AssignmentError(f"invalid {self.fqname}.log.{setting} setting", exc)
         # propagate to children
         if isinstance(self.cargo, Recipe):
             self.cargo.update_log_options(**options)
 
     _instantiated_cabs = {}
 
-    def finalize(self, config=None, log=None, fqname=None, nesting=0):
+    def finalize(self, config=None, log=None, fqname=None, backend=None, nesting=0):
         from .recipe import Recipe, RecipeSchema
         if not self.finalized:
             if fqname is not None:
                 self.fqname = fqname
             self.config = config = config or stimela.CONFIG
 
             # if recipe, validate the recipe with our parameters
@@ -237,43 +239,29 @@
 
             # if logger is not provided, then init one
             if log is None:
                 log = stimela.logger().getChild(self.fqname)
                 log.propagate = False
 
             # finalize the cargo
-            self.cargo.finalize(config, log=log, fqname=self.fqname, nesting=nesting)
+            self.cargo.finalize(config, log=log, fqname=self.fqname, backend=backend, nesting=nesting)
 
             # build dictionary of defaults from cargo
             self.defaults = {name: schema.default for name, schema in self.cargo.inputs_outputs.items() 
                              if schema.default is not UNSET and not isinstance(schema.default, Unresolved) }
             self.defaults.update(**self.cargo.defaults)
             
             # set missing parameters from defaults
             for name, value in self.defaults.items():
                 if name not in self.params:
                     self.params[name] = value
 
             # check for valid backend
-            if type(self.cargo) is Cab:
-                if self.backend is not None:
-                    self._backend = self.backend
-                    if self._backend.name not in stimela.config.AVAILABLE_BACKENDS:
-                        status = stimela.config.get_backend_status(self._backend.name)
-                        raise StepValidationError(f"backend '{self._backend.name}' is not available ({status})")
-                elif self.cargo.backend is not None:
-                    self._backend = self.cargo.backend
-                    if self._backend.name not in stimela.config.AVAILABLE_BACKENDS:
-                        status = stimela.config.get_backend_status(self._backend.name)
-                        raise StepValidationError(f"backend '{self._backend.name}' specified by cab is not available ({status})")
-                # no need to check this, it's checked at startup
-                else:
-                    self._backend =  stimela.CONFIG.opts.backend
-            else:
-                self._backend = None
+            runner.validate_backend_settings(OmegaConf.merge(backend or {}, self.cargo.backend or {}, self.backend or {}))
+
 
     def prevalidate(self, subst: Optional[SubstitutionNS]=None, root=False):
         self.finalize()
         # validate cab or recipe
         params = self.validated_params = self.cargo.prevalidate(self.params, subst, root=root)
         # add missing outputs
         for name in self.cargo.outputs:
@@ -314,20 +302,23 @@
         if key in self.inputs_outputs:
             self.params[key] = value
             # and remove from prevalidated params
             if self.validated_params and key in self.validated_params:
                 del self.validated_params[key]
         # else delegate to cargo to assign
         else:
-            self.cargo.assign_value(key, value, override=override, subst=subst)
+            try:
+                self.cargo.assign_value(key, value, override=override)
+            except ScabhaBaseException as exc:
+                raise AssignmentError(f"{self.name}: invalid assignment {key}={value}", exc)
 
-    def run(self, subst=None, batch=None, parent_log=None):
+
+    def run(self, backend={}, subst=None, parent_log=None):
         """Runs the step"""
         from .recipe import Recipe
-        from . import runners
 
         # some messages go to the parent logger -- if not defined, default to our own logger
         if parent_log is None:
             parent_log = self.log
 
         # if step is being explicitly skipped, omit from profiling, and drop info/warning messages to debug level
         explicit_skip = self.skip is True 
@@ -410,75 +401,121 @@
                     parent_log_warning(f"invalid inputs: {join_quote(invalid)}")
                     if not skip_warned:
                         parent_log_warning("since the step was skipped, this is not fatal")
                         skip_warned = True
                 else:
                     raise StepValidationError(f"step '{self.name}': invalid inputs: {join_quote(invalid)}", log=self.log)
 
-            ## check if we need to skip based on existing file outputs
-            if self.skip_if_outputs:
+            ## check if we need to skip based on existing/fresh file outputs
+            ## if skip on fresh outputs is in effect, find mtime of most recent input 
+            if not skip and self.skip_if_outputs:
+                # max_mtime will remain 0 if we're not echecking for freshness, or if there are no file-type inputs
                 max_mtime, max_mtime_path = 0, None
                 if self.skip_if_outputs == OUTPUTS_FRESH:
                     parent_log_info("checking if file-type outputs of step are fresh")
                     for name, value in params.items():
                         schema = self.inputs_outputs[name]
-                        if schema.is_input and schema.is_file_type and type(value) is str and os.path.exists(value):
-                            mtime = os.path.getmtime(value)
-                            if mtime > max_mtime:
-                                max_mtime = mtime
-                                max_mtime_path = value
+                        if schema.is_input and not schema.skip_freshness_checks:
+                            if schema.is_file_type:
+                                values = [value]
+                            elif schema.is_file_list_type:
+                                values = value
+                            else:
+                                continue
+                            for filename in values:
+                                if type(filename) is str and os.path.exists(filename):
+                                    mtime = os.path.getmtime(filename)
+                                    if mtime > max_mtime:
+                                        max_mtime = mtime
+                                        max_mtime_path = filename
                     if max_mtime:
                         parent_log_info(f"  most recently modified input is {max_mtime_path} ({time.ctime(max_mtime)})")
                 else:
                     parent_log_info("checking if file-type outputs of step exist")
 
+                ## now go through outputs -- all_exist flag will be cleared if we find one that doesn't exist,
+                ## or is older than an input
                 all_exist = True
-                for name, value in params.items():
-                    schema = self.inputs_outputs[name]
-                    if schema.is_output and schema.is_file_type:
-                        if os.path.exists(value):
-                            if max_mtime:
-                                mtime = os.path.getmtime(value)
-                                if mtime < max_mtime:
-                                    parent_log_info(f"  {name} = {value} is not fresh")
+                for name, schema in self.outputs.items():
+                    # ignore outputs not in params (implicit outputs will be already in there thanks to validation above)
+                    if name in params:
+                        # check for files or lists of files, and skip otherwise
+                        if schema.is_file_type:
+                            filenames = [params[name]]
+                        elif schema.is_file_list_type:
+                            filenames = params[name]
+                            # empty list of files treated as non-existing output
+                            if not filenames:
+                                if schema.must_exist:
                                     all_exist = False
-                                    break
+                                    parent_log_info(f"  {name}: no existing file(s)")
+                                    break  # abort the check
                                 else:
-                                    parent_log_info(f"  {name} = {value} is fresh")
-                            else:
-                                parent_log_info(f"  {name} = {value} already exists")
+                                    parent_log_info(f"  {name}: no existing file(s), but they are not required")
+                                    continue
                         else:
-                            all_exist = False
-                            parent_log_info(f"  {name} = {value} doesn't exist")
+                            continue # go on to next parameter
+                        # collect messages rather than logging them directly, to avoid log diarrhea for long file lists
+                        messages = []
+                        # ok, we have a list of files to check
+                        for num, value in enumerate(filenames):
+                            if type(value) is not str:  # skip funny values that aren't strings
+                                continue
+                            # form up label for messages
+                            label = f"{name}[{num}]" if schema.is_file_list_type else name
+                            if os.path.exists(value):
+                                # max_mtime==0 means we're only checking for existence, not freshness
+                                if max_mtime:
+                                    if schema.skip_freshness_checks:
+                                        messages.append(f"{label} = {value} marked as skipped from freshness checks")
+                                    else:
+                                        mtime = os.path.getmtime(value)
+                                        if mtime < max_mtime:
+                                            parent_log_info(f"{label} = {value} is not fresh")
+                                            all_exist = False
+                                            break
+                                        else:
+                                            messages.append(f"{label} = {value} is fresh")
+                                else:
+                                    messages.append(f"{label} = {value} exists")
+                            elif schema.must_exist is not False:
+                                all_exist = False
+                                parent_log_info(f"  {label} = {value} doesn't exist")
+                                break
+                            else:
+                                messages.append(f"{label} = {value} doesn't exist, but is not required to")
+                        # abort the checks if we encountered a fail
+                        if not all_exist:
                             break
+                        # else log the collected messages
+                        if len(messages) > 2:
+                            messages = [messages[0], "  ...", messages[-1]]
+                        for msg in messages:
+                            parent_log_info(f"  {msg}")
                 if all_exist:
                     parent_log_info("all required outputs are OK, skipping this step")
                     skip = True
 
             if not skip:
                 # check for outputs that need removal
                 for name, schema in self.outputs.items():
                     if name in params and schema.remove_if_exists and schema.is_file_type:
                         path = params[name]
-                        if os.path.exists(path):
+                        if type(path) is str and os.path.exists(path):
                             if os.path.isdir(path) and not os.path.islink(path):
                                 shutil.rmtree(path)
                             else:
                                 os.unlink(path)
 
                 if type(self.cargo) is Recipe:
-                    self.cargo._run(params, subst)
+                    backend = OmegaConf.merge(backend, self.cargo.backend or {}, self.backend or {})
+                    self.cargo._run(params, subst, backend=backend)
                 elif type(self.cargo) is Cab:
-                    if self.backend is not None:
-                        backend = self.backend
-                    elif self.cargo.backend is not None:
-                        backend = self.cargo.backend
-                    else:
-                        backend =  stimela.CONFIG.opts.backend
-                    cabstat = runners.run_cab(self, params, backend=backend, subst=subst, batch=batch)
+                    backend = OmegaConf.merge(backend, self.cargo.backend or {}, self.backend or {})
+                    cabstat = runner.run_cab(self, params, backend=backend, subst=subst)
                     # check for runstate
                     if cabstat.success is False:
                         raise StimelaCabRuntimeError(f"error running cab '{self.cargo.name}'", cabstat.errors)
                     for msg in cabstat.warnings:
                         self.log.warning(f"cab '{self.cargo.name}': {msg}")
                     params.update(**cabstat.outputs)
                 else:
```

### Comparing `stimela-2.0rc4/stimela/kitchen/wranglers.py` & `stimela-2.0rc6/stimela/kitchen/wranglers.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,16 @@
         """
         raise RuntimeError("derived class does not implement an apply() method")
 
 class Replace(_BaseWrangler):
     """
     This wrangler will replace the matching pattern with the given string. Specified as REPLACE:replacement.
     Uses re.sub() internally, so look that up for more complex usage.
-    """
+    """ 
+
     specifier = "REPLACE:(?P<replace>.*)"
     
     def apply(self, cabstat: CabStatus, output: str, match: re.Match):
         return self.regex.sub(self.replace, output), None
 
 class Highlight(_BaseWrangler):
     """
```

### Comparing `stimela-2.0rc4/stimela/main.py` & `stimela-2.0rc6/stimela/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import glob
 import sys
 import click
 import datetime
 from dataclasses import dataclass
 from omegaconf import OmegaConf
 import stimela
-from stimela import config, stimelogging
+from stimela import config, stimelogging, backends
 
 UID = stimela.UID
 GID = stimela.GID
 LOG_HOME = stimela.LOG_HOME
 LOG_FILE = stimela.LOG_FILE
 
 log = None
@@ -36,29 +36,29 @@
     def resolve_command(self, ctx, args):
         # always return the full command name
         _, cmd, args = super().resolve_command(ctx, args)
         return cmd.name, cmd, args
 
 
 @click.group(cls=RunExecGroup)
-@click.option('--backend', '-b', type=click.Choice(config.Backend._member_names_), 
-                help="Backend to use (for containerization).")
+@click.option('--backend', '-b', type=click.Choice(backends.SUPPORTED_BACKENDS), 
+                 help="Backend to use (for containerization).")
 @click.option('--config', '-c', 'config_files', metavar='FILE', multiple=True,
                 help="Extra user-defined config file(s) to load.")
 @click.option('--set', '-s', 'config_dotlist', metavar='SECTION.VAR=VALUE', multiple=True,
                 help="Extra user-defined config settings to apply.")
 @click.option('--no-sys-config', is_flag=True, 
                 help="Do not load standard config files.")
 @click.option('-I', '--include', metavar="DIR", multiple=True, 
                 help="Add directory to _include paths. Can be given multiple times.")
 @click.option('--clear-cache', '-C', is_flag=True, 
                 help="Reset the configuration cache. First thing to try in case of strange configuration errors.")
 @click.option('--verbose', '-v', is_flag=True, help='Be extra verbose in output.')
 @click.version_option(str(stimela.__version__))
-def cli(backend, config_files=[], config_dotlist=[], include=[], verbose=False, no_sys_config=False, clear_cache=False):
+def cli(config_files=[], config_dotlist=[], include=[], backend=None, verbose=False, no_sys_config=False, clear_cache=False):
     global log
     log = stimela.logger(loglevel=logging.DEBUG if verbose else logging.INFO)
     log.info(f"starting")        # remove this eventually, but it's handy for timing things right now
 
     stimela.VERBOSE = verbose
     if verbose:
         log.debug("verbose output enabled")
@@ -81,48 +81,46 @@
     if stimela.CONFIG is None:
         log.error("failed to load configuration, exiting")
         sys.exit(1)
 
     if config.CONFIG_LOADED:
         log.info(f"loaded config from {config.CONFIG_LOADED}") 
 
+    # select backend
+    if backend:
+        if backends.get_backend(backend) is None:
+            log.error(f"backend '{backend}' not available: {backends.get_backend_status(backend)}")
+            sys.exit(1)
+
+        stimela.CONFIG.opts.backend.select = [backend]
+
     # enable logfiles and such
     if stimela.CONFIG.opts.log.enable:
         if verbose:
             stimela.CONFIG.opts.log.level = "DEBUG"
         # setup file logging
         subst = OmegaConf.create(dict(
                     info=OmegaConf.create(dict(fqname='stimela')), 
                     config=stimela.CONFIG))
         stimelogging.update_file_logger(log, stimela.CONFIG.opts.log, nesting=-1, subst=subst)
 
-
-    # print backends
-    log.info(f"available backends: {' '.join(config.AVAILABLE_BACKENDS)}")
-
-    # get default backend module
-    global BACKEND 
-    if backend:
-        stimela.CONFIG.opts.backend = backend
-
-    if stimela.CONFIG.opts.backend.name not in config.AVAILABLE_BACKENDS:
-        status = config.get_backend_status(stimela.CONFIG.opts.backend.name)
-        log.error(f"the backend '{stimela.CONFIG.opts.backend.name}' is not available: {status}")
-        sys.exit(1)
-
-    log.info(f"default backend is {stimela.CONFIG.opts.backend.name}")
-
     # report dependencies
     for filename, attrs in config.CONFIG_DEPS.get_description().items():
         log.debug(f"config dependency {', '.join([filename] + attrs)}")
 
     # dump dependencies
     filename = os.path.join(stimelogging.get_logfile_dir(log) or '.', "stimela.config.deps")
     log.info(f"saving config dependencies to {filename}")
     config.CONFIG_DEPS.save(filename)
 
 
 # import commands
-from stimela.commands import doc, run, images, build, push, save_config
+from stimela.commands import doc, run, save_config
+
+## These one needs to be reimplemented, current backed auto-pulls and auto-builds:
+# images, pull, build, clean
+
+## this one is deprecated, stimela doc does the trick
+# cabs
 
-## the ones not listed above haven't been converted to click yet. They are:
-# cabs, clean, containers, kill, ps, pull
+## the ones below should be deprecated, since we don't do async containers anymore
+# containers, kill, ps
```

### Comparing `stimela-2.0rc4/stimela/schedulers/slurm.py` & `stimela-2.0rc6/stimela/schedulers/slurm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import shlex
 from typing import Dict, Optional, Any 
-from stimela.kitchen.cab import Cab
 from stimela.kitchen.batch import Batch
 from stimela import logger
 from stimela.utils.xrun_poll import xrun
 from stimela.exceptions import StimelaCabRuntimeError
 import subprocess
```

### Comparing `stimela-2.0rc4/stimela/stimelogging.py` & `stimela-2.0rc6/stimela/stimelogging.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/stimela/task_stats.py` & `stimela-2.0rc6/stimela/task_stats.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/stimela/utils/xrun_asyncio.py` & `stimela-2.0rc6/stimela/utils/xrun_asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,15 @@
             """Returns string representing elapsed time"""
             return str(datetime.datetime.now() - start_time).split('.', 1)[0]
         
         loop = asyncio.get_event_loop()
         
         proc = loop.run_until_complete(
                 asyncio.create_subprocess_exec(*command,
+                    limit=1024**3,
                     stdout=asyncio.subprocess.PIPE,
                     stderr=asyncio.subprocess.PIPE))
 
         async def stream_reader(stream, stream_name):
             while not stream.at_eof():
                 line = await stream.readline()
                 line = (line.decode('utf-8') if type(line) is bytes else line).rstrip()
```

### Comparing `stimela-2.0rc4/stimela/utils/xrun_poll.py` & `stimela-2.0rc6/stimela/utils/xrun_poll.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/tests/scabha_tests/test_configuratt.py` & `stimela-2.0rc6/tests/scabha_tests/test_configuratt.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/tests/scabha_tests/test_dynschema.py` & `stimela-2.0rc6/tests/scabha_tests/test_dynschema.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/tests/scabha_tests/test_parsing.py` & `stimela-2.0rc6/tests/scabha_tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/tests/scabha_tests/test_schema.py` & `stimela-2.0rc6/tests/scabha_tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/tests/scabha_tests/test_substitutions.py` & `stimela-2.0rc6/tests/scabha_tests/test_substitutions.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/tests/scabha_tests/testconf.yaml` & `stimela-2.0rc6/tests/scabha_tests/testconf.yaml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/tests/stimela_tests/example_dynschema.py` & `stimela-2.0rc6/tests/stimela_tests/example_dynschema.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/tests/stimela_tests/test_aliasing.yml` & `stimela-2.0rc6/tests/stimela_tests/test_aliasing.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/tests/stimela_tests/test_callables.py` & `stimela-2.0rc6/tests/stimela_tests/test_callables.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/tests/stimela_tests/test_callables.yml` & `stimela-2.0rc6/tests/stimela_tests/test_callables.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/tests/stimela_tests/test_kube.yml` & `stimela-2.0rc6/tests/stimela_tests/test_kube.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/tests/stimela_tests/test_loop_recipe.yml` & `stimela-2.0rc6/tests/stimela_tests/test_loop_recipe.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/tests/stimela_tests/test_loop_recipe_slurm.yml` & `stimela-2.0rc6/tests/stimela_tests/test_loop_recipe_slurm.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/tests/stimela_tests/test_nesting.yml` & `stimela-2.0rc6/tests/stimela_tests/test_nesting.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/tests/stimela_tests/test_recipe.py` & `stimela-2.0rc6/tests/stimela_tests/test_recipe.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/tests/stimela_tests/test_recipe.yml` & `stimela-2.0rc6/tests/stimela_tests/test_recipe.yml`

 * *Files 6% similar despite different names*

```diff
@@ -2,34 +2,27 @@
   simms:
     image: null
     command: echo 
     policies:
       skip_implicits: True
     # simms
     inputs:
-      msname:
-        dtype: str
-        required: true
-      tel:
-        dtype: str
-      dtime:
-        dtype: int
-      synthesis:
-        dtype: float
+      msname: str * "* marks required value"
+      tel: str
+      dtime: int
+      synthesis: float
     outputs:
       ms:
         dtype: MS
         implicit: "{current.msname}"
         must_exist: false
         
   cubical:
     command: echo
     # gocubical
-    virtual_env: 
-    # ~/.venv/cc
     inputs:
       ms:
         dtype: MS
         required: true
         writable: true
         nom_de_guerre: data-ms
         must_exist: false   # for testing
@@ -43,19 +36,31 @@
   wsclean:
     image: null
     command: echo
     policies:
       skip_implicits: True
     inputs:
       ms:
+        dtype: MS
         must_exist: false  # for testing
+      prefix:
+        dtype: str
+      scale:
+        dtype: str
+      size:
+        dtype: int
       dummy:
         dtype: str
       dummy2:
         dtype: str
+    outputs:
+      restored:
+        implicit: "foo"
+      dirty:
+        implicit: "foo"
 
   aimfast:
     command: /bin/true ## dummy command for now, since this is just a dummy example step
     inputs:
       image:
         dtype: str
         required: true
```

### Comparing `stimela-2.0rc4/tests/stimela_tests/test_scatter.yml` & `stimela-2.0rc6/tests/stimela_tests/test_scatter.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/tests/stimela_tests/test_wranglers.py` & `stimela-2.0rc6/tests/stimela_tests/test_wranglers.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/tests/stimela_tests/test_wranglers.yml` & `stimela-2.0rc6/tests/stimela_tests/test_wranglers.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/tests/stimela_tests/test_xrun.yml` & `stimela-2.0rc6/tests/stimela_tests/test_xrun.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc4/PKG-INFO` & `stimela-2.0rc6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stimela
-Version: 2.0rc4
+Version: 2.0rc6
 Summary: Framework for system agnostic pipelines for radio interferometry arrays
 License: GNU GPL v2
 Author: Sphesihle Makhathini
 Author-email: sphemakh@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

