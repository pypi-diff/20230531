# Comparing `tmp/gl_client-0.1.6.tar.gz` & `tmp/gl_client-0.1.7-cp37-abi3-manylinux_2_27_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

