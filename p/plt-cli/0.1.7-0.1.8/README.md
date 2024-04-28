# Comparing `tmp/plt-cli-0.1.7.tar.gz` & `tmp/plt_cli-0.1.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plt-cli-0.1.7.tar", last modified: Sun Feb 18 17:43:03 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

