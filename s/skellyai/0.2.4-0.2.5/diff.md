# Comparing `tmp/skellyai-0.2.4.tar.gz` & `tmp/skellyai-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/skellyai-0.2.4.tar", last modified: Wed Jul 12 20:59:24 2023, max compression
+gzip compressed data, was "dist/skellyai-0.2.5.tar", last modified: Wed Jul 26 04:01:21 2023, max compression
```

## Comparing `skellyai-0.2.4.tar` & `skellyai-0.2.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-07-12 20:59:24.516902 skellyai-0.2.4/
--rw-r--r--   0 bennicholl   (501) staff       (20)      407 2023-07-12 20:59:24.516470 skellyai-0.2.4/PKG-INFO
--rw-r--r--   0 bennicholl   (501) staff       (20)       38 2023-07-12 20:59:24.517067 skellyai-0.2.4/setup.cfg
--rw-r--r--   0 bennicholl   (501) staff       (20)      713 2023-07-12 20:20:19.000000 skellyai-0.2.4/setup.py
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-07-12 20:59:24.508735 skellyai-0.2.4/skellyai/
--rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.2.4/skellyai/__init__.py
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-07-12 20:59:24.513046 skellyai-0.2.4/skellyai/get_multi_labels/
--rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.2.4/skellyai/get_multi_labels/__init__.py
--rw-r--r--   0 bennicholl   (501) staff       (20)     1686 2023-05-19 20:23:21.000000 skellyai-0.2.4/skellyai/get_multi_labels/get_multi_labels.py
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-07-12 20:59:24.515767 skellyai-0.2.4/skellyai/perform_inference/
--rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.2.4/skellyai/perform_inference/__init__.py
--rw-r--r--   0 bennicholl   (501) staff       (20)      838 2023-06-09 19:43:52.000000 skellyai-0.2.4/skellyai/perform_inference/get_probs.py
--rw-r--r--   0 bennicholl   (501) staff       (20)     3092 2023-07-12 20:52:55.000000 skellyai-0.2.4/skellyai/perform_inference/get_probs_mult_keywords.py
--rw-r--r--   0 bennicholl   (501) staff       (20)      955 2023-07-12 20:55:20.000000 skellyai-0.2.4/skellyai/perform_inference/test.py
--rw-r--r--   0 bennicholl   (501) staff       (20)     3183 2023-05-18 18:08:51.000000 skellyai-0.2.4/skellyai/train_transformer.py
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-07-12 20:59:24.512145 skellyai-0.2.4/skellyai.egg-info/
--rw-r--r--   0 bennicholl   (501) staff       (20)      407 2023-07-12 20:59:24.000000 skellyai-0.2.4/skellyai.egg-info/PKG-INFO
--rw-r--r--   0 bennicholl   (501) staff       (20)      470 2023-07-12 20:59:24.000000 skellyai-0.2.4/skellyai.egg-info/SOURCES.txt
--rw-r--r--   0 bennicholl   (501) staff       (20)        1 2023-07-12 20:59:24.000000 skellyai-0.2.4/skellyai.egg-info/dependency_links.txt
--rw-r--r--   0 bennicholl   (501) staff       (20)       33 2023-07-12 20:59:24.000000 skellyai-0.2.4/skellyai.egg-info/requires.txt
--rw-r--r--   0 bennicholl   (501) staff       (20)       62 2023-07-12 20:59:24.000000 skellyai-0.2.4/skellyai.egg-info/top_level.txt
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-07-26 04:01:21.160641 skellyai-0.2.5/
+-rw-r--r--   0 bennicholl   (501) staff       (20)      407 2023-07-26 04:01:21.160152 skellyai-0.2.5/PKG-INFO
+-rw-r--r--   0 bennicholl   (501) staff       (20)       38 2023-07-26 04:01:21.160833 skellyai-0.2.5/setup.cfg
+-rw-r--r--   0 bennicholl   (501) staff       (20)      713 2023-07-26 03:59:44.000000 skellyai-0.2.5/setup.py
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-07-26 04:01:21.152650 skellyai-0.2.5/skellyai/
+-rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.2.5/skellyai/__init__.py
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-07-26 04:01:21.156513 skellyai-0.2.5/skellyai/get_multi_labels/
+-rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.2.5/skellyai/get_multi_labels/__init__.py
+-rw-r--r--   0 bennicholl   (501) staff       (20)     1686 2023-05-19 20:23:21.000000 skellyai-0.2.5/skellyai/get_multi_labels/get_multi_labels.py
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-07-26 04:01:21.159184 skellyai-0.2.5/skellyai/perform_inference/
+-rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.2.5/skellyai/perform_inference/__init__.py
+-rw-r--r--   0 bennicholl   (501) staff       (20)      838 2023-06-09 19:43:52.000000 skellyai-0.2.5/skellyai/perform_inference/get_probs.py
+-rw-r--r--   0 bennicholl   (501) staff       (20)     3092 2023-07-12 20:52:55.000000 skellyai-0.2.5/skellyai/perform_inference/get_probs_mult_keywords.py
+-rw-r--r--   0 bennicholl   (501) staff       (20)      955 2023-07-12 20:55:20.000000 skellyai-0.2.5/skellyai/perform_inference/test.py
+-rw-r--r--   0 bennicholl   (501) staff       (20)     3183 2023-05-18 18:08:51.000000 skellyai-0.2.5/skellyai/train_transformer.py
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-07-26 04:01:21.155721 skellyai-0.2.5/skellyai.egg-info/
+-rw-r--r--   0 bennicholl   (501) staff       (20)      407 2023-07-26 04:01:20.000000 skellyai-0.2.5/skellyai.egg-info/PKG-INFO
+-rw-r--r--   0 bennicholl   (501) staff       (20)      470 2023-07-26 04:01:21.000000 skellyai-0.2.5/skellyai.egg-info/SOURCES.txt
+-rw-r--r--   0 bennicholl   (501) staff       (20)        1 2023-07-26 04:01:20.000000 skellyai-0.2.5/skellyai.egg-info/dependency_links.txt
+-rw-r--r--   0 bennicholl   (501) staff       (20)       33 2023-07-26 04:01:20.000000 skellyai-0.2.5/skellyai.egg-info/requires.txt
+-rw-r--r--   0 bennicholl   (501) staff       (20)       62 2023-07-26 04:01:20.000000 skellyai-0.2.5/skellyai.egg-info/top_level.txt
```

### Comparing `skellyai-0.2.4/skellyai/get_multi_labels/get_multi_labels.py` & `skellyai-0.2.5/skellyai/get_multi_labels/get_multi_labels.py`

 * *Files identical despite different names*

### Comparing `skellyai-0.2.4/skellyai/perform_inference/get_probs.py` & `skellyai-0.2.5/skellyai/perform_inference/get_probs.py`

 * *Files identical despite different names*

### Comparing `skellyai-0.2.4/skellyai/perform_inference/get_probs_mult_keywords.py` & `skellyai-0.2.5/skellyai/perform_inference/get_probs_mult_keywords.py`

 * *Files identical despite different names*

### Comparing `skellyai-0.2.4/skellyai/perform_inference/test.py` & `skellyai-0.2.5/skellyai/perform_inference/test.py`

 * *Files identical despite different names*

### Comparing `skellyai-0.2.4/skellyai/train_transformer.py` & `skellyai-0.2.5/skellyai/train_transformer.py`

 * *Files identical despite different names*

