# Comparing `tmp/torch_snippets-0.500.tar.gz` & `tmp/torch_snippets-0.501.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_snippets-0.500.tar", last modified: Mon Jul 24 15:26:45 2023, max compression
+gzip compressed data, was "torch_snippets-0.501.tar", last modified: Wed Jul 26 09:45:30 2023, max compression
```

## Comparing `torch_snippets-0.500.tar` & `torch_snippets-0.501.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-24 15:26:45.225734 torch_snippets-0.500/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    11357 2021-12-31 15:06:08.000000 torch_snippets-0.500/LICENSE
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1062 2023-01-17 16:58:23.000000 torch_snippets-0.500/LICENSE.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      111 2021-12-31 15:06:08.000000 torch_snippets-0.500/MANIFEST.in
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5691 2023-07-24 15:26:45.226009 torch_snippets-0.500/PKG-INFO
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4999 2023-01-17 16:58:23.000000 torch_snippets-0.500/README.md
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      862 2023-07-24 15:26:22.000000 torch_snippets-0.500/settings.ini
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       79 2023-07-24 15:26:45.226663 torch_snippets-0.500/setup.cfg
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2001 2022-06-03 13:10:38.000000 torch_snippets-0.500/setup.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-24 15:26:45.220080 torch_snippets-0.500/torch_snippets/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      307 2023-07-24 15:26:43.000000 torch_snippets-0.500/torch_snippets/__init__.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    46227 2023-07-24 15:26:43.000000 torch_snippets-0.500/torch_snippets/_modidx.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4482 2023-01-17 16:58:25.000000 torch_snippets-0.500/torch_snippets/_nbdev.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6211 2023-07-24 15:26:42.000000 torch_snippets-0.500/torch_snippets/adapters.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    12112 2023-07-24 15:26:42.000000 torch_snippets-0.500/torch_snippets/bb_utils.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1436 2023-07-24 15:26:42.000000 torch_snippets-0.500/torch_snippets/bokeh_loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1672 2023-07-24 15:26:42.000000 torch_snippets-0.500/torch_snippets/charts.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1483 2023-07-24 13:12:35.000000 torch_snippets-0.500/torch_snippets/dates.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1206 2023-07-24 15:26:42.000000 torch_snippets-0.500/torch_snippets/decorators.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       73 2022-05-07 11:30:59.000000 torch_snippets-0.500/torch_snippets/fastcores.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4126 2023-07-24 15:26:42.000000 torch_snippets-0.500/torch_snippets/imgaug_loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     3429 2023-07-24 15:26:42.000000 torch_snippets-0.500/torch_snippets/inspector.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     8376 2023-07-24 15:26:43.000000 torch_snippets-0.500/torch_snippets/interactive_show.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4662 2023-07-24 15:26:43.000000 torch_snippets-0.500/torch_snippets/ipython.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      597 2023-07-24 15:26:43.000000 torch_snippets-0.500/torch_snippets/load_defaults.py
--rwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    20934 2023-07-24 14:02:41.000000 torch_snippets-0.500/torch_snippets/loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     3464 2023-07-24 15:26:43.000000 torch_snippets-0.500/torch_snippets/logger.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     7555 2023-07-24 15:26:43.000000 torch_snippets-0.500/torch_snippets/markup.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1654 2023-07-24 15:26:43.000000 torch_snippets-0.500/torch_snippets/misc.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     9763 2023-07-24 15:26:43.000000 torch_snippets-0.500/torch_snippets/paths.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1370 2023-07-24 15:26:43.000000 torch_snippets-0.500/torch_snippets/pdf_loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      822 2023-07-24 15:26:43.000000 torch_snippets-0.500/torch_snippets/registry.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6144 2023-07-24 15:26:43.000000 torch_snippets-0.500/torch_snippets/sklegos.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    14237 2023-06-10 19:35:22.000000 torch_snippets-0.500/torch_snippets/text_utils.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-24 15:26:45.223736 torch_snippets-0.500/torch_snippets/thinc_parser/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-24 15:26:43.000000 torch_snippets-0.500/torch_snippets/thinc_parser/__init__.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1082 2022-10-16 17:20:20.000000 torch_snippets-0.500/torch_snippets/thinc_parser/parser.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    13258 2022-11-08 11:22:58.000000 torch_snippets-0.500/torch_snippets/torch_loader.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-24 15:26:45.225159 torch_snippets-0.500/torch_snippets/trainer/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       23 2023-07-24 15:26:43.000000 torch_snippets-0.500/torch_snippets/trainer/__init__.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6802 2023-07-24 15:26:42.000000 torch_snippets-0.500/torch_snippets/trainer/capsule.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1537 2023-07-24 15:26:42.000000 torch_snippets-0.500/torch_snippets/trainer/config.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-24 15:26:45.222803 torch_snippets-0.500/torch_snippets.egg-info/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5691 2023-07-24 15:26:45.000000 torch_snippets-0.500/torch_snippets.egg-info/PKG-INFO
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1165 2023-07-24 15:26:45.000000 torch_snippets-0.500/torch_snippets.egg-info/SOURCES.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        1 2023-07-24 15:26:45.000000 torch_snippets-0.500/torch_snippets.egg-info/dependency_links.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-01-17 16:58:23.000000 torch_snippets-0.500/torch_snippets.egg-info/not-zip-safe
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      272 2023-07-24 15:26:45.000000 torch_snippets-0.500/torch_snippets.egg-info/requires.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       15 2023-07-24 15:26:45.000000 torch_snippets-0.500/torch_snippets.egg-info/top_level.txt
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-26 09:45:30.812419 torch_snippets-0.501/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    11357 2021-12-31 15:06:08.000000 torch_snippets-0.501/LICENSE
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1062 2023-01-17 16:58:23.000000 torch_snippets-0.501/LICENSE.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      111 2021-12-31 15:06:08.000000 torch_snippets-0.501/MANIFEST.in
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5691 2023-07-26 09:45:30.812938 torch_snippets-0.501/PKG-INFO
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4999 2023-01-17 16:58:23.000000 torch_snippets-0.501/README.md
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      862 2023-07-26 09:45:09.000000 torch_snippets-0.501/settings.ini
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       79 2023-07-26 09:45:30.813884 torch_snippets-0.501/setup.cfg
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2001 2022-06-03 13:10:38.000000 torch_snippets-0.501/setup.py
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-26 09:45:30.798189 torch_snippets-0.501/torch_snippets/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      307 2023-07-26 09:45:28.000000 torch_snippets-0.501/torch_snippets/__init__.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    46129 2023-07-26 09:45:28.000000 torch_snippets-0.501/torch_snippets/_modidx.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4482 2023-01-17 16:58:25.000000 torch_snippets-0.501/torch_snippets/_nbdev.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6211 2023-07-26 09:45:28.000000 torch_snippets-0.501/torch_snippets/adapters.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    12112 2023-07-26 09:45:28.000000 torch_snippets-0.501/torch_snippets/bb_utils.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1436 2023-07-26 09:45:28.000000 torch_snippets-0.501/torch_snippets/bokeh_loader.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1672 2023-07-26 09:45:28.000000 torch_snippets-0.501/torch_snippets/charts.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1539 2023-07-26 06:38:17.000000 torch_snippets-0.501/torch_snippets/dates.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1206 2023-07-26 09:45:28.000000 torch_snippets-0.501/torch_snippets/decorators.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       73 2022-05-07 11:30:59.000000 torch_snippets-0.501/torch_snippets/fastcores.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4126 2023-07-26 09:45:28.000000 torch_snippets-0.501/torch_snippets/imgaug_loader.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     3429 2023-07-26 09:45:28.000000 torch_snippets-0.501/torch_snippets/inspector.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     8376 2023-07-26 09:45:28.000000 torch_snippets-0.501/torch_snippets/interactive_show.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4662 2023-07-26 09:45:28.000000 torch_snippets-0.501/torch_snippets/ipython.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      597 2023-07-26 09:45:28.000000 torch_snippets-0.501/torch_snippets/load_defaults.py
+-rwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    20928 2023-07-26 06:29:56.000000 torch_snippets-0.501/torch_snippets/loader.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     3840 2023-07-26 09:45:28.000000 torch_snippets-0.501/torch_snippets/logger.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     7555 2023-07-26 09:45:28.000000 torch_snippets-0.501/torch_snippets/markup.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1657 2023-07-26 09:45:28.000000 torch_snippets-0.501/torch_snippets/misc.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     9763 2023-07-26 09:45:28.000000 torch_snippets-0.501/torch_snippets/paths.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1370 2023-07-26 09:45:28.000000 torch_snippets-0.501/torch_snippets/pdf_loader.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      822 2023-07-26 09:45:28.000000 torch_snippets-0.501/torch_snippets/registry.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6144 2023-07-26 09:45:28.000000 torch_snippets-0.501/torch_snippets/sklegos.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    14237 2023-06-10 19:35:22.000000 torch_snippets-0.501/torch_snippets/text_utils.py
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-26 09:45:30.808374 torch_snippets-0.501/torch_snippets/thinc_parser/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-26 09:45:28.000000 torch_snippets-0.501/torch_snippets/thinc_parser/__init__.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1082 2022-10-16 17:20:20.000000 torch_snippets-0.501/torch_snippets/thinc_parser/parser.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    13258 2022-11-08 11:22:58.000000 torch_snippets-0.501/torch_snippets/torch_loader.py
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-26 09:45:30.811118 torch_snippets-0.501/torch_snippets/trainer/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       23 2023-07-26 09:45:28.000000 torch_snippets-0.501/torch_snippets/trainer/__init__.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6802 2023-07-26 09:45:28.000000 torch_snippets-0.501/torch_snippets/trainer/capsule.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1537 2023-07-26 09:45:28.000000 torch_snippets-0.501/torch_snippets/trainer/config.py
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-26 09:45:30.806617 torch_snippets-0.501/torch_snippets.egg-info/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5691 2023-07-26 09:45:30.000000 torch_snippets-0.501/torch_snippets.egg-info/PKG-INFO
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1165 2023-07-26 09:45:30.000000 torch_snippets-0.501/torch_snippets.egg-info/SOURCES.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        1 2023-07-26 09:45:30.000000 torch_snippets-0.501/torch_snippets.egg-info/dependency_links.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-01-17 16:58:23.000000 torch_snippets-0.501/torch_snippets.egg-info/not-zip-safe
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      272 2023-07-26 09:45:30.000000 torch_snippets-0.501/torch_snippets.egg-info/requires.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       15 2023-07-26 09:45:30.000000 torch_snippets-0.501/torch_snippets.egg-info/top_level.txt
```

### Comparing `torch_snippets-0.500/LICENSE` & `torch_snippets-0.501/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.500/LICENSE.txt` & `torch_snippets-0.501/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.500/PKG-INFO` & `torch_snippets-0.501/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch_snippets
-Version: 0.500
+Version: 0.501
 Summary: One line functions for common tasks
 Home-page: https://github.com/sizhky/torch_snippets/tree/master/
 Author: Yeshwanth Reddy
 Author-email: 1992chinna@gmail.com
 License: Apache Software License 2.0
 Keywords: snippets,torch
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `torch_snippets-0.500/README.md` & `torch_snippets-0.501/README.md`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.500/settings.ini` & `torch_snippets-0.501/settings.ini`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 user = sizhky
 description = One line functions for common tasks
 keywords = snippets, torch
 author = Yeshwanth Reddy
 author_email = 1992chinna@gmail.com
 copyright = sizhky
 branch = master
-version = 0.500
+version = 0.501
 min_python = 3.7
 audience = Developers
 language = English
 custom_sidebar = False
 license = apache2
 status = 2
 requirements = fastcore matplotlib Pillow altair dill ipython loguru numpy pandas tqdm rich PyYAML catalogue confection pydantic typing srsly typing_extensions wasabi jsonlines imgaug>=0.4.0 xmltodict fuzzywuzzy scikit-learn nltk python-Levenshtein pre-commit pymupdf nbconvert nbformat
```

