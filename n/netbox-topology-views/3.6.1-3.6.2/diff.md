# Comparing `tmp/netbox-topology-views-3.6.1.tar.gz` & `tmp/netbox-topology-views-3.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-topology-views-3.6.1.tar", last modified: Tue Jul 11 13:29:30 2023, max compression
+gzip compressed data, was "netbox-topology-views-3.6.2.tar", last modified: Fri Jul 28 09:12:54 2023, max compression
```

## Comparing `netbox-topology-views-3.6.1.tar` & `netbox-topology-views-3.6.2.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:29:30.330277 netbox-topology-views-3.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 13:29:20.000000 netbox-topology-views-3.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-11 13:29:20.000000 netbox-topology-views-3.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12109 2023-07-11 13:29:30.326277 netbox-topology-views-3.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-07-11 13:29:20.000000 netbox-topology-views-3.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:29:30.314277 netbox-topology-views-3.6.1/netbox_topology_views/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:29:30.314277 netbox-topology-views-3.6.1/netbox_topology_views/api/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:29:30.314277 netbox-topology-views-3.6.1/netbox_topology_views/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/migrations/0002_individualoptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/migrations/0003_individualoptions_show_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/migrations/0004_coordinategroup_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/migrations/0005_individualoptions_save_coords.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:29:30.310277 netbox-topology-views-3.6.1/netbox_topology_views/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:29:30.310277 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:29:30.314277 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/css/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/css/app.css
--rw-r--r--   0 runner    (1001) docker     (123)   220074 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/css/vendor.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:29:30.322277 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/
--rw-r--r--   0 runner    (1001) docker     (123)    20139 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/access-switch.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/backhaul.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/backup.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/cable-doubler.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/camera-server.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/camera.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10537 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/circuit.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/console-server.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/core-router.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/core-switch.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/database-server.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/database.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/dect-station.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/desktop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/distribution-switch.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/docking-station.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/environment-monitor.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/fire-alarm-control-panel.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/firewall.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/fo-patch-panel.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/intrusion-alarm-system.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/kvm-over-ip.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/kvm.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/load-balancer.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/mobile-phone.svg
--rw-r--r--   0 runner    (1001) docker     (123)    17466 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/modem.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/network-socket.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/notebook.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/pabx.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/patch-panel.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/pdu.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/phone.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/power-panel.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/power-units.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/printer.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/provider-networks.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/proxy.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/role-unknown.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/router.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/server.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/siem.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/storage.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/switch.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/time-recording-terminal.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/ups.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/usb-lan-adapter.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/wan-network.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/wireless-ap.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:29:30.326277 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/js/
--rw-r--r--   0 runner    (1001) docker     (123)   350199 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/js/app.js
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/js/images.js
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/js/images.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:29:30.310277 netbox-topology-views-3.6.1/netbox_topology_views/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:29:30.326277 netbox-topology-views-3.6.1/netbox_topology_views/templates/netbox_topology_views/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/templates/netbox_topology_views/coordinate.html
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/templates/netbox_topology_views/coordinate_add.html
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/templates/netbox_topology_views/coordinate_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/templates/netbox_topology_views/coordinate_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/templates/netbox_topology_views/coordinategroup.html
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/templates/netbox_topology_views/coordinategroup_add.html
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/templates/netbox_topology_views/coordinategroup_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/templates/netbox_topology_views/coordinategroup_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/templates/netbox_topology_views/htmx_topology.html
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/templates/netbox_topology_views/images.html
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/templates/netbox_topology_views/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/templates/netbox_topology_views/individual_options.html
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/templates/netbox_topology_views/location_button.html
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/templates/netbox_topology_views/site_button.html
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/templates/netbox_topology_views/toasts.html
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    10681 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    36784 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/netbox_topology_views/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:29:30.314277 netbox-topology-views-3.6.1/netbox_topology_views.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12109 2023-07-11 13:29:30.000000 netbox-topology-views-3.6.1/netbox_topology_views.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-07-11 13:29:30.000000 netbox-topology-views-3.6.1/netbox_topology_views.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 13:29:30.000000 netbox-topology-views-3.6.1/netbox_topology_views.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 13:29:30.000000 netbox-topology-views-3.6.1/netbox_topology_views.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 13:29:30.330277 netbox-topology-views-3.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-11 13:29:21.000000 netbox-topology-views-3.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:12:54.257548 netbox-topology-views-3.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12109 2023-07-28 09:12:54.257548 netbox-topology-views-3.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:12:54.245548 netbox-topology-views-3.6.2/netbox_topology_views/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:12:54.245548 netbox-topology-views-3.6.2/netbox_topology_views/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:12:54.245548 netbox-topology-views-3.6.2/netbox_topology_views/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/migrations/0002_individualoptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/migrations/0003_individualoptions_show_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/migrations/0004_coordinategroup_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/migrations/0005_individualoptions_save_coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:12:54.241548 netbox-topology-views-3.6.2/netbox_topology_views/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:12:54.241548 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:12:54.245548 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/css/app.css
+-rw-r--r--   0 runner    (1001) docker     (123)   220074 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/css/vendor.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:12:54.253548 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    20139 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/access-switch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/backhaul.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/backup.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/cable-doubler.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/camera-server.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/camera.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10537 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/circuit.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/console-server.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/core-router.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/core-switch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/database-server.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/database.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/dect-station.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/desktop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/distribution-switch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/docking-station.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/environment-monitor.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/fire-alarm-control-panel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/firewall.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/fo-patch-panel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/intrusion-alarm-system.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/kvm-over-ip.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/kvm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/load-balancer.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/mobile-phone.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    17466 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/modem.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/network-socket.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/notebook.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/pabx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/patch-panel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/pdu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/phone.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/power-panel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/power-units.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/printer.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/provider-networks.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/proxy.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/role-unknown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/router.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/server.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/siem.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/storage.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/switch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/time-recording-terminal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/ups.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/usb-lan-adapter.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/wan-network.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/wireless-ap.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:12:54.253548 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   350199 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/js/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/js/images.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/js/images.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:12:54.241548 netbox-topology-views-3.6.2/netbox_topology_views/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:12:54.257548 netbox-topology-views-3.6.2/netbox_topology_views/templates/netbox_topology_views/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/templates/netbox_topology_views/coordinate.html
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/templates/netbox_topology_views/coordinate_add.html
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/templates/netbox_topology_views/coordinate_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/templates/netbox_topology_views/coordinate_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/templates/netbox_topology_views/coordinategroup.html
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/templates/netbox_topology_views/coordinategroup_add.html
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/templates/netbox_topology_views/coordinategroup_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/templates/netbox_topology_views/coordinategroup_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/templates/netbox_topology_views/htmx_topology.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/templates/netbox_topology_views/images.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/templates/netbox_topology_views/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/templates/netbox_topology_views/individual_options.html
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/templates/netbox_topology_views/location_button.html
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/templates/netbox_topology_views/site_button.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/templates/netbox_topology_views/toasts.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10681 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36784 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/netbox_topology_views/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:12:54.245548 netbox-topology-views-3.6.2/netbox_topology_views.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12109 2023-07-28 09:12:54.000000 netbox-topology-views-3.6.2/netbox_topology_views.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-07-28 09:12:54.000000 netbox-topology-views-3.6.2/netbox_topology_views.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 09:12:54.000000 netbox-topology-views-3.6.2/netbox_topology_views.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 09:12:54.000000 netbox-topology-views-3.6.2/netbox_topology_views.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 09:12:54.257548 netbox-topology-views-3.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-28 09:12:44.000000 netbox-topology-views-3.6.2/setup.py
```

### Comparing `netbox-topology-views-3.6.1/LICENSE` & `netbox-topology-views-3.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/PKG-INFO` & `netbox-topology-views-3.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-topology-views
-Version: 3.6.1
+Version: 3.6.2
 Summary: An NetBox plugin to create Topology maps
 Home-page: https://github.com/mattieserver/netbox-topology-views
 Author: Mattijs Vanhaverbeke
 License: Apache 2.0
 Project-URL: Source, https://github.com/mattieserver/netbox-topology-views
 Keywords: netbox-plugin
 Classifier: Programming Language :: Python
