# Comparing `tmp/relativedate-1.3.2.tar.gz` & `tmp/relativedate-1.3.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relativedate-1.3.2.tar", last modified: Mon May 29 20:15:27 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

