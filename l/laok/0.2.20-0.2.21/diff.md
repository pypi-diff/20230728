# Comparing `tmp/laok-0.2.20.tar.gz` & `tmp/laok-0.2.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laok-0.2.20.tar", last modified: Fri Jul 14 09:20:51 2023, max compression
+gzip compressed data, was "laok-0.2.21.tar", last modified: Fri Jul 28 11:44:55 2023, max compression
```

## Comparing `laok-0.2.20.tar` & `laok-0.2.21.tar`

### file list

```diff
@@ -1,182 +1,192 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.687990 laok-0.2.20/
--rw-rw-rw-   0        0        0      214 2023-07-14 09:20:51.687990 laok-0.2.20/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.571301 laok-0.2.20/laok/
--rw-rw-rw-   0        0        0       19 2023-07-11 03:35:21.000000 laok-0.2.20/laok/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.575291 laok-0.2.20/laok/base/
--rw-rw-rw-   0        0        0      266 2023-07-14 09:20:48.000000 laok-0.2.20/laok/base/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.577286 laok-0.2.20/laok/base/alg/
--rw-rw-rw-   0        0        0       26 2023-04-20 13:21:17.000000 laok-0.2.20/laok/base/alg/__init__.py
--rw-rw-rw-   0        0        0     4923 2023-04-20 13:20:53.000000 laok-0.2.20/laok/base/alg/addict.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.580277 laok-0.2.20/laok/base/conf/
--rw-rw-rw-   0        0        0       32 2023-06-10 01:32:44.000000 laok-0.2.20/laok/base/conf/__init__.py
--rw-rw-rw-   0        0        0      360 2023-04-19 14:40:47.000000 laok-0.2.20/laok/base/conf/conf_global.py
--rw-rw-rw-   0        0        0     3022 2023-06-10 01:32:49.000000 laok-0.2.20/laok/base/conf/factory.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.583269 laok-0.2.20/laok/base/dataset/
--rw-rw-rw-   0        0        0        0 2023-04-21 04:27:16.000000 laok-0.2.20/laok/base/dataset/__init__.py
--rw-rw-rw-   0        0        0     6406 2023-04-21 04:29:54.000000 laok-0.2.20/laok/base/dataset/cvt_voc_yolo.py
--rw-rw-rw-   0        0        0     2405 2019-09-12 10:55:17.000000 laok-0.2.20/laok/base/dataset/darknet-voc2yolo.py
--rw-rw-rw-   0        0        0     2241 2019-02-18 15:12:05.000000 laok-0.2.20/laok/base/dataset/voc_label.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.586262 laok-0.2.20/laok/base/dtime/
--rw-rw-rw-   0        0        0       47 2022-10-21 10:13:37.000000 laok-0.2.20/laok/base/dtime/__init__.py
--rw-rw-rw-   0        0        0      556 2022-11-17 01:18:56.000000 laok-0.2.20/laok/base/dtime/datetime_.py
--rw-rw-rw-   0        0        0     2727 2023-04-19 11:27:09.000000 laok-0.2.20/laok/base/dtime/timer.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.593243 laok-0.2.20/laok/base/fs/
--rw-rw-rw-   0        0        0      134 2023-05-04 11:06:57.000000 laok-0.2.20/laok/base/fs/__init__.py
--rw-rw-rw-   0        0        0     2591 2023-06-27 16:15:40.000000 laok-0.2.20/laok/base/fs/fdata.py
--rw-rw-rw-   0        0        0     2937 2022-11-03 16:22:33.000000 laok-0.2.20/laok/base/fs/fname.py
--rw-rw-rw-   0        0        0     4629 2023-06-27 16:03:41.000000 laok-0.2.20/laok/base/fs/fpath.py
--rw-rw-rw-   0        0        0     1785 2023-05-04 11:06:06.000000 laok-0.2.20/laok/base/fs/fsearch.py
--rw-rw-rw-   0        0        0     2819 2023-05-05 03:57:37.000000 laok-0.2.20/laok/base/fs/fwalk.py
--rw-rw-rw-   0        0        0     1413 2023-04-19 09:23:34.000000 laok-0.2.20/laok/base/fs/name_index.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.595237 laok-0.2.20/laok/base/log/
--rw-rw-rw-   0        0        0       50 2023-04-19 14:41:08.000000 laok-0.2.20/laok/base/log/__init__.py
--rw-rw-rw-   0        0        0     2187 2023-07-14 02:24:25.000000 laok-0.2.20/laok/base/log/log.py
--rw-rw-rw-   0        0        0      672 2023-04-19 14:43:17.000000 laok-0.2.20/laok/base/log/log_default.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.599227 laok-0.2.20/laok/base/net/
--rw-rw-rw-   0        0        0       78 2023-06-06 16:23:58.000000 laok-0.2.20/laok/base/net/__init__.py
--rw-rw-rw-   0        0        0      691 2022-09-23 00:45:15.000000 laok-0.2.20/laok/base/net/ip.py
--rw-rw-rw-   0        0        0     3792 2023-06-27 10:59:29.000000 laok-0.2.20/laok/base/net/requests_.py
--rw-rw-rw-   0        0        0     1200 2023-06-27 10:55:31.000000 laok-0.2.20/laok/base/net/url.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.600224 laok-0.2.20/laok/base/paral/
--rw-rw-rw-   0        0        0       20 2022-10-21 10:13:37.000000 laok-0.2.20/laok/base/paral/__init__.py
--rw-rw-rw-   0        0        0     2010 2023-04-20 15:21:46.000000 laok-0.2.20/laok/base/paral/pool.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.602219 laok-0.2.20/laok/base/pkg/
--rw-rw-rw-   0        0        0       32 2023-07-03 15:46:47.000000 laok-0.2.20/laok/base/pkg/__init__.py
--rw-rw-rw-   0        0        0    27875 2023-07-03 15:50:30.000000 laok-0.2.20/laok/base/pkg/_lazy.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.610197 laok-0.2.20/laok/base/ser/
--rw-rw-rw-   0        0        0      156 2023-06-06 14:13:13.000000 laok-0.2.20/laok/base/ser/__init__.py
--rw-rw-rw-   0        0        0     1367 2023-04-25 06:50:06.000000 laok-0.2.20/laok/base/ser/json_.py
--rw-rw-rw-   0        0        0      750 2023-04-20 13:46:22.000000 laok-0.2.20/laok/base/ser/marshal_.py
--rw-rw-rw-   0        0        0      676 2023-06-01 07:58:10.000000 laok-0.2.20/laok/base/ser/numpy_.py
--rw-rw-rw-   0        0        0      621 2023-04-25 06:50:29.000000 laok-0.2.20/laok/base/ser/pickle_.py
--rw-rw-rw-   0        0        0     1369 2023-06-10 01:42:11.000000 laok-0.2.20/laok/base/ser/torch_.py
--rw-rw-rw-   0        0        0     1452 2023-06-06 17:03:52.000000 laok-0.2.20/laok/base/ser/xml_.py
--rw-rw-rw-   0        0        0     1341 2023-06-01 07:57:17.000000 laok-0.2.20/laok/base/ser/yaml_.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.614187 laok-0.2.20/laok/base/str/
--rw-rw-rw-   0        0        0       84 2023-06-10 01:11:15.000000 laok-0.2.20/laok/base/str/__init__.py
--rw-rw-rw-   0        0        0      735 2023-06-10 01:09:44.000000 laok-0.2.20/laok/base/str/cvt.py
--rw-rw-rw-   0        0        0      427 2023-06-10 01:10:45.000000 laok-0.2.20/laok/base/str/fmt.py
--rw-rw-rw-   0        0        0     1705 2023-06-10 01:10:56.000000 laok-0.2.20/laok/base/str/misc.py
--rw-rw-rw-   0        0        0     2588 2023-06-01 07:58:57.000000 laok-0.2.20/laok/base/str/print_info.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.618177 laok-0.2.20/laok/base/syst/
--rw-rw-rw-   0        0        0       74 2023-07-03 11:23:20.000000 laok-0.2.20/laok/base/syst/__init__.py
--rw-rw-rw-   0        0        0      518 2023-05-04 15:23:10.000000 laok-0.2.20/laok/base/syst/platform_.py
--rw-rw-rw-   0        0        0     1871 2022-10-21 10:13:37.000000 laok-0.2.20/laok/base/syst/print_info.py
--rw-rw-rw-   0        0        0      380 2023-07-03 11:23:24.000000 laok-0.2.20/laok/base/syst/sys_.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.620171 laok-0.2.20/laok/base/test/
--rw-rw-rw-   0        0        0       43 2022-10-21 10:13:37.000000 laok-0.2.20/laok/base/test/__init__.py
--rw-rw-rw-   0        0        0     8790 2023-07-11 07:18:36.000000 laok-0.2.20/laok/base/test/_dump.py
--rw-rw-rw-   0        0        0     4551 2023-06-01 05:41:11.000000 laok-0.2.20/laok/base/test/_run.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.621168 laok-0.2.20/laok/cv2d/
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.622166 laok-0.2.20/laok/cv2d/PIL_/
--rw-rw-rw-   0        0        0        0 2023-07-12 09:00:52.000000 laok-0.2.20/laok/cv2d/PIL_/__init__.py
--rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.20/laok/cv2d/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.634133 laok-0.2.20/laok/cv2d/cv2_/
--rw-rw-rw-   0        0        0      252 2023-07-12 14:13:06.000000 laok-0.2.20/laok/cv2d/cv2_/__init__.py
--rw-rw-rw-   0        0        0     2115 2023-07-12 12:32:21.000000 laok-0.2.20/laok/cv2d/cv2_/bin.py
--rw-rw-rw-   0        0        0      951 2023-07-12 14:53:01.000000 laok-0.2.20/laok/cv2d/cv2_/contours.py
--rw-rw-rw-   0        0        0     2580 2023-07-11 11:20:43.000000 laok-0.2.20/laok/cv2d/cv2_/cvt.py
--rw-rw-rw-   0        0        0     4358 2023-07-12 06:55:54.000000 laok-0.2.20/laok/cv2d/cv2_/draw.py
--rw-rw-rw-   0        0        0      956 2023-07-12 14:26:53.000000 laok-0.2.20/laok/cv2d/cv2_/edge.py
--rw-rw-rw-   0        0        0     1268 2023-07-12 13:43:27.000000 laok-0.2.20/laok/cv2d/cv2_/filter.py
--rw-rw-rw-   0        0        0      630 2023-07-12 07:16:54.000000 laok-0.2.20/laok/cv2d/cv2_/geo.py
--rw-rw-rw-   0        0        0     1019 2023-07-11 16:28:07.000000 laok-0.2.20/laok/cv2d/cv2_/info.py
--rw-rw-rw-   0        0        0     3240 2023-07-11 14:03:03.000000 laok-0.2.20/laok/cv2d/cv2_/io.py
--rw-rw-rw-   0        0        0     2787 2023-07-12 13:56:20.000000 laok-0.2.20/laok/cv2d/cv2_/morph.py
--rw-rw-rw-   0        0        0     1230 2023-07-11 15:01:26.000000 laok-0.2.20/laok/cv2d/cv2_/show.py
--rw-rw-rw-   0        0        0      828 2023-07-11 15:21:15.000000 laok-0.2.20/laok/cv2d/cv2_/util.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.635131 laok-0.2.20/laok/cv2d/skimage_/
--rw-rw-rw-   0        0        0      330 2023-07-11 05:10:30.000000 laok-0.2.20/laok/cv2d/skimage_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.635131 laok-0.2.20/laok/cv3d/
--rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.20/laok/cv3d/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.636129 laok-0.2.20/laok/cv3d/open3d_/
--rw-rw-rw-   0        0        0      330 2023-07-11 05:10:30.000000 laok-0.2.20/laok/cv3d/open3d_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.637125 laok-0.2.20/laok/data/
--rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.20/laok/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.638123 laok-0.2.20/laok/data/lxml_/
--rw-rw-rw-   0        0        0     1982 2023-07-11 06:14:29.000000 laok-0.2.20/laok/data/lxml_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.639120 laok-0.2.20/laok/data/yaml_/
--rw-rw-rw-   0        0        0      330 2023-07-11 05:10:30.000000 laok-0.2.20/laok/data/yaml_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.639120 laok-0.2.20/laok/dnn/
--rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.20/laok/dnn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.640117 laok-0.2.20/laok/dnn/onnx_/
--rw-rw-rw-   0        0        0     3116 2023-07-11 03:56:12.000000 laok-0.2.20/laok/dnn/onnx_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.641115 laok-0.2.20/laok/dnn/torch_/
--rw-rw-rw-   0        0        0       88 2023-04-19 08:20:33.000000 laok-0.2.20/laok/dnn/torch_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.643109 laok-0.2.20/laok/dnn/torch_/datasets/
--rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.20/laok/dnn/torch_/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.646101 laok-0.2.20/laok/dnn/torch_/datasets/kitti/
--rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.20/laok/dnn/torch_/datasets/kitti/__init__.py
--rw-rw-rw-   0        0        0    12031 2022-11-03 16:22:33.000000 laok-0.2.20/laok/dnn/torch_/datasets/kitti/kitti.py
--rw-rw-rw-   0        0        0    27294 2022-10-28 06:48:12.000000 laok-0.2.20/laok/dnn/torch_/datasets/kitti/obj.py
--rw-rw-rw-   0        0        0    26349 2022-11-03 16:22:33.000000 laok-0.2.20/laok/dnn/torch_/datasets/kitti/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.652086 laok-0.2.20/laok/dnn/torch_/datasets/model_net/
--rw-rw-rw-   0        0        0      954 2022-11-03 16:22:33.000000 laok-0.2.20/laok/dnn/torch_/datasets/model_net/__init__.py
--rw-rw-rw-   0        0        0     3721 2022-11-03 16:22:33.000000 laok-0.2.20/laok/dnn/torch_/datasets/model_net/model_net.py
--rw-rw-rw-   0        0        0     4467 2022-11-03 16:22:33.000000 laok-0.2.20/laok/dnn/torch_/datasets/model_net/model_net_ineratia.py
--rw-rw-rw-   0        0        0     3895 2022-11-03 16:22:33.000000 laok-0.2.20/laok/dnn/torch_/datasets/model_net/model_net_normals.py
--rw-rw-rw-   0        0        0     4553 2022-11-03 16:22:33.000000 laok-0.2.20/laok/dnn/torch_/datasets/model_net/model_net_normals_diff.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.653083 laok-0.2.20/laok/dnn/torch_/datasets/shape_net/
--rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.20/laok/dnn/torch_/datasets/shape_net/__init__.py
--rw-rw-rw-   0        0        0     5463 2022-10-21 10:13:37.000000 laok-0.2.20/laok/dnn/torch_/datasets/shape_net/shape_net.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.655077 laok-0.2.20/laok/dnn/torch_/datasets/stanford_indoor/
--rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.20/laok/dnn/torch_/datasets/stanford_indoor/__init__.py
--rw-rw-rw-   0        0        0    11035 2022-10-12 15:00:14.000000 laok-0.2.20/laok/dnn/torch_/datasets/stanford_indoor/_stanford_indoor.py
--rw-rw-rw-   0        0        0     2811 2022-11-02 07:35:53.000000 laok-0.2.20/laok/dnn/torch_/datasets/ustc_lidar.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.660064 laok-0.2.20/laok/dnn/torch_/io/
--rw-rw-rw-   0        0        0       80 2022-10-21 10:13:37.000000 laok-0.2.20/laok/dnn/torch_/io/__init__.py
--rw-rw-rw-   0        0        0      732 2022-10-21 10:13:37.000000 laok-0.2.20/laok/dnn/torch_/io/img.py
--rw-rw-rw-   0        0        0      844 2022-10-21 10:13:37.000000 laok-0.2.20/laok/dnn/torch_/io/jit.py
--rw-rw-rw-   0        0        0     1344 2022-10-21 10:13:37.000000 laok-0.2.20/laok/dnn/torch_/io/model.py
--rw-rw-rw-   0        0        0      466 2022-10-21 10:13:37.000000 laok-0.2.20/laok/dnn/torch_/io/onnx.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.663056 laok-0.2.20/laok/dnn/torch_/op/
--rw-rw-rw-   0        0        0       70 2023-04-19 08:22:19.000000 laok-0.2.20/laok/dnn/torch_/op/__init__.py
--rw-rw-rw-   0        0        0      965 2023-04-19 08:22:06.000000 laok-0.2.20/laok/dnn/torch_/op/device.py
--rw-rw-rw-   0        0        0     1703 2023-04-19 08:27:44.000000 laok-0.2.20/laok/dnn/torch_/op/module.py
--rw-rw-rw-   0        0        0     1403 2023-04-19 08:25:22.000000 laok-0.2.20/laok/dnn/torch_/op/print_info.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.668043 laok-0.2.20/laok/dnn/torch_/trainval/
--rw-rw-rw-   0        0        0       89 2022-10-21 10:13:37.000000 laok-0.2.20/laok/dnn/torch_/trainval/__init__.py
--rw-rw-rw-   0        0        0     3943 2023-04-19 09:12:20.000000 laok-0.2.20/laok/dnn/torch_/trainval/check_point.py
--rw-rw-rw-   0        0        0     2280 2023-04-19 09:25:29.000000 laok-0.2.20/laok/dnn/torch_/trainval/infer.py
--rw-rw-rw-   0        0        0     2848 2023-04-19 08:44:39.000000 laok-0.2.20/laok/dnn/torch_/trainval/train.py
--rw-rw-rw-   0        0        0     2308 2023-04-19 09:08:59.000000 laok-0.2.20/laok/dnn/torch_/trainval/val.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.669041 laok-0.2.20/laok/gui/
--rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.20/laok/gui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.671035 laok-0.2.20/laok/gui/matplot_/
--rw-rw-rw-   0        0        0       19 2023-07-12 09:01:52.000000 laok-0.2.20/laok/gui/matplot_/__init__.py
--rw-rw-rw-   0        0        0     2096 2023-07-12 16:09:46.000000 laok-0.2.20/laok/gui/matplot_/show.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.674027 laok-0.2.20/laok/gui/qt_/
--rw-rw-rw-   0        0        0       62 2023-07-14 02:30:38.000000 laok-0.2.20/laok/gui/qt_/__init__.py
--rw-rw-rw-   0        0        0      582 2023-07-14 03:03:10.000000 laok-0.2.20/laok/gui/qt_/dialog.py
--rw-rw-rw-   0        0        0     1004 2023-07-14 02:15:56.000000 laok-0.2.20/laok/gui/qt_/run.py
--rw-rw-rw-   0        0        0     1931 2023-07-14 03:22:35.000000 laok-0.2.20/laok/gui/qt_/ui.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.675024 laok-0.2.20/laok/matical/
--rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.20/laok/matical/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.676021 laok-0.2.20/laok/matical/numpy_/
--rw-rw-rw-   0        0        0        0 2023-04-20 14:21:33.000000 laok-0.2.20/laok/matical/numpy_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.677019 laok-0.2.20/laok/ml/
--rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.20/laok/ml/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.677019 laok-0.2.20/laok/ml/sklearn_/
--rw-rw-rw-   0        0        0      330 2023-07-11 05:10:30.000000 laok-0.2.20/laok/ml/sklearn_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.678016 laok-0.2.20/laok/net/
--rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.20/laok/net/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.680011 laok-0.2.20/laok/net/flask_/
--rw-rw-rw-   0        0        0       42 2023-04-19 15:05:48.000000 laok-0.2.20/laok/net/flask_/__init__.py
--rw-rw-rw-   0        0        0      395 2023-04-19 15:05:30.000000 laok-0.2.20/laok/net/flask_/app.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.682006 laok-0.2.20/laok/net/flask_/basic/
--rw-rw-rw-   0        0        0       22 2023-04-19 15:06:08.000000 laok-0.2.20/laok/net/flask_/basic/__init__.py
--rw-rw-rw-   0        0        0      633 2023-04-19 15:38:09.000000 laok-0.2.20/laok/net/flask_/basic/views.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.683003 laok-0.2.20/laok/net/requests_/
--rw-rw-rw-   0        0        0     3808 2023-07-11 04:59:34.000000 laok-0.2.20/laok/net/requests_/__init__.py
--rw-rw-rw-   0        0        0      649 2023-07-11 04:06:36.000000 laok-0.2.20/laok/third_lib.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.686993 laok-0.2.20/laok/tool/
--rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.20/laok/tool/__init__.py
--rw-rw-rw-   0        0        0     3604 2023-07-11 06:29:13.000000 laok-0.2.20/laok/tool/download_m3u8.py
--rw-rw-rw-   0        0        0     2310 2023-07-04 03:20:00.000000 laok-0.2.20/laok/tool/ultralytics_.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.575291 laok-0.2.20/laok.egg-info/
--rw-rw-rw-   0        0        0      214 2023-07-14 09:20:51.000000 laok-0.2.20/laok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3708 2023-07-14 09:20:51.000000 laok-0.2.20/laok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 09:20:51.000000 laok-0.2.20/laok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-14 09:20:51.000000 laok-0.2.20/laok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 09:20:51.687990 laok-0.2.20/setup.cfg
--rw-rw-rw-   0        0        0      322 2023-07-14 09:20:27.000000 laok-0.2.20/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.980780 laok-0.2.21/
+-rw-rw-rw-   0        0        0      214 2023-07-28 11:44:55.979783 laok-0.2.21/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.815223 laok-0.2.21/laok/
+-rw-rw-rw-   0        0        0       19 2023-07-11 03:35:21.000000 laok-0.2.21/laok/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.820210 laok-0.2.21/laok/base/
+-rw-rw-rw-   0        0        0      271 2023-07-14 12:09:19.000000 laok-0.2.21/laok/base/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.822204 laok-0.2.21/laok/base/alg/
+-rw-rw-rw-   0        0        0       26 2023-04-20 13:21:17.000000 laok-0.2.21/laok/base/alg/__init__.py
+-rw-rw-rw-   0        0        0     4922 2023-07-14 11:34:02.000000 laok-0.2.21/laok/base/alg/addict.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.823202 laok-0.2.21/laok/base/colors/
+-rw-rw-rw-   0        0        0     1611 2023-07-14 12:10:26.000000 laok-0.2.21/laok/base/colors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.827191 laok-0.2.21/laok/base/conf/
+-rw-rw-rw-   0        0        0       32 2023-06-10 01:32:44.000000 laok-0.2.21/laok/base/conf/__init__.py
+-rw-rw-rw-   0        0        0      360 2023-04-19 14:40:47.000000 laok-0.2.21/laok/base/conf/conf_global.py
+-rw-rw-rw-   0        0        0     3054 2023-07-14 11:33:47.000000 laok-0.2.21/laok/base/conf/factory.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.831180 laok-0.2.21/laok/base/dataset/
+-rw-rw-rw-   0        0        0        0 2023-04-21 04:27:16.000000 laok-0.2.21/laok/base/dataset/__init__.py
+-rw-rw-rw-   0        0        0     6406 2023-04-21 04:29:54.000000 laok-0.2.21/laok/base/dataset/cvt_voc_yolo.py
+-rw-rw-rw-   0        0        0     2405 2019-09-12 10:55:17.000000 laok-0.2.21/laok/base/dataset/darknet-voc2yolo.py
+-rw-rw-rw-   0        0        0     2241 2019-02-18 15:12:05.000000 laok-0.2.21/laok/base/dataset/voc_label.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.834172 laok-0.2.21/laok/base/dtime/
+-rw-rw-rw-   0        0        0       47 2022-10-21 10:13:37.000000 laok-0.2.21/laok/base/dtime/__init__.py
+-rw-rw-rw-   0        0        0      503 2023-07-14 11:48:34.000000 laok-0.2.21/laok/base/dtime/datetime_.py
+-rw-rw-rw-   0        0        0     2727 2023-04-19 11:27:09.000000 laok-0.2.21/laok/base/dtime/timer.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.844146 laok-0.2.21/laok/base/fs/
+-rw-rw-rw-   0        0        0      134 2023-05-04 11:06:57.000000 laok-0.2.21/laok/base/fs/__init__.py
+-rw-rw-rw-   0        0        0     2713 2023-07-14 11:45:15.000000 laok-0.2.21/laok/base/fs/fdata.py
+-rw-rw-rw-   0        0        0     2937 2022-11-03 16:22:33.000000 laok-0.2.21/laok/base/fs/fname.py
+-rw-rw-rw-   0        0        0     4629 2023-06-27 16:03:41.000000 laok-0.2.21/laok/base/fs/fpath.py
+-rw-rw-rw-   0        0        0     1785 2023-05-04 11:06:06.000000 laok-0.2.21/laok/base/fs/fsearch.py
+-rw-rw-rw-   0        0        0     2819 2023-05-05 03:57:37.000000 laok-0.2.21/laok/base/fs/fwalk.py
+-rw-rw-rw-   0        0        0     1413 2023-04-19 09:23:34.000000 laok-0.2.21/laok/base/fs/name_index.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.846140 laok-0.2.21/laok/base/log/
+-rw-rw-rw-   0        0        0       50 2023-04-19 14:41:08.000000 laok-0.2.21/laok/base/log/__init__.py
+-rw-rw-rw-   0        0        0     2185 2023-07-14 11:57:41.000000 laok-0.2.21/laok/base/log/log.py
+-rw-rw-rw-   0        0        0      672 2023-04-19 14:43:17.000000 laok-0.2.21/laok/base/log/log_default.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.849132 laok-0.2.21/laok/base/net/
+-rw-rw-rw-   0        0        0       41 2023-07-14 11:52:08.000000 laok-0.2.21/laok/base/net/__init__.py
+-rw-rw-rw-   0        0        0      691 2022-09-23 00:45:15.000000 laok-0.2.21/laok/base/net/ip.py
+-rw-rw-rw-   0        0        0     1200 2023-06-27 10:55:31.000000 laok-0.2.21/laok/base/net/url.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.851127 laok-0.2.21/laok/base/paral/
+-rw-rw-rw-   0        0        0       20 2022-10-21 10:13:37.000000 laok-0.2.21/laok/base/paral/__init__.py
+-rw-rw-rw-   0        0        0     2010 2023-04-20 15:21:46.000000 laok-0.2.21/laok/base/paral/pool.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.853122 laok-0.2.21/laok/base/pkg/
+-rw-rw-rw-   0        0        0       32 2023-07-03 15:46:47.000000 laok-0.2.21/laok/base/pkg/__init__.py
+-rw-rw-rw-   0        0        0    27875 2023-07-03 15:50:30.000000 laok-0.2.21/laok/base/pkg/_lazy.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.863095 laok-0.2.21/laok/base/ser/
+-rw-rw-rw-   0        0        0      164 2023-07-14 11:56:30.000000 laok-0.2.21/laok/base/ser/__init__.py
+-rw-rw-rw-   0        0        0     1367 2023-04-25 06:50:06.000000 laok-0.2.21/laok/base/ser/json_.py
+-rw-rw-rw-   0        0        0      750 2023-04-20 13:46:22.000000 laok-0.2.21/laok/base/ser/marshal_.py
+-rw-rw-rw-   0        0        0      676 2023-06-01 07:58:10.000000 laok-0.2.21/laok/base/ser/numpy_.py
+-rw-rw-rw-   0        0        0      621 2023-04-25 06:50:29.000000 laok-0.2.21/laok/base/ser/pickle_.py
+-rw-rw-rw-   0        0        0     1369 2023-06-10 01:42:11.000000 laok-0.2.21/laok/base/ser/torch_.py
+-rw-rw-rw-   0        0        0     1452 2023-06-06 17:03:52.000000 laok-0.2.21/laok/base/ser/xml_.py
+-rw-rw-rw-   0        0        0     1341 2023-06-01 07:57:17.000000 laok-0.2.21/laok/base/ser/yaml_.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.868082 laok-0.2.21/laok/base/str/
+-rw-rw-rw-   0        0        0       84 2023-06-10 01:11:15.000000 laok-0.2.21/laok/base/str/__init__.py
+-rw-rw-rw-   0        0        0      735 2023-06-10 01:09:44.000000 laok-0.2.21/laok/base/str/cvt.py
+-rw-rw-rw-   0        0        0      427 2023-06-10 01:10:45.000000 laok-0.2.21/laok/base/str/fmt.py
+-rw-rw-rw-   0        0        0     1705 2023-06-10 01:10:56.000000 laok-0.2.21/laok/base/str/misc.py
+-rw-rw-rw-   0        0        0     2588 2023-06-01 07:58:57.000000 laok-0.2.21/laok/base/str/print_info.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.872071 laok-0.2.21/laok/base/sys_/
+-rw-rw-rw-   0        0        0       74 2023-07-03 11:23:20.000000 laok-0.2.21/laok/base/sys_/__init__.py
+-rw-rw-rw-   0        0        0      518 2023-05-04 15:23:10.000000 laok-0.2.21/laok/base/sys_/platform_.py
+-rw-rw-rw-   0        0        0     1871 2022-10-21 10:13:37.000000 laok-0.2.21/laok/base/sys_/print_info.py
+-rw-rw-rw-   0        0        0      380 2023-07-03 11:23:24.000000 laok-0.2.21/laok/base/sys_/sys_.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.875063 laok-0.2.21/laok/base/test/
+-rw-rw-rw-   0        0        0       43 2022-10-21 10:13:37.000000 laok-0.2.21/laok/base/test/__init__.py
+-rw-rw-rw-   0        0        0     8807 2023-07-14 11:30:11.000000 laok-0.2.21/laok/base/test/_dump.py
+-rw-rw-rw-   0        0        0     4550 2023-07-14 11:28:48.000000 laok-0.2.21/laok/base/test/_run.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.876061 laok-0.2.21/laok/ext/
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.878056 laok-0.2.21/laok/ext/PIL_/
+-rw-rw-rw-   0        0        0        0 2023-07-12 09:00:52.000000 laok-0.2.21/laok/ext/PIL_/__init__.py
+-rw-rw-rw-   0        0        0      439 2023-07-14 12:17:58.000000 laok-0.2.21/laok/ext/PIL_/io.py
+-rw-rw-rw-   0        0        0        0 2023-07-17 13:24:54.000000 laok-0.2.21/laok/ext/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.895010 laok-0.2.21/laok/ext/cv2_/
+-rw-rw-rw-   0        0        0      252 2023-07-12 14:13:06.000000 laok-0.2.21/laok/ext/cv2_/__init__.py
+-rw-rw-rw-   0        0        0     2115 2023-07-12 12:32:21.000000 laok-0.2.21/laok/ext/cv2_/bin.py
+-rw-rw-rw-   0        0        0     1592 2023-07-14 12:35:51.000000 laok-0.2.21/laok/ext/cv2_/contours.py
+-rw-rw-rw-   0        0        0     2580 2023-07-11 11:20:43.000000 laok-0.2.21/laok/ext/cv2_/cvt.py
+-rw-rw-rw-   0        0        0     4565 2023-07-14 12:16:27.000000 laok-0.2.21/laok/ext/cv2_/draw.py
+-rw-rw-rw-   0        0        0      956 2023-07-12 14:26:53.000000 laok-0.2.21/laok/ext/cv2_/edge.py
+-rw-rw-rw-   0        0        0     1268 2023-07-12 13:43:27.000000 laok-0.2.21/laok/ext/cv2_/filter.py
+-rw-rw-rw-   0        0        0      630 2023-07-12 07:16:54.000000 laok-0.2.21/laok/ext/cv2_/geo.py
+-rw-rw-rw-   0        0        0      344 2023-07-15 08:10:53.000000 laok-0.2.21/laok/ext/cv2_/hist.py
+-rw-rw-rw-   0        0        0     1019 2023-07-11 16:28:07.000000 laok-0.2.21/laok/ext/cv2_/info.py
+-rw-rw-rw-   0        0        0     3515 2023-07-15 13:22:38.000000 laok-0.2.21/laok/ext/cv2_/io.py
+-rw-rw-rw-   0        0        0     2787 2023-07-12 13:56:20.000000 laok-0.2.21/laok/ext/cv2_/morph.py
+-rw-rw-rw-   0        0        0     1230 2023-07-11 15:01:26.000000 laok-0.2.21/laok/ext/cv2_/show.py
+-rw-rw-rw-   0        0        0      828 2023-07-11 15:21:15.000000 laok-0.2.21/laok/ext/cv2_/util.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.897004 laok-0.2.21/laok/ext/flask_/
+-rw-rw-rw-   0        0        0       42 2023-04-19 15:05:48.000000 laok-0.2.21/laok/ext/flask_/__init__.py
+-rw-rw-rw-   0        0        0      395 2023-04-19 15:05:30.000000 laok-0.2.21/laok/ext/flask_/app.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.899000 laok-0.2.21/laok/ext/flask_/basic/
+-rw-rw-rw-   0        0        0       22 2023-04-19 15:06:08.000000 laok-0.2.21/laok/ext/flask_/basic/__init__.py
+-rw-rw-rw-   0        0        0      633 2023-04-19 15:38:09.000000 laok-0.2.21/laok/ext/flask_/basic/views.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.901991 laok-0.2.21/laok/ext/lxml_/
+-rw-rw-rw-   0        0        0     1931 2023-07-14 11:55:04.000000 laok-0.2.21/laok/ext/lxml_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.903986 laok-0.2.21/laok/ext/matplot_/
+-rw-rw-rw-   0        0        0       19 2023-07-12 09:01:52.000000 laok-0.2.21/laok/ext/matplot_/__init__.py
+-rw-rw-rw-   0        0        0     2153 2023-07-15 13:24:30.000000 laok-0.2.21/laok/ext/matplot_/show.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.905980 laok-0.2.21/laok/ext/numpy_/
+-rw-rw-rw-   0        0        0        0 2023-04-20 14:21:33.000000 laok-0.2.21/laok/ext/numpy_/__init__.py
+-rw-rw-rw-   0        0        0      391 2023-07-14 11:56:30.000000 laok-0.2.21/laok/ext/numpy_/io.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.906978 laok-0.2.21/laok/ext/onnx_/
+-rw-rw-rw-   0        0        0     3116 2023-07-11 03:56:12.000000 laok-0.2.21/laok/ext/onnx_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.907975 laok-0.2.21/laok/ext/open3d_/
+-rw-rw-rw-   0        0        0      330 2023-07-11 05:10:30.000000 laok-0.2.21/laok/ext/open3d_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.911964 laok-0.2.21/laok/ext/qt_/
+-rw-rw-rw-   0        0        0       62 2023-07-14 02:30:38.000000 laok-0.2.21/laok/ext/qt_/__init__.py
+-rw-rw-rw-   0        0        0      582 2023-07-14 03:03:10.000000 laok-0.2.21/laok/ext/qt_/dialog.py
+-rw-rw-rw-   0        0        0     1004 2023-07-14 02:15:56.000000 laok-0.2.21/laok/ext/qt_/run.py
+-rw-rw-rw-   0        0        0     1931 2023-07-14 03:22:35.000000 laok-0.2.21/laok/ext/qt_/ui.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.912962 laok-0.2.21/laok/ext/requests_/
+-rw-rw-rw-   0        0        0     4021 2023-07-14 11:43:36.000000 laok-0.2.21/laok/ext/requests_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.914957 laok-0.2.21/laok/ext/skimage_/
+-rw-rw-rw-   0        0        0      330 2023-07-11 05:10:30.000000 laok-0.2.21/laok/ext/skimage_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.915954 laok-0.2.21/laok/ext/sklearn_/
+-rw-rw-rw-   0        0        0      330 2023-07-11 05:10:30.000000 laok-0.2.21/laok/ext/sklearn_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.916951 laok-0.2.21/laok/ext/torch_/
+-rw-rw-rw-   0        0        0       88 2023-04-19 08:20:33.000000 laok-0.2.21/laok/ext/torch_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.917949 laok-0.2.21/laok/ext/torch_/cv2d/
+-rw-rw-rw-   0        0        0        2 2023-07-17 13:22:43.000000 laok-0.2.21/laok/ext/torch_/cv2d/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.918946 laok-0.2.21/laok/ext/torch_/cv3d/
+-rw-rw-rw-   0        0        0        2 2023-07-17 13:22:43.000000 laok-0.2.21/laok/ext/torch_/cv3d/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.920941 laok-0.2.21/laok/ext/torch_/cv3d/io/
+-rw-rw-rw-   0        0        0       24 2023-04-21 09:18:03.000000 laok-0.2.21/laok/ext/torch_/cv3d/io/__init__.py
+-rw-rw-rw-   0        0        0      832 2023-04-25 06:52:21.000000 laok-0.2.21/laok/ext/torch_/cv3d/io/_simple.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.934906 laok-0.2.21/laok/ext/torch_/cv3d/trans/
+-rw-rw-rw-   0        0        0      220 2023-06-16 08:02:42.000000 laok-0.2.21/laok/ext/torch_/cv3d/trans/__init__.py
+-rw-rw-rw-   0        0        0      895 2023-04-25 05:31:18.000000 laok-0.2.21/laok/ext/torch_/cv3d/trans/_dropout.py
+-rw-rw-rw-   0        0        0      726 2023-04-25 05:40:44.000000 laok-0.2.21/laok/ext/torch_/cv3d/trans/_jitter.py
+-rw-rw-rw-   0        0        0      660 2023-04-25 03:33:54.000000 laok-0.2.21/laok/ext/torch_/cv3d/trans/_normal.py
+-rw-rw-rw-   0        0        0     5025 2023-04-27 08:53:41.000000 laok-0.2.21/laok/ext/torch_/cv3d/trans/_rotate.py
+-rw-rw-rw-   0        0        0     2164 2023-04-28 03:50:24.000000 laok-0.2.21/laok/ext/torch_/cv3d/trans/_sample.py
+-rw-rw-rw-   0        0        0      618 2023-04-25 02:57:52.000000 laok-0.2.21/laok/ext/torch_/cv3d/trans/_scale.py
+-rw-rw-rw-   0        0        0      585 2023-06-16 09:05:52.000000 laok-0.2.21/laok/ext/torch_/cv3d/trans/_swap_filed.py
+-rw-rw-rw-   0        0        0      485 2023-04-25 03:05:55.000000 laok-0.2.21/laok/ext/torch_/cv3d/trans/_torch.py
+-rw-rw-rw-   0        0        0      680 2023-04-25 05:38:23.000000 laok-0.2.21/laok/ext/torch_/cv3d/trans/_translate.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.936898 laok-0.2.21/laok/ext/torch_/datasets/
+-rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.21/laok/ext/torch_/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.941884 laok-0.2.21/laok/ext/torch_/datasets/kitti/
+-rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.21/laok/ext/torch_/datasets/kitti/__init__.py
+-rw-rw-rw-   0        0        0    12031 2022-11-03 16:22:33.000000 laok-0.2.21/laok/ext/torch_/datasets/kitti/kitti.py
+-rw-rw-rw-   0        0        0    27294 2022-10-28 06:48:12.000000 laok-0.2.21/laok/ext/torch_/datasets/kitti/obj.py
+-rw-rw-rw-   0        0        0    26349 2022-11-03 16:22:33.000000 laok-0.2.21/laok/ext/torch_/datasets/kitti/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.949864 laok-0.2.21/laok/ext/torch_/datasets/model_net/
+-rw-rw-rw-   0        0        0      954 2022-11-03 16:22:33.000000 laok-0.2.21/laok/ext/torch_/datasets/model_net/__init__.py
+-rw-rw-rw-   0        0        0     3615 2023-07-17 13:21:28.000000 laok-0.2.21/laok/ext/torch_/datasets/model_net/model_net.py
+-rw-rw-rw-   0        0        0     4467 2022-11-03 16:22:33.000000 laok-0.2.21/laok/ext/torch_/datasets/model_net/model_net_ineratia.py
+-rw-rw-rw-   0        0        0     3895 2022-11-03 16:22:33.000000 laok-0.2.21/laok/ext/torch_/datasets/model_net/model_net_normals.py
+-rw-rw-rw-   0        0        0     4553 2022-11-03 16:22:33.000000 laok-0.2.21/laok/ext/torch_/datasets/model_net/model_net_normals_diff.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.952857 laok-0.2.21/laok/ext/torch_/datasets/shape_net/
+-rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.21/laok/ext/torch_/datasets/shape_net/__init__.py
+-rw-rw-rw-   0        0        0     5463 2022-10-21 10:13:37.000000 laok-0.2.21/laok/ext/torch_/datasets/shape_net/shape_net.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.953853 laok-0.2.21/laok/ext/torch_/datasets/stanford_indoor/
+-rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.21/laok/ext/torch_/datasets/stanford_indoor/__init__.py
+-rw-rw-rw-   0        0        0    11035 2022-10-12 15:00:14.000000 laok-0.2.21/laok/ext/torch_/datasets/stanford_indoor/_stanford_indoor.py
+-rw-rw-rw-   0        0        0     2811 2022-11-02 07:35:53.000000 laok-0.2.21/laok/ext/torch_/datasets/ustc_lidar.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.959836 laok-0.2.21/laok/ext/torch_/io/
+-rw-rw-rw-   0        0        0       80 2022-10-21 10:13:37.000000 laok-0.2.21/laok/ext/torch_/io/__init__.py
+-rw-rw-rw-   0        0        0      732 2022-10-21 10:13:37.000000 laok-0.2.21/laok/ext/torch_/io/img.py
+-rw-rw-rw-   0        0        0      844 2022-10-21 10:13:37.000000 laok-0.2.21/laok/ext/torch_/io/jit.py
+-rw-rw-rw-   0        0        0     1344 2022-10-21 10:13:37.000000 laok-0.2.21/laok/ext/torch_/io/model.py
+-rw-rw-rw-   0        0        0      466 2022-10-21 10:13:37.000000 laok-0.2.21/laok/ext/torch_/io/onnx.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.965821 laok-0.2.21/laok/ext/torch_/op/
+-rw-rw-rw-   0        0        0       70 2023-04-19 08:22:19.000000 laok-0.2.21/laok/ext/torch_/op/__init__.py
+-rw-rw-rw-   0        0        0      965 2023-04-19 08:22:06.000000 laok-0.2.21/laok/ext/torch_/op/device.py
+-rw-rw-rw-   0        0        0     1703 2023-04-19 08:27:44.000000 laok-0.2.21/laok/ext/torch_/op/module.py
+-rw-rw-rw-   0        0        0     1403 2023-04-19 08:25:22.000000 laok-0.2.21/laok/ext/torch_/op/print_info.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.972801 laok-0.2.21/laok/ext/torch_/trainval/
+-rw-rw-rw-   0        0        0       89 2022-10-21 10:13:37.000000 laok-0.2.21/laok/ext/torch_/trainval/__init__.py
+-rw-rw-rw-   0        0        0     3943 2023-04-19 09:12:20.000000 laok-0.2.21/laok/ext/torch_/trainval/check_point.py
+-rw-rw-rw-   0        0        0     2280 2023-04-19 09:25:29.000000 laok-0.2.21/laok/ext/torch_/trainval/infer.py
+-rw-rw-rw-   0        0        0     2848 2023-04-19 08:44:39.000000 laok-0.2.21/laok/ext/torch_/trainval/train.py
+-rw-rw-rw-   0        0        0     2308 2023-04-19 09:08:59.000000 laok-0.2.21/laok/ext/torch_/trainval/val.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.974796 laok-0.2.21/laok/ext/vtk_/
+-rw-rw-rw-   0        0        0       22 2023-07-17 13:24:43.000000 laok-0.2.21/laok/ext/vtk_/__init__.py
+-rw-rw-rw-   0        0        0     3986 2023-07-17 13:24:32.000000 laok-0.2.21/laok/ext/vtk_/win.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.975793 laok-0.2.21/laok/ext/yaml_/
+-rw-rw-rw-   0        0        0     1329 2023-07-14 11:55:04.000000 laok-0.2.21/laok/ext/yaml_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.978786 laok-0.2.21/laok/tool/
+-rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.21/laok/tool/__init__.py
+-rw-rw-rw-   0        0        0     3604 2023-07-11 06:29:13.000000 laok-0.2.21/laok/tool/download_m3u8.py
+-rw-rw-rw-   0        0        0     2352 2023-07-28 10:46:18.000000 laok-0.2.21/laok/tool/ultralytics_.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:44:55.819213 laok-0.2.21/laok.egg-info/
+-rw-rw-rw-   0        0        0      214 2023-07-28 11:44:55.000000 laok-0.2.21/laok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4153 2023-07-28 11:44:55.000000 laok-0.2.21/laok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 11:44:55.000000 laok-0.2.21/laok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-28 11:44:55.000000 laok-0.2.21/laok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 11:44:55.980780 laok-0.2.21/setup.cfg
+-rw-rw-rw-   0        0        0      322 2023-07-28 11:44:40.000000 laok-0.2.21/setup.py
```

### Comparing `laok-0.2.20/laok/base/alg/addict.py` & `laok-0.2.21/laok/base/alg/addict.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import copy
 # from 'addict' module
 
 class Dict(dict):
