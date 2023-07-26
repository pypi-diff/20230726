# Comparing `tmp/nikl-corpus-io-0.0.1.tar.gz` & `tmp/nikl-corpus-io-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nikl-corpus-io-0.0.1.tar", last modified: Wed Jul 26 07:37:18 2023, max compression
+gzip compressed data, was "nikl-corpus-io-0.0.2.tar", last modified: Wed Jul 26 08:35:16 2023, max compression
```

## Comparing `nikl-corpus-io-0.0.1.tar` & `nikl-corpus-io-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 postbg     (501) staff       (20)        0 2023-07-26 07:37:18.083266 nikl-corpus-io-0.0.1/
--rw-r--r--   0 postbg     (501) staff       (20)     1062 2023-07-26 07:17:56.000000 nikl-corpus-io-0.0.1/LICENSE.txt
--rw-r--r--   0 postbg     (501) staff       (20)      560 2023-07-26 07:37:18.082736 nikl-corpus-io-0.0.1/PKG-INFO
--rw-r--r--   0 postbg     (501) staff       (20)       46 2023-07-26 07:24:45.000000 nikl-corpus-io-0.0.1/README.md
--rw-r--r--   0 postbg     (501) staff       (20)      105 2023-07-26 07:22:53.000000 nikl-corpus-io-0.0.1/pyproject.toml
--rw-r--r--   0 postbg     (501) staff       (20)       38 2023-07-26 07:37:18.083417 nikl-corpus-io-0.0.1/setup.cfg
--rw-r--r--   0 postbg     (501) staff       (20)      809 2023-07-26 07:36:19.000000 nikl-corpus-io-0.0.1/setup.py
-drwxr-xr-x   0 postbg     (501) staff       (20)        0 2023-07-26 07:37:18.070100 nikl-corpus-io-0.0.1/src/
-drwxr-xr-x   0 postbg     (501) staff       (20)        0 2023-07-26 07:37:18.073034 nikl-corpus-io-0.0.1/src/commons/
--rw-r--r--   0 postbg     (501) staff       (20)        0 2023-07-19 06:36:15.000000 nikl-corpus-io-0.0.1/src/commons/__init__.py
--rw-r--r--   0 postbg     (501) staff       (20)      952 2023-07-25 02:46:13.000000 nikl-corpus-io-0.0.1/src/commons/json_services.py
--rw-r--r--   0 postbg     (501) staff       (20)      163 2023-07-19 07:21:26.000000 nikl-corpus-io-0.0.1/src/commons/utils.py
-drwxr-xr-x   0 postbg     (501) staff       (20)        0 2023-07-26 07:37:18.074005 nikl-corpus-io-0.0.1/src/file_io/
--rw-r--r--   0 postbg     (501) staff       (20)        0 2023-07-24 09:22:00.000000 nikl-corpus-io-0.0.1/src/file_io/__init__.py
--rw-r--r--   0 postbg     (501) staff       (20)     1330 2023-07-26 04:51:00.000000 nikl-corpus-io-0.0.1/src/file_io/morphemes_io.py
-drwxr-xr-x   0 postbg     (501) staff       (20)        0 2023-07-26 07:37:18.075237 nikl-corpus-io-0.0.1/src/nikl/
--rw-r--r--   0 postbg     (501) staff       (20)       60 2023-07-26 07:33:05.000000 nikl-corpus-io-0.0.1/src/nikl/__init__.py
--rw-r--r--   0 postbg     (501) staff       (20)     1159 2023-07-26 04:57:54.000000 nikl-corpus-io-0.0.1/src/nikl/abc.py
-drwxr-xr-x   0 postbg     (501) staff       (20)        0 2023-07-26 07:37:18.076404 nikl-corpus-io-0.0.1/src/nikl/commons/
--rw-r--r--   0 postbg     (501) staff       (20)        0 2023-07-25 02:24:23.000000 nikl-corpus-io-0.0.1/src/nikl/commons/__init__.py
--rw-r--r--   0 postbg     (501) staff       (20)      747 2023-07-24 09:16:42.000000 nikl-corpus-io-0.0.1/src/nikl/commons/mappers.py
-drwxr-xr-x   0 postbg     (501) staff       (20)        0 2023-07-26 07:37:18.077440 nikl-corpus-io-0.0.1/src/nikl/newspapers/
--rw-r--r--   0 postbg     (501) staff       (20)        0 2023-07-19 06:36:03.000000 nikl-corpus-io-0.0.1/src/nikl/newspapers/__init__.py
--rw-r--r--   0 postbg     (501) staff       (20)      164 2023-07-26 04:57:54.000000 nikl-corpus-io-0.0.1/src/nikl/newspapers/services.py
-drwxr-xr-x   0 postbg     (501) staff       (20)        0 2023-07-26 07:37:18.078494 nikl-corpus-io-0.0.1/src/nikl/usecases/
--rw-r--r--   0 postbg     (501) staff       (20)        0 2023-07-25 03:06:49.000000 nikl-corpus-io-0.0.1/src/nikl/usecases/__init__.py
--rw-r--r--   0 postbg     (501) staff       (20)     1488 2023-07-26 04:57:54.000000 nikl-corpus-io-0.0.1/src/nikl/usecases/corpus_merge_usecase.py
-drwxr-xr-x   0 postbg     (501) staff       (20)        0 2023-07-26 07:37:18.079481 nikl-corpus-io-0.0.1/src/nikl/written/
--rw-r--r--   0 postbg     (501) staff       (20)        0 2023-07-24 16:40:28.000000 nikl-corpus-io-0.0.1/src/nikl/written/__init__.py
--rw-r--r--   0 postbg     (501) staff       (20)      160 2023-07-26 04:57:54.000000 nikl-corpus-io-0.0.1/src/nikl/written/services.py
-drwxr-xr-x   0 postbg     (501) staff       (20)        0 2023-07-26 07:37:18.081988 nikl-corpus-io-0.0.1/src/nikl_corpus_io.egg-info/
--rw-r--r--   0 postbg     (501) staff       (20)      560 2023-07-26 07:37:18.000000 nikl-corpus-io-0.0.1/src/nikl_corpus_io.egg-info/PKG-INFO
--rw-r--r--   0 postbg     (501) staff       (20)      627 2023-07-26 07:37:18.000000 nikl-corpus-io-0.0.1/src/nikl_corpus_io.egg-info/SOURCES.txt
--rw-r--r--   0 postbg     (501) staff       (20)        1 2023-07-26 07:37:18.000000 nikl-corpus-io-0.0.1/src/nikl_corpus_io.egg-info/dependency_links.txt
--rw-r--r--   0 postbg     (501) staff       (20)       21 2023-07-26 07:37:18.000000 nikl-corpus-io-0.0.1/src/nikl_corpus_io.egg-info/top_level.txt
+drwxr-xr-x   0 postbg     (501) staff       (20)        0 2023-07-26 08:35:16.537537 nikl-corpus-io-0.0.2/
+-rw-r--r--   0 postbg     (501) staff       (20)     1062 2023-07-26 07:17:56.000000 nikl-corpus-io-0.0.2/LICENSE.txt
+-rw-r--r--   0 postbg     (501) staff       (20)      560 2023-07-26 08:35:16.537227 nikl-corpus-io-0.0.2/PKG-INFO
+-rw-r--r--   0 postbg     (501) staff       (20)       46 2023-07-26 07:24:45.000000 nikl-corpus-io-0.0.2/README.md
+drwxr-xr-x   0 postbg     (501) staff       (20)        0 2023-07-26 08:35:16.527058 nikl-corpus-io-0.0.2/corpus_io/
+-rw-r--r--   0 postbg     (501) staff       (20)        0 2023-07-26 07:28:32.000000 nikl-corpus-io-0.0.2/corpus_io/__init__.py
+drwxr-xr-x   0 postbg     (501) staff       (20)        0 2023-07-26 08:35:16.528616 nikl-corpus-io-0.0.2/corpus_io/commons/
+-rw-r--r--   0 postbg     (501) staff       (20)        0 2023-07-19 06:36:15.000000 nikl-corpus-io-0.0.2/corpus_io/commons/__init__.py
+-rw-r--r--   0 postbg     (501) staff       (20)      952 2023-07-25 02:46:13.000000 nikl-corpus-io-0.0.2/corpus_io/commons/json_services.py
+-rw-r--r--   0 postbg     (501) staff       (20)      163 2023-07-19 07:21:26.000000 nikl-corpus-io-0.0.2/corpus_io/commons/utils.py
+drwxr-xr-x   0 postbg     (501) staff       (20)        0 2023-07-26 08:35:16.529539 nikl-corpus-io-0.0.2/corpus_io/file_io/
+-rw-r--r--   0 postbg     (501) staff       (20)        0 2023-07-24 09:22:00.000000 nikl-corpus-io-0.0.2/corpus_io/file_io/__init__.py
+-rw-r--r--   0 postbg     (501) staff       (20)     1350 2023-07-26 08:29:53.000000 nikl-corpus-io-0.0.2/corpus_io/file_io/morphemes_io.py
+-rw-r--r--   0 postbg     (501) staff       (20)      629 2023-07-24 16:33:51.000000 nikl-corpus-io-0.0.2/corpus_io/morphemes.py
+drwxr-xr-x   0 postbg     (501) staff       (20)        0 2023-07-26 08:35:16.530863 nikl-corpus-io-0.0.2/corpus_io/nikl/
+-rw-r--r--   0 postbg     (501) staff       (20)       66 2023-07-26 08:29:53.000000 nikl-corpus-io-0.0.2/corpus_io/nikl/__init__.py
+-rw-r--r--   0 postbg     (501) staff       (20)     1189 2023-07-26 08:29:53.000000 nikl-corpus-io-0.0.2/corpus_io/nikl/abc.py
+drwxr-xr-x   0 postbg     (501) staff       (20)        0 2023-07-26 08:35:16.531808 nikl-corpus-io-0.0.2/corpus_io/nikl/commons/
+-rw-r--r--   0 postbg     (501) staff       (20)        0 2023-07-25 02:24:23.000000 nikl-corpus-io-0.0.2/corpus_io/nikl/commons/__init__.py
+-rw-r--r--   0 postbg     (501) staff       (20)      757 2023-07-26 08:29:53.000000 nikl-corpus-io-0.0.2/corpus_io/nikl/commons/mappers.py
+drwxr-xr-x   0 postbg     (501) staff       (20)        0 2023-07-26 08:35:16.532727 nikl-corpus-io-0.0.2/corpus_io/nikl/newspapers/
+-rw-r--r--   0 postbg     (501) staff       (20)        0 2023-07-19 06:36:03.000000 nikl-corpus-io-0.0.2/corpus_io/nikl/newspapers/__init__.py
+-rw-r--r--   0 postbg     (501) staff       (20)      174 2023-07-26 08:29:53.000000 nikl-corpus-io-0.0.2/corpus_io/nikl/newspapers/services.py
+drwxr-xr-x   0 postbg     (501) staff       (20)        0 2023-07-26 08:35:16.533728 nikl-corpus-io-0.0.2/corpus_io/nikl/usecases/
+-rw-r--r--   0 postbg     (501) staff       (20)        0 2023-07-25 03:06:49.000000 nikl-corpus-io-0.0.2/corpus_io/nikl/usecases/__init__.py
+-rw-r--r--   0 postbg     (501) staff       (20)     1512 2023-07-26 08:29:53.000000 nikl-corpus-io-0.0.2/corpus_io/nikl/usecases/corpus_merge_usecase.py
+drwxr-xr-x   0 postbg     (501) staff       (20)        0 2023-07-26 08:35:16.534762 nikl-corpus-io-0.0.2/corpus_io/nikl/written/
+-rw-r--r--   0 postbg     (501) staff       (20)        0 2023-07-24 16:40:28.000000 nikl-corpus-io-0.0.2/corpus_io/nikl/written/__init__.py
+-rw-r--r--   0 postbg     (501) staff       (20)      170 2023-07-26 08:29:53.000000 nikl-corpus-io-0.0.2/corpus_io/nikl/written/services.py
+drwxr-xr-x   0 postbg     (501) staff       (20)        0 2023-07-26 08:35:16.536656 nikl-corpus-io-0.0.2/nikl_corpus_io.egg-info/
+-rw-r--r--   0 postbg     (501) staff       (20)      560 2023-07-26 08:35:16.000000 nikl-corpus-io-0.0.2/nikl_corpus_io.egg-info/PKG-INFO
+-rw-r--r--   0 postbg     (501) staff       (20)      746 2023-07-26 08:35:16.000000 nikl-corpus-io-0.0.2/nikl_corpus_io.egg-info/SOURCES.txt
+-rw-r--r--   0 postbg     (501) staff       (20)        1 2023-07-26 08:35:16.000000 nikl-corpus-io-0.0.2/nikl_corpus_io.egg-info/dependency_links.txt
+-rw-r--r--   0 postbg     (501) staff       (20)       10 2023-07-26 08:35:16.000000 nikl-corpus-io-0.0.2/nikl_corpus_io.egg-info/top_level.txt
+-rw-r--r--   0 postbg     (501) staff       (20)      105 2023-07-26 07:22:53.000000 nikl-corpus-io-0.0.2/pyproject.toml
+-rw-r--r--   0 postbg     (501) staff       (20)       38 2023-07-26 08:35:16.537626 nikl-corpus-io-0.0.2/setup.cfg
+-rw-r--r--   0 postbg     (501) staff       (20)      769 2023-07-26 08:35:05.000000 nikl-corpus-io-0.0.2/setup.py
```

### Comparing `nikl-corpus-io-0.0.1/LICENSE.txt` & `nikl-corpus-io-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nikl-corpus-io-0.0.1/PKG-INFO` & `nikl-corpus-io-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nikl-corpus-io
-Version: 0.0.1
+Version: 0.0.2
 Summary: Read/write nikl corpus
 Home-page: https://github.com/re-writers/corpusIO.python
 Author: postBG
 Author-email: profile2697@gmail.com
 Project-URL: Bug Tracker, https://github.com/re-writers/corpusIO.python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nikl-corpus-io-0.0.1/setup.py` & `nikl-corpus-io-0.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nikl-corpus-io",
