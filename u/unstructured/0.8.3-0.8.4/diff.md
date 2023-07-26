# Comparing `tmp/unstructured-0.8.3.tar.gz` & `tmp/unstructured-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured-0.8.3.tar", last modified: Wed Jul 26 14:54:16 2023, max compression
+gzip compressed data, was "unstructured-0.8.4.tar", last modified: Wed Jul 26 18:24:21 2023, max compression
```

## Comparing `unstructured-0.8.3.tar` & `unstructured-0.8.4.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:54:16.892879 unstructured-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-26 14:54:07.000000 unstructured-0.8.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-26 14:54:07.000000 unstructured-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20030 2023-07-26 14:54:16.892879 unstructured-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16273 2023-07-26 14:54:07.000000 unstructured-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:54:16.876879 unstructured-0.8.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-26 14:54:07.000000 unstructured-0.8.3/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 14:54:07.000000 unstructured-0.8.3/requirements/huggingface.in
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-26 14:54:07.000000 unstructured-0.8.3/requirements/ingest-azure.in
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-26 14:54:07.000000 unstructured-0.8.3/requirements/ingest-discord.in
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-26 14:54:07.000000 unstructured-0.8.3/requirements/ingest-dropbox.in
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-26 14:54:07.000000 unstructured-0.8.3/requirements/ingest-gcs.in
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-26 14:54:07.000000 unstructured-0.8.3/requirements/ingest-github.in
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-26 14:54:07.000000 unstructured-0.8.3/requirements/ingest-gitlab.in
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-26 14:54:07.000000 unstructured-0.8.3/requirements/ingest-google-drive.in
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 14:54:07.000000 unstructured-0.8.3/requirements/ingest-onedrive.in
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 14:54:07.000000 unstructured-0.8.3/requirements/ingest-outlook.in
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-26 14:54:07.000000 unstructured-0.8.3/requirements/ingest-reddit.in
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-26 14:54:07.000000 unstructured-0.8.3/requirements/ingest-s3.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-26 14:54:07.000000 unstructured-0.8.3/requirements/ingest-slack.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-26 14:54:07.000000 unstructured-0.8.3/requirements/ingest-wikipedia.in
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-26 14:54:07.000000 unstructured-0.8.3/requirements/local-inference.in
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-26 14:54:16.892879 unstructured-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-26 14:54:07.000000 unstructured-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:54:16.876879 unstructured-0.8.3/test_unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:54:07.000000 unstructured-0.8.3/test_unstructured/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:54:16.876879 unstructured-0.8.3/test_unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:54:07.000000 unstructured-0.8.3/test_unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-26 14:54:07.000000 unstructured-0.8.3/test_unstructured/nlp/mock_nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-26 14:54:07.000000 unstructured-0.8.3/test_unstructured/nlp/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-26 14:54:07.000000 unstructured-0.8.3/test_unstructured/nlp/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-26 14:54:07.000000 unstructured-0.8.3/test_unstructured/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:54:16.876879 unstructured-0.8.3/unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:54:16.880879 unstructured-0.8.3/unstructured/cleaners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/cleaners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/cleaners/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/cleaners/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/cleaners/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:54:16.880879 unstructured-0.8.3/unstructured/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/documents/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/documents/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/documents/email_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/documents/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/documents/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:54:16.880879 unstructured-0.8.3/unstructured/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/file_utils/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/file_utils/exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/file_utils/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    20069 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/file_utils/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/file_utils/google_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/file_utils/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:54:16.880879 unstructured-0.8.3/unstructured/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:54:16.880879 unstructured-0.8.3/unstructured/ingest/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/ingest/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/ingest/connector/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/ingest/connector/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/ingest/connector/confluence.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/ingest/connector/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/ingest/connector/dropbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/ingest/connector/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/ingest/connector/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/ingest/connector/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/ingest/connector/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/ingest/connector/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/ingest/connector/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/ingest/connector/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/ingest/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/ingest/connector/onedrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/ingest/connector/outlook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/ingest/connector/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/ingest/connector/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/ingest/connector/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/ingest/connector/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:54:16.884879 unstructured-0.8.3/unstructured/ingest/doc_processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/ingest/doc_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/ingest/doc_processor/generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/ingest/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/ingest/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33906 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/ingest/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:54:16.884879 unstructured-0.8.3/unstructured/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:54:16.888879 unstructured-0.8.3/unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/nlp/english-words.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/nlp/english_words.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/nlp/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/nlp/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/nlp/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:54:16.888879 unstructured-0.8.3/unstructured/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/partition/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10611 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/partition/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/partition/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/partition/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/partition/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11798 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/partition/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)    14262 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/partition/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/partition/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/partition/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/partition/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/partition/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/partition/md.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/partition/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/partition/odt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/partition/org.py
--rw-r--r--   0 runner    (1001) docker     (123)    15851 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/partition/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/partition/ppt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/partition/pptx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/partition/rst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/partition/rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/partition/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     9835 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/partition/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/partition/text_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/partition/tsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/partition/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/partition/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:54:16.892879 unstructured-0.8.3/unstructured/staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/staging/argilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/staging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/staging/baseplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/staging/datasaur.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/staging/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/staging/label_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/staging/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/staging/prodigy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/staging/weaviate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-26 14:54:07.000000 unstructured-0.8.3/unstructured/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:54:16.880879 unstructured-0.8.3/unstructured.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20030 2023-07-26 14:54:16.000000 unstructured-0.8.3/unstructured.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-26 14:54:16.000000 unstructured-0.8.3/unstructured.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:54:16.000000 unstructured-0.8.3/unstructured.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 14:54:16.000000 unstructured-0.8.3/unstructured.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-26 14:54:16.000000 unstructured-0.8.3/unstructured.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-26 14:54:16.000000 unstructured-0.8.3/unstructured.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.186249 unstructured-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-26 18:24:08.000000 unstructured-0.8.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-26 18:24:08.000000 unstructured-0.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20030 2023-07-26 18:24:21.186249 unstructured-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16273 2023-07-26 18:24:08.000000 unstructured-0.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.158249 unstructured-0.8.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/huggingface.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/ingest-azure.in
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/ingest-discord.in
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/ingest-dropbox.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/ingest-gcs.in
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/ingest-github.in
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/ingest-gitlab.in
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/ingest-google-drive.in
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/ingest-onedrive.in
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/ingest-outlook.in
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/ingest-reddit.in
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/ingest-s3.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/ingest-slack.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/ingest-wikipedia.in
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/local-inference.in
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-26 18:24:21.186249 unstructured-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-26 18:24:08.000000 unstructured-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.158249 unstructured-0.8.4/test_unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:08.000000 unstructured-0.8.4/test_unstructured/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.158249 unstructured-0.8.4/test_unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:08.000000 unstructured-0.8.4/test_unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-26 18:24:08.000000 unstructured-0.8.4/test_unstructured/nlp/mock_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-26 18:24:08.000000 unstructured-0.8.4/test_unstructured/nlp/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-26 18:24:08.000000 unstructured-0.8.4/test_unstructured/nlp/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-26 18:24:08.000000 unstructured-0.8.4/test_unstructured/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.158249 unstructured-0.8.4/unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.162248 unstructured-0.8.4/unstructured/cleaners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/cleaners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/cleaners/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/cleaners/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/cleaners/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.162248 unstructured-0.8.4/unstructured/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/documents/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/documents/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/documents/email_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/documents/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/documents/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.162248 unstructured-0.8.4/unstructured/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/file_utils/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/file_utils/exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/file_utils/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20069 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/file_utils/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/file_utils/google_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/file_utils/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.162248 unstructured-0.8.4/unstructured/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.166248 unstructured-0.8.4/unstructured/ingest/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/confluence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/onedrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/outlook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.166248 unstructured-0.8.4/unstructured/ingest/doc_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/doc_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/doc_processor/generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33906 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.166248 unstructured-0.8.4/unstructured/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.178249 unstructured-0.8.4/unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/nlp/english-words.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/nlp/english_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/nlp/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/nlp/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/nlp/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.182249 unstructured-0.8.4/unstructured/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10611 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11798 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14262 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/odt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/org.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15851 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9835 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/text_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/tsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.186249 unstructured-0.8.4/unstructured/staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/staging/argilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/staging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/staging/baseplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/staging/datasaur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/staging/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/staging/label_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/staging/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/staging/prodigy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/staging/weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.162248 unstructured-0.8.4/unstructured.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20030 2023-07-26 18:24:20.000000 unstructured-0.8.4/unstructured.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-26 18:24:21.000000 unstructured-0.8.4/unstructured.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:24:20.000000 unstructured-0.8.4/unstructured.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 18:24:20.000000 unstructured-0.8.4/unstructured.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-26 18:24:20.000000 unstructured-0.8.4/unstructured.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-26 18:24:20.000000 unstructured-0.8.4/unstructured.egg-info/top_level.txt
```

### Comparing `unstructured-0.8.3/LICENSE.md` & `unstructured-0.8.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/MANIFEST.in` & `unstructured-0.8.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/PKG-INFO` & `unstructured-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.8.3
+Version: 0.8.4
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.8.3 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.8.4 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
```

### Comparing `unstructured-0.8.3/README.md` & `unstructured-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/setup.py` & `unstructured-0.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/test_unstructured/nlp/mock_nltk.py` & `unstructured-0.8.4/test_unstructured/nlp/mock_nltk.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/test_unstructured/nlp/test_tokenize.py` & `unstructured-0.8.4/test_unstructured/nlp/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/test_unstructured/test_utils.py` & `unstructured-0.8.4/test_unstructured/test_utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/cleaners/core.py` & `unstructured-0.8.4/unstructured/cleaners/core.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/cleaners/extract.py` & `unstructured-0.8.4/unstructured/cleaners/extract.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/cleaners/translate.py` & `unstructured-0.8.4/unstructured/cleaners/translate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/documents/base.py` & `unstructured-0.8.4/unstructured/documents/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/documents/coordinates.py` & `unstructured-0.8.4/unstructured/documents/coordinates.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/documents/elements.py` & `unstructured-0.8.4/unstructured/documents/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/documents/email_elements.py` & `unstructured-0.8.4/unstructured/documents/email_elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/documents/html.py` & `unstructured-0.8.4/unstructured/documents/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/documents/xml.py` & `unstructured-0.8.4/unstructured/documents/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/file_utils/encoding.py` & `unstructured-0.8.4/unstructured/file_utils/encoding.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/file_utils/exploration.py` & `unstructured-0.8.4/unstructured/file_utils/exploration.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/file_utils/file_conversion.py` & `unstructured-0.8.4/unstructured/file_utils/file_conversion.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/file_utils/filetype.py` & `unstructured-0.8.4/unstructured/file_utils/filetype.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/file_utils/metadata.py` & `unstructured-0.8.4/unstructured/file_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/ingest/connector/azure.py` & `unstructured-0.8.4/unstructured/ingest/connector/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/ingest/connector/biomed.py` & `unstructured-0.8.4/unstructured/ingest/connector/biomed.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/ingest/connector/confluence.py` & `unstructured-0.8.4/unstructured/ingest/connector/confluence.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/ingest/connector/discord.py` & `unstructured-0.8.4/unstructured/ingest/connector/discord.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/ingest/connector/dropbox.py` & `unstructured-0.8.4/unstructured/ingest/connector/dropbox.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/ingest/connector/elasticsearch.py` & `unstructured-0.8.4/unstructured/ingest/connector/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/ingest/connector/fsspec.py` & `unstructured-0.8.4/unstructured/ingest/connector/fsspec.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/ingest/connector/gcs.py` & `unstructured-0.8.4/unstructured/ingest/connector/gcs.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/ingest/connector/git.py` & `unstructured-0.8.4/unstructured/ingest/connector/git.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/ingest/connector/github.py` & `unstructured-0.8.4/unstructured/ingest/connector/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/ingest/connector/gitlab.py` & `unstructured-0.8.4/unstructured/ingest/connector/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/ingest/connector/google_drive.py` & `unstructured-0.8.4/unstructured/ingest/connector/google_drive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/ingest/connector/local.py` & `unstructured-0.8.4/unstructured/ingest/connector/local.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/ingest/connector/onedrive.py` & `unstructured-0.8.4/unstructured/ingest/connector/onedrive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/ingest/connector/outlook.py` & `unstructured-0.8.4/unstructured/ingest/connector/outlook.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/ingest/connector/reddit.py` & `unstructured-0.8.4/unstructured/ingest/connector/reddit.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/ingest/connector/s3.py` & `unstructured-0.8.4/unstructured/ingest/connector/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/ingest/connector/slack.py` & `unstructured-0.8.4/unstructured/ingest/connector/slack.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/ingest/connector/wikipedia.py` & `unstructured-0.8.4/unstructured/ingest/connector/wikipedia.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/ingest/doc_processor/generalized.py` & `unstructured-0.8.4/unstructured/ingest/doc_processor/generalized.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/ingest/interfaces.py` & `unstructured-0.8.4/unstructured/ingest/interfaces.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/ingest/main.py` & `unstructured-0.8.4/unstructured/ingest/main.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/nlp/english-words.txt` & `unstructured-0.8.4/unstructured/nlp/english-words.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/nlp/english_words.py` & `unstructured-0.8.4/unstructured/nlp/english_words.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/nlp/patterns.py` & `unstructured-0.8.4/unstructured/nlp/patterns.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/nlp/tokenize.py` & `unstructured-0.8.4/unstructured/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/partition/__init__.py` & `unstructured-0.8.4/unstructured/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/partition/api.py` & `unstructured-0.8.4/unstructured/partition/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,18 +49,14 @@
     exactly_one(filename=filename, file=file)
 
     headers = {
         "ACCEPT": "application/json",
         "UNSTRUCTURED-API-KEY": api_key,
     }
 
