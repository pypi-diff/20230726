# Comparing `tmp/uniparser-erzya-1.1.2.tar.gz` & `tmp/uniparser-erzya-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniparser-erzya-1.1.2.tar", last modified: Tue Jul  6 11:19:48 2021, max compression
+gzip compressed data, was "uniparser-erzya-1.1.3.tar", last modified: Wed Jul 26 14:19:53 2023, max compression
```

## Comparing `uniparser-erzya-1.1.2.tar` & `uniparser-erzya-1.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2021-07-06 11:19:48.621674 uniparser-erzya-1.1.2/
--rw-rw-rw-   0        0        0     1152 2021-07-06 11:08:25.000000 uniparser-erzya-1.1.2/LICENSE
--rw-rw-rw-   0        0        0      182 2021-06-21 08:27:56.000000 uniparser-erzya-1.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4206 2021-07-06 11:19:48.621674 uniparser-erzya-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3495 2021-06-21 08:27:56.000000 uniparser-erzya-1.1.2/README.md
--rw-rw-rw-   0        0        0      108 2021-06-21 08:27:56.000000 uniparser-erzya-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      820 2021-07-06 11:19:48.624664 uniparser-erzya-1.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2021-07-06 11:19:48.517950 uniparser-erzya-1.1.2/uniparser_erzya/
--rw-rw-rw-   0        0        0     2479 2021-06-21 08:27:56.000000 uniparser-erzya-1.1.2/uniparser_erzya/__init__.py
-drwxrwxrwx   0        0        0        0 2021-07-06 11:19:48.604718 uniparser-erzya-1.1.2/uniparser_erzya/data_nodiacritics/
--rw-rw-rw-   0        0        0        0 2021-06-21 08:27:56.000000 uniparser-erzya-1.1.2/uniparser_erzya/data_nodiacritics/__init__.py
--rw-rw-rw-   0        0        0     1755 2021-07-06 11:05:25.000000 uniparser-erzya-1.1.2/uniparser_erzya/data_nodiacritics/bad_analyses.txt
--rw-rw-rw-   0        0        0        0 2021-07-06 11:07:19.000000 uniparser-erzya-1.1.2/uniparser_erzya/data_nodiacritics/lex_rules.txt
--rw-rw-rw-   0        0        0  4492914 2021-07-06 11:07:19.000000 uniparser-erzya-1.1.2/uniparser_erzya/data_nodiacritics/lexemes.txt
--rw-rw-rw-   0        0        0    95487 2021-07-06 11:07:19.000000 uniparser-erzya-1.1.2/uniparser_erzya/data_nodiacritics/paradigms.txt
-drwxrwxrwx   0        0        0        0 2021-07-06 11:19:48.619679 uniparser-erzya-1.1.2/uniparser_erzya/data_strict/
--rw-rw-rw-   0        0        0        0 2021-06-21 08:27:56.000000 uniparser-erzya-1.1.2/uniparser_erzya/data_strict/__init__.py
--rw-rw-rw-   0        0        0     1755 2021-07-06 11:05:25.000000 uniparser-erzya-1.1.2/uniparser_erzya/data_strict/bad_analyses.txt
--rw-rw-rw-   0        0        0        0 2021-07-06 11:07:19.000000 uniparser-erzya-1.1.2/uniparser_erzya/data_strict/lex_rules.txt
--rw-rw-rw-   0        0        0  4472853 2021-07-06 11:07:19.000000 uniparser-erzya-1.1.2/uniparser_erzya/data_strict/lexemes.txt
--rw-rw-rw-   0        0        0    95070 2021-07-06 11:07:19.000000 uniparser-erzya-1.1.2/uniparser_erzya/data_strict/paradigms.txt
-drwxrwxrwx   0        0        0        0 2021-07-06 11:19:48.556846 uniparser-erzya-1.1.2/uniparser_erzya.egg-info/
--rw-rw-rw-   0        0        0     4206 2021-07-06 11:19:48.000000 uniparser-erzya-1.1.2/uniparser_erzya.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      724 2021-07-06 11:19:48.000000 uniparser-erzya-1.1.2/uniparser_erzya.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-07-06 11:19:48.000000 uniparser-erzya-1.1.2/uniparser_erzya.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2021-07-06 11:19:48.000000 uniparser-erzya-1.1.2/uniparser_erzya.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2021-07-06 11:19:48.000000 uniparser-erzya-1.1.2/uniparser_erzya.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 14:19:53.224507 uniparser-erzya-1.1.3/
+-rw-rw-rw-   0        0        0     1152 2023-07-26 12:46:08.000000 uniparser-erzya-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0      182 2023-07-26 12:46:08.000000 uniparser-erzya-1.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4165 2023-07-26 14:19:53.224507 uniparser-erzya-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3495 2023-07-26 12:46:08.000000 uniparser-erzya-1.1.3/README.md
+-rw-rw-rw-   0        0        0      108 2023-07-26 12:46:08.000000 uniparser-erzya-1.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0      820 2023-07-26 14:19:53.228517 uniparser-erzya-1.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-26 14:19:53.148508 uniparser-erzya-1.1.3/uniparser_erzya/
+-rw-rw-rw-   0        0        0     2479 2023-07-26 12:46:08.000000 uniparser-erzya-1.1.3/uniparser_erzya/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:19:53.212508 uniparser-erzya-1.1.3/uniparser_erzya/data_nodiacritics/
+-rw-rw-rw-   0        0        0        0 2023-07-26 12:46:08.000000 uniparser-erzya-1.1.3/uniparser_erzya/data_nodiacritics/__init__.py
+-rw-rw-rw-   0        0        0     1755 2023-07-26 12:46:08.000000 uniparser-erzya-1.1.3/uniparser_erzya/data_nodiacritics/bad_analyses.txt
+-rw-rw-rw-   0        0        0        0 2023-07-26 14:06:20.000000 uniparser-erzya-1.1.3/uniparser_erzya/data_nodiacritics/lex_rules.txt
+-rw-rw-rw-   0        0        0  4501798 2023-07-26 14:06:20.000000 uniparser-erzya-1.1.3/uniparser_erzya/data_nodiacritics/lexemes.txt
+-rw-rw-rw-   0        0        0    96494 2023-07-26 14:06:20.000000 uniparser-erzya-1.1.3/uniparser_erzya/data_nodiacritics/paradigms.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 14:19:53.224507 uniparser-erzya-1.1.3/uniparser_erzya/data_strict/
+-rw-rw-rw-   0        0        0        0 2023-07-26 12:46:08.000000 uniparser-erzya-1.1.3/uniparser_erzya/data_strict/__init__.py
+-rw-rw-rw-   0        0        0     1755 2023-07-26 12:46:08.000000 uniparser-erzya-1.1.3/uniparser_erzya/data_strict/bad_analyses.txt
+-rw-rw-rw-   0        0        0        0 2023-07-26 14:06:20.000000 uniparser-erzya-1.1.3/uniparser_erzya/data_strict/lex_rules.txt
+-rw-rw-rw-   0        0        0  4481737 2023-07-26 14:06:20.000000 uniparser-erzya-1.1.3/uniparser_erzya/data_strict/lexemes.txt
+-rw-rw-rw-   0        0        0    96069 2023-07-26 14:06:20.000000 uniparser-erzya-1.1.3/uniparser_erzya/data_strict/paradigms.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 14:19:53.172539 uniparser-erzya-1.1.3/uniparser_erzya.egg-info/
+-rw-rw-rw-   0        0        0     4165 2023-07-26 14:19:53.000000 uniparser-erzya-1.1.3/uniparser_erzya.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      724 2023-07-26 14:19:53.000000 uniparser-erzya-1.1.3/uniparser_erzya.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 14:19:53.000000 uniparser-erzya-1.1.3/uniparser_erzya.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-07-26 14:19:53.000000 uniparser-erzya-1.1.3/uniparser_erzya.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-26 14:19:53.000000 uniparser-erzya-1.1.3/uniparser_erzya.egg-info/top_level.txt
```

### Comparing `uniparser-erzya-1.1.2/LICENSE` & `uniparser-erzya-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `uniparser-erzya-1.1.2/PKG-INFO` & `uniparser-erzya-1.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: uniparser-erzya
-Version: 1.1.2
+Version: 1.1.3
 Summary: Rule-based morphological analysis for Erzya
 Home-page: https://github.com/timarkh/uniparser-grammar-erzya
 Author: Timofey Arkhangelskiy
 Author-email: timarkh@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/timarkh/uniparser-grammar-erzya/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -60,9 +58,7 @@
 Disambiguation is not yet available for this language.
 
 ### Word lists
 Alternatively, you can use a preprocessed word list. The ``wordlists`` directory contains a list of words from a 2.3-million-word [Erzya corpus](http://erzya.web-corpora.net/) (``wordlist_main.csv``), list of analyzed tokens (``wordlist_analyzed.txt``; each line contains all possible analyses for one word in an XML format), and list of tokens the parser could not analyze (``wordlist_unanalyzed.txt``). The recall of the analyzer is 93.6% on literary texts and 90.7% on social media texts.
 
 ## Description format
 The description is carried out in the ``uniparser-morph`` format and involves a description of the inflection (paradigms.txt), a grammatical dictionary (kpv_lexemes_XXX.txt files), a list of rules that annotate combinations of lexemes and grammatical values with additional Russian translations (lex_rules.txt), and a short list of analyses that should be avoided (bad_analyses.txt). The dictionary contains descriptions of individual lexemes, each of which is accompanied by information about its stem, its part-of-speech tag and some other grammatical/borrowing information, its inflectional type (paradigm), and Russian translation. See more about the format [in the uniparser-morph documentation](https://uniparser-morph.readthedocs.io/en/latest/format.html).
-
-
```

### Comparing `uniparser-erzya-1.1.2/README.md` & `uniparser-erzya-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `uniparser-erzya-1.1.2/setup.cfg` & `uniparser-erzya-1.1.3/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2075 6e69 7061 7273 6572 2d65 727a   = uniparser-erz
 00000020: 7961 0d0a 7665 7273 696f 6e20 3d20 312e  ya..version = 1.
-00000030: 312e 320d 0a61 7574 686f 7220 3d20 5469  1.2..author = Ti
+00000030: 312e 330d 0a61 7574 686f 7220 3d20 5469  1.3..author = Ti
 00000040: 6d6f 6665 7920 4172 6b68 616e 6765 6c73  mofey Arkhangels
 00000050: 6b69 790d 0a61 7574 686f 725f 656d 6169  kiy..author_emai
 00000060: 6c20 3d20 7469 6d61 726b 6840 676d 6169  l = timarkh@gmai
 00000070: 6c2e 636f 6d0d 0a64 6573 6372 6970 7469  l.com..descripti
 00000080: 6f6e 203d 2052 756c 652d 6261 7365 6420  on = Rule-based 
 00000090: 6d6f 7270 686f 6c6f 6769 6361 6c20 616e  morphological an
 000000a0: 616c 7973 6973 2066 6f72 2045 727a 7961  alysis for Erzya
```

### Comparing `uniparser-erzya-1.1.2/uniparser_erzya/__init__.py` & `uniparser-erzya-1.1.3/uniparser_erzya/__init__.py`

 * *Files identical despite different names*

### Comparing `uniparser-erzya-1.1.2/uniparser_erzya/data_nodiacritics/bad_analyses.txt` & `uniparser-erzya-1.1.3/uniparser_erzya/data_nodiacritics/bad_analyses.txt`

 * *Files identical despite different names*

### Comparing `uniparser-erzya-1.1.2/uniparser_erzya/data_nodiacritics/lexemes.txt` & `uniparser-erzya-1.1.3/uniparser_erzya/data_nodiacritics/lexemes.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5112,14 +5112,22 @@
  lex: Артемьевна
  stem: артемьевна.
  gramm: N,PN,patrn
  paradigm: N-back
  trans_ru: Артемьевна
 
 -lexeme
+ lex: Артип
+ gramm: N,PN,persn
+ stem: артип.
+ paradigm: N-front
+ paradigm: N-back
+ trans_ru: Артип (Архип)
+
+-lexeme
  lex: Артистов
  stem: артистов.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Артистов
 
 -lexeme
@@ -5658,14 +5666,22 @@
  lex: Атюрьева
  stem: атюрьева.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Атюрьева
 
 -lexeme
+ lex: Атямарькин
+ gramm: N,PN,famn
+ stem: атямарькин.
+ paradigm: N-front
+ paradigm: N-back
+ trans_ru: Атямарькин
+
+-lexeme
  lex: Атяшева
  stem: атяшева.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Атяшева
 
 -lexeme
@@ -15333,14 +15349,28 @@
  lex: Гаруда
  stem: гаруда.
  gramm: N,PN
  paradigm: N-back
  trans_ru: Гаруда
 
 -lexeme
+ lex: Гаруз
+ gramm: N,persn,PN
+ stem: гаруз.
+ paradigm: N-back
+ trans_ru: Гарузов
+
+-lexeme
+ lex: Гарузов
+ gramm: N,famn,PN
+ stem: гарузов.
+ paradigm: N-back
+ trans_ru: Гарузов
+
+-lexeme
  lex: Гаспаров
  stem: гаспаров.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Гаспаров
 
 -lexeme
@@ -17034,14 +17064,22 @@
  lex: Гостехнадзор
  stem: гостехнадзор.
  gramm: N,PN
  paradigm: N-back
  trans_ru: Гостехнадзор
 
 -lexeme
+ lex: Гостя
+ gramm: N,PN,persn
+ stem: гостя.
+ paradigm: N-front
+ paradigm: N-back
+ trans_ru: Гостя (Костя)
+
+-lexeme
  lex: Готович
  stem: готович.
  gramm: N,PN,patrn
  paradigm: N-front
  trans_ru: Готович
 
 -lexeme
@@ -22321,14 +22359,22 @@
  lex: Занчарова
  stem: занчарова.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Занчарова
 
 -lexeme