-
     def __init__(__self, *args, **kwargs):
         object.__setattr__(__self, '__parent', kwargs.pop('__parent', None))
         object.__setattr__(__self, '__key', kwargs.pop('__key', None))
         object.__setattr__(__self, '__frozen', False)
         for arg in args:
             if not arg:
                 continue
```

### Comparing `laok-0.2.20/laok/base/conf/factory.py` & `laok-0.2.21/laok/base/conf/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,24 @@
 class ObjectFactory:
     def __init__(self):
         self._creator_list = defaultdict(list)
         self._name_list = defaultdict(list)
 
     def get_creator(self, _name, category=None, *args, **kws):
         for creator in self.get_creator_list(category):
-            if _ctor:= creator(_name, *args, **kws):
+            _ctor = creator(_name, *args, **kws)
+            if _ctor:
                 return _ctor
 
     def get_instance(self, _name, category=None, _args=None, _kws=None, *args, **kws):
         if _args is None: _args = ()
         if _kws is None: _kws = {}
         if args is None: args = ()
-        if ctor := self.get_creator(category, _name, *_args, **_kws):
+        ctor = self.get_creator(category, _name, *_args, **_kws)
+        if ctor:
             return ctor(*args, **kws)
 
     def _add_name(self, _list, name):
         if name:
             _list.append(name)
 
     def add_name(self, category, *names):
