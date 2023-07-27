# Comparing `tmp/typedhtml-0.1.8.tar.gz` & `tmp/typedhtml-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedhtml-0.1.8.tar", max compression
+gzip compressed data, was "typedhtml-0.1.9.tar", max compression
```

## Comparing `typedhtml-0.1.8.tar` & `typedhtml-0.1.9.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0        0 2023-07-21 23:03:24.783891 typedhtml-0.1.8/README.md
--rw-r--r--   0        0        0      444 2023-07-27 20:47:51.845767 typedhtml-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      154 2023-07-23 17:35:32.083325 typedhtml-0.1.8/typedhtml/__init__.py
--rw-r--r--   0        0        0    17304 2023-07-24 23:24:43.336075 typedhtml-0.1.8/typedhtml/attributes.py
--rw-r--r--   0        0        0      763 2023-07-27 20:47:38.082477 typedhtml-0.1.8/typedhtml/document.py
--rw-r--r--   0        0        0     2969 2023-07-22 18:24:49.759970 typedhtml-0.1.8/typedhtml/events.py
--rw-r--r--   0        0        0     7348 2023-07-23 19:50:40.425730 typedhtml-0.1.8/typedhtml/globals.py
--rw-r--r--   0        0        0        0 2023-07-25 19:54:45.714922 typedhtml-0.1.8/typedhtml/py.typed
--rw-r--r--   0        0        0     1211 2023-07-23 06:34:06.643229 typedhtml-0.1.8/typedhtml/svg.py
--rw-r--r--   0        0        0    31931 2023-07-27 20:43:26.614161 typedhtml-0.1.8/typedhtml/tags.py
--rw-r--r--   0        0        0     9230 2023-07-25 19:34:32.723450 typedhtml-0.1.8/typedhtml/ui5/__init__.py
--rw-r--r--   0        0        0     3264 2023-07-24 03:41:38.489987 typedhtml-0.1.8/typedhtml/ui5/avatar.py
--rw-r--r--   0        0        0      863 2023-07-24 03:38:24.465498 typedhtml-0.1.8/typedhtml/ui5/badge.py
--rw-r--r--   0        0        0      539 2023-07-25 12:44:07.138808 typedhtml-0.1.8/typedhtml/ui5/bar.py
--rw-r--r--   0        0        0      244 2023-07-25 12:45:43.227706 typedhtml-0.1.8/typedhtml/ui5/barcode_scanner_dialog.py
--rw-r--r--   0        0        0      692 2023-07-27 16:15:58.159590 typedhtml-0.1.8/typedhtml/ui5/base.py
--rw-r--r--   0        0        0     1354 2023-07-24 03:41:10.194619 typedhtml-0.1.8/typedhtml/ui5/breadcrumbs.py
--rw-r--r--   0        0        0      797 2023-07-24 03:42:17.102817 typedhtml-0.1.8/typedhtml/ui5/busy_indicator.py
--rw-r--r--   0        0        0     1091 2023-07-24 03:42:46.370478 typedhtml-0.1.8/typedhtml/ui5/button.py
--rw-r--r--   0        0        0     1214 2023-07-24 21:22:07.958588 typedhtml-0.1.8/typedhtml/ui5/calendar.py
--rw-r--r--   0        0        0     1424 2023-07-24 03:44:35.261001 typedhtml-0.1.8/typedhtml/ui5/card.py
--rw-r--r--   0        0        0     1356 2023-07-24 03:44:57.515274 typedhtml-0.1.8/typedhtml/ui5/carousel.py
--rw-r--r--   0        0        0     1405 2023-07-24 03:45:38.605099 typedhtml-0.1.8/typedhtml/ui5/checkbox.py
--rw-r--r--   0        0        0     1551 2023-07-24 03:48:24.851505 typedhtml-0.1.8/typedhtml/ui5/color_palette.py
--rw-r--r--   0        0        0      619 2023-07-24 03:48:50.205563 typedhtml-0.1.8/typedhtml/ui5/color_picker.py
--rw-r--r--   0        0        0     1018 2023-07-24 03:49:37.145966 typedhtml-0.1.8/typedhtml/ui5/combobox.py
--rw-r--r--   0        0        0     1062 2023-07-24 03:50:02.077503 typedhtml-0.1.8/typedhtml/ui5/datepicker.py
--rw-r--r--   0        0        0      797 2023-07-24 21:22:33.226998 typedhtml-0.1.8/typedhtml/ui5/daterange_picker.py
--rw-r--r--   0        0        0      634 2023-07-24 03:51:37.839555 typedhtml-0.1.8/typedhtml/ui5/datetime_picker.py
--rw-r--r--   0        0        0      724 2023-07-24 03:51:59.287201 typedhtml-0.1.8/typedhtml/ui5/dialog.py
--rw-r--r--   0        0        0      920 2023-07-25 12:52:50.880741 typedhtml-0.1.8/typedhtml/ui5/dynamic_side_content.py
--rw-r--r--   0        0        0     1018 2023-07-24 03:52:52.259960 typedhtml-0.1.8/typedhtml/ui5/file_uploader.py
--rw-r--r--   0        0        0     1066 2023-07-25 13:05:33.331084 typedhtml-0.1.8/typedhtml/ui5/flexible_column_layout.py
--rw-r--r--   0        0        0      989 2023-07-24 03:53:09.125464 typedhtml-0.1.8/typedhtml/ui5/icon.py
--rw-r--r--   0        0        0     3220 2023-07-25 15:00:10.774344 typedhtml-0.1.8/typedhtml/ui5/illustrated_message.py
--rw-r--r--   0        0        0     1104 2023-07-24 18:46:05.721707 typedhtml-0.1.8/typedhtml/ui5/input.py
--rw-r--r--   0        0        0      677 2023-07-24 03:35:27.924512 typedhtml-0.1.8/typedhtml/ui5/label.py
--rw-r--r--   0        0        0      848 2023-07-24 04:19:28.264763 typedhtml-0.1.8/typedhtml/ui5/link.py
--rw-r--r--   0        0        0     2336 2023-07-24 04:55:43.979158 typedhtml-0.1.8/typedhtml/ui5/list.py
--rw-r--r--   0        0        0     1113 2023-07-25 15:12:47.396435 typedhtml-0.1.8/typedhtml/ui5/media_gallery.py
--rw-r--r--   0        0        0     1292 2023-07-24 05:07:02.147480 typedhtml-0.1.8/typedhtml/ui5/menu.py
--rw-r--r--   0        0        0      934 2023-07-24 05:11:38.448763 typedhtml-0.1.8/typedhtml/ui5/message_strip.py
--rw-r--r--   0        0        0     2111 2023-07-24 05:32:56.437095 typedhtml-0.1.8/typedhtml/ui5/multi_combobox.py
--rw-r--r--   0        0        0     1217 2023-07-24 05:47:28.390516 typedhtml-0.1.8/typedhtml/ui5/multi_input.py
--rw-r--r--   0        0        0     1341 2023-07-25 15:35:21.371287 typedhtml-0.1.8/typedhtml/ui5/notification_list_group.py
--rw-r--r--   0        0        0      651 2023-07-25 19:36:15.108104 typedhtml-0.1.8/typedhtml/ui5/notification_list_item.py
--rw-r--r--   0        0        0      822 2023-07-25 16:29:47.448554 typedhtml-0.1.8/typedhtml/ui5/page.py
--rw-r--r--   0        0        0      786 2023-07-24 05:56:13.272720 typedhtml-0.1.8/typedhtml/ui5/panel.py
--rw-r--r--   0        0        0     1049 2023-07-24 16:47:51.776836 typedhtml-0.1.8/typedhtml/ui5/popover.py
--rw-r--r--   0        0        0      851 2023-07-25 16:47:28.910479 typedhtml-0.1.8/typedhtml/ui5/product_switch.py
--rw-r--r--   0        0        0      813 2023-07-24 16:53:02.111474 typedhtml-0.1.8/typedhtml/ui5/progress.py
--rw-r--r--   0        0        0     1147 2023-07-24 17:23:34.365913 typedhtml-0.1.8/typedhtml/ui5/radio.py
--rw-r--r--   0        0        0      739 2023-07-24 17:26:16.577498 typedhtml-0.1.8/typedhtml/ui5/range_slider.py
--rw-r--r--   0        0        0      846 2023-07-24 17:30:46.775794 typedhtml-0.1.8/typedhtml/ui5/rating_indicator.py
--rw-r--r--   0        0        0      460 2023-07-24 19:03:12.882005 typedhtml-0.1.8/typedhtml/ui5/responsive_popover.py
--rw-r--r--   0        0        0     1240 2023-07-24 17:45:46.706947 typedhtml-0.1.8/typedhtml/ui5/segmented_button.py
--rw-r--r--   0        0        0     1330 2023-07-24 17:52:58.144971 typedhtml-0.1.8/typedhtml/ui5/select.py
--rw-r--r--   0        0        0     1267 2023-07-25 19:13:16.274085 typedhtml-0.1.8/typedhtml/ui5/shell_bar.py
--rw-r--r--   0        0        0     1369 2023-07-25 17:45:11.869783 typedhtml-0.1.8/typedhtml/ui5/side_nav.py
--rw-r--r--   0        0        0      686 2023-07-24 18:07:42.261132 typedhtml-0.1.8/typedhtml/ui5/slider.py
--rw-r--r--   0        0        0      992 2023-07-24 18:15:29.579762 typedhtml-0.1.8/typedhtml/ui5/split_button.py
--rw-r--r--   0        0        0      925 2023-07-24 18:19:41.715572 typedhtml-0.1.8/typedhtml/ui5/step_input.py
--rw-r--r--   0        0        0      915 2023-07-24 18:23:43.502304 typedhtml-0.1.8/typedhtml/ui5/switch.py
--rw-r--r--   0        0        0     1051 2023-07-24 18:37:11.846161 typedhtml-0.1.8/typedhtml/ui5/tab_container.py
--rw-r--r--   0        0        0     2066 2023-07-24 19:41:17.961063 typedhtml-0.1.8/typedhtml/ui5/table.py
--rw-r--r--   0        0        0      904 2023-07-24 20:54:41.376476 typedhtml-0.1.8/typedhtml/ui5/textarea.py
--rw-r--r--   0        0        0      665 2023-07-24 20:57:46.970970 typedhtml-0.1.8/typedhtml/ui5/time_picker.py
--rw-r--r--   0        0        0      784 2023-07-25 17:58:03.447272 typedhtml-0.1.8/typedhtml/ui5/timeline.py
--rw-r--r--   0        0        0      566 2023-07-24 21:01:29.280885 typedhtml-0.1.8/typedhtml/ui5/title.py
--rw-r--r--   0        0        0      708 2023-07-24 21:04:14.974066 typedhtml-0.1.8/typedhtml/ui5/toast.py
--rw-r--r--   0        0        0      496 2023-07-24 22:06:21.633647 typedhtml-0.1.8/typedhtml/ui5/toggle_button.py
--rw-r--r--   0        0        0     1135 2023-07-24 22:10:33.706725 typedhtml-0.1.8/typedhtml/ui5/tree.py
--rw-r--r--   0        0        0     1470 2023-07-25 18:12:53.064206 typedhtml-0.1.8/typedhtml/ui5/upload_collection.py
--rw-r--r--   0        0        0     1685 2023-07-25 19:37:34.851255 typedhtml-0.1.8/typedhtml/ui5/view_settings_dialog.py
--rw-r--r--   0        0        0      871 2023-07-25 18:36:11.056458 typedhtml-0.1.8/typedhtml/ui5/wizard.py
--rw-r--r--   0        0        0      536 2023-07-27 16:09:36.125132 typedhtml-0.1.8/typedhtml/util.py
--rw-r--r--   0        0        0      427 1970-01-01 00:00:00.000000 typedhtml-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-21 23:03:24.783891 typedhtml-0.1.9/README.md
+-rw-r--r--   0        0        0      444 2023-07-27 21:07:33.093189 typedhtml-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      154 2023-07-23 17:35:32.083325 typedhtml-0.1.9/typedhtml/__init__.py
+-rw-r--r--   0        0        0    17304 2023-07-24 23:24:43.336075 typedhtml-0.1.9/typedhtml/attributes.py
+-rw-r--r--   0        0        0      763 2023-07-27 20:47:38.082477 typedhtml-0.1.9/typedhtml/document.py
+-rw-r--r--   0        0        0     2969 2023-07-22 18:24:49.759970 typedhtml-0.1.9/typedhtml/events.py
+-rw-r--r--   0        0        0     7348 2023-07-23 19:50:40.425730 typedhtml-0.1.9/typedhtml/globals.py
+-rw-r--r--   0        0        0        0 2023-07-25 19:54:45.714922 typedhtml-0.1.9/typedhtml/py.typed
+-rw-r--r--   0        0        0     1211 2023-07-23 06:34:06.643229 typedhtml-0.1.9/typedhtml/svg.py
+-rw-r--r--   0        0        0    31931 2023-07-27 20:43:26.614161 typedhtml-0.1.9/typedhtml/tags.py
+-rw-r--r--   0        0        0     9230 2023-07-25 19:34:32.723450 typedhtml-0.1.9/typedhtml/ui5/__init__.py
+-rw-r--r--   0        0        0     3264 2023-07-24 03:41:38.489987 typedhtml-0.1.9/typedhtml/ui5/avatar.py
+-rw-r--r--   0        0        0      863 2023-07-24 03:38:24.465498 typedhtml-0.1.9/typedhtml/ui5/badge.py
+-rw-r--r--   0        0        0      528 2023-07-27 21:07:09.900283 typedhtml-0.1.9/typedhtml/ui5/bar.py
+-rw-r--r--   0        0        0      244 2023-07-25 12:45:43.227706 typedhtml-0.1.9/typedhtml/ui5/barcode_scanner_dialog.py
+-rw-r--r--   0        0        0      692 2023-07-27 16:15:58.159590 typedhtml-0.1.9/typedhtml/ui5/base.py
+-rw-r--r--   0        0        0     1354 2023-07-24 03:41:10.194619 typedhtml-0.1.9/typedhtml/ui5/breadcrumbs.py
+-rw-r--r--   0        0        0      797 2023-07-24 03:42:17.102817 typedhtml-0.1.9/typedhtml/ui5/busy_indicator.py
+-rw-r--r--   0        0        0     1091 2023-07-24 03:42:46.370478 typedhtml-0.1.9/typedhtml/ui5/button.py
+-rw-r--r--   0        0        0     1214 2023-07-24 21:22:07.958588 typedhtml-0.1.9/typedhtml/ui5/calendar.py
+-rw-r--r--   0        0        0     1424 2023-07-24 03:44:35.261001 typedhtml-0.1.9/typedhtml/ui5/card.py
+-rw-r--r--   0        0        0     1356 2023-07-24 03:44:57.515274 typedhtml-0.1.9/typedhtml/ui5/carousel.py
+-rw-r--r--   0        0        0     1405 2023-07-24 03:45:38.605099 typedhtml-0.1.9/typedhtml/ui5/checkbox.py
+-rw-r--r--   0        0        0     1551 2023-07-24 03:48:24.851505 typedhtml-0.1.9/typedhtml/ui5/color_palette.py
+-rw-r--r--   0        0        0      619 2023-07-24 03:48:50.205563 typedhtml-0.1.9/typedhtml/ui5/color_picker.py
+-rw-r--r--   0        0        0     1018 2023-07-24 03:49:37.145966 typedhtml-0.1.9/typedhtml/ui5/combobox.py
+-rw-r--r--   0        0        0     1062 2023-07-24 03:50:02.077503 typedhtml-0.1.9/typedhtml/ui5/datepicker.py
+-rw-r--r--   0        0        0      797 2023-07-24 21:22:33.226998 typedhtml-0.1.9/typedhtml/ui5/daterange_picker.py
+-rw-r--r--   0        0        0      634 2023-07-24 03:51:37.839555 typedhtml-0.1.9/typedhtml/ui5/datetime_picker.py
+-rw-r--r--   0        0        0      724 2023-07-24 03:51:59.287201 typedhtml-0.1.9/typedhtml/ui5/dialog.py
+-rw-r--r--   0        0        0      920 2023-07-25 12:52:50.880741 typedhtml-0.1.9/typedhtml/ui5/dynamic_side_content.py
+-rw-r--r--   0        0        0     1018 2023-07-24 03:52:52.259960 typedhtml-0.1.9/typedhtml/ui5/file_uploader.py
+-rw-r--r--   0        0        0     1066 2023-07-25 13:05:33.331084 typedhtml-0.1.9/typedhtml/ui5/flexible_column_layout.py
+-rw-r--r--   0        0        0      989 2023-07-24 03:53:09.125464 typedhtml-0.1.9/typedhtml/ui5/icon.py
+-rw-r--r--   0        0        0     3220 2023-07-25 15:00:10.774344 typedhtml-0.1.9/typedhtml/ui5/illustrated_message.py
+-rw-r--r--   0        0        0     1104 2023-07-24 18:46:05.721707 typedhtml-0.1.9/typedhtml/ui5/input.py
+-rw-r--r--   0        0        0      677 2023-07-24 03:35:27.924512 typedhtml-0.1.9/typedhtml/ui5/label.py
+-rw-r--r--   0        0        0      848 2023-07-24 04:19:28.264763 typedhtml-0.1.9/typedhtml/ui5/link.py
+-rw-r--r--   0        0        0     2336 2023-07-24 04:55:43.979158 typedhtml-0.1.9/typedhtml/ui5/list.py
+-rw-r--r--   0        0        0     1113 2023-07-25 15:12:47.396435 typedhtml-0.1.9/typedhtml/ui5/media_gallery.py
+-rw-r--r--   0        0        0     1292 2023-07-24 05:07:02.147480 typedhtml-0.1.9/typedhtml/ui5/menu.py
+-rw-r--r--   0        0        0      934 2023-07-24 05:11:38.448763 typedhtml-0.1.9/typedhtml/ui5/message_strip.py
+-rw-r--r--   0        0        0     2111 2023-07-24 05:32:56.437095 typedhtml-0.1.9/typedhtml/ui5/multi_combobox.py
+-rw-r--r--   0        0        0     1217 2023-07-24 05:47:28.390516 typedhtml-0.1.9/typedhtml/ui5/multi_input.py
+-rw-r--r--   0        0        0     1341 2023-07-25 15:35:21.371287 typedhtml-0.1.9/typedhtml/ui5/notification_list_group.py
+-rw-r--r--   0        0        0      651 2023-07-25 19:36:15.108104 typedhtml-0.1.9/typedhtml/ui5/notification_list_item.py
+-rw-r--r--   0        0        0      822 2023-07-25 16:29:47.448554 typedhtml-0.1.9/typedhtml/ui5/page.py
+-rw-r--r--   0        0        0      786 2023-07-24 05:56:13.272720 typedhtml-0.1.9/typedhtml/ui5/panel.py
+-rw-r--r--   0        0        0     1049 2023-07-24 16:47:51.776836 typedhtml-0.1.9/typedhtml/ui5/popover.py
+-rw-r--r--   0        0        0      851 2023-07-25 16:47:28.910479 typedhtml-0.1.9/typedhtml/ui5/product_switch.py
+-rw-r--r--   0        0        0      813 2023-07-24 16:53:02.111474 typedhtml-0.1.9/typedhtml/ui5/progress.py
+-rw-r--r--   0        0        0     1147 2023-07-24 17:23:34.365913 typedhtml-0.1.9/typedhtml/ui5/radio.py
+-rw-r--r--   0        0        0      739 2023-07-24 17:26:16.577498 typedhtml-0.1.9/typedhtml/ui5/range_slider.py
+-rw-r--r--   0        0        0      846 2023-07-24 17:30:46.775794 typedhtml-0.1.9/typedhtml/ui5/rating_indicator.py
+-rw-r--r--   0        0        0      460 2023-07-24 19:03:12.882005 typedhtml-0.1.9/typedhtml/ui5/responsive_popover.py
+-rw-r--r--   0        0        0     1240 2023-07-24 17:45:46.706947 typedhtml-0.1.9/typedhtml/ui5/segmented_button.py
+-rw-r--r--   0        0        0     1330 2023-07-24 17:52:58.144971 typedhtml-0.1.9/typedhtml/ui5/select.py
+-rw-r--r--   0        0        0     1267 2023-07-25 19:13:16.274085 typedhtml-0.1.9/typedhtml/ui5/shell_bar.py
+-rw-r--r--   0        0        0     1369 2023-07-25 17:45:11.869783 typedhtml-0.1.9/typedhtml/ui5/side_nav.py
+-rw-r--r--   0        0        0      686 2023-07-24 18:07:42.261132 typedhtml-0.1.9/typedhtml/ui5/slider.py
+-rw-r--r--   0        0        0      992 2023-07-24 18:15:29.579762 typedhtml-0.1.9/typedhtml/ui5/split_button.py
+-rw-r--r--   0        0        0      925 2023-07-24 18:19:41.715572 typedhtml-0.1.9/typedhtml/ui5/step_input.py
+-rw-r--r--   0        0        0      915 2023-07-24 18:23:43.502304 typedhtml-0.1.9/typedhtml/ui5/switch.py
+-rw-r--r--   0        0        0     1051 2023-07-24 18:37:11.846161 typedhtml-0.1.9/typedhtml/ui5/tab_container.py
+-rw-r--r--   0        0        0     2066 2023-07-24 19:41:17.961063 typedhtml-0.1.9/typedhtml/ui5/table.py
+-rw-r--r--   0        0        0      904 2023-07-24 20:54:41.376476 typedhtml-0.1.9/typedhtml/ui5/textarea.py
+-rw-r--r--   0        0        0      665 2023-07-24 20:57:46.970970 typedhtml-0.1.9/typedhtml/ui5/time_picker.py
+-rw-r--r--   0        0        0      784 2023-07-25 17:58:03.447272 typedhtml-0.1.9/typedhtml/ui5/timeline.py
+-rw-r--r--   0        0        0      566 2023-07-24 21:01:29.280885 typedhtml-0.1.9/typedhtml/ui5/title.py
+-rw-r--r--   0        0        0      708 2023-07-24 21:04:14.974066 typedhtml-0.1.9/typedhtml/ui5/toast.py
+-rw-r--r--   0        0        0      496 2023-07-24 22:06:21.633647 typedhtml-0.1.9/typedhtml/ui5/toggle_button.py
+-rw-r--r--   0        0        0     1135 2023-07-24 22:10:33.706725 typedhtml-0.1.9/typedhtml/ui5/tree.py
+-rw-r--r--   0        0        0     1470 2023-07-25 18:12:53.064206 typedhtml-0.1.9/typedhtml/ui5/upload_collection.py
+-rw-r--r--   0        0        0     1685 2023-07-25 19:37:34.851255 typedhtml-0.1.9/typedhtml/ui5/view_settings_dialog.py
+-rw-r--r--   0        0        0      871 2023-07-25 18:36:11.056458 typedhtml-0.1.9/typedhtml/ui5/wizard.py
+-rw-r--r--   0        0        0      536 2023-07-27 16:09:36.125132 typedhtml-0.1.9/typedhtml/util.py
+-rw-r--r--   0        0        0      427 1970-01-01 00:00:00.000000 typedhtml-0.1.9/PKG-INFO
```

### Comparing `typedhtml-0.1.8/typedhtml/attributes.py` & `typedhtml-0.1.9/typedhtml/attributes.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/document.py` & `typedhtml-0.1.9/typedhtml/document.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/events.py` & `typedhtml-0.1.9/typedhtml/events.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/globals.py` & `typedhtml-0.1.9/typedhtml/globals.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/svg.py` & `typedhtml-0.1.9/typedhtml/svg.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/tags.py` & `typedhtml-0.1.9/typedhtml/tags.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/__init__.py` & `typedhtml-0.1.9/typedhtml/ui5/__init__.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/avatar.py` & `typedhtml-0.1.9/typedhtml/ui5/avatar.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/badge.py` & `typedhtml-0.1.9/typedhtml/ui5/badge.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/bar.py` & `typedhtml-0.1.9/typedhtml/ui5/panel.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,24 @@
 # license that can be found in the LICENSE file.
 
 from typing import Literal, Unpack
 
 from typedhtml.ui5.base import ui5_tag, ui5_tag_props
 
 
