# Comparing `tmp/pvxslibs-1.2.0a1.tar.gz` & `tmp/pvxslibs-1.2.1a1-cp37-cp37m-manylinux1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvxslibs-1.2.0a1.tar", last modified: Sun May 14 15:50:35 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

