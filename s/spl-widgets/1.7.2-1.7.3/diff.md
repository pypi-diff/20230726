# Comparing `tmp/spl_widgets-1.7.2.tar.gz` & `tmp/spl_widgets-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spl_widgets-1.7.2.tar", last modified: Wed Jul 26 19:01:12 2023, max compression
+gzip compressed data, was "spl_widgets-1.7.3.tar", last modified: Wed Jul 26 19:07:05 2023, max compression
```

## Comparing `spl_widgets-1.7.2.tar` & `spl_widgets-1.7.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 19:01:12.722581 spl_widgets-1.7.2/
--rw-r--r--   0 colin      (501) staff       (20)     1073 2021-11-03 16:44:37.000000 spl_widgets-1.7.2/LICENSE
--rw-r--r--   0 colin      (501) staff       (20)      411 2023-07-26 19:01:12.722450 spl_widgets-1.7.2/PKG-INFO
--rw-r--r--   0 colin      (501) staff       (20)     2101 2022-06-26 15:02:40.000000 spl_widgets-1.7.2/README.md
--rw-r--r--   0 colin      (501) staff       (20)      103 2021-11-03 16:36:22.000000 spl_widgets-1.7.2/pyproject.toml
--rw-r--r--   0 colin      (501) staff       (20)       38 2023-07-26 19:01:12.722623 spl_widgets-1.7.2/setup.cfg
--rw-r--r--   0 colin      (501) staff       (20)     1240 2023-07-26 19:01:05.000000 spl_widgets-1.7.2/setup.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 19:01:12.709608 spl_widgets-1.7.2/src/
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 19:01:12.712125 spl_widgets-1.7.2/src/spl_widgets/
--rw-r--r--   0 colin      (501) staff       (20)      279 2022-06-26 16:32:08.000000 spl_widgets-1.7.2/src/spl_widgets/__init__.py
--rw-r--r--   0 colin      (501) staff       (20)        0 2022-06-26 14:59:05.000000 spl_widgets-1.7.2/src/spl_widgets/__main__.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 19:01:12.713526 spl_widgets-1.7.2/src/spl_widgets/autoscorer/
--rw-r--r--   0 colin      (501) staff       (20)    14016 2023-07-26 18:59:47.000000 spl_widgets-1.7.2/src/spl_widgets/autoscorer/autoscore.py
--rw-r--r--   0 colin      (501) staff       (20)    18685 2023-07-26 19:00:37.000000 spl_widgets-1.7.2/src/spl_widgets/autoscorer/autoscorer_gui.py
--rw-r--r--   0 colin      (501) staff       (20)     5387 2023-07-02 19:26:17.000000 spl_widgets-1.7.2/src/spl_widgets/autoscorer/tokenize_to_ipa.py
--rw-r--r--   0 colin      (501) staff       (20)     3722 2023-05-26 16:24:48.000000 spl_widgets-1.7.2/src/spl_widgets/batch_tune.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 19:01:12.720431 spl_widgets-1.7.2/src/spl_widgets/data/
--rw-r--r--   0 colin      (501) staff       (20)  9670656 2023-05-26 16:25:12.000000 spl_widgets-1.7.2/src/spl_widgets/data/cmudict.sqlite
--rw-r--r--   0 colin      (501) staff       (20)       73 2023-07-26 16:35:15.000000 spl_widgets-1.7.2/src/spl_widgets/data/help_text.json
--rwxr-xr-x   0 colin      (501) staff       (20)     5378 2022-10-21 13:14:40.000000 spl_widgets-1.7.2/src/spl_widgets/gorilla_clean.py
--rw-r--r--   0 colin      (501) staff       (20)     2483 2022-12-17 21:45:28.000000 spl_widgets-1.7.2/src/spl_widgets/jukemake.py
--rw-r--r--   0 colin      (501) staff       (20)     4166 2023-05-25 22:28:36.000000 spl_widgets-1.7.2/src/spl_widgets/misc_util.py
--rwxr-xr-x   0 colin      (501) staff       (20)     3598 2023-04-14 19:27:21.000000 spl_widgets-1.7.2/src/spl_widgets/stk_swx.py
--rw-r--r--   0 colin      (501) staff       (20)     3614 2023-04-23 14:58:27.000000 spl_widgets-1.7.2/src/spl_widgets/tune_freq.py
--rw-r--r--   0 colin      (501) staff       (20)    17694 2023-05-26 16:20:21.000000 spl_widgets-1.7.2/src/spl_widgets/tuner.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 19:01:12.722242 spl_widgets-1.7.2/src/spl_widgets/util/
--rw-r--r--   0 colin      (501) staff       (20)     1169 2023-07-10 17:51:43.000000 spl_widgets-1.7.2/src/spl_widgets/util/color_util.py
--rw-r--r--   0 colin      (501) staff       (20)     5635 2023-07-26 16:35:15.000000 spl_widgets-1.7.2/src/spl_widgets/util/gui_util.py
--rw-r--r--   0 colin      (501) staff       (20)     3642 2023-05-26 16:25:13.000000 spl_widgets-1.7.2/src/spl_widgets/util/sqlite_db.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 19:01:12.713022 spl_widgets-1.7.2/src/spl_widgets.egg-info/
--rw-r--r--   0 colin      (501) staff       (20)      411 2023-07-26 19:01:12.000000 spl_widgets-1.7.2/src/spl_widgets.egg-info/PKG-INFO
--rw-r--r--   0 colin      (501) staff       (20)      839 2023-07-26 19:01:12.000000 spl_widgets-1.7.2/src/spl_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 colin      (501) staff       (20)        1 2023-07-26 19:01:12.000000 spl_widgets-1.7.2/src/spl_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 colin      (501) staff       (20)      265 2023-07-26 19:01:12.000000 spl_widgets-1.7.2/src/spl_widgets.egg-info/entry_points.txt
--rw-r--r--   0 colin      (501) staff       (20)       43 2023-07-26 19:01:12.000000 spl_widgets-1.7.2/src/spl_widgets.egg-info/requires.txt
--rw-r--r--   0 colin      (501) staff       (20)       12 2023-07-26 19:01:12.000000 spl_widgets-1.7.2/src/spl_widgets.egg-info/top_level.txt
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 19:07:05.666792 spl_widgets-1.7.3/
+-rw-r--r--   0 colin      (501) staff       (20)     1073 2021-11-03 16:44:37.000000 spl_widgets-1.7.3/LICENSE
+-rw-r--r--   0 colin      (501) staff       (20)      411 2023-07-26 19:07:05.666671 spl_widgets-1.7.3/PKG-INFO
+-rw-r--r--   0 colin      (501) staff       (20)     2101 2022-06-26 15:02:40.000000 spl_widgets-1.7.3/README.md
+-rw-r--r--   0 colin      (501) staff       (20)      103 2021-11-03 16:36:22.000000 spl_widgets-1.7.3/pyproject.toml
+-rw-r--r--   0 colin      (501) staff       (20)       38 2023-07-26 19:07:05.666833 spl_widgets-1.7.3/setup.cfg
+-rw-r--r--   0 colin      (501) staff       (20)     1240 2023-07-26 19:06:57.000000 spl_widgets-1.7.3/setup.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 19:07:05.658722 spl_widgets-1.7.3/src/
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 19:07:05.660621 spl_widgets-1.7.3/src/spl_widgets/
+-rw-r--r--   0 colin      (501) staff       (20)      279 2022-06-26 16:32:08.000000 spl_widgets-1.7.3/src/spl_widgets/__init__.py
+-rw-r--r--   0 colin      (501) staff       (20)        0 2022-06-26 14:59:05.000000 spl_widgets-1.7.3/src/spl_widgets/__main__.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 19:07:05.661928 spl_widgets-1.7.3/src/spl_widgets/autoscorer/
+-rw-r--r--   0 colin      (501) staff       (20)    14016 2023-07-26 18:59:47.000000 spl_widgets-1.7.3/src/spl_widgets/autoscorer/autoscore.py
+-rw-r--r--   0 colin      (501) staff       (20)    18685 2023-07-26 19:00:37.000000 spl_widgets-1.7.3/src/spl_widgets/autoscorer/autoscorer_gui.py
+-rw-r--r--   0 colin      (501) staff       (20)     5389 2023-07-26 19:06:46.000000 spl_widgets-1.7.3/src/spl_widgets/autoscorer/tokenize_to_ipa.py
+-rw-r--r--   0 colin      (501) staff       (20)     3722 2023-05-26 16:24:48.000000 spl_widgets-1.7.3/src/spl_widgets/batch_tune.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 19:07:05.666136 spl_widgets-1.7.3/src/spl_widgets/data/
+-rw-r--r--   0 colin      (501) staff       (20)  9670656 2023-05-26 16:25:12.000000 spl_widgets-1.7.3/src/spl_widgets/data/cmudict.sqlite
+-rw-r--r--   0 colin      (501) staff       (20)       73 2023-07-26 16:35:15.000000 spl_widgets-1.7.3/src/spl_widgets/data/help_text.json
+-rwxr-xr-x   0 colin      (501) staff       (20)     5378 2022-10-21 13:14:40.000000 spl_widgets-1.7.3/src/spl_widgets/gorilla_clean.py
+-rw-r--r--   0 colin      (501) staff       (20)     2483 2022-12-17 21:45:28.000000 spl_widgets-1.7.3/src/spl_widgets/jukemake.py
+-rw-r--r--   0 colin      (501) staff       (20)     4166 2023-05-25 22:28:36.000000 spl_widgets-1.7.3/src/spl_widgets/misc_util.py
+-rwxr-xr-x   0 colin      (501) staff       (20)     3598 2023-04-14 19:27:21.000000 spl_widgets-1.7.3/src/spl_widgets/stk_swx.py
+-rw-r--r--   0 colin      (501) staff       (20)     3614 2023-04-23 14:58:27.000000 spl_widgets-1.7.3/src/spl_widgets/tune_freq.py
+-rw-r--r--   0 colin      (501) staff       (20)    17694 2023-05-26 16:20:21.000000 spl_widgets-1.7.3/src/spl_widgets/tuner.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 19:07:05.666501 spl_widgets-1.7.3/src/spl_widgets/util/
+-rw-r--r--   0 colin      (501) staff       (20)     1169 2023-07-10 17:51:43.000000 spl_widgets-1.7.3/src/spl_widgets/util/color_util.py
+-rw-r--r--   0 colin      (501) staff       (20)     5635 2023-07-26 16:35:15.000000 spl_widgets-1.7.3/src/spl_widgets/util/gui_util.py
+-rw-r--r--   0 colin      (501) staff       (20)     3642 2023-05-26 16:25:13.000000 spl_widgets-1.7.3/src/spl_widgets/util/sqlite_db.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 19:07:05.661533 spl_widgets-1.7.3/src/spl_widgets.egg-info/
+-rw-r--r--   0 colin      (501) staff       (20)      411 2023-07-26 19:07:05.000000 spl_widgets-1.7.3/src/spl_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 colin      (501) staff       (20)      839 2023-07-26 19:07:05.000000 spl_widgets-1.7.3/src/spl_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 colin      (501) staff       (20)        1 2023-07-26 19:07:05.000000 spl_widgets-1.7.3/src/spl_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 colin      (501) staff       (20)      265 2023-07-26 19:07:05.000000 spl_widgets-1.7.3/src/spl_widgets.egg-info/entry_points.txt
+-rw-r--r--   0 colin      (501) staff       (20)       43 2023-07-26 19:07:05.000000 spl_widgets-1.7.3/src/spl_widgets.egg-info/requires.txt
+-rw-r--r--   0 colin      (501) staff       (20)       12 2023-07-26 19:07:05.000000 spl_widgets-1.7.3/src/spl_widgets.egg-info/top_level.txt
```

### Comparing `spl_widgets-1.7.2/LICENSE` & `spl_widgets-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.2/README.md` & `spl_widgets-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.2/setup.py` & `spl_widgets-1.7.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 # with open("README.md", "r", encoding="utf-8") as fh:
 #     long_description = fh.read()
 
 setuptools.setup(
     name="spl_widgets",
-    version="1.7.2",
+    version="1.7.3",
     author="Colin Simon-Fellowes",
     author_email="colin.tsf@gmail.com",
     description="Widgets for the Barnard Speech Perception Laboratory",
     # long_description=long_description,
     # long_description_content_type="text/markdown",
     url="https://github.com/clntsf/spl_widgets",
     classifiers=[
```

### Comparing `spl_widgets-1.7.2/src/spl_widgets/autoscorer/autoscore.py` & `spl_widgets-1.7.3/src/spl_widgets/autoscorer/autoscore.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.2/src/spl_widgets/autoscorer/autoscorer_gui.py` & `spl_widgets-1.7.3/src/spl_widgets/autoscorer/autoscorer_gui.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.2/src/spl_widgets/autoscorer/tokenize_to_ipa.py` & `spl_widgets-1.7.3/src/spl_widgets/autoscorer/tokenize_to_ipa.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 
 # https://en.wikipedia.org/wiki/ARPABET#Symbols
 phonemes = {
   "AA": "ɑ",
   "AE": "æ",
   "AH": "ʌ",
   "AO": "ɔ",
-  "AW": "aʊ",
+  "AW": "ɑʊ",
   "AX": "ə",
   "AXR": "ɚ",
-  "AY": "ai",
+  "AY": "ɑi",
   "EH": "ɛ",
   "ER": "ɝ",
   "EY": "ɛi",
   "IH": "ɪ",
   "IX": "ɨ",
   "IY": "i",
   "OW": "oʊ",
```

### Comparing `spl_widgets-1.7.2/src/spl_widgets/batch_tune.py` & `spl_widgets-1.7.3/src/spl_widgets/batch_tune.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.2/src/spl_widgets/data/cmudict.sqlite` & `spl_widgets-1.7.3/src/spl_widgets/data/cmudict.sqlite`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.2/src/spl_widgets/gorilla_clean.py` & `spl_widgets-1.7.3/src/spl_widgets/gorilla_clean.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.2/src/spl_widgets/jukemake.py` & `spl_widgets-1.7.3/src/spl_widgets/jukemake.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.2/src/spl_widgets/misc_util.py` & `spl_widgets-1.7.3/src/spl_widgets/misc_util.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.2/src/spl_widgets/stk_swx.py` & `spl_widgets-1.7.3/src/spl_widgets/stk_swx.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.2/src/spl_widgets/tune_freq.py` & `spl_widgets-1.7.3/src/spl_widgets/tune_freq.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.2/src/spl_widgets/tuner.py` & `spl_widgets-1.7.3/src/spl_widgets/tuner.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.2/src/spl_widgets/util/color_util.py` & `spl_widgets-1.7.3/src/spl_widgets/util/color_util.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.2/src/spl_widgets/util/gui_util.py` & `spl_widgets-1.7.3/src/spl_widgets/util/gui_util.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.2/src/spl_widgets/util/sqlite_db.py` & `spl_widgets-1.7.3/src/spl_widgets/util/sqlite_db.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.2/src/spl_widgets.egg-info/SOURCES.txt` & `spl_widgets-1.7.3/src/spl_widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