```

### Comparing `netbox-topology-views-3.6.1/README.md` & `netbox-topology-views-3.6.2/README.md`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/__init__.py` & `netbox-topology-views-3.6.2/netbox_topology_views/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from extras.plugins import PluginConfig
 
 
 class TopologyViewsConfig(PluginConfig):
     name = "netbox_topology_views"
     verbose_name = "Topology views"
     description = "An plugin to render topology maps"
-    version = "3.6.1"
+    version = "3.6.2"
     author = "Mattijs Vanhaverbeke"
     author_email = "author@example.com"
     base_url = "netbox_topology_views"
     required_settings = []
     default_settings = {
         "static_image_directory": "netbox_topology_views/img",
         "allow_coordinates_saving": False,
```

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/api/serializers.py` & `netbox-topology-views-3.6.2/netbox_topology_views/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/api/views.py` & `netbox-topology-views-3.6.2/netbox_topology_views/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/filters.py` & `netbox-topology-views-3.6.2/netbox_topology_views/filters.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/forms.py` & `netbox-topology-views-3.6.2/netbox_topology_views/forms.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/migrations/0001_initial.py` & `netbox-topology-views-3.6.2/netbox_topology_views/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/migrations/0002_individualoptions.py` & `netbox-topology-views-3.6.2/netbox_topology_views/migrations/0002_individualoptions.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/migrations/0004_coordinategroup_coordinate.py` & `netbox-topology-views-3.6.2/netbox_topology_views/migrations/0004_coordinategroup_coordinate.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/models.py` & `netbox-topology-views-3.6.2/netbox_topology_views/models.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/navigation.py` & `netbox-topology-views-3.6.2/netbox_topology_views/navigation.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,50 +3,54 @@
 
 coordinategroup_buttons = (
     PluginMenuButton(
         link='plugins:netbox_topology_views:coordinategroup_add',
         title='Add',
         icon_class='mdi mdi-plus-thick',
         color=ButtonColorChoices.GREEN,
+        permissions=['netbox_topology_views.add_coordinategroup']
     ),
     PluginMenuButton(
         link='plugins:netbox_topology_views:coordinategroup_import',
         title='Import',
         icon_class='mdi mdi-upload',
         color=ButtonColorChoices.CYAN,
+        permissions=['netbox_topology_views.add_coordinategroup']
     )
 )
 
 coordinate_buttons = (
     PluginMenuButton(
         link='plugins:netbox_topology_views:coordinate_add',
         title='Add',
         icon_class='mdi mdi-plus-thick',
         color=ButtonColorChoices.GREEN,
+        permissions=['netbox_topology_views.add_coordinate']
     ),
     PluginMenuButton(
         link='plugins:netbox_topology_views:coordinate_import',
         title='Import',
         icon_class='mdi mdi-upload',
         color=ButtonColorChoices.CYAN,
+        permissions=['netbox_topology_views.add_coordinate']
     )
 )
 
 menu = PluginMenu(
     label='Topology Views',
     icon_class="mdi mdi-sitemap",
     groups=(
         ('TOPOLOGY', 
             (
-                PluginMenuItem(link="plugins:netbox_topology_views:home", link_text="Topology"),
-                PluginMenuItem(link="plugins:netbox_topology_views:coordinategroup_list", link_text="Coordinate Groups", buttons=coordinategroup_buttons),
-                PluginMenuItem(link="plugins:netbox_topology_views:coordinate_list", link_text="Coordinates", buttons=coordinate_buttons),
+                PluginMenuItem(link="plugins:netbox_topology_views:home", link_text="Topology", permissions=["dcim.view_site", "dcim.view_device"]),
+                PluginMenuItem(link="plugins:netbox_topology_views:coordinategroup_list", link_text="Coordinate Groups", buttons=coordinategroup_buttons, permissions=['netbox_topology_views.view_coordinategroup']),
+                PluginMenuItem(link="plugins:netbox_topology_views:coordinate_list", link_text="Coordinates", buttons=coordinate_buttons, permissions=['netbox_topology_views.view_coordinate']),
             ),
         ),
         ('PREFERENCES', 
             (
-                PluginMenuItem(link="plugins:netbox_topology_views:images", link_text="Images"),
-                PluginMenuItem(link="plugins:netbox_topology_views:individualoptions", link_text="Individual Options"),
+                PluginMenuItem(link="plugins:netbox_topology_views:images", link_text="Images", permissions=[ "dcim.view_site","dcim.view_device_role"]),
+                PluginMenuItem(link="plugins:netbox_topology_views:individualoptions", link_text="Individual Options", permissions=['netbox_topology_views.change_individualoptions']),
             ),
         ),
     ),
 )