-    version="0.0.1",
+    version="0.0.2",
     author="postBG",
     author_email="profile2697@gmail.com",
     description="Read/write nikl corpus",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/re-writers/corpusIO.python",
     project_urls={
         "Bug Tracker": "https://github.com/re-writers/corpusIO.python/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    package_dir={"": "src"},
-    packages=setuptools.find_packages(where="src"),
+    packages=setuptools.find_packages(),
     python_requires=">=3.8",
 )
```

### Comparing `nikl-corpus-io-0.0.1/src/commons/json_services.py` & `nikl-corpus-io-0.0.2/corpus_io/commons/json_services.py`

 * *Files identical despite different names*

### Comparing `nikl-corpus-io-0.0.1/src/file_io/morphemes_io.py` & `nikl-corpus-io-0.0.2/corpus_io/file_io/morphemes_io.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from tqdm import tqdm
 
-from morphemes import Morpheme
-from nikl.abc import TOKENIZED_SENT_GEN_TYPE
+from corpus_io.morphemes import Morpheme
+from corpus_io.nikl.abc import TOKENIZED_SENT_GEN_TYPE
 
 SENT_MORPHEME_SEP = "__SEN|||MOR__"
 MORPHEME_SEP = "__ML|||MR__"
 
 
 def convert_morpheme_stream_to_writable_format(morpheme_stream):
     for sentence, morphemes in morpheme_stream:
```

### Comparing `nikl-corpus-io-0.0.1/src/nikl/abc.py` & `nikl-corpus-io-0.0.2/corpus_io/nikl/abc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import abc
 from inspect import isabstract
 from typing import Iterator, Tuple, List
 
-from commons.json_services import JsonLoadService
-from morphemes import Morpheme
-from nikl.commons.mappers import extract_sentences_as_stream_from, tokenize_to_morphemes
+from corpus_io.commons.json_services import JsonLoadService
+from corpus_io.morphemes import Morpheme
+from corpus_io.nikl.commons.mappers import extract_sentences_as_stream_from, tokenize_to_morphemes
 
 TOKENIZED_SENT_GEN_TYPE = Iterator[Tuple[str, List[Morpheme]]]
 
 
 class NIKLTokenizeIOService(abc.ABC):
     registered_subclasses = {}
```

### Comparing `nikl-corpus-io-0.0.1/src/nikl/commons/mappers.py` & `nikl-corpus-io-0.0.2/corpus_io/nikl/commons/mappers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Iterable
 from kiwipiepy import Kiwi
 
-from morphemes import Morpheme
+from corpus_io.morphemes import Morpheme
 
 _kiwi = Kiwi()
 
 
 def extract_sentence_as_stream(json_data: dict):
     paragraphs = [news["paragraph"] for news in json_data["document"]]
     for paragraph in paragraphs:
```

### Comparing `nikl-corpus-io-0.0.1/src/nikl/usecases/corpus_merge_usecase.py` & `nikl-corpus-io-0.0.2/corpus_io/nikl/usecases/corpus_merge_usecase.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from typing import Dict, List, Optional
 
-from file_io.morphemes_io import MorphemeIOService
-from nikl import NIKLTokenizeIOService
+from corpus_io.file_io.morphemes_io import MorphemeIOService
+from corpus_io.nikl.abc import NIKLTokenizeIOService
 
 
 @dataclass(frozen=True)
 class CorpusMergeOption:
     dir_path: str
     max_file_num: Optional[int] = None
```

### Comparing `nikl-corpus-io-0.0.1/src/nikl_corpus_io.egg-info/PKG-INFO` & `nikl-corpus-io-0.0.2/nikl_corpus_io.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nikl-corpus-io
-Version: 0.0.1
+Version: 0.0.2
 Summary: Read/write nikl corpus
 Home-page: https://github.com/re-writers/corpusIO.python
 Author: postBG
 Author-email: profile2697@gmail.com
 Project-URL: Bug Tracker, https://github.com/re-writers/corpusIO.python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

