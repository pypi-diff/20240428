# Comparing `tmp/glabel-1.0.3.tar.gz` & `tmp/glabel-1.0.3b1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glabel-1.0.3.tar", last modified: Fri Apr 26 16:27:32 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

