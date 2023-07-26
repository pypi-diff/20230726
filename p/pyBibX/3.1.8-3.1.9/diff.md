# Comparing `tmp/pyBibX-3.1.8.tar.gz` & `tmp/pyBibX-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyBibX-3.1.8.tar", last modified: Tue Jul 25 12:42:52 2023, max compression
+gzip compressed data, was "dist\pyBibX-3.1.9.tar", last modified: Wed Jul 26 20:31:06 2023, max compression
```

## Comparing `pyBibX-3.1.8.tar` & `pyBibX-3.1.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 12:42:52.000000 pyBibX-3.1.8/
--rw-rw-rw-   0        0        0      644 2022-03-01 19:24:07.000000 pyBibX-3.1.8/LICENSE
--rw-rw-rw-   0        0        0       40 2022-05-19 14:46:22.000000 pyBibX-3.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     9608 2023-07-25 12:42:52.000000 pyBibX-3.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     9165 2023-05-06 14:18:32.000000 pyBibX-3.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 12:42:51.000000 pyBibX-3.1.8/pyBibX/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-3.1.8/pyBibX/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 12:42:51.000000 pyBibX-3.1.8/pyBibX/base/
--rw-rw-rw-   0        0        0       27 2022-03-16 15:26:25.000000 pyBibX-3.1.8/pyBibX/base/__init__.py
--rw-rw-rw-   0        0        0   265828 2023-07-25 12:41:38.000000 pyBibX-3.1.8/pyBibX/base/pbx.py
-drwxrwxrwx   0        0        0        0 2023-07-25 12:42:52.000000 pyBibX-3.1.8/pyBibX/base/stws/
--rw-rw-rw-   0        0        0     6482 2023-05-31 13:32:50.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Arabic.txt
--rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Bengali.txt
--rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Bulgarian.txt
--rw-rw-rw-   0        0        0     3295 2023-05-28 21:46:34.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Chinese.txt
--rw-rw-rw-   0        0        0     1934 2023-05-31 13:36:06.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Czech.txt
--rw-rw-rw-   0        0        0     4284 2023-05-31 13:37:00.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-English.txt
--rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Finnish.txt
--rw-rw-rw-   0        0        0     3484 2023-05-31 13:37:46.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-French.txt
--rw-rw-rw-   0        0        0     4302 2023-05-31 13:39:46.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-German.txt
--rw-rw-rw-   0        0        0     7901 2023-05-28 21:47:27.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Greek.txt
--rw-rw-rw-   0        0        0     1656 2023-05-28 21:47:36.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Hebrew.txt
--rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Hindi.txt
--rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Hungarian.txt
--rw-rw-rw-   0        0        0     4074 2023-05-31 13:48:26.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Italian.txt
--rw-rw-rw-   0        0        0     2202 2023-05-28 21:48:04.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Japanese.txt
--rw-rw-rw-   0        0        0     7417 2023-05-28 21:48:29.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Korean.txt
--rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Marathi.txt
--rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Persian.txt
--rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Polish.txt
--rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Portuguese-br.txt
--rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Romanian.txt
--rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Russian.txt
--rw-rw-rw-   0        0        0      883 2023-05-28 21:48:40.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Slovak.txt
--rw-rw-rw-   0        0        0     3128 2023-05-31 13:53:58.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Spanish.txt
--rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Swedish.txt
--rw-rw-rw-   0        0        0     1521 2023-05-28 21:58:26.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Thai.txt
--rw-rw-rw-   0        0        0      627 2023-05-28 21:49:00.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Ukrainian.txt
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-3.1.8/pyBibX/base/stws/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 12:42:51.000000 pyBibX-3.1.8/pyBibX.egg-info/
--rw-rw-rw-   0        0        0     9608 2023-07-25 12:42:50.000000 pyBibX-3.1.8/pyBibX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1354 2023-07-25 12:42:50.000000 pyBibX-3.1.8/pyBibX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 12:42:50.000000 pyBibX-3.1.8/pyBibX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      218 2023-07-25 12:42:50.000000 pyBibX-3.1.8/pyBibX.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-25 12:42:50.000000 pyBibX-3.1.8/pyBibX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-07-25 12:42:50.000000 pyBibX-3.1.8/pyBibX.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-07-25 12:42:52.000000 pyBibX-3.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1101 2023-07-25 12:41:51.000000 pyBibX-3.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 20:31:06.000000 pyBibX-3.1.9/
+-rw-rw-rw-   0        0        0      644 2022-03-01 19:24:07.000000 pyBibX-3.1.9/LICENSE
+-rw-rw-rw-   0        0        0       40 2022-05-19 14:46:22.000000 pyBibX-3.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     9608 2023-07-26 20:31:06.000000 pyBibX-3.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     9165 2023-05-06 14:18:32.000000 pyBibX-3.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 20:31:06.000000 pyBibX-3.1.9/pyBibX/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-3.1.9/pyBibX/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 20:31:06.000000 pyBibX-3.1.9/pyBibX/base/
+-rw-rw-rw-   0        0        0       27 2022-03-16 15:26:25.000000 pyBibX-3.1.9/pyBibX/base/__init__.py
+-rw-rw-rw-   0        0        0   268495 2023-07-26 20:29:07.000000 pyBibX-3.1.9/pyBibX/base/pbx.py
+drwxrwxrwx   0        0        0        0 2023-07-26 20:31:06.000000 pyBibX-3.1.9/pyBibX/base/stws/
+-rw-rw-rw-   0        0        0     6482 2023-05-31 13:32:50.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Arabic.txt
+-rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Bengali.txt
+-rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Bulgarian.txt
+-rw-rw-rw-   0        0        0     3295 2023-05-28 21:46:34.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Chinese.txt
+-rw-rw-rw-   0        0        0     1934 2023-05-31 13:36:06.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Czech.txt
+-rw-rw-rw-   0        0        0     4284 2023-05-31 13:37:00.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-English.txt
+-rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Finnish.txt
+-rw-rw-rw-   0        0        0     3484 2023-05-31 13:37:46.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-French.txt
+-rw-rw-rw-   0        0        0     4302 2023-05-31 13:39:46.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-German.txt
+-rw-rw-rw-   0        0        0     7901 2023-05-28 21:47:27.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Greek.txt
+-rw-rw-rw-   0        0        0     1656 2023-05-28 21:47:36.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Hebrew.txt
+-rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Hindi.txt
+-rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Hungarian.txt
+-rw-rw-rw-   0        0        0     4074 2023-05-31 13:48:26.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Italian.txt
+-rw-rw-rw-   0        0        0     2202 2023-05-28 21:48:04.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Japanese.txt
+-rw-rw-rw-   0        0        0     7417 2023-05-28 21:48:29.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Korean.txt
+-rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Marathi.txt
+-rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Persian.txt
+-rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Polish.txt
+-rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Portuguese-br.txt
+-rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Romanian.txt
+-rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Russian.txt
+-rw-rw-rw-   0        0        0      883 2023-05-28 21:48:40.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Slovak.txt
+-rw-rw-rw-   0        0        0     3128 2023-05-31 13:53:58.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Spanish.txt
+-rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Swedish.txt
+-rw-rw-rw-   0        0        0     1521 2023-05-28 21:58:26.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Thai.txt
+-rw-rw-rw-   0        0        0      627 2023-05-28 21:49:00.000000 pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Ukrainian.txt
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-3.1.9/pyBibX/base/stws/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 20:31:06.000000 pyBibX-3.1.9/pyBibX.egg-info/
+-rw-rw-rw-   0        0        0     9608 2023-07-26 20:31:04.000000 pyBibX-3.1.9/pyBibX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1354 2023-07-26 20:31:05.000000 pyBibX-3.1.9/pyBibX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 20:31:04.000000 pyBibX-3.1.9/pyBibX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      218 2023-07-26 20:31:04.000000 pyBibX-3.1.9/pyBibX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-26 20:31:04.000000 pyBibX-3.1.9/pyBibX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-26 20:31:04.000000 pyBibX-3.1.9/pyBibX.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-07-26 20:31:06.000000 pyBibX-3.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1101 2023-07-26 20:29:21.000000 pyBibX-3.1.9/setup.py
```

### Comparing `pyBibX-3.1.8/LICENSE` & `pyBibX-3.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.8/PKG-INFO` & `pyBibX-3.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBibX
-Version: 3.1.8
+Version: 3.1.9
 Summary: A Bibliometric and Scientometric Library Powered with Artificial Intelligence Tools
 Home-page: https://github.com/Valdecy/pyBibX
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyBibX-3.1.8/README.md` & `pyBibX-3.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.8/pyBibX/base/pbx.py` & `pyBibX-3.1.9/pyBibX/base/pbx.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,29 +50,29 @@
 
 ############################################################################
 
 # pbx Class
 class pbx_probe():
     def __init__(self, file_bib, db = 'scopus', del_duplicated = True):
         self.institution_names =  [ 
-                                    'acad', 'academy', 'ctr', 'center', 'centre', 'chuo kikuu', 'cient', 'coll', 'college', 'conservatory', 
-                                    'egyetemi', 'escola', 'education', 'escuela', 'eyunivesithi', 'fac', 'faculdade', 'facultad', 'fakultet', 
-                                    'fakultät', 'fdn', 'fundacion', 'foundation', 'gradevinski', 'higher', 'hsch', 'hochschule', 'hgsk', 
-                                    'hogeschool',  'háskóli', 'högskola', 'ibmec', 'inivèsite', 'ist', 'istituto', 'institutional', 'int', 'inst', 
-                                    'institut', 'institute', 'institute of technology',  'inyuvesi', 'iskola', 'iunivesite', 'jaamacad', "jami'a", 
-                                    'kolej', 'koulu', 'kulanui', 'lab.', 'lab', 'labs', 'laborat', 'mahadum', 'med', 'medicine', 'medical', 
-                                    'observatory', 'oilthigh', 'okulu', 'ollscoile', 'oniversite', 'politecnico', 'polytechnic', 'prifysgol', 'rech', 
-                                    'recherche', 'research', 'sch', 'school', 'schule', 'scuola', 'seminary', 'skola', 'supérieur', 'sveučilište', 
-                                    'szkoła', 'tech', 'technical', 'technische', 'technique', 'technological', 'uff', 
-                                    'unibersidad', 'unibertsitatea', 'univ', 'universidad', 'universidade', 'universitas', 'universitat', 
-                                    'universitate', 'universitato', 'universite', 'universiteit', 'universitet', 'universitetas', 'universiti', 
-                                    'university', 'università', 'universität', 'université', 'universitāte', 'univerza', 'univerzita',
-                                    'univerzitet', 'univesithi', 'uniwersytet', 'vniuersitatis', 'whare wananga', 'yliopisto',
-                                    'yunifasiti', 'yunivesite', 'yunivhesiti', 'zanko', 'école', 'ülikool', 'üniversite',
-                                    'πανεπιστήμιο', 'σχολείο', 'универзитет', 'университет', 'універсітэт', 'школа'
+                                    'acad', 'academy', 'akad', 'aachen', 'assoc', 'cambridge', 'ctr', 'cefet', 'center', 'centre', 'chuo kikuu', 
+                                    'cient', 'coll', 'college', 'colegio', 'conservatory', 'dept', 'egyetemi', 'escola', 'education', 'escuela', 
+                                    'eyunivesithi', 'fac', 'faculdade', 'facultad', 'fakultet', 'fakultät', 'fdn', 'fundacion', 'foundation', 
+                                    'gradevinski', 'higher', 'hsch', 'hochschule', 'hosp', 'hgsk', 'hogeschool',  'háskóli', 'högskola', 'ibmec', 
+                                    'inivèsite', 'ist', 'istituto', 'imd', 'institutional', 'int', 'inst',  'institut', 'institute', 
+                                    'institute of technology',  'inyuvesi', 'iskola', 'iunivesite', 'jaamacad', "jami'a",  'kolej', 'koulu', 
+                                    'kulanui', 'lab.', 'lab', 'labs', 'laborat', 'learning', 'mahadum', 'med', 'medicine', 'medical', 'observatory', 
+                                    'oilthigh', 'okulu', 'ollscoile', 'oniversite', 'politecnico', 'polytechnic', 'prifysgol', 'rech', 'recherche', 
+                                    'research', 'sch', 'school', 'schule', 'scuola', 'seminary', 'skola', 'supérieur', 'sveučilište', 'szkoła', 
+                                    'tech', 'technical', 'technische', 'technique', 'technological', 'uff', 'uned', 'unibersidad', 'unibertsitatea', 
+                                    'univ', 'universidad', 'universidade', 'universitas', 'universitat', 'universitate', 'universitato', 
+                                    'universite', 'universiteit', 'universitet', 'universitetas', 'universiti', 'university', 'università', 
+                                    'universität', 'université', 'universitāte', 'univerza', 'univerzita','univerzitet', 'univesithi', 'uniwersytet', 
+                                    'vniuersitatis', 'whare wananga', 'yliopisto','yunifasiti', 'yunivesite', 'yunivhesiti', 'zanko', 'école', 
+                                    'ülikool', 'üniversite','πανεπιστήμιο', 'σχολείο', 'универзитет', 'университет', 'універсітэт', 'школа'
                                   ]
 
         self.language_names  =    { 
                                     'afr': 'Afrikaans', 'alb': 'Albanian','amh': 'Amharic', 'ara': 'Arabic', 'arm': 'Armenian', 
                                     'aze': 'Azerbaijani', 'bos': 'Bosnian', 'bul': 'Bulgarian', 'cat': 'Catalan', 'chi': 'Chinese', 
                                     'cze': 'Czech', 'dan': 'Danish', 'dut': 'Dutch', 'eng': 'English', 'epo': 'Esperanto', 
                                     'est': 'Estonian', 'fin': 'Finnish', 'fre': 'French', 'geo': 'Georgian', 'ger': 'German', 
@@ -123,15 +123,15 @@
                                    'Suriname', 'Svalbard and Jan Mayen', 'Sweden', 'Switzerland', 'Syrian Arab Republic', 'Taiwan', 
                                    'Tajikistan', 'Tanzania', 'Thailand', 'Timor-Leste', 'Togo', 'Tokelau', 'Tonga', 
                                    'Trinidad and Tobago', 'Tunisia', 'Turkey', 'Turkmenistan', 'Turks and Caicos Islands', 'Tuvalu', 
                                    'Uganda', 'Ukraine', 'United Arab Emirates', 'United Kingdom', 
                                    'United States Minor Outlying Islands', 'United States of America', 'Uruguay', 'Uzbekistan', 
                                    'Vanuatu', 'Venezuela', 'Viet Nam', 'Virgin Islands (British)', 'Virgin Islands (U.S.)', 
                                    'Wallis and Futuna', 'Western Sahara', 'Yemen', 'Zambia', 'Zimbabwe', 'Aland Islands'
-                                  ]
+                                  ] 
         self.country_alpha_2 =    [
                                    'AF', 'AL', 'DZ', 'AS', 'AD', 'AO', 'AI', 'AQ', 'AG', 'AR', 'AM', 'AW', 'AU', 'AT', 'AZ', 'BS', 
                                    'BH', 'BD', 'BB', 'BY', 'BE', 'BZ', 'BJ', 'BM', 'BT', 'BO', 'BQ', 'BA', 'BW', 'BV', 'BR', 'IO', 
                                    'BN', 'BG', 'BF', 'BI', 'CV', 'KH', 'CM', 'CA', 'KY', 'CF', 'TD', 'CL', 'CN', 'CX', 'CC', 'CO', 
                                    'KM', 'CD', 'CG', 'CK', 'CR', 'HR', 'CU', 'CW', 'CY', 'CZ', 'CI', 'DK', 'DJ', 'DM', 'DO', 'EC', 
                                    'EG', 'SV', 'GQ', 'ER', 'EE', 'SZ', 'ET', 'FK', 'FO', 'FJ', 'FI', 'FR', 'GF', 'PF', 'TF', 'GA', 
                                    'GM', 'GE', 'DE', 'GH', 'GI', 'GR', 'GL', 'GD', 'GP', 'GU', 'GT', 'GG', 'GN', 'GW', 'GY', 'HT', 
@@ -1253,33 +1253,66 @@
     def __get_countries(self):
         df = pd.Series(np.zeros(self.data.shape[0]))
         for i in range(0, self.data.shape[0]):
             if (self.data.loc[i, 'source'].lower() == 'scopus' or self.data.loc[i, 'source'].lower() == 'pubmed'):
                 df[i] = self.data.loc[i, 'affiliation']
             elif (self.data.loc[i, 'source'].lower() == 'wos'):
                 df[i] = self.data.loc[i, 'affiliation_'].replace('(Corresponding Author)', '')
+                if (',' in df[i] and ', ' not in df[i]):
+                    df[i] = df[i].replace(',', ', ')
         df = df.str.replace(' USA',            ' United States of America',   case = False, regex = True)
         df = df.str.replace('ENGLAND',         'United Kingdom',              case = False, regex = True)
         df = df.str.replace('Antigua & Barbu', 'Antigua and Barbuda',         case = False, regex = True)
         df = df.str.replace('Bosnia & Herceg', 'Bosnia and Herzegovina',      case = False, regex = True)
         df = df.str.replace('Cent Afr Republ', 'Central African Republic',    case = False, regex = True)
+        df = df.str.replace('Czech Republic',  'Czechia',                     case = False, regex = True)
         df = df.str.replace('Dominican Rep',   'Dominican Republic',          case = False, regex = True)
         df = df.str.replace('Equat Guinea',    'Equatorial Guinea',           case = False, regex = True)
         df = df.str.replace('Fr Austr Lands',  'French Southern Territories', case = False, regex = True)
         df = df.str.replace('Fr Polynesia',    'French Polynesia',            case = False, regex = True)
         df = df.str.replace('Malagasy Republ', 'Madagascar',                  case = False, regex = True)
         df = df.str.replace('Mongol Peo Rep',  'Mongolia',                    case = False, regex = True)
         df = df.str.replace('Neth Antilles',   'Saint Martin',                case = False, regex = True)
         df = df.str.replace('North Ireland',   'Ireland',                     case = False, regex = True)
         df = df.str.replace('Peoples R China', 'China',                       case = False, regex = True)
         df = df.str.replace('Rep of Georgia',  'Georgia',                     case = False, regex = True)
+        df = df.str.replace('Russia',          'Russian Federation',          case = False, regex = True)
         df = df.str.replace('Sao Tome E Prin', 'Sao Tome and Principe',       case = False, regex = True)
+        df = df.str.replace('Scotland',        'United Kingdom',              case = False, regex = True)
         df = df.str.replace('St Kitts & Nevi', 'Saint Kitts and Nevis',       case = False, regex = True)
         df = df.str.replace('Trinid & Tobago', 'Trinidad and Tobago',         case = False, regex = True)
         df = df.str.replace('U Arab Emirates', 'United Arab Emirates',        case = False, regex = True)
+        df = df.str.replace('USA',             'United States of America',    case = False, regex = True)
+        df = df.str.replace('VietNam',         'Viet Nam',                    case = False, regex = True)
+        #for i in range(0, df.shape[0]):
+            #df[i] = df[i].replace(' USA',            ' United States of America')
+            #df[i] = df[i].replace('ENGLAND',         'United Kingdom')
+            #df[i] = df[i].replace('Antigua & Barbu', 'Antigua and Barbuda')
+            #df[i] = df[i].replace('Bosnia & Herceg', 'Bosnia and Herzegovina')
+            #df[i] = df[i].replace('Cent Afr Republ', 'Central African Republic')
+            #df[i] = df[i].replace('Czech Republic',  'Czechia')
+            #df[i] = df[i].replace('Dominican Rep',   'Dominican Republic')
+            #df[i] = df[i].replace('England',         'United Kingdom')
+            #df[i] = df[i].replace('Equat Guinea',    'Equatorial Guinea')
+            #df[i] = df[i].replace('Fr Austr Lands',  'French Southern Territories')
+            #df[i] = df[i].replace('Fr Polynesia',    'French Polynesia')
+            #df[i] = df[i].replace('Malagasy Republ', 'Madagascar')
+            #df[i] = df[i].replace('Mongol Peo Rep',  'Mongolia')
+            #df[i] = df[i].replace('Neth Antilles',   'Saint Martin')
+            #df[i] = df[i].replace('North Ireland',   'Ireland')
+            #df[i] = df[i].replace('Peoples R China', 'China')
+            #df[i] = df[i].replace('Rep of Georgia',  'Georgia')
+            #df[i] = df[i].replace('Russia',          'Russian Federation')
+            #df[i] = df[i].replace('Sao Tome E Prin', 'Sao Tome and Principe')
+            #df[i] = df[i].replace('Scotland',        'United Kingdom')
+            #df[i] = df[i].replace('St Kitts & Nevi', 'Saint Kitts and Nevis')
+            #df[i] = df[i].replace('Trinid & Tobago', 'Trinidad and Tobago')
+            #df[i] = df[i].replace('U Arab Emirates', 'United Arab Emirates')
+            #df[i] = df[i].replace('USA',             'United States of America')
+            #df[i] = df[i].replace('VietNam',         'Viet Nam')
         df = df.str.lower()
         for i in range(0, len(self.aut)):
             for j in range(0, len(self.aut[i])):
                 for k in range(0, df.shape[0]):
                     df[k] = df[k].replace(self.aut[i][j], self.aut[i][j].replace('.', ''))
         ctrs = [[] for i in range(0, df.shape[0])]
         for i in range(0, self.data.shape[0]):
```

### Comparing `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Arabic.txt` & `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Arabic.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Bengali.txt` & `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Bengali.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Bulgarian.txt` & `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Bulgarian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Chinese.txt` & `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Chinese.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Czech.txt` & `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Czech.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-English.txt` & `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-English.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Finnish.txt` & `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Finnish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-French.txt` & `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-French.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-German.txt` & `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-German.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Greek.txt` & `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Greek.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Hebrew.txt` & `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Hebrew.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Hindi.txt` & `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Hindi.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Hungarian.txt` & `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Hungarian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Italian.txt` & `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Italian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Japanese.txt` & `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Japanese.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Korean.txt` & `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Korean.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Marathi.txt` & `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Marathi.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Persian.txt` & `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Persian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Polish.txt` & `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Polish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Portuguese-br.txt` & `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Portuguese-br.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Romanian.txt` & `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Romanian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Russian.txt` & `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Russian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Slovak.txt` & `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Slovak.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Spanish.txt` & `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Spanish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Swedish.txt` & `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Swedish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Thai.txt` & `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Thai.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Ukrainian.txt` & `pyBibX-3.1.9/pyBibX/base/stws/Stopwords-Ukrainian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.8/pyBibX.egg-info/PKG-INFO` & `pyBibX-3.1.9/pyBibX.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBibX
-Version: 3.1.8
+Version: 3.1.9
 Summary: A Bibliometric and Scientometric Library Powered with Artificial Intelligence Tools
 Home-page: https://github.com/Valdecy/pyBibX
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyBibX-3.1.8/pyBibX.egg-info/SOURCES.txt` & `pyBibX-3.1.9/pyBibX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.8/setup.py` & `pyBibX-3.1.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyBibX',
-    version='3.1.8',
+    version='3.1.9',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyBibX',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
```

