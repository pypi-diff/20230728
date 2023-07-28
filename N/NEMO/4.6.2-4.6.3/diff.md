# Comparing `tmp/NEMO-4.6.2.tar.gz` & `tmp/NEMO-4.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NEMO-4.6.2.tar", last modified: Wed Jul 26 20:15:31 2023, max compression
+gzip compressed data, was "NEMO-4.6.3.tar", last modified: Fri Jul 28 21:19:22 2023, max compression
```

## Comparing `NEMO-4.6.2.tar` & `NEMO-4.6.3.tar`

### file list

```diff
@@ -1,513 +1,514 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.267285 NEMO-4.6.2/
--rw-rw-rw-   0 root         (0) root         (0)     1865 2023-07-18 17:03:12.000000 NEMO-4.6.2/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-07-18 17:03:12.000000 NEMO-4.6.2/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.166285 NEMO-4.6.2/NEMO/
--rw-rw-rw-   0 root         (0) root         (0)     1254 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4594 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/actions.py
--rw-rw-rw-   0 root         (0) root         (0)    49666 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.169285 NEMO-4.6.2/NEMO/apps/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 20:15:15.000000 NEMO-4.6.2/NEMO/apps/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.169285 NEMO-4.6.2/NEMO/apps/area_access/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 20:15:15.000000 NEMO-4.6.2/NEMO/apps/area_access/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.144285 NEMO-4.6.2/NEMO/apps/area_access/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.169285 NEMO-4.6.2/NEMO/apps/area_access/static/area_access/
--rw-rw-rw-   0 root         (0) root         (0)      304 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/area_access/static/area_access/area_access.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.144285 NEMO-4.6.2/NEMO/apps/area_access/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.173285 NEMO-4.6.2/NEMO/apps/area_access/templates/area_access/
--rw-rw-rw-   0 root         (0) root         (0)     1727 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/area_access/templates/area_access/already_logged_in.html
--rw-rw-rw-   0 root         (0) root         (0)      349 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/area_access/templates/area_access/badge_not_found.html
--rw-rw-rw-   0 root         (0) root         (0)     9006 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/area_access/templates/area_access/base.html
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/area_access/templates/area_access/choose_project.html
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/area_access/templates/area_access/door_is_open.html
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/area_access/templates/area_access/farewell_screen.html
--rw-rw-rw-   0 root         (0) root         (0)      143 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/area_access/templates/area_access/inactive.html
--rw-rw-rw-   0 root         (0) root         (0)      397 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/area_access/templates/area_access/login_success.html
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/area_access/templates/area_access/logout_success.html
--rw-rw-rw-   0 root         (0) root         (0)      666 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/area_access/templates/area_access/logout_warning.html
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/area_access/templates/area_access/no_active_projects.html
--rw-rw-rw-   0 root         (0) root         (0)      338 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/area_access/templates/area_access/not_logged_in.html
--rw-rw-rw-   0 root         (0) root         (0)      210 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/area_access/templates/area_access/physical_access_denied.html
--rw-rw-rw-   0 root         (0) root         (0)      566 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/area_access/templates/area_access/resource_unavailable.html
--rw-rw-rw-   0 root         (0) root         (0)      224 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/area_access/templates/area_access/welcome_screen.html
--rw-rw-rw-   0 root         (0) root         (0)      629 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/area_access/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    12663 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/area_access/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.174285 NEMO-4.6.2/NEMO/apps/contracts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 20:15:15.000000 NEMO-4.6.2/NEMO/apps/contracts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4147 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/contracts/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      212 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/contracts/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/contracts/customization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.175285 NEMO-4.6.2/NEMO/apps/contracts/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 20:15:15.000000 NEMO-4.6.2/NEMO/apps/contracts/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.175285 NEMO-4.6.2/NEMO/apps/contracts/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 20:15:15.000000 NEMO-4.6.2/NEMO/apps/contracts/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      335 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/contracts/management/commands/send_email_contract_reminders.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.176285 NEMO-4.6.2/NEMO/apps/contracts/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     5839 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/contracts/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 20:15:15.000000 NEMO-4.6.2/NEMO/apps/contracts/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5550 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/contracts/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.144285 NEMO-4.6.2/NEMO/apps/contracts/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.177285 NEMO-4.6.2/NEMO/apps/contracts/templates/contracts/
--rw-rw-rw-   0 root         (0) root         (0)     4319 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/contracts/templates/contracts/contractors.html
--rw-rw-rw-   0 root         (0) root         (0)     4204 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/contracts/templates/contracts/contracts_and_procurements.html
--rw-rw-rw-   0 root         (0) root         (0)     3726 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/contracts/templates/contracts/procurements.html
--rw-rw-rw-   0 root         (0) root         (0)     5069 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/contracts/templates/contracts/service_contracts.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.177285 NEMO-4.6.2/NEMO/apps/contracts/templates/customizations/
--rw-rw-rw-   0 root         (0) root         (0)     2580 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/contracts/templates/customizations/customizations_contracts.html
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/contracts/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.178285 NEMO-4.6.2/NEMO/apps/contracts/views/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 20:15:15.000000 NEMO-4.6.2/NEMO/apps/contracts/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10827 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/contracts/views/contracts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.178285 NEMO-4.6.2/NEMO/apps/kiosk/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 20:15:15.000000 NEMO-4.6.2/NEMO/apps/kiosk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.145285 NEMO-4.6.2/NEMO/apps/kiosk/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.179285 NEMO-4.6.2/NEMO/apps/kiosk/static/kiosk/
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/kiosk/static/kiosk/kiosk.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.145285 NEMO-4.6.2/NEMO/apps/kiosk/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.181285 NEMO-4.6.2/NEMO/apps/kiosk/templates/kiosk/
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/kiosk/templates/kiosk/acknowledgement.html
--rw-rw-rw-   0 root         (0) root         (0)     2125 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/kiosk/templates/kiosk/category_choices.html
--rw-rw-rw-   0 root         (0) root         (0)     2044 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/kiosk/templates/kiosk/choices.html
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/kiosk/templates/kiosk/error.html
--rw-rw-rw-   0 root         (0) root         (0)     2923 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/kiosk/templates/kiosk/individual_reservation.html
--rw-rw-rw-   0 root         (0) root         (0)    12592 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/kiosk/templates/kiosk/kiosk.html
--rw-rw-rw-   0 root         (0) root         (0)      901 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/kiosk/templates/kiosk/success.html
--rw-rw-rw-   0 root         (0) root         (0)    17312 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/kiosk/templates/kiosk/tool_information.html
--rw-rw-rw-   0 root         (0) root         (0)     1108 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/kiosk/templates/kiosk/tool_project_selection_snippet.html
--rw-rw-rw-   0 root         (0) root         (0)     4472 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/kiosk/templates/kiosk/tool_reservation.html
--rw-rw-rw-   0 root         (0) root         (0)     1271 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/kiosk/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    13386 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/kiosk/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.183285 NEMO-4.6.2/NEMO/apps/sensors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 20:15:15.000000 NEMO-4.6.2/NEMO/apps/sensors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7128 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/sensors/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      567 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/sensors/customizations.py
--rw-rw-rw-   0 root         (0) root         (0)     5237 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/sensors/evaluators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.183285 NEMO-4.6.2/NEMO/apps/sensors/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 20:15:15.000000 NEMO-4.6.2/NEMO/apps/sensors/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.183285 NEMO-4.6.2/NEMO/apps/sensors/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 20:15:15.000000 NEMO-4.6.2/NEMO/apps/sensors/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/sensors/management/commands/manage_sensor_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.184285 NEMO-4.6.2/NEMO/apps/sensors/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     7794 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/sensors/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 20:15:15.000000 NEMO-4.6.2/NEMO/apps/sensors/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13007 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/sensors/models.py
--rw-rw-rw-   0 root         (0) root         (0)     4906 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/sensors/sensors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.146285 NEMO-4.6.2/NEMO/apps/sensors/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.186285 NEMO-4.6.2/NEMO/apps/sensors/static/sensors/
--rw-rw-rw-   0 root         (0) root         (0)   408236 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/sensors/static/sensors/chart.js
--rw-rw-rw-   0 root         (0) root         (0)   195090 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/sensors/static/sensors/chart.min.js
--rw-rw-rw-   0 root         (0) root         (0)     1376 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/sensors/static/sensors/chartjs-adapter-moment.js
--rw-rw-rw-   0 root         (0) root         (0)     7659 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/sensors/static/sensors/daterangepicker.css
--rw-rw-rw-   0 root         (0) root         (0)    66305 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/sensors/static/sensors/daterangepicker.js
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/sensors/static/sensors/sensors.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.147285 NEMO-4.6.2/NEMO/apps/sensors/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.187285 NEMO-4.6.2/NEMO/apps/sensors/templates/customizations/
--rw-rw-rw-   0 root         (0) root         (0)     4718 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/sensors/templates/customizations/customizations_sensors.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.187285 NEMO-4.6.2/NEMO/apps/sensors/templates/sensors/
--rw-rw-rw-   0 root         (0) root         (0)      347 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/sensors/templates/sensors/sensor_alerts.html
--rw-rw-rw-   0 root         (0) root         (0)    15165 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/sensors/templates/sensors/sensor_data.html
--rw-rw-rw-   0 root         (0) root         (0)     3879 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/sensors/templates/sensors/sensors.html
--rw-rw-rw-   0 root         (0) root         (0)      790 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/sensors/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     5650 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/apps/sensors/views.py
--rw-rw-rw-   0 root         (0) root         (0)     3966 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/context_processors.py
--rw-rw-rw-   0 root         (0) root         (0)     5776 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3833 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/fields.py
--rw-rw-rw-   0 root         (0) root         (0)    14224 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/forms.py
--rw-rw-rw-   0 root         (0) root         (0)    17784 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/interlocks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.187285 NEMO-4.6.2/NEMO/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 20:15:15.000000 NEMO-4.6.2/NEMO/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.190285 NEMO-4.6.2/NEMO/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 20:15:15.000000 NEMO-4.6.2/NEMO/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/management/commands/cancel_unused_reservations.py
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/management/commands/create_closure_alerts.py
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/management/commands/manage_recurring_charges.py
--rw-rw-rw-   0 root         (0) root         (0)      431 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/management/commands/manage_tool_qualifications.py
--rw-rw-rw-   0 root         (0) root         (0)      417 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/management/commands/send_email_out_of_time_reservation_notification.py
--rw-rw-rw-   0 root         (0) root         (0)      415 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/management/commands/send_email_reservation_ending_reminders.py
--rw-rw-rw-   0 root         (0) root         (0)      408 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/management/commands/send_email_reservation_reminders.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/management/commands/send_email_usage_reminders.py
--rw-rw-rw-   0 root         (0) root         (0)      456 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/management/commands/send_email_user_access_expiration_reminders.py
--rw-rw-rw-   0 root         (0) root         (0)      406 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/management/commands/send_email_weekend_access_notification.py
--rw-rw-rw-   0 root         (0) root         (0)     5578 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.197285 NEMO-4.6.2/NEMO/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    50307 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations/0001_version_1_0_0.py
--rw-rw-rw-   0 root         (0) root         (0)    32962 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations/0002_version_1_0_0_squashed.py
--rw-rw-rw-   0 root         (0) root         (0)     7988 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations/0012_version_2_0_0_squashed.py
--rw-rw-rw-   0 root         (0) root         (0)     9904 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations/0020_version_3_0_0.py
--rw-rw-rw-   0 root         (0) root         (0)     1712 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations/0021_version_3_1_0.py
--rw-rw-rw-   0 root         (0) root         (0)     1095 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations/0022_version_3_3_0.py
--rw-rw-rw-   0 root         (0) root         (0)      913 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations/0023_badgereader.py
--rw-rw-rw-   0 root         (0) root         (0)      705 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations/0024_contactinformation_user.py
--rw-rw-rw-   0 root         (0) root         (0)     2674 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations/0025_version_3_6_0.py
--rw-rw-rw-   0 root         (0) root         (0)     5405 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations/0026_version_3_7_0.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations/0027_version_3_8_0.py
--rw-rw-rw-   0 root         (0) root         (0)     2231 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations/0028_version_3_9_0.py
--rw-rw-rw-   0 root         (0) root         (0)     1127 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations/0030_version_3_9_2.py
--rw-rw-rw-   0 root         (0) root         (0)     2785 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations/0031_version_3_10_0.py
--rw-rw-rw-   0 root         (0) root         (0)     3166 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations/0032_version_3_11_0.py
--rw-rw-rw-   0 root         (0) root         (0)      380 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations/0033_version_3_12_0.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations/0034_version_3_13_0.py
--rw-rw-rw-   0 root         (0) root         (0)     6747 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations/0035_version_3_14_0.py
--rw-rw-rw-   0 root         (0) root         (0)     7792 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations/0036_version_3_15_0.py
--rw-rw-rw-   0 root         (0) root         (0)     3717 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations/0037_version_3_16_0.py
--rw-rw-rw-   0 root         (0) root         (0)      935 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations/0038_version_4_0_0.py
--rw-rw-rw-   0 root         (0) root         (0)     3601 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations/0039_version_4_1_0.py
--rw-rw-rw-   0 root         (0) root         (0)     2444 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations/0040_version_4_2_0.py
--rw-rw-rw-   0 root         (0) root         (0)      487 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations/0041_version_4_2_1.py
--rw-rw-rw-   0 root         (0) root         (0)    16447 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations/0042_version_4_3_0.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations/0043_version_4_3_2.py
--rw-rw-rw-   0 root         (0) root         (0)     5416 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations/0044_version_4_4_0.py
--rw-rw-rw-   0 root         (0) root         (0)    13447 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations/0045_version_4_5_0.py
--rw-rw-rw-   0 root         (0) root         (0)     2037 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations/0045_version_4_5_5.py
--rw-rw-rw-   0 root         (0) root         (0)     2997 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations/0046_version_4_6_0.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-07-25 22:28:19.000000 NEMO-4.6.2/NEMO/migrations/0047_version_4_6_1.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 20:15:15.000000 NEMO-4.6.2/NEMO/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2299 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/migrations_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     7993 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/mixins.py
--rw-rw-rw-   0 root         (0) root         (0)     3855 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/model_tree.py
--rw-rw-rw-   0 root         (0) root         (0)   148192 2023-07-25 22:28:19.000000 NEMO-4.6.2/NEMO/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1429 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)    49662 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/policy.py
--rw-rw-rw-   0 root         (0) root         (0)     9943 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/provisioning.py
--rw-rw-rw-   0 root         (0) root         (0)     5646 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/rates.py
--rw-rw-rw-   0 root         (0) root         (0)     1037 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/rest_filter_backend.py
--rw-rw-rw-   0 root         (0) root         (0)    11173 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/serializers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.203285 NEMO-4.6.2/NEMO/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.204285 NEMO-4.6.2/NEMO/static/admin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.204285 NEMO-4.6.2/NEMO/static/admin/physical_access_level/
--rw-rw-rw-   0 root         (0) root         (0)      607 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/admin/physical_access_level/access_level.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.204285 NEMO-4.6.2/NEMO/static/admin/questions_preview/
--rw-rw-rw-   0 root         (0) root         (0)     4122 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/admin/questions_preview/questions_preview.css
--rw-rw-rw-   0 root         (0) root         (0)     1372 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/admin/questions_preview/questions_preview.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.205285 NEMO-4.6.2/NEMO/static/admin/reservation_questions/
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/admin/reservation_questions/reservation_questions.js
--rw-rw-rw-   0 root         (0) root         (0)     1225 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/admin/time_options_override.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.205285 NEMO-4.6.2/NEMO/static/admin/tool/
--rw-rw-rw-   0 root         (0) root         (0)     1437 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/admin/tool/tool.js
--rw-rw-rw-   0 root         (0) root         (0)     1515 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/badge_reader.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.149285 NEMO-4.6.2/NEMO/static/bootstrap/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.207285 NEMO-4.6.2/NEMO/static/bootstrap/css/
--rw-rw-rw-   0 root         (0) root         (0)    22608 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/bootstrap/css/bootstrap-theme.css
--rw-rw-rw-   0 root         (0) root         (0)    43339 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/bootstrap/css/bootstrap-theme.css.map
--rw-rw-rw-   0 root         (0) root         (0)    19963 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/bootstrap/css/bootstrap-theme.min.css
--rw-rw-rw-   0 root         (0) root         (0)   141622 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/bootstrap/css/bootstrap.css
--rw-rw-rw-   0 root         (0) root         (0)   380986 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/bootstrap/css/bootstrap.css.map
--rw-rw-rw-   0 root         (0) root         (0)   117305 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.209285 NEMO-4.6.2/NEMO/static/bootstrap/fonts/
--rw-rw-rw-   0 root         (0) root         (0)    20127 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.eot
--rw-rw-rw-   0 root         (0) root         (0)   108738 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.svg
--rw-rw-rw-   0 root         (0) root         (0)    45404 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)    23424 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff
--rw-rw-rw-   0 root         (0) root         (0)    18028 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.210285 NEMO-4.6.2/NEMO/static/bootstrap/js/
--rw-rw-rw-   0 root         (0) root         (0)    67546 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/bootstrap/js/bootstrap.js
--rw-rw-rw-   0 root         (0) root         (0)    35951 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/bootstrap/js/bootstrap.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.210285 NEMO-4.6.2/NEMO/static/datetimepicker/
--rw-rw-rw-   0 root         (0) root         (0)     9020 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/datetimepicker/bootstrap-datetimepicker.css
--rw-rw-rw-   0 root         (0) root         (0)   105978 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/datetimepicker/bootstrap-datetimepicker.js
--rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.212285 NEMO-4.6.2/NEMO/static/fullcalendar/
--rw-rw-rw-   0 root         (0) root         (0)    28531 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/fullcalendar/fullcalendar.css
--rw-rw-rw-   0 root         (0) root         (0)   357749 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/fullcalendar/fullcalendar.js
--rw-rw-rw-   0 root         (0) root         (0)    13687 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/fullcalendar/fullcalendar.min.css
--rw-rw-rw-   0 root         (0) root         (0)   168700 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/fullcalendar/fullcalendar.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.213285 NEMO-4.6.2/NEMO/static/icons/
--rw-rw-rw-   0 root         (0) root         (0)    24065 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/icons/agreement.png
--rw-rw-rw-   0 root         (0) root         (0)    16685 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/icons/caution.png
--rw-rw-rw-   0 root         (0) root         (0)     4664 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/icons/preferences.png
--rw-rw-rw-   0 root         (0) root         (0)   247387 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/jquery.js
--rw-rw-rw-   0 root         (0) root         (0)    84320 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/jquery.min.js
--rw-rw-rw-   0 root         (0) root         (0)  1183392 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/jumbotron_watermark.bmp
--rw-rw-rw-   0 root         (0) root         (0)     1017 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/mobile.js
--rw-rw-rw-   0 root         (0) root         (0)   174603 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/moment.js
--rw-rw-rw-   0 root         (0) root         (0)    58102 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/moment.min.js
--rw-rw-rw-   0 root         (0) root         (0)    86041 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/moment.min.js.map
--rw-rw-rw-   0 root         (0) root         (0)    18266 2023-07-26 20:15:15.000000 NEMO-4.6.2/NEMO/static/nemo.css
--rw-rw-rw-   0 root         (0) root         (0)    21828 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/nemo.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.213285 NEMO-4.6.2/NEMO/static/numpad/
--rw-rw-rw-   0 root         (0) root         (0)    12285 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/numpad/custom_numpad.jquery.js
--rw-rw-rw-   0 root         (0) root         (0)      255 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/numpad/numpad.jquery.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.215285 NEMO-4.6.2/NEMO/static/pickadate/
--rw-rw-rw-   0 root         (0) root         (0)     3795 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/pickadate/default.css
--rw-rw-rw-   0 root         (0) root         (0)     6040 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/pickadate/default.date.css
--rw-rw-rw-   0 root         (0) root         (0)     2785 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/pickadate/default.time.css
--rw-rw-rw-   0 root         (0) root         (0)    48215 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/pickadate/picker.date.js
--rw-rw-rw-   0 root         (0) root         (0)    36941 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/pickadate/picker.js
--rw-rw-rw-   0 root         (0) root         (0)    31899 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/pickadate/picker.time.js
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/robots.txt
--rw-rw-rw-   0 root         (0) root         (0)    48446 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/typeahead.jquery.js
--rw-rw-rw-   0 root         (0) root         (0)    20748 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/typeahead.jquery.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.216285 NEMO-4.6.2/NEMO/static/virtualkeyboard/
--rw-rw-rw-   0 root         (0) root         (0)   113008 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/virtualkeyboard/jquery.keyboard.js
--rw-rw-rw-   0 root         (0) root         (0)    47325 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/virtualkeyboard/jquery.keyboard.min.js
--rw-rw-rw-   0 root         (0) root         (0)     7848 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/virtualkeyboard/keyboard-basic.css
--rw-rw-rw-   0 root         (0) root         (0)     5889 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/static/virtualkeyboard/keyboard-basic.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.219285 NEMO-4.6.2/NEMO/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.219285 NEMO-4.6.2/NEMO/templates/abuse/
--rw-rw-rw-   0 root         (0) root         (0)     4059 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/abuse/abuse.html
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/abuse/user_drill_down.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.221285 NEMO-4.6.2/NEMO/templates/accounts_and_projects/
--rw-rw-rw-   0 root         (0) root         (0)     7665 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/accounts_and_projects/account_and_projects.html
--rw-rw-rw-   0 root         (0) root         (0)     6409 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/accounts_and_projects/accounts_and_projects.html
--rw-rw-rw-   0 root         (0) root         (0)     2843 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/accounts_and_projects/create_account.html
--rw-rw-rw-   0 root         (0) root         (0)     6693 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/accounts_and_projects/create_project.html
--rw-rw-rw-   0 root         (0) root         (0)      888 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/accounts_and_projects/documents_for_project.html
--rw-rw-rw-   0 root         (0) root         (0)     3544 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/accounts_and_projects/projects.html
--rw-rw-rw-   0 root         (0) root         (0)      917 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/accounts_and_projects/users_for_project.html
--rw-rw-rw-   0 root         (0) root         (0)      433 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/acknowledgement.html
--rw-rw-rw-   0 root         (0) root         (0)     4694 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/alerts.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.222285 NEMO-4.6.2/NEMO/templates/area_access/
--rw-rw-rw-   0 root         (0) root         (0)     2951 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/area_access/area_access.html
--rw-rw-rw-   0 root         (0) root         (0)     1748 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/area_access/calendar_self_login.html
--rw-rw-rw-   0 root         (0) root         (0)     1111 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/area_access/change_project.html
--rw-rw-rw-   0 root         (0) root         (0)     1141 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/area_access/login_areas.html
--rw-rw-rw-   0 root         (0) root         (0)     1245 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/area_access/new_area_access_record.html
--rw-rw-rw-   0 root         (0) root         (0)     1938 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/area_access/new_area_access_record_details.html
--rw-rw-rw-   0 root         (0) root         (0)     1454 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/area_access/self_login.html
--rw-rw-rw-   0 root         (0) root         (0)      837 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/authorization_failed.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.223285 NEMO-4.6.2/NEMO/templates/base/
--rw-rw-rw-   0 root         (0) root         (0)      308 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/base/footer.html
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/base/impersonate_header.html
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/base/navbar.html
--rw-rw-rw-   0 root         (0) root         (0)     8117 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/base/navbar_base.html
--rw-rw-rw-   0 root         (0) root         (0)      308 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/base/popup.html
--rw-rw-rw-   0 root         (0) root         (0)     6174 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.230285 NEMO-4.6.2/NEMO/templates/calendar/
--rw-rw-rw-   0 root         (0) root         (0)    24673 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/calendar/calendar.html
--rw-rw-rw-   0 root         (0) root         (0)     1442 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/calendar/configuration.html
--rw-rw-rw-   0 root         (0) root         (0)     2834 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/calendar/configuration_helper.html
--rw-rw-rw-   0 root         (0) root         (0)     1315 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/calendar/policy_dialog.html
--rw-rw-rw-   0 root         (0) root         (0)     1361 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/calendar/project_choice.html
--rw-rw-rw-   0 root         (0) root         (0)     1512 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/calendar/proxy_reservation.html
--rw-rw-rw-   0 root         (0) root         (0)     1862 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/calendar/reservation_event_feed.html
--rw-rw-rw-   0 root         (0) root         (0)     1680 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/calendar/reservation_questions.html
--rw-rw-rw-   0 root         (0) root         (0)     1285 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/calendar/reservation_warning.html
--rw-rw-rw-   0 root         (0) root         (0)     4410 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/calendar/scheduled_outage_information.html
--rw-rw-rw-   0 root         (0) root         (0)     2011 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/calendar/specific_user_feed.html
--rw-rw-rw-   0 root         (0) root         (0)     2543 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/calendar/usage_event_feed.html
--rw-rw-rw-   0 root         (0) root         (0)     6530 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/configuration_agenda.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.231285 NEMO-4.6.2/NEMO/templates/consumables/
--rw-rw-rw-   0 root         (0) root         (0)     8224 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/consumables/consumables.html
--rw-rw-rw-   0 root         (0) root         (0)     1538 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/consumables/consumables_order.html
--rw-rw-rw-   0 root         (0) root         (0)    11695 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/consumables/recurring_charge.html
--rw-rw-rw-   0 root         (0) root         (0)     5473 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/consumables/recurring_charges.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.231285 NEMO-4.6.2/NEMO/templates/contact/
--rw-rw-rw-   0 root         (0) root         (0)      692 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/contact/contact_staff.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.235285 NEMO-4.6.2/NEMO/templates/customizations/
--rw-rw-rw-   0 root         (0) root         (0)     1848 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/customizations/customizations.html
--rw-rw-rw-   0 root         (0) root         (0)     4882 2023-07-25 22:28:19.000000 NEMO-4.6.2/NEMO/templates/customizations/customizations_application.html
--rw-rw-rw-   0 root         (0) root         (0)     7799 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/customizations/customizations_calendar.html
--rw-rw-rw-   0 root         (0) root         (0)     7634 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/customizations/customizations_dashboard.html
--rw-rw-rw-   0 root         (0) root         (0)     4202 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/customizations/customizations_emails.html
--rw-rw-rw-   0 root         (0) root         (0)     2545 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/customizations/customizations_interlock.html
--rw-rw-rw-   0 root         (0) root         (0)     5553 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/customizations/customizations_projects_and_accounts.html
--rw-rw-rw-   0 root         (0) root         (0)     2224 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/customizations/customizations_rates.html
--rw-rw-rw-   0 root         (0) root         (0)     3519 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/customizations/customizations_recurring_charges.html
--rw-rw-rw-   0 root         (0) root         (0)     2183 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/customizations/customizations_remote_work.html
--rw-rw-rw-   0 root         (0) root         (0)    16717 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/customizations/customizations_requests.html
--rw-rw-rw-   0 root         (0) root         (0)     3678 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/customizations/customizations_safety.html
--rw-rw-rw-   0 root         (0) root         (0)    27806 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/customizations/customizations_templates.html
--rw-rw-rw-   0 root         (0) root         (0)     9253 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/customizations/customizations_tool.html
--rw-rw-rw-   0 root         (0) root         (0)     1731 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/customizations/customizations_upload.html
--rw-rw-rw-   0 root         (0) root         (0)     5214 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/customizations/customizations_user.html
--rw-rw-rw-   0 root         (0) root         (0)      502 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/display_success_and_redirect.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.236285 NEMO-4.6.2/NEMO/templates/email/
--rw-rw-rw-   0 root         (0) root         (0)     7825 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/email/compose_email.html
--rw-rw-rw-   0 root         (0) root         (0)     3153 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/email/email_broadcast.html
--rw-rw-rw-   0 root         (0) root         (0)     1045 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/email/email_form.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.236285 NEMO-4.6.2/NEMO/templates/event_details/
--rw-rw-rw-   0 root         (0) root         (0)      751 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/event_details/area_access_details.html
--rw-rw-rw-   0 root         (0) root         (0)     1376 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/event_details/outage_details.html
--rw-rw-rw-   0 root         (0) root         (0)    12242 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/event_details/reservation_details.html
--rw-rw-rw-   0 root         (0) root         (0)      589 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/event_details/usage_details.html
--rw-rw-rw-   0 root         (0) root         (0)      426 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/facility_rules.html
--rw-rw-rw-   0 root         (0) root         (0)     1247 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/feedback.html
--rw-rw-rw-   0 root         (0) root         (0)      937 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/history.html
--rw-rw-rw-   0 root         (0) root         (0)     1260 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/impersonate.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.237285 NEMO-4.6.2/NEMO/templates/jumbotron/
--rw-rw-rw-   0 root         (0) root         (0)     2059 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/jumbotron/jumbotron.html
--rw-rw-rw-   0 root         (0) root         (0)     3835 2023-07-26 20:15:15.000000 NEMO-4.6.2/NEMO/templates/jumbotron/jumbotron_content.html
--rw-rw-rw-   0 root         (0) root         (0)     8670 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/landing.html
--rw-rw-rw-   0 root         (0) root         (0)     3496 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/login.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.238285 NEMO-4.6.2/NEMO/templates/maintenance/
--rw-rw-rw-   0 root         (0) root         (0)     1558 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/maintenance/closed_task_details.html
--rw-rw-rw-   0 root         (0) root         (0)     5566 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/maintenance/maintenance.html
--rw-rw-rw-   0 root         (0) root         (0)     7450 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/maintenance/pending_task_details.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.240285 NEMO-4.6.2/NEMO/templates/mobile/
--rw-rw-rw-   0 root         (0) root         (0)      762 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/mobile/cancellation_result.html
--rw-rw-rw-   0 root         (0) root         (0)     1916 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/mobile/choose_item.html
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/mobile/error.html
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/mobile/individual_outage.html
--rw-rw-rw-   0 root         (0) root         (0)     2625 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/mobile/individual_reservation.html
--rw-rw-rw-   0 root         (0) root         (0)     5899 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/mobile/new_reservation.html
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/mobile/no_active_projects.html
--rw-rw-rw-   0 root         (0) root         (0)      777 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/mobile/reservation_success.html
--rw-rw-rw-   0 root         (0) root         (0)     1442 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/mobile/view_calendar.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.240285 NEMO-4.6.2/NEMO/templates/news/
--rw-rw-rw-   0 root         (0) root         (0)      981 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/news/archived_news.html
--rw-rw-rw-   0 root         (0) root         (0)     1027 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/news/new_news_form.html
--rw-rw-rw-   0 root         (0) root         (0)     1198 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/news/news_update_form.html
--rw-rw-rw-   0 root         (0) root         (0)     2038 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/news/recent_news.html
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/no_project.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.241285 NEMO-4.6.2/NEMO/templates/occupancy/
--rw-rw-rw-   0 root         (0) root         (0)      490 2023-07-26 20:15:15.000000 NEMO-4.6.2/NEMO/templates/occupancy/occupancy.html
--rw-rw-rw-   0 root         (0) root         (0)     1811 2023-07-26 20:15:15.000000 NEMO-4.6.2/NEMO/templates/occupancy/occupancy_content.html
--rw-rw-rw-   0 root         (0) root         (0)     1147 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/occupancy/occupancy_count.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.242285 NEMO-4.6.2/NEMO/templates/pagination/
--rw-rw-rw-   0 root         (0) root         (0)      865 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/pagination/pagination_base.html
--rw-rw-rw-   0 root         (0) root         (0)      521 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/pagination/pagination_column.html
--rw-rw-rw-   0 root         (0) root         (0)      673 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/pagination/pagination_pages.html
--rw-rw-rw-   0 root         (0) root         (0)      642 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/pagination/pagination_selector.html
--rw-rw-rw-   0 root         (0) root         (0)     2841 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/qualifications.html
--rw-rw-rw-   0 root         (0) root         (0)     5462 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/refresh_sidebar_icons.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.242285 NEMO-4.6.2/NEMO/templates/remote_work/
--rw-rw-rw-   0 root         (0) root         (0)    10616 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/remote_work/remote_work.html
--rw-rw-rw-   0 root         (0) root         (0)     1081 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/remote_work/remote_work_base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.243285 NEMO-4.6.2/NEMO/templates/requests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.243285 NEMO-4.6.2/NEMO/templates/requests/access_requests/
--rw-rw-rw-   0 root         (0) root         (0)     7754 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/requests/access_requests/access_request.html
--rw-rw-rw-   0 root         (0) root         (0)     3450 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/requests/access_requests/access_requests.html
--rw-rw-rw-   0 root         (0) root         (0)     3480 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/requests/access_requests/access_requests_table.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.244285 NEMO-4.6.2/NEMO/templates/requests/adjustment_requests/
--rw-rw-rw-   0 root         (0) root         (0)     8607 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/requests/adjustment_requests/adjustment_request.html
--rw-rw-rw-   0 root         (0) root         (0)     3733 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/requests/adjustment_requests/adjustment_requests.html
--rw-rw-rw-   0 root         (0) root         (0)     7257 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/requests/adjustment_requests/adjustment_requests_table.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.244285 NEMO-4.6.2/NEMO/templates/requests/buddy_requests/
--rw-rw-rw-   0 root         (0) root         (0)     3910 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/requests/buddy_requests/buddy_request.html
--rw-rw-rw-   0 root         (0) root         (0)     5602 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/requests/buddy_requests/buddy_requests.html
--rw-rw-rw-   0 root         (0) root         (0)     4246 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/requests/user_requests.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.245285 NEMO-4.6.2/NEMO/templates/resources/
--rw-rw-rw-   0 root         (0) root         (0)     2950 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/resources/modify_resource.html
--rw-rw-rw-   0 root         (0) root         (0)     3846 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/resources/resource_details.html
--rw-rw-rw-   0 root         (0) root         (0)     1423 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/resources/resources.html
--rw-rw-rw-   0 root         (0) root         (0)     3898 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/resources/scheduled_outage.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.246285 NEMO-4.6.2/NEMO/templates/rest_framework/
--rw-rw-rw-   0 root         (0) root         (0)     2736 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/rest_framework/api.html
--rw-rw-rw-   0 root         (0) root         (0)      446 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/rest_framework/custom_error.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.247285 NEMO-4.6.2/NEMO/templates/safety/
--rw-rw-rw-   0 root         (0) root         (0)     3112 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/safety/safety.html
--rw-rw-rw-   0 root         (0) root         (0)     1733 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/safety/safety_base.html
--rw-rw-rw-   0 root         (0) root         (0)     7807 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/safety/safety_data_sheets.html
--rw-rw-rw-   0 root         (0) root         (0)     1976 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/safety/safety_issues.html
--rw-rw-rw-   0 root         (0) root         (0)     1723 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/safety/safety_issues_create.html
--rw-rw-rw-   0 root         (0) root         (0)     1722 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/safety/safety_issues_resolved.html
--rw-rw-rw-   0 root         (0) root         (0)     1762 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/safety/safety_issues_update.html
--rw-rw-rw-   0 root         (0) root         (0)     1877 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/safety/safety_items.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.248285 NEMO-4.6.2/NEMO/templates/snippets/
--rw-rw-rw-   0 root         (0) root         (0)      516 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/snippets/button.html
--rw-rw-rw-   0 root         (0) root         (0)      904 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/snippets/contact_person.html
--rw-rw-rw-   0 root         (0) root         (0)      962 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/snippets/document_list.html
--rw-rw-rw-   0 root         (0) root         (0)     1128 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/snippets/embedded_document.html
--rw-rw-rw-   0 root         (0) root         (0)     1673 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/snippets/tool_info.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.250285 NEMO-4.6.2/NEMO/templates/staff_charges/
--rw-rw-rw-   0 root         (0) root         (0)      860 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/staff_charges/change_status.html
--rw-rw-rw-   0 root         (0) root         (0)     1242 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/staff_charges/choose_project.html
--rw-rw-rw-   0 root         (0) root         (0)      498 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/staff_charges/end_area_charge.html
--rw-rw-rw-   0 root         (0) root         (0)     1198 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/staff_charges/new_staff_charge.html
--rw-rw-rw-   0 root         (0) root         (0)     1014 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/staff_charges/reminder.html
--rw-rw-rw-   0 root         (0) root         (0)     1854 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/staff_charges/staff_charges_base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.251285 NEMO-4.6.2/NEMO/templates/status_dashboard/
--rw-rw-rw-   0 root         (0) root         (0)     1636 2023-07-26 20:15:15.000000 NEMO-4.6.2/NEMO/templates/status_dashboard/occupancy.html
--rw-rw-rw-   0 root         (0) root         (0)     9772 2023-07-25 22:28:19.000000 NEMO-4.6.2/NEMO/templates/status_dashboard/staff.html
--rw-rw-rw-   0 root         (0) root         (0)     7709 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/status_dashboard/staff_absence.html
--rw-rw-rw-   0 root         (0) root         (0)     6650 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/status_dashboard/status_dashboard.html
--rw-rw-rw-   0 root         (0) root         (0)     3717 2023-07-26 20:15:15.000000 NEMO-4.6.2/NEMO/templates/status_dashboard/tools.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.251285 NEMO-4.6.2/NEMO/templates/tasks/
--rw-rw-rw-   0 root         (0) root         (0)     2542 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/tasks/resolve.html
--rw-rw-rw-   0 root         (0) root         (0)     5037 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/tasks/update.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.253285 NEMO-4.6.2/NEMO/templates/tool_control/
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/tool_control/get_projects.html
--rw-rw-rw-   0 root         (0) root         (0)      737 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/tool_control/interlock_error.html
--rw-rw-rw-   0 root         (0) root         (0)     3502 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/tool_control/past_tasks_and_comments.html
--rw-rw-rw-   0 root         (0) root         (0)     2466 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/tool_control/qualified_users.html
--rw-rw-rw-   0 root         (0) root         (0)    15303 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/tool_control/tool_control.html
--rw-rw-rw-   0 root         (0) root         (0)    37737 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/tool_control/tool_status.html
--rw-rw-rw-   0 root         (0) root         (0)     6142 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/tool_control/usage_data.html
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/tool_control/use_tool_for_other.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.254285 NEMO-4.6.2/NEMO/templates/training/
--rw-rw-rw-   0 root         (0) root         (0)      512 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/training/get_projects.html
--rw-rw-rw-   0 root         (0) root         (0)     4971 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/training/training.html
--rw-rw-rw-   0 root         (0) root         (0)     1962 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/training/training_entry.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.254285 NEMO-4.6.2/NEMO/templates/usage/
--rw-rw-rw-   0 root         (0) root         (0)      976 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/usage/adjustment_request_button.html
--rw-rw-rw-   0 root         (0) root         (0)     3573 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/usage/billing.html
--rw-rw-rw-   0 root         (0) root         (0)     9218 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/usage/usage.html
--rw-rw-rw-   0 root         (0) root         (0)     7812 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/usage/usage_base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.255285 NEMO-4.6.2/NEMO/templates/users/
--rw-rw-rw-   0 root         (0) root         (0)    20776 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/users/create_or_modify_user.html
--rw-rw-rw-   0 root         (0) root         (0)    18558 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/users/preferences.html
--rw-rw-rw-   0 root         (0) root         (0)     3758 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/users/safe_deactivation.html
--rw-rw-rw-   0 root         (0) root         (0)     4181 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templates/users/users.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.256285 NEMO-4.6.2/NEMO/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 20:15:15.000000 NEMO-4.6.2/NEMO/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8447 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/templatetags/custom_tags_and_filters.py
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/typing.py
--rw-rw-rw-   0 root         (0) root         (0)    26303 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    24695 2023-07-25 22:28:19.000000 NEMO-4.6.2/NEMO/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.265285 NEMO-4.6.2/NEMO/views/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 20:15:15.000000 NEMO-4.6.2/NEMO/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4308 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/abuse.py
--rw-rw-rw-   0 root         (0) root         (0)    14733 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/access_requests.py
--rw-rw-rw-   0 root         (0) root         (0)     8275 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/accounts_and_projects.py
--rw-rw-rw-   0 root         (0) root         (0)    19286 2023-07-25 22:28:19.000000 NEMO-4.6.2/NEMO/views/adjustment_requests.py
--rw-rw-rw-   0 root         (0) root         (0)     1812 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/alerts.py
--rw-rw-rw-   0 root         (0) root         (0)    14004 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/api.py
--rw-rw-rw-   0 root         (0) root         (0)    12252 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/api_billing.py
--rw-rw-rw-   0 root         (0) root         (0)     2415 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/api_file_import.py
--rw-rw-rw-   0 root         (0) root         (0)    19170 2023-07-26 20:15:15.000000 NEMO-4.6.2/NEMO/views/area_access.py
--rw-rw-rw-   0 root         (0) root         (0)    12070 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     6625 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/buddy_requests.py
--rw-rw-rw-   0 root         (0) root         (0)    71831 2023-07-25 22:28:19.000000 NEMO-4.6.2/NEMO/views/calendar.py
--rw-rw-rw-   0 root         (0) root         (0)     2334 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/charge_validation.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/configuration_agenda.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    10947 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/consumables.py
--rw-rw-rw-   0 root         (0) root         (0)      467 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/contact_staff.py
--rw-rw-rw-   0 root         (0) root         (0)    18748 2023-07-25 22:28:19.000000 NEMO-4.6.2/NEMO/views/customization.py
--rw-rw-rw-   0 root         (0) root         (0)     3442 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/documents.py
--rw-rw-rw-   0 root         (0) root         (0)    10015 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/email.py
--rw-rw-rw-   0 root         (0) root         (0)     1973 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/event_details.py
--rw-rw-rw-   0 root         (0) root         (0)     1482 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/feedback.py
--rw-rw-rw-   0 root         (0) root         (0)     1672 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/get_projects.py
--rw-rw-rw-   0 root         (0) root         (0)     4168 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/history.py
--rw-rw-rw-   0 root         (0) root         (0)     1155 2023-07-26 20:15:15.000000 NEMO-4.6.2/NEMO/views/jumbotron.py
--rw-rw-rw-   0 root         (0) root         (0)     3293 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/landing.py
--rw-rw-rw-   0 root         (0) root         (0)     2718 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/maintenance.py
--rw-rw-rw-   0 root         (0) root         (0)     8072 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/mobile.py
--rw-rw-rw-   0 root         (0) root         (0)     3356 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/news.py
--rw-rw-rw-   0 root         (0) root         (0)     5095 2023-07-25 22:28:19.000000 NEMO-4.6.2/NEMO/views/notifications.py
--rw-rw-rw-   0 root         (0) root         (0)     1326 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/pagination.py
--rw-rw-rw-   0 root         (0) root         (0)     4822 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/qualifications.py
--rw-rw-rw-   0 root         (0) root         (0)     9506 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/remote_work.py
--rw-rw-rw-   0 root         (0) root         (0)     3700 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/resources.py
--rw-rw-rw-   0 root         (0) root         (0)     8877 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/safety.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/sidebar.py
--rw-rw-rw-   0 root         (0) root         (0)    20496 2023-07-26 20:15:15.000000 NEMO-4.6.2/NEMO/views/status_dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)    13615 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)    23995 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/tool_control.py
--rw-rw-rw-   0 root         (0) root         (0)     6043 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/training.py
--rw-rw-rw-   0 root         (0) root         (0)     1909 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/tutorials.py
--rw-rw-rw-   0 root         (0) root         (0)    18360 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/usage.py
--rw-rw-rw-   0 root         (0) root         (0)     1049 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/user_requests.py
--rw-rw-rw-   0 root         (0) root         (0)    20715 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/views/users.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.266285 NEMO-4.6.2/NEMO/widgets/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 20:15:15.000000 NEMO-4.6.2/NEMO/widgets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2968 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/widgets/configuration_editor.py
--rw-rw-rw-   0 root         (0) root         (0)    26383 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/widgets/dynamic_form.py
--rw-rw-rw-   0 root         (0) root         (0)     8029 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/widgets/item_tree.py
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-07-18 17:03:12.000000 NEMO-4.6.2/NEMO/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.168285 NEMO-4.6.2/NEMO.egg-info/
--rw-r--r--   0 root         (0) root         (0)      904 2023-07-26 20:15:31.000000 NEMO-4.6.2/NEMO.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    17413 2023-07-26 20:15:31.000000 NEMO-4.6.2/NEMO.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 20:15:31.000000 NEMO-4.6.2/NEMO.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-26 20:15:31.000000 NEMO-4.6.2/NEMO.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      264 2023-07-26 20:15:31.000000 NEMO-4.6.2/NEMO.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-26 20:15:31.000000 NEMO-4.6.2/NEMO.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      904 2023-07-26 20:15:31.267285 NEMO-4.6.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4066 2023-07-18 17:03:12.000000 NEMO-4.6.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:31.266285 NEMO-4.6.2/resources/
--rw-rw-rw-   0 root         (0) root         (0)    17163 2023-07-25 22:28:19.000000 NEMO-4.6.2/resources/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     3981 2023-07-18 17:03:12.000000 NEMO-4.6.2/resources/splash_pad_settings.py
--rw-r--r--   0 root         (0) root         (0)      109 2023-07-26 20:15:31.267285 NEMO-4.6.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-07-26 20:15:15.000000 NEMO-4.6.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.414472 NEMO-4.6.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1865 2023-07-18 17:03:12.000000 NEMO-4.6.3/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-07-18 17:03:12.000000 NEMO-4.6.3/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.344471 NEMO-4.6.3/NEMO/
+-rw-rw-rw-   0 root         (0) root         (0)     1254 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4594 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)    49699 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/admin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.345471 NEMO-4.6.3/NEMO/apps/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/apps/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.346471 NEMO-4.6.3/NEMO/apps/area_access/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/apps/area_access/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.331471 NEMO-4.6.3/NEMO/apps/area_access/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.346471 NEMO-4.6.3/NEMO/apps/area_access/static/area_access/
+-rw-rw-rw-   0 root         (0) root         (0)      304 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/area_access/static/area_access/area_access.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.331471 NEMO-4.6.3/NEMO/apps/area_access/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.350471 NEMO-4.6.3/NEMO/apps/area_access/templates/area_access/
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/area_access/templates/area_access/already_logged_in.html
+-rw-rw-rw-   0 root         (0) root         (0)      349 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/area_access/templates/area_access/badge_not_found.html
+-rw-rw-rw-   0 root         (0) root         (0)     9006 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/area_access/templates/area_access/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/area_access/templates/area_access/choose_project.html
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/area_access/templates/area_access/door_is_open.html
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/area_access/templates/area_access/farewell_screen.html
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/area_access/templates/area_access/inactive.html
+-rw-rw-rw-   0 root         (0) root         (0)      397 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/area_access/templates/area_access/login_success.html
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/area_access/templates/area_access/logout_success.html
+-rw-rw-rw-   0 root         (0) root         (0)      666 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/area_access/templates/area_access/logout_warning.html
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/area_access/templates/area_access/no_active_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)      338 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/area_access/templates/area_access/not_logged_in.html
+-rw-rw-rw-   0 root         (0) root         (0)      210 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/area_access/templates/area_access/physical_access_denied.html
+-rw-rw-rw-   0 root         (0) root         (0)      566 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/area_access/templates/area_access/resource_unavailable.html
+-rw-rw-rw-   0 root         (0) root         (0)      224 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/area_access/templates/area_access/welcome_screen.html
+-rw-rw-rw-   0 root         (0) root         (0)      629 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/area_access/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    12663 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/area_access/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.351471 NEMO-4.6.3/NEMO/apps/contracts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/apps/contracts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4147 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/contracts/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      212 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/contracts/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/contracts/customization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.351471 NEMO-4.6.3/NEMO/apps/contracts/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/apps/contracts/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.352471 NEMO-4.6.3/NEMO/apps/contracts/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/apps/contracts/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/contracts/management/commands/send_email_contract_reminders.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.352471 NEMO-4.6.3/NEMO/apps/contracts/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     5839 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/contracts/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/apps/contracts/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5550 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/contracts/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.332471 NEMO-4.6.3/NEMO/apps/contracts/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.353471 NEMO-4.6.3/NEMO/apps/contracts/templates/contracts/
+-rw-rw-rw-   0 root         (0) root         (0)     4319 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/contracts/templates/contracts/contractors.html
+-rw-rw-rw-   0 root         (0) root         (0)     4204 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/contracts/templates/contracts/contracts_and_procurements.html
+-rw-rw-rw-   0 root         (0) root         (0)     3726 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/contracts/templates/contracts/procurements.html
+-rw-rw-rw-   0 root         (0) root         (0)     5069 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/contracts/templates/contracts/service_contracts.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.353471 NEMO-4.6.3/NEMO/apps/contracts/templates/customizations/
+-rw-rw-rw-   0 root         (0) root         (0)     2580 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/contracts/templates/customizations/customizations_contracts.html
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/contracts/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.353471 NEMO-4.6.3/NEMO/apps/contracts/views/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/apps/contracts/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10827 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/contracts/views/contracts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.354472 NEMO-4.6.3/NEMO/apps/kiosk/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/apps/kiosk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.332471 NEMO-4.6.3/NEMO/apps/kiosk/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.354472 NEMO-4.6.3/NEMO/apps/kiosk/static/kiosk/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/kiosk/static/kiosk/kiosk.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.332471 NEMO-4.6.3/NEMO/apps/kiosk/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.356471 NEMO-4.6.3/NEMO/apps/kiosk/templates/kiosk/
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/kiosk/templates/kiosk/acknowledgement.html
+-rw-rw-rw-   0 root         (0) root         (0)     2125 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/kiosk/templates/kiosk/category_choices.html
+-rw-rw-rw-   0 root         (0) root         (0)     2044 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/kiosk/templates/kiosk/choices.html
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/kiosk/templates/kiosk/error.html
+-rw-rw-rw-   0 root         (0) root         (0)     2923 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/kiosk/templates/kiosk/individual_reservation.html
+-rw-rw-rw-   0 root         (0) root         (0)    12592 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/kiosk/templates/kiosk/kiosk.html
+-rw-rw-rw-   0 root         (0) root         (0)      901 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/kiosk/templates/kiosk/success.html
+-rw-rw-rw-   0 root         (0) root         (0)    17312 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/kiosk/templates/kiosk/tool_information.html
+-rw-rw-rw-   0 root         (0) root         (0)     1108 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/kiosk/templates/kiosk/tool_project_selection_snippet.html
+-rw-rw-rw-   0 root         (0) root         (0)     4472 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/kiosk/templates/kiosk/tool_reservation.html
+-rw-rw-rw-   0 root         (0) root         (0)     1271 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/kiosk/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    13554 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/apps/kiosk/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.357472 NEMO-4.6.3/NEMO/apps/sensors/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/apps/sensors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7128 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/sensors/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      567 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/sensors/customizations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5237 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/sensors/evaluators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.357472 NEMO-4.6.3/NEMO/apps/sensors/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/apps/sensors/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.357472 NEMO-4.6.3/NEMO/apps/sensors/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/apps/sensors/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/sensors/management/commands/manage_sensor_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.358471 NEMO-4.6.3/NEMO/apps/sensors/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     7794 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/sensors/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/apps/sensors/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13007 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/sensors/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     4906 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/sensors/sensors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.332471 NEMO-4.6.3/NEMO/apps/sensors/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.360472 NEMO-4.6.3/NEMO/apps/sensors/static/sensors/
+-rw-rw-rw-   0 root         (0) root         (0)   408236 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/sensors/static/sensors/chart.js
+-rw-rw-rw-   0 root         (0) root         (0)   195090 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/sensors/static/sensors/chart.min.js
+-rw-rw-rw-   0 root         (0) root         (0)     1376 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/sensors/static/sensors/chartjs-adapter-moment.js
+-rw-rw-rw-   0 root         (0) root         (0)     7659 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/sensors/static/sensors/daterangepicker.css
+-rw-rw-rw-   0 root         (0) root         (0)    66305 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/sensors/static/sensors/daterangepicker.js
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/sensors/static/sensors/sensors.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.333471 NEMO-4.6.3/NEMO/apps/sensors/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.361472 NEMO-4.6.3/NEMO/apps/sensors/templates/customizations/
+-rw-rw-rw-   0 root         (0) root         (0)     4718 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/sensors/templates/customizations/customizations_sensors.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.361472 NEMO-4.6.3/NEMO/apps/sensors/templates/sensors/
+-rw-rw-rw-   0 root         (0) root         (0)      347 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/sensors/templates/sensors/sensor_alerts.html
+-rw-rw-rw-   0 root         (0) root         (0)    15165 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/sensors/templates/sensors/sensor_data.html
+-rw-rw-rw-   0 root         (0) root         (0)     3879 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/sensors/templates/sensors/sensors.html
+-rw-rw-rw-   0 root         (0) root         (0)      790 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/sensors/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     5650 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/apps/sensors/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     3966 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/context_processors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5776 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3833 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    14341 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)    17784 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/interlocks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.362471 NEMO-4.6.3/NEMO/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.363472 NEMO-4.6.3/NEMO/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/management/commands/cancel_unused_reservations.py
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/management/commands/create_closure_alerts.py
+-rw-rw-rw-   0 root         (0) root         (0)      376 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/management/commands/manage_recurring_charges.py
+-rw-rw-rw-   0 root         (0) root         (0)      431 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/management/commands/manage_tool_qualifications.py
+-rw-rw-rw-   0 root         (0) root         (0)      417 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/management/commands/send_email_out_of_time_reservation_notification.py
+-rw-rw-rw-   0 root         (0) root         (0)      415 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/management/commands/send_email_reservation_ending_reminders.py
+-rw-rw-rw-   0 root         (0) root         (0)      408 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/management/commands/send_email_reservation_reminders.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/management/commands/send_email_usage_reminders.py
+-rw-rw-rw-   0 root         (0) root         (0)      456 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/management/commands/send_email_user_access_expiration_reminders.py
+-rw-rw-rw-   0 root         (0) root         (0)      406 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/management/commands/send_email_weekend_access_notification.py
+-rw-rw-rw-   0 root         (0) root         (0)     5578 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.368472 NEMO-4.6.3/NEMO/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    50307 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations/0001_version_1_0_0.py
+-rw-rw-rw-   0 root         (0) root         (0)    32962 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations/0002_version_1_0_0_squashed.py
+-rw-rw-rw-   0 root         (0) root         (0)     7988 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations/0012_version_2_0_0_squashed.py
+-rw-rw-rw-   0 root         (0) root         (0)     9904 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations/0020_version_3_0_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     1712 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations/0021_version_3_1_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations/0022_version_3_3_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      913 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations/0023_badgereader.py
+-rw-rw-rw-   0 root         (0) root         (0)      705 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations/0024_contactinformation_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     2674 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations/0025_version_3_6_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     5405 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations/0026_version_3_7_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations/0027_version_3_8_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     2231 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations/0028_version_3_9_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     1127 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations/0030_version_3_9_2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2785 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations/0031_version_3_10_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     3166 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations/0032_version_3_11_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      380 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations/0033_version_3_12_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations/0034_version_3_13_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     6747 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations/0035_version_3_14_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     7792 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations/0036_version_3_15_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     3717 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations/0037_version_3_16_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      935 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations/0038_version_4_0_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     3601 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations/0039_version_4_1_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     2444 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations/0040_version_4_2_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      487 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations/0041_version_4_2_1.py
+-rw-rw-rw-   0 root         (0) root         (0)    16447 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations/0042_version_4_3_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      524 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations/0043_version_4_3_2.py
+-rw-rw-rw-   0 root         (0) root         (0)     5416 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations/0044_version_4_4_0.py
+-rw-rw-rw-   0 root         (0) root         (0)    13447 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations/0045_version_4_5_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     2037 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations/0045_version_4_5_5.py
+-rw-rw-rw-   0 root         (0) root         (0)     2997 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations/0046_version_4_6_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-07-25 22:28:19.000000 NEMO-4.6.3/NEMO/migrations/0047_version_4_6_1.py
+-rw-rw-rw-   0 root         (0) root         (0)      607 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/migrations/0048_version_4_6_3.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2299 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/migrations_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     7993 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)     3855 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/model_tree.py
+-rw-rw-rw-   0 root         (0) root         (0)   148419 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1429 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)    49842 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/policy.py
+-rw-rw-rw-   0 root         (0) root         (0)     9943 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/provisioning.py
+-rw-rw-rw-   0 root         (0) root         (0)     5646 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/rates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1037 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/rest_filter_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)    11173 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/serializers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.373472 NEMO-4.6.3/NEMO/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.373472 NEMO-4.6.3/NEMO/static/admin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.373472 NEMO-4.6.3/NEMO/static/admin/physical_access_level/
+-rw-rw-rw-   0 root         (0) root         (0)      607 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/admin/physical_access_level/access_level.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.374472 NEMO-4.6.3/NEMO/static/admin/questions_preview/
+-rw-rw-rw-   0 root         (0) root         (0)     4122 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/admin/questions_preview/questions_preview.css
+-rw-rw-rw-   0 root         (0) root         (0)     1372 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/admin/questions_preview/questions_preview.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.374472 NEMO-4.6.3/NEMO/static/admin/reservation_questions/
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/admin/reservation_questions/reservation_questions.js
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/admin/time_options_override.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.374472 NEMO-4.6.3/NEMO/static/admin/tool/
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/admin/tool/tool.js
+-rw-rw-rw-   0 root         (0) root         (0)     1515 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/badge_reader.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.334471 NEMO-4.6.3/NEMO/static/bootstrap/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.375472 NEMO-4.6.3/NEMO/static/bootstrap/css/
+-rw-rw-rw-   0 root         (0) root         (0)    22608 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/bootstrap/css/bootstrap-theme.css
+-rw-rw-rw-   0 root         (0) root         (0)    43339 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/bootstrap/css/bootstrap-theme.css.map
+-rw-rw-rw-   0 root         (0) root         (0)    19963 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/bootstrap/css/bootstrap-theme.min.css
+-rw-rw-rw-   0 root         (0) root         (0)   141622 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/bootstrap/css/bootstrap.css
+-rw-rw-rw-   0 root         (0) root         (0)   380986 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/bootstrap/css/bootstrap.css.map
+-rw-rw-rw-   0 root         (0) root         (0)   117305 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.377472 NEMO-4.6.3/NEMO/static/bootstrap/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)    20127 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.eot
+-rw-rw-rw-   0 root         (0) root         (0)   108738 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.svg
+-rw-rw-rw-   0 root         (0) root         (0)    45404 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)    23424 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff
+-rw-rw-rw-   0 root         (0) root         (0)    18028 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.377472 NEMO-4.6.3/NEMO/static/bootstrap/js/
+-rw-rw-rw-   0 root         (0) root         (0)    67546 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/bootstrap/js/bootstrap.js
+-rw-rw-rw-   0 root         (0) root         (0)    35951 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/bootstrap/js/bootstrap.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.377472 NEMO-4.6.3/NEMO/static/datetimepicker/
+-rw-rw-rw-   0 root         (0) root         (0)     9020 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/datetimepicker/bootstrap-datetimepicker.css
+-rw-rw-rw-   0 root         (0) root         (0)   105978 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/datetimepicker/bootstrap-datetimepicker.js
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.379472 NEMO-4.6.3/NEMO/static/fullcalendar/
+-rw-rw-rw-   0 root         (0) root         (0)    28531 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/fullcalendar/fullcalendar.css
+-rw-rw-rw-   0 root         (0) root         (0)   357749 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/fullcalendar/fullcalendar.js
+-rw-rw-rw-   0 root         (0) root         (0)    13687 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/fullcalendar/fullcalendar.min.css
+-rw-rw-rw-   0 root         (0) root         (0)   168700 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/fullcalendar/fullcalendar.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.379472 NEMO-4.6.3/NEMO/static/icons/
+-rw-rw-rw-   0 root         (0) root         (0)    24065 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/icons/agreement.png
+-rw-rw-rw-   0 root         (0) root         (0)    16685 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/icons/caution.png
+-rw-rw-rw-   0 root         (0) root         (0)     4664 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/icons/preferences.png
+-rw-rw-rw-   0 root         (0) root         (0)   247387 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/jquery.js
+-rw-rw-rw-   0 root         (0) root         (0)    84320 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/jquery.min.js
+-rw-rw-rw-   0 root         (0) root         (0)  1183392 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/jumbotron_watermark.bmp
+-rw-rw-rw-   0 root         (0) root         (0)     1017 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/mobile.js
+-rw-rw-rw-   0 root         (0) root         (0)   174603 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/moment.js
+-rw-rw-rw-   0 root         (0) root         (0)    58102 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/moment.min.js
+-rw-rw-rw-   0 root         (0) root         (0)    86041 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/moment.min.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    18266 2023-07-26 20:15:15.000000 NEMO-4.6.3/NEMO/static/nemo.css
+-rw-rw-rw-   0 root         (0) root         (0)    21828 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/nemo.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.380472 NEMO-4.6.3/NEMO/static/numpad/
+-rw-rw-rw-   0 root         (0) root         (0)    12285 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/numpad/custom_numpad.jquery.js
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/numpad/numpad.jquery.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.381472 NEMO-4.6.3/NEMO/static/pickadate/
+-rw-rw-rw-   0 root         (0) root         (0)     3795 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/pickadate/default.css
+-rw-rw-rw-   0 root         (0) root         (0)     6040 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/pickadate/default.date.css
+-rw-rw-rw-   0 root         (0) root         (0)     2785 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/pickadate/default.time.css
+-rw-rw-rw-   0 root         (0) root         (0)    48215 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/pickadate/picker.date.js
+-rw-rw-rw-   0 root         (0) root         (0)    36941 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/pickadate/picker.js
+-rw-rw-rw-   0 root         (0) root         (0)    31899 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/pickadate/picker.time.js
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/robots.txt
+-rw-rw-rw-   0 root         (0) root         (0)    48446 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/typeahead.jquery.js
+-rw-rw-rw-   0 root         (0) root         (0)    20748 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/typeahead.jquery.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.382472 NEMO-4.6.3/NEMO/static/virtualkeyboard/
+-rw-rw-rw-   0 root         (0) root         (0)   113008 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/virtualkeyboard/jquery.keyboard.js
+-rw-rw-rw-   0 root         (0) root         (0)    47325 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/virtualkeyboard/jquery.keyboard.min.js
+-rw-rw-rw-   0 root         (0) root         (0)     7848 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/virtualkeyboard/keyboard-basic.css
+-rw-rw-rw-   0 root         (0) root         (0)     5889 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/static/virtualkeyboard/keyboard-basic.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.384472 NEMO-4.6.3/NEMO/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.384472 NEMO-4.6.3/NEMO/templates/abuse/
+-rw-rw-rw-   0 root         (0) root         (0)     4059 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/abuse/abuse.html
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/abuse/user_drill_down.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.385472 NEMO-4.6.3/NEMO/templates/accounts_and_projects/
+-rw-rw-rw-   0 root         (0) root         (0)     7665 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/accounts_and_projects/account_and_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)     6409 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/accounts_and_projects/accounts_and_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)     2843 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/accounts_and_projects/create_account.html
+-rw-rw-rw-   0 root         (0) root         (0)     6693 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/accounts_and_projects/create_project.html
+-rw-rw-rw-   0 root         (0) root         (0)      888 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/accounts_and_projects/documents_for_project.html
+-rw-rw-rw-   0 root         (0) root         (0)     3544 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/accounts_and_projects/projects.html
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/accounts_and_projects/users_for_project.html
+-rw-rw-rw-   0 root         (0) root         (0)      433 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/acknowledgement.html
+-rw-rw-rw-   0 root         (0) root         (0)     4694 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/alerts.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.386472 NEMO-4.6.3/NEMO/templates/area_access/
+-rw-rw-rw-   0 root         (0) root         (0)     2951 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/area_access/area_access.html
+-rw-rw-rw-   0 root         (0) root         (0)     1748 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/area_access/calendar_self_login.html
+-rw-rw-rw-   0 root         (0) root         (0)     1111 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/area_access/change_project.html
+-rw-rw-rw-   0 root         (0) root         (0)     1141 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/area_access/login_areas.html
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/area_access/new_area_access_record.html
+-rw-rw-rw-   0 root         (0) root         (0)     1938 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/area_access/new_area_access_record_details.html
+-rw-rw-rw-   0 root         (0) root         (0)     1454 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/area_access/self_login.html
+-rw-rw-rw-   0 root         (0) root         (0)      837 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/authorization_failed.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.387472 NEMO-4.6.3/NEMO/templates/base/
+-rw-rw-rw-   0 root         (0) root         (0)      308 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/base/footer.html
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/base/impersonate_header.html
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/base/navbar.html
+-rw-rw-rw-   0 root         (0) root         (0)     8117 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/base/navbar_base.html
+-rw-rw-rw-   0 root         (0) root         (0)      308 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/base/popup.html
+-rw-rw-rw-   0 root         (0) root         (0)     6174 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.389472 NEMO-4.6.3/NEMO/templates/calendar/
+-rw-rw-rw-   0 root         (0) root         (0)    24673 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/calendar/calendar.html
+-rw-rw-rw-   0 root         (0) root         (0)     1442 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/calendar/configuration.html
+-rw-rw-rw-   0 root         (0) root         (0)     2834 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/calendar/configuration_helper.html
+-rw-rw-rw-   0 root         (0) root         (0)     1315 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/calendar/policy_dialog.html
+-rw-rw-rw-   0 root         (0) root         (0)     1361 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/calendar/project_choice.html
+-rw-rw-rw-   0 root         (0) root         (0)     1512 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/calendar/proxy_reservation.html
+-rw-rw-rw-   0 root         (0) root         (0)     1862 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/calendar/reservation_event_feed.html
+-rw-rw-rw-   0 root         (0) root         (0)     1680 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/calendar/reservation_questions.html
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/calendar/reservation_warning.html
+-rw-rw-rw-   0 root         (0) root         (0)     4410 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/calendar/scheduled_outage_information.html
+-rw-rw-rw-   0 root         (0) root         (0)     2011 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/calendar/specific_user_feed.html
+-rw-rw-rw-   0 root         (0) root         (0)     2543 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/calendar/usage_event_feed.html
+-rw-rw-rw-   0 root         (0) root         (0)     6530 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/configuration_agenda.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.389472 NEMO-4.6.3/NEMO/templates/consumables/
+-rw-rw-rw-   0 root         (0) root         (0)     8224 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/consumables/consumables.html
+-rw-rw-rw-   0 root         (0) root         (0)     1538 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/consumables/consumables_order.html
+-rw-rw-rw-   0 root         (0) root         (0)    11695 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/consumables/recurring_charge.html
+-rw-rw-rw-   0 root         (0) root         (0)     5473 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/consumables/recurring_charges.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.389472 NEMO-4.6.3/NEMO/templates/contact/
+-rw-rw-rw-   0 root         (0) root         (0)      692 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/contact/contact_staff.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.392472 NEMO-4.6.3/NEMO/templates/customizations/
+-rw-rw-rw-   0 root         (0) root         (0)     1848 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/customizations/customizations.html
+-rw-rw-rw-   0 root         (0) root         (0)     4882 2023-07-25 22:28:19.000000 NEMO-4.6.3/NEMO/templates/customizations/customizations_application.html
+-rw-rw-rw-   0 root         (0) root         (0)     7799 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/customizations/customizations_calendar.html
+-rw-rw-rw-   0 root         (0) root         (0)     7634 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/customizations/customizations_dashboard.html
+-rw-rw-rw-   0 root         (0) root         (0)     4202 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/customizations/customizations_emails.html
+-rw-rw-rw-   0 root         (0) root         (0)     2545 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/customizations/customizations_interlock.html
+-rw-rw-rw-   0 root         (0) root         (0)     5553 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/customizations/customizations_projects_and_accounts.html
+-rw-rw-rw-   0 root         (0) root         (0)     2224 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/customizations/customizations_rates.html
+-rw-rw-rw-   0 root         (0) root         (0)     3519 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/customizations/customizations_recurring_charges.html
+-rw-rw-rw-   0 root         (0) root         (0)     2183 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/customizations/customizations_remote_work.html
+-rw-rw-rw-   0 root         (0) root         (0)    16717 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/customizations/customizations_requests.html
+-rw-rw-rw-   0 root         (0) root         (0)     3678 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/customizations/customizations_safety.html
+-rw-rw-rw-   0 root         (0) root         (0)    27806 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/customizations/customizations_templates.html
+-rw-rw-rw-   0 root         (0) root         (0)     9253 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/customizations/customizations_tool.html
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/customizations/customizations_upload.html
+-rw-rw-rw-   0 root         (0) root         (0)     5214 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/customizations/customizations_user.html
+-rw-rw-rw-   0 root         (0) root         (0)      502 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/display_success_and_redirect.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.392472 NEMO-4.6.3/NEMO/templates/email/
+-rw-rw-rw-   0 root         (0) root         (0)     7825 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/email/compose_email.html
+-rw-rw-rw-   0 root         (0) root         (0)     3153 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/email/email_broadcast.html
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/email/email_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.393472 NEMO-4.6.3/NEMO/templates/event_details/
+-rw-rw-rw-   0 root         (0) root         (0)      751 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/event_details/area_access_details.html
+-rw-rw-rw-   0 root         (0) root         (0)     1376 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/event_details/outage_details.html
+-rw-rw-rw-   0 root         (0) root         (0)    12242 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/event_details/reservation_details.html
+-rw-rw-rw-   0 root         (0) root         (0)      589 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/event_details/usage_details.html
+-rw-rw-rw-   0 root         (0) root         (0)      426 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/facility_rules.html
+-rw-rw-rw-   0 root         (0) root         (0)     1247 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/feedback.html
+-rw-rw-rw-   0 root         (0) root         (0)      937 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/history.html
+-rw-rw-rw-   0 root         (0) root         (0)     1260 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/impersonate.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.393472 NEMO-4.6.3/NEMO/templates/jumbotron/
+-rw-rw-rw-   0 root         (0) root         (0)     2059 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/jumbotron/jumbotron.html
+-rw-rw-rw-   0 root         (0) root         (0)     3832 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/templates/jumbotron/jumbotron_content.html
+-rw-rw-rw-   0 root         (0) root         (0)     8670 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/landing.html
+-rw-rw-rw-   0 root         (0) root         (0)     3496 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/login.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.394472 NEMO-4.6.3/NEMO/templates/maintenance/
+-rw-rw-rw-   0 root         (0) root         (0)     1558 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/maintenance/closed_task_details.html
+-rw-rw-rw-   0 root         (0) root         (0)     5566 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/maintenance/maintenance.html
+-rw-rw-rw-   0 root         (0) root         (0)     7450 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/maintenance/pending_task_details.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.395472 NEMO-4.6.3/NEMO/templates/mobile/
+-rw-rw-rw-   0 root         (0) root         (0)      762 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/mobile/cancellation_result.html
+-rw-rw-rw-   0 root         (0) root         (0)     1916 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/mobile/choose_item.html
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/mobile/error.html
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/mobile/individual_outage.html
+-rw-rw-rw-   0 root         (0) root         (0)     2625 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/mobile/individual_reservation.html
+-rw-rw-rw-   0 root         (0) root         (0)     5899 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/mobile/new_reservation.html
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/mobile/no_active_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)      777 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/mobile/reservation_success.html
+-rw-rw-rw-   0 root         (0) root         (0)     1442 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/mobile/view_calendar.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.395472 NEMO-4.6.3/NEMO/templates/news/
+-rw-rw-rw-   0 root         (0) root         (0)      981 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/news/archived_news.html
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/news/new_news_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     1198 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/news/news_update_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     2038 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/news/recent_news.html
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/no_project.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.396472 NEMO-4.6.3/NEMO/templates/occupancy/
+-rw-rw-rw-   0 root         (0) root         (0)      487 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/templates/occupancy/occupancy.html
+-rw-rw-rw-   0 root         (0) root         (0)     1811 2023-07-26 20:15:15.000000 NEMO-4.6.3/NEMO/templates/occupancy/occupancy_content.html
+-rw-rw-rw-   0 root         (0) root         (0)     1147 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/occupancy/occupancy_count.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.396472 NEMO-4.6.3/NEMO/templates/pagination/
+-rw-rw-rw-   0 root         (0) root         (0)      865 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/pagination/pagination_base.html
+-rw-rw-rw-   0 root         (0) root         (0)      521 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/pagination/pagination_column.html
+-rw-rw-rw-   0 root         (0) root         (0)      673 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/pagination/pagination_pages.html
+-rw-rw-rw-   0 root         (0) root         (0)      642 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/pagination/pagination_selector.html
+-rw-rw-rw-   0 root         (0) root         (0)     2841 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/qualifications.html
+-rw-rw-rw-   0 root         (0) root         (0)     5462 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/refresh_sidebar_icons.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.397472 NEMO-4.6.3/NEMO/templates/remote_work/
+-rw-rw-rw-   0 root         (0) root         (0)    10616 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/remote_work/remote_work.html
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/remote_work/remote_work_base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.397472 NEMO-4.6.3/NEMO/templates/requests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.397472 NEMO-4.6.3/NEMO/templates/requests/access_requests/
+-rw-rw-rw-   0 root         (0) root         (0)     7754 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/requests/access_requests/access_request.html
+-rw-rw-rw-   0 root         (0) root         (0)     3450 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/requests/access_requests/access_requests.html
+-rw-rw-rw-   0 root         (0) root         (0)     3480 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/requests/access_requests/access_requests_table.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.398472 NEMO-4.6.3/NEMO/templates/requests/adjustment_requests/
+-rw-rw-rw-   0 root         (0) root         (0)     8607 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/requests/adjustment_requests/adjustment_request.html
+-rw-rw-rw-   0 root         (0) root         (0)     3733 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/requests/adjustment_requests/adjustment_requests.html
+-rw-rw-rw-   0 root         (0) root         (0)     7257 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/requests/adjustment_requests/adjustment_requests_table.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.398472 NEMO-4.6.3/NEMO/templates/requests/buddy_requests/
+-rw-rw-rw-   0 root         (0) root         (0)     3910 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/requests/buddy_requests/buddy_request.html
+-rw-rw-rw-   0 root         (0) root         (0)     5602 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/requests/buddy_requests/buddy_requests.html
+-rw-rw-rw-   0 root         (0) root         (0)     4246 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/requests/user_requests.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.399472 NEMO-4.6.3/NEMO/templates/resources/
+-rw-rw-rw-   0 root         (0) root         (0)     2950 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/resources/modify_resource.html
+-rw-rw-rw-   0 root         (0) root         (0)     3846 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/resources/resource_details.html
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/resources/resources.html
+-rw-rw-rw-   0 root         (0) root         (0)     3898 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/resources/scheduled_outage.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.399472 NEMO-4.6.3/NEMO/templates/rest_framework/
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/rest_framework/api.html
+-rw-rw-rw-   0 root         (0) root         (0)      446 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/rest_framework/custom_error.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.400472 NEMO-4.6.3/NEMO/templates/safety/
+-rw-rw-rw-   0 root         (0) root         (0)     3112 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/safety/safety.html
+-rw-rw-rw-   0 root         (0) root         (0)     1733 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/safety/safety_base.html
+-rw-rw-rw-   0 root         (0) root         (0)     7807 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/safety/safety_data_sheets.html
+-rw-rw-rw-   0 root         (0) root         (0)     1976 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/safety/safety_issues.html
+-rw-rw-rw-   0 root         (0) root         (0)     1723 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/safety/safety_issues_create.html
+-rw-rw-rw-   0 root         (0) root         (0)     1722 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/safety/safety_issues_resolved.html
+-rw-rw-rw-   0 root         (0) root         (0)     1762 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/safety/safety_issues_update.html
+-rw-rw-rw-   0 root         (0) root         (0)     1877 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/safety/safety_items.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.401472 NEMO-4.6.3/NEMO/templates/snippets/
+-rw-rw-rw-   0 root         (0) root         (0)      516 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/snippets/button.html
+-rw-rw-rw-   0 root         (0) root         (0)      904 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/snippets/contact_person.html
+-rw-rw-rw-   0 root         (0) root         (0)      962 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/snippets/document_list.html
+-rw-rw-rw-   0 root         (0) root         (0)     1128 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/snippets/embedded_document.html
+-rw-rw-rw-   0 root         (0) root         (0)     1673 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/snippets/tool_info.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.402472 NEMO-4.6.3/NEMO/templates/staff_charges/
+-rw-rw-rw-   0 root         (0) root         (0)      860 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/staff_charges/change_status.html
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/staff_charges/choose_project.html
+-rw-rw-rw-   0 root         (0) root         (0)      498 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/staff_charges/end_area_charge.html
+-rw-rw-rw-   0 root         (0) root         (0)     1198 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/staff_charges/new_staff_charge.html
+-rw-rw-rw-   0 root         (0) root         (0)     1014 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/staff_charges/reminder.html
+-rw-rw-rw-   0 root         (0) root         (0)     1854 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/staff_charges/staff_charges_base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.402472 NEMO-4.6.3/NEMO/templates/status_dashboard/
+-rw-rw-rw-   0 root         (0) root         (0)     1633 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/templates/status_dashboard/occupancy.html
+-rw-rw-rw-   0 root         (0) root         (0)     9772 2023-07-25 22:28:19.000000 NEMO-4.6.3/NEMO/templates/status_dashboard/staff.html
+-rw-rw-rw-   0 root         (0) root         (0)     7709 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/status_dashboard/staff_absence.html
+-rw-rw-rw-   0 root         (0) root         (0)     6650 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/status_dashboard/status_dashboard.html
+-rw-rw-rw-   0 root         (0) root         (0)     3717 2023-07-26 20:15:15.000000 NEMO-4.6.3/NEMO/templates/status_dashboard/tools.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.403472 NEMO-4.6.3/NEMO/templates/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)     2542 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/tasks/resolve.html
+-rw-rw-rw-   0 root         (0) root         (0)     5037 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/tasks/update.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.404472 NEMO-4.6.3/NEMO/templates/tool_control/
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/tool_control/get_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)      737 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/tool_control/interlock_error.html
+-rw-rw-rw-   0 root         (0) root         (0)     3502 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/tool_control/past_tasks_and_comments.html
+-rw-rw-rw-   0 root         (0) root         (0)     2466 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/tool_control/qualified_users.html
+-rw-rw-rw-   0 root         (0) root         (0)    15303 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/tool_control/tool_control.html
+-rw-rw-rw-   0 root         (0) root         (0)    37737 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/tool_control/tool_status.html
+-rw-rw-rw-   0 root         (0) root         (0)     6142 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/tool_control/usage_data.html
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/tool_control/use_tool_for_other.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.404472 NEMO-4.6.3/NEMO/templates/training/
+-rw-rw-rw-   0 root         (0) root         (0)      512 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/training/get_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)     4971 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/training/training.html
+-rw-rw-rw-   0 root         (0) root         (0)     1962 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/training/training_entry.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.405472 NEMO-4.6.3/NEMO/templates/usage/
+-rw-rw-rw-   0 root         (0) root         (0)      976 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/usage/adjustment_request_button.html
+-rw-rw-rw-   0 root         (0) root         (0)     3573 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/usage/billing.html
+-rw-rw-rw-   0 root         (0) root         (0)     9218 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/usage/usage.html
+-rw-rw-rw-   0 root         (0) root         (0)     7812 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/usage/usage_base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.406472 NEMO-4.6.3/NEMO/templates/users/
+-rw-rw-rw-   0 root         (0) root         (0)    20776 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/users/create_or_modify_user.html
+-rw-rw-rw-   0 root         (0) root         (0)    20758 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/templates/users/preferences.html
+-rw-rw-rw-   0 root         (0) root         (0)     3758 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/users/safe_deactivation.html
+-rw-rw-rw-   0 root         (0) root         (0)     4181 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templates/users/users.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.406472 NEMO-4.6.3/NEMO/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8447 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/templatetags/custom_tags_and_filters.py
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)    26303 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    24695 2023-07-25 22:28:19.000000 NEMO-4.6.3/NEMO/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.413472 NEMO-4.6.3/NEMO/views/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4308 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/abuse.py
+-rw-rw-rw-   0 root         (0) root         (0)    14733 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/access_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)     8275 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/accounts_and_projects.py
+-rw-rw-rw-   0 root         (0) root         (0)    19797 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/views/adjustment_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)     1812 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/alerts.py
+-rw-rw-rw-   0 root         (0) root         (0)    14004 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    12252 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/api_billing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2415 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/api_file_import.py
+-rw-rw-rw-   0 root         (0) root         (0)    19170 2023-07-26 20:15:15.000000 NEMO-4.6.3/NEMO/views/area_access.py
+-rw-rw-rw-   0 root         (0) root         (0)    12070 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     6625 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/buddy_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)    71831 2023-07-25 22:28:19.000000 NEMO-4.6.3/NEMO/views/calendar.py
+-rw-rw-rw-   0 root         (0) root         (0)     2334 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/charge_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/configuration_agenda.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    10972 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/views/consumables.py
+-rw-rw-rw-   0 root         (0) root         (0)      467 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/contact_staff.py
+-rw-rw-rw-   0 root         (0) root         (0)    18748 2023-07-25 22:28:19.000000 NEMO-4.6.3/NEMO/views/customization.py
+-rw-rw-rw-   0 root         (0) root         (0)     3442 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/documents.py
+-rw-rw-rw-   0 root         (0) root         (0)    10015 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/email.py
+-rw-rw-rw-   0 root         (0) root         (0)     1973 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/event_details.py
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/feedback.py
+-rw-rw-rw-   0 root         (0) root         (0)     1672 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/get_projects.py
+-rw-rw-rw-   0 root         (0) root         (0)     4168 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/history.py
+-rw-rw-rw-   0 root         (0) root         (0)     1155 2023-07-26 20:15:15.000000 NEMO-4.6.3/NEMO/views/jumbotron.py
+-rw-rw-rw-   0 root         (0) root         (0)     3293 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/landing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2718 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/maintenance.py
+-rw-rw-rw-   0 root         (0) root         (0)     8072 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/mobile.py
+-rw-rw-rw-   0 root         (0) root         (0)     3356 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/news.py
+-rw-rw-rw-   0 root         (0) root         (0)     5095 2023-07-25 22:28:19.000000 NEMO-4.6.3/NEMO/views/notifications.py
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)     4822 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/qualifications.py
+-rw-rw-rw-   0 root         (0) root         (0)     9506 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/remote_work.py
+-rw-rw-rw-   0 root         (0) root         (0)     3700 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/resources.py
+-rw-rw-rw-   0 root         (0) root         (0)     8877 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/safety.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/sidebar.py
+-rw-rw-rw-   0 root         (0) root         (0)    20549 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/views/status_dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)    13615 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)    24092 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/views/tool_control.py
+-rw-rw-rw-   0 root         (0) root         (0)     6043 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/training.py
+-rw-rw-rw-   0 root         (0) root         (0)     1909 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/tutorials.py
+-rw-rw-rw-   0 root         (0) root         (0)    18360 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/usage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1049 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/user_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)    20715 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/views/users.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.414472 NEMO-4.6.3/NEMO/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/widgets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2968 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/widgets/configuration_editor.py
+-rw-rw-rw-   0 root         (0) root         (0)    26102 2023-07-28 21:19:09.000000 NEMO-4.6.3/NEMO/widgets/dynamic_form.py
+-rw-rw-rw-   0 root         (0) root         (0)     8029 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/widgets/item_tree.py
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-07-18 17:03:12.000000 NEMO-4.6.3/NEMO/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.345471 NEMO-4.6.3/NEMO.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      904 2023-07-28 21:19:22.000000 NEMO-4.6.3/NEMO.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    17451 2023-07-28 21:19:22.000000 NEMO-4.6.3/NEMO.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 21:19:22.000000 NEMO-4.6.3/NEMO.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-28 21:19:22.000000 NEMO-4.6.3/NEMO.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      264 2023-07-28 21:19:22.000000 NEMO-4.6.3/NEMO.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-28 21:19:22.000000 NEMO-4.6.3/NEMO.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      904 2023-07-28 21:19:22.414472 NEMO-4.6.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4066 2023-07-18 17:03:12.000000 NEMO-4.6.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:19:22.414472 NEMO-4.6.3/resources/
+-rw-rw-rw-   0 root         (0) root         (0)    17163 2023-07-25 22:28:19.000000 NEMO-4.6.3/resources/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     3981 2023-07-18 17:03:12.000000 NEMO-4.6.3/resources/splash_pad_settings.py
+-rw-r--r--   0 root         (0) root         (0)      109 2023-07-28 21:19:22.415472 NEMO-4.6.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-07-28 21:19:09.000000 NEMO-4.6.3/setup.py
```

### Comparing `NEMO-4.6.2/LICENSE.md` & `NEMO-4.6.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/__init__.py` & `NEMO-4.6.3/NEMO/__init__.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/actions.py` & `NEMO-4.6.3/NEMO/actions.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/admin.py` & `NEMO-4.6.3/NEMO/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -868,15 +868,15 @@
 	list_display = ("name",)
 
 
 @register(UserPreferences)
 class UserPreferencesAdmin(admin.ModelAdmin):
 	list_display = ("user",)
 	search_fields = ["user_preferences__user__first_name", "user_preferences__user__last_name", "user_preferences__user__username"]
