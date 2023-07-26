# Comparing `tmp/pyaadhaar-1.1.3.tar.gz` & `tmp/pyaadhaar-2.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaadhaar-1.1.3.tar", last modified: Sat Apr  9 06:57:49 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