-class bar_props(ui5_tag_props, total=False):
-    design: Literal["Header", "SubHeader", "FloatingFooter", "Footer"]
-
-
-class bar(ui5_tag):
-    def __init__(self, *args, **kwargs: Unpack[bar_props]) -> None:
-        self.tagname = "ui5-bar"
-        super().__init__("ui5-bar", *args, **kwargs)
+class panel_props(ui5_tag_props):
+    header_text: str
+    accessible_name: str
+    accessible_role: str
+    collapsed: bool
+    fixed: bool
+    header_level: Literal["H6", "H5", "H4", "H3", "H2", "H1"]
+    no_animation: bool
+
+
+class panel(ui5_tag):
+    """The ui5-panel component is a container which has a header and a content area and
+    can be collapsed to save space on the screen."""
+
+    def __init__(self, *args, **kwargs: Unpack[panel_props]) -> None:
+        self.tagname = "ui5-panel"
+        super().__init__(*args, **kwargs)
```

### Comparing `typedhtml-0.1.8/typedhtml/ui5/base.py` & `typedhtml-0.1.9/typedhtml/ui5/base.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/breadcrumbs.py` & `typedhtml-0.1.9/typedhtml/ui5/breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/busy_indicator.py` & `typedhtml-0.1.9/typedhtml/ui5/busy_indicator.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/button.py` & `typedhtml-0.1.9/typedhtml/ui5/button.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/calendar.py` & `typedhtml-0.1.9/typedhtml/ui5/calendar.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/card.py` & `typedhtml-0.1.9/typedhtml/ui5/card.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/carousel.py` & `typedhtml-0.1.9/typedhtml/ui5/carousel.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/checkbox.py` & `typedhtml-0.1.9/typedhtml/ui5/checkbox.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/color_palette.py` & `typedhtml-0.1.9/typedhtml/ui5/color_palette.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/color_picker.py` & `typedhtml-0.1.9/typedhtml/ui5/color_picker.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/combobox.py` & `typedhtml-0.1.9/typedhtml/ui5/combobox.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/datepicker.py` & `typedhtml-0.1.9/typedhtml/ui5/datepicker.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/daterange_picker.py` & `typedhtml-0.1.9/typedhtml/ui5/daterange_picker.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/datetime_picker.py` & `typedhtml-0.1.9/typedhtml/ui5/datetime_picker.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/dialog.py` & `typedhtml-0.1.9/typedhtml/ui5/dialog.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/dynamic_side_content.py` & `typedhtml-0.1.9/typedhtml/ui5/dynamic_side_content.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/file_uploader.py` & `typedhtml-0.1.9/typedhtml/ui5/file_uploader.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/flexible_column_layout.py` & `typedhtml-0.1.9/typedhtml/ui5/flexible_column_layout.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/icon.py` & `typedhtml-0.1.9/typedhtml/ui5/icon.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/illustrated_message.py` & `typedhtml-0.1.9/typedhtml/ui5/illustrated_message.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/input.py` & `typedhtml-0.1.9/typedhtml/ui5/input.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/label.py` & `typedhtml-0.1.9/typedhtml/ui5/label.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/link.py` & `typedhtml-0.1.9/typedhtml/ui5/link.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/list.py` & `typedhtml-0.1.9/typedhtml/ui5/list.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/media_gallery.py` & `typedhtml-0.1.9/typedhtml/ui5/media_gallery.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/menu.py` & `typedhtml-0.1.9/typedhtml/ui5/menu.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/message_strip.py` & `typedhtml-0.1.9/typedhtml/ui5/message_strip.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/multi_combobox.py` & `typedhtml-0.1.9/typedhtml/ui5/multi_combobox.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/multi_input.py` & `typedhtml-0.1.9/typedhtml/ui5/multi_input.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/notification_list_group.py` & `typedhtml-0.1.9/typedhtml/ui5/notification_list_group.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/notification_list_item.py` & `typedhtml-0.1.9/typedhtml/ui5/notification_list_item.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/page.py` & `typedhtml-0.1.9/typedhtml/ui5/page.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/panel.py` & `typedhtml-0.1.9/typedhtml/ui5/textarea.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 # Copyright 2023 Takin Profit. All rights reserved.
 # Use of this source code is governed by a BSD-style
 # license that can be found in the LICENSE file.
 