```

### Comparing `laok-0.2.20/laok/base/dataset/cvt_voc_yolo.py` & `laok-0.2.21/laok/base/dataset/cvt_voc_yolo.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/base/dataset/darknet-voc2yolo.py` & `laok-0.2.21/laok/base/dataset/darknet-voc2yolo.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/base/dataset/voc_label.py` & `laok-0.2.21/laok/base/dataset/voc_label.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/base/dtime/timer.py` & `laok-0.2.21/laok/base/dtime/timer.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/base/fs/fname.py` & `laok-0.2.21/laok/base/fs/fname.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/base/fs/fpath.py` & `laok-0.2.21/laok/base/fs/fpath.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/base/fs/fsearch.py` & `laok-0.2.21/laok/base/fs/fsearch.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/base/fs/fwalk.py` & `laok-0.2.21/laok/base/fs/fwalk.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/base/fs/name_index.py` & `laok-0.2.21/laok/base/fs/name_index.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/base/log/log.py` & `laok-0.2.21/laok/base/log/log.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     def inner(*args, sep=' ', **kws):
         msg = sep.join(str(x) for x in args)
         return func(msg, **kws)
     return inner
 
 def get_logger(name=None, level=logging.DEBUG):
     if name is None:
-        name = "[laok]"
+        name = "laok"
 
     if name in _logger_cache:
         return _logger_cache[name]
 
     log = logging.getLogger(name)
     _logger_cache[name] = log
     log.setLevel(level)
