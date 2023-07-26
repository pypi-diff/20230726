# Comparing `tmp/lexikanon-0.2.3.tar.gz` & `tmp/lexikanon-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexikanon-0.2.3.tar", max compression
+gzip compressed data, was "lexikanon-0.2.4.tar", max compression
```

## Comparing `lexikanon-0.2.3.tar` & `lexikanon-0.2.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1071 2023-07-25 00:17:11.589010 lexikanon-0.2.3/LICENSE
--rw-r--r--   0        0        0     2129 2023-07-25 00:17:11.589010 lexikanon-0.2.3/README.md
--rw-r--r--   0        0        0     2932 2023-07-25 00:17:45.328831 lexikanon-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      184 2023-07-25 00:17:11.593010 lexikanon-0.2.3/src/lexikanon/__cli__.py
--rw-r--r--   0        0        0      473 2023-07-25 00:17:11.593010 lexikanon-0.2.3/src/lexikanon/__init__.py
--rw-r--r--   0        0        0       22 2023-07-25 00:17:45.276831 lexikanon-0.2.3/src/lexikanon/_version.py
--rw-r--r--   0        0        0        0 2023-07-25 00:17:11.593010 lexikanon-0.2.3/src/lexikanon/conf/__init__.py
--rw-r--r--   0        0        0      177 2023-07-25 00:17:11.593010 lexikanon-0.2.3/src/lexikanon/conf/about/lexikanon.yaml
--rw-r--r--   0        0        0      162 2023-07-25 00:17:11.593010 lexikanon-0.2.3/src/lexikanon/conf/normalizer/__init__.yaml
--rw-r--r--   0        0        0       54 2023-07-25 00:17:11.593010 lexikanon-0.2.3/src/lexikanon/conf/normalizer/formal_en.yaml
--rw-r--r--   0        0        0       77 2023-07-25 00:17:11.593010 lexikanon-0.2.3/src/lexikanon/conf/normalizer/formal_en_parantheses.yaml
--rw-r--r--   0        0        0       43 2023-07-25 00:17:11.593010 lexikanon-0.2.3/src/lexikanon/conf/normalizer/formal_ko.yaml
--rw-r--r--   0        0        0      363 2023-07-25 00:17:11.593010 lexikanon-0.2.3/src/lexikanon/conf/normalizer/ftfy/__init__.yaml
--rw-r--r--   0        0        0       67 2023-07-25 00:17:11.593010 lexikanon-0.2.3/src/lexikanon/conf/normalizer/informal_ko.yaml
--rw-r--r--   0        0        0      102 2023-07-25 00:17:11.593010 lexikanon-0.2.3/src/lexikanon/conf/normalizer/spaces/__init__.yaml
--rw-r--r--   0        0        0      151 2023-07-25 00:17:11.593010 lexikanon-0.2.3/src/lexikanon/conf/normalizer/special_characters/__init__.yaml
--rw-r--r--   0        0        0      135 2023-07-25 00:17:11.593010 lexikanon-0.2.3/src/lexikanon/conf/stopwords/__init__.yaml
--rw-r--r--   0        0        0      491 2023-07-25 00:17:11.593010 lexikanon-0.2.3/src/lexikanon/conf/tokenizer/__init__.yaml
--rw-r--r--   0        0        0      241 2023-07-25 00:17:11.593010 lexikanon-0.2.3/src/lexikanon/conf/tokenizer/mecab.yaml
--rw-r--r--   0        0        0      151 2023-07-25 00:17:11.593010 lexikanon-0.2.3/src/lexikanon/conf/tokenizer/nltk.yaml
--rw-r--r--   0        0        0       87 2023-07-25 00:17:11.593010 lexikanon-0.2.3/src/lexikanon/conf/tokenizer/simple.yaml
--rw-r--r--   0        0        0       88 2023-07-25 00:17:11.593010 lexikanon-0.2.3/src/lexikanon/conf/tokenizer/tagger/mecab.yaml
--rw-r--r--   0        0        0      125 2023-07-25 00:17:11.593010 lexikanon-0.2.3/src/lexikanon/conf/tokenizer/tagger/nltk.yaml
--rw-r--r--   0        0        0       61 2023-07-25 00:17:11.593010 lexikanon-0.2.3/src/lexikanon/normalizers/__init__.py
--rw-r--r--   0        0        0    10196 2023-07-25 00:17:11.593010 lexikanon-0.2.3/src/lexikanon/normalizers/normalizer.py
--rw-r--r--   0        0        0      195 2023-07-25 00:17:11.593010 lexikanon-0.2.3/src/lexikanon/project.toml
--rw-r--r--   0        0        0        0 2023-07-25 00:17:11.593010 lexikanon-0.2.3/src/lexikanon/py.typed
--rw-r--r--   0        0        0  2355775 2023-07-25 00:17:11.605011 lexikanon-0.2.3/src/lexikanon/resources/dictionaries/mecab/ekon_v1.dic
--rw-r--r--   0        0        0       58 2023-07-25 00:17:11.605011 lexikanon-0.2.3/src/lexikanon/stopwords/__init__.py
--rw-r--r--   0        0        0     2803 2023-07-25 00:17:11.605011 lexikanon-0.2.3/src/lexikanon/stopwords/stopwords.py
--rw-r--r--   0        0        0      181 2023-07-25 00:17:11.605011 lexikanon-0.2.3/src/lexikanon/tokenizers/__init__.py
--rw-r--r--   0        0        0     9219 2023-07-25 00:17:11.605011 lexikanon-0.2.3/src/lexikanon/tokenizers/base.py
--rw-r--r--   0        0        0      732 2023-07-25 00:17:11.605011 lexikanon-0.2.3/src/lexikanon/tokenizers/mecab.py
--rw-r--r--   0        0        0     3074 2023-07-25 00:17:11.605011 lexikanon-0.2.3/src/lexikanon/tokenizers/nltk.py
--rw-r--r--   0        0        0    14339 2023-07-25 00:17:11.605011 lexikanon-0.2.3/src/lexikanon/utils/__init__.py
--rw-r--r--   0        0        0     8294 2023-07-25 00:17:11.605011 lexikanon-0.2.3/src/lexikanon/utils/hangle.py
--rw-r--r--   0        0        0      255 2023-07-25 00:17:11.609011 lexikanon-0.2.3/src/lexikanon/utils/hanja/__init__.py
--rw-r--r--   0        0        0     2123 2023-07-25 00:17:11.609011 lexikanon-0.2.3/src/lexikanon/utils/hanja/hangul.py
--rw-r--r--   0        0        0     2813 2023-07-25 00:17:11.609011 lexikanon-0.2.3/src/lexikanon/utils/hanja/impl.py
--rw-r--r--   0        0        0      427 2023-07-25 00:17:11.609011 lexikanon-0.2.3/src/lexikanon/utils/hanja/table.py
--rw-r--r--   0        0        0   522443 2023-07-25 00:17:11.609011 lexikanon-0.2.3/src/lexikanon/utils/hanja/table.yml
--rw-r--r--   0        0        0     2920 1970-01-01 00:00:00.000000 lexikanon-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-25 19:37:58.120350 lexikanon-0.2.4/LICENSE
+-rw-r--r--   0        0        0     2129 2023-07-25 19:37:58.120350 lexikanon-0.2.4/README.md
+-rw-r--r--   0        0        0     3155 2023-07-25 19:38:31.260685 lexikanon-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      184 2023-07-25 19:37:58.124350 lexikanon-0.2.4/src/lexikanon/__cli__.py
+-rw-r--r--   0        0        0      473 2023-07-25 19:37:58.124350 lexikanon-0.2.4/src/lexikanon/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-25 19:38:31.220684 lexikanon-0.2.4/src/lexikanon/_version.py
+-rw-r--r--   0        0        0        0 2023-07-25 19:37:58.124350 lexikanon-0.2.4/src/lexikanon/conf/__init__.py
+-rw-r--r--   0        0        0      177 2023-07-25 19:37:58.124350 lexikanon-0.2.4/src/lexikanon/conf/about/lexikanon.yaml
+-rw-r--r--   0        0        0      162 2023-07-25 19:37:58.124350 lexikanon-0.2.4/src/lexikanon/conf/normalizer/__init__.yaml
+-rw-r--r--   0        0        0       54 2023-07-25 19:37:58.124350 lexikanon-0.2.4/src/lexikanon/conf/normalizer/formal_en.yaml
+-rw-r--r--   0        0        0       77 2023-07-25 19:37:58.124350 lexikanon-0.2.4/src/lexikanon/conf/normalizer/formal_en_parantheses.yaml
+-rw-r--r--   0        0        0       43 2023-07-25 19:37:58.124350 lexikanon-0.2.4/src/lexikanon/conf/normalizer/formal_ko.yaml
+-rw-r--r--   0        0        0      363 2023-07-25 19:37:58.124350 lexikanon-0.2.4/src/lexikanon/conf/normalizer/ftfy/__init__.yaml
+-rw-r--r--   0        0        0       67 2023-07-25 19:37:58.124350 lexikanon-0.2.4/src/lexikanon/conf/normalizer/informal_ko.yaml
+-rw-r--r--   0        0        0      102 2023-07-25 19:37:58.124350 lexikanon-0.2.4/src/lexikanon/conf/normalizer/spaces/__init__.yaml
+-rw-r--r--   0        0        0      151 2023-07-25 19:37:58.124350 lexikanon-0.2.4/src/lexikanon/conf/normalizer/special_characters/__init__.yaml
+-rw-r--r--   0        0        0      154 2023-07-25 19:37:58.124350 lexikanon-0.2.4/src/lexikanon/conf/stopwords/__init__.yaml
+-rw-r--r--   0        0        0      491 2023-07-25 19:37:58.124350 lexikanon-0.2.4/src/lexikanon/conf/tokenizer/__init__.yaml
+-rw-r--r--   0        0        0      241 2023-07-25 19:37:58.124350 lexikanon-0.2.4/src/lexikanon/conf/tokenizer/mecab.yaml
+-rw-r--r--   0        0        0      151 2023-07-25 19:37:58.124350 lexikanon-0.2.4/src/lexikanon/conf/tokenizer/nltk.yaml
+-rw-r--r--   0        0        0       87 2023-07-25 19:37:58.124350 lexikanon-0.2.4/src/lexikanon/conf/tokenizer/simple.yaml
+-rw-r--r--   0        0        0       88 2023-07-25 19:37:58.124350 lexikanon-0.2.4/src/lexikanon/conf/tokenizer/tagger/mecab.yaml
+-rw-r--r--   0        0        0      125 2023-07-25 19:37:58.124350 lexikanon-0.2.4/src/lexikanon/conf/tokenizer/tagger/nltk.yaml
+-rw-r--r--   0        0        0       61 2023-07-25 19:37:58.124350 lexikanon-0.2.4/src/lexikanon/normalizers/__init__.py
+-rw-r--r--   0        0        0    10196 2023-07-25 19:37:58.124350 lexikanon-0.2.4/src/lexikanon/normalizers/normalizer.py
+-rw-r--r--   0        0        0      195 2023-07-25 19:37:58.124350 lexikanon-0.2.4/src/lexikanon/project.toml
+-rw-r--r--   0        0        0        0 2023-07-25 19:37:58.124350 lexikanon-0.2.4/src/lexikanon/py.typed
+-rw-r--r--   0        0        0  2355775 2023-07-25 19:37:58.136350 lexikanon-0.2.4/src/lexikanon/resources/dictionaries/mecab/ekon_v1.dic
+-rw-r--r--   0        0        0       58 2023-07-25 19:37:58.136350 lexikanon-0.2.4/src/lexikanon/stopwords/__init__.py
+-rw-r--r--   0        0        0     5072 2023-07-25 19:37:58.136350 lexikanon-0.2.4/src/lexikanon/stopwords/stopwords.py
+-rw-r--r--   0        0        0      181 2023-07-25 19:37:58.136350 lexikanon-0.2.4/src/lexikanon/tokenizers/__init__.py
+-rw-r--r--   0        0        0     9219 2023-07-25 19:37:58.136350 lexikanon-0.2.4/src/lexikanon/tokenizers/base.py
+-rw-r--r--   0        0        0      732 2023-07-25 19:37:58.136350 lexikanon-0.2.4/src/lexikanon/tokenizers/mecab.py
+-rw-r--r--   0        0        0     3074 2023-07-25 19:37:58.136350 lexikanon-0.2.4/src/lexikanon/tokenizers/nltk.py
+-rw-r--r--   0        0        0    14339 2023-07-25 19:37:58.136350 lexikanon-0.2.4/src/lexikanon/utils/__init__.py
+-rw-r--r--   0        0        0     8294 2023-07-25 19:37:58.136350 lexikanon-0.2.4/src/lexikanon/utils/hangle.py
+-rw-r--r--   0        0        0      255 2023-07-25 19:37:58.136350 lexikanon-0.2.4/src/lexikanon/utils/hanja/__init__.py
+-rw-r--r--   0        0        0     2123 2023-07-25 19:37:58.136350 lexikanon-0.2.4/src/lexikanon/utils/hanja/hangul.py
+-rw-r--r--   0        0        0     2813 2023-07-25 19:37:58.136350 lexikanon-0.2.4/src/lexikanon/utils/hanja/impl.py
+-rw-r--r--   0        0        0      427 2023-07-25 19:37:58.136350 lexikanon-0.2.4/src/lexikanon/utils/hanja/table.py
+-rw-r--r--   0        0        0   522443 2023-07-25 19:37:58.140350 lexikanon-0.2.4/src/lexikanon/utils/hanja/table.yml
+-rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 lexikanon-0.2.4/PKG-INFO
```

### Comparing `lexikanon-0.2.3/LICENSE` & `lexikanon-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lexikanon-0.2.3/README.md` & `lexikanon-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `lexikanon-0.2.3/src/lexikanon/normalizers/normalizer.py` & `lexikanon-0.2.4/src/lexikanon/normalizers/normalizer.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.2.3/src/lexikanon/resources/dictionaries/mecab/ekon_v1.dic` & `lexikanon-0.2.4/src/lexikanon/resources/dictionaries/mecab/ekon_v1.dic`

 * *Files identical despite different names*

