# Comparing `tmp/pymmcore_plus-0.7.0.tar.gz` & `tmp/pymmcore_plus-0.7.1.tar.gz`

## Comparing `pymmcore_plus-0.7.0.tar` & `pymmcore_plus-0.7.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/codecov.yml
--rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/mkdocs.yml
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/setup.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/.github/workflows/test_and_deploy.yml
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/docs/_hooks.py
--rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/docs/contributing.md
--rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/docs/index.md
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/docs/install.md
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/docs/api/cmmcoreplus.md
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/docs/api/configuration.md
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/docs/api/constants.md
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/docs/api/device.md
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/docs/api/events.md
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/docs/api/mda.md
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/docs/api/metadata.md
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/docs/api/utils.md
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/docs/examples/context-set.md
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/docs/examples/following_changes_in_core.md
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/docs/examples/integration-with-qt.md
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/docs/examples/mda.md
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/docs/examples/napari-micromanager.md
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/docs/guides/logging.md
--rw-r--r--   0        0        0    79333 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/docs/images/components.png
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/docs/images/favicon.ico
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/docs/stylesheets/extra.css
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/examples/napari.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/examples/properties_and_state_events.py
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/examples/qt_integration.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/examples/run_mda.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/examples/set_as_context.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/__init__.py
--rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/_build.py
--rw-r--r--   0        0        0    12170 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/_cli.py
--rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/_logger.py
--rw-r--r--   0        0        0     9549 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/_util.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/_version.py
--rw-r--r--   0        0        0     7950 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/install.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/py.typed
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/core/__init__.py
--rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/core/_adapter.py
--rw-r--r--   0        0        0    10558 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/core/_config.py
--rw-r--r--   0        0        0     8492 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/core/_config_group.py
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/core/_constants.py
--rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/core/_device.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/core/_metadata.py
--rw-r--r--   0        0        0    76552 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/core/_mmcore_plus.py
--rw-r--r--   0        0        0     8312 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/core/_property.py
--rw-r--r--   0        0        0    11633 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/core/_sequencing.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/core/events/__init__.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/core/events/_device_signal_view.py
--rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/core/events/_norm_slot.py
--rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/core/events/_prop_event_mixin.py
--rw-r--r--   0        0        0     7274 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/core/events/_protocol.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/core/events/_psygnal.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/core/events/_qsignals.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/mda/__init__.py
--rw-r--r--   0        0        0    10713 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/mda/_engine.py
--rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/mda/_protocol.py
--rw-r--r--   0        0        0    10794 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/mda/_runner.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/mda/events/__init__.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/mda/events/_protocol.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/mda/events/_psygnal.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/src/pymmcore_plus/mda/events/_qsignals.py
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/tests/conftest.py
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/tests/local_config.cfg
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/tests/test_adapter_class.py
--rw-r--r--   0        0        0     9560 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/tests/test_cli.py
--rw-r--r--   0        0        0     4635 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/tests/test_config_group_class.py
--rw-r--r--   0        0        0    17063 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/tests/test_core.py
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/tests/test_device_class.py
--rw-r--r--   0        0        0     9278 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/tests/test_events.py
--rw-r--r--   0        0        0     7011 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/tests/test_mda.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/tests/test_misc.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/tests/test_property_class.py
--rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/tests/test_sequencing.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/.gitignore
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/LICENSE
--rw-r--r--   0        0        0     5255 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/README.md
--rw-r--r--   0        0        0     4737 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     7745 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/codecov.yml
+-rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/mkdocs.yml
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/setup.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/_hooks.py
+-rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/contributing.md
+-rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/index.md
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/install.md
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/api/cmmcoreplus.md
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/api/configuration.md
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/api/constants.md
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/api/device.md
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/api/events.md
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/api/mda.md
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/api/metadata.md
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/api/utils.md
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/examples/context-set.md
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/examples/following_changes_in_core.md
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/examples/integration-with-qt.md
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/examples/mda.md
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/examples/napari-micromanager.md
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/guides/logging.md
+-rw-r--r--   0        0        0    79333 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/images/components.png
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/images/favicon.ico
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/examples/napari.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/examples/properties_and_state_events.py
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/examples/qt_integration.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/examples/run_mda.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/examples/set_as_context.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/__init__.py
+-rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/_build.py
+-rw-r--r--   0        0        0    12170 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/_cli.py
+-rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/_logger.py
+-rw-r--r--   0        0        0     9549 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/_util.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/_version.py
+-rw-r--r--   0        0        0     7950 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/install.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/py.typed
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/__init__.py
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/_adapter.py
+-rw-r--r--   0        0        0    10558 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/_config.py
+-rw-r--r--   0        0        0     8492 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/_config_group.py
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/_constants.py
+-rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/_device.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/_metadata.py
+-rw-r--r--   0        0        0    76552 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/_mmcore_plus.py
+-rw-r--r--   0        0        0     8312 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/_property.py
+-rw-r--r--   0        0        0    11636 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/_sequencing.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/events/__init__.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/events/_device_signal_view.py
+-rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/events/_norm_slot.py
+-rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/events/_prop_event_mixin.py
+-rw-r--r--   0        0        0     7274 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/events/_protocol.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/events/_psygnal.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/core/events/_qsignals.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/mda/__init__.py
+-rw-r--r--   0        0        0    11051 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/mda/_engine.py
+-rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/mda/_protocol.py
+-rw-r--r--   0        0        0    10794 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/mda/_runner.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/mda/events/__init__.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/mda/events/_protocol.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/mda/events/_psygnal.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/src/pymmcore_plus/mda/events/_qsignals.py
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/tests/conftest.py
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/tests/local_config.cfg
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/tests/test_adapter_class.py
+-rw-r--r--   0        0        0     9560 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/tests/test_cli.py
+-rw-r--r--   0        0        0     4635 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/tests/test_config_group_class.py
+-rw-r--r--   0        0        0    17063 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/tests/test_core.py
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/tests/test_device_class.py
+-rw-r--r--   0        0        0     9278 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/tests/test_events.py
+-rw-r--r--   0        0        0     7011 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/tests/test_mda.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/tests/test_misc.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/tests/test_property_class.py
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/tests/test_sequencing.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/LICENSE
+-rw-r--r--   0        0        0     5255 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/README.md
+-rw-r--r--   0        0        0     4737 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     7745 2020-02-02 00:00:00.000000 pymmcore_plus-0.7.1/PKG-INFO
```

### Comparing `pymmcore_plus-0.7.0/.pre-commit-config.yaml` & `pymmcore_plus-0.7.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/mkdocs.yml` & `pymmcore_plus-0.7.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/setup.py` & `pymmcore_plus-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/.github/workflows/docs.yml` & `pymmcore_plus-0.7.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/.github/workflows/test_and_deploy.yml` & `pymmcore_plus-0.7.1/.github/workflows/test_and_deploy.yml`

 * *Files 23% similar despite different names*

```diff
@@ -6,26 +6,26 @@
       - main
     tags:
       - "v*" # Push events to matching v*, i.e. v1.0, v20.15.10
   pull_request:
     branches:
       - main
   schedule:
-     - cron: "0 16 * * 1" # monday at noon est
+    - cron: "0 16 * * 1" # monday at noon est
   workflow_dispatch:
 
 jobs:
   test:
     name: ${{ matrix.platform }} py${{ matrix.python-version }}
     runs-on: ${{ matrix.platform }}
     strategy:
       fail-fast: false
       matrix:
         platform: [windows-latest, macos-latest]
-        python-version: ['3.8', '3.9', '3.10', '3.11']
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
 
     steps:
       - name: Cancel Previous Runs
         uses: styfle/cancel-workflow-action@0.11.0
         with:
           access_token: ${{ github.token }}
 
@@ -80,14 +80,52 @@
       - name: Install Micro-Manager
         run: mmcore install
 
       - name: Run pymmcore-widgets tests
         run: python -m pytest -v --color=yes -W ignore
         working-directory: pymmcore-widgets
 
+  test-napari-micro:
+    name: test napari-micromanager
+    runs-on: windows-latest
+    steps:
+      - uses: actions/checkout@v3
+        with:
+          path: pymmcore-plus
+          fetch-depth: 0
+
+      - uses: actions/checkout@v3
+        with:
+          repository: pymmcore-plus/napari-micromanager
+          path: napari-micromanager
+          fetch-depth: 0
+
+      - uses: actions/setup-python@v4
+        with:
+          python-version: "3.10"
+
+      - name: Install Windows OpenGL
+        if: runner.os == 'Windows'
+        run: |
+          git clone --depth 1 https://github.com/pyvista/gl-ci-helpers.git
+          powershell gl-ci-helpers/appveyor/install_opengl.ps1
+
+      - name: Install dependencies
+        run: |
+          python -m pip install -U pip
+          python -m pip install -e ./napari-micromanager[testing]
+          python -m pip install -e ./pymmcore-plus[testing]
+
+      - name: Install Micro-Manager
+        run: mmcore install
+
+      - name: Run napari-micromanager tests
+        run: python -m pytest -v --color=yes -W ignore
+        working-directory: napari-micromanager
+
   deploy:
     needs: test
     runs-on: ubuntu-latest
     if: ${{ github.repository == 'pymmcore-plus/pymmcore-plus' && contains(github.ref, 'tags') }}
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
```

### Comparing `pymmcore_plus-0.7.0/docs/_hooks.py` & `pymmcore_plus-0.7.1/docs/_hooks.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/docs/contributing.md` & `pymmcore_plus-0.7.1/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/docs/index.md` & `pymmcore_plus-0.7.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/docs/install.md` & `pymmcore_plus-0.7.1/docs/install.md`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/docs/api/cmmcoreplus.md` & `pymmcore_plus-0.7.1/docs/api/cmmcoreplus.md`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/docs/api/configuration.md` & `pymmcore_plus-0.7.1/docs/api/configuration.md`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/docs/api/constants.md` & `pymmcore_plus-0.7.1/docs/api/constants.md`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/docs/api/device.md` & `pymmcore_plus-0.7.1/docs/api/device.md`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/docs/examples/context-set.md` & `pymmcore_plus-0.7.1/docs/examples/context-set.md`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/docs/examples/following_changes_in_core.md` & `pymmcore_plus-0.7.1/docs/examples/following_changes_in_core.md`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/docs/examples/integration-with-qt.md` & `pymmcore_plus-0.7.1/docs/examples/integration-with-qt.md`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/docs/examples/mda.md` & `pymmcore_plus-0.7.1/docs/examples/mda.md`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/docs/examples/napari-micromanager.md` & `pymmcore_plus-0.7.1/docs/examples/napari-micromanager.md`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/docs/guides/logging.md` & `pymmcore_plus-0.7.1/docs/guides/logging.md`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/docs/images/components.png` & `pymmcore_plus-0.7.1/docs/images/components.png`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/docs/images/favicon.ico` & `pymmcore_plus-0.7.1/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/docs/stylesheets/extra.css` & `pymmcore_plus-0.7.1/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/examples/properties_and_state_events.py` & `pymmcore_plus-0.7.1/examples/properties_and_state_events.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/examples/qt_integration.py` & `pymmcore_plus-0.7.1/examples/qt_integration.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/examples/run_mda.py` & `pymmcore_plus-0.7.1/examples/run_mda.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/src/pymmcore_plus/__init__.py` & `pymmcore_plus-0.7.1/src/pymmcore_plus/__init__.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/src/pymmcore_plus/_build.py` & `pymmcore_plus-0.7.1/src/pymmcore_plus/_build.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/src/pymmcore_plus/_cli.py` & `pymmcore_plus-0.7.1/src/pymmcore_plus/_cli.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/src/pymmcore_plus/_logger.py` & `pymmcore_plus-0.7.1/src/pymmcore_plus/_logger.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/src/pymmcore_plus/_util.py` & `pymmcore_plus-0.7.1/src/pymmcore_plus/_util.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/src/pymmcore_plus/install.py` & `pymmcore_plus-0.7.1/src/pymmcore_plus/install.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/src/pymmcore_plus/core/__init__.py` & `pymmcore_plus-0.7.1/src/pymmcore_plus/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/src/pymmcore_plus/core/_adapter.py` & `pymmcore_plus-0.7.1/src/pymmcore_plus/core/_adapter.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/src/pymmcore_plus/core/_config.py` & `pymmcore_plus-0.7.1/src/pymmcore_plus/core/_config.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/src/pymmcore_plus/core/_config_group.py` & `pymmcore_plus-0.7.1/src/pymmcore_plus/core/_config_group.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/src/pymmcore_plus/core/_constants.py` & `pymmcore_plus-0.7.1/src/pymmcore_plus/core/_constants.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/src/pymmcore_plus/core/_device.py` & `pymmcore_plus-0.7.1/src/pymmcore_plus/core/_device.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/src/pymmcore_plus/core/_metadata.py` & `pymmcore_plus-0.7.1/src/pymmcore_plus/core/_metadata.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/src/pymmcore_plus/core/_mmcore_plus.py` & `pymmcore_plus-0.7.1/src/pymmcore_plus/core/_mmcore_plus.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/src/pymmcore_plus/core/_property.py` & `pymmcore_plus-0.7.1/src/pymmcore_plus/core/_property.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/src/pymmcore_plus/core/_sequencing.py` & `pymmcore_plus-0.7.1/src/pymmcore_plus/core/_sequencing.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,25 +240,25 @@
             if not core.isPropertySequenceable(dev, prop):
                 return _nope(f"'{dev}-{prop}' is not sequenceable")
             max_len = core.getPropertySequenceMaxLength(dev, prop)
             if cur_length >= max_len:  # pragma: no cover
                 return _nope(f"'{dev}-{prop}' {max_len=} < {cur_length=}")
 
     # Z