```

### Comparing `laok-0.2.20/laok/base/log/log_default.py` & `laok-0.2.21/laok/base/log/log_default.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/base/net/ip.py` & `laok-0.2.21/laok/base/net/ip.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/base/net/requests_.py` & `laok-0.2.21/laok/ext/requests_/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 # -*- coding: utf-8 -*-
 '''
 Created on 2023/4/19 19:43:45
 @author: LiuKuan
 @copyright: Apache License, Version 2.0
 '''
 from laok.third_lib import requests as _request
-from ..fs import file_write_bin, path_exist
-from ..net import url_make_file
+from laok.base.fs import file_write_bin, path_exist
+from laok.base.net import url_make_file
 #===============================================================================
 r'''使得 requests库 可以随机生成 user_agent
 '''
 #===============================================================================
-__all__ = ['random_user_agent', 'req_save', 'req_text', 'req_json', 'req_content']
+__all__ = ['random_user_agent', 'req', 'req_text', 'req_json', 'req_content', 'req_save', 'req_save_auto']
 
 _random_user_agent = False
 def random_user_agent():
     ''' 拦截请求的参数,将headers修改为 自定义的 user_agent
     :return:
     '''
     global _random_user_agent
@@ -51,30 +51,37 @@
             headers = {}
         headers['User-Agent'] = random.choice(user_agent_pc)
         kwargs['headers'] = headers
         return _req(*args, **kwargs)
     _request.Session.request = user_agent_req
 
 def req(url, method='get', **kws):
