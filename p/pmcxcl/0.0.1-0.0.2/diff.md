# Comparing `tmp/pmcxcl-0.0.1.tar.gz` & `tmp/pmcxcl-0.0.2-pp38-pypy38_pp73-macosx_11_0_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmcxcl-0.0.1.tar", last modified: Thu Jul 27 18:22:26 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

