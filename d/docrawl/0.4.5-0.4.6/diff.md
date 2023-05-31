# Comparing `tmp/docrawl-0.4.5.tar.gz` & `tmp/docrawl-0.4.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docrawl-0.4.5.tar", last modified: Thu Apr 27 23:47:40 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