+    '''设置随机 user-agent,然后执行请求
+    '''
     random_user_agent()
     return _request.request(method=method, url=url, **kws)
 
 def req_text(url, method='get', **kws):
+    '''返回 text '''
     return req(url=url, method=method, **kws).text
 
 def req_json(url, method='get', **kws):
+    '''返回 json '''
     return req(url=url, method=method, **kws).json()
 
 def req_content(url, method='get', **kws):
+    '''返回二进制内容'''
     return req(url=url, method=method, **kws).content
 
 def req_save(fname, url, method='get', skip_exist=False, **kws):
+    '''baocun数据'''
     if skip_exist and path_exist(fname):
-        return
+        return fname
     data = req_content(url=url, method=method, **kws)
     file_write_bin(fname, data)
+    return fname
 
 def req_save_auto(url, method='get', skip_exist=False, **kws):
     fname = url_make_file(url)
     req_save(fname=fname, url=url, method=method, skip_exist=skip_exist, **kws)
     return fname
```

### Comparing `laok-0.2.20/laok/base/net/url.py` & `laok-0.2.21/laok/base/net/url.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/base/paral/pool.py` & `laok-0.2.21/laok/base/paral/pool.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/base/pkg/_lazy.py` & `laok-0.2.21/laok/base/pkg/_lazy.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/base/ser/json_.py` & `laok-0.2.21/laok/base/ser/json_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/base/ser/marshal_.py` & `laok-0.2.21/laok/base/ser/marshal_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/base/ser/numpy_.py` & `laok-0.2.21/laok/base/ser/numpy_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/base/ser/pickle_.py` & `laok-0.2.21/laok/base/ser/pickle_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/base/ser/torch_.py` & `laok-0.2.21/laok/base/ser/torch_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/base/ser/xml_.py` & `laok-0.2.21/laok/base/ser/xml_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/base/ser/yaml_.py` & `laok-0.2.21/laok/base/ser/yaml_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/base/str/cvt.py` & `laok-0.2.21/laok/base/str/cvt.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/base/str/misc.py` & `laok-0.2.21/laok/base/str/misc.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/base/str/print_info.py` & `laok-0.2.21/laok/base/str/print_info.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/base/syst/platform_.py` & `laok-0.2.21/laok/base/sys_/platform_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/base/syst/print_info.py` & `laok-0.2.21/laok/base/sys_/print_info.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/base/test/_dump.py` & `laok-0.2.21/laok/base/test/_dump.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,21 @@
                           '__loader__', '__name__', '__package__', '__path__', '__spec__']
 
 _CLASS_DEFAULT_FIELDS = ['__dict__', '__doc__', '__module__', '__weakref__',
                          '__init_subclass__', '__subclasshook__', '__class__']
 
 def get_module_path(mod):
     pth = ''
