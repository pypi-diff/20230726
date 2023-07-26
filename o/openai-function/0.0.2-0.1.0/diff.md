# Comparing `tmp/openai_function-0.0.2.tar.gz` & `tmp/openai_function-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_function-0.0.2.tar", max compression
+gzip compressed data, was "openai_function-0.1.0.tar", max compression
```

## Comparing `openai_function-0.0.2.tar` & `openai_function-0.1.0.tar`

### file list

```diff
@@ -1,6 +1,4 @@
--rw-r--r--   0        0        0        0 2023-07-26 09:25:07.990457 openai_function-0.0.2/README.md
--rw-r--r--   0        0        0       82 2023-07-26 09:55:24.966933 openai_function-0.0.2/openai_function/__init__.py
--rw-r--r--   0        0        0      873 2023-07-26 09:44:02.850227 openai_function-0.0.2/openai_function/chat_completion.py
--rw-r--r--   0        0        0     1871 2023-07-26 09:57:08.477737 openai_function-0.0.2/openai_function/functions.py
--rw-r--r--   0        0        0      408 2023-07-26 09:57:33.754352 openai_function-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      503 1970-01-01 00:00:00.000000 openai_function-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-26 09:19:51.461293 openai_function-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-26 09:19:51.461293 openai_function-0.1.0/openai_function/__init__.py
+-rw-r--r--   0        0        0      336 2023-07-26 09:20:16.627339 openai_function-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      413 1970-01-01 00:00:00.000000 openai_function-0.1.0/PKG-INFO
```