-	filter_horizontal = ["tool_freed_time_notifications", "tool_adjustment_notifications"]
+	filter_horizontal = ["tool_freed_time_notifications", "tool_adjustment_notifications", "area_adjustment_notifications"]
 	form = UserPreferencesForm
 
 
 class UserAdminForm(forms.ModelForm):
 	class Meta:
 		model = User
 		fields = "__all__"
```

### Comparing `NEMO-4.6.2/NEMO/apps/area_access/templates/area_access/already_logged_in.html` & `NEMO-4.6.3/NEMO/apps/area_access/templates/area_access/already_logged_in.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/area_access/templates/area_access/base.html` & `NEMO-4.6.3/NEMO/apps/area_access/templates/area_access/base.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/area_access/templates/area_access/choose_project.html` & `NEMO-4.6.3/NEMO/apps/area_access/templates/area_access/choose_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/area_access/templates/area_access/logout_warning.html` & `NEMO-4.6.3/NEMO/apps/area_access/templates/area_access/logout_warning.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/area_access/templates/area_access/resource_unavailable.html` & `NEMO-4.6.3/NEMO/apps/area_access/templates/area_access/resource_unavailable.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/area_access/urls.py` & `NEMO-4.6.3/NEMO/apps/area_access/urls.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/area_access/views.py` & `NEMO-4.6.3/NEMO/apps/area_access/views.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/contracts/admin.py` & `NEMO-4.6.3/NEMO/apps/contracts/admin.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/contracts/migrations/0001_initial.py` & `NEMO-4.6.3/NEMO/apps/contracts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/contracts/models.py` & `NEMO-4.6.3/NEMO/apps/contracts/models.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/contracts/templates/contracts/contractors.html` & `NEMO-4.6.3/NEMO/apps/contracts/templates/contracts/contractors.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/contracts/templates/contracts/contracts_and_procurements.html` & `NEMO-4.6.3/NEMO/apps/contracts/templates/contracts/contracts_and_procurements.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/contracts/templates/contracts/procurements.html` & `NEMO-4.6.3/NEMO/apps/contracts/templates/contracts/procurements.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/contracts/templates/contracts/service_contracts.html` & `NEMO-4.6.3/NEMO/apps/contracts/templates/contracts/service_contracts.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/contracts/templates/customizations/customizations_contracts.html` & `NEMO-4.6.3/NEMO/apps/contracts/templates/customizations/customizations_contracts.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/contracts/urls.py` & `NEMO-4.6.3/NEMO/apps/contracts/urls.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/contracts/views/contracts.py` & `NEMO-4.6.3/NEMO/apps/contracts/views/contracts.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/kiosk/templates/kiosk/category_choices.html` & `NEMO-4.6.3/NEMO/apps/kiosk/templates/kiosk/category_choices.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/kiosk/templates/kiosk/choices.html` & `NEMO-4.6.3/NEMO/apps/kiosk/templates/kiosk/choices.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/kiosk/templates/kiosk/error.html` & `NEMO-4.6.3/NEMO/apps/kiosk/templates/kiosk/error.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/kiosk/templates/kiosk/individual_reservation.html` & `NEMO-4.6.3/NEMO/apps/kiosk/templates/kiosk/individual_reservation.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/kiosk/templates/kiosk/kiosk.html` & `NEMO-4.6.3/NEMO/apps/kiosk/templates/kiosk/kiosk.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/kiosk/templates/kiosk/success.html` & `NEMO-4.6.3/NEMO/apps/kiosk/templates/kiosk/success.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/kiosk/templates/kiosk/tool_information.html` & `NEMO-4.6.3/NEMO/apps/kiosk/templates/kiosk/tool_information.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/kiosk/templates/kiosk/tool_project_selection_snippet.html` & `NEMO-4.6.3/NEMO/apps/kiosk/templates/kiosk/tool_project_selection_snippet.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/kiosk/templates/kiosk/tool_reservation.html` & `NEMO-4.6.3/NEMO/apps/kiosk/templates/kiosk/tool_reservation.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/kiosk/urls.py` & `NEMO-4.6.3/NEMO/apps/kiosk/urls.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/kiosk/views.py` & `NEMO-4.6.3/NEMO/apps/kiosk/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,19 +92,19 @@
 	if tool.interlock and not tool.interlock.lock():
 		if bypass_interlock and interlock_bypass_allowed(customer):
 			pass
 		else:
 			return interlock_error("Disable", customer)
 
 	# Shorten the user's tool reservation since we are now done using the tool