+ lex: Заня
+ gramm: N,PN,persn
+ stem: заня.
+ paradigm: N-front
+ paradigm: N-back
+ trans_ru: Заня (Захар)
+
+-lexeme
  lex: Заполярье
  stem: заполярье.
  gramm: N,PN,topn
  paradigm: N-front
  trans_ru: Заполярье
 
 -lexeme
@@ -26634,14 +26680,21 @@
  lex: Кандаумов
  stem: кандаумов.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Кандаумов
 
 -lexeme
+ lex: Кандра
+ gramm: N,persn,PN
+ stem: кандра.
+ paradigm: N-back
+ trans_ru: Кандра (Кондрат)
+
+-lexeme
  lex: Каневский
  stem: каневски.
  gramm: N,PN,famn
  paradigm: N-front-j
  trans_ru: Каневский
 
 -lexeme
@@ -32991,14 +33044,21 @@
  lex: Лааксо
  stem: лааксо.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Лааксо
 
 -lexeme
+ lex: Лабырь
+ gramm: N,PN,persn
+ stem: лабыр.
+ paradigm: N-front-soft
+ trans_ru: Лабырь
+
+-lexeme
  lex: Лаванов
  stem: лаванов.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Лаванов
 
 -lexeme
@@ -36946,14 +37006,22 @@
  lex: Матросов
  stem: матросов.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Матросов
 
 -lexeme
+ lex: Матря
+ gramm: N,persn,PN
+ stem: матря.
+ paradigm: N-front
+ paradigm: N-back
+ trans_ru: Матря (Матрёна)
+
+-lexeme
  lex: Матрёна
  stem: матрёна.//матрена.
  gramm: N,PN,persn
  paradigm: N-back
  trans_ru: Матрёна
 
 -lexeme
@@ -36967,14 +37035,22 @@
  lex: Матюшенко
  stem: матюшенко.//матюшеҥко.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Матюшенко
 
 -lexeme
+ lex: Матя
+ gramm: N,PN,persn
+ stem: матя.
+ paradigm: N-front
+ paradigm: N-back
+ trans_ru: Матя (Матрёна)
+
+-lexeme
  lex: Махметов
  stem: махметов.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Махметов
 
 -lexeme
@@ -40638,14 +40714,21 @@
  lex: Найдёнков
  stem: найдёнков.//найденков.//найдёҥков.//найдеҥков.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Найдёнков
 
 -lexeme
+ lex: Найман
+ gramm: N,topn,PN
+ stem: найман.
+ paradigm: N-back
+ trans_ru: Найманы
+
+-lexeme
  lex: Наймушин
  stem: наймушин.
  gramm: N,PN,famn
  paradigm: N-front
  trans_ru: Наймушин
 
 -lexeme
@@ -43151,14 +43234,21 @@
  lex: Олда
  gramm: N,persn,PN
  stem: олда.
  paradigm: N-front
  trans_ru: Олда
 
 -lexeme
+ lex: Олдай
+ gramm: N,persn,PN
+ stem: олда.
+ paradigm: N-front-j
+ trans_ru: Олдай (Авдотья)
+
+-lexeme
  lex: Олег
  stem: олег.
  gramm: N,PN,persn
  paradigm: N-front
  trans_ru: Олег
 
 -lexeme
@@ -44527,22 +44617,15 @@
  trans_ru: Пархоменко
 
 -lexeme
  lex: Парынза
  gramm: N,PN,topn
  stem: парынза.
  paradigm: N-back
- trans_ru: Чёрная промза (село; название музыкального коллектива)
-
--lexeme
- lex: Парынза
- gramm: N,PN,topn
- stem: парынза.
- paradigm: N-front
- trans_ru: Чёрная промза (село; название музыкального коллектива)
+ trans_ru: Чёрная Промза (село; название музыкального коллектива)
 
 -lexeme
  lex: Пастернак
  stem: пастернак.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Пастернак
@@ -44649,14 +44732,22 @@
  lex: Пахмутова
  stem: пахмутова.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Пахмутова
 
 -lexeme
+ lex: Пахом
+ gramm: N,persn,PN
+ stem: пахом.
+ paradigm: N-front
+ paradigm: N-back
+ trans_ru: Пахом
+
+-lexeme
  lex: Пахомов
  stem: пахомов.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Пахомов
 
 -lexeme
@@ -51265,14 +51356,22 @@
  lex: Салдаева
  stem: салдаева.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Салдаева
 
 -lexeme
+ lex: Салдин
+ gramm: N,famn,PN
+ stem: салдин.
+ paradigm: N-front
+ paradigm: N-back
+ trans_ru: Салдин
+
+-lexeme
  lex: Салехард
  stem: салехард.
  gramm: N,PN,topn
  paradigm: N-back
  trans_ru: Салехард
 
 -lexeme
@@ -51636,14 +51735,21 @@
  lex: Самойлова
  stem: самойлова.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Самойлова
 
 -lexeme
+ lex: Самойловна
+ gramm: N,PN,patrn
+ stem: самойловна.
+ paradigm: N-back
+ trans_ru: Самойловна
+
+-lexeme
  lex: Самоленко
  stem: самоленко.//самолеҥко.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Самоленко
 
 -lexeme
@@ -55633,14 +55739,22 @@
  lex: Студитских
  stem: студитских.
  gramm: N,PN,famn
  paradigm: N-front
  trans_ru: Студитских
 
 -lexeme
+ lex: Стяпан
+ gramm: N,persn,PN
+ stem: стяпан.
+ paradigm: N-front
+ paradigm: N-back
+ trans_ru: Степан
+
+-lexeme
  lex: Стёпа
  stem: стёпа.//степа.
  gramm: N,PN,persn
  paradigm: N-back
  trans_ru: Стёпа
 
 -lexeme
@@ -73165,14 +73279,21 @@
  lex: алкине
  stem: алкине.
  gramm: A,dim
  paradigm: A-front
  trans_ru: низкорослый
 
 -lexeme
+ lex: алкинестэ
+ gramm: ADV
+ stem: алкинестэ.
+ paradigm: Clitics
+ trans_ru: низко; неглубоко
+
+-lexeme
  lex: алкиньгадомс
  stem: алкиньга.
  gramm: V
  paradigm: V-do
  trans_ru: снизиться, осесть
 
 -lexeme
@@ -73306,14 +73427,21 @@
  stem: алнэ.
  gramm: N,dim
  paradigm: N-front
  trans_ru: личинка
 
 -lexeme
  lex: ало
+ gramm: A
+ stem: ало.
+ paradigm: A-back
+ trans_ru: нижний
+
+-lexeme
+ lex: ало
  stem: ало.
  gramm: ADV
  paradigm: Clitics
  trans_ru: внизу
 
 -lexeme
  lex: ало
@@ -74941,14 +75069,21 @@
  stem: апаркст.
  gramm: V
  paradigm: V-o
  trans_ru: расстроиться
 
 -lexeme
  lex: апаро
+ gramm: ADV
+ stem: апаро.
+ paradigm: Clitics
+ trans_ru: неприятно
+
+-lexeme
+ lex: апаро
  stem: апаро.
  gramm: A
  paradigm: A-back
  trans_ru: нехороший
 
 -lexeme
  lex: апаро
@@ -78550,14 +78685,21 @@
  stem: банкет.//банькет.//баҥкет.
  gramm: N,rus
  paradigm: N-front
  paradigm: N-back
  trans_ru: банкет
 
 -lexeme
+ lex: банкине
+ gramm: N,rus,dim
+ stem: банкине.
+ paradigm: N-front
+ trans_ru: баночка
+
+-lexeme
  lex: банкир
  stem: банкир.//банькир.//баҥкир.//банькир.
  gramm: N,rus,anim,hum
  paradigm: N-front
  trans_ru: банкир
 
 -lexeme
@@ -78594,14 +78736,21 @@
  stem: баннер.
  gramm: N,rus
  paradigm: N-back
  paradigm: N-front
  trans_ru: баннер
 
 -lexeme
+ lex: банок
+ gramm: A,rus
+ stem: банок.
+ paradigm: A-back
+ trans_ru: банка
+
+-lexeme
  lex: бант
  stem: бант.
  gramm: N,rus
  paradigm: N-back
  trans_ru: бант
 
 -lexeme
@@ -79480,14 +79629,21 @@
  lex: бедной
  stem: бедно.//бѣдно.
  gramm: A,rus
  paradigm: A-front-j
  trans_ru: бедный
 
 -lexeme
+ lex: беднойчи
+ gramm: N,rus
+ stem: беднойчи.
+ paradigm: N-front
+ trans_ru: бедность
+
+-lexeme
  lex: беднота
  stem: беднота.
  gramm: N,rus
  paradigm: N-back
  trans_ru: беднота
 
 -lexeme
@@ -80699,14 +80855,22 @@
  lex: бизьганя
  stem: бизьганя.
  gramm: N
  paradigm: N-back
  trans_ru: волчья ягода
 
 -lexeme
+ lex: бизьгатаев
+ gramm: A
+ stem: бизьгатаев.
+ paradigm: A-front
+ paradigm: A-back
+ trans_ru: веснушчатый
+
+-lexeme
  lex: бийнемс
  stem: бийн.//бійн.
  gramm: V
  paradigm: V-ye
  trans_ru: пищать
 
 -lexeme
@@ -81535,14 +81699,21 @@
  lex: бобаске
  stem: бобаске.|бобаск.
  gramm: N
  paradigm: N-front
  trans_ru: сказка
 
 -lexeme
+ lex: бобка
+ gramm: N,rus
+ stem: бобка.
+ paradigm: N-back
+ trans_ru: боб
+
+-lexeme
  lex: бобо
  stem: бобо.
  gramm: N
  paradigm: N-back
  trans_ru: пугало
 
 -lexeme
@@ -82691,14 +82862,21 @@
  lex: братик
  stem: братик.
  gramm: N,rus,anim,hum
  paradigm: N-front
  trans_ru: братик
 
 -lexeme
+ lex: братиники
+ gramm: N,rus,anim,hum
+ stem: братиники.
+ paradigm: N-front
+ trans_ru: братья
+
+-lexeme
  lex: братишка
  stem: братишка.
  gramm: N,rus,anim,hum
  paradigm: N-back
  trans_ru: братишка
 
 -lexeme
@@ -84721,19 +84899,26 @@
  lex: вакан
  stem: вакан.
  gramm: N
  paradigm: N-back
  trans_ru: кваканье
 
 -lexeme
+ lex: вакан
+ stem: вакан.
+ gramm: N
+ paradigm: N-back
+ trans_ru: миска
+
+-lexeme
  lex: ваканнэ
  stem: ваканнэ.
- gramm: N
+ gramm: N,dim
  paradigm: N-front
- trans_ru: миска
+ trans_ru: мисочка
 
 -lexeme
  lex: вакансия
  stem: вакансия.//вакансія.
  gramm: N,rus
  paradigm: N-back
  trans_ru: вакансия
@@ -84753,15 +84938,22 @@
  trans_ru: квакать
 
 -lexeme
  lex: вакс
  stem: вакс.
  gramm: N
  paradigm: N-back
- trans_ru: вершок; возле, к, около
+ trans_ru: вершок
+
+-lexeme
+ lex: вакс
+ stem: вакс.
+ gramm: N,rel_n
+ paradigm: N-back
+ trans_ru: возле, к, около
 
 -lexeme
  lex: вакснэ
  stem: вакснэ.
  gramm: POST
  paradigm: Clitics
  trans_ru: рядом
@@ -88346,14 +88538,22 @@
  stem: вельдерьма.
  gramm: N
  paradigm: N-back
  trans_ru: дымоход
 
 -lexeme
  lex: велькс
+ gramm: N
+ stem: велькс.
+ paradigm: N-front
+ paradigm: N-back
+ trans_ru: верхняя часть чего-либо
+
+-lexeme
+ lex: велькс
  stem: велькс.
  gramm: N
  paradigm: N-front
  trans_ru: навес, одеяло; сливки, сметана
 
 -lexeme
  lex: велькска
@@ -88869,14 +89069,21 @@
  stem: верде.|верд.
  gramm: ADV
  paradigm: Clitics
  trans_ru: сверху
 
 -lexeme
  lex: вере
+ gramm: A
+ stem: вере.
+ paradigm: A-front
+ trans_ru: верхний
+
+-lexeme
+ lex: вере
  stem: вере.
  gramm: ADV
  paradigm: Clitics
  trans_ru: наверху, сверху
 
 -lexeme
  lex: верев
@@ -96954,14 +97161,22 @@
  lex: гренадёр
  stem: гренадёр.//гренадер.//гренадер.
  gramm: N,rus,anim,hum
  paradigm: N-back
  trans_ru: гренадёр
 
 -lexeme
+ lex: грех
+ gramm: N,rus
+ stem: грех.
+ paradigm: N-front
+ paradigm: N-back
+ trans_ru: грех
+
+-lexeme
  lex: грецкой
  stem: грецко.
  gramm: A,rus
  paradigm: A-front-j
  trans_ru: грецкий
 
 -lexeme
@@ -97575,14 +97790,21 @@
  lex: гурсо
  stem: гурсо.
  gramm: IMIT
  paradigm: Clitics
  trans_ru: хорошо (гореть)
 
 -lexeme
+ lex: гурьба
+ gramm: N,rus
+ stem: гурьба.
+ paradigm: N-back
+ trans_ru: гурьба
+
+-lexeme
  lex: гурямс
  stem: гур.
  gramm: V
  paradigm: V-ya
  trans_ru: водить в прятки, прятаться
 
 -lexeme
@@ -102182,14 +102404,21 @@
  lex: егошихинской
  stem: егошихинско.
  gramm: A,rus
  paradigm: A-front-j
  trans_ru: егошихинский
 
 -lexeme
+ lex: едак
+ gramm: N,rus
+ stem: едак.
+ paradigm: N-back
+ trans_ru: едок
+
+-lexeme
  lex: единица
  stem: единица.
  gramm: N,rus
  paradigm: N-back
  trans_ru: единица
 
 -lexeme
@@ -103367,14 +103596,21 @@
  lex: забытой
  stem: забыто.
  gramm: A,rus
  paradigm: A-front-j
  trans_ru: забытый
 
 -lexeme