+
 from typing import Literal, Unpack
 
 from typedhtml.ui5.base import ui5_tag, ui5_tag_props
 
 
-class panel_props(ui5_tag_props):
-    header_text: str
+class textarea_props(ui5_tag_props, total=False):
+    placeholder: str
     accessible_name: str
-    accessible_role: str
-    collapsed: bool
-    fixed: bool
-    header_level: Literal["H6", "H5", "H4", "H3", "H2", "H1"]
-    no_animation: bool
+    accessible_name_ref: str
+    disabled: bool
+    growing: bool
+    growing_max_lines: int
+    maxlength: int
+    name: str
+    readonly: bool
+    required: bool
+    rows: int
+    show_exceeded_text: bool
+    value: str
+    value_state: Literal["None", "Error", "Warning", "Success", "Information"]
 
 
-class panel(ui5_tag):
-    """The ui5-panel component is a container which has a header and a content area and
-    can be collapsed to save space on the screen."""
+class textarea(ui5_tag):
+    """The ui5-textarea component is used to enter multiple lines of text."""
 
-    def __init__(self, *args, **kwargs: Unpack[panel_props]) -> None:
-        self.tagname = "ui5-panel"
+    def __init__(self, *args, **kwargs: Unpack[textarea_props]) -> None:
+        self.tagname = "ui5-textarea"
         super().__init__(*args, **kwargs)
