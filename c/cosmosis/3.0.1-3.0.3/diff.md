# Comparing `tmp/cosmosis-3.0.1.tar.gz` & `tmp/cosmosis-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmosis-3.0.1.tar", last modified: Fri Jul 28 09:33:18 2023, max compression
+gzip compressed data, was "cosmosis-3.0.3.tar", last modified: Fri Jul 28 18:31:33 2023, max compression
```

## Comparing `cosmosis-3.0.1.tar` & `cosmosis-3.0.3.tar`

### file list

```diff
@@ -1,290 +1,290 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.629813 cosmosis-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-28 09:33:17.000000 cosmosis-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-07-28 09:33:17.000000 cosmosis-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-28 09:33:18.629813 cosmosis-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-28 09:33:17.000000 cosmosis-3.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.605813 cosmosis-3.0.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      102 2023-07-28 09:33:17.000000 cosmosis-3.0.1/bin/cosmosis
--rwxr-xr-x   0 runner    (1001) docker     (123)      122 2023-07-28 09:33:17.000000 cosmosis-3.0.1/bin/cosmosis-campaign
--rwxr-xr-x   0 runner    (1001) docker     (123)      792 2023-07-28 09:33:17.000000 cosmosis-3.0.1/bin/cosmosis-configure
--rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-07-28 09:33:17.000000 cosmosis-3.0.1/bin/cosmosis-extract
--rwxr-xr-x   0 runner    (1001) docker     (123)      102 2023-07-28 09:33:17.000000 cosmosis-3.0.1/bin/cosmosis-postprocess
--rwxr-xr-x   0 runner    (1001) docker     (123)     1527 2023-07-28 09:33:17.000000 cosmosis-3.0.1/bin/cosmosis-sample-fisher
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.609813 cosmosis-3.0.1/cosmosis/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20918 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/campaign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.609813 cosmosis-3.0.1/cosmosis/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/config/compilers.mk
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/config/subdirs.mk
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.609813 cosmosis-3.0.1/cosmosis/datablock/
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51706 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/c_datablock.cc
--rw-r--r--   0 runner    (1001) docker     (123)    22811 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/c_datablock.h
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/clamp.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/cosmosis_constants.fh
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/cosmosis_constants.h
--rw-r--r--   0 runner    (1001) docker     (123)    34029 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/cosmosis_modules.F90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.613813 cosmosis-3.0.1/cosmosis/datablock/cosmosis_py/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/cosmosis_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52767 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/cosmosis_py/block.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/cosmosis_py/dbt_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/cosmosis_py/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/cosmosis_py/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/cosmosis_py/section_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/cosmosis_section_names.F90
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/cosmosis_types.F90
--rw-r--r--   0 runner    (1001) docker     (123)    28871 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/cosmosis_wrappers.F90
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/datablock.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11180 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/datablock.hh
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/datablock_logging.cc
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/datablock_logging.h
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/datablock_status.h
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/datablock_types.h
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/entry.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11879 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/entry.hh
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/exceptions.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/generate_sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/handler.c
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/ndarray.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/section.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/section.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/section_names.h
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/datablock/section_names.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/gaussian_likelihood.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22922 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/names.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.613813 cosmosis-3.0.1/cosmosis/output/
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/output/astropy_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/output/cosmomc_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/output/fits_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/output/in_memory_output.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/output/null_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/output/output_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/output/text_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/output/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.613813 cosmosis-3.0.1/cosmosis/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/plotting/chain_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/plotting/grid_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/plotting/kde.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      404 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/plotting/plot_demo_3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/plotting/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/plotting/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5392 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.613813 cosmosis-3.0.1/cosmosis/postprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocessing/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16175 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocessing/cosmology_theory_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocessing/density.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocessing/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocessing/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocessing/latex.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocessing/lazy_pylab.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocessing/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocessing/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    49133 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocessing/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocessing/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocessing/postprocess_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocessing/reruns.py
--rw-r--r--   0 runner    (1001) docker     (123)    31638 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocessing/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/postprocessing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/attribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    13893 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/declare.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/runtime/julia_modules/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/julia_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/julia_modules/julia.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/memmon.py
--rw-r--r--   0 runner    (1001) docker     (123)    17198 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/mpi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    55645 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    21210 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/process_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/runtime/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/abc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/abc/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7126 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/abc/abc_sampler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6698 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/abc/abc_sampler_mpi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/apriori/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/apriori/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2176 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/apriori/apriori_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/dynesty/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/dynesty/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3722 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/dynesty/dynesty_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/emcee/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/emcee/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7452 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/emcee/emcee_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/fisher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/fisher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/fisher/fisher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6652 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/fisher/fisher_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/grid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/grid/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4683 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/grid/grid_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/gridmax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/gridmax/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4370 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/gridmax/gridmax_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/hints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/importance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/importance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/importance/importance_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/kombine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/kombine/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4932 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/kombine/kombine_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/list/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/list/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4888 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/list/list_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/maxlike/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/maxlike/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4578 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/maxlike/maxlike_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/metropolis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/metropolis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/metropolis/metropolis.py
--rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/metropolis/metropolis_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/metropolis/proposal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/metropolis/proposal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/metropolis/proposal/cobaya_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/metropolis/proposal/standard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/minuit/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/minuit/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/minuit/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7325 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/minuit/minuit_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/minuit/minuit_wrapper.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.617813 cosmosis-3.0.1/cosmosis/samplers/multinest/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/multinest/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/multinest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.621813 cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    19512 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/README
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/cwrapper.f90
--rw-r--r--   0 runner    (1001) docker     (123)    42915 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90
--rw-r--r--   0 runner    (1001) docker     (123)   107766 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/nested.f90
--rw-r--r--   0 runner    (1001) docker     (123)    22010 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/posterior.f90
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/priors.f90
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/utils.f90
--rw-r--r--   0 runner    (1001) docker     (123)    28039 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/utils1.f90
--rw-r--r--   0 runner    (1001) docker     (123)    86938 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.621813 cosmosis-3.0.1/cosmosis/samplers/nautilus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/nautilus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/nautilus/nautilus_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.621813 cosmosis-3.0.1/cosmosis/samplers/pmaxlike/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/pmaxlike/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4151 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.621813 cosmosis-3.0.1/cosmosis/samplers/pmc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/pmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/pmc/pmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/pmc/pmc_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.621813 cosmosis-3.0.1/cosmosis/samplers/poco/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/poco/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3660 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/poco/poco_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.621813 cosmosis-3.0.1/cosmosis/samplers/polychord/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.621813 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/README
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/abort.F90
--rw-r--r--   0 runner    (1001) docker     (123)    18110 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/array_utils.f90
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/c_interface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/calculate.f90
--rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90
--rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/clustering.f90
--rw-r--r--   0 runner    (1001) docker     (123)    13421 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/feedback.f90
--rw-r--r--   0 runner    (1001) docker     (123)    26147 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/generate.F90
--rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/ini.f90
--rw-r--r--   0 runner    (1001) docker     (123)    20999 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/interfaces.F90
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/interfaces.h
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/interfaces.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    24257 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90
--rw-r--r--   0 runner    (1001) docker     (123)    20674 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/params.f90
--rw-r--r--   0 runner    (1001) docker     (123)    19675 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/priors.f90
--rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/random_utils.F90
--rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/read_write.f90
--rw-r--r--   0 runner    (1001) docker     (123)    47427 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/run_time_info.f90
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/settings.f90
--rw-r--r--   0 runner    (1001) docker     (123)    29353 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/utils.F90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.625813 cosmosis-3.0.1/cosmosis/samplers/pymc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/pymc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/pymc/pymc_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.625813 cosmosis-3.0.1/cosmosis/samplers/snake/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/snake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/snake/snake.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1987 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/snake/snake_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.625813 cosmosis-3.0.1/cosmosis/samplers/star/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/star/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4422 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/star/star_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.625813 cosmosis-3.0.1/cosmosis/samplers/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/test/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3221 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/test/test_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.625813 cosmosis-3.0.1/cosmosis/samplers/zeus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/zeus/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11469 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/samplers/zeus/zeus_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.625813 cosmosis-3.0.1/cosmosis/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/campaign.yml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/example-priors.ini
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/example-values.ini
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/example.ini
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/example_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/example_module2.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/example_module3.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/example_module4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.625813 cosmosis-3.0.1/cosmosis/test/libtest/
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/c_datablock_complex_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/c_datablock_double_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/c_datablock_int_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/c_datablock_test.c
--rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/cosmosis_test.F90
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/cosmosis_tests.supp
--rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/datablock_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/entry_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/ndarray_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/section_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    28088 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/test_c_datablock_scalars.h
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/libtest/test_c_datablock_scalars.template
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/test_campaign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/test_chaining.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/test_polychord.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/test_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/test_text_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 09:33:17.000000 cosmosis-3.0.1/cosmosis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:33:18.609813 cosmosis-3.0.1/cosmosis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-28 09:33:18.000000 cosmosis-3.0.1/cosmosis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-07-28 09:33:18.000000 cosmosis-3.0.1/cosmosis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 09:33:18.000000 cosmosis-3.0.1/cosmosis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-28 09:33:18.000000 cosmosis-3.0.1/cosmosis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-28 09:33:18.000000 cosmosis-3.0.1/cosmosis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 09:33:17.000000 cosmosis-3.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 09:33:18.629813 cosmosis-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-07-28 09:33:17.000000 cosmosis-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.566161 cosmosis-3.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-28 18:31:29.000000 cosmosis-3.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-07-28 18:31:29.000000 cosmosis-3.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-28 18:31:33.566161 cosmosis-3.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-28 18:31:29.000000 cosmosis-3.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.538161 cosmosis-3.0.3/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      102 2023-07-28 18:31:29.000000 cosmosis-3.0.3/bin/cosmosis
+-rwxr-xr-x   0 runner    (1001) docker     (123)      122 2023-07-28 18:31:29.000000 cosmosis-3.0.3/bin/cosmosis-campaign
+-rwxr-xr-x   0 runner    (1001) docker     (123)      792 2023-07-28 18:31:29.000000 cosmosis-3.0.3/bin/cosmosis-configure
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-07-28 18:31:29.000000 cosmosis-3.0.3/bin/cosmosis-extract
+-rwxr-xr-x   0 runner    (1001) docker     (123)      102 2023-07-28 18:31:29.000000 cosmosis-3.0.3/bin/cosmosis-postprocess
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1527 2023-07-28 18:31:29.000000 cosmosis-3.0.3/bin/cosmosis-sample-fisher
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.542161 cosmosis-3.0.3/cosmosis/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20918 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/campaign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.542161 cosmosis-3.0.3/cosmosis/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/config/compilers.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/config/subdirs.mk
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.546161 cosmosis-3.0.3/cosmosis/datablock/
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51706 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/c_datablock.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    22811 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/c_datablock.h
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/clamp.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/cosmosis_constants.fh
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/cosmosis_constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34029 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/cosmosis_modules.F90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.546161 cosmosis-3.0.3/cosmosis/datablock/cosmosis_py/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/cosmosis_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52767 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/cosmosis_py/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/cosmosis_py/dbt_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/cosmosis_py/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/cosmosis_py/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/cosmosis_py/section_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/cosmosis_section_names.F90
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/cosmosis_types.F90
+-rw-r--r--   0 runner    (1001) docker     (123)    28871 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/cosmosis_wrappers.F90
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/datablock.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11180 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/datablock.hh
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/datablock_logging.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/datablock_logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/datablock_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/datablock_types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/entry.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11879 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/entry.hh
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/exceptions.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/generate_sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/handler.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/ndarray.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/section.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/section.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/section_names.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/section_names.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/gaussian_likelihood.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22922 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/names.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.546161 cosmosis-3.0.3/cosmosis/output/
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/output/astropy_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/output/cosmomc_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/output/fits_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/output/in_memory_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/output/null_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/output/output_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/output/text_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/output/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.546161 cosmosis-3.0.3/cosmosis/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/plotting/chain_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/plotting/grid_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/plotting/kde.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      404 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/plotting/plot_demo_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/plotting/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/plotting/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5392 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.550161 cosmosis-3.0.3/cosmosis/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocessing/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16175 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocessing/cosmology_theory_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocessing/density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocessing/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocessing/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocessing/latex.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocessing/lazy_pylab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocessing/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocessing/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49133 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocessing/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocessing/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocessing/postprocess_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocessing/reruns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31638 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocessing/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocessing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.550161 cosmosis-3.0.3/cosmosis/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/attribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13893 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/declare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.550161 cosmosis-3.0.3/cosmosis/runtime/julia_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/julia_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/julia_modules/julia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/memmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17198 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/mpi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55669 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21210 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/process_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.550161 cosmosis-3.0.3/cosmosis/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.550161 cosmosis-3.0.3/cosmosis/samplers/abc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/abc/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7126 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/abc/abc_sampler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6698 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/abc/abc_sampler_mpi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.550161 cosmosis-3.0.3/cosmosis/samplers/apriori/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/apriori/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2176 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/apriori/apriori_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.550161 cosmosis-3.0.3/cosmosis/samplers/dynesty/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/dynesty/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3722 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/dynesty/dynesty_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.550161 cosmosis-3.0.3/cosmosis/samplers/emcee/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/emcee/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7516 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/emcee/emcee_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.554161 cosmosis-3.0.3/cosmosis/samplers/fisher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/fisher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/fisher/fisher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6642 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/fisher/fisher_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.554161 cosmosis-3.0.3/cosmosis/samplers/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/grid/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4745 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/grid/grid_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.554161 cosmosis-3.0.3/cosmosis/samplers/gridmax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/gridmax/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4370 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/gridmax/gridmax_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/hints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.554161 cosmosis-3.0.3/cosmosis/samplers/importance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/importance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/importance/importance_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.554161 cosmosis-3.0.3/cosmosis/samplers/kombine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/kombine/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4932 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/kombine/kombine_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.554161 cosmosis-3.0.3/cosmosis/samplers/list/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/list/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4888 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/list/list_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.554161 cosmosis-3.0.3/cosmosis/samplers/maxlike/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/maxlike/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4666 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/maxlike/maxlike_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.554161 cosmosis-3.0.3/cosmosis/samplers/metropolis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/metropolis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9773 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/metropolis/metropolis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/metropolis/metropolis_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.554161 cosmosis-3.0.3/cosmosis/samplers/metropolis/proposal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/metropolis/proposal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/metropolis/proposal/cobaya_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/metropolis/proposal/standard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.554161 cosmosis-3.0.3/cosmosis/samplers/minuit/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/minuit/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/minuit/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7323 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/minuit/minuit_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/minuit/minuit_wrapper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.554161 cosmosis-3.0.3/cosmosis/samplers/multinest/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/multinest/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/multinest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.554161 cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    19512 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/README
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/cwrapper.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    42915 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90
+-rw-r--r--   0 runner    (1001) docker     (123)   107766 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/nested.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    22010 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/posterior.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/priors.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/utils.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    28039 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/utils1.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    86938 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.558161 cosmosis-3.0.3/cosmosis/samplers/nautilus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/nautilus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/nautilus/nautilus_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.558161 cosmosis-3.0.3/cosmosis/samplers/pmaxlike/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/pmaxlike/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4151 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.558161 cosmosis-3.0.3/cosmosis/samplers/pmc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/pmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/pmc/pmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/pmc/pmc_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.558161 cosmosis-3.0.3/cosmosis/samplers/poco/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/poco/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3703 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/poco/poco_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.558161 cosmosis-3.0.3/cosmosis/samplers/polychord/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12986 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.558161 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/README
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/abort.F90
+-rw-r--r--   0 runner    (1001) docker     (123)    18110 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/array_utils.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/c_interface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/calculate.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/clustering.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    13421 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/feedback.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    26147 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/generate.F90
+-rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/ini.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    20999 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/interfaces.F90
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/interfaces.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/interfaces.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24257 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90
+-rw-r--r--   0 runner    (1001) docker     (123)    20674 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/params.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    19675 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/priors.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/random_utils.F90
+-rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/read_write.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    47427 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/run_time_info.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/settings.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    29353 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/utils.F90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.562161 cosmosis-3.0.3/cosmosis/samplers/pymc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/pymc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/pymc/pymc_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.562161 cosmosis-3.0.3/cosmosis/samplers/snake/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/snake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/snake/snake.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2017 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/snake/snake_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.562161 cosmosis-3.0.3/cosmosis/samplers/star/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/star/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4468 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/star/star_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.562161 cosmosis-3.0.3/cosmosis/samplers/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/test/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3221 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/test/test_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.562161 cosmosis-3.0.3/cosmosis/samplers/zeus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/zeus/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11554 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/zeus/zeus_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.562161 cosmosis-3.0.3/cosmosis/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/campaign.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/example-priors.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/example-values.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/example.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/example_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/example_module2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/example_module3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/example_module4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.566161 cosmosis-3.0.3/cosmosis/test/libtest/
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/c_datablock_complex_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/c_datablock_double_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/c_datablock_int_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/c_datablock_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/cosmosis_test.F90
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/cosmosis_tests.supp
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/datablock_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/entry_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/ndarray_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/section_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    28088 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/test_c_datablock_scalars.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/test_c_datablock_scalars.template
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/test_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/test_chaining.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/test_polychord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/test_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/test_text_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.542161 cosmosis-3.0.3/cosmosis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-28 18:31:33.000000 cosmosis-3.0.3/cosmosis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-07-28 18:31:33.000000 cosmosis-3.0.3/cosmosis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:31:33.000000 cosmosis-3.0.3/cosmosis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-28 18:31:33.000000 cosmosis-3.0.3/cosmosis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-28 18:31:33.000000 cosmosis-3.0.3/cosmosis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 18:31:29.000000 cosmosis-3.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 18:31:33.566161 cosmosis-3.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-07-28 18:31:29.000000 cosmosis-3.0.3/setup.py
```

### Comparing `cosmosis-3.0.1/LICENSE` & `cosmosis-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/MANIFEST.in` & `cosmosis-3.0.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/bin/cosmosis-configure` & `cosmosis-3.0.3/bin/cosmosis-configure`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/bin/cosmosis-extract` & `cosmosis-3.0.3/bin/cosmosis-extract`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/bin/cosmosis-sample-fisher` & `cosmosis-3.0.3/bin/cosmosis-sample-fisher`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/__init__.py` & `cosmosis-3.0.3/cosmosis/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/campaign.py` & `cosmosis-3.0.3/cosmosis/campaign.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/config/compilers.mk` & `cosmosis-3.0.3/cosmosis/config/compilers.mk`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/configure.py` & `cosmosis-3.0.3/cosmosis/configure.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/constants.py` & `cosmosis-3.0.3/cosmosis/constants.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/datablock/Makefile` & `cosmosis-3.0.3/cosmosis/datablock/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/datablock/c_datablock.cc` & `cosmosis-3.0.3/cosmosis/datablock/c_datablock.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/datablock/c_datablock.h` & `cosmosis-3.0.3/cosmosis/datablock/c_datablock.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/datablock/clamp.hh` & `cosmosis-3.0.3/cosmosis/datablock/clamp.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/datablock/cosmosis_constants.fh` & `cosmosis-3.0.3/cosmosis/datablock/cosmosis_constants.fh`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/datablock/cosmosis_constants.h` & `cosmosis-3.0.3/cosmosis/datablock/cosmosis_constants.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/datablock/cosmosis_modules.F90` & `cosmosis-3.0.3/cosmosis/datablock/cosmosis_modules.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/datablock/cosmosis_py/block.py` & `cosmosis-3.0.3/cosmosis/datablock/cosmosis_py/block.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/datablock/cosmosis_py/errors.py` & `cosmosis-3.0.3/cosmosis/datablock/cosmosis_py/errors.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/datablock/cosmosis_py/lib.py` & `cosmosis-3.0.3/cosmosis/datablock/cosmosis_py/lib.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/datablock/cosmosis_py/section_names.py` & `cosmosis-3.0.3/cosmosis/datablock/cosmosis_py/section_names.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/datablock/cosmosis_section_names.F90` & `cosmosis-3.0.3/cosmosis/datablock/cosmosis_section_names.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/datablock/cosmosis_wrappers.F90` & `cosmosis-3.0.3/cosmosis/datablock/cosmosis_wrappers.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/datablock/datablock.cc` & `cosmosis-3.0.3/cosmosis/datablock/datablock.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/datablock/datablock.hh` & `cosmosis-3.0.3/cosmosis/datablock/datablock.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/datablock/datablock_logging.cc` & `cosmosis-3.0.3/cosmosis/datablock/datablock_logging.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/datablock/datablock_logging.h` & `cosmosis-3.0.3/cosmosis/datablock/datablock_logging.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/datablock/datablock_status.h` & `cosmosis-3.0.3/cosmosis/datablock/datablock_status.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/datablock/entry.cc` & `cosmosis-3.0.3/cosmosis/datablock/entry.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/datablock/entry.hh` & `cosmosis-3.0.3/cosmosis/datablock/entry.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/datablock/generate_sections.py` & `cosmosis-3.0.3/cosmosis/datablock/generate_sections.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/datablock/handler.c` & `cosmosis-3.0.3/cosmosis/datablock/handler.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/datablock/ndarray.hh` & `cosmosis-3.0.3/cosmosis/datablock/ndarray.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/datablock/section.cc` & `cosmosis-3.0.3/cosmosis/datablock/section.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/datablock/section.hh` & `cosmosis-3.0.3/cosmosis/datablock/section.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/datablock/section_names.h` & `cosmosis-3.0.3/cosmosis/datablock/section_names.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/datablock/section_names.txt` & `cosmosis-3.0.3/cosmosis/datablock/section_names.txt`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/gaussian_likelihood.py` & `cosmosis-3.0.3/cosmosis/gaussian_likelihood.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/main.py` & `cosmosis-3.0.3/cosmosis/main.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/output/__init__.py` & `cosmosis-3.0.3/cosmosis/output/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/output/astropy_output.py` & `cosmosis-3.0.3/cosmosis/output/astropy_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/output/cosmomc_output.py` & `cosmosis-3.0.3/cosmosis/output/cosmomc_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/output/fits_output.py` & `cosmosis-3.0.3/cosmosis/output/fits_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/output/in_memory_output.py` & `cosmosis-3.0.3/cosmosis/output/in_memory_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/output/null_output.py` & `cosmosis-3.0.3/cosmosis/output/null_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/output/output_base.py` & `cosmosis-3.0.3/cosmosis/output/output_base.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/output/text_output.py` & `cosmosis-3.0.3/cosmosis/output/text_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/output/utils.py` & `cosmosis-3.0.3/cosmosis/output/utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/plotting/chain_plots.py` & `cosmosis-3.0.3/cosmosis/plotting/chain_plots.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/plotting/grid_plots.py` & `cosmosis-3.0.3/cosmosis/plotting/grid_plots.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/plotting/kde.py` & `cosmosis-3.0.3/cosmosis/plotting/kde.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/plotting/plotter.py` & `cosmosis-3.0.3/cosmosis/plotting/plotter.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/postprocess.py` & `cosmosis-3.0.3/cosmosis/postprocess.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/postprocessing/__init__.py` & `cosmosis-3.0.3/cosmosis/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/postprocessing/cosmology_theory_plots.py` & `cosmosis-3.0.3/cosmosis/postprocessing/cosmology_theory_plots.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/postprocessing/density.py` & `cosmosis-3.0.3/cosmosis/postprocessing/density.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/postprocessing/elements.py` & `cosmosis-3.0.3/cosmosis/postprocessing/elements.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/postprocessing/inputs.py` & `cosmosis-3.0.3/cosmosis/postprocessing/inputs.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/postprocessing/latex.ini` & `cosmosis-3.0.3/cosmosis/postprocessing/latex.ini`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/postprocessing/lazy_pylab.py` & `cosmosis-3.0.3/cosmosis/postprocessing/lazy_pylab.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/postprocessing/main.py` & `cosmosis-3.0.3/cosmosis/postprocessing/main.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/postprocessing/outputs.py` & `cosmosis-3.0.3/cosmosis/postprocessing/outputs.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/postprocessing/plots.py` & `cosmosis-3.0.3/cosmosis/postprocessing/plots.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/postprocessing/postprocess.py` & `cosmosis-3.0.3/cosmosis/postprocessing/postprocess.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/postprocessing/postprocess_base.py` & `cosmosis-3.0.3/cosmosis/postprocessing/postprocess_base.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/postprocessing/reruns.py` & `cosmosis-3.0.3/cosmosis/postprocessing/reruns.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/postprocessing/statistics.py` & `cosmosis-3.0.3/cosmosis/postprocessing/statistics.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/postprocessing/utils.py` & `cosmosis-3.0.3/cosmosis/postprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/runtime/analytics.py` & `cosmosis-3.0.3/cosmosis/runtime/analytics.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/runtime/attribution.py` & `cosmosis-3.0.3/cosmosis/runtime/attribution.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/runtime/config.py` & `cosmosis-3.0.3/cosmosis/runtime/config.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/runtime/declare.py` & `cosmosis-3.0.3/cosmosis/runtime/declare.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/runtime/julia_modules/julia.py` & `cosmosis-3.0.3/cosmosis/runtime/julia_modules/julia.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/runtime/logs.py` & `cosmosis-3.0.3/cosmosis/runtime/logs.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/runtime/memmon.py` & `cosmosis-3.0.3/cosmosis/runtime/memmon.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/runtime/module.py` & `cosmosis-3.0.3/cosmosis/runtime/module.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/runtime/mpi_pool.py` & `cosmosis-3.0.3/cosmosis/runtime/mpi_pool.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/runtime/parameter.py` & `cosmosis-3.0.3/cosmosis/runtime/parameter.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/runtime/pipeline.py` & `cosmosis-3.0.3/cosmosis/runtime/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -1264,19 +1264,19 @@
         for _,key in data.keys(section_names.likelihoods):
             if key.endswith("_like"):
                 name = key[:-5]
                 likelihood_names.append(name)
         self.likelihood_names = likelihood_names
 
         # Tell the user what we found.
-        print("Using likelihooods from first run:")
+        logs.overview("Using likelihooods from first run:")
         for name in self.likelihood_names:
-            print(f" - {name}")
+            logs.overview(f" - {name}")
         if not self.likelihood_names:
-            print(" - (None found)")
+            logs.overview(" - (None found)")
 
     def _extract_likelihoods(self, data):
         "Extract the likelihoods from the block"
 
         section_name = section_names.likelihoods
 
         # loop through named likelihoods and sum their values
```