+ lex: завалинка
+ gramm: N,rus
+ stem: завалинка.
+ paradigm: N-back
+ trans_ru: завалинка
+
+-lexeme
  lex: заведения
  stem: заведения.//заведение.//заведения.//заведеніе.
  gramm: N,rus
  paradigm: N-back
  paradigm: N-front
  trans_ru: заведение
 
@@ -105089,14 +105325,21 @@
  lex: знярс
  stem: знярс.
  gramm: ADVPRO
  paradigm: Clitics
  trans_ru: сколько
 
 -lexeme
+ lex: знярыя
+ gramm: ADVPRO
+ stem: знярыя.
+ paradigm: Clitics
+ trans_ru: столько
+
+-lexeme
  lex: зобня
  stem: зобня.
  gramm: N,body
  paradigm: N-back
  trans_ru: желудок
 
 -lexeme
@@ -106531,14 +106774,21 @@
  stem: икеле.
  gramm: ADV
  paradigm: Clitics
  trans_ru: впереди; раньше
 
 -lexeme
  lex: икеле
+ stem: икеле.
+ gramm: POST
+ paradigm: Clitics
+ trans_ru: перед, напротив; до
+
+-lexeme
+ lex: икеле
  stem: икеле.|икель.
  gramm: N,rel_n
  paradigm: N-front
  trans_ru: впереди; раньше
 
 -lexeme
  lex: икелевал
@@ -111894,14 +112144,21 @@
  lex: камфорной
  stem: камфорно.
  gramm: A,rus
  paradigm: A-front-j
  trans_ru: камфорный
 
 -lexeme
+ lex: камчадал
+ gramm: N,rus
+ stem: камчадал.
+ paradigm: N-back
+ trans_ru: камчадал
+
+-lexeme
  lex: камыш
  stem: камыш.
  gramm: N,rus
  paradigm: N-back
  trans_ru: камыш
 
 -lexeme
@@ -112540,14 +112797,21 @@
  lex: каподемс
  stem: капод.
  gramm: V
  paradigm: V-ye
  trans_ru: схватить, уцепиться
 
 -lexeme
+ lex: капоемс
+ gramm: V,intr
+ stem: капо.
+ paradigm: V-ye
+ trans_ru: многокр. к схватить, уцепиться
+
+-lexeme
  lex: капор
  stem: капор.
  gramm: N,rus
  paradigm: N-back
  trans_ru: капор
 
 -lexeme
@@ -113339,14 +113603,21 @@
  lex: каркс
  stem: каркс.
  gramm: N
  paradigm: N-back
  trans_ru: бандаж, пояс
 
 -lexeme
+ lex: карксамга
+ gramm: ADV
+ stem: карксамга.
+ paradigm: Clitics
+ trans_ru: по пояс
+
+-lexeme
  lex: карксамопель
  stem: карксамопел.
  gramm: N
  paradigm: N-front-soft
  trans_ru: кушак, пояс
 
 -lexeme
@@ -114029,14 +114300,21 @@
  lex: касовкске
  stem: касовкске.
  gramm: N,dim
  paradigm: N-front
  trans_ru: растеньице
 
 -lexeme
+ lex: касоль
+ gramm: N,rus
+ stem: касол.
+ paradigm: N-front-soft
+ trans_ru: фасоль
+
+-lexeme
  lex: касом
  stem: касом.
  gramm: N
  paradigm: N-back
  trans_ru: пробор в волосах
 
 -lexeme
@@ -114725,14 +115003,21 @@
  lex: качоловажа
  stem: качоловажа.
  gramm: N,body
  paradigm: N-back
  trans_ru: бедренная кость
 
 -lexeme
+ lex: каша
+ gramm: N,rus
+ stem: каша.
+ paradigm: N-back
+ trans_ru: каша
+
+-lexeme
  lex: кашамс
  stem: каш.
  gramm: V
  paradigm: V-a
  trans_ru: запорошить
 
 -lexeme
@@ -117876,15 +118161,15 @@
  stem: кие.//кіе.
  gramm: PRO,nom,sg
  paradigm: Clitics
  trans_ru: кто
 
 -lexeme
  lex: кие-бути
- stem: кие-бути//кіе-бути
+ stem: кие.-бути//кіе.-бути
  gramm: PRO,nom,sg
  paradigm: Clitics
  trans_ru: кто-нибудь, кто-то
 
 -lexeme
  lex: кие-кие
  stem: кие-кие.//кие-кіе.
@@ -121046,14 +121331,21 @@
  lex: козомс
  stem: коз.
  gramm: V
  paradigm: V-o
  trans_ru: кашлять
 
 -lexeme
+ lex: козонь
+ gramm: ADVPRO
+ stem: козонь.
+ paradigm: Clitics
+ trans_ru: где, куда
+
+-lexeme
  lex: козылька
  stem: козылька.
  gramm: N
  paradigm: N-back
  trans_ru: череда
 
 -lexeme
@@ -121629,14 +121921,21 @@
  lex: колесница
  stem: колесница.
  gramm: N,rus,transport
  paradigm: N-back
  trans_ru: колесница
 
 -lexeme
+ lex: коли
+ gramm: CONJ,rus
+ stem: коли.
+ paradigm: Clitics
+ trans_ru: коли, если
+
+-lexeme
  lex: количественной
  stem: количественно.
  gramm: A,rus
  paradigm: A-front-j
  trans_ru: количественный
 
 -lexeme
@@ -125282,14 +125581,21 @@
  lex: кортавкске
  stem: кортавкске.
  gramm: N,dim
  paradigm: N-front
  trans_ru: разговорчик
 
 -lexeme
+ lex: кортавомс
+ gramm: V,intr
+ stem: кортав.
+ paradigm: V-o
+ trans_ru: возм. к говорить
+
+-lexeme
  lex: кортавт
  stem: кортавт.
  gramm: N
  paradigm: N-back
  trans_ru: разговор; слухи
 
 -lexeme
@@ -127871,14 +128177,21 @@
  lex: куваня
  stem: куваня.
  gramm: ADVPRO
  paradigm: Clitics
  trans_ru: где
 
 -lexeme
+ lex: куватень
+ gramm: A
+ stem: куватен.
+ paradigm: A-front-soft
+ trans_ru: долгий
+
+-lexeme
  lex: кувать
  stem: кувать.
  gramm: ADV
  paradigm: Clitics
  trans_ru: долго
 
 -lexeme
@@ -131400,14 +131713,21 @@
  lex: лавтовловажа
  stem: лавтовловажа.
  gramm: N,body
  paradigm: N-back
  trans_ru: ключица
 
 -lexeme
+ lex: лавтово
+ gramm: N,body
+ stem: лавтово.
+ paradigm: N-back
+ trans_ru: плечо
+
+-lexeme
  lex: лавтовов
  stem: лавтовов.
  gramm: A
  paradigm: A-back
  trans_ru: плечистый
 
 -lexeme
@@ -138112,14 +138432,22 @@
  stem: магазин.
  gramm: N,rus
  paradigm: N-front
  paradigm: N-back
  trans_ru: в разн. магазин
 
 -lexeme
+ lex: магарыч
+ gramm: N,rus
+ stem: магарыч.
+ paradigm: N-front
+ paradigm: N-back
+ trans_ru: магарыч
+
+-lexeme
  lex: магистерской
  stem: магистерско.
  gramm: A,rus
  paradigm: A-front-j
  trans_ru: магистерский
 
 -lexeme
@@ -141509,14 +141837,21 @@
  stem: межэтническо.
  gramm: A,rus
  paradigm: A-front-j
  trans_ru: межэтнический
 
 -lexeme
  lex: мезде
+ gramm: ADVPRO
+ stem: мезде.
+ paradigm: Clitics
+ trans_ru: за сколько, о чём, кого, чего, за что
+
+-lexeme
+ lex: мезде
  stem: мезде.
  gramm: PRO
  paradigm: Clitics
  trans_ru: за сколько, из-за чего, о чем
 
 -lexeme
  lex: мездеяк
@@ -141648,14 +141983,21 @@
  lex: мейле
  stem: мейле.
  gramm: ADVPRO
  paradigm: Clitics
  trans_ru: затем, после, потом
 
 -lexeme
+ lex: мейле
+ stem: мейле.
+ gramm: POST
+ paradigm: Clitics
+ trans_ru: после
+
+-lexeme
  lex: мейс
  stem: мейс.
  gramm: ADVPRO
  paradigm: Clitics
  trans_ru: почему
 
 -lexeme
@@ -142223,14 +142565,21 @@
  lex: мельпаз
  stem: мельпаз.
  gramm: N,supernat
  paradigm: N-back
  trans_ru: держатель неба
 
 -lexeme
+ lex: мельпаросо
+ gramm: ADV
+ stem: мельпаросо.
+ paradigm: Clitics
+ trans_ru: охотно, с удовольствием
+
+-lexeme
  lex: мельполадкс
  stem: мельполадкс.
  gramm: N
  paradigm: N-back
  trans_ru: статья
 
 -lexeme
@@ -144973,14 +145322,22 @@
  stem: могильник.
  gramm: N,rus
  paradigm: N-front
  paradigm: N-back
  trans_ru: могильник
 
 -lexeme
+ lex: могорыч
+ gramm: N,rus
+ stem: могорыч.
+ paradigm: N-front
+ paradigm: N-back
+ trans_ru: магарыч
+
+-lexeme
  lex: мода
  stem: мода.
  gramm: N
  paradigm: N-back
  trans_ru: земля; территория
 
 -lexeme
@@ -149541,14 +149898,21 @@
  lex: нарошной
  stem: нарошно.
  gramm: A,rus
  paradigm: A-front-j
  trans_ru: нарочный
 
 -lexeme
+ lex: нарсемс
+ gramm: V,intr
+ stem: нарс.
+ paradigm: V-ye
+ trans_ru: многокр. к стричь, брить, стричься, бриться
+
+-lexeme
  lex: нарсуд
  stem: нарсуд.
  gramm: N,rus
  paradigm: N-back
  trans_ru: нарсуд
 
 -lexeme
@@ -150182,14 +150546,21 @@
  stem: нацсобрания.//нацсобрание.//нацсобрания.//нацсобраніе.
  gramm: N,rus
  paradigm: N-back
  paradigm: N-front
  trans_ru: нацсобрание
 
 -lexeme
+ lex: начал
+ gramm: N,rus,anim,hum
+ stem: начал.
+ paradigm: N-back
+ trans_ru: начальник
+
+-lexeme
  lex: началка
  stem: началка.
  gramm: N,rus
  paradigm: N-back
  trans_ru: началка
 
 -lexeme
@@ -153325,14 +153696,21 @@
  lex: ноцкадемс
  stem: ноцкад.
  gramm: V
  paradigm: V-ye
  trans_ru: вырвать, дёрнуть, кольнуть
 
 -lexeme
+ lex: ноцковтнемс
+ gramm: V,tr
+ stem: ноцковтн.
+ paradigm: V-ye
+ trans_ru: многокр. к дёрнуть, вырвать
+
+-lexeme
  lex: ноцковтомс
  stem: ноцковт.
  gramm: V
  paradigm: V-o
  trans_ru: вырвать
 
 -lexeme
@@ -158622,14 +159000,21 @@
  stem: оршамот-карсемат.
  gramm: N
  paradigm: N-back
  trans_ru: одежда и обувь
 
 -lexeme
  lex: оршамс
+ gramm: V,tr
+ stem: оршамо.
+ paradigm: Clitics
+ trans_ru: надеть на себя
+
+-lexeme
+ lex: оршамс
  stem: орш.
  gramm: V
  paradigm: V-a
  trans_ru: надеть; одеться
 
 -lexeme
  lex: оршамс-карсемс
@@ -171327,14 +171712,22 @@
  lex: покой
  stem: поко.
  gramm: N,rus
  paradigm: N-front-j
  trans_ru: покой
 
 -lexeme
+ lex: покойник
+ gramm: N,rus,anim,hum
+ stem: покойник.
+ paradigm: N-front
+ paradigm: N-back
+ trans_ru: покойник
+
+-lexeme
  lex: поколев
  stem: поколев.
  gramm: A
  paradigm: A-front
  trans_ru: комковатый
 
 -lexeme
@@ -174136,14 +174529,21 @@
  lex: потомственной
  stem: потомственно.
  gramm: A,rus
  paradigm: A-front-j
  trans_ru: потомственный
 
 -lexeme
+ lex: потомтнемс
+ gramm: V,intr
+ stem: потомтн.
+ paradigm: V-ye
+ trans_ru: закрываться
+
+-lexeme
  lex: поточной
  stem: поточно.
  gramm: A,rus
  paradigm: A-front-j
  trans_ru: поточный
 
 -lexeme
@@ -174945,14 +175345,21 @@
  lex: праздничной
  stem: празднично.
  gramm: A,rus
  paradigm: A-front-j
  trans_ru: праздничный
 
 -lexeme
+ lex: праздновамс
+ gramm: V,tr,rus
+ stem: празднов.
+ paradigm: V-a
+ trans_ru: праздновать
+
+-lexeme
  lex: празднования
  stem: празднования.//празднование.//празднованія.//празднованіе.
  gramm: N,rus
  paradigm: N-back
  paradigm: N-front
  trans_ru: празднование
 
@@ -179361,14 +179768,21 @@
  lex: пуворямс
  stem: пувор.
  gramm: V
  paradigm: V-ya
  trans_ru: измять, крутить
 
 -lexeme
+ lex: пувсемс
+ gramm: V,intr
+ stem: пувс.
+ paradigm: V-ye
+ trans_ru: многокр. к дуть, подуть, веять, развеять
+
+-lexeme
  lex: пувтамс
  stem: пувт.
  gramm: V
  paradigm: V-a
  trans_ru: разбудить
 
 -lexeme
@@ -184878,14 +185292,21 @@
  lex: риснемс
  stem: рисн.
  gramm: V
  paradigm: V-ye
  trans_ru: излучать, литься, моросить
 
 -lexeme
