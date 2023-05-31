# Comparing `tmp/configdict-2.6.0.tar.gz` & `tmp/configdict-2.6.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configdict-2.6.0.tar", last modified: Wed Mar 29 14:40:11 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

