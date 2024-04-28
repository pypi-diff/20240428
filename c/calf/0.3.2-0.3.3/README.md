# Comparing `tmp/calf-0.3.2.tar.gz` & `tmp/calf-0.3.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/calf-0.3.2.tar", last modified: Sun Mar 15 15:27:48 2020, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