+ lex: рисовавкс
+ gramm: N,rus
+ stem: рисовавкс.
+ paradigm: N-back
+ trans_ru: рисунок
+
+-lexeme
  lex: рисовамс
  stem: рисов.
  gramm: V
  paradigm: V-a
  trans_ru: нарисовать
 
 -lexeme
@@ -186638,14 +187059,21 @@
  lex: саевть
  stem: саевт.
  gramm: A
  paradigm: A-front-soft
  trans_ru: взятый
 
 -lexeme
+ lex: саезь
+ gramm: POST
+ stem: саезь.
+ paradigm: Clitics
+ trans_ru: с
+
+-lexeme
  lex: саема
  stem: саема.
  gramm: N
  paradigm: N-back
  trans_ru: взятие, вычет
 
 -lexeme
@@ -187923,14 +188351,21 @@
  stem: сас.
  gramm: V
  paradigm: V-a
  trans_ru: гнаться, догнать
 
 -lexeme
  lex: састо
+ gramm: ADV
+ stem: састо.
+ paradigm: Clitics
+ trans_ru: тихо, негромко
+
+-lexeme
+ lex: састо
  stem: састо.|саст.
  gramm: A
  paradigm: A-back
  trans_ru: медленный, негромкий, тихий
 
 -lexeme
  lex: састыне
@@ -193718,14 +194153,21 @@
  lex: содазь
  stem: содазь.
  gramm: ADV
  paradigm: Clitics
  trans_ru: известно; сознательно
 
 -lexeme
+ lex: содамо
+ stem: содамо.
+ gramm: N,anim,hum
+ paradigm: N-back
+ trans_ru: зять
+
+-lexeme
  lex: содамоаравкс
  stem: содамоаравкс.
  gramm: N
  paradigm: N-back
  trans_ru: задача
 
 -lexeme
@@ -197086,14 +197528,21 @@
  lex: стопка
  stem: стопка.
  gramm: N,rus
  paradigm: N-back
  trans_ru: стопка
 
 -lexeme
+ lex: стопкине
+ gramm: N,dim,rus
+ stem: стопкине.
+ paradigm: N-front
+ trans_ru: стопка
+
+-lexeme
  lex: сторож
  stem: сторож.
  gramm: N,rus,anim,hum
  paradigm: N-back
  trans_ru: сторож
 
 -lexeme
@@ -197459,14 +197908,21 @@
  lex: струнной
  stem: струнно.
  gramm: A,rus
  paradigm: A-front-j
  trans_ru: струнный
 
 -lexeme
+ lex: струя
+ gramm: N,rus
+ stem: струя.
+ paradigm: N-back
+ trans_ru: струя
+
+-lexeme
  lex: стряпавкс
  stem: стряпавкс.
  gramm: N,rus
  paradigm: N-back
  trans_ru: стряпня
 
 -lexeme
@@ -201333,14 +201789,21 @@
  stem: сёксен.//сексен.
  gramm: A
  paradigm: A-front-soft
  trans_ru: осенний, осенниё
 
 -lexeme
  lex: сёксня
+ gramm: ADV
+ stem: сексня.
+ paradigm: Clitics
+ trans_ru: осенью
+
+-lexeme
+ lex: сёксня
  stem: сёксня.//сексня.
  gramm: ADV
  paradigm: Clitics
  trans_ru: осенью
 
 -lexeme
  lex: сёксь
@@ -203229,14 +203692,21 @@
  lex: тарнышка
  stem: тарнышка.
  gramm: N,anim,hum
  paradigm: N-back
  trans_ru: торопыга
 
 -lexeme
+ lex: тарск
+ gramm: IMIT
+ stem: тарск.
+ paradigm: Clitics
+ trans_ru: вздрогнуть (тарск теемс)
+
+-lexeme
  lex: тарскадемс
  stem: тарскад.
  gramm: V
  paradigm: V-ye
  trans_ru: вздрогнуть
 
 -lexeme
@@ -213511,14 +213981,21 @@
  lex: урямо
  stem: урямо.
  gramm: N
  paradigm: N-back
  trans_ru: тальник
 
 -lexeme
+ lex: уса
+ gramm: N,rus,body
+ stem: уса.
+ paradigm: N-back
+ trans_ru: усы
+
+-lexeme
  lex: усад
  stem: усад.
  gramm: N,rus
  paradigm: N-back
  trans_ru: усадьба
 
 -lexeme
@@ -217517,14 +217994,21 @@
  lex: хартия
  stem: хартия.//хартія.
  gramm: N,rus
  paradigm: N-back
  trans_ru: хартия
 
 -lexeme
+ lex: харч
+ gramm: N,rus
+ stem: харч.
+ paradigm: N-back
+ trans_ru: харч
+
+-lexeme
  lex: харчо
  stem: харчо.
  gramm: N,rus
  paradigm: N-back
  trans_ru: харчо
 
 -lexeme
@@ -219417,14 +219901,21 @@
  lex: цилик-пулик
  stem: цилик-пулик.
  gramm: IMIT
  paradigm: Clitics
  trans_ru: об игре на струнах
 
 -lexeme
+ lex: цилим
+ stem: цилим.
+ gramm: N
+ paradigm: N-front
+ trans_ru: курительная трубка
+
+-lexeme
  lex: цилимпей
  stem: цилимпе.
  gramm: N,body
  paradigm: N-front-j
  trans_ru: зуб мудрости
 
 -lexeme
@@ -220253,14 +220744,21 @@
  lex: цюцев
  stem: цюцев.
  gramm: N
  paradigm: N-front
  trans_ru: вершина (дерева); гроздь, кисть, соцветие
 
 -lexeme
+ lex: цюцка
+ gramm: N
+ stem: цюцка.
+ paradigm: N-back
+ trans_ru: гроздь, кисть (плодов, ягод)
+
+-lexeme
  lex: цюцёв
  stem: цюцёв.//цюцев.
  gramm: N
  paradigm: N-back
  trans_ru: гроздья, кисти; серёжки
 
 -lexeme
@@ -221283,14 +221781,21 @@
  lex: чалгсемс
  stem: чалгс.
  gramm: V
  paradigm: V-ye
  trans_ru: топтать
 
 -lexeme
+ lex: чалксемс
+ gramm: V,tr
+ stem: чалкс.
+ paradigm: V-ye
+ trans_ru: многокр. к наступить, мять
+
+-lexeme
  lex: чалма
  stem: чалма.
  gramm: N,rus
  paradigm: N-back
  trans_ru: чалма
 
 -lexeme
@@ -222211,18 +222716,18 @@
  stem: чевельд.
  gramm: V
  paradigm: V-ya
  trans_ru: примять, раздавить
 
 -lexeme
  lex: чевелямс
- stem: чевел.
+ stem: чевел.//чевил.
  gramm: V
  paradigm: V-ya
- trans_ru: жевать (о беззубых)
+ trans_ru: мять, жевать (о беззубых)
 
 -lexeme
  lex: чевкс
  stem: чевкс.
  gramm: N
  paradigm: N-front
  trans_ru: сухое полено для лучин
```

### Comparing `uniparser-erzya-1.1.2/uniparser_erzya/data_nodiacritics/paradigms.txt` & `uniparser-erzya-1.1.3/uniparser_erzya/data_nodiacritics/paradigms.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2306,18 +2306,22 @@
   paradigm: V-ye-proper
   paradigm: V-e-proper
 
 
 -paradigm: V-a-proper
  -flex: .<.>
   gramm: non_obj
-  paradigm: V-npst-a
   paradigm: V-pst-a
+ -flex: .<.>
+  gramm: non_obj,npst
+  paradigm: V-npst-a
  -flex: .[а]<.>
+  gramm: npst
   paradigm: V-npst-obj
+ -flex: .[а]<.>
   paradigm: V-opt
   paradigm: V-imp-back
  -flex: .[а]<.>
   gramm: neg
   paradigm: Clitics
  -flex: .[а]з<.>
   gramm: ptcp.pst
@@ -2436,19 +2440,23 @@
  -flex: .[а]м|га<.>
   gramm: cvb.caus
   gloss: NMLZ|PROL
   paradigm: N-poss-back-vowel
 
 -paradigm: V-ya-proper
  -flex: .<.>
-  gramm: non_obj
+  gramm: non_obj,npst
   paradigm: V-npst-ya
+ -flex: .<.>
+  gramm: non_obj
   paradigm: V-pst-ya
  -flex: .[я]<.>
+  gramm: npst
   paradigm: V-npst-obj
+ -flex: .[я]<.>
   paradigm: V-imp-back
   paradigm: V-opt
  -flex: .[я]<.>
   gramm: neg
   paradigm: Clitics
  -flex: .[я]з<.>
   gramm: ptcp.pst
@@ -2526,25 +2534,32 @@
  -flex: .[я]м|га<.>
   gramm: cvb.caus
   gloss: NMLZ|PROL
   paradigm: N-poss-back-vowel
 
 -paradigm: V-o-proper
  -flex: .<.>
-  gramm: non_obj
+  gramm: non_obj,npst
   paradigm: V-npst-o
+ -flex: .<.>
+  gramm: non_obj
   paradigm: V-opt-o
   paradigm: V-pst-o
  -flex: .о<.>//.<.>
+  gramm: npst
   paradigm: V-npst-obj
+ -flex: .о<.>//.<.>
   paradigm: V-imp-back
  -flex: .а<.>//.<.>
-  gramm: missp
+  gramm: npst,missp
   regex-prev: ^(ловн|ванст)[<>.]*$
   paradigm: V-npst-obj
+ -flex: .а<.>//.<.>
+  gramm: missp
+  regex-prev: ^(ловн|ванст)[<>.]*$
   paradigm: V-imp-back
  -flex: .о<.>//.<.>
   gramm: neg
   paradigm: Clitics
  -flex: .оз<.>
   gramm: ptcp.pst
   gloss: PTCP.PST
@@ -2662,23 +2677,29 @@
  -flex: .ом|га<.>
   gramm: cvb.caus
   gloss: NMLZ|PROL
   paradigm: N-poss-back-vowel
 
 -paradigm: V-yo-proper
  -flex: .<.>
-  gramm: non_obj
+  gramm: non_obj,npst
   paradigm: V-npst-ye
+ -flex: .<.>
+  gramm: non_obj
   paradigm: V-opt-ye
   paradigm: V-pst-ye
  -flex: .ё<.>//.е<.>//.[ь]<.>
+  gramm: npst
   paradigm: V-npst-obj
+ -flex: .ё<.>//.е<.>//.[ь]<.>
   paradigm: V-imp-back
  -flex: .<.>
+  gramm: npst
   paradigm: V-npst-obj
+ -flex: .<.>
   paradigm: V-imp-front
   regex-next: ^[<>.]*[дт][ьеи].*
  -flex: .ё<.>//.е<.>//.[ь]<.>
   gramm: neg
   paradigm: Clitics
  -flex: .<.>
   paradigm: V-npst-obj
@@ -2762,20 +2783,24 @@
  -flex: .ём|га<.>//.ем|га<.>
   gramm: cvb.caus
   gloss: NMLZ|PROL
   paradigm: N-poss-back-vowel
 
 -paradigm: V-e-proper
  -flex: .<.>
-  gramm: non_obj
+  gramm: non_obj,npst
   paradigm: V-npst-e
+ -flex: .<.>
+  gramm: non_obj
   paradigm: V-opt-e
   paradigm: V-pst-e
  -flex: .э<.>//.<.>
+  gramm: npst
   paradigm: V-npst-obj
+ -flex: .э<.>//.<.>
   paradigm: V-imp-front
  -flex: .э<.>//.<.>
   gramm: neg
   paradigm: Clitics
  -flex: .эз<.>
   gramm: ptcp.pst
   gloss: PTCP.PST
@@ -2897,42 +2922,55 @@
  -flex: .эм|га<.>
   gramm: cvb.caus
   gloss: NMLZ|PROL
   paradigm: N-poss-back-vowel
 
 -paradigm: V-ye-proper
  -flex: .<.>
-  gramm: non_obj
+  gramm: non_obj,npst
   paradigm: V-npst-ye
+  paradigm: V-npst-obj-soft
+ -flex: .<.>
+  gramm: non_obj
   paradigm: V-opt-ye
   paradigm: V-pst-ye
-  paradigm: V-npst-obj-soft
  -flex: .е<.>//.[ь]<.>
+  gramm: npst
   paradigm: V-npst-obj
+ -flex: .е<.>//.[ь]<.>
   paradigm: V-imp-front
  -flex: .и<.>
-  gramm: missp
+  gramm: npst,missp
   paradigm: V-npst-obj
+ -flex: .и<.>
+  gramm: missp
   paradigm: V-imp-front
  -flex: .<.>
+  gramm: npst
   paradigm: V-npst-obj
+  regex-next: ^[<>.]*[дт][ьеи].*
+ -flex: .<.>
   paradigm: V-imp-front
   regex-next: ^[<>.]*[дт][ьеи].*
  -flex: .е<.>//.[ь]<.>
   gramm: neg
   paradigm: Clitics
  -flex: .и<.>
   gramm: neg,missp
   paradigm: Clitics
  -flex: .<.>
   paradigm: V-npst-obj
   regex-prev: (.*[бвгжкмпхчшщ]|^не|^му|^ту)[<>.]*$
  -flex: .[й]<.>
+  gramm: npst
   paradigm: V-npst-obj
   regex-prev: .*[аеёиоуыэюя][<>.]*$
+ -flex: .[й]<.>
+  paradigm: V-imp-front
+  regex-prev: .*[аеёиоуыэюя][<>.]*$
  -flex: .ез<.>
   gramm: ptcp.pst
   gloss: PTCP.PST
   paradigm: PTCP-front-soft
  -flex: .из<.>
   gramm: ptcp.pst,missp
   gloss: PTCP.PST
@@ -3454,15 +3492,15 @@
   gramm: 1.s,sg.s,pst
   gloss: PST.1SG
   regex-prev: .*[бвгжкмпхчшщ][<>.]*$
  -flex: .ить<.>
   gramm: 2.s,sg.s,pst
   gloss: PST.2SG
   regex-prev: .*[бвгжкмпхчшщ][<>.]*$
