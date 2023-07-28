# Comparing `tmp/dkist_processing_visp-2.6.3.tar.gz` & `tmp/dkist_processing_visp-2.7.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_processing_visp-2.6.3.tar", last modified: Wed Jul 26 23:42:02 2023, max compression
+gzip compressed data, was "dkist_processing_visp-2.7.0rc1.tar", last modified: Fri Jul 28 15:53:48 2023, max compression
```

## Comparing `dkist_processing_visp-2.6.3.tar` & `dkist_processing_visp-2.7.0rc1.tar`

### file list

```diff
@@ -1,115 +1,116 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 23:42:02.719574 dkist_processing_visp-2.6.3/
--rw-rw-rw-   0 root         (0) root         (0)     2461 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      306 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    22523 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     6213 2023-07-26 23:42:02.719574 dkist_processing_visp-2.6.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5645 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     3652 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/SCIENCE_CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     3428 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 23:42:02.707574 dkist_processing_visp-2.6.3/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/changelog/.gitempty
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 23:42:02.707574 dkist_processing_visp-2.6.3/dkist_processing_visp/
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 23:42:02.711574 dkist_processing_visp-2.6.3/dkist_processing_visp/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/fonts/Lato-Regular.ttf
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 23:42:02.711574 dkist_processing_visp-2.6.3/dkist_processing_visp/models/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3440 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    11306 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1271 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/models/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 23:42:02.711574 dkist_processing_visp-2.6.3/dkist_processing_visp/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5370 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/parsers/map_repeats.py
--rw-rw-rw-   0 root         (0) root         (0)     3005 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/parsers/modulator_states.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/parsers/polarimeter_mode.py
--rw-rw-rw-   0 root         (0) root         (0)     2913 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/parsers/raster_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1268 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/parsers/task.py
--rw-rw-rw-   0 root         (0) root         (0)     1869 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     1335 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/parsers/visp_l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/parsers/visp_l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      843 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/parsers/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 23:42:02.715574 dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3296 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    14744 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/background_light.py
--rw-rw-rw-   0 root         (0) root         (0)     4137 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/dark.py
--rw-rw-rw-   0 root         (0) root         (0)    41082 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/geometric.py
--rw-rw-rw-   0 root         (0) root         (0)    20368 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/instrument_polarization.py
--rw-rw-rw-   0 root         (0) root         (0)      395 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)     5343 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/lamp.py
--rw-rw-rw-   0 root         (0) root         (0)     7068 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/make_movie_frames.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 23:42:02.715574 dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5642 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/mixin/corrections.py
--rw-rw-rw-   0 root         (0) root         (0)     1343 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/mixin/downsample.py
--rw-rw-rw-   0 root         (0) root         (0)     7112 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/mixin/input_frame_loaders.py
--rw-rw-rw-   0 root         (0) root         (0)    10506 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     4329 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/parse.py
--rw-rw-rw-   0 root         (0) root         (0)     7944 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)    28173 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/science.py
--rw-rw-rw-   0 root         (0) root         (0)    28801 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/solar.py
--rw-rw-rw-   0 root         (0) root         (0)     1611 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1559 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/visp_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6846 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 23:42:02.715574 dkist_processing_visp-2.6.3/dkist_processing_visp/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16409 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tests/conftest.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 23:42:02.715574 dkist_processing_visp-2.6.3/dkist_processing_visp/tests/local_trial_workflows/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tests/local_trial_workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18994 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tests/local_trial_workflows/l0_to_l1.py
--rw-rw-rw-   0 root         (0) root         (0)     8247 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tests/local_trial_workflows/local_trial_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2514 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    18443 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_background_light.py
--rw-rw-rw-   0 root         (0) root         (0)     1171 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_build_quality_report.py
--rw-rw-rw-   0 root         (0) root         (0)     5272 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_dark.py
--rw-rw-rw-   0 root         (0) root         (0)     2173 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_downsample.py
--rw-rw-rw-   0 root         (0) root         (0)    14009 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_geometric.py
--rw-rw-rw-   0 root         (0) root         (0)    12613 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_instrument_polarization.py
--rw-rw-rw-   0 root         (0) root         (0)     5651 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_lamp.py
--rw-rw-rw-   0 root         (0) root         (0)     4021 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_make_movie_frames.py
--rw-rw-rw-   0 root         (0) root         (0)    11818 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_map_repeats.py
--rw-rw-rw-   0 root         (0) root         (0)     2588 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    20093 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_parse.py
--rw-rw-rw-   0 root         (0) root         (0)     4383 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    19734 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_science.py
--rw-rw-rw-   0 root         (0) root         (0)     9883 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_solar.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_submit_quality.py
--rw-rw-rw-   0 root         (0) root         (0)     5340 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)     5091 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_visp_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1731 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_visp_constants.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_workflows.py
--rw-rw-rw-   0 root         (0) root         (0)     5752 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 23:42:02.719574 dkist_processing_visp-2.6.3/dkist_processing_visp/workflows/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3280 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/workflows/l0_processing.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/workflows/single_task_workflows.py
--rw-rw-rw-   0 root         (0) root         (0)     3314 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/dkist_processing_visp/workflows/trial_workflows.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 23:42:02.711574 dkist_processing_visp-2.6.3/dkist_processing_visp.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     6213 2023-07-26 23:42:02.000000 dkist_processing_visp-2.6.3/dkist_processing_visp.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3923 2023-07-26 23:42:02.000000 dkist_processing_visp-2.6.3/dkist_processing_visp.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-26 23:42:02.000000 dkist_processing_visp-2.6.3/dkist_processing_visp.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-07-26 23:42:02.000000 dkist_processing_visp-2.6.3/dkist_processing_visp.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-26 23:42:02.000000 dkist_processing_visp-2.6.3/dkist_processing_visp.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 23:42:02.719574 dkist_processing_visp-2.6.3/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     4844 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/docs/background_light.rst
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     2028 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     6427 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/docs/gain_correction.rst
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      623 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/docs/l0_to_l1_visp.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)     4995 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/docs/polarization_calibration.rst
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/docs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/docs/requirements_table.rst
--rw-rw-rw-   0 root         (0) root         (0)     2429 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/docs/science_calibration.rst
--rw-rw-rw-   0 root         (0) root         (0)      300 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/docs/scientific_changelog.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 23:42:02.719574 dkist_processing_visp-2.6.3/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       60 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/science_towncrier.sh
--rw-rw-rw-   0 root         (0) root         (0)     1687 2023-07-26 23:42:02.719574 dkist_processing_visp-2.6.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      422 2023-07-26 23:41:57.000000 dkist_processing_visp-2.6.3/towncrier_science.toml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-28 15:53:48.532338 dkist_processing_visp-2.7.0rc1/
+-rw-rw-rw-   0 root         (0) root         (0)     2461 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    22523 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6216 2023-07-28 15:53:48.532338 dkist_processing_visp-2.7.0rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5645 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3652 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/SCIENCE_CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3429 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-28 15:53:48.520337 dkist_processing_visp-2.7.0rc1/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/changelog/123.bugfix.rst
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-28 15:53:48.520337 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-28 15:53:48.520337 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/fonts/Lato-Regular.ttf
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-28 15:53:48.520337 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/models/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4534 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    11306 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1271 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/models/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-28 15:53:48.524337 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5370 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/parsers/map_repeats.py
+-rw-rw-rw-   0 root         (0) root         (0)     3005 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/parsers/modulator_states.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/parsers/polarimeter_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)     2913 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/parsers/raster_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1268 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/parsers/task.py
+-rw-rw-rw-   0 root         (0) root         (0)      901 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     1335 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/parsers/visp_l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      859 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/parsers/visp_l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      843 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/parsers/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-28 15:53:48.524337 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3296 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    15944 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/background_light.py
+-rw-rw-rw-   0 root         (0) root         (0)     4811 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/dark.py
+-rw-rw-rw-   0 root         (0) root         (0)    42350 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/geometric.py
+-rw-rw-rw-   0 root         (0) root         (0)    20606 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/instrument_polarization.py
+-rw-rw-rw-   0 root         (0) root         (0)      395 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     5894 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/lamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     7068 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/make_movie_frames.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-28 15:53:48.524337 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5642 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/mixin/corrections.py
+-rw-rw-rw-   0 root         (0) root         (0)     1343 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/mixin/downsample.py
+-rw-rw-rw-   0 root         (0) root         (0)     7412 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/mixin/input_frame_loaders.py
+-rw-rw-rw-   0 root         (0) root         (0)    10986 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     5775 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     7944 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)    28745 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/science.py
+-rw-rw-rw-   0 root         (0) root         (0)    29417 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1611 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1559 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/visp_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6846 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-28 15:53:48.528338 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17036 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/conftest.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-28 15:53:48.528338 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/local_trial_workflows/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/local_trial_workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19339 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/local_trial_workflows/l0_to_l1.py
+-rw-rw-rw-   0 root         (0) root         (0)     8247 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/local_trial_workflows/local_trial_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2514 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    18552 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_background_light.py
+-rw-rw-rw-   0 root         (0) root         (0)     1171 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_build_quality_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     5601 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_dark.py
+-rw-rw-rw-   0 root         (0) root         (0)     2173 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_downsample.py
+-rw-rw-rw-   0 root         (0) root         (0)    14378 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_geometric.py
+-rw-rw-rw-   0 root         (0) root         (0)    12640 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_instrument_polarization.py
+-rw-rw-rw-   0 root         (0) root         (0)     5798 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_lamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4021 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_make_movie_frames.py
+-rw-rw-rw-   0 root         (0) root         (0)    11818 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_map_repeats.py
+-rw-rw-rw-   0 root         (0) root         (0)     2588 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    20619 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     4383 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    22743 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_science.py
+-rw-rw-rw-   0 root         (0) root         (0)     9997 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_submit_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     5340 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     5094 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_visp_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_visp_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)     5752 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-28 15:53:48.532338 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3280 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/workflows/l0_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/workflows/single_task_workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)     3314 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp/workflows/trial_workflows.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-28 15:53:48.520337 dkist_processing_visp-2.7.0rc1/dkist_processing_visp.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     6216 2023-07-28 15:53:48.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3948 2023-07-28 15:53:48.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-28 15:53:48.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      624 2023-07-28 15:53:48.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-28 15:53:48.000000 dkist_processing_visp-2.7.0rc1/dkist_processing_visp.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-28 15:53:48.532338 dkist_processing_visp-2.7.0rc1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     4844 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/docs/background_light.rst
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2028 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     6427 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/docs/gain_correction.rst
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      623 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/docs/l0_to_l1_visp.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)     4995 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/docs/polarization_calibration.rst
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/docs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/docs/requirements_table.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/docs/science_calibration.rst
+-rw-rw-rw-   0 root         (0) root         (0)      300 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/docs/scientific_changelog.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-28 15:53:48.532338 dkist_processing_visp-2.7.0rc1/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       60 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/science_towncrier.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2023-07-28 15:53:48.532338 dkist_processing_visp-2.7.0rc1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      422 2023-07-28 15:53:40.000000 dkist_processing_visp-2.7.0rc1/towncrier_science.toml
```

### Comparing `dkist_processing_visp-2.6.3/.gitignore` & `dkist_processing_visp-2.7.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/.pre-commit-config.yaml` & `dkist_processing_visp-2.7.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/CHANGELOG.rst` & `dkist_processing_visp-2.7.0rc1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/PKG-INFO` & `dkist_processing_visp-2.7.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist_processing_visp
-Version: 2.6.3
+Version: 2.7.0rc1
 Summary: Science processing code for the ViSP instrument on DKIST
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-visp/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/visp
 Classifier: Programming Language :: Python
```

### Comparing `dkist_processing_visp-2.6.3/README.rst` & `dkist_processing_visp-2.7.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/SCIENCE_CHANGELOG.rst` & `dkist_processing_visp-2.7.0rc1/SCIENCE_CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/bitbucket-pipelines.yml` & `dkist_processing_visp-2.7.0rc1/bitbucket-pipelines.yml`

 * *Files 0% similar despite different names*

```diff
@@ -100,10 +100,10 @@
     'v*':
       - parallel:
         - step: *check_changelog
         - step: *lint
       - parallel:
         - step: *scan
         - step: *test
-        - step: *docs
+        #- step: *docs
       - step: *push_workflow
       - step: *push_code
```

### Comparing `dkist_processing_visp-2.6.3/check_changelog_updated.sh` & `dkist_processing_visp-2.7.0rc1/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/fonts/Lato-Regular.ttf` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/models/constants.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/models/constants.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,17 +9,21 @@
     """Names to be used in Visp buds."""
 
     num_raster_steps = "NUM_RASTER_STEPS"
     polarimeter_mode = "POLARIMETER_MODE"
     wavelength = "WAVELENGTH"
     obs_ip_start_time = "OBS_IP_START_TIME"
     lamp_exposure_times = "LAMP_EXPOSURE_TIMES"
+    lamp_readout_exp_times = "LAMP_READOUT_EXP_TIMES"
     solar_exposure_times = "SOLAR_EXPOSURE_TIMES"
+    solar_readout_exp_times = "SOLAR_READOUT_EXP_TIMES"
     observe_exposure_times = "OBSERVE_EXPOSURE_TIMES"
+    observe_readout_exp_times = "OBSERVE_READOUT_EXP_TIMES"
     polcal_exposure_times = "POLCAL_EXPOSURE_TIMES"
+    polcal_readout_exp_times = "POLCAL_READOUT_EXP_TIMES"
     num_map_scans = "NUM_MAP_SCANS"
     axis_1_type = "AXIS_1_TYPE"
     axis_2_type = "AXIS_2_TYPE"
     axis_3_type = "AXIS_3_TYPE"
 
 
 class VispConstants(ConstantsBase):
@@ -89,14 +93,37 @@
 
     @property
     def observe_exposure_times(self) -> [float]:
         """Find the observation exposure time."""
         return self._db_dict[VispBudName.observe_exposure_times.value]
 
     @property
+    def lamp_readout_exp_times(self) -> [float]:
+        """Find the lamp readout exposure time."""
+        return self._db_dict[VispBudName.lamp_readout_exp_times.value]
+
+    @property
+    def solar_readout_exp_times(self) -> [float]:
+        """Find the solar readout exposure time."""
+        return self._db_dict[VispBudName.solar_readout_exp_times.value]
+
+    @property
+    def polcal_readout_exp_times(self) -> [float]:
+        """Find the polarization calibration readout exposure time."""
+        if self.correct_for_polarization:
+            return self._db_dict[VispBudName.polcal_readout_exp_times.value]
+        else:
+            return []
+
+    @property
+    def observe_readout_exp_times(self) -> [float]:
+        """Find the observation readout exposure time."""
+        return self._db_dict[VispBudName.observe_readout_exp_times.value]
+
+    @property
     def axis_1_type(self) -> str:
         """Find the type of the first array axis."""
         return self._db_dict[VispBudName.axis_1_type.value]
 
     @property
     def axis_2_type(self) -> str:
         """Find the type of the second array axis."""
```

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/models/parameters.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/models/tags.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/parsers/map_repeats.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/parsers/map_repeats.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/parsers/modulator_states.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/parsers/modulator_states.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/parsers/polarimeter_mode.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/parsers/polarimeter_mode.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/parsers/raster_step.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/parsers/raster_step.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/parsers/task.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/parsers/task.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/parsers/visp_l0_fits_access.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/parsers/visp_l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/parsers/visp_l1_fits_access.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/parsers/visp_l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/parsers/wavelength.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/parsers/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/assemble_movie.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/background_light.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/background_light.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """ViSP background light calibration task."""
 import gc
 import time
 
 import numpy as np
 import scipy.optimize as spo
 from astropy.io import fits