```

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/signals.py` & `netbox-topology-views-3.6.2/netbox_topology_views/signals.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/css/vendor.css` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/css/vendor.css`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/LICENSE` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/access-switch.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/access-switch.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/backhaul.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/backhaul.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/backup.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/backup.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/cable-doubler.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/cable-doubler.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/camera-server.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/camera-server.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/camera.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/camera.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/circuit.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/circuit.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/console-server.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/console-server.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/core-router.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/core-router.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/core-switch.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/core-switch.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/database-server.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/database-server.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/database.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/database.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/dect-station.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/dect-station.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/desktop.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/desktop.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/distribution-switch.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/distribution-switch.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/docking-station.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/docking-station.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/environment-monitor.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/environment-monitor.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/fire-alarm-control-panel.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/fire-alarm-control-panel.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/firewall.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/firewall.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/fo-patch-panel.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/fo-patch-panel.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/intrusion-alarm-system.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/intrusion-alarm-system.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/kvm-over-ip.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/kvm-over-ip.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/kvm.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/kvm.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/load-balancer.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/load-balancer.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/mobile-phone.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/mobile-phone.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/modem.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/modem.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/network-socket.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/network-socket.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/notebook.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/notebook.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/pabx.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/pabx.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/patch-panel.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/patch-panel.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/pdu.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/pdu.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/phone.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/phone.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/power-panel.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/power-panel.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/power-units.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/power-units.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/printer.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/printer.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/provider-networks.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/provider-networks.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/proxy.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/proxy.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/role-unknown.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/role-unknown.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/router.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/router.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/server.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/server.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/siem.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/siem.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/storage.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/storage.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/switch.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/switch.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/time-recording-terminal.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/time-recording-terminal.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/ups.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/ups.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/usb-lan-adapter.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/usb-lan-adapter.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/wan-network.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/wan-network.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/img/wireless-ap.svg` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/img/wireless-ap.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/js/app.js` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/js/app.js`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/js/images.js` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/js/images.js`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/static/netbox_topology_views/js/images.js.map` & `netbox-topology-views-3.6.2/netbox_topology_views/static/netbox_topology_views/js/images.js.map`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/tables.py` & `netbox-topology-views-3.6.2/netbox_topology_views/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/template_content.py` & `netbox-topology-views-3.6.2/netbox_topology_views/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/templates/netbox_topology_views/coordinate.html` & `netbox-topology-views-3.6.2/netbox_topology_views/templates/netbox_topology_views/coordinate.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/templates/netbox_topology_views/coordinategroup.html` & `netbox-topology-views-3.6.2/netbox_topology_views/templates/netbox_topology_views/coordinategroup.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/templates/netbox_topology_views/htmx_topology.html` & `netbox-topology-views-3.6.2/netbox_topology_views/templates/netbox_topology_views/htmx_topology.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/templates/netbox_topology_views/images.html` & `netbox-topology-views-3.6.2/netbox_topology_views/templates/netbox_topology_views/images.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/templates/netbox_topology_views/index.html` & `netbox-topology-views-3.6.2/netbox_topology_views/templates/netbox_topology_views/index.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/templates/netbox_topology_views/toasts.html` & `netbox-topology-views-3.6.2/netbox_topology_views/templates/netbox_topology_views/toasts.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/urls.py` & `netbox-topology-views-3.6.2/netbox_topology_views/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/utils.py` & `netbox-topology-views-3.6.2/netbox_topology_views/utils.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views/views.py` & `netbox-topology-views-3.6.2/netbox_topology_views/views.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views.egg-info/PKG-INFO` & `netbox-topology-views-3.6.2/netbox_topology_views.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-topology-views
-Version: 3.6.1
+Version: 3.6.2
 Summary: An NetBox plugin to create Topology maps
 Home-page: https://github.com/mattieserver/netbox-topology-views
 Author: Mattijs Vanhaverbeke
 License: Apache 2.0
 Project-URL: Source, https://github.com/mattieserver/netbox-topology-views
 Keywords: netbox-plugin
 Classifier: Programming Language :: Python
```

### Comparing `netbox-topology-views-3.6.1/netbox_topology_views.egg-info/SOURCES.txt` & `netbox-topology-views-3.6.2/netbox_topology_views.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.1/setup.py` & `netbox-topology-views-3.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 readme = Path(__file__).parent / "README.md"
 long_description = readme.read_text()
 
 setup(
     name="netbox-topology-views",
-    version="3.6.1",
+    version="3.6.2",
     description="An NetBox plugin to create Topology maps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mattieserver/netbox-topology-views",
     author="Mattijs Vanhaverbeke",
     license="Apache 2.0",
     install_requires=[],
```

