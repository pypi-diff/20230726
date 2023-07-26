# Comparing `tmp/mentat-ai-0.1.1.tar.gz` & `tmp/mentat-ai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentat-ai-0.1.1.tar", last modified: Tue Jul 25 18:56:19 2023, max compression
+gzip compressed data, was "mentat-ai-0.1.2.tar", last modified: Wed Jul 26 04:00:56 2023, max compression
```

## Comparing `mentat-ai-0.1.1.tar` & `mentat-ai-0.1.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-25 18:56:19.067427 mentat-ai-0.1.1/
--rw-r--r--   0 biobootloader   (501) staff       (20)    11357 2023-07-08 00:24:17.000000 mentat-ai-0.1.1/LICENSE
--rw-r--r--   0 biobootloader   (501) staff       (20)       75 2023-07-25 18:56:19.067309 mentat-ai-0.1.1/PKG-INFO
--rw-r--r--   0 biobootloader   (501) staff       (20)     2332 2023-07-25 13:33:37.000000 mentat-ai-0.1.1/README.md
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-25 18:56:19.064490 mentat-ai-0.1.1/mentat/
--rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-07-12 23:06:24.000000 mentat-ai-0.1.1/mentat/__init__.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      166 2023-07-21 00:32:22.000000 mentat-ai-0.1.1/mentat/__main__.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     6013 2023-07-25 13:33:37.000000 mentat-ai-0.1.1/mentat/app.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     4175 2023-07-22 22:55:34.000000 mentat-ai-0.1.1/mentat/change_conflict_resolution.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     5095 2023-07-22 22:55:34.000000 mentat-ai-0.1.1/mentat/code_change.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     4283 2023-07-22 22:55:34.000000 mentat-ai-0.1.1/mentat/code_change_display.py
--rw-r--r--   0 biobootloader   (501) staff       (20)    13048 2023-07-25 13:33:37.000000 mentat-ai-0.1.1/mentat/code_file_manager.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1536 2023-07-21 00:32:22.000000 mentat-ai-0.1.1/mentat/config_manager.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     2340 2023-07-22 22:55:34.000000 mentat-ai-0.1.1/mentat/conversation.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      325 2023-07-25 13:34:36.000000 mentat-ai-0.1.1/mentat/default_config.json
--rw-r--r--   0 biobootloader   (501) staff       (20)     3798 2023-07-25 13:33:37.000000 mentat-ai-0.1.1/mentat/llm_api.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1696 2023-07-22 22:55:34.000000 mentat-ai-0.1.1/mentat/logging_config.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     8169 2023-07-22 22:55:34.000000 mentat-ai-0.1.1/mentat/parsing.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     3559 2023-07-15 05:21:35.000000 mentat-ai-0.1.1/mentat/prompts.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1452 2023-07-21 00:32:22.000000 mentat-ai-0.1.1/mentat/streaming_printer.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     3193 2023-07-21 00:32:22.000000 mentat-ai-0.1.1/mentat/user_input_manager.py
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-25 18:56:19.065137 mentat-ai-0.1.1/mentat_ai.egg-info/
--rw-r--r--   0 biobootloader   (501) staff       (20)       75 2023-07-25 18:56:19.000000 mentat-ai-0.1.1/mentat_ai.egg-info/PKG-INFO
--rw-r--r--   0 biobootloader   (501) staff       (20)      997 2023-07-25 18:56:19.000000 mentat-ai-0.1.1/mentat_ai.egg-info/SOURCES.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)        1 2023-07-25 18:56:19.000000 mentat-ai-0.1.1/mentat_ai.egg-info/dependency_links.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)       46 2023-07-25 18:56:19.000000 mentat-ai-0.1.1/mentat_ai.egg-info/entry_points.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)      765 2023-07-25 18:56:19.000000 mentat-ai-0.1.1/mentat_ai.egg-info/requires.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)       21 2023-07-25 18:56:19.000000 mentat-ai-0.1.1/mentat_ai.egg-info/top_level.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)       91 2023-07-21 00:32:22.000000 mentat-ai-0.1.1/pyproject.toml
--rw-r--r--   0 biobootloader   (501) staff       (20)       38 2023-07-25 18:56:19.067462 mentat-ai-0.1.1/setup.cfg
--rw-r--r--   0 biobootloader   (501) staff       (20)      463 2023-07-25 18:55:48.000000 mentat-ai-0.1.1/setup.py
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-25 18:56:19.065241 mentat-ai-0.1.1/testbed/
--rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-05-31 00:08:09.000000 mentat-ai-0.1.1/testbed/__init__.py
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-25 18:56:19.065590 mentat-ai-0.1.1/testbed/multifile_calculator/
--rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-05-31 00:07:36.000000 mentat-ai-0.1.1/testbed/multifile_calculator/__init__.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      580 2023-07-18 20:17:52.000000 mentat-ai-0.1.1/testbed/multifile_calculator/calculator.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      179 2023-07-18 20:17:50.000000 mentat-ai-0.1.1/testbed/multifile_calculator/operations.py
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-25 18:56:19.067154 mentat-ai-0.1.1/tests/
--rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-07-12 22:56:07.000000 mentat-ai-0.1.1/tests/__init__.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     4010 2023-07-21 00:32:22.000000 mentat-ai-0.1.1/tests/benchmark_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     2580 2023-07-21 00:32:22.000000 mentat-ai-0.1.1/tests/code_file_manager_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     7507 2023-07-22 22:55:34.000000 mentat-ai-0.1.1/tests/codechange_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      148 2023-07-21 00:32:22.000000 mentat-ai-0.1.1/tests/config_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     3689 2023-07-21 00:32:22.000000 mentat-ai-0.1.1/tests/conftest.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1467 2023-07-12 22:02:48.000000 mentat-ai-0.1.1/tests/measure_api_speed.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     2605 2023-07-25 13:33:37.000000 mentat-ai-0.1.1/tests/record_benchmark.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     2924 2023-07-22 22:55:34.000000 mentat-ai-0.1.1/tests/system_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      825 2023-07-21 00:32:22.000000 mentat-ai-0.1.1/tests/ui_test.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-26 04:00:56.298325 mentat-ai-0.1.2/
+-rw-r--r--   0 biobootloader   (501) staff       (20)    11357 2023-07-08 00:24:17.000000 mentat-ai-0.1.2/LICENSE
+-rw-r--r--   0 biobootloader   (501) staff       (20)       75 2023-07-26 04:00:56.298210 mentat-ai-0.1.2/PKG-INFO
+-rw-r--r--   0 biobootloader   (501) staff       (20)     2722 2023-07-26 03:56:30.000000 mentat-ai-0.1.2/README.md
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-26 04:00:56.295221 mentat-ai-0.1.2/mentat/
+-rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-07-12 23:06:24.000000 mentat-ai-0.1.2/mentat/__init__.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      166 2023-07-21 00:32:22.000000 mentat-ai-0.1.2/mentat/__main__.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     6013 2023-07-25 13:33:37.000000 mentat-ai-0.1.2/mentat/app.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4175 2023-07-22 22:55:34.000000 mentat-ai-0.1.2/mentat/change_conflict_resolution.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     5095 2023-07-22 22:55:34.000000 mentat-ai-0.1.2/mentat/code_change.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4283 2023-07-22 22:55:34.000000 mentat-ai-0.1.2/mentat/code_change_display.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)    13118 2023-07-26 03:57:32.000000 mentat-ai-0.1.2/mentat/code_file_manager.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1536 2023-07-21 00:32:22.000000 mentat-ai-0.1.2/mentat/config_manager.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     2340 2023-07-22 22:55:34.000000 mentat-ai-0.1.2/mentat/conversation.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      325 2023-07-25 13:34:36.000000 mentat-ai-0.1.2/mentat/default_config.json
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3798 2023-07-25 13:33:37.000000 mentat-ai-0.1.2/mentat/llm_api.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1696 2023-07-22 22:55:34.000000 mentat-ai-0.1.2/mentat/logging_config.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     8169 2023-07-22 22:55:34.000000 mentat-ai-0.1.2/mentat/parsing.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3559 2023-07-15 05:21:35.000000 mentat-ai-0.1.2/mentat/prompts.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1452 2023-07-21 00:32:22.000000 mentat-ai-0.1.2/mentat/streaming_printer.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3193 2023-07-21 00:32:22.000000 mentat-ai-0.1.2/mentat/user_input_manager.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-26 04:00:56.295902 mentat-ai-0.1.2/mentat_ai.egg-info/
+-rw-r--r--   0 biobootloader   (501) staff       (20)       75 2023-07-26 04:00:56.000000 mentat-ai-0.1.2/mentat_ai.egg-info/PKG-INFO
+-rw-r--r--   0 biobootloader   (501) staff       (20)      997 2023-07-26 04:00:56.000000 mentat-ai-0.1.2/mentat_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)        1 2023-07-26 04:00:56.000000 mentat-ai-0.1.2/mentat_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)       46 2023-07-26 04:00:56.000000 mentat-ai-0.1.2/mentat_ai.egg-info/entry_points.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)      765 2023-07-26 04:00:56.000000 mentat-ai-0.1.2/mentat_ai.egg-info/requires.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)       21 2023-07-26 04:00:56.000000 mentat-ai-0.1.2/mentat_ai.egg-info/top_level.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)       91 2023-07-21 00:32:22.000000 mentat-ai-0.1.2/pyproject.toml
+-rw-r--r--   0 biobootloader   (501) staff       (20)       38 2023-07-26 04:00:56.298356 mentat-ai-0.1.2/setup.cfg
+-rw-r--r--   0 biobootloader   (501) staff       (20)      463 2023-07-26 04:00:19.000000 mentat-ai-0.1.2/setup.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-26 04:00:56.296009 mentat-ai-0.1.2/testbed/
+-rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-05-31 00:08:09.000000 mentat-ai-0.1.2/testbed/__init__.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-26 04:00:56.296393 mentat-ai-0.1.2/testbed/multifile_calculator/
+-rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-05-31 00:07:36.000000 mentat-ai-0.1.2/testbed/multifile_calculator/__init__.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      580 2023-07-18 20:17:52.000000 mentat-ai-0.1.2/testbed/multifile_calculator/calculator.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      179 2023-07-18 20:17:50.000000 mentat-ai-0.1.2/testbed/multifile_calculator/operations.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-26 04:00:56.298045 mentat-ai-0.1.2/tests/
+-rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-07-12 22:56:07.000000 mentat-ai-0.1.2/tests/__init__.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4010 2023-07-21 00:32:22.000000 mentat-ai-0.1.2/tests/benchmark_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     2580 2023-07-21 00:32:22.000000 mentat-ai-0.1.2/tests/code_file_manager_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     7507 2023-07-22 22:55:34.000000 mentat-ai-0.1.2/tests/codechange_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      148 2023-07-21 00:32:22.000000 mentat-ai-0.1.2/tests/config_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3689 2023-07-21 00:32:22.000000 mentat-ai-0.1.2/tests/conftest.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1467 2023-07-12 22:02:48.000000 mentat-ai-0.1.2/tests/measure_api_speed.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     2605 2023-07-25 13:33:37.000000 mentat-ai-0.1.2/tests/record_benchmark.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     2924 2023-07-22 22:55:34.000000 mentat-ai-0.1.2/tests/system_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      825 2023-07-21 00:32:22.000000 mentat-ai-0.1.2/tests/ui_test.py
```

### Comparing `mentat-ai-0.1.1/LICENSE` & `mentat-ai-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.1/README.md` & `mentat-ai-0.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -14,52 +14,57 @@
 
 Unlike Copilot, Mentat coordinates edits across multiple locations and files. And unlike ChatGPT, Mentat already has the context of your project - no copy and pasting required!
 
 Want help understanding a new codebase? Need to add a new feature? Refactor existing code? Mentat can do it!
 
 # 🍿 Example Videos
 