### Comparing `torch_snippets-0.500/setup.py` & `torch_snippets-0.501/setup.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.500/torch_snippets/_modidx.py` & `torch_snippets-0.501/torch_snippets/_modidx.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,16 +154,15 @@
                                               'torch_snippets.load_defaults.loadifexists': ( 'load_defautls.html#loadifexists',
                                                                                              'torch_snippets/load_defaults.py')},
             'torch_snippets.loader': {},
             'torch_snippets.logger': { 'torch_snippets.logger.RichHandler.render': ( 'logging.html#richhandler.render',
                                                                                      'torch_snippets/logger.py'),
                                        'torch_snippets.logger.enter_exit': ('logging.html#enter_exit', 'torch_snippets/logger.py'),
                                        'torch_snippets.logger.get_console': ('logging.html#get_console', 'torch_snippets/logger.py'),
-                                       'torch_snippets.logger.reset_logger_width': ( 'logging.html#reset_logger_width',
-                                                                                     'torch_snippets/logger.py')},
+                                       'torch_snippets.logger.reset_logger': ('logging.html#reset_logger', 'torch_snippets/logger.py')},
             'torch_snippets.markup': { 'torch_snippets.markup.AttrDict': ('markups.html#attrdict', 'torch_snippets/markup.py'),
                                        'torch_snippets.markup.AttrDict.__contains__': ( 'markups.html#attrdict.__contains__',
                                                                                         'torch_snippets/markup.py'),
                                        'torch_snippets.markup.AttrDict.__delitem__': ( 'markups.html#attrdict.__delitem__',
                                                                                        'torch_snippets/markup.py'),
                                        'torch_snippets.markup.AttrDict.__dir__': ( 'markups.html#attrdict.__dir__',
                                                                                    'torch_snippets/markup.py'),
```

### Comparing `torch_snippets-0.500/torch_snippets/_nbdev.py` & `torch_snippets-0.501/torch_snippets/_nbdev.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.500/torch_snippets/adapters.py` & `torch_snippets-0.501/torch_snippets/adapters.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.500/torch_snippets/bb_utils.py` & `torch_snippets-0.501/torch_snippets/bb_utils.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.500/torch_snippets/bokeh_loader.py` & `torch_snippets-0.501/torch_snippets/bokeh_loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.500/torch_snippets/charts.py` & `torch_snippets-0.501/torch_snippets/charts.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.500/torch_snippets/decorators.py` & `torch_snippets-0.501/torch_snippets/decorators.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.500/torch_snippets/imgaug_loader.py` & `torch_snippets-0.501/torch_snippets/imgaug_loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.500/torch_snippets/inspector.py` & `torch_snippets-0.501/torch_snippets/inspector.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.500/torch_snippets/interactive_show.py` & `torch_snippets-0.501/torch_snippets/interactive_show.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.500/torch_snippets/ipython.py` & `torch_snippets-0.501/torch_snippets/ipython.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.500/torch_snippets/load_defaults.py` & `torch_snippets-0.501/torch_snippets/load_defaults.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.500/torch_snippets/loader.py` & `torch_snippets-0.501/torch_snippets/loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     "xywh2xyXY",
     "df2bbs",
     "bbs2df",
     "Info",
     "Warn",
     "Debug",
     "Excep",
-    "reset_logger_width",
+    "reset_logger",
     "display",
     "typedispatch",
     "defaultdict",
     "Counter",
     "dcopy",
     "patch_to",
 ]
