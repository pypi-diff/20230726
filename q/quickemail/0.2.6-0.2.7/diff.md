# Comparing `tmp/quickemail-0.2.6.tar.gz` & `tmp/quickemail-0.2.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\quickemail-0.2.6.tar", last modified: Tue Jul 25 07:55:45 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

