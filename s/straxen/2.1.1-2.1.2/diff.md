# Comparing `tmp/straxen-2.1.1.tar.gz` & `tmp/straxen-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "straxen-2.1.1.tar", last modified: Fri Jul  7 03:53:00 2023, max compression
+gzip compressed data, was "straxen-2.1.2.tar", last modified: Fri Jul 28 13:50:48 2023, max compression
```

## Comparing `straxen-2.1.1.tar` & `straxen-2.1.2.tar`

### file list

```diff
@@ -1,242 +1,242 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.505946 straxen-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    40896 2023-07-07 03:52:57.000000 straxen-2.1.1/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-07 03:52:57.000000 straxen-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-07 03:52:57.000000 straxen-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    53674 2023-07-07 03:53:00.505946 straxen-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-07 03:52:57.000000 straxen-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.485943 straxen-2.1.1/bin/
--rw-r--r--   0 runner    (1001) docker     (123)    37235 2023-07-07 03:52:57.000000 straxen-2.1.1/bin/ajax
--rwxr-xr-x   0 runner    (1001) docker     (123)    67099 2023-07-07 03:52:57.000000 straxen-2.1.1/bin/bootstrax
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-07-07 03:52:57.000000 straxen-2.1.1/bin/fake_daq
--rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-07-07 03:52:57.000000 straxen-2.1.1/bin/microstrax
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-07-07 03:52:57.000000 straxen-2.1.1/bin/refresh_raw_records
--rw-r--r--   0 runner    (1001) docker     (123)    35964 2023-07-07 03:52:57.000000 straxen-2.1.1/bin/restrax
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-07 03:52:57.000000 straxen-2.1.1/bin/straxen-print_versions
--rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-07-07 03:52:57.000000 straxen-2.1.1/bin/straxer
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.485943 straxen-2.1.1/extra_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-07 03:52:57.000000 straxen-2.1.1/extra_requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-07 03:52:57.000000 straxen-2.1.1/extra_requirements/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-07 03:52:57.000000 straxen-2.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-07 03:53:00.509946 straxen-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-07 03:52:57.000000 straxen-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.485943 straxen-2.1.1/straxen/
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.489944 straxen-2.1.1/straxen/analyses/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/analyses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38941 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/analyses/bokeh_waveform_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/analyses/daq_waveforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    18579 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/analyses/event_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    17242 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/analyses/holoviews_waveform_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/analyses/posrec_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/analyses/pulse_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/analyses/quick_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/analyses/records_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/analyses/waveform_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/bokeh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21032 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    22966 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)    18385 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/corrections_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/daq_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/get_corrections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.489944 straxen-2.1.1/straxen/holoviews/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/holoviews/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/holoviews/holoviews_inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)    13244 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/holoviews/holoviews_peak_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/holoviews/holoviews_pmt_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    17711 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/holoviews/holoviews_tpc_event_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    21799 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/holoviews_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/itp_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.489944 straxen-2.1.1/straxen/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/legacy/contexts_1t.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/legacy/hitfinder_thresholds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.489944 straxen-2.1.1/straxen/legacy/plugins_1t/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/legacy/plugins_1t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/legacy/plugins_1t/event_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/legacy/plugins_1t/pax_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/legacy/plugins_1t/peak_positions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/legacy/plugins_1t/x1t_cuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/legacy/xenon1t_url_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/matplotlib_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/mini_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/numbafied_scipy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.489944 straxen-2.1.1/straxen/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.489944 straxen-2.1.1/straxen/plugins/afterpulses/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/afterpulses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11243 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/afterpulses/afterpulse_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.493944 straxen-2.1.1/straxen/plugins/aqmon_hits/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/aqmon_hits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/aqmon_hits/aqmon_hits.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.493944 straxen-2.1.1/straxen/plugins/detector_time_offsets/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/detector_time_offsets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/detector_time_offsets/detector_time_offsets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.493944 straxen-2.1.1/straxen/plugins/events/
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/_event_s1_positions_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/_event_s2_positions_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/corrected_areas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/distinct_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/energy_estimates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/event_ambience.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/event_area_per_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    16617 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/event_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/event_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/event_info_double.py
--rw-r--r--   0 runner    (1001) docker     (123)    25160 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/event_pattern_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/event_positions.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/event_s1_positions_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/event_s2_positions_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/event_s2_positions_gcn.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/event_s2_positions_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/event_shadow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/event_top_bottom_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/event_w_bayes_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/event_waveform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/local_minimum_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/multi_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/s2_recon_pos_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/veto_proximity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.493944 straxen-2.1.1/straxen/plugins/events_mv/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events_mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events_mv/events_mv.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events_mv/events_sync_mv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.497945 straxen-2.1.1/straxen/plugins/events_nv/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events_nv/event_positions_nv.py
--rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events_nv/events_nv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events_nv/events_sync_nv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.497945 straxen-2.1.1/straxen/plugins/hitlets_mv/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/hitlets_mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/hitlets_mv/hitlets_mv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.497945 straxen-2.1.1/straxen/plugins/hitlets_nv/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/hitlets_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/hitlets_nv/hitlets_nv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.497945 straxen-2.1.1/straxen/plugins/individual_peak_monitor/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/individual_peak_monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/individual_peak_monitor/individual_peak_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.497945 straxen-2.1.1/straxen/plugins/led_cal/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/led_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/led_cal/led_calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.497945 straxen-2.1.1/straxen/plugins/merged_s2s/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/merged_s2s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/merged_s2s/merged_s2s.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.497945 straxen-2.1.1/straxen/plugins/merged_s2s_he/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/merged_s2s_he/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/merged_s2s_he/merged_s2s_he.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.497945 straxen-2.1.1/straxen/plugins/online_monitor_mv/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/online_monitor_mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/online_monitor_mv/online_monitor_mv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.497945 straxen-2.1.1/straxen/plugins/online_monitor_nv/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/online_monitor_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/online_monitor_nv/online_monitor_nv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.497945 straxen-2.1.1/straxen/plugins/online_peak_monitor/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/online_peak_monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/online_peak_monitor/online_peak_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.497945 straxen-2.1.1/straxen/plugins/peaklets/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaklets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaklets/peaklet_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    25757 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaklets/peaklets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.497945 straxen-2.1.1/straxen/plugins/peaklets_he/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaklets_he/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaklets_he/peaklet_classification_he.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaklets_he/peaklets_he.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.501945 straxen-2.1.1/straxen/plugins/peaks/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/_peak_positions_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/_peak_s1_positions_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/peak_ambience.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/peak_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/peak_classification_bayes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/peak_corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/peak_per_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/peak_positions.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/peak_positions_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/peak_positions_gcn.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/peak_positions_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/peak_proximity.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/peak_s1_positions_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9637 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/peak_shadow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/peak_top_bottom_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/peaks_subtyping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.501945 straxen-2.1.1/straxen/plugins/peaks_he/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks_he/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks_he/peak_basics_he.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks_he/peaks_he.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.501945 straxen-2.1.1/straxen/plugins/raw_records/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/raw_records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16653 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/raw_records/daqreader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.501945 straxen-2.1.1/straxen/plugins/raw_records_coin_nv/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/raw_records_coin_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19659 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/raw_records_coin_nv/nveto_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.501945 straxen-2.1.1/straxen/plugins/records/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17703 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/records/records.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.501945 straxen-2.1.1/straxen/plugins/records_he/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/records_he/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/records_he/records_he.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.501945 straxen-2.1.1/straxen/plugins/records_mv/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/records_mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/records_mv/records_mv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.501945 straxen-2.1.1/straxen/plugins/records_nv/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/records_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/records_nv/records_nv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.501945 straxen-2.1.1/straxen/plugins/veto_intervals/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/veto_intervals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/veto_intervals/veto_intervals.py
--rw-r--r--   0 runner    (1001) docker     (123)    27943 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/scada.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.501945 straxen-2.1.1/straxen/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/storage/mongo_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/storage/online_monitor_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/storage/rucio_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/storage/rucio_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    13251 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/storage/rundb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    25282 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/url_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.489944 straxen-2.1.1/straxen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    53674 2023-07-07 03:53:00.000000 straxen-2.1.1/straxen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-07-07 03:53:00.000000 straxen-2.1.1/straxen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 03:53:00.000000 straxen-2.1.1/straxen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 03:53:00.000000 straxen-2.1.1/straxen.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-07 03:53:00.000000 straxen-2.1.1/straxen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-07 03:53:00.000000 straxen-2.1.1/straxen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.505946 straxen-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.505946 straxen-2.1.1/tests/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9751 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/storage/test_database_frontends.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/storage/test_mongo_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/storage/test_mongo_interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/storage/test_rucio_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/storage/test_rucio_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_1T_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    10536 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_aqmon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_channel_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_cmt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_count_pulses.py
--rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_daq_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_holoviews_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_itp_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_led_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)    17347 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_mini_analyses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_nveto_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_nveto_recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_patternfit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_peaklet_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_scada.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_testing_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_url_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_veto_hitlets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.044876 straxen-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    41447 2023-07-28 13:50:43.000000 straxen-2.1.2/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-28 13:50:43.000000 straxen-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 13:50:43.000000 straxen-2.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    54313 2023-07-28 13:50:48.044876 straxen-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-28 13:50:43.000000 straxen-2.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.000874 straxen-2.1.2/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    37235 2023-07-28 13:50:43.000000 straxen-2.1.2/bin/ajax
+-rwxr-xr-x   0 runner    (1001) docker     (123)    67099 2023-07-28 13:50:43.000000 straxen-2.1.2/bin/bootstrax
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-07-28 13:50:43.000000 straxen-2.1.2/bin/fake_daq
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-07-28 13:50:43.000000 straxen-2.1.2/bin/microstrax
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-07-28 13:50:43.000000 straxen-2.1.2/bin/refresh_raw_records
+-rw-r--r--   0 runner    (1001) docker     (123)    35964 2023-07-28 13:50:43.000000 straxen-2.1.2/bin/restrax
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-28 13:50:43.000000 straxen-2.1.2/bin/straxen-print_versions
+-rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-07-28 13:50:43.000000 straxen-2.1.2/bin/straxer
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.000874 straxen-2.1.2/extra_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-28 13:50:43.000000 straxen-2.1.2/extra_requirements/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-28 13:50:43.000000 straxen-2.1.2/extra_requirements/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-28 13:50:43.000000 straxen-2.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-28 13:50:48.044876 straxen-2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-28 13:50:43.000000 straxen-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.004874 straxen-2.1.2/straxen/
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.008874 straxen-2.1.2/straxen/analyses/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/analyses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38941 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/analyses/bokeh_waveform_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/analyses/daq_waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18579 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/analyses/event_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17242 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/analyses/holoviews_waveform_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/analyses/posrec_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/analyses/pulse_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/analyses/quick_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/analyses/records_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/analyses/waveform_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/bokeh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21032 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22966 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18385 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/corrections_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/daq_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/get_corrections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.008874 straxen-2.1.2/straxen/holoviews/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/holoviews/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/holoviews/holoviews_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13244 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/holoviews/holoviews_peak_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/holoviews/holoviews_pmt_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17711 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/holoviews/holoviews_tpc_event_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21799 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/holoviews_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14119 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/itp_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.008874 straxen-2.1.2/straxen/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/legacy/contexts_1t.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/legacy/hitfinder_thresholds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.008874 straxen-2.1.2/straxen/legacy/plugins_1t/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/legacy/plugins_1t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/legacy/plugins_1t/event_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/legacy/plugins_1t/pax_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/legacy/plugins_1t/peak_positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/legacy/plugins_1t/x1t_cuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/legacy/xenon1t_url_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/matplotlib_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/mini_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/numbafied_scipy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.008874 straxen-2.1.2/straxen/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.012874 straxen-2.1.2/straxen/plugins/afterpulses/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/afterpulses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11243 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/afterpulses/afterpulse_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.012874 straxen-2.1.2/straxen/plugins/aqmon_hits/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/aqmon_hits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/aqmon_hits/aqmon_hits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.012874 straxen-2.1.2/straxen/plugins/detector_time_offsets/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/detector_time_offsets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/detector_time_offsets/detector_time_offsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.016875 straxen-2.1.2/straxen/plugins/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events/_event_s1_positions_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events/_event_s2_positions_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events/corrected_areas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events/distinct_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events/energy_estimates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events/event_ambience.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events/event_area_per_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16617 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events/event_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events/event_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events/event_info_double.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25160 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events/event_pattern_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events/event_positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events/event_s1_positions_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events/event_s2_positions_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events/event_s2_positions_gcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events/event_s2_positions_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events/event_shadow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events/event_top_bottom_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events/event_w_bayes_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events/event_waveform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events/local_minimum_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events/multi_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events/s2_recon_pos_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events/veto_proximity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.016875 straxen-2.1.2/straxen/plugins/events_mv/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events_mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events_mv/events_mv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events_mv/events_sync_mv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.020875 straxen-2.1.2/straxen/plugins/events_nv/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events_nv/event_positions_nv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events_nv/events_nv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/events_nv/events_sync_nv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.020875 straxen-2.1.2/straxen/plugins/hitlets_mv/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/hitlets_mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/hitlets_mv/hitlets_mv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.020875 straxen-2.1.2/straxen/plugins/hitlets_nv/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/hitlets_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/hitlets_nv/hitlets_nv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.020875 straxen-2.1.2/straxen/plugins/individual_peak_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/individual_peak_monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/individual_peak_monitor/individual_peak_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.020875 straxen-2.1.2/straxen/plugins/led_cal/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/led_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/led_cal/led_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.020875 straxen-2.1.2/straxen/plugins/merged_s2s/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/merged_s2s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/merged_s2s/merged_s2s.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.024875 straxen-2.1.2/straxen/plugins/merged_s2s_he/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/merged_s2s_he/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/merged_s2s_he/merged_s2s_he.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.024875 straxen-2.1.2/straxen/plugins/online_monitor_mv/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/online_monitor_mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/online_monitor_mv/online_monitor_mv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.024875 straxen-2.1.2/straxen/plugins/online_monitor_nv/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/online_monitor_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/online_monitor_nv/online_monitor_nv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.024875 straxen-2.1.2/straxen/plugins/online_peak_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/online_peak_monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/online_peak_monitor/online_peak_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.024875 straxen-2.1.2/straxen/plugins/peaklets/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/peaklets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/peaklets/peaklet_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25757 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/peaklets/peaklets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.028875 straxen-2.1.2/straxen/plugins/peaklets_he/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/peaklets_he/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/peaklets_he/peaklet_classification_he.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/peaklets_he/peaklets_he.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.032875 straxen-2.1.2/straxen/plugins/peaks/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/peaks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/peaks/_peak_positions_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/peaks/_peak_s1_positions_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/peaks/peak_ambience.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/peaks/peak_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/peaks/peak_classification_bayes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/peaks/peak_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/peaks/peak_per_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/peaks/peak_positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/peaks/peak_positions_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/peaks/peak_positions_gcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/peaks/peak_positions_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/peaks/peak_proximity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/peaks/peak_s1_positions_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9637 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/peaks/peak_shadow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/peaks/peak_top_bottom_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/peaks/peaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/peaks/peaks_subtyping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.032875 straxen-2.1.2/straxen/plugins/peaks_he/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/peaks_he/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/peaks_he/peak_basics_he.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/peaks_he/peaks_he.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.032875 straxen-2.1.2/straxen/plugins/raw_records/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/raw_records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16653 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/raw_records/daqreader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.032875 straxen-2.1.2/straxen/plugins/raw_records_coin_nv/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/raw_records_coin_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19659 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/raw_records_coin_nv/nveto_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.032875 straxen-2.1.2/straxen/plugins/records/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17703 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/records/records.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.036875 straxen-2.1.2/straxen/plugins/records_he/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/records_he/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/records_he/records_he.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.036875 straxen-2.1.2/straxen/plugins/records_mv/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/records_mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/records_mv/records_mv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.036875 straxen-2.1.2/straxen/plugins/records_nv/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/records_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/records_nv/records_nv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.036875 straxen-2.1.2/straxen/plugins/veto_intervals/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/veto_intervals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/plugins/veto_intervals/veto_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27943 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/scada.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.036875 straxen-2.1.2/straxen/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/storage/mongo_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/storage/online_monitor_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/storage/rucio_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/storage/rucio_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13251 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/storage/rundb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25950 2023-07-28 13:50:43.000000 straxen-2.1.2/straxen/url_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.004874 straxen-2.1.2/straxen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    54313 2023-07-28 13:50:47.000000 straxen-2.1.2/straxen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-07-28 13:50:47.000000 straxen-2.1.2/straxen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:50:47.000000 straxen-2.1.2/straxen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:50:47.000000 straxen-2.1.2/straxen.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-28 13:50:47.000000 straxen-2.1.2/straxen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-28 13:50:47.000000 straxen-2.1.2/straxen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.044876 straxen-2.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:48.044876 straxen-2.1.2/tests/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9751 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/storage/test_database_frontends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/storage/test_mongo_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/storage/test_mongo_interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/storage/test_rucio_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/storage/test_rucio_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/test_1T_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10536 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/test_aqmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/test_channel_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/test_cmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/test_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/test_count_pulses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/test_daq_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/test_holoviews_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/test_itp_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/test_led_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17347 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/test_mini_analyses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/test_nveto_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/test_nveto_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/test_patternfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/test_peaklet_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/test_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/test_scada.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/test_testing_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/test_url_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-28 13:50:43.000000 straxen-2.1.2/tests/test_veto_hitlets.py
```

### Comparing `straxen-2.1.1/HISTORY.md` & `straxen-2.1.2/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,30 @@
-v2.1.1 / 2023-07-06
+2.1.2 / 2023-07-28
+-------------------
+* Validate final type after URL eval by @jmosbacher in https://github.com/XENONnT/straxen/pull/1217
+* Fix URLConfig.evaluate_dry by @jmosbacher in https://github.com/XENONnT/straxen/pull/1219
+* Add function to save itp_map InterpolatingMap related dictionary into pickle by @dachengx in https://github.com/XENONnT/straxen/pull/1221
+* Rename `tf_peak_model_s1_cnn` to `tf_model_s1_cnn` by @dachengx in https://github.com/XENONnT/straxen/pull/1223
+
+
+**Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.1.1...v2.1.2
+
+
+2.1.1 / 2023-07-06
 -------------------
 * Fix timing of peaks when ordering in `center_time` by @dachengx in https://github.com/XENONnT/straxen/pull/1208
 * Move `get_window_size` factor of merged_s2s as untracked configuration by @dachengx in https://github.com/XENONnT/straxen/pull/1209
 * Sort `hitlets` in `nVETOHitlets` by @dachengx in https://github.com/XENONnT/straxen/pull/1210
 * Only print out warning once by @LuisSanchez25 in https://github.com/XENONnT/straxen/pull/1211
 
 
 **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.1.0...v2.1.1
 
 
