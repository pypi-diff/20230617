# Comparing `tmp/yakinori-0.1.0.tar.gz` & `tmp/yakinori-0.1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yakinori-0.1.0.tar", last modified: Sat Jun 17 04:32:46 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

