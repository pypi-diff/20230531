# Comparing `tmp/PyUpyog-0.5.14.tar.gz` & `tmp/PyUpyog-0.5.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyUpyog-0.5.14.tar", last modified: Wed May 31 19:47:12 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