+from dkist_processing_common.codecs.fits import fits_access_decoder
 from dkist_processing_common.codecs.fits import fits_array_encoder
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 from dkist_processing_math.arithmetic import subtract_array_from_arrays
 from dkist_processing_math.statistics import average_numpy_arrays
 from dkist_processing_math.transform.binning import resize_arrays
 from logging42 import logger
 
 from dkist_processing_visp.models.tags import VispTag
+from dkist_processing_visp.parsers.visp_l0_fits_access import VispL0FitsAccess
 from dkist_processing_visp.tasks.mixin.corrections import CorrectionsMixin
 from dkist_processing_visp.tasks.mixin.downsample import DownsampleMixin
 from dkist_processing_visp.tasks.mixin.input_frame_loaders import InputFrameLoadersMixin
 from dkist_processing_visp.tasks.mixin.intermediate_frame_helpers import (
     IntermediateFrameHelpersMixin,
 )
 from dkist_processing_visp.tasks.visp_base import VispTaskBase
@@ -134,15 +136,20 @@
                     + self.constants.solar_exposure_times
                     + self.constants.observe_exposure_times
                 )
             )
             != 1
         ):
             raise ValueError(
-                "Polcal, solar_gain, and observe frames do not all have the same exposure time. Background light correction is not possible."
+                "Polcal, solar_gain, and observe frames do not all have the same FPA exposure time. Background light correction is not possible."
+            )
+
+        if len(self.constants.polcal_exposure_times) > 1:
+            raise ValueError(
+                f"Only a single polcal time is currently supported. Found {self.constants.polcal_exposure_times}"
             )
 
     def reduce_and_resample_polcals(self, beam: int, num_bins: int) -> tuple[int, int, np.ndarray]:
         """
         Remove dark signal from all polcal frames, resample their spatial dimension, and collect them in a big array stack.
 
         Polcal dark frames are ignored.
@@ -164,49 +171,68 @@
         #
         # We don't resample the wavelength dimension right now because the full, unsampled wavelength range is crucial
         # to the goodness-of-fit parameter. Basically, the spatial dimension can be resampled prior to fitting because
         # the spatial pixels are completely independent. The wavelength pixels are not, though, and therefor the full
         # set of data along the wavelength axis is required at the time of fitting. The wavelength subsample factor
         # *only* reduces the number of fit variables.
 
-        if len(self.constants.polcal_exposure_times) > 1:
-            raise ValueError(
-                f"Only a single polcal time is currently supported. Found {self.constants.polcal_exposure_times}"
-            )
-        exp_time = self.constants.polcal_exposure_times[0]
-        dark_array = self.intermediate_frame_helpers_load_dark_array(
-            beam=beam, exposure_time=exp_time
-        )
-
-        num_wave, num_slit_pos = dark_array.shape
-
         # Have to build this up dynamically because we don't want to hardcode the number of dark steps
         array_list = []
         logger.info(f"Using median filtering to resample spatial dimension to {num_bins} bins")
 
         for modstate in range(1, self.constants.num_modstates + 1):
             for cs_step in range(self.constants.num_cs_steps):
+                cs_step_tags = [
+                    VispTag.input(),
+                    VispTag.frame(),
+                    VispTag.task("POLCAL"),
+                    VispTag.modstate(modstate),
+                    VispTag.cs_step(cs_step),
+                ]
                 pol_cal_objs = list(
-                    self.input_frame_loaders_polcal_fits_access_generator(
-                        modstate=modstate, cs_step=cs_step, exposure_time=exp_time
+                    self.read(
+                        tags=cs_step_tags,
+                        decoder=fits_access_decoder,
+                        fits_access_class=VispL0FitsAccess,
                     )
                 )
                 if pol_cal_objs[0].gos_level0_status == "DarkShutter":
                     logger.info(f"Skipping dark step {modstate = } and {cs_step = }")
                     continue
+
                 logger.info(f"working on {modstate = } and {cs_step = }")
+                all_readout_frames = []
+                for readout_exp_time in self.constants.polcal_readout_exp_times:
+                    dark_array = self.intermediate_frame_helpers_load_dark_array(
+                        beam=beam, readout_exp_time=readout_exp_time
+                    )
+                    num_wave, num_slit_pos = dark_array.shape
 
-                pol_cal_arrays = [
-                    self.input_frame_loaders_get_beam(obj.data, beam=beam) for obj in pol_cal_objs
-                ]
-                input_data = average_numpy_arrays(pol_cal_arrays)
-                dark_subtracted_array = next(subtract_array_from_arrays(input_data, dark_array))
+                    tags = cs_step_tags + [VispTag.readout_exp_time(readout_exp_time)]
+                    pol_cal_objs = list(
+                        self.read(
+                            tags=tags,
+                            decoder=fits_access_decoder,
+                            fits_access_class=VispL0FitsAccess,
+                        )
+                    )
+
+                    readout_normalized_arrays = [
+                        self.input_frame_loaders_get_beam(obj.data, beam=beam)
+                        / obj.num_raw_frames_per_fpa
+                        for obj in pol_cal_objs
+                    ]
+                    input_data = average_numpy_arrays(readout_normalized_arrays)
+                    dark_subtracted_array = next(subtract_array_from_arrays(input_data, dark_array))
+                    all_readout_frames.append(dark_subtracted_array)
+
+                avg_readout_frames = average_numpy_arrays(all_readout_frames)
 
                 resampled_array = self.downsample_spatial_dimension_local_median(
-                    dark_subtracted_array,
+                    avg_readout_frames,
                     num_spatial_bins=self.parameters.background_num_spatial_bins,
                 )
 
                 array_list.append(resampled_array)
 
         output_array = np.stack(array_list)
         logger.info(
```

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/dark.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/dark.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Visp dark task."""
+from dkist_processing_common.codecs.fits import fits_access_decoder
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 from dkist_processing_math.statistics import average_numpy_arrays
 from logging42 import logger
 
 from dkist_processing_visp.models.tags import VispTag
+from dkist_processing_visp.parsers.visp_l0_fits_access import VispL0FitsAccess
 from dkist_processing_visp.tasks.mixin.input_frame_loaders import InputFrameLoadersMixin
 from dkist_processing_visp.tasks.mixin.intermediate_frame_helpers import (
     IntermediateFrameHelpersMixin,
 )
 from dkist_processing_visp.tasks.visp_base import VispTaskBase
 
 
@@ -42,57 +44,68 @@
             - Record quality metrics
 
         Returns
         -------
         None
 
         """
-        target_exp_times = list(
+        target_readout_exp_times = list(
             set(
-                self.constants.solar_exposure_times
-                + self.constants.observe_exposure_times
-                + self.constants.polcal_exposure_times
-                + self.constants.lamp_exposure_times
+                self.constants.solar_readout_exp_times
+                + self.constants.observe_readout_exp_times
+                + self.constants.polcal_readout_exp_times
+                + self.constants.lamp_readout_exp_times
             )
         )
-        logger.info(f"{target_exp_times = }")
+        logger.info(f"{target_readout_exp_times = }")
         with self.apm_task_step(
-            f"Calculating dark frames for {self.constants.num_beams} beams and {len(target_exp_times)} exp times"
+            f"Calculating dark frames for {self.constants.num_beams} beams and "
+            f"{len(target_readout_exp_times)} readout exp times"
         ):
             total_dark_frames_used = 0
-            for exp_time in target_exp_times:
+            for readout_exp_time in target_readout_exp_times:
                 for beam in range(1, self.constants.num_beams + 1):
-                    logger.info(f"Gathering input dark frames for {exp_time = } and {beam = }")
+                    logger.info(
+                        f"Gathering input dark frames for {readout_exp_time = } and {beam = }"
+                    )
                     dark_tags = [
                         VispTag.input(),
                         VispTag.frame(),
                         VispTag.task("DARK"),
-                        VispTag.exposure_time(exp_time),
+                        VispTag.readout_exp_time(readout_exp_time),
                     ]
                     current_exp_dark_count = self.scratch.count_all(tags=dark_tags)
                     if current_exp_dark_count == 0:
-                        raise ValueError(f"Could not find any darks for {exp_time = }")
+                        raise ValueError(f"Could not find any darks for {readout_exp_time = }")
                     total_dark_frames_used += current_exp_dark_count
-                    input_dark_arrays = self.input_frame_loaders_dark_array_generator(
-                        beam=beam, exposure_time=exp_time
+
+                    input_dark_objs = self.read(
+                        tags=dark_tags,
+                        decoder=fits_access_decoder,
+                        fits_access_class=VispL0FitsAccess,
                     )
 
                     with self.apm_processing_step(
-                        f"Calculating dark for {exp_time = } and {beam = }"
+                        f"Calculating dark for {readout_exp_time = } and {beam = }"
                     ):
-                        logger.info(f"Calculating dark for {exp_time = } and {beam = }")
-                        averaged_dark_array = average_numpy_arrays(input_dark_arrays)
+                        logger.info(f"Calculating dark for {readout_exp_time = } and {beam = }")
+                        readout_normalized_arrays = (
+                            self.input_frame_loaders_get_beam(o.data, beam=beam)
+                            / o.num_raw_frames_per_fpa
+                            for o in input_dark_objs
+                        )
+                        averaged_dark_array = average_numpy_arrays(readout_normalized_arrays)
 
-                    with self.apm_writing_step(f"Writing dark for {exp_time = } {beam = }"):
-                        logger.info(f"Writing dark for {exp_time = } {beam = }")
+                    with self.apm_writing_step(f"Writing dark for {readout_exp_time = } {beam = }"):
+                        logger.info(f"Writing dark for {readout_exp_time = } {beam = }")
                         self.intermediate_frame_helpers_write_arrays(
                             averaged_dark_array,
                             beam=beam,
                             task="DARK",
-                            exposure_time=exp_time,
+                            readout_exp_time=readout_exp_time,
                         )
 
         with self.apm_processing_step("Computing and logging quality metrics"):
             no_of_raw_dark_frames: int = self.scratch.count_all(
                 tags=[
                     VispTag.input(),
                     VispTag.frame(),
```

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/geometric.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/geometric.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,24 +8,26 @@
 import skimage.exposure as skie
 import skimage.metrics as skim
 import skimage.morphology as skimo
 import skimage.registration as skir
 from astropy.modeling import fitting
 from astropy.modeling import models
 from astropy.stats import sigma_clip
+from dkist_processing_common.codecs.fits import fits_access_decoder
 from dkist_processing_common.codecs.fits import fits_array_encoder
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 from dkist_processing_math.arithmetic import subtract_array_from_arrays
 from dkist_processing_math.statistics import average_numpy_arrays
 from logging42 import logger
 from scipy.fft import fftn
 from scipy.optimize import minimize
 from skimage.registration._phase_cross_correlation import _upsampled_dft
 
 from dkist_processing_visp.models.tags import VispTag
+from dkist_processing_visp.parsers.visp_l0_fits_access import VispL0FitsAccess
 from dkist_processing_visp.tasks.mixin.corrections import CorrectionsMixin
 from dkist_processing_visp.tasks.mixin.input_frame_loaders import InputFrameLoadersMixin
 from dkist_processing_visp.tasks.mixin.intermediate_frame_helpers import (
     IntermediateFrameHelpersMixin,
 )
 from dkist_processing_visp.tasks.solar import SolarCalibration
 from dkist_processing_visp.tasks.visp_base import VispTaskBase
@@ -265,31 +267,45 @@
     def do_basic_corrections(self):
         """Apply dark correction to all data that will be used for Geometric Calibration."""
         self._prep_lamp_gain()
         self._prep_input_solar_gain()
 
     def _prep_lamp_gain(self):
         """Apply dark corrections fo INPUT lamp frames."""
-        for exp_time in self.constants.lamp_exposure_times:
+        for readout_exp_time in self.constants.lamp_readout_exp_times:
             for beam in range(1, self.constants.num_beams + 1):
-                logger.info(f"Starting basic lamp reductions for {exp_time = } and {beam = }")
+                logger.info(
+                    f"Starting basic lamp reductions for {readout_exp_time = } and {beam = }"
+                )
                 try:
                     dark_array = self.intermediate_frame_helpers_load_dark_array(
-                        beam=beam, exposure_time=exp_time
+                        beam=beam, readout_exp_time=readout_exp_time
                     )
                 except StopIteration:
-                    raise ValueError(f"No matching dark found for {exp_time = } s")
+                    raise ValueError(f"No matching dark found for {readout_exp_time = } s")
 
                 for modstate in range(1, self.constants.num_modstates + 1):
-                    input_lamp_arrays = self.input_frame_loaders_lamp_gain_array_generator(
-                        beam=beam,
-                        modstate=modstate,
-                        exposure_time=exp_time,
+                    tags = [
+                        VispTag.input(),
+                        VispTag.frame(),
+                        VispTag.task("LAMP_GAIN"),
+                        VispTag.modstate(modstate),
+                        VispTag.readout_exp_time(readout_exp_time),
+                    ]
+                    input_lamp_gain_objs = self.read(
+                        tags=tags, decoder=fits_access_decoder, fits_access_class=VispL0FitsAccess
+                    )
+
+                    readout_normalized_arrays = (
+                        self.input_frame_loaders_get_beam(o.data, beam=beam)
+                        / o.num_raw_frames_per_fpa
+                        for o in input_lamp_gain_objs
                     )
-                    avg_lamp_array = average_numpy_arrays(input_lamp_arrays)
+
+                    avg_lamp_array = average_numpy_arrays(readout_normalized_arrays)
 
                     dark_corrected_lamp_array = next(
                         subtract_array_from_arrays(
                             arrays=avg_lamp_array, array_to_subtract=dark_array
                         )
                     )
 
@@ -303,31 +319,44 @@
 
     def _prep_input_solar_gain(self):
         """
         Apply dark correction to INPUT solar gain images.
 
         Lamp correction is not applied because it was found to reduce contrast between the spectra and the hairlines.
         """
-        for exp_time in self.constants.solar_exposure_times:
+        for readout_exp_time in self.constants.solar_readout_exp_times:
             for beam in range(1, self.constants.num_beams + 1):
-                logger.info(f"Starting basic reductions for {exp_time = } and {beam = }")
+                logger.info(f"Starting basic reductions for {readout_exp_time = } and {beam = }")
                 try:
                     dark_array = self.intermediate_frame_helpers_load_dark_array(
-                        beam=beam, exposure_time=exp_time
+                        beam=beam, readout_exp_time=readout_exp_time
                     )
                 except StopIteration:
-                    raise ValueError(f"No matching dark found for {exp_time = } s")
+                    raise ValueError(f"No matching dark found for {readout_exp_time = } s")
 
                 for modstate in range(1, self.constants.num_modstates + 1):
-                    input_solar_arrays = self.input_frame_loaders_solar_gain_array_generator(
-                        beam=beam,
-                        modstate=modstate,
-                        exposure_time=exp_time,
+
+                    tags = [
+                        VispTag.input(),
+                        VispTag.frame(),
+                        VispTag.task("SOLAR_GAIN"),
+                        VispTag.modstate(modstate),
+                        VispTag.readout_exp_time(readout_exp_time),
+                    ]
+                    input_solar_gain_objs = self.read(
+                        tags=tags, decoder=fits_access_decoder, fits_access_class=VispL0FitsAccess
                     )
-                    avg_solar_array = average_numpy_arrays(input_solar_arrays)
+
+                    readout_normalized_arrays = (
+                        self.input_frame_loaders_get_beam(o.data, beam=beam)
+                        / o.num_raw_frames_per_fpa
+                        for o in input_solar_gain_objs
+                    )
+
+                    avg_solar_array = average_numpy_arrays(readout_normalized_arrays)
 
                     dark_corrected_solar_array = next(
                         subtract_array_from_arrays(
                             arrays=avg_solar_array, array_to_subtract=dark_array
                         )
                     )
```

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/instrument_polarization.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/instrument_polarization.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """ViSP instrument polarization task. See :doc:`this page </polarization_calibration>` for more information."""
 from collections import defaultdict
 
 import numpy as np
 import scipy.ndimage as spnd
 from astropy.io import fits
+from dkist_processing_common.codecs.fits import fits_access_decoder
 from dkist_processing_common.codecs.fits import fits_array_encoder
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 from dkist_processing_math.arithmetic import divide_arrays_by_array
 from dkist_processing_math.arithmetic import subtract_array_from_arrays
 from dkist_processing_math.statistics import average_numpy_arrays
 from dkist_processing_math.transform.binning import resize_arrays
 from dkist_processing_pac.fitter.polcal_fitter import PolcalFitter
@@ -187,35 +188,35 @@
         for modstate in range(1, self.constants.num_modstates + 1):
             angle = self.intermediate_frame_helpers_load_angle(beam=beam)
             state_offset = self.intermediate_frame_helpers_load_state_offset(
                 beam=beam, modstate=modstate
             )
             spec_shift = self.intermediate_frame_helpers_load_spec_shift(beam=beam)
 
-            for exp_time in self.constants.polcal_exposure_times:
+            for readout_exp_time in self.constants.polcal_readout_exp_times:
                 # Put this loop here because the geometric objects will be constant across exposure times
-                logger.info(f"Loading dark for {exp_time = } and {beam = }")
+                logger.info(f"Loading dark for {readout_exp_time = } and {beam = }")
                 try:
                     dark_array = self.intermediate_frame_helpers_load_dark_array(
-                        beam, exposure_time=exp_time
+                        beam, readout_exp_time=readout_exp_time
                     )
                 except StopIteration:
-                    raise ValueError(f"No matching dark found for {exp_time = } s")
+                    raise ValueError(f"No matching dark found for {readout_exp_time = } s")
 
                 if background_array is None:
                     background_array = np.zeros(dark_array.shape)
 
                 for cs_step in range(self.constants.num_cs_steps):
                     local_obj, global_obj = self.reduce_single_step(
                         beam,
                         dark_array,
                         background_array,
                         modstate,
                         cs_step,
-                        exp_time,
+                        readout_exp_time,
                         angle,
                         state_offset,
                         spec_shift,
                     )
                     local_reduced_array_dict[cs_step].append(local_obj)
                     global_reduced_array_dict[cs_step].append(global_obj)
 
@@ -224,67 +225,77 @@
     def reduce_single_step(
         self,
         beam: int,
         dark_array: np.ndarray,
         background_array: np.ndarray,
         modstate: int,
         cs_step: int,
-        exp_time: float,
+        readout_exp_time: float,
         angle: float,
         state_offset: np.ndarray,
         spec_shift: np.ndarray,
     ) -> tuple[VispL0FitsAccess, VispL0FitsAccess]:
         """
         Reduce a single calibration step for this beam, cs step and modulator state.
 
         Parameters
         ----------
         beam : int
             The current beam being processed
