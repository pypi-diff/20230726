# Comparing `tmp/robokami-py-0.11.tar.gz` & `tmp/robokami_py-0.11.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robokami-py-0.11.tar", last modified: Wed Jul 12 17:43:57 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

