# Comparing `tmp/cosmosis-3.0.tar.gz` & `tmp/cosmosis-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmosis-3.0.tar", last modified: Thu Jul 27 14:15:44 2023, max compression
+gzip compressed data, was "cosmosis-3.0.1.tar", last modified: Fri Jul 28 09:33:18 2023, max compression
```

## Comparing `cosmosis-3.0.tar` & `cosmosis-3.0.1.tar`

### file list

```diff
@@ -1,290 +1,290 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.823149 cosmosis-3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-27 14:15:42.000000 cosmosis-3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-07-27 14:15:42.000000 cosmosis-3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-27 14:15:44.823149 cosmosis-3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-27 14:15:42.000000 cosmosis-3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.799148 cosmosis-3.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      102 2023-07-27 14:15:42.000000 cosmosis-3.0/bin/cosmosis
--rwxr-xr-x   0 runner    (1001) docker     (123)      122 2023-07-27 14:15:42.000000 cosmosis-3.0/bin/cosmosis-campaign
--rwxr-xr-x   0 runner    (1001) docker     (123)      792 2023-07-27 14:15:42.000000 cosmosis-3.0/bin/cosmosis-configure
--rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-07-27 14:15:42.000000 cosmosis-3.0/bin/cosmosis-extract
--rwxr-xr-x   0 runner    (1001) docker     (123)      102 2023-07-27 14:15:42.000000 cosmosis-3.0/bin/cosmosis-postprocess
--rwxr-xr-x   0 runner    (1001) docker     (123)     1527 2023-07-27 14:15:42.000000 cosmosis-3.0/bin/cosmosis-sample-fisher
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.803148 cosmosis-3.0/cosmosis/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20918 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/campaign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.803148 cosmosis-3.0/cosmosis/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/config/compilers.mk
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/config/subdirs.mk
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.803148 cosmosis-3.0/cosmosis/datablock/
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51706 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/c_datablock.cc
--rw-r--r--   0 runner    (1001) docker     (123)    22811 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/c_datablock.h
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/clamp.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/cosmosis_constants.fh
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/cosmosis_constants.h
--rw-r--r--   0 runner    (1001) docker     (123)    34029 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/cosmosis_modules.F90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.807148 cosmosis-3.0/cosmosis/datablock/cosmosis_py/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/cosmosis_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52767 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/cosmosis_py/block.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/cosmosis_py/dbt_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/cosmosis_py/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/cosmosis_py/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/cosmosis_py/section_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/cosmosis_section_names.F90
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/cosmosis_types.F90
--rw-r--r--   0 runner    (1001) docker     (123)    28871 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/cosmosis_wrappers.F90
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/datablock.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11180 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/datablock.hh
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/datablock_logging.cc
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/datablock_logging.h
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/datablock_status.h
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/datablock_types.h
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/entry.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11879 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/entry.hh
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/exceptions.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/generate_sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/handler.c
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/ndarray.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/section.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/section.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/section_names.h
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/section_names.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/gaussian_likelihood.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22922 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/names.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.807148 cosmosis-3.0/cosmosis/output/
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/output/astropy_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/output/cosmomc_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/output/fits_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/output/in_memory_output.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/output/null_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/output/output_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/output/text_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/output/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.807148 cosmosis-3.0/cosmosis/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/plotting/chain_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/plotting/grid_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/plotting/kde.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      404 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/plotting/plot_demo_3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/plotting/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/plotting/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5362 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.807148 cosmosis-3.0/cosmosis/postprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocessing/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16175 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocessing/cosmology_theory_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocessing/density.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocessing/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocessing/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocessing/latex.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocessing/lazy_pylab.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocessing/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocessing/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    49133 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocessing/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocessing/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocessing/postprocess_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocessing/reruns.py
--rw-r--r--   0 runner    (1001) docker     (123)    31559 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocessing/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocessing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/attribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    13893 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/declare.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/runtime/julia_modules/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/julia_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/julia_modules/julia.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/memmon.py
--rw-r--r--   0 runner    (1001) docker     (123)    17198 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/mpi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    55629 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    21210 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/process_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/samplers/abc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/abc/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7126 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/abc/abc_sampler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6698 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/abc/abc_sampler_mpi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/samplers/apriori/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/apriori/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2176 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/apriori/apriori_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/samplers/dynesty/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/dynesty/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3722 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/dynesty/dynesty_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/samplers/emcee/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/emcee/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7452 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/emcee/emcee_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/samplers/fisher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/fisher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/fisher/fisher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6652 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/fisher/fisher_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/samplers/grid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/grid/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4683 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/grid/grid_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/samplers/gridmax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/gridmax/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4370 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/gridmax/gridmax_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/hints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/samplers/importance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/importance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/importance/importance_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/samplers/kombine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/kombine/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4932 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/kombine/kombine_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/samplers/list/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/list/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4888 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/list/list_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/samplers/maxlike/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/maxlike/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4578 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/maxlike/maxlike_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/samplers/metropolis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/metropolis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/metropolis/metropolis.py
--rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/metropolis/metropolis_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/samplers/metropolis/proposal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/metropolis/proposal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/metropolis/proposal/cobaya_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/metropolis/proposal/standard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.815148 cosmosis-3.0/cosmosis/samplers/minuit/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/minuit/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/minuit/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7325 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/minuit/minuit_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/minuit/minuit_wrapper.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.815148 cosmosis-3.0/cosmosis/samplers/multinest/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/multinest/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/multinest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/multinest/multinest_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.815148 cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    19512 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/README
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/cwrapper.f90
--rw-r--r--   0 runner    (1001) docker     (123)    42915 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90
--rw-r--r--   0 runner    (1001) docker     (123)   106166 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/nested.f90
--rw-r--r--   0 runner    (1001) docker     (123)    22010 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/posterior.f90
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/priors.f90
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/utils.f90
--rw-r--r--   0 runner    (1001) docker     (123)    28039 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/utils1.f90
--rw-r--r--   0 runner    (1001) docker     (123)    86938 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.815148 cosmosis-3.0/cosmosis/samplers/nautilus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/nautilus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/nautilus/nautilus_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.815148 cosmosis-3.0/cosmosis/samplers/pmaxlike/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/pmaxlike/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4151 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.815148 cosmosis-3.0/cosmosis/samplers/pmc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/pmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/pmc/pmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/pmc/pmc_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.815148 cosmosis-3.0/cosmosis/samplers/poco/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/poco/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3660 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/poco/poco_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.815148 cosmosis-3.0/cosmosis/samplers/polychord/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.819149 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/README
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/abort.F90
--rw-r--r--   0 runner    (1001) docker     (123)    18110 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/array_utils.f90
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/c_interface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/calculate.f90
--rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90
--rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/clustering.f90
--rw-r--r--   0 runner    (1001) docker     (123)    13421 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/feedback.f90
--rw-r--r--   0 runner    (1001) docker     (123)    26147 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/generate.F90
--rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/ini.f90
--rw-r--r--   0 runner    (1001) docker     (123)    20999 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/interfaces.F90
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/interfaces.h
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/interfaces.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    24257 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90
--rw-r--r--   0 runner    (1001) docker     (123)    20674 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/params.f90
--rw-r--r--   0 runner    (1001) docker     (123)    19675 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/priors.f90
--rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/random_utils.F90
--rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/read_write.f90
--rw-r--r--   0 runner    (1001) docker     (123)    47427 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/run_time_info.f90
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/settings.f90
--rw-r--r--   0 runner    (1001) docker     (123)    29353 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/utils.F90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.819149 cosmosis-3.0/cosmosis/samplers/pymc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/pymc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/pymc/pymc_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.819149 cosmosis-3.0/cosmosis/samplers/snake/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/snake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/snake/snake.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1987 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/snake/snake_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.819149 cosmosis-3.0/cosmosis/samplers/star/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/star/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4422 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/star/star_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.819149 cosmosis-3.0/cosmosis/samplers/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/test/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3221 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/test/test_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.819149 cosmosis-3.0/cosmosis/samplers/zeus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/zeus/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11469 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/zeus/zeus_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.823149 cosmosis-3.0/cosmosis/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/campaign.yml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/example-priors.ini
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/example-values.ini
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/example.ini
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/example_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/example_module2.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/example_module3.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/example_module4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.823149 cosmosis-3.0/cosmosis/test/libtest/
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/c_datablock_complex_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/c_datablock_double_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/c_datablock_int_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/c_datablock_test.c
--rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/cosmosis_test.F90
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/cosmosis_tests.supp
--rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/datablock_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/entry_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/ndarray_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/section_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    28088 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/test_c_datablock_scalars.h
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/test_c_datablock_scalars.template
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/test_campaign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/test_chaining.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/test_polychord.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/test_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/test_text_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.803148 cosmosis-3.0/cosmosis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-27 14:15:44.000000 cosmosis-3.0/cosmosis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-07-27 14:15:44.000000 cosmosis-3.0/cosmosis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:15:44.000000 cosmosis-3.0/cosmosis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-27 14:15:44.000000 cosmosis-3.0/cosmosis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 14:15:44.000000 cosmosis-3.0/cosmosis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-27 14:15:42.000000 cosmosis-3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 14:15:44.823149 cosmosis-3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-07-27 14:15:42.000000 cosmosis-3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.629813 cosmosis-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-28 09:33:17.000000 cosmosis-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-07-28 09:33:17.000000 cosmosis-3.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-28 09:33:18.629813 cosmosis-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-28 09:33:17.000000 cosmosis-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.605813 cosmosis-3.0.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      102 2023-07-28 09:33:17.000000 cosmosis-3.0.1/bin/cosmosis
+-rwxr-xr-x   0 runner    (1001) docker     (123)      122 2023-07-28 09:33:17.000000 cosmosis-3.0.1/bin/cosmosis-campaign
+-rwxr-xr-x   0 runner    (1001) docker     (123)      792 2023-07-28 09:33:17.000000 cosmosis-3.0.1/bin/cosmosis-configure
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-07-28 09:33:17.000000 cosmosis-3.0.1/bin/cosmosis-extract
+-rwxr-xr-x   0 runner    (1001) docker     (123)      102 2023-07-28 09:33:17.000000 cosmosis-3.0.1/bin/cosmosis-postprocess
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1527 2023-07-28 09:33:17.000000 cosmosis-3.0.1/bin/cosmosis-sample-fisher
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.609813 cosmosis-3.0.1/cosmosis/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20918 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/campaign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.609813 cosmosis-3.0.1/cosmosis/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/config/compilers.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/config/subdirs.mk
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.609813 cosmosis-3.0.1/cosmosis/datablock/
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51706 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/c_datablock.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    22811 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/c_datablock.h
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/clamp.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/cosmosis_constants.fh
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/cosmosis_constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34029 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/cosmosis_modules.F90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.613813 cosmosis-3.0.1/cosmosis/datablock/cosmosis_py/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/cosmosis_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52767 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/cosmosis_py/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/cosmosis_py/dbt_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/cosmosis_py/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/cosmosis_py/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/cosmosis_py/section_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/cosmosis_section_names.F90
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/cosmosis_types.F90
+-rw-r--r--   0 runner    (1001) docker     (123)    28871 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/cosmosis_wrappers.F90
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/datablock.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11180 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/datablock.hh
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/datablock_logging.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/datablock_logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/datablock_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/datablock_types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/entry.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11879 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/entry.hh
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/exceptions.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/generate_sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/handler.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/ndarray.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/section.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/section.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/section_names.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/section_names.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/gaussian_likelihood.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22922 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/names.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.613813 cosmosis-3.0.1/cosmosis/output/
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/output/astropy_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/output/cosmomc_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/output/fits_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/output/in_memory_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/output/null_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/output/output_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/output/text_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/output/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.613813 cosmosis-3.0.1/cosmosis/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/plotting/chain_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/plotting/grid_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/plotting/kde.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      404 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/plotting/plot_demo_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/plotting/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/plotting/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5392 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.613813 cosmosis-3.0.1/cosmosis/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocessing/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16175 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocessing/cosmology_theory_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocessing/density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocessing/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocessing/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocessing/latex.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocessing/lazy_pylab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocessing/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocessing/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49133 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocessing/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocessing/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocessing/postprocess_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocessing/reruns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31638 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocessing/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocessing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/attribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13893 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/declare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/runtime/julia_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/julia_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/julia_modules/julia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/memmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17198 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/mpi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55645 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21210 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/process_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/abc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/abc/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7126 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/abc/abc_sampler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6698 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/abc/abc_sampler_mpi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/apriori/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/apriori/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2176 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/apriori/apriori_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/dynesty/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/dynesty/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3722 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/dynesty/dynesty_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/emcee/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/emcee/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7452 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/emcee/emcee_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/fisher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/fisher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/fisher/fisher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6652 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/fisher/fisher_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/grid/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4683 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/grid/grid_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/gridmax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/gridmax/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4370 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/gridmax/gridmax_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/hints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/importance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/importance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/importance/importance_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/kombine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/kombine/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4932 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/kombine/kombine_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/list/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/list/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4888 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/list/list_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/maxlike/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/maxlike/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4578 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/maxlike/maxlike_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/metropolis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/metropolis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/metropolis/metropolis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/metropolis/metropolis_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/metropolis/proposal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/metropolis/proposal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/metropolis/proposal/cobaya_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/metropolis/proposal/standard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/minuit/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/minuit/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/minuit/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7325 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/minuit/minuit_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/minuit/minuit_wrapper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/multinest/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/multinest/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/multinest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.621813 cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    19512 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/README
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/cwrapper.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    42915 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90
+-rw-r--r--   0 runner    (1001) docker     (123)   107766 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/nested.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    22010 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/posterior.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/priors.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/utils.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    28039 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/utils1.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    86938 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.621813 cosmosis-3.0.1/cosmosis/samplers/nautilus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/nautilus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/nautilus/nautilus_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.621813 cosmosis-3.0.1/cosmosis/samplers/pmaxlike/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/pmaxlike/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4151 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.621813 cosmosis-3.0.1/cosmosis/samplers/pmc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/pmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/pmc/pmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/pmc/pmc_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.621813 cosmosis-3.0.1/cosmosis/samplers/poco/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/poco/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3660 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/poco/poco_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.621813 cosmosis-3.0.1/cosmosis/samplers/polychord/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.621813 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/README
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/abort.F90
+-rw-r--r--   0 runner    (1001) docker     (123)    18110 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/array_utils.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/c_interface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/calculate.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/clustering.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    13421 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/feedback.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    26147 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/generate.F90
+-rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/ini.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    20999 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/interfaces.F90
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/interfaces.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/interfaces.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24257 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90
+-rw-r--r--   0 runner    (1001) docker     (123)    20674 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/params.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    19675 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/priors.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/random_utils.F90
+-rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/read_write.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    47427 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/run_time_info.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/settings.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    29353 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/utils.F90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.625813 cosmosis-3.0.1/cosmosis/samplers/pymc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/pymc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/pymc/pymc_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.625813 cosmosis-3.0.1/cosmosis/samplers/snake/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/snake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/snake/snake.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1987 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/snake/snake_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.625813 cosmosis-3.0.1/cosmosis/samplers/star/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/star/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4422 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/star/star_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.625813 cosmosis-3.0.1/cosmosis/samplers/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/test/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3221 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/test/test_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.625813 cosmosis-3.0.1/cosmosis/samplers/zeus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/zeus/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11469 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/zeus/zeus_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.625813 cosmosis-3.0.1/cosmosis/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/campaign.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/example-priors.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/example-values.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/example.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/example_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/example_module2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/example_module3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/example_module4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.625813 cosmosis-3.0.1/cosmosis/test/libtest/
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/c_datablock_complex_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/c_datablock_double_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/c_datablock_int_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/c_datablock_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/cosmosis_test.F90
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/cosmosis_tests.supp
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/datablock_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/entry_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/ndarray_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/section_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    28088 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/test_c_datablock_scalars.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/test_c_datablock_scalars.template
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/test_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/test_chaining.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/test_polychord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/test_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/test_text_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.609813 cosmosis-3.0.1/cosmosis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-28 09:33:18.000000 cosmosis-3.0.1/cosmosis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-07-28 09:33:18.000000 cosmosis-3.0.1/cosmosis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 09:33:18.000000 cosmosis-3.0.1/cosmosis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-28 09:33:18.000000 cosmosis-3.0.1/cosmosis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-28 09:33:18.000000 cosmosis-3.0.1/cosmosis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 09:33:17.000000 cosmosis-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 09:33:18.629813 cosmosis-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-07-28 09:33:17.000000 cosmosis-3.0.1/setup.py
```

### Comparing `cosmosis-3.0/LICENSE` & `cosmosis-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/MANIFEST.in` & `cosmosis-3.0.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/bin/cosmosis-configure` & `cosmosis-3.0.1/bin/cosmosis-configure`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/bin/cosmosis-extract` & `cosmosis-3.0.1/bin/cosmosis-extract`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/bin/cosmosis-sample-fisher` & `cosmosis-3.0.1/bin/cosmosis-sample-fisher`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/__init__.py` & `cosmosis-3.0.1/cosmosis/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/campaign.py` & `cosmosis-3.0.1/cosmosis/campaign.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/config/compilers.mk` & `cosmosis-3.0.1/cosmosis/config/compilers.mk`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/configure.py` & `cosmosis-3.0.1/cosmosis/configure.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/constants.py` & `cosmosis-3.0.1/cosmosis/constants.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/datablock/Makefile` & `cosmosis-3.0.1/cosmosis/datablock/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/datablock/c_datablock.cc` & `cosmosis-3.0.1/cosmosis/datablock/c_datablock.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/datablock/c_datablock.h` & `cosmosis-3.0.1/cosmosis/datablock/c_datablock.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/datablock/clamp.hh` & `cosmosis-3.0.1/cosmosis/datablock/clamp.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/datablock/cosmosis_constants.fh` & `cosmosis-3.0.1/cosmosis/datablock/cosmosis_constants.fh`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/datablock/cosmosis_constants.h` & `cosmosis-3.0.1/cosmosis/datablock/cosmosis_constants.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/datablock/cosmosis_modules.F90` & `cosmosis-3.0.1/cosmosis/datablock/cosmosis_modules.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/datablock/cosmosis_py/block.py` & `cosmosis-3.0.1/cosmosis/datablock/cosmosis_py/block.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/datablock/cosmosis_py/errors.py` & `cosmosis-3.0.1/cosmosis/datablock/cosmosis_py/errors.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/datablock/cosmosis_py/lib.py` & `cosmosis-3.0.1/cosmosis/datablock/cosmosis_py/lib.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/datablock/cosmosis_py/section_names.py` & `cosmosis-3.0.1/cosmosis/datablock/cosmosis_py/section_names.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/datablock/cosmosis_section_names.F90` & `cosmosis-3.0.1/cosmosis/datablock/cosmosis_section_names.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/datablock/cosmosis_wrappers.F90` & `cosmosis-3.0.1/cosmosis/datablock/cosmosis_wrappers.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/datablock/datablock.cc` & `cosmosis-3.0.1/cosmosis/datablock/datablock.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/datablock/datablock.hh` & `cosmosis-3.0.1/cosmosis/datablock/datablock.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/datablock/datablock_logging.cc` & `cosmosis-3.0.1/cosmosis/datablock/datablock_logging.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/datablock/datablock_logging.h` & `cosmosis-3.0.1/cosmosis/datablock/datablock_logging.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/datablock/datablock_status.h` & `cosmosis-3.0.1/cosmosis/datablock/datablock_status.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/datablock/entry.cc` & `cosmosis-3.0.1/cosmosis/datablock/entry.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/datablock/entry.hh` & `cosmosis-3.0.1/cosmosis/datablock/entry.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/datablock/generate_sections.py` & `cosmosis-3.0.1/cosmosis/datablock/generate_sections.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/datablock/handler.c` & `cosmosis-3.0.1/cosmosis/datablock/handler.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/datablock/ndarray.hh` & `cosmosis-3.0.1/cosmosis/datablock/ndarray.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/datablock/section.cc` & `cosmosis-3.0.1/cosmosis/datablock/section.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/datablock/section.hh` & `cosmosis-3.0.1/cosmosis/datablock/section.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/datablock/section_names.h` & `cosmosis-3.0.1/cosmosis/datablock/section_names.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/datablock/section_names.txt` & `cosmosis-3.0.1/cosmosis/datablock/section_names.txt`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/gaussian_likelihood.py` & `cosmosis-3.0.1/cosmosis/gaussian_likelihood.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/main.py` & `cosmosis-3.0.1/cosmosis/main.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/output/__init__.py` & `cosmosis-3.0.1/cosmosis/output/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/output/astropy_output.py` & `cosmosis-3.0.1/cosmosis/output/astropy_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/output/cosmomc_output.py` & `cosmosis-3.0.1/cosmosis/output/cosmomc_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/output/fits_output.py` & `cosmosis-3.0.1/cosmosis/output/fits_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/output/in_memory_output.py` & `cosmosis-3.0.1/cosmosis/output/in_memory_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/output/null_output.py` & `cosmosis-3.0.1/cosmosis/output/null_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/output/output_base.py` & `cosmosis-3.0.1/cosmosis/output/output_base.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/output/text_output.py` & `cosmosis-3.0.1/cosmosis/output/text_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/output/utils.py` & `cosmosis-3.0.1/cosmosis/output/utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/plotting/chain_plots.py` & `cosmosis-3.0.1/cosmosis/plotting/chain_plots.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/plotting/grid_plots.py` & `cosmosis-3.0.1/cosmosis/plotting/grid_plots.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/plotting/kde.py` & `cosmosis-3.0.1/cosmosis/plotting/kde.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/plotting/plotter.py` & `cosmosis-3.0.1/cosmosis/plotting/plotter.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/postprocess.py` & `cosmosis-3.0.1/cosmosis/postprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,12 +56,14 @@
 	args = parser.parse_args(args)
 
 	for ini_filename in args.inifile:
 		if not os.path.exists(ini_filename):
 			raise ValueError("The file (or directory) {} does not exist.".format(ini_filename))
 
 	processor = run_cosmosis_postprocess(args.inifile, **vars(args))