-v2.1.0 / 2023-06-22
+2.1.0 / 2023-06-22
 -------------------
 * Added peaks subtyping by @Jianyu010 in https://github.com/XENONnT/straxen/pull/1152
 * Fix ipython version by @dachengx in https://github.com/XENONnT/straxen/pull/1169
 * Fix bug in hitlets time ordering by @dachengx in https://github.com/XENONnT/straxen/pull/1173
 * Bump actions/setup-python from 4.5.0 to 4.6.0 by @dependabot in https://github.com/XENONnT/straxen/pull/1170
 * Save hits level information(hits height and time difference) in peak and event level by @dachengx in https://github.com/XENONnT/straxen/pull/1155
 * Fix argsort inside numba.jit using kind='mergesort' by @dachengx in https://github.com/XENONnT/straxen/pull/1176
@@ -36,15 +47,15 @@
 New Contributors
 * @PeterGy made their first contribution in https://github.com/XENONnT/straxen/pull/1202
 * @minzhong98 made their first contribution in https://github.com/XENONnT/straxen/pull/1191
 
 **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.7...v2.1.0
 
 
-v2.0.7 / 2023-04-25
+2.0.7 / 2023-04-25
 -------------------
 * Bootstrax target removal after failures by @cfuselli in https://github.com/XENONnT/straxen/pull/1145
 * reforming _raw_path and _processed_path by @FaroutYLq in https://github.com/XENONnT/straxen/pull/1149
 * Adding correction of Z position due to non-uniform drift velocity by @terliuk in https://github.com/XENONnT/straxen/pull/1148
 * Bump the versions of peaklets and quality check runs-on by @dachengx in https://github.com/XENONnT/straxen/pull/1153
 * S1-Based 3D Position Reconstruction by @matteoguida in https://github.com/XENONnT/straxen/pull/1146
 * Bump xedocs from 0.2.14 to 0.2.16 in /extra_requirements by @dependabot in https://github.com/XENONnT/straxen/pull/1158
@@ -55,79 +66,79 @@
 * @cfuselli made their first contribution in https://github.com/XENONnT/straxen/pull/1145
 * @matteoguida made their first contribution in https://github.com/XENONnT/straxen/pull/1146
 * @hmdyt made their first contribution in https://github.com/XENONnT/straxen/pull/1159
 
 **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.6...v2.0.7
 
 
