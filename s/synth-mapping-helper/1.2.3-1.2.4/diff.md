# Comparing `tmp/synth_mapping_helper-1.2.3.tar.gz` & `tmp/synth_mapping_helper-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synth_mapping_helper-1.2.3.tar", last modified: Sun Jun 11 15:46:05 2023, max compression
+gzip compressed data, was "synth_mapping_helper-1.2.4.tar", last modified: Wed Jul 26 17:48:12 2023, max compression
```

## Comparing `synth_mapping_helper-1.2.3.tar` & `synth_mapping_helper-1.2.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:46:05.556155 synth_mapping_helper-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-11 15:45:55.000000 synth_mapping_helper-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-11 15:45:55.000000 synth_mapping_helper-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-11 15:46:05.556155 synth_mapping_helper-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-11 15:45:55.000000 synth_mapping_helper-1.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-11 15:45:55.000000 synth_mapping_helper-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-11 15:46:05.556155 synth_mapping_helper-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-11 15:45:55.000000 synth_mapping_helper-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:46:05.552155 synth_mapping_helper-1.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:46:05.552155 synth_mapping_helper-1.2.3/src/synth_mapping_helper/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-11 15:45:55.000000 synth_mapping_helper-1.2.3/src/synth_mapping_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28834 2023-06-11 15:45:55.000000 synth_mapping_helper-1.2.3/src/synth_mapping_helper/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    28072 2023-06-11 15:45:55.000000 synth_mapping_helper-1.2.3/src/synth_mapping_helper/companion.py
--rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-06-11 15:45:55.000000 synth_mapping_helper-1.2.3/src/synth_mapping_helper/finalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-06-11 15:45:55.000000 synth_mapping_helper-1.2.3/src/synth_mapping_helper/movement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-11 15:45:55.000000 synth_mapping_helper-1.2.3/src/synth_mapping_helper/pattern_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-06-11 15:45:55.000000 synth_mapping_helper-1.2.3/src/synth_mapping_helper/rails.py
--rw-r--r--   0 runner    (1001) docker     (123)    16429 2023-06-11 15:45:55.000000 synth_mapping_helper-1.2.3/src/synth_mapping_helper/synth_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-06-11 15:45:55.000000 synth_mapping_helper-1.2.3/src/synth_mapping_helper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:46:05.552155 synth_mapping_helper-1.2.3/src/synth_mapping_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-11 15:46:05.000000 synth_mapping_helper-1.2.3/src/synth_mapping_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-11 15:46:05.000000 synth_mapping_helper-1.2.3/src/synth_mapping_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 15:46:05.000000 synth_mapping_helper-1.2.3/src/synth_mapping_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-11 15:46:05.000000 synth_mapping_helper-1.2.3/src/synth_mapping_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-11 15:46:05.000000 synth_mapping_helper-1.2.3/src/synth_mapping_helper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:46:05.556155 synth_mapping_helper-1.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-11 15:45:55.000000 synth_mapping_helper-1.2.3/tests/test_synth_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:48:12.177260 synth_mapping_helper-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-26 17:48:00.000000 synth_mapping_helper-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 17:48:00.000000 synth_mapping_helper-1.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-26 17:48:12.177260 synth_mapping_helper-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-26 17:48:00.000000 synth_mapping_helper-1.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-26 17:48:00.000000 synth_mapping_helper-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-26 17:48:12.181260 synth_mapping_helper-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-26 17:48:00.000000 synth_mapping_helper-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:48:12.173260 synth_mapping_helper-1.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:48:12.177260 synth_mapping_helper-1.2.4/src/synth_mapping_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-26 17:48:00.000000 synth_mapping_helper-1.2.4/src/synth_mapping_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28834 2023-07-26 17:48:00.000000 synth_mapping_helper-1.2.4/src/synth_mapping_helper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28137 2023-07-26 17:48:00.000000 synth_mapping_helper-1.2.4/src/synth_mapping_helper/companion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-07-26 17:48:00.000000 synth_mapping_helper-1.2.4/src/synth_mapping_helper/finalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-07-26 17:48:00.000000 synth_mapping_helper-1.2.4/src/synth_mapping_helper/movement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-26 17:48:00.000000 synth_mapping_helper-1.2.4/src/synth_mapping_helper/pattern_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-07-26 17:48:00.000000 synth_mapping_helper-1.2.4/src/synth_mapping_helper/rails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16878 2023-07-26 17:48:00.000000 synth_mapping_helper-1.2.4/src/synth_mapping_helper/synth_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-26 17:48:00.000000 synth_mapping_helper-1.2.4/src/synth_mapping_helper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:48:12.177260 synth_mapping_helper-1.2.4/src/synth_mapping_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-26 17:48:12.000000 synth_mapping_helper-1.2.4/src/synth_mapping_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-26 17:48:12.000000 synth_mapping_helper-1.2.4/src/synth_mapping_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 17:48:12.000000 synth_mapping_helper-1.2.4/src/synth_mapping_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-26 17:48:12.000000 synth_mapping_helper-1.2.4/src/synth_mapping_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-26 17:48:12.000000 synth_mapping_helper-1.2.4/src/synth_mapping_helper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:48:12.177260 synth_mapping_helper-1.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-26 17:48:00.000000 synth_mapping_helper-1.2.4/tests/test_synth_format.py
```

### Comparing `synth_mapping_helper-1.2.3/LICENSE` & `synth_mapping_helper-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.3/PKG-INFO` & `synth_mapping_helper-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synth_mapping_helper
-Version: 1.2.3
+Version: 1.2.4
 Summary: Toolbox for manipulating the JSON-Format used by Synth Riders Beatmap Editor in the clipboard
 Home-page: https://github.com/adosikas/synth_mapping_helper
 Author: adosikas
 Author-email: 
 Project-URL: Documentation, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Bug Reports, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Source Code, https://github.com/adosikas/synth_mapping_helper