### Comparing `lexikanon-0.2.3/src/lexikanon/tokenizers/base.py` & `lexikanon-0.2.4/src/lexikanon/tokenizers/base.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.2.3/src/lexikanon/tokenizers/mecab.py` & `lexikanon-0.2.4/src/lexikanon/tokenizers/mecab.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.2.3/src/lexikanon/tokenizers/nltk.py` & `lexikanon-0.2.4/src/lexikanon/tokenizers/nltk.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.2.3/src/lexikanon/utils/__init__.py` & `lexikanon-0.2.4/src/lexikanon/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.2.3/src/lexikanon/utils/hangle.py` & `lexikanon-0.2.4/src/lexikanon/utils/hangle.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.2.3/src/lexikanon/utils/hanja/hangul.py` & `lexikanon-0.2.4/src/lexikanon/utils/hanja/hangul.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.2.3/src/lexikanon/utils/hanja/impl.py` & `lexikanon-0.2.4/src/lexikanon/utils/hanja/impl.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.2.3/src/lexikanon/utils/hanja/table.yml` & `lexikanon-0.2.4/src/lexikanon/utils/hanja/table.yml`

 * *Files identical despite different names*

### Comparing `lexikanon-0.2.3/PKG-INFO` & `lexikanon-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: lexikanon
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Python Library for Tokenizers
 Home-page: https://lexikanon.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: ekonlpy (>=2.0.2,<3.0.0)
 Requires-Dist: ftfy (>=6.1.1,<7.0.0)
-Requires-Dist: hyfi (>=1.9.3,<2.0.0)
+Requires-Dist: hyfi (>=1.10.0,<2.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Project-URL: Repository, https://github.com/entelecheia/lexikanon
 Description-Content-Type: text/markdown
 
 # Lexikanon
 
 [![pypi-image]][pypi-url]
```