-    # set default values for kwargs
-    strategy = request_kwargs.pop("strategy", "hi_res")
-    request_kwargs["strategy"] = strategy
-
     if filename is not None:
         with open(filename, "rb") as f:
             files = [
                 ("files", (filename, f, content_type)),
             ]
             response = requests.post(
                 api_url,
@@ -114,35 +110,27 @@
         A list of strings defining the target filename paths.
     content_types
         A list of strings defining the file contents in MIME types.
     files
         A list of file-like object using "rb" mode --> open(filename, "rb").
     file_filename
         When file is not None, the filename (string) to store in element metadata. E.g. "foo.txt"
-    strategy
-        The strategy to use for partitioning the PDF. Uses a layout detection model if set
-        to 'hi_res', otherwise partition_pdf simply extracts the text from the document
-        and processes it.
     api_url
         The URL for the Unstructured API. Defaults to the hosted Unstructured API.
     api_key
         The API key to pass to the Unstructured API.
     request_kwargs
         Additional parameters to pass to the data field of the request to the Unstructured API.
         For example the `strategy` parameter.
     """
     headers = {
         "ACCEPT": "application/json",
         "UNSTRUCTURED-API-KEY": api_key,
     }
 
-    # set default values for kwargs
-    strategy = request_kwargs.pop("strategy", "hi_res")
-    request_kwargs["strategy"] = strategy
-
     if filenames is not None:
         if content_types and len(content_types) != len(filenames):
             raise ValueError("content_types and filenames must have the same length.")
 
         with contextlib.ExitStack() as stack:
             files = [stack.enter_context(open(f, "rb")) for f in filenames]  # type: ignore
```

### Comparing `unstructured-0.8.3/unstructured/partition/auto.py` & `unstructured-0.8.4/unstructured/partition/auto.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/partition/common.py` & `unstructured-0.8.4/unstructured/partition/common.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/partition/csv.py` & `unstructured-0.8.4/unstructured/partition/csv.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/partition/doc.py` & `unstructured-0.8.4/unstructured/partition/doc.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/partition/docx.py` & `unstructured-0.8.4/unstructured/partition/docx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/partition/email.py` & `unstructured-0.8.4/unstructured/partition/email.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/partition/epub.py` & `unstructured-0.8.4/unstructured/partition/epub.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/partition/html.py` & `unstructured-0.8.4/unstructured/partition/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/partition/image.py` & `unstructured-0.8.4/unstructured/partition/image.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/partition/json.py` & `unstructured-0.8.4/unstructured/partition/json.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/partition/md.py` & `unstructured-0.8.4/unstructured/partition/md.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/partition/msg.py` & `unstructured-0.8.4/unstructured/partition/msg.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/partition/odt.py` & `unstructured-0.8.4/unstructured/partition/odt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/partition/org.py` & `unstructured-0.8.4/unstructured/partition/org.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/partition/pdf.py` & `unstructured-0.8.4/unstructured/partition/pdf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/partition/ppt.py` & `unstructured-0.8.4/unstructured/partition/ppt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/partition/pptx.py` & `unstructured-0.8.4/unstructured/partition/pptx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/partition/rst.py` & `unstructured-0.8.4/unstructured/partition/rst.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/partition/rtf.py` & `unstructured-0.8.4/unstructured/partition/rtf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/partition/strategies.py` & `unstructured-0.8.4/unstructured/partition/strategies.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/partition/text.py` & `unstructured-0.8.4/unstructured/partition/text.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/partition/text_type.py` & `unstructured-0.8.4/unstructured/partition/text_type.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/partition/tsv.py` & `unstructured-0.8.4/unstructured/partition/tsv.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/partition/xlsx.py` & `unstructured-0.8.4/unstructured/partition/xlsx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/partition/xml.py` & `unstructured-0.8.4/unstructured/partition/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/staging/argilla.py` & `unstructured-0.8.4/unstructured/staging/argilla.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/staging/base.py` & `unstructured-0.8.4/unstructured/staging/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/staging/baseplate.py` & `unstructured-0.8.4/unstructured/staging/baseplate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/staging/datasaur.py` & `unstructured-0.8.4/unstructured/staging/datasaur.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/staging/huggingface.py` & `unstructured-0.8.4/unstructured/staging/huggingface.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/staging/label_box.py` & `unstructured-0.8.4/unstructured/staging/label_box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/staging/label_studio.py` & `unstructured-0.8.4/unstructured/staging/label_studio.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/staging/prodigy.py` & `unstructured-0.8.4/unstructured/staging/prodigy.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/staging/weaviate.py` & `unstructured-0.8.4/unstructured/staging/weaviate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured/utils.py` & `unstructured-0.8.4/unstructured/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured.egg-info/PKG-INFO` & `unstructured-0.8.4/unstructured.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.8.3
+Version: 0.8.4
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.8.3 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.8.4 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
```

### Comparing `unstructured-0.8.3/unstructured.egg-info/SOURCES.txt` & `unstructured-0.8.4/unstructured.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.3/unstructured.egg-info/requires.txt` & `unstructured-0.8.4/unstructured.egg-info/requires.txt`

 * *Files identical despite different names*