-    if e1.z_pos and e2.z_pos and (e1.z_pos != e2.z_pos):
+    if (e1.z_pos or e2.z_pos) and (e1.z_pos != e2.z_pos):
         focus_dev = core.getFocusDevice()
         if not core.isStageSequenceable(focus_dev):
             return _nope(f"Focus device {focus_dev!r} is not sequenceable")
         max_len = core.getStageSequenceMaxLength(focus_dev)
         if cur_length >= max_len:  # pragma: no cover
             return _nope(f"Focus device {focus_dev!r} {max_len=} < {cur_length=}")
 
     # XY
-    if (e1.x_pos and e2.x_pos and (e1.x_pos != e2.x_pos)) or (
-        e1.y_pos and e2.y_pos and (e1.y_pos != e2.y_pos)
+    if ((e1.x_pos or e2.x_pos) and (e1.x_pos != e2.x_pos)) or (
+        (e1.y_pos or e2.y_pos) and (e1.y_pos != e2.y_pos)
     ):
         stage = core.getXYStageDevice()
         if not core.isXYStageSequenceable(stage):
             return _nope(f"XYStage {stage!r} is not sequenceable")
         max_len = core.getXYStageSequenceMaxLength(stage)
         if cur_length >= max_len:  # pragma: no cover
             return _nope(f"XYStage {stage!r} {max_len=} < {cur_length=}")
```

### Comparing `pymmcore_plus-0.7.0/src/pymmcore_plus/core/events/__init__.py` & `pymmcore_plus-0.7.1/src/pymmcore_plus/core/events/__init__.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/src/pymmcore_plus/core/events/_device_signal_view.py` & `pymmcore_plus-0.7.1/src/pymmcore_plus/core/events/_device_signal_view.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/src/pymmcore_plus/core/events/_norm_slot.py` & `pymmcore_plus-0.7.1/src/pymmcore_plus/core/events/_norm_slot.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/src/pymmcore_plus/core/events/_prop_event_mixin.py` & `pymmcore_plus-0.7.1/src/pymmcore_plus/core/events/_prop_event_mixin.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/src/pymmcore_plus/core/events/_protocol.py` & `pymmcore_plus-0.7.1/src/pymmcore_plus/core/events/_protocol.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/src/pymmcore_plus/core/events/_psygnal.py` & `pymmcore_plus-0.7.1/src/pymmcore_plus/core/events/_psygnal.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/src/pymmcore_plus/core/events/_qsignals.py` & `pymmcore_plus-0.7.1/src/pymmcore_plus/core/events/_qsignals.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/src/pymmcore_plus/mda/_engine.py` & `pymmcore_plus-0.7.1/src/pymmcore_plus/mda/_engine.py`

 * *Files 8% similar despite different names*

```diff
@@ -177,25 +177,37 @@
         # is changed to accept the camera in the future, that should be kept in mind.
         self._mmc.startSequenceAcquisition(
             n_events,
             0,  # intervalMS  # TODO: add support for this
             True,  # stopOnOverflow
         )
 
-        # block until the sequence is done
+        # block until the sequence is done, popping images in the meantime
+        images = []
         while self._mmc.isSequenceRunning():
-            time.sleep(0.001)
+            if self._mmc.getRemainingImageCount():
+                images.append(self._mmc.popNextImage())
+            else:
+                time.sleep(0.001)
 
-        # TODO: collect images
-        tagged_imgs = []
-        for _ in range(n_events):  # or getRemainingImageCount()
-            if self._mmc.isBufferOverflowed():
-                raise MemoryError("Buffer overflowed")
-            tagged_imgs.append(self._mmc.popNextImage())
-        return EventPayload(image_sequence=tagged_imgs)
+        if self._mmc.isBufferOverflowed():
+            raise MemoryError("Buffer overflowed")
+
+        while self._mmc.getRemainingImageCount():
+            images.append(self._mmc.popNextImage())
+
+        if len(images) != n_events:
+            logger.warning(
+                "Unexpected number of images returned from sequence. "
+                "Expected {}, got {}",
+                n_events,
+                len(images),
+            )
+
+        return EventPayload(image_sequence=images)
 
     def exec_single_event(self, event: MDAEvent) -> EventPayload | None:
         """Execute a single (non-triggered) event and return the image data.
 
         This method is not part of the PMDAEngine protocol (it is called by
         `exec_event`, which *is* part of the protocol), but it is made public
         in case a user wants to subclass this engine and override this method.
```

### Comparing `pymmcore_plus-0.7.0/src/pymmcore_plus/mda/_protocol.py` & `pymmcore_plus-0.7.1/src/pymmcore_plus/mda/_protocol.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/src/pymmcore_plus/mda/_runner.py` & `pymmcore_plus-0.7.1/src/pymmcore_plus/mda/_runner.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/src/pymmcore_plus/mda/events/__init__.py` & `pymmcore_plus-0.7.1/src/pymmcore_plus/mda/events/__init__.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/src/pymmcore_plus/mda/events/_protocol.py` & `pymmcore_plus-0.7.1/src/pymmcore_plus/mda/events/_protocol.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/tests/conftest.py` & `pymmcore_plus-0.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/tests/local_config.cfg` & `pymmcore_plus-0.7.1/tests/local_config.cfg`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/tests/test_adapter_class.py` & `pymmcore_plus-0.7.1/tests/test_adapter_class.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/tests/test_cli.py` & `pymmcore_plus-0.7.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/tests/test_config_group_class.py` & `pymmcore_plus-0.7.1/tests/test_config_group_class.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/tests/test_core.py` & `pymmcore_plus-0.7.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/tests/test_device_class.py` & `pymmcore_plus-0.7.1/tests/test_device_class.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/tests/test_events.py` & `pymmcore_plus-0.7.1/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/tests/test_mda.py` & `pymmcore_plus-0.7.1/tests/test_mda.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/tests/test_misc.py` & `pymmcore_plus-0.7.1/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/tests/test_property_class.py` & `pymmcore_plus-0.7.1/tests/test_property_class.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/tests/test_sequencing.py` & `pymmcore_plus-0.7.1/tests/test_sequencing.py`

 * *Files 15% similar despite different names*

```diff
@@ -47,14 +47,23 @@
     expected_exposure = [call(5), call(10)] * 2
     assert core_mock.setExposure.call_args_list == expected_exposure
 
     expected_pos = [call(0, 0), call(0, 0), call(1, 1), call(1, 1)]
     assert core_mock.setXYPosition.call_args_list == expected_pos
 
 
+def test_sequenced_mda_with_zero_values() -> None:
+    # just testing a bug I found where if z, x, or y are 0, they accidentally
+    # get sequenced
+    mda = useq.MDASequence(z_plan=useq.ZRangeAround(range=3.0, step=0.5))
+    core = CMMCorePlus()
+    core.loadSystemConfiguration()
+    core.mda.run(mda)
+
+
 def test_fully_sequenceable_core():
     mda = useq.MDASequence(
         stage_positions=[(0, 0, 0), (1, 1, 1)],
         z_plan=useq.ZRangeAround(range=3, step=1),
         channels=[
             useq.Channel(config="DAPI", exposure=5),
             useq.Channel(config="FITC", exposure=10),
@@ -63,14 +72,15 @@
     )
 
     CAM = "Camera"
     XYSTAGE = "XYStage"
     FOCUS = "Z"
     core_mock = cast("CMMCorePlus", MagicMock(spec=CMMCorePlus))
     core_mock.isSequenceRunning.return_value = False
+    core_mock.getRemainingImageCount.return_value = 0
     core_mock.isBufferOverflowed.return_value = False
     core_mock.getCameraDevice.return_value = CAM
     core_mock.getXYStageDevice.return_value = XYSTAGE
     core_mock.getFocusDevice.return_value = FOCUS
     core_mock.getFocusDevice.return_value = FOCUS
     core_mock.getPixelSizeUm.return_value = None
 
@@ -89,7 +99,18 @@
     core_mock.startSequenceAcquisition.assert_called_once_with(n_img, 0, True)
     core_mock.loadExposureSequence.assert_called_once_with(
         CAM, seq_event.exposure_sequence
     )
     core_mock.loadXYStageSequence.assert_called_once_with(
         XYSTAGE, seq_event.x_sequence, seq_event.y_sequence
     )
+
+
+def test_sequenced_circular_buffer(core: CMMCorePlus):
+    core.initializeCircularBuffer()
+    core.setCircularBufferMemoryFootprint(20)
+    max_imgs = core.getBufferFreeCapacity()
+    mda = useq.MDASequence(
+        channels=["DAPI"],
+        time_plan=useq.TIntervalLoops(interval=0, loops=max_imgs * 2),
+    )
+    core.mda.run(mda)
```

### Comparing `pymmcore_plus-0.7.0/.gitignore` & `pymmcore_plus-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/LICENSE` & `pymmcore_plus-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/README.md` & `pymmcore_plus-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/pyproject.toml` & `pymmcore_plus-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.7.0/PKG-INFO` & `pymmcore_plus-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymmcore-plus
-Version: 0.7.0
+Version: 0.7.1
 Summary: pymmcore superset providing improved APIs, event connection, and a pure python acquisition engine
 Project-URL: Source, https://github.com/pymmcore-plus/pymmcore-plus
 Project-URL: Tracker, https://github.com/pymmcore-plus/pymmcore-plus/issues
 Project-URL: Documentation, https://pymmcore-plus.github.io/pymmcore-plus
 Author-email: Talley Lambert <talley.lambert@gmail.com>, Federico Gasparoli <federico.gasparoli@gmail.com>, Ian Hunt-Isaak <ianhuntisaak@gmail.com>
 License: BSD 3-Clause License
 License-File: LICENSE
```

