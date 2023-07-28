# Comparing `tmp/byquant-1.7.27.tar.gz` & `tmp/byquant-1.7.28-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byquant-1.7.27.tar", last modified: Fri Jul 28 10:29:17 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