-    if fname := getattr(mod, '__file__', ''):
+
+    fname = getattr(mod, '__file__', '')
+    if fname:
         pth = fname
-    if nsPath := getattr(mod, '__path__', tuple() ):
+
+    nsPath = getattr(mod, '__path__', None)
+    if nsPath:
         pth = nsPath[0]
     return pth
 
 def _is_third_pkg(mod):
     return 'site-packages' in get_module_path(mod)
 
 def _is_in_same_pkg(mod1, mod2):
```

### Comparing `laok-0.2.20/laok/base/test/_run.py` & `laok-0.2.21/laok/base/test/_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # 交互式运行
 #===============================================================================
 PRINT_FUNC_COUNT = 3
 
 __all__ = ['run', 'main_module']
 main_module = sys.modules.get('__main__')
 
-
 # 执行计时
 def _time_run(_kvfunc, _repeat = 1, **kws):
     name, func = _kvfunc
     print('{}==begin[date:{}]'.format(name, datetime.now().strftime('%Y-%m-%d %H:%M:%S')))
 
     t0 = time.time()
     for i in range(_repeat):
```

### Comparing `laok-0.2.20/laok/cv2d/cv2_/bin.py` & `laok-0.2.21/laok/ext/cv2_/bin.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/cv2d/cv2_/cvt.py` & `laok-0.2.21/laok/ext/cv2_/cvt.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/cv2d/cv2_/draw.py` & `laok-0.2.21/laok/ext/cv2_/draw.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 # -*- coding: utf-8 -*-
 '''
 Created on 2023/7/11 20:36:06
 
 @author: LiuKuan
 @copyright: Apache License, Version 2.0
 '''
-import cv2, numpy as np
+import cv2
+from laok.base.colors import color_rand
 from .info import image_size, image_center
-from .util import keep_uint8, keep_int32
+from .util import keep_int32
 # ===============================================================================
 r'''
 
 绘制图元:
     line
     circle
     rectangle
@@ -29,18 +30,18 @@
     lineType：线的类型，是否为8连接线，抗锯齿线等。
         默认情况下，为8连接线。**cv.LINE_AA**给出了抗锯齿的线条，看起来非常适合曲线。
 '''
 # ===============================================================================
 __all__ = [
             'draw_point',
             'draw_line', 'draw_polylines',
-           'draw_rect',
-           'draw_circle', 'draw_ellipse', 'draw_arc',
-           'draw_text',
-           'draw_contour', 'draw_contours'
+            'draw_rect',
+            'draw_circle', 'draw_ellipse', 'draw_arc',
+            'draw_text',
+            'draw_contour', 'draw_contours'
 ]
 
 def draw_point(img, pt=None, size=1, color=(255,255,255)):
     if pt is None: #默认使用中心点
         pt = image_center(img)
     return cv2.circle(img, center=keep_int32(pt), radius=int(size), color=color, thickness=-1, lineType=cv2.LINE_AA)
 
@@ -89,8 +90,12 @@
     return cv2.putText(img, text=text, org=pos, fontFace=fontFace, fontScale=fontScale,
                 color=color, thickness=thickness, lineType=lineType)
 
 def draw_contour(img, contour, color=(255,255,255), thickness=2, lineType=cv2.LINE_AA):
     return cv2.drawContours(img, [contour], contourIdx=-1, color=color, thickness=thickness, lineType=lineType)
 
 def draw_contours(img, contours, color=(255,255,255), thickness=2, lineType=cv2.LINE_AA):
-    return cv2.drawContours(img, contours, contourIdx=-1, color=color, thickness=thickness, lineType=lineType)
+    if color is None:
+        for i, contour in enumerate(contours):
+            draw_contour(img, contour, color=color_rand(i), thickness=thickness, lineType=lineType)
+    else:
+        return cv2.drawContours(img, contours, contourIdx=-1, color=color, thickness=thickness, lineType=lineType)
```

### Comparing `laok-0.2.20/laok/cv2d/cv2_/edge.py` & `laok-0.2.21/laok/ext/cv2_/edge.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/cv2d/cv2_/filter.py` & `laok-0.2.21/laok/ext/cv2_/filter.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/cv2d/cv2_/geo.py` & `laok-0.2.21/laok/ext/cv2_/geo.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/cv2d/cv2_/info.py` & `laok-0.2.21/laok/ext/cv2_/info.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/cv2d/cv2_/io.py` & `laok-0.2.21/laok/ext/cv2_/io.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,19 +36,24 @@
     if not bgr:
         return swap_rb(img)
     return img
 
 def read_gray(filename):
     return read_image(filename, cv2.IMREAD_GRAYSCALE)
 
-def write_image(data, filename):
+def write_image(filename, data, params=None):
     name, ext = os.path.splitext(filename)
-    retval, buf = cv2.imencode(ext, data)
+    retval, buf = cv2.imencode(ext, data, params)
     return buf.tofile(filename)
 
+def write_jpg(filename, data, quality=95):
+    return write_image(filename, data, [cv2.IMWRITE_JPEG_QUALITY, quality])
+
+def write_png(filename, data, compression=1):
+    return write_image(filename, data, [cv2.IMWRITE_PNG_COMPRESSION, compression])
 ####################    读取视频和相机
 def _read_capture(fileOrId):
     try:
         cap = cv2.VideoCapture(fileOrId)
         while True:
             ret, frame = cap.read()
             if not ret:  # 如果正确读取帧，ret为True
```

### Comparing `laok-0.2.20/laok/cv2d/cv2_/morph.py` & `laok-0.2.21/laok/ext/cv2_/morph.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/cv2d/cv2_/show.py` & `laok-0.2.21/laok/ext/cv2_/show.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/cv2d/cv2_/util.py` & `laok-0.2.21/laok/ext/cv2_/util.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/data/lxml_/__init__.py` & `laok-0.2.21/laok/ext/lxml_/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Created on 2023/7/11 11:49:12
 
 @author: LiuKuan
 @copyright: Apache License, Version 2.0
 '''
 from lxml import etree, objectify
 from laok.base.fs import file_read_text, file_write_text, path_exist
-from laok.base.net.requests_ import req_text
+from laok.net.requests_ import req_text
 # ===============================================================================
 r'''
 '''
 # ===============================================================================
 __all__ = ['load_html', 'load_html_text', 'load_html_url',
            'load_xml', 'load_xml_text',
            'save_xml']
@@ -52,11 +52,10 @@
         data = etree.ElementTree(data)
 
     if isinstance(data, objectify.ObjectifiedElement):
         data = etree.ElementTree(data)
 
     if isinstance(data, etree._ElementTree):
         kws.setdefault('encoding', 'utf8')
-        # kws.setdefault('strip_text', True)
         kws.setdefault('pretty_print', True)
         data.write(filename, **kws)
         return True
```

### Comparing `laok-0.2.20/laok/dnn/onnx_/__init__.py` & `laok-0.2.21/laok/ext/onnx_/__init__.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/dnn/torch_/datasets/kitti/kitti.py` & `laok-0.2.21/laok/ext/torch_/datasets/kitti/kitti.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/dnn/torch_/datasets/kitti/obj.py` & `laok-0.2.21/laok/ext/torch_/datasets/kitti/obj.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/dnn/torch_/datasets/kitti/utils.py` & `laok-0.2.21/laok/ext/torch_/datasets/kitti/utils.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/dnn/torch_/datasets/model_net/__init__.py` & `laok-0.2.21/laok/ext/torch_/datasets/model_net/__init__.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/dnn/torch_/datasets/model_net/model_net.py` & `laok-0.2.21/laok/ext/torch_/datasets/model_net/model_net_normals.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,28 +7,33 @@
 @copyright: Apache License, Version 2.0
 '''
 import os
 import numpy as np
 from torch.utils.data import Dataset
 import laok.util.log as klog
 import laok.cv3d as kcv3
