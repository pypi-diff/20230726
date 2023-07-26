# Comparing `tmp/lexikanon-0.3.0.tar.gz` & `tmp/lexikanon-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexikanon-0.3.0.tar", max compression
+gzip compressed data, was "lexikanon-0.3.1.tar", max compression
```

## Comparing `lexikanon-0.3.0.tar` & `lexikanon-0.3.1.tar`

### file list

```diff
@@ -1,47 +1,49 @@
--rw-r--r--   0        0        0     1071 2023-07-26 03:11:19.835217 lexikanon-0.3.0/LICENSE
--rw-r--r--   0        0        0     2129 2023-07-26 03:11:19.835217 lexikanon-0.3.0/README.md
--rw-r--r--   0        0        0     3201 2023-07-26 03:11:53.127674 lexikanon-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      184 2023-07-26 03:11:19.839217 lexikanon-0.3.0/src/lexikanon/__cli__.py
--rw-r--r--   0        0        0      473 2023-07-26 03:11:19.839217 lexikanon-0.3.0/src/lexikanon/__init__.py
--rw-r--r--   0        0        0       22 2023-07-26 03:11:53.083674 lexikanon-0.3.0/src/lexikanon/_version.py
--rw-r--r--   0        0        0        0 2023-07-26 03:11:19.839217 lexikanon-0.3.0/src/lexikanon/conf/__init__.py
--rw-r--r--   0        0        0      177 2023-07-26 03:11:19.839217 lexikanon-0.3.0/src/lexikanon/conf/about/lexikanon.yaml
--rw-r--r--   0        0        0      162 2023-07-26 03:11:19.839217 lexikanon-0.3.0/src/lexikanon/conf/normalizer/__init__.yaml
--rw-r--r--   0        0        0       54 2023-07-26 03:11:19.839217 lexikanon-0.3.0/src/lexikanon/conf/normalizer/formal_en.yaml
--rw-r--r--   0        0        0       77 2023-07-26 03:11:19.839217 lexikanon-0.3.0/src/lexikanon/conf/normalizer/formal_en_parantheses.yaml
--rw-r--r--   0        0        0       43 2023-07-26 03:11:19.839217 lexikanon-0.3.0/src/lexikanon/conf/normalizer/formal_ko.yaml
--rw-r--r--   0        0        0      363 2023-07-26 03:11:19.839217 lexikanon-0.3.0/src/lexikanon/conf/normalizer/ftfy/__init__.yaml
--rw-r--r--   0        0        0       67 2023-07-26 03:11:19.839217 lexikanon-0.3.0/src/lexikanon/conf/normalizer/informal_ko.yaml
--rw-r--r--   0        0        0      102 2023-07-26 03:11:19.839217 lexikanon-0.3.0/src/lexikanon/conf/normalizer/spaces/__init__.yaml
--rw-r--r--   0        0        0      151 2023-07-26 03:11:19.839217 lexikanon-0.3.0/src/lexikanon/conf/normalizer/special_characters/__init__.yaml
--rw-r--r--   0        0        0       67 2023-07-26 03:11:19.839217 lexikanon-0.3.0/src/lexikanon/conf/pipe/dataset_extract_nouns.yaml
--rw-r--r--   0        0        0      451 2023-07-26 03:11:19.839217 lexikanon-0.3.0/src/lexikanon/conf/pipe/dataset_extract_tokens.yaml
--rw-r--r--   0        0        0      343 2023-07-26 03:11:19.839217 lexikanon-0.3.0/src/lexikanon/conf/pipe/dataset_tokenize.yaml
--rw-r--r--   0        0        0      154 2023-07-26 03:11:19.839217 lexikanon-0.3.0/src/lexikanon/conf/stopwords/__init__.yaml
--rw-r--r--   0        0        0      491 2023-07-26 03:11:19.839217 lexikanon-0.3.0/src/lexikanon/conf/tokenizer/__init__.yaml
--rw-r--r--   0        0        0      241 2023-07-26 03:11:19.839217 lexikanon-0.3.0/src/lexikanon/conf/tokenizer/mecab.yaml
--rw-r--r--   0        0        0      151 2023-07-26 03:11:19.839217 lexikanon-0.3.0/src/lexikanon/conf/tokenizer/nltk.yaml
--rw-r--r--   0        0        0       87 2023-07-26 03:11:19.839217 lexikanon-0.3.0/src/lexikanon/conf/tokenizer/simple.yaml
--rw-r--r--   0        0        0       88 2023-07-26 03:11:19.839217 lexikanon-0.3.0/src/lexikanon/conf/tokenizer/tagger/mecab.yaml
--rw-r--r--   0        0        0      125 2023-07-26 03:11:19.839217 lexikanon-0.3.0/src/lexikanon/conf/tokenizer/tagger/nltk.yaml
--rw-r--r--   0        0        0       61 2023-07-26 03:11:19.839217 lexikanon-0.3.0/src/lexikanon/normalizers/__init__.py
--rw-r--r--   0        0        0    10196 2023-07-26 03:11:19.839217 lexikanon-0.3.0/src/lexikanon/normalizers/normalizer.py
--rw-r--r--   0        0        0        0 2023-07-26 03:11:19.839217 lexikanon-0.3.0/src/lexikanon/pipe/__init__.py
--rw-r--r--   0        0        0     2931 2023-07-26 03:11:19.839217 lexikanon-0.3.0/src/lexikanon/pipe/tokenize.py
--rw-r--r--   0        0        0      195 2023-07-26 03:11:19.839217 lexikanon-0.3.0/src/lexikanon/project.toml
--rw-r--r--   0        0        0        0 2023-07-26 03:11:19.839217 lexikanon-0.3.0/src/lexikanon/py.typed
--rw-r--r--   0        0        0  2355775 2023-07-26 03:11:19.855216 lexikanon-0.3.0/src/lexikanon/resources/dictionaries/mecab/ekon_v1.dic
--rw-r--r--   0        0        0       58 2023-07-26 03:11:19.855216 lexikanon-0.3.0/src/lexikanon/stopwords/__init__.py
--rw-r--r--   0        0        0     5072 2023-07-26 03:11:19.855216 lexikanon-0.3.0/src/lexikanon/stopwords/stopwords.py
--rw-r--r--   0        0        0      181 2023-07-26 03:11:19.855216 lexikanon-0.3.0/src/lexikanon/tokenizers/__init__.py
--rw-r--r--   0        0        0     9219 2023-07-26 03:11:19.855216 lexikanon-0.3.0/src/lexikanon/tokenizers/base.py
--rw-r--r--   0        0        0      732 2023-07-26 03:11:19.855216 lexikanon-0.3.0/src/lexikanon/tokenizers/mecab.py
--rw-r--r--   0        0        0     3074 2023-07-26 03:11:19.855216 lexikanon-0.3.0/src/lexikanon/tokenizers/nltk.py
--rw-r--r--   0        0        0    14339 2023-07-26 03:11:19.855216 lexikanon-0.3.0/src/lexikanon/utils/__init__.py
--rw-r--r--   0        0        0     8294 2023-07-26 03:11:19.855216 lexikanon-0.3.0/src/lexikanon/utils/hangle.py
--rw-r--r--   0        0        0      255 2023-07-26 03:11:19.855216 lexikanon-0.3.0/src/lexikanon/utils/hanja/__init__.py
--rw-r--r--   0        0        0     2123 2023-07-26 03:11:19.855216 lexikanon-0.3.0/src/lexikanon/utils/hanja/hangul.py
--rw-r--r--   0        0        0     2813 2023-07-26 03:11:19.855216 lexikanon-0.3.0/src/lexikanon/utils/hanja/impl.py
--rw-r--r--   0        0        0      427 2023-07-26 03:11:19.855216 lexikanon-0.3.0/src/lexikanon/utils/hanja/table.py
--rw-r--r--   0        0        0   522443 2023-07-26 03:11:19.855216 lexikanon-0.3.0/src/lexikanon/utils/hanja/table.yml
--rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 lexikanon-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-26 06:45:31.649738 lexikanon-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2129 2023-07-26 06:45:31.649738 lexikanon-0.3.1/README.md
+-rw-r--r--   0        0        0     3201 2023-07-26 06:46:15.304884 lexikanon-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      184 2023-07-26 06:45:31.653739 lexikanon-0.3.1/src/lexikanon/__cli__.py
+-rw-r--r--   0        0        0      473 2023-07-26 06:45:31.653739 lexikanon-0.3.1/src/lexikanon/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-26 06:46:15.252880 lexikanon-0.3.1/src/lexikanon/_version.py
+-rw-r--r--   0        0        0        0 2023-07-26 06:45:31.653739 lexikanon-0.3.1/src/lexikanon/conf/__init__.py
+-rw-r--r--   0        0        0      177 2023-07-26 06:45:31.653739 lexikanon-0.3.1/src/lexikanon/conf/about/lexikanon.yaml
+-rw-r--r--   0        0        0      162 2023-07-26 06:45:31.653739 lexikanon-0.3.1/src/lexikanon/conf/normalizer/__init__.yaml
+-rw-r--r--   0        0        0       54 2023-07-26 06:45:31.653739 lexikanon-0.3.1/src/lexikanon/conf/normalizer/formal_en.yaml
+-rw-r--r--   0        0        0       77 2023-07-26 06:45:31.653739 lexikanon-0.3.1/src/lexikanon/conf/normalizer/formal_en_parantheses.yaml
+-rw-r--r--   0        0        0       43 2023-07-26 06:45:31.653739 lexikanon-0.3.1/src/lexikanon/conf/normalizer/formal_ko.yaml
+-rw-r--r--   0        0        0      363 2023-07-26 06:45:31.653739 lexikanon-0.3.1/src/lexikanon/conf/normalizer/ftfy/__init__.yaml
+-rw-r--r--   0        0        0       67 2023-07-26 06:45:31.653739 lexikanon-0.3.1/src/lexikanon/conf/normalizer/informal_ko.yaml
+-rw-r--r--   0        0        0      102 2023-07-26 06:45:31.653739 lexikanon-0.3.1/src/lexikanon/conf/normalizer/spaces/__init__.yaml
+-rw-r--r--   0        0        0      151 2023-07-26 06:45:31.653739 lexikanon-0.3.1/src/lexikanon/conf/normalizer/special_characters/__init__.yaml
+-rw-r--r--   0        0        0       62 2023-07-26 06:45:31.653739 lexikanon-0.3.1/src/lexikanon/conf/pipe/dataset_extract_nouns.yaml
+-rw-r--r--   0        0        0      109 2023-07-26 06:45:31.653739 lexikanon-0.3.1/src/lexikanon/conf/pipe/dataset_extract_tokens.yaml
+-rw-r--r--   0        0        0      111 2023-07-26 06:45:31.653739 lexikanon-0.3.1/src/lexikanon/conf/pipe/dataset_tokenize.yaml
+-rw-r--r--   0        0        0      399 2023-07-26 06:45:31.653739 lexikanon-0.3.1/src/lexikanon/conf/run/extract_tokens.yaml
+-rw-r--r--   0        0        0      303 2023-07-26 06:45:31.653739 lexikanon-0.3.1/src/lexikanon/conf/run/tokenize_dataset.yaml
+-rw-r--r--   0        0        0      154 2023-07-26 06:45:31.653739 lexikanon-0.3.1/src/lexikanon/conf/stopwords/__init__.yaml
+-rw-r--r--   0        0        0      491 2023-07-26 06:45:31.653739 lexikanon-0.3.1/src/lexikanon/conf/tokenizer/__init__.yaml
+-rw-r--r--   0        0        0      241 2023-07-26 06:45:31.653739 lexikanon-0.3.1/src/lexikanon/conf/tokenizer/mecab.yaml
+-rw-r--r--   0        0        0      151 2023-07-26 06:45:31.653739 lexikanon-0.3.1/src/lexikanon/conf/tokenizer/nltk.yaml
+-rw-r--r--   0        0        0       87 2023-07-26 06:45:31.653739 lexikanon-0.3.1/src/lexikanon/conf/tokenizer/simple.yaml
+-rw-r--r--   0        0        0       88 2023-07-26 06:45:31.653739 lexikanon-0.3.1/src/lexikanon/conf/tokenizer/tagger/mecab.yaml
+-rw-r--r--   0        0        0      125 2023-07-26 06:45:31.653739 lexikanon-0.3.1/src/lexikanon/conf/tokenizer/tagger/nltk.yaml
+-rw-r--r--   0        0        0       61 2023-07-26 06:45:31.653739 lexikanon-0.3.1/src/lexikanon/normalizers/__init__.py
+-rw-r--r--   0        0        0    10196 2023-07-26 06:45:31.653739 lexikanon-0.3.1/src/lexikanon/normalizers/normalizer.py
+-rw-r--r--   0        0        0        0 2023-07-26 06:45:31.653739 lexikanon-0.3.1/src/lexikanon/pipe/__init__.py
+-rw-r--r--   0        0        0     3430 2023-07-26 06:45:31.653739 lexikanon-0.3.1/src/lexikanon/pipe/tokenize.py
+-rw-r--r--   0        0        0      195 2023-07-26 06:45:31.653739 lexikanon-0.3.1/src/lexikanon/project.toml
+-rw-r--r--   0        0        0        0 2023-07-26 06:45:31.653739 lexikanon-0.3.1/src/lexikanon/py.typed
+-rw-r--r--   0        0        0  2355775 2023-07-26 06:45:31.669739 lexikanon-0.3.1/src/lexikanon/resources/dictionaries/mecab/ekon_v1.dic
+-rw-r--r--   0        0        0       58 2023-07-26 06:45:31.673739 lexikanon-0.3.1/src/lexikanon/stopwords/__init__.py
+-rw-r--r--   0        0        0     5072 2023-07-26 06:45:31.673739 lexikanon-0.3.1/src/lexikanon/stopwords/stopwords.py
+-rw-r--r--   0        0        0      181 2023-07-26 06:45:31.673739 lexikanon-0.3.1/src/lexikanon/tokenizers/__init__.py
+-rw-r--r--   0        0        0     9219 2023-07-26 06:45:31.673739 lexikanon-0.3.1/src/lexikanon/tokenizers/base.py
+-rw-r--r--   0        0        0      732 2023-07-26 06:45:31.673739 lexikanon-0.3.1/src/lexikanon/tokenizers/mecab.py
+-rw-r--r--   0        0        0     3074 2023-07-26 06:45:31.673739 lexikanon-0.3.1/src/lexikanon/tokenizers/nltk.py
+-rw-r--r--   0        0        0    14339 2023-07-26 06:45:31.673739 lexikanon-0.3.1/src/lexikanon/utils/__init__.py
+-rw-r--r--   0        0        0     8294 2023-07-26 06:45:31.673739 lexikanon-0.3.1/src/lexikanon/utils/hangle.py
+-rw-r--r--   0        0        0      255 2023-07-26 06:45:31.673739 lexikanon-0.3.1/src/lexikanon/utils/hanja/__init__.py
+-rw-r--r--   0        0        0     2123 2023-07-26 06:45:31.673739 lexikanon-0.3.1/src/lexikanon/utils/hanja/hangul.py
+-rw-r--r--   0        0        0     2813 2023-07-26 06:45:31.673739 lexikanon-0.3.1/src/lexikanon/utils/hanja/impl.py
+-rw-r--r--   0        0        0      427 2023-07-26 06:45:31.673739 lexikanon-0.3.1/src/lexikanon/utils/hanja/table.py
+-rw-r--r--   0        0        0   522443 2023-07-26 06:45:31.673739 lexikanon-0.3.1/src/lexikanon/utils/hanja/table.yml
+-rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 lexikanon-0.3.1/PKG-INFO
```

### Comparing `lexikanon-0.3.0/LICENSE` & `lexikanon-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lexikanon-0.3.0/README.md` & `lexikanon-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `lexikanon-0.3.0/pyproject.toml` & `lexikanon-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "lexikanon"
-version = "0.3.0"
+version = "0.3.1"
 description = "A Python Library for Tokenizers"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://lexikanon.entelecheia.ai"
 repository = "https://github.com/entelecheia/lexikanon"
 readme = "README.md"
 packages = [{ include = "lexikanon", from = "src" }]
 
 [tool.poetry.scripts]
 lexikanon = 'lexikanon.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 click = "^8.1.3"
-hyfi = "^1.10.2"
+hyfi = "^1.11.0"
 ftfy = "^6.1.1"
 nltk = "^3.8.1"
 ekonlpy = "^2.0.2"
 # hyfi = { path = "../hyfi", develop = true }
 
 [tool.poetry.group.dev]
 optional = true
```

