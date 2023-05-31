# Comparing `tmp/pnsgraph-0.0.1.tar.gz` & `tmp/pnsgraph-0.0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pnsgraph-0.0.1.tar", last modified: Tue May 30 03:40:04 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

