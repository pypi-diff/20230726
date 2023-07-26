# Comparing `tmp/spl_widgets-1.7.1.tar.gz` & `tmp/spl_widgets-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spl_widgets-1.7.1.tar", last modified: Wed Jul 26 16:15:58 2023, max compression
+gzip compressed data, was "spl_widgets-1.7.2.tar", last modified: Wed Jul 26 19:01:12 2023, max compression
```

## Comparing `spl_widgets-1.7.1.tar` & `spl_widgets-1.7.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 16:15:58.414147 spl_widgets-1.7.1/
--rw-r--r--   0 colin      (501) staff       (20)     1073 2021-11-03 16:44:37.000000 spl_widgets-1.7.1/LICENSE
--rw-r--r--   0 colin      (501) staff       (20)      411 2023-07-26 16:15:58.414011 spl_widgets-1.7.1/PKG-INFO
--rw-r--r--   0 colin      (501) staff       (20)     2101 2022-06-26 15:02:40.000000 spl_widgets-1.7.1/README.md
--rw-r--r--   0 colin      (501) staff       (20)      103 2021-11-03 16:36:22.000000 spl_widgets-1.7.1/pyproject.toml
--rw-r--r--   0 colin      (501) staff       (20)       38 2023-07-26 16:15:58.414195 spl_widgets-1.7.1/setup.cfg
--rw-r--r--   0 colin      (501) staff       (20)     1232 2023-07-26 16:15:49.000000 spl_widgets-1.7.1/setup.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 16:15:58.403554 spl_widgets-1.7.1/src/
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 16:15:58.405708 spl_widgets-1.7.1/src/spl_widgets/
--rw-r--r--   0 colin      (501) staff       (20)      279 2022-06-26 16:32:08.000000 spl_widgets-1.7.1/src/spl_widgets/__init__.py
--rw-r--r--   0 colin      (501) staff       (20)        0 2022-06-26 14:59:05.000000 spl_widgets-1.7.1/src/spl_widgets/__main__.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 16:15:58.407046 spl_widgets-1.7.1/src/spl_widgets/autoscorer/
--rw-r--r--   0 colin      (501) staff       (20)    13846 2023-07-26 16:15:39.000000 spl_widgets-1.7.1/src/spl_widgets/autoscorer/autoscore.py
--rw-r--r--   0 colin      (501) staff       (20)    18662 2023-07-26 16:15:14.000000 spl_widgets-1.7.1/src/spl_widgets/autoscorer/autoscorer_gui.py
--rw-r--r--   0 colin      (501) staff       (20)     5387 2023-07-02 19:26:17.000000 spl_widgets-1.7.1/src/spl_widgets/autoscorer/tokenize_to_ipa.py
--rw-r--r--   0 colin      (501) staff       (20)     3722 2023-05-26 16:24:48.000000 spl_widgets-1.7.1/src/spl_widgets/batch_tune.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 16:15:58.411723 spl_widgets-1.7.1/src/spl_widgets/data/
--rw-r--r--   0 colin      (501) staff       (20)  9670656 2023-05-26 16:25:12.000000 spl_widgets-1.7.1/src/spl_widgets/data/cmudict.sqlite
--rw-r--r--   0 colin      (501) staff       (20)       73 2023-07-11 18:30:01.000000 spl_widgets-1.7.1/src/spl_widgets/data/help_text.json
--rwxr-xr-x   0 colin      (501) staff       (20)     5378 2022-10-21 13:14:40.000000 spl_widgets-1.7.1/src/spl_widgets/gorilla_clean.py
--rw-r--r--   0 colin      (501) staff       (20)     2483 2022-12-17 21:45:28.000000 spl_widgets-1.7.1/src/spl_widgets/jukemake.py
--rw-r--r--   0 colin      (501) staff       (20)     4166 2023-05-25 22:28:36.000000 spl_widgets-1.7.1/src/spl_widgets/misc_util.py
--rwxr-xr-x   0 colin      (501) staff       (20)     3598 2023-04-14 19:27:21.000000 spl_widgets-1.7.1/src/spl_widgets/stk_swx.py
--rw-r--r--   0 colin      (501) staff       (20)     3614 2023-04-23 14:58:27.000000 spl_widgets-1.7.1/src/spl_widgets/tune_freq.py
--rw-r--r--   0 colin      (501) staff       (20)    17694 2023-05-26 16:20:21.000000 spl_widgets-1.7.1/src/spl_widgets/tuner.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 16:15:58.413833 spl_widgets-1.7.1/src/spl_widgets/util/
--rw-r--r--   0 colin      (501) staff       (20)     1169 2023-07-10 17:51:43.000000 spl_widgets-1.7.1/src/spl_widgets/util/color_util.py
--rw-r--r--   0 colin      (501) staff       (20)     5635 2023-07-26 16:11:56.000000 spl_widgets-1.7.1/src/spl_widgets/util/gui_util.py
--rw-r--r--   0 colin      (501) staff       (20)     3642 2023-05-26 16:25:13.000000 spl_widgets-1.7.1/src/spl_widgets/util/sqlite_db.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 16:15:58.406595 spl_widgets-1.7.1/src/spl_widgets.egg-info/
--rw-r--r--   0 colin      (501) staff       (20)      411 2023-07-26 16:15:58.000000 spl_widgets-1.7.1/src/spl_widgets.egg-info/PKG-INFO
--rw-r--r--   0 colin      (501) staff       (20)      839 2023-07-26 16:15:58.000000 spl_widgets-1.7.1/src/spl_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 colin      (501) staff       (20)        1 2023-07-26 16:15:58.000000 spl_widgets-1.7.1/src/spl_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 colin      (501) staff       (20)      265 2023-07-26 16:15:58.000000 spl_widgets-1.7.1/src/spl_widgets.egg-info/entry_points.txt
--rw-r--r--   0 colin      (501) staff       (20)       38 2023-07-26 16:15:58.000000 spl_widgets-1.7.1/src/spl_widgets.egg-info/requires.txt
--rw-r--r--   0 colin      (501) staff       (20)       12 2023-07-26 16:15:58.000000 spl_widgets-1.7.1/src/spl_widgets.egg-info/top_level.txt
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 19:01:12.722581 spl_widgets-1.7.2/
+-rw-r--r--   0 colin      (501) staff       (20)     1073 2021-11-03 16:44:37.000000 spl_widgets-1.7.2/LICENSE
+-rw-r--r--   0 colin      (501) staff       (20)      411 2023-07-26 19:01:12.722450 spl_widgets-1.7.2/PKG-INFO
+-rw-r--r--   0 colin      (501) staff       (20)     2101 2022-06-26 15:02:40.000000 spl_widgets-1.7.2/README.md
+-rw-r--r--   0 colin      (501) staff       (20)      103 2021-11-03 16:36:22.000000 spl_widgets-1.7.2/pyproject.toml
+-rw-r--r--   0 colin      (501) staff       (20)       38 2023-07-26 19:01:12.722623 spl_widgets-1.7.2/setup.cfg
+-rw-r--r--   0 colin      (501) staff       (20)     1240 2023-07-26 19:01:05.000000 spl_widgets-1.7.2/setup.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 19:01:12.709608 spl_widgets-1.7.2/src/
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 19:01:12.712125 spl_widgets-1.7.2/src/spl_widgets/
+-rw-r--r--   0 colin      (501) staff       (20)      279 2022-06-26 16:32:08.000000 spl_widgets-1.7.2/src/spl_widgets/__init__.py
+-rw-r--r--   0 colin      (501) staff       (20)        0 2022-06-26 14:59:05.000000 spl_widgets-1.7.2/src/spl_widgets/__main__.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 19:01:12.713526 spl_widgets-1.7.2/src/spl_widgets/autoscorer/
+-rw-r--r--   0 colin      (501) staff       (20)    14016 2023-07-26 18:59:47.000000 spl_widgets-1.7.2/src/spl_widgets/autoscorer/autoscore.py
+-rw-r--r--   0 colin      (501) staff       (20)    18685 2023-07-26 19:00:37.000000 spl_widgets-1.7.2/src/spl_widgets/autoscorer/autoscorer_gui.py
+-rw-r--r--   0 colin      (501) staff       (20)     5387 2023-07-02 19:26:17.000000 spl_widgets-1.7.2/src/spl_widgets/autoscorer/tokenize_to_ipa.py
+-rw-r--r--   0 colin      (501) staff       (20)     3722 2023-05-26 16:24:48.000000 spl_widgets-1.7.2/src/spl_widgets/batch_tune.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 19:01:12.720431 spl_widgets-1.7.2/src/spl_widgets/data/
+-rw-r--r--   0 colin      (501) staff       (20)  9670656 2023-05-26 16:25:12.000000 spl_widgets-1.7.2/src/spl_widgets/data/cmudict.sqlite
+-rw-r--r--   0 colin      (501) staff       (20)       73 2023-07-26 16:35:15.000000 spl_widgets-1.7.2/src/spl_widgets/data/help_text.json
+-rwxr-xr-x   0 colin      (501) staff       (20)     5378 2022-10-21 13:14:40.000000 spl_widgets-1.7.2/src/spl_widgets/gorilla_clean.py
+-rw-r--r--   0 colin      (501) staff       (20)     2483 2022-12-17 21:45:28.000000 spl_widgets-1.7.2/src/spl_widgets/jukemake.py
+-rw-r--r--   0 colin      (501) staff       (20)     4166 2023-05-25 22:28:36.000000 spl_widgets-1.7.2/src/spl_widgets/misc_util.py
+-rwxr-xr-x   0 colin      (501) staff       (20)     3598 2023-04-14 19:27:21.000000 spl_widgets-1.7.2/src/spl_widgets/stk_swx.py
+-rw-r--r--   0 colin      (501) staff       (20)     3614 2023-04-23 14:58:27.000000 spl_widgets-1.7.2/src/spl_widgets/tune_freq.py
+-rw-r--r--   0 colin      (501) staff       (20)    17694 2023-05-26 16:20:21.000000 spl_widgets-1.7.2/src/spl_widgets/tuner.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 19:01:12.722242 spl_widgets-1.7.2/src/spl_widgets/util/
+-rw-r--r--   0 colin      (501) staff       (20)     1169 2023-07-10 17:51:43.000000 spl_widgets-1.7.2/src/spl_widgets/util/color_util.py
+-rw-r--r--   0 colin      (501) staff       (20)     5635 2023-07-26 16:35:15.000000 spl_widgets-1.7.2/src/spl_widgets/util/gui_util.py
+-rw-r--r--   0 colin      (501) staff       (20)     3642 2023-05-26 16:25:13.000000 spl_widgets-1.7.2/src/spl_widgets/util/sqlite_db.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 19:01:12.713022 spl_widgets-1.7.2/src/spl_widgets.egg-info/
+-rw-r--r--   0 colin      (501) staff       (20)      411 2023-07-26 19:01:12.000000 spl_widgets-1.7.2/src/spl_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 colin      (501) staff       (20)      839 2023-07-26 19:01:12.000000 spl_widgets-1.7.2/src/spl_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 colin      (501) staff       (20)        1 2023-07-26 19:01:12.000000 spl_widgets-1.7.2/src/spl_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 colin      (501) staff       (20)      265 2023-07-26 19:01:12.000000 spl_widgets-1.7.2/src/spl_widgets.egg-info/entry_points.txt
+-rw-r--r--   0 colin      (501) staff       (20)       43 2023-07-26 19:01:12.000000 spl_widgets-1.7.2/src/spl_widgets.egg-info/requires.txt
+-rw-r--r--   0 colin      (501) staff       (20)       12 2023-07-26 19:01:12.000000 spl_widgets-1.7.2/src/spl_widgets.egg-info/top_level.txt
```

### Comparing `spl_widgets-1.7.1/LICENSE` & `spl_widgets-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.1/README.md` & `spl_widgets-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.1/setup.py` & `spl_widgets-1.7.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import setuptools
 
 # with open("README.md", "r", encoding="utf-8") as fh:
 #     long_description = fh.read()
 
 setuptools.setup(
     name="spl_widgets",
-    version="1.7.1",
+    version="1.7.2",
     author="Colin Simon-Fellowes",
     author_email="colin.tsf@gmail.com",
     description="Widgets for the Barnard Speech Perception Laboratory",
     # long_description=long_description,
     # long_description_content_type="text/markdown",
     url="https://github.com/clntsf/spl_widgets",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: MacOS",
     ],
     package_dir={"": "src"},
     packages=["spl_widgets", "spl_widgets.autoscorer", "spl_widgets.util"],