+	current_usage_event = tool.get_current_usage_event()
 	staff_shortening = request.POST.get("shorten", False)
-	shorten_reservation(user=customer, item=tool, new_end=timezone.now() + downtime, force=staff_shortening)
+	shorten_reservation(user=current_usage_event.user, item=tool, new_end=timezone.now() + downtime, force=staff_shortening)
 
 	# End the current usage event for the tool and save it.
-	current_usage_event = tool.get_current_usage_event()
 	current_usage_event.end = timezone.now() + downtime
 
 	# Collect post-usage questions
 	dynamic_form = DynamicForm(tool.post_usage_questions)
 
 	try:
 		current_usage_event.run_data = dynamic_form.extract(request)
@@ -113,21 +113,25 @@
 			# if a staff is forcing somebody off the tool and there are required questions, send an email and proceed
 			current_usage_event.run_data = e.run_data
 			email_managers_required_questions_disable_tool(current_usage_event.operator, customer, tool, e.questions)
 		else:
 			dictionary = {"message": str(e), "delay": 10}
 			return render(request, "kiosk/acknowledgement.html", dictionary)
 
-	dynamic_form.charge_for_consumables(
-		current_usage_event.user,
-		current_usage_event.operator,
-		current_usage_event.project,
-		current_usage_event.run_data,
-		request,
-	)
+	try:
+		dynamic_form.charge_for_consumables(
+			current_usage_event.user,
+			current_usage_event.operator,
+			current_usage_event.project,
+			current_usage_event.run_data,
+			request,
+		)
+	except Exception as e:
+		dictionary = {"message": str(e), "delay": 10}
+		return render(request, "kiosk/acknowledgement.html", dictionary)
 	dynamic_form.update_tool_counters(current_usage_event.run_data, tool.id)
 
 	current_usage_event.save()
 	dictionary = {"message": "You are no longer using the {}".format(tool), "badge_number": customer.badge_number}
 	return render(request, "kiosk/acknowledgement.html", dictionary)