```

### Comparing `torch_snippets-0.500/torch_snippets/logger.py` & `torch_snippets-0.501/torch_snippets/logger.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/logging.ipynb.
 
 # %% auto 0
-__all__ = ['console', 'print', 'logger', 'Debug', 'Info', 'Warn', 'Excep', 'get_console', 'reset_logger_width', 'enter_exit']
+__all__ = ['console', 'print', 'reset_logger_width', 'logger', 'Debug', 'Info', 'Warn', 'Excep', 'get_console', 'reset_logger',
+           'enter_exit']
 
-# %% ../nbs/logging.ipynb 2
+# %% ../nbs/logging.ipynb 3
 from rich.console import Console
 from rich.theme import Theme
 from loguru import logger
 from datetime import datetime
-from fastcore.basics import patch_to
+from fastcore.basics import patch_to, ifnone
 from rich.logging import RichHandler
 from pathlib import Path
 
 # from torch_snippets.ipython import is_in_notebook
 
 from functools import wraps
 import time
 
-# %% ../nbs/logging.ipynb 3
+# %% ../nbs/logging.ipynb 4
 def get_console(width=None):
     return Console(
         width=width,
         theme=Theme(
             {
                 "repr.number": "bold cyan",
                 "repr.string": "bold green",
@@ -32,15 +33,15 @@
         ),
     )
 
 
 console = get_console()
 print = console.print
 
-# %% ../nbs/logging.ipynb 6
+# %% ../nbs/logging.ipynb 7
 @patch_to(RichHandler)
 def render(
     self,
     *,
     record,
     traceback,
     message_renderable: "ConsoleRenderable",
@@ -60,49 +61,54 @@
         path=path,
         line_no=f"{record.funcName}:{record.lineno}",
         link_path=record.pathname if self.enable_link_path else None,
     )
     return log_renderable
 
 
-logger.configure(
-    handlers=[
-        {
-            "sink": RichHandler(
-                rich_tracebacks=True, console=console, tracebacks_show_locals=False
-            ),
-            "format": "<level>{message}</level>",
-            "backtrace": True,
-        }
-    ]
-)
+def reset_logger(level="INFO", width=120, silent=True):
+    if level is not None:
+        [logger.remove() for _ in range(100)]
+        logger.configure(
+            handlers=[
+                {
+                    "sink": RichHandler(
+                        rich_tracebacks=True,
+                        console=console,
+                        tracebacks_show_locals=False,
+                    ),
+                    "format": "<level>{message}</level>",
+                    "backtrace": True,
+                    "level": level,
+                }
+            ],
+        )
+    if width is not None:
+        for handler_id in logger._core.handlers:
+            try:
+                handler = logger._core.handlers[handler_id]
+                handler._sink._handler.console = get_console(width=width)
+            except:
+                ...
+    if not silent:
+        logger.info(f"reset logger's console width to {width} and level to {level}!")
+
+
+reset_logger_width = lambda width: reset_logger(width=width)
+
+reset_logger(width=100, silent=True)
+reset_logger(width=100, silent=True)
 
 logger = logger
 
 Debug = lambda x, depth=0: logger.opt(depth=depth + 1).log("DEBUG", x)
 Info = lambda x, depth=0: logger.opt(depth=depth + 1).log("INFO", x)
 Warn = lambda x, depth=0: logger.opt(depth=depth + 1).log("WARNING", x)
 Excep = lambda x, depth=0: logger.opt(depth=depth + 1).log("ERROR", x)
 
-# %% ../nbs/logging.ipynb 9
-def reset_logger_width(logger, width):
-    for handler_id in logger._core.handlers:
-        try:
-            handler = logger._core.handlers[handler_id]
-            handler._sink._handler.console = get_console(width=width)
-            logger.info(f"reset logger's console width to {width}!")
-        except:
-            ...
-
-
-# Excep("TESTING {1,2,3}")
-# if is_in_notebook():
-#     reset_logger_width(logger, 115)
-# Excep("TESTING {1,2,3}")
-
 # %% ../nbs/logging.ipynb 10
 def enter_exit(func):
     """
     Logs the time taken to execute a function along with entry & exit time stamps
     """
     logger_ = logger.opt(depth=1)
```

### Comparing `torch_snippets-0.500/torch_snippets/markup.py` & `torch_snippets-0.501/torch_snippets/markup.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.500/torch_snippets/misc.py` & `torch_snippets-0.501/torch_snippets/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/misc.ipynb.
 
 # %% auto 0
 __all__ = ['Timer', 'timeit', 'io']
 
 # %% ../nbs/misc.ipynb 2
 import time
-from .logger import Info
+from .logger import Debug
 from .inspector import inspect
 
 # %% ../nbs/misc.ipynb 3
 class Timer:
     def __init__(self, N):
         "print elapsed time every iteration and print out remaining time"
         "assumes this timer is called exactly N times or less"
@@ -42,21 +42,21 @@
         self.ix += 1
 
 # %% ../nbs/misc.ipynb 5
 def timeit(func):
     def inner(*args, **kwargs):
         s = time.time()
         o = func(*args, **kwargs)
-        Info(f"{time.time() - s:.2f} seconds to execute `{func.__name__}`")
+        Debug(f"{time.time() - s:.2f} seconds to execute `{func.__name__}`")
         return o
 
     return inner
 
 
 def io(func):
     def inner(*args, **kwargs):
         s = time.time()
         o = func(*args, **kwargs)
-        Info(f"Args: {inspect(args)}\nKWargs: {inspect(kwargs)}\nOutput: {inspect(o)}")
+        Debug(f"Args: {inspect(args)}\nKWargs: {inspect(kwargs)}\nOutput: {inspect(o)}")
         return o
 
     return inner
```

### Comparing `torch_snippets-0.500/torch_snippets/paths.py` & `torch_snippets-0.501/torch_snippets/paths.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.500/torch_snippets/pdf_loader.py` & `torch_snippets-0.501/torch_snippets/pdf_loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.500/torch_snippets/registry.py` & `torch_snippets-0.501/torch_snippets/registry.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.500/torch_snippets/sklegos.py` & `torch_snippets-0.501/torch_snippets/sklegos.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.500/torch_snippets/text_utils.py` & `torch_snippets-0.501/torch_snippets/text_utils.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.500/torch_snippets/thinc_parser/parser.py` & `torch_snippets-0.501/torch_snippets/thinc_parser/parser.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.500/torch_snippets/torch_loader.py` & `torch_snippets-0.501/torch_snippets/torch_loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.500/torch_snippets/trainer/capsule.py` & `torch_snippets-0.501/torch_snippets/trainer/capsule.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.500/torch_snippets/trainer/config.py` & `torch_snippets-0.501/torch_snippets/trainer/config.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.500/torch_snippets.egg-info/PKG-INFO` & `torch_snippets-0.501/torch_snippets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-snippets
-Version: 0.500
+Version: 0.501
 Summary: One line functions for common tasks
 Home-page: https://github.com/sizhky/torch_snippets/tree/master/
 Author: Yeshwanth Reddy
 Author-email: 1992chinna@gmail.com
 License: Apache Software License 2.0
 Keywords: snippets,torch
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `torch_snippets-0.500/torch_snippets.egg-info/SOURCES.txt` & `torch_snippets-0.501/torch_snippets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