```

### Comparing `typedhtml-0.1.8/typedhtml/ui5/popover.py` & `typedhtml-0.1.9/typedhtml/ui5/popover.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/product_switch.py` & `typedhtml-0.1.9/typedhtml/ui5/product_switch.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/progress.py` & `typedhtml-0.1.9/typedhtml/ui5/progress.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/radio.py` & `typedhtml-0.1.9/typedhtml/ui5/radio.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/range_slider.py` & `typedhtml-0.1.9/typedhtml/ui5/range_slider.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/rating_indicator.py` & `typedhtml-0.1.9/typedhtml/ui5/rating_indicator.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/segmented_button.py` & `typedhtml-0.1.9/typedhtml/ui5/segmented_button.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/select.py` & `typedhtml-0.1.9/typedhtml/ui5/select.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/shell_bar.py` & `typedhtml-0.1.9/typedhtml/ui5/shell_bar.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/side_nav.py` & `typedhtml-0.1.9/typedhtml/ui5/side_nav.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/slider.py` & `typedhtml-0.1.9/typedhtml/ui5/slider.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/split_button.py` & `typedhtml-0.1.9/typedhtml/ui5/split_button.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/step_input.py` & `typedhtml-0.1.9/typedhtml/ui5/step_input.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/switch.py` & `typedhtml-0.1.9/typedhtml/ui5/switch.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/tab_container.py` & `typedhtml-0.1.9/typedhtml/ui5/tab_container.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/table.py` & `typedhtml-0.1.9/typedhtml/ui5/table.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/textarea.py` & `typedhtml-0.1.9/typedhtml/ui5/time_picker.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,23 @@
 # Copyright 2023 Takin Profit. All rights reserved.
 # Use of this source code is governed by a BSD-style
 # license that can be found in the LICENSE file.
 
 