### Comparing `cosmosis-3.0.1/cosmosis/runtime/prior.py` & `cosmosis-3.0.3/cosmosis/runtime/prior.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/runtime/process_pool.py` & `cosmosis-3.0.3/cosmosis/runtime/process_pool.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/__init__.py` & `cosmosis-3.0.3/cosmosis/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/abc/abc_sampler.py` & `cosmosis-3.0.3/cosmosis/samplers/abc/abc_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/abc/abc_sampler_mpi.py` & `cosmosis-3.0.3/cosmosis/samplers/abc/abc_sampler_mpi.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/apriori/apriori_sampler.py` & `cosmosis-3.0.3/cosmosis/samplers/apriori/apriori_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/dynesty/dynesty_sampler.py` & `cosmosis-3.0.3/cosmosis/samplers/dynesty/dynesty_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/emcee/emcee_sampler.py` & `cosmosis-3.0.3/cosmosis/samplers/emcee/emcee_sampler.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,24 +42,24 @@
             #Starting positions and values for the chain
             self.num_samples = 0
             self.prob0 = None
             self.blob0 = None
 
             if start_file:
                 self.p0 = self.load_start(start_file)
-                print("Loaded starting position from %s", start_file)
+                logs.overview(f"Loaded starting position from {start_file}")
             elif self.distribution_hints.has_cov():
                 center = self.start_estimate()
                 cov = self.distribution_hints.get_cov()
                 self.p0 = sample_ellipsoid(center, cov, size=self.nwalkers)