### Comparing `lexikanon-0.3.0/src/lexikanon/normalizers/normalizer.py` & `lexikanon-0.3.1/src/lexikanon/normalizers/normalizer.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.3.0/src/lexikanon/pipe/tokenize.py` & `lexikanon-0.3.1/src/lexikanon/pipe/tokenize.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     num_workers: int = 1,
     batched: bool = True,
     batch_size: int = 1000,
     text_col: str = "bodyText",
     token_col: str = "tokenizedText",
     remove_columns: Optional[Union[List[str], str]] = None,
     load_from_cache_file: bool = True,
+    num_heads: Optional[int] = 1,
+    num_tails: Optional[int] = 1,
     verbose: bool = False,
 ) -> Dataset:
     def pos_tagging(batch):
         tokenizer = HyFI.instantiate_config(f"tokenizer={tokenizer_config_name}")
         batch_tokens = []
         for text in batch[text_col]:
             sentences = text.split("\n")
@@ -36,15 +38,20 @@
         batched=batched,
         batch_size=batch_size,
         remove_columns=remove_columns,
         load_from_cache_file=load_from_cache_file,
     )
     logger.info("POS tagging done. See column '%s'.", token_col)
     if verbose:
-        print(data[0][token_col])
+        if num_heads:
+            num_heads = min(num_heads, len(data))
+            print(data[:num_heads][token_col])
+        if num_tails:
+            num_tails = min(num_tails, len(data))
+            print(data[-num_tails:][token_col])
     return data
 
 
 def extract_tokens(
     data: Dataset,
     tokenizer_config_name: str = "simple",
     num_workers: int = 1,
@@ -56,14 +63,16 @@
     postags: Optional[List[str]] = None,
     stop_postags: Optional[List[str]] = None,
     strip_pos: Optional[bool] = None,
     postag_delim: Optional[str] = None,
     postag_length: Optional[int] = None,
     remove_columns: Optional[Union[List[str], str]] = None,
     load_from_cache_file: bool = True,
+    num_heads: Optional[int] = 1,
+    num_tails: Optional[int] = 1,
     verbose: bool = False,
 ) -> Dataset:
     def pos_tagging(batch):
         tokenizer = HyFI.instantiate_config(f"tokenizer={tokenizer_config_name}")
         batch_tokens = []
         for tokens in batch[token_col]:
             batch_tokens.append(
@@ -85,10 +94,14 @@
         batched=batched,
         batch_size=batch_size,
         remove_columns=remove_columns,
         load_from_cache_file=load_from_cache_file,
     )
     logger.info("Extracting tokens done, see column '%s'.", extracted_col)
     if verbose:
-        num_samples = min(5, len(data))
-        print(data[:num_samples][extracted_col])
+        if num_heads:
+            num_heads = min(num_heads, len(data))
+            print(data[:num_heads][extracted_col])
+        if num_tails:
+            num_tails = min(num_tails, len(data))
+            print(data[-num_tails:][extracted_col])
     return data
```

### Comparing `lexikanon-0.3.0/src/lexikanon/resources/dictionaries/mecab/ekon_v1.dic` & `lexikanon-0.3.1/src/lexikanon/resources/dictionaries/mecab/ekon_v1.dic`

 * *Files identical despite different names*

### Comparing `lexikanon-0.3.0/src/lexikanon/stopwords/stopwords.py` & `lexikanon-0.3.1/src/lexikanon/stopwords/stopwords.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.3.0/src/lexikanon/tokenizers/base.py` & `lexikanon-0.3.1/src/lexikanon/tokenizers/base.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.3.0/src/lexikanon/tokenizers/mecab.py` & `lexikanon-0.3.1/src/lexikanon/tokenizers/mecab.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.3.0/src/lexikanon/tokenizers/nltk.py` & `lexikanon-0.3.1/src/lexikanon/tokenizers/nltk.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.3.0/src/lexikanon/utils/__init__.py` & `lexikanon-0.3.1/src/lexikanon/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.3.0/src/lexikanon/utils/hangle.py` & `lexikanon-0.3.1/src/lexikanon/utils/hangle.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.3.0/src/lexikanon/utils/hanja/hangul.py` & `lexikanon-0.3.1/src/lexikanon/utils/hanja/hangul.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.3.0/src/lexikanon/utils/hanja/impl.py` & `lexikanon-0.3.1/src/lexikanon/utils/hanja/impl.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.3.0/src/lexikanon/utils/hanja/table.yml` & `lexikanon-0.3.1/src/lexikanon/utils/hanja/table.yml`

 * *Files identical despite different names*

### Comparing `lexikanon-0.3.0/PKG-INFO` & `lexikanon-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: lexikanon
-Version: 0.3.0
+Version: 0.3.1
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
-Requires-Dist: hyfi (>=1.10.2,<2.0.0)
+Requires-Dist: hyfi (>=1.11.0,<2.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Project-URL: Repository, https://github.com/entelecheia/lexikanon
 Description-Content-Type: text/markdown
 
 # Lexikanon
 
 [![pypi-image]][pypi-url]
```

