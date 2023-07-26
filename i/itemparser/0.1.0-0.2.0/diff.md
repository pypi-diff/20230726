# Comparing `tmp/itemparser-0.1.0.tar.gz` & `tmp/itemparser-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itemparser-0.1.0.tar", max compression
+gzip compressed data, was "itemparser-0.2.0.tar", max compression
```

## Comparing `itemparser-0.1.0.tar` & `itemparser-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,7 @@
--rw-r--r--   0        0        0       12 2023-07-25 09:25:44.756449 itemparser-0.1.0/README.md
--rw-r--r--   0        0        0      332 2023-07-25 09:28:04.635762 itemparser-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-25 09:24:58.043197 itemparser-0.1.0/src/itemparser/__init__.py
--rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 itemparser-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       12 2023-07-26 03:43:21.765278 itemparser-0.2.0/README.md
+-rw-r--r--   0        0        0      407 2023-07-26 03:43:21.765278 itemparser-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      106 2023-07-26 03:43:21.765278 itemparser-0.2.0/src/itemparser/__init__.py
+-rw-r--r--   0        0        0     1490 2023-07-26 03:43:21.765278 itemparser-0.2.0/src/itemparser/field.py
+-rw-r--r--   0        0        0     2243 2023-07-26 03:43:21.765278 itemparser-0.2.0/src/itemparser/parser.py
+-rw-r--r--   0        0        0     3317 2023-07-26 03:43:21.765278 itemparser-0.2.0/src/itemparser/processor.py
+-rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 itemparser-0.2.0/PKG-INFO
```