- -flex: .ось<.>//.сь<.>
+ -flex: .отсь<.>//.ось<.>//.сь<.>
   gramm: 3.s,sg.s,pst
   gloss: PST.3SG
  -flex: .ь<.>
   gramm: 3.s,sg.s,pst
   gloss: PST.3SG
   regex-prev: .*с[<>.]*$
  -flex: .ынек<.>
@@ -3475,17 +3513,21 @@
   gramm: 1.s,pl.s,pst
   gloss: PST.1PL
   regex-prev: .*[бвгжкмпхчшщ][<>.]*$
  -flex: .иде<.>
   gramm: 2.s,pl.s,pst
   gloss: PST.2PL
   regex-prev: .*[бвгжкмпхчшщ][<>.]*$
- -flex: .ость<.>//.сть<.>
+ -flex: .отсть<.>//.ость<.>//.сть<.>
+  gramm: 3.s,pl.s,pst
+  gloss: PST.3PL
+ -flex: .ть<.>
   gramm: 3.s,pl.s,pst
   gloss: PST.3PL
+  regex-prev: .*с[<>.]*$
  paradigm: Clitics
 
 -paradigm: V-pst-e
  -flex: .ынь<.>
   gramm: 1.s,sg.s,pst
   gloss: PST.1SG
  -flex: .ыть<.>
@@ -3519,33 +3561,37 @@
  -flex: .иде<.>
   gramm: 2.s,pl.s,pst
   gloss: PST.2PL
   regex-prev: .*[бвгжкмпхчшщ][<>.]*$
  -flex: .эсть<.>//.сть<.>
   gramm: 3.s,pl.s,pst
   gloss: PST.3PL
+ -flex: .ть<.>
+  gramm: 3.s,pl.s,pst
+  gloss: PST.3PL
+  regex-prev: .*с[<>.]*$
  paradigm: Clitics
 
 -paradigm: V-pst-ye
  -flex: .инь<.>
   gramm: 1.s,sg.s,pst
   gloss: PST.1SG
  -flex: .ить<.>
   gramm: 2.s,sg.s,pst
   gloss: PST.2SG
- -flex: .есь<.>//.сь<.>//.[ь]сь<.>//.[й]сь<.>
+ -flex: .етсь<.>//.есь<.>//.сь<.>//.[ь]сь<.>//.[й]сь<.>
   gramm: 3.s,sg.s,pst
   gloss: PST.3SG
  -flex: .инек<.>
   gramm: 1.s,pl.s,pst
   gloss: PST.1PL
  -flex: .иде<.>
   gramm: 2.s,pl.s,pst
   gloss: PST.2PL
- -flex: .есть<.>//.сть<.>//.[ь]сть<.>//.[й]сть<.>
+ -flex: .етсть<.>//.есть<.>//.сть<.>//.[ь]сть<.>//.[й]сть<.>
   gramm: 3.s,pl.s,pst
   gloss: PST.3PL
  paradigm: Clitics
 
 -paradigm: V-pst-ezj-voiceless
  -flex: .ть<.>//.[ь]ть<.>
   gramm: 3.s,pl.s,pst,non_obj
@@ -3722,15 +3768,15 @@
   gloss: IMP.2SG›3SG
  -flex: .нк<.>//.ньк<.>//.ҥк<.>
   gramm: imp,2.s,pl.s,1.o,sg.o
   gloss: IMP.2PL›3SG
  -flex: .мизь<.>//.мызь<.>
   gramm: imp,2.s,1.o,pl.o
   gloss: IMP.2›1PL
- -flex: .т<.>//.ть<.>
+ -flex: .ить<.>
   gramm: imp,2.s,sg.s,3.o,pl.o
   gloss: IMP.2SG›3PL
  -flex: .нк<.>//.ньк<.>//.ҥк<.>
   gramm: imp,2.s,pl.s,1.o,pl.o
   gloss: IMP.2PL›3PL
  paradigm: Clitics
 
@@ -3755,15 +3801,15 @@
   gloss: IMP.2PL›1SG
  -flex: .ньк<.>
   gramm: imp,2.s,pl.s,1.o,sg.o
   gloss: IMP.2PL›3SG
  -flex: .мизь<.>
   gramm: imp,2.s,1.o,pl.o
   gloss: IMP.2›1PL
- -flex: .ть<.>
+ -flex: .ить<.>
   gramm: imp,2.s,sg.s,3.o,pl.o
   gloss: IMP.2SG›3PL
  -flex: .ньк<.>
   gramm: imp,2.s,pl.s,1.o,pl.o
   gloss: IMP.2PL›3PL
 
 -paradigm: V-pst-obj
```

### Comparing `uniparser-erzya-1.1.2/uniparser_erzya/data_strict/bad_analyses.txt` & `uniparser-erzya-1.1.3/uniparser_erzya/data_strict/bad_analyses.txt`

 * *Files identical despite different names*

### Comparing `uniparser-erzya-1.1.2/uniparser_erzya/data_strict/lexemes.txt` & `uniparser-erzya-1.1.3/uniparser_erzya/data_strict/lexemes.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5112,14 +5112,22 @@
  lex: Артемьевна
  stem: артемьевна.
  gramm: N,PN,patrn
  paradigm: N-back
  trans_ru: Артемьевна
 
 -lexeme
+ lex: Артип
+ gramm: N,PN,persn
+ stem: артип.
+ paradigm: N-front
+ paradigm: N-back
+ trans_ru: Артип (Архип)
+
+-lexeme
  lex: Артистов
  stem: артистов.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Артистов
 
 -lexeme
@@ -5658,14 +5666,22 @@
  lex: Атюрьева
  stem: атюрьева.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Атюрьева
 
 -lexeme
+ lex: Атямарькин
+ gramm: N,PN,famn
+ stem: атямарькин.
+ paradigm: N-front
+ paradigm: N-back
+ trans_ru: Атямарькин
+
+-lexeme
  lex: Атяшева
  stem: атяшева.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Атяшева
 
 -lexeme
@@ -15333,14 +15349,28 @@
  lex: Гаруда
  stem: гаруда.
  gramm: N,PN
  paradigm: N-back
  trans_ru: Гаруда
 
 -lexeme
+ lex: Гаруз
+ gramm: N,persn,PN
+ stem: гаруз.
+ paradigm: N-back
+ trans_ru: Гарузов
+
+-lexeme
+ lex: Гарузов
+ gramm: N,famn,PN
+ stem: гарузов.
+ paradigm: N-back
+ trans_ru: Гарузов
+
+-lexeme
  lex: Гаспаров
  stem: гаспаров.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Гаспаров
 
 -lexeme
@@ -17034,14 +17064,22 @@
  lex: Гостехнадзор
  stem: гостехнадзор.
  gramm: N,PN
  paradigm: N-back
  trans_ru: Гостехнадзор
 
 -lexeme
+ lex: Гостя
+ gramm: N,PN,persn
+ stem: гостя.
+ paradigm: N-front
+ paradigm: N-back
+ trans_ru: Гостя (Костя)
+
+-lexeme
  lex: Готович
  stem: готович.
  gramm: N,PN,patrn
  paradigm: N-front
  trans_ru: Готович
 
 -lexeme
@@ -22321,14 +22359,22 @@
  lex: Занчарова
  stem: занчарова.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Занчарова
 
 -lexeme
+ lex: Заня
+ gramm: N,PN,persn
+ stem: заня.
+ paradigm: N-front
+ paradigm: N-back
+ trans_ru: Заня (Захар)
+
+-lexeme
  lex: Заполярье
  stem: заполярье.
  gramm: N,PN,topn
  paradigm: N-front
  trans_ru: Заполярье
 
 -lexeme
@@ -26634,14 +26680,21 @@
  lex: Кандаумов
  stem: кандаумов.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Кандаумов
 
 -lexeme
+ lex: Кандра
+ gramm: N,persn,PN
+ stem: кандра.
+ paradigm: N-back
+ trans_ru: Кандра (Кондрат)
+
+-lexeme
  lex: Каневский
  stem: каневски.
  gramm: N,PN,famn
  paradigm: N-front-j
  trans_ru: Каневский
 
 -lexeme
@@ -32991,14 +33044,21 @@
  lex: Лааксо
  stem: лааксо.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Лааксо
 
 -lexeme
+ lex: Лабырь
+ gramm: N,PN,persn
+ stem: лабыр.
+ paradigm: N-front-soft
+ trans_ru: Лабырь
+
+-lexeme
  lex: Лаванов
  stem: лаванов.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Лаванов
 
 -lexeme
@@ -36946,14 +37006,22 @@
  lex: Матросов
  stem: матросов.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Матросов
 
 -lexeme
+ lex: Матря
+ gramm: N,persn,PN
+ stem: матря.
+ paradigm: N-front
+ paradigm: N-back
+ trans_ru: Матря (Матрёна)
+
+-lexeme
  lex: Матрёна
  stem: матрёна.
  gramm: N,PN,persn
  paradigm: N-back
  trans_ru: Матрёна
 
 -lexeme
@@ -36967,14 +37035,22 @@
  lex: Матюшенко
  stem: матюшенко.//матюшеҥко.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Матюшенко
 
 -lexeme
+ lex: Матя
+ gramm: N,PN,persn
+ stem: матя.
+ paradigm: N-front
+ paradigm: N-back
+ trans_ru: Матя (Матрёна)
+
+-lexeme
  lex: Махметов
  stem: махметов.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Махметов
 
 -lexeme
@@ -40638,14 +40714,21 @@
  lex: Найдёнков
  stem: найдёнков.//найдёҥков.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Найдёнков
 
 -lexeme
+ lex: Найман
+ gramm: N,topn,PN
+ stem: найман.
+ paradigm: N-back
+ trans_ru: Найманы
+
+-lexeme
  lex: Наймушин
  stem: наймушин.
  gramm: N,PN,famn
  paradigm: N-front
  trans_ru: Наймушин
 
 -lexeme
@@ -43151,14 +43234,21 @@
  lex: Олда
  gramm: N,persn,PN
  stem: олда.
  paradigm: N-front
  trans_ru: Олда
 
 -lexeme
+ lex: Олдай
+ gramm: N,persn,PN
+ stem: олда.
+ paradigm: N-front-j
+ trans_ru: Олдай (Авдотья)
+
+-lexeme
  lex: Олег
  stem: олег.
  gramm: N,PN,persn
  paradigm: N-front
  trans_ru: Олег
 
 -lexeme
@@ -44527,22 +44617,15 @@
  trans_ru: Пархоменко
 
 -lexeme
  lex: Парынза
  gramm: N,PN,topn
  stem: парынза.
  paradigm: N-back
- trans_ru: Чёрная промза (село; название музыкального коллектива)
-
--lexeme
- lex: Парынза
- gramm: N,PN,topn
- stem: парынза.
- paradigm: N-front
- trans_ru: Чёрная промза (село; название музыкального коллектива)
+ trans_ru: Чёрная Промза (село; название музыкального коллектива)
 
 -lexeme
  lex: Пастернак
  stem: пастернак.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Пастернак
@@ -44649,14 +44732,22 @@
  lex: Пахмутова
  stem: пахмутова.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Пахмутова
 
 -lexeme
+ lex: Пахом
+ gramm: N,persn,PN
+ stem: пахом.
+ paradigm: N-front
+ paradigm: N-back
+ trans_ru: Пахом
+
+-lexeme
  lex: Пахомов
  stem: пахомов.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Пахомов
 
 -lexeme
@@ -51265,14 +51356,22 @@
  lex: Салдаева
  stem: салдаева.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Салдаева
 
 -lexeme
+ lex: Салдин
+ gramm: N,famn,PN
+ stem: салдин.
+ paradigm: N-front
+ paradigm: N-back
+ trans_ru: Салдин
+
+-lexeme
  lex: Салехард
  stem: салехард.
  gramm: N,PN,topn
  paradigm: N-back
  trans_ru: Салехард
 
 -lexeme
@@ -51636,14 +51735,21 @@
  lex: Самойлова
  stem: самойлова.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Самойлова
 
 -lexeme
+ lex: Самойловна
+ gramm: N,PN,patrn
+ stem: самойловна.
+ paradigm: N-back
+ trans_ru: Самойловна
+
+-lexeme
  lex: Самоленко
  stem: самоленко.//самолеҥко.
  gramm: N,PN,famn
  paradigm: N-back
  trans_ru: Самоленко
 
 -lexeme
@@ -55633,14 +55739,22 @@
  lex: Студитских
  stem: студитских.
  gramm: N,PN,famn
  paradigm: N-front
  trans_ru: Студитских
 
 -lexeme
+ lex: Стяпан
+ gramm: N,persn,PN
+ stem: стяпан.
+ paradigm: N-front
+ paradigm: N-back
+ trans_ru: Степан
+
+-lexeme
  lex: Стёпа
  stem: стёпа.
  gramm: N,PN,persn
  paradigm: N-back
  trans_ru: Стёпа
 
 -lexeme
@@ -73165,14 +73279,21 @@
  lex: алкине
  stem: алкине.
  gramm: A,dim
  paradigm: A-front
  trans_ru: низкорослый
 
 -lexeme
+ lex: алкинестэ
+ gramm: ADV
+ stem: алкинестэ.
+ paradigm: Clitics
+ trans_ru: низко; неглубоко
+
+-lexeme
  lex: алкиньгадомс
  stem: алкиньга.
  gramm: V
  paradigm: V-do
  trans_ru: снизиться, осесть
 
 -lexeme
@@ -73306,14 +73427,21 @@
  stem: алнэ.
  gramm: N,dim
  paradigm: N-front
  trans_ru: личинка
 
 -lexeme
  lex: ало
+ gramm: A
+ stem: ало.
+ paradigm: A-back
+ trans_ru: нижний
+
+-lexeme
+ lex: ало
  stem: ало.
  gramm: ADV
  paradigm: Clitics
  trans_ru: внизу
 
 -lexeme
  lex: ало
