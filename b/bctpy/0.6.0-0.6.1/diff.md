# Comparing `tmp/bctpy-0.6.0.tar.gz` & `tmp/bctpy-0.6.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bctpy-0.6.0.tar", last modified: Mon Dec  5 17:36:03 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

