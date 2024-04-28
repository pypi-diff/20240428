# Comparing `tmp/allopy-0.1.5.tar.gz` & `tmp/allopy-0.2.0-pp39-pypy39_pp73-manylinux_2_28_x86_64.whl.zip`

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

