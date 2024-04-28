# Comparing `tmp/scorescanner-0.1.1.tar.gz` & `tmp/scorescanner-0.1.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scorescanner-0.1.1.tar", last modified: Mon Feb 12 22:43:50 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

