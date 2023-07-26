# Comparing `tmp/coder_retriever-0.1.2.tar.gz` & `tmp/coder_retriever-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coder_retriever-0.1.2.tar", max compression
+gzip compressed data, was "coder_retriever-0.1.3.tar", max compression
```

## Comparing `coder_retriever-0.1.2.tar` & `coder_retriever-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       30 2023-07-25 07:44:46.520439 coder_retriever-0.1.2/coder_retriever/__init__.py
--rw-r--r--   0        0        0       40 2023-07-25 07:44:46.520439 coder_retriever-0.1.2/coder_retriever/ai/__init__.py
--rw-r--r--   0        0        0     4056 2023-07-25 08:15:22.524423 coder_retriever-0.1.2/coder_retriever/ai/assistant.py
--rw-r--r--   0        0        0     1088 2023-07-25 07:44:46.519440 coder_retriever-0.1.2/LICENSE
--rw-r--r--   0        0        0      630 2023-07-25 08:47:58.694204 coder_retriever-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      178 2023-07-25 07:44:46.519440 coder_retriever-0.1.2/README.md
--rw-r--r--   0        0        0      898 1970-01-01 00:00:00.000000 coder_retriever-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-21 08:21:50.647795 coder_retriever-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1577 2023-07-26 07:33:20.293166 coder_retriever-0.1.3/README.md
+-rw-r--r--   0        0        0       55 2023-07-26 07:33:20.293711 coder_retriever-0.1.3/coder_retriever/__init__.py
+-rw-r--r--   0        0        0       76 2023-07-26 07:33:20.294177 coder_retriever-0.1.3/coder_retriever/ai/__init__.py
+-rw-r--r--   0        0        0     5138 2023-07-26 07:33:20.294817 coder_retriever-0.1.3/coder_retriever/ai/assistant.py
+-rw-r--r--   0        0        0      625 2023-07-26 08:19:48.628977 coder_retriever-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2349 1970-01-01 00:00:00.000000 coder_retriever-0.1.3/PKG-INFO
```

