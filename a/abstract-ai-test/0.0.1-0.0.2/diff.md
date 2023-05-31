# Comparing `tmp/abstract_ai_test-0.0.1.tar.gz` & `tmp/abstract_ai_test-0.0.2-py3.11.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_ai_test-0.0.1.tar", last modified: Tue May 30 23:49:30 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