+
         dark_array : np.ndarray
             The dark array for the current beam
+
         modstate : int
             The current modulator state
+
         cs_step : int
             The current cal sequence step
-        exp_time : float
-            The exposure time
+
+        readout_exp_time : float
+            The per-readout exposure time
+
         angle : float
             The beam angle for the current modstate
+
         state_offset : np.ndarray
             The state offset for the current modstate
+
         spec_shift : np.ndarray
             The spectral shift for the current modstate
 
         Returns
         -------
         The final reduced result for this single step
         """
-        apm_str = f"{beam = }, {modstate = }, {cs_step = }, and {exp_time = }"
+        apm_str = f"{beam = }, {modstate = }, {cs_step = }, and {readout_exp_time = }"
         logger.info(f"Reducing {apm_str}")
         # Get the iterable of objects for this beam, cal seq step and mod state
 
         # Get the headers and arrays as iterables
-        pol_cal_headers = (
-            obj.header
-            for obj in self.input_frame_loaders_polcal_fits_access_generator(
-                modstate=modstate, cs_step=cs_step, exposure_time=exp_time
-            )
-        )
-        pol_cal_arrays = (
-            self.input_frame_loaders_get_beam(obj.data, beam)
-            for obj in self.input_frame_loaders_polcal_fits_access_generator(
-                modstate=modstate, cs_step=cs_step, exposure_time=exp_time
-            )
+        tags = [
+            VispTag.frame(),
+            VispTag.input(),
+            VispTag.task("POLCAL"),
+            VispTag.modstate(modstate),
+            VispTag.cs_step(cs_step),
+            VispTag.readout_exp_time(readout_exp_time),
+        ]
+        polcal_objs = list(
+            self.read(tags=tags, decoder=fits_access_decoder, fits_access_class=VispL0FitsAccess)
         )
         # Grab the 1st header
-        avg_inst_pol_cal_header = next(pol_cal_headers)
+        avg_inst_pol_cal_header = polcal_objs[0].header
 
         # Average the arrays (this works for a single array as well)
-        avg_inst_pol_cal_array = average_numpy_arrays(pol_cal_arrays)
+        readout_normalized_arrays = (
+            self.input_frame_loaders_get_beam(o.data, beam=beam) / o.num_raw_frames_per_fpa
+            for o in polcal_objs
+        )
+        avg_inst_pol_cal_array = average_numpy_arrays(readout_normalized_arrays)
 
         with self.apm_processing_step(f"Apply basic corrections for {apm_str}"):
             dark_corrected_array = subtract_array_from_arrays(avg_inst_pol_cal_array, dark_array)
 
             background_corrected_array = subtract_array_from_arrays(
                 dark_corrected_array, background_array
             )
```

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/lamp.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/lamp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """ViSP lamp calibration task. See :doc:`this page </gain_correction>` for more information."""
 import numpy as np
+from dkist_processing_common.codecs.fits import fits_access_decoder
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 from dkist_processing_math.arithmetic import subtract_array_from_arrays
 from dkist_processing_math.statistics import average_numpy_arrays
 from logging42 import logger
 
 from dkist_processing_visp.models.tags import VispTag
+from dkist_processing_visp.parsers.visp_l0_fits_access import VispL0FitsAccess
 from dkist_processing_visp.tasks.mixin.corrections import CorrectionsMixin
 from dkist_processing_visp.tasks.mixin.input_frame_loaders import InputFrameLoadersMixin
 from dkist_processing_visp.tasks.mixin.intermediate_frame_helpers import (
     IntermediateFrameHelpersMixin,
 )
 from dkist_processing_visp.tasks.visp_base import VispTaskBase
 
@@ -48,37 +50,37 @@
 
         Returns
         -------
         None
 
         """
         with self.apm_task_step(
-            f"Generate lamp gains for {self.constants.num_beams} beams and {len(self.constants.lamp_exposure_times)} exposure times"
+            f"Generate lamp gains for {self.constants.num_beams} beams and {len(self.constants.lamp_readout_exp_times)} exposure times"
         ):
-            for exp_time in self.constants.lamp_exposure_times:
+            for readout_exp_time in self.constants.lamp_readout_exp_times:
                 for beam in range(1, self.constants.num_beams + 1):
                     logger.info(f"Load dark for beam {beam}")
                     try:
                         dark_array = self.intermediate_frame_helpers_load_dark_array(
-                            beam=beam, exposure_time=exp_time
+                            beam=beam, readout_exp_time=readout_exp_time
                         )
                     except StopIteration:
-                        raise ValueError(f"No matching dark found for {exp_time = } s")
+                        raise ValueError(f"No matching dark found for {readout_exp_time = } s")
 
                     for state_num in range(
                         1, self.constants.num_modstates + 1
                     ):  # modulator states go from 1 to n
                         logger.info(
                             f"Calculating average lamp gain for beam {beam}, modulator state {state_num}"
                         )
                         self.compute_and_write_master_lamp_gain_for_modstate(
                             modstate=state_num,
                             dark_array=dark_array,
                             beam=beam,
-                            exp_time=exp_time,
+                            readout_exp_time=readout_exp_time,
                         )
 
         with self.apm_processing_step("Computing and logging quality metrics"):
             no_of_raw_lamp_frames: int = self.scratch.count_all(
                 tags=[
                     VispTag.input(),
                     VispTag.frame(),
@@ -91,15 +93,15 @@
             )
 
     def compute_and_write_master_lamp_gain_for_modstate(
         self,
         modstate: int,
         dark_array: np.ndarray,
         beam: int,
-        exp_time: float,
+        readout_exp_time: float,
     ) -> None:
         """
         Compute and write master lamp gain for a given modstate and beam.
 
         Generally the algorithm is:
             1. Average input gain arrays
             2. Subtract average dark to get the dark corrected gain data
@@ -113,31 +115,42 @@
 
         dark_array : np.ndarray
             The master dark to be subtracted from each lamp gain file
 
         beam : int
             The number of the beam
 
-        exp_time : float
-            Exposure time
+        readout_exp_time : float
+            Exposure time of single readout
 
         Returns
         -------
         None
         """
-        apm_str = f"{beam = }, {modstate = }, and {exp_time = }"
+        apm_str = f"{beam = }, {modstate = }, and {readout_exp_time = }"
         # Get the input lamp gain arrays
-        input_lamp_gain_arrays = self.input_frame_loaders_lamp_gain_array_generator(
-            beam=beam, modstate=modstate, exposure_time=exp_time
+        tags = [
+            VispTag.input(),
+            VispTag.frame(),
+            VispTag.task("LAMP_GAIN"),
+            VispTag.modstate(modstate),
+            VispTag.readout_exp_time(readout_exp_time),
+        ]
+        input_lamp_gain_objs = self.read(
+            tags=tags, decoder=fits_access_decoder, fits_access_class=VispL0FitsAccess
         )
 
         with self.apm_processing_step(f"Computing gain for {apm_str}"):
-            # Calculate the average of the input gain arrays
-            averaged_gain_data = average_numpy_arrays(input_lamp_gain_arrays)
-            # subtract dark
+
+            readout_normalized_arrays = (
+                self.input_frame_loaders_get_beam(o.data, beam=beam) / o.num_raw_frames_per_fpa
+                for o in input_lamp_gain_objs
+            )
+            averaged_gain_data = average_numpy_arrays(readout_normalized_arrays)
+
             dark_corrected_gain_data = next(
                 subtract_array_from_arrays(averaged_gain_data, dark_array)
             )
             filtered_gain_data = self.corrections_mask_hairlines(dark_corrected_gain_data)
 
         with self.apm_writing_step(f"Writing gain array for {apm_str}"):
             self.intermediate_frame_helpers_write_arrays(
```

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/make_movie_frames.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/mixin/corrections.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/mixin/corrections.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/mixin/downsample.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/mixin/downsample.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/mixin/input_frame_loaders.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/mixin/input_frame_loaders.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,35 +19,44 @@
         beam: int | None = None,
         modstate: int | None = None,
         map_scan: int | None = None,
         raster_step: int | None = None,
         task: str | None = None,
         cs_step: int | None = None,
         exposure_time: float | None = None,
+        readout_exp_time: float | None = None,
     ) -> Generator[F, None, None]:
         """
         Load in intermediate fits frames.
 
         Parameters
         ----------
         beam : int
             The current beam being processed
+
         modstate : int
             The current modulator state
+
         map_scan : int
              The current map scan
+
         raster_step : int
             The slit step for this step
+
         task : str
             The task type of the data currently being processed
+
         cs_step : int
             The current cal sequence step
+
         exposure_time : float
-            The exposure time
+            The FPA exposure time
 
+        readout_exp_time
+            The exposure time of each readout
 
         Returns
         -------
         Generator
             Intermediate frames with correct tags
         """
         passed_args = locals()
@@ -185,41 +194,48 @@
 
     def input_frame_loaders_polcal_fits_access_generator(
         self,
         beam: int | None = None,
         modstate: int | None = None,
         cs_step: int | None = None,
         exposure_time: float | None = None,
+        readout_exp_time: float | None = None,
     ) -> Generator[FitsAccessBase, None, None]:
         """
         Load in intermediate polcal frames.
 
         Parameters
         ----------
         beam : int
             The current beam being processed
+
         modstate : int
             The current modulator state
+
         cs_step : int
             The current cal sequence step
+
         exposure_time : float
-            The exposure time
+            The FPA exposure time
 
+        readout_exp_time
+            The exposure time of each readout
 
         Returns
         -------
         Generator
             Intermediate polcal frames with correct tags
         """
         return self.input_frame_loaders_fits_access_generator(
             task="POLCAL",
             beam=beam,
             modstate=modstate,
             cs_step=cs_step,
             exposure_time=exposure_time,
+            readout_exp_time=readout_exp_time,
         )
 
     def input_frame_loaders_get_beam(self, array: np.ndarray, beam: int) -> np.ndarray:
         """
         Extract a single beam array from a dual-beam array.
 
         Parameters
```

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,29 +22,35 @@
 
     def intermediate_frame_helpers_load_intermediate_arrays(
         self,
         beam: int | None = None,
         task: str | None = None,
         modstate: int | None = None,
         exposure_time: float | None = None,
+        readout_exp_time: float | None = None,
     ) -> Generator[np.ndarray, None, None]:
         """
         Yield a generator that produces ndarrays for the requested tags.
 
         Parameters
         ----------
         beam : int
             The current beam being processed
+
         task : str
             The task type of the data currently being processed
+
         modstate : int
             The current modulator state
+
         exposure_time : float
-            The exposure time
+            The FPA exposure time
 
+        readout_exp_time
+            Exposure time of a single readout
 
         Returns
         -------
         Generator
             Array(s) of loaded intermediate data with requested tags
         """
         # See intermediate_frame_helpers_write_arrays for an explanation of how this works, to add new tags *all* that's needed
@@ -54,35 +60,44 @@
         for t, v in passed_args.items():
             if t not in ["self"] and v is not None:
                 tags.append(getattr(VispTag, t)(v))
 
         yield from self.read(decoder=fits_array_decoder, tags=tags)
 
     def intermediate_frame_helpers_load_dark_array(
-        self, beam: int | None = None, exposure_time: float | None = None
+        self,
+        beam: int | None = None,
+        exposure_time: float | None = None,
+        readout_exp_time: float | None = None,
     ) -> np.ndarray:
         """
         Produce dark ndarrays for the requested tags.
 
         Parameters
         ----------
         beam : int
             The current beam being processed
+
         exposure_time : float
-            The exposure time
+            The FPA exposure time
 
+        readout_exp_time
+            Exposure time of a single readout
 
         Returns
         -------
         ndarray
             Array of loaded intermediate dark data with requested tags
         """
         return next(
             self.intermediate_frame_helpers_load_intermediate_arrays(
-                beam=beam, task="DARK", exposure_time=exposure_time
+                beam=beam,
+                task="DARK",
+                exposure_time=exposure_time,
+                readout_exp_time=readout_exp_time,
             )
         )
 
     def intermediate_frame_helpers_load_background_array(
         self,
         beam: int | None = None,
     ) -> np.ndarray:
@@ -182,37 +197,49 @@
         headers: Iterable[fits.Header] | fits.Header | None = None,
         beam: int | None = None,
         modstate: int | None = None,
         map_scan: int | None = None,
         raster_step: int | None = None,
         task: str | None = None,
         exposure_time: float | None = None,
+        readout_exp_time: float | None = None,
         file_id: str | None = None,
     ) -> None:
         """
         Write out intermediate files with requested tags.
 
         Parameters
         ----------
         arrays
             pass
+
         headers
             pass
+
         beam : int
             The current beam being processed
+
         modstate : int
             The current modulator state
+
         map_scan : int
              The current map scan
+
         raster_step : int
             The slit step for this step
+
         task : str
             The task type of the data currently being processed
+
         exposure_time : float
-            The exposure time
+            The FPA exposure time
+
+        readout_exp_time
+            Exposure time of a single readout
+
         file_id:
             The unique file_id
 
         Returns
         -------
         None
         """
```

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/parse.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/parse.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 """ViSP parse task."""
 from typing import TypeVar
 
 from dkist_processing_common.models.flower_pot import Stem
 from dkist_processing_common.parsers.cs_step import CSStepFlower
 from dkist_processing_common.parsers.cs_step import NumCSStepBud
 from dkist_processing_common.parsers.time import ExposureTimeFlower
+from dkist_processing_common.parsers.time import ReadoutExpTimeFlower
+from dkist_processing_common.parsers.time import TaskExposureTimesBud
+from dkist_processing_common.parsers.time import TaskReadoutExpTimesBud
 from dkist_processing_common.parsers.unique_bud import UniqueBud
 from dkist_processing_common.tasks import ParseL0InputDataBase
 from dkist_processing_common.tasks.mixin.input_dataset import InputDatasetMixin
 
 from dkist_processing_visp.models.constants import VispBudName
 from dkist_processing_visp.models.parameters import VispParameters
 from dkist_processing_visp.parsers.map_repeats import MapScanFlower
 from dkist_processing_visp.parsers.map_repeats import NumMapScansBud
 from dkist_processing_visp.parsers.modulator_states import ModulatorStateFlower
 from dkist_processing_visp.parsers.modulator_states import NumberModulatorStatesBud
 from dkist_processing_visp.parsers.polarimeter_mode import PolarimeterModeBud
 from dkist_processing_visp.parsers.raster_step import RasterScanStepFlower
 from dkist_processing_visp.parsers.raster_step import TotalRasterStepsBud
+from dkist_processing_visp.parsers.task import parse_header_ip_task
 from dkist_processing_visp.parsers.task import VispTaskTypeFlower
 from dkist_processing_visp.parsers.time import ObsIpStartTimeBud
-from dkist_processing_visp.parsers.time import VispTaskExposureTimesBud
 from dkist_processing_visp.parsers.visp_l0_fits_access import VispL0FitsAccess
 from dkist_processing_visp.parsers.wavelength import ObserveWavelengthBud
 
 S = TypeVar("S", bound=Stem)
 
 
 class ParseL0VispInputData(ParseL0InputDataBase, InputDatasetMixin):
@@ -67,25 +70,53 @@
             NumMapScansBud(),
             TotalRasterStepsBud(),
             NumCSStepBud(self.parameters.max_cs_step_time_sec),
             ObsIpStartTimeBud(),
             NumberModulatorStatesBud(),
             ObserveWavelengthBud(),
             PolarimeterModeBud(),
-            VispTaskExposureTimesBud(
-                stem_name=VispBudName.lamp_exposure_times.value, ip_task_type="LAMP_GAIN"
+            TaskExposureTimesBud(
+                stem_name=VispBudName.lamp_exposure_times.value,
+                ip_task_type="LAMP_GAIN",
+                header_task_parsing_func=parse_header_ip_task,
             ),
-            VispTaskExposureTimesBud(
-                stem_name=VispBudName.solar_exposure_times.value, ip_task_type="SOLAR_GAIN"
+            TaskExposureTimesBud(
+                stem_name=VispBudName.solar_exposure_times.value,
+                ip_task_type="SOLAR_GAIN",
+                header_task_parsing_func=parse_header_ip_task,
             ),
-            VispTaskExposureTimesBud(
-                stem_name=VispBudName.observe_exposure_times.value, ip_task_type="OBSERVE"
+            TaskExposureTimesBud(
+                stem_name=VispBudName.observe_exposure_times.value,
+                ip_task_type="OBSERVE",
+                header_task_parsing_func=parse_header_ip_task,
             ),
-            VispTaskExposureTimesBud(
-                stem_name=VispBudName.polcal_exposure_times.value, ip_task_type="POLCAL"
+            TaskExposureTimesBud(
+                stem_name=VispBudName.polcal_exposure_times.value,
+                ip_task_type="POLCAL",
+                header_task_parsing_func=parse_header_ip_task,
+            ),
+            TaskReadoutExpTimesBud(
+                stem_name=VispBudName.lamp_readout_exp_times.value,
+                ip_task_type="LAMP_GAIN",
+                header_task_parsing_func=parse_header_ip_task,
+            ),
+            TaskReadoutExpTimesBud(
+                stem_name=VispBudName.solar_readout_exp_times.value,
+                ip_task_type="SOLAR_GAIN",
+                header_task_parsing_func=parse_header_ip_task,
+            ),
+            TaskReadoutExpTimesBud(
+                stem_name=VispBudName.observe_readout_exp_times.value,
+                ip_task_type="OBSERVE",
+                header_task_parsing_func=parse_header_ip_task,
+            ),
+            TaskReadoutExpTimesBud(
+                stem_name=VispBudName.polcal_readout_exp_times.value,
+                ip_task_type="POLCAL",
+                header_task_parsing_func=parse_header_ip_task,
             ),
             UniqueBud(constant_name=VispBudName.axis_1_type.value, metadata_key="axis_1_type"),
             UniqueBud(constant_name=VispBudName.axis_2_type.value, metadata_key="axis_2_type"),
             UniqueBud(constant_name=VispBudName.axis_3_type.value, metadata_key="axis_3_type"),
         ]
 
     @property
@@ -94,8 +125,9 @@
         return super().tag_flowers + [
             CSStepFlower(max_cs_step_time_sec=self.parameters.max_cs_step_time_sec),
             MapScanFlower(),
             VispTaskTypeFlower(),
             RasterScanStepFlower(),
             ModulatorStateFlower(),
             ExposureTimeFlower(),
+            ReadoutExpTimeFlower(),
         ]
```

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/quality_metrics.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/science.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/science.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from functools import cached_property
 from typing import Iterable
 
 import numpy as np
 from astropy.io import fits
 from astropy.time import Time
 from astropy.time import TimeDelta
+from dkist_processing_common.codecs.fits import fits_access_decoder
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 from dkist_processing_math.arithmetic import divide_arrays_by_array
 from dkist_processing_math.arithmetic import subtract_array_from_arrays
 from dkist_processing_math.statistics import average_numpy_arrays
 from dkist_processing_pac.optics.telescope import Telescope
 from logging42 import logger
 
@@ -149,25 +150,27 @@
         solar_dict = defaultdict(dict)
         angle_dict = dict()
         state_offset_dict = defaultdict(dict)
         spec_shift_dict = dict()
         demod_dict = dict() if self.constants.correct_for_polarization else None
 
         for beam in range(1, self.constants.num_beams + 1):
-            for exp_time in self.constants.observe_exposure_times:
+            for readout_exp_time in self.constants.observe_readout_exp_times:
                 # Dark
                 ######
                 try:
                     dark_array = self.intermediate_frame_helpers_load_dark_array(
-                        beam=beam, exposure_time=exp_time
+                        beam=beam, readout_exp_time=readout_exp_time
                     )
                 except StopIteration:
-                    raise ValueError(f"No matching dark found for {exp_time = } s")
+                    raise ValueError(f"No matching dark found for {readout_exp_time = } s")
 
-                dark_dict[VispTag.beam(beam)][VispTag.exposure_time(exp_time)] = dark_array
+                dark_dict[VispTag.beam(beam)][
+                    VispTag.readout_exp_time(readout_exp_time)
+                ] = dark_array
 
             # Residual background light
             ###########################
             try:
                 background_dict[
                     VispTag.beam(beam)
                 ] = self.intermediate_frame_helpers_load_background_array(beam=beam)
@@ -224,15 +227,15 @@
 
         - Apply all dark, background, gain, geometric corrections
         - Demodulate if needed
         - Combine beams
         - Apply telescope correction, if needed
         - Write calibrated arrays
         """
-        for exp_time in self.constants.observe_exposure_times:
+        for readout_exp_time in self.constants.observe_readout_exp_times:
             for map_scan in range(1, self.constants.num_map_scans + 1):
                 for raster_step in range(0, self.constants.num_raster_steps):
                     beam_storage = dict()
                     header_storage = dict()
                     for beam in range(1, self.constants.num_beams + 1):
                         apm_str = f"{map_scan = }, {raster_step = }, and {beam = }"
                         with self.apm_processing_step(f"Basic corrections for {apm_str}"):
@@ -244,27 +247,27 @@
                                 (
                                     intermediate_array,
                                     intermediate_header,
                                 ) = self.process_polarimetric_modstates(
                                     beam=beam,
                                     raster_step=raster_step,
                                     map_scan=map_scan,
-                                    exp_time=exp_time,
+                                    readout_exp_time=readout_exp_time,
                                     calibrations=calibrations,
                                 )
                             else:
                                 logger.info(
                                     f"Processing spectrographic observe frames from {apm_str}"
                                 )
                                 intermediate_array, intermediate_header = self.correct_single_frame(
                                     beam=beam,
                                     modstate=1,
                                     raster_step=raster_step,
                                     map_scan=map_scan,
-                                    exp_time=exp_time,
+                                    readout_exp_time=readout_exp_time,
                                     calibrations=calibrations,
                                 )
                                 intermediate_header = self._compute_date_keys(intermediate_header)
                             beam_storage[VispTag.beam(beam)] = intermediate_array
                             header_storage[VispTag.beam(beam)] = intermediate_header
 
                     with self.apm_processing_step("Combining beams"):
@@ -284,36 +287,38 @@
                         )
 
     def process_polarimetric_modstates(
         self,
         beam: int,
         raster_step: int,
         map_scan: int,
-        exp_time: float,
+        readout_exp_time: float,
         calibrations: CalibrationCollection,
     ) -> tuple[np.ndarray, fits.Header]:
         """
         Process a single polarimetric beam as much as is possible.
 
         This includes basic corrections and demodulation. Beam combination happens elsewhere.
         """
         # Create the 3D stack of corrected modulated arrays
-        array_shape = calibrations.dark[VispTag.beam(1)][VispTag.exposure_time(exp_time)].shape
+        array_shape = calibrations.dark[VispTag.beam(1)][
+            VispTag.readout_exp_time(readout_exp_time)
+        ].shape
         array_stack = np.zeros(array_shape + (self.constants.num_modstates,))
         header_stack = []
 
         with self.apm_processing_step(f"Correcting {self.constants.num_modstates} modstates"):
             for modstate in range(1, self.constants.num_modstates + 1):
                 # Correct the arrays
                 corrected_array, corrected_header = self.correct_single_frame(
                     beam=beam,
                     modstate=modstate,
                     raster_step=raster_step,
                     map_scan=map_scan,
-                    exp_time=exp_time,
+                    readout_exp_time=readout_exp_time,
                     calibrations=calibrations,
                 )
                 # Add this result to the 3D stack
                 array_stack[:, :, modstate - 1] = corrected_array
                 header_stack.append(corrected_header)
 
         with self.apm_processing_step("Applying instrument polarization correction"):
@@ -441,15 +446,15 @@
 
     def correct_single_frame(
         self,
         beam: int,
         modstate: int,
         raster_step: int,
         map_scan: int,
-        exp_time: float,
+        readout_exp_time: float,
         calibrations: CalibrationCollection,
     ) -> tuple[np.ndarray, fits.Header]:
         """
         Apply basic corrections to a single frame.
 
         Generally the algorithm is:
             1. Dark correct the array
@@ -464,49 +469,57 @@
             The beam number for this single step
         modstate
             The modulator state for this single step
         raster_step
             The slit step for this single step
         map_scan
             The current map scan
-        exp_time
+        readout_exp_time
             The exposure time for this single step
         calibrations
             Collection of all calibration objects
 
         Returns
         -------
             Corrected array, header
         """
         # Extract calibrations
-        dark_array = calibrations.dark[VispTag.beam(beam)][VispTag.exposure_time(exp_time)]
+        dark_array = calibrations.dark[VispTag.beam(beam)][
+            VispTag.readout_exp_time(readout_exp_time)
+        ]
         background_array = calibrations.background[VispTag.beam(beam)]
         solar_gain_array = calibrations.solar_gain[VispTag.beam(beam)][VispTag.modstate(modstate)]
         angle = calibrations.angle[VispTag.beam(beam)]
         spec_shift = calibrations.spec_shift[VispTag.beam(beam)]
         state_offset = calibrations.state_offset[VispTag.beam(beam)][VispTag.modstate(modstate)]
 
         # Grab the input observe frame
+        tags = [
+            VispTag.input(),
+            VispTag.frame(),
+            VispTag.task("OBSERVE"),
+            VispTag.modstate(modstate),
+            VispTag.map_scan(map_scan),
+            VispTag.raster_step(raster_step),
+            VispTag.readout_exp_time(readout_exp_time),
+        ]
         observe_object_list = list(
-            self.input_frame_loaders_observe_fits_access_generator(
-                map_scan=map_scan,
-                raster_step=raster_step,
-                modstate=modstate,
-                exposure_time=exp_time,
-            )
+            self.read(tags=tags, decoder=fits_access_decoder, fits_access_class=VispL0FitsAccess)
         )
+
         if len(observe_object_list) > 1:
             raise ValueError(
                 f"Found more than one observe frame for {map_scan = }, {raster_step = }, {modstate = }, "
-                f"and {exp_time = }. This should NEVER have happened!"
+                f"and {readout_exp_time = }. This should NEVER have happened!"
             )
         observe_object = observe_object_list[0]
 
         # Split the beam we want
-        observe_data = self.input_frame_loaders_get_beam(observe_object.data, beam=beam)
+        readout_normalized_data = observe_object.data / observe_object.num_raw_frames_per_fpa
+        observe_data = self.input_frame_loaders_get_beam(readout_normalized_data, beam=beam)
 
         # Dark correction
         dark_corrected_array = next(subtract_array_from_arrays(observe_data, dark_array))
 
         # Residual background correction
         background_corrected_array = next(
             subtract_array_from_arrays(dark_corrected_array, background_array)
```

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/solar.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/solar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """ViSP solar calibration task. See :doc:`this page </gain_correction>` for more information."""
 import numpy as np
 import peakutils
 import scipy.ndimage as spnd
 import scipy.optimize as spo
 import scipy.signal as sps
+from dkist_processing_common.codecs.fits import fits_access_decoder
 from dkist_processing_common.codecs.fits import fits_array_encoder
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 from dkist_processing_math.arithmetic import divide_arrays_by_array
 from dkist_processing_math.arithmetic import subtract_array_from_arrays
 from dkist_processing_math.statistics import average_numpy_arrays
 from logging42 import logger
 
 from dkist_processing_visp.models.tags import VispTag
+from dkist_processing_visp.parsers.visp_l0_fits_access import VispL0FitsAccess
 from dkist_processing_visp.tasks.mixin.corrections import CorrectionsMixin
 from dkist_processing_visp.tasks.mixin.input_frame_loaders import InputFrameLoadersMixin
 from dkist_processing_visp.tasks.mixin.intermediate_frame_helpers import (
     IntermediateFrameHelpersMixin,
 )
 from dkist_processing_visp.tasks.visp_base import VispTaskBase
 
@@ -278,44 +280,53 @@
             The modulator state for this array
 
 
         Returns
         -------
         None
         """
-        for exp_time in self.constants.solar_exposure_times:
+        for readout_exp_time in self.constants.solar_readout_exp_times:
             try:
                 dark_array = self.intermediate_frame_helpers_load_dark_array(
-                    beam=beam, exposure_time=exp_time
+                    beam=beam, readout_exp_time=readout_exp_time
                 )
             except StopIteration:
-                raise ValueError(f"No matching dark found for {exp_time = } s")
+                raise ValueError(f"No matching dark found for {readout_exp_time = } s")
 
             try:
                 background_array = self.intermediate_frame_helpers_load_background_array(beam=beam)
             except StopIteration:
                 if self.constants.correct_for_polarization and self.parameters.background_on:
                     raise ValueError(f"No matching background light found for {beam = }")
 
                 logger.info("Skipping background light correction")
                 background_array = np.zeros(dark_array.shape)
 
             logger.info(
                 f"Doing dark, background, lamp, and geo corrections for {beam=} and {modstate=}"
             )
             ## Load frames
-            input_solar_arrays = self.input_frame_loaders_solar_gain_array_generator(
-                beam=beam, modstate=modstate, exposure_time=exp_time
+            tags = [
+                VispTag.input(),
+                VispTag.frame(),
+                VispTag.task("SOLAR_GAIN"),
+                VispTag.modstate(modstate),
+                VispTag.readout_exp_time(readout_exp_time),
+            ]
+            input_solar_gain_objs = self.read(
+                tags=tags, decoder=fits_access_decoder, fits_access_class=VispL0FitsAccess
             )
-            lamp_array = self.intermediate_frame_helpers_load_lamp_gain_array(
-                beam=beam, modstate=modstate
+
+            readout_normalized_arrays = (
+                self.input_frame_loaders_get_beam(o.data, beam=beam) / o.num_raw_frames_per_fpa
+                for o in input_solar_gain_objs
             )
 
             ## Average
-            avg_solar_array = average_numpy_arrays(input_solar_arrays)
+            avg_solar_array = average_numpy_arrays(readout_normalized_arrays)
 
             ## Dark correction
             dark_corrected_solar_array = subtract_array_from_arrays(
                 arrays=avg_solar_array, array_to_subtract=dark_array
             )
 
             ## Residual background correction
@@ -328,14 +339,17 @@
                 arrays=background_corrected_solar_array,
                 beam=beam,
                 modstate=modstate,
                 task="SC_BG_ONLY",
             )
 
             ## Lamp correction
+            lamp_array = self.intermediate_frame_helpers_load_lamp_gain_array(
+                beam=beam, modstate=modstate
+            )
             lamp_corrected_solar_array = next(
                 divide_arrays_by_array(
                     arrays=background_corrected_solar_array, array_to_divide_by=lamp_array
                 )
             )
 
             self.intermediate_frame_helpers_write_arrays(
```

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/trial_output_data.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/trial_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/visp_base.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/visp_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tasks/write_l1.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tests/conftest.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,14 +80,16 @@
         self.add_constant_key("VISP_019", 1)
         self.add_constant_key("VISP_020", 1)
         self.add_constant_key("ID___004")
         self.add_constant_key(
             "WAVELNTH", 0.0
         )  # Intentionally bad to make sure it doesn't get parsed
         self.add_constant_key("CAM__004", 1.0)
+        self.add_constant_key("CAM__005", 2.0)
+        self.add_constant_key("CAM__014", 10)
 
 
 class VispHeadersValidLampGainFrames(VispHeaders):
     def __init__(
         self,
         dataset_shape: tuple[int, ...],
         array_shape: tuple[int, ...],
@@ -106,14 +108,16 @@
         self.add_constant_key("VISP_019", 1)
         self.add_constant_key("VISP_020", 1)
         self.add_constant_key("PAC__003", "on")
         self.add_constant_key("ID___004")
         self.add_constant_key("VISP_010", num_modstates)
         self.add_constant_key("VISP_011", modstate)
         self.add_constant_key("CAM__004", 10.0)
+        self.add_constant_key("CAM__005", 20.0)
+        self.add_constant_key("CAM__014", 10)
 
 
 class VispHeadersValidSolarGainFrames(VispHeaders):
     def __init__(
         self,
         dataset_shape: tuple[int, ...],
         array_shape: tuple[int, ...],
@@ -132,14 +136,16 @@
         self.add_constant_key("VISP_020", 1)
         self.add_constant_key("PAC__002", "clear")
         self.add_constant_key("TELSCAN", "Raster")
         self.add_constant_key("ID___004")
         self.add_constant_key("VISP_010", num_modstates)
         self.add_constant_key("VISP_011", modstate)
         self.add_constant_key("CAM__004", 20.0)
+        self.add_constant_key("CAM__005", 40.0)
+        self.add_constant_key("CAM__014", 10)
 
 
 class VispHeadersValidPolcalFrames(VispHeaders):
     def __init__(
         self,
         dataset_shape: tuple[int, ...],
         array_shape: tuple[int, ...],
@@ -162,14 +168,16 @@
         self.add_constant_key("PAC__005", "60.")
         self.add_constant_key("PAC__006", "clear")
         self.add_constant_key("PAC__007", "0.0")
         self.add_constant_key("PAC__008", "FieldStop (5arcmin)")
         self.add_constant_key("VISP_010", num_modstates)
         self.add_constant_key("VISP_011", modstate)
         self.add_constant_key("CAM__004", 0.01)
+        self.add_constant_key("CAM__005", 0.02)
+        self.add_constant_key("CAM__014", 10)
 
 
 class VispHeadersValidObserveFrames(VispHeaders):
     def __init__(
         self,
         dataset_shape: tuple[int, ...],
         array_shape: tuple[int, ...],
@@ -188,14 +196,15 @@
         self.add_constant_key("VISP_019", num_raster_steps)
         self.add_constant_key("VISP_020", raster_step)
         self.add_constant_key("ID___004")
         self.add_constant_key("VISP_010", num_modstates)
         self.add_constant_key("VISP_011", modstate)
         self.add_constant_key("WAVELNTH", 656.28)
         self.add_constant_key("EXPER_ID", "EXPERIMENT ID")
+        self.add_constant_key("CAM__014", 10)
 
 
 def generate_fits_frame(header_generator: Iterable, shape=None) -> fits.HDUList:
     shape = shape or (1, 10, 10)
     generated_header = next(header_generator)
     translated_header = translate_spec122_to_spec214_l0(generated_header)
     del translated_header["COMMENT"]
@@ -293,14 +302,18 @@
     MAXIMUM_CADENCE: float = 10.0
     VARIANCE_CADENCE: float = 0.0
     WAVELENGTH: float = 588.0
     LAMP_EXPOSURE_TIMES: tuple[float] = (100.0,)
     SOLAR_EXPOSURE_TIMES: tuple[float] = (1.0,)
     OBSERVE_EXPOSURE_TIMES: tuple[float] = (0.01,)
     POLCAL_EXPOSURE_TIMES: tuple[float] = ()
+    LAMP_READOUT_EXP_TIMES: tuple[float] = (200.0,)
+    SOLAR_READOUT_EXP_TIMES: tuple[float] = (2.0,)
+    OBSERVE_READOUT_EXP_TIMES: tuple[float] = (0.02,)
+    POLCAL_READOUT_EXP_TIMES: tuple[float] = ()
     SPECTRAL_LINE: str = "VISP Ca II H"
     STOKES_PARAMS: tuple[str] = (
         "I",
         "Q",
         "U",
         "V",
     )  # A tuple because lists aren't allowed on dataclasses
@@ -397,15 +410,15 @@
     visp_solar_zone_bg_order: WavelengthParameter = WavelengthParameter(values=(21, 22, 11, 22))
     visp_solar_zone_normalization_percentile: WavelengthParameter = WavelengthParameter(
         values=(90, 99, 90, 90)
     )
     visp_solar_zone_rel_height: float = 0.97
     visp_max_cs_step_time_sec: float = 180.0
     visp_polcal_spatial_median_filter_width_px: int = 10
-    visp_polcal_num_spatial_bins: int = 5
+    visp_polcal_num_spatial_bins: int = 10
     visp_polcal_demod_spatial_smooth_fit_order: int = 17
     visp_polcal_demod_spatial_smooth_min_samples: float = 0.9
     visp_polcal_demod_upsample_order: int = 3
     visp_pac_remove_linear_I_trend: bool = True
     visp_pac_fit_mode: str = "use_M12_I_sys_per_step"
     visp_pac_init_set: str = "OCCal_VIS"
```

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tests/local_trial_workflows/l0_to_l1.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/local_trial_workflows/l0_to_l1.py`

 * *Files 3% similar despite different names*

```diff
@@ -163,19 +163,24 @@
     def run(self) -> None:
         logger.info(f"{self.constants.correct_for_polarization = }")
 
 
 class ShowExposureTimes(VispTaskBase):
     def run(self) -> None:
         logger.info(f"{self.constants.dark_exposure_times = }")
+        logger.info(f"{self.constants.dark_readout_exp_times = }")
         logger.info(f"{self.constants.lamp_exposure_times = }")
+        logger.info(f"{self.constants.lamp_readout_exp_times = }")
         logger.info(f"{self.constants.solar_exposure_times = }")
+        logger.info(f"{self.constants.solar_readout_exp_times = }")
         if self.constants.correct_for_polarization:
             logger.info(f"{self.constants.polcal_exposure_times = }")
+            logger.info(f"{self.constants.polcal_readout_exp_times = }")
         logger.info(f"{self.constants.observe_exposure_times = }")
+        logger.info(f"{self.constants.observe_readout_exp_times = }")
 
 
 class ShowMapMapping(VispTaskBase):
     def run(self) -> None:
         logger.info(f"Found {self.constants.num_map_scans} map scans")
         step = 0
         logger.info(f"Step {step} is organized thusly:")
```

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tests/local_trial_workflows/local_trial_helpers.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/local_trial_workflows/local_trial_helpers.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_assemble_movie.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_background_light.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_background_light.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,14 +292,15 @@
     background_full_beam_shape,
     background_testing_parameters,
 ):
     constants_db = VispConstantsDb(
         SOLAR_EXPOSURE_TIMES=(10.0,),
         OBSERVE_EXPOSURE_TIMES=(10.0,),
         POLCAL_EXPOSURE_TIMES=(10.0,),
+        POLCAL_READOUT_EXP_TIMES=(0.02,),
         NUM_CS_STEPS=len(fully_realistic_cs),
     )
     init_visp_constants_db(recipe_run_id, constants_db)
     with BackgroundLightCalibration(
         recipe_run_id=recipe_run_id,
         workflow_name="background_light_calibration",
         workflow_version="vX.Y",
@@ -311,15 +312,15 @@
             )
             assign_input_dataset_doc_to_task(task, background_testing_parameters)
 
             dark_cal = np.zeros(background_full_beam_shape)
             # Need a dark for each beam
             for b in range(number_of_beams):
                 task.intermediate_frame_helpers_write_arrays(
-                    arrays=dark_cal, beam=b + 1, task="DARK", exposure_time=10.0
+                    arrays=dark_cal, beam=b + 1, task="DARK", readout_exp_time=0.02
                 )
 
             # Now write polcal frames
             num_steps = len(fully_realistic_cs)
             num_mod = len(fully_realistic_cs[0])
             total_polcal_files = num_mod * num_steps
             num_dark_polcal_files = num_mod * 2
@@ -334,14 +335,15 @@
                         hdu_list=hdul,
                         tags=[
                             VispTag.input(),
                             VispTag.task("POLCAL"),
                             VispTag.modstate(m + 1),
                             VispTag.cs_step(n),
                             VispTag.exposure_time(10.0),
+                            VispTag.readout_exp_time(0.02),
                             VispTag.frame(),
                         ],
                     )
             yield task, total_polcal_files, num_dark_polcal_files
         except:
             raise
         finally:
@@ -459,15 +461,15 @@
     When: Trying to run BackgroundLightCalibration
     Then: An error is raised
     """
     mocker.patch(
         "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
     )
     task = background_light_calibration_task_with_bad_exposure_times
-    with pytest.raises(ValueError, match="do not all have the same exposure time"):
+    with pytest.raises(ValueError, match="do not all have the same FPA exposure time"):
         task()
 
 
 def test_background_light_non_polarimetric_dataset(
     background_light_calibration_task_non_polarimetric_dataset, mocker
 ):
     """
```

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_build_quality_report.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_build_quality_report.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_dark.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_dark.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,27 +23,29 @@
 
 
 @pytest.fixture(scope="function")
 def dark_calibration_task(
     tmp_path, assign_input_dataset_doc_to_task, init_visp_constants_db, recipe_run_id
 ):
     constants_db = VispConstantsDb(
-        LAMP_EXPOSURE_TIMES=(100.0,),
-        SOLAR_EXPOSURE_TIMES=(1.0,),
-        OBSERVE_EXPOSURE_TIMES=(0.01,),
-        POLCAL_EXPOSURE_TIMES=(),
+        LAMP_READOUT_EXP_TIMES=(200.0,),
+        SOLAR_READOUT_EXP_TIMES=(2.0,),
+        OBSERVE_READOUT_EXP_TIMES=(0.02,),
+        POLCAL_READOUT_EXP_TIMES=(),
     )
     init_visp_constants_db(recipe_run_id, constants_db)
     with DarkCalibration(
         recipe_run_id=recipe_run_id, workflow_name="dark_calibration", workflow_version="VX.Y"
     ) as task:
         num_beam = 2
-        exp_times = [0.01, 1.0, 100.0]
-        unused_time = 200.0
-        num_exp_time = len(exp_times)
+        readout_exp_times = [0.02, 2.0, 200.0]
+        num_raw_values = [3, 4, 5]
+        unused_time = 100.0
+        unused_num_raw = 6
+        num_exp_time = len(readout_exp_times)
         num_frames_per = 3
         array_shape = (1, 20, 10)
         dataset_shape = ((num_exp_time + 1) * num_frames_per, 20, 10)
         try:  # This try... block is here to make sure the dbs get cleaned up if there's a failure in the fixture
             task.scratch = WorkflowFileSystem(
                 scratch_base_path=tmp_path, recipe_run_id=recipe_run_id
             )
@@ -56,33 +58,36 @@
             )
             header_generator = (
                 spec122_validator.validate_and_translate_to_214_l0(
                     d.header(), return_type=fits.HDUList
                 )[0].header
                 for d in ds
             )
-            for e in exp_times + [unused_time]:  # Make some darks we won't use
+            for e, n in zip(
+                readout_exp_times + [unused_time], num_raw_values + [unused_num_raw]
+            ):  # Make some darks we won't use
                 for _ in range(num_frames_per):
                     hdul = generate_fits_frame(header_generator=header_generator, shape=array_shape)
+                    hdul[0].header["NSUMEXP"] = n
                     hdul[0].data *= 0
                     # Create combined 2-beam array
                     beam = 1
                     hdul[0].data[0, :beam_border, :] = beam * e
                     beam = 2
                     hdul[0].data[0, beam_border:, :] = beam * e
                     task.fits_data_write(
                         hdu_list=hdul,
                         tags=[
                             VispTag.input(),
                             VispTag.frame(),
                             VispTag.task("DARK"),
-                            VispTag.exposure_time(e),
+                            VispTag.readout_exp_time(e),
                         ],
                     )
-            yield task, num_beam, exp_times, unused_time
+            yield task, num_beam, readout_exp_times, num_raw_values, unused_time
         except:
             raise
         finally:
             task.scratch.purge()
             task.constants._purge()
 
 
@@ -92,42 +97,42 @@
     When: Calling the task instance
     Then: Only one average intermediate dark frame exists for each exposure time and unused times are not made
     """
     mocker.patch(
         "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
     )
     # When
-    task, num_beam, exp_times, unused_time = dark_calibration_task
+    task, num_beam, readout_exp_times, num_raw_frames, unused_time = dark_calibration_task
     task()
     # Then
-    for e in exp_times:
+    for e, n in zip(readout_exp_times, num_raw_frames):
         for b in range(num_beam):
             files = list(
                 task.read(
                     tags=[
                         VispTag.task("DARK"),
                         VispTag.intermediate(),
                         VispTag.frame(),
                         VispTag.beam(b + 1),
-                        VispTag.exposure_time(e),
+                        VispTag.readout_exp_time(e),
                     ]
                 )
             )
             assert len(files) == 1
-            expected = np.ones((10, 10)) * (b + 1) * e
+            expected = np.ones((10, 10)) * (b + 1) * e / n
             hdul = fits.open(files[0])
-            np.testing.assert_equal(expected, hdul[0].data)
+            np.testing.assert_allclose(expected, hdul[0].data, rtol=1e-15)
             hdul.close()
 
     unused_time_read = task.read(
         tags=[
             VispTag.task("DARK"),
             VispTag.intermediate(),
             VispTag.frame(),
-            VispTag.exposure_time(unused_time),
+            VispTag.readout_exp_time(unused_time),
         ]
     )
     assert len(list(unused_time_read)) == 0
 
     quality_files = task.read(tags=[Tag.quality("TASK_TYPES")])
     for file in quality_files:
         with file.open() as f:
```

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_downsample.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_geometric.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_geometric.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 from dataclasses import dataclass
 
 import numpy as np
 import pytest
-from astropy.io import fits
 from dkist_processing_common._util.scratch import WorkflowFileSystem
 from dkist_processing_common.models.tags import Tag
 from dkist_processing_common.tests.conftest import FakeGQLClient
 from dkist_processing_math import transform
 
 from dkist_processing_visp.models.tags import VispTag
 from dkist_processing_visp.tasks.geometric import GeometricCalibration
@@ -30,23 +29,23 @@
     # This fixture makes data that look enough like real data that all of the feature detection stuff at least runs
     # through (mostly this is an issue for the angle calculation). It would be great to contrive data that
     # produce a geometric calibration with real numbers that can be checked, but for now we'll rely on the grogu
     # tests for that. In other words, this fixture just tests if the machinery of the task completes and some object
     # (ANY object) is written correctly.
     number_of_modstates = 3
     number_of_beams = 2
-    solar_exp_time = 20.0  # From VispHeadersValidSolarGainFrames fixture
-    lamp_exp_time = 10.0  # From VispHeadersValidLampGainFrames fixture
+    solar_exp_time = 40.0  # From VispHeadersValidSolarGainFrames fixture
+    lamp_exp_time = 20.0  # From VispHeadersValidLampGainFrames fixture
     intermediate_shape = (30, 100)
     array_shape = (1, 60, 100)
     dataset_shape = array_shape
     constants_db = VispConstantsDb(
         NUM_MODSTATES=number_of_modstates,
-        SOLAR_EXPOSURE_TIMES=(solar_exp_time,),
-        LAMP_EXPOSURE_TIMES=(lamp_exp_time,),
+        SOLAR_READOUT_EXP_TIMES=(solar_exp_time,),
+        LAMP_READOUT_EXP_TIMES=(lamp_exp_time,),
     )
     init_visp_constants_db(recipe_run_id, constants_db)
     with GeometricCalibration(
         recipe_run_id=recipe_run_id, workflow_name="geometric_calibration", workflow_version="VX.Y"
     ) as task:
         try:  # This try... block is here to make sure the dbs get cleaned up if there's a failure in the fixture
             task.scratch = WorkflowFileSystem(
@@ -56,30 +55,31 @@
             task.angles = np.array([0.01, -0.01])
             task.offsets = np.zeros((number_of_beams, number_of_modstates, 2))
             task.shifts = np.zeros(intermediate_shape[0])
             for beam in range(1, number_of_beams + 1):
 
                 dark_cal = np.ones(intermediate_shape) * 3.0
                 task.intermediate_frame_helpers_write_arrays(
-                    arrays=dark_cal, beam=beam, task="DARK", exposure_time=solar_exp_time
+                    arrays=dark_cal, beam=beam, task="DARK", readout_exp_time=solar_exp_time
                 )
 
                 task.intermediate_frame_helpers_write_arrays(
-                    arrays=dark_cal, beam=beam, task="DARK", exposure_time=lamp_exp_time
+                    arrays=dark_cal, beam=beam, task="DARK", readout_exp_time=lamp_exp_time
                 )
 
                 for modstate in range(1, number_of_modstates + 1):
                     solar_ds = VispHeadersValidSolarGainFrames(
                         dataset_shape=dataset_shape,
                         array_shape=array_shape,
                         time_delta=10,
                         num_modstates=number_of_modstates,
                         modstate=modstate,
                     )
                     solar_header = solar_ds.header()
+                    solar_num_raw_per_fpa = solar_header["CAM__014"]
                     true_solar = 10 * (np.ones(array_shape[1:]) + modstate + beam)
                     translated_solar = next(
                         transform.translate_arrays(
                             arrays=true_solar, translation=task.offsets[beam - 1][modstate - 1]
                         )
                     )
                     translated_solar[translated_solar == 0] = 10 * (modstate + beam + 1)
@@ -89,38 +89,39 @@
                     translated_solar[:, 70] = 5.0
                     distorted_solar = next(
                         transform.rotate_arrays_about_point(
                             arrays=translated_solar, angle=task.angles[beam - 1]
                         )
                     )
                     raw_dark = np.concatenate((dark_cal, dark_cal))
-                    raw_solar = distorted_solar + raw_dark
+                    raw_solar = (distorted_solar + raw_dark) * solar_num_raw_per_fpa
                     solar_hdul = generate_214_l0_fits_frame(
                         data=raw_solar, s122_header=solar_header
                     )
                     task.fits_data_write(
                         hdu_list=solar_hdul,
                         tags=[
                             VispTag.input(),
                             VispTag.task("SOLAR_GAIN"),
                             VispTag.modstate(modstate),
                             VispTag.frame(),
                             VispTag.beam(beam),
-                            VispTag.exposure_time(solar_exp_time),
+                            VispTag.readout_exp_time(solar_exp_time),
                         ],
                     )
 
                     lamp_ds = VispHeadersValidLampGainFrames(
                         dataset_shape=dataset_shape,
                         array_shape=array_shape,
                         time_delta=10,
                         num_modstates=number_of_modstates,
                         modstate=modstate,
                     )
                     lamp_header = lamp_ds.header()
+                    lamp_num_raw_per_fpa = lamp_header["CAM__014"]
                     true_lamp = 10 * (np.ones(array_shape[1:]) + modstate + beam)
                     translated_lamp = next(
                         transform.translate_arrays(
                             arrays=true_lamp, translation=task.offsets[beam - 1][modstate - 1]
                         )
                     )
                     translated_lamp[translated_lamp == 0] = 10 * (modstate + beam + 1)
@@ -131,25 +132,25 @@
                     # Chop out part of the second hairline so the fitter has to skip over these pixels
                     translated_lamp[5:9, 70] = 10 * (modstate + beam + 1)
                     distorted_lamp = next(
                         transform.rotate_arrays_about_point(
                             arrays=translated_lamp, angle=task.angles[beam - 1]
                         )
                     )
-                    raw_lamp = distorted_lamp + raw_dark
+                    raw_lamp = (distorted_lamp + raw_dark) * lamp_num_raw_per_fpa
                     lamp_hdul = generate_214_l0_fits_frame(data=raw_lamp, s122_header=lamp_header)
                     task.fits_data_write(
                         hdu_list=lamp_hdul,
                         tags=[
                             VispTag.input(),
                             VispTag.task("LAMP_GAIN"),
                             VispTag.modstate(modstate),
                             VispTag.frame(),
                             VispTag.beam(beam),
-                            VispTag.exposure_time(lamp_exp_time),
+                            VispTag.readout_exp_time(lamp_exp_time),
                         ],
                     )
 
             yield task
         except:
             raise
         finally:
@@ -164,48 +165,48 @@
 
 @pytest.fixture(scope="function")
 def geometric_calibration_task_with_simple_raw_data(
     tmp_path, recipe_run_id, assign_input_dataset_doc_to_task, init_visp_constants_db
 ):
     number_of_modstates = 3
     number_of_beams = 2
-    solar_exp_time = 20.0  # From VispHeadersValidSolarGainFrames fixture
-    lamp_exp_time = 10.0  # From VispHeadersValidLampGainFrames fixture
+    solar_exp_time = 40.0  # From VispHeadersValidSolarGainFrames fixture
+    lamp_exp_time = 20.0  # From VispHeadersValidLampGainFrames fixture
     data_shape_int = (10, 10)
     data_shape_raw = (20, 10)
     constants_db = VispConstantsDb(
         NUM_MODSTATES=number_of_modstates,
-        SOLAR_EXPOSURE_TIMES=(solar_exp_time,),
-        LAMP_EXPOSURE_TIMES=(lamp_exp_time,),
+        SOLAR_READOUT_EXP_TIMES=(solar_exp_time,),
+        LAMP_READOUT_EXP_TIMES=(lamp_exp_time,),
     )
     init_visp_constants_db(recipe_run_id, constants_db)
     with GeometricCalibration(
         recipe_run_id=recipe_run_id, workflow_name="geometric_calibration", workflow_version="VX.Y"
     ) as task:
         task.scratch = WorkflowFileSystem(scratch_base_path=tmp_path, recipe_run_id=recipe_run_id)
         assign_input_dataset_doc_to_task(task, VispGeoTestingParameters10())
 
         # Create the intermediate frames needed
         for beam in range(1, number_of_beams + 1):
 
             dark_cal = np.ones(data_shape_int) * 3.0
             task.intermediate_frame_helpers_write_arrays(
-                arrays=dark_cal, beam=beam, task="DARK", exposure_time=solar_exp_time
+                arrays=dark_cal, beam=beam, task="DARK", readout_exp_time=solar_exp_time
             )
 
             task.intermediate_frame_helpers_write_arrays(
-                arrays=dark_cal, beam=beam, task="DARK", exposure_time=lamp_exp_time
+                arrays=dark_cal, beam=beam, task="DARK", readout_exp_time=lamp_exp_time
             )
 
             # Let's write a dark with the wrong exposure time, just to make sure it doesn't get used
             task.intermediate_frame_helpers_write_arrays(
                 arrays=np.ones(data_shape_int) * 1e6,
                 beam=beam,
                 task="DARK",
-                exposure_time=solar_exp_time**2,
+                readout_exp_time=solar_exp_time**2,
             )
 
         # Create the raw data, which is based on two beams per frame
         beam1 = 1
         beam2 = 2
         dark_cal_two_beams = np.concatenate((dark_cal, dark_cal))
         for modstate in range(1, number_of_modstates + 1):
@@ -215,54 +216,56 @@
                 dataset_shape=(1,) + data_shape_raw,
                 array_shape=(1,) + data_shape_raw,
                 time_delta=10,
                 num_modstates=number_of_modstates,
                 modstate=modstate,
             )
             solar_header = solar_ds.header()
+            solar_num_raw_per_fpa = solar_header["CAM__014"]
             true_solar = np.ones(data_shape_raw) + modstate
             # Now add the beam number to each beam in the array
             true_solar[: task.parameters.beam_border, :] += beam1
             true_solar[task.parameters.beam_border :, :] += beam2
-            raw_solar = true_solar + dark_cal_two_beams
+            raw_solar = (true_solar + dark_cal_two_beams) * solar_num_raw_per_fpa
             solar_hdul = generate_214_l0_fits_frame(data=raw_solar, s122_header=solar_header)
             task.fits_data_write(
                 hdu_list=solar_hdul,
                 tags=[
                     VispTag.input(),
                     VispTag.task("SOLAR_GAIN"),
                     VispTag.modstate(modstate),
                     VispTag.frame(),
-                    VispTag.exposure_time(solar_exp_time),
+                    VispTag.readout_exp_time(solar_exp_time),
                 ],
             )
 
             # Lamp
             lamp_ds = VispHeadersValidLampGainFrames(
                 dataset_shape=(1,) + data_shape_raw,
                 array_shape=(1,) + data_shape_raw,
                 time_delta=10,
                 num_modstates=number_of_modstates,
                 modstate=modstate,
             )
             lamp_header = lamp_ds.header()
+            lamp_num_raw_per_fpa = lamp_header["CAM__014"]
             true_lamp = np.ones(data_shape_raw) + modstate
             # Now add the beam number to each beam in the array
             true_lamp[: task.parameters.beam_border, :] += beam1
             true_lamp[task.parameters.beam_border :, :] += beam2
-            raw_lamp = true_lamp + dark_cal_two_beams
+            raw_lamp = (true_lamp + dark_cal_two_beams) * lamp_num_raw_per_fpa
             lamp_hdul = generate_214_l0_fits_frame(data=raw_lamp, s122_header=lamp_header)
             task.fits_data_write(
                 hdu_list=lamp_hdul,
                 tags=[
                     VispTag.input(),
                     VispTag.task("LAMP_GAIN"),
                     VispTag.modstate(modstate),
                     VispTag.frame(),
-                    VispTag.exposure_time(lamp_exp_time),
+                    VispTag.readout_exp_time(lamp_exp_time),
                 ],
             )
 
         yield task
         task.scratch.purge()
         task.constants._purge()
```

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_instrument_polarization.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_instrument_polarization.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,26 +63,26 @@
     init_visp_constants_db,
     mocker,
     background_on,
 ):
     num_beams = 2
     num_modstates = 2
     num_cs_steps = 2
-    exposure_time = 0.01  # From VispHeadersValidPolcalFrames fixture
+    readout_exp_time = 0.02  # From VispHeadersValidPolcalFrames fixture
     intermediate_shape = (10, 10)
     dataset_shape = (num_cs_steps, 20, 10)
     array_shape = (1, 20, 10)
     spatial_size = array_shape[-1]
     spectral_size = array_shape[-2] // 2  # Divide by two for a single beam
     constants_db = VispConstantsDb(
         POLARIMETER_MODE="observe_polarimetric",
         NUM_MODSTATES=num_modstates,
         NUM_BEAMS=num_beams,
         NUM_CS_STEPS=num_cs_steps,
-        POLCAL_EXPOSURE_TIMES=(exposure_time,),
+        POLCAL_READOUT_EXP_TIMES=(readout_exp_time,),
     )
     init_visp_constants_db(recipe_run_id, constants_db)
     with InstrumentPolarizationCalibration(
         recipe_run_id=recipe_run_id,
         workflow_name="instrument_polarization_calibration",
         workflow_version="VX.Y",
     ) as task:
@@ -120,15 +120,15 @@
                     task.intermediate_frame_helpers_write_arrays(
                         arrays=offset, beam=beam, modstate=modstate, task="GEOMETRIC_OFFSET"
                     )
 
             # Create fake dark and background intermediate arrays
             for beam in range(1, num_beams + 1):
                 task.intermediate_frame_helpers_write_arrays(
-                    all_zeros, beam=beam, task="DARK", exposure_time=exposure_time
+                    all_zeros, beam=beam, task="DARK", readout_exp_time=readout_exp_time
                 )
 
                 if background_on:
                     # BackgroundLight object
                     task.intermediate_frame_helpers_write_arrays(
                         arrays=all_zeros, beam=beam, task="BACKGROUND"
                     )
@@ -141,15 +141,15 @@
                         hdu_list=gain_hdul,
                         tags=[
                             VispTag.intermediate(),
                             VispTag.frame(),
                             VispTag.task("SOLAR_GAIN"),
                             VispTag.beam(beam),
                             VispTag.modstate(modstate),
-                            VispTag.exposure_time(exposure_time),
+                            VispTag.readout_exp_time(readout_exp_time),
                         ],
                     )
 
             start_time = datetime.now()
             for modstate in range(1, num_modstates + 1):
                 # Create polcal input frames for this modstate
                 ds = VispHeadersValidPolcalFrames(
@@ -173,15 +173,15 @@
                         hdu_list=hdul,
                         tags=[
                             VispTag.task("POLCAL"),
                             VispTag.modstate(modstate),
                             VispTag.cs_step(cs_step),
                             VispTag.input(),
                             VispTag.frame(),
-                            VispTag.exposure_time(exposure_time),
+                            VispTag.readout_exp_time(readout_exp_time),
                         ],
                     )
 
             yield task, quality_metric_mocker, spectral_size, spatial_size, num_modstates
         except:
             raise
         finally:
```

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_lamp.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_lamp.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,24 +23,27 @@
 @dataclass
 class VispLampTestingParameters(VispTestingParameters):
     visp_beam_border: int = 10
 
 
 @pytest.fixture(scope="function")
 def lamp_calibration_task(
-    tmp_path, recipe_run_id, assign_input_dataset_doc_to_task, init_visp_constants_db, mocker
+    tmp_path,
+    recipe_run_id,
+    assign_input_dataset_doc_to_task,
+    init_visp_constants_db,
 ):
     number_of_modstates = 2
     number_of_beams = 2
-    exposure_time = 10.0  # From VispHeadersValidLampGainFrames fixture
+    readout_exp_time = 20.0  # From VispHeadersValidLampGainFrames fixture
     dataset_shape = (number_of_modstates, 20, 10)
     array_shape = (1, 20, 10)
     intermediate_shape = (10, 10)
     constants_db = VispConstantsDb(
-        NUM_MODSTATES=number_of_modstates, LAMP_EXPOSURE_TIMES=(exposure_time,)
+        NUM_MODSTATES=number_of_modstates, LAMP_READOUT_EXP_TIMES=(readout_exp_time,)
     )
     init_visp_constants_db(recipe_run_id, constants_db)
     with LampCalibration(
         recipe_run_id=recipe_run_id, workflow_name="lamp_gain_calibration", workflow_version="VX.Y"
     ) as task:
         try:  # This try... block is here to make sure the dbs get cleaned up if there's a failure in the fixture
             task.scratch = WorkflowFileSystem(
@@ -51,15 +54,15 @@
             dark_signal = 3.0
             start_time = datetime.now()
             # Make intermediate dark frame
             dark_cal = np.ones(intermediate_shape) * dark_signal
             # Need a dark for each beam
             for b in range(number_of_beams):
                 task.intermediate_frame_helpers_write_arrays(
-                    arrays=dark_cal, beam=b + 1, task="DARK", exposure_time=exposure_time
+                    arrays=dark_cal, beam=b + 1, task="DARK", readout_exp_time=readout_exp_time
                 )
             # These images are for two combined beams
             for i in range(number_of_modstates):
                 ds = VispHeadersValidLampGainFrames(
                     dataset_shape=dataset_shape,
                     array_shape=array_shape,
                     time_delta=10,
@@ -70,25 +73,26 @@
                 header_generator = (
                     spec122_validator.validate_and_translate_to_214_l0(
                         d.header(), return_type=fits.HDUList
                     )[0].header
                     for d in ds
                 )
                 hdul = generate_fits_frame(header_generator=header_generator, shape=array_shape)
+                num_raw_frames_per_fpa = hdul[0].header["NSUMEXP"]
                 # Tweak data so that beam sides are slightly different
-                hdul[0].data[0, :beam_border, :] = 1.1 + dark_signal
-                hdul[0].data[0, beam_border:, :] = 1.2 + dark_signal
+                hdul[0].data[0, :beam_border, :] = (1.1 + dark_signal) * num_raw_frames_per_fpa
+                hdul[0].data[0, beam_border:, :] = (1.2 + dark_signal) * num_raw_frames_per_fpa
                 task.fits_data_write(
                     hdu_list=hdul,
                     tags=[
                         VispTag.input(),
                         VispTag.task("LAMP_GAIN"),
                         VispTag.modstate(i + 1),
                         VispTag.frame(),
-                        VispTag.exposure_time(exposure_time),
+                        VispTag.readout_exp_time(readout_exp_time),
                     ],
                 )
             yield task, number_of_modstates, number_of_beams
         except:
             raise
         finally:
             task.scratch.purge()
```

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_make_movie_frames.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_map_repeats.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_map_repeats.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_parameters.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_parse.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,15 @@
                             num_modstates=num_modstates,
                             modstate=m,
                             polarimeter_mode="observe_polarimetric",
                             start_time=start_time + i * time_delta,
                         )
                         header = next(ds).header()
                         header["CAM__004"] = [0.02, 0.03][m % 2]
+                        header["CAM__005"] = [0.04, 0.06][m % 2]
                         translated_header = translate_spec122_to_spec214_l0(header)
                         hdu = fits.PrimaryHDU(
                             data=np.ones((1, 2, 2)), header=fits.Header(translated_header)
                         )
                         hdul = fits.HDUList([hdu])
                         task.fits_data_write(hdu_list=hdul, tags=[Tag.input(), Tag.frame()])
                         i += 1
@@ -361,14 +362,19 @@
     assert parse_inputs_valid_task.constants._db_dict["NUM_RASTER_STEPS"] == 3
     assert parse_inputs_valid_task.constants._db_dict["WAVELENGTH"] == 656.28
     assert parse_inputs_valid_task.constants._db_dict["DARK_EXPOSURE_TIMES"] == [1.0]
     assert parse_inputs_valid_task.constants._db_dict["LAMP_EXPOSURE_TIMES"] == [10.0]
     assert parse_inputs_valid_task.constants._db_dict["SOLAR_EXPOSURE_TIMES"] == [20.0]
     assert parse_inputs_valid_task.constants._db_dict["POLCAL_EXPOSURE_TIMES"] == [0.01]
     assert parse_inputs_valid_task.constants._db_dict["OBSERVE_EXPOSURE_TIMES"] == [0.02, 0.03]
+    assert parse_inputs_valid_task.constants._db_dict["DARK_READOUT_EXP_TIMES"] == [2.0]
+    assert parse_inputs_valid_task.constants._db_dict["LAMP_READOUT_EXP_TIMES"] == [20.0]
+    assert parse_inputs_valid_task.constants._db_dict["SOLAR_READOUT_EXP_TIMES"] == [40.0]
+    assert parse_inputs_valid_task.constants._db_dict["POLCAL_READOUT_EXP_TIMES"] == [0.02]
+    assert parse_inputs_valid_task.constants._db_dict["OBSERVE_READOUT_EXP_TIMES"] == [0.04, 0.06]
 
 
 def test_parse_visp_values(parse_inputs_valid_task, mocker):
     """
     :Given: A valid parse input task
     :When: Calling the task instance
     :Then: Values are correctly loaded into the constants mutable mapping
```

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_quality.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_science.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_science.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     init_visp_constants_db,
     request,
     background_on,
 ):
     num_map_scans = 2
     num_beams = 2
     num_raster_steps = 2
-    exposure_time = 0.02  # From VispHeadersValidObserveFrames fixture
+    readout_exp_time = 0.04  # From VispHeadersValidObserveFrames fixture
     if request.param == "Full Stokes":
         num_modstates = 2
         polarimeter_mode = "observe_polarimetric"
     else:
         num_modstates = 1
         polarimeter_mode = "observe_intensity"
     array_shape = (1, 50, 20)
@@ -56,15 +56,15 @@
 
     constants_db = VispConstantsDb(
         POLARIMETER_MODE=polarimeter_mode,
         NUM_MODSTATES=num_modstates,
         NUM_MAP_SCANS=num_map_scans,
         NUM_RASTER_STEPS=num_raster_steps,
         NUM_BEAMS=num_beams,
-        OBSERVE_EXPOSURE_TIMES=(exposure_time,),
+        OBSERVE_READOUT_EXP_TIMES=(readout_exp_time,),
     )
     init_visp_constants_db(recipe_run_id, constants_db)
     with ScienceCalibration(
         recipe_run_id=recipe_run_id, workflow_name="science_calibration", workflow_version="VX.Y"
     ) as task:
         try:  # This try... block is here to make sure the dbs get cleaned up if there's a failure in the fixture
             all_zeros = np.zeros(intermediate_shape)
@@ -109,15 +109,15 @@
                         modstate=modstate,
                         task="GEOMETRIC_OFFSET",
                     )
 
             # Create fake dark intermediate arrays
             for beam in range(1, num_beams + 1):
                 task.intermediate_frame_helpers_write_arrays(
-                    all_zeros, beam=beam, task="DARK", exposure_time=exposure_time
+                    all_zeros, beam=beam, task="DARK", readout_exp_time=readout_exp_time
                 )
 
                 if request.param == "Full Stokes" and background_on:
                     # BackgroundLight object
                     task.intermediate_frame_helpers_write_arrays(
                         arrays=all_zeros, beam=beam, task="BACKGROUND"
                     )
@@ -168,26 +168,54 @@
                             tags=[
                                 VispTag.task("OBSERVE"),
                                 VispTag.raster_step(raster_step),
                                 VispTag.map_scan(map_scan),
                                 VispTag.modstate(modstate),
                                 VispTag.input(),
                                 VispTag.frame(),
-                                VispTag.exposure_time(exposure_time),
+                                VispTag.readout_exp_time(readout_exp_time),
                             ],
                         )
 
             yield task, request.param, offset, header, intermediate_shape
         except:
             raise
         finally:
             task.scratch.purge()
             task.constants._purge()
 
 
+@pytest.fixture(scope="function")
+def dummy_calibration_collection():
+    intermediate_shape = (25, 20)
+    array_shape = (50, 20)
+
+    beam = 1
+    modstate = 1
+
+    dark_dict = {VispTag.beam(beam): {VispTag.readout_exp_time(0.04): np.zeros(intermediate_shape)}}
+    background_dict = {VispTag.beam(beam): np.zeros(intermediate_shape)}
+    solar_dict = {VispTag.beam(beam): {VispTag.modstate(modstate): np.ones(intermediate_shape)}}
+    angle_dict = {VispTag.beam(beam): 0.0}
+    spec_dict = {VispTag.beam(beam): np.zeros(intermediate_shape[1])}
+    offset_dict = {VispTag.beam(beam): {VispTag.modstate(modstate): np.zeros(2)}}
+
+    collection = CalibrationCollection(
+        dark=dark_dict,
+        background=background_dict,
+        solar_gain=solar_dict,
+        angle=angle_dict,
+        spec_shift=spec_dict,
+        state_offset=offset_dict,
+        demod_matrices=None,
+    )
+
+    return collection, intermediate_shape, array_shape
+
+
 @pytest.fixture(scope="session")
 def headers_with_dates() -> tuple[list[fits.Header], str, int, int]:
     num_headers = 5
     start_time = "1969-12-06T18:00:00"
     exp_time = 12
     time_delta = 10
     ds = VispHeadersValidObserveFrames(
@@ -247,14 +275,15 @@
     if request.param == "Full Stokes":
         polarimeter_mode = "observe_polarimetric"
     else:
         polarimeter_mode = "observe_intensity"
 
     constants_db = VispConstantsDb(
         POLARIMETER_MODE=polarimeter_mode,
+        OBSERVE_READOUT_EXP_TIMES=(0.04,),
     )
     init_visp_constants_db(recipe_run_id, constants_db)
     with ScienceCalibration(
         recipe_run_id=recipe_run_id, workflow_name="science_calibration", workflow_version="VX.Y"
     ) as task:
         try:
             yield task
@@ -368,14 +397,74 @@
             data = json.load(f)
             assert isinstance(data, dict)
             assert data["total_frames"] == task.scratch.count_all(
                 tags=[VispTag.input(), VispTag.frame(), VispTag.task("OBSERVE")]
             )
 
 
+def test_readout_normalization_correct(
+    science_calibration_task_no_data, dummy_calibration_collection, assign_input_dataset_doc_to_task
+):
+    """
+    Given: A ScienceCalibration task with associated observe frames
+    When: Correcting a single array
+    Then: The correct normalization by the number of readouts per FPA is performed
+    """
+    task = science_calibration_task_no_data
+    corrections, intermediate_shape, array_shape = dummy_calibration_collection
+    assign_input_dataset_doc_to_task(task, VispScienceTestingParameters())
+    # Assign a single input observe frame
+    ds = VispHeadersValidObserveFrames(
+        dataset_shape=(1, *array_shape),
+        array_shape=(1, *array_shape),
+        time_delta=10,
+        num_raster_steps=1,
+        raster_step=1,
+        num_modstates=1,
+        modstate=1,
+        start_time=datetime.now(),
+    )
+    header_generator = (
+        spec122_validator.validate_and_translate_to_214_l0(d.header(), return_type=fits.HDUList)[
+            0
+        ].header
+        for d in ds
+    )
+
+    hdul = generate_fits_frame(header_generator=header_generator, shape=array_shape)
+    num_raw_per_fpa = hdul[0].header["CAM__014"]
+    hdul[0].data = np.ones(array_shape) * 100.0 * num_raw_per_fpa
+    readout_exp_time = task.constants.observe_readout_exp_times[0]
+    task.fits_data_write(
+        hdu_list=hdul,
+        tags=[
+            VispTag.task("OBSERVE"),
+            VispTag.raster_step(1),
+            VispTag.map_scan(1),
+            VispTag.modstate(1),
+            VispTag.input(),
+            VispTag.frame(),
+            VispTag.readout_exp_time(readout_exp_time),
+        ],
+    )
+
+    # When:
+    corrected_array, _ = task.correct_single_frame(
+        beam=1,
+        modstate=1,
+        raster_step=1,
+        map_scan=1,
+        readout_exp_time=readout_exp_time,
+        calibrations=corrections,
+    )
+
+    expected = np.ones(intermediate_shape) * 100.0
+    np.testing.assert_allclose(corrected_array, expected, rtol=1e-15)
+
+
 def test_compute_date_keys(headers_with_dates, recipe_run_id, init_visp_constants_db):
     """
     Given: A set of headers with different DATE-OBS values
     When: Computing the time over which the headers were taken
     Then: A header with correct DATE-BEG, DATE-END, and DATE-AVG keys is returned
     """
     headers, start_time, exp_time, time_delta = headers_with_dates
```

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_solar.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_solar.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,20 +27,20 @@
     recipe_run_id,
     assign_input_dataset_doc_to_task,
     init_visp_constants_db,
     background_on,
 ):
     number_of_modstates = 3
     number_of_beams = 2
-    exposure_time = 20.0  # From VispHeadersValidSolarGainFrames fixture
+    readout_exp_time = 40.0  # From VispHeadersValidSolarGainFrames fixture
     intermediate_shape = (10, 10)
     dataset_shape = (1, 20, 10)
     array_shape = (1, 20, 10)
     constants_db = VispConstantsDb(
-        NUM_MODSTATES=number_of_modstates, SOLAR_EXPOSURE_TIMES=(exposure_time,)
+        NUM_MODSTATES=number_of_modstates, SOLAR_READOUT_EXP_TIMES=(readout_exp_time,)
     )
     init_visp_constants_db(recipe_run_id, constants_db)
     with SolarCalibration(
         recipe_run_id=recipe_run_id, workflow_name="geometric_calibration", workflow_version="VX.Y"
     ) as task:
         try:  # This try... block is here to make sure the dbs get cleaned up if there's a failure in the fixture
             task.scratch = WorkflowFileSystem(
@@ -55,15 +55,15 @@
             # I'm so sorry; this is kind of a hack because I didn't want to refactor this whole nested loop.
             raw_solar_dict = defaultdict(dict)
             for beam in range(1, number_of_beams + 1):
 
                 # DarkCal object
                 dark_cal = np.ones(intermediate_shape) * 3.0
                 task.intermediate_frame_helpers_write_arrays(
-                    arrays=dark_cal, beam=beam, task="DARK", exposure_time=exposure_time
+                    arrays=dark_cal, beam=beam, task="DARK", readout_exp_time=readout_exp_time
                 )
 
                 if background_on:
                     # BackgroundLight object
                     bg_cal = np.zeros(intermediate_shape)
                     task.intermediate_frame_helpers_write_arrays(
                         arrays=bg_cal, beam=beam, task="BACKGROUND"
@@ -100,26 +100,28 @@
                     dataset_shape=dataset_shape,
                     array_shape=array_shape,
                     time_delta=10,
                     num_modstates=number_of_modstates,
                     modstate=modstate,
                 )
                 header = ds.header()
-                raw_solar_array = np.concatenate(
-                    (raw_solar_dict[1][modstate], raw_solar_dict[2][modstate])
+                num_raw_per_fpa = header["CAM__014"]
+                raw_solar_array = (
+                    np.concatenate((raw_solar_dict[1][modstate], raw_solar_dict[2][modstate]))
+                    * num_raw_per_fpa
                 )
                 solar_hdul = generate_214_l0_fits_frame(data=raw_solar_array, s122_header=header)
                 task.fits_data_write(
                     hdu_list=solar_hdul,
                     tags=[
                         VispTag.input(),
                         VispTag.task("SOLAR_GAIN"),
                         VispTag.modstate(modstate),
                         VispTag.frame(),
-                        VispTag.exposure_time(exposure_time),
+                        VispTag.readout_exp_time(readout_exp_time),
                     ],
                 )
 
             yield task
         except:
             raise
         finally:
```

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_submit_quality.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_submit_quality.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_trial_output_data.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_trial_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_visp_base.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_visp_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     init_visp_constants_db(recipe_run_id, VispConstantsDb())
     task = Task(
         recipe_run_id=recipe_run_id,
         workflow_name="parse_visp_input_data",
         workflow_version="VX.Y",
     )
     task._scratch = WorkflowFileSystem(scratch_base_path=tmpdir_factory.mktemp("data"))
-    tag_names = [["beam"], ["exposure_time", "task"], ["modstate"]]
+    tag_names = [["beam"], ["readout_exp_time", "task"], ["modstate"]]
     tag_vals = [[1], [10.23, "dark"], [3]]
     tag_fcns = [[getattr(VispTag, n) for n in nl] for nl in tag_names]
     tag_list = [[f(v) for f, v in zip(fl, vl)] for fl, vl in zip(tag_fcns, tag_vals)]
     for i, tags in enumerate(tag_list):
         hdul = fits.HDUList([fits.PrimaryHDU(data=np.ones((2, 2)) * i)])
         fname = task.scratch.workflow_base_path / f"file{i}.fits"
         hdul.writeto(fname)
```

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_visp_constants.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_visp_constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,17 @@
     num_cs_steps: int = 18
     num_raster_steps: int = 1000
     polarimeter_mode: str = "observe_polarimetric"
     wavelength: float = 666.6
     lamp_exposure_times: tuple[float] = (100.0,)
     solar_exposure_times: tuple[float] = (1.0,)
     observe_exposure_times: tuple[float] = (0.01,)
+    lamp_readout_exp_times: tuple[float] = (200.0,)
+    solar_readout_exp_times: tuple[float] = (2.0,)
+    observe_readout_exp_times: tuple[float] = (0.02,)
     # We don't need all the common ones, but let's put one just to check
     instrument: str = "CHECK_OUT_THIS_INSTRUMENT"
 
 
 @pytest.fixture(scope="session")
 def expected_constant_dict() -> dict:
     lower_dict = asdict(testing_constants())
```

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/tests/test_write_l1.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/workflows/l0_processing.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/workflows/l0_processing.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp/workflows/trial_workflows.py` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp/workflows/trial_workflows.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp.egg-info/PKG-INFO` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-visp
-Version: 2.6.3
+Version: 2.7.0rc1
 Summary: Science processing code for the ViSP instrument on DKIST
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-visp/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/visp
 Classifier: Programming Language :: Python
```

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp.egg-info/SOURCES.txt` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 check_changelog_updated.sh
 pyproject.toml
 science_towncrier.sh
 setup.cfg
 setup.py
 towncrier_science.toml
 changelog/.gitempty
+changelog/123.bugfix.rst
 dkist_processing_visp/__init__.py
 dkist_processing_visp.egg-info/PKG-INFO
 dkist_processing_visp.egg-info/SOURCES.txt
 dkist_processing_visp.egg-info/dependency_links.txt
 dkist_processing_visp.egg-info/requires.txt
 dkist_processing_visp.egg-info/top_level.txt
 dkist_processing_visp/fonts/Lato-Regular.ttf
```

### Comparing `dkist_processing_visp-2.6.3/dkist_processing_visp.egg-info/requires.txt` & `dkist_processing_visp-2.7.0rc1/dkist_processing_visp.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-dkist-processing-common==4.0.3
+dkist-processing-common==4.1.0rc5
 dkist-processing-math==2.0.0
 dkist-processing-pac==3.0.0
 dkist-header-validator==4.1.0
 dkist-fits-specifications==3.7.1
 astropy==5.3.0
 numpy==1.24.3
 sunpy==5.0.0
```

### Comparing `dkist_processing_visp-2.6.3/docs/Makefile` & `dkist_processing_visp-2.7.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/docs/background_light.rst` & `dkist_processing_visp-2.7.0rc1/docs/background_light.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/docs/conf.py` & `dkist_processing_visp-2.7.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/docs/gain_correction.rst` & `dkist_processing_visp-2.7.0rc1/docs/gain_correction.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/docs/l0_to_l1_visp.rst` & `dkist_processing_visp-2.7.0rc1/docs/l0_to_l1_visp.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/docs/make.bat` & `dkist_processing_visp-2.7.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/docs/polarization_calibration.rst` & `dkist_processing_visp-2.7.0rc1/docs/polarization_calibration.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/docs/science_calibration.rst` & `dkist_processing_visp-2.7.0rc1/docs/science_calibration.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/licenses/LICENSE.rst` & `dkist_processing_visp-2.7.0rc1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/pyproject.toml` & `dkist_processing_visp-2.7.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.3/setup.cfg` & `dkist_processing_visp-2.7.0rc1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [options]
 python_requires = >=3.11
 setup_requires = setuptools_scm
 packages = find:
 include_package_data = True
 install_requires = 
-	dkist-processing-common == 4.0.3
+	dkist-processing-common == 4.1.0rc5
 	dkist-processing-math == 2.0.0
 	dkist-processing-pac == 3.0.0
 	dkist-header-validator == 4.1.0
 	dkist-fits-specifications == 3.7.1
 	astropy == 5.3.0
 	numpy == 1.24.3
 	sunpy == 5.0.0
```