-import laok.util.fs as kfs
-import laok.util.parallel as kparal
 # ===============================================================================
 r'''
 '''
 # ===============================================================================
 
-class Modelnet(Dataset):
-    def __init__(self, root, split='train', num_point=1024, num_category=40, transforms=None, cached=False, show_info=False):
+class ModelnetNormals(Dataset):
+    def __init__(self, root, split='train',
+                 num_point = 1024,
+                 num_category = 40,
+                 normal_knn = 3,
+                 transform=None,
+                 cached = False,
+                 show_info = False,
+                 ):
         self.root = root
         self.npoints = num_point
         self.num_category = num_category
-        self.transforms = transforms
         self.split = split
+        self.transform = transform
         klog.debug(f'===== {self.__class__.__name__}')
         klog.debug(f'root={root}')
         klog.debug(f'split={split}, num_point={num_point}, num_category={num_category}')
 
         if self.num_category == 10:
             self.catfile = os.path.join(self.root, 'modelnet10_shape_names.txt')
         else:
@@ -51,46 +56,50 @@
             shape_ids['test'] = [line.rstrip() for line in open(os.path.join(self.root, 'modelnet40_test.txt'))]
 
         assert (split == 'train' or split == 'test')
         shape_names = ['_'.join(x.split('_')[0:-1]) for x in shape_ids[split]]
         self.datapath = [(shape_names[i], os.path.join(self.root, shape_names[i], shape_ids[split][i]) + '.txt') for i
                          in range(len(shape_ids[split]))]
         print('The size of %s data is %d' % (split, len(self.datapath)))
+
+        self.normal_knn = normal_knn
         self.show_info = show_info
 
     def __len__(self):
         return len(self.datapath)
 
     def _get_item(self, index):
-        name, fname = self.datapath[index]
+        name, ptfile = self.datapath[index]
+
+        if self.show_info:
+            klog.info(f'{name} {ptfile}')
+
         cls = self.classes[name]
         label = np.array([cls]).astype(np.int32)
+        point_set = np.loadtxt(ptfile, delimiter=',').astype(np.float32)
+
+        normal_file = ptfile.replace('.txt', "-%02d.normals" % self.normal_knn)
         if self.show_info:
-            klog.info(f'load {fname}')
-        point_set = np.loadtxt(fname, delimiter=',').astype(np.float32)
+            klog.info(f'normal_file: {normal_file}')
+
+        normal_set = np.loadtxt(normal_file, delimiter=',').astype(np.float32)
+        point_set = np.concatenate([point_set[:, 0:3], normal_set], axis=1)
         # point_set = kcv3.farthest_point_sample(point_set, self.npoints)
         if self.split == 'train':
             point_set = kcv3.random_sample(point_set, self.npoints)
         else:
             point_set = point_set[:self.npoints, :]
-
         point_set[:, 0:3] = kcv3.pc_normalize(point_set[:, 0:3])
-        if self.transforms:
-            point_set = self.transforms(point_set)
+
+        if self.transform:
+            point_set = self.transform(point_set)
         return point_set, label[0]
 
     def __getitem__(self, index):
         return self._get_item(index)
 
+
+
 if __name__ == '__main__':
-    import torch
-    import laok.util.torch_ as ktorch
     import laok.util.conf as kconf
+    data = ModelnetNormals(kconf.get_conf('datasets').ModelnetNormals,  num_point=1024, show_info=True, cached=True)
 
-    dataset = Modelnet(kconf.get_conf('datasets').Modelnet ,  num_point=1024, show_info=True, cached=True)
-    # DataLoader = torch.utils.data.DataLoader(dataset, batch_size=2, shuffle=False)
-    # for point, label in dataset:
-    #     ktorch.pr(point)
-    #     ktorch.pr(label)
-
-    #     kcv3.show_cld_xyz(point[0])
-    #     break
```

### Comparing `laok-0.2.20/laok/dnn/torch_/datasets/model_net/model_net_ineratia.py` & `laok-0.2.21/laok/ext/torch_/datasets/model_net/model_net_ineratia.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/dnn/torch_/datasets/model_net/model_net_normals.py` & `laok-0.2.21/laok/ext/torch_/datasets/model_net/model_net_normals_diff.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,34 +6,37 @@
 @author: LiuKuan
 @copyright: Apache License, Version 2.0
 '''
 import os
 import numpy as np
 from torch.utils.data import Dataset
 import laok.util.log as klog
+import laok.util.fs as kfs
+import laok.util.parallel as kparal
 import laok.cv3d as kcv3
 # ===============================================================================
 r'''
 '''
 # ===============================================================================
 
-class ModelnetNormals(Dataset):
+class ModelnetNormalsDiff(Dataset):
     def __init__(self, root, split='train',
                  num_point = 1024,
                  num_category = 40,
-                 normal_knn = 3,
+                 normal_small_knn = 3,
+                 normal_large_knn = 6,
                  transform=None,
                  cached = False,
                  show_info = False,
                  ):
         self.root = root
         self.npoints = num_point
         self.num_category = num_category
-        self.split = split
         self.transform = transform
+        self.split = split
         klog.debug(f'===== {self.__class__.__name__}')
         klog.debug(f'root={root}')
         klog.debug(f'split={split}, num_point={num_point}, num_category={num_category}')
 
         if self.num_category == 10:
             self.catfile = os.path.join(self.root, 'modelnet10_shape_names.txt')
         else:
@@ -57,15 +60,17 @@
 
         assert (split == 'train' or split == 'test')
         shape_names = ['_'.join(x.split('_')[0:-1]) for x in shape_ids[split]]
         self.datapath = [(shape_names[i], os.path.join(self.root, shape_names[i], shape_ids[split][i]) + '.txt') for i
                          in range(len(shape_ids[split]))]
         print('The size of %s data is %d' % (split, len(self.datapath)))
 
-        self.normal_knn = normal_knn
+        self._cache = {}
+        self.normal_small_knn = normal_small_knn
+        self.normal_large_knn = normal_large_knn
         self.show_info = show_info
 
     def __len__(self):
         return len(self.datapath)
 
     def _get_item(self, index):
         name, ptfile = self.datapath[index]
@@ -73,33 +78,43 @@
         if self.show_info:
             klog.info(f'{name} {ptfile}')
 
         cls = self.classes[name]
         label = np.array([cls]).astype(np.int32)
         point_set = np.loadtxt(ptfile, delimiter=',').astype(np.float32)
 
-        normal_file = ptfile.replace('.txt', "-%02d.normals" % self.normal_knn)
+        normal_samll_file = ptfile.replace('.txt', "-%02d.normals" % self.normal_small_knn)
+        if self.show_info:
+            klog.info(f'normal_samll_file: {normal_samll_file}')
+        normal_small_set = np.loadtxt(normal_samll_file, delimiter=',').astype(np.float32)
+
+        normal_large_file = ptfile.replace('.txt', "-%02d.normals" % self.normal_large_knn)
         if self.show_info:
-            klog.info(f'normal_file: {normal_file}')
+            klog.info(f'normal_large_file: {normal_large_file}')
+        normal_large_set = np.loadtxt(normal_large_file, delimiter=',').astype(np.float32)
 
-        normal_set = np.loadtxt(normal_file, delimiter=',').astype(np.float32)
+        normal_set = (normal_small_set - normal_large_set) / 2
         point_set = np.concatenate([point_set[:, 0:3], normal_set], axis=1)
         # point_set = kcv3.farthest_point_sample(point_set, self.npoints)
         if self.split == 'train':
             point_set = kcv3.random_sample(point_set, self.npoints)
         else:
             point_set = point_set[:self.npoints, :]
+
         point_set[:, 0:3] = kcv3.pc_normalize(point_set[:, 0:3])
 
         if self.transform:
             point_set = self.transform(point_set)
         return point_set, label[0]
 
     def __getitem__(self, index):
+        '''
+        :param index:
+        :return:  point_set, label
+        '''
         return self._get_item(index)
 
 
-
 if __name__ == '__main__':
     import laok.util.conf as kconf
-    data = ModelnetNormals(kconf.get_conf('datasets').ModelnetNormals,  num_point=1024, show_info=True, cached=True)
+    data = ModelnetNormalsDiff(kconf.get_conf('datasets').ModelnetNormals,  num_point=1024, show_info=True, cached=True)
```

### Comparing `laok-0.2.20/laok/dnn/torch_/datasets/model_net/model_net_normals_diff.py` & `laok-0.2.21/laok/ext/torch_/datasets/model_net/model_net.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,116 +5,90 @@
 
 @author: LiuKuan
 @copyright: Apache License, Version 2.0
 '''
 import os
 import numpy as np
 from torch.utils.data import Dataset
-import laok.util.log as klog
-import laok.util.fs as kfs
-import laok.util.parallel as kparal
-import laok.cv3d as kcv3
+from laok import log_info
 # ===============================================================================
 r'''
 '''
 # ===============================================================================
 
-class ModelnetNormalsDiff(Dataset):
-    def __init__(self, root, split='train',
-                 num_point = 1024,
-                 num_category = 40,
-                 normal_small_knn = 3,
-                 normal_large_knn = 6,
-                 transform=None,
-                 cached = False,
-                 show_info = False,
-                 ):
+class Modelnet(Dataset):
+    def __init__(self, root, split='train', num_point=1024, num_category=40, transforms=None, cached=False, show_info=False):
         self.root = root
         self.npoints = num_point
         self.num_category = num_category