-                print("Generating starting positions from covmat from earlier in pipeline")
+                logs.overview("Generating starting positions from covmat from earlier in pipeline")
             elif covmat_file:
                 center = self.start_estimate()
                 cov = self.load_covmat(covmat_file)
-                print("Generating starting position from covmat in  %s", covmat_file)
+                logs.overview(f"Generating starting position from covmat in  {covmat_file}")
                 iterations_limit = 100000
                 n=0
                 p0 = []
                 for i in range(iterations_limit):
                     p = sample_ellipsoid(center, cov)[0]
                     if np.isfinite(self.pipeline.prior(p)):
                         p0.append(p)
@@ -67,23 +67,23 @@
                         break
                 else:
                     raise ValueError("The covmat you used could not generate points inside the prior")
                 self.p0 = np.array(p0)
             elif random_start:
                 self.p0 = [self.pipeline.randomized_start()
                            for i in range(self.nwalkers)]
-                print("Generating random starting positions from within prior")
+                logs.overview("Generating random starting positions from within prior")
             else:
                 center_norm = self.pipeline.normalize_vector(self.start_estimate())
                 sigma_norm=np.repeat(1e-3, center_norm.size)
                 p0_norm = sample_ball(center_norm, sigma_norm, size=self.nwalkers)
                 p0_norm[p0_norm<=0] = 0.001
                 p0_norm[p0_norm>=1] = 0.999
                 self.p0 = [self.pipeline.denormalize_vector(p0_norm_i) for p0_norm_i in p0_norm]
