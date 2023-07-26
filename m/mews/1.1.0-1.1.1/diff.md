# Comparing `tmp/mews-1.1.0.tar.gz` & `tmp/mews-1.1.1-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mews-1.1.0.tar", last modified: Tue Feb 28 21:30:33 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

