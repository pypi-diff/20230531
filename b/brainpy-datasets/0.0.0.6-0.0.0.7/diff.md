# Comparing `tmp/brainpy_datasets-0.0.0.6.tar.gz` & `tmp/brainpy_datasets-0.0.0.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainpy_datasets-0.0.0.6.tar", last modified: Mon Feb 27 04:51:33 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

