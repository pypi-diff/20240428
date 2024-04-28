# Comparing `tmp/abess-0.4.7rc1.tar.gz` & `tmp/abess-0.4.8-cp311-cp311-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abess-0.4.7rc1.tar", last modified: Sat Aug  5 14:12:20 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