```

### Comparing `synth_mapping_helper-1.2.3/README.md` & `synth_mapping_helper-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.3/setup.py` & `synth_mapping_helper-1.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.3/src/synth_mapping_helper/cli.py` & `synth_mapping_helper-1.2.4/src/synth_mapping_helper/cli.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.3/src/synth_mapping_helper/companion.py` & `synth_mapping_helper-1.2.4/src/synth_mapping_helper/companion.py`

 * *Files 1% similar despite different names*

```diff
@@ -412,14 +412,16 @@
     active_platform = 0
 
     difficulties: list[tuple["difficulty_name", "prepared_data"]] = None
     def replace_prepared_data():
         nonlocal difficulties
         logging.info("Preparing data")
         difficulties = [(d, prepare_data(data.difficulties[d], options)) for d in synth_format.DIFFICULTIES if d in data.difficulties]
+        if not difficulties:
+            abort("No notes found")
         logging.info("Preparing complete")
 
     replace_prepared_data()
 
     def redraw():
         tab_name, tab_func = TABS[active_tab]
         diff_name, prepared_data = difficulties[active_difficulty]
```

### Comparing `synth_mapping_helper-1.2.3/src/synth_mapping_helper/finalize.py` & `synth_mapping_helper-1.2.4/src/synth_mapping_helper/finalize.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.3/src/synth_mapping_helper/movement.py` & `synth_mapping_helper-1.2.4/src/synth_mapping_helper/movement.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.3/src/synth_mapping_helper/pattern_generation.py` & `synth_mapping_helper-1.2.4/src/synth_mapping_helper/pattern_generation.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.3/src/synth_mapping_helper/rails.py` & `synth_mapping_helper-1.2.4/src/synth_mapping_helper/rails.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.3/src/synth_mapping_helper/synth_format.py` & `synth_mapping_helper-1.2.4/src/synth_mapping_helper/synth_format.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #/usr/bin/env python3
 from io import BytesIO
 import dataclasses
 import json
 from pathlib import Path
+import time
 from typing import Union
 from zipfile import ZipFile
 
 import numpy as np
 import pyperclip
 
 # For simplicity, we exclusively use grid coordinates (x, y) and use measures for time (z)
@@ -53,17 +54,21 @@
 DIFFICULTIES = ("Easy", "Normal", "Hard", "Expert", "Master", "Custom")
 META_KEYS = ("Name", "Author", "Beatmapper", "CustomDifficultyName", "BPM")
 
 BETA_WARNING_SHOWN = False
 
 
 def beta_warning() -> None:
+    global BETA_WARNING_SHOWN
     if not BETA_WARNING_SHOWN:
-        print("This was tested with the beta version of the editor only. You may want to switch to it.")
+        print("\n\n ⚠️  W A R N I N G ⚠️")
+        print("\tThis was tested with the beta version of the editor only.")
+        print("\tYou may want to switch to it if you encounter bugs or weird behavior.\n\n")
         BETA_WARNING_SHOWN = True
+        time.sleep(0.5)
 
 def round_time_to_fractions(time: float) -> float:
     # 192 is the lowest common multiple of 64 and 48, so this covers all steps the editor supports and more
     # effectively this is 3 intermediate steps for each 1/64 step, or 4 for each 1/48 step
     # those intermediate steps are also possible in the editor by abusing snap or copy-paste and switching
     # between 1/64 and 1/48 step.
     # But the editor does no rounding at all, leading to float erros creeping up. 
@@ -291,16 +296,15 @@
         dest_list = "slides"
     else:
         dest_list = WALL_LOOKUP[wall_type] + "s"
         del wall_dict["slideType"]
     return dest_list, wall_dict
 
 # full json
-def import_clipboard(use_original: bool = False) -> ClipboardDataContainer:
-    original_json = pyperclip.paste()
+def import_clipboard_json(original_json: str, use_original: bool = False) -> ClipboardDataContainer:
     clipboard = json.loads(original_json)
     if "original_json" in clipboard:
         original_json = clipboard["original_json"]
     if use_original:
         clipboard = json.loads(original_json)
     bpm = clipboard["BPM"]
     startMeasure = clipboard["startMeasure"]
@@ -323,15 +327,18 @@
             continue  # these are only in the beta editor
         for wall_dict in clipboard[wall_type + "s"]:
             wall = wall_from_synth(bpm, startMeasure, wall_dict, WALL_TYPES[wall_type][0])
             walls[wall[0, 2]] = wall
 
     return ClipboardDataContainer(bpm, *notes, walls, original_json)
 
-def export_clipboard(data: DataContainer, realign_start: bool = True):
+def import_clipboard(use_original: bool = False) -> ClipboardDataContainer:
+    return import_clipboard_json(pyperclip.paste(), use_original)
+
+def export_clipboard_json(data: DataContainer, realign_start: bool = True) -> str:
     clipboard = {
         "BPM": data.bpm,
         "startMeasure": 0,
         "startTime": 0,
         "lenght": 0,
         "notes": {},
         "effects": [],
@@ -370,14 +377,16 @@
         # position of selection start in ms
         clipboard["startTime"] = first * ms_per_min / data.bpm
         # length of the selection in milliseconds
         # and yes, the editor has a typo, so we need to missspell it too
         clipboard["lenght"] = last * ms_per_min / data.bpm
     # always update length
     clipboard["lenght"] = (last - first) * ms_per_min / data.bpm
+    return json.dumps(clipboard)
 
-    pyperclip.copy(json.dumps(clipboard))
+def export_clipboard(data: DataContainer, realign_start: bool = True):
+    pyperclip.copy(export_clipboard_json(data, realign_start))
 
 def import_file(file_path: Path) -> SynthFile:
     out = SynthFile(file_path, {}, {}, {})
     out.reload()
     return out
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `synth_mapping_helper-1.2.3/src/synth_mapping_helper/utils.py` & `synth_mapping_helper-1.2.4/src/synth_mapping_helper/utils.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.3/src/synth_mapping_helper.egg-info/PKG-INFO` & `synth_mapping_helper-1.2.4/src/synth_mapping_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synth-mapping-helper
-Version: 1.2.3
+Version: 1.2.4
 Summary: Toolbox for manipulating the JSON-Format used by Synth Riders Beatmap Editor in the clipboard
 Home-page: https://github.com/adosikas/synth_mapping_helper
 Author: adosikas
 Author-email: 
 Project-URL: Documentation, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Bug Reports, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Source Code, https://github.com/adosikas/synth_mapping_helper
```

### Comparing `synth_mapping_helper-1.2.3/src/synth_mapping_helper.egg-info/SOURCES.txt` & `synth_mapping_helper-1.2.4/src/synth_mapping_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

