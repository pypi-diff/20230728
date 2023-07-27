# Comparing `tmp/mesh_database_client-1.1.tar.gz` & `tmp/mesh_database_client-1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mesh_database_client-1.1.tar", last modified: Tue Jul 18 06:24:18 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

