# Comparing `tmp/mypy-boto3-scheduler-1.28.12.tar.gz` & `tmp/mypy_boto3_scheduler-1.28.15-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-scheduler-1.28.12.tar", last modified: Thu Jul 27 11:49:35 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