```

### Comparing `NEMO-4.6.2/NEMO/apps/sensors/admin.py` & `NEMO-4.6.3/NEMO/apps/sensors/admin.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/sensors/customizations.py` & `NEMO-4.6.3/NEMO/apps/sensors/customizations.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/sensors/evaluators.py` & `NEMO-4.6.3/NEMO/apps/sensors/evaluators.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/sensors/migrations/0001_initial.py` & `NEMO-4.6.3/NEMO/apps/sensors/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/sensors/models.py` & `NEMO-4.6.3/NEMO/apps/sensors/models.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/sensors/sensors.py` & `NEMO-4.6.3/NEMO/apps/sensors/sensors.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/sensors/static/sensors/chart.js` & `NEMO-4.6.3/NEMO/apps/sensors/static/sensors/chart.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/sensors/static/sensors/chart.min.js` & `NEMO-4.6.3/NEMO/apps/sensors/static/sensors/chart.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/sensors/static/sensors/chartjs-adapter-moment.js` & `NEMO-4.6.3/NEMO/apps/sensors/static/sensors/chartjs-adapter-moment.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/sensors/static/sensors/daterangepicker.css` & `NEMO-4.6.3/NEMO/apps/sensors/static/sensors/daterangepicker.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/sensors/static/sensors/daterangepicker.js` & `NEMO-4.6.3/NEMO/apps/sensors/static/sensors/daterangepicker.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/sensors/static/sensors/sensors.css` & `NEMO-4.6.3/NEMO/apps/sensors/static/sensors/sensors.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/sensors/templates/customizations/customizations_sensors.html` & `NEMO-4.6.3/NEMO/apps/sensors/templates/customizations/customizations_sensors.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/sensors/templates/sensors/sensor_data.html` & `NEMO-4.6.3/NEMO/apps/sensors/templates/sensors/sensor_data.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/sensors/templates/sensors/sensors.html` & `NEMO-4.6.3/NEMO/apps/sensors/templates/sensors/sensors.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/sensors/urls.py` & `NEMO-4.6.3/NEMO/apps/sensors/urls.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/apps/sensors/views.py` & `NEMO-4.6.3/NEMO/apps/sensors/views.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/context_processors.py` & `NEMO-4.6.3/NEMO/context_processors.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/decorators.py` & `NEMO-4.6.3/NEMO/decorators.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/exceptions.py` & `NEMO-4.6.3/NEMO/exceptions.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/fields.py` & `NEMO-4.6.3/NEMO/fields.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/forms.py` & `NEMO-4.6.3/NEMO/forms.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from django.utils import timezone
 
 from NEMO.models import (
 	Account,
 	AdjustmentRequest,
 	Alert,
 	AlertCategory,
+	Area,
 	BuddyRequest,
 	Comment,
 	Consumable,
 	ConsumableWithdraw,
 	Project,
 	RecurringConsumableCharge,
 	ReservationItemType,
@@ -383,14 +384,15 @@
 		model = UserPreferences
 		fields = "__all__"
 
 	def __init__(self, *args, **kwargs):
 		super().__init__(*args, **kwargs)
 		self.fields["tool_freed_time_notifications"].queryset = Tool.objects.filter(visible=True, parent_tool__isnull=True)
 		self.fields["tool_adjustment_notifications"].queryset = Tool.objects.filter(visible=True, parent_tool__isnull=True)
+		self.fields["area_adjustment_notifications"].queryset = Area.objects.filter(area_children_set__isnull=True)
 		self.fields["tool_task_notifications"].queryset = Tool.objects.filter(visible=True, parent_tool__isnull=True)
 
 	def clean_recurring_charges_reminder_days(self):
 		recurring_charges_reminder_days = self.cleaned_data["recurring_charges_reminder_days"]
 		try:
 			for reminder_days in recurring_charges_reminder_days.split(","):
 				try:
```

### Comparing `NEMO-4.6.2/NEMO/interlocks.py` & `NEMO-4.6.3/NEMO/interlocks.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/management/commands/send_email_usage_reminders.py` & `NEMO-4.6.3/NEMO/management/commands/send_email_usage_reminders.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/middleware.py` & `NEMO-4.6.3/NEMO/middleware.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/migrations/0001_version_1_0_0.py` & `NEMO-4.6.3/NEMO/migrations/0001_version_1_0_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/migrations/0002_version_1_0_0_squashed.py` & `NEMO-4.6.3/NEMO/migrations/0002_version_1_0_0_squashed.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/migrations/0012_version_2_0_0_squashed.py` & `NEMO-4.6.3/NEMO/migrations/0012_version_2_0_0_squashed.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/migrations/0020_version_3_0_0.py` & `NEMO-4.6.3/NEMO/migrations/0020_version_3_0_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/migrations/0021_version_3_1_0.py` & `NEMO-4.6.3/NEMO/migrations/0021_version_3_1_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/migrations/0022_version_3_3_0.py` & `NEMO-4.6.3/NEMO/migrations/0022_version_3_3_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/migrations/0023_badgereader.py` & `NEMO-4.6.3/NEMO/migrations/0023_badgereader.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/migrations/0024_contactinformation_user.py` & `NEMO-4.6.3/NEMO/migrations/0024_contactinformation_user.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/migrations/0025_version_3_6_0.py` & `NEMO-4.6.3/NEMO/migrations/0025_version_3_6_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/migrations/0026_version_3_7_0.py` & `NEMO-4.6.3/NEMO/migrations/0026_version_3_7_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/migrations/0028_version_3_9_0.py` & `NEMO-4.6.3/NEMO/migrations/0028_version_3_9_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/migrations/0030_version_3_9_2.py` & `NEMO-4.6.3/NEMO/migrations/0030_version_3_9_2.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/migrations/0031_version_3_10_0.py` & `NEMO-4.6.3/NEMO/migrations/0031_version_3_10_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/migrations/0032_version_3_11_0.py` & `NEMO-4.6.3/NEMO/migrations/0032_version_3_11_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/migrations/0035_version_3_14_0.py` & `NEMO-4.6.3/NEMO/migrations/0035_version_3_14_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/migrations/0036_version_3_15_0.py` & `NEMO-4.6.3/NEMO/migrations/0036_version_3_15_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/migrations/0037_version_3_16_0.py` & `NEMO-4.6.3/NEMO/migrations/0037_version_3_16_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/migrations/0038_version_4_0_0.py` & `NEMO-4.6.3/NEMO/migrations/0038_version_4_0_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/migrations/0039_version_4_1_0.py` & `NEMO-4.6.3/NEMO/migrations/0039_version_4_1_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/migrations/0040_version_4_2_0.py` & `NEMO-4.6.3/NEMO/migrations/0040_version_4_2_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/migrations/0042_version_4_3_0.py` & `NEMO-4.6.3/NEMO/migrations/0042_version_4_3_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/migrations/0043_version_4_3_2.py` & `NEMO-4.6.3/NEMO/migrations/0043_version_4_3_2.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/migrations/0044_version_4_4_0.py` & `NEMO-4.6.3/NEMO/migrations/0044_version_4_4_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/migrations/0045_version_4_5_0.py` & `NEMO-4.6.3/NEMO/migrations/0045_version_4_5_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/migrations/0045_version_4_5_5.py` & `NEMO-4.6.3/NEMO/migrations/0045_version_4_5_5.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/migrations/0046_version_4_6_0.py` & `NEMO-4.6.3/NEMO/migrations/0046_version_4_6_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/migrations_utils.py` & `NEMO-4.6.3/NEMO/migrations_utils.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/mixins.py` & `NEMO-4.6.3/NEMO/mixins.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/model_tree.py` & `NEMO-4.6.3/NEMO/model_tree.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/models.py` & `NEMO-4.6.3/NEMO/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,14 +295,15 @@
 	email_send_reservation_ending_reminders = models.PositiveIntegerField(default=EmailNotificationType.BOTH_EMAILS, choices=EmailNotificationType.Choices, help_text="Reservation ending reminders")
 	recurring_charges_reminder_days = models.CharField(null=True, blank=True, default="60,7", max_length=200, help_text="The number of days to send a reminder before a recurring charge is due. A comma-separated list can be used for multiple reminders.")
 	email_send_recurring_charges_reminder_emails = models.PositiveIntegerField(default=EmailNotificationType.BOTH_EMAILS, choices=EmailNotificationType.Choices, help_text="Recurring charges reminders")
 	tool_freed_time_notifications = models.ManyToManyField("Tool", blank=True, help_text="Tools to receive notification when reservation time is freed.")
 	tool_freed_time_notifications_min_time = models.PositiveIntegerField(default=120, help_text="Minimum amount of minutes freed to receive a notification.")
 	tool_freed_time_notifications_max_future_days = models.PositiveIntegerField(default=7, help_text="Maximum number of days in the future to receive a notification for.")
 	tool_adjustment_notifications = models.ManyToManyField("Tool", related_name="+", blank=True, help_text="Tools to see/receive adjustment notifications for. If empty all notifications will be received.")
+	area_adjustment_notifications = models.ManyToManyField("Area", related_name="+", blank=True, help_text="Areas to see/receive adjustment notifications for. If empty all notifications will be received.")
 	tool_task_notifications = models.ManyToManyField("Tool", related_name="+", blank=True, help_text="Tools to see maintenance records and receive task notifications for. If empty all notifications will be received.")
 
 	def get_recurring_charges_days(self) -> List[int]:
 		return [int(days) for days in self.recurring_charges_reminder_days.split(",") if self.recurring_charges_reminder_days]
 
 	def __str__(self):
 		return f"{self.user.username}'s preferences"
@@ -1272,15 +1273,15 @@
 		the staff sufficient advance notice to configure a tool. """
 		for config in self.enabled_configurations().all():
 			advance_notice = start - timezone.now()
 			if advance_notice < timedelta(hours=config.advance_notice_limit):
 				return True
 		return False
 
-	def get_current_usage_event(self):
+	def get_current_usage_event(self) -> Optional[UsageEvent]:
 		""" Gets the usage event for the current user of this tool. """
 		try:
 			return UsageEvent.objects.get(end=None, tool_id__in=self.get_family_tool_ids())
 		except UsageEvent.DoesNotExist:
 			return None
 
 	def requires_area_reservation(self):
```

### Comparing `NEMO-4.6.2/NEMO/parsers.py` & `NEMO-4.6.3/NEMO/parsers.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/permissions.py` & `NEMO-4.6.3/NEMO/permissions.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/policy.py` & `NEMO-4.6.3/NEMO/policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -863,16 +863,17 @@
                         raise ItemNotAllowedForProjectException(project, user, item.name, msg)
                     elif isinstance(item, Area) and item.id not in distinct_qs_value_list(
                         allowed_tools, "_requires_area_access_id"
                     ):
                         msg = f"{item.name} is not allowed for project {project.name}"
                         raise ItemNotAllowedForProjectException(project, user, item.name, msg)
                 # Check if consumable withdrawals are allowed
-                if isinstance(item, Consumable):
-                    if not project.allow_consumable_withdrawals:
+                # But only when doing a direct withdrawal, we cannot prevent tool usage consumable withdrawals
+                if isinstance(item, Consumable) and isinstance(charge, ConsumableWithdraw):
+                    if not charge.tool_usage and not project.allow_consumable_withdrawals:
                         msg = f"Consumable withdrawals are not allowed for project {project.name}"
                         raise ItemNotAllowedForProjectException(project, user, "Staff Charges", msg)
 
     def check_maximum_users_in_overlapping_reservations(self, reservations: List[Reservation]) -> (int, datetime):
         """
         Returns the maximum number of overlapping reservations and the earlier time the maximum is reached
         This will only count reservations made by different users. i.e. if a user has 3 reservations at the same
```

### Comparing `NEMO-4.6.2/NEMO/provisioning.py` & `NEMO-4.6.3/NEMO/provisioning.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/rates.py` & `NEMO-4.6.3/NEMO/rates.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/rest_filter_backend.py` & `NEMO-4.6.3/NEMO/rest_filter_backend.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/serializers.py` & `NEMO-4.6.3/NEMO/serializers.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/admin/physical_access_level/access_level.js` & `NEMO-4.6.3/NEMO/static/admin/physical_access_level/access_level.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/admin/questions_preview/questions_preview.css` & `NEMO-4.6.3/NEMO/static/admin/questions_preview/questions_preview.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/admin/questions_preview/questions_preview.js` & `NEMO-4.6.3/NEMO/static/admin/questions_preview/questions_preview.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/admin/time_options_override.js` & `NEMO-4.6.3/NEMO/static/admin/time_options_override.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/admin/tool/tool.js` & `NEMO-4.6.3/NEMO/static/admin/tool/tool.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/badge_reader.js` & `NEMO-4.6.3/NEMO/static/badge_reader.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/bootstrap/css/bootstrap-theme.css` & `NEMO-4.6.3/NEMO/static/bootstrap/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/bootstrap/css/bootstrap-theme.css.map` & `NEMO-4.6.3/NEMO/static/bootstrap/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/bootstrap/css/bootstrap-theme.min.css` & `NEMO-4.6.3/NEMO/static/bootstrap/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/bootstrap/css/bootstrap.css` & `NEMO-4.6.3/NEMO/static/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/bootstrap/css/bootstrap.css.map` & `NEMO-4.6.3/NEMO/static/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/bootstrap/css/bootstrap.min.css` & `NEMO-4.6.3/NEMO/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.eot` & `NEMO-4.6.3/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.svg` & `NEMO-4.6.3/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.ttf` & `NEMO-4.6.3/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff` & `NEMO-4.6.3/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff2` & `NEMO-4.6.3/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/bootstrap/js/bootstrap.js` & `NEMO-4.6.3/NEMO/static/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/bootstrap/js/bootstrap.min.js` & `NEMO-4.6.3/NEMO/static/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/datetimepicker/bootstrap-datetimepicker.css` & `NEMO-4.6.3/NEMO/static/datetimepicker/bootstrap-datetimepicker.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/datetimepicker/bootstrap-datetimepicker.js` & `NEMO-4.6.3/NEMO/static/datetimepicker/bootstrap-datetimepicker.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/favicon.ico` & `NEMO-4.6.3/NEMO/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/fullcalendar/fullcalendar.css` & `NEMO-4.6.3/NEMO/static/fullcalendar/fullcalendar.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/fullcalendar/fullcalendar.js` & `NEMO-4.6.3/NEMO/static/fullcalendar/fullcalendar.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/fullcalendar/fullcalendar.min.css` & `NEMO-4.6.3/NEMO/static/fullcalendar/fullcalendar.min.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/fullcalendar/fullcalendar.min.js` & `NEMO-4.6.3/NEMO/static/fullcalendar/fullcalendar.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/icons/agreement.png` & `NEMO-4.6.3/NEMO/static/icons/agreement.png`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/icons/caution.png` & `NEMO-4.6.3/NEMO/static/icons/caution.png`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/icons/preferences.png` & `NEMO-4.6.3/NEMO/static/icons/preferences.png`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/jquery.js` & `NEMO-4.6.3/NEMO/static/jquery.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/jquery.min.js` & `NEMO-4.6.3/NEMO/static/jquery.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/jumbotron_watermark.bmp` & `NEMO-4.6.3/NEMO/static/jumbotron_watermark.bmp`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/mobile.js` & `NEMO-4.6.3/NEMO/static/mobile.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/moment.js` & `NEMO-4.6.3/NEMO/static/moment.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/moment.min.js` & `NEMO-4.6.3/NEMO/static/moment.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/moment.min.js.map` & `NEMO-4.6.3/NEMO/static/moment.min.js.map`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/nemo.css` & `NEMO-4.6.3/NEMO/static/nemo.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/nemo.js` & `NEMO-4.6.3/NEMO/static/nemo.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/numpad/custom_numpad.jquery.js` & `NEMO-4.6.3/NEMO/static/numpad/custom_numpad.jquery.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/pickadate/default.css` & `NEMO-4.6.3/NEMO/static/pickadate/default.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/pickadate/default.date.css` & `NEMO-4.6.3/NEMO/static/pickadate/default.date.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/pickadate/default.time.css` & `NEMO-4.6.3/NEMO/static/pickadate/default.time.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/pickadate/picker.date.js` & `NEMO-4.6.3/NEMO/static/pickadate/picker.date.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/pickadate/picker.js` & `NEMO-4.6.3/NEMO/static/pickadate/picker.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/pickadate/picker.time.js` & `NEMO-4.6.3/NEMO/static/pickadate/picker.time.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/typeahead.jquery.js` & `NEMO-4.6.3/NEMO/static/typeahead.jquery.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/typeahead.jquery.min.js` & `NEMO-4.6.3/NEMO/static/typeahead.jquery.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/virtualkeyboard/jquery.keyboard.js` & `NEMO-4.6.3/NEMO/static/virtualkeyboard/jquery.keyboard.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/virtualkeyboard/jquery.keyboard.min.js` & `NEMO-4.6.3/NEMO/static/virtualkeyboard/jquery.keyboard.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/virtualkeyboard/keyboard-basic.css` & `NEMO-4.6.3/NEMO/static/virtualkeyboard/keyboard-basic.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/static/virtualkeyboard/keyboard-basic.min.css` & `NEMO-4.6.3/NEMO/static/virtualkeyboard/keyboard-basic.min.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/abuse/abuse.html` & `NEMO-4.6.3/NEMO/templates/abuse/abuse.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/abuse/user_drill_down.html` & `NEMO-4.6.3/NEMO/templates/abuse/user_drill_down.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/accounts_and_projects/account_and_projects.html` & `NEMO-4.6.3/NEMO/templates/accounts_and_projects/account_and_projects.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/accounts_and_projects/accounts_and_projects.html` & `NEMO-4.6.3/NEMO/templates/accounts_and_projects/accounts_and_projects.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/accounts_and_projects/create_account.html` & `NEMO-4.6.3/NEMO/templates/accounts_and_projects/create_account.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/accounts_and_projects/create_project.html` & `NEMO-4.6.3/NEMO/templates/accounts_and_projects/create_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/accounts_and_projects/documents_for_project.html` & `NEMO-4.6.3/NEMO/templates/accounts_and_projects/documents_for_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/accounts_and_projects/projects.html` & `NEMO-4.6.3/NEMO/templates/accounts_and_projects/projects.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/accounts_and_projects/users_for_project.html` & `NEMO-4.6.3/NEMO/templates/accounts_and_projects/users_for_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/alerts.html` & `NEMO-4.6.3/NEMO/templates/alerts.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/area_access/area_access.html` & `NEMO-4.6.3/NEMO/templates/area_access/area_access.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/area_access/calendar_self_login.html` & `NEMO-4.6.3/NEMO/templates/area_access/calendar_self_login.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/area_access/change_project.html` & `NEMO-4.6.3/NEMO/templates/area_access/change_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/area_access/login_areas.html` & `NEMO-4.6.3/NEMO/templates/area_access/login_areas.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/area_access/new_area_access_record.html` & `NEMO-4.6.3/NEMO/templates/area_access/new_area_access_record.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/area_access/new_area_access_record_details.html` & `NEMO-4.6.3/NEMO/templates/area_access/new_area_access_record_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/area_access/self_login.html` & `NEMO-4.6.3/NEMO/templates/area_access/self_login.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/authorization_failed.html` & `NEMO-4.6.3/NEMO/templates/authorization_failed.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/base/navbar_base.html` & `NEMO-4.6.3/NEMO/templates/base/navbar_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/base.html` & `NEMO-4.6.3/NEMO/templates/base.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/calendar/calendar.html` & `NEMO-4.6.3/NEMO/templates/calendar/calendar.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/calendar/configuration.html` & `NEMO-4.6.3/NEMO/templates/calendar/configuration.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/calendar/configuration_helper.html` & `NEMO-4.6.3/NEMO/templates/calendar/configuration_helper.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/calendar/policy_dialog.html` & `NEMO-4.6.3/NEMO/templates/calendar/policy_dialog.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/calendar/project_choice.html` & `NEMO-4.6.3/NEMO/templates/calendar/project_choice.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/calendar/proxy_reservation.html` & `NEMO-4.6.3/NEMO/templates/calendar/proxy_reservation.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/calendar/reservation_event_feed.html` & `NEMO-4.6.3/NEMO/templates/calendar/reservation_event_feed.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/calendar/reservation_questions.html` & `NEMO-4.6.3/NEMO/templates/calendar/reservation_questions.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/calendar/reservation_warning.html` & `NEMO-4.6.3/NEMO/templates/calendar/reservation_warning.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/calendar/scheduled_outage_information.html` & `NEMO-4.6.3/NEMO/templates/calendar/scheduled_outage_information.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/calendar/specific_user_feed.html` & `NEMO-4.6.3/NEMO/templates/calendar/specific_user_feed.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/calendar/usage_event_feed.html` & `NEMO-4.6.3/NEMO/templates/calendar/usage_event_feed.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/configuration_agenda.html` & `NEMO-4.6.3/NEMO/templates/configuration_agenda.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/consumables/consumables.html` & `NEMO-4.6.3/NEMO/templates/consumables/consumables.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/consumables/consumables_order.html` & `NEMO-4.6.3/NEMO/templates/consumables/consumables_order.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/consumables/recurring_charge.html` & `NEMO-4.6.3/NEMO/templates/consumables/recurring_charge.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/consumables/recurring_charges.html` & `NEMO-4.6.3/NEMO/templates/consumables/recurring_charges.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/contact/contact_staff.html` & `NEMO-4.6.3/NEMO/templates/contact/contact_staff.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/customizations/customizations.html` & `NEMO-4.6.3/NEMO/templates/customizations/customizations.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/customizations/customizations_application.html` & `NEMO-4.6.3/NEMO/templates/customizations/customizations_application.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/customizations/customizations_calendar.html` & `NEMO-4.6.3/NEMO/templates/customizations/customizations_calendar.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/customizations/customizations_dashboard.html` & `NEMO-4.6.3/NEMO/templates/customizations/customizations_dashboard.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/customizations/customizations_emails.html` & `NEMO-4.6.3/NEMO/templates/customizations/customizations_emails.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/customizations/customizations_interlock.html` & `NEMO-4.6.3/NEMO/templates/customizations/customizations_interlock.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/customizations/customizations_projects_and_accounts.html` & `NEMO-4.6.3/NEMO/templates/customizations/customizations_projects_and_accounts.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/customizations/customizations_rates.html` & `NEMO-4.6.3/NEMO/templates/customizations/customizations_rates.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/customizations/customizations_recurring_charges.html` & `NEMO-4.6.3/NEMO/templates/customizations/customizations_recurring_charges.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/customizations/customizations_remote_work.html` & `NEMO-4.6.3/NEMO/templates/customizations/customizations_remote_work.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/customizations/customizations_requests.html` & `NEMO-4.6.3/NEMO/templates/customizations/customizations_requests.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/customizations/customizations_safety.html` & `NEMO-4.6.3/NEMO/templates/customizations/customizations_safety.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/customizations/customizations_templates.html` & `NEMO-4.6.3/NEMO/templates/customizations/customizations_templates.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/customizations/customizations_tool.html` & `NEMO-4.6.3/NEMO/templates/customizations/customizations_tool.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/customizations/customizations_upload.html` & `NEMO-4.6.3/NEMO/templates/customizations/customizations_upload.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/customizations/customizations_user.html` & `NEMO-4.6.3/NEMO/templates/customizations/customizations_user.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/email/compose_email.html` & `NEMO-4.6.3/NEMO/templates/email/compose_email.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/email/email_broadcast.html` & `NEMO-4.6.3/NEMO/templates/email/email_broadcast.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/email/email_form.html` & `NEMO-4.6.3/NEMO/templates/email/email_form.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/event_details/area_access_details.html` & `NEMO-4.6.3/NEMO/templates/event_details/area_access_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/event_details/outage_details.html` & `NEMO-4.6.3/NEMO/templates/event_details/outage_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/event_details/reservation_details.html` & `NEMO-4.6.3/NEMO/templates/event_details/reservation_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/event_details/usage_details.html` & `NEMO-4.6.3/NEMO/templates/event_details/usage_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/feedback.html` & `NEMO-4.6.3/NEMO/templates/feedback.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/history.html` & `NEMO-4.6.3/NEMO/templates/history.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/impersonate.html` & `NEMO-4.6.3/NEMO/templates/impersonate.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/jumbotron/jumbotron.html` & `NEMO-4.6.3/NEMO/templates/jumbotron/jumbotron.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/jumbotron/jumbotron_content.html` & `NEMO-4.6.3/NEMO/templates/jumbotron/jumbotron_content.html`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 				<h2>Nobody is in an access controlled<br>{{ facility_name }} area</h2>
 			{% else %}
 				{% regroup facility_occupants by area as area_occupants %}
 				<h2>Area occupancy</h2>
 				<p>
 					Staff members are highlighted in <span class="bg-success">&nbsp;green&nbsp;</span><br>
                     Service personnel are highlighted in <span class="bg-warning">&nbsp;orange&nbsp;</span><br>
-                    {% if reservation_required_items %}
+                    {% if reservations_can_expire %}
                     Users with expired reservations are highlighted in <span class="bg-danger">&nbsp;red&nbsp;</span>
                     {% endif %}
 				</p>
 				{% for area in area_occupants %}
 					{% include 'occupancy/occupancy_content.html' with area=area.grouper occupants=area.list transparent_bg=True center_th=True %}
 				{% endfor %}
 			{% endif %}
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 {% if not facility_occupants %}
 ***** Nobody is in an access controlled
 {{ facility_name }} area *****
 {% else %} {% regroup facility_occupants by area as area_occupants %}
 ***** Area occupancy *****
 Staff members are highlighted in  green 
 Service personnel are highlighted in  orange 
-{% if reservation_required_items %} Users with expired reservations are
+{% if reservations_can_expire %} Users with expired reservations are
 highlighted in  red  {% endif %}
 {% for area in area_occupants %} {% include 'occupancy/occupancy_content.html'
 with area=area.grouper occupants=area.list transparent_bg=True center_th=True
 %} {% endfor %} {% endif %}
 {% endif %} {% if tools_exist %}
 {% if usage_events %}
 ***** Tool usage *****
```

### Comparing `NEMO-4.6.2/NEMO/templates/landing.html` & `NEMO-4.6.3/NEMO/templates/landing.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/login.html` & `NEMO-4.6.3/NEMO/templates/login.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/maintenance/closed_task_details.html` & `NEMO-4.6.3/NEMO/templates/maintenance/closed_task_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/maintenance/maintenance.html` & `NEMO-4.6.3/NEMO/templates/maintenance/maintenance.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/maintenance/pending_task_details.html` & `NEMO-4.6.3/NEMO/templates/maintenance/pending_task_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/mobile/cancellation_result.html` & `NEMO-4.6.3/NEMO/templates/mobile/cancellation_result.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/mobile/choose_item.html` & `NEMO-4.6.3/NEMO/templates/mobile/choose_item.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/mobile/individual_outage.html` & `NEMO-4.6.3/NEMO/templates/mobile/individual_outage.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/mobile/individual_reservation.html` & `NEMO-4.6.3/NEMO/templates/mobile/individual_reservation.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/mobile/new_reservation.html` & `NEMO-4.6.3/NEMO/templates/mobile/new_reservation.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/mobile/reservation_success.html` & `NEMO-4.6.3/NEMO/templates/mobile/reservation_success.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/mobile/view_calendar.html` & `NEMO-4.6.3/NEMO/templates/mobile/view_calendar.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/news/archived_news.html` & `NEMO-4.6.3/NEMO/templates/news/archived_news.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/news/new_news_form.html` & `NEMO-4.6.3/NEMO/templates/news/new_news_form.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/news/news_update_form.html` & `NEMO-4.6.3/NEMO/templates/news/news_update_form.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/news/recent_news.html` & `NEMO-4.6.3/NEMO/templates/news/recent_news.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/occupancy/occupancy_content.html` & `NEMO-4.6.3/NEMO/templates/occupancy/occupancy_content.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/occupancy/occupancy_count.html` & `NEMO-4.6.3/NEMO/templates/occupancy/occupancy_count.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/pagination/pagination_base.html` & `NEMO-4.6.3/NEMO/templates/pagination/pagination_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/pagination/pagination_column.html` & `NEMO-4.6.3/NEMO/templates/pagination/pagination_column.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/pagination/pagination_pages.html` & `NEMO-4.6.3/NEMO/templates/pagination/pagination_pages.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/pagination/pagination_selector.html` & `NEMO-4.6.3/NEMO/templates/pagination/pagination_selector.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/qualifications.html` & `NEMO-4.6.3/NEMO/templates/qualifications.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/refresh_sidebar_icons.html` & `NEMO-4.6.3/NEMO/templates/refresh_sidebar_icons.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/remote_work/remote_work.html` & `NEMO-4.6.3/NEMO/templates/remote_work/remote_work.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/remote_work/remote_work_base.html` & `NEMO-4.6.3/NEMO/templates/remote_work/remote_work_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/requests/access_requests/access_request.html` & `NEMO-4.6.3/NEMO/templates/requests/access_requests/access_request.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/requests/access_requests/access_requests.html` & `NEMO-4.6.3/NEMO/templates/requests/access_requests/access_requests.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/requests/access_requests/access_requests_table.html` & `NEMO-4.6.3/NEMO/templates/requests/access_requests/access_requests_table.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/requests/adjustment_requests/adjustment_request.html` & `NEMO-4.6.3/NEMO/templates/requests/adjustment_requests/adjustment_request.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/requests/adjustment_requests/adjustment_requests.html` & `NEMO-4.6.3/NEMO/templates/requests/adjustment_requests/adjustment_requests.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/requests/adjustment_requests/adjustment_requests_table.html` & `NEMO-4.6.3/NEMO/templates/requests/adjustment_requests/adjustment_requests_table.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/requests/buddy_requests/buddy_request.html` & `NEMO-4.6.3/NEMO/templates/requests/buddy_requests/buddy_request.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/requests/buddy_requests/buddy_requests.html` & `NEMO-4.6.3/NEMO/templates/requests/buddy_requests/buddy_requests.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/requests/user_requests.html` & `NEMO-4.6.3/NEMO/templates/requests/user_requests.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/resources/modify_resource.html` & `NEMO-4.6.3/NEMO/templates/resources/modify_resource.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/resources/resource_details.html` & `NEMO-4.6.3/NEMO/templates/resources/resource_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/resources/resources.html` & `NEMO-4.6.3/NEMO/templates/resources/resources.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/resources/scheduled_outage.html` & `NEMO-4.6.3/NEMO/templates/resources/scheduled_outage.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/rest_framework/api.html` & `NEMO-4.6.3/NEMO/templates/rest_framework/api.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/safety/safety.html` & `NEMO-4.6.3/NEMO/templates/safety/safety.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/safety/safety_base.html` & `NEMO-4.6.3/NEMO/templates/safety/safety_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/safety/safety_data_sheets.html` & `NEMO-4.6.3/NEMO/templates/safety/safety_data_sheets.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/safety/safety_issues.html` & `NEMO-4.6.3/NEMO/templates/safety/safety_issues.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/safety/safety_issues_create.html` & `NEMO-4.6.3/NEMO/templates/safety/safety_issues_create.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/safety/safety_issues_resolved.html` & `NEMO-4.6.3/NEMO/templates/safety/safety_issues_resolved.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/safety/safety_issues_update.html` & `NEMO-4.6.3/NEMO/templates/safety/safety_issues_update.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/safety/safety_items.html` & `NEMO-4.6.3/NEMO/templates/safety/safety_items.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/snippets/button.html` & `NEMO-4.6.3/NEMO/templates/snippets/button.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/snippets/contact_person.html` & `NEMO-4.6.3/NEMO/templates/snippets/contact_person.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/snippets/document_list.html` & `NEMO-4.6.3/NEMO/templates/snippets/document_list.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/snippets/embedded_document.html` & `NEMO-4.6.3/NEMO/templates/snippets/embedded_document.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/snippets/tool_info.html` & `NEMO-4.6.3/NEMO/templates/snippets/tool_info.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/staff_charges/change_status.html` & `NEMO-4.6.3/NEMO/templates/staff_charges/change_status.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/staff_charges/choose_project.html` & `NEMO-4.6.3/NEMO/templates/staff_charges/choose_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/staff_charges/new_staff_charge.html` & `NEMO-4.6.3/NEMO/templates/staff_charges/new_staff_charge.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/staff_charges/reminder.html` & `NEMO-4.6.3/NEMO/templates/staff_charges/reminder.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/staff_charges/staff_charges_base.html` & `NEMO-4.6.3/NEMO/templates/staff_charges/staff_charges_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/status_dashboard/occupancy.html` & `NEMO-4.6.3/NEMO/templates/status_dashboard/occupancy.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% if no_occupants %}
 	Nobody is in an access controlled {{ facility_name }} area.
 {% else %}
 	<p>
 		Staff members are highlighted in <span class="bg-success">&nbsp;green&nbsp;</span><br>
 		Service personnel are highlighted in <span class="bg-warning">&nbsp;orange&nbsp;</span><br>
