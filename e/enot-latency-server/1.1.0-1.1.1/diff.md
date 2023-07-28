# Comparing `tmp/enot-latency-server-1.1.0.tar.gz` & `tmp/enot_latency_server-1.1.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/yanchenko/dev/enot-latency-server/dist/tmph68fz4je/enot-latency-server-1.1.0.tar", last modified: Fri Jul 28 08:55:30 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