@@ -74941,14 +75069,21 @@
  stem: апаркст.
  gramm: V
  paradigm: V-o
  trans_ru: расстроиться
 
 -lexeme
  lex: апаро
+ gramm: ADV
+ stem: апаро.
+ paradigm: Clitics
+ trans_ru: неприятно
+
+-lexeme
+ lex: апаро
  stem: апаро.
  gramm: A
  paradigm: A-back
  trans_ru: нехороший
 
 -lexeme
  lex: апаро
@@ -78550,14 +78685,21 @@
  stem: банкет.//банькет.//баҥкет.
  gramm: N,rus
  paradigm: N-front
  paradigm: N-back
  trans_ru: банкет
 
 -lexeme
+ lex: банкине
+ gramm: N,rus,dim
+ stem: банкине.
+ paradigm: N-front
+ trans_ru: баночка
+
+-lexeme
  lex: банкир
  stem: банкир.//банькир.//баҥкир.//банькир.
  gramm: N,rus,anim,hum
  paradigm: N-front
  trans_ru: банкир
 
 -lexeme
@@ -78594,14 +78736,21 @@
  stem: баннер.
  gramm: N,rus
  paradigm: N-back
  paradigm: N-front
  trans_ru: баннер
 
 -lexeme
+ lex: банок
+ gramm: A,rus
+ stem: банок.
+ paradigm: A-back
+ trans_ru: банка
+
+-lexeme
  lex: бант
  stem: бант.
  gramm: N,rus
  paradigm: N-back
  trans_ru: бант
 
 -lexeme
@@ -79480,14 +79629,21 @@
  lex: бедной
  stem: бедно.//бѣдно.
  gramm: A,rus
  paradigm: A-front-j
  trans_ru: бедный
 
 -lexeme
+ lex: беднойчи
+ gramm: N,rus
+ stem: беднойчи.
+ paradigm: N-front
+ trans_ru: бедность
+
+-lexeme
  lex: беднота
  stem: беднота.
  gramm: N,rus
  paradigm: N-back
  trans_ru: беднота
 
 -lexeme
@@ -80699,14 +80855,22 @@
  lex: бизьганя
  stem: бизьганя.
  gramm: N
  paradigm: N-back
  trans_ru: волчья ягода
 
 -lexeme
+ lex: бизьгатаев
+ gramm: A
+ stem: бизьгатаев.
+ paradigm: A-front
+ paradigm: A-back
+ trans_ru: веснушчатый
+
+-lexeme
  lex: бийнемс
  stem: бийн.//бійн.
  gramm: V
  paradigm: V-ye
  trans_ru: пищать
 
 -lexeme
@@ -81535,14 +81699,21 @@
  lex: бобаске
  stem: бобаске.|бобаск.
  gramm: N
  paradigm: N-front
  trans_ru: сказка
 
 -lexeme
+ lex: бобка
+ gramm: N,rus
+ stem: бобка.
+ paradigm: N-back
+ trans_ru: боб
+
+-lexeme
  lex: бобо
  stem: бобо.
  gramm: N
  paradigm: N-back
  trans_ru: пугало
 
 -lexeme
@@ -82691,14 +82862,21 @@
  lex: братик
  stem: братик.
  gramm: N,rus,anim,hum
  paradigm: N-front
  trans_ru: братик
 
 -lexeme
+ lex: братиники
+ gramm: N,rus,anim,hum
+ stem: братиники.
+ paradigm: N-front
+ trans_ru: братья
+
+-lexeme
  lex: братишка
  stem: братишка.
  gramm: N,rus,anim,hum
  paradigm: N-back
  trans_ru: братишка
 
 -lexeme
@@ -84721,19 +84899,26 @@
  lex: вакан
  stem: вакан.
  gramm: N
  paradigm: N-back
  trans_ru: кваканье
 
 -lexeme
+ lex: вакан
+ stem: вакан.
+ gramm: N
+ paradigm: N-back
+ trans_ru: миска
+
+-lexeme
  lex: ваканнэ
  stem: ваканнэ.
- gramm: N
+ gramm: N,dim
  paradigm: N-front
- trans_ru: миска
+ trans_ru: мисочка
 
 -lexeme
  lex: вакансия
  stem: вакансия.//вакансія.
  gramm: N,rus
  paradigm: N-back
  trans_ru: вакансия
@@ -84753,15 +84938,22 @@
  trans_ru: квакать
 
 -lexeme
  lex: вакс
  stem: вакс.
  gramm: N
  paradigm: N-back
- trans_ru: вершок; возле, к, около
+ trans_ru: вершок
+
+-lexeme
+ lex: вакс
+ stem: вакс.
+ gramm: N,rel_n
+ paradigm: N-back
+ trans_ru: возле, к, около
 
 -lexeme
  lex: вакснэ
  stem: вакснэ.
  gramm: POST
  paradigm: Clitics
  trans_ru: рядом
@@ -88346,14 +88538,22 @@
  stem: вельдерьма.
  gramm: N
  paradigm: N-back
  trans_ru: дымоход
 
 -lexeme
  lex: велькс
+ gramm: N
+ stem: велькс.
+ paradigm: N-front
+ paradigm: N-back
+ trans_ru: верхняя часть чего-либо
+
+-lexeme
+ lex: велькс
  stem: велькс.
  gramm: N
  paradigm: N-front
  trans_ru: навес, одеяло; сливки, сметана
 
 -lexeme
  lex: велькска
@@ -88869,14 +89069,21 @@
  stem: верде.|верд.
  gramm: ADV
  paradigm: Clitics
  trans_ru: сверху
 
 -lexeme
  lex: вере
+ gramm: A
+ stem: вере.
+ paradigm: A-front
+ trans_ru: верхний
+
+-lexeme
+ lex: вере
  stem: вере.
  gramm: ADV
  paradigm: Clitics
  trans_ru: наверху, сверху
 
 -lexeme
  lex: верев
@@ -96954,14 +97161,22 @@
  lex: гренадёр
  stem: гренадёр.//гренадер.
  gramm: N,rus,anim,hum
  paradigm: N-back
  trans_ru: гренадёр
 
 -lexeme
+ lex: грех
+ gramm: N,rus
+ stem: грех.
+ paradigm: N-front
+ paradigm: N-back
+ trans_ru: грех
+
+-lexeme
  lex: грецкой
  stem: грецко.
  gramm: A,rus
  paradigm: A-front-j
  trans_ru: грецкий
 
 -lexeme
@@ -97575,14 +97790,21 @@
  lex: гурсо
  stem: гурсо.
  gramm: IMIT
  paradigm: Clitics
  trans_ru: хорошо (гореть)
 
 -lexeme
+ lex: гурьба
+ gramm: N,rus
+ stem: гурьба.
+ paradigm: N-back
+ trans_ru: гурьба
+
+-lexeme
  lex: гурямс
  stem: гур.
  gramm: V
  paradigm: V-ya
  trans_ru: водить в прятки, прятаться
 
 -lexeme
@@ -102182,14 +102404,21 @@
  lex: егошихинской
  stem: егошихинско.
  gramm: A,rus
  paradigm: A-front-j
  trans_ru: егошихинский
 
 -lexeme
+ lex: едак
+ gramm: N,rus
+ stem: едак.
+ paradigm: N-back
+ trans_ru: едок
+
+-lexeme
  lex: единица
  stem: единица.
  gramm: N,rus
  paradigm: N-back
  trans_ru: единица
 
 -lexeme
@@ -103367,14 +103596,21 @@
  lex: забытой
  stem: забыто.
  gramm: A,rus
  paradigm: A-front-j
  trans_ru: забытый
 
 -lexeme
+ lex: завалинка
+ gramm: N,rus
+ stem: завалинка.
+ paradigm: N-back
+ trans_ru: завалинка
+
+-lexeme
  lex: заведения
  stem: заведения.//заведение.//заведения.//заведеніе.
  gramm: N,rus
  paradigm: N-back
  paradigm: N-front
  trans_ru: заведение
 
@@ -105089,14 +105325,21 @@
  lex: знярс
  stem: знярс.
  gramm: ADVPRO
  paradigm: Clitics
  trans_ru: сколько
 
 -lexeme
+ lex: знярыя
+ gramm: ADVPRO
+ stem: знярыя.
+ paradigm: Clitics
+ trans_ru: столько
+
+-lexeme
  lex: зобня
  stem: зобня.
  gramm: N,body
  paradigm: N-back
  trans_ru: желудок
 
 -lexeme
@@ -106531,14 +106774,21 @@
  stem: икеле.
  gramm: ADV
  paradigm: Clitics
  trans_ru: впереди; раньше
 
 -lexeme
  lex: икеле
+ stem: икеле.
+ gramm: POST
+ paradigm: Clitics
+ trans_ru: перед, напротив; до
+
+-lexeme
+ lex: икеле
  stem: икеле.|икель.
  gramm: N,rel_n
  paradigm: N-front
  trans_ru: впереди; раньше
 
 -lexeme
  lex: икелевал
@@ -111894,14 +112144,21 @@
  lex: камфорной
  stem: камфорно.
  gramm: A,rus
  paradigm: A-front-j
  trans_ru: камфорный
 
 -lexeme
+ lex: камчадал
+ gramm: N,rus
+ stem: камчадал.
+ paradigm: N-back
+ trans_ru: камчадал
+
+-lexeme
  lex: камыш
  stem: камыш.
  gramm: N,rus
  paradigm: N-back
  trans_ru: камыш
 
 -lexeme
@@ -112540,14 +112797,21 @@
  lex: каподемс
  stem: капод.
  gramm: V
  paradigm: V-ye
  trans_ru: схватить, уцепиться
 
 -lexeme
+ lex: капоемс
+ gramm: V,intr
+ stem: капо.
+ paradigm: V-ye
+ trans_ru: многокр. к схватить, уцепиться
+
+-lexeme
  lex: капор
  stem: капор.
  gramm: N,rus
  paradigm: N-back
  trans_ru: капор
 
 -lexeme
@@ -113339,14 +113603,21 @@
  lex: каркс
  stem: каркс.
  gramm: N
  paradigm: N-back
  trans_ru: бандаж, пояс
 
 -lexeme
+ lex: карксамга
+ gramm: ADV
+ stem: карксамга.
+ paradigm: Clitics
+ trans_ru: по пояс
+
+-lexeme
  lex: карксамопель
  stem: карксамопел.
  gramm: N
  paradigm: N-front-soft
  trans_ru: кушак, пояс
 
 -lexeme
@@ -114029,14 +114300,21 @@
  lex: касовкске
  stem: касовкске.
  gramm: N,dim
  paradigm: N-front
  trans_ru: растеньице
 
 -lexeme
+ lex: касоль
+ gramm: N,rus
+ stem: касол.
+ paradigm: N-front-soft
+ trans_ru: фасоль
+
+-lexeme
  lex: касом
  stem: касом.
  gramm: N
  paradigm: N-back
  trans_ru: пробор в волосах
 
 -lexeme
@@ -114725,14 +115003,21 @@
  lex: качоловажа
  stem: качоловажа.
  gramm: N,body
  paradigm: N-back
  trans_ru: бедренная кость
 
 -lexeme
+ lex: каша
+ gramm: N,rus
+ stem: каша.
+ paradigm: N-back
+ trans_ru: каша
+
+-lexeme
  lex: кашамс
  stem: каш.
  gramm: V
  paradigm: V-a
  trans_ru: запорошить
 
 -lexeme
@@ -117876,15 +118161,15 @@
  stem: кие.//кіе.
  gramm: PRO,nom,sg
  paradigm: Clitics
  trans_ru: кто
 
 -lexeme
  lex: кие-бути
- stem: кие-бути//кіе-бути
+ stem: кие.-бути//кіе.-бути
  gramm: PRO,nom,sg
  paradigm: Clitics
  trans_ru: кто-нибудь, кто-то
 
 -lexeme
  lex: кие-кие
  stem: кие-кие.//кие-кіе.
@@ -121046,14 +121331,21 @@
  lex: козомс
  stem: коз.
  gramm: V
  paradigm: V-o
  trans_ru: кашлять
 
 -lexeme
+ lex: козонь
+ gramm: ADVPRO
+ stem: козонь.
+ paradigm: Clitics
+ trans_ru: где, куда
+
+-lexeme
  lex: козылька
  stem: козылька.
  gramm: N
  paradigm: N-back
  trans_ru: череда
 
 -lexeme
@@ -121629,14 +121921,21 @@
  lex: колесница
  stem: колесница.
  gramm: N,rus,transport
  paradigm: N-back
  trans_ru: колесница
 
 -lexeme
+ lex: коли
+ gramm: CONJ,rus
+ stem: коли.
+ paradigm: Clitics
+ trans_ru: коли, если
+
+-lexeme
  lex: количественной
  stem: количественно.
  gramm: A,rus
  paradigm: A-front-j
  trans_ru: количественный
 
 -lexeme
@@ -125282,14 +125581,21 @@
  lex: кортавкске
  stem: кортавкске.
  gramm: N,dim
  paradigm: N-front
  trans_ru: разговорчик
 
 -lexeme
+ lex: кортавомс
+ gramm: V,intr
+ stem: кортав.
+ paradigm: V-o
+ trans_ru: возм. к говорить
+
+-lexeme
  lex: кортавт
  stem: кортавт.
  gramm: N
  paradigm: N-back
  trans_ru: разговор; слухи
 
 -lexeme
@@ -127871,14 +128177,21 @@
  lex: куваня
  stem: куваня.
  gramm: ADVPRO
  paradigm: Clitics
  trans_ru: где
 
 -lexeme
+ lex: куватень
+ gramm: A
+ stem: куватен.
+ paradigm: A-front-soft
+ trans_ru: долгий
+
+-lexeme
  lex: кувать
  stem: кувать.
  gramm: ADV
  paradigm: Clitics
  trans_ru: долго
 
 -lexeme
@@ -131400,14 +131713,21 @@
  lex: лавтовловажа
  stem: лавтовловажа.
  gramm: N,body
  paradigm: N-back
  trans_ru: ключица
 
 -lexeme
