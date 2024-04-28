# Comparing `tmp/mns-scheduler-1.0.3.5.tar.gz` & `tmp/mns_scheduler-1.0.3.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns-scheduler-1.0.3.5.tar", last modified: Sat Apr 27 03:58:43 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