-v2.0.6 / 2023-03-08
+2.0.6 / 2023-03-08
 -------------------
 * Bump supercharge/mongodb-github-action from 1.8.0 to 1.9.0 by @dependabot in https://github.com/XENONnT/straxen/pull/1140
 * Small patches to restrax module by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1143, d04a3428c52c159577b61af2a28ddd0af5652027, 602b807291211f083c8f54df6768b8198fbf6b55
 * Ms events by @michaweiss89 and @HenningSE in https://github.com/XENONnT/straxen/pull/1080
 
 New Contributors
 * @michaweiss89 made their first contribution in https://github.com/XENONnT/straxen/pull/1080
 
 **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.5...v2.0.6
 
 Notes:
  - new data types: `peaks_per_event`, `event_top_bottom_params`, `peaks_corrections` (see #1080)
 
 
-v2.0.5 / 2023-02-24
+2.0.5 / 2023-02-24
 -------------------
 * fix xedocs for testing by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1139
 * Restart python style guide by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1138
 * Decrease number of chunks by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1123
 * Restrax by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1074
 
 
 **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.4...v2.0.5
 
 
-v2.0.4 / 2023-01-16
+2.0.4 / 2023-01-16
 -------------------
 * Top and bottom timing parameters at event and peak level by @terliuk in https://github.com/XENONnT/straxen/pull/1119
 * Allow use of xedocs context configs by @jmosbacher in https://github.com/XENONnT/straxen/pull/1125
 * Bump actions/setup-python from 4.3.0 to 4.4.0 by @dependabot in https://github.com/XENONnT/straxen/pull/1128
 * Add entry points by @jmosbacher in https://github.com/XENONnT/straxen/pull/1120
 * URLConfig preprocessor by @jmosbacher in https://github.com/XENONnT/straxen/pull/1110
 * Fix bootstrax timeouts by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1133
 
 
 **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.3...v2.1.0
 
 Notes:
  - new data types: `peak_top_bottom_params`, `event_top_bottom_params`
 
-v2.0.3 / 2022-11-09
+2.0.3 / 2022-11-09
 -------------------
 * Adding peak waveforms at event level by @terliuk in https://github.com/XENONnT/straxen/pull/1112
 
 
 **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.2...v2.0.3
 
 Notes:
  * lineage changes for event_area_per_channel
 
 
-v2.0.2 / 2022-10-24
+2.0.2 / 2022-10-24
 -------------------
 * New URLConfig protocols - list-to-array and list-to-dict by @LuisSanchez25 in https://github.com/XENONnT/straxen/pull/1104
 * Single core 1T test by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1109
 
 New Contributors
 * @LuisSanchez25 made their first contribution in https://github.com/XENONnT/straxen/pull/1104
 
 
 **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.1...v2.0.2
 
 
-v2.0.1 / 2022-10-20
+2.0.1 / 2022-10-20
 -------------------
 * Use mongodb v4.4.1 when testing to match real version used in production by @jmosbacher in https://github.com/XENONnT/straxen/pull/1103
 * Pass tests from remote forks by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1105
 * Local minimum info 2 by @JYangQi00 in https://github.com/XENONnT/straxen/pull/1106
 * Don't test without `strax.processor.SHMExecutor` by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1107
 * Lower the default config value of online_max_bytes by @mflierm in https://github.com/XENONnT/straxen/pull/1108
 
@@ -135,15 +146,15 @@
 New Contributors
 * @JYangQi00 made their first contribution in https://github.com/XENONnT/straxen/pull/1106
 
 
 **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.0...v2.0.1
 
 
-v2.0.0 / 2022-10-17
+2.0.0 / 2022-10-17
 -------------------
 * Fix acqmon veto field by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1072
 * Use self.dtype also for empty peaks by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1058
 * Re Start style guide by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1084
 * Transition plugins to URLConfig by @jmosbacher in https://github.com/XENONnT/straxen/pull/1079
 * Fix help of peak basics. by @WenzDaniel in https://github.com/XENONnT/straxen/pull/1081
 * Remove `tight_coincidence_channel` fix #1078 by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1092
@@ -163,39 +174,39 @@
  * Changed signatures of plugins in [#1094](https://github.com/XENONnT/straxen/pull/1094)
  * New plugins for event level processing by [#1097](https://github.com/XENONnT/straxen/pull/1097)
 
 
 **Full Changelog**: https://github.com/XENONnT/straxen/compare/v1.8.3...v2.0.0
 
 
-v1.8.3 / 2022-07-18
+1.8.3 / 2022-07-18
 -------------------
 * Bootstrax file-check fix by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1064
 * Fix hanging straxer by @jmosbacher in https://github.com/XENONnT/straxen/pull/1065
 
 Notes:
 * No lineage changes
 
 Full Changelog:
  - https://github.com/XENONnT/straxen/compare/v1.8.2...v1.8.3
 
 
-v1.8.2 / 2022-07-12
+1.8.2 / 2022-07-12
 -------------------
 * Stop tf pbar by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1063
 * Allow long runs by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1062
 
 Notes:
 * No lineage changes
 
 Full Changelog:
 - https://github.com/XENONnT/straxen/compare/v1.8.1...v1.8.2
 
 
-v1.8.1 / 2022-06-07
+1.8.1 / 2022-06-07
 -------------------
 Minor:
 * Change FDC z offset and add alternative interaction by @ftoschi in #1017
 * Plugin for online individual peak monitoring by @mflierm in #1054
 
 Notes:
 * Lineage changes for event_positions, corrected_areas, energy_estimates, event_info, event_info_double
@@ -211,15 +222,15 @@
 * Add kicp to query by @JoranAngevaare in #1052
 * Bump sphinx from 4.5.0 to 5.0.1 in /extra_requirements by @dependabot in #1051
 * Allow constant tuple options by @JoranAngevaare in #1039
 
 Full changelog:
 - https://github.com/XENONnT/straxen/compare/v1.7.1...v1.8.0
 
-v1.7.2 / 2022-07-18
+1.7.2 / 2022-07-18
 -------------------
 Patch:
  * Upload cherry picks by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1066
  * Fix hanging straxer by @jmosbacher in https://github.com/XENONnT/straxen/pull/1065
  * Stop tf pbar by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1063
  * update docs ev interactive display by @JoranAngevaare in #1042
  * allow dry eval of URL configs by @JoranAngevaare in #1040
@@ -229,15 +240,15 @@
  * Add kicp to query by @JoranAngevaare in #1052
  * Bump sphinx from 4.5.0 to 5.0.1 in /extra_requirements by @dependabot in #1051
  * Allow constant tuple options by @JoranAngevaare in #1039
 
 **Full Changelog**: https://github.com/XENONnT/straxen/compare/v1.7.1...v1.7.2
 
 
-v1.7.1 / 2022-05-16
+1.7.1 / 2022-05-16
 -------------------
 Patch:
 * Check if processed data already exists in --production mode by @mflierm in https://github.com/XENONnT/straxen/pull/1024
 
 
 Notes:
 - No lineage changes
@@ -245,15 +256,15 @@
 Full Changelog: 
  - https://github.com/XENONnT/straxen/compare/v1.7.0...v1.7.1
 
 New Contributors
  - @mflierm made their first contribution in https://github.com/XENONnT/straxen/pull/1024
 
 
-v1.7.0 / 2022-05-11
+1.7.0 / 2022-05-11
 ---------------------
 Minor:
 - Fix detector sync (#1033) 
 - Numbafy function (#1015) 
 - Fixing binomial (#991) 
 - Patched wrong setting (#1014) 
 - Partitioned tpc (#1027) 
@@ -270,15 +281,15 @@
 - Lineage changes for event_area_per_channel, event_pattern_fit, peak_classification_bayes, detector_time_offsets, event_sync_nv
 
 
 Full Changelog:
  - https://github.com/XENONnT/straxen/compare/v1.6.2...v1.7.0
 
 
-v1.6.2 / 2022-05-06
+1.6.2 / 2022-05-06
 ---------------------
 Patch:
 -  Add MV trigger channel to acqmon hits https://github.com/XENONnT/straxen/pull/1035
 
 Notes:
  - only lineage changes for dtypes > `aqmon_hits`  (https://github.com/XENONnT/straxen/pull/1035)
```

### Comparing `straxen-2.1.1/LICENSE` & `straxen-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/PKG-INFO` & `straxen-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: straxen
-Version: 2.1.1
+Version: 2.1.2
 Summary: Streaming analysis for XENON
 Home-page: https://github.com/XENONnT/straxen
 Author: Straxen contributors, the XENON collaboration
 License: UNKNOWN
 Description: # straxen
         Streaming analysis for XENON(nT)
         
@@ -25,26 +25,37 @@
         [![Python Versions](https://img.shields.io/pypi/pyversions/straxen.svg)](https://pypi.python.org/pypi/straxen)
         [![PyPI downloads](https://img.shields.io/pypi/dm/straxen.svg)](https://pypistats.org/packages/straxen)
         
         [![Update context collection](https://github.com/XENONnT/straxen/workflows/Update%20context%20collection/badge.svg)](https://github.com/XENONnT/straxen/actions/workflows/contexts.yml)
         [![Python style](https://github.com/XENONnT/straxen/actions/workflows/code_style.yml/badge.svg)](https://github.com/XENONnT/straxen/actions/workflows/code_style.yml)
         
         
-        v2.1.1 / 2023-07-06
+        2.1.2 / 2023-07-28
+        -------------------
+        * Validate final type after URL eval by @jmosbacher in https://github.com/XENONnT/straxen/pull/1217
+        * Fix URLConfig.evaluate_dry by @jmosbacher in https://github.com/XENONnT/straxen/pull/1219
+        * Add function to save itp_map InterpolatingMap related dictionary into pickle by @dachengx in https://github.com/XENONnT/straxen/pull/1221
+        * Rename `tf_peak_model_s1_cnn` to `tf_model_s1_cnn` by @dachengx in https://github.com/XENONnT/straxen/pull/1223
+        
+        
+        **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.1.1...v2.1.2
+        
+        
+        2.1.1 / 2023-07-06
         -------------------
         * Fix timing of peaks when ordering in `center_time` by @dachengx in https://github.com/XENONnT/straxen/pull/1208
         * Move `get_window_size` factor of merged_s2s as untracked configuration by @dachengx in https://github.com/XENONnT/straxen/pull/1209
         * Sort `hitlets` in `nVETOHitlets` by @dachengx in https://github.com/XENONnT/straxen/pull/1210
         * Only print out warning once by @LuisSanchez25 in https://github.com/XENONnT/straxen/pull/1211
         
         
         **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.1.0...v2.1.1
         
         
-        v2.1.0 / 2023-06-22
+        2.1.0 / 2023-06-22
         -------------------
         * Added peaks subtyping by @Jianyu010 in https://github.com/XENONnT/straxen/pull/1152
         * Fix ipython version by @dachengx in https://github.com/XENONnT/straxen/pull/1169
         * Fix bug in hitlets time ordering by @dachengx in https://github.com/XENONnT/straxen/pull/1173
         * Bump actions/setup-python from 4.5.0 to 4.6.0 by @dependabot in https://github.com/XENONnT/straxen/pull/1170
         * Save hits level information(hits height and time difference) in peak and event level by @dachengx in https://github.com/XENONnT/straxen/pull/1155
         * Fix argsort inside numba.jit using kind='mergesort' by @dachengx in https://github.com/XENONnT/straxen/pull/1176
@@ -67,15 +78,15 @@
         New Contributors
         * @PeterGy made their first contribution in https://github.com/XENONnT/straxen/pull/1202
         * @minzhong98 made their first contribution in https://github.com/XENONnT/straxen/pull/1191
         
         **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.7...v2.1.0
         
         
-        v2.0.7 / 2023-04-25
+        2.0.7 / 2023-04-25
         -------------------
         * Bootstrax target removal after failures by @cfuselli in https://github.com/XENONnT/straxen/pull/1145
         * reforming _raw_path and _processed_path by @FaroutYLq in https://github.com/XENONnT/straxen/pull/1149
         * Adding correction of Z position due to non-uniform drift velocity by @terliuk in https://github.com/XENONnT/straxen/pull/1148
         * Bump the versions of peaklets and quality check runs-on by @dachengx in https://github.com/XENONnT/straxen/pull/1153
         * S1-Based 3D Position Reconstruction by @matteoguida in https://github.com/XENONnT/straxen/pull/1146
         * Bump xedocs from 0.2.14 to 0.2.16 in /extra_requirements by @dependabot in https://github.com/XENONnT/straxen/pull/1158
@@ -86,79 +97,79 @@
         * @cfuselli made their first contribution in https://github.com/XENONnT/straxen/pull/1145
         * @matteoguida made their first contribution in https://github.com/XENONnT/straxen/pull/1146
         * @hmdyt made their first contribution in https://github.com/XENONnT/straxen/pull/1159
         
         **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.6...v2.0.7
         
         
-        v2.0.6 / 2023-03-08
+        2.0.6 / 2023-03-08
         -------------------
         * Bump supercharge/mongodb-github-action from 1.8.0 to 1.9.0 by @dependabot in https://github.com/XENONnT/straxen/pull/1140
         * Small patches to restrax module by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1143, d04a3428c52c159577b61af2a28ddd0af5652027, 602b807291211f083c8f54df6768b8198fbf6b55
         * Ms events by @michaweiss89 and @HenningSE in https://github.com/XENONnT/straxen/pull/1080
         
         New Contributors
         * @michaweiss89 made their first contribution in https://github.com/XENONnT/straxen/pull/1080
         
         **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.5...v2.0.6
         
         Notes:
          - new data types: `peaks_per_event`, `event_top_bottom_params`, `peaks_corrections` (see #1080)
         
         
-        v2.0.5 / 2023-02-24
+        2.0.5 / 2023-02-24
         -------------------
         * fix xedocs for testing by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1139
         * Restart python style guide by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1138
         * Decrease number of chunks by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1123
         * Restrax by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1074
         
         
         **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.4...v2.0.5
         
         
-        v2.0.4 / 2023-01-16
+        2.0.4 / 2023-01-16
         -------------------
         * Top and bottom timing parameters at event and peak level by @terliuk in https://github.com/XENONnT/straxen/pull/1119
         * Allow use of xedocs context configs by @jmosbacher in https://github.com/XENONnT/straxen/pull/1125
         * Bump actions/setup-python from 4.3.0 to 4.4.0 by @dependabot in https://github.com/XENONnT/straxen/pull/1128
         * Add entry points by @jmosbacher in https://github.com/XENONnT/straxen/pull/1120
         * URLConfig preprocessor by @jmosbacher in https://github.com/XENONnT/straxen/pull/1110
         * Fix bootstrax timeouts by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1133
         
         
         **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.3...v2.1.0
         
         Notes:
          - new data types: `peak_top_bottom_params`, `event_top_bottom_params`
         
-        v2.0.3 / 2022-11-09
+        2.0.3 / 2022-11-09
         -------------------
         * Adding peak waveforms at event level by @terliuk in https://github.com/XENONnT/straxen/pull/1112
         
         
         **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.2...v2.0.3
         
         Notes:
          * lineage changes for event_area_per_channel
         
         
-        v2.0.2 / 2022-10-24
+        2.0.2 / 2022-10-24
         -------------------
         * New URLConfig protocols - list-to-array and list-to-dict by @LuisSanchez25 in https://github.com/XENONnT/straxen/pull/1104
         * Single core 1T test by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1109
         
         New Contributors
         * @LuisSanchez25 made their first contribution in https://github.com/XENONnT/straxen/pull/1104
         
         
         **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.1...v2.0.2
         
         
-        v2.0.1 / 2022-10-20
+        2.0.1 / 2022-10-20
         -------------------
         * Use mongodb v4.4.1 when testing to match real version used in production by @jmosbacher in https://github.com/XENONnT/straxen/pull/1103
         * Pass tests from remote forks by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1105
         * Local minimum info 2 by @JYangQi00 in https://github.com/XENONnT/straxen/pull/1106
         * Don't test without `strax.processor.SHMExecutor` by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1107
         * Lower the default config value of online_max_bytes by @mflierm in https://github.com/XENONnT/straxen/pull/1108
         
@@ -166,15 +177,15 @@
         New Contributors
         * @JYangQi00 made their first contribution in https://github.com/XENONnT/straxen/pull/1106
         
         
         **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.0...v2.0.1
         
         
-        v2.0.0 / 2022-10-17
+        2.0.0 / 2022-10-17
         -------------------
         * Fix acqmon veto field by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1072
         * Use self.dtype also for empty peaks by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1058
         * Re Start style guide by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1084
         * Transition plugins to URLConfig by @jmosbacher in https://github.com/XENONnT/straxen/pull/1079
         * Fix help of peak basics. by @WenzDaniel in https://github.com/XENONnT/straxen/pull/1081
         * Remove `tight_coincidence_channel` fix #1078 by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1092
@@ -194,39 +205,39 @@
          * Changed signatures of plugins in [#1094](https://github.com/XENONnT/straxen/pull/1094)
          * New plugins for event level processing by [#1097](https://github.com/XENONnT/straxen/pull/1097)
         
         
         **Full Changelog**: https://github.com/XENONnT/straxen/compare/v1.8.3...v2.0.0
         
         
-        v1.8.3 / 2022-07-18
+        1.8.3 / 2022-07-18
         -------------------
         * Bootstrax file-check fix by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1064
         * Fix hanging straxer by @jmosbacher in https://github.com/XENONnT/straxen/pull/1065
         
         Notes:
         * No lineage changes
         
         Full Changelog:
          - https://github.com/XENONnT/straxen/compare/v1.8.2...v1.8.3
         
         
-        v1.8.2 / 2022-07-12
+        1.8.2 / 2022-07-12
         -------------------
         * Stop tf pbar by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1063
         * Allow long runs by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1062
         
         Notes:
         * No lineage changes
         
         Full Changelog:
         - https://github.com/XENONnT/straxen/compare/v1.8.1...v1.8.2
         
         
-        v1.8.1 / 2022-06-07
+        1.8.1 / 2022-06-07
         -------------------
         Minor:
         * Change FDC z offset and add alternative interaction by @ftoschi in #1017
         * Plugin for online individual peak monitoring by @mflierm in #1054
         
         Notes:
         * Lineage changes for event_positions, corrected_areas, energy_estimates, event_info, event_info_double
@@ -242,15 +253,15 @@
         * Add kicp to query by @JoranAngevaare in #1052
         * Bump sphinx from 4.5.0 to 5.0.1 in /extra_requirements by @dependabot in #1051
         * Allow constant tuple options by @JoranAngevaare in #1039
         
         Full changelog:
         - https://github.com/XENONnT/straxen/compare/v1.7.1...v1.8.0
         
-        v1.7.2 / 2022-07-18
+        1.7.2 / 2022-07-18
         -------------------
         Patch:
          * Upload cherry picks by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1066
          * Fix hanging straxer by @jmosbacher in https://github.com/XENONnT/straxen/pull/1065
          * Stop tf pbar by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1063
          * update docs ev interactive display by @JoranAngevaare in #1042
          * allow dry eval of URL configs by @JoranAngevaare in #1040
@@ -260,15 +271,15 @@
          * Add kicp to query by @JoranAngevaare in #1052
          * Bump sphinx from 4.5.0 to 5.0.1 in /extra_requirements by @dependabot in #1051
          * Allow constant tuple options by @JoranAngevaare in #1039
         
         **Full Changelog**: https://github.com/XENONnT/straxen/compare/v1.7.1...v1.7.2
         
         
-        v1.7.1 / 2022-05-16
+        1.7.1 / 2022-05-16
         -------------------
         Patch:
         * Check if processed data already exists in --production mode by @mflierm in https://github.com/XENONnT/straxen/pull/1024
         
         
         Notes:
         - No lineage changes
@@ -276,15 +287,15 @@
         Full Changelog: 
          - https://github.com/XENONnT/straxen/compare/v1.7.0...v1.7.1
         
         New Contributors
          - @mflierm made their first contribution in https://github.com/XENONnT/straxen/pull/1024
         
         
-        v1.7.0 / 2022-05-11
+        1.7.0 / 2022-05-11
         ---------------------
         Minor:
         - Fix detector sync (#1033) 
         - Numbafy function (#1015) 
         - Fixing binomial (#991) 
         - Patched wrong setting (#1014) 
         - Partitioned tpc (#1027) 
@@ -301,15 +312,15 @@
         - Lineage changes for event_area_per_channel, event_pattern_fit, peak_classification_bayes, detector_time_offsets, event_sync_nv
         
         
         Full Changelog:
          - https://github.com/XENONnT/straxen/compare/v1.6.2...v1.7.0
         
         
-        v1.6.2 / 2022-05-06
+        1.6.2 / 2022-05-06
         ---------------------
         Patch:
         -  Add MV trigger channel to acqmon hits https://github.com/XENONnT/straxen/pull/1035
         
         Notes:
          - only lineage changes for dtypes > `aqmon_hits`  (https://github.com/XENONnT/straxen/pull/1035)
```

### Comparing `straxen-2.1.1/README.md` & `straxen-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/bin/ajax` & `straxen-2.1.2/bin/ajax`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/bin/bootstrax` & `straxen-2.1.2/bin/bootstrax`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/bin/fake_daq` & `straxen-2.1.2/bin/fake_daq`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/bin/microstrax` & `straxen-2.1.2/bin/microstrax`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/bin/refresh_raw_records` & `straxen-2.1.2/bin/refresh_raw_records`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/bin/restrax` & `straxen-2.1.2/bin/restrax`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/bin/straxen-print_versions` & `straxen-2.1.2/bin/straxen-print_versions`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/bin/straxer` & `straxen-2.1.2/bin/straxer`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/setup.cfg` & `straxen-2.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/setup.py` & `straxen-2.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 with open('README.md') as file:
     readme = file.read()
 
 with open('HISTORY.md') as file:
     history = file.read()
 
 setuptools.setup(name='straxen',
-                 version='2.1.1',
+                 version='2.1.2',
                  description='Streaming analysis for XENON',
                  author='Straxen contributors, the XENON collaboration',
                  url='https://github.com/XENONnT/straxen',
                  long_description=readme + '\n\n' + history,
                  long_description_content_type="text/markdown",
                  setup_requires=['pytest-runner'],
                  install_requires=requires,
```

### Comparing `straxen-2.1.1/straxen/__init__.py` & `straxen-2.1.2/straxen/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '2.1.1'
+__version__ = '2.1.2'
 
 from utilix import uconfig
 from .common import *
 # contexts.py below
 from .corrections_services import *
 from .get_corrections import *
```

### Comparing `straxen-2.1.1/straxen/analyses/bokeh_waveform_plot.py` & `straxen-2.1.2/straxen/analyses/bokeh_waveform_plot.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/analyses/daq_waveforms.py` & `straxen-2.1.2/straxen/analyses/daq_waveforms.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/analyses/event_display.py` & `straxen-2.1.2/straxen/analyses/event_display.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/analyses/holoviews_waveform_display.py` & `straxen-2.1.2/straxen/analyses/holoviews_waveform_display.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/analyses/posrec_comparison.py` & `straxen-2.1.2/straxen/analyses/posrec_comparison.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/analyses/pulse_plots.py` & `straxen-2.1.2/straxen/analyses/pulse_plots.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/analyses/quick_checks.py` & `straxen-2.1.2/straxen/analyses/quick_checks.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/analyses/records_matrix.py` & `straxen-2.1.2/straxen/analyses/records_matrix.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/analyses/waveform_plot.py` & `straxen-2.1.2/straxen/analyses/waveform_plot.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/bokeh_utils.py` & `straxen-2.1.2/straxen/bokeh_utils.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/common.py` & `straxen-2.1.2/straxen/common.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/contexts.py` & `straxen-2.1.2/straxen/contexts.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/corrections_services.py` & `straxen-2.1.2/straxen/corrections_services.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/daq_core.py` & `straxen-2.1.2/straxen/daq_core.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/entry_points.py` & `straxen-2.1.2/straxen/entry_points.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/get_corrections.py` & `straxen-2.1.2/straxen/get_corrections.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/holoviews/holoviews_inspector.py` & `straxen-2.1.2/straxen/holoviews/holoviews_inspector.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/holoviews/holoviews_peak_data.py` & `straxen-2.1.2/straxen/holoviews/holoviews_peak_data.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/holoviews/holoviews_pmt_array.py` & `straxen-2.1.2/straxen/holoviews/holoviews_pmt_array.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/holoviews/holoviews_tpc_event_display.py` & `straxen-2.1.2/straxen/holoviews/holoviews_tpc_event_display.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/holoviews_utils.py` & `straxen-2.1.2/straxen/holoviews_utils.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/itp_map.py` & `straxen-2.1.2/straxen/itp_map.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,25 @@
-import logging
+import os
+import re
 import gzip
 import json
-import re
+import time
+import pickle
+import logging
+import warnings
+from typing import Type, List, Literal
+from textwrap import dedent
 
 import numpy as np
 from scipy.spatial import cKDTree
 from scipy.interpolate import RectBivariateSpline, RegularGridInterpolator
+
 import straxen
 import strax
+
 export, __all__ = strax.exporter()
 
 
 @export
 class InterpolateAndExtrapolate:
     """Linearly interpolate- and extrapolate using inverse-distance
     weighted averaging between nearby points.
@@ -46,16 +54,16 @@
         valid = (distances < float('inf')).max(axis=-1)
 
         values = self.values[indices[valid]]
         weights = 1 / np.clip(distances[valid], 1e-6, float('inf'))
         if self.array_valued:
             weights = np.repeat(weights, self.n_dim).reshape(values.shape)
 
-        result[valid] = np.average(values, weights=weights,
-                                   axis=-2 if self.array_valued else -1)
+        result[valid] = np.average(
+            values, weights=weights, axis=-2 if self.array_valued else -1)
         return result
 
 
 @export
 class InterpolatingMap:
     """Correction map that computes values using inverse-weighted distance
     interpolation.
@@ -129,23 +137,24 @@
             self.dimensions = len(grid)
         else:
             csys = np.array(csys)
             self.dimensions = len(csys[0])
 
         self.coordinate_system = csys
         self.interpolators = {}
-        self.map_names = sorted([k for k in self.data.keys()
-                                 if k not in self.metadata_field_names])
+        self.map_names = sorted([
+            k for k in self.data.keys()
+            if k not in self.metadata_field_names])
 
         log = logging.getLogger('InterpolatingMap')
-        log.debug('Map name: %s' % self.data.get('name',
-                                                 "NO NAME?!"))
-        log.debug('Map description:\n    ' +
-                  re.sub(r'\n', r'\n    ', self.data.get('description',
-                                                         "NO DESCRIPTION?!")))
+        log.debug(
+            'Map name: %s' % self.data.get('name', "NO NAME?!"))
+        log.debug(
+            'Map description:\n    ' +
+            re.sub(r'\n', r'\n    ', self.data.get('description', "NO DESCRIPTION?!")))
         log.debug("Map names found: %s" % self.map_names)
 
         for map_name in self.map_names:
             # Specify dtype float to set Nones to nan
             map_data = np.array(self.data[map_name], dtype=np.float64)
             if len(self.coordinate_system) == len(map_data):
                 array_valued = len(map_data.shape) == 2
@@ -245,11 +254,98 @@
         map_data = np.array(self.data[map_name])
         if len(self.coordinate_system) == len(map_data):
             array_valued = len(map_data.shape) == 2
         else:
             array_valued = len(map_data.shape) == self.dimensions + 1
         if array_valued:
             map_data = map_data.reshape((-1, map_data.shape[-1]))
-        itp_fun = InterpolateAndExtrapolate(points=np.array(alt_csys),
-                                            values=np.array(map_data),
-                                            array_valued=array_valued)
+        itp_fun = InterpolateAndExtrapolate(
+            points=np.array(alt_csys),
+            values=np.array(map_data),
+            array_valued=array_valued)
         self.interpolators[map_name] = itp_fun
+
+
+@export
+def save_interpolation_formatted_map(
+        itp_map,
+        coordinate_system: List,
+        filename: str,
+        map_name: str = None,
+        quantum: float = None,
+        quantum_dtype = np.int16,
+        map_description: str = '',
+        compressor: Literal['bz2', 'zstd', 'blosc', 'lz4'] = 'zstd',
+    ):
+    """
+    Make a straxen-style InterpolatingMap.
+    To fit the large XENONnT per-PMT maps into strax_auxiliary files,
+    quantized them to values of 1e-5,
+    and store the maps as 16-bit integer multiples of 1e-5, instead of 64-bit floats.
+    :param itp_map: numpy itp_map or list of floats,
+    should follow the shape indicated by coordinate_system
+    :param coordinate_system: coordinate system of the itp_map,
+    list of [['x', [x_min, x_max, n_x]], [['y', [y_min, y_max, n_y], ...] for each dimension,
+    or [[x1, y1], [x2, y2], [x3, y3], [x4, y4], ...]
+    :param filename: filename with '.pkl' extension
+    :param map_name: name of map
+    :param quantum: quantum of the map if quantized
+    :param map_description: map's description
+    :param compressor: key of compressor in strax.io.COMPRESSORS
+    """
+    if isinstance(itp_map, list):
+        itp_map = np.array(itp_map)
+
+    if isinstance(coordinate_system[0][0], str):
+        itp_map_shape = list(itp_map.shape)
+        coordinate_shape = [c[1][2] for c in coordinate_system]
+        mask = (len(itp_map_shape) == len(coordinate_shape))
+        mask &= all([hs == cs for hs, cs in zip(itp_map_shape, coordinate_shape)])
+    else:
+        itp_map_shape = len(itp_map)
+        coordinate_shape = len(coordinate_system)
+        mask = (itp_map_shape == coordinate_shape)
+    if not mask:
+        raise ValueError(
+            f"The shape of itp_map: {itp_map_shape} and "
+            f"coordinate system: {coordinate_shape} do not match")
+
+    if quantum is None:
+        # if quantum is not specified, just use float32
+        q = 1
+        quantum_dtype = np.float32
+        map = itp_map.astype(quantum_dtype)
+    else:
+        q = quantum
+        if not np.issubdtype(quantum_dtype, np.integer):
+            raise ValueError(
+                "If using quantization, quantum_dtype must be an integer type,"
+                f" but it is now {quantum_dtype}")
+        encode_until = np.iinfo(quantum_dtype).max * q
+        if itp_map.max() > encode_until:
+            raise ValueError(
+                f"Map maximum value is {itp_map.max():.4f},"
+                " can encode values until {encode_until:.4f}")
+        map = np.round(itp_map / q).astype(quantum_dtype)
+
+    output = dict(
+        coordinate_system=coordinate_system,
+        map=strax.io.COMPRESSORS[compressor]['compress'](map),
+        description=dedent(map_description),
+        timestamp=time.time(),
+        compressed=(compressor, quantum_dtype, map.shape),
+    )
+    if quantum is not None:
+        output['quantized'] = q
+    if map_name is not None:
+        output['name'] = map_name
+
+    if 'pkl' not in filename:
+        warnings.warn("Better use .pkl or .pkl.gz extension for map files")
+    splitext = os.path.splitext(filename)
+    if splitext[-1] == '.gz':
+        opener = gzip.open
+    else:
+        opener = open
+    with opener(filename, mode='wb') as f:
+        pickle.dump(output, f)
+    print(f"Wrote new map file {filename}, {os.path.getsize(filename) / 1e6:.2f} MB")
```

### Comparing `straxen-2.1.1/straxen/legacy/contexts_1t.py` & `straxen-2.1.2/straxen/legacy/contexts_1t.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/legacy/hitfinder_thresholds.py` & `straxen-2.1.2/straxen/legacy/hitfinder_thresholds.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/legacy/plugins_1t/event_info.py` & `straxen-2.1.2/straxen/legacy/plugins_1t/event_info.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/legacy/plugins_1t/pax_interface.py` & `straxen-2.1.2/straxen/legacy/plugins_1t/pax_interface.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/legacy/plugins_1t/peak_positions.py` & `straxen-2.1.2/straxen/legacy/plugins_1t/peak_positions.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/legacy/plugins_1t/x1t_cuts.py` & `straxen-2.1.2/straxen/legacy/plugins_1t/x1t_cuts.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/legacy/xenon1t_url_configs.py` & `straxen-2.1.2/straxen/legacy/xenon1t_url_configs.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/matplotlib_utils.py` & `straxen-2.1.2/straxen/matplotlib_utils.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/mini_analysis.py` & `straxen-2.1.2/straxen/mini_analysis.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/misc.py` & `straxen-2.1.2/straxen/misc.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/numbafied_scipy.py` & `straxen-2.1.2/straxen/numbafied_scipy.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/__init__.py` & `straxen-2.1.2/straxen/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/afterpulses/afterpulse_processing.py` & `straxen-2.1.2/straxen/plugins/afterpulses/afterpulse_processing.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/aqmon_hits/aqmon_hits.py` & `straxen-2.1.2/straxen/plugins/aqmon_hits/aqmon_hits.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/defaults.py` & `straxen-2.1.2/straxen/plugins/defaults.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/detector_time_offsets/detector_time_offsets.py` & `straxen-2.1.2/straxen/plugins/detector_time_offsets/detector_time_offsets.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events/__init__.py` & `straxen-2.1.2/straxen/plugins/events/__init__.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events/_event_s1_positions_base.py` & `straxen-2.1.2/straxen/plugins/events/_event_s1_positions_base.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events/_event_s2_positions_base.py` & `straxen-2.1.2/straxen/plugins/events/_event_s2_positions_base.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events/corrected_areas.py` & `straxen-2.1.2/straxen/plugins/events/corrected_areas.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events/distinct_channels.py` & `straxen-2.1.2/straxen/plugins/events/distinct_channels.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events/energy_estimates.py` & `straxen-2.1.2/straxen/plugins/events/energy_estimates.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events/event_ambience.py` & `straxen-2.1.2/straxen/plugins/events/event_ambience.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events/event_area_per_channel.py` & `straxen-2.1.2/straxen/plugins/events/event_area_per_channel.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events/event_basics.py` & `straxen-2.1.2/straxen/plugins/events/event_basics.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events/event_info.py` & `straxen-2.1.2/straxen/plugins/events/event_info.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events/event_info_double.py` & `straxen-2.1.2/straxen/plugins/events/event_info_double.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events/event_pattern_fit.py` & `straxen-2.1.2/straxen/plugins/events/event_pattern_fit.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events/event_positions.py` & `straxen-2.1.2/straxen/plugins/events/event_positions.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events/event_s1_positions_cnn.py` & `straxen-2.1.2/straxen/plugins/events/event_s1_positions_cnn.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events/event_s2_positions_cnn.py` & `straxen-2.1.2/straxen/plugins/events/event_s2_positions_cnn.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events/event_s2_positions_gcn.py` & `straxen-2.1.2/straxen/plugins/events/event_s2_positions_gcn.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events/event_s2_positions_mlp.py` & `straxen-2.1.2/straxen/plugins/events/event_s2_positions_mlp.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events/event_shadow.py` & `straxen-2.1.2/straxen/plugins/events/event_shadow.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events/event_top_bottom_params.py` & `straxen-2.1.2/straxen/plugins/events/event_top_bottom_params.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events/event_w_bayes_class.py` & `straxen-2.1.2/straxen/plugins/events/event_w_bayes_class.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events/event_waveform.py` & `straxen-2.1.2/straxen/plugins/events/event_waveform.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events/events.py` & `straxen-2.1.2/straxen/plugins/events/events.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events/local_minimum_info.py` & `straxen-2.1.2/straxen/plugins/events/local_minimum_info.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events/multi_scatter.py` & `straxen-2.1.2/straxen/plugins/events/multi_scatter.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events/s2_recon_pos_diff.py` & `straxen-2.1.2/straxen/plugins/events/s2_recon_pos_diff.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events/veto_proximity.py` & `straxen-2.1.2/straxen/plugins/events/veto_proximity.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events_mv/events_mv.py` & `straxen-2.1.2/straxen/plugins/events_mv/events_mv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events_mv/events_sync_mv.py` & `straxen-2.1.2/straxen/plugins/events_mv/events_sync_mv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events_nv/event_positions_nv.py` & `straxen-2.1.2/straxen/plugins/events_nv/event_positions_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events_nv/events_nv.py` & `straxen-2.1.2/straxen/plugins/events_nv/events_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/events_nv/events_sync_nv.py` & `straxen-2.1.2/straxen/plugins/events_nv/events_sync_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/hitlets_mv/hitlets_mv.py` & `straxen-2.1.2/straxen/plugins/hitlets_mv/hitlets_mv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/hitlets_nv/hitlets_nv.py` & `straxen-2.1.2/straxen/plugins/hitlets_nv/hitlets_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/individual_peak_monitor/individual_peak_monitor.py` & `straxen-2.1.2/straxen/plugins/individual_peak_monitor/individual_peak_monitor.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/led_cal/led_calibration.py` & `straxen-2.1.2/straxen/plugins/led_cal/led_calibration.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/merged_s2s/merged_s2s.py` & `straxen-2.1.2/straxen/plugins/merged_s2s/merged_s2s.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/merged_s2s_he/merged_s2s_he.py` & `straxen-2.1.2/straxen/plugins/merged_s2s_he/merged_s2s_he.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/online_monitor_mv/online_monitor_mv.py` & `straxen-2.1.2/straxen/plugins/online_monitor_mv/online_monitor_mv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/online_monitor_nv/online_monitor_nv.py` & `straxen-2.1.2/straxen/plugins/online_monitor_nv/online_monitor_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/online_peak_monitor/online_peak_monitor.py` & `straxen-2.1.2/straxen/plugins/online_peak_monitor/online_peak_monitor.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/peaklets/peaklet_classification.py` & `straxen-2.1.2/straxen/plugins/peaklets/peaklet_classification.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/peaklets/peaklets.py` & `straxen-2.1.2/straxen/plugins/peaklets/peaklets.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/peaklets_he/peaklet_classification_he.py` & `straxen-2.1.2/straxen/plugins/peaklets_he/peaklet_classification_he.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/peaklets_he/peaklets_he.py` & `straxen-2.1.2/straxen/plugins/peaklets_he/peaklets_he.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/peaks/__init__.py` & `straxen-2.1.2/straxen/plugins/peaks/__init__.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/peaks/_peak_positions_base.py` & `straxen-2.1.2/straxen/plugins/peaks/_peak_positions_base.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/peaks/_peak_s1_positions_base.py` & `straxen-2.1.2/straxen/plugins/peaks/_peak_s1_positions_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,18 +44,18 @@
                   ]
 
         dtype += strax.time_fields
         return dtype
     
     def get_tf_model(self):
         """
-        Simple wrapper to have several tf_peak_model_s1_cnn, ..
+        Simple wrapper to have several tf_model_s1_cnn, ..
         point to this same function in the compute method
         """
-        model = getattr(self, f'tf_peak_model_{self.algorithm}', None)
+        model = getattr(self, f'tf_model_{self.algorithm}', None)
         if model is None:
             warn(f'Setting model to None for {self.__class__.__name__} will '
                  f'set only nans as output for {self.algorithm}')
         if isinstance(model, str):
             raise ValueError(f'open files from tf:// protocol! Got {model} '
                              f'instead, see tests/test_s1_posrec.py for examples.')
         return model
```

### Comparing `straxen-2.1.1/straxen/plugins/peaks/peak_ambience.py` & `straxen-2.1.2/straxen/plugins/peaks/peak_ambience.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/peaks/peak_basics.py` & `straxen-2.1.2/straxen/plugins/peaks/peak_basics.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/peaks/peak_classification_bayes.py` & `straxen-2.1.2/straxen/plugins/peaks/peak_classification_bayes.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/peaks/peak_corrections.py` & `straxen-2.1.2/straxen/plugins/peaks/peak_corrections.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/peaks/peak_per_event.py` & `straxen-2.1.2/straxen/plugins/peaks/peak_per_event.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/peaks/peak_positions.py` & `straxen-2.1.2/straxen/plugins/peaks/peak_positions.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/peaks/peak_positions_cnn.py` & `straxen-2.1.2/straxen/plugins/peaks/peak_positions_cnn.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/peaks/peak_positions_gcn.py` & `straxen-2.1.2/straxen/plugins/peaks/peak_positions_gcn.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/peaks/peak_positions_mlp.py` & `straxen-2.1.2/straxen/plugins/peaks/peak_positions_mlp.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/peaks/peak_proximity.py` & `straxen-2.1.2/straxen/plugins/peaks/peak_proximity.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/peaks/peak_s1_positions_cnn.py` & `straxen-2.1.2/straxen/plugins/peaks/peak_s1_positions_cnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     """
     S1 CNN for (x,y,z) position S1 reconstruction at peak level
     """
     provides = "peak_s1_positions_cnn"
     algorithm = "s1_cnn"
     __version__ = '0.0.1'
 
-    tf_peak_model_s1_cnn = straxen.URLConfig(
+    tf_model_s1_cnn = straxen.URLConfig(
         default=f'tf://'
                 f'resource://'
                 f'xedocs://posrec_models'
                 f'?version=ONLINE'
                 f'&run_id=plugin.run_id'
                 f'&kind=s1_cnn'
                 f'&fmt=abs_path'
```

### Comparing `straxen-2.1.1/straxen/plugins/peaks/peak_shadow.py` & `straxen-2.1.2/straxen/plugins/peaks/peak_shadow.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/peaks/peak_top_bottom_params.py` & `straxen-2.1.2/straxen/plugins/peaks/peak_top_bottom_params.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/peaks/peaks.py` & `straxen-2.1.2/straxen/plugins/peaks/peaks.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/peaks/peaks_subtyping.py` & `straxen-2.1.2/straxen/plugins/peaks/peaks_subtyping.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/peaks_he/peaks_he.py` & `straxen-2.1.2/straxen/plugins/peaks_he/peaks_he.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/raw_records/daqreader.py` & `straxen-2.1.2/straxen/plugins/raw_records/daqreader.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/raw_records_coin_nv/nveto_recorder.py` & `straxen-2.1.2/straxen/plugins/raw_records_coin_nv/nveto_recorder.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/records/records.py` & `straxen-2.1.2/straxen/plugins/records/records.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/records_he/records_he.py` & `straxen-2.1.2/straxen/plugins/records_he/records_he.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/records_mv/records_mv.py` & `straxen-2.1.2/straxen/plugins/records_mv/records_mv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/records_nv/records_nv.py` & `straxen-2.1.2/straxen/plugins/records_nv/records_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/plugins/veto_intervals/veto_intervals.py` & `straxen-2.1.2/straxen/plugins/veto_intervals/veto_intervals.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/scada.py` & `straxen-2.1.2/straxen/scada.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/storage/mongo_storage.py` & `straxen-2.1.2/straxen/storage/mongo_storage.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/storage/online_monitor_frontend.py` & `straxen-2.1.2/straxen/storage/online_monitor_frontend.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/storage/rucio_local.py` & `straxen-2.1.2/straxen/storage/rucio_local.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/storage/rucio_remote.py` & `straxen-2.1.2/straxen/storage/rucio_remote.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/storage/rundb.py` & `straxen-2.1.2/straxen/storage/rundb.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/test_utils.py` & `straxen-2.1.2/straxen/test_utils.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/units.py` & `straxen-2.1.2/straxen/units.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/straxen/url_config.py` & `straxen-2.1.2/straxen/url_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 from ast import literal_eval
 from strax.config import OMITTED
 from utilix import xent_collection
 from scipy.interpolate import interp1d
 from straxen.misc import filter_kwargs
 from typing import Container, Mapping, Union, Iterable
 
+from pydantic.validators import find_validators
+from pydantic.config import get_config
+from pydantic.errors import PydanticTypeError
+
 export, __all__ = strax.exporter()
 
 _CACHES = {}
 
 WARN = True
 
 
@@ -35,22 +39,22 @@
 def clear_config_caches():
     for cache in _CACHES.values():
         cache.clear()
 
 
 @export
 def config_cache_size_mb():
-    return straxen.total_size(_CACHES)//1e6
+    return straxen.total_size(_CACHES) // 1e6
 
 
 def parse_val(val: str):
-    '''Attempt to parse a string value as
+    """Attempt to parse a string value as
     a python literal, falls back to returning just
     the original string if cant be parsed.
-    '''
+    """
     try:
         val = literal_eval(val)
     except ValueError:
         pass
     except SyntaxError:
         pass
     return val
@@ -64,116 +68,116 @@
 
 @export
 class URLConfig(strax.Config):
     """Dispatch on URL protocol.
     unrecognized protocol returns identity
     inspired by dasks Dispatch and fsspec fs protocols.
     """
+
     _LOOKUP = {}
     _PREPROCESSORS = ()
 
-    SCHEME_SEP = '://'
-    QUERY_SEP = '?'
-    NAMESPACE_SEP = '.'
-    PLUGIN_ATTR_PREFIX = 'plugin.'
+    SCHEME_SEP = "://"
+    QUERY_SEP = "?"
+    NAMESPACE_SEP = "."
+    PLUGIN_ATTR_PREFIX = "plugin."
 
     def __init__(self, cache=0, **kwargs):
         """
-        :param cache: number of values to keep in cache, 
+        :param cache: number of values to keep in cache,
                       if set to True will cache all values
         :param **kwargs: additional keyword arguments accepted by strax.Option
         """
         self.final_type = OMITTED
         super().__init__(**kwargs)
         # Ensure backwards compatibility with Option validation
         # type of the config value can be different from the fetched value.
         if self.type is not OMITTED:
             self.final_type = self.type
             self.type = OMITTED  # do not enforce type on the URL
         if cache:
-            cache_len = 100 if cache is True else int(cache) 
+            cache_len = 100 if cache is True else int(cache)
             cache = straxen.CacheDict(cache_len=cache_len)
             _CACHES[id(self)] = cache
 
     @property
     def cache(self):
         return _CACHES.get(id(self), {})
 
     @classmethod
     def register(cls, protocol, func=None):
         """Register dispatch of `func` on urls
-        starting with protocol name `protocol` """
+        starting with protocol name `protocol`"""
 
         def wrapper(func):
             if isinstance(protocol, tuple):
                 for t in protocol:
                     cls.register(t, func)
                 return func
 
             if not isinstance(protocol, str):
-                raise ValueError('Protocol name must be a string.')
+                raise ValueError("Protocol name must be a string.")
 
             if protocol in cls._LOOKUP:
-                raise ValueError(f'Protocol with name {protocol} already registered.')
+                raise ValueError(f"Protocol with name {protocol} already registered.")
             cls._LOOKUP[protocol] = func
             return func
+
         return wrapper(func) if func is not None else wrapper
 
     @classmethod
     def preprocessor(cls, func=None, precedence=0):
-        '''Register a new processor to modify the config values
+        """Register a new processor to modify the config values
         before they are used.
-        '''
+        """
+
         def wrapper(func):
             entry = (precedence, func)
             if entry in cls._PREPROCESSORS:
-                raise ValueError(f'This processor is already registered.')
-            cls._PREPROCESSORS += (entry, )
+                raise ValueError(f"This processor is already registered.")
+            cls._PREPROCESSORS += (entry,)
             return func
+
         return wrapper(func) if func is not None else wrapper
 
     @classmethod
-    def eval(cls, protocol: str,
-                  arg: Union[str,tuple] = None,
-                  kwargs: dict = None):
-        '''Evaluate a URL/AST by recusively dispatching protocols by name 
+    def eval(cls, protocol: str, arg: Union[str, tuple] = None, kwargs: dict = None):
+        """Evaluate a URL/AST by recusively dispatching protocols by name
             with argument arg and keyword arguments kwargs
            and return the value. If protocol does not exist, returnes arg
         :param protocol: name of the protocol or a URL
         :param arg: argument to pass to protocol, can be another (sub-protocol,
             arg, kwargs) tuple, in which case sub-protocol will be evaluated
             and passed to protocol
         :param kwargs: keyword arguments to be passed to the protocol
         :return: (Any) The return value of the protocol on these arguments
-        '''
-        
+        """
 
         if protocol is not None and arg is None:
             protocol, arg, kwargs = cls.url_to_ast(protocol)
 
         if protocol is None:
             return arg
 
         if kwargs is None:
             kwargs = {}
 
         meth = cls._LOOKUP[protocol]
 
         if isinstance(arg, tuple):
             arg = cls.eval(*arg)
-        
+
         # Just to be on the safe side
         kwargs = straxen.filter_kwargs(meth, kwargs)
 
         return meth(arg, **kwargs)
 
     @classmethod
     def split_url_kwargs(cls, url):
-        """split a url into path and kwargs
-        """
+        """split a url into path and kwargs"""
         path, _, _ = url.partition(cls.QUERY_SEP)
         kwargs = {}
         for k, v in parse_qs(urlparse(url).query).items():
             # values of query arguments are evaluated as lists
             # split logic depending on length
             n = len(v)
             if not n:
@@ -184,189 +188,225 @@
                 kwargs[k] = list(map(parse_val, v))
         return path, kwargs
 
     @classmethod
     def kwarg_from_url(cls, url: str, key: str):
         path, kwargs = cls.split_url_kwargs(url)
         return kwargs.get(key, None)
-        
+
     @classmethod
     def format_url_kwargs(cls, url, **kwargs):
-        '''Add keyword arguments to a URL.
+        """Add keyword arguments to a URL.
         Sorts all arguments by key for hash consistency
-        '''
+        """
         url, extra_kwargs = cls.split_url_kwargs(url)
         kwargs = dict(extra_kwargs, **kwargs)
         arg_list = []
         for k, v in sorted(kwargs.items()):
             if isinstance(v, list):
                 # lists are passed as multiple arguments with the same key
                 arg_list.extend([f"{k}={vi}" for vi in v])
             else:
                 arg_list.append(f"{k}={v}")
         arg_str = "&".join(arg_list)
-        arg_str = cls.QUERY_SEP + arg_str if arg_str else ''
+        arg_str = cls.QUERY_SEP + arg_str if arg_str else ""
         return url + arg_str
 
     @classmethod
     def lookup_value(cls, value, **namespace):
-        '''Optionally fetch an attribute from namespace
+        """Optionally fetch an attribute from namespace
         if value is a string with cls.NAMESPACE_SEP in
         it, the string is split and the first part is used
         to lookup an object in namespace and the second part
         is used to lookup the value in the object.
         If the value is not a string or the target object is
         not in the namesapce, the value is returned as is.
-        '''
+        """
 
         if isinstance(value, list):
             return [cls.lookup_value(v, **namespace) for v in value]
 
         if isinstance(value, str) and cls.NAMESPACE_SEP in value:
             name, _, key = value.partition(cls.NAMESPACE_SEP)
             if name in namespace:
                 obj = namespace[name]
                 if isinstance(obj, Mapping):
                     value = obj.get(key, value)
                 else:
                     value = getattr(obj, key, value)
-                
+
         return value
 
     @classmethod
     def deref_ast(cls, protocol, arg, kwargs, **namespace):
-        '''Dereference an AST by looking up values in namespace
-        '''
+        """Dereference an AST by looking up values in namespace"""
         if isinstance(arg, tuple):
             arg = cls.deref_ast(*arg, **namespace)
         else:
             arg = cls.lookup_value(arg, **namespace)
         kwargs = {k: cls.lookup_value(v, **namespace) for k, v in kwargs.items()}
         return protocol, arg, kwargs
 
-    def validate(self, config,
-                 run_id=None,   # TODO: will soon be removed
-                 run_defaults=None, set_defaults=True):
+    def validate(
+        self,
+        config,
+        run_id=None,  # TODO: will soon be removed
+        run_defaults=None,
+        set_defaults=True,
+    ):
         """This method is called by the context on plugin initialization
         at this stage, the run_id and context config are already known but the
         config values are not yet set on the plugin. Therefore its the perfect
         place to run any preprocessors on the config values to make any needed
         changes before the configs are hashed.
         """
         super().validate(config, run_id, run_defaults, set_defaults)
 
         cfg = config[self.name]
 
-        sorted_preprocessors = reversed(sorted(self._PREPROCESSORS,
-                                               key=lambda x: x[0]))
+        sorted_preprocessors = reversed(sorted(self._PREPROCESSORS, key=lambda x: x[0]))
 
-        full_kwargs = dict(name=self.name, 
-                           run_id=run_id, 
-                           run_defaults=run_defaults, 
-                           set_defaults=set_defaults)
+        full_kwargs = dict(
+            name=self.name,
+            run_id=run_id,
+            run_defaults=run_defaults,
+            set_defaults=set_defaults,
+        )
 
         for _, preprocessor in sorted_preprocessors:
             kwargs = filter_kwargs(preprocessor, full_kwargs)
             new_cfg = preprocessor(cfg, **kwargs)
             cfg = new_cfg if new_cfg is not None else cfg
-        
+
         config[self.name] = cfg
 
         if not isinstance(cfg, str) or self.SCHEME_SEP not in cfg:
             # if the value is not a url config it is validated against
             # its intended type (final_type)
-            if self.final_type is not OMITTED and not isinstance(cfg, self.final_type):
-                # TODO replace back with InvalidConfiguration
-                UserWarning(
-                    f"Invalid type for option {self.name}. "
-                    f"Excepted a {self.final_type}, got a {type(cfg)}")
+            self.validate_type(cfg)
+
+    def validate_type(self, value):
+        """Validate the type of a value against its intended type"""
+        msg = (
+            f"Invalid type for option {self.name}. "
+            f"Expected a {self.final_type} instance, got {type(value)}"
+            )
+        
+        if self.final_type is not OMITTED:
+            # Use pydantic to validate the type
+            # its validation is more flexible than isinstance
+            # it will coerce standard equivalent types
+            cfg = get_config(dict(arbitrary_types_allowed=True))
+            if isinstance(self.final_type, tuple):
+                validators = [ v for t in self.final_type for v in find_validators(t, config=cfg)]
+            else:
+                validators = find_validators(self.final_type, config=cfg)
+            for validator in validators:
+                try:
+                    validator(value)
+                    break
+                except:
+                    pass
+            else:
+                raise TypeError(msg)
+    
+        return value
 
     def fetch(self, plugin):
         """override the Config.fetch method
-           this is called when the attribute is accessed
-           from withing the Plugin instance
+        this is called when the attribute is accessed
+        from withing the Plugin instance
         """
         # first fetch the user-set value
 
         # from the config dictionary
         url = super().fetch(plugin)
 
         if not isinstance(url, str):
             # if the value is not a string it is evaluated
             # as a literal config and returned as is.
-            return url
+            return self.validate_type(url)
 
         if self.SCHEME_SEP not in url:
             # no protocol in the url so its evaluated
             # as string-literal config and returned as is
-            return url
+            return self.validate_type(url)
 
         # evaluate the url as AST
         protocol, arg, kwargs = self.url_to_ast(url)
 
+        # allow run_id to be missing
+        run_id = getattr(plugin, "run_id", "000000")
+
         # construct a deterministic hash key from AST
-        key = strax.deterministic_hash((protocol, arg, kwargs))
+        key = strax.deterministic_hash(
+            (plugin.config, run_id, protocol, arg, kwargs)
+        )
 
         # fetch from cache if exists
         value = self.cache.get(key, None)
 
         # not in cache, lets fetch it
         if value is None:
             # resolve any referenced to plugin or config attributes
-            protocol, arg, kwargs = self.deref_ast(protocol, arg, kwargs,
-                                                config=plugin.config, 
-                                                plugin=plugin)
-                                                
+            protocol, arg, kwargs = self.deref_ast(
+                protocol, arg, kwargs, config=plugin.config, plugin=plugin
+            )
+
             value = self.eval(protocol, arg, kwargs)
+            value = self.validate_type(value)
             self.cache[key] = value
 
         return value
-        
+
     @classmethod
-    def ast_to_url(cls,
-                   protocol: Union[str, tuple],
-                   arg: Union[str, tuple] = None,
-                   kwargs: dict = None):
-        """Convert a protocol abstract syntax tree to a valid URL 
-        """
+    def ast_to_url(
+        cls,
+        protocol: Union[str, tuple],
+        arg: Union[str, tuple] = None,
+        kwargs: dict = None,
+    ):
+        """Convert a protocol abstract syntax tree to a valid URL"""
 
         if isinstance(protocol, tuple):
             protocol, arg, kwargs = protocol
 
         if kwargs is None:
             kwargs = {}
 
         if protocol is None:
             return arg
-        
-        if isinstance(arg, (list, dict, numbers.Number)) and protocol != 'json':
-            arg = ('json', json.dumps(arg),)
+
+        if isinstance(arg, (list, dict, numbers.Number)) and protocol != "json":
+            arg = (
+                "json",
+                json.dumps(arg),
+            )
 
         if isinstance(arg, tuple):
             arg = cls.ast_to_url(*arg)
 
         if not isinstance(arg, str):
             raise TypeError(f"Type {type(arg)} is not supported as an argument.")
 
         arg, extra_kwargs = cls.split_url_kwargs(arg)
 
         kwargs.update(extra_kwargs)
-        
-        url = f'{protocol}{cls.SCHEME_SEP}{arg}'
-        
+
+        url = f"{protocol}{cls.SCHEME_SEP}{arg}"
+
         url = cls.format_url_kwargs(url, **kwargs)
 
         return url
 
     @classmethod
     def url_to_ast(cls, url, **kwargs):
-        """Convert a URL to a protocol abstract syntax tree
-        """
+        """Convert a URL to a protocol abstract syntax tree"""
         if not isinstance(url, str):
-            raise TypeError(f'URL must be a string, got {type(url)}')
+            raise TypeError(f"URL must be a string, got {type(url)}")
 
         if cls.SCHEME_SEP not in url:
             # no protocol in the url so its evaluated
             # as string-literal config and returned as is
             return None, url, {}
 
         # separate the protocol name from the path
@@ -374,94 +414,92 @@
 
         # find the corresponding protocol method
         meth = cls._LOOKUP.get(protocol, None)
         if meth is None:
             # unrecognized protocol
             # evaluate as string-literal
             return None, url, {}
-        
+
         arg, url_kwargs = cls.split_url_kwargs(path)
         kwargs.update(url_kwargs)
 
-
         if cls.SCHEME_SEP in arg:
             # url contains a nested protocol
             # first parsce sub-protocol
             arg = cls.url_to_ast(arg, **kwargs)
 
         # Filter unused kwargs for this method.
         # This is done also at the eval level but
         # probably better to be safe.
         kwargs = straxen.filter_kwargs(meth, kwargs)
-        
+
         # Always sort kwargs for consistent ASTs
         kwargs = dict(sorted(kwargs.items()))
 
         return protocol, arg, kwargs
 
     @classmethod
     def are_equal(cls, first, second):
-        """Return whether two URLs are equivalent (have equal ASTs)
-        """
+        """Return whether two URLs are equivalent (have equal ASTs)"""
         return cls.url_to_ast(first) == cls.url_to_ast(second)
 
     @classmethod
     def protocol_descr(cls):
         rows = []
         for k, v in cls._LOOKUP.items():
             descr = v.__doc__
             if descr is not None:
-                descr = descr.split('\n')[0]
+                descr = descr.split("\n")[0]
 
             row = {
-                'name': f"{k}://",
-                'description': descr, 
-                'signature': str(inspect.signature(v)),
-                'location': v.__module__,
+                "name": f"{k}://",
+                "description": descr,
+                "signature": str(inspect.signature(v)),
+                "location": v.__module__,
             }
             rows.append(row)
         return pd.DataFrame(rows)
 
     @classmethod
     def print_protocols(cls):
         df = cls.protocol_descr()
         if len(df):
             print(df)
         else:
-            print('No protocols registered.')
+            print("No protocols registered.")
 
     @classmethod
     def preprocessor_descr(cls):
         rows = []
-        for k,v in cls._PREPROCESSORS:
+        for k, v in cls._PREPROCESSORS:
             descr = v.__doc__
             if descr is not None:
-                descr = descr.split('\n')[0]
+                descr = descr.split("\n")[0]
             row = {
-                'precedence': k,
-                'description': descr,
-                'signature': str(inspect.signature(v)),
-                'location': v.__module__,
+                "precedence": k,
+                "description": descr,
+                "signature": str(inspect.signature(v)),
+                "location": v.__module__,
             }
             rows.append(row)
         return pd.DataFrame(rows)
 
     @classmethod
     def print_preprocessors(cls):
         df = cls.preprocessor_descr()
         if len(df):
             print(df)
         else:
-            print('No Preprocessors registered.')
+            print("No Preprocessors registered.")
 
     @classmethod
     def print_summary(cls):
-        print('='*30+' Protocols '+ '='*30)
+        print("=" * 30 + " Protocols " + "=" * 30)
         cls.print_protocols()
-        print('='*30+' Preprocessors '+ '='*30)
+        print("=" * 30 + " Preprocessors " + "=" * 30)
         cls.print_preprocessors()
 
     @classmethod
     def evaluate_dry(cls, url: str, **kwargs):
         """
         Utility function to quickly test and evaluate URL configs,
         without the initialization of plugins (so no plugin attributes).
@@ -481,262 +519,269 @@
         attributes of the plugin are not yet note to this dry evaluation
         of the url-string.
 
         :param url: URL to evaluate, see above for example.
         :keyword: any additional kwargs are passed to self.dispatch (see example)
         :return: evaluated value of the URL.
         """
-        protocol, url_arg, url_kwarg = cls.url_to_ast(url)
-
-        combined_kwargs = dict(url_kwarg, **kwargs)
+        url = cls.format_url_kwargs(url, **kwargs)
+        _, combined_kwargs = cls.split_url_kwargs(url)
 
-        for k,v in combined_kwargs.items():
+        for k, v in combined_kwargs.items():
             if isinstance(v, str) and cls.PLUGIN_ATTR_PREFIX in v:
-                raise ValueError(f'The URL parameter {k} depends on the plugin'
-                                'You must specify the value for this parameter'
-                                'for this URL to be evaluated correctly.'
-                                f'Try passing {k} as a keyword argument.'
-                                f'e.g.: `URLConfig.evaluate_dry({url}, {k}=SOME_VALUE)`')
-
-        return cls.eval(protocol, url_arg, combined_kwargs)
-
-@URLConfig.register('cmt')
-def get_correction(name: str,
-                   run_id: str = None,
-                   version: str = 'ONLINE',
-                   detector: str = 'nt',
-                   **kwargs):
+                raise ValueError(
+                    f"The URL parameter {k} depends on the plugin. "
+                    "You must specify the value for this parameter "
+                    "for this URL to be evaluated correctly. "
+                    f"Try passing {k} as a keyword argument. "
+                    f"e.g.: `URLConfig.evaluate_dry({url}, {k}=SOME_VALUE)`."
+                )
+        
+        return cls.eval(url)
+
+
+@URLConfig.register("cmt")
+def get_correction(
+    name: str,
+    run_id: str = None,
+    version: str = "ONLINE",
+    detector: str = "nt",
+    **kwargs,
+):
     """Get value for name from CMT"""
 
     if run_id is None:
-        raise ValueError('Attempting to fetch a correction without a run id.')    
+        raise ValueError("Attempting to fetch a correction without a run id.")
 
-    return straxen.get_correction_from_cmt(run_id, (name, version, detector == 'nt'))
+    return straxen.get_correction_from_cmt(run_id, (name, version, detector == "nt"))
 
 
-@URLConfig.register('resource')
-def get_resource(name: str,
-                 fmt: str = 'text',
-                 **kwargs):
+@URLConfig.register("resource")
+def get_resource(name: str, fmt: str = "text", **kwargs):
     """
     Fetch a straxen resource
     Allow a direct download using <fmt='abs_path'> otherwise kwargs are
     passed directly to straxen.get_resource.
     """
-    if fmt == 'abs_path':
+    if fmt == "abs_path":
         downloader = straxen.MongoDownloader()
         return downloader.download_single(name)
     return straxen.get_resource(name, fmt=fmt)
 
 
-@URLConfig.register('fsspec')
+@URLConfig.register("fsspec")
 def read_file(path: str, **kwargs):
-    """Support fetching files from arbitrary filesystems
-    """
+    """Support fetching files from arbitrary filesystems"""
     with fsspec.open(path, **kwargs) as f:
         content = f.read()
     return content
 
 
-@URLConfig.register('json')
+@URLConfig.register("json")
 def read_json(content: str, **kwargs):
-    """Load json string as a python object
-    """
+    """Load json string as a python object"""
     return json.loads(content)
 
 
-@URLConfig.register('take')
+@URLConfig.register("take")
 def get_key(container: Container, take=None, **kwargs):
-    """return a single element of a container
-    """
+    """return a single element of a container"""
     if take is None:
         return container
     if not isinstance(take, list):
         take = [take]
 
     # support for multiple keys for
     # nested objects
     for t in take:
         container = container[t]
 
     return container
 
 
-@URLConfig.register('format')
+@URLConfig.register("format")
 def format_arg(arg: str, **kwargs):
     """apply pythons builtin format function to a string"""
     return arg.format(**kwargs)
 
 
-@URLConfig.register('itp_map')
-def load_map(some_map, method='WeightedNearestNeighbors', scale_coordinates=None, **kwargs):
+@URLConfig.register("itp_map")
+def load_map(
+    some_map, method="WeightedNearestNeighbors", scale_coordinates=None, **kwargs
+):
     """Make an InterpolatingMap"""
     itp_map = straxen.InterpolatingMap(some_map, method=method, **kwargs)
     if scale_coordinates is not None:
         itp_map.scale_coordinates(scale_coordinates)
     return itp_map
 
-@URLConfig.register('bodega')
+
+@URLConfig.register("bodega")
 def load_value(name: str, bodega_version=None):
     """Load a number from BODEGA file"""
     if bodega_version is None:
-        raise ValueError('Provide version see e.g. tests/test_url_config.py')
+        raise ValueError("Provide version see e.g. tests/test_url_config.py")
     nt_numbers = straxen.get_resource("XENONnT_numbers.json", fmt="json")
     return nt_numbers[name][bodega_version]["value"]
 
 
-@URLConfig.register('tf')
+@URLConfig.register("tf")
 def open_neural_net(model_path: str, custom_objects=None, **kwargs):
-    '''Open a tensorflow file and return a keras model.
-    '''
+    """Open a tensorflow file and return a keras model."""
     # Nested import to reduce loading time of import straxen and it not
     # base requirement
     import tensorflow as tf
+
     if not os.path.exists(model_path):
-        raise FileNotFoundError(f'No file at {model_path}')
+        raise FileNotFoundError(f"No file at {model_path}")
     with tempfile.TemporaryDirectory() as tmpdirname:
         tar = tarfile.open(model_path, mode="r:gz")
         tar.extractall(path=tmpdirname)
         return tf.keras.models.load_model(tmpdirname, custom_objects=custom_objects)
 
 
-@URLConfig.register('itp_dict')
-def get_itp_dict(loaded_json,
-                 run_id=None,
-                 time_key='time',
-                 itp_keys='correction',
-                 **kwargs) -> typing.Union[np.ndarray, typing.Dict[str, np.ndarray]]:
+@URLConfig.register("itp_dict")
+def get_itp_dict(
+    loaded_json, run_id=None, time_key="time", itp_keys="correction", **kwargs
+) -> typing.Union[np.ndarray, typing.Dict[str, np.ndarray]]:
     """
     Interpolate a dictionary at the start time that is queried from
     a run-id.
 
     :param loaded_json: a dictionary with a time-series
     :param run_id: run_id
     :param time_key: key that gives the timestamps
     :param itp_keys: which keys from the dict to read. Should be
         comma (',') separated!
 
     :return: Interpolated values of dict at the start time, either
         returned as an np.ndarray (single value) or as a dict
         (multiple itp_dict_keys)
     """
-    keys = strax.to_str_tuple(itp_keys.split(','))
+    keys = strax.to_str_tuple(itp_keys.split(","))
     for key in list(keys) + [time_key]:
         if key not in loaded_json:
-            raise KeyError(f"The json does contain the key '{key}'. Try one of: {loaded_json.keys()}")
+            raise KeyError(
+                f"The json does contain the key '{key}'. Try one of: {loaded_json.keys()}"
+            )
 
     times = loaded_json[time_key]
 
     # get start time of this run. Need to make tz-aware
-    start = xent_collection().find_one({'number': int(run_id)}, {'start': 1})['start']
+    start = xent_collection().find_one({"number": int(run_id)}, {"start": 1})["start"]
     start = pytz.utc.localize(start).timestamp() * 1e9
 
     try:
         if len(strax.to_str_tuple(keys)) > 1:
-            return {key:
-                    interp1d(times, loaded_json[key], bounds_error=True)(start)
-                    for key in keys}
+            return {
+                key: interp1d(times, loaded_json[key], bounds_error=True)(start)
+                for key in keys
+            }
 
         else:
             interp = interp1d(times, loaded_json[keys[0]], bounds_error=True)
             return interp(start)
     except ValueError as e:
         raise ValueError(f"Correction is not defined for run {run_id}") from e
 
 
-@URLConfig.register('rekey_dict')
-def rekey_dict(d, replace_keys='', with_keys=''):
-    '''Replace the keys of a dictionary.
+@URLConfig.register("rekey_dict")
+def rekey_dict(d, replace_keys="", with_keys=""):
+    """Replace the keys of a dictionary.
     :param d: dictionary that will have its keys renamed
     :param replace_keys: comma-separated string of keys that will be replaced
     :param with_keys:  comma-separated string of keys that will replace the replace_keys
     :return: dictionary with renamed keys
-    '''
+    """
     new_dict = d.copy()
-    replace_keys = strax.to_str_tuple(replace_keys.split(','))
-    with_keys = strax.to_str_tuple(with_keys.split(','))
+    replace_keys = strax.to_str_tuple(replace_keys.split(","))
+    with_keys = strax.to_str_tuple(with_keys.split(","))
     if len(replace_keys) != len(with_keys):
         raise RuntimeError("replace_keys and with_keys must have the same length")
     for old_key, new_key in zip(replace_keys, with_keys):
         new_dict[new_key] = new_dict.pop(old_key)
     return new_dict
 
 
-@URLConfig.register('objects-to-dict')
-def objects_to_dict(objects: list, key_attr=None, value_attr='value', immutable=False):
-    '''Converts a list of objects/dicts to a single dictionary by taking the 
+@URLConfig.register("objects-to-dict")
+def objects_to_dict(objects: list, key_attr=None, value_attr="value", immutable=False):
+    """Converts a list of objects/dicts to a single dictionary by taking the
     key and value from each of the objects/dicts. If key_attr is not provided,
     the list index is used as the key.
 
     :param objects: list of objects/dicts that will be converted to a dictionary
     :param key_attr: key/attribute of the objects that will be used as key in the dictionary
     :param value_attr: key/attribute of the objects that will be used as value in the dictionary
-    '''
+    """
     if not isinstance(objects, Iterable):
-        raise TypeError(f'The objects-to-dict protocol expects an iterable '
-                        f'of objects but received {type(objects)} instead.')
+        raise TypeError(
+            f"The objects-to-dict protocol expects an iterable "
+            f"of objects but received {type(objects)} instead."
+        )
     result = {}
     for i, obj in enumerate(objects):
         key = i if key_attr is None else get_item_or_attr(obj, key_attr)
         result[key] = get_item_or_attr(obj, value_attr)
 
     if immutable:
         result = immutabledict(result)
-        
+
     return result
 
 
-@URLConfig.register('list-to-array')
+@URLConfig.register("list-to-array")
 def objects_to_array(objects: list):
-    '''
+    """
     Converts a list of objects/dicts to a numpy array.
-    :param objects: Any list of objects'''
-        
+    :param objects: Any list of objects"""
+
     if not isinstance(objects, Iterable):
-        raise TypeError(f'The list-to-array protocol expects an '
-                        f'iterable but recieved a {type(objects)} instead')
-        
+        raise TypeError(
+            f"The list-to-array protocol expects an "
+            f"iterable but recieved a {type(objects)} instead"
+        )
+
     return np.array(objects)
 
 
 @URLConfig.preprocessor
 def alphabetize_url_kwargs(url: str):
     """
     Reorders queries for urlconfigs to avoid hashing issues
     """
-    
+
     global WARN
 
     if isinstance(url, str) and URLConfig.SCHEME_SEP in url:
         if url != URLConfig.format_url_kwargs(url) and WARN:
-            warnings.warn("From straxen version 2.1.0 onward, URLConfig parameters"
-              "will be sorted alphabetically before being passed to the plugins,"
-              " this will change the lineage hash for non-sorted URLs. To load"
-              " data processed with non-sorted URLs, you will need to use an"
-              " older version.")
+            warnings.warn(
+                "From straxen version 2.1.0 onward, URLConfig parameters"
+                "will be sorted alphabetically before being passed to the plugins,"
+                " this will change the lineage hash for non-sorted URLs. To load"
+                " data processed with non-sorted URLs, you will need to use an"
+                " older version."
+            )
             WARN = False
         return URLConfig.format_url_kwargs(url)
     return url
 
 
-@URLConfig.register('run_doc')
+@URLConfig.register("run_doc")
 def read_rundoc(path, run_id=None, default=None):
-    """Read a path from the rundoc.
-    """
+    """Read a path from the rundoc."""
     if run_id is None:
-        raise ValueError('rundoc protocol: missing run_id.')
+        raise ValueError("rundoc protocol: missing run_id.")
     runs = xent_collection()
-    rundoc = runs.find_one({'number': int(run_id)}, {'_id': 0, path: 1})
+    rundoc = runs.find_one({"number": int(run_id)}, {"_id": 0, path: 1})
     if rundoc is None:
-        raise ValueError(f'No rundoc found for run {run_id}')
+        raise ValueError(f"No rundoc found for run {run_id}")
 
-    for part in path.split('.'):
-        if isinstance(rundoc, list) and part.isdigit() and len(rundoc)>int(part):
+    for part in path.split("."):
+        if isinstance(rundoc, list) and part.isdigit() and len(rundoc) > int(part):
             rundoc = rundoc[int(part)]
         elif isinstance(rundoc, dict) and part in rundoc:
             rundoc = rundoc[part]
         elif default is not None:
             return default
         else:
-            raise ValueError(f'No path {path} found in rundoc for run {run_id}')
+            raise ValueError(f"No path {path} found in rundoc for run {run_id}")
     return rundoc
-
```

### Comparing `straxen-2.1.1/straxen.egg-info/PKG-INFO` & `straxen-2.1.2/straxen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: straxen
-Version: 2.1.1
+Version: 2.1.2
 Summary: Streaming analysis for XENON
 Home-page: https://github.com/XENONnT/straxen
 Author: Straxen contributors, the XENON collaboration
 License: UNKNOWN
 Description: # straxen
         Streaming analysis for XENON(nT)
         
@@ -25,26 +25,37 @@
         [![Python Versions](https://img.shields.io/pypi/pyversions/straxen.svg)](https://pypi.python.org/pypi/straxen)
         [![PyPI downloads](https://img.shields.io/pypi/dm/straxen.svg)](https://pypistats.org/packages/straxen)
         
         [![Update context collection](https://github.com/XENONnT/straxen/workflows/Update%20context%20collection/badge.svg)](https://github.com/XENONnT/straxen/actions/workflows/contexts.yml)
         [![Python style](https://github.com/XENONnT/straxen/actions/workflows/code_style.yml/badge.svg)](https://github.com/XENONnT/straxen/actions/workflows/code_style.yml)
         
         
-        v2.1.1 / 2023-07-06
+        2.1.2 / 2023-07-28
+        -------------------
+        * Validate final type after URL eval by @jmosbacher in https://github.com/XENONnT/straxen/pull/1217
+        * Fix URLConfig.evaluate_dry by @jmosbacher in https://github.com/XENONnT/straxen/pull/1219
+        * Add function to save itp_map InterpolatingMap related dictionary into pickle by @dachengx in https://github.com/XENONnT/straxen/pull/1221
+        * Rename `tf_peak_model_s1_cnn` to `tf_model_s1_cnn` by @dachengx in https://github.com/XENONnT/straxen/pull/1223
+        
+        
+        **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.1.1...v2.1.2
+        
+        
+        2.1.1 / 2023-07-06
         -------------------
         * Fix timing of peaks when ordering in `center_time` by @dachengx in https://github.com/XENONnT/straxen/pull/1208
         * Move `get_window_size` factor of merged_s2s as untracked configuration by @dachengx in https://github.com/XENONnT/straxen/pull/1209
         * Sort `hitlets` in `nVETOHitlets` by @dachengx in https://github.com/XENONnT/straxen/pull/1210
         * Only print out warning once by @LuisSanchez25 in https://github.com/XENONnT/straxen/pull/1211
         
         
         **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.1.0...v2.1.1
         
         
-        v2.1.0 / 2023-06-22
+        2.1.0 / 2023-06-22
         -------------------
         * Added peaks subtyping by @Jianyu010 in https://github.com/XENONnT/straxen/pull/1152
         * Fix ipython version by @dachengx in https://github.com/XENONnT/straxen/pull/1169
         * Fix bug in hitlets time ordering by @dachengx in https://github.com/XENONnT/straxen/pull/1173
         * Bump actions/setup-python from 4.5.0 to 4.6.0 by @dependabot in https://github.com/XENONnT/straxen/pull/1170
         * Save hits level information(hits height and time difference) in peak and event level by @dachengx in https://github.com/XENONnT/straxen/pull/1155
         * Fix argsort inside numba.jit using kind='mergesort' by @dachengx in https://github.com/XENONnT/straxen/pull/1176
@@ -67,15 +78,15 @@
         New Contributors
         * @PeterGy made their first contribution in https://github.com/XENONnT/straxen/pull/1202
         * @minzhong98 made their first contribution in https://github.com/XENONnT/straxen/pull/1191
         
         **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.7...v2.1.0
         
         
-        v2.0.7 / 2023-04-25
+        2.0.7 / 2023-04-25
         -------------------
         * Bootstrax target removal after failures by @cfuselli in https://github.com/XENONnT/straxen/pull/1145
         * reforming _raw_path and _processed_path by @FaroutYLq in https://github.com/XENONnT/straxen/pull/1149
         * Adding correction of Z position due to non-uniform drift velocity by @terliuk in https://github.com/XENONnT/straxen/pull/1148
         * Bump the versions of peaklets and quality check runs-on by @dachengx in https://github.com/XENONnT/straxen/pull/1153
         * S1-Based 3D Position Reconstruction by @matteoguida in https://github.com/XENONnT/straxen/pull/1146
         * Bump xedocs from 0.2.14 to 0.2.16 in /extra_requirements by @dependabot in https://github.com/XENONnT/straxen/pull/1158
@@ -86,79 +97,79 @@
         * @cfuselli made their first contribution in https://github.com/XENONnT/straxen/pull/1145
         * @matteoguida made their first contribution in https://github.com/XENONnT/straxen/pull/1146
         * @hmdyt made their first contribution in https://github.com/XENONnT/straxen/pull/1159
         
         **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.6...v2.0.7
         
         
-        v2.0.6 / 2023-03-08
+        2.0.6 / 2023-03-08
         -------------------
         * Bump supercharge/mongodb-github-action from 1.8.0 to 1.9.0 by @dependabot in https://github.com/XENONnT/straxen/pull/1140
         * Small patches to restrax module by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1143, d04a3428c52c159577b61af2a28ddd0af5652027, 602b807291211f083c8f54df6768b8198fbf6b55
         * Ms events by @michaweiss89 and @HenningSE in https://github.com/XENONnT/straxen/pull/1080
         
         New Contributors
         * @michaweiss89 made their first contribution in https://github.com/XENONnT/straxen/pull/1080
         
         **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.5...v2.0.6
         
         Notes:
          - new data types: `peaks_per_event`, `event_top_bottom_params`, `peaks_corrections` (see #1080)
         
         
-        v2.0.5 / 2023-02-24
+        2.0.5 / 2023-02-24
         -------------------
         * fix xedocs for testing by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1139
         * Restart python style guide by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1138
         * Decrease number of chunks by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1123
         * Restrax by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1074
         
         
         **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.4...v2.0.5
         
         
-        v2.0.4 / 2023-01-16
+        2.0.4 / 2023-01-16
         -------------------
         * Top and bottom timing parameters at event and peak level by @terliuk in https://github.com/XENONnT/straxen/pull/1119
         * Allow use of xedocs context configs by @jmosbacher in https://github.com/XENONnT/straxen/pull/1125
         * Bump actions/setup-python from 4.3.0 to 4.4.0 by @dependabot in https://github.com/XENONnT/straxen/pull/1128
         * Add entry points by @jmosbacher in https://github.com/XENONnT/straxen/pull/1120
         * URLConfig preprocessor by @jmosbacher in https://github.com/XENONnT/straxen/pull/1110
         * Fix bootstrax timeouts by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1133
         
         
         **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.3...v2.1.0
         
         Notes:
          - new data types: `peak_top_bottom_params`, `event_top_bottom_params`
         
-        v2.0.3 / 2022-11-09
+        2.0.3 / 2022-11-09
         -------------------
         * Adding peak waveforms at event level by @terliuk in https://github.com/XENONnT/straxen/pull/1112
         
         
         **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.2...v2.0.3
         
         Notes:
          * lineage changes for event_area_per_channel
         
         
-        v2.0.2 / 2022-10-24
+        2.0.2 / 2022-10-24
         -------------------
         * New URLConfig protocols - list-to-array and list-to-dict by @LuisSanchez25 in https://github.com/XENONnT/straxen/pull/1104
         * Single core 1T test by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1109
         
         New Contributors
         * @LuisSanchez25 made their first contribution in https://github.com/XENONnT/straxen/pull/1104
         
         
         **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.1...v2.0.2
         
         
-        v2.0.1 / 2022-10-20
+        2.0.1 / 2022-10-20
         -------------------
         * Use mongodb v4.4.1 when testing to match real version used in production by @jmosbacher in https://github.com/XENONnT/straxen/pull/1103
         * Pass tests from remote forks by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1105
         * Local minimum info 2 by @JYangQi00 in https://github.com/XENONnT/straxen/pull/1106
         * Don't test without `strax.processor.SHMExecutor` by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1107
         * Lower the default config value of online_max_bytes by @mflierm in https://github.com/XENONnT/straxen/pull/1108
         
@@ -166,15 +177,15 @@
         New Contributors
         * @JYangQi00 made their first contribution in https://github.com/XENONnT/straxen/pull/1106
         
         
         **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.0...v2.0.1
         
         
-        v2.0.0 / 2022-10-17
+        2.0.0 / 2022-10-17
         -------------------
         * Fix acqmon veto field by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1072
         * Use self.dtype also for empty peaks by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1058
         * Re Start style guide by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1084
         * Transition plugins to URLConfig by @jmosbacher in https://github.com/XENONnT/straxen/pull/1079
         * Fix help of peak basics. by @WenzDaniel in https://github.com/XENONnT/straxen/pull/1081
         * Remove `tight_coincidence_channel` fix #1078 by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1092
@@ -194,39 +205,39 @@
          * Changed signatures of plugins in [#1094](https://github.com/XENONnT/straxen/pull/1094)
          * New plugins for event level processing by [#1097](https://github.com/XENONnT/straxen/pull/1097)
         
         
         **Full Changelog**: https://github.com/XENONnT/straxen/compare/v1.8.3...v2.0.0
         
         
-        v1.8.3 / 2022-07-18
+        1.8.3 / 2022-07-18
         -------------------
         * Bootstrax file-check fix by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1064
         * Fix hanging straxer by @jmosbacher in https://github.com/XENONnT/straxen/pull/1065
         
         Notes:
         * No lineage changes
         
         Full Changelog:
          - https://github.com/XENONnT/straxen/compare/v1.8.2...v1.8.3
         
         
-        v1.8.2 / 2022-07-12
+        1.8.2 / 2022-07-12
         -------------------
         * Stop tf pbar by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1063
         * Allow long runs by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1062
         
         Notes:
         * No lineage changes
         
         Full Changelog:
         - https://github.com/XENONnT/straxen/compare/v1.8.1...v1.8.2
         
         
-        v1.8.1 / 2022-06-07
+        1.8.1 / 2022-06-07
         -------------------
         Minor:
         * Change FDC z offset and add alternative interaction by @ftoschi in #1017
         * Plugin for online individual peak monitoring by @mflierm in #1054
         
         Notes:
         * Lineage changes for event_positions, corrected_areas, energy_estimates, event_info, event_info_double
@@ -242,15 +253,15 @@
         * Add kicp to query by @JoranAngevaare in #1052
         * Bump sphinx from 4.5.0 to 5.0.1 in /extra_requirements by @dependabot in #1051
         * Allow constant tuple options by @JoranAngevaare in #1039
         
         Full changelog:
         - https://github.com/XENONnT/straxen/compare/v1.7.1...v1.8.0
         
-        v1.7.2 / 2022-07-18
+        1.7.2 / 2022-07-18
         -------------------
         Patch:
          * Upload cherry picks by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1066
          * Fix hanging straxer by @jmosbacher in https://github.com/XENONnT/straxen/pull/1065
          * Stop tf pbar by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1063
          * update docs ev interactive display by @JoranAngevaare in #1042
          * allow dry eval of URL configs by @JoranAngevaare in #1040
@@ -260,15 +271,15 @@
          * Add kicp to query by @JoranAngevaare in #1052
          * Bump sphinx from 4.5.0 to 5.0.1 in /extra_requirements by @dependabot in #1051
          * Allow constant tuple options by @JoranAngevaare in #1039
         
         **Full Changelog**: https://github.com/XENONnT/straxen/compare/v1.7.1...v1.7.2
         
         
-        v1.7.1 / 2022-05-16
+        1.7.1 / 2022-05-16
         -------------------
         Patch:
         * Check if processed data already exists in --production mode by @mflierm in https://github.com/XENONnT/straxen/pull/1024
         
         
         Notes:
         - No lineage changes
@@ -276,15 +287,15 @@
         Full Changelog: 
          - https://github.com/XENONnT/straxen/compare/v1.7.0...v1.7.1
         
         New Contributors
          - @mflierm made their first contribution in https://github.com/XENONnT/straxen/pull/1024
         
         
-        v1.7.0 / 2022-05-11
+        1.7.0 / 2022-05-11
         ---------------------
         Minor:
         - Fix detector sync (#1033) 
         - Numbafy function (#1015) 
         - Fixing binomial (#991) 
         - Patched wrong setting (#1014) 
         - Partitioned tpc (#1027) 
@@ -301,15 +312,15 @@
         - Lineage changes for event_area_per_channel, event_pattern_fit, peak_classification_bayes, detector_time_offsets, event_sync_nv
         
         
         Full Changelog:
          - https://github.com/XENONnT/straxen/compare/v1.6.2...v1.7.0
         
         
-        v1.6.2 / 2022-05-06
+        1.6.2 / 2022-05-06
         ---------------------
         Patch:
         -  Add MV trigger channel to acqmon hits https://github.com/XENONnT/straxen/pull/1035
         
         Notes:
          - only lineage changes for dtypes > `aqmon_hits`  (https://github.com/XENONnT/straxen/pull/1035)
```

### Comparing `straxen-2.1.1/straxen.egg-info/SOURCES.txt` & `straxen-2.1.2/straxen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/tests/storage/test_database_frontends.py` & `straxen-2.1.2/tests/storage/test_database_frontends.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/tests/storage/test_mongo_downloader.py` & `straxen-2.1.2/tests/storage/test_mongo_downloader.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/tests/storage/test_mongo_interactions.py` & `straxen-2.1.2/tests/storage/test_mongo_interactions.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/tests/storage/test_rucio_local.py` & `straxen-2.1.2/tests/storage/test_rucio_local.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/tests/storage/test_rucio_remote.py` & `straxen-2.1.2/tests/storage/test_rucio_remote.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/tests/test_1T_plugins.py` & `straxen-2.1.2/tests/test_1T_plugins.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/tests/test_aqmon.py` & `straxen-2.1.2/tests/test_aqmon.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/tests/test_basics.py` & `straxen-2.1.2/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/tests/test_channel_split.py` & `straxen-2.1.2/tests/test_channel_split.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/tests/test_cmt.py` & `straxen-2.1.2/tests/test_cmt.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/tests/test_common.py` & `straxen-2.1.2/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/tests/test_contexts.py` & `straxen-2.1.2/tests/test_contexts.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/tests/test_count_pulses.py` & `straxen-2.1.2/tests/test_count_pulses.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/tests/test_daq_reader.py` & `straxen-2.1.2/tests/test_daq_reader.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/tests/test_holoviews_utils.py` & `straxen-2.1.2/tests/test_holoviews_utils.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/tests/test_led_calibration.py` & `straxen-2.1.2/tests/test_led_calibration.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/tests/test_mini_analyses.py` & `straxen-2.1.2/tests/test_mini_analyses.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/tests/test_misc.py` & `straxen-2.1.2/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/tests/test_nveto_events.py` & `straxen-2.1.2/tests/test_nveto_events.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/tests/test_nveto_recorder.py` & `straxen-2.1.2/tests/test_nveto_recorder.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/tests/test_patternfit.py` & `straxen-2.1.2/tests/test_patternfit.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/tests/test_peaklet_processing.py` & `straxen-2.1.2/tests/test_peaklet_processing.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/tests/test_peaks.py` & `straxen-2.1.2/tests/test_peaks.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/tests/test_scada.py` & `straxen-2.1.2/tests/test_scada.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/tests/test_url_config.py` & `straxen-2.1.2/tests/test_url_config.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.1/tests/test_veto_hitlets.py` & `straxen-2.1.2/tests/test_veto_hitlets.py`

 * *Files identical despite different names*