-	#Save all the image files and close the text files
-	processor.save()
+
+	if processor is not None:
+		#Save all the image files and close the text files
+		processor.save()
 
 if __name__=="__main__":
 	main(sys.argv[1:])
```

### Comparing `cosmosis-3.0/cosmosis/postprocessing/__init__.py` & `cosmosis-3.0.1/cosmosis/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/postprocessing/cosmology_theory_plots.py` & `cosmosis-3.0.1/cosmosis/postprocessing/cosmology_theory_plots.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/postprocessing/density.py` & `cosmosis-3.0.1/cosmosis/postprocessing/density.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/postprocessing/elements.py` & `cosmosis-3.0.1/cosmosis/postprocessing/elements.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/postprocessing/inputs.py` & `cosmosis-3.0.1/cosmosis/postprocessing/inputs.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/postprocessing/latex.ini` & `cosmosis-3.0.1/cosmosis/postprocessing/latex.ini`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/postprocessing/lazy_pylab.py` & `cosmosis-3.0.1/cosmosis/postprocessing/lazy_pylab.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/postprocessing/main.py` & `cosmosis-3.0.1/cosmosis/postprocessing/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     else:
         labels = [f"chain_{i}" for i in range(len(inputs))]
 
     if len(inputs)>1 and run_max_post:
         raise ValueError("Can only use the --run-max-post argument with a single parameter file for now")
 
     processors = []
+    processor = None
 
     for i, ini_filename in enumerate(inputs):
         if "astropy" in str(type(ini_filename)):
             ini_filename.meta.setdefault("chain_name", labels[i])
 
         sampler, ini = read_input(ini_filename, text, weights)
         processor_class = postprocessor_for_sampler(sampler.split()[-1])
@@ -76,14 +77,18 @@
         #Run the postprocessor and make the outputs for this chain
         processor.run()
 
         #Save the outputs ready for the next post-processor in case
         #they want to add to it (e.g. two constriants on the same axes)
         outputs.update(processor.outputs)
 
+    # If there was no successul postprocessor then we are done
+    if processor is None:
+        return
+
     # Finalize all the elements - this adds legends to any plots
     # that need them. This final processor knows about all the
     # outputs that we made.
     processor.finalize()
 
     if sampler is None:
         return
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cosmosis-3.0/cosmosis/postprocessing/outputs.py` & `cosmosis-3.0.1/cosmosis/postprocessing/outputs.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/postprocessing/plots.py` & `cosmosis-3.0.1/cosmosis/postprocessing/plots.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/postprocessing/postprocess.py` & `cosmosis-3.0.1/cosmosis/postprocessing/postprocess.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/postprocessing/postprocess_base.py` & `cosmosis-3.0.1/cosmosis/postprocessing/postprocess_base.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/postprocessing/reruns.py` & `cosmosis-3.0.1/cosmosis/postprocessing/reruns.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/postprocessing/statistics.py` & `cosmosis-3.0.1/cosmosis/postprocessing/statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -416,19 +416,19 @@
         self.report_screen_median()
         self.report_screen_mode()
         #self.report_screen_limits()
 
     def report_file(self):
         #Get the filenames to make
         return [
-            self.report_file_mean(),
-            self.report_file_median(),
-            self.report_file_mode(),
-            self.report_file_l95(),
-            self.report_file_u95(),
+            self.report_centroid("means", self.mu),
+            self.report_centroid("medians", self.median),
+            # self.report_centroid("modes", self.peak1d),
+            self.report_limit("l95", self.l95),
+            self.report_limit("u95", self.u95),
             ]
 
     def compute_stats(self):
         #1D stats
         self.mu = np.zeros(self.ncol)
         self.median = np.zeros(self.ncol)
         self.sigma = np.zeros(self.ncol)
```