-        {% if reservation_required_items %}
+        {% if reservations_can_expire %}
         Users with expired reservations are highlighted in <span class="bg-danger">&nbsp;red&nbsp;</span>
         {% endif %}
 	</p>
 	<ul class="area-tree-list area-tree-root" style="margin-top: 25px;padding-left: 0">
 		{% for area_item in area_items %}
 			{% if area_item == "in" %}
 				<ul class="area-tree-list collapse in" aria-expanded="true" id="area-{{ forloop.counter }}">
```

### Comparing `NEMO-4.6.2/NEMO/templates/status_dashboard/staff.html` & `NEMO-4.6.3/NEMO/templates/status_dashboard/staff.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/status_dashboard/staff_absence.html` & `NEMO-4.6.3/NEMO/templates/status_dashboard/staff_absence.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/status_dashboard/status_dashboard.html` & `NEMO-4.6.3/NEMO/templates/status_dashboard/status_dashboard.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/status_dashboard/tools.html` & `NEMO-4.6.3/NEMO/templates/status_dashboard/tools.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/tasks/resolve.html` & `NEMO-4.6.3/NEMO/templates/tasks/resolve.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/tasks/update.html` & `NEMO-4.6.3/NEMO/templates/tasks/update.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/tool_control/get_projects.html` & `NEMO-4.6.3/NEMO/templates/tool_control/get_projects.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/tool_control/interlock_error.html` & `NEMO-4.6.3/NEMO/templates/tool_control/interlock_error.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/tool_control/past_tasks_and_comments.html` & `NEMO-4.6.3/NEMO/templates/tool_control/past_tasks_and_comments.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/tool_control/qualified_users.html` & `NEMO-4.6.3/NEMO/templates/tool_control/qualified_users.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/tool_control/tool_control.html` & `NEMO-4.6.3/NEMO/templates/tool_control/tool_control.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/tool_control/tool_status.html` & `NEMO-4.6.3/NEMO/templates/tool_control/tool_status.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/tool_control/usage_data.html` & `NEMO-4.6.3/NEMO/templates/tool_control/usage_data.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/training/get_projects.html` & `NEMO-4.6.3/NEMO/templates/training/get_projects.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/training/training.html` & `NEMO-4.6.3/NEMO/templates/training/training.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/training/training_entry.html` & `NEMO-4.6.3/NEMO/templates/training/training_entry.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/usage/adjustment_request_button.html` & `NEMO-4.6.3/NEMO/templates/usage/adjustment_request_button.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/usage/billing.html` & `NEMO-4.6.3/NEMO/templates/usage/billing.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/usage/usage.html` & `NEMO-4.6.3/NEMO/templates/usage/usage.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/usage/usage_base.html` & `NEMO-4.6.3/NEMO/templates/usage/usage_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/users/create_or_modify_user.html` & `NEMO-4.6.3/NEMO/templates/users/create_or_modify_user.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/users/preferences.html` & `NEMO-4.6.3/NEMO/templates/users/preferences.html`

 * *Files 6% similar despite different names*

```diff
@@ -87,18 +87,29 @@
                         <div class="form-group">
                             <label class="col-sm-5 col-md-4 col-lg-3 form-control-static" for="tool_adjustment_notification_search">Only manage requests for tools</label>
                             <div class="col-sm-6 col-lg-4">
                                 <input id="tool_adjustment_notification_search" type="text" autocomplete="off" class="form-control" placeholder="Add a tool">
                             </div>
                         </div>
                         <div class="form-group">
