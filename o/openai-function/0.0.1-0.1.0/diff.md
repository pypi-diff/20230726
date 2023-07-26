# Comparing `tmp/openai_function-0.0.1.tar.gz` & `tmp/openai_function-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_function-0.0.1.tar", max compression
+gzip compressed data, was "openai_function-0.1.0.tar", max compression
```

## Comparing `openai_function-0.0.1.tar` & `openai_function-0.1.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-07-26 09:25:07.990457 openai_function-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-07-26 09:25:07.990457 openai_function-0.0.1/openai_function/__init__.py
--rw-r--r--   0        0        0      336 2023-07-26 09:25:25.721704 openai_function-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      413 1970-01-01 00:00:00.000000 openai_function-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-26 09:19:51.461293 openai_function-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-26 09:19:51.461293 openai_function-0.1.0/openai_function/__init__.py
+-rw-r--r--   0        0        0      336 2023-07-26 09:20:16.627339 openai_function-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      413 1970-01-01 00:00:00.000000 openai_function-0.1.0/PKG-INFO
```