-                print("Generating starting positions in small ball around starting point")
+                logs.overview("Generating starting positions in small ball around starting point")
 
             if self.emcee_version < 3:
                 kw = {"a": self.a}
             else:
                 kw = {"moves": [(emcee.moves.StretchMove(a=self.a), 1.0)]}
 
             #Finally we can create the sampler
@@ -94,18 +94,18 @@
     def resume(self):
         if self.output.resumed:
             data = np.genfromtxt(self.output._filename, invalid_raise=False)[:, :self.ndim]
             num_samples = len(data) // self.nwalkers
             self.p0 = data[-self.nwalkers:]
             self.num_samples += num_samples
             if self.num_samples >= self.samples:
-                print("You told me to resume the chain - it has already completed (with {} samples), so sampling will end.".format(len(data)))
-                print("Increase the 'samples' parameter to keep going.")
+                logs.error("You told me to resume the chain - it has already completed (with {} samples), so sampling will end.".format(len(data)))
+                logs.error("Increase the 'samples' parameter to keep going.")
             else:
-                print("Continuing emcee from existing chain - have {} samples already".format(len(data)))
+                logs.overview("Continuing emcee from existing chain - have {} samples already".format(len(data)))
 
     def load_start(self, filename):
         #Load the data and cut to the bits we need.
         #This means you can either just use a test file with
         #starting points, or an emcee output file.
         data = np.genfromtxt(filename, invalid_raise=False)[-self.nwalkers:, :self.ndim]
         if data.shape != (self.nwalkers, self.ndim):
@@ -134,15 +134,15 @@
         for params, post, extra in zip(pos,prob,extra_info):
             prior, extra = extra      
             self.output.parameters(params, extra, prior, post)
 
     def execute(self):
         #Run the emcee sampler.
         if self.num_samples == 0:
-            print("Begun sampling")
+            logs.overview("Begun sampling")
         outputs = []
         if self.emcee_version < 3:
             kwargs = dict(lnprob0=self.prob0, blobs0=self.blob0, 
                           iterations=self.nsteps, storechain=False)
         else:
             # In emcee3 we have to enable storing the chain because
             # we want the acceptance fraction.  Also the name of one
```

### Comparing `cosmosis-3.0.1/cosmosis/samplers/fisher/fisher.py` & `cosmosis-3.0.3/cosmosis/samplers/fisher/fisher.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/fisher/fisher_sampler.py` & `cosmosis-3.0.3/cosmosis/samplers/fisher/fisher_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,16 +68,16 @@
         self.tolerance = self.read_ini("tolerance", float, 0.01)
         self.maxiter = self.read_ini("maxiter", int, 10)
         self.use_numdifftools = self.read_ini("use_numdifftools", bool, False)
 
         if self.output:
             for p in self.pipeline.extra_saves:
                 name = '%s--%s'%p
-                print("NOTE: You set extra_output to include parameter %s in the parameter file" % name)
-                print("      But the Fisher Sampler cannot do that, so this will be ignored.")
+                logs.warning("NOTE: You set extra_output to include parameter %s in the parameter file" % name)
+                logs.warning("      But the Fisher Sampler cannot do that, so this will be ignored.")
                 self.output.del_column(name)
 
         self.converged = False
 
     def compute_prior_matrix(self):
         #We include the priors as an additional matrix term
         #This is just added to the fisher matrix
@@ -88,15 +88,14 @@
                 logs.important("Applying additional prior sigma = {0} to {1}".format(param.prior.sigma, param))
                 logs.important("This will be assumed to be centered at the parameter center regardless of what the ini file says")
                 logs.important("The limits of the parameter will also not be respected.") 
                 P[i,i] = 1./param.prior.sigma**2
             elif isinstance(param.prior, prior.ExponentialPrior) or isinstance(param.prior, prior.TruncatedExponentialPrior):
                 logs.important("There is an exponential prior applied to parameter {0}".format(param))
                 logs.important("This is *not* accounted for in the Fisher matrix")
-                print()
             #uniform prior should have no effect on the fisher matrix.
             #at least up until the assumptions of the FM are violated anyway
         return P
```

### Comparing `cosmosis-3.0.1/cosmosis/samplers/grid/grid_sampler.py` & `cosmosis-3.0.3/cosmosis/samplers/grid/grid_sampler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import itertools
 import numpy as np
-
+from ... runtime import logs
 from .. import ParallelSampler
 
 
 def task(p):
     i,p = p
     results = grid_sampler.pipeline.run_results(p)
     #If requested, save the data to file
@@ -47,24 +47,24 @@
                 self.nstep = self.nsample
 
 
         #Also Generate the complete collection of parameter sets to run over.
         #This doesn't actually keep them all in memory, it is just the conceptual
         #outer product
         total_samples = self.nsample**len(self.pipeline.varied_params)
-        print("Total number of grid samples: ", total_samples)
+        logs.overview(f"Total number of grid samples: {total_samples}")
 
         if total_samples>LARGE_JOB_SIZE:
-            print("That is a very large number of samples.")
+            logs.error("That is a very large number of samples.")
             if self.allow_large:
-                print("But you set allow_large=T so I will continue")
+                logs.error("But you set allow_large=T so I will continue")
             else:
-                print("This is suspicously large so I am going to stop")
-                print("If you really want to do this set allow_large=T in the")
-                print("[grid] section of the ini file.")
+                logs.error("This is suspicously large so I am going to stop")
+                logs.error("If you really want to do this set allow_large=T in the")
+                logs.error("[grid] section of the ini file.")
                 raise ValueError("Suspicously large number of grid points %d ( = n_samp ^ n_dim = %d ^ %d); set allow_large=T in [grid] section to permit this."%(total_samples,self.nsample,len(self.pipeline.varied_params)))
         
         # If our pipeline allows it we arrange it so that the
         # fast parameters change fastest in the sequence.
         # This is still not optimal for the multiprocessing case
         if self.pipeline.do_fast_slow:
             param_order = self.pipeline.slow_params + self.pipeline.fast_params
```

### Comparing `cosmosis-3.0.1/cosmosis/samplers/gridmax/gridmax_sampler.py` & `cosmosis-3.0.3/cosmosis/samplers/gridmax/gridmax_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/hints.py` & `cosmosis-3.0.3/cosmosis/samplers/hints.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/importance/importance_sampler.py` & `cosmosis-3.0.3/cosmosis/samplers/importance/importance_sampler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import itertools
 import collections
 import numpy as np
+from ...runtime import logs
 
 from .. import ParallelSampler
 
 
 INI_SECTION = "importance"
 
 
@@ -47,45 +48,45 @@
         #   - one that are fixed - WHAT SHOULD WE DO ABOUT THESE???
         #   - extras ones - these should be saved and put in the output
 
         self.original_extras = collections.OrderedDict()
         self.samples = []
         self.varied_params = []
         self.number_samples = len(cols[0])
-        print("Have %d samples from old chain." % self.number_samples)
+        logs.overview("Have %d samples from old chain." % self.number_samples)
         for code,col in zip(col_names, cols[0].T):
             #we have already handled the likelihood
             if code=='post':continue
             #parse the header names in to (section,name)
             bits = code.split("--")
             if len(bits)==2:
                 section, name = bits
                 #No parameter should be varied in the old chain
                 #but listed as fixed here
                 if (section,name) in self.pipeline.fixed_params:
-                    print("WARNING: %s varied in old chain now fixed.  I will fix it <--------- Read this warning." % name)
+                    logs.error("WARNING: %s varied in old chain now fixed.  I will fix it <--------- Read this warning." % name)
                 elif (section,name) in self.pipeline.varied_params:
                     #Record the values of this parameter for later importance
                     #sampling
-                    print("Found column in both pipelines:", code)
+                    logs.overview(f"Found column in both pipelines {code}:")
                     self.samples.append(col)
                     self.varied_params.append(bits)
                 else:
-                    print("Found column just in old pipeline:", code)
+                    logs.overview(f"Found column just in old pipeline: {code}")
                     #This parameter was varied in the old code but is not
                     #here.  So we just save it for output
                     self.original_extras[code] = col
                     self.output.add_column(code, float)
             # anything here must be a sampler-specific 
             else:
-                print("Found non-parameter column:", code)
+                logs.overview(f"Found non-parameter column: {code}")
                 self.original_extras[code] = col
                 if code=="weight":
                     code="old_weight"
-                    print("Renaming weight -> old_weight")
+                    logs.overview("Renaming weight -> old_weight")
                 self.output.add_column(code, float)
 
         #Now finally add our actual two sampler outputs, old_like and like
         #P is the original likelihood in the old chain we have samples from
         #P' is the new likelihood.
         self.output.add_column("old_post", float) #This is the old likelihood, log(P)
         self.output.add_column("log_weight", float) #This is the log-weight, the ratio of the likelihoods
```

### Comparing `cosmosis-3.0.1/cosmosis/samplers/kombine/kombine_sampler.py` & `cosmosis-3.0.3/cosmosis/samplers/kombine/kombine_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/list/list_sampler.py` & `cosmosis-3.0.3/cosmosis/samplers/list/list_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/maxlike/maxlike_sampler.py` & `cosmosis-3.0.3/cosmosis/samplers/maxlike/maxlike_sampler.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,26 +11,26 @@
         self.maxiter = self.read_ini("maxiter", int, 1000)
         self.output_ini = self.read_ini("output_ini", str, "")
         self.output_cov = self.read_ini("output_covmat", str, "")
         self.method = self.read_ini("method",str,"Nelder-Mead")
         self.max_posterior = self.read_ini("max_posterior", bool, False)
 
         if self.max_posterior:
-            print("------------------------------------------------")
-            print("NOTE: Running optimizer in **max-posterior** mode:")
-            print("NOTE: Will maximize the combined likelihood and prior")
-            print("------------------------------------------------")
+            logs.overview("------------------------------------------------")
+            logs.overview("NOTE: Running optimizer in **max-posterior** mode:")
+            logs.overview("NOTE: Will maximize the combined likelihood and prior")
+            logs.overview("------------------------------------------------")
         else:
-            print("--------------------------------------------------")
-            print("NOTE: Running optimizer in **max-like** mode:")
-            print("NOTE: not including the prior, just the likelihood.")
-            print("NOTE: Set the parameter max_posterior=T to change this.")
-            print("NOTE: This won't matter unless you set some non-flat")
-            print("NOTE: priors in a separate priors file.")
-            print("--------------------------------------------------")
+            logs.overview("--------------------------------------------------")
+            logs.overview("NOTE: Running optimizer in **max-like** mode:")
+            logs.overview("NOTE: not including the prior, just the likelihood.")
+            logs.overview("NOTE: Set the parameter max_posterior=T to change this.")
+            logs.overview("NOTE: This won't matter unless you set some non-flat")
+            logs.overview("NOTE: priors in a separate priors file.")
+            logs.overview("--------------------------------------------------")
 
         self.converged = False
 
     def execute(self):
         import scipy.optimize
 
         def likefn(p_in):
```

### Comparing `cosmosis-3.0.1/cosmosis/samplers/metropolis/metropolis.py` & `cosmosis-3.0.3/cosmosis/samplers/metropolis/metropolis.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,15 +228,15 @@
         else:
             logs.warning("Cov estimate not SPD.  If this keeps happening, be concerned.")
 
 
     def set_fast_slow(self, fast_indices, slow_indices, oversampling):
         if self.n_drag:
             oversampling = 1
-            print("Overriding oversampling parameter -> 1 since using dragging")
+            logs.noisy("Overriding oversampling parameter -> 1 since using dragging")
         self.fast_indices = fast_indices
         self.slow_indices = slow_indices
         self.oversampling = oversampling
         self.fast_slow_is_ready = True
 
         if self.use_cobaya:
             from .proposal import cobaya_proposal
```

### Comparing `cosmosis-3.0.1/cosmosis/samplers/metropolis/metropolis_sampler.py` & `cosmosis-3.0.3/cosmosis/samplers/metropolis/metropolis_sampler.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,38 +49,38 @@
         #Any other options go here
 
         # if we are not tunning then there is no tuning phase
         if tuning_frequency == -1:
             self.tuning_end = 0
 
         if (self.drag > 0) and not self.pipeline.do_fast_slow:
-            print("You asked for dragging, but the pipeline does not have fast/slow enabled"
+            logs.warning("You asked for dragging, but the pipeline does not have fast/slow enabled"
                   ", so no draggng will be done."
                 )
 
         if (self.pipeline.do_fast_slow) and not (self.pipeline.first_fast_module):
             raise ValueError("To use fast/slow splitting with metropolis please "
                              "manually define first_fast_module in the pipeline "
                              "section.")
 
 
         #Covariance matrix
         covmat = self.load_covariance_matrix()
 
         #start values from prior
         start = self.define_parameters(random_start, covmat_sample_start, covmat)
-        print("MCMC starting point:")
+        logs.overview("MCMC starting point:")
         for param, x in zip(self.pipeline.varied_params, start):
-            print("    ", param, x)
+            logs.overview(f"    {param}  {x}")
 
 
         if use_cobaya:
-            print("Using the Cobaya proposal")
+            logs.overview("Using the Cobaya proposal")
 
-        print(f"Will tune every {tuning_frequency} samples, from samples "
+        logs.overview(f"Will tune every {tuning_frequency} samples, from samples "
               f"{tuning_grace} to {self.tuning_end}.")
 
         self.sampler = metropolis.MCMC(start, posterior, covmat,
             tuning_frequency=tuning_frequency, # Will be multiplied by the oversampling
             tuning_grace=tuning_grace,         # within the sampler if needed
             tuning_end=self.tuning_end,
             exponential_probability=self.exponential_probability,
@@ -113,22 +113,22 @@
             data = np.genfromtxt(self.output._filename, invalid_raise=False)[:, :self.ndim]
             self.analytics.add_traces(data)
         except IndexError:
             data = None
 
         
         if self.num_samples >= self.samples:
-            print("You told me to resume the chain - it has already completed (with {} samples), so sampling will end.".format(len(data)))
-            print("Increase the 'samples' parameter to keep going.")
+            logs.important("You told me to resume the chain - it has already completed (with {} samples), so sampling will end.".format(len(data)))
+            logs.important("Increase the 'samples' parameter to keep going.")
         elif self.is_converged():
-            print("The resumed chain was already converged.  You can change the converged testing parameters to extend it.")
+            logs.overview("The resumed chain was already converged.  You can change the converged testing parameters to extend it.")
         elif data is None:
-            print("Continuing metropolis from existing chain - you were in the tuning phase, which will continue")
+            logs.overview("Continuing metropolis from existing chain - you were in the tuning phase, which will continue")
         else:
-            print("Continuing metropolis from existing chain - have {} samples already".format(len(data)))
+            logs.overview("Continuing metropolis from existing chain - have {} samples already".format(len(data)))
 
 
 
 
 
 
     def execute(self):
@@ -176,15 +176,16 @@
         self.write_resume_info([self.sampler, self.num_samples, self.num_samples_post_tuning])
 
     def is_converged(self):
          # user has pressed Ctrl-C
         if self.interrupted:
             return True
         if self.num_samples >= self.samples:
-            print("Full number of samples generated; sampling complete")
+            rank = self.pool.rank if self.pool is not None else 0
+            logs.overview(f"Rank {rank}: Full number of samples generated; sampling complete")
             return True
         elif (self.num_samples > 0 and
               self.pool is not None and
               self.Rconverge is not None and
               self.num_samples_post_tuning > 0):
             R = self.analytics.gelman_rubin()
             R1 = abs(R - 1)
@@ -193,24 +194,24 @@
             return False
 
 
 
     def load_covariance_matrix(self):
         covmat_filename = self.read_ini("covmat", str, "").strip()
         if covmat_filename == "" and self.distribution_hints.has_cov():
-                covmat =  self.distribution_hints.get_cov() 
-                print("Using covariance from previous sampler")
+                covmat =  self.distribution_hints.get_cov()
+                logs.overview("Using covariance from previous sampler")
         elif covmat_filename == "":
-            print("Using default covariance 1% of param widths")
+            logs.overview("Using default covariance 1% of param widths")
             covmat = np.array([p.width()/100.0 for p in self.pipeline.varied_params])
         elif not os.path.exists(covmat_filename):
             raise ValueError(
             "Covariance matrix %s not found" % covmat_filename)
         else:
-            print("Loading covariance from {}".format(covmat_filename))
+            logs.overview("Loading covariance from {}".format(covmat_filename))
             covmat = np.loadtxt(covmat_filename)
 
         if covmat.ndim == 0:
             covmat = covmat.reshape((1, 1))
         elif covmat.ndim == 1:
             covmat = np.diag(covmat ** 2)
```

### Comparing `cosmosis-3.0.1/cosmosis/samplers/metropolis/proposal/cobaya_proposal.py` & `cosmosis-3.0.3/cosmosis/samplers/metropolis/proposal/cobaya_proposal.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/metropolis/proposal/standard.py` & `cosmosis-3.0.3/cosmosis/samplers/metropolis/proposal/standard.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/minuit/Makefile` & `cosmosis-3.0.3/cosmosis/samplers/minuit/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/minuit/minuit_sampler.py` & `cosmosis-3.0.3/cosmosis/samplers/minuit/minuit_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,23 +139,22 @@
 
         if self.output_ini:
             self.pipeline.create_ini(param_vector, self.output_ini)
 
         for name, value in zip(param_names, param_vector):
             sec,name=name.split('--')
             if section!=sec:
-                print()
-                print("[%s]" % sec)
+                logs.important("[%s]" % sec)
                 section=sec
-            print("%s = %g" % (name,value))
-        print()
-        print("Likelihood = ", results.like)
+            logs.important("%s = %g" % (name,value))
+
+        logs.important(f"Likelihood = {results.like}")
 
         if self.save_dir:
-            print("Saving best-fit model cosmology to ", self.save_dir)
+            logs.overview(f"Saving best-fit model cosmology to {self.save_dir}")
             results.block.save_to_directory(self.save_dir, clobber=True)
 
         self.converged = True
 
     def sample(self):
 
         param_names = [str(p) for p in self.pipeline.varied_params]
```

### Comparing `cosmosis-3.0.1/cosmosis/samplers/minuit/minuit_wrapper.cpp` & `cosmosis-3.0.3/cosmosis/samplers/minuit/minuit_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_sampler.py` & `cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,17 +136,17 @@
             try:
                 P = p.split('--')
             except ValueError:
                 raise ValueError("You included {} in wrapped_params mulitnest option but should be format: section--name".format(p))
             if P in self.pipeline.varied_params:
                 index = self.pipeline.varied_params.index(P)
                 self.wrapping[index] = 1
-                print("MULTINEST: Parameter {} ({}) will be wrapped around the edge of its prior".format(index,p))
+                logs.overview("MULTINEST: Parameter {} ({}) will be wrapped around the edge of its prior".format(index,p))
             elif P in self.pipeline.parameters:
-                print("MULTINEST NOTE: You asked for wrapped sampling on {}. That parameter is not varied in this pipeline, so this will have no effect.".format(p))
+                logs.warnings("MULTINEST NOTE: You asked for wrapped sampling on {}. That parameter is not varied in this pipeline, so this will have no effect.".format(p))
             else:
                 raise ValueError("You asked for an unknown parameter, {} to be wrapped around in the multinest wrapped_params option.".format(p))
 
 
 
         if self.output:
             def dumper(nsample, nlive, nparam, live, post, paramConstr, max_log_like, logz, ins_logz, log_z_err, context):
```

### Comparing `cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/LICENCE` & `cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/LICENCE`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/Makefile` & `cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/README` & `cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/README`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/cwrapper.f90` & `cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/cwrapper.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90` & `cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/nested.f90` & `cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/nested.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/posterior.f90` & `cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/posterior.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/priors.f90` & `cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/priors.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/utils.f90` & `cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/utils.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/utils1.f90` & `cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/utils1.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90` & `cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/nautilus/nautilus_sampler.py` & `cosmosis-3.0.3/cosmosis/samplers/nautilus/nautilus_sampler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .. import ParallelSampler
+from ...runtime import logs
 import numpy as np
 import os
 
 
 def log_probability_function(p):
     r = pipeline.run_results(p)
     out = [r.like, r.prior]
@@ -63,15 +64,16 @@
             resume_filepath = self.output.name_for_sampler_resume_info()
         except NotImplementedError:
             resume_filepath = None
 
         if resume_filepath is not None:
             resume_filepath = resume_filepath + ".hdf5"
             if self.resume_ and os.path.exists(resume_filepath):
-                print(f"Resuming Nautilus from file {resume_filepath}")
+                if self.is_master():
+                    logs.overview(f"Resuming Nautilus from file {resume_filepath}")
 
         sampler = Sampler(
             prior_transform,
             log_probability_function,
             n_dim,
             n_live=self.n_live,
             n_update=self.n_update,
```

### Comparing `cosmosis-3.0.1/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py` & `cosmosis-3.0.3/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/pmc/pmc.py` & `cosmosis-3.0.3/cosmosis/samplers/pmc/pmc.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/pmc/pmc_sampler.py` & `cosmosis-3.0.3/cosmosis/samplers/pmc/pmc_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/poco/poco_sampler.py` & `cosmosis-3.0.3/cosmosis/samplers/poco/poco_sampler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .. import ParallelSampler
+from ...runtime import logs
 import numpy as np
 
 
 def log_likelihood(p):
     like, _ = pipeline.likelihood(p)
     # PocoMC cannot cope with infinities
     if not np.isfinite(like):
@@ -47,15 +48,15 @@
             # Starting positions and values for the chain
             self.num_samples = 0
             self.prob0 = None
 
             self.p0 = np.array(
                 [self.pipeline.randomized_start() for i in range(self.nparticles)]
             )
-            print(
+            logs.overview(
                 "Generating random starting positions from within prior"
             )
 
             bounds = np.array([p.limits for p in self.pipeline.varied_params])
 
             # Finally we can create the sampler
             self.sampler = self.pocomc.Sampler(
@@ -75,15 +76,15 @@
                 bounds=bounds,
             )
 
             self.converged = False
 
             for sec, name in pipeline.extra_saves:
                 col = "{}--{}".format(sec, name)
-                print(
+                logs.warning(
                     "WARNING: POCO DOES NOT SUPPORT DERIVED PARAMS - NOT SAVING {}".format(
                         col
                     )
                 )
                 self.output.del_column(col)
 
     def execute(self):
```

### Comparing `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_sampler.py` & `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,37 +212,37 @@
 
         self.output.final("log_z", self.log_z)
         self.output.final("log_z_error", self.log_z_err)
 
     def sample(self):
 
         if self.pipeline.do_fast_slow and (self.pipeline.n_fast_params > 0):
-            print("Using two grades of parameter speed in polychord.")
+            logs.overview("Using two grades of parameter speed in polychord.")
             n_grade = 2
         elif self.pipeline.do_fast_slow:
-            print("You asked for fast/slow, but there were no fast parameters, so "
+            logs.warning("You asked for fast/slow, but there were no fast parameters, so "
                   "I have switched off Polychord's fast/slow mechanism to avoid a hang")
             n_grade = 1
         else:
-            print("Using a single grade of parameter speeds in polychord.")
+            logs.overview("Using a single grade of parameter speeds in polychord.")
             n_grade = 1
 
         grade_dims = (ct.c_int*n_grade)()
         grade_frac = (ct.c_double*n_grade)()
 
 
         if n_grade > 1:
             if self.pipeline.n_slow_params == 0:
                 raise ValueError("All your parameters have been classified as fast.  This will now work in polychord.  Change your fast/slow settings.")
 
             grade_dims[0] = self.pipeline.n_slow_params
             grade_dims[1] = self.pipeline.n_fast_params
             grade_frac[0] = 1 - self.fast_fraction
             grade_frac[1] = self.fast_fraction
-            print("Telling Polychord to spend fraction {} if its time in the fast subspace (adjust with fast_fraction option)".format(self.fast_fraction))
+            logs.overview("Telling Polychord to spend fraction {} if its time in the fast subspace (adjust with fast_fraction option)".format(self.fast_fraction))
         else:
             grade_dims[0] = self.pipeline.nvaried
             grade_frac[0] = 1.0
 
 
         n_nlives = 0
         loglikes = (ct.c_double*n_nlives)()
@@ -254,18 +254,18 @@
 
         if output_to_file:
             mkdir(self.base_dir)
             mkdir(os.path.join(self.base_dir, "clusters"))
             
         if self.num_repeats == 0:
             num_repeats = 3 * grade_dims[0]
-            print("Polychord num_repeats = {}  (3 * n_slow_params [{}])".format(num_repeats, grade_dims[0]))
+            logs.overview("Polychord num_repeats = {}  (3 * n_slow_params [{}])".format(num_repeats, grade_dims[0]))
         else:
             num_repeats = self.num_repeats
-            print("Polychord num_repeats = {}  (from parameter file)".format(num_repeats))
+            logs.overview("Polychord num_repeats = {}  (from parameter file)".format(num_repeats))
 
         self._run(
                 self.wrapped_likelihood,      #loglike,
                 self.wrapped_prior,           #prior,
                 self.wrapped_output_logger,   #dumper,
                 self.live_points,             #nlive
                 num_repeats,                  #nrepeats
```

### Comparing `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/LICENCE` & `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/LICENCE`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/Makefile` & `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/README` & `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/README`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/abort.F90` & `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/abort.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/array_utils.f90` & `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/array_utils.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/c_interface.cpp` & `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/c_interface.cpp`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/calculate.f90` & `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/calculate.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90` & `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/clustering.f90` & `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/clustering.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/feedback.f90` & `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/feedback.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/generate.F90` & `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/generate.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/ini.f90` & `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/ini.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/interfaces.F90` & `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/interfaces.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/interfaces.h` & `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/interfaces.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/interfaces.hpp` & `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/interfaces.hpp`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90` & `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90` & `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/params.f90` & `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/params.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/priors.f90` & `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/priors.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/random_utils.F90` & `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/random_utils.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/read_write.f90` & `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/read_write.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/run_time_info.f90` & `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/run_time_info.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/settings.f90` & `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/settings.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/polychord/polychord_src/utils.F90` & `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/utils.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/pymc/pymc_sampler.py` & `cosmosis-3.0.3/cosmosis/samplers/pymc/pymc_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/sampler.py` & `cosmosis-3.0.3/cosmosis/samplers/sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/snake/snake.py` & `cosmosis-3.0.3/cosmosis/samplers/snake/snake.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/snake/snake_sampler.py` & `cosmosis-3.0.3/cosmosis/samplers/snake/snake_sampler.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             except ValueError:
                 logs.noisy("The snake is trying to escape its bounds!")
 
 
 
     def is_converged(self):
         if self.snake.converged():
-            print("Snake has converged!")
-            print("Best post = %f    Best surface point = %f" %(self.snake.best_like_ever, self.snake.best_fit_like))
+            logs.overview("Snake has converged!")
+            logs.overview("Best post = %f    Best surface point = %f" %(self.snake.best_like_ever, self.snake.best_fit_like))
             return True
         if self.snake.iterations > self.maxiter:
-            print("Run out of iterations.")
-            print("Done %d, max allowed %d" % (self.snake.iterations, self.maxiter))
+            logs.warning("Run out of iterations.")
+            logs.warning("Done %d, max allowed %d" % (self.snake.iterations, self.maxiter))
             return True
         return False
```

### Comparing `cosmosis-3.0.1/cosmosis/samplers/star/star_sampler.py` & `cosmosis-3.0.3/cosmosis/samplers/star/star_sampler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import itertools
 import numpy as np
-
+from ...runtime import logs
 from .. import ParallelSampler
 
 
 def task(p):
     i,p = p
     results = star_sampler.pipeline.run_results(p)
     #If requested, save the data to file
@@ -51,27 +51,27 @@
                 self.output.metadata("fid_{0}".format(name), value)
 
 
         #Also Generate the complete collection of parameter sets to run over.
         #This doesn't actually keep them all in memory, it is just the conceptual
         #outer product
         total_samples = self.nsample*len(self.pipeline.varied_params)
-        print()
-        print("Total number of star samples: ", total_samples)
+
+        logs.overview(f"Total number of star samples: {total_samples}")
 
         if total_samples>LARGE_JOB_SIZE:
-            print("That is a very large number of samples.")
+            logs.overview("That is a very large number of samples.")
             if self.allow_large:
-                print("But you set allow_large=T so I will continue")
+                logs.overview("But you set allow_large=T so I will continue")
             else:
-                print("This is suspicously large so I am going to stop")
-                print("If you really want to do this set allow_large=T in the")
-                print("[star] section of the ini file.")
+                logs.overview("This is suspicously large so I am going to stop")
+                logs.overview("If you really want to do this set allow_large=T in the")
+                logs.overview("[star] section of the ini file.")
                 raise ValueError("Suspicously large number of star points %d ( = n_samp * n_dim = %d * %d); set allow_large=T in [star] section to permit this."%(total_samples,self.nsample,len(self.pipeline.varied_params)))
-        print()
+
         
 
         sample_points = []
         start = self.pipeline.start_vector()
         for i,param in enumerate(self.pipeline.varied_params):
             for p in np.linspace(*param.limits, num=self.nsample):
                 v = start.copy()
```

### Comparing `cosmosis-3.0.1/cosmosis/samplers/test/test_sampler.py` & `cosmosis-3.0.3/cosmosis/samplers/test/test_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/samplers/zeus/zeus_sampler.py` & `cosmosis-3.0.3/cosmosis/samplers/zeus/zeus_sampler.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,16 +63,16 @@
                     move_name, move_weight = move.split(':')
                 else:
                     move_name = move
                     move_weight = 1.0
                 move_cls = move_names[move_name]
                 self.moves.append((move_cls(), move_weight))
 
-            print("Running zeus with moves:")
-            print(self.moves)
+            logs.overview("Running zeus with moves:")
+            logs.overview(str(self.moves))
 
             # Other zeus options
             self.tune = self.read_ini("tune", bool, True)
             self.tolerance = self.read_ini("tolerance", float, 0.05)
             self.maxsteps = self.read_ini("maxsteps", int, 10000)
             self.patience = self.read_ini("patience", int, 5)
             self.maxiter = self.read_ini("maxiter", int, 10000)
@@ -82,24 +82,24 @@
             self.num_samples = 0
             self.prob0 = None
             self.blob0 = None
 
             # Generate starting point
             if start_file:
                 self.p0 = self.load_start(start_file)
-                print("Loaded starting position from %s", start_file)
+                logs.overview(f"Loaded starting position from {start_file}")
             elif self.distribution_hints.has_cov():
                 center = self.start_estimate()
                 cov = self.distribution_hints.get_cov()
                 self.p0 = sample_ellipsoid(center, cov, size=self.nwalkers)
-                print("Generating starting positions from covmat from earlier in pipeline")
+                logs.overview("Generating starting positions from covmat from earlier in pipeline")
             elif covmat_file:
                 center = self.start_estimate()
                 cov = self.load_covmat(covmat_file)
-                print("Generating starting position from covmat in  %s", covmat_file)
+                logs.overview(f"Generating starting position from covmat in  {covmat_file}")
                 iterations_limit = 100000
                 n=0
                 p0 = []
                 for i in range(iterations_limit):
                     p = sample_ellipsoid(center, cov)[0]
                     if np.isfinite(self.pipeline.prior(p)):
                         p0.append(p)
@@ -107,23 +107,23 @@
                         break
                 else:
                     raise ValueError("The covmat you used could not generate points inside the prior")
                 self.p0 = np.array(p0)
             elif random_start:
                 self.p0 = [self.pipeline.randomized_start()
                            for i in range(self.nwalkers)]
-                print("Generating random starting positions from within prior")
+                logs.overview("Generating random starting positions from within prior")
             else:
                 center_norm = self.pipeline.normalize_vector(self.start_estimate())
                 sigma_norm=np.repeat(1e-3, center_norm.size)
                 p0_norm = sample_ball(center_norm, sigma_norm, size=self.nwalkers)
                 p0_norm[p0_norm<=0] = 0.001
                 p0_norm[p0_norm>=1] = 0.999
                 self.p0 = [self.pipeline.denormalize_vector(p0_norm_i) for p0_norm_i in p0_norm]
-                print("Generating starting positions in small ball around starting point")
+                logs.overview("Generating starting positions in small ball around starting point")
 
             #Finally we can create the sampler
             self.started = False
             self.sampler = self.zeus.EnsembleSampler(self.nwalkers, self.ndim,
                                                      log_probability_function,
                                                      tune=self.tune,
                                                      tolerance=self.tolerance,
@@ -155,40 +155,40 @@
                 "the Move objects since re-running this chain. "
                 "You can't directly resume a chain with different moves, "
                 "so either: (a) change them back (to {}), "
                 "(b) delete the sample_status output file, "
                 "(c) switch off runtime.resume.  If you just want to restart the "
                 "walkers from old positions, set zeus.start_points")
 
-        print("Loaded 'Move' objects from resume file:")
+        logs.overview("Loaded 'Move' objects from resume file:")
         for m, w in zip(moves, weights):
-            print(    "{} mu0={}  weight={}  tuning={}".format(m.__class__.__name__, m.mu0, w, m.tune))
+            logs.overview(    "{} mu0={}  weight={}  tuning={}".format(m.__class__.__name__, m.mu0, w, m.tune))
         self.sampler._moves = moves
         self.sampler._weights = weights
         self.sampler.tune = tune
         self.sampler.mu = mu
         self.sampler.mus = mus
 
         if tune:
-            print("Resumed sampler is still tuning")
+            logs.overview("Resumed sampler is still tuning")
         else:
-            print("Resumed sampler has finished tuning")
+            logs.overview("Resumed sampler has finished tuning")
 
         # if we have some chain, read it here and use it to get
         # the p0 value and number of samples
         if self.output.resumed:
             data = np.genfromtxt(self.output._filename, invalid_raise=False)[:, :self.ndim]
             num_samples = len(data) // self.nwalkers
             self.p0 = data[-self.nwalkers:]
             self.num_samples += num_samples
             if self.num_samples >= self.samples:
-                print("You told me to resume the chain - it has already completed (with {} samples), so sampling will end.".format(len(data)))
-                print("Increase the 'samples' parameter to keep going.")
+                logs.error("You told me to resume the chain - it has already completed (with {} samples), so sampling will end.".format(len(data)))
+                logs.error("Increase the 'samples' parameter to keep going.")
             else:
-                print("Continuing zeus from existing chain - have {} samples already".format(len(data)))
+                logs.overview("Continuing zeus from existing chain - have {} samples already".format(len(data)))
 
     def load_start(self, filename):
         #Load the data and cut to the bits we need.
         #This means you can either just use a test file with
         #starting points, or an emcee output file.
         data = np.genfromtxt(filename, invalid_raise=False)[-self.nwalkers:, :self.ndim]
         if data.shape != (self.nwalkers, self.ndim):
@@ -219,15 +219,15 @@
 
 
     def execute(self):
         #Run the zeus sampler.
         if self.started:
             start = self.sampler.chain.shape[0]
         else:
-            print("Begun sampling")
+            logs.error("Begun sampling")
             self.started = True
             start = 0
 
         # Main execution
         self.sampler.run(self.p0, self.nsteps)
         # Update patience (relevant when self.nsteps<self.patience)
         self.sampler.patience-= self.nsteps
@@ -248,26 +248,25 @@
         #to the last ones for this chunk
         # get_last_sample changed from an attribute to a method recently
         try:
             self.p0 = self.sampler.get_last_sample()
         except TypeError:
             self.p0 = self.sampler.get_last_sample
         self.num_samples += self.nsteps
-        import scipy.fft
+
         taus = self.zeus.AutoCorrTime(chain)
-        print("\nHave {} samples from zeus. Current auto-correlation estimates are:".format(
-            self.num_samples*self.nwalkers))
+        logs.overview(f"Have {self.num_samples} samples from zeus. Current auto-correlation estimates are:")
         for par, tau in zip(self.pipeline.varied_params, taus):
-            print("   {}:  {:.2f}".format(par, tau))
+            logs.overview("   {}:  {:.2f}".format(par, tau))
         sys.stdout.flush()
 
         if self.sampler.tune:
-            print("Sampler is (still) tuning")
+            logs.overview("Sampler is (still) tuning")
         else:
-            print("Sampler is no longer tuning")
+            logs.overview("Sampler is no longer tuning")
 
         self.write_resume_info([self.sampler._moves, self.sampler._weights,
                                 self.sampler.tune, self.sampler.mu, self.sampler.mus])
 
     def is_converged(self):
         return self.num_samples >= self.samples
```

### Comparing `cosmosis-3.0.1/cosmosis/test/example_module2.py` & `cosmosis-3.0.3/cosmosis/test/example_module2.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/test/libtest/Makefile` & `cosmosis-3.0.3/cosmosis/test/libtest/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/test/libtest/c_datablock_complex_array_test.c` & `cosmosis-3.0.3/cosmosis/test/libtest/c_datablock_complex_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/test/libtest/c_datablock_double_array_test.c` & `cosmosis-3.0.3/cosmosis/test/libtest/c_datablock_double_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/test/libtest/c_datablock_int_array_test.c` & `cosmosis-3.0.3/cosmosis/test/libtest/c_datablock_int_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c` & `cosmosis-3.0.3/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c` & `cosmosis-3.0.3/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c` & `cosmosis-3.0.3/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/test/libtest/c_datablock_test.c` & `cosmosis-3.0.3/cosmosis/test/libtest/c_datablock_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/test/libtest/cosmosis_test.F90` & `cosmosis-3.0.3/cosmosis/test/libtest/cosmosis_test.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/test/libtest/datablock_test.cc` & `cosmosis-3.0.3/cosmosis/test/libtest/datablock_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/test/libtest/entry_test.cc` & `cosmosis-3.0.3/cosmosis/test/libtest/entry_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/test/libtest/ndarray_test.cc` & `cosmosis-3.0.3/cosmosis/test/libtest/ndarray_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/test/libtest/section_test.cc` & `cosmosis-3.0.3/cosmosis/test/libtest/section_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/test/libtest/test_c_datablock_scalars.h` & `cosmosis-3.0.3/cosmosis/test/libtest/test_c_datablock_scalars.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/test/libtest/test_c_datablock_scalars.template` & `cosmosis-3.0.3/cosmosis/test/libtest/test_c_datablock_scalars.template`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/test/test_block.py` & `cosmosis-3.0.3/cosmosis/test/test_block.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/test/test_campaign.py` & `cosmosis-3.0.3/cosmosis/test/test_campaign.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/test/test_chaining.py` & `cosmosis-3.0.3/cosmosis/test/test_chaining.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/test/test_gaussian.py` & `cosmosis-3.0.3/cosmosis/test/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/test/test_lib.py` & `cosmosis-3.0.3/cosmosis/test/test_lib.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/test/test_modules.py` & `cosmosis-3.0.3/cosmosis/test/test_modules.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/test/test_parameters.py` & `cosmosis-3.0.3/cosmosis/test/test_parameters.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/test/test_pipeline.py` & `cosmosis-3.0.3/cosmosis/test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/test/test_polychord.py` & `cosmosis-3.0.3/cosmosis/test/test_polychord.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/test/test_samplers.py` & `cosmosis-3.0.3/cosmosis/test/test_samplers.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/test/test_text_output.py` & `cosmosis-3.0.3/cosmosis/test/test_text_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/test/test_utils.py` & `cosmosis-3.0.3/cosmosis/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis/utils.py` & `cosmosis-3.0.3/cosmosis/utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/cosmosis.egg-info/SOURCES.txt` & `cosmosis-3.0.3/cosmosis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.1/setup.py` & `cosmosis-3.0.3/setup.py`

 * *Files identical despite different names*