-                            <div id="adjustment-notification-list" class="col-sm-offset-5 col-md-offset-4 col-lg-offset-3 col-sm-7">
+                            <div id="tool-adjustment-notification-list" class="col-sm-offset-5 col-md-offset-4 col-lg-offset-3 col-sm-7">
                                 You are currently receiving adjustment request notifications for all tools.
                             </div>
                         </div>
+                        <div class="form-group">
+                            <label class="col-sm-5 col-md-4 col-lg-3 form-control-static" for="area_adjustment_notification_search">Only manage requests for areas</label>
+                            <div class="col-sm-6 col-lg-4">
+                                <input id="area_adjustment_notification_search" type="text" autocomplete="off" class="form-control" placeholder="Add an area">
+                            </div>
+                        </div>
+                        <div class="form-group">
+                            <div id="area-adjustment-notification-list" class="col-sm-offset-5 col-md-offset-4 col-lg-offset-3 col-sm-7">
+                                You are currently receiving adjustment request notifications for all areas.
+                            </div>
+                        </div>
                     {% endif %}
                 </div>
             </div>
             {% if user.is_staff or user.is_facility_manager or user.is_service_personnel %}
                 <div class="panel panel-default">
                     <div class="panel-body">
                         <h3 id="adjustment_requests_label">Tool maintenance & notifications</h3>
