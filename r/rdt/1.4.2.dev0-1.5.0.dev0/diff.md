# Comparing `tmp/rdt-1.4.2.dev0.tar.gz` & `tmp/rdt-1.5.0.dev0-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdt-1.4.2.dev0.tar", last modified: Mon May  1 18:10:49 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