### Comparing `cosmosis-3.0/cosmosis/postprocessing/utils.py` & `cosmosis-3.0.1/cosmosis/postprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/runtime/analytics.py` & `cosmosis-3.0.1/cosmosis/runtime/analytics.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/runtime/attribution.py` & `cosmosis-3.0.1/cosmosis/runtime/attribution.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/runtime/config.py` & `cosmosis-3.0.1/cosmosis/runtime/config.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/runtime/declare.py` & `cosmosis-3.0.1/cosmosis/runtime/declare.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/runtime/julia_modules/julia.py` & `cosmosis-3.0.1/cosmosis/runtime/julia_modules/julia.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/runtime/logs.py` & `cosmosis-3.0.1/cosmosis/runtime/logs.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/runtime/memmon.py` & `cosmosis-3.0.1/cosmosis/runtime/memmon.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/runtime/module.py` & `cosmosis-3.0.1/cosmosis/runtime/module.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/runtime/mpi_pool.py` & `cosmosis-3.0.1/cosmosis/runtime/mpi_pool.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/runtime/parameter.py` & `cosmosis-3.0.1/cosmosis/runtime/parameter.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/runtime/pipeline.py` & `cosmosis-3.0.1/cosmosis/runtime/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -640,24 +640,24 @@
 
             if self.timing:
                 t2 = time.time()
                 timings.append(t2-t1)
                 sys.stdout.write("%s took: %.3f seconds\n"% (module,t2-t1))
 
             if status:
-                if logs.is_enabled_for(logs.debug):
+                if logs.is_enabled_for(logs.logging.DEBUG):
                     data_package.print_log()
                     logs.noisy("Because you set debug verbosity I printed a log of "
                                    "all access to data printed above. "
                                    "Look for the word 'FAIL' \n"
                                    "Though the error message could also be "
                                    "somewhere above that.\n")
 
                 logs.warning("Error running pipeline ({status}). Returning zero likelihood. Error may be above.")
-                if not logs.is_enabled_for(logs.debug):
+                if not logs.is_enabled_for(logs.logging.DEBUG):
                     logs.warning("Set log level to 'debug' for more info.")
                 return None
 
             # If we are using a fast/slow split (and we are not already running on a cached subset)
             # Then see if it wants to cache these results
             if self.slow_subspace_cache and first_module==0:
                 self.slow_subspace_cache.next_module_results(module_number, data_package)
```

### Comparing `cosmosis-3.0/cosmosis/runtime/prior.py` & `cosmosis-3.0.1/cosmosis/runtime/prior.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/runtime/process_pool.py` & `cosmosis-3.0.1/cosmosis/runtime/process_pool.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/__init__.py` & `cosmosis-3.0.1/cosmosis/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/abc/abc_sampler.py` & `cosmosis-3.0.1/cosmosis/samplers/abc/abc_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/abc/abc_sampler_mpi.py` & `cosmosis-3.0.1/cosmosis/samplers/abc/abc_sampler_mpi.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/apriori/apriori_sampler.py` & `cosmosis-3.0.1/cosmosis/samplers/apriori/apriori_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/dynesty/dynesty_sampler.py` & `cosmosis-3.0.1/cosmosis/samplers/dynesty/dynesty_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/emcee/emcee_sampler.py` & `cosmosis-3.0.1/cosmosis/samplers/emcee/emcee_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/fisher/fisher.py` & `cosmosis-3.0.1/cosmosis/samplers/fisher/fisher.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/fisher/fisher_sampler.py` & `cosmosis-3.0.1/cosmosis/samplers/fisher/fisher_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/grid/grid_sampler.py` & `cosmosis-3.0.1/cosmosis/samplers/grid/grid_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/gridmax/gridmax_sampler.py` & `cosmosis-3.0.1/cosmosis/samplers/gridmax/gridmax_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/hints.py` & `cosmosis-3.0.1/cosmosis/samplers/hints.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/importance/importance_sampler.py` & `cosmosis-3.0.1/cosmosis/samplers/importance/importance_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/kombine/kombine_sampler.py` & `cosmosis-3.0.1/cosmosis/samplers/kombine/kombine_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/list/list_sampler.py` & `cosmosis-3.0.1/cosmosis/samplers/list/list_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/maxlike/maxlike_sampler.py` & `cosmosis-3.0.1/cosmosis/samplers/maxlike/maxlike_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/metropolis/metropolis.py` & `cosmosis-3.0.1/cosmosis/samplers/metropolis/metropolis.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/metropolis/metropolis_sampler.py` & `cosmosis-3.0.1/cosmosis/samplers/metropolis/metropolis_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/metropolis/proposal/cobaya_proposal.py` & `cosmosis-3.0.1/cosmosis/samplers/metropolis/proposal/cobaya_proposal.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/metropolis/proposal/standard.py` & `cosmosis-3.0.1/cosmosis/samplers/metropolis/proposal/standard.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/minuit/Makefile` & `cosmosis-3.0.1/cosmosis/samplers/minuit/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/minuit/minuit_sampler.py` & `cosmosis-3.0.1/cosmosis/samplers/minuit/minuit_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/minuit/minuit_wrapper.cpp` & `cosmosis-3.0.1/cosmosis/samplers/minuit/minuit_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/multinest/multinest_sampler.py` & `cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,37 +56,42 @@
     dumper_type, #dumper,
     ct.c_voidp, #context
 ]
 
 
 MULTINEST_SECTION='multinest'
 
