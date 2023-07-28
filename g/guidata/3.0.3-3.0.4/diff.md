# Comparing `tmp/guidata-3.0.3.tar.gz` & `tmp/guidata-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guidata-3.0.3.tar", last modified: Wed Jul 26 12:43:40 2023, max compression
+gzip compressed data, was "guidata-3.0.4.tar", last modified: Fri Jul 28 10:12:06 2023, max compression
```

## Comparing `guidata-3.0.3.tar` & `guidata-3.0.4.tar`

### file list

```diff
@@ -1,220 +1,223 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.597999 guidata-3.0.3/
--rw-rw-rw-   0        0        0     1563 2023-07-06 12:28:58.000000 guidata-3.0.3/LICENSE
--rw-rw-rw-   0        0        0        9 2023-07-26 09:34:47.000000 guidata-3.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6016 2023-07-26 12:43:40.597000 guidata-3.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2977 2023-07-26 12:41:54.000000 guidata-3.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.025030 guidata-3.0.3/doc/
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.027030 guidata-3.0.3/doc/_static/
--rw-rw-rw-   0        0        0    97375 2023-06-30 10:35:52.000000 guidata-3.0.3/doc/_static/favicon.ico
--rw-rw-rw-   0        0        0      734 2023-06-12 16:28:37.000000 guidata-3.0.3/doc/basic_example.py
--rw-rw-rw-   0        0        0     1659 2023-07-21 12:45:55.000000 guidata-3.0.3/doc/conf.py
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.039031 guidata-3.0.3/doc/dev/
--rw-rw-rw-   0        0        0     2675 2023-07-21 10:37:23.000000 guidata-3.0.3/doc/dev/contribute.rst
--rw-rw-rw-   0        0        0      975 2023-07-06 12:59:03.000000 guidata-3.0.3/doc/dev/howto.rst
--rw-rw-rw-   0        0        0      123 2023-07-06 12:57:35.000000 guidata-3.0.3/doc/dev/index.rst
--rw-rw-rw-   0        0        0     2171 2023-07-19 10:06:27.000000 guidata-3.0.3/doc/dev/v2_to_v3.csv
--rw-rw-rw-   0        0        0     1186 2023-07-26 08:50:26.000000 guidata-3.0.3/doc/dev/v2_to_v3.rst
--rw-rw-rw-   0        0        0     1631 2023-07-06 14:12:31.000000 guidata-3.0.3/doc/examples.rst
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.048046 guidata-3.0.3/doc/images/
--rw-rw-rw-   0        0        0     4718 2023-07-06 12:12:29.000000 guidata-3.0.3/doc/images/basic_example.png
--rw-rw-rw-   0        0        0    16573 2023-07-06 15:02:39.000000 guidata-3.0.3/doc/images/guidata-banner.png
--rw-rw-rw-   0        0        0     6176 2023-06-30 10:38:57.000000 guidata-3.0.3/doc/images/guidata-vertical.png
--rw-rw-rw-   0        0        0    14799 2023-07-06 12:21:56.000000 guidata-3.0.3/doc/images/layout_example.png
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.069030 guidata-3.0.3/doc/images/screenshots/
--rw-rw-rw-   0        0        0    78499 2023-07-06 12:13:38.000000 guidata-3.0.3/doc/images/screenshots/__init__.png
--rw-rw-rw-   0        0        0     4765 2023-07-06 12:14:34.000000 guidata-3.0.3/doc/images/screenshots/activable_dataset.png
--rw-rw-rw-   0        0        0    31447 2023-07-06 12:15:25.000000 guidata-3.0.3/doc/images/screenshots/all_features.png
--rw-rw-rw-   0        0        0    37993 2023-07-06 12:15:56.000000 guidata-3.0.3/doc/images/screenshots/all_items.png
--rw-rw-rw-   0        0        0     8866 2023-07-06 12:16:16.000000 guidata-3.0.3/doc/images/screenshots/bool_selector.png
--rw-rw-rw-   0        0        0    32420 2023-07-06 12:16:41.000000 guidata-3.0.3/doc/images/screenshots/datasetgroup.png
--rw-rw-rw-   0        0        0    20345 2023-07-06 12:17:05.000000 guidata-3.0.3/doc/images/screenshots/editgroupbox.png
--rw-rw-rw-   0        0        0      933 2023-07-18 09:00:42.000000 guidata-3.0.3/doc/index.rst
--rw-rw-rw-   0        0        0      181 2023-07-21 12:29:31.000000 guidata-3.0.3/doc/installation.rst
--rw-rw-rw-   0        0        0     1731 2023-07-06 12:22:51.000000 guidata-3.0.3/doc/overview.rst
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.086038 guidata-3.0.3/doc/reference/
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.096032 guidata-3.0.3/doc/reference/dataset/
--rw-rw-rw-   0        0        0       43 2023-06-30 13:46:46.000000 guidata-3.0.3/doc/reference/dataset/dataitems.rst
--rw-rw-rw-   0        0        0       43 2023-06-30 13:46:54.000000 guidata-3.0.3/doc/reference/dataset/datatypes.rst
--rw-rw-rw-   0        0        0      144 2023-07-07 14:10:24.000000 guidata-3.0.3/doc/reference/dataset/index.rst
--rw-rw-rw-   0        0        0       34 2023-07-19 09:25:53.000000 guidata-3.0.3/doc/reference/dataset/io.rst
--rw-rw-rw-   0        0        0       43 2023-06-30 13:46:30.000000 guidata-3.0.3/doc/reference/dataset/qtwidgets.rst
--rw-rw-rw-   0        0        0       33 2023-06-30 12:46:29.000000 guidata-3.0.3/doc/reference/guitest.rst
--rw-rw-rw-   0        0        0      148 2023-07-07 14:21:56.000000 guidata-3.0.3/doc/reference/index.rst
--rw-rw-rw-   0        0        0       34 2023-07-07 14:22:12.000000 guidata-3.0.3/doc/reference/userconfig.rst
--rw-rw-rw-   0        0        0      130 2023-06-30 12:45:12.000000 guidata-3.0.3/doc/reference/utils.rst
--rw-rw-rw-   0        0        0      120 2023-06-30 10:49:38.000000 guidata-3.0.3/doc/reference/widgets.rst
--rw-rw-rw-   0        0        0     2460 2023-07-26 12:43:21.000000 guidata-3.0.3/doc/requirements.rst
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.114032 guidata-3.0.3/guidata/
--rw-rw-rw-   0        0        0     3004 2023-07-26 12:34:51.000000 guidata-3.0.3/guidata/__init__.py
--rw-rw-rw-   0        0        0    11296 2023-07-06 14:12:49.000000 guidata-3.0.3/guidata/config.py
--rw-rw-rw-   0        0        0    13964 2023-07-19 16:04:51.000000 guidata-3.0.3/guidata/configtools.py
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.145033 guidata-3.0.3/guidata/dataset/
--rw-rw-rw-   0        0        0      535 2023-07-06 12:39:33.000000 guidata-3.0.3/guidata/dataset/__init__.py
--rw-rw-rw-   0        0        0    33518 2023-07-19 16:11:47.000000 guidata-3.0.3/guidata/dataset/dataitems.py
--rw-rw-rw-   0        0        0    45137 2023-07-19 16:09:55.000000 guidata-3.0.3/guidata/dataset/datatypes.py
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.159032 guidata-3.0.3/guidata/dataset/io/
--rw-rw-rw-   0        0        0     1702 2023-07-19 16:10:46.000000 guidata-3.0.3/guidata/dataset/io/__init__.py
--rw-rw-rw-   0        0        0     5978 2023-07-19 09:51:48.000000 guidata-3.0.3/guidata/dataset/io/base.py
--rw-rw-rw-   0        0        0    23319 2023-07-19 16:04:45.000000 guidata-3.0.3/guidata/dataset/io/h5fmt.py
--rw-rw-rw-   0        0        0     5576 2023-07-19 10:06:28.000000 guidata-3.0.3/guidata/dataset/io/inifmt.py
--rw-rw-rw-   0        0        0     8428 2023-07-19 09:51:48.000000 guidata-3.0.3/guidata/dataset/io/jsonfmt.py
--rw-rw-rw-   0        0        0    40609 2023-07-18 14:45:16.000000 guidata-3.0.3/guidata/dataset/qtitemwidgets.py
--rw-rw-rw-   0        0        0    23426 2023-07-06 12:39:33.000000 guidata-3.0.3/guidata/dataset/qtwidgets.py
--rw-rw-rw-   0        0        0      820 2023-07-06 12:39:33.000000 guidata-3.0.3/guidata/dataset/textedit.py
--rw-rw-rw-   0        0        0     6093 2023-07-06 12:40:25.000000 guidata-3.0.3/guidata/env.py
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.161033 guidata-3.0.3/guidata/external/
--rw-rw-rw-   0        0        0        1 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/external/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.176037 guidata-3.0.3/guidata/external/darkdetect/
--rw-rw-rw-   0        0        0     1289 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/external/darkdetect/__init__.py
--rw-rw-rw-   0        0        0      377 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/external/darkdetect/_dummy.py
--rw-rw-rw-   0        0        0      890 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/external/darkdetect/_linux_detect.py
--rw-rw-rw-   0        0        0     2212 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/external/darkdetect/_mac_detect.py
--rw-rw-rw-   0        0        0     1257 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/external/darkdetect/_windows_detect.py
--rw-rw-rw-   0        0        0   394832 2023-07-26 12:43:19.000000 guidata-3.0.3/guidata/guidata.chm
--rw-rw-rw-   0        0        0    11214 2023-07-19 16:04:52.000000 guidata-3.0.3/guidata/guitest.py
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.298038 guidata-3.0.3/guidata/images/
--rw-rw-rw-   0        0        0      785 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/apply.png
--rw-rw-rw-   0        0        0     1123 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/arredit.png
--rw-rw-rw-   0        0        0      721 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/busy.png
--rw-rw-rw-   0        0        0      689 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/cell_edit.png
--rw-rw-rw-   0        0        0      830 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/copy.png
--rw-rw-rw-   0        0        0      722 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/delete.png
--rw-rw-rw-   0        0        0      911 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/dictedit.png
--rw-rw-rw-   0        0        0      735 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/dtype.png
--rw-rw-rw-   0        0        0      929 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/edit.png
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.342877 guidata-3.0.3/guidata/images/editors/
--rw-rw-rw-   0        0        0      911 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/editors/copywop.png
--rw-rw-rw-   0        0        0      929 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/editors/edit.png
--rw-rw-rw-   0        0        0     1001 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/editors/edit_add.png
--rw-rw-rw-   0        0        0     1777 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/editors/editclear.png
--rw-rw-rw-   0        0        0     1048 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/editors/editcopy.png
--rw-rw-rw-   0        0        0      824 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/editors/editcut.png
--rw-rw-rw-   0        0        0     1453 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/editors/editdelete.png
--rw-rw-rw-   0        0        0     1295 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/editors/editpaste.png
--rw-rw-rw-   0        0        0     2248 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/editors/fileimport.png
--rw-rw-rw-   0        0        0     1144 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/editors/filesave.png
--rw-rw-rw-   0        0        0      727 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/editors/imshow.png
--rw-rw-rw-   0        0        0      525 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/editors/insert.png
--rw-rw-rw-   0        0        0      515 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/editors/plot.png
--rw-rw-rw-   0        0        0      689 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/editors/rename.png
--rw-rw-rw-   0        0        0     1184 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/editors/selectall.png
--rw-rw-rw-   0        0        0     1164 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/exit.png
--rw-rw-rw-   0        0        0      165 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/expander_down.png
--rw-rw-rw-   0        0        0      432 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/expander_right.png
--rw-rw-rw-   0        0        0      530 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/file.png
--rw-rw-rw-   0        0        0     1424 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/fileclose.png
--rw-rw-rw-   0        0        0     1556 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/fileimport.png
--rw-rw-rw-   0        0        0      463 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filenew.png
--rw-rw-rw-   0        0        0     1539 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/fileopen.png
--rw-rw-rw-   0        0        0     1144 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filesave.png
--rw-rw-rw-   0        0        0     1443 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filesaveas.png
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.390044 guidata-3.0.3/guidata/images/filetypes/
--rw-rw-rw-   0        0        0     1601 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filetypes/doc.png
--rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filetypes/gif.png
--rw-rw-rw-   0        0        0     1848 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filetypes/html.png
--rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filetypes/jpg.png
--rw-rw-rw-   0        0        0     1543 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filetypes/pdf.png
--rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filetypes/png.png
--rw-rw-rw-   0        0        0     1439 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filetypes/pps.png
--rw-rw-rw-   0        0        0     1428 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filetypes/ps.png
--rw-rw-rw-   0        0        0     1577 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filetypes/tar.png
--rw-rw-rw-   0        0        0     1577 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filetypes/tgz.png
--rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filetypes/tif.png
--rw-rw-rw-   0        0        0     1801 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filetypes/txt.png
--rw-rw-rw-   0        0        0     1237 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filetypes/xls.png
--rw-rw-rw-   0        0        0     1577 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filetypes/zip.png
--rw-rw-rw-   0        0        0    16434 2023-07-06 15:03:14.000000 guidata-3.0.3/guidata/images/guidata-banner.svg
--rw-rw-rw-   0        0        0    16406 2023-06-30 10:39:39.000000 guidata-3.0.3/guidata/images/guidata-vertical.svg
--rw-rw-rw-   0        0        0    15818 2023-06-30 10:21:40.000000 guidata-3.0.3/guidata/images/guidata.svg
--rw-rw-rw-   0        0        0      356 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/max.png
--rw-rw-rw-   0        0        0      351 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/min.png
--rw-rw-rw-   0        0        0      331 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/none.png
--rw-rw-rw-   0        0        0      531 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/not_found.png
--rw-rw-rw-   0        0        0      887 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/python.png
--rw-rw-rw-   0        0        0      888 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/quickview.png
--rw-rw-rw-   0        0        0     1599 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/save_all.png
--rw-rw-rw-   0        0        0      744 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/selection.png
--rw-rw-rw-   0        0        0     2445 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/settings.png
--rw-rw-rw-   0        0        0      361 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/shape.png
--rw-rw-rw-   0        0        0      354 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/xmax.png
--rw-rw-rw-   0        0        0      353 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/xmin.png
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:39.979028 guidata-3.0.3/guidata/locale/
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:39.984030 guidata-3.0.3/guidata/locale/fr/
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.394045 guidata-3.0.3/guidata/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0    10186 2023-06-29 17:09:10.000000 guidata-3.0.3/guidata/locale/fr/LC_MESSAGES/guidata.mo
--rw-rw-rw-   0        0        0    20476 2023-07-19 16:01:55.000000 guidata-3.0.3/guidata/qthelpers.py
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.497996 guidata-3.0.3/guidata/tests/
--rw-rw-rw-   0        0        0      368 2023-07-06 12:39:33.000000 guidata-3.0.3/guidata/tests/__init__.py
--rw-rw-rw-   0        0        0     1709 2023-06-30 14:48:32.000000 guidata-3.0.3/guidata/tests/_all_tests.py
--rw-rw-rw-   0        0        0      469 2023-07-18 14:57:07.000000 guidata-3.0.3/guidata/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:39.989056 guidata-3.0.3/guidata/tests/data/
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.501996 guidata-3.0.3/guidata/tests/data/genreqs/
--rw-rw-rw-   0        0        0     2002 2023-07-21 12:09:05.000000 guidata-3.0.3/guidata/tests/data/genreqs/pyproject.toml
--rw-rw-rw-   0        0        0     1493 2023-07-21 12:25:47.000000 guidata-3.0.3/guidata/tests/data/genreqs/setup.cfg
--rw-rw-rw-   0        0        0     1724 2023-07-06 14:13:35.000000 guidata-3.0.3/guidata/tests/test_activable_dataset.py
--rw-rw-rw-   0        0        0     1153 2023-07-06 14:13:43.000000 guidata-3.0.3/guidata/tests/test_activable_items.py
--rw-rw-rw-   0        0        0     4858 2023-07-06 14:13:50.000000 guidata-3.0.3/guidata/tests/test_all_features.py
--rw-rw-rw-   0        0        0     3577 2023-07-06 14:13:57.000000 guidata-3.0.3/guidata/tests/test_all_items.py
--rw-rw-rw-   0        0        0     2601 2023-07-06 14:14:03.000000 guidata-3.0.3/guidata/tests/test_arrayeditor.py
--rw-rw-rw-   0        0        0     1932 2023-07-06 14:14:10.000000 guidata-3.0.3/guidata/tests/test_bool_selector.py
--rw-rw-rw-   0        0        0     2049 2023-07-06 14:14:16.000000 guidata-3.0.3/guidata/tests/test_callbacks.py
--rw-rw-rw-   0        0        0      652 2023-07-06 14:14:23.000000 guidata-3.0.3/guidata/tests/test_codeeditor.py
--rw-rw-rw-   0        0        0     3955 2023-07-18 15:13:56.000000 guidata-3.0.3/guidata/tests/test_collectionseditor.py
--rw-rw-rw-   0        0        0     1068 2023-07-06 12:39:33.000000 guidata-3.0.3/guidata/tests/test_config.py
--rw-rw-rw-   0        0        0      598 2023-07-06 14:14:35.000000 guidata-3.0.3/guidata/tests/test_console.py
--rw-rw-rw-   0        0        0     1413 2023-07-06 14:14:42.000000 guidata-3.0.3/guidata/tests/test_data.py
--rw-rw-rw-   0        0        0     2104 2023-07-18 14:56:56.000000 guidata-3.0.3/guidata/tests/test_dataframeeditor.py
--rw-rw-rw-   0        0        0      869 2023-07-06 12:39:33.000000 guidata-3.0.3/guidata/tests/test_datasetgroup.py
--rw-rw-rw-   0        0        0      962 2023-07-06 12:41:46.000000 guidata-3.0.3/guidata/tests/test_disthelpers.py
--rw-rw-rw-   0        0        0     6052 2023-07-18 14:11:17.000000 guidata-3.0.3/guidata/tests/test_editgroupbox.py
--rw-rw-rw-   0        0        0      839 2023-07-21 12:12:15.000000 guidata-3.0.3/guidata/tests/test_genreqs.py
--rw-rw-rw-   0        0        0      779 2023-07-06 14:15:14.000000 guidata-3.0.3/guidata/tests/test_importwizard.py
--rw-rw-rw-   0        0        0     1511 2023-07-06 14:15:21.000000 guidata-3.0.3/guidata/tests/test_inheritance.py
--rw-rw-rw-   0        0        0     1321 2023-07-06 14:15:27.000000 guidata-3.0.3/guidata/tests/test_item_order.py
--rw-rw-rw-   0        0        0     1142 2023-07-26 11:35:40.000000 guidata-3.0.3/guidata/tests/test_loadsave_hdf5.py
--rw-rw-rw-   0        0        0     1078 2023-07-26 11:35:40.000000 guidata-3.0.3/guidata/tests/test_loadsave_json.py
--rw-rw-rw-   0        0        0      714 2023-07-07 12:57:07.000000 guidata-3.0.3/guidata/tests/test_no_qt.py
--rw-rw-rw-   0        0        0     1578 2023-07-18 15:02:08.000000 guidata-3.0.3/guidata/tests/test_objecteditor.py
--rw-rw-rw-   0        0        0     1361 2023-07-06 14:15:41.000000 guidata-3.0.3/guidata/tests/test_rotatedlabel.py
--rw-rw-rw-   0        0        0      818 2023-07-06 14:15:48.000000 guidata-3.0.3/guidata/tests/test_text.py
--rw-rw-rw-   0        0        0      493 2023-07-06 12:40:58.000000 guidata-3.0.3/guidata/tests/test_translations.py
--rw-rw-rw-   0        0        0      778 2023-06-29 14:26:00.000000 guidata-3.0.3/guidata/tests/test_userconfig_app.py
--rw-rw-rw-   0        0        0    15176 2023-07-07 14:24:22.000000 guidata-3.0.3/guidata/userconfig.py
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.526996 guidata-3.0.3/guidata/utils/
--rw-rw-rw-   0        0        0     2858 2023-07-19 16:04:50.000000 guidata-3.0.3/guidata/utils/__init__.py
--rw-rw-rw-   0        0        0    43150 2023-07-06 12:41:24.000000 guidata-3.0.3/guidata/utils/disthelpers.py
--rw-rw-rw-   0        0        0     6408 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/utils/encoding.py
--rw-rw-rw-   0        0        0     6977 2023-07-21 12:45:00.000000 guidata-3.0.3/guidata/utils/genreqs.py
--rw-rw-rw-   0        0        0     4025 2023-07-06 12:39:27.000000 guidata-3.0.3/guidata/utils/gettext_helpers.py
--rw-rw-rw-   0        0        0    10494 2023-07-19 16:04:50.000000 guidata-3.0.3/guidata/utils/misc.py
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.562998 guidata-3.0.3/guidata/widgets/
--rw-rw-rw-   0        0        0      729 2023-07-06 12:41:42.000000 guidata-3.0.3/guidata/widgets/__init__.py
--rw-rw-rw-   0        0        0    33274 2023-06-30 13:14:39.000000 guidata-3.0.3/guidata/widgets/arrayeditor.py
--rw-rw-rw-   0        0        0    13477 2023-06-30 14:48:54.000000 guidata-3.0.3/guidata/widgets/codeeditor.py
--rw-rw-rw-   0        0        0    55677 2023-07-18 15:07:59.000000 guidata-3.0.3/guidata/widgets/collectionseditor.py
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.594999 guidata-3.0.3/guidata/widgets/console/
--rw-rw-rw-   0        0        0     3257 2023-06-30 12:22:39.000000 guidata-3.0.3/guidata/widgets/console/__init__.py
--rw-rw-rw-   0        0        0    59019 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/widgets/console/base.py
--rw-rw-rw-   0        0        0    12513 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/widgets/console/calltip.py
--rw-rw-rw-   0        0        0    11610 2023-06-30 15:04:24.000000 guidata-3.0.3/guidata/widgets/console/dochelpers.py
--rw-rw-rw-   0        0        0    15411 2023-06-30 14:59:03.000000 guidata-3.0.3/guidata/widgets/console/internalshell.py
--rw-rw-rw-   0        0        0    12585 2023-06-30 12:28:06.000000 guidata-3.0.3/guidata/widgets/console/interpreter.py
--rw-rw-rw-   0        0        0    30662 2023-06-30 12:40:32.000000 guidata-3.0.3/guidata/widgets/console/mixins.py
--rw-rw-rw-   0        0        0    33285 2023-07-06 14:15:58.000000 guidata-3.0.3/guidata/widgets/console/shell.py
--rw-rw-rw-   0        0        0     4099 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/widgets/console/terminal.py
--rw-rw-rw-   0        0        0    32563 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/widgets/dataframeeditor.py
--rw-rw-rw-   0        0        0     3614 2023-07-19 16:00:45.000000 guidata-3.0.3/guidata/widgets/dockable.py
--rw-rw-rw-   0        0        0    24121 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/widgets/importwizard.py
--rw-rw-rw-   0        0        0    23460 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/widgets/nsview.py
--rw-rw-rw-   0        0        0     3533 2023-07-19 16:04:51.000000 guidata-3.0.3/guidata/widgets/objecteditor.py
--rw-rw-rw-   0        0        0     2122 2023-07-06 12:41:23.000000 guidata-3.0.3/guidata/widgets/rotatedlabel.py
--rw-rw-rw-   0        0        0    62527 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/widgets/syntaxhighlighters.py
--rw-rw-rw-   0        0        0     4022 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/widgets/texteditor.py
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.129033 guidata-3.0.3/guidata.egg-info/
--rw-rw-rw-   0        0        0     6016 2023-07-26 12:43:39.000000 guidata-3.0.3/guidata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5799 2023-07-26 12:43:39.000000 guidata-3.0.3/guidata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 12:43:39.000000 guidata-3.0.3/guidata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      224 2023-07-26 12:43:39.000000 guidata-3.0.3/guidata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-26 12:43:39.000000 guidata-3.0.3/guidata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1974 2023-07-26 12:28:44.000000 guidata-3.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-26 12:43:40.597999 guidata-3.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:06.384640 guidata-3.0.4/
+-rw-rw-rw-   0        0        0     1563 2023-07-06 12:28:58.000000 guidata-3.0.4/LICENSE
+-rw-rw-rw-   0        0        0       28 2023-07-28 10:11:21.000000 guidata-3.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     6016 2023-07-28 10:12:06.362902 guidata-3.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2977 2023-07-26 12:41:54.000000 guidata-3.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:05.731010 guidata-3.0.4/doc/
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:05.733007 guidata-3.0.4/doc/_static/
+-rw-rw-rw-   0        0        0    97375 2023-06-30 10:35:52.000000 guidata-3.0.4/doc/_static/favicon.ico
+-rw-rw-rw-   0        0        0      734 2023-06-12 16:28:37.000000 guidata-3.0.4/doc/basic_example.py
+-rw-rw-rw-   0        0        0     1528 2023-07-28 09:19:34.000000 guidata-3.0.4/doc/conf.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:05.746007 guidata-3.0.4/doc/dev/
+-rw-rw-rw-   0        0        0     2675 2023-07-21 10:37:23.000000 guidata-3.0.4/doc/dev/contribute.rst
+-rw-rw-rw-   0        0        0      975 2023-07-06 12:59:03.000000 guidata-3.0.4/doc/dev/howto.rst
+-rw-rw-rw-   0        0        0      123 2023-07-06 12:57:35.000000 guidata-3.0.4/doc/dev/index.rst
+-rw-rw-rw-   0        0        0     2171 2023-07-19 10:06:27.000000 guidata-3.0.4/doc/dev/v2_to_v3.csv
+-rw-rw-rw-   0        0        0     1186 2023-07-26 08:50:26.000000 guidata-3.0.4/doc/dev/v2_to_v3.rst
+-rw-rw-rw-   0        0        0     1631 2023-07-06 14:12:31.000000 guidata-3.0.4/doc/examples.rst
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:05.756005 guidata-3.0.4/doc/images/
+-rw-rw-rw-   0        0        0     4718 2023-07-06 12:12:29.000000 guidata-3.0.4/doc/images/basic_example.png
+-rw-rw-rw-   0        0        0    16573 2023-07-06 15:02:39.000000 guidata-3.0.4/doc/images/guidata-banner.png
+-rw-rw-rw-   0        0        0     6176 2023-06-30 10:38:57.000000 guidata-3.0.4/doc/images/guidata-vertical.png
+-rw-rw-rw-   0        0        0    14799 2023-07-06 12:21:56.000000 guidata-3.0.4/doc/images/layout_example.png
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:05.776004 guidata-3.0.4/doc/images/screenshots/
+-rw-rw-rw-   0        0        0    78499 2023-07-06 12:13:38.000000 guidata-3.0.4/doc/images/screenshots/__init__.png
+-rw-rw-rw-   0        0        0     4765 2023-07-06 12:14:34.000000 guidata-3.0.4/doc/images/screenshots/activable_dataset.png
+-rw-rw-rw-   0        0        0    31447 2023-07-06 12:15:25.000000 guidata-3.0.4/doc/images/screenshots/all_features.png
+-rw-rw-rw-   0        0        0    37993 2023-07-06 12:15:56.000000 guidata-3.0.4/doc/images/screenshots/all_items.png
+-rw-rw-rw-   0        0        0     8866 2023-07-06 12:16:16.000000 guidata-3.0.4/doc/images/screenshots/bool_selector.png
+-rw-rw-rw-   0        0        0    32420 2023-07-06 12:16:41.000000 guidata-3.0.4/doc/images/screenshots/datasetgroup.png
+-rw-rw-rw-   0        0        0    20345 2023-07-06 12:17:05.000000 guidata-3.0.4/doc/images/screenshots/editgroupbox.png
+-rw-rw-rw-   0        0        0      933 2023-07-18 09:00:42.000000 guidata-3.0.4/doc/index.rst
+-rw-rw-rw-   0        0        0      540 2023-07-26 16:55:42.000000 guidata-3.0.4/doc/installation.rst
+-rw-rw-rw-   0        0        0     1731 2023-07-06 12:22:51.000000 guidata-3.0.4/doc/overview.rst
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:05.789008 guidata-3.0.4/doc/reference/
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:05.800007 guidata-3.0.4/doc/reference/dataset/
+-rw-rw-rw-   0        0        0       43 2023-06-30 13:46:46.000000 guidata-3.0.4/doc/reference/dataset/dataitems.rst
+-rw-rw-rw-   0        0        0       43 2023-06-30 13:46:54.000000 guidata-3.0.4/doc/reference/dataset/datatypes.rst
+-rw-rw-rw-   0        0        0      144 2023-07-07 14:10:24.000000 guidata-3.0.4/doc/reference/dataset/index.rst
+-rw-rw-rw-   0        0        0       34 2023-07-19 09:25:53.000000 guidata-3.0.4/doc/reference/dataset/io.rst
+-rw-rw-rw-   0        0        0       43 2023-06-30 13:46:30.000000 guidata-3.0.4/doc/reference/dataset/qtwidgets.rst
+-rw-rw-rw-   0        0        0       33 2023-06-30 12:46:29.000000 guidata-3.0.4/doc/reference/guitest.rst
+-rw-rw-rw-   0        0        0      148 2023-07-07 14:21:56.000000 guidata-3.0.4/doc/reference/index.rst
+-rw-rw-rw-   0        0        0       34 2023-07-07 14:22:12.000000 guidata-3.0.4/doc/reference/userconfig.rst
+-rw-rw-rw-   0        0        0      130 2023-06-30 12:45:12.000000 guidata-3.0.4/doc/reference/utils.rst
+-rw-rw-rw-   0        0        0      120 2023-06-30 10:49:38.000000 guidata-3.0.4/doc/reference/widgets.rst
+-rw-rw-rw-   0        0        0     2460 2023-07-28 10:11:37.000000 guidata-3.0.4/doc/requirements.rst
+-rw-rw-rw-   0        0        0      721 2023-07-28 09:23:28.000000 guidata-3.0.4/doc/update_requirements.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:05.819008 guidata-3.0.4/guidata/
+-rw-rw-rw-   0        0        0     3004 2023-07-28 09:45:46.000000 guidata-3.0.4/guidata/__init__.py
+-rw-rw-rw-   0        0        0    11296 2023-07-06 14:12:49.000000 guidata-3.0.4/guidata/config.py
+-rw-rw-rw-   0        0        0    13964 2023-07-19 16:04:51.000000 guidata-3.0.4/guidata/configtools.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:05.845011 guidata-3.0.4/guidata/dataset/
+-rw-rw-rw-   0        0        0      535 2023-07-06 12:39:33.000000 guidata-3.0.4/guidata/dataset/__init__.py
+-rw-rw-rw-   0        0        0    33518 2023-07-19 16:11:47.000000 guidata-3.0.4/guidata/dataset/dataitems.py
+-rw-rw-rw-   0        0        0    45137 2023-07-19 16:09:55.000000 guidata-3.0.4/guidata/dataset/datatypes.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:05.856013 guidata-3.0.4/guidata/dataset/io/
+-rw-rw-rw-   0        0        0     1702 2023-07-19 16:10:46.000000 guidata-3.0.4/guidata/dataset/io/__init__.py
+-rw-rw-rw-   0        0        0     5978 2023-07-19 09:51:48.000000 guidata-3.0.4/guidata/dataset/io/base.py
+-rw-rw-rw-   0        0        0    23319 2023-07-19 16:04:45.000000 guidata-3.0.4/guidata/dataset/io/h5fmt.py
+-rw-rw-rw-   0        0        0     5576 2023-07-19 10:06:28.000000 guidata-3.0.4/guidata/dataset/io/inifmt.py
+-rw-rw-rw-   0        0        0     8428 2023-07-19 09:51:48.000000 guidata-3.0.4/guidata/dataset/io/jsonfmt.py
+-rw-rw-rw-   0        0        0    40609 2023-07-18 14:45:16.000000 guidata-3.0.4/guidata/dataset/qtitemwidgets.py
+-rw-rw-rw-   0        0        0    23426 2023-07-06 12:39:33.000000 guidata-3.0.4/guidata/dataset/qtwidgets.py
+-rw-rw-rw-   0        0        0      820 2023-07-06 12:39:33.000000 guidata-3.0.4/guidata/dataset/textedit.py
+-rw-rw-rw-   0        0        0     6093 2023-07-06 12:40:25.000000 guidata-3.0.4/guidata/env.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:05.857008 guidata-3.0.4/guidata/external/
+-rw-rw-rw-   0        0        0        1 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/external/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:05.870007 guidata-3.0.4/guidata/external/darkdetect/
+-rw-rw-rw-   0        0        0     1289 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/external/darkdetect/__init__.py
+-rw-rw-rw-   0        0        0      377 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/external/darkdetect/_dummy.py
+-rw-rw-rw-   0        0        0      890 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/external/darkdetect/_linux_detect.py
+-rw-rw-rw-   0        0        0     2212 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/external/darkdetect/_mac_detect.py
+-rw-rw-rw-   0        0        0     1257 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/external/darkdetect/_windows_detect.py
+-rw-rw-rw-   0        0        0   395446 2023-07-28 10:11:47.000000 guidata-3.0.4/guidata/guidata.chm
+-rw-rw-rw-   0        0        0    11214 2023-07-19 16:04:52.000000 guidata-3.0.4/guidata/guitest.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:05.949006 guidata-3.0.4/guidata/images/
+-rw-rw-rw-   0        0        0      785 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/apply.png
+-rw-rw-rw-   0        0        0     1123 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/arredit.png
+-rw-rw-rw-   0        0        0      721 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/busy.png
+-rw-rw-rw-   0        0        0      689 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/cell_edit.png
+-rw-rw-rw-   0        0        0      830 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/copy.png
+-rw-rw-rw-   0        0        0      722 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/delete.png
+-rw-rw-rw-   0        0        0      911 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/dictedit.png
+-rw-rw-rw-   0        0        0      735 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/dtype.png
+-rw-rw-rw-   0        0        0      929 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/edit.png
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:05.999009 guidata-3.0.4/guidata/images/editors/
+-rw-rw-rw-   0        0        0      911 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/editors/copywop.png
+-rw-rw-rw-   0        0        0      929 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/editors/edit.png
+-rw-rw-rw-   0        0        0     1001 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/editors/edit_add.png
+-rw-rw-rw-   0        0        0     1777 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/editors/editclear.png
+-rw-rw-rw-   0        0        0     1048 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/editors/editcopy.png
+-rw-rw-rw-   0        0        0      824 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/editors/editcut.png
+-rw-rw-rw-   0        0        0     1453 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/editors/editdelete.png
+-rw-rw-rw-   0        0        0     1295 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/editors/editpaste.png
+-rw-rw-rw-   0        0        0     2248 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/editors/fileimport.png
+-rw-rw-rw-   0        0        0     1144 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/editors/filesave.png
+-rw-rw-rw-   0        0        0      727 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/editors/imshow.png
+-rw-rw-rw-   0        0        0      525 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/editors/insert.png
+-rw-rw-rw-   0        0        0      515 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/editors/plot.png
+-rw-rw-rw-   0        0        0      689 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/editors/rename.png
+-rw-rw-rw-   0        0        0     1184 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/editors/selectall.png
+-rw-rw-rw-   0        0        0     1164 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/exit.png
+-rw-rw-rw-   0        0        0      165 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/expander_down.png
+-rw-rw-rw-   0        0        0      432 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/expander_right.png
+-rw-rw-rw-   0        0        0      530 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/file.png
+-rw-rw-rw-   0        0        0     1424 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/fileclose.png
+-rw-rw-rw-   0        0        0     1556 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/fileimport.png
+-rw-rw-rw-   0        0        0      463 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/filenew.png
+-rw-rw-rw-   0        0        0     1539 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/fileopen.png
+-rw-rw-rw-   0        0        0     1144 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/filesave.png
+-rw-rw-rw-   0        0        0     1443 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/filesaveas.png
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:06.064006 guidata-3.0.4/guidata/images/filetypes/
+-rw-rw-rw-   0        0        0     1601 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/filetypes/doc.png
+-rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/filetypes/gif.png
+-rw-rw-rw-   0        0        0     1848 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/filetypes/html.png
+-rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/filetypes/jpg.png
+-rw-rw-rw-   0        0        0     1543 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/filetypes/pdf.png
+-rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/filetypes/png.png
+-rw-rw-rw-   0        0        0     1439 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/filetypes/pps.png
+-rw-rw-rw-   0        0        0     1428 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/filetypes/ps.png
+-rw-rw-rw-   0        0        0     1577 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/filetypes/tar.png
+-rw-rw-rw-   0        0        0     1577 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/filetypes/tgz.png
+-rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/filetypes/tif.png
+-rw-rw-rw-   0        0        0     1801 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/filetypes/txt.png
+-rw-rw-rw-   0        0        0     1237 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/filetypes/xls.png
+-rw-rw-rw-   0        0        0     1577 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/filetypes/zip.png
+-rw-rw-rw-   0        0        0    16434 2023-07-06 15:03:14.000000 guidata-3.0.4/guidata/images/guidata-banner.svg
+-rw-rw-rw-   0        0        0    16406 2023-06-30 10:39:39.000000 guidata-3.0.4/guidata/images/guidata-vertical.svg
+-rw-rw-rw-   0        0        0    15818 2023-06-30 10:21:40.000000 guidata-3.0.4/guidata/images/guidata.svg
+-rw-rw-rw-   0        0        0      356 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/max.png
+-rw-rw-rw-   0        0        0      351 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/min.png
+-rw-rw-rw-   0        0        0      331 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/none.png
+-rw-rw-rw-   0        0        0      531 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/not_found.png
+-rw-rw-rw-   0        0        0      887 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/python.png
+-rw-rw-rw-   0        0        0      888 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/quickview.png
+-rw-rw-rw-   0        0        0     1599 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/save_all.png
+-rw-rw-rw-   0        0        0      744 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/selection.png
+-rw-rw-rw-   0        0        0     2445 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/settings.png
+-rw-rw-rw-   0        0        0      361 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/shape.png
+-rw-rw-rw-   0        0        0      354 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/xmax.png
+-rw-rw-rw-   0        0        0      353 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/images/xmin.png
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:05.691007 guidata-3.0.4/guidata/locale/
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:05.693008 guidata-3.0.4/guidata/locale/fr/
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:06.067007 guidata-3.0.4/guidata/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0    10186 2023-06-29 17:09:10.000000 guidata-3.0.4/guidata/locale/fr/LC_MESSAGES/guidata.mo
+-rw-rw-rw-   0        0        0    20476 2023-07-19 16:01:55.000000 guidata-3.0.4/guidata/qthelpers.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:06.262858 guidata-3.0.4/guidata/tests/
+-rw-rw-rw-   0        0        0      368 2023-07-06 12:39:33.000000 guidata-3.0.4/guidata/tests/__init__.py
+-rw-rw-rw-   0        0        0     1709 2023-06-30 14:48:32.000000 guidata-3.0.4/guidata/tests/_all_tests.py
+-rw-rw-rw-   0        0        0      469 2023-07-18 14:57:07.000000 guidata-3.0.4/guidata/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:05.697008 guidata-3.0.4/guidata/tests/data/
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:06.271516 guidata-3.0.4/guidata/tests/data/genreqs/
+-rw-rw-rw-   0        0        0     2002 2023-07-21 12:09:05.000000 guidata-3.0.4/guidata/tests/data/genreqs/pyproject.toml
+-rw-rw-rw-   0        0        0     1493 2023-07-21 12:25:47.000000 guidata-3.0.4/guidata/tests/data/genreqs/setup.cfg
+-rw-rw-rw-   0        0        0     1724 2023-07-06 14:13:35.000000 guidata-3.0.4/guidata/tests/test_activable_dataset.py
+-rw-rw-rw-   0        0        0     1153 2023-07-06 14:13:43.000000 guidata-3.0.4/guidata/tests/test_activable_items.py
+-rw-rw-rw-   0        0        0     4858 2023-07-06 14:13:50.000000 guidata-3.0.4/guidata/tests/test_all_features.py
+-rw-rw-rw-   0        0        0     3577 2023-07-06 14:13:57.000000 guidata-3.0.4/guidata/tests/test_all_items.py
+-rw-rw-rw-   0        0        0     2601 2023-07-06 14:14:03.000000 guidata-3.0.4/guidata/tests/test_arrayeditor.py
+-rw-rw-rw-   0        0        0     1932 2023-07-06 14:14:10.000000 guidata-3.0.4/guidata/tests/test_bool_selector.py
+-rw-rw-rw-   0        0        0     2049 2023-07-06 14:14:16.000000 guidata-3.0.4/guidata/tests/test_callbacks.py
+-rw-rw-rw-   0        0        0      652 2023-07-06 14:14:23.000000 guidata-3.0.4/guidata/tests/test_codeeditor.py
+-rw-rw-rw-   0        0        0     3955 2023-07-18 15:13:56.000000 guidata-3.0.4/guidata/tests/test_collectionseditor.py
+-rw-rw-rw-   0        0        0     1068 2023-07-06 12:39:33.000000 guidata-3.0.4/guidata/tests/test_config.py
+-rw-rw-rw-   0        0        0      598 2023-07-06 14:14:35.000000 guidata-3.0.4/guidata/tests/test_console.py
+-rw-rw-rw-   0        0        0     1413 2023-07-06 14:14:42.000000 guidata-3.0.4/guidata/tests/test_data.py
+-rw-rw-rw-   0        0        0     2104 2023-07-18 14:56:56.000000 guidata-3.0.4/guidata/tests/test_dataframeeditor.py
+-rw-rw-rw-   0        0        0      869 2023-07-06 12:39:33.000000 guidata-3.0.4/guidata/tests/test_datasetgroup.py
+-rw-rw-rw-   0        0        0      962 2023-07-06 12:41:46.000000 guidata-3.0.4/guidata/tests/test_disthelpers.py
+-rw-rw-rw-   0        0        0     6052 2023-07-18 14:11:17.000000 guidata-3.0.4/guidata/tests/test_editgroupbox.py
+-rw-rw-rw-   0        0        0      839 2023-07-21 12:12:15.000000 guidata-3.0.4/guidata/tests/test_genreqs.py
+-rw-rw-rw-   0        0        0      779 2023-07-06 14:15:14.000000 guidata-3.0.4/guidata/tests/test_importwizard.py
+-rw-rw-rw-   0        0        0     1511 2023-07-06 14:15:21.000000 guidata-3.0.4/guidata/tests/test_inheritance.py
+-rw-rw-rw-   0        0        0     1321 2023-07-06 14:15:27.000000 guidata-3.0.4/guidata/tests/test_item_order.py
+-rw-rw-rw-   0        0        0     1142 2023-07-26 11:35:40.000000 guidata-3.0.4/guidata/tests/test_loadsave_hdf5.py
+-rw-rw-rw-   0        0        0     1078 2023-07-26 11:35:40.000000 guidata-3.0.4/guidata/tests/test_loadsave_json.py
+-rw-rw-rw-   0        0        0      714 2023-07-07 12:57:07.000000 guidata-3.0.4/guidata/tests/test_no_qt.py
+-rw-rw-rw-   0        0        0     1578 2023-07-18 15:02:08.000000 guidata-3.0.4/guidata/tests/test_objecteditor.py
+-rw-rw-rw-   0        0        0     1361 2023-07-06 14:15:41.000000 guidata-3.0.4/guidata/tests/test_rotatedlabel.py
+-rw-rw-rw-   0        0        0      818 2023-07-06 14:15:48.000000 guidata-3.0.4/guidata/tests/test_text.py
+-rw-rw-rw-   0        0        0      493 2023-07-06 12:40:58.000000 guidata-3.0.4/guidata/tests/test_translations.py
+-rw-rw-rw-   0        0        0      778 2023-06-29 14:26:00.000000 guidata-3.0.4/guidata/tests/test_userconfig_app.py
+-rw-rw-rw-   0        0        0    15176 2023-07-07 14:24:22.000000 guidata-3.0.4/guidata/userconfig.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:06.293867 guidata-3.0.4/guidata/utils/
+-rw-rw-rw-   0        0        0     2858 2023-07-19 16:04:50.000000 guidata-3.0.4/guidata/utils/__init__.py
+-rw-rw-rw-   0        0        0    43150 2023-07-06 12:41:24.000000 guidata-3.0.4/guidata/utils/disthelpers.py
+-rw-rw-rw-   0        0        0     6408 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/utils/encoding.py
+-rw-rw-rw-   0        0        0     6977 2023-07-21 12:45:00.000000 guidata-3.0.4/guidata/utils/genreqs.py
+-rw-rw-rw-   0        0        0     4025 2023-07-06 12:39:27.000000 guidata-3.0.4/guidata/utils/gettext_helpers.py
+-rw-rw-rw-   0        0        0    10494 2023-07-19 16:04:50.000000 guidata-3.0.4/guidata/utils/misc.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:06.323305 guidata-3.0.4/guidata/widgets/
+-rw-rw-rw-   0        0        0      729 2023-07-06 12:41:42.000000 guidata-3.0.4/guidata/widgets/__init__.py
+-rw-rw-rw-   0        0        0    33274 2023-06-30 13:14:39.000000 guidata-3.0.4/guidata/widgets/arrayeditor.py
+-rw-rw-rw-   0        0        0    13477 2023-06-30 14:48:54.000000 guidata-3.0.4/guidata/widgets/codeeditor.py
+-rw-rw-rw-   0        0        0    55677 2023-07-18 15:07:59.000000 guidata-3.0.4/guidata/widgets/collectionseditor.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:06.344937 guidata-3.0.4/guidata/widgets/console/
+-rw-rw-rw-   0        0        0     3257 2023-06-30 12:22:39.000000 guidata-3.0.4/guidata/widgets/console/__init__.py
+-rw-rw-rw-   0        0        0    59019 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/widgets/console/base.py
+-rw-rw-rw-   0        0        0    12513 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/widgets/console/calltip.py
+-rw-rw-rw-   0        0        0    11610 2023-06-30 15:04:24.000000 guidata-3.0.4/guidata/widgets/console/dochelpers.py
+-rw-rw-rw-   0        0        0    15411 2023-06-30 14:59:03.000000 guidata-3.0.4/guidata/widgets/console/internalshell.py
+-rw-rw-rw-   0        0        0    12585 2023-06-30 12:28:06.000000 guidata-3.0.4/guidata/widgets/console/interpreter.py
+-rw-rw-rw-   0        0        0    30662 2023-06-30 12:40:32.000000 guidata-3.0.4/guidata/widgets/console/mixins.py
+-rw-rw-rw-   0        0        0    33285 2023-07-06 14:15:58.000000 guidata-3.0.4/guidata/widgets/console/shell.py
+-rw-rw-rw-   0        0        0     4099 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/widgets/console/terminal.py
+-rw-rw-rw-   0        0        0    32563 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/widgets/dataframeeditor.py
+-rw-rw-rw-   0        0        0     3614 2023-07-19 16:00:45.000000 guidata-3.0.4/guidata/widgets/dockable.py
+-rw-rw-rw-   0        0        0    24121 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/widgets/importwizard.py
+-rw-rw-rw-   0        0        0    23460 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/widgets/nsview.py
+-rw-rw-rw-   0        0        0     3533 2023-07-19 16:04:51.000000 guidata-3.0.4/guidata/widgets/objecteditor.py
+-rw-rw-rw-   0        0        0     2122 2023-07-06 12:41:23.000000 guidata-3.0.4/guidata/widgets/rotatedlabel.py
+-rw-rw-rw-   0        0        0    62527 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/widgets/syntaxhighlighters.py
+-rw-rw-rw-   0        0        0     4022 2023-04-28 09:36:06.000000 guidata-3.0.4/guidata/widgets/texteditor.py
+-rw-rw-rw-   0        0        0      280 2023-07-28 09:44:33.000000 guidata-3.0.4/guidata-tests.desktop
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:05.831006 guidata-3.0.4/guidata.egg-info/
+-rw-rw-rw-   0        0        0     6016 2023-07-28 10:12:05.000000 guidata-3.0.4/guidata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5882 2023-07-28 10:12:05.000000 guidata-3.0.4/guidata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 10:12:05.000000 guidata-3.0.4/guidata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-28 10:12:05.000000 guidata-3.0.4/guidata.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      224 2023-07-28 10:12:05.000000 guidata-3.0.4/guidata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-28 10:12:05.000000 guidata-3.0.4/guidata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2015 2023-07-28 09:37:10.000000 guidata-3.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-28 10:12:06.386280 guidata-3.0.4/setup.cfg
```

### Comparing `guidata-3.0.3/LICENSE` & `guidata-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/PKG-INFO` & `guidata-3.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guidata
-Version: 3.0.3
+Version: 3.0.4
 Summary: Automatic GUI generation for easy dataset editing and display
 Author-email: Codra <p.raybaut@codra.fr>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, CEA-Codra, Pierre Raybaut.
         All rights reserved.