-from typing import Literal, Unpack
+from typing import Unpack
 
 from typedhtml.ui5.base import ui5_tag, ui5_tag_props
 
 
-class textarea_props(ui5_tag_props, total=False):
-    placeholder: str
-    accessible_name: str
-    accessible_name_ref: str
-    disabled: bool
-    growing: bool
-    growing_max_lines: int
-    maxlength: int
-    name: str
-    readonly: bool
-    required: bool
-    rows: int
-    show_exceeded_text: bool
-    value: str
-    value_state: Literal["None", "Error", "Warning", "Success", "Information"]
+class time_picker_props(ui5_tag_props, total=False):
+    date_value: str
+    format_pattern: str
+    place_holder: str
 
 
-class textarea(ui5_tag):
-    """The ui5-textarea component is used to enter multiple lines of text."""
+class time_picker(ui5_tag):
+    """The ui5-time-picker component provides an input field with assigned clocks
+    which opens on user action."""
 
-    def __init__(self, *args, **kwargs: Unpack[textarea_props]) -> None:
-        self.tagname = "ui5-textarea"
+    def __init__(self, *args, **kwargs: Unpack[time_picker_props]) -> None:
+        self.tagname = "ui5-time-picker"
         super().__init__(*args, **kwargs)
```

### Comparing `typedhtml-0.1.8/typedhtml/ui5/timeline.py` & `typedhtml-0.1.9/typedhtml/ui5/timeline.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/title.py` & `typedhtml-0.1.9/typedhtml/ui5/title.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/toast.py` & `typedhtml-0.1.9/typedhtml/ui5/toast.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/tree.py` & `typedhtml-0.1.9/typedhtml/ui5/tree.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/upload_collection.py` & `typedhtml-0.1.9/typedhtml/ui5/upload_collection.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/view_settings_dialog.py` & `typedhtml-0.1.9/typedhtml/ui5/view_settings_dialog.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/ui5/wizard.py` & `typedhtml-0.1.9/typedhtml/ui5/wizard.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.8/typedhtml/util.py` & `typedhtml-0.1.9/typedhtml/util.py`

 * *Files identical despite different names*