+ lex: лавтово
+ gramm: N,body
+ stem: лавтово.
+ paradigm: N-back
+ trans_ru: плечо
+
+-lexeme
  lex: лавтовов
  stem: лавтовов.
  gramm: A
  paradigm: A-back
  trans_ru: плечистый
 
 -lexeme
@@ -138112,14 +138432,22 @@
  stem: магазин.
  gramm: N,rus
  paradigm: N-front
  paradigm: N-back
  trans_ru: в разн. магазин
 
 -lexeme
+ lex: магарыч
+ gramm: N,rus
+ stem: магарыч.
+ paradigm: N-front
+ paradigm: N-back
+ trans_ru: магарыч
+
+-lexeme
  lex: магистерской
  stem: магистерско.
  gramm: A,rus
  paradigm: A-front-j
  trans_ru: магистерский
 
 -lexeme
@@ -141509,14 +141837,21 @@
  stem: межэтническо.
  gramm: A,rus
  paradigm: A-front-j
  trans_ru: межэтнический
 
 -lexeme
  lex: мезде
+ gramm: ADVPRO
+ stem: мезде.
+ paradigm: Clitics
+ trans_ru: за сколько, о чём, кого, чего, за что
+
+-lexeme
+ lex: мезде
  stem: мезде.
  gramm: PRO
  paradigm: Clitics
  trans_ru: за сколько, из-за чего, о чем
 
 -lexeme
  lex: мездеяк
@@ -141648,14 +141983,21 @@
  lex: мейле
  stem: мейле.
  gramm: ADVPRO
  paradigm: Clitics
  trans_ru: затем, после, потом
 
 -lexeme
+ lex: мейле
+ stem: мейле.
+ gramm: POST
+ paradigm: Clitics
+ trans_ru: после
+
+-lexeme
  lex: мейс
  stem: мейс.
  gramm: ADVPRO
  paradigm: Clitics
  trans_ru: почему
 
 -lexeme
@@ -142223,14 +142565,21 @@
  lex: мельпаз
  stem: мельпаз.
  gramm: N,supernat
  paradigm: N-back
  trans_ru: держатель неба
 
 -lexeme
+ lex: мельпаросо
+ gramm: ADV
+ stem: мельпаросо.
+ paradigm: Clitics
+ trans_ru: охотно, с удовольствием
+
+-lexeme
  lex: мельполадкс
  stem: мельполадкс.
  gramm: N
  paradigm: N-back
  trans_ru: статья
 
 -lexeme
@@ -144973,14 +145322,22 @@
  stem: могильник.
  gramm: N,rus
  paradigm: N-front
  paradigm: N-back
  trans_ru: могильник
 
 -lexeme
+ lex: могорыч
+ gramm: N,rus
+ stem: могорыч.
+ paradigm: N-front
+ paradigm: N-back
+ trans_ru: магарыч
+
+-lexeme
  lex: мода
  stem: мода.
  gramm: N
  paradigm: N-back
  trans_ru: земля; территория
 
 -lexeme
@@ -149541,14 +149898,21 @@
  lex: нарошной
  stem: нарошно.
  gramm: A,rus
  paradigm: A-front-j
  trans_ru: нарочный
 
 -lexeme
+ lex: нарсемс
+ gramm: V,intr
+ stem: нарс.
+ paradigm: V-ye
+ trans_ru: многокр. к стричь, брить, стричься, бриться
+
+-lexeme
  lex: нарсуд
  stem: нарсуд.
  gramm: N,rus
  paradigm: N-back
  trans_ru: нарсуд
 
 -lexeme
@@ -150182,14 +150546,21 @@
  stem: нацсобрания.//нацсобрание.//нацсобрания.//нацсобраніе.
  gramm: N,rus
  paradigm: N-back
  paradigm: N-front
  trans_ru: нацсобрание
 
 -lexeme
+ lex: начал
+ gramm: N,rus,anim,hum
+ stem: начал.
+ paradigm: N-back
+ trans_ru: начальник
+
+-lexeme
  lex: началка
  stem: началка.
  gramm: N,rus
  paradigm: N-back
  trans_ru: началка
 
 -lexeme
@@ -153325,14 +153696,21 @@
  lex: ноцкадемс
  stem: ноцкад.
  gramm: V
  paradigm: V-ye
  trans_ru: вырвать, дёрнуть, кольнуть
 
 -lexeme
+ lex: ноцковтнемс
+ gramm: V,tr
+ stem: ноцковтн.
+ paradigm: V-ye
+ trans_ru: многокр. к дёрнуть, вырвать
+
+-lexeme
  lex: ноцковтомс
  stem: ноцковт.
  gramm: V
  paradigm: V-o
  trans_ru: вырвать
 
 -lexeme
@@ -158622,14 +159000,21 @@
  stem: оршамот-карсемат.
  gramm: N
  paradigm: N-back
  trans_ru: одежда и обувь
 
 -lexeme
  lex: оршамс
+ gramm: V,tr
+ stem: оршамо.
+ paradigm: Clitics
+ trans_ru: надеть на себя
+
+-lexeme
+ lex: оршамс
  stem: орш.
  gramm: V
  paradigm: V-a
  trans_ru: надеть; одеться
 
 -lexeme
  lex: оршамс-карсемс
@@ -171327,14 +171712,22 @@
  lex: покой
  stem: поко.
  gramm: N,rus
  paradigm: N-front-j
  trans_ru: покой
 
 -lexeme
+ lex: покойник
+ gramm: N,rus,anim,hum
+ stem: покойник.
+ paradigm: N-front
+ paradigm: N-back
+ trans_ru: покойник
+
+-lexeme
  lex: поколев
  stem: поколев.
  gramm: A
  paradigm: A-front
  trans_ru: комковатый
 
 -lexeme
@@ -174136,14 +174529,21 @@
  lex: потомственной
  stem: потомственно.
  gramm: A,rus
  paradigm: A-front-j
  trans_ru: потомственный
 
 -lexeme
+ lex: потомтнемс
+ gramm: V,intr
+ stem: потомтн.
+ paradigm: V-ye
+ trans_ru: закрываться
+
+-lexeme
  lex: поточной
  stem: поточно.
  gramm: A,rus
  paradigm: A-front-j
  trans_ru: поточный
 
 -lexeme
@@ -174945,14 +175345,21 @@
  lex: праздничной
  stem: празднично.
  gramm: A,rus
  paradigm: A-front-j
  trans_ru: праздничный
 
 -lexeme
+ lex: праздновамс
+ gramm: V,tr,rus
+ stem: празднов.
+ paradigm: V-a
+ trans_ru: праздновать
+
+-lexeme
  lex: празднования
  stem: празднования.//празднование.//празднованія.//празднованіе.
  gramm: N,rus
  paradigm: N-back
  paradigm: N-front
  trans_ru: празднование
 
@@ -179361,14 +179768,21 @@
  lex: пуворямс
  stem: пувор.
  gramm: V
  paradigm: V-ya
  trans_ru: измять, крутить
 
 -lexeme
+ lex: пувсемс
+ gramm: V,intr
+ stem: пувс.
+ paradigm: V-ye
+ trans_ru: многокр. к дуть, подуть, веять, развеять
+
+-lexeme
  lex: пувтамс
  stem: пувт.
  gramm: V
  paradigm: V-a
  trans_ru: разбудить
 
 -lexeme
@@ -184878,14 +185292,21 @@
  lex: риснемс
  stem: рисн.
  gramm: V
  paradigm: V-ye
  trans_ru: излучать, литься, моросить
 
 -lexeme
+ lex: рисовавкс
+ gramm: N,rus
+ stem: рисовавкс.
+ paradigm: N-back
+ trans_ru: рисунок
+
+-lexeme
  lex: рисовамс
  stem: рисов.
  gramm: V
  paradigm: V-a
  trans_ru: нарисовать
 
 -lexeme
@@ -186638,14 +187059,21 @@
  lex: саевть
  stem: саевт.
  gramm: A
  paradigm: A-front-soft
  trans_ru: взятый
 
 -lexeme
+ lex: саезь
+ gramm: POST
+ stem: саезь.
+ paradigm: Clitics
+ trans_ru: с
+
+-lexeme
  lex: саема
  stem: саема.
  gramm: N
  paradigm: N-back
  trans_ru: взятие, вычет
 
 -lexeme
@@ -187923,14 +188351,21 @@
  stem: сас.
  gramm: V
  paradigm: V-a
  trans_ru: гнаться, догнать
 
 -lexeme
  lex: састо
+ gramm: ADV
+ stem: састо.
+ paradigm: Clitics
+ trans_ru: тихо, негромко
+
+-lexeme
+ lex: састо
  stem: састо.|саст.
  gramm: A
  paradigm: A-back
  trans_ru: медленный, негромкий, тихий
 
 -lexeme
  lex: састыне
@@ -193718,14 +194153,21 @@
  lex: содазь
  stem: содазь.
  gramm: ADV
  paradigm: Clitics
  trans_ru: известно; сознательно
 
 -lexeme
+ lex: содамо
+ stem: содамо.
+ gramm: N,anim,hum
+ paradigm: N-back
+ trans_ru: зять
+
+-lexeme
  lex: содамоаравкс
  stem: содамоаравкс.
  gramm: N
  paradigm: N-back
  trans_ru: задача
 
 -lexeme
@@ -197086,14 +197528,21 @@
  lex: стопка
  stem: стопка.
  gramm: N,rus
  paradigm: N-back
  trans_ru: стопка
 
 -lexeme
+ lex: стопкине
+ gramm: N,dim,rus
+ stem: стопкине.
+ paradigm: N-front
+ trans_ru: стопка
+
+-lexeme
  lex: сторож
  stem: сторож.
  gramm: N,rus,anim,hum
  paradigm: N-back
  trans_ru: сторож
 
 -lexeme
@@ -197459,14 +197908,21 @@
  lex: струнной
  stem: струнно.
  gramm: A,rus
  paradigm: A-front-j
  trans_ru: струнный
 
 -lexeme
+ lex: струя
+ gramm: N,rus
+ stem: струя.
+ paradigm: N-back
+ trans_ru: струя
+
+-lexeme
  lex: стряпавкс
  stem: стряпавкс.
  gramm: N,rus
  paradigm: N-back
  trans_ru: стряпня
 
 -lexeme
@@ -201333,14 +201789,21 @@
  stem: сёксен.
  gramm: A
  paradigm: A-front-soft
  trans_ru: осенний, осенниё
 
 -lexeme
  lex: сёксня
+ gramm: ADV
+ stem: сексня.
+ paradigm: Clitics
+ trans_ru: осенью
+
+-lexeme
+ lex: сёксня
  stem: сёксня.
  gramm: ADV
  paradigm: Clitics
  trans_ru: осенью
 
 -lexeme
  lex: сёксь
@@ -203229,14 +203692,21 @@
  lex: тарнышка
  stem: тарнышка.
  gramm: N,anim,hum
  paradigm: N-back
  trans_ru: торопыга
 
 -lexeme
+ lex: тарск
+ gramm: IMIT
+ stem: тарск.
+ paradigm: Clitics
+ trans_ru: вздрогнуть (тарск теемс)
+
+-lexeme
  lex: тарскадемс
  stem: тарскад.
  gramm: V
  paradigm: V-ye
  trans_ru: вздрогнуть
 
 -lexeme
@@ -213511,14 +213981,21 @@
  lex: урямо
  stem: урямо.
  gramm: N
  paradigm: N-back
  trans_ru: тальник
 
 -lexeme
+ lex: уса
+ gramm: N,rus,body
+ stem: уса.
+ paradigm: N-back
+ trans_ru: усы
+
+-lexeme
  lex: усад
  stem: усад.
  gramm: N,rus
  paradigm: N-back
  trans_ru: усадьба
 
 -lexeme
@@ -217517,14 +217994,21 @@
  lex: хартия
  stem: хартия.//хартія.
  gramm: N,rus
  paradigm: N-back
  trans_ru: хартия
 
 -lexeme
+ lex: харч
+ gramm: N,rus
+ stem: харч.
+ paradigm: N-back
+ trans_ru: харч
+
+-lexeme
  lex: харчо
  stem: харчо.
  gramm: N,rus
  paradigm: N-back
  trans_ru: харчо
 
 -lexeme
@@ -219417,14 +219901,21 @@
  lex: цилик-пулик
  stem: цилик-пулик.
  gramm: IMIT
  paradigm: Clitics
  trans_ru: об игре на струнах
 
 -lexeme
+ lex: цилим
+ stem: цилим.
+ gramm: N
+ paradigm: N-front
+ trans_ru: курительная трубка
+
+-lexeme
  lex: цилимпей
  stem: цилимпе.
  gramm: N,body
  paradigm: N-front-j
  trans_ru: зуб мудрости
 
 -lexeme
@@ -220253,14 +220744,21 @@
  lex: цюцев
  stem: цюцев.
  gramm: N
  paradigm: N-front
  trans_ru: вершина (дерева); гроздь, кисть, соцветие
 
 -lexeme
+ lex: цюцка
+ gramm: N
+ stem: цюцка.
+ paradigm: N-back
+ trans_ru: гроздь, кисть (плодов, ягод)
+
+-lexeme
  lex: цюцёв
  stem: цюцёв.
  gramm: N
  paradigm: N-back
  trans_ru: гроздья, кисти; серёжки
 
 -lexeme
@@ -221283,14 +221781,21 @@
  lex: чалгсемс
  stem: чалгс.
  gramm: V
  paradigm: V-ye
  trans_ru: топтать
 
 -lexeme
+ lex: чалксемс
+ gramm: V,tr
+ stem: чалкс.
+ paradigm: V-ye
+ trans_ru: многокр. к наступить, мять
+
+-lexeme
  lex: чалма
  stem: чалма.
  gramm: N,rus
  paradigm: N-back
  trans_ru: чалма
 
 -lexeme
@@ -222211,18 +222716,18 @@
  stem: чевельд.
  gramm: V
  paradigm: V-ya
  trans_ru: примять, раздавить
 
 -lexeme
  lex: чевелямс
