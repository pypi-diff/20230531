# Comparing `tmp/pybasilica-0.1.2.tar.gz` & `tmp/pybasilica-0.1.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybasilica-0.1.2.tar", last modified: Sun Nov 20 17:48:07 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

