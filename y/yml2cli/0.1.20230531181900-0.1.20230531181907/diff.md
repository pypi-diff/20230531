# Comparing `tmp/yml2cli-0.1.20230531181900.tar.gz` & `tmp/yml2cli-0.1.20230531181907-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yml2cli-0.1.20230531181900.tar", last modified: Wed May 31 18:19:00 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