- stem: чевел.
+ stem: чевел.//чевил.
  gramm: V
  paradigm: V-ya
- trans_ru: жевать (о беззубых)
+ trans_ru: мять, жевать (о беззубых)
 
 -lexeme
  lex: чевкс
  stem: чевкс.
  gramm: N
  paradigm: N-front
  trans_ru: сухое полено для лучин
```

### Comparing `uniparser-erzya-1.1.2/uniparser_erzya/data_strict/paradigms.txt` & `uniparser-erzya-1.1.3/uniparser_erzya/data_strict/paradigms.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2306,18 +2306,22 @@
   paradigm: V-ye-proper
   paradigm: V-e-proper
 
 
 -paradigm: V-a-proper
  -flex: .<.>
   gramm: non_obj
-  paradigm: V-npst-a
   paradigm: V-pst-a
+ -flex: .<.>
+  gramm: non_obj,npst
+  paradigm: V-npst-a
  -flex: .[а]<.>
+  gramm: npst
   paradigm: V-npst-obj
+ -flex: .[а]<.>
   paradigm: V-opt
   paradigm: V-imp-back
  -flex: .[а]<.>
   gramm: neg
   paradigm: Clitics
  -flex: .[а]з<.>
   gramm: ptcp.pst
@@ -2436,19 +2440,23 @@
  -flex: .[а]м|га<.>
   gramm: cvb.caus
   gloss: NMLZ|PROL
   paradigm: N-poss-back-vowel
 
 -paradigm: V-ya-proper
  -flex: .<.>
-  gramm: non_obj
+  gramm: non_obj,npst
   paradigm: V-npst-ya
+ -flex: .<.>
+  gramm: non_obj
   paradigm: V-pst-ya
  -flex: .[я]<.>
+  gramm: npst
   paradigm: V-npst-obj
+ -flex: .[я]<.>
   paradigm: V-imp-back
   paradigm: V-opt
  -flex: .[я]<.>
   gramm: neg
   paradigm: Clitics
  -flex: .[я]з<.>
   gramm: ptcp.pst
@@ -2526,25 +2534,32 @@
  -flex: .[я]м|га<.>
   gramm: cvb.caus
   gloss: NMLZ|PROL
   paradigm: N-poss-back-vowel
 
 -paradigm: V-o-proper
  -flex: .<.>
-  gramm: non_obj
+  gramm: non_obj,npst
   paradigm: V-npst-o
+ -flex: .<.>
+  gramm: non_obj
   paradigm: V-opt-o
   paradigm: V-pst-o
  -flex: .о<.>//.<.>
+  gramm: npst
   paradigm: V-npst-obj
+ -flex: .о<.>//.<.>
   paradigm: V-imp-back
  -flex: .а<.>//.<.>
-  gramm: missp
+  gramm: npst,missp
   regex-prev: ^(ловн|ванст)[<>.]*$
   paradigm: V-npst-obj
+ -flex: .а<.>//.<.>
+  gramm: missp
+  regex-prev: ^(ловн|ванст)[<>.]*$
   paradigm: V-imp-back
  -flex: .о<.>//.<.>
   gramm: neg
   paradigm: Clitics
  -flex: .оз<.>
   gramm: ptcp.pst
   gloss: PTCP.PST
@@ -2662,23 +2677,29 @@
  -flex: .ом|га<.>
   gramm: cvb.caus
   gloss: NMLZ|PROL
   paradigm: N-poss-back-vowel
 
 -paradigm: V-yo-proper
  -flex: .<.>
-  gramm: non_obj
+  gramm: non_obj,npst
   paradigm: V-npst-ye
+ -flex: .<.>
+  gramm: non_obj
   paradigm: V-opt-ye
   paradigm: V-pst-ye
  -flex: .ё<.>//.[ь]<.>
+  gramm: npst
   paradigm: V-npst-obj
+ -flex: .ё<.>//.[ь]<.>
   paradigm: V-imp-back
  -flex: .<.>
+  gramm: npst
   paradigm: V-npst-obj
+ -flex: .<.>
   paradigm: V-imp-front
   regex-next: ^[<>.]*[дт][ьеи].*
  -flex: .ё<.>//.[ь]<.>
   gramm: neg
   paradigm: Clitics
  -flex: .<.>
   paradigm: V-npst-obj
@@ -2762,20 +2783,24 @@
  -flex: .ём|га<.>
   gramm: cvb.caus
   gloss: NMLZ|PROL
   paradigm: N-poss-back-vowel
 
 -paradigm: V-e-proper
  -flex: .<.>
-  gramm: non_obj
+  gramm: non_obj,npst
   paradigm: V-npst-e
+ -flex: .<.>
+  gramm: non_obj
   paradigm: V-opt-e
   paradigm: V-pst-e
  -flex: .э<.>//.<.>
+  gramm: npst
   paradigm: V-npst-obj
+ -flex: .э<.>//.<.>
   paradigm: V-imp-front
  -flex: .э<.>//.<.>
   gramm: neg
   paradigm: Clitics
  -flex: .эз<.>
   gramm: ptcp.pst
   gloss: PTCP.PST
@@ -2897,42 +2922,55 @@
  -flex: .эм|га<.>
   gramm: cvb.caus
   gloss: NMLZ|PROL
   paradigm: N-poss-back-vowel
 
 -paradigm: V-ye-proper
  -flex: .<.>
-  gramm: non_obj
+  gramm: non_obj,npst
   paradigm: V-npst-ye
+  paradigm: V-npst-obj-soft
+ -flex: .<.>
+  gramm: non_obj
   paradigm: V-opt-ye
   paradigm: V-pst-ye
-  paradigm: V-npst-obj-soft
  -flex: .е<.>//.[ь]<.>
+  gramm: npst
   paradigm: V-npst-obj
+ -flex: .е<.>//.[ь]<.>
   paradigm: V-imp-front
  -flex: .и<.>
-  gramm: missp
+  gramm: npst,missp
   paradigm: V-npst-obj
+ -flex: .и<.>
+  gramm: missp
   paradigm: V-imp-front
  -flex: .<.>
+  gramm: npst
   paradigm: V-npst-obj
+  regex-next: ^[<>.]*[дт][ьеи].*
+ -flex: .<.>
   paradigm: V-imp-front
   regex-next: ^[<>.]*[дт][ьеи].*
  -flex: .е<.>//.[ь]<.>
   gramm: neg
   paradigm: Clitics
  -flex: .и<.>
   gramm: neg,missp
   paradigm: Clitics
  -flex: .<.>
   paradigm: V-npst-obj
   regex-prev: (.*[бвгжкмпхчшщ]|^не|^му|^ту)[<>.]*$
  -flex: .[й]<.>
+  gramm: npst
   paradigm: V-npst-obj
   regex-prev: .*[аеёиоуыэюя][<>.]*$
+ -flex: .[й]<.>
+  paradigm: V-imp-front
+  regex-prev: .*[аеёиоуыэюя][<>.]*$
  -flex: .ез<.>
   gramm: ptcp.pst
   gloss: PTCP.PST
   paradigm: PTCP-front-soft
  -flex: .из<.>
   gramm: ptcp.pst,missp
   gloss: PTCP.PST
@@ -3454,15 +3492,15 @@
   gramm: 1.s,sg.s,pst
   gloss: PST.1SG
   regex-prev: .*[бвгжкмпхчшщ][<>.]*$
  -flex: .ить<.>
   gramm: 2.s,sg.s,pst
   gloss: PST.2SG
   regex-prev: .*[бвгжкмпхчшщ][<>.]*$
- -flex: .ось<.>//.сь<.>
+ -flex: .отсь<.>//.ось<.>//.сь<.>
   gramm: 3.s,sg.s,pst
   gloss: PST.3SG
  -flex: .ь<.>
   gramm: 3.s,sg.s,pst
   gloss: PST.3SG
   regex-prev: .*с[<>.]*$
  -flex: .ынек<.>
@@ -3475,17 +3513,21 @@
   gramm: 1.s,pl.s,pst
   gloss: PST.1PL
   regex-prev: .*[бвгжкмпхчшщ][<>.]*$
  -flex: .иде<.>
   gramm: 2.s,pl.s,pst
   gloss: PST.2PL
   regex-prev: .*[бвгжкмпхчшщ][<>.]*$
- -flex: .ость<.>//.сть<.>
+ -flex: .отсть<.>//.ость<.>//.сть<.>
+  gramm: 3.s,pl.s,pst
+  gloss: PST.3PL
+ -flex: .ть<.>
   gramm: 3.s,pl.s,pst
   gloss: PST.3PL
+  regex-prev: .*с[<>.]*$
  paradigm: Clitics
 
 -paradigm: V-pst-e
  -flex: .ынь<.>
   gramm: 1.s,sg.s,pst
   gloss: PST.1SG
  -flex: .ыть<.>
@@ -3519,33 +3561,37 @@
  -flex: .иде<.>
   gramm: 2.s,pl.s,pst
   gloss: PST.2PL
   regex-prev: .*[бвгжкмпхчшщ][<>.]*$
  -flex: .эсть<.>//.сть<.>
   gramm: 3.s,pl.s,pst
   gloss: PST.3PL
+ -flex: .ть<.>
+  gramm: 3.s,pl.s,pst
+  gloss: PST.3PL
+  regex-prev: .*с[<>.]*$
  paradigm: Clitics
 
 -paradigm: V-pst-ye
  -flex: .инь<.>
   gramm: 1.s,sg.s,pst
   gloss: PST.1SG
  -flex: .ить<.>
   gramm: 2.s,sg.s,pst
   gloss: PST.2SG
- -flex: .есь<.>//.сь<.>//.[ь]сь<.>//.[й]сь<.>
+ -flex: .етсь<.>//.есь<.>//.сь<.>//.[ь]сь<.>//.[й]сь<.>
   gramm: 3.s,sg.s,pst
   gloss: PST.3SG
  -flex: .инек<.>
   gramm: 1.s,pl.s,pst
   gloss: PST.1PL
  -flex: .иде<.>
   gramm: 2.s,pl.s,pst
   gloss: PST.2PL
- -flex: .есть<.>//.сть<.>//.[ь]сть<.>//.[й]сть<.>
+ -flex: .етсть<.>//.есть<.>//.сть<.>//.[ь]сть<.>//.[й]сть<.>
   gramm: 3.s,pl.s,pst
   gloss: PST.3PL
  paradigm: Clitics
 
 -paradigm: V-pst-ezj-voiceless
  -flex: .ть<.>//.[ь]ть<.>
   gramm: 3.s,pl.s,pst,non_obj
@@ -3722,15 +3768,15 @@
   gloss: IMP.2SG›3SG
  -flex: .нк<.>//.ньк<.>//.ҥк<.>
   gramm: imp,2.s,pl.s,1.o,sg.o
   gloss: IMP.2PL›3SG
  -flex: .мизь<.>//.мызь<.>
   gramm: imp,2.s,1.o,pl.o
   gloss: IMP.2›1PL
- -flex: .т<.>//.ть<.>
+ -flex: .ить<.>
   gramm: imp,2.s,sg.s,3.o,pl.o
   gloss: IMP.2SG›3PL
  -flex: .нк<.>//.ньк<.>//.ҥк<.>
   gramm: imp,2.s,pl.s,1.o,pl.o
   gloss: IMP.2PL›3PL
  paradigm: Clitics
 
@@ -3755,15 +3801,15 @@
   gloss: IMP.2PL›1SG
  -flex: .ньк<.>
   gramm: imp,2.s,pl.s,1.o,sg.o
   gloss: IMP.2PL›3SG
  -flex: .мизь<.>
   gramm: imp,2.s,1.o,pl.o
   gloss: IMP.2›1PL
- -flex: .ть<.>
+ -flex: .ить<.>
   gramm: imp,2.s,sg.s,3.o,pl.o
   gloss: IMP.2SG›3PL
  -flex: .ньк<.>
   gramm: imp,2.s,pl.s,1.o,pl.o
   gloss: IMP.2PL›3PL
 
 -paradigm: V-pst-obj
```

### Comparing `uniparser-erzya-1.1.2/uniparser_erzya.egg-info/PKG-INFO` & `uniparser-erzya-1.1.3/uniparser_erzya.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: uniparser-erzya
-Version: 1.1.2
+Version: 1.1.3
 Summary: Rule-based morphological analysis for Erzya
 Home-page: https://github.com/timarkh/uniparser-grammar-erzya
 Author: Timofey Arkhangelskiy
 Author-email: timarkh@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/timarkh/uniparser-grammar-erzya/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -60,9 +58,7 @@
 Disambiguation is not yet available for this language.
 
 ### Word lists
 Alternatively, you can use a preprocessed word list. The ``wordlists`` directory contains a list of words from a 2.3-million-word [Erzya corpus](http://erzya.web-corpora.net/) (``wordlist_main.csv``), list of analyzed tokens (``wordlist_analyzed.txt``; each line contains all possible analyses for one word in an XML format), and list of tokens the parser could not analyze (``wordlist_unanalyzed.txt``). The recall of the analyzer is 93.6% on literary texts and 90.7% on social media texts.
 
 ## Description format
 The description is carried out in the ``uniparser-morph`` format and involves a description of the inflection (paradigms.txt), a grammatical dictionary (kpv_lexemes_XXX.txt files), a list of rules that annotate combinations of lexemes and grammatical values with additional Russian translations (lex_rules.txt), and a short list of analyses that should be avoided (bad_analyses.txt). The dictionary contains descriptions of individual lexemes, each of which is accompanied by information about its stem, its part-of-speech tag and some other grammatical/borrowing information, its inflectional type (paradigm), and Russian translation. See more about the format [in the uniparser-morph documentation](https://uniparser-morph.readthedocs.io/en/latest/format.html).
-
-
```

### Comparing `uniparser-erzya-1.1.2/uniparser_erzya.egg-info/SOURCES.txt` & `uniparser-erzya-1.1.3/uniparser_erzya.egg-info/SOURCES.txt`

 * *Files identical despite different names*