-Coming soon!
+See the videos on [Twitter](https://twitter.com/bio_bootloader/status/1683906735248125955) or YouTube:
+- [Intro (2 min)](https://www.youtube.com/watch?v=lODjaWclwpY)
+- [Explaining and editing Llama2.c (3 min)](https://www.youtube.com/watch?v=qSyTWMFOjPs)
+- [More Mentat features (4 min)](https://www.youtube.com/watch?v=YJLDIqq8k2A)
 
 # ⚙️ Setup
 
 ## Install
 
-If you just want to use Mentat, use one of these methods to install it:
-- PyPI: coming soon!
+Before installing, it's suggested that you create a virtual environment to install it in:
+
+```
+python3 -m venv .venv
+source .venv/bin/activate
+```
+
+Note that you'll have to have activated the virtual environment to run mentat if you install it there.
+
+There are then 3 install methods. The first two will just let you run it:
+- PyPI: `python -m pip install mentat-ai`
 - Github: `python -m pip install git+https://github.com/biobootloader/mentat.git`
 
-If you are more adventurous and would like to use and edit Mentat, try this:
+The third option is useful if you'd also like to modify Mentat's code, as well as run it:
+
 ```
-# Clone the repo
 git clone https://github.com/biobootloader/mentat.git
 cd mentat
 
-# optionally, set up a virtual environment to install it in
-# if you do this, you'll only be able to run mentat while it's activated
-python -m venv .venv
-source .venv/bin/activate
-
-pip install -r requirements.txt
-
 # install with pip in editable mode:
 pip install -e .
 ```
 
 ## Add your OpenAI API Key
 
 You'll need to have API access to GPT-4 to run Mentat. There are a few options to provide Mentat with your OpenAI API key:
 
 1. Create a `.env` file with the line `OPENAI_API_KEY=<your-api-key>` in the directory you plan to run mentat in or in `~/.mentat/.env`
 2. Run `export OPENAI_API_KEY=<your key here>` prior to running Mentat
 3. Place the previous command in your `.bashrc` or `.zshrc` to export your key on every terminal startup
 
 ## Configuration
 
-For custom configuration options see [here](docs/configuration.md)
+For custom configuration options see [configuration.md](docs/configuration.md)
 
 
 # 🚀 Usage
 Run Mentat with:
 
 `mentat <paths to files or directories>`
```

### Comparing `mentat-ai-0.1.1/mentat/app.py` & `mentat-ai-0.1.2/mentat/app.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.1/mentat/change_conflict_resolution.py` & `mentat-ai-0.1.2/mentat/change_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.1/mentat/code_change.py` & `mentat-ai-0.1.2/mentat/code_change.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.1/mentat/code_change_display.py` & `mentat-ai-0.1.2/mentat/code_change_display.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.1/mentat/code_file_manager.py` & `mentat-ai-0.1.2/mentat/code_file_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,16 @@
     ".lua",     # Lua
     ".pl",      # Perl
     ".sql",     # SQL
     ".r",       # R
     ".m",       # objective-c
     ".sh",      # shell scripts
     ".f",       # fortran
+    ".jsx",     # javascript react
+    ".tsx",     # typescript react
 ]
 default_filetype_exclude_list = []
 # fmt: on
 
 
 def _get_git_diff_for_path(git_root, path: str) -> str:
     return subprocess.check_output(["git", "diff", path], cwd=git_root).decode("utf-8")
```

### Comparing `mentat-ai-0.1.1/mentat/config_manager.py` & `mentat-ai-0.1.2/mentat/config_manager.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.1/mentat/conversation.py` & `mentat-ai-0.1.2/mentat/conversation.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.1/mentat/llm_api.py` & `mentat-ai-0.1.2/mentat/llm_api.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.1/mentat/logging_config.py` & `mentat-ai-0.1.2/mentat/logging_config.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.1/mentat/parsing.py` & `mentat-ai-0.1.2/mentat/parsing.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.1/mentat/prompts.py` & `mentat-ai-0.1.2/mentat/prompts.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.1/mentat/streaming_printer.py` & `mentat-ai-0.1.2/mentat/streaming_printer.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.1/mentat/user_input_manager.py` & `mentat-ai-0.1.2/mentat/user_input_manager.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.1/mentat_ai.egg-info/SOURCES.txt` & `mentat-ai-0.1.2/mentat_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.1/mentat_ai.egg-info/requires.txt` & `mentat-ai-0.1.2/mentat_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.1/testbed/multifile_calculator/calculator.py` & `mentat-ai-0.1.2/testbed/multifile_calculator/calculator.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.1/tests/benchmark_test.py` & `mentat-ai-0.1.2/tests/benchmark_test.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.1/tests/code_file_manager_test.py` & `mentat-ai-0.1.2/tests/code_file_manager_test.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.1/tests/codechange_test.py` & `mentat-ai-0.1.2/tests/codechange_test.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.1/tests/conftest.py` & `mentat-ai-0.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.1/tests/measure_api_speed.py` & `mentat-ai-0.1.2/tests/measure_api_speed.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.1/tests/record_benchmark.py` & `mentat-ai-0.1.2/tests/record_benchmark.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.1/tests/system_test.py` & `mentat-ai-0.1.2/tests/system_test.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.1/tests/ui_test.py` & `mentat-ai-0.1.2/tests/ui_test.py`

 * *Files identical despite different names*