+def load_multinest_library(mpi_version):
+    if mpi_version:
+        libname = "libnest3_mpi.so"
+    else:
+        libname = "libnest3.so"
+    dirname = os.path.split(__file__)[0]
+    libname = os.path.join(dirname, "multinest_src", libname)
+        
+    try:
+        libnest3 = ct.cdll.LoadLibrary(libname)
+    except Exception as error:
+        raise RuntimeError("Multinest could not be loaded.\n"
+                            "This may mean an MPI compiler was not found to compile it,\n"
+                            "or that some other error occurred.  More info below:\n"
+                            + str(error)+'\n')
+
+    return libnest3
+
+
 
 class MultinestSampler(ParallelSampler):
     parallel_output = False
     sampler_outputs = [("prior", float), ("like", float), ("post", float), ("weight", float)]
     supports_smp=False
     internal_resume = True
 
     def config(self):
-        if self.pool:
-            libname = "libnest3_mpi.so"
-        else:
-            libname = "libnest3.so"
-
-        dirname = os.path.split(__file__)[0]
-        libname = os.path.join(dirname, "multinest_src", libname)
-            
-        try:
-            libnest3 = ct.cdll.LoadLibrary(libname)
-        except Exception as error:
-            raise RuntimeError("Multinest could not be loaded.\n"
-                             "This may mean an MPI compiler was not found to compile it,\n"
-                             "or that some other error occurred.  More info below:\n"
-                             + str(error)+'\n')
+        libnest3 = load_multinest_library(self.pool is not None)
 
         self._run = libnest3.run
         self._run.restype=None
         self._run.argtypes = multinest_args
         self.converged=False
 
         self.ndim = len(self.pipeline.varied_params)