```

### Comparing `guidata-3.0.3/README.md` & `guidata-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/doc/_static/favicon.ico` & `guidata-3.0.4/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/doc/basic_example.py` & `guidata-3.0.4/doc/basic_example.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/doc/conf.py` & `guidata-3.0.4/doc/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 
 import os
 import sys
 
 sys.path.insert(0, os.path.abspath(".."))
 
 import guidata  # noqa: E402
-from guidata.utils.genreqs import gen_module_req_rst  # noqa: E402
-
-gen_module_req_rst(guidata, ["Python>=3.7", "PyQt5>=5.11"])
 
 creator = "Pierre Raybaut"
 project = "guidata"
 copyright = "2009 CEA, " + creator
 version = ".".join(guidata.__version__.split(".")[:2])
 release = guidata.__version__
```

### Comparing `guidata-3.0.3/doc/dev/contribute.rst` & `guidata-3.0.4/doc/dev/contribute.rst`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/doc/dev/howto.rst` & `guidata-3.0.4/doc/dev/howto.rst`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/doc/dev/v2_to_v3.csv` & `guidata-3.0.4/doc/dev/v2_to_v3.csv`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/doc/dev/v2_to_v3.rst` & `guidata-3.0.4/doc/dev/v2_to_v3.rst`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/doc/examples.rst` & `guidata-3.0.4/doc/examples.rst`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/doc/images/basic_example.png` & `guidata-3.0.4/doc/images/basic_example.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/doc/images/guidata-banner.png` & `guidata-3.0.4/doc/images/guidata-banner.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/doc/images/guidata-vertical.png` & `guidata-3.0.4/doc/images/guidata-vertical.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/doc/images/layout_example.png` & `guidata-3.0.4/doc/images/layout_example.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/doc/images/screenshots/__init__.png` & `guidata-3.0.4/doc/images/screenshots/__init__.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/doc/images/screenshots/activable_dataset.png` & `guidata-3.0.4/doc/images/screenshots/activable_dataset.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/doc/images/screenshots/all_features.png` & `guidata-3.0.4/doc/images/screenshots/all_features.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/doc/images/screenshots/all_items.png` & `guidata-3.0.4/doc/images/screenshots/all_items.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/doc/images/screenshots/bool_selector.png` & `guidata-3.0.4/doc/images/screenshots/bool_selector.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/doc/images/screenshots/datasetgroup.png` & `guidata-3.0.4/doc/images/screenshots/datasetgroup.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/doc/images/screenshots/editgroupbox.png` & `guidata-3.0.4/doc/images/screenshots/editgroupbox.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/doc/index.rst` & `guidata-3.0.4/doc/index.rst`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/doc/overview.rst` & `guidata-3.0.4/doc/overview.rst`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/doc/requirements.rst` & `guidata-3.0.4/doc/requirements.rst`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/__init__.py` & `guidata-3.0.4/guidata/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 =======
 
 Based on the Qt library :mod:`guidata` is a Python library generating graphical
 user interfaces for easy dataset editing and display. It also provides helpers
 and application development tools for Qt.
 """
 
-__version__ = "3.0.3"
+__version__ = "3.0.4"
 
 
 # Dear (Debian, RPM, ...) package makers, please feel free to customize the
 # following path to module's data (images) and translations:
 DATAPATH = LOCALEPATH = ""
```

### Comparing `guidata-3.0.3/guidata/config.py` & `guidata-3.0.4/guidata/config.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/configtools.py` & `guidata-3.0.4/guidata/configtools.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/dataset/__init__.py` & `guidata-3.0.4/guidata/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/dataset/dataitems.py` & `guidata-3.0.4/guidata/dataset/dataitems.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/dataset/datatypes.py` & `guidata-3.0.4/guidata/dataset/datatypes.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/dataset/io/__init__.py` & `guidata-3.0.4/guidata/dataset/io/__init__.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/dataset/io/base.py` & `guidata-3.0.4/guidata/dataset/io/base.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/dataset/io/h5fmt.py` & `guidata-3.0.4/guidata/dataset/io/h5fmt.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/dataset/io/inifmt.py` & `guidata-3.0.4/guidata/dataset/io/inifmt.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/dataset/io/jsonfmt.py` & `guidata-3.0.4/guidata/dataset/io/jsonfmt.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/dataset/qtitemwidgets.py` & `guidata-3.0.4/guidata/dataset/qtitemwidgets.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/dataset/qtwidgets.py` & `guidata-3.0.4/guidata/dataset/qtwidgets.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/dataset/textedit.py` & `guidata-3.0.4/guidata/dataset/textedit.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/env.py` & `guidata-3.0.4/guidata/env.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/external/darkdetect/__init__.py` & `guidata-3.0.4/guidata/external/darkdetect/__init__.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/external/darkdetect/_linux_detect.py` & `guidata-3.0.4/guidata/external/darkdetect/_linux_detect.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/external/darkdetect/_mac_detect.py` & `guidata-3.0.4/guidata/external/darkdetect/_mac_detect.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/external/darkdetect/_windows_detect.py` & `guidata-3.0.4/guidata/external/darkdetect/_windows_detect.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/guitest.py` & `guidata-3.0.4/guidata/guitest.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/apply.png` & `guidata-3.0.4/guidata/images/apply.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/arredit.png` & `guidata-3.0.4/guidata/images/arredit.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/busy.png` & `guidata-3.0.4/guidata/images/busy.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/cell_edit.png` & `guidata-3.0.4/guidata/images/cell_edit.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/copy.png` & `guidata-3.0.4/guidata/images/copy.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/delete.png` & `guidata-3.0.4/guidata/images/delete.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/dictedit.png` & `guidata-3.0.4/guidata/images/dictedit.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/dtype.png` & `guidata-3.0.4/guidata/images/dtype.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/edit.png` & `guidata-3.0.4/guidata/images/edit.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/editors/copywop.png` & `guidata-3.0.4/guidata/images/editors/copywop.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/editors/edit.png` & `guidata-3.0.4/guidata/images/editors/edit.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/editors/edit_add.png` & `guidata-3.0.4/guidata/images/editors/edit_add.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/editors/editclear.png` & `guidata-3.0.4/guidata/images/editors/editclear.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/editors/editcopy.png` & `guidata-3.0.4/guidata/images/editors/editcopy.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/editors/editcut.png` & `guidata-3.0.4/guidata/images/editors/editcut.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/editors/editdelete.png` & `guidata-3.0.4/guidata/images/editors/editdelete.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/editors/editpaste.png` & `guidata-3.0.4/guidata/images/editors/editpaste.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/editors/fileimport.png` & `guidata-3.0.4/guidata/images/editors/fileimport.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/editors/filesave.png` & `guidata-3.0.4/guidata/images/editors/filesave.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/editors/imshow.png` & `guidata-3.0.4/guidata/images/editors/imshow.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/editors/insert.png` & `guidata-3.0.4/guidata/images/editors/insert.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/editors/plot.png` & `guidata-3.0.4/guidata/images/editors/plot.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/editors/rename.png` & `guidata-3.0.4/guidata/images/editors/rename.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/editors/selectall.png` & `guidata-3.0.4/guidata/images/editors/selectall.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/exit.png` & `guidata-3.0.4/guidata/images/exit.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/file.png` & `guidata-3.0.4/guidata/images/file.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/fileclose.png` & `guidata-3.0.4/guidata/images/fileclose.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/fileimport.png` & `guidata-3.0.4/guidata/images/fileimport.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/fileopen.png` & `guidata-3.0.4/guidata/images/fileopen.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/filesave.png` & `guidata-3.0.4/guidata/images/filesave.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/filesaveas.png` & `guidata-3.0.4/guidata/images/filesaveas.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/filetypes/doc.png` & `guidata-3.0.4/guidata/images/filetypes/doc.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/filetypes/gif.png` & `guidata-3.0.4/guidata/images/filetypes/gif.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/filetypes/html.png` & `guidata-3.0.4/guidata/images/filetypes/html.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/filetypes/jpg.png` & `guidata-3.0.4/guidata/images/filetypes/jpg.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/filetypes/pdf.png` & `guidata-3.0.4/guidata/images/filetypes/pdf.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/filetypes/png.png` & `guidata-3.0.4/guidata/images/filetypes/png.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/filetypes/pps.png` & `guidata-3.0.4/guidata/images/filetypes/pps.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/filetypes/ps.png` & `guidata-3.0.4/guidata/images/filetypes/ps.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/filetypes/tar.png` & `guidata-3.0.4/guidata/images/filetypes/tar.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/filetypes/tgz.png` & `guidata-3.0.4/guidata/images/filetypes/tgz.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/filetypes/tif.png` & `guidata-3.0.4/guidata/images/filetypes/tif.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/filetypes/txt.png` & `guidata-3.0.4/guidata/images/filetypes/txt.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/filetypes/xls.png` & `guidata-3.0.4/guidata/images/filetypes/xls.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/filetypes/zip.png` & `guidata-3.0.4/guidata/images/filetypes/zip.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/guidata-banner.svg` & `guidata-3.0.4/guidata/images/guidata-banner.svg`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/guidata-vertical.svg` & `guidata-3.0.4/guidata/images/guidata-vertical.svg`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/guidata.svg` & `guidata-3.0.4/guidata/images/guidata.svg`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/not_found.png` & `guidata-3.0.4/guidata/images/not_found.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/python.png` & `guidata-3.0.4/guidata/images/python.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/quickview.png` & `guidata-3.0.4/guidata/images/quickview.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/save_all.png` & `guidata-3.0.4/guidata/images/save_all.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/selection.png` & `guidata-3.0.4/guidata/images/selection.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/images/settings.png` & `guidata-3.0.4/guidata/images/settings.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/locale/fr/LC_MESSAGES/guidata.mo` & `guidata-3.0.4/guidata/locale/fr/LC_MESSAGES/guidata.mo`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/qthelpers.py` & `guidata-3.0.4/guidata/qthelpers.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/tests/_all_tests.py` & `guidata-3.0.4/guidata/tests/_all_tests.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/tests/data/genreqs/pyproject.toml` & `guidata-3.0.4/guidata/tests/data/genreqs/pyproject.toml`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/tests/data/genreqs/setup.cfg` & `guidata-3.0.4/guidata/tests/data/genreqs/setup.cfg`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/tests/test_activable_dataset.py` & `guidata-3.0.4/guidata/tests/test_activable_dataset.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/tests/test_activable_items.py` & `guidata-3.0.4/guidata/tests/test_activable_items.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/tests/test_all_features.py` & `guidata-3.0.4/guidata/tests/test_all_features.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/tests/test_all_items.py` & `guidata-3.0.4/guidata/tests/test_all_items.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/tests/test_arrayeditor.py` & `guidata-3.0.4/guidata/tests/test_arrayeditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/tests/test_bool_selector.py` & `guidata-3.0.4/guidata/tests/test_bool_selector.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/tests/test_callbacks.py` & `guidata-3.0.4/guidata/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/tests/test_codeeditor.py` & `guidata-3.0.4/guidata/tests/test_codeeditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/tests/test_collectionseditor.py` & `guidata-3.0.4/guidata/tests/test_collectionseditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/tests/test_config.py` & `guidata-3.0.4/guidata/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/tests/test_console.py` & `guidata-3.0.4/guidata/tests/test_console.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/tests/test_data.py` & `guidata-3.0.4/guidata/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/tests/test_dataframeeditor.py` & `guidata-3.0.4/guidata/tests/test_dataframeeditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/tests/test_datasetgroup.py` & `guidata-3.0.4/guidata/tests/test_datasetgroup.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/tests/test_disthelpers.py` & `guidata-3.0.4/guidata/tests/test_disthelpers.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/tests/test_editgroupbox.py` & `guidata-3.0.4/guidata/tests/test_editgroupbox.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/tests/test_genreqs.py` & `guidata-3.0.4/guidata/tests/test_genreqs.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/tests/test_importwizard.py` & `guidata-3.0.4/guidata/tests/test_importwizard.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/tests/test_inheritance.py` & `guidata-3.0.4/guidata/tests/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/tests/test_item_order.py` & `guidata-3.0.4/guidata/tests/test_item_order.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/tests/test_loadsave_hdf5.py` & `guidata-3.0.4/guidata/tests/test_loadsave_hdf5.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/tests/test_loadsave_json.py` & `guidata-3.0.4/guidata/tests/test_loadsave_json.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/tests/test_no_qt.py` & `guidata-3.0.4/guidata/tests/test_no_qt.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/tests/test_objecteditor.py` & `guidata-3.0.4/guidata/tests/test_objecteditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/tests/test_rotatedlabel.py` & `guidata-3.0.4/guidata/tests/test_rotatedlabel.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/tests/test_text.py` & `guidata-3.0.4/guidata/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/tests/test_userconfig_app.py` & `guidata-3.0.4/guidata/tests/test_userconfig_app.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/userconfig.py` & `guidata-3.0.4/guidata/userconfig.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/utils/__init__.py` & `guidata-3.0.4/guidata/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/utils/disthelpers.py` & `guidata-3.0.4/guidata/utils/disthelpers.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/utils/encoding.py` & `guidata-3.0.4/guidata/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/utils/genreqs.py` & `guidata-3.0.4/guidata/utils/genreqs.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/utils/gettext_helpers.py` & `guidata-3.0.4/guidata/utils/gettext_helpers.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/utils/misc.py` & `guidata-3.0.4/guidata/utils/misc.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/widgets/__init__.py` & `guidata-3.0.4/guidata/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/widgets/arrayeditor.py` & `guidata-3.0.4/guidata/widgets/arrayeditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/widgets/codeeditor.py` & `guidata-3.0.4/guidata/widgets/codeeditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/widgets/collectionseditor.py` & `guidata-3.0.4/guidata/widgets/collectionseditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/widgets/console/__init__.py` & `guidata-3.0.4/guidata/widgets/console/__init__.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/widgets/console/base.py` & `guidata-3.0.4/guidata/widgets/console/base.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/widgets/console/calltip.py` & `guidata-3.0.4/guidata/widgets/console/calltip.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/widgets/console/dochelpers.py` & `guidata-3.0.4/guidata/widgets/console/dochelpers.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/widgets/console/internalshell.py` & `guidata-3.0.4/guidata/widgets/console/internalshell.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/widgets/console/interpreter.py` & `guidata-3.0.4/guidata/widgets/console/interpreter.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/widgets/console/mixins.py` & `guidata-3.0.4/guidata/widgets/console/mixins.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/widgets/console/shell.py` & `guidata-3.0.4/guidata/widgets/console/shell.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/widgets/console/terminal.py` & `guidata-3.0.4/guidata/widgets/console/terminal.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/widgets/dataframeeditor.py` & `guidata-3.0.4/guidata/widgets/dataframeeditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/widgets/dockable.py` & `guidata-3.0.4/guidata/widgets/dockable.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/widgets/importwizard.py` & `guidata-3.0.4/guidata/widgets/importwizard.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/widgets/nsview.py` & `guidata-3.0.4/guidata/widgets/nsview.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/widgets/objecteditor.py` & `guidata-3.0.4/guidata/widgets/objecteditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/widgets/rotatedlabel.py` & `guidata-3.0.4/guidata/widgets/rotatedlabel.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/widgets/syntaxhighlighters.py` & `guidata-3.0.4/guidata/widgets/syntaxhighlighters.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata/widgets/texteditor.py` & `guidata-3.0.4/guidata/widgets/texteditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.3/guidata.egg-info/PKG-INFO` & `guidata-3.0.4/guidata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guidata
-Version: 3.0.3
+Version: 3.0.4
 Summary: Automatic GUI generation for easy dataset editing and display
 Author-email: Codra <p.raybaut@codra.fr>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, CEA-Codra, Pierre Raybaut.
         All rights reserved.
```

### Comparing `guidata-3.0.3/guidata.egg-info/SOURCES.txt` & `guidata-3.0.4/guidata.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 LICENSE
 MANIFEST.in
 README.md
+guidata-tests.desktop
 pyproject.toml
 doc/basic_example.py
 doc/conf.py
 doc/examples.rst
 doc/index.rst
 doc/installation.rst
 doc/overview.rst
 doc/requirements.rst
+doc/update_requirements.py
 doc/_static/favicon.ico
 doc/dev/contribute.rst
 doc/dev/howto.rst
 doc/dev/index.rst
 doc/dev/v2_to_v3.csv
 doc/dev/v2_to_v3.rst
 doc/images/basic_example.png
@@ -43,14 +45,15 @@
 guidata/guidata.chm
 guidata/guitest.py
 guidata/qthelpers.py
 guidata/userconfig.py
 guidata.egg-info/PKG-INFO
 guidata.egg-info/SOURCES.txt
 guidata.egg-info/dependency_links.txt
+guidata.egg-info/entry_points.txt
 guidata.egg-info/requires.txt
 guidata.egg-info/top_level.txt
 guidata/dataset/__init__.py
 guidata/dataset/dataitems.py
 guidata/dataset/datatypes.py
 guidata/dataset/qtitemwidgets.py
 guidata/dataset/qtwidgets.py
```

### Comparing `guidata-3.0.3/pyproject.toml` & `guidata-3.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,16 @@
 dependencies = ["h5py>=3.0", "NumPy>=1.21", "QtPy>=1.9", "requests", "tomli"]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/CODRA-Ingenierie-Informatique/guidata/"
 Documentation = "https://guidata.readthedocs.io/en/latest/"
 
-[project.scripts]
+[project.gui-scripts]
+guidata-tests = "guidata.tests:run"
 
 [project.optional-dependencies]
 dev = ["black", "isort", "pylint", "Coverage"]
 doc = [
     "PyQt5",
     "pillow",
     "pandas",
```

