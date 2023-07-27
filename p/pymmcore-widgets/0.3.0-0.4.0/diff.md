# Comparing `tmp/pymmcore-widgets-0.3.0.tar.gz` & `tmp/pymmcore-widgets-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymmcore-widgets-0.3.0.tar", last modified: Thu Jan 19 21:45:44 2023, max compression
+gzip compressed data, was "pymmcore-widgets-0.4.0.tar", last modified: Thu Jul 27 22:56:11 2023, max compression
```

## Comparing `pymmcore-widgets-0.3.0.tar` & `pymmcore-widgets-0.4.0.tar`

### file list

```diff
@@ -1,127 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 21:45:44.607253 pymmcore-widgets-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 21:45:44.599253 pymmcore-widgets-0.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 21:45:44.599253 pymmcore-widgets-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/.github/workflows/cron.yml
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/.github_changelog_generator
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-01-19 21:45:44.607253 pymmcore-widgets-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 21:45:44.599253 pymmcore-widgets-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/docs/_gen_widget_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/docs/_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 21:45:44.599253 pymmcore-widgets-0.3.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/docs/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 21:45:44.599253 pymmcore-widgets-0.3.0/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/docs/stylesheets/extra.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 21:45:44.599253 pymmcore-widgets-0.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/examples/camera_roi_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/examples/channel_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/examples/configuration_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/examples/default_camera_exposure_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/examples/device_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/examples/exposure_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/examples/group_preset_table_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/examples/image_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/examples/live_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/examples/mda_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/examples/objectives_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/examples/pixel_size_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/examples/position_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/examples/presets_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/examples/properties_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/examples/property_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/examples/property_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/examples/sample_explorer_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/examples/shutters_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/examples/snap_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/examples/stage_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/examples/state_device_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/examples/time_plan_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/examples/z_stack_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-19 21:45:44.607253 pymmcore-widgets-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 21:45:44.595253 pymmcore-widgets-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 21:45:44.603253 pymmcore-widgets-0.3.0/src/pymmcore_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17056 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_camera_roi_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_channel_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_device_property_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_device_type_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_device_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_exposure_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 21:45:44.603253 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_group_preset_widget/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_group_preset_widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_group_preset_widget/_add_first_preset_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_group_preset_widget/_add_group_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_group_preset_widget/_add_preset_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_group_preset_widget/_edit_group_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_group_preset_widget/_edit_preset_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    15295 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_group_preset_widget/_group_preset_table_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_image_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_live_button_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_load_system_cfg_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 21:45:44.607253 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_mda/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_mda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_mda/_channel_table_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_mda/_general_mda_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_mda/_grid_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    12076 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_mda/_mda_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_mda/_positions_table_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    15945 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_mda/_sample_explorer_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_mda/_time_plan_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_mda/_zstack_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_objective_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    20705 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_pixel_size_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    11485 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_presets_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_properties_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_property_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)    13905 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_property_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    12934 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_shutter_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_snap_button_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_stage_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 21:45:44.603253 pymmcore-widgets-0.3.0/src/pymmcore_widgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-01-19 21:45:44.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-01-19 21:45:44.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 21:45:44.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 21:45:44.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-01-19 21:45:44.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-19 21:45:44.000000 pymmcore-widgets-0.3.0/src/pymmcore_widgets.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 21:45:44.607253 pymmcore-widgets-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/tests/test_camera_roi_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/tests/test_channel_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/tests/test_combo_message_box_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/tests/test_config.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/tests/test_device_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/tests/test_exposure_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     9970 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/tests/test_group_preset_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/tests/test_image_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/tests/test_live_button.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/tests/test_load_system_cfg_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/tests/test_mda_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/tests/test_objective_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/tests/test_position_table_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/tests/test_presets_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/tests/test_prop_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/tests/test_properties_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/tests/test_property_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/tests/test_sample_explorer_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     9603 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/tests/test_shutter_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/tests/test_snap_button_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/tests/test_stage_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/tests/test_table_pixel_size_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-01-19 21:45:26.000000 pymmcore-widgets-0.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:56:11.267498 pymmcore-widgets-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:56:11.255498 pymmcore-widgets-0.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:56:11.255498 pymmcore-widgets-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/.github/workflows/cron.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/.github_changelog_generator
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-27 22:56:11.267498 pymmcore-widgets-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:56:11.255498 pymmcore-widgets-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/docs/_gen_widget_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/docs/_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:56:11.255498 pymmcore-widgets-0.4.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/docs/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:56:11.255498 pymmcore-widgets-0.4.0/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/docs/stylesheets/extra.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:56:11.259498 pymmcore-widgets-0.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/camera_roi_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/channel_group_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/channel_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/channel_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/configuration_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/default_camera_exposure_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/device_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/exposure_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/grid_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/group_preset_table_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/image_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/live_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/mda_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/objectives_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/pixel_size_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/position_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/presets_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/properties_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/property_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/property_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/shutters_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/snap_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/stage_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/state_device_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/time_plan_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/z_stack_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 22:56:11.267498 pymmcore-widgets-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:56:11.251498 pymmcore-widgets-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:56:11.259498 pymmcore-widgets-0.4.0/src/pymmcore_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_camera_roi_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_channel_group_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_channel_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_device_property_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_device_type_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_device_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_exposure_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:56:11.263498 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_group_preset_widget/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_group_preset_widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_group_preset_widget/_add_first_preset_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_group_preset_widget/_add_group_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_group_preset_widget/_add_preset_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_group_preset_widget/_edit_group_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_group_preset_widget/_edit_preset_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_group_preset_widget/_group_preset_table_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_image_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_live_button_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_load_system_cfg_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:56:11.263498 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/_autofocus_device_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17375 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/_channel_table_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/_checkable_tabwidget_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/_general_mda_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28046 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/_grid_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23943 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/_mda_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32010 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/_positions_table_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/_time_plan_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/_zstack_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_objective_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20718 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_pixel_size_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11624 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_presets_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_properties_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_property_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13904 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_property_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13222 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_shutter_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_snap_button_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13375 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_stage_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:56:11.259498 pymmcore-widgets-0.4.0/src/pymmcore_widgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-27 22:56:11.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-07-27 22:56:11.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 22:56:11.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 22:56:10.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-27 22:56:11.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 22:56:11.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:56:11.267498 pymmcore-widgets-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_camera_roi_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_channel_group_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_channel_table_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_channel_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_combo_message_box_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_config.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_core_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_device_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_exposure_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_grid_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_group_preset_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_image_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_live_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_load_system_cfg_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_mda_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_objective_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15068 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_position_table_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_presets_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_prop_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_properties_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_property_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11019 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_shutter_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_snap_button_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_stage_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_table_pixel_size_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_time_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tox.ini
```

### Comparing `pymmcore-widgets-0.3.0/.cruft.json` & `pymmcore-widgets-0.4.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/.github/workflows/ci.yml` & `pymmcore-widgets-0.4.0/.github/workflows/cron.yml`

 * *Files 27% similar despite different names*

```diff
@@ -1,111 +1,61 @@
-name: CI
+name: --pre Test
+# An "early warning" cron job that will install dependencies
+# with `pip install --pre` periodically to test for breakage
+# (and open an issue if a test fails)
 
 on:
-  push:
-    branches:
-      - main
-    tags:
-      - "v*"
-  pull_request: {}
+  schedule:
+    - cron: '0 */12 * * *'  # every 12 hours
   workflow_dispatch:
 
 jobs:
-  check-manifest:
-    name: Check Manifest
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
-        with:
-          python-version: "3.x"
-      - run: pip install check-manifest && check-manifest
 
   test:
-    name: ${{ matrix.platform }} py${{ matrix.python-version }} ${{ matrix.backend }}
+    name: ${{ matrix.platform }} (${{ matrix.python-version }})
     runs-on: ${{ matrix.platform }}
     strategy:
       fail-fast: false
       matrix:
+        python-version: ['3.8', '3.9', '3.10']
         platform: [macos-latest, windows-latest]
-        python-version: ["3.8", "3.10"]
         backend: [pyside2, pyqt5]
-        include:
-          - platform: windows-latest
-            python-version: "3.10"
-            backend: pyside6
-          - platform: windows-latest
-            python-version: "3.10"
-            backend: pyqt6
-          - platform: windows-latest
-            python-version: "3.9"
-            backend: pyside2
-          - platform: windows-latest
-            python-version: "3.9"
-            backend: pyqt5
 
     steps:
-      - name: Cancel Previous Runs
-        uses: styfle/cancel-workflow-action@0.11.0
-        with:
-          access_token: ${{ github.token }}
-
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies
         run: |
           python -m pip install -U pip
-          python -m pip install -e .[test,image,${{ matrix.backend }}]
+          python -m pip install --pre -e .[test,image,${{ matrix.backend }}]
 
       - name: Install Windows OpenGL
         if: runner.os == 'Windows'
         run: |
           git clone --depth 1 https://github.com/pyvista/gl-ci-helpers.git
           powershell gl-ci-helpers/appveyor/install_opengl.ps1
           if (Test-Path -Path "C:\Windows\system32\opengl32.dll" -PathType Leaf) {Exit 0} else {Exit 1}
 
       - name: Install Micro-Manager
         run: mmcore install
 
       - name: Test
         run: pytest -v --cov=pymmcore_widgets --cov-report=xml --color=yes
 
-      - name: Coverage
-        uses: codecov/codecov-action@v3
-
-  deploy:
-    name: Deploy
-    needs: test
-    if: "success() && startsWith(github.ref, 'refs/tags/')"
-    runs-on: ubuntu-latest
-
-    steps:
-      - uses: actions/checkout@v3
-
-      - name: Set up Python
-        uses: actions/setup-python@v4
-        with:
-          python-version: "3.x"
-
-      - name: install
-        run: |
-          git tag
-          pip install -U pip
-          pip install -U build twine
-          python -m build
-          twine check dist/*
-          ls -lh dist
-
-      - name: Build and publish
-        run: twine upload dist/*
+      # If something goes wrong, we can open an issue in the repo
+      - name: Report Failures
+        if: ${{ failure() }}
+        uses: JasonEtco/create-an-issue@v2
         env:
-          TWINE_USERNAME: __token__
-          TWINE_PASSWORD: ${{ secrets.PYPI_API_TOKEN }}
-
-      - uses: softprops/action-gh-release@v1
+          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+          PLATFORM: ${{ matrix.platform }}
+          PYTHON: ${{ matrix.python }}
+          RUN_ID: ${{ github.run_id }}
+          TITLE: '[test-bot] pip install --pre is failing'
         with:
-          generate_release_notes: true
+          filename: .github/TEST_FAIL_TEMPLATE.md
+          update_existing: true
```

### Comparing `pymmcore-widgets-0.3.0/.github/workflows/docs.yml` & `pymmcore-widgets-0.4.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/.gitignore` & `pymmcore-widgets-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/.pre-commit-config.yaml` & `pymmcore-widgets-0.4.0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -16,29 +16,29 @@
     rev: v4.4.0
     hooks:
       - id: check-docstring-first
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.206
+    rev: v0.0.275
     hooks:
       - id: ruff
         args: [--fix]
 
   - repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.10.1
+    rev: v0.13
     hooks:
       - id: validate-pyproject
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.991
+    rev: v1.4.1
     hooks:
       - id: mypy
         files: "^src/"
         additional_dependencies:
-          - pymmcore-plus>=0.6.3
+          - pymmcore-plus>=0.6.6
```

### Comparing `pymmcore-widgets-0.3.0/LICENSE` & `pymmcore-widgets-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/PKG-INFO` & `pymmcore-widgets-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymmcore-widgets
-Version: 0.3.0
+Version: 0.4.0
 Summary: A set of Qt-based widgets onto the pymmcore-plus model
 Author-email: Federico Gasparoli <federico.gasparoli@gmail.com>, Talley Lambert <talley.lambert@gmail.com>, Ian Hunt-Isaak <ianhuntisaak@gmail.com>
 License: BSD 3-Clause License
 Project-URL: homepage, https://github.com/pymmcore-plus/pymmcore-widgets
 Project-URL: repository, https://github.com/pymmcore-plus/pymmcore-widgets
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pymmcore-widgets-0.3.0/README.md` & `pymmcore-widgets-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/docs/_gen_widget_pages.py` & `pymmcore-widgets-0.4.0/docs/_gen_widget_pages.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/docs/_hooks.py` & `pymmcore-widgets-0.4.0/docs/_hooks.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/docs/images/favicon.ico` & `pymmcore-widgets-0.4.0/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/docs/index.md` & `pymmcore-widgets-0.4.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/docs/stylesheets/extra.css` & `pymmcore-widgets-0.4.0/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/examples/device_widget.py` & `pymmcore-widgets-0.4.0/examples/device_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/examples/image_preview.py` & `pymmcore-widgets-0.4.0/examples/image_preview.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/examples/mda_widget.py` & `pymmcore-widgets-0.4.0/examples/mda_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/examples/presets_widget.py` & `pymmcore-widgets-0.4.0/examples/presets_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/examples/properties_widget.py` & `pymmcore-widgets-0.4.0/examples/properties_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/examples/property_widget.py` & `pymmcore-widgets-0.4.0/examples/property_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/examples/stage_widget.py` & `pymmcore-widgets-0.4.0/examples/stage_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/examples/state_device_widget.py` & `pymmcore-widgets-0.4.0/examples/state_device_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/mkdocs.yml` & `pymmcore-widgets-0.4.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/pyproject.toml` & `pymmcore-widgets-0.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -21,29 +21,29 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dynamic = ["version"]
 dependencies = [
-    'pymmcore-plus>=0.6.3',
-    'useq-schema >=0.1.2',
-    'superqt >=0.3.1',
+    'pymmcore-plus>=0.6.6',
+    'useq-schema >=0.2.0',
+    'superqt[quantity] >=0.3.1',
     'fonticon-materialdesignicons6',
     'qtpy',
 ]
 
 # extras
 # https://peps.python.org/pep-0621/#dependencies-optional-dependencies
 [project.optional-dependencies]
 test = ["pytest>=6.0", "pytest-cov", "pytest-qt"]
 pyqt5 = ["PyQt5"]
 pyside2 = ["PySide2"]
 pyqt6 = ["PyQt6"]
-pyside6 = ["PySide6"]
+pyside6 = ["PySide6<6.5"]
 image = ["vispy"]
 
 dev = [
     "black",
     "cruft",
     "ruff",
     "ipython",
@@ -101,25 +101,26 @@
     "E",    # style errors
     "F",    # flakes
     "D",    # pydocstyle
     "I001", # isort
     "UP",    # pyupgrade
     # "N",  # pep8-naming
     # "S",  # bandit
-    "C",    # flake8-comprehensions
+    "C4",    # flake8-comprehensions
     "B",    # flake8-bugbear
     "A001", # flake8-builtins
     "RUF",  # ruff-specific rules
 ]
-extend-ignore = [
+ignore = [
     "D100", # Missing docstring in public module
     "D107", # Missing docstring in __init__
     "D203", # 1 blank line required before class docstring
     "D212", # Multi-line docstring summary should start at the first line
     "D213", # Multi-line docstring summary should start at the second line
+    "D401", # First line should be in imperative mood
     "D413", # Missing blank line after last section
     "D416", # Section name should end with a colon
     "C901", # Function is too complex
 ]
 
 
 [tool.ruff.per-file-ignores]
@@ -138,14 +139,15 @@
 [tool.mypy]
 files = "src/**/"
 strict = true
 disallow_any_generics = false
 disallow_subclassing_any = false
 show_error_codes = true
 pretty = true
+plugins = ["pydantic.mypy"]
 
 
 # https://coverage.readthedocs.io/en/6.4/config.html
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "if TYPE_CHECKING:",
```

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets/__init__.py` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 
 try:
     __version__ = version("pymmcore-widgets")
 except PackageNotFoundError:
     __version__ = "uninstalled"
 
 from ._camera_roi_widget import CameraRoiWidget
+from ._channel_group_widget import ChannelGroupWidget
 from ._channel_widget import ChannelWidget
 from ._device_widget import DeviceWidget, StateDeviceWidget
 from ._exposure_widget import DefaultCameraExposureWidget, ExposureWidget
 from ._group_preset_widget._group_preset_table_widget import GroupPresetTableWidget
 from ._image_widget import ImagePreview
 from ._live_button_widget import LiveButton
 from ._load_system_cfg_widget import ConfigurationWidget
 from ._mda import (
+    ChannelTable,
+    GridWidget,
     MDAWidget,
     PositionTable,
-    SampleExplorerWidget,
     TimePlanWidget,
     ZStackWidget,
 )
 from ._objective_widget import ObjectivesWidget
 from ._pixel_size_widget import PixelSizeWidget
 from ._presets_widget import PresetsWidget
 from ._properties_widget import PropertiesWidget
@@ -29,31 +31,33 @@
 from ._property_widget import PropertyWidget
 from ._shutter_widget import ShuttersWidget
 from ._snap_button_widget import SnapButton
 from ._stage_widget import StageWidget
 
 __all__ = [
     "CameraRoiWidget",
+    "ChannelGroupWidget",
+    "ChannelTable",
     "ChannelWidget",
     "ConfigurationWidget",
     "DefaultCameraExposureWidget",
     "DeviceWidget",
     "ExposureWidget",
+    "GridWidget",
     "GroupPresetTableWidget",
     "ImagePreview",
     "LiveButton",
     "MDAWidget",
     "ObjectivesWidget",
     "PixelSizeWidget",
     "PositionTable",
     "PresetsWidget",
     "PropertiesWidget",
     "PropertyBrowser",
     "PropertyWidget",
-    "SampleExplorerWidget",
     "ShuttersWidget",
     "SnapButton",
     "StageWidget",
     "StateDeviceWidget",
     "TimePlanWidget",
     "ZStackWidget",
 ]
```

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets/_camera_roi_widget.py` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_camera_roi_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,14 @@
 
     def _disconnect(self) -> None:
         self._mmc.events.systemConfigurationLoaded.disconnect(self._on_sys_cfg_loaded)
         self._mmc.events.pixelSizeChanged.disconnect(self._update_lbl_info)
         self._mmc.events.roiSet.disconnect(self._on_roi_set)
 
     def _create_main_wdg(self) -> QWidget:
-
         wdg = QWidget()
         layout = QGridLayout()
         layout.setVerticalSpacing(3)
         layout.setHorizontalSpacing(5)
         layout.setContentsMargins(3, 3, 3, 3)
         wdg.setLayout(layout)
 
@@ -125,15 +124,14 @@
         bottom_layout.addWidget(self.crop_btn)
 
         layout.addWidget(bottom_wdg, 1, 0, 1, 2)
 
         return wdg
 
     def _create_selection_combo_wdg(self) -> QWidget:
-
         wdg = QWidget()
         layout = QHBoxLayout()
         layout.setSpacing(5)
         layout.setContentsMargins(0, 0, 0, 0)
         wdg.setLayout(layout)
 
         self.cam_roi_combo = QComboBox()
@@ -141,15 +139,14 @@
         self.cam_roi_combo.currentTextChanged.connect(self._on_roi_combobox_change)
 
         layout.addWidget(self.cam_roi_combo)
 
         return wdg
 
     def _create_selection_wdg(self) -> QGroupBox:
-
         wdg = QGroupBox()
         wdg.setSizePolicy(QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Fixed)
         layout = QVBoxLayout()
         layout.setSpacing(5)
         layout.setContentsMargins(3, 3, 3, 3)
         wdg.setLayout(layout)
 
@@ -159,15 +156,14 @@
         self.center_checkbox = QCheckBox(text="center custom ROI")
         self.center_checkbox.toggled.connect(self._on_center_checkbox)
         layout.addWidget(self.center_checkbox)
 
         return wdg
 
     def _create_custom_roi_group(self) -> QGroupBox:
-
         group = QGroupBox()
         layout = QGridLayout()
         layout.setSpacing(5)
         layout.setContentsMargins(3, 3, 3, 3)
         group.setLayout(layout)
 
         roi_start_x_label = QLabel("Start x:")
@@ -258,15 +254,14 @@
             height = round(chip_size_y / val)
             items.append(f"{width} x {height}")
         return items
 
     def _on_roi_set(
         self, cam_label: str, x: int, y: int, width: int, height: int
     ) -> None:
-
         self.start_x.setMaximum(self.chip_size_x)
         self.start_y.setMaximum(self.chip_size_y)
 
         self._set_roi_groupbox_values(x, y, width, height, False)
 
         if (x, y, width, height) == (0, 0, self.chip_size_x, self.chip_size_y):
             with signals_blocked(self.cam_roi_combo):
@@ -292,15 +287,14 @@
         self._setEnabled(True)
         spin_list = [self.start_x, self.start_y, self.roi_width, self.roi_height]
         self._hide_spinbox_button(spin_list, False)
         with signals_blocked(self.center_checkbox):
             self.center_checkbox.setChecked(checkbox_state)
 
     def _update_lbl_info(self) -> None:
-
         start_x, start_y, width, height = self._get_roi_groupbox_values()
 
         px_size = self._mmc.getPixelSizeUm() or 0
 
         width_um = width * px_size
         height_um = height * px_size
 
@@ -374,15 +368,14 @@
 
             if self.snap_checkbox.isChecked():
                 self._mmc.snap()
 
         self._update_lbl_info()
 
     def _on_roi_spinbox_changed(self) -> None:
-
         self._update_lbl_info()
 
         if self.cam_roi_combo.currentText() != CUSTOM_ROI:
             return
 
         self._check_size_reset_snap()
 
@@ -433,15 +426,14 @@
         start_x = self.start_x.value()
         start_y = self.start_y.value()
         width = self.roi_width.value()
         height = self.roi_height.value()
         return start_x, start_y, width, height
 
     def _on_center_checkbox(self, state: bool) -> None:
-
         self.start_x.setEnabled(not state)
         self.start_y.setEnabled(not state)
         self._hide_spinbox_button([self.start_x, self.start_y], state)
 
         if not state or self.cam_roi_combo.currentText() != CUSTOM_ROI:
             return
```

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets/_channel_widget.py` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_channel_widget.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from pymmcore_plus import CMMCorePlus, DeviceType
+from pymmcore_plus import CMMCorePlus
 from qtpy.QtWidgets import QComboBox, QVBoxLayout, QWidget
 
 from ._presets_widget import PresetsWidget
 from ._util import ComboMessageBox
 
 
 class ChannelWidget(QWidget):
@@ -41,15 +41,14 @@
     def __init__(
         self,
         channel_group: str | None = None,
         *,
         parent: QWidget | None = None,
         mmcore: CMMCorePlus | None = None,
     ) -> None:
-
         super().__init__(parent=parent)
         self._mmc = mmcore or CMMCorePlus.instance()
 
         self._channel_group = channel_group or self._get_channel_group()
 
         self.channel_wdg: PresetsWidget | QComboBox
 
@@ -58,15 +57,14 @@
         self.setLayout(QVBoxLayout())
         self.layout().setContentsMargins(0, 0, 0, 0)
         self.layout().setSpacing(0)
         self.layout().addWidget(self.channel_wdg)
 
         self._mmc.events.systemConfigurationLoaded.connect(self._on_sys_cfg_loaded)
         self._mmc.events.channelGroupChanged.connect(self._on_channel_group_changed)
-        self._mmc.events.configSet.connect(self._on_channel_set)
 
         # presetDeleted signal is handled by the PresetsWidget
         self._mmc.events.configDefined.connect(self._on_new_group_preset)
         self._mmc.events.configGroupDeleted.connect(self._on_group_deleted)
 
         self.destroyed.connect(self._disconnect)
         self._on_sys_cfg_loaded()
@@ -94,25 +92,14 @@
         if channel_group is not None:
             self._mmc.setChannelGroup(channel_group)
             # if the channel_group name is the same as the one in the previously
             # loaded cfg and it contains different presets, the 'channelGroupChanged'
             # signal is not emitted and we get a ValueError. So we need to call:
             self._on_channel_group_changed(channel_group)
 
-    def _on_channel_set(self, group: str, preset: str) -> None:
-        ch = self._mmc.getChannelGroup()
-        if group != ch:
-            return  # pragma: no cover
-        for d in self._mmc.getConfigData(ch, preset):
-            _dev = d[0]
-            _type = self._mmc.getDeviceType(_dev)
-            if _type is DeviceType.Shutter:
-                self._mmc.setProperty("Core", "Shutter", _dev)
-                break
-
     def _on_channel_group_changed(self, new_channel_group: str) -> None:
         """When Channel group is changed, recreate combo."""
         _wdg = QWidget()
         self.channel_wdg.setParent(_wdg)
         self.channel_wdg.deleteLater()
         self._update_widget(new_channel_group)
 
@@ -132,10 +119,9 @@
     def _update_widget(self, channel_group: str) -> None:
         self._create_channel_widget(channel_group)
         self.layout().addWidget(self.channel_wdg)
 
     def _disconnect(self) -> None:
         self._mmc.events.systemConfigurationLoaded.disconnect(self._on_sys_cfg_loaded)
         self._mmc.events.channelGroupChanged.disconnect(self._on_channel_group_changed)
-        self._mmc.events.configSet.disconnect(self._on_channel_set)
         self._mmc.events.configDefined.disconnect(self._on_new_group_preset)
         self._mmc.events.configGroupDeleted.connect(self._on_group_deleted)
```

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets/_core.py` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_core.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets/_device_property_table.py` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_device_property_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,14 @@
             self.item(row, 0).setFlags(flags)
 
     def _rebuild_table(self) -> None:
         self.clearContents()
         props = list(self._mmc.iterProperties(as_object=True))
         self.setRowCount(len(props))
         for i, prop in enumerate(props):
-
             item = QTableWidgetItem(f"{prop.device}-{prop.name}")
             item.setData(self.PROP_ROLE, prop)
             # TODO: make sure to add icons for all possible device types
             icon_string = ICONS.get(prop.deviceType(), None)
             if icon_string:
                 item.setIcon(icon(icon_string, color="Gray"))
             self.setItem(i, 0, item)
```

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets/_device_type_filter.py` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_device_type_filter.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets/_device_widget.py` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_device_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         return self._mmc.getDeviceName(self._device_label)
 
     def deviceType(self) -> DeviceType:
         """Return type of Device (`pymmcore_plus.DeviceType`)."""
         return self._mmc.getDeviceType(self._device_label)
 
     @classmethod
-    def for_device(cls, device_label: str) -> "DeviceWidget":
+    def for_device(cls, device_label: str) -> DeviceWidget:
         """Create a type-appropriate subclass for device with label `device_label`.
 
         Parameters
         ----------
         device_label : str
             A deviceLabel for which to create a widget.
```

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets/_exposure_widget.py` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_exposure_widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
         see [ImagePreview](../ImagePreview#example)
 
     """
 
     def __init__(
         self,
-        camera: str = None,  # type: ignore
+        camera: str | None = None,
         *,
         parent: QWidget | None = None,
         mmcore: CMMCorePlus | None = None,
     ):
         super().__init__(parent=parent)
 
         self._mmc = mmcore or CMMCorePlus.instance()
@@ -63,15 +63,15 @@
 
         self.destroyed.connect(self._disconnect)
 
     def _disconnect(self) -> None:
         self._mmc.events.exposureChanged.disconnect(self._on_exp_changed)
         self._mmc.events.systemConfigurationLoaded.disconnect(self._on_load)
 
-    def setCamera(self, camera: str = None) -> None:  # type: ignore
+    def setCamera(self, camera: str | None = None) -> None:
         """Set which camera this widget tracks.
 
         Parameters
         ----------
         camera : str
             The camera device label. By default, None. If not specified,
             the widget will use the current Camera device.
@@ -129,17 +129,15 @@
     def _disconnect(self) -> None:
         self._mmc.events.exposureChanged.disconnect(self._on_exp_changed)
         self._mmc.events.systemConfigurationLoaded.disconnect(self._on_load)
         self._mmc.events.devicePropertyChanged(
             g_Keyword_CoreDevice, g_Keyword_CoreCamera
         ).disconnect(self._camera_updated)
 
-    def setCamera(
-        self, camera: str = None, force: bool = False  # type: ignore
-    ) -> None:
+    def setCamera(self, camera: str | None = None, force: bool = False) -> None:
         """Set which camera this widget tracks.
 
         Using this on the ``DefaultCameraExposureWidget``widget may cause unexpected
         behavior, instead try to use an ``ExposureWidget``.
 
         Parameters
         ----------
```

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets/_group_preset_widget/_add_first_preset_widget.py` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_group_preset_widget/_add_first_preset_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,14 @@
         self._dev_prop_val_list = dev_prop_val_list
 
         self._create_gui()
 
         self._populate_table()
 
     def _create_gui(self) -> None:
-
         self.setWindowTitle(f"Add the first Preset to the new '{self._group}' Group")
 
         main_layout = QVBoxLayout()
         main_layout.setSpacing(0)
         main_layout.setContentsMargins(10, 10, 10, 10)
         self.setLayout(main_layout)
 
@@ -98,15 +97,14 @@
         return wdg
 
     def _get_placeholder_name(self) -> str:
         idx = sum("NewPreset" in p for p in self._mmc.getAvailableConfigs(self._group))
         return f"NewPreset_{idx}" if idx > 0 else "NewPreset"
 
     def _create_bottom_wdg(self) -> QWidget:
-
         wdg = QWidget()
         wdg_layout = QHBoxLayout()
         wdg_layout.setSpacing(5)
         wdg_layout.setContentsMargins(0, 0, 0, 0)
         wdg.setLayout(wdg_layout)
 
         self.apply_button = QPushButton(text="Create Preset")
@@ -121,27 +119,25 @@
 
         wdg_layout.addItem(spacer)
         wdg_layout.addWidget(self.apply_button)
 
         return wdg
 
     def _populate_table(self) -> None:
-
         self.table.clearContents()
 
         self.table.setRowCount(len(self._dev_prop_val_list))
         for idx, (dev, prop, _) in enumerate(self._dev_prop_val_list):
             item = QTableWidgetItem(f"{dev}-{prop}")
             wdg = PropertyWidget(dev, prop, mmcore=self._mmc)
             wdg._value_widget.valueChanged.disconnect()  # type: ignore
             self.table.setItem(idx, 0, item)
             self.table.setCellWidget(idx, 1, wdg)
 
     def _create_first_preset(self) -> None:
-
         dev_prop_val = []
         for row in range(self.table.rowCount()):
             device_property = self.table.item(row, 0).text()
             dev = device_property.split("-")[0]
             prop = device_property.split("-")[1]
             value = str(self.table.cellWidget(row, 1).value())
             dev_prop_val.append((dev, prop, value))
```

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets/_group_preset_widget/_add_group_widget.py` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_group_preset_widget/_add_group_widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,14 @@
     def closeEvent(self, event: QCloseEvent) -> None:
         """Close also 'AddFirstPresetWidget' if is open."""
         if hasattr(self, "_first_preset_wdg"):
             self._first_preset_wdg.close()  # type: ignore
         event.accept()
 
     def _create_gui(self) -> None:
-
         self.setWindowTitle("Create a new Group")
 
         main_layout = QVBoxLayout()
         main_layout.setSpacing(10)
         main_layout.setContentsMargins(10, 10, 10, 10)
         self.setLayout(main_layout)
 
@@ -55,15 +54,14 @@
         table = self._create_table_wdg()
         main_layout.addWidget(table)
 
         btn = self._create_button_wdg()
         main_layout.addWidget(btn)
 
     def _create_group_lineedit_wdg(self) -> QGroupBox:
-
         wdg = QGroupBox()
         layout = QHBoxLayout()
         layout.setContentsMargins(5, 5, 5, 5)
         layout.setSpacing(10)
         wdg.setLayout(layout)
 
         group_lbl = QLabel(text="Group name:")
@@ -75,15 +73,14 @@
 
         layout.addWidget(group_lbl)
         layout.addWidget(self.group_lineedit)
 
         return wdg
 
     def _create_table_wdg(self) -> QGroupBox:
-
         wdg = QGroupBox()
         layout = QHBoxLayout()
         layout.setContentsMargins(5, 5, 5, 5)
         layout.setSpacing(0)
         wdg.setLayout(layout)
 
         self._filter_text = QLineEdit()
@@ -111,15 +108,14 @@
         self.layout().addWidget(right)
         layout.addWidget(left)
         layout.addWidget(right)
 
         return wdg
 
     def _create_button_wdg(self) -> QWidget:
-
         wdg = QWidget()
         layout = QHBoxLayout()
         layout.setContentsMargins(0, 0, 0, 0)
         layout.setSpacing(0)
         wdg.setLayout(layout)
 
         self.info_lbl = QLabel()
@@ -141,34 +137,33 @@
     def _update_filter(self) -> None:
         filt = self._filter_text.text().lower()
         self._prop_table.filterDevices(
             filt, self._device_filters.filters(), self._device_filters.showReadOnly()
         )
 
     def _add_group(self) -> None:
-
         group = self.group_lineedit.text()
 
         if not group:
-            warnings.warn("Give a name to the group!")
+            warnings.warn("Give a name to the group!", stacklevel=2)
             self.info_lbl.setStyleSheet("color: magenta;")
             self.info_lbl.setText("Give a name to the group!")
             return
 
         if group in self._mmc.getAvailableConfigGroups():
-            warnings.warn(f"There is already a preset called '{group}'.")
+            warnings.warn(f"There is already a preset called '{group}'.", stacklevel=2)
             self.info_lbl.setStyleSheet("color: magenta;")
             self.info_lbl.setText(f"'{group}' already exist!")
             return
 
         # [(device, property, value_to_set), ...]
         dev_prop_val_list = self._prop_table.getCheckedProperties()
 
         if not dev_prop_val_list:
-            warnings.warn("Select at lest one property!")
+            warnings.warn("Select at lest one property!", stacklevel=2)
             self.info_lbl.setStyleSheet("color: magenta;")
             self.info_lbl.setText("Select at lest one property!")
             return
 
         if hasattr(self, "_first_preset_wdg"):
             self._first_preset_wdg.close()  # type: ignore
         self._first_preset_wdg = AddFirstPresetWidget(
```

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets/_group_preset_widget/_add_preset_widget.py` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_group_preset_widget/_add_preset_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,14 @@
         self._group = group
 
         self._create_gui()
 
         self._populate_table()
 
     def _create_gui(self) -> None:
-
         self.setWindowTitle(f"Add a new Preset to the '{self._group}' Group")
 
         main_layout = QVBoxLayout()
         main_layout.setSpacing(0)
         main_layout.setContentsMargins(10, 10, 10, 10)
         self.setLayout(main_layout)
 
@@ -60,15 +59,14 @@
 
         bottom_wdg = self._create_bottom_wdg()
         wdg_layout.addWidget(bottom_wdg)
 
         main_layout.addWidget(wdg)
 
     def _create_top_wdg(self) -> QGroupBox:
-
         wdg = QGroupBox()
         wdg_layout = QHBoxLayout()
         wdg_layout.setSpacing(5)
         wdg_layout.setContentsMargins(5, 5, 5, 5)
         wdg.setLayout(wdg_layout)
 
         lbl_sizepolicy = QSizePolicy(QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Fixed)
@@ -94,15 +92,14 @@
         return wdg
 
     def _get_placeholder_name(self) -> str:
         idx = sum("NewPreset" in p for p in self._mmc.getAvailableConfigs(self._group))
         return f"NewPreset_{idx}" if idx > 0 else "NewPreset"
 
     def _create_bottom_wdg(self) -> QWidget:
-
         wdg = QWidget()
         wdg_layout = QHBoxLayout()
         wdg_layout.setSpacing(5)
         wdg_layout.setContentsMargins(0, 0, 0, 0)
         wdg.setLayout(wdg_layout)
 
         self.info_lbl = QLabel()
@@ -114,15 +111,14 @@
 
         wdg_layout.addWidget(self.info_lbl)
         wdg_layout.addWidget(self.add_preset_button)
 
         return wdg
 
     def _populate_table(self) -> None:
-
         self.table.clearContents()
 
         dev_prop = []
         for preset in self._mmc.getAvailableConfigs(self._group):
             dev_prop.extend(
                 [
                     (k[0], k[1])
@@ -136,19 +132,20 @@
             item = QTableWidgetItem(f"{dev}-{prop}")
             wdg = PropertyWidget(dev, prop, mmcore=self._mmc)
             wdg._value_widget.valueChanged.disconnect()  # type: ignore
             self.table.setItem(idx, 0, item)
             self.table.setCellWidget(idx, 1, wdg)
 
     def _add_preset(self) -> None:
-
         preset_name = self.preset_name_lineedit.text()
 
         if preset_name in self._mmc.getAvailableConfigs(self._group):
-            warnings.warn(f"There is already a preset called '{preset_name}'.")
+            warnings.warn(
+                f"There is already a preset called '{preset_name}'.", stacklevel=2
+            )
             self.info_lbl.setStyleSheet("color: magenta;")
             self.info_lbl.setText(f"'{preset_name}' already exist!")
             return
 
         if not preset_name:
             preset_name = self.preset_name_lineedit.placeholderText()
 
@@ -163,15 +160,16 @@
         for p in self._mmc.getAvailableConfigs(self._group):
             dpv_preset = [
                 (k[0], k[1], k[2]) for k in self._mmc.getConfigData(self._group, p)
             ]
             if dpv_preset == dev_prop_val:
                 warnings.warn(
                     "There is already a preset with the same "
-                    f"devices, properties and values: '{p}'."
+                    f"devices, properties and values: '{p}'.",
+                    stacklevel=2,
                 )
                 self.info_lbl.setStyleSheet("color: magenta;")
                 self.info_lbl.setText(f"'{p}' already has the same properties!")
                 return
 
         with block_core(self._mmc.events):
             for d, p, v in dev_prop_val:
```

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets/_group_preset_widget/_edit_group_widget.py` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_group_preset_widget/_edit_group_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 
         self.group_lineedit.setText(self._group)
         self.group_lineedit.setEnabled(False)
 
         self.destroyed.connect(self._disconnect)
 
     def _create_gui(self) -> None:
-
         self.setWindowTitle(f"Edit the '{self._group}' Group.")
 
         main_layout = QVBoxLayout()
         main_layout.setSpacing(10)
         main_layout.setContentsMargins(10, 10, 10, 10)
         self.setLayout(main_layout)
 
@@ -55,15 +54,14 @@
         table = self._create_table_wdg()
         main_layout.addWidget(table)
 
         btn = self._create_button_wdg()
         main_layout.addWidget(btn)
 
     def _create_group_lineedit_wdg(self) -> QGroupBox:
-
         wdg = QGroupBox()
         layout = QHBoxLayout()
         layout.setContentsMargins(5, 5, 5, 5)
         layout.setSpacing(10)
         wdg.setLayout(layout)
 
         group_lbl = QLabel(text="Group name:")
@@ -75,15 +73,14 @@
 
         layout.addWidget(group_lbl)
         layout.addWidget(self.group_lineedit)
 
         return wdg
 
     def _create_table_wdg(self) -> QGroupBox:
-
         wdg = QGroupBox()
         layout = QHBoxLayout()
         layout.setContentsMargins(5, 5, 5, 5)
         layout.setSpacing(0)
         wdg.setLayout(layout)
 
         self._filter_text = QLineEdit()
@@ -112,15 +109,14 @@
         self.layout().addWidget(right)
         layout.addWidget(left)
         layout.addWidget(right)
 
         return wdg
 
     def _create_button_wdg(self) -> QWidget:
-
         wdg = QWidget()
         layout = QHBoxLayout()
         layout.setContentsMargins(0, 0, 0, 0)
         layout.setSpacing(0)
         wdg.setLayout(layout)
 
         self.info_lbl = QLabel()
@@ -142,15 +138,14 @@
     def _update_filter(self) -> None:
         filt = self._filter_text.text().lower()
         self._prop_table.filterDevices(
             filt, self._device_filters.filters(), self._device_filters.showReadOnly()
         )
 
     def _add_group(self) -> None:
-
         # [(device, property, value), ...], need to remove the value
         new_dev_prop = [x[:2] for x in self._prop_table.getCheckedProperties()]
 
         presets = self._mmc.getAvailableConfigs(self._group)
         preset_dev_prop = [
             (k[0], k[1]) for k in self._mmc.getConfigData(self._group, presets[0])
         ]
@@ -175,15 +170,14 @@
                 (d, p, v) for d, p, v in preset_dev_prop_val if (d, p) in new_dev_prop
             ]
             _prop_to_keep.append(_to_keep)
 
         self._mmc.deleteConfigGroup(self._group)
 
         for idx, preset in enumerate(presets):
-
             preset_dpv = _prop_to_keep[idx]
             if _to_add:
                 preset_dpv.extend(_to_add)
 
             with block_core(self._mmc.events):
                 for d, p, v in preset_dpv:
                     self._mmc.defineConfig(self._group, preset, d, p, v)
```

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets/_group_preset_widget/_edit_preset_widget.py` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_group_preset_widget/_edit_preset_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,14 @@
         self._preset = preset
 
         self._create_gui()
 
         self._populate_table_and_combo()
 
     def _create_gui(self) -> None:  # sourcery skip: class-extract-method
-
         self.setWindowTitle(
             f"Edit the '{self._preset}' Preset from the '{self._group}' Group"
         )
 
         main_layout = QVBoxLayout()
         main_layout.setSpacing(0)
         main_layout.setContentsMargins(10, 10, 10, 10)
@@ -113,15 +112,14 @@
         wdg_layout.addWidget(ps_lbl)
         wdg_layout.addWidget(self._presets_combo)
         wdg_layout.addWidget(self.preset_name_lineedit)
 
         return wdg
 
     def _create_bottom_wdg(self) -> QWidget:
-
         wdg = QWidget()
         wdg_layout = QHBoxLayout()
         wdg_layout.setSpacing(5)
         wdg_layout.setContentsMargins(0, 0, 0, 0)
         wdg.setLayout(wdg_layout)
 
         self.info_lbl = QLabel()
@@ -133,15 +131,14 @@
 
         wdg_layout.addWidget(self.info_lbl)
         wdg_layout.addWidget(self.apply_button)
 
         return wdg
 
     def _update_combo(self) -> None:
-
         presets = self._mmc.getAvailableConfigs(self._group)
         with signals_blocked(self._presets_combo):
             self._presets_combo.clear()
             self._presets_combo.addItems(presets)
             self._presets_combo.setCurrentText(self._preset)
             self.preset_name_lineedit.setText(f"{self._preset}")
             self._resize_combo_height(len(presets))
@@ -149,15 +146,14 @@
 
     def _resize_combo_height(self, max_items: int) -> None:
         self._presets_combo.setEditable(True)
         self._presets_combo.setMaxVisibleItems(max_items)
         self._presets_combo.setEditable(False)
 
     def _populate_table_and_combo(self) -> None:
-
         self._update_combo()
 
         self.table.clearContents()
 
         dev_prop_val = [
             (k[0], k[1], k[2])
             for k in self._mmc.getConfigData(self._group, self._preset)
@@ -168,22 +164,20 @@
             wdg = PropertyWidget(dev, prop, mmcore=self._mmc)
             wdg._value_widget.valueChanged.disconnect()  # type: ignore
             wdg.setValue(val)
             self.table.setItem(idx, 0, item)
             self.table.setCellWidget(idx, 1, wdg)
 
     def _on_combo_changed(self, preset: str) -> None:
-
         self._preset = preset
         self.info_lbl.setStyleSheet("")
         self.info_lbl.setText("")
         self._populate_table_and_combo()
 
     def _apply_changes(self) -> None:
-
         dev_prop_val = []
         for row in range(self.table.rowCount()):
             device_property = self.table.item(row, 0).text()
             dev = device_property.split("-")[0]
             prop = device_property.split("-")[1]
             value = str(self.table.cellWidget(row, 1).value())
             dev_prop_val.append((dev, prop, value))
@@ -196,15 +190,16 @@
                 dpv_preset == dev_prop_val
                 and self._preset == self.preset_name_lineedit.text()
             ):
                 if p == self._preset:
                     return
                 warnings.warn(
                     "Threre is already a preset with the same "
-                    f"devices, properties and values: '{p}'."
+                    f"devices, properties and values: '{p}'.",
+                    stacklevel=2,
                 )
                 self.info_lbl.setStyleSheet("color: magenta;")
                 self.info_lbl.setText(f"'{p}' already has the same properties!")
                 return
 
         self._mmc.deleteConfig(self._group, self._preset)
```

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets/_group_preset_widget/_group_preset_table_widget.py` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_group_preset_widget/_group_preset_table_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,15 +78,14 @@
         self._create_gui()
 
         self._populate_table()
 
         self.destroyed.connect(self._disconnect)
 
     def _create_gui(self) -> None:
-
         self.setLayout(QVBoxLayout())
         self.layout().setSpacing(5)
         self.setContentsMargins(0, 0, 0, 0)
 
         save_btn = self._add_save_button()
         self.layout().addWidget(save_btn)
 
@@ -96,15 +95,14 @@
 
         btns = self._add_groups_presets_buttons()
         self.layout().addWidget(btns)
 
         self._enable_buttons(False)
 
     def _add_groups_presets_buttons(self) -> QWidget:
-
         main_wdg = QWidget()
         main_wdg_layout = QHBoxLayout()
         main_wdg_layout.setSpacing(10)
         main_wdg_layout.setContentsMargins(0, 0, 0, 0)
         main_wdg.setLayout(main_wdg_layout)
 
         lbl_sizepolicy = QSizePolicy(QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Fixed)
@@ -152,15 +150,14 @@
         presets_layout.addWidget(self.presets_edit_btn)
 
         main_wdg_layout.addWidget(presets_btn_wdg)
 
         return main_wdg
 
     def _add_save_button(self) -> QWidget:
-
         save_btn_wdg = QWidget()
         save_btn_layout = QHBoxLayout()
         save_btn_layout.setSpacing(5)
         save_btn_layout.setContentsMargins(0, 0, 0, 0)
         save_btn_wdg.setLayout(save_btn_layout)
 
         spacer = QSpacerItem(
@@ -196,23 +193,21 @@
 
     def _on_system_cfg_loaded(self) -> None:
         self._populate_table()
 
     def _on_new_group_preset(
         self, group: str, preset: str, device: str, property: str, value: str
     ) -> None:
-
         if not device or not property or not value:
             return
 
         if matching_item := self.table_wdg.findItems(group, Qt.MatchFlag.MatchExactly):
             row = matching_item[0].row()
 
             if isinstance(self.table_wdg.cellWidget(row, 1), PropertyWidget):
-
                 dev_prop_val = [
                     (k[0], k[1], k[2]) for k in self._mmc.getConfigData(group, preset)
                 ]
 
                 self._mmc.deleteConfigGroup(group)
 
                 if not preset:
@@ -304,16 +299,15 @@
             self.table_wdg.item(row, 0).text()
             for row in sorted(selected_rows, reverse=True)
         ]
 
         msg = self._msg_box(f"Delete '{',  '.join(groups)}'?")
 
         if msg == QMessageBox.StandardButton.Ok:
-            for row, group in enumerate(groups):
-                self.table_wdg.removeRow(row)
+            for group in groups:
                 self._mmc.deleteConfigGroup(group)
 
     def _msg_box(self, msg: str) -> Any:
         msgBox = QMessageBox(parent=self)
         msgBox.setIcon(QMessageBox.Icon.Warning)
         msgBox.setWindowTitle("Delete")
         msgBox.setText(msg)
@@ -356,40 +350,38 @@
     def _delete_preset(self) -> None:
         selected_rows = {r.row() for r in self.table_wdg.selectedIndexes()}
 
         if not selected_rows:
             return
 
         groups_preset = [
-            (row, self.table_wdg.item(row, 0).text(), self.table_wdg.cellWidget(row, 1))
+            (self.table_wdg.item(row, 0).text(), self.table_wdg.cellWidget(row, 1))
             for row in sorted(selected_rows, reverse=True)
         ]
 
         _text = []
-        for _, group, wdg in groups_preset:
+        for group, wdg in groups_preset:
             if isinstance(wdg, PresetsWidget):
                 _text.append(f"({group},  {wdg._combo.currentText()})")
             else:
                 _text.append(f"({group})")
 
         msg = self._msg_box(f"Delete '{',  '.join(_text)}'?")
 
         if msg == QMessageBox.StandardButton.Ok:
-            for row, group, wdg in groups_preset:
+            for group, wdg in groups_preset:
                 if isinstance(wdg, PresetsWidget):
                     preset = wdg._combo.currentText()
 
                     if len(wdg.allowedValues()) > 1:
                         self._mmc.deleteConfig(group, preset)
                     else:
-                        self.table_wdg.removeRow(row)
                         self._mmc.deleteConfigGroup(group)
 
                 elif isinstance(wdg, PropertyWidget):
-                    self.table_wdg.removeRow(row)
                     self._mmc.deleteConfigGroup(group)
 
     def _edit_preset(self) -> None:
         selected_rows = {r.row() for r in self.table_wdg.selectedIndexes()}
         if not selected_rows or len(selected_rows) > 1:
             return
```

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets/_image_widget.py` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_image_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets/_live_button_widget.py` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_live_button_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 
     def __init__(
         self,
         *,
         parent: QWidget | None = None,
         mmcore: CMMCorePlus | None = None,
     ) -> None:
-
         super().__init__(parent=parent)
 
         self._mmc = mmcore or CMMCorePlus.instance()
         self._button_text_on: str = "Live"
         self._button_text_off: str = "Stop"
         self._icon_color_on: COLOR_TYPE = (0, 255, 0)
         self._icon_color_off: COLOR_TYPE = "magenta"
```

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets/_load_system_cfg_widget.py` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_load_system_cfg_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets/_mda/_general_mda_widgets.py` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/_general_mda_widgets.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,154 +1,56 @@
 from __future__ import annotations
 
 from fonticon_mdi6 import MDI6
 from pymmcore_plus import CMMCorePlus
 from qtpy.QtCore import QSize, Qt
 from qtpy.QtWidgets import (
-    QAbstractItemView,
     QComboBox,
-    QGroupBox,
     QHBoxLayout,
     QLabel,
     QPushButton,
     QSizePolicy,
     QSpacerItem,
-    QTableWidget,
-    QVBoxLayout,
     QWidget,
 )
 from superqt.fonticon import icon
 
 
-class _MDAPositionTable(QGroupBox):
-    def __init__(self, header: list[str], *, parent: QWidget | None = None) -> None:
-        super().__init__(parent=parent)
-
-        self._mmc = CMMCorePlus.instance()
-
-        self.header = header
-
-        self._create_pos_gui()
-
-    def _create_pos_gui(self) -> None:
-
-        self.setTitle("Stage Positions")
-
-        self.setCheckable(True)
-        self.setChecked(False)
-
-        group_layout = QHBoxLayout()
-        group_layout.setSpacing(15)
-        group_layout.setContentsMargins(10, 10, 10, 10)
-        self.setLayout(group_layout)
-
-        # table
-        self.stage_tableWidget = QTableWidget()
-        self.stage_tableWidget.setSelectionBehavior(
-            QAbstractItemView.SelectionBehavior.SelectRows
-        )
-        hdr = self.stage_tableWidget.horizontalHeader()
-        hdr.setSectionResizeMode(hdr.ResizeMode.Stretch)
-        self.stage_tableWidget.verticalHeader().setVisible(False)
-        self.stage_tableWidget.setTabKeyNavigation(True)
-        self.stage_tableWidget.setColumnCount(4)
-        self.stage_tableWidget.setRowCount(0)
-        self.stage_tableWidget.setHorizontalHeaderLabels(self.header)
-        group_layout.addWidget(self.stage_tableWidget)
-
-        # buttons
-        wdg = QWidget()
-        layout = QVBoxLayout()
-        layout.setSpacing(10)
-        layout.setContentsMargins(0, 0, 0, 0)
-        wdg.setLayout(layout)
-
-        btn_sizepolicy = QSizePolicy(QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Fixed)
-        min_size = 100
-        self.add_pos_button = QPushButton(text="Add")
-        self.add_pos_button.setMinimumWidth(min_size)
-        self.add_pos_button.setSizePolicy(btn_sizepolicy)
-        self.remove_pos_button = QPushButton(text="Remove")
-        self.remove_pos_button.setMinimumWidth(min_size)
-        self.remove_pos_button.setSizePolicy(btn_sizepolicy)
-        self.clear_pos_button = QPushButton(text="Clear")
-        self.clear_pos_button.setMinimumWidth(min_size)
-        self.clear_pos_button.setSizePolicy(btn_sizepolicy)
-        self.grid_button = QPushButton(text="Grid")
-        self.grid_button.setMinimumWidth(min_size)
-        self.grid_button.setSizePolicy(btn_sizepolicy)
-        self.go = QPushButton(text="Go")
-        self.go.clicked.connect(self._move_to_position)
-        self.go.setMinimumWidth(min_size)
-        self.go.setSizePolicy(btn_sizepolicy)
-
-        spacer = QSpacerItem(
-            10, 0, QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Expanding
-        )
-
-        layout.addWidget(self.add_pos_button)
-        layout.addWidget(self.remove_pos_button)
-        layout.addWidget(self.clear_pos_button)
-        layout.addWidget(self.grid_button)
-        layout.addWidget(self.go)
-        layout.addItem(spacer)
-
-        group_layout.addWidget(wdg)
-
-    def _move_to_position(self) -> None:
-        if not self._mmc.getXYStageDevice():
-            return
-        curr_row = self.stage_tableWidget.currentRow()
-        x_val = self.stage_tableWidget.item(curr_row, 1).text()
-        y_val = self.stage_tableWidget.item(curr_row, 2).text()
-        z_val = self.stage_tableWidget.item(curr_row, 3).text()
-        self._mmc.setXYPosition(float(x_val), float(y_val))
-        self._mmc.setPosition(self._mmc.getFocusDevice(), float(z_val))
-
-
 class _MDAControlButtons(QWidget):
     def __init__(self, *, parent: QWidget | None = None) -> None:
         super().__init__(parent=parent)
 
         self._mmc = CMMCorePlus.instance()
         self._mmc.mda.events.sequencePauseToggled.connect(self._on_mda_paused)
+        self._mmc.mda.events.sequenceStarted.connect(self._on_mda_started)
+        self._mmc.mda.events.sequenceFinished.connect(self._on_mda_finished)
 
         self._create_btns_gui()
 
     def _create_btns_gui(self) -> None:
-
+        self.setMinimumWidth(300)
         self.setSizePolicy(QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Fixed)
         wdg_layout = QHBoxLayout()
         wdg_layout.setAlignment(Qt.AlignmentFlag.AlignVCenter)
         wdg_layout.setSpacing(10)
         wdg_layout.setContentsMargins(10, 5, 10, 10)
         self.setLayout(wdg_layout)
 
         acq_wdg = QWidget()
         acq_wdg_layout = QHBoxLayout()
         acq_wdg_layout.setSpacing(0)
         acq_wdg_layout.setContentsMargins(0, 0, 0, 0)
         acq_wdg.setLayout(acq_wdg_layout)
-        acquisition_order_label = QLabel(text="Acquisition Order:")
-        acquisition_order_label.setSizePolicy(
-            QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Fixed
-        )
-        self.acquisition_order_comboBox = QComboBox()
-        self.acquisition_order_comboBox.setMinimumWidth(100)
-        self.acquisition_order_comboBox.addItems(["tpcz", "tpzc", "ptzc", "ptcz"])
-        acq_wdg_layout.addWidget(acquisition_order_label)
-        acq_wdg_layout.addWidget(self.acquisition_order_comboBox)
 
         btn_sizepolicy = QSizePolicy(
             QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Fixed
         )
         min_width = 130
         icon_size = 40
         self.run_button = QPushButton(text="Run")
-        self.run_button.setEnabled(False)
         self.run_button.setMinimumWidth(min_width)
         self.run_button.setStyleSheet("QPushButton { text-align: center; }")
         self.run_button.setSizePolicy(btn_sizepolicy)
         self.run_button.setIcon(icon(MDI6.play_circle_outline, color=(0, 255, 0)))
         self.run_button.setIconSize(QSize(icon_size, icon_size))
         self.pause_button = QPushButton("Pause")
         self.pause_button.setStyleSheet("QPushButton { text-align: center; }")
@@ -169,18 +71,48 @@
 
         wdg_layout.addWidget(acq_wdg)
         wdg_layout.addItem(spacer)
         wdg_layout.addWidget(self.run_button)
         wdg_layout.addWidget(self.pause_button)
         wdg_layout.addWidget(self.cancel_button)
 
+    def _on_mda_started(self) -> None:
+        self.run_button.hide()
+        self.pause_button.show()
+        self.cancel_button.show()
+
+    def _on_mda_finished(self) -> None:
+        self.run_button.show()
+        self.pause_button.hide()
+        self.cancel_button.hide()
+        self.pause_button.setText("Pause")
+
     def _on_mda_paused(self, paused: bool) -> None:
         self.pause_button.setText("Resume" if paused else "Pause")
 
 
+class _AcquisitionOrderWidget(QWidget):
+    def __init__(self, *, parent: QWidget | None = None) -> None:
+        super().__init__(parent=parent)
+        self.setMaximumWidth(300)
+        acq_wdg_layout = QHBoxLayout()
+        self.setLayout(acq_wdg_layout)
+        acquisition_order_label = QLabel(text="Acquisition Order:")
+        acquisition_order_label.setSizePolicy(
+            QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Fixed
+        )
+        self.acquisition_order_comboBox = QComboBox()
+        self.acquisition_order_comboBox.setMinimumWidth(100)
+        self.acquisition_order_comboBox.addItems(
+            ["tpgcz", "tpgzc", "tpcgz", "tpzgc", "pgtzc", "ptzgc", "ptcgz", "pgtcz"]
+        )
+        acq_wdg_layout.addWidget(acquisition_order_label)
+        acq_wdg_layout.addWidget(self.acquisition_order_comboBox)
+
+
 class _MDATimeLabel(QWidget):
     def __init__(self, *, parent: QWidget | None = None) -> None:
         super().__init__(parent=parent)
 
         wdg_lay = QHBoxLayout()
         wdg_lay.setSpacing(5)
         wdg_lay.setContentsMargins(10, 5, 10, 5)
@@ -189,7 +121,29 @@
 
         self._total_time_lbl = QLabel()
         self._total_time_lbl.setAlignment(Qt.AlignmentFlag.AlignLeft)
         self._total_time_lbl.setSizePolicy(
             QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Fixed
         )
         wdg_lay.addWidget(self._total_time_lbl)
+
+
+class _SaveLoadSequenceWidget(QWidget):
+    def __init__(self, parent: QWidget | None = None) -> None:
+        super().__init__(parent)
+
+        self._save_button = QPushButton("Save")
+        self._load_button = QPushButton("Load")
+
+        self._save_button.setMaximumWidth(self._save_button.sizeHint().width())
+        self._load_button.setMaximumWidth(self._load_button.sizeHint().width())
+
+        self.setLayout(QHBoxLayout())
+
+        spacer = QSpacerItem(1, 1, QSizePolicy.Expanding, QSizePolicy.Minimum)
+
+        self.layout().addItem(spacer)
+        self.layout().addWidget(self._save_button)
+        self.layout().addWidget(self._load_button)
+
+        self.layout().setContentsMargins(0, 0, 0, 0)
+        self.layout().setSpacing(10)
```

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets/_mda/_mda_widget.py` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_stage_widget.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,333 +1,366 @@
 from __future__ import annotations
 
-from pathlib import Path
-from typing import TYPE_CHECKING
+from itertools import chain, product, repeat
+from typing import ClassVar
 
-from pymmcore_plus import CMMCorePlus
-from qtpy import QtWidgets as QtW
-from qtpy.QtCore import Qt
-from qtpy.QtWidgets import QScrollArea, QSizePolicy, QVBoxLayout, QWidget
-from useq import MDASequence
-
-from .._util import _select_output_unit, guess_channel_group
-from ._channel_table_widget import ChannelTable
-from ._general_mda_widgets import _MDAControlButtons, _MDATimeLabel
-from ._positions_table_widget import PositionTable
-from ._time_plan_widget import TimePlanWidget
-from ._zstack_widget import ZStackWidget
-
-if TYPE_CHECKING:
-    from typing_extensions import TypedDict
-
-    class PositionDict(TypedDict, total=False):
-        """Position dictionary."""
-
-        x: float | None
-        y: float | None
-        z: float | None
-        name: str | None
-
-
-LBL_SIZEPOLICY = QSizePolicy(QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Fixed)
-
-
-class MDAWidget(QWidget):
-    """A Multi-dimensional acquisition Widget.
-
-    The `MDAWidget` provides a GUI to construct a
-    [`useq.MDASequence`](https://github.com/tlambert03/useq-schema) object.
-    If the `include_run_button` parameter is set to `True`, a "run" button is added
-    to the GUI and, when clicked, the generated
-    [`useq.MDASequence`](https://github.com/tlambert03/useq-schema)
-    is passed to the
-    [`CMMCorePlus.instance`][pymmcore_plus.core._mmcore_plus.CMMCorePlus.run_mda]
-    method and the acquisition
-    is executed.
+from fonticon_mdi6 import MDI6
+from pymmcore_plus import CMMCorePlus, DeviceType
+from qtpy.QtCore import Qt, QTimer
+from qtpy.QtWidgets import (
+    QCheckBox,
+    QDoubleSpinBox,
+    QGridLayout,
+    QHBoxLayout,
+    QLabel,
+    QPushButton,
+    QRadioButton,
+    QSpinBox,
+    QVBoxLayout,
+    QWidget,
+)
+from superqt.fonticon import setTextIcon
+from superqt.utils import signals_blocked
+
+AlignCenter = Qt.AlignmentFlag.AlignCenter
+PREFIX = MDI6.__name__.lower()
+STAGE_DEVICES = {DeviceType.Stage, DeviceType.XYStage}
+STYLE = """
+QPushButton {
+    border: none;
+    background: transparent;
+    color: rgb(0, 180, 0);
+    font-size: 40px;
+}
+QPushButton:hover:!pressed {
+    color: rgb(0, 255, 0);
+}
+QPushButton:pressed {
+    color: rgb(0, 100, 0);
+}
+QSpinBox {
+    min-width: 35px;
+    height: 22px;
+}
+QLabel {
+    color: #999;
+}
+QCheckBox {
+    color: #999;
+}
+QCheckBox::indicator {
+    width: 11px;
+    height: 11px;
+}
+"""
+
+
+class StageWidget(QWidget):
+    """A Widget to control a XY and/or a Z stage.
 
     Parameters
     ----------
+    device: str:
+        Stage device.
+    levels: int | None:
+        Number of "arrow" buttons per widget per direction, by default, 2.
     parent : QWidget | None
-        Optional parent widget, by default None.
-    include_run_button: bool
-        By default, `False`. If `True`, a "run" button is added to the widget.
-        The acquisition defined by the
-        [`useq.MDASequence`](https://github.com/tlambert03/useq-schema)
-        built through the widget is executed when clicked.
+        Optional parent widget.
     mmcore : CMMCorePlus | None
         Optional [`pymmcore_plus.CMMCorePlus`][] micromanager core.
         By default, None. If not specified, the widget will use the active
         (or create a new)
         [`CMMCorePlus.instance`][pymmcore_plus.core._mmcore_plus.CMMCorePlus.instance].
     """
 
+    # fmt: off
+    BTNS: ClassVar[ dict]= {
+        # btn glyph                (r, c, xmag, ymag)
+        MDI6.chevron_triple_up:    (0, 3,  0,  3),
+        MDI6.chevron_double_up:    (1, 3,  0,  2),
+        MDI6.chevron_up:           (2, 3,  0,  1),
+        MDI6.chevron_down:         (4, 3,  0, -1),
+        MDI6.chevron_double_down:  (5, 3,  0, -2),
+        MDI6.chevron_triple_down:  (6, 3,  0, -3),
+        MDI6.chevron_triple_left:  (3, 0, -3,  0),
+        MDI6.chevron_double_left:  (3, 1, -2,  0),
+        MDI6.chevron_left:         (3, 2, -1,  0),
+        MDI6.chevron_right:        (3, 4,  1,  0),
+        MDI6.chevron_double_right: (3, 5,  2,  0),
+        MDI6.chevron_triple_right: (3, 6,  3,  0),
+    }
+    BTN_SIZE = 30
+    # fmt: on
+
     def __init__(
         self,
+        device: str,
+        levels: int | None = 2,
         *,
-        parent: QtW.QWidget | None = None,
-        include_run_button: bool = False,
+        parent: QWidget | None = None,
         mmcore: CMMCorePlus | None = None,
-    ) -> None:
+    ):
         super().__init__(parent=parent)
 
-        self._mmc = mmcore or CMMCorePlus.instance()
-        self._include_run_button = include_run_button
+        self.setStyleSheet(STYLE)
 
-        # Widgets for Channels, Time, ZStack, and Positions in the Scroll Area
-        self.channel_groupbox = ChannelTable()
-        self.channel_groupbox.valueChanged.connect(self._enable_run_btn)
-
-        self.time_groupbox = TimePlanWidget()
-        self.time_groupbox.setChecked(False)
-
-        self.stack_groupbox = ZStackWidget()
-        self.stack_groupbox.setChecked(False)
-
-        self.position_groupbox = PositionTable()
-        self.position_groupbox.setChecked(False)
-
-        # below the scroll area, some feedback widgets and buttons
-        self.time_lbl = _MDATimeLabel()
-
-        self.buttons_wdg = _MDAControlButtons()
-        self.buttons_wdg.pause_button.hide()
-        self.buttons_wdg.cancel_button.hide()
-        self.buttons_wdg.run_button.hide()
-
-        # LAYOUT
-
-        central_layout = QVBoxLayout()
-        central_layout.setSpacing(20)
-        central_layout.setContentsMargins(10, 10, 10, 10)
-        central_layout.addWidget(self.channel_groupbox)
-        central_layout.addWidget(self.time_groupbox)
-        central_layout.addWidget(self.stack_groupbox)
-        central_layout.addWidget(self.position_groupbox)
-        self._central_widget = QWidget()
-        self._central_widget.setLayout(central_layout)
-
-        scroll = QScrollArea()
-        scroll.setWidgetResizable(True)
-        scroll.setAlignment(Qt.AlignmentFlag.AlignCenter)
-        scroll.setWidget(self._central_widget)
+        self._mmc = mmcore or CMMCorePlus.instance()
+        self._levels = levels
+        self._device = device
+        self._dtype = self._mmc.getDeviceType(self._device)
+        assert self._dtype in STAGE_DEVICES, f"{self._dtype} not in {STAGE_DEVICES}"
+
+        self._create_widget()
+
+        self._connect_events()
+
+        self._set_as_default()
+
+        self.destroyed.connect(self._disconnect)
+
+    def _create_widget(self) -> None:
+        self._step = QDoubleSpinBox()
+        self._step.setValue(10)
+        self._step.setMaximum(9999)
+        self._step.valueChanged.connect(self._update_ttips)
+        self._step.clearFocus()
+        self._step.setAttribute(Qt.WidgetAttribute.WA_MacShowFocusRect, 0)
+        self._step.setButtonSymbols(QSpinBox.ButtonSymbols.NoButtons)
+        self._step.setAlignment(AlignCenter)
+
+        self._btns = QWidget()
+        self._btns.setLayout(QGridLayout())
+        self._btns.layout().setContentsMargins(0, 0, 0, 0)
+        self._btns.layout().setSpacing(0)
+        for glpyh, (row, col, *_) in self.BTNS.items():
+            btn = QPushButton()
+            btn.setAutoRepeat(True)
+            btn.setFlat(True)
+            btn.setFixedSize(self.BTN_SIZE, self.BTN_SIZE)
+            btn.setFocusPolicy(Qt.FocusPolicy.NoFocus)
+            btn.setCursor(Qt.CursorShape.PointingHandCursor)
+            setTextIcon(btn, glpyh)
+            btn.clicked.connect(self._on_click)
+            self._btns.layout().addWidget(btn, row, col, AlignCenter)
+
+        self._btns.layout().addWidget(self._step, 3, 3, AlignCenter)
+        self._set_visible_levels(self._levels)  # type: ignore
+        self._set_xy_visible()
+        self._update_ttips()
+
+        self._readout = QLabel()
+        self._readout.setAlignment(AlignCenter)
+        self._update_position_label()
+
+        self._poll_cb = QCheckBox("poll")
+        self._poll_cb.setMaximumWidth(50)
+        self._poll_timer = QTimer()
+        self._poll_timer.setInterval(500)
+        self._poll_timer.timeout.connect(self._update_position_label)
+        self._poll_cb.toggled.connect(self._toggle_poll_timer)
+
+        self.snap_checkbox = QCheckBox(text="Snap on Click")
+
+        self.radiobutton = QRadioButton(text="Set as Default")
+        self.radiobutton.toggled.connect(self._on_radiobutton_toggled)
+
+        top_row = QWidget()
+        top_row_layout = QHBoxLayout()
+        top_row_layout.setAlignment(AlignCenter)
+        top_row.setLayout(top_row_layout)
+        top_row.layout().addWidget(self.radiobutton)
+
+        bottom_row_1 = QWidget()
+        bottom_row_1.setLayout(QHBoxLayout())
+        bottom_row_1.layout().addWidget(self._readout)
+
+        bottom_row_2 = QWidget()
+        bottom_row_2_layout = QHBoxLayout()
+        bottom_row_2_layout.setSpacing(10)
+        bottom_row_2_layout.setContentsMargins(0, 0, 0, 0)
+        bottom_row_2_layout.setAlignment(AlignCenter)
+        bottom_row_2.setLayout(bottom_row_2_layout)
+        bottom_row_2.layout().addWidget(self.snap_checkbox)
+        bottom_row_2.layout().addWidget(self._poll_cb)
 
         self.setLayout(QVBoxLayout())
-        self.layout().setSpacing(10)
-        self.layout().setContentsMargins(10, 10, 10, 10)
-        self.layout().addWidget(scroll)
-        self.layout().addWidget(self.time_lbl)
-        self.layout().addWidget(self.buttons_wdg)
-
-        # CONNECTIONS
-
-        self.buttons_wdg.pause_button.released.connect(self._mmc.mda.toggle_pause)
-        self.buttons_wdg.cancel_button.released.connect(self._mmc.mda.cancel)
-        # connect valueUpdated signal
-        self.channel_groupbox.valueChanged.connect(self._update_total_time)
-        self.stack_groupbox.valueChanged.connect(self._update_total_time)
-        self.time_groupbox.valueChanged.connect(self._update_total_time)
-        self.time_groupbox.toggled.connect(self._update_total_time)
-        self.position_groupbox.valueChanged.connect(self._update_total_time)
-        # connect mmcore signals
-        self._mmc.mda.events.sequenceStarted.connect(self._on_mda_started)
-        self._mmc.mda.events.sequenceFinished.connect(self._on_mda_finished)
-        self._mmc.events.systemConfigurationLoaded.connect(self._on_sys_cfg_loaded)
-
-        # connect run button
-        if self._include_run_button:
-            self.buttons_wdg.run_button.clicked.connect(self._on_run_clicked)
-            self.buttons_wdg.run_button.show()
-
-        self._on_sys_cfg_loaded()
-
-    def _on_sys_cfg_loaded(self) -> None:
-        if channel_group := self._mmc.getChannelGroup() or guess_channel_group():
-            self._mmc.setChannelGroup(channel_group)
-        self.channel_groupbox.clear()
-
-    def _set_enabled(self, enabled: bool) -> None:
-        self.time_groupbox.setEnabled(enabled)
-        self.buttons_wdg.acquisition_order_comboBox.setEnabled(enabled)
-        self.channel_groupbox.setEnabled(enabled)
-
-        if not self._mmc.getXYStageDevice():
-            self.position_groupbox.setChecked(False)
-            self.position_groupbox.setEnabled(False)
-        else:
-            self.position_groupbox.setEnabled(enabled)
-
-        if not self._mmc.getFocusDevice():
-            self.stack_groupbox.setChecked(False)
-            self.stack_groupbox.setEnabled(False)
-        else:
-            self.stack_groupbox.setEnabled(enabled)
-
-    def _on_mda_started(self) -> None:
-        self._set_enabled(False)
-        if self._include_run_button:
-            self.buttons_wdg.pause_button.show()
-            self.buttons_wdg.cancel_button.show()
-        self.buttons_wdg.run_button.hide()
-
-    def _on_mda_finished(self) -> None:
-        self._set_enabled(True)
-        self.buttons_wdg.pause_button.hide()
-        self.buttons_wdg.cancel_button.hide()
-        if self._include_run_button:
-            self.buttons_wdg.run_button.show()
-
-    def _on_mda_paused(self, paused: bool) -> None:
-        self.buttons_wdg.pause_button.setText("Resume" if paused else "Pause")
-
-    def set_state(self, state: dict | MDASequence | str | Path) -> None:
-        """Set current state of MDA widget.
-
-        Parameters
-        ----------
-        state : dict | MDASequence | str | Path
-            MDASequence state in the form of a dict, MDASequence object, or a str or
-            Path pointing to a sequence.yaml file
-        """
-        # sourcery skip: low-code-quality
-        if isinstance(state, (str, Path)):
-            state = MDASequence.parse_file(state)
-        elif isinstance(state, dict):
-            state = MDASequence(**state)
-        if not isinstance(state, MDASequence):
-            raise TypeError("state must be an MDASequence, dict, or yaml file")
-
-        self.buttons_wdg.acquisition_order_comboBox.setCurrentText(state.axis_order)
-
-        # set channel table
-        if state.channels:
-            self.channel_groupbox.set_state([c.dict() for c in state.channels])
-
-        # set Z
-        if state.z_plan:
-            self.stack_groupbox.setChecked(True)
-            self.stack_groupbox.set_state(state.z_plan.dict())
-        else:
-            self.stack_groupbox.setChecked(False)
-
-        # set time
-        if state.time_plan:
-            self.time_groupbox.setChecked(True)
-            self.time_groupbox.set_state(state.time_plan.dict())
+        self.layout().setSpacing(0)
+        self.layout().setContentsMargins(5, 5, 5, 5)
+        self.layout().addWidget(top_row)
+        self.layout().addWidget(self._btns, AlignCenter)
+        self.layout().addWidget(bottom_row_1)
+        self.layout().addWidget(bottom_row_2)
+
+    def _connect_events(self) -> None:
+        self._mmc.events.propertyChanged.connect(self._on_prop_changed)
+        self._mmc.events.systemConfigurationLoaded.connect(self._on_system_cfg)
+        if self._dtype is DeviceType.XYStage:
+            event = self._mmc.events.XYStagePositionChanged
+        elif self._dtype is DeviceType.Stage:
+            event = self._mmc.events.stagePositionChanged
+        event.connect(self._update_position_label)
+
+    def _enable_wdg(self, enabled: bool) -> None:
+        self._step.setEnabled(enabled)
+        self._btns.setEnabled(enabled)
+        self.snap_checkbox.setEnabled(enabled)
+        self.radiobutton.setEnabled(enabled)
+        self._poll_cb.setEnabled(enabled)
+
+    def _on_system_cfg(self) -> None:
+        if self._dtype is DeviceType.XYStage:
+            if self._device not in self._mmc.getLoadedDevicesOfType(DeviceType.XYStage):
+                self._enable_and_update(False)
+            else:
+                self._enable_and_update(True)
+
+        if self._dtype is DeviceType.Stage:
+            if self._device not in self._mmc.getLoadedDevicesOfType(DeviceType.Stage):
+                self._enable_and_update(False)
+            else:
+                self._enable_and_update(True)
+
+        self._set_as_default()
+
+    def _enable_and_update(self, enable: bool) -> None:
+        if enable:
+            self._enable_wdg(True)
+            self._update_position_label()
         else:
-            self.time_groupbox.setChecked(False)
+            self._readout.setText(f"{self._device} not loaded.")
+            self._enable_wdg(False)
 
-        # set stage positions
-        if state.stage_positions:
-            self.position_groupbox.set_state([p.dict() for p in state.stage_positions])
+    def _set_as_default(self) -> None:
+        current_xy = self._mmc.getXYStageDevice()
+        current_z = self._mmc.getFocusDevice()
+        if self._dtype is DeviceType.XYStage and current_xy == self._device:
+            self.radiobutton.setChecked(True)
+        elif self._dtype is DeviceType.Stage and current_z == self._device:
+            self.radiobutton.setChecked(True)
+
+    def _on_radiobutton_toggled(self, state: bool) -> None:
+        if self._dtype is DeviceType.XYStage:
+            if state:
+                self._mmc.setProperty("Core", "XYStage", self._device)
+            elif (
+                not state
+                and len(self._mmc.getLoadedDevicesOfType(DeviceType.XYStage)) == 1
+            ):
+                with signals_blocked(self.radiobutton):
+                    self.radiobutton.setChecked(True)
+            else:
+                self._mmc.setProperty("Core", "XYStage", "")
+
+        elif self._dtype is DeviceType.Stage:
+            if state:
+                self._mmc.setProperty("Core", "Focus", self._device)
+            elif (
+                not state
+                and len(self._mmc.getLoadedDevicesOfType(DeviceType.Stage)) == 1
+            ):
+                with signals_blocked(self.radiobutton):
+                    self.radiobutton.setChecked(True)
+            else:
+                self._mmc.setProperty("Core", "Focus", "")
+
+    def _on_prop_changed(self, dev: str, prop: str, val: str) -> None:
+        if dev != "Core":
+            return
+
+        if self._dtype is DeviceType.XYStage and prop == "XYStage":
+            with signals_blocked(self.radiobutton):
+                self.radiobutton.setChecked(val == self._device)
+
+        if self._dtype is DeviceType.Stage and prop == "Focus":
+            with signals_blocked(self.radiobutton):
+                self.radiobutton.setChecked(val == self._device)
+
+    def _toggle_poll_timer(self, on: bool) -> None:
+        self._poll_timer.start() if on else self._poll_timer.stop()
+
+    def _update_position_label(self) -> None:
+        if (
+            self._dtype is DeviceType.XYStage
+            and self._device in self._mmc.getLoadedDevicesOfType(DeviceType.XYStage)
+        ):
+            pos = self._mmc.getXYPosition(self._device)  # type: ignore # pymmcore wrong
+            p = ", ".join(str(round(x, 2)) for x in pos)
+            self._readout.setText(f"{self._device}:  {p}")
+        elif (
+            self._dtype is DeviceType.Stage
+            and self._device in self._mmc.getLoadedDevicesOfType(DeviceType.Stage)
+        ):
+            p = str(round(self._mmc.getPosition(self._device), 2))
+            self._readout.setText(f"{self._device}:  {p}")
+
+    def _update_ttips(self) -> None:
+        coords = chain(zip(repeat(3), range(7)), zip(range(7), repeat(3)))
+        Y = {DeviceType.XYStage: "Y"}.get(self._dtype, "Z")
+
+        btn_layout: QGridLayout = self._btns.layout()
+        for r, c in coords:
+            if item := btn_layout.itemAtPosition(r, c):
+                if (r, c) == (3, 3):
+                    continue
+                if btn := item.widget():
+                    xmag, ymag = self.BTNS[f"{PREFIX}.{btn.text()}"][-2:]
+                    if xmag:
+                        btn.setToolTip(f"move X by {self._scale(xmag)} µm")
+                    elif ymag:
+                        btn.setToolTip(f"move {Y} by {self._scale(ymag)} µm")
+
+    def _set_xy_visible(self) -> None:
+        if self._dtype is not DeviceType.XYStage:
+            btn_layout: QGridLayout = self._btns.layout()
+            for c in (0, 1, 2, 4, 5, 6):
+                if item := btn_layout.itemAtPosition(3, c):
+                    item.widget().hide()
+
+    def _set_visible_levels(self, levels: int) -> None:
+        """Hide upper-level stage buttons as desired. Levels must be between 1-3."""
+        assert 1 <= levels <= 3, "levels must be between 1-3"
+        btn_layout: QGridLayout = self._btns.layout()
+        for btn in self._btns.findChildren(QPushButton):
+            btn.show()
+        if levels < 3:
+            # hide row/col 0, 6
+            for r, c in product(range(7), (0, 6)):
+                if item := btn_layout.itemAtPosition(r, c):
+                    item.widget().hide()
+                if item := btn_layout.itemAtPosition(c, r):
+                    item.widget().hide()
+        if levels < 2:
+            # hide row/col 1, 5
+            for r, c in product(range(1, 6), (1, 5)):
+                if item := btn_layout.itemAtPosition(r, c):
+                    item.widget().hide()
+                if item := btn_layout.itemAtPosition(c, r):
+                    item.widget().hide()
+
+    def _on_click(self) -> None:
+        btn: QPushButton = self.sender()
+        xmag, ymag = self.BTNS[f"{PREFIX}.{btn.text()}"][-2:]
+        self._move_stage(self._scale(xmag), self._scale(ymag))
+
+    def _move_stage(self, x: float, y: float) -> None:
+        if self._dtype is DeviceType.XYStage:
+            self._mmc.setRelativeXYPosition(self._device, x, y)
         else:
-            self.position_groupbox.setChecked(False)
+            self._mmc.setRelativePosition(self._device, y)
+        if self.snap_checkbox.isChecked():
+            self._mmc.snap()
 
-    def get_state(self) -> MDASequence:
-        """Get current state of widget and build a useq.MDASequence.
+    def _scale(self, mag: int) -> float:
+        """Convert step mag of (1, 2, 3) to absolute XY units.
 
-        Returns
-        -------
-        useq.MDASequence
+        Can be used to step 1x field of view, etc...
         """
-        channels = self.channel_groupbox.value()
-
-        z_plan = (
-            self.stack_groupbox.value() if self.stack_groupbox.isChecked() else None
-        )
-        time_plan = (
-            self.time_groupbox.value() if self.time_groupbox.isChecked() else None
-        )
-
-        stage_positions = (
-            self.position_groupbox.value()
-            if self.position_groupbox.isChecked()
-            else self._get_current_position()
-        )
-
-        return MDASequence(
-            axis_order=self.buttons_wdg.acquisition_order_comboBox.currentText(),
-            channels=channels,
-            stage_positions=stage_positions,
-            z_plan=z_plan,
-            time_plan=time_plan,
-        )
-
-    def _get_current_position(self) -> list[PositionDict]:
-        return [
-            {
-                "name": "Pos000",
-                "x": (
-                    self._mmc.getXPosition() if self._mmc.getXYStageDevice() else None
-                ),
-                "y": (
-                    self._mmc.getYPosition() if self._mmc.getXYStageDevice() else None
-                ),
-                "z": (self._mmc.getZPosition() if self._mmc.getFocusDevice() else None),
-            }
-        ]
-
-    def _on_run_clicked(self) -> None:
-        """Run the MDA sequence experiment."""
-        # construct a `useq.MDASequence` object from the values inserted in the widget
-        experiment = self.get_state()
-        # run the MDA experiment asynchronously
-        self._mmc.run_mda(experiment)
-        return
-
-    def _enable_run_btn(self) -> None:
-        self.buttons_wdg.run_button.setEnabled(
-            self.channel_groupbox._table.rowCount() > 0
-        )
-
-    def _update_total_time(self, *, tiles: int = 1) -> None:
-        """Update the minimum total acquisition time info."""
-        # channel
-        exp: list[float] = [
-            e for c in self.channel_groupbox.value() if (e := c.get("exposure"))
-        ]
-
-        # time
-        if self.time_groupbox.isChecked():
-            val = self.time_groupbox.value()
-            timepoints = val["loops"]
-            interval = val["interval"].total_seconds()
-        else:
-            timepoints = 1
-            interval = -1.0
-
-        # z stack
-        n_z_images = (
-            self.stack_groupbox.n_images() if self.stack_groupbox.isChecked() else 1
-        )
-
-        # positions
-        if self.position_groupbox.isChecked():
-            n_pos = len(self.position_groupbox.value()) or 1
-        else:
-            n_pos = 1
+        return float(mag * self._step.value())
 
-        # acq time per timepoint
-        time_chs: float = 0.0  # s
-        for e in exp:
-            time_chs = time_chs + ((e / 1000) * n_z_images * n_pos * tiles)
-
-        min_aq_tp, unit_1 = _select_output_unit(time_chs)
-
-        addition_time = 0.0
-        effective_interval = 0.0
-        if interval >= time_chs:
-            effective_interval = float(interval) - time_chs  # s
-            addition_time = effective_interval * timepoints  # s
-
-        min_tot_time, unit_4 = _select_output_unit(
-            (time_chs * timepoints) + addition_time - effective_interval
-        )
-
-        self.time_groupbox.setWarningVisible(0 < interval < time_chs)
-
-        t_per_tp_msg = ""
-        tot_acq_msg = f"Minimum total acquisition time: {min_tot_time:.4f} {unit_4}.\n"
-        if self.time_groupbox.isChecked():
-            t_per_tp_msg = (
-                f"Minimum acquisition time per timepoint: {min_aq_tp:.4f} {unit_1}."
-            )
-        self.time_lbl._total_time_lbl.setText(f"{tot_acq_msg}{t_per_tp_msg}")
+    def _disconnect(self) -> None:
+        self._mmc.events.propertyChanged.disconnect(self._on_prop_changed)
+        self._mmc.events.systemConfigurationLoaded.disconnect(self._on_system_cfg)
+        if self._dtype is DeviceType.XYStage:
+            event = self._mmc.events.XYStagePositionChanged
+        elif self._dtype is DeviceType.Stage:
+            event = self._mmc.events.stagePositionChanged
+        event.disconnect(self._update_position_label)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets/_mda/_positions_table_widget.py` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/_channel_table_widget.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,453 +1,455 @@
 from __future__ import annotations
 
 import warnings
-from itertools import groupby
 from typing import TYPE_CHECKING, cast
 
+from fonticon_mdi6 import MDI6
 from pymmcore_plus import CMMCorePlus
-from qtpy.QtCore import Qt, Signal
+from qtpy.QtCore import QSize, Qt, Signal
 from qtpy.QtWidgets import (
-    QAbstractItemView,
     QAbstractSpinBox,
+    QCheckBox,
+    QComboBox,
     QDoubleSpinBox,
-    QGroupBox,
+    QGridLayout,
     QHBoxLayout,
+    QLabel,
     QPushButton,
     QSizePolicy,
     QSpacerItem,
+    QSpinBox,
     QTableWidget,
-    QTableWidgetItem,
     QVBoxLayout,
     QWidget,
 )
+from superqt import fonticon
 from superqt.utils import signals_blocked
 
-from ._grid_widget import GridWidget
-
 if TYPE_CHECKING:
-    from typing_extensions import TypedDict
-
-    class PositionDict(TypedDict, total=False):
-        """Position dictionary."""
+    from typing_extensions import Required, TypedDict
 
-        x: float | None
-        y: float | None
-        z: float | None
-        name: str | None
+    class ChannelDict(TypedDict, total=False):
+        """Channel dictionary."""
 
+        config: Required[str]
+        group: str
+        exposure: float | None
+        z_offset: float
+        do_stack: bool
+        camera: str | None
+        acquire_every: int
 
-AlignCenter = Qt.AlignmentFlag.AlignHCenter | Qt.AlignmentFlag.AlignVCenter
 
-
-class PositionTable(QGroupBox):
-    """Widget providing options for setting up a multi-position acquisition.
+class ChannelTable(QWidget):
+    """Widget providing options for setting up a multi-channel acquisition.
 
     The `value()` method returns a dictionary with the current state of the widget, in a
-    format that matches one of the [useq-schema Position
-    specifications](https://pymmcore-plus.github.io/useq-schema/schema/axes/#useq.Position).
+    format that matches one of the [useq-schema Channel
+    specifications](https://pymmcore-plus.github.io/useq-schema/schema/axes/#useq.Channel).
+
+    Parameters
+    ----------
+    parent : QWidget | None
+        Optional parent widget. By default, None.
+    channel_group : str | None
+        Optional channel group that will be set as the widget's initial ChannelGroup.
+        By default, None.
+    mmcore : CMMCorePlus | None
+        Optional [`pymmcore_plus.CMMCorePlus`][] micromanager core.
+        By default, None. If not specified, the widget will use the active
+        (or create a new)
+        [`CMMCorePlus.instance`][pymmcore_plus.core._mmcore_plus.CMMCorePlus.instance].
     """
 
     valueChanged = Signal()
-    POS_ROLE = QTableWidgetItem.ItemType.UserType + 1
+    CH_GROUP_ROLE = Qt.ItemDataRole.UserRole + 1
 
     def __init__(
         self,
-        title: str = "Stage Positions",
         parent: QWidget | None = None,
+        *,
+        channel_group: str | None = None,
+        mmcore: CMMCorePlus | None = None,
     ) -> None:
         super().__init__(parent=parent)
 
-        self._mmc = CMMCorePlus.instance()
+        self._mmc = mmcore or CMMCorePlus.instance()
 
-        self.setTitle(title)
-
-        self.setCheckable(True)
-
-        group_layout = QHBoxLayout()
+        group_layout = QGridLayout()
         group_layout.setSpacing(15)
         group_layout.setContentsMargins(10, 10, 10, 10)
         self.setLayout(group_layout)
 
-        # table
+        # channel table
         self._table = QTableWidget()
-        self._table.setSelectionBehavior(QAbstractItemView.SelectionBehavior.SelectRows)
+        self._table.setMinimumHeight(175)
         hdr = self._table.horizontalHeader()
         hdr.setSectionResizeMode(hdr.ResizeMode.Stretch)
         self._table.verticalHeader().setVisible(False)
         self._table.setTabKeyNavigation(True)
-        self._table.setColumnCount(4)
+        self._table.setColumnCount(5)
         self._table.setRowCount(0)
-        self._table.setHorizontalHeaderLabels(["Pos", "X", "Y", "Z"])
-        group_layout.addWidget(self._table)
+        self._table.setHorizontalHeaderLabels(
+            ["Channel", "Exposure (ms)", "Z offset", "Z stack", "Acquire Every"]
+        )
+        group_layout.addWidget(self._table, 0, 0)
 
         # buttons
         wdg = QWidget()
         layout = QVBoxLayout()
         layout.setSpacing(10)
         layout.setContentsMargins(0, 0, 0, 0)
         wdg.setLayout(layout)
 
-        btn_sizepolicy = QSizePolicy(QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Fixed)
-        min_size = 100
-        self.add_button = QPushButton(text="Add")
-        self.add_button.setMinimumWidth(min_size)
-        self.add_button.setSizePolicy(btn_sizepolicy)
-        self.remove_button = QPushButton(text="Remove")
-        self.remove_button.setEnabled(False)
-        self.remove_button.setMinimumWidth(min_size)
-        self.remove_button.setSizePolicy(btn_sizepolicy)
-        self.clear_button = QPushButton(text="Clear")
-        self.clear_button.setMinimumWidth(min_size)
-        self.clear_button.setSizePolicy(btn_sizepolicy)
-        self.grid_button = QPushButton(text="Grid")
-        self.grid_button.setMinimumWidth(min_size)
-        self.grid_button.setSizePolicy(btn_sizepolicy)
-        self.go_button = QPushButton(text="Go")
-        self.go_button.setEnabled(False)
-        self.go_button.setMinimumWidth(min_size)
-        self.go_button.setSizePolicy(btn_sizepolicy)
+        # ChannelGroup combobox
+        self.channel_group_combo = ChannelGroupCombo(
+            self, channel_group=channel_group, mmcore=self._mmc
+        )
+        layout.addWidget(self.channel_group_combo)
+
+        self._add_button = QPushButton(text="Add")
+        self._remove_button = QPushButton(text="Remove")
+        self._clear_button = QPushButton(text="Clear")
+
+        self._add_button.clicked.connect(self._create_new_row)
+        self._remove_button.clicked.connect(self._remove_selected_rows)
+        self._clear_button.clicked.connect(self.clear)
 
         spacer = QSpacerItem(
             10, 0, QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Expanding
         )
 
-        layout.addWidget(self.add_button)
-        layout.addWidget(self.remove_button)
-        layout.addWidget(self.clear_button)
-        layout.addWidget(self.grid_button)
-        layout.addWidget(self.go_button)
+        advanced_wdg = QWidget()
+        advanced_wdg.setSizePolicy(QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Fixed)
+        advanced_layout = QHBoxLayout()
+        advanced_layout.setSpacing(5)
+        advanced_layout.setContentsMargins(0, 0, 0, 0)
+        advanced_wdg.setLayout(advanced_layout)
+        self._advanced_cbox = QCheckBox("Advanced")
+        self._advanced_cbox.toggled.connect(self._on_advanced_toggled)
+        self._warn_icon = QLabel()
+        self._warn_icon.setToolTip("Warning: some 'Advanced' values are selected!")
+        _icon = fonticon.icon(MDI6.alert_outline, color="magenta")
+        self._warn_icon.setPixmap(_icon.pixmap(QSize(25, 25)))
+        advanced_layout.addWidget(self._advanced_cbox)
+        advanced_layout.addWidget(self._warn_icon)
+        _w = (
+            self._advanced_cbox.sizeHint().width()
+            + self._warn_icon.sizeHint().width()
+            + advanced_layout.spacing()
+        )
+        advanced_wdg.setMinimumWidth(_w)
+        advanced_wdg.setMinimumHeight(advanced_wdg.sizeHint().height())
+        self._warn_icon.hide()
+
+        self._add_button.setMinimumWidth(_w)
+        self._remove_button.setMinimumWidth(_w)
+        self._clear_button.setMinimumWidth(_w)
+
+        layout.addWidget(self._add_button)
+        layout.addWidget(self._remove_button)
+        layout.addWidget(self._clear_button)
+        layout.addWidget(advanced_wdg)
         layout.addItem(spacer)
 
-        group_layout.addWidget(wdg)
-
-        self.add_button.clicked.connect(self._add_position)
-        self.remove_button.clicked.connect(self._remove_position)
-        self.clear_button.clicked.connect(self._clear_positions)
-        self.grid_button.clicked.connect(self._grid_widget)
-        self.go_button.clicked.connect(self._move_to_position)
-
-        self._table.selectionModel().selectionChanged.connect(self._enable_go_button)
-        self._table.selectionModel().selectionChanged.connect(
-            self._enable_remove_button
-        )
-        self._table.selectionModel().selectionChanged.connect(
-            self._select_all_grid_positions
-        )
+        group_layout.addWidget(wdg, 0, 1)
 
-        self._mmc.events.systemConfigurationLoaded.connect(self._clear_positions)
+        self._mmc.events.systemConfigurationLoaded.connect(self._on_sys_cfg_loaded)
+        self._mmc.events.configGroupDeleted.connect(self._on_group_deleted)
+        self._mmc.events.configDeleted.connect(self._on_config_deleted)
 
         self.destroyed.connect(self._disconnect)
 
-    def _enable_go_button(self) -> None:
-        rows = {r.row() for r in self._table.selectedIndexes()}
-        self.go_button.setEnabled(len(rows) == 1)
-
-    def _enable_remove_button(self) -> None:
-        rows = {r.row() for r in self._table.selectedIndexes()}
-        self.remove_button.setEnabled(len(rows) >= 1)
+        self._on_sys_cfg_loaded()
 
-    def _select_all_grid_positions(self) -> None:
-        """Select all grid positions from the same 'Gridnnn'."""
-        rows = {r.row() for r in self._table.selectedIndexes()}
+    def _on_sys_cfg_loaded(self) -> None:
+        self.clear()
+        self._advanced_cbox.setChecked(False)
+        self._on_advanced_toggled(False)
+
+    def _on_group_deleted(self, group: str) -> None:
+        """Remove rows that are using channels from the deleted group."""
+        row = 0
+        for ch in self.value():
+            if ch["group"] == group:
+                self._table.removeRow(row)
+            else:
+                row += 1
 
-        # get all the grid selected in the table
-        grid_to_select = []
-        for row in rows:
-            pos = self._table.item(row, 0).data(self.POS_ROLE).split("_")[0]
-            if "Grid" not in pos:
-                continue
-            if pos not in grid_to_select:
-                grid_to_select.append(pos)
-
-        # select all positions from the same grid
-        # activate MultiSelection
-        self._table.setSelectionMode(QAbstractItemView.MultiSelection)
+    def _on_config_deleted(self, group: str, config: str) -> None:
+        """Remove deleted config from channel combo if present."""
         for row in range(self._table.rowCount()):
-            n_grid = self._table.item(row, 0).data(self.POS_ROLE).split("_")[0]
-            if (
-                n_grid in grid_to_select
-                and not self._table.selectionModel().isRowSelected(row)
-            ):
-                with signals_blocked(self._table.selectionModel()):
-                    self._table.selectRow(row)
-        # revert back to ExtendedSelection
-        self._table.setSelectionMode(QAbstractItemView.ExtendedSelection)
-
-    def _add_position(self) -> None:
-
-        if not self._mmc.getXYStageDevice() and not self._mmc.getFocusDevice():
-            raise ValueError("No XY and Z Stage devices loaded.")
-
-        name = f"Pos{self._table.rowCount():03d}"
-        xpos = self._mmc.getXPosition() if self._mmc.getXYStageDevice() else None
-        ypos = self._mmc.getYPosition() if self._mmc.getXYStageDevice() else None
-        zpos = self._mmc.getZPosition() if self._mmc.getFocusDevice() else None
-
-        self._create_new_row(name, xpos, ypos, zpos)
+            combo = cast(QComboBox, self._table.cellWidget(row, 0))
+            items = [combo.itemText(ch) for ch in range(combo.count())]
+            items_data = {
+                combo.itemData(ch, self.CH_GROUP_ROLE) for ch in range(combo.count())
+            }
+            if group in items_data and config in items:
+                combo.clear()
+                combo.addItems(self._mmc.getAvailableConfigs(group))
+                for i in range(combo.count()):
+                    combo.setItemData(i, group, self.CH_GROUP_ROLE)
+                if self._mmc.getChannelGroup() != config:
+                    combo.setCurrentText(self._mmc.getChannelGroup())
+
+    def _on_advanced_toggled(self, state: bool) -> None:
+        for c in range(2, self._table.columnCount()):
+            self._table.setColumnHidden(c, not state)
+
+        if not state:
+            for v in self.value():
+                # if any of the advanced settings are different from their default
+                if v["z_offset"] != 0 or not v["do_stack"] or v["acquire_every"] != 1:
+                    self._warn_icon.show()
+                    return
+        self._warn_icon.hide()
+
+    def _pick_first_unused_channel(self, available: tuple[str, ...]) -> str:
+        """Return index of first unused channel."""
+        used = set()
+        for row in range(self._table.rowCount()):
+            combo = cast(QComboBox, self._table.cellWidget(row, 0))
+            used.add(combo.currentText())
 
-        self._rename_positions()
+        for ch in available:
+            if ch not in used:
+                return ch
+        return available[0]
+
+    def _create_spinbox(
+        self, range: tuple[int, int], double: bool = False
+    ) -> QDoubleSpinBox:
+        dspinbox = QDoubleSpinBox() if double else QSpinBox()
+        dspinbox.setButtonSymbols(QAbstractSpinBox.NoButtons)
+        dspinbox.setRange(*range)
+        dspinbox.setAlignment(Qt.AlignCenter)
+        dspinbox.wheelEvent = lambda event: None  # block mouse scroll
+        dspinbox.setKeyboardTracking(False)
+        dspinbox.valueChanged.connect(self.valueChanged)
+        return dspinbox
 
     def _create_new_row(
         self,
-        name: str | None,
-        xpos: float | None,
-        ypos: float | None,
-        zpos: float | None,
+        channel: str | None = None,
+        exposure: float | None = None,
+        channel_group: str | None = None,
+        z_offset: float = 0.0,
+        do_stack: bool = True,
+        acquire_every: int = 1,
     ) -> None:
+        """Create a new row in the table.
 
-        if not self._mmc.getXYStageDevice() and not self._mmc.getFocusDevice():
-            raise ValueError("No XY and Z Stage devices loaded.")
+        If 'channel' is not provided, the first unused channel will be used.
+        If 'exposure' is not provided, the current exposure will be used (or 100).
+        """
+        if len(self._mmc.getLoadedDevices()) <= 1:
+            warnings.warn("No devices loaded.", stacklevel=2)
+            return
 
-        row = self._add_position_row()
+        _channel_group = channel_group or self.channel_group_combo.currentText()
 
-        self._add_table_item(name, row, 0)
-        self._add_table_value(xpos, row, 1)
-        self._add_table_value(ypos, row, 2)
-        if zpos is None or not self._mmc.getFocusDevice():
-            self.valueChanged.emit()
+        if not _channel_group:
+            warnings.warn("First select Micro-Manager 'ChannelGroup'.", stacklevel=2)
             return
-        self._add_table_value(zpos, row, 3)
 
-        self.valueChanged.emit()
+        # channel dropdown
+        channel_combo = QComboBox()
+        available = self._mmc.getAvailableConfigs(_channel_group)
+        channel = channel or self._pick_first_unused_channel(available)
+        channel_combo.addItems(available)
+        for i in range(channel_combo.count()):
+            channel_combo.setItemData(i, _channel_group, self.CH_GROUP_ROLE)
+        channel_combo.setCurrentText(channel)
+
+        # exposure spinbox
+        channel_exp_spinbox = self._create_spinbox((0, 10000), True)
+        channel_exp_spinbox.setMinimum(1)
+        channel_exp_spinbox.setValue(exposure or self._mmc.getExposure() or 100)
+
+        # z offset spinbox
+        z_offset_spinbox = self._create_spinbox((-10000, 10000), True)
+        z_offset_spinbox.setValue(z_offset)
+
+        # z stack checkbox
+        # creating a wrapper widget so that the checkbox appears centered.
+        z_stack_wdg = QWidget()
+        z_stack_layout = QHBoxLayout()
+        z_stack_layout.setContentsMargins(0, 0, 0, 0)
+        z_stack_layout.setAlignment(Qt.AlignCenter)
+        z_stack_wdg.setLayout(z_stack_layout)
+        z_stack_checkbox = QCheckBox()
+        z_stack_checkbox.setChecked(do_stack)
+        z_stack_checkbox.stateChanged.connect(self.valueChanged)
+        z_stack_layout.addWidget(z_stack_checkbox)
+
+        # acqire every spinbox
+        acquire_every_spinbox = self._create_spinbox((1, 10000))
+        acquire_every_spinbox.setValue(acquire_every)
 
-    def _add_position_row(self) -> int:
         idx = self._table.rowCount()
         self._table.insertRow(idx)
-        return cast(int, idx)
-
-    def _add_table_value(self, value: float | None, row: int, col: int) -> None:
-        if value is None:
-            return
-        spin = QDoubleSpinBox()
-        spin.setAlignment(AlignCenter)
-        spin.setMaximum(1000000.0)
-        spin.setMinimum(-1000000.0)
-        spin.setButtonSymbols(QAbstractSpinBox.ButtonSymbols.NoButtons)
-        spin.setValue(value)
-        self._table.setCellWidget(row, col, spin)
-
-    def _add_table_item(self, table_item: str | None, row: int, col: int) -> None:
-        item = QTableWidgetItem(table_item)
-        # data(self.POS_ROLE) is used to keep track of grid and/or position
-        # even when the user changed the name in the table.
-        item.setData(self.POS_ROLE, table_item)
-        item.setToolTip(table_item)
-        item.setTextAlignment(AlignCenter)
-        self._table.setItem(row, col, item)
+        self._table.setCellWidget(idx, 0, channel_combo)
+        self._table.setCellWidget(idx, 1, channel_exp_spinbox)
+        self._table.setCellWidget(idx, 2, z_offset_spinbox)
+        self._table.setCellWidget(idx, 3, z_stack_wdg)
+        self._table.setCellWidget(idx, 4, acquire_every_spinbox)
+        self.valueChanged.emit()
 
-    def _remove_position(self) -> None:
+    def _z_stack_checkbox(self, row: int) -> QCheckBox:
+        return self._table.cellWidget(row, 3).layout().itemAt(0).widget()
 
+    def _remove_selected_rows(self) -> None:
         rows = {r.row() for r in self._table.selectedIndexes()}
-        grid_to_delete = []
-
+        if not rows:
+            return
         for idx in sorted(rows, reverse=True):
+            self._table.removeRow(idx)
+        self.valueChanged.emit()
 
-            pos_role = self._table.item(idx, 0).data(self.POS_ROLE)
-            # store grid name if is a grid position
-            if "Grid" in pos_role:
-                grid_name = pos_role.split("_")[0]
-                grid_to_delete.append(grid_name)
-            else:
-                # remove if is a single position
-                self._table.removeRow(idx)
+    def clear(self) -> None:
+        """Clear the channel table."""
+        if self._table.rowCount():
+            self._table.clearContents()
+            self._table.setRowCount(0)
+            self.valueChanged.emit()
 
-        # remove grid positions
-        for gridname in grid_to_delete:
-            self._delete_grid_positions(gridname)
+    def value(self) -> list[ChannelDict]:
+        """Return the current channels settings as a list of dictionaries.
 
-        self._rename_positions()
-        self.valueChanged.emit()
+        Note that the output will match the [useq-schema Channel
+        specifications](https://pymmcore-plus.github.io/useq-schema/schema/axes/#useq.Channel).
+        """
+        values: list[ChannelDict] = []
+        for c in range(self._table.rowCount()):
+            name_widget = cast("QComboBox", self._table.cellWidget(c, 0))
+            exposure_widget = cast("QDoubleSpinBox", self._table.cellWidget(c, 1))
+            if name_widget and exposure_widget:
+                values.append(
+                    {
+                        "config": name_widget.currentText(),
+                        "group": name_widget.itemData(
+                            name_widget.currentIndex(), self.CH_GROUP_ROLE
+                        ),
+                        "exposure": exposure_widget.value(),
+                        # NOTE: the columns representing these values *may* be hidden
+                        # ... but we are still using them
+                        "z_offset": (
+                            cast("QDoubleSpinBox", self._table.cellWidget(c, 2)).value()
+                        ),
+                        "do_stack": (self._z_stack_checkbox(c).isChecked()),
+                        "acquire_every": (
+                            cast("QSpinBox", self._table.cellWidget(c, 4)).value()
+                        ),
+                    }
+                )
+        return values
 
-    def _delete_grid_positions(self, name: list[str]) -> None:
-        """Remove all positions related to the same grid."""
-        for row in reversed(range(self._table.rowCount())):
-            if name in self._table.item(row, 0).data(self.POS_ROLE):
-                self._table.removeRow(row)
+    # note: this really ought to be ChannelDict, but it makes typing elsewhere harder
+    # TODO: also accept actual useq objects
+    def set_state(self, channels: list[dict]) -> None:
+        """Set the state of the widget.
+
+        Parameters
+        ----------
+        channels : list[dict]
+            A list of dictionaries following the [useq-schema Channel specifications](
+            https://pymmcore-plus.github.io/useq-schema/schema/axes/#useq.Channel).
+        """
+        _advanced_bool = False
+        with signals_blocked(self):
+            self.clear()
+            for channel in channels:
+                ch = channel.get("config")
+                group = channel.get("group")
+
+                if not ch:
+                    raise ValueError("Dictionary should contain channel 'config' name.")
+                avail_configs = self._mmc.getAvailableConfigs(
+                    group or self.channel_group_combo.currentText()
+                )
+                if ch not in avail_configs:
+                    warnings.warn(
+                        f"'{ch}' config or its group doesn't exist in the "
+                        f"'{group}' ChannelGroup!",
+                        stacklevel=2,
+                    )
+                    continue
+
+                exposure = channel.get("exposure") or self._mmc.getExposure()
+                z_offset = channel.get("z_offset") or 0.0
+                do_stack = channel["do_stack"] if "do_stack" in channel else True
+                acquire_every = channel.get("acquire_every") or 1
+                self._create_new_row(
+                    ch, exposure, group, z_offset, do_stack, acquire_every
+                )
+
+                # if any of the advanced settings are different from their default
+                if z_offset != 0.0 or not do_stack or acquire_every != 1:
+                    _advanced_bool = True
 
-    def _rename_positions(self) -> None:
-        single_pos_count = 0
-        single_pos_rows: list[int] = []
-        grid_info: list[tuple[str, str, int]] = []
-        for row in range(self._table.rowCount()):
-            name = self._table.item(row, 0).text()
-            pos_role = self._table.item(row, 0).data(self.POS_ROLE)
+            self._advanced_cbox.setChecked(_advanced_bool)
 
-            if "Grid" in pos_role.split("_")[0]:
-                grid_info.append((name, pos_role, row))
-                continue
-
-            if name == pos_role:  # name = Posnnn and pos_role = Posnnn
-                pos_number = self._update_number(single_pos_count, single_pos_rows)
-                new_name = f"Pos{pos_number:03d}"
-                single_pos_count = pos_number + 1
-                self._update_table_item(new_name, row, 0)
-
-            elif "Grid" not in pos_role:  # pos_role = Posnnn
-                single_pos_rows.append(row)
-                new_pos_role = f"Pos{row:03d}"
-                self._update_table_item(new_pos_role, row, 0, False)
+        self.valueChanged.emit()
 
-        if not grid_info:
-            return
+    def _disconnect(self) -> None:
+        self._mmc.events.systemConfigurationLoaded.disconnect(self._on_sys_cfg_loaded)
+        self._mmc.events.configGroupDeleted.disconnect(self._on_group_deleted)
+        self._mmc.events.configDeleted.disconnect(self._on_config_deleted)
 
-        self._rename_grid_positions(grid_info)
 
-    def _update_table_item(
-        self, name: str, row: int, col: int, update_name: bool = True
-    ) -> None:
-        if update_name:
-            self._table.item(row, col).setText(name)
-        self._table.item(row, col).setData(self.POS_ROLE, name)
-        self._table.item(row, col).setToolTip(name)
-
-    def _update_number(self, number: int, exixting_numbers: list[int]) -> int:
-        loop = True
-        while loop:
-            if number in exixting_numbers:
-                number += 1
-            else:
-                loop = False
-        return number
+class ChannelGroupCombo(QComboBox):
+    """QComboBox to set the channel group to use in the ChannelTable."""
 
-    def _rename_grid_positions(self, grid_info: list[tuple[str, str, int]]) -> None:
-        """Rename postions created with the GridWidget.
+    def __init__(
+        self,
+        parent: QWidget | None = None,
+        *,
+        channel_group: str | None = None,
+        mmcore: CMMCorePlus | None = None,
+    ) -> None:
+        super().__init__(parent)
 
-        grid_info = [(name, pos_role, row), ...].
-        By default, name is 'Gridnnn_Posnnn' but users can rename.
+        self.setSizeAdjustPolicy(QComboBox.AdjustToContents)
 
-        Example
-        -------
-        grid_info = [
-            (Grid000_Pos000, Grid000_Pos000, 1),
-            (Grid000_Pos001, Grid000_Pos001, 2),
-            (test0, Grid001_Pos000, 3),
-            (test1, Grid001_Pos001, 4),
-        ]
-        """
-        # first create a new list with items grouped by grid pos_role property
-        ordered_by_grid_n = [
-            list(grid_n)
-            for _, grid_n in groupby(grid_info, lambda x: x[1].split("_")[0])
-        ]
-
-        # then rename each grid with new neame and new pos_role
-        for idx, i in enumerate(ordered_by_grid_n):
-            for pos_idx, n in enumerate(i):
-                name, pos_role, row = n
-                new_name = f"Grid{idx:03d}_Pos{pos_idx:03d}"
-                self._update_table_item(new_name, row, 0, name == pos_role)
-
-    def _clear_positions(self) -> None:
-        """clear all positions."""
-        self._table.clearContents()
-        self._table.setRowCount(0)
-        self.valueChanged.emit()
+        self._mmc = mmcore or CMMCorePlus.instance()
+        self._channel_group = channel_group or self._mmc.getChannelGroup()
 
-    def _grid_widget(self) -> None:
-        if not self._mmc.getXYStageDevice():
-            return
-        if not hasattr(self, "_grid_wdg"):
-            self._grid_wdg = GridWidget(parent=self)
-            self._grid_wdg.sendPosList.connect(self._add_grid_positions_to_table)
-        self._grid_wdg.show()
-        self._grid_wdg.raise_()
+        # connect core
+        self._mmc.events.systemConfigurationLoaded.connect(self._on_sys_cfg_loaded)
+        self._mmc.events.configGroupDeleted.connect(self._update_channel_group_combo)
+        self._mmc.events.configDefined.connect(self._update_channel_group_combo)
 
-    def _add_grid_positions_to_table(
-        self, position_list: list[tuple[float, ...]], clear: bool
-    ) -> None:
+        self.destroyed.connect(self._disconnect)
 
-        grid_number = -1
+        self._update_channel_group_combo()
 
-        if clear:
-            self._clear_positions()
-        else:
-            for r in range(self._table.rowCount()):
-                pos_name = self._table.item(r, 0).data(self.POS_ROLE)
-                grid_name = pos_name.split("_")[0]  # e.g. Grid000
-                if "Grid" in grid_name:
-                    grid_n = grid_name[-3:]
-                    if int(grid_n) > grid_number:
-                        grid_number = int(grid_n)
-
-        grid_number = 0 if grid_number < 0 else grid_number + 1
-
-        for idx, position in enumerate(position_list):
-            name = f"Grid{grid_number:03d}_Pos{idx:03d}"
-            if len(position) == 3:
-                x, y, z = position
-            else:
-                x, y = position
-                z = None
+        self.currentTextChanged.connect(self._on_text_changed)
 
-            self._create_new_row(name, x, y, z)
+    def _on_sys_cfg_loaded(self) -> None:
+        if not self._channel_group:
+            self._channel_group = self._mmc.getChannelGroup()
+        self._update_channel_group_combo()
 
-    def _move_to_position(self) -> None:
-        if not self._mmc.getXYStageDevice():
+    def _update_channel_group_combo(self) -> None:
+        if len(self._mmc.getLoadedDevices()) <= 1:
             return
-        curr_row = self._table.currentRow()
-        self._mmc.setXYPosition(
-            self.value()[curr_row].get("x"), self.value()[curr_row].get("y")
-        )
-        if self._mmc.getFocusDevice() and self.value()[curr_row].get("z"):
-            self._mmc.setPosition(self.value()[curr_row].get("z"))
-
-    def value(self) -> list[PositionDict]:
-        """Return the current positions settings.
+        with signals_blocked(self):
+            self.clear()
+            groups = self._mmc.getAvailableConfigGroups()
+            self.addItems(groups)
+            self.adjustSize()
 
-        Note that output dict will match the Positions from useq schema:
-        <https://pymmcore-plus.github.io/useq-schema/schema/axes/#useq.Position>
-        """
-        values: list[PositionDict] = [
-            {
-                "name": self._table.item(row, 0).text() or None,
-                "x": self._get_table_value(row, 1),
-                "y": self._get_table_value(row, 2),
-                "z": self._get_table_value(row, 3),
-            }
-            for row in range(self._table.rowCount())
-        ]
-        return values
+        if not self._channel_group or self._channel_group not in groups:
+            self._channel_group = self.currentText()
+            return
 
-    def _get_table_value(self, row: int, col: int) -> float | None:
-        try:
-            wdg = cast(QDoubleSpinBox, self._table.cellWidget(row, col))
-            value = wdg.value()
-        except AttributeError:
-            value = None
-        return value  # type: ignore
-
-    # note: this should to be PositionDict, but it makes typing elsewhere harder
-    def set_state(self, positions: list[dict]) -> None:
-        """Set the state of the widget from a useq position dictionary."""
-        self._clear_positions()
-
-        if not self._mmc.getXYStageDevice() and not self._mmc.getFocusDevice():
-            raise ValueError("No XY and Z Stage devices loaded.")
-
-        self.setChecked(True)
-
-        for idx, pos in enumerate(positions):
-            name = pos.get("name") or f"Pos{idx:03d}"
-            x = pos.get("x")
-            y = pos.get("y")
-            z = pos.get("z")
-
-            if (x is not None or y is not None) and not self._mmc.getXYStageDevice():
-                x, y = (None, None)
-                warnings.warn("No XY Stage device loaded.")
-
-            if z and not self._mmc.getFocusDevice():
-                z = None
-                warnings.warn("No Focus device loaded.")
-
-            self._add_position_row()
-
-            self._add_table_item(name, idx, 0)
-            self._add_table_value(x, idx, 1)
-            self._add_table_value(y, idx, 2)
-            self._add_table_value(z, idx, 3)
+        self.setCurrentText(self._channel_group)
 
-        self.valueChanged.emit()
+    def _on_text_changed(self, group: str) -> None:
+        if group != self._channel_group:
+            self._channel_group = group
 
     def _disconnect(self) -> None:
-        self._mmc.events.systemConfigurationLoaded.disconnect(self._clear_positions)
+        self._mmc.events.systemConfigurationLoaded.disconnect(self._on_sys_cfg_loaded)
+        self._mmc.events.configGroupDeleted.disconnect(self._update_channel_group_combo)
+        self._mmc.events.configDefined.disconnect(self._update_channel_group_combo)
```

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets/_mda/_zstack_widget.py` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/_zstack_widget.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,17 +13,18 @@
     QLabel,
     QPushButton,
     QSizePolicy,
     QTabWidget,
     QVBoxLayout,
     QWidget,
 )
+from superqt.utils import signals_blocked
 
 if TYPE_CHECKING:
-    from typing_extensions import Protocol
+    from typing import Protocol
 
     # fmt: off
     class ZPicker(Protocol):
         valueChanged: Signal
         def value(self) -> dict:...
         def z_range(self) -> float: ...
     # fmt: on
@@ -52,27 +53,30 @@
         self._bottom_btn = QPushButton(text="Set Bottom")
         self._bottom_btn.clicked.connect(self._set_bottom)
 
         # current top position spinbox
         self._top_spinbox = QDoubleSpinBox()
         self._top_spinbox.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self._top_spinbox.setRange(self._MIN_Z, self._MAX_Z)
+        self._top_spinbox.setKeyboardTracking(False)
         self._top_spinbox.valueChanged.connect(self._update_zrange_and_emit)
 
         # current bottom position spinbox
         self._bottom_spinbox = QDoubleSpinBox()
         self._bottom_spinbox.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self._bottom_spinbox.setRange(self._MIN_Z, self._MAX_Z)
+        self._bottom_spinbox.setKeyboardTracking(False)
         self._bottom_spinbox.valueChanged.connect(self._update_zrange_and_emit)
 
         # read only z range spinbox
         self._zrange_spinbox = QDoubleSpinBox()
         self._zrange_spinbox.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self._zrange_spinbox.setMaximum(self._MAX_Z - self._MIN_Z)
         self._zrange_spinbox.setButtonSymbols(QAbstractSpinBox.ButtonSymbols.NoButtons)
+        self._zrange_spinbox.setKeyboardTracking(False)
         self._zrange_spinbox.setReadOnly(True)
 
         grid = QGridLayout()
         grid.setContentsMargins(10, 10, 10, 10)
         grid.addWidget(self._top_btn, 0, 0)
         grid.addWidget(self._top_spinbox, 1, 0)
         grid.addWidget(self._bottom_btn, 0, 1)
@@ -198,37 +202,45 @@
             "below": self._below_spinbox.value(),
         }
 
     def z_range(self) -> float:
         return self._above_spinbox.value() + self._below_spinbox.value()  # type: ignore
 
 
-class ZStackWidget(QGroupBox):
+class ZStackWidget(QWidget):
     """Widget providing options for setting up a z-stack range and step size.
 
     Each tab represents a different way of specifying a z-stack range. The `value()`
     method returns a dictionary with the current state of the widget, in a format that
     matches one of the [useq-schema Z Plan
     specifications](https://pymmcore-plus.github.io/useq-schema/schema/axes/#z-plans).
+
+    Parameters
+    ----------
+    parent : QWidget | None
+        Optional parent widget, by default None.
+    mmcore : CMMCorePlus | None
+        Optional [`pymmcore_plus.CMMCorePlus`][] micromanager core.
+        By default, None. If not specified, the widget will use the active
+        (or create a new)
+        [`CMMCorePlus.instance`][pymmcore_plus.core._mmcore_plus.CMMCorePlus.instance].
     """
 
     valueChanged = Signal(dict)
 
     _MAX_STEP = 100000
     _NIMG_PREFIX = "Number of Images:"
 
     def __init__(
         self,
-        title: str = "Z Stack",
         parent: QWidget | None = None,
         *,
         mmcore: CMMCorePlus | None = None,
     ) -> None:
-        super().__init__(title, parent=parent)
-        self.setCheckable(True)
+        super().__init__(parent=parent)
         self.setSizePolicy(QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Fixed)
 
         self._mmc = mmcore or CMMCorePlus.instance()
 
         # tabs for each z selection mode
         self._zmode_tabs = QTabWidget()
         self._zmode_tabs.setLayout(QVBoxLayout())
@@ -246,27 +258,28 @@
         # spinbox for the step size
         self._zstep_spinbox = QDoubleSpinBox()
         self._zstep_spinbox.setValue(1)
         self._zstep_spinbox.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self._zstep_spinbox.setMinimum(0.05)
         self._zstep_spinbox.setMaximum(self._MAX_STEP)
         self._zstep_spinbox.setSingleStep(0.1)
+        self._zstep_spinbox.setKeyboardTracking(False)
         self._zstep_spinbox.valueChanged.connect(self._update_and_emit)
 
         # readout for the number of images
         self.n_images_label = QLabel(self._NIMG_PREFIX)
 
         # bottom row with step size and number of images
         bottom_layout = QHBoxLayout()
-        bottom_layout.setContentsMargins(10, 0, 10, 0)
+        bottom_layout.setContentsMargins(5, 5, 5, 5)
         bottom_layout.addWidget(QLabel("Step Size (µm):"))
         bottom_layout.addWidget(self._zstep_spinbox)
         bottom_layout.addStretch()
         bottom_layout.addWidget(self.n_images_label)
-        bottom_row = QWidget()
+        bottom_row = QGroupBox()
         bottom_row.setLayout(bottom_layout)
 
         # layout
         self.setLayout(QVBoxLayout())
         self.layout().setSpacing(10)
         self.layout().setContentsMargins(10, 10, 10, 10)
         self.layout().addWidget(self._zmode_tabs)
@@ -279,46 +292,52 @@
 
     def _update_and_emit(self) -> None:
         """Update the number of images readout and emit the valueChanged signal."""
         self.n_images_label.setText(f"{self._NIMG_PREFIX} {self.n_images()}")
         self.valueChanged.emit(self.value())
 
     def value(self) -> dict:
-        """Return the current z-stack settings.
+        """Return the current z-stack settings as a dictionary.
 
-        Note that output dict will match one of the Z plans from useq schema:
-        <https://pymmcore-plus.github.io/useq-schema/schema/axes/#z-plans>
+        Note that the output will match one of the [useq-schema Z Plan
+        specifications](https://pymmcore-plus.github.io/useq-schema/schema/axes/#z-plans).
         """
         value = cast("ZPicker", self._zmode_tabs.currentWidget()).value()
         value["step"] = self._zstep_spinbox.value()
         return value
 
     def n_images(self) -> int:
         """Return the current number of images in the z-stack."""
         step = self._zstep_spinbox.value()
         _range = cast("ZPicker", self._zmode_tabs.currentWidget()).z_range()
-        return round((_range / step) + 1)
+        return int(round((_range / step) + 1))
 
     def set_state(self, z_plan: dict) -> None:
-        """Set the state of the widget from a dictionary."""
-        tabs = self._zmode_tabs
-        wdg: "ZPicker"
-        if "top" in z_plan and "bottom" in z_plan:
-            wdg = cast(ZTopBottomSelect, tabs.findChild(ZTopBottomSelect))
-            wdg._top_spinbox.setValue(z_plan["top"])
-            wdg._bottom_spinbox.setValue(z_plan["bottom"])
-            tabs.setCurrentWidget(wdg)
-        elif "above" in z_plan and "below" in z_plan:
-            wdg = cast(ZAboveBelowSelect, tabs.findChild(ZAboveBelowSelect))
-            wdg._above_spinbox.setValue(z_plan["above"])
-            wdg._below_spinbox.setValue(z_plan["below"])
-            tabs.setCurrentWidget(wdg)
-        elif "range" in z_plan:
-            wdg = cast(ZRangeAroundSelect, tabs.findChild(ZRangeAroundSelect))
-            wdg._zrange_spinbox.setValue(z_plan["range"])
-            tabs.setCurrentWidget(wdg)
+        """Set the state of the widget.
 
-        disabled = set(z_plan).isdisjoint({"top", "bottom", "above", "below", "range"})
-        self.setChecked(not disabled)
+        Parameters
+        ----------
+        z_plan : dict
+            A dictionary following the [useq-schema Z Plan specifications](
+            https://pymmcore-plus.github.io/useq-schema/schema/axes/#z-plans).
+        """
+        tabs = self._zmode_tabs
+        wdg: ZPicker
+        with signals_blocked(self):
+            if "top" in z_plan and "bottom" in z_plan:
+                wdg = cast(ZTopBottomSelect, tabs.findChild(ZTopBottomSelect))
+                wdg._top_spinbox.setValue(z_plan["top"])
+                wdg._bottom_spinbox.setValue(z_plan["bottom"])
+                tabs.setCurrentWidget(wdg)
+            elif "above" in z_plan and "below" in z_plan:
+                wdg = cast(ZAboveBelowSelect, tabs.findChild(ZAboveBelowSelect))
+                wdg._above_spinbox.setValue(z_plan["above"])
+                wdg._below_spinbox.setValue(z_plan["below"])
+                tabs.setCurrentWidget(wdg)
+            elif "range" in z_plan:
+                wdg = cast(ZRangeAroundSelect, tabs.findChild(ZRangeAroundSelect))
+                wdg._zrange_spinbox.setValue(z_plan["range"])
+                tabs.setCurrentWidget(wdg)
 
-        if "step" in z_plan:
-            self._zstep_spinbox.setValue(z_plan["step"])
+            if "step" in z_plan:
+                self._zstep_spinbox.setValue(z_plan["step"])
+        self.valueChanged.emit(self.value())
```

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets/_objective_widget.py` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_objective_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         By default, None. If not specified, the widget will use the active
         (or create a new)
         [`CMMCorePlus.instance`][pymmcore_plus.core._mmcore_plus.CMMCorePlus.instance].
     """
 
     def __init__(
         self,
-        objective_device: str = None,  # type: ignore
+        objective_device: str | None = None,
         *,
         parent: QWidget | None = None,
         mmcore: CMMCorePlus | None = None,
     ):
         super().__init__(parent=parent)
         self._mmc = mmcore or CMMCorePlus.instance()
         self._objective_device = objective_device or guess_objective_or_prompt(
```

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets/_pixel_size_widget.py` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_pixel_size_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import contextlib
 import itertools
 import re
 import warnings
-from typing import Any, cast
+from typing import Any, ClassVar, cast
 
 from pymmcore_plus import CMMCorePlus
 from qtpy.QtCore import Qt
 from qtpy.QtGui import QDoubleValidator
 from qtpy.QtWidgets import (
     QAbstractItemView,
     QDialog,
@@ -35,15 +35,15 @@
 MAGNIFICATION = 3
 IMAGE_PX_SIZE = 4
 
 
 class PixelSizeTable(QTableWidget):
     """Create a QTableWidget to set pixel size configurations."""
 
-    HEADERS = {
+    HEADERS: ClassVar[dict] = {
         "objective": "Objective",
         "resolutionID": "Resolution ID",
         "cameraPixelSize": "Camera Pixel Size (um)",
         "magnification": "Magnification",
         "imagePixelSize": "Image Pixel Size (um)",
         "delete": "Delete",
     }
@@ -57,29 +57,29 @@
         vh = self.verticalHeader()
         vh.setVisible(False)
         vh.setSectionResizeMode(hh.ResizeMode.Stretch)
         self.setSelectionBehavior(QAbstractItemView.SelectionBehavior.SelectItems)
         self.setDragDropMode(QAbstractItemView.DragDropMode.NoDragDrop)
 
     def _rebuild(
-        self, obj_dev: str, _cam_mag_dict: dict[str, tuple[float, float]] = None  # type: ignore # noqa:E501
+        self, obj_dev: str, _cam_mag_dict: dict[str, tuple[float, float]] | None = None
     ) -> None:
         records = self._get_pixel_info(obj_dev, _cam_mag_dict)
         self.clear()
         self.setRowCount(len(records))
         self.setColumnCount(len(self.HEADERS))
         self.setHorizontalHeaderLabels(list(self.HEADERS.values()))
 
         for row, record in enumerate(records):
             self._populate_row(row, record)
 
         self._update_status()
 
     def _get_pixel_info(
-        self, obj_dev: str, _cam_mag_dict: dict[str, tuple[float, float]] = None  # type: ignore # noqa:E501
+        self, obj_dev: str, _cam_mag_dict: dict[str, tuple[float, float]] | None = None
     ) -> list[dict[str, Any]]:
         """Returns a list of records, that can be used to build a table.
 
         [
             {'objective': 'Something', 'resolutionID": 'something', ...},
             ...
         ]
@@ -312,15 +312,14 @@
                     item.setStyleSheet("color:magenta")
 
     def _on_sys_cfg_loaded(self) -> None:
         self.objective_device = guess_objective_or_prompt(parent=self)
         self._rebuild()
 
     def _on_px_set(self, value: float) -> None:
-
         rows = []
         for cfg in self._mmc.getAvailablePixelSizeConfigs():
             if value == self._mmc.getPixelSizeUmByID(cfg):
                 for r in range(self.table.rowCount()):
                     resID = self.table.cellWidget(r, RESOLUTION_ID).text()
                     if resID == cfg:
                         rows.append(r)
@@ -434,23 +433,23 @@
         sender = self.sender()
         row = self.table.indexAt(sender.pos()).row()
         wdg = cast(QLineEdit, self.table.cellWidget(row, RESOLUTION_ID))
         wdg.focusNextChild()
         value = wdg.text()
 
         if value in self._mmc.getAvailablePixelSizeConfigs():
-
             if wdg.property("resID") == value:
                 return
 
             wdg.setText("None")
 
             warnings.warn(
                 f"There is already a configuration called '{value}'. "
-                "Choose a different resolutionID."
+                "Choose a different resolutionID.",
+                stacklevel=2,
             )
             with contextlib.suppress(ValueError):
                 self._mmc.deletePixelSizeConfig(wdg.property("resID"))
 
             self.table._update_status()
 
             return
```

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets/_presets_widget.py` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_presets_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     def __init__(
         self,
         group: str,
         *,
         parent: QWidget | None = None,
         mmcore: CMMCorePlus | None = None,
     ) -> None:
-
         super().__init__(parent=parent)
 
         self._mmc = mmcore or CMMCorePlus.instance()
 
         self._group = group
 
         if self._group not in self._mmc.getAvailableConfigGroups():
@@ -98,17 +97,19 @@
         self._combo.setStyleSheet("")
 
     def _on_combo_changed(self, text: str) -> None:
         self._mmc.setConfig(self._group, text)
         self._combo.setStyleSheet("")
 
     def _set_style_if_props_not_match_preset(self) -> None:
+        if not self._mmc.getAvailableConfigs(self._group):
+            return
         for preset in self._presets:
             _set_combo = True
-            for (dev, prop, value) in self._mmc.getConfigData(self._group, preset):
+            for dev, prop, value in self._mmc.getConfigData(self._group, preset):
                 cache_value = self._mmc.getPropertyFromCache(dev, prop)
                 if cache_value != value:
                     _set_combo = False
                     break
             if _set_combo:
                 with signals_blocked(self._combo):
                     self._combo.setCurrentText(preset)
@@ -130,15 +131,14 @@
             if len(dev_prop) != len(self.dev_prop):
                 idx = self._presets.index(preset)
                 self._combo.setItemData(
                     idx, QBrush(Qt.GlobalColor.magenta), Qt.ItemDataRole.ForegroundRole
                 )
 
     def _on_cfg_set(self, group: str, preset: str) -> None:
-
         if group == self._group and self._combo.currentText() != preset:
             with signals_blocked(self._combo):
                 self._combo.setCurrentText(preset)
                 self._combo.setStyleSheet("")
         else:
             dev_prop_list = self._get_preset_dev_prop(self._group, self._presets[0])
             if any(dev_prop for dev_prop in dev_prop_list if dev_prop in self.dev_prop):
@@ -226,15 +226,14 @@
                     _to_delete.append(dp)
                     break
         return _to_delete
 
     def _on_new_group_preset(
         self, group: str, preset: str, device: str, property: str, value: str
     ) -> None:
-
         if group != self._group:
             return
 
         if not device or not property or not value:
             self._refresh()
             return
 
@@ -250,15 +249,16 @@
             ]
 
             _to_delete = self._find_dev_prop_to_remove(preset)
 
             if _to_delete:
                 warnings.warn(
                     f"{_to_delete} are not included in the '{self._group}' "
-                    "group and will not be added!"
+                    "group and will not be added!",
+                    stacklevel=2,
                 )
 
                 dev_prop_val = [
                     (k[0], k[1], k[2]) for k in self._mmc.getConfigData(group, preset)
                 ]
 
                 with block_core(self._mmc.events):
@@ -275,15 +275,16 @@
 
         preset_dev_props = self._get_preset_dev_prop(self._group, preset)
 
         if len(preset_dev_props) != len(set(self.dev_prop)) and self.dev_prop:
             missing_props = set(self.dev_prop) - set(preset_dev_props)
             warnings.warn(
                 f"'{preset}' preset is missing the following properties: "
-                f"{list(missing_props)}."
+                f"{list(missing_props)}.",
+                stacklevel=2,
             )
 
         self._refresh()
 
     def _disconnect(self) -> None:
         self._mmc.events.configSet.disconnect(self._on_cfg_set)
         self._mmc.events.systemConfigurationLoaded.disconnect(self._refresh)
```

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets/_properties_widget.py` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_properties_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets/_property_browser.py` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_property_browser.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets/_property_widget.py` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_property_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,15 +284,14 @@
         self,
         device_label: str,
         prop_name: str,
         *,
         parent: QWidget | None = None,
         mmcore: CMMCorePlus | None = None,
     ) -> None:
-
         super().__init__(parent=parent)
 
         self._mmc = mmcore or CMMCorePlus.instance()
 
         if device_label not in self._mmc.getLoadedDevices():
             raise ValueError(f"Device not loaded: {device_label!r}")
```

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets/_shutter_widget.py` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_shutter_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,22 +67,22 @@
 
         self._create_wdg()
 
         self._refresh_shutter_widget()
 
         self._mmc.events.systemConfigurationLoaded.connect(self._refresh_shutter_widget)
         self._mmc.events.autoShutterSet.connect(self._on_autoshutter_changed)
-        self._mmc.events.propertyChanged.connect(self._on_prop_changed)
+        self._mmc.events.propertyChanged.connect(self._on_shutter_device_changed)
+        self._mmc.events.propertyChanged.connect(self._on_shutter_state_changed)
+        self._mmc.events.configSet.connect(self._on_channel_set)
         self._mmc.events.continuousSequenceAcquisitionStarted.connect(
-            self._on_seq_started
+            self._on_live_mode
         )
-        self._mmc.events.sequenceAcquisitionStarted.connect(self._on_seq_started)
-        self._mmc.events.sequenceAcquisitionStopped.connect(self._on_seq_stopped)
-        self._mmc.events.imageSnapped.connect(self._on_seq_stopped)
-        self._mmc.events.configSet.connect(self._on_channel_set)
+        self._mmc.events.sequenceAcquisitionStarted.connect(self._on_live_mode)
+        self._mmc.events.sequenceAcquisitionStopped.connect(self._on_live_mode)
 
         self.destroyed.connect(self._disconnect)
 
     @property
     def icon_open(self) -> str:
         """
         Set the icon of the QPushButton when the shutter is open.
@@ -197,15 +197,14 @@
     @button_text_closed.setter
     def button_text_closed(self, text: str) -> None:
         if not self._mmc.getShutterOpen(self.shutter_device):
             self.shutter_button.setText(text)
         self._button_text_closed = text
 
     def _create_wdg(self) -> None:
-
         main_layout = QHBoxLayout()
         main_layout.setContentsMargins(0, 0, 0, 0)
         main_layout.setSpacing(3)
 
         self.shutter_button = QPushButton(text=self._button_text_closed)
         sizepolicy_btn = QSizePolicy(QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Fixed)
         self.shutter_button.setSizePolicy(sizepolicy_btn)
@@ -234,66 +233,83 @@
         self._refresh_shutter_widget()
 
     def _refresh_shutter_widget(self) -> None:
         if self.shutter_device not in self._mmc.getLoadedDevicesOfType(
             DeviceType.ShutterDevice
         ):
             if self.shutter_device != "":
-                warnings.warn(f"No device with label {self.shutter_device}!")
+                warnings.warn(
+                    f"No device with label {self.shutter_device}!", stacklevel=2
+                )
             self.shutter_button.setText("None")
             self.shutter_button.setEnabled(False)
             if self.autoshutter:
                 self.autoshutter_checkbox.setEnabled(False)
         else:
-            self._close_shutter(self.shutter_device)
             if self.autoshutter:
                 self.autoshutter_checkbox.setEnabled(True)
-                self.autoshutter_checkbox.setChecked(True)
-                self.shutter_button.setEnabled(False)
+                self.autoshutter_checkbox.setChecked(self._mmc.getAutoShutter())
             else:
+                self.autoshutter_checkbox.setChecked(False)
+            if self._mmc.getShutterDevice() == self.shutter_device:
                 self.shutter_button.setEnabled(not self._mmc.getAutoShutter())
+            else:
+                self.shutter_button.setEnabled(True)
+            if self._mmc.getShutterOpen(self.shutter_device):
+                self._set_shutter_wdg_to_opened()
+            else:
+                self._set_shutter_wdg_to_closed()
 
             # bool to define if the shutter_device is a Micro-Manager 'Multi Shutter'
             props = self._mmc.getDevicePropertyNames(self.shutter_device)
             self._is_multiShutter = bool([x for x in props if "Physical Shutter" in x])
 
-    def _on_seq_started(self) -> None:
-        if self._mmc.getShutterOpen(self.shutter_device):
-            self._set_shutter_wdg_to_opened()
-
-    def _on_seq_stopped(self) -> None:
-        self._close_shutter(self.shutter_device)
-
-    def _on_prop_changed(self, dev_name: str, prop_name: str, value: Any) -> None:
+    def _on_shutter_state_changed(
+        self, dev_name: str, prop_name: str, value: Any
+    ) -> None:
         if dev_name != self.shutter_device or prop_name != "State":
             return
         state = value in [True, "1"]
         (
             self._set_shutter_wdg_to_opened()
             if state
             else self._set_shutter_wdg_to_closed()
         )
-        if self._is_multiShutter and state:
+        if self._is_multiShutter:
             for i in range(1, 6):
                 value = self._mmc.getProperty(
                     self.shutter_device, f"Physical Shutter {i}"
                 )
                 if value != "Undefined":
-                    self._mmc.events.propertyChanged.emit(value, "State", True)
+                    self._mmc.events.propertyChanged.emit(value, "State", state)
+
+    def _on_shutter_device_changed(
+        self, dev_name: str, prop_name: str, value: Any
+    ) -> None:
+        if dev_name != "Core" and prop_name != "Shutter":
+            return
+
+        if value != self.shutter_device:
+            self.shutter_button.setEnabled(True)
+        else:
+            self.shutter_button.setEnabled(not self._mmc.getAutoShutter())
+
+    def _on_live_mode(self) -> None:
+        if not self._mmc.getShutterOpen(self.shutter_device):
+            self._set_shutter_wdg_to_closed()
+        else:
+            self._set_shutter_wdg_to_opened()
 
     def _on_channel_set(self, group: str, preset: str) -> None:
-        ch = self._mmc.getChannelGroup()
-        if group != ch:
-            return  # pragma: no cover
-        for d in self._mmc.getConfigData(ch, preset):
-            _dev = d[0]
-            _type = self._mmc.getDeviceType(_dev)
-            if _type is DeviceType.Shutter:
-                self._mmc.setProperty("Core", "Shutter", _dev)
-                break
+        if (
+            self._mmc.getShutterDevice() == self.shutter_device
+        ) and self._mmc.getAutoShutter():
+            self.shutter_button.setEnabled(False)
+        else:
+            self.shutter_button.setEnabled(True)
 
     def _on_shutter_btn_clicked(self) -> None:
         if self._mmc.getShutterOpen(self.shutter_device):
             self._close_shutter(self.shutter_device)
         else:
             self._open_shutter(self.shutter_device)
 
@@ -306,18 +322,16 @@
                 else:
                     self._mmc.events.propertyChanged.emit(shutter, "State", False)
 
     def _on_autoshutter_changed(self, state: bool) -> None:
         if self.autoshutter:
             with signals_blocked(self.autoshutter_checkbox):
                 self.autoshutter_checkbox.setChecked(state)
-        self.shutter_button.setEnabled(not state)
-
-        if state and self._mmc.isSequenceRunning():
-            self._mmc.stopSequenceAcquisition()
+        if self._mmc.getShutterDevice() == self.shutter_device:
+            self.shutter_button.setEnabled(not state)
 
     def _close_shutter(self, shutter: str) -> None:
         self._set_shutter_wdg_to_closed()
         self._mmc.setShutterOpen(shutter, False)
 
     def _open_shutter(self, shutter: str) -> None:
         self._set_shutter_wdg_to_opened()
@@ -337,15 +351,10 @@
         )
 
     def _disconnect(self) -> None:
         self._mmc.events.systemConfigurationLoaded.disconnect(
             self._refresh_shutter_widget
         )
         self._mmc.events.autoShutterSet.disconnect(self._on_autoshutter_changed)
-        self._mmc.events.propertyChanged.disconnect(self._on_prop_changed)
-        self._mmc.events.continuousSequenceAcquisitionStarted.disconnect(
-            self._on_seq_started
-        )
-        self._mmc.events.sequenceAcquisitionStarted.disconnect(self._on_seq_started)
-        self._mmc.events.sequenceAcquisitionStopped.disconnect(self._on_seq_stopped)
-        self._mmc.events.imageSnapped.disconnect(self._on_seq_stopped)
+        self._mmc.events.propertyChanged.disconnect(self._on_shutter_device_changed)
+        self._mmc.events.propertyChanged.disconnect(self._on_shutter_state_changed)
         self._mmc.events.configSet.disconnect(self._on_channel_set)
```

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets/_snap_button_widget.py` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_snap_button_widget.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 
     def __init__(
         self,
         *,
         parent: QWidget | None = None,
         mmcore: CMMCorePlus | None = None,
     ) -> None:
-
         super().__init__(parent=parent)
 
         self.setSizePolicy(
             QSizePolicy(QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Fixed)
         )
 
         self._mmc = mmcore or CMMCorePlus.instance()
@@ -75,19 +74,34 @@
         self.setIcon(icon(MDI6.camera_outline, color=(0, 255, 0)))
         self.setIconSize(QSize(30, 30))
         self.clicked.connect(self._snap)
 
     def _snap(self) -> None:
         if self._mmc.isSequenceRunning():
             self._mmc.stopSequenceAcquisition()
-        if self._mmc.getAutoShutter():
-            self._mmc.events.propertyChanged.emit(
-                self._mmc.getShutterDevice(), "State", True
-            )
-        create_worker(self._mmc.snap, _start_thread=True)
+
+        def snap_with_shutter() -> None:
+            """
+            Perform a snap and ensure shutter signals are sent.
+
+            This is necessary as not all shutter devices properly
+            send signals as they are opened and closed.
+            """
+            autoshutter = self._mmc.getAutoShutter()
+            if autoshutter:
+                self._mmc.events.propertyChanged.emit(
+                    self._mmc.getShutterDevice(), "State", True
+                )
+            self._mmc.snap()
+            if autoshutter:
+                self._mmc.events.propertyChanged.emit(
+                    self._mmc.getShutterDevice(), "State", False
+                )
+
+        create_worker(snap_with_shutter, _start_thread=True)
 
     def _on_system_cfg_loaded(self) -> None:
         self.setEnabled(bool(self._mmc.getCameraDevice()))
 
     def _disconnect(self) -> None:
         self._mmc.events.systemConfigurationLoaded.disconnect(
             self._on_system_cfg_loaded
```

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets/_util.py` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_util.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from __future__ import annotations
 
+from datetime import timedelta
 from typing import ContextManager, Sequence
 
 from pymmcore_plus import CMMCorePlus
 from pymmcore_plus.core.events import CMMCoreSignaler, PCoreSignaler
 from qtpy.QtWidgets import (
     QComboBox,
     QDialog,
     QDialogButtonBox,
     QLabel,
     QVBoxLayout,
     QWidget,
 )
 from superqt.utils import signals_blocked
+from useq import AnyGridPlan, MDASequence
 
 
 class ComboMessageBox(QDialog):
     """Dialog that presents a combo box of `items`."""
 
     def __init__(
         self,
@@ -97,7 +99,40 @@
 
 def block_core(mmcore_events: CMMCoreSignaler | PCoreSignaler) -> ContextManager:
     """Block core signals."""
     if isinstance(mmcore_events, CMMCoreSignaler):
         return mmcore_events.blocked()  # type: ignore
     elif isinstance(mmcore_events, PCoreSignaler):
         return signals_blocked(mmcore_events)  # type: ignore
+
+
+def fmt_timedelta(time: timedelta) -> str:
+    """Take timedelta and return formatted string.
+
+    Examples
+    --------
+    >>> fmt_timedelta(timedelta(seconds=100))
+    '01 min  40 sec'
+    >>> fmt_timedelta(timedelta(minutes=320, seconds=2500))
+    '06 hours  01 min  40 sec'
+    """
+    d = "day" if time.days == 1 else "days"
+    _time = str(time).replace(f" {d}, ", ":") if time.days >= 1 else f"0:{time!s}"
+    out: list = []
+    keys = ["days", "hours", "min", "sec", "ms"]
+    for i, t in enumerate(_time.split(":")):
+        if i == 3:
+            s = t.split(".")
+            if len(s) == 2:
+                sec = f"{int(s[0]):02d} sec " if int(s[0]) > 0 else ""
+                ms = f"{int(s[1][:3]):03d} ms" if int(s[1][:3]) > 0 else ""
+                out.append(f"{sec}{ms}")
+            else:
+                out.append(f"{int(s[0]):02d} sec") if int(s[0]) > 0 else ""
+        else:
+            out.append(f"{int(float(t)):02d} {keys[i]}") if int(float(t)) > 0 else ""
+    return "  ".join(out)
+
+
+def get_grid_type(grid: dict) -> AnyGridPlan | None:
+    """Get the grid type from the grid_plan."""
+    return MDASequence(grid_plan=grid).grid_plan
```

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets.egg-info/PKG-INFO` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymmcore-widgets
-Version: 0.3.0
+Version: 0.4.0
 Summary: A set of Qt-based widgets onto the pymmcore-plus model
 Author-email: Federico Gasparoli <federico.gasparoli@gmail.com>, Talley Lambert <talley.lambert@gmail.com>, Ian Hunt-Isaak <ianhuntisaak@gmail.com>
 License: BSD 3-Clause License
 Project-URL: homepage, https://github.com/pymmcore-plus/pymmcore-widgets
 Project-URL: repository, https://github.com/pymmcore-plus/pymmcore-widgets
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pymmcore-widgets-0.3.0/src/pymmcore_widgets.egg-info/SOURCES.txt` & `pymmcore-widgets-0.4.0/src/pymmcore_widgets.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -16,39 +16,42 @@
 .github/workflows/docs.yml
 docs/_gen_widget_pages.py
 docs/_hooks.py
 docs/index.md
 docs/images/favicon.ico
 docs/stylesheets/extra.css
 examples/camera_roi_widget.py
+examples/channel_group_widget.py
+examples/channel_table.py
 examples/channel_widget.py
 examples/configuration_widget.py
 examples/default_camera_exposure_widget.py
 examples/device_widget.py
 examples/exposure_widget.py
+examples/grid_widget.py
 examples/group_preset_table_widget.py
 examples/image_preview.py
 examples/live_button.py
 examples/mda_widget.py
 examples/objectives_widget.py
 examples/pixel_size_widget.py
 examples/position_table.py
 examples/presets_widget.py
 examples/properties_widget.py
 examples/property_browser.py
 examples/property_widget.py
-examples/sample_explorer_widget.py
 examples/shutters_widget.py
 examples/snap_button.py
 examples/stage_widget.py
 examples/state_device_widget.py
 examples/time_plan_widget.py
 examples/z_stack_widget.py
 src/pymmcore_widgets/__init__.py
 src/pymmcore_widgets/_camera_roi_widget.py
+src/pymmcore_widgets/_channel_group_widget.py
 src/pymmcore_widgets/_channel_widget.py
 src/pymmcore_widgets/_core.py
 src/pymmcore_widgets/_device_property_table.py
 src/pymmcore_widgets/_device_type_filter.py
 src/pymmcore_widgets/_device_widget.py
 src/pymmcore_widgets/_exposure_widget.py
 src/pymmcore_widgets/_image_widget.py
@@ -75,38 +78,43 @@
 src/pymmcore_widgets/_group_preset_widget/_add_first_preset_widget.py
 src/pymmcore_widgets/_group_preset_widget/_add_group_widget.py
 src/pymmcore_widgets/_group_preset_widget/_add_preset_widget.py
 src/pymmcore_widgets/_group_preset_widget/_edit_group_widget.py
 src/pymmcore_widgets/_group_preset_widget/_edit_preset_widget.py
 src/pymmcore_widgets/_group_preset_widget/_group_preset_table_widget.py
 src/pymmcore_widgets/_mda/__init__.py
+src/pymmcore_widgets/_mda/_autofocus_device_widget.py
 src/pymmcore_widgets/_mda/_channel_table_widget.py
+src/pymmcore_widgets/_mda/_checkable_tabwidget_widget.py
 src/pymmcore_widgets/_mda/_general_mda_widgets.py
 src/pymmcore_widgets/_mda/_grid_widget.py
 src/pymmcore_widgets/_mda/_mda_widget.py
 src/pymmcore_widgets/_mda/_positions_table_widget.py
-src/pymmcore_widgets/_mda/_sample_explorer_widget.py
 src/pymmcore_widgets/_mda/_time_plan_widget.py
 src/pymmcore_widgets/_mda/_zstack_widget.py
 tests/conftest.py
 tests/test_camera_roi_widget.py
+tests/test_channel_group_widget.py
+tests/test_channel_table_widget.py
 tests/test_channel_widget.py
 tests/test_combo_message_box_widget.py
 tests/test_config.cfg
+tests/test_core_state.py
 tests/test_device_widget.py
 tests/test_exposure_widget.py
+tests/test_grid_widget.py
 tests/test_group_preset_widget.py
 tests/test_image_preview.py
 tests/test_live_button.py
 tests/test_load_system_cfg_widget.py
 tests/test_mda_widget.py
 tests/test_objective_widget.py
 tests/test_position_table_widget.py
 tests/test_presets_widget.py
 tests/test_prop_widget.py
 tests/test_properties_widget.py
 tests/test_property_browser.py
-tests/test_sample_explorer_widget.py
 tests/test_shutter_widget.py
 tests/test_snap_button_widget.py
 tests/test_stage_widget.py
-tests/test_table_pixel_size_widget.py
+tests/test_table_pixel_size_widget.py
+tests/test_time_table.py
```

### Comparing `pymmcore-widgets-0.3.0/tests/conftest.py` & `pymmcore-widgets-0.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/tests/test_camera_roi_widget.py` & `pymmcore-widgets-0.4.0/tests/test_camera_roi_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/tests/test_channel_widget.py` & `pymmcore-widgets-0.4.0/tests/test_channel_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,28 +10,24 @@
 from pymmcore_widgets._util import block_core
 
 if TYPE_CHECKING:
     from pytestqt.qtbot import QtBot
 
 
 def test_channel_widget(qtbot: QtBot, global_mmcore: CMMCorePlus):
-
     wdg = ChannelWidget()
     qtbot.addWidget(wdg)
 
     assert global_mmcore.getChannelGroup() == "Channel"
 
     assert isinstance(wdg.channel_wdg, PresetsWidget)
 
-    global_mmcore.setProperty("Core", "Shutter", "")
-    assert not global_mmcore.getShutterDevice()
-
     wdg.channel_wdg.setValue("DAPI")
     assert global_mmcore.getCurrentConfig("Channel") == "DAPI"
-    assert global_mmcore.getShutterDevice() == "Multi Shutter"
+    assert global_mmcore.getShutterDevice() == "Shutter"
 
     global_mmcore.setConfig("Channel", "FITC")
     assert wdg.channel_wdg.value() == "FITC"
 
     global_mmcore.setProperty("Emission", "Label", "Chroma-HQ700")
     assert wdg.channel_wdg._combo.styleSheet() == "color: magenta;"
 
@@ -53,15 +49,14 @@
     with qtbot.waitSignal(global_mmcore.events.configGroupDeleted):
         global_mmcore.deleteConfigGroup("Channel")
     assert isinstance(wdg.channel_wdg, QComboBox)
     assert wdg.channel_wdg.count() == 0
     assert global_mmcore.getChannelGroup() == ""
 
     with qtbot.waitSignal(global_mmcore.events.configDefined):
-
         dev_prop_val = [
             ("Dichroic", "Label", "400DCLP"),
             ("Emission", "Label", "Chroma-HQ700"),
             ("Excitation", "Label", "Chroma-HQ570"),
         ]
 
         with block_core(global_mmcore.events):
```

### Comparing `pymmcore-widgets-0.3.0/tests/test_combo_message_box_widget.py` & `pymmcore-widgets-0.4.0/tests/test_combo_message_box_widget.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from pymmcore_widgets._util import ComboMessageBox
 
 if TYPE_CHECKING:
     from pytestqt.qtbot import QtBot
 
 
 def test_combo_message_box_widget(qtbot: QtBot):
-
     items = ["item_1", "item_2", "item_3"]
 
     wdg = ComboMessageBox(items)
     qtbot.add_widget(wdg)
 
     assert wdg._combo.count() == 3
```

### Comparing `pymmcore-widgets-0.3.0/tests/test_config.cfg` & `pymmcore-widgets-0.4.0/tests/test_config.cfg`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/tests/test_device_widget.py` & `pymmcore-widgets-0.4.0/tests/test_device_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/tests/test_exposure_widget.py` & `pymmcore-widgets-0.4.0/tests/test_exposure_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/tests/test_group_preset_widget.py` & `pymmcore-widgets-0.4.0/tests/test_group_preset_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 def test_populating_group_preset_table(global_mmcore: CMMCorePlus, qtbot: QtBot):
     gp = GroupPresetTableWidget()
     qtbot.addWidget(gp)
 
     assert len(list(global_mmcore.getAvailableConfigGroups())) == 9
 
     for r in range(gp.table_wdg.rowCount()):
-
         group_name = gp.table_wdg.item(r, 0).text()
         wdg = gp.table_wdg.cellWidget(r, 1)
 
         if group_name == "Channel":
             assert set(wdg.allowedValues()) == {"DAPI", "FITC", "Cy5", "Rhodamine"}
             wdg.setValue("FITC")
             assert global_mmcore.getCurrentConfig(group_name) == "FITC"
@@ -173,28 +172,28 @@
     gp = GroupPresetTableWidget()
     qtbot.addWidget(gp)
     mmc = global_mmcore
 
     assert "Camera" in mmc.getAvailableConfigGroups()
 
     for r in range(gp.table_wdg.rowCount()):
-
         group_name = gp.table_wdg.item(r, 0).text()
 
         if group_name == "Camera":
-
             with qtbot.waitSignal(mmc.events.configGroupDeleted):
                 mmc.deleteConfigGroup("Camera")
             break
 
     assert "Camera" not in mmc.getAvailableConfigGroups()
     groups_in_table = [
         gp.table_wdg.item(r, 0).text() for r in range(gp.table_wdg.rowCount())
     ]
+
     assert "Camera" not in groups_in_table
+    assert gp.table_wdg.rowCount() == 8
 
 
 def test_add_preset(global_mmcore: CMMCorePlus, qtbot: QtBot):
     add_prs = AddPresetWidget("Channel")
     qtbot.addWidget(add_prs)
     gp = GroupPresetTableWidget()
     qtbot.addWidget(gp)
@@ -234,15 +233,14 @@
         ("Multi Shutter", "Physical Shutter 3", "StateDev Shutter"),
         ("Multi Shutter", "Physical Shutter 4", "Undefined"),
         ("StateDev Shutter", "State Device", "StateDev"),
         ("StateDev", "Label", "State-1"),
     ]
 
     for r in range(gp.table_wdg.rowCount()):
-
         group_name = gp.table_wdg.item(r, 0).text()
         if group_name == "Channel":
             wdg = cast(PresetsWidget, gp.table_wdg.cellWidget(r, 1))
             assert wdg.allowedValues() == mmc.getAvailableConfigs("Channel")
             break
 
 
@@ -272,15 +270,14 @@
     mmc = global_mmcore
 
     assert "Camera" in mmc.getAvailableConfigGroups()
     assert ["HighRes", "LowRes", "MedRes"] == list(mmc.getAvailableConfigs("Camera"))
 
     camera_group_row = 0
     for r in range(gp.table_wdg.rowCount()):
-
         group_name = gp.table_wdg.item(r, 0).text()
         wdg = cast(PresetsWidget, gp.table_wdg.cellWidget(r, 1))
 
         if group_name == "Camera":
             camera_group_row = r
             assert wdg.allowedValues() == mmc.getAvailableConfigs("Camera")
             break
```

### Comparing `pymmcore-widgets-0.3.0/tests/test_image_preview.py` & `pymmcore-widgets-0.4.0/tests/test_image_preview.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/tests/test_live_button.py` & `pymmcore-widgets-0.4.0/tests/test_live_button.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 if TYPE_CHECKING:
     from pymmcore_plus import CMMCorePlus
     from pytestqt.qtbot import QtBot
 
 
 def test_live_button_widget(qtbot: QtBot, global_mmcore: CMMCorePlus):
-
     live_btn = LiveButton()
 
     qtbot.addWidget(live_btn)
 
     assert live_btn.text() == "Live"
     assert live_btn.iconSize() == QSize(30, 30)
     assert live_btn.icon_color_on == (0, 255, 0)
```

### Comparing `pymmcore-widgets-0.3.0/tests/test_load_system_cfg_widget.py` & `pymmcore-widgets-0.4.0/tests/test_load_system_cfg_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 if TYPE_CHECKING:
     from pymmcore_plus import CMMCorePlus
     from pytestqt.qtbot import QtBot
 
 
 def test_load_system_cfg_widget(qtbot: QtBot, global_mmcore: CMMCorePlus):
-
     cfg = ConfigurationWidget()
     qtbot.addWidget(cfg)
 
     global_mmcore.unloadAllDevices()
 
     assert len(global_mmcore.getLoadedDevices()) <= 1
```

### Comparing `pymmcore-widgets-0.3.0/tests/test_objective_widget.py` & `pymmcore-widgets-0.4.0/tests/test_objective_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/tests/test_presets_widget.py` & `pymmcore-widgets-0.4.0/tests/test_presets_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/tests/test_prop_widget.py` & `pymmcore-widgets-0.4.0/tests/test_prop_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/tests/test_properties_widget.py` & `pymmcore-widgets-0.4.0/tests/test_properties_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/tests/test_property_browser.py` & `pymmcore-widgets-0.4.0/tests/test_property_browser.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/tests/test_shutter_widget.py` & `pymmcore-widgets-0.4.0/tests/test_shutter_widget.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,61 +26,57 @@
         shutter._refresh_shutter_widget()
         _shutters.append(shutter)
         qtbot.addWidget(shutter)
     return tuple(_shutters)  # type: ignore
 
 
 def test_create_shutter_widgets(qtbot: QtBot):
-
     shutter, state_dev_shutter, multi_shutter = _make_shutters(qtbot)
 
-    assert shutter.shutter_button.text() == "Shutter closed"
+    assert shutter.shutter_button.text() == "Shutter opened"
     assert not shutter.shutter_button.isEnabled()
-    assert state_dev_shutter.shutter_button.text() == "StateDev Shutter closed"
-    assert not state_dev_shutter.shutter_button.isEnabled()
+    assert state_dev_shutter.shutter_button.text() == "StateDev Shutter opened"
+    assert state_dev_shutter.shutter_button.isEnabled()
     assert multi_shutter.shutter_button.text() == "Multi Shutter closed"
     assert multi_shutter.autoshutter_checkbox.isChecked()
-    assert not multi_shutter.shutter_button.isEnabled()
+    assert multi_shutter.shutter_button.isEnabled()
 
 
 def test_shutter_widget_propertyChanged(qtbot: QtBot):
-
     shutter, _, multi_shutter = _make_shutters(qtbot)
     mmc = CMMCorePlus.instance()
 
     with qtbot.waitSignal(mmc.events.propertyChanged):
-        mmc.setProperty("Shutter", "State", True)
+        mmc.setProperty("Shutter", "State", False)
     assert not shutter.shutter_button.isEnabled()
-    assert mmc.getShutterOpen("Shutter")
-    assert shutter.shutter_button.text() == "Shutter opened"
-    assert mmc.getProperty("Shutter", "State") == "1"
-    assert not multi_shutter.shutter_button.isEnabled()
+    assert not mmc.getShutterOpen("Shutter")
+    assert shutter.shutter_button.text() == "Shutter closed"
+    assert mmc.getProperty("Shutter", "State") == "0"
+    assert multi_shutter.shutter_button.isEnabled()
     assert not mmc.getShutterOpen("Multi Shutter")
     assert multi_shutter.shutter_button.text() == "Multi Shutter closed"
     assert mmc.getProperty("Multi Shutter", "State") == "0"
 
 
 def test_shutter_widget_autoShutterSet(qtbot: QtBot):
-
     shutter, state_dev_shutter, multi_shutter = _make_shutters(qtbot)
     mmc = CMMCorePlus.instance()
 
     with qtbot.waitSignal(mmc.events.autoShutterSet):
         mmc.setAutoShutter(False)
     assert shutter.shutter_button.isEnabled()
     assert state_dev_shutter.shutter_button.isEnabled()
     assert multi_shutter.shutter_button.isEnabled()
     mmc.setAutoShutter(True)
     assert not shutter.shutter_button.isEnabled()
-    assert not state_dev_shutter.shutter_button.isEnabled()
-    assert not multi_shutter.shutter_button.isEnabled()
+    assert state_dev_shutter.shutter_button.isEnabled()
+    assert multi_shutter.shutter_button.isEnabled()
 
 
 def test_shutter_widget_configSet(qtbot: QtBot):
-
     shutter, state_dev_shutter, multi_shutter = _make_shutters(qtbot)
     mmc = CMMCorePlus.instance()
 
     with qtbot.waitSignals(
         [
             mmc.events.configSet,
             mmc.events.propertyChanged,
@@ -96,93 +92,84 @@
     assert mmc.getShutterOpen("Shutter")
     assert state_dev_shutter.shutter_button.text() == "StateDev Shutter opened"
     assert mmc.getShutterOpen("StateDev Shutter")
     assert mmc.getProperty("StateDev", "Label") == "State-1"
 
 
 def test_shutter_widget_SequenceAcquisition(qtbot: QtBot):
-
     shutter, state_dev_shutter, multi_shutter = _make_shutters(qtbot)
     mmc = CMMCorePlus.instance()
 
     with qtbot.waitSignal(mmc.events.configSet):
         mmc.setConfig("Channel", "DAPI")
 
     with qtbot.waitSignal(mmc.events.continuousSequenceAcquisitionStarted):
         mmc.startContinuousSequenceAcquisition()
-        assert multi_shutter.shutter_button.text() == "Multi Shutter opened"
-        assert not multi_shutter.shutter_button.isEnabled()
-        assert shutter.shutter_button.text() == "Shutter opened"
-        assert not shutter.shutter_button.isEnabled()
-        assert state_dev_shutter.shutter_button.text() == "StateDev Shutter opened"
-        assert not state_dev_shutter.shutter_button.isEnabled()
+    assert shutter.shutter_button.text() == "Shutter opened"
+    assert not shutter.shutter_button.isEnabled()
 
     with qtbot.waitSignal(mmc.events.autoShutterSet):
         mmc.setAutoShutter(False)
     assert shutter.shutter_button.isEnabled()
     assert state_dev_shutter.shutter_button.isEnabled()
     assert multi_shutter.shutter_button.isEnabled()
-    assert multi_shutter.shutter_button.text() == "Multi Shutter opened"
     assert shutter.shutter_button.text() == "Shutter opened"
-    assert state_dev_shutter.shutter_button.text() == "StateDev Shutter opened"
 
+    with qtbot.waitSignal(mmc.events.autoShutterSet):
+        mmc.setAutoShutter(True)
     with qtbot.waitSignal(mmc.events.sequenceAcquisitionStopped):
         mmc.stopSequenceAcquisition()
-    assert shutter.shutter_button.isEnabled()
+    assert not shutter.shutter_button.isEnabled()
     assert state_dev_shutter.shutter_button.isEnabled()
     assert multi_shutter.shutter_button.isEnabled()
-    assert multi_shutter.shutter_button.text() == "Multi Shutter closed"
     assert shutter.shutter_button.text() == "Shutter closed"
-    assert state_dev_shutter.shutter_button.text() == "StateDev Shutter closed"
 
 
 def test_shutter_widget_autoshutter(qtbot: QtBot):
-
     shutter, state_dev_shutter, multi_shutter = _make_shutters(qtbot)
     mmc = CMMCorePlus.instance()
 
     assert multi_shutter.autoshutter_checkbox.isChecked()
 
     with qtbot.waitSignal(mmc.events.autoShutterSet):
         multi_shutter.autoshutter_checkbox.setChecked(False)
     assert shutter.shutter_button.isEnabled()
     assert state_dev_shutter.shutter_button.isEnabled()
     assert multi_shutter.shutter_button.isEnabled()
 
     with qtbot.waitSignal(mmc.events.autoShutterSet):
         multi_shutter.autoshutter_checkbox.setChecked(True)
     assert not shutter.shutter_button.isEnabled()
-    assert not state_dev_shutter.shutter_button.isEnabled()
-    assert not multi_shutter.shutter_button.isEnabled()
+    assert state_dev_shutter.shutter_button.isEnabled()
+    assert multi_shutter.shutter_button.isEnabled()
 
 
 def test_shutter_widget_button(qtbot: QtBot):
-
     shutter, state_dev_shutter, multi_shutter = _make_shutters(qtbot)
     mmc = CMMCorePlus.instance()
 
     with qtbot.waitSignal(mmc.events.configSet):
         mmc.setConfig("Channel", "DAPI")
 
     with qtbot.waitSignal(mmc.events.autoShutterSet):
         multi_shutter.autoshutter_checkbox.setChecked(False)
 
     with qtbot.waitSignal(mmc.events.propertyChanged):
         shutter.shutter_button.click()
-    assert shutter.shutter_button.text() == "Shutter opened"
-    assert mmc.getShutterOpen("Shutter")
-    assert mmc.getProperty("Shutter", "State") == "1"
-
-    with qtbot.waitSignal(mmc.events.propertyChanged):
-        shutter.shutter_button.click()
     assert shutter.shutter_button.text() == "Shutter closed"
     assert not mmc.getShutterOpen("Shutter")
     assert mmc.getProperty("Shutter", "State") == "0"
 
     with qtbot.waitSignal(mmc.events.propertyChanged):
+        shutter.shutter_button.click()
+    assert shutter.shutter_button.text() == "Shutter opened"
+    assert mmc.getShutterOpen("Shutter")
+    assert mmc.getProperty("Shutter", "State") == "1"
+
+    with qtbot.waitSignal(mmc.events.propertyChanged):
         state_dev_shutter.shutter_button.click()
     assert state_dev_shutter.shutter_button.text() == "StateDev Shutter opened"
     assert mmc.getShutterOpen("StateDev Shutter")
     assert mmc.getProperty("StateDev", "Label") == "State-1"
 
     with qtbot.waitSignal(mmc.events.propertyChanged):
         state_dev_shutter.shutter_button.click()
@@ -199,15 +186,14 @@
     assert mmc.getShutterOpen("Shutter")
     assert mmc.getProperty("Shutter", "State") == "1"
     assert mmc.getShutterOpen("StateDev Shutter")
     assert mmc.getProperty("StateDev", "Label") == "State-1"
 
 
 def test_shutter_widget_setters(qtbot: QtBot):
-
     shutter, _, _ = _make_shutters(qtbot)
     mmc = CMMCorePlus.instance()
 
     assert shutter.icon_size == 25
     shutter.icon_size = 30
     assert shutter.icon_size == 30
 
@@ -232,16 +218,65 @@
     assert shutter.shutter_button.text() == "O"
     with qtbot.waitSignal(mmc.events.sequenceAcquisitionStopped):
         mmc.stopSequenceAcquisition()
     assert shutter.shutter_button.text() == "C"
 
 
 def test_shutter_widget_UserWarning(qtbot: QtBot):
-
     _, _, multi_shutter = _make_shutters(qtbot)
     mmc = CMMCorePlus.instance()
 
     assert multi_shutter.shutter_button.text() == "Multi Shutter closed"
     with qtbot.waitSignal(mmc.events.systemConfigurationLoaded):
         with pytest.warns(UserWarning):
             mmc.loadSystemConfiguration("MMConfig_demo.cfg")
             assert multi_shutter.shutter_button.text() == "None"
+
+
+def test_multi_shutter_state_changed(qtbot: QtBot):
+    shutter, shutter1, multi_shutter = _make_shutters(qtbot)
+    mmc = CMMCorePlus.instance()
+
+    with qtbot.waitSignals([mmc.events.propertyChanged, mmc.events.configSet]):
+        mmc.setProperty("Core", "Shutter", "Multi Shutter")
+        mmc.setConfig("Channel", "DAPI")
+
+    with qtbot.waitSignal(mmc.events.propertyChanged):
+        mmc.setProperty("Multi Shutter", "State", "0")
+
+    assert mmc.getProperty("Multi Shutter", "State") == "0"
+    assert mmc.getProperty("Shutter", "State") == "0"
+
+    assert multi_shutter.shutter_button.text() == "Multi Shutter closed"
+    assert shutter.shutter_button.text() == "Shutter closed"
+
+    with qtbot.waitSignal(mmc.events.propertyChanged):
+        mmc.setProperty("Multi Shutter", "State", "1")
+
+    assert mmc.getProperty("Multi Shutter", "State") == "1"
+    assert mmc.getProperty("Shutter", "State") == "1"
+
+    assert multi_shutter.shutter_button.text() == "Multi Shutter opened"
+    assert shutter.shutter_button.text() == "Shutter opened"
+
+
+def test_on_shutter_device_changed(qtbot: QtBot):
+    shutter, shutter1, multi_shutter = _make_shutters(qtbot)
+    mmc = CMMCorePlus.instance()
+
+    with qtbot.waitSignals([mmc.events.propertyChanged, mmc.events.configSet]):
+        mmc.setProperty("Core", "Shutter", "Multi Shutter")
+        mmc.setConfig("Channel", "DAPI")
+
+    assert mmc.getShutterDevice() == "Multi Shutter"
+    assert not multi_shutter.shutter_button.isEnabled()
+    assert shutter.shutter_button.isEnabled()
+    assert shutter1.shutter_button.isEnabled()
+
+    with qtbot.waitSignals([mmc.events.propertyChanged, mmc.events.configSet]):
+        mmc.setProperty("Core", "Shutter", "Shutter")
+        mmc.setConfig("Channel", "DAPI")
+
+    assert mmc.getShutterDevice() == "Shutter"
+    assert multi_shutter.shutter_button.isEnabled()
+    assert not shutter.shutter_button.isEnabled()
+    assert shutter1.shutter_button.isEnabled()
```

### Comparing `pymmcore-widgets-0.3.0/tests/test_snap_button_widget.py` & `pymmcore-widgets-0.4.0/tests/test_snap_button_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 if TYPE_CHECKING:
     from pymmcore_plus import CMMCorePlus
     from pytestqt.qtbot import QtBot
 
 
 def test_snap_button_widget(qtbot: QtBot, global_mmcore: CMMCorePlus):
-
     snap_btn = SnapButton()
 
     qtbot.addWidget(snap_btn)
 
     assert snap_btn.text() == "Snap"
     assert snap_btn.iconSize() == QSize(30, 30)
```

### Comparing `pymmcore-widgets-0.3.0/tests/test_stage_widget.py` & `pymmcore-widgets-0.4.0/tests/test_stage_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 if TYPE_CHECKING:
     from pymmcore_plus import CMMCorePlus
     from pytestqt.qtbot import QtBot
 
 
 def test_stage_widget(qtbot: QtBot, global_mmcore: CMMCorePlus):
-
     # test XY stage
     stage_xy = StageWidget("XY", levels=3)
 
     qtbot.addWidget(stage_xy)
 
     assert global_mmcore.getXYStageDevice() == "XY"
     assert stage_xy.radiobutton.isChecked()
```

### Comparing `pymmcore-widgets-0.3.0/tests/test_table_pixel_size_widget.py` & `pymmcore-widgets-0.4.0/tests/test_table_pixel_size_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.3.0/tox.ini` & `pymmcore-widgets-0.4.0/tox.ini`

 * *Files identical despite different names*

