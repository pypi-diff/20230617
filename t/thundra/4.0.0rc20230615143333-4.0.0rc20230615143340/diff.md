# Comparing `tmp/thundra-4.0.0rc20230615143333.tar.gz` & `tmp/thundra-4.0.0rc20230615143340-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thundra-4.0.0rc20230615143333.tar", last modified: Thu Jun 15 14:33:34 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