@@ -197,24 +208,33 @@
             function add_tool_task_notification(jquery_event, search_selection, dataset_name)
             {
                 add_to_list("#task-notification-list", "remove_tool_task_notification", search_selection.id, search_selection.name, "Remove the " + search_selection.name, "tool_task_notifications");
                 $("#tool_task_notification_search").typeahead('val', '').focus();
             }
             function remove_tool_task_notification(tool_id)
             {
-                remove_from_list("#task-notification-list", "#tool_task_notifications_" + tool_id, "You are currently receiving adjustment request notifications for all tools.");
+                remove_from_list("#task-notification-list", "#tool_task_notifications_" + tool_id, "You are currently viewing/receiving maintenance notifications for all tools{% if not user.is_facility_manager or not 'tool'|customization:'tool_task_updates_facility_managers' == 'enabled' %} you are an owner or backup owners of{% endif %}.");
             }
             function add_tool_adjustment_notification(jquery_event, search_selection, dataset_name)
             {
-                add_to_list("#adjustment-notification-list", "remove_tool_adjustment_notification", search_selection.id, search_selection.name, "Remove the " + search_selection.name, "tool_adjustment_notifications");
+                add_to_list("#tool-adjustment-notification-list", "remove_tool_adjustment_notification", search_selection.id, search_selection.name, "Remove the " + search_selection.name, "tool_adjustment_notifications");
                 $("#tool_adjustment_notification_search").typeahead('val', '').focus();
             }
             function remove_tool_adjustment_notification(tool_id)
             {
-                remove_from_list("#adjustment-notification-list", "#tool_adjustment_notifications_" + tool_id, "You are currently viewing/receiving maintenance notifications for all tools{% if not user.is_facility_manager or not 'tool'|customization:'tool_task_updates_facility_managers' == 'enabled' %} you are an owner or backup owners of{% endif %}.");
+                remove_from_list("#tool-adjustment-notification-list", "#tool_adjustment_notifications_" + tool_id, "You are currently receiving adjustment request notifications for all tools.");
+            }
+            function add_area_adjustment_notification(jquery_event, search_selection, dataset_name)
+            {
+                add_to_list("#area-adjustment-notification-list", "remove_area_adjustment_notification", search_selection.id, search_selection.name, "Remove the " + search_selection.name, "area_adjustment_notifications");
+                $("#area_adjustment_notification_search").typeahead('val', '').focus();
+            }
+            function remove_area_adjustment_notification(area_id)
+            {
+                remove_from_list("#area-adjustment-notification-list", "#area_adjustment_notifications_" + area_id, "You are currently receiving adjustment request notifications for all areas.");
             }
             function add_tool_notification(jquery_event, search_selection, dataset_name)
             {
                 add_to_list("#notification-list", "remove_tool_notification", search_selection.id, search_selection.name, "Remove the " + search_selection.name, "tool_freed_time_notifications");
                 $("#tool_notification_search").typeahead('val', '').focus();
             }
             function remove_tool_notification(tool_id)
@@ -230,25 +250,31 @@
                             {% if tool.id == tool_id|to_int %}
                                 add_tool_notification(null, {'name': '{{ tool.name }}', 'id': {{ tool.id }} });
                             {% endif %}
                         {% endfor %}
                     {% endfor %}
                 {% endif %}
                 $('#tool_adjustment_notification_search').autocomplete('tools', add_tool_adjustment_notification, {{ form.fields.tool_adjustment_notifications.queryset|json_search_base }});
+                $('#area_adjustment_notification_search').autocomplete('areas', add_area_adjustment_notification, {{ form.fields.area_adjustment_notifications.queryset|json_search_base }});
+                $('#tool_task_notification_search').autocomplete('tools', add_tool_task_notification, {{ form.fields.tool_task_notifications.queryset|json_search_base }});
                 {% if form.instance.id %}
                     {% for tool_id in form.tool_adjustment_notifications.value %}
                         {% for tool in form.fields.tool_adjustment_notifications.queryset %}
                             {% if tool.id == tool_id|to_int %}
                                 add_tool_adjustment_notification(null, {'name': '{{ tool.name }}', 'id': {{ tool.id }} });
                             {% endif %}
                         {% endfor %}
                     {% endfor %}
