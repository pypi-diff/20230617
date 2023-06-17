# Comparing `tmp/pdf-docx-pic-0.0.0.tar.gz` & `tmp/pdf-docx-pic-3.0.0.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf-docx-pic-0.0.0.tar", last modified: Sat Jun 17 02:50:09 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

