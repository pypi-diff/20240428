# Comparing `tmp/SqlAddImage-1.0.0.tar.gz` & `tmp/SqlAddImage-1.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SqlAddImage-1.0.0.tar", last modified: Mon Apr  8 14:56:31 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

