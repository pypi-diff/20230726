# Comparing `tmp/spl_widgets-1.6.1.tar.gz` & `tmp/spl_widgets-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spl_widgets-1.6.1.tar", last modified: Mon Jul 10 21:05:00 2023, max compression
+gzip compressed data, was "spl_widgets-1.7.1.tar", last modified: Wed Jul 26 16:15:58 2023, max compression
```

## Comparing `spl_widgets-1.6.1.tar` & `spl_widgets-1.7.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-10 21:05:00.441568 spl_widgets-1.6.1/
--rw-r--r--   0 colin      (501) staff       (20)     1073 2021-11-03 16:44:37.000000 spl_widgets-1.6.1/LICENSE
--rw-r--r--   0 colin      (501) staff       (20)      411 2023-07-10 21:05:00.441100 spl_widgets-1.6.1/PKG-INFO
--rw-r--r--   0 colin      (501) staff       (20)     2101 2022-06-26 15:02:40.000000 spl_widgets-1.6.1/README.md
--rw-r--r--   0 colin      (501) staff       (20)      103 2021-11-03 16:36:22.000000 spl_widgets-1.6.1/pyproject.toml
--rw-r--r--   0 colin      (501) staff       (20)       38 2023-07-10 21:05:00.441705 spl_widgets-1.6.1/setup.cfg
--rw-r--r--   0 colin      (501) staff       (20)     1232 2023-07-10 21:04:49.000000 spl_widgets-1.6.1/setup.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-10 21:05:00.396727 spl_widgets-1.6.1/src/
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-10 21:05:00.407590 spl_widgets-1.6.1/src/spl_widgets/
--rw-r--r--   0 colin      (501) staff       (20)      279 2022-06-26 16:32:08.000000 spl_widgets-1.6.1/src/spl_widgets/__init__.py
--rw-r--r--   0 colin      (501) staff       (20)        0 2022-06-26 14:59:05.000000 spl_widgets-1.6.1/src/spl_widgets/__main__.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-10 21:05:00.413266 spl_widgets-1.6.1/src/spl_widgets/autoscorer/
--rw-r--r--   0 colin      (501) staff       (20)    13846 2023-07-10 17:51:43.000000 spl_widgets-1.6.1/src/spl_widgets/autoscorer/autoscore.py
--rw-r--r--   0 colin      (501) staff       (20)    16304 2023-07-10 21:04:34.000000 spl_widgets-1.6.1/src/spl_widgets/autoscorer/autoscorer_gui.py
--rw-r--r--   0 colin      (501) staff       (20)     5387 2023-07-02 19:26:17.000000 spl_widgets-1.6.1/src/spl_widgets/autoscorer/tokenize_to_ipa.py
--rw-r--r--   0 colin      (501) staff       (20)     3722 2023-05-26 16:24:48.000000 spl_widgets-1.6.1/src/spl_widgets/batch_tune.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-10 21:05:00.433890 spl_widgets-1.6.1/src/spl_widgets/data/
--rw-r--r--   0 colin      (501) staff       (20)  9670656 2023-05-26 16:25:12.000000 spl_widgets-1.6.1/src/spl_widgets/data/cmudict.sqlite
--rw-r--r--   0 colin      (501) staff       (20)       73 2023-07-09 17:07:05.000000 spl_widgets-1.6.1/src/spl_widgets/data/help_text.json
--rwxr-xr-x   0 colin      (501) staff       (20)     5378 2022-10-21 13:14:40.000000 spl_widgets-1.6.1/src/spl_widgets/gorilla_clean.py
--rw-r--r--   0 colin      (501) staff       (20)     2483 2022-12-17 21:45:28.000000 spl_widgets-1.6.1/src/spl_widgets/jukemake.py
--rw-r--r--   0 colin      (501) staff       (20)     4166 2023-05-25 22:28:36.000000 spl_widgets-1.6.1/src/spl_widgets/misc_util.py
--rwxr-xr-x   0 colin      (501) staff       (20)     3598 2023-04-14 19:27:21.000000 spl_widgets-1.6.1/src/spl_widgets/stk_swx.py
--rw-r--r--   0 colin      (501) staff       (20)     3614 2023-04-23 14:58:27.000000 spl_widgets-1.6.1/src/spl_widgets/tune_freq.py
--rw-r--r--   0 colin      (501) staff       (20)    17694 2023-05-26 16:20:21.000000 spl_widgets-1.6.1/src/spl_widgets/tuner.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-10 21:05:00.439969 spl_widgets-1.6.1/src/spl_widgets/util/
--rw-r--r--   0 colin      (501) staff       (20)     1169 2023-07-10 17:51:43.000000 spl_widgets-1.6.1/src/spl_widgets/util/color_util.py
--rw-r--r--   0 colin      (501) staff       (20)     3923 2023-05-26 16:25:12.000000 spl_widgets-1.6.1/src/spl_widgets/util/gui_util.py
--rw-r--r--   0 colin      (501) staff       (20)     3642 2023-05-26 16:25:13.000000 spl_widgets-1.6.1/src/spl_widgets/util/sqlite_db.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-10 21:05:00.410950 spl_widgets-1.6.1/src/spl_widgets.egg-info/
--rw-r--r--   0 colin      (501) staff       (20)      411 2023-07-10 21:05:00.000000 spl_widgets-1.6.1/src/spl_widgets.egg-info/PKG-INFO
--rw-r--r--   0 colin      (501) staff       (20)      839 2023-07-10 21:05:00.000000 spl_widgets-1.6.1/src/spl_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 colin      (501) staff       (20)        1 2023-07-10 21:05:00.000000 spl_widgets-1.6.1/src/spl_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 colin      (501) staff       (20)      265 2023-07-10 21:05:00.000000 spl_widgets-1.6.1/src/spl_widgets.egg-info/entry_points.txt
--rw-r--r--   0 colin      (501) staff       (20)       38 2023-07-10 21:05:00.000000 spl_widgets-1.6.1/src/spl_widgets.egg-info/requires.txt
--rw-r--r--   0 colin      (501) staff       (20)       12 2023-07-10 21:05:00.000000 spl_widgets-1.6.1/src/spl_widgets.egg-info/top_level.txt
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 16:15:58.414147 spl_widgets-1.7.1/
+-rw-r--r--   0 colin      (501) staff       (20)     1073 2021-11-03 16:44:37.000000 spl_widgets-1.7.1/LICENSE
+-rw-r--r--   0 colin      (501) staff       (20)      411 2023-07-26 16:15:58.414011 spl_widgets-1.7.1/PKG-INFO
+-rw-r--r--   0 colin      (501) staff       (20)     2101 2022-06-26 15:02:40.000000 spl_widgets-1.7.1/README.md
+-rw-r--r--   0 colin      (501) staff       (20)      103 2021-11-03 16:36:22.000000 spl_widgets-1.7.1/pyproject.toml
+-rw-r--r--   0 colin      (501) staff       (20)       38 2023-07-26 16:15:58.414195 spl_widgets-1.7.1/setup.cfg
+-rw-r--r--   0 colin      (501) staff       (20)     1232 2023-07-26 16:15:49.000000 spl_widgets-1.7.1/setup.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 16:15:58.403554 spl_widgets-1.7.1/src/
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 16:15:58.405708 spl_widgets-1.7.1/src/spl_widgets/
+-rw-r--r--   0 colin      (501) staff       (20)      279 2022-06-26 16:32:08.000000 spl_widgets-1.7.1/src/spl_widgets/__init__.py
+-rw-r--r--   0 colin      (501) staff       (20)        0 2022-06-26 14:59:05.000000 spl_widgets-1.7.1/src/spl_widgets/__main__.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 16:15:58.407046 spl_widgets-1.7.1/src/spl_widgets/autoscorer/
+-rw-r--r--   0 colin      (501) staff       (20)    13846 2023-07-26 16:15:39.000000 spl_widgets-1.7.1/src/spl_widgets/autoscorer/autoscore.py
+-rw-r--r--   0 colin      (501) staff       (20)    18662 2023-07-26 16:15:14.000000 spl_widgets-1.7.1/src/spl_widgets/autoscorer/autoscorer_gui.py
+-rw-r--r--   0 colin      (501) staff       (20)     5387 2023-07-02 19:26:17.000000 spl_widgets-1.7.1/src/spl_widgets/autoscorer/tokenize_to_ipa.py
+-rw-r--r--   0 colin      (501) staff       (20)     3722 2023-05-26 16:24:48.000000 spl_widgets-1.7.1/src/spl_widgets/batch_tune.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 16:15:58.411723 spl_widgets-1.7.1/src/spl_widgets/data/
+-rw-r--r--   0 colin      (501) staff       (20)  9670656 2023-05-26 16:25:12.000000 spl_widgets-1.7.1/src/spl_widgets/data/cmudict.sqlite
+-rw-r--r--   0 colin      (501) staff       (20)       73 2023-07-11 18:30:01.000000 spl_widgets-1.7.1/src/spl_widgets/data/help_text.json
+-rwxr-xr-x   0 colin      (501) staff       (20)     5378 2022-10-21 13:14:40.000000 spl_widgets-1.7.1/src/spl_widgets/gorilla_clean.py
+-rw-r--r--   0 colin      (501) staff       (20)     2483 2022-12-17 21:45:28.000000 spl_widgets-1.7.1/src/spl_widgets/jukemake.py
+-rw-r--r--   0 colin      (501) staff       (20)     4166 2023-05-25 22:28:36.000000 spl_widgets-1.7.1/src/spl_widgets/misc_util.py
+-rwxr-xr-x   0 colin      (501) staff       (20)     3598 2023-04-14 19:27:21.000000 spl_widgets-1.7.1/src/spl_widgets/stk_swx.py
+-rw-r--r--   0 colin      (501) staff       (20)     3614 2023-04-23 14:58:27.000000 spl_widgets-1.7.1/src/spl_widgets/tune_freq.py
+-rw-r--r--   0 colin      (501) staff       (20)    17694 2023-05-26 16:20:21.000000 spl_widgets-1.7.1/src/spl_widgets/tuner.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 16:15:58.413833 spl_widgets-1.7.1/src/spl_widgets/util/
+-rw-r--r--   0 colin      (501) staff       (20)     1169 2023-07-10 17:51:43.000000 spl_widgets-1.7.1/src/spl_widgets/util/color_util.py
+-rw-r--r--   0 colin      (501) staff       (20)     5635 2023-07-26 16:11:56.000000 spl_widgets-1.7.1/src/spl_widgets/util/gui_util.py
+-rw-r--r--   0 colin      (501) staff       (20)     3642 2023-05-26 16:25:13.000000 spl_widgets-1.7.1/src/spl_widgets/util/sqlite_db.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 16:15:58.406595 spl_widgets-1.7.1/src/spl_widgets.egg-info/
+-rw-r--r--   0 colin      (501) staff       (20)      411 2023-07-26 16:15:58.000000 spl_widgets-1.7.1/src/spl_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 colin      (501) staff       (20)      839 2023-07-26 16:15:58.000000 spl_widgets-1.7.1/src/spl_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 colin      (501) staff       (20)        1 2023-07-26 16:15:58.000000 spl_widgets-1.7.1/src/spl_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 colin      (501) staff       (20)      265 2023-07-26 16:15:58.000000 spl_widgets-1.7.1/src/spl_widgets.egg-info/entry_points.txt
+-rw-r--r--   0 colin      (501) staff       (20)       38 2023-07-26 16:15:58.000000 spl_widgets-1.7.1/src/spl_widgets.egg-info/requires.txt
+-rw-r--r--   0 colin      (501) staff       (20)       12 2023-07-26 16:15:58.000000 spl_widgets-1.7.1/src/spl_widgets.egg-info/top_level.txt
```

### Comparing `spl_widgets-1.6.1/LICENSE` & `spl_widgets-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.6.1/README.md` & `spl_widgets-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.6.1/setup.py` & `spl_widgets-1.7.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 # with open("README.md", "r", encoding="utf-8") as fh:
 #     long_description = fh.read()
 
 setuptools.setup(
     name="spl_widgets",
-    version="1.6.1",
+    version="1.7.1",
     author="Colin Simon-Fellowes",
     author_email="colin.tsf@gmail.com",
     description="Widgets for the Barnard Speech Perception Laboratory",
     # long_description=long_description,
     # long_description_content_type="text/markdown",
     url="https://github.com/clntsf/spl_widgets",
     classifiers=[
```

### Comparing `spl_widgets-1.6.1/src/spl_widgets/autoscorer/autoscore.py` & `spl_widgets-1.7.1/src/spl_widgets/autoscorer/autoscore.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.6.1/src/spl_widgets/autoscorer/autoscorer_gui.py` & `spl_widgets-1.7.1/src/spl_widgets/autoscorer/autoscorer_gui.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,26 +3,29 @@
 from tkinterdnd2 import TkinterDnD
 
 from pathlib import Path
 from subprocess import run
 import re
 import pandas as pd
 
-from spl_widgets.util.gui_util import RadioFrame, MarginListBox, HelpLinkLabel
+import pkg_resources
+import json
+
+from spl_widgets.util.gui_util import RadioFrame, MarginListBox, HelpLinkLabel, HelpTextParser, NOTEBOOK_TAB_WIDTH
 from spl_widgets.autoscorer import autoscore
 
 HL = "*"*29
 
 class AutoscorerGUI:
     scoring_mode_radios: RadioFrame
     input_data_listbox: MarginListBox
     ideal_ipa_listbox: MarginListBox
     output_data_listbox: MarginListBox
 
-    def __init__(self, master):
+    def __init__(self, master: tk.Tk):
         self.master = master
 
         self.make_help_window()
         self.hide_help()
     
         self.make_data_input_frame()
         self.make_options_frame()
@@ -168,16 +171,22 @@
         if combine_output:
             self.process_output_combined(input_files, ideal_ipa_path)
         else:
             self.process_output_separate(input_files, ideal_ipa_path)
 
     def make_help_window(self):
         self.help_window = tk.Toplevel(self.master)
+        self.help_window.resizable(False,True)
         self.help_window.title("Autoscorer GUI Help Menu")
-        self.help_app = AutoscorerHelpWindow(self.help_window)
+
+        help_text_fp = pkg_resources.resource_filename("spl_widgets", "data/help_text.json")
+        with open(help_text_fp, "r") as reader:
+            help_text_json = json.load(reader)
+
+        self.help_app = AutoscorerHelpWindow(self.help_window, help_text_json)
 
     def update_scoring_mode_radios(self):
         if self.ideal_ipa_listbox.size() == 1:
             self.scoring_mode_radios.radios[0].configure(state="normal")
         else:
             self.scoring_mode_radios.radios[0].configure(state="disabled")
             self.scoring_mode_radios.variable.set(1)
@@ -390,14 +399,19 @@
         )
 
     def show_help(self):
         try:
             self.help_window.deiconify()
         except tk.TclError:
             self.make_help_window()
+            return self.show_help()
+
+        # set the heights of the scrollbars - done here because the window must be loaded for it to work,
+        # and it isn't time consuming so it's not an issue if it runs each time the window opens
+        self.help_app.set_scroll_heights()
 
     def hide_help(self):
         self.help_window.withdraw()
 
     def open_file(self, listbox: MarginListBox):
         selected = listbox.curselection()
         for idx in selected:
@@ -412,69 +426,96 @@
         nb = self.help_app.help_notebook
         tab_names = [nb.tab(i, option="text") for i in nb.tabs()]
 
         tab_idx = tab_names.index(tab_name)
         nb.select(tab_idx)
 
 class AutoscorerHelpWindow:
-    def __init__(self, master: tk.Toplevel):
+    def __init__(self, master: tk.Toplevel, text: dict):
         self.master = master
+        self.text = text
 
         help_main_frame = tk.Frame(self.master)
         help_main_frame.pack(fill="both", expand=True, pady=10)
 
         self.help_notebook = ttk.Notebook(
-            help_main_frame, width=200, height=200, padding=0
+            help_main_frame, width=NOTEBOOK_TAB_WIDTH+20, height=250, padding=0
         )
         self.help_notebook.pack(side="top", fill="both", expand=True)
 
+        # this is an unbelievably ridiculous hack brought on by the idiocy of MacOS somehow
+        # refusing to work properly with tkinter. When a notebook tab is switched, tkinter
+        # refuses to draw the contents of the tab until the mouse is moved (or, less reliably,
+        # another mouse click occurs). As such, we wait 20ms and simulate a mouse move event
+        # whenever we switch tabs, because we just can't have nice things
+        def force_refresh(evt: tk.Event):
+            sim_event= lambda: self.help_notebook.event_generate("<Motion>", x=100, y=100)
+            self.master.after(20, sim_event)
 
+        self.help_notebook.bind("<<NotebookTabChanged>>", force_refresh)
+
+        # File input help tab
         notebook_tab_FILE_INPUT = tk.Frame(
-            self.help_notebook,
+            help_main_frame,
             highlightbackground="black",
             highlightthickness=1
         )
         notebook_tab_FILE_INPUT.pack(fill="both", expand=True)
-        # TODO: ADD INPUT HELP TEXT HERE
-        
+        self.input_help = HelpTextParser(notebook_tab_FILE_INPUT, text["input-help"])
+        self.input_help.pack(side="left", anchor="nw", fill="both", expand=True)
 
+        # Scoring mode help tab
         notebook_tab_SCORING_MODE = tk.Frame(
-            self.help_notebook,
+            help_main_frame,
             highlightbackground="black",
             highlightthickness=1
         )
         notebook_tab_SCORING_MODE.pack(fill="both", expand=True)
-        # TODO: ADD SCORING MODE HELP TEXT HERE
-
+        self.scoring_help = HelpTextParser(notebook_tab_SCORING_MODE, text["scoring-mode-help"])
+        self.scoring_help.pack(side="top", anchor="nw", fill="both", expand=True)
 
+        # File output help tab
         notebook_tab_FILE_OUTPUT = tk.Frame(
-            self.help_notebook,
+            help_main_frame,
             highlightbackground="black",
             highlightthickness=1
         )
         notebook_tab_FILE_OUTPUT.pack(fill="both", expand=True)
-        # TODO: ADD OUTPUT HELP TEXT HERE
-
+        self.output_help = HelpTextParser(notebook_tab_FILE_OUTPUT, text["output-help"])
+        self.output_help.pack(side="top", anchor="nw", fill="both", expand=True)
+        
+        # Add the tabs to the notebook
         self.help_notebook.add(notebook_tab_FILE_INPUT, text="File Input", sticky="nsew")
         self.help_notebook.add(notebook_tab_SCORING_MODE, text="Scoring Mode Options", sticky="nsew")
         self.help_notebook.add(notebook_tab_FILE_OUTPUT, text="File Output", sticky="nsew")
 
+        # Add the quit button
         help_quitbutton = tk.Button(
             help_main_frame,
             text="Hide this window",
             command=self.master.withdraw
         )
         help_quitbutton.pack(
-            side="bottom", anchor="se", pady=(0,5), padx=5
+            side="bottom", anchor="se", pady=0, padx=5
         )
 
+    # set the scroll region of the tabs in the notebook. Can only be run once the help window is loaded
+    def set_scroll_heights(self):
+        
+        for tab_content in [self.input_help, self.scoring_help, self.output_help]:
+            width = tab_content.content.winfo_width()
+            height = tab_content.content.winfo_height()
+            
+            tab_content.canvas.configure(scrollregion=(0,0,width,height))
+
 # for use in the output side
 
 def main():
     root = TkinterDnD.Tk()
     root.title("Autoscorer GUI")
+    root.resizable(False, False)
 
     app = AutoscorerGUI(root)
     root.mainloop()
 
 if __name__ == "__main__":
     main()
```

### Comparing `spl_widgets-1.6.1/src/spl_widgets/autoscorer/tokenize_to_ipa.py` & `spl_widgets-1.7.1/src/spl_widgets/autoscorer/tokenize_to_ipa.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.6.1/src/spl_widgets/batch_tune.py` & `spl_widgets-1.7.1/src/spl_widgets/batch_tune.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.6.1/src/spl_widgets/data/cmudict.sqlite` & `spl_widgets-1.7.1/src/spl_widgets/data/cmudict.sqlite`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.6.1/src/spl_widgets/gorilla_clean.py` & `spl_widgets-1.7.1/src/spl_widgets/gorilla_clean.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.6.1/src/spl_widgets/jukemake.py` & `spl_widgets-1.7.1/src/spl_widgets/jukemake.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.6.1/src/spl_widgets/misc_util.py` & `spl_widgets-1.7.1/src/spl_widgets/misc_util.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.6.1/src/spl_widgets/stk_swx.py` & `spl_widgets-1.7.1/src/spl_widgets/stk_swx.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.6.1/src/spl_widgets/tune_freq.py` & `spl_widgets-1.7.1/src/spl_widgets/tune_freq.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.6.1/src/spl_widgets/tuner.py` & `spl_widgets-1.7.1/src/spl_widgets/tuner.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.6.1/src/spl_widgets/util/color_util.py` & `spl_widgets-1.7.1/src/spl_widgets/util/color_util.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.6.1/src/spl_widgets/util/gui_util.py` & `spl_widgets-1.7.1/src/spl_widgets/util/gui_util.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import tkinter as tk
+from tkinter import ttk
 from typing import Callable
 
 class RadioFrame(tk.Frame):
 
     def __init__(
         self,
         master: tk.Frame,
         options: "list[str]",
         label_text: str,
         onchange: Callable = None,
         orientation: str = "v",
         **kwargs
-        ) -> tk.Frame:
-        tk.Frame.__init__(self, master, **kwargs)
+        ):
+        super().__init__(master, **kwargs)
 
         self.master = master
         self.variable = tk.IntVar()
         self.onchange = lambda: onchange(self.variable) if onchange else None
 
         self.packsides = ["top", "bottom"] if orientation == "v" else ["left", "right"]
         self.anchorside = "w" if orientation == "v" else "n"
@@ -106,8 +107,57 @@
         self.pack( side="left", padx = 0 )
 
         helplink = tk.Label(self.enclosing_frame, text="(?)", fg="blue", cursor="hand2")
         helplink.bind("<Button-1>", lambda e: onclick(tab_name))
         helplink.pack(side="left", padx=0)
 
     def pack_frame(self, **kwargs):
-        self.enclosing_frame.pack(**kwargs)
+        self.enclosing_frame.pack(**kwargs)
+
+FONT_TITLE = ("TkDefaultFont", 14, "bold")
+NOTEBOOK_TAB_WIDTH = 350
+NOTEBOOK_TAB_MARG=30
+
+class HelpTextParser(tk.Frame):
+    content: tk.Frame
+
+    def __init__(self, master, items: dict[str,str], **kwargs):
+        super().__init__( master, **kwargs )
+
+        self.canvas=tk.Canvas(self,width=NOTEBOOK_TAB_WIDTH, scrollregion=(0,0,300,500))
+        
+        scrollbar=tk.Scrollbar(self, command=self.canvas.yview)
+        scrollbar.pack(side="right",fill="y", expand=True)
+        scrollbar.config(command=self.canvas.yview)
+
+        self.content = tk.Frame(self.canvas)
+        self.canvas.create_window((0,0), window=self.content, anchor="nw")
+        
+        self.canvas.config(yscrollcommand=scrollbar.set)
+        self.canvas.pack(side="left",expand=True,fill='both')
+
+        self.parse_text(items)
+
+    def parse_text(self, items: dict[str, str]) -> None:
+
+        for (title, content) in items.items():
+            heading_frame = tk.Frame(self.content, padx=10)
+            heading_frame.pack(side="top", anchor="w")
+
+            heading_title = tk.Label(
+                heading_frame, text = title, font = FONT_TITLE,
+                wraplength=NOTEBOOK_TAB_WIDTH-NOTEBOOK_TAB_MARG,
+                justify="left"
+            )
+            heading_title.pack(side="top", anchor="w", pady=3)
+
+            heading_text = tk.Label(
+                heading_frame, text = content,
+                wraplength=NOTEBOOK_TAB_WIDTH-NOTEBOOK_TAB_MARG,
+                justify="left"
+            )
+            heading_text.pack(side="top", anchor="w", padx=5, pady=5)
+
+            sep = ttk.Separator(heading_frame, orient="horizontal")
+            sep.pack(fill="x", side="top", pady=5)
+
+
```

### Comparing `spl_widgets-1.6.1/src/spl_widgets/util/sqlite_db.py` & `spl_widgets-1.7.1/src/spl_widgets/util/sqlite_db.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.6.1/src/spl_widgets.egg-info/SOURCES.txt` & `spl_widgets-1.7.1/src/spl_widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