-        self.transform = transform
+        self.transforms = transforms
         self.split = split
-        klog.debug(f'===== {self.__class__.__name__}')
-        klog.debug(f'root={root}')
-        klog.debug(f'split={split}, num_point={num_point}, num_category={num_category}')
+
+        log_info(f'===== {self.__class__.__name__}')
+        log_info(f'root={root}')
+        log_info(f'split={split}, num_point={num_point}, num_category={num_category}')
 
         if self.num_category == 10:
             self.catfile = os.path.join(self.root, 'modelnet10_shape_names.txt')
         else:
             self.catfile = os.path.join(self.root, 'modelnet40_shape_names.txt')
 
-        klog.debug(f'catfile={self.catfile}')
+        log_info(f'catfile={self.catfile}')
 
         self.cat = [line.rstrip() for line in open(self.catfile)]
         self.classes = dict(zip(self.cat, range(len(self.cat))))
 
-        klog.debug(f'cat={self.cat}')
-        klog.debug(f'classes={self.classes}')
+        log_info(f'cat={self.cat}')
+        log_info(f'classes={self.classes}')
 
         shape_ids = {}
         if self.num_category == 10:
             shape_ids['train'] = [line.rstrip() for line in open(os.path.join(self.root, 'modelnet10_train.txt'))]
             shape_ids['test'] = [line.rstrip() for line in open(os.path.join(self.root, 'modelnet10_test.txt'))]
         else:
             shape_ids['train'] = [line.rstrip() for line in open(os.path.join(self.root, 'modelnet40_train.txt'))]
             shape_ids['test'] = [line.rstrip() for line in open(os.path.join(self.root, 'modelnet40_test.txt'))]
 
         assert (split == 'train' or split == 'test')
         shape_names = ['_'.join(x.split('_')[0:-1]) for x in shape_ids[split]]
         self.datapath = [(shape_names[i], os.path.join(self.root, shape_names[i], shape_ids[split][i]) + '.txt') for i
                          in range(len(shape_ids[split]))]
-        print('The size of %s data is %d' % (split, len(self.datapath)))
-
-        self._cache = {}
-        self.normal_small_knn = normal_small_knn
-        self.normal_large_knn = normal_large_knn
+        log_info(f'The size of {split} data is {len(self.datapath)}')
         self.show_info = show_info
 
     def __len__(self):
         return len(self.datapath)
 
     def _get_item(self, index):
-        name, ptfile = self.datapath[index]
-
-        if self.show_info:
-            klog.info(f'{name} {ptfile}')
-
+        name, fname = self.datapath[index]
         cls = self.classes[name]
         label = np.array([cls]).astype(np.int32)
-        point_set = np.loadtxt(ptfile, delimiter=',').astype(np.float32)
-
-        normal_samll_file = ptfile.replace('.txt', "-%02d.normals" % self.normal_small_knn)
         if self.show_info:
-            klog.info(f'normal_samll_file: {normal_samll_file}')
-        normal_small_set = np.loadtxt(normal_samll_file, delimiter=',').astype(np.float32)
-
-        normal_large_file = ptfile.replace('.txt', "-%02d.normals" % self.normal_large_knn)
-        if self.show_info:
-            klog.info(f'normal_large_file: {normal_large_file}')
-        normal_large_set = np.loadtxt(normal_large_file, delimiter=',').astype(np.float32)
-
-        normal_set = (normal_small_set - normal_large_set) / 2
-        point_set = np.concatenate([point_set[:, 0:3], normal_set], axis=1)
+            log_info(f'load {fname}')
+        point_set = np.loadtxt(fname, delimiter=',').astype(np.float32)
         # point_set = kcv3.farthest_point_sample(point_set, self.npoints)
         if self.split == 'train':
             point_set = kcv3.random_sample(point_set, self.npoints)
         else:
             point_set = point_set[:self.npoints, :]
 
         point_set[:, 0:3] = kcv3.pc_normalize(point_set[:, 0:3])
-
-        if self.transform:
-            point_set = self.transform(point_set)
+        if self.transforms:
+            point_set = self.transforms(point_set)
         return point_set, label[0]
 
     def __getitem__(self, index):
-        '''
-        :param index:
-        :return:  point_set, label
-        '''
         return self._get_item(index)
 
-
 if __name__ == '__main__':
+    import torch
+    import laok.util.torch_ as ktorch
     import laok.util.conf as kconf
-    data = ModelnetNormalsDiff(kconf.get_conf('datasets').ModelnetNormals,  num_point=1024, show_info=True, cached=True)
 
+    dataset = Modelnet(kconf.get_conf('datasets').Modelnet ,  num_point=1024, show_info=True, cached=True)
+    # DataLoader = torch.utils.data.DataLoader(dataset, batch_size=2, shuffle=False)
+    # for point, label in dataset:
+    #     ktorch.pr(point)
+    #     ktorch.pr(label)
+
+    #     kcv3.show_cld_xyz(point[0])
+    #     break
```

### Comparing `laok-0.2.20/laok/dnn/torch_/datasets/shape_net/shape_net.py` & `laok-0.2.21/laok/ext/torch_/datasets/shape_net/shape_net.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/dnn/torch_/datasets/stanford_indoor/_stanford_indoor.py` & `laok-0.2.21/laok/ext/torch_/datasets/stanford_indoor/_stanford_indoor.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/dnn/torch_/datasets/ustc_lidar.py` & `laok-0.2.21/laok/ext/torch_/datasets/ustc_lidar.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/dnn/torch_/io/img.py` & `laok-0.2.21/laok/ext/torch_/io/img.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/dnn/torch_/io/jit.py` & `laok-0.2.21/laok/ext/torch_/io/jit.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/dnn/torch_/io/model.py` & `laok-0.2.21/laok/ext/torch_/io/model.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/dnn/torch_/op/device.py` & `laok-0.2.21/laok/ext/torch_/op/device.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/dnn/torch_/op/module.py` & `laok-0.2.21/laok/ext/torch_/op/module.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/dnn/torch_/op/print_info.py` & `laok-0.2.21/laok/ext/torch_/op/print_info.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/dnn/torch_/trainval/check_point.py` & `laok-0.2.21/laok/ext/torch_/trainval/check_point.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/dnn/torch_/trainval/infer.py` & `laok-0.2.21/laok/ext/torch_/trainval/infer.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/dnn/torch_/trainval/train.py` & `laok-0.2.21/laok/ext/torch_/trainval/train.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/dnn/torch_/trainval/val.py` & `laok-0.2.21/laok/ext/torch_/trainval/val.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/gui/matplot_/show.py` & `laok-0.2.21/laok/ext/matplot_/show.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,17 +23,17 @@
     if img_kws is None:
         img_kws = {}
 
     if is_opencv:
         if img.ndim == 2:
             img_kws.setdefault('cmap', 'gray')
         if img.ndim == 3:
-            im_swap = img.copy()
-            im_swap[:, :, 0], im_swap[:, :, 2] = img[:, :, 2], img[:, :, 0]
-            img = im_swap
+            # im_swap = img.copy()
+            # im_swap[:, :, 0], im_swap[:, :, 2] = img[:, :, 2], img[:, :, 0]
+            img = img[:, :, ::-1]
 
     axes.imshow(img, **img_kws)
 
     axes.get_xaxis().set_visible(False) #隐藏x轴
     axes.get_yaxis().set_visible(False) #隐藏y轴
 
     plt.show()
@@ -52,15 +52,16 @@
         if i < len(images):
 
             img = images[i]
             if is_opencv:
                 if img.ndim == 2:
                     img_kws.setdefault('cmap', 'gray')
                 if img.ndim == 3:
-                    img = img[:, :, [2,1,0]]
+                    # img = img[:, :, [2,1,0]]
+                    img = img[:, :, ::-1]
 
             f.imshow(img, **img_kws)
 
             if labels and i < len(labels):
                 f.set_title(labels[i])
         else:
             f.spines['top'].set_visible(False)
```

### Comparing `laok-0.2.20/laok/gui/qt_/dialog.py` & `laok-0.2.21/laok/ext/qt_/dialog.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/gui/qt_/run.py` & `laok-0.2.21/laok/ext/qt_/run.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/gui/qt_/ui.py` & `laok-0.2.21/laok/ext/qt_/ui.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/net/flask_/basic/views.py` & `laok-0.2.21/laok/ext/flask_/basic/views.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/tool/download_m3u8.py` & `laok-0.2.21/laok/tool/download_m3u8.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.20/laok/tool/ultralytics_.py` & `laok-0.2.21/laok/tool/ultralytics_.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 # -*- coding: utf-8 -*-
 '''
 Created on 2023/5/4 20:27:02
 @author: LiuKuan
 @copyright: Apache License, Version 2.0
 '''
 import laok
-from laok.cv2d.io import fix_cv_read
+from laok.ext.cv2_.io import fix_cv_read
+from laok.ext.yaml_ import save_yaml_file
 from ultralytics import YOLO
 #===============================================================================
 r'''支持 yolo训练的脚本
 需要 文件夹 root_dir下:
                 ---- xxx.pt
                 ---- xxx.names
                 ---- Image/
@@ -24,15 +25,15 @@
     dataset.path = laok.path_native(root_dir)
     dataset.train = 'Image'
     dataset.val = 'Image'
     dataset.test = ''
     dataset.names = list(laok.file_read_lines(names_file))
     if filename is None:
         filename = laok.path_replace_ext(names_file, ".yaml")
-    laok.save_yaml_file(filename, dataset, indent=4, encoding='utf8')
+    save_yaml_file(filename, dataset, indent=4, encoding='utf8')
     return filename
 
 def train_det(root_dir, model_file=None, data_file=None, imgsz=(512, 1248), epochs=100, batch=16, **kwargs):
     print(f'root_dir: {root_dir}')
 
     if model_file is None:
         model_file = laok.path_search_cur_ext(root_dir, ".pt")
```