```

### Comparing `cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/LICENCE` & `cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/LICENCE`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/Makefile` & `cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/README` & `cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/README`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/cwrapper.f90` & `cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/cwrapper.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90` & `cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/nested.f90` & `cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/nested.f90`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,49 @@
   logical debug, prior_warning, resume, outfile
   !importance sampling
   logical :: IS = .true.
   logical bogus
 
 contains
   
+
+#ifdef MPI
+! This is a workaround for an MPICH bug
+! https://github.com/pmodels/mpich/issues/5995
+  subroutine mpi_bcast_logical(logical_var, ierror)
+	implicit none
+	logical logical_var
+	integer ierror
+	integer integer_var
+	integer_var = 0
+	if (logical_var) integer_var = 1
+	call MPI_BCAST(integer_var, 1, MPI_INTEGER, 0, MPI_COMM_WORLD, ierror)
+	logical_var = (integer_var == 1)
+  end subroutine mpi_bcast_logical
+
+  subroutine mpi_bcast_logical_array(n, logical_arr, ierror)
+	implicit none
+	integer n
+	logical logical_arr(n)
+	integer ierror
+	integer integer_arr(n)
+	integer i
+	integer_arr(:) = 0
+	do i=1,n
+		if (logical_arr(i)) integer_arr(i) = 1
+	end do
+
+	call MPI_BCAST(integer_arr, n, MPI_INTEGER, 0, MPI_COMM_WORLD, ierror)
+	do i=1,n
+		logical_arr(i) = (integer_arr(i) == 1)
+	end do
+	
+  end subroutine mpi_bcast_logical_array
+#endif
+
   subroutine nestRun(nest_IS,nest_mmodal,nest_ceff,nest_nlive,nest_tol,nest_ef,nest_ndims,nest_totPar,nest_nCdims,maxClst, &
   nest_updInt,nest_Ztol,nest_root,seed,nest_pWrap,nest_fb,nest_resume,nest_outfile,initMPI,nest_logZero,nest_maxIter, &
   loglike,dumper,context)
         
   	implicit none
         
 	integer nest_ndims,nest_nlive,nest_updInt,context,seed,i
@@ -340,17 +375,21 @@
 		
 		endif
 	
 		gZ=logZero
 		ginfo=0.d0
 	endif
 
+
+
 #ifdef MPI
 	call MPI_BARRIER(MPI_COMM_WORLD,errcode)
-	call MPI_BCAST(genLive,1,MPI_LOGICAL,0,MPI_COMM_WORLD,errcode)
+	!call MPI_BCAST(genLive,1,MPI_LOGICAL,0,MPI_COMM_WORLD,errcode)
+	!JAZ
+	call mpi_bcast_logical(genLive, errcode)
 #endif
 	
 	if(genLive) then
 		if(my_rank==0 .and. fback) write(*,*) 'generating live points'
 		
 		call gen_initial_live(p,phyP,l,loglike,dumper,context)
 	
@@ -593,15 +632,16 @@
             					write(u_phys,fmt2) phyP(:,m),l(m),1
 					enddo
 				endif
 			endif
 		endif
 
 #ifdef MPI
-		call MPI_BCAST(bogus,1,MPI_LOGICAL,0,MPI_COMM_WORLD,errcode)
+		! call MPI_BCAST(bogus,1,MPI_LOGICAL,0,MPI_COMM_WORLD,errcode)
+		call mpi_bcast_logical(bogus, errcode)
 #endif
 
 		if(k==nptPerProc .or. bogus) exit
 	enddo
 	
 	
 		
@@ -1078,15 +1118,16 @@
 	call MPI_BCAST(ic_npt(1:ic_n),ic_n,MPI_INTEGER,0,MPI_COMM_WORLD,errcode)
 #endif
 		
 	do ff=1,maxIter
 
 #ifdef MPI
     		call MPI_BARRIER(MPI_COMM_WORLD,errcode)
-    		call MPI_BCAST(ic_done(0:ic_n),ic_n+1,MPI_LOGICAL,0,MPI_COMM_WORLD,errcode)
+    		! call MPI_BCAST(ic_done(0:ic_n),ic_n+1,MPI_LOGICAL,0,MPI_COMM_WORLD,errcode)
+			call mpi_bcast_logical_array(ic_n+1, ic_done(0:ic_n), errcode)
 #endif	
 		!stopping condition reached
 		if(ic_done(0)) then
 			if(my_rank==0) then
                         
 				if(outfile) then
 	                        	!write the resume file
@@ -1585,23 +1626,36 @@
 			ic_rFlag(1:ic_n)=.false.
 		endif
 		
 		
             	if(my_rank==0 .and. eswitch .and. sc_n==0) eswitch=.false.
 #ifdef MPI
 		call MPI_BARRIER(MPI_COMM_WORLD,errcode)
-		call MPI_BCAST(eswitch,1,MPI_LOGICAL,0,MPI_COMM_WORLD,errcode)
-		call MPI_BCAST(flag2,1,MPI_LOGICAL,0,MPI_COMM_WORLD,errcode)
-		call MPI_BCAST(modeFound,1,MPI_LOGICAL,0,MPI_COMM_WORLD,errcode)
+
+		! call MPI_BCAST(eswitch,1,MPI_LOGICAL,0,MPI_COMM_WORLD,errcode)
+		! JAZ
+		call mpi_bcast_logical(eswitch, errcode)
+
+		! call MPI_BCAST(flag2,1,MPI_LOGICAL,0,MPI_COMM_WORLD,errcode)
+		! JAZ 
+		call mpi_bcast_logical(flag2, errcode)
+
+		! call MPI_BCAST(modeFound,1,MPI_LOGICAL,0,MPI_COMM_WORLD,errcode)
+		! JAZ
+		call mpi_bcast_logical(modeFound, errcode)
+
 		call MPI_BCAST(lowlike,1,MPI_DOUBLE_PRECISION,0,MPI_COMM_WORLD,errcode)
 		
 		if(modeFound) then
 			call MPI_BCAST(ic_n,1,MPI_INTEGER,0,MPI_COMM_WORLD,errcode)
 			call MPI_BCAST(ic_npt(1:ic_n),ic_n,MPI_INTEGER,0,MPI_COMM_WORLD,errcode)
-    			call MPI_BCAST(ic_done(0:ic_n),ic_n+1,MPI_LOGICAL,0,MPI_COMM_WORLD,errcode)
+
+			! JAZ
+			! call MPI_BCAST(ic_done(0:ic_n),ic_n+1,MPI_LOGICAL,0,MPI_COMM_WORLD,errcode)
+			call mpi_bcast_logical_array(ic_n+1, ic_done(0:ic_n), errcode)
 		endif
 		
 		if(flag2 .and. eswitch) then
 			call MPI_BCAST(sc_n,1,MPI_INTEGER,0,MPI_COMM_WORLD,errcode)
 			call MPI_BCAST(ic_sc(1:ic_n),ic_n,MPI_INTEGER,0,MPI_COMM_WORLD,errcode)
 			call MPI_BCAST(sc_mean(1:sc_n,1:ndims),sc_n*ndims,MPI_DOUBLE_PRECISION,0,MPI_COMM_WORLD,errcode)
 			call MPI_BCAST(sc_tmat(1:sc_n,1:ndims,1:ndims),sc_n*ndims*ndims,MPI_DOUBLE_PRECISION,0,MPI_COMM_WORLD,errcode)
@@ -1806,15 +1860,17 @@
 				!now find a new point inside the hard constraint
 				if(.not.eswitch) then
 	            			acpt=.false.
 					do
 						if(my_rank==0) remFlag=remain(nd)
 #ifdef MPI
 						call MPI_BARRIER(MPI_COMM_WORLD,errcode)
-						call MPI_BCAST(remFlag,1,MPI_LOGICAL,0,MPI_COMM_WORLD,errcode)
+						! call MPI_BCAST(remFlag,1,MPI_LOGICAL,0,MPI_COMM_WORLD,errcode)
+						! JAZ
+						call mpi_bcast_logical(remFlag, errcode)
 #endif
 	                  			if(.not.remFlag) then
 	            					!generate mpi_nthreads potential points
 							call samp(pnew,phyPnew,lnew,sc_mean(1,:),d1,sc_tMat(1,:,:),ic_climits(nd,:,:),loglike,eswitch,lowlike,n,context)
 						
 							if(my_rank==0) then
 								lnewa(nd,1)=lnew
@@ -1897,16 +1953,21 @@
 									rIdx(nd)=1
 								endif
 							enddo
 						endif
 					
 #ifdef MPI
 						call MPI_BARRIER(MPI_COMM_WORLD,errcode)
-						call MPI_BCAST(acpt,1,MPI_LOGICAL,0,MPI_COMM_WORLD,errcode)
-						call MPI_BCAST(bogus,1,MPI_LOGICAL,0,MPI_COMM_WORLD,errcode)
+						! call MPI_BCAST(acpt,1,MPI_LOGICAL,0,MPI_COMM_WORLD,errcode)
+						! JAZ
+						call mpi_bcast_logical(acpt, errcode)
+
+						! call MPI_BCAST(bogus,1,MPI_LOGICAL,0,MPI_COMM_WORLD,errcode)
+						! JAZ
+						call mpi_bcast_logical(bogus, errcode)
 #endif
 	                        	
 						if(acpt .or. bogus) exit
 					enddo
 				
 	                        	if(my_rank==0) then      	
 	                  			p(:,indx(1))=pnew(:)
@@ -1950,15 +2011,17 @@
 					num_old=numlike
 					
 					acpt=.false.
 					do
 						if(my_rank==0) remFlag=remain(nd)
 #ifdef MPI
 						call MPI_BARRIER(MPI_COMM_WORLD,errcode)
-						call MPI_BCAST(remFlag,1,MPI_LOGICAL,0,MPI_COMM_WORLD,errcode)
+						! call MPI_BCAST(remFlag,1,MPI_LOGICAL,0,MPI_COMM_WORLD,errcode)
+						! JAZ
+						call mpi_bcast_logical(remFlag, errcode)
 #endif
 						if(.not.remFlag) then
 							!first pick an ellipsoid according to the vol
 							do
 								!pick a sub-cluster according to the vol
 								call selectEll(ic_sc(nd),sc_vol(nd_i+1:nd_i+ic_sc(nd)),i)
 								i=i+nd_i
@@ -2109,16 +2172,22 @@
 									rIdx(nd)=1
 								endif
 							enddo
 						endif
 					
 #ifdef MPI
 						call MPI_BARRIER(MPI_COMM_WORLD,errcode)
-						call MPI_BCAST(acpt,1,MPI_LOGICAL,0,MPI_COMM_WORLD,errcode)
-						call MPI_BCAST(bogus,1,MPI_LOGICAL,0,MPI_COMM_WORLD,errcode)
+						! call MPI_BCAST(acpt,1,MPI_LOGICAL,0,MPI_COMM_WORLD,errcode)
+						! JAZ
+						call mpi_bcast_logical(acpt, errcode)
+
+						! call MPI_BCAST(bogus,1,MPI_LOGICAL,0,MPI_COMM_WORLD,errcode)
+						! JAZ
+						call mpi_bcast_logical(bogus, errcode)
+
 #endif
 					
 						if( bogus ) exit
 					
 	                        		if(acpt) then
 							if(my_rank==0) then
 								pnew=pnewa(nd,j1,:)
```