-    install_requires=['pandas', 'tkinterdnd2-universal', 'openpyxl'],
+    install_requires=['pandas', 'tkinterdnd2-universal', 'openpyxl', 'lxml'],
     python_requires=">=3.8",
     entry_points='''
         [console_scripts]
         gorilla_clean=spl_widgets.gorilla_clean:main
         tuner=spl_widgets.tuner:main
         stk_swx=spl_widgets.stk_swx:main
         batch_tune=spl_widgets.batch_tune:main
```

### Comparing `spl_widgets-1.7.1/src/spl_widgets/autoscorer/autoscore.py` & `spl_widgets-1.7.2/src/spl_widgets/autoscorer/autoscore.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,19 @@
             # get the potential jump-ahead index of the character in the sentence IPA
             new_sentence_ipa_idx = sentence_ipa.index(token)
 
             # make a token we can append to _prev_scored if we decide to omit these characters
             tokens_between = "".join(                                    # get the omitted tokens
                 sentence_ipa[sentence_ipa_idx:new_sentence_ipa_idx]
             )
-            omitted_idx = max(n[1] for n in _prev_scored)+1                         # get the index of the first omitted char in this group
+
+            # get the index of the first omitted char in this group
+            omitted_idx = 0                 # prevent the program breaking if the omitted character is the very first of the transcription
+            if len(_prev_scored) > 0:
+                omitted_idx = max(n[1] for n in _prev_scored)+1
             omitted_chars = [(tokens_between.strip(), omitted_idx, None)]            # create the token
 
             return max(
                 # take this char as the next valid one and jump forward to it in the sentence IPA
                 score_transcription(
                     sentence_ipa[new_sentence_ipa_idx+1:],
                     transcription_ipa[i+1:],
```

### Comparing `spl_widgets-1.7.1/src/spl_widgets/autoscorer/autoscorer_gui.py` & `spl_widgets-1.7.2/src/spl_widgets/autoscorer/autoscorer_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,15 @@
         )
 
         # utility functions for the drag-and-drop boxes
         def add_subject_data_file(listbox: tk.Listbox, data: dict, e) -> None:
             
             FILENAME_RE = r"({.+?}|[\S]+)"
             filepaths = re.findall(FILENAME_RE, e.data)
-            filepaths = [Path(re.sub(r"[{}]", "", fp)) for fp in filepaths]
+            filepaths = [Path(re.sub(r"[\{\}]", "", fp)) for fp in filepaths]
 
             def try_add_file(f: Path):
                 if f.suffix != ".xlsx":
                     print(f"[WARNING]: Only files of type .xlsx allowed, received type '{f.suffix}'")
                     return
     
                 name = f.name
@@ -233,15 +233,15 @@
             item_name = listbox.get(delete_item)
             if item_name in data:
                 data.pop(item_name)
 
             listbox.delete(delete_item)
 
         def add_ideal_ipa_file(listbox: tk.Listbox, data: dict, e) -> None:
-            f = Path(e.data)
+            f = Path(re.sub(r"[{}]", "", e.data))
             if f.suffix != ".xlsx":
                 print(f"[WARNING]: Only files of type .xlsx allowed, received type '{f.suffix}'")
                 return
     
             name = f.name
             remove_ideal_ipa_file(listbox, data)
             data[name] = f
```

### Comparing `spl_widgets-1.7.1/src/spl_widgets/autoscorer/tokenize_to_ipa.py` & `spl_widgets-1.7.2/src/spl_widgets/autoscorer/tokenize_to_ipa.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.1/src/spl_widgets/batch_tune.py` & `spl_widgets-1.7.2/src/spl_widgets/batch_tune.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.1/src/spl_widgets/data/cmudict.sqlite` & `spl_widgets-1.7.2/src/spl_widgets/data/cmudict.sqlite`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.1/src/spl_widgets/gorilla_clean.py` & `spl_widgets-1.7.2/src/spl_widgets/gorilla_clean.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.1/src/spl_widgets/jukemake.py` & `spl_widgets-1.7.2/src/spl_widgets/jukemake.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.1/src/spl_widgets/misc_util.py` & `spl_widgets-1.7.2/src/spl_widgets/misc_util.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.1/src/spl_widgets/stk_swx.py` & `spl_widgets-1.7.2/src/spl_widgets/stk_swx.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.1/src/spl_widgets/tune_freq.py` & `spl_widgets-1.7.2/src/spl_widgets/tune_freq.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.1/src/spl_widgets/tuner.py` & `spl_widgets-1.7.2/src/spl_widgets/tuner.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.1/src/spl_widgets/util/color_util.py` & `spl_widgets-1.7.2/src/spl_widgets/util/color_util.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.1/src/spl_widgets/util/gui_util.py` & `spl_widgets-1.7.2/src/spl_widgets/util/gui_util.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.1/src/spl_widgets/util/sqlite_db.py` & `spl_widgets-1.7.2/src/spl_widgets/util/sqlite_db.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.1/src/spl_widgets.egg-info/SOURCES.txt` & `spl_widgets-1.7.2/src/spl_widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

