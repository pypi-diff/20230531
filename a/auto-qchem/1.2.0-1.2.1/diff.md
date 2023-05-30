# Comparing `tmp/auto-qchem-1.2.0.tar.gz` & `tmp/auto_qchem-1.2.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/auto-qchem-1.2.0.tar", last modified: Tue May 30 23:15:22 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