### Comparing `cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/posterior.f90` & `cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/posterior.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/priors.f90` & `cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/priors.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/utils.f90` & `cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/utils.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/utils1.f90` & `cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/utils1.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90` & `cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/nautilus/nautilus_sampler.py` & `cosmosis-3.0.1/cosmosis/samplers/nautilus/nautilus_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py` & `cosmosis-3.0.1/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/pmc/pmc.py` & `cosmosis-3.0.1/cosmosis/samplers/pmc/pmc.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/pmc/pmc_sampler.py` & `cosmosis-3.0.1/cosmosis/samplers/pmc/pmc_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/poco/poco_sampler.py` & `cosmosis-3.0.1/cosmosis/samplers/poco/poco_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/polychord/polychord_sampler.py` & `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/LICENCE` & `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/LICENCE`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/Makefile` & `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/README` & `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/README`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/abort.F90` & `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/abort.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/array_utils.f90` & `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/array_utils.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/c_interface.cpp` & `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/c_interface.cpp`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/calculate.f90` & `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/calculate.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90` & `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/clustering.f90` & `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/clustering.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/feedback.f90` & `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/feedback.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/generate.F90` & `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/generate.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/ini.f90` & `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/ini.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/interfaces.F90` & `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/interfaces.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/interfaces.h` & `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/interfaces.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/interfaces.hpp` & `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/interfaces.hpp`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90` & `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90` & `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/params.f90` & `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/params.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/priors.f90` & `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/priors.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/random_utils.F90` & `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/random_utils.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/read_write.f90` & `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/read_write.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/run_time_info.f90` & `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/run_time_info.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/settings.f90` & `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/settings.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/utils.F90` & `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/utils.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/pymc/pymc_sampler.py` & `cosmosis-3.0.1/cosmosis/samplers/pymc/pymc_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/sampler.py` & `cosmosis-3.0.1/cosmosis/samplers/sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/snake/snake.py` & `cosmosis-3.0.1/cosmosis/samplers/snake/snake.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/snake/snake_sampler.py` & `cosmosis-3.0.1/cosmosis/samplers/snake/snake_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/star/star_sampler.py` & `cosmosis-3.0.1/cosmosis/samplers/star/star_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/test/test_sampler.py` & `cosmosis-3.0.1/cosmosis/samplers/test/test_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/samplers/zeus/zeus_sampler.py` & `cosmosis-3.0.1/cosmosis/samplers/zeus/zeus_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/test/example_module2.py` & `cosmosis-3.0.1/cosmosis/test/example_module2.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/test/libtest/Makefile` & `cosmosis-3.0.1/cosmosis/test/libtest/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/test/libtest/c_datablock_complex_array_test.c` & `cosmosis-3.0.1/cosmosis/test/libtest/c_datablock_complex_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/test/libtest/c_datablock_double_array_test.c` & `cosmosis-3.0.1/cosmosis/test/libtest/c_datablock_double_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/test/libtest/c_datablock_int_array_test.c` & `cosmosis-3.0.1/cosmosis/test/libtest/c_datablock_int_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c` & `cosmosis-3.0.1/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c` & `cosmosis-3.0.1/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c` & `cosmosis-3.0.1/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/test/libtest/c_datablock_test.c` & `cosmosis-3.0.1/cosmosis/test/libtest/c_datablock_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/test/libtest/cosmosis_test.F90` & `cosmosis-3.0.1/cosmosis/test/libtest/cosmosis_test.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/test/libtest/datablock_test.cc` & `cosmosis-3.0.1/cosmosis/test/libtest/datablock_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/test/libtest/entry_test.cc` & `cosmosis-3.0.1/cosmosis/test/libtest/entry_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/test/libtest/ndarray_test.cc` & `cosmosis-3.0.1/cosmosis/test/libtest/ndarray_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/test/libtest/section_test.cc` & `cosmosis-3.0.1/cosmosis/test/libtest/section_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/test/libtest/test_c_datablock_scalars.h` & `cosmosis-3.0.1/cosmosis/test/libtest/test_c_datablock_scalars.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/test/libtest/test_c_datablock_scalars.template` & `cosmosis-3.0.1/cosmosis/test/libtest/test_c_datablock_scalars.template`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/test/test_block.py` & `cosmosis-3.0.1/cosmosis/test/test_block.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/test/test_campaign.py` & `cosmosis-3.0.1/cosmosis/test/test_campaign.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/test/test_chaining.py` & `cosmosis-3.0.1/cosmosis/test/test_chaining.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/test/test_gaussian.py` & `cosmosis-3.0.1/cosmosis/test/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/test/test_lib.py` & `cosmosis-3.0.1/cosmosis/test/test_lib.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/test/test_modules.py` & `cosmosis-3.0.1/cosmosis/test/test_modules.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/test/test_parameters.py` & `cosmosis-3.0.1/cosmosis/test/test_parameters.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/test/test_pipeline.py` & `cosmosis-3.0.1/cosmosis/test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/test/test_polychord.py` & `cosmosis-3.0.1/cosmosis/test/test_polychord.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/test/test_samplers.py` & `cosmosis-3.0.1/cosmosis/test/test_samplers.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/test/test_text_output.py` & `cosmosis-3.0.1/cosmosis/test/test_text_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/test/test_utils.py` & `cosmosis-3.0.1/cosmosis/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis/utils.py` & `cosmosis-3.0.1/cosmosis/utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/cosmosis.egg-info/SOURCES.txt` & `cosmosis-3.0.1/cosmosis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0/setup.py` & `cosmosis-3.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -123,14 +123,27 @@
         # and the MPI compiler
         env["MPIFC"] = "mpif90"
 
     env['FC'] = env.get('FC', 'gfortran')
 
     subprocess.check_call(["make"], env=env, cwd="cosmosis")
 
+class build_cosmosis(setuptools.Command):
+    description = "Build CosmoSIS and do nothing else"
+    user_options = []
+
+    def initialize_options(self):
+        pass
+
+    def finalize_options(self):
+        pass
+
+    def run(self):
+        make_cosmosis()
+
 
 
 class build_py_cosmosis(setuptools.command.build_py.build_py):
     def run(self):
         make_cosmosis()
         super().run()
 
@@ -194,14 +207,15 @@
     author_email      = "joezuntz@googlemail.com",
     url               = "https://github.com/joezuntz/cosmosis",
     packages = setuptools.find_packages(),
     package_data = {"cosmosis" : all_package_files},
     scripts = scripts,
     install_requires = requirements,
     cmdclass={
+        "build_cosmosis": build_cosmosis,
         "build_py": build_py_cosmosis,
         "install": install_cosmosis,
         "develop": develop_cosmosis,
         "clean": clean_cosmosis,
     },
     version=version,
 )
```

