# Comparing `tmp/spatiafi-1.0.0.tar.gz` & `tmp/spatiafi-1.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatiafi-1.0.0.tar", last modified: Mon Jun 12 18:13:44 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