-                {% endif %}
-                $('#tool_task_notification_search').autocomplete('tools', add_tool_task_notification, {{ form.fields.tool_task_notifications.queryset|json_search_base }});
-                {% if form.instance.id %}
+                    {% for area_id in form.area_adjustment_notifications.value %}
+                        {% for area in form.fields.area_adjustment_notifications.queryset %}
+                            {% if area.id == area_id|to_int %}
+                                add_area_adjustment_notification(null, {'name': '{{ area.name }}', 'id': {{ area.id }} });
+                            {% endif %}
+                        {% endfor %}
+                    {% endfor %}
                     {% for tool_id in form.tool_task_notifications.value %}
                         {% for tool in form.fields.tool_task_notifications.queryset %}
                             {% if tool.id == tool_id|to_int %}
                                 add_tool_task_notification(null, {'name': '{{ tool.name }}', 'id': {{ tool.id }} });
                             {% endif %}
                         {% endfor %}
                     {% endfor %}
```

### Comparing `NEMO-4.6.2/NEMO/templates/users/safe_deactivation.html` & `NEMO-4.6.3/NEMO/templates/users/safe_deactivation.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templates/users/users.html` & `NEMO-4.6.3/NEMO/templates/users/users.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/templatetags/custom_tags_and_filters.py` & `NEMO-4.6.3/NEMO/templatetags/custom_tags_and_filters.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/urls.py` & `NEMO-4.6.3/NEMO/urls.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/utilities.py` & `NEMO-4.6.3/NEMO/utilities.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/abuse.py` & `NEMO-4.6.3/NEMO/views/abuse.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/access_requests.py` & `NEMO-4.6.3/NEMO/views/access_requests.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/accounts_and_projects.py` & `NEMO-4.6.3/NEMO/views/accounts_and_projects.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/adjustment_requests.py` & `NEMO-4.6.3/NEMO/views/adjustment_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     RequestMessage,
     RequestStatus,
     Reservation,
     StaffCharge,
     UsageEvent,
     User,
 )
+from NEMO.typing import QuerySetType
 from NEMO.utilities import (
     BasicDisplayTable,
     bootstrap_primary_color,
     EmailCategory,
     export_format_datetime,
     get_full_url,
     quiet_int,
@@ -51,23 +52,21 @@
         return HttpResponseBadRequest("Adjustment requests are not enabled")
 
     user: User = request.user
     max_requests = quiet_int(UserRequestsCustomization.get("adjustment_requests_display_max"), None)
     adj_requests = AdjustmentRequest.objects.filter(deleted=False)
     if not user.is_facility_manager and not user.is_user_office and not user.is_accounting_officer:
         adj_requests = adj_requests.filter(creator=user)
-    if user.is_facility_manager and user.get_preferences().tool_adjustment_notifications.all():
+    if user.is_facility_manager and (user.get_preferences().tool_adjustment_notifications.exists() or user.get_preferences().area_adjustment_notifications.exists()):
         exclude = []
-        tools = user.get_preferences().tool_adjustment_notifications.all()
-        if tools:
-            for adj in adj_requests:
-                tool = getattr(adj.item, "tool", None) if adj.item else None
-                if tool and tool not in tools:
-                    exclude.append(adj.pk)
-            adj_requests = adj_requests.exclude(pk__in=exclude)
+        for adj in adj_requests:
+            managers = managers_for_adjustment_request(adj)
+            if user not in managers:
+                exclude.append(adj.pk)
+        adj_requests = adj_requests.exclude(pk__in=exclude)
 
     dictionary = {
         "pending_adjustment_requests": adj_requests.filter(status=RequestStatus.PENDING),
         "approved_adjustment_requests": adj_requests.filter(status=RequestStatus.APPROVED)[:max_requests],
         "denied_adjustment_requests": adj_requests.filter(status=RequestStatus.DENIED)[:max_requests],
         "adjustment_requests_description": UserRequestsCustomization.get("adjustment_requests_description"),
         "request_notifications": get_notifications(
@@ -143,25 +142,15 @@
                     else:
                         adjustment_request.status = RequestStatus.DENIED
                     adjustment_request.reviewer = user
 
             form.instance.last_updated_by = user
             new_adjustment_request = form.save()
 
-            # Create the list of facility managers to notify. If the adjustment request has a tool and no one added that
-            # tool to their adjustment request list, send to everyone (otherwise nobody would see it)
-            managers_to_notify: Set[User] = set()
-            tool = getattr(adjustment_request.item, "tool", None) if adjustment_request.item else None
-            reviewers: QuerySet = User.objects.filter(is_active=True, is_facility_manager=True)
-            if tool:
-                reviewers_filter = reviewers.filter(Q(preferences__tool_adjustment_notifications__isnull=True) | Q(preferences__tool_adjustment_notifications__in=[tool]))
-                if reviewers_filter.exists():
-                    # Only limit managers if at least one person will receive the notification.
-                    reviewers = reviewers_filter
-            managers_to_notify.update(list(reviewers))
+            managers_to_notify: Set[User] = set(list(managers_for_adjustment_request(adjustment_request)))
 
             create_adjustment_request_notification(new_adjustment_request, managers_to_notify)
             if edit:
                 # remove notification for current user and other facility managers
                 delete_notification(Notification.Types.ADJUSTMENT_REQUEST, adjustment_request.id, [user])
                 if user.is_facility_manager:
                     managers = User.objects.filter(is_active=True, is_facility_manager=True)
@@ -398,7 +387,28 @@
             }
         )
 
     filename = f"adjustment_requests_{export_format_datetime()}.csv"
     response = table_result.to_csv()
     response["Content-Disposition"] = f'attachment; filename="{filename}"'
     return response
+
+
+def managers_for_adjustment_request(adjustment_request: AdjustmentRequest) -> QuerySetType[User]:
+    # Create the list of facility managers to notify/show request to. If the adjustment request has a tool/area and no
+    # one added that tool/area to their adjustment request list, send/show to everyone (otherwise nobody would see it)
+    tool = getattr(adjustment_request.item, "tool", None) if adjustment_request.item else None
+    area = getattr(adjustment_request.item, "area", None) if adjustment_request.item else None
+    reviewers = User.objects.filter(is_active=True, is_facility_manager=True)
+    if tool:
+        reviewers_filter = reviewers.filter(Q(preferences__tool_adjustment_notifications__isnull=True) | Q(
+            preferences__tool_adjustment_notifications__in=[tool]))
+        if reviewers_filter.exists():
+            # Only limit managers if at least one person will receive the notification.
+            reviewers = reviewers_filter
+    if area:
+        reviewers_filter = reviewers.filter(Q(preferences__area_adjustment_notifications__isnull=True) | Q(
+            preferences__area_adjustment_notifications__in=[area]))
+        if reviewers_filter.exists():
+            # Only limit managers if at least one person will receive the notification.
+            reviewers = reviewers_filter
+    return reviewers
```

### Comparing `NEMO-4.6.2/NEMO/views/alerts.py` & `NEMO-4.6.3/NEMO/views/alerts.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/api.py` & `NEMO-4.6.3/NEMO/views/api.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/api_billing.py` & `NEMO-4.6.3/NEMO/views/api_billing.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/api_file_import.py` & `NEMO-4.6.3/NEMO/views/api_file_import.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/area_access.py` & `NEMO-4.6.3/NEMO/views/area_access.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/authentication.py` & `NEMO-4.6.3/NEMO/views/authentication.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/buddy_requests.py` & `NEMO-4.6.3/NEMO/views/buddy_requests.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/calendar.py` & `NEMO-4.6.3/NEMO/views/calendar.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/charge_validation.py` & `NEMO-4.6.3/NEMO/views/charge_validation.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/configuration_agenda.py` & `NEMO-4.6.3/NEMO/views/configuration_agenda.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/consumables.py` & `NEMO-4.6.3/NEMO/views/consumables.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,22 +255,24 @@
 def extended_permissions(request) -> bool:
 	user: User = request.user
 	lock_charges = RecurringChargesCustomization.get_bool("recurring_charges_lock")
 	return not lock_charges or user.is_facility_manager or user.is_superuser
 
 
 def make_withdrawal(consumable_id: int, quantity: int, project_id: int, merchant: User, customer_id: int, tool_usage=False, request=None):
-	withdraw = ConsumableWithdraw.objects.create(
+	withdraw = ConsumableWithdraw(
 		consumable_id=consumable_id,
 		quantity=quantity,
 		merchant=merchant,
 		customer_id=customer_id,
 		project_id=project_id,
 		tool_usage=tool_usage
 	)
+	withdraw.full_clean()
+	withdraw.save()
 	if not withdraw.consumable.reusable:
 		# Only withdraw if it's an actual consumable (not reusable)
 		withdraw.consumable.quantity -= withdraw.quantity
 	withdraw.consumable.save()
 	# Only add notification message if request is present
 	if request:
 		if request.user.id == customer_id:
```

### Comparing `NEMO-4.6.2/NEMO/views/customization.py` & `NEMO-4.6.3/NEMO/views/customization.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/documents.py` & `NEMO-4.6.3/NEMO/views/documents.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/email.py` & `NEMO-4.6.3/NEMO/views/email.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/event_details.py` & `NEMO-4.6.3/NEMO/views/event_details.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/feedback.py` & `NEMO-4.6.3/NEMO/views/feedback.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/get_projects.py` & `NEMO-4.6.3/NEMO/views/get_projects.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/history.py` & `NEMO-4.6.3/NEMO/views/history.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/jumbotron.py` & `NEMO-4.6.3/NEMO/views/jumbotron.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/landing.py` & `NEMO-4.6.3/NEMO/views/landing.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/maintenance.py` & `NEMO-4.6.3/NEMO/views/maintenance.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/mobile.py` & `NEMO-4.6.3/NEMO/views/mobile.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/news.py` & `NEMO-4.6.3/NEMO/views/news.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/notifications.py` & `NEMO-4.6.3/NEMO/views/notifications.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/pagination.py` & `NEMO-4.6.3/NEMO/views/pagination.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/qualifications.py` & `NEMO-4.6.3/NEMO/views/qualifications.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/remote_work.py` & `NEMO-4.6.3/NEMO/views/remote_work.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/resources.py` & `NEMO-4.6.3/NEMO/views/resources.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/safety.py` & `NEMO-4.6.3/NEMO/views/safety.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/sidebar.py` & `NEMO-4.6.3/NEMO/views/sidebar.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/status_dashboard.py` & `NEMO-4.6.3/NEMO/views/status_dashboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,15 +215,16 @@
 	absences = StaffAbsence.objects.filter(start_date__lte=end, end_date__gte=start).order_by("creation_time").prefetch_related("staff_member")
 	for staff_absence in absences:
 		for day in days:
 			# comparing dates here so no timezone issues (dates don't have timezones)
 			# non-working days should not count as absence
 			staff_works_this_day = staff_absence.staff_member.weekly_availability()[day.weekday()]
 			if staff_works_this_day and staff_absence.start_date <= day.date() <= staff_absence.end_date:
-				dictionary[staff_absence.staff_member.id][day.day] = staff_absence
+				if staff_absence.staff_member.id in dictionary:
+					dictionary[staff_absence.staff_member.id][day.day] = staff_absence
 	return dictionary
 
 
 def closures_dict(days, start, end):
 	dictionary = {}
 	l_start, l_end = localize(start), localize(end)
 	closure_times = ClosureTime.objects.filter(start_time__lte=l_end, end_time__gte=l_start, closure__staff_absent=True)
```

### Comparing `NEMO-4.6.2/NEMO/views/tasks.py` & `NEMO-4.6.3/NEMO/views/tasks.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/tool_control.py` & `NEMO-4.6.3/NEMO/views/tool_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -401,19 +401,19 @@
 	if tool.interlock and not tool.interlock.lock():
 		if bypass_interlock and interlock_bypass_allowed(user):
 			pass
 		else:
 			return interlock_error("Disable", user)
 
 	# Shorten the user's tool reservation since we are now done using the tool
+	current_usage_event = tool.get_current_usage_event()
 	staff_shortening = request.POST.get("shorten", False)
-	shorten_reservation(user=user, item=tool, new_end=timezone.now() + downtime, force=staff_shortening)
+	shorten_reservation(user=current_usage_event.user, item=tool, new_end=timezone.now() + downtime, force=staff_shortening)
 
 	# End the current usage event for the tool
-	current_usage_event = tool.get_current_usage_event()
 	current_usage_event.end = timezone.now() + downtime
 
 	# Collect post-usage questions
 	dynamic_form = DynamicForm(tool.post_usage_questions)
 
 	try:
 		current_usage_event.run_data = dynamic_form.extract(request)
@@ -421,21 +421,24 @@
 		if (user.is_staff or user.is_user_office) and user != current_usage_event.operator and current_usage_event.user != user:
 			# if a staff is forcing somebody off the tool and there are required questions, send an email and proceed
 			current_usage_event.run_data = e.run_data
 			email_managers_required_questions_disable_tool(current_usage_event.operator, user, tool, e.questions)
 		else:
 			return HttpResponseBadRequest(str(e))
 
-	dynamic_form.charge_for_consumables(
-		current_usage_event.user,
-		current_usage_event.operator,
-		current_usage_event.project,
-		current_usage_event.run_data,
-		request
-	)
+	try:
+		dynamic_form.charge_for_consumables(
+			current_usage_event.user,
+			current_usage_event.operator,
+			current_usage_event.project,
+			current_usage_event.run_data,
+			request
+		)
+	except Exception as e:
+		return HttpResponseBadRequest(str(e))
 	dynamic_form.update_tool_counters(current_usage_event.run_data, tool.id)
 
 	current_usage_event.save()
 	if user.charging_staff_time():
 		existing_staff_charge = user.get_staff_charge()
 		if (
 				existing_staff_charge.customer == current_usage_event.user
```

### Comparing `NEMO-4.6.2/NEMO/views/training.py` & `NEMO-4.6.3/NEMO/views/training.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/tutorials.py` & `NEMO-4.6.3/NEMO/views/tutorials.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/usage.py` & `NEMO-4.6.3/NEMO/views/usage.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/user_requests.py` & `NEMO-4.6.3/NEMO/views/user_requests.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/views/users.py` & `NEMO-4.6.3/NEMO/views/users.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/widgets/configuration_editor.py` & `NEMO-4.6.3/NEMO/widgets/configuration_editor.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO/widgets/dynamic_form.py` & `NEMO-4.6.3/NEMO/widgets/dynamic_form.py`

 * *Files 2% similar despite different names*

```diff
@@ -545,40 +545,33 @@
 			except Consumable.DoesNotExist:
 				raise Exception(f"Consumable with name '{question.consumable}' could not be found. Make sure the names match.")
 
 
 def withdraw_consumable_for_question(question, input_data, customer, merchant, project, request):
 	if isinstance(question, PostUsageNumberFieldQuestion):
 		if question.consumable:
-			try:
-				consumable = Consumable.objects.get(name=question.consumable)
-				quantity = 0
-				if input_data and "user_input" in input_data and input_data["user_input"]:
-					if isinstance(input_data["user_input"], dict):
-						for user_input in input_data["user_input"].values():
-							if question.name in user_input and user_input[question.name]:
-								quantity += int(user_input[question.name])
-					else:
-						quantity = int(input_data["user_input"])
-				if quantity > 0:
-					make_withdrawal(
-						consumable_id=consumable.id,
-						customer_id=customer.id,
-						merchant=merchant,
-						quantity=quantity,
-						project_id=project.id,
-						tool_usage=True,
-						request=request,
-					)
-			except Exception as e:
-				dynamic_form_logger.warning(
-					f"Could not withdraw consumable: '{question.consumable}' with quantity: '{input_data}' for customer: '{customer}' by merchant: '{merchant}' for project: '{project}'",
-					e,
+			consumable = Consumable.objects.get(name=question.consumable)
+			quantity = 0
+			if input_data and "user_input" in input_data and input_data["user_input"]:
+				if isinstance(input_data["user_input"], dict):
+					for user_input in input_data["user_input"].values():
+						if question.name in user_input and user_input[question.name]:
+							quantity += int(user_input[question.name])
+				else:
+					quantity = int(input_data["user_input"])
+			if quantity > 0:
+				make_withdrawal(
+					consumable_id=consumable.id,
+					customer_id=customer.id,
+					merchant=merchant,
+					quantity=quantity,
+					project_id=project.id,
+					tool_usage=True,
+					request=request,
 				)
-				pass
 
 
 def get_counter_increment_for_question(question, input_data, counter_question):
 	additional_value = 0
 	if isinstance(question, PostUsageNumberFieldQuestion) or isinstance(question, PostUsageFloatFieldQuestion):
 		if question.name == counter_question and "user_input" in input_data and input_data["user_input"]:
 			if isinstance(input_data["user_input"], dict):
```

### Comparing `NEMO-4.6.2/NEMO/widgets/item_tree.py` & `NEMO-4.6.3/NEMO/widgets/item_tree.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/NEMO.egg-info/PKG-INFO` & `NEMO-4.6.3/NEMO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NEMO
-Version: 4.6.2
+Version: 4.6.3
 Summary: NEMO is a laboratory logistics web application. Use it to schedule reservations, control tool access, track maintenance issues, and more.
 Home-page: https://github.com/usnistgov/NEMO
 Author: Center for Nanoscale Science and Technology
 Author-email: CNSTapplications@nist.gov
 License: Public domain
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `NEMO-4.6.2/NEMO.egg-info/SOURCES.txt` & `NEMO-4.6.3/NEMO.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -148,14 +148,15 @@
 NEMO/migrations/0042_version_4_3_0.py
 NEMO/migrations/0043_version_4_3_2.py
 NEMO/migrations/0044_version_4_4_0.py
 NEMO/migrations/0045_version_4_5_0.py
 NEMO/migrations/0045_version_4_5_5.py
 NEMO/migrations/0046_version_4_6_0.py
 NEMO/migrations/0047_version_4_6_1.py
+NEMO/migrations/0048_version_4_6_3.py
 NEMO/migrations/__init__.py
 NEMO/static/badge_reader.js
 NEMO/static/favicon.ico
 NEMO/static/jquery.js
 NEMO/static/jquery.min.js
 NEMO/static/jumbotron_watermark.bmp
 NEMO/static/mobile.js
```

### Comparing `NEMO-4.6.2/PKG-INFO` & `NEMO-4.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NEMO
-Version: 4.6.2
+Version: 4.6.3
 Summary: NEMO is a laboratory logistics web application. Use it to schedule reservations, control tool access, track maintenance issues, and more.
 Home-page: https://github.com/usnistgov/NEMO
 Author: Center for Nanoscale Science and Technology
 Author-email: CNSTapplications@nist.gov
 License: Public domain
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `NEMO-4.6.2/README.md` & `NEMO-4.6.3/README.md`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/resources/settings.py` & `NEMO-4.6.3/resources/settings.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/resources/splash_pad_settings.py` & `NEMO-4.6.3/resources/splash_pad_settings.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.2/setup.py` & `NEMO-4.6.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, setup
 
 setup(
 	name='NEMO',
-	version='4.6.2',
+	version='4.6.3',
 	python_requires='>=3.8, <4',
 	packages=find_namespace_packages(exclude=['NEMO.tests', 'NEMO.tests.*']),
 	include_package_data=True,
 	url='https://github.com/usnistgov/NEMO',
 	license='Public domain',
 	author='Center for Nanoscale Science and Technology',
 	author_email='CNSTapplications@nist.gov',
```

