# Comparing `tmp/recipe2txt-0.1.1.tar.gz` & `tmp/recipe2txt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recipe2txt-0.1.1.tar", last modified: Tue Jul 25 21:05:38 2023, max compression
+gzip compressed data, was "recipe2txt-0.2.0.tar", last modified: Wed Jul 26 13:20:22 2023, max compression
```

## Comparing `recipe2txt-0.1.1.tar` & `recipe2txt-0.2.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2023-07-25 21:05:38.320814 recipe2txt-0.1.1/
--rw-rw-r--   0 pc        (1000) pc        (1000)    35149 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/LICENSE
--rw-rw-r--   0 pc        (1000) pc        (1000)     5359 2023-07-25 21:05:38.320814 recipe2txt-0.1.1/PKG-INFO
--rw-rw-r--   0 pc        (1000) pc        (1000)     4239 2023-07-25 20:13:34.000000 recipe2txt-0.1.1/README.md
--rw-rw-r--   0 pc        (1000) pc        (1000)     1622 2023-07-25 21:03:53.000000 recipe2txt-0.1.1/pyproject.toml
-drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2023-07-25 21:05:38.312814 recipe2txt-0.1.1/recipe2txt/
--rw-rw-r--   0 pc        (1000) pc        (1000)        0 2023-07-11 12:26:00.000000 recipe2txt-0.1.1/recipe2txt/__init__.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     9047 2023-07-25 20:13:34.000000 recipe2txt-0.1.1/recipe2txt/argparse.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     3736 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/recipe2txt/fetcher_abstract.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     3057 2023-07-25 20:13:00.000000 recipe2txt-0.1.1/recipe2txt/fetcher_async.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     2164 2023-07-25 20:13:00.000000 recipe2txt-0.1.1/recipe2txt/fetcher_serial.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     7580 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/recipe2txt/file_setup.py
--rw-rw-r--   0 pc        (1000) pc        (1000)    13148 2023-07-25 21:02:27.000000 recipe2txt-0.1.1/recipe2txt/html2recipe.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     1300 2023-07-25 20:13:00.000000 recipe2txt-0.1.1/recipe2txt/re2txt.py
--rw-rw-r--   0 pc        (1000) pc        (1000)    10373 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/recipe2txt/sql.py
-drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2023-07-25 21:05:38.316814 recipe2txt-0.1.1/recipe2txt/utils/
--rw-rw-r--   0 pc        (1000) pc        (1000)    11382 2023-07-25 19:34:56.000000 recipe2txt-0.1.1/recipe2txt/utils/ContextLogger.py
--rw-rw-r--   0 pc        (1000) pc        (1000)        2 2023-03-10 12:21:19.000000 recipe2txt-0.1.1/recipe2txt/utils/__init__.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     1069 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/recipe2txt/utils/conditional_imports.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     4255 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/recipe2txt/utils/markdown.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     7316 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/recipe2txt/utils/misc.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     2347 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/recipe2txt/utils/timer.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     3203 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/recipe2txt/utils/traceback_utils.py
-drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2023-07-25 21:05:38.316814 recipe2txt-0.1.1/recipe2txt.egg-info/
--rw-rw-r--   0 pc        (1000) pc        (1000)     5359 2023-07-25 21:05:38.000000 recipe2txt-0.1.1/recipe2txt.egg-info/PKG-INFO
--rw-rw-r--   0 pc        (1000) pc        (1000)      882 2023-07-25 21:05:38.000000 recipe2txt-0.1.1/recipe2txt.egg-info/SOURCES.txt
--rw-rw-r--   0 pc        (1000) pc        (1000)        1 2023-07-25 21:05:38.000000 recipe2txt-0.1.1/recipe2txt.egg-info/dependency_links.txt
--rw-rw-r--   0 pc        (1000) pc        (1000)       86 2023-07-25 21:05:38.000000 recipe2txt-0.1.1/recipe2txt.egg-info/entry_points.txt
--rw-rw-r--   0 pc        (1000) pc        (1000)      199 2023-07-25 21:05:38.000000 recipe2txt-0.1.1/recipe2txt.egg-info/requires.txt
--rw-rw-r--   0 pc        (1000) pc        (1000)       11 2023-07-25 21:05:38.000000 recipe2txt-0.1.1/recipe2txt.egg-info/top_level.txt
--rw-rw-r--   0 pc        (1000) pc        (1000)       38 2023-07-25 21:05:38.320814 recipe2txt-0.1.1/setup.cfg
-drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2023-07-25 21:05:38.320814 recipe2txt-0.1.1/test/
--rw-rw-r--   0 pc        (1000) pc        (1000)    14635 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/test/test_contextlogger.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     3484 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/test/test_fetcher.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     5694 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/test/test_file_setup.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     5155 2023-07-25 20:03:06.000000 recipe2txt-0.1.1/test/test_helpers.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     4477 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/test/test_html2recipe.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     6332 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/test/test_misc.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     8542 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/test/test_sql.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     1458 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/test/test_timer.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     3197 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/test/test_traceback_utils.py
+drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2023-07-26 13:20:22.589468 recipe2txt-0.2.0/
+-rw-rw-r--   0 pc        (1000) pc        (1000)    35149 2023-07-25 13:15:25.000000 recipe2txt-0.2.0/LICENSE
+-rw-rw-r--   0 pc        (1000) pc        (1000)     5494 2023-07-26 13:20:22.589468 recipe2txt-0.2.0/PKG-INFO
+-rw-rw-r--   0 pc        (1000) pc        (1000)     4374 2023-07-26 13:18:36.000000 recipe2txt-0.2.0/README.md
+-rw-rw-r--   0 pc        (1000) pc        (1000)     1622 2023-07-26 13:18:36.000000 recipe2txt-0.2.0/pyproject.toml
+drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2023-07-26 13:20:22.585468 recipe2txt-0.2.0/recipe2txt/
+-rw-rw-r--   0 pc        (1000) pc        (1000)        0 2023-07-11 12:26:00.000000 recipe2txt-0.2.0/recipe2txt/__init__.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     9060 2023-07-26 13:18:36.000000 recipe2txt-0.2.0/recipe2txt/argparse.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     3774 2023-07-26 13:10:14.000000 recipe2txt-0.2.0/recipe2txt/fetcher_abstract.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     3057 2023-07-25 20:13:00.000000 recipe2txt-0.2.0/recipe2txt/fetcher_async.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     2164 2023-07-25 20:13:00.000000 recipe2txt-0.2.0/recipe2txt/fetcher_serial.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     8120 2023-07-26 13:10:14.000000 recipe2txt-0.2.0/recipe2txt/file_setup.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)    13261 2023-07-26 13:18:36.000000 recipe2txt-0.2.0/recipe2txt/html2recipe.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     1300 2023-07-25 20:13:00.000000 recipe2txt-0.2.0/recipe2txt/re2txt.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)    10373 2023-07-25 13:15:25.000000 recipe2txt-0.2.0/recipe2txt/sql.py
+drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2023-07-26 13:20:22.585468 recipe2txt-0.2.0/recipe2txt/utils/
+-rw-rw-r--   0 pc        (1000) pc        (1000)    11488 2023-07-26 13:10:14.000000 recipe2txt-0.2.0/recipe2txt/utils/ContextLogger.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)        2 2023-03-10 12:21:19.000000 recipe2txt-0.2.0/recipe2txt/utils/__init__.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     1069 2023-07-25 13:15:25.000000 recipe2txt-0.2.0/recipe2txt/utils/conditional_imports.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     4255 2023-07-25 13:15:25.000000 recipe2txt-0.2.0/recipe2txt/utils/markdown.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     7316 2023-07-25 13:15:25.000000 recipe2txt-0.2.0/recipe2txt/utils/misc.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     2347 2023-07-25 13:15:25.000000 recipe2txt-0.2.0/recipe2txt/utils/timer.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     3203 2023-07-25 13:15:25.000000 recipe2txt-0.2.0/recipe2txt/utils/traceback_utils.py
+drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2023-07-26 13:20:22.585468 recipe2txt-0.2.0/recipe2txt.egg-info/
+-rw-rw-r--   0 pc        (1000) pc        (1000)     5494 2023-07-26 13:20:22.000000 recipe2txt-0.2.0/recipe2txt.egg-info/PKG-INFO
+-rw-rw-r--   0 pc        (1000) pc        (1000)      882 2023-07-26 13:20:22.000000 recipe2txt-0.2.0/recipe2txt.egg-info/SOURCES.txt
+-rw-rw-r--   0 pc        (1000) pc        (1000)        1 2023-07-26 13:20:22.000000 recipe2txt-0.2.0/recipe2txt.egg-info/dependency_links.txt
+-rw-rw-r--   0 pc        (1000) pc        (1000)       86 2023-07-26 13:20:22.000000 recipe2txt-0.2.0/recipe2txt.egg-info/entry_points.txt
+-rw-rw-r--   0 pc        (1000) pc        (1000)      199 2023-07-26 13:20:22.000000 recipe2txt-0.2.0/recipe2txt.egg-info/requires.txt
+-rw-rw-r--   0 pc        (1000) pc        (1000)       11 2023-07-26 13:20:22.000000 recipe2txt-0.2.0/recipe2txt.egg-info/top_level.txt
+-rw-rw-r--   0 pc        (1000) pc        (1000)       38 2023-07-26 13:20:22.589468 recipe2txt-0.2.0/setup.cfg
+drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2023-07-26 13:20:22.589468 recipe2txt-0.2.0/test/
+-rw-rw-r--   0 pc        (1000) pc        (1000)    14635 2023-07-25 13:15:25.000000 recipe2txt-0.2.0/test/test_contextlogger.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     3484 2023-07-25 13:15:25.000000 recipe2txt-0.2.0/test/test_fetcher.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     5834 2023-07-26 13:10:14.000000 recipe2txt-0.2.0/test/test_file_setup.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     5155 2023-07-26 13:10:14.000000 recipe2txt-0.2.0/test/test_helpers.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     4942 2023-07-26 13:10:14.000000 recipe2txt-0.2.0/test/test_html2recipe.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     6332 2023-07-25 13:15:25.000000 recipe2txt-0.2.0/test/test_misc.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     8542 2023-07-25 13:15:25.000000 recipe2txt-0.2.0/test/test_sql.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     1458 2023-07-25 13:15:25.000000 recipe2txt-0.2.0/test/test_timer.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     3197 2023-07-25 13:15:25.000000 recipe2txt-0.2.0/test/test_traceback_utils.py
```

### Comparing `recipe2txt-0.1.1/LICENSE` & `recipe2txt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.1/PKG-INFO` & `recipe2txt-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recipe2txt
-Version: 0.1.1
+Version: 0.2.0
 Summary: Scrapes recipes and converts them to txt or markdown
 Author-email: Jan Philipp Berg <git.7ksst@aleeas.com>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Homepage, https://github.com/jp-berg/recipe2txt
 Project-URL: Bug Tracker, https://github.com/jp-berg/recipe2txt/issues
 Keywords: recipes,cooking,scraping,website
 Classifier: Programming Language :: Python :: 3
@@ -37,16 +37,20 @@
 
 # WARNING
 
 THIS SOFTWARE IS AT AN EARLY DEVELOPEMENT STAGE.
 
 BE CAREFUL SETTING THE `--output`-FLAG, ANY EXISTING FILES WITH THE SAME NAME WILL BE OVERWRITTEN.
 
+TESTED ONLY ON KUBUNTU 23.04.
+
 # Usage
 
+Install with `pip install recipe2txt`. You can either use `recipe2txt` or `re2txt` to run the program.
+
 ```
 usage: recipes2txt [-h] [-u URL [URL ...]] [-f FILE [FILE ...]] [-o OUTPUT]
                    [-v {debug,info,warning,error,critical}] [-con CONNECTIONS] [-ia] [-c {only,new,default}] [-d]
                    [-t TIMEOUT] [-md] [-sa | -erase | -do DEFAULT_OUTPUT_FILE]
 
 Scrapes URLs of recipes into text files
```

### Comparing `recipe2txt-0.1.1/README.md` & `recipe2txt-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,20 @@
 
 # WARNING
 
 THIS SOFTWARE IS AT AN EARLY DEVELOPEMENT STAGE.
 
 BE CAREFUL SETTING THE `--output`-FLAG, ANY EXISTING FILES WITH THE SAME NAME WILL BE OVERWRITTEN.
 
+TESTED ONLY ON KUBUNTU 23.04.
+
 # Usage
 
+Install with `pip install recipe2txt`. You can either use `recipe2txt` or `re2txt` to run the program.
+
 ```
 usage: recipes2txt [-h] [-u URL [URL ...]] [-f FILE [FILE ...]] [-o OUTPUT]
                    [-v {debug,info,warning,error,critical}] [-con CONNECTIONS] [-ia] [-c {only,new,default}] [-d]
                    [-t TIMEOUT] [-md] [-sa | -erase | -do DEFAULT_OUTPUT_FILE]
 
 Scrapes URLs of recipes into text files
```

### Comparing `recipe2txt-0.1.1/pyproject.toml` & `recipe2txt-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "recipe2txt"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
   { name="Jan Philipp Berg", email="git.7ksst@aleeas.com" },
 ]
 description = "Scrapes recipes and converts them to txt or markdown"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "GNU General Public License v3 or later (GPLv3+)"}
```

### Comparing `recipe2txt-0.1.1/recipe2txt/argparse.py` & `recipe2txt-0.2.0/recipe2txt/argparse.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
     db_file, recipe_file, log_file = file_setup(a.debug, a.output, a.markdown)
     root_log_setup(string2level[a.verbosity], str(log_file))
     if logger.isEnabledFor(logging.DEBUG):
         logger.debug("CLI-ARGS: %s\t%s", os.linesep, (os.linesep + '\t').join(args2strs(a)))
     logger.info("--- Preparing arguments ---")
     sancheck_args(a, recipe_file)
     if recipe_file.stat().st_size > 0:
-        logger.warning("The output-file %s already exists. It will be overwritten.")
+        logger.warning("The output-file %s already exists. It will be overwritten.", recipe_file)
     else:
         logger.info("Output set to: %s", recipe_file)
     unprocessed: list[str] = read_files(*a.file)
     unprocessed += a.url
     processed: set[URL] = extract_urls(unprocessed)
     if not processed:
         logger.critical("No valid URL passed")
```

### Comparing `recipe2txt-0.1.1/recipe2txt/fetcher_abstract.py` & `recipe2txt-0.2.0/recipe2txt/fetcher_abstract.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,20 +75,22 @@
 
     @abstractmethod
     def fetch(self, urls: set[URL]) -> None:
         pass
 
     def gen_lines(self) -> list[str]:
         recipes = []
+        count = 0
         for recipe in self.db.get_recipes():
             if formatted := h2r.recipe2out(recipe, self.counts, md=self.markdown):
+                count += 1
                 for line in formatted:
                     recipes.append(line)
 
-        if len(recipes) > 2:
+        if count > 3:
             titles_raw = self.db.get_titles()
             if self.markdown:
                 titles_md_fmt = [f"{section_link(esc(name), fragmentified=True)} - {esc(host)}{linesep}"
                                  for name, host in titles_raw]
                 titles = ordered(*titles_md_fmt)
             else:
                 titles = [f"{name} - {host}{linesep}" for name, host in titles_raw]
```

### Comparing `recipe2txt-0.1.1/recipe2txt/fetcher_async.py` & `recipe2txt-0.2.0/recipe2txt/fetcher_async.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.1/recipe2txt/fetcher_serial.py` & `recipe2txt-0.2.0/recipe2txt/fetcher_serial.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.1/recipe2txt/file_setup.py` & `recipe2txt-0.2.0/recipe2txt/file_setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,77 +13,89 @@
 # You should have received a copy of the GNU General Public License along with recipe2txt.
 # If not, see <https://www.gnu.org/licenses/>.
 
 import os
 import sys
 from shutil import rmtree
 from time import strftime, gmtime
-from typing import Final, Tuple, Literal
+from typing import Final, Tuple, Literal, NamedTuple
 from pathlib import Path
 
-from xdg_base_dirs import xdg_data_home
+from xdg_base_dirs import xdg_data_home, xdg_config_home, xdg_state_home
 
 from recipe2txt.utils.conditional_imports import LiteralString
 from recipe2txt.html2recipe import errors2str
 from recipe2txt.sql import AccessibleDatabase, ensure_accessible_db_critical
 from recipe2txt.utils.ContextLogger import get_logger
 from recipe2txt.utils.misc import ensure_existence_dir, ensure_accessible_file_critical, File, Directory, full_path
 
 logger = get_logger(__name__)
 
 PROGRAM_NAME: Final[LiteralString] = "recipes2txt"
 
-DEFAULT_DATA_DIRECTORY: Final[Path] = Path(xdg_data_home(), PROGRAM_NAME)
-DEBUG_DATA_DIRECTORY: Final[Path] = Path(Path(__file__).parents[1], "test", "testfiles", "data")
 
+class ProgramDirectories(NamedTuple):
+    data: Path
+    config: Path
+    state: Path
+
+
+default_dirs: Final[ProgramDirectories] = ProgramDirectories(xdg_data_home() / PROGRAM_NAME,
+                                                             xdg_config_home() / PROGRAM_NAME,
+                                                             xdg_state_home() / PROGRAM_NAME)
+
+DEBUG_DIRECTORY_BASE: Final[Path] = Path(__file__).parents[1] / "test" / "testfiles" / "debug-dirs"
+
+debug_dirs: Final[ProgramDirectories] = ProgramDirectories(DEBUG_DIRECTORY_BASE / "data",
+                                                           DEBUG_DIRECTORY_BASE / "config",
+                                                           DEBUG_DIRECTORY_BASE / "state")
 
 LOG_NAME: Final[LiteralString] = "debug.log"
 DB_NAME: Final[LiteralString] = PROGRAM_NAME + ".sqlite3"
 RECIPES_NAME: Final[LiteralString] = "recipes"
 RECIPES_NAME_TXT: Final[LiteralString] = RECIPES_NAME + ".txt"
 RECIPES_NAME_MD: Final[LiteralString] = RECIPES_NAME + ".md"
 DEFAULT_URLS_NAME: Final[LiteralString] = "urls.txt"
 DEFAULT_OUTPUT_LOCATION_NAME: Final[LiteralString] = "default_output_location.txt"
 
 
 def file_setup(debug: bool = False, output: str = "", markdown: bool = False) -> Tuple[AccessibleDatabase, File, File]:
-    data_path = DEBUG_DATA_DIRECTORY if debug else DEFAULT_DATA_DIRECTORY
-    db_file = ensure_accessible_db_critical(data_path, DB_NAME)
-    log_file = ensure_accessible_file_critical(data_path, LOG_NAME)
+    directory = debug_dirs if debug else default_dirs
+
+    db_file = ensure_accessible_db_critical(directory.data, DB_NAME)
+    log_file = ensure_accessible_file_critical(directory.state, LOG_NAME)
 
     if output:
         output_file = ensure_accessible_file_critical(output)
     else:
-        output_file = get_default_output(Directory(data_path), markdown)
+        output_file = get_default_output(directory.config, markdown)
 
     return db_file, output_file, log_file
 
 
 def get_files(debug: bool = False) -> list[str]:
-    files = []
-    if DEFAULT_DATA_DIRECTORY.is_dir() and not debug:
-        files = [str(file) for file in DEFAULT_DATA_DIRECTORY.iterdir()]
-    if DEBUG_DATA_DIRECTORY.is_dir():
-        files += [str(file) for file in DEBUG_DATA_DIRECTORY.iterdir()]
-
+    directories = list(debug_dirs)
+    directories = directories if debug else directories + list(default_dirs)
+    files = [str(file) for directory in directories if directory.is_dir()
+             for file in directory.iterdir()]
     return files
 
 
 def erase_files(debug: bool = False) -> None:
-    if DEFAULT_DATA_DIRECTORY.is_dir() and not debug:
-        logger.warning("Deleting %s", DEFAULT_DATA_DIRECTORY)
-        rmtree(DEFAULT_DATA_DIRECTORY)
+    directories = list(debug_dirs)
+    directories = directories if debug else directories + list(default_dirs)
 
-    if DEBUG_DATA_DIRECTORY.is_dir():
-        logger.warning("Deleting: %s", DEBUG_DATA_DIRECTORY)
-        rmtree(DEBUG_DATA_DIRECTORY)
+    for directory in directories:
+        if directory.is_dir():
+            logger.warning("Deleting %s", directory)
+            rmtree(directory)
 
 
-def get_default_output(data_path: Directory, markdown: bool) -> File:
-    output_location_file = data_path / DEFAULT_OUTPUT_LOCATION_NAME
+def get_default_output(config_path: Path, markdown: bool) -> File:
+    output_location_file = config_path / DEFAULT_OUTPUT_LOCATION_NAME
     if output_location_file.is_file():
         text = output_location_file.read_text().split(os.linesep)
         text = [line for line in text if line]
         if len(text) != 2:
             logger.error(f"The config file ({output_location_file}) has unexpected content.")
             sys.exit(os.EX_DATAERR)
         output = text[1] if markdown else text[0]
@@ -91,15 +103,15 @@
     else:
         recipes_name = RECIPES_NAME_MD if markdown else RECIPES_NAME_TXT
         output_file = ensure_accessible_file_critical(Directory(Path.cwd()), recipes_name)
     return output_file
 
 
 def set_default_output(filepath: str | Literal["RESET"], debug: bool = False) -> None:
-    data_dir = DEBUG_DATA_DIRECTORY if debug else DEFAULT_DATA_DIRECTORY
+    data_dir = debug_dirs.config if debug else default_dirs.config
     if filepath == "RESET":
         try:
             os.remove(data_dir / DEFAULT_OUTPUT_LOCATION_NAME)
             logger.warning("Removed default output location. When called without specifying the output-file recipes"
                            " will now be written in the current working directory with the name %s", RECIPES_NAME_TXT)
         except FileNotFoundError:
             logger.warning("No default output set")
@@ -135,15 +147,15 @@
 
 def write_errors(debug: bool = False) -> int:
     if not (errors := errors2str()):
         return 0
 
     logger.info("---Writing error reports---")
 
-    data_path = DEBUG_DATA_DIRECTORY if debug else DEFAULT_DATA_DIRECTORY
+    data_path = debug_dirs.state if debug else default_dirs.state
     if not (error_dir := ensure_existence_dir(data_path, "error_reports")):
         logger.error("Could not create %s, no reports will be written", data_path / "error_reports")
         return 0
     how_to_report_file = error_dir / "how_to_report_errors.txt"
     if not how_to_report_file.is_file():
         how_to_report_file.write_text(how_to_report_txt)
```

### Comparing `recipe2txt-0.1.1/recipe2txt/html2recipe.py` & `recipe2txt-0.2.0/recipe2txt/html2recipe.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 # recipe2txt is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with recipe2txt.
 # If not, see <https://www.gnu.org/licenses/>.
 
-import logging
 import urllib
 from enum import IntEnum
 from typing import NewType, Final, Optional, NamedTuple, Any, Callable
+import re
 from os import linesep
 import traceback
 from importlib_metadata import version
 import recipe_scrapers
 from recipe_scrapers._exceptions import WebsiteNotImplementedError, NoSchemaFoundInWildMode, SchemaOrgException, \
     ElementNotFoundInHtml
 from recipe2txt.utils.markdown import *
@@ -173,15 +173,15 @@
                                   "recipe-scrapers version: " + code(SCRAPER_VERSION),
                                   "exception: " + code(exception_name),
                                   "triggered by calling: " +  code(triggered_by),
                                   "triggered on: ") + unordered(*urls, level=1)
 
                 tb_ex_list = [error.traceback for error in parsing_error_list]
                 shared_frames = get_shared_frames(tb_ex_list)
-                formatted_stacks = format_stacks(tb_ex_list, shared_frames, "Rezepte")
+                formatted_stacks = format_stacks(tb_ex_list, shared_frames, "recipe2txt")
 
                 if len(urls) > 1:
                     dot_explanation = italic("'...' indicates frames present in all traces"
                                              "(but only shown in the first)") + linesep * 2
                 else:
                     dot_explanation = ""
 
@@ -194,14 +194,16 @@
 
                 msg += "".join(infos) + linesep + "".join(stack_traces)
                 reports.append((title, msg))
 
     return reports
 
 
+contains_alphanumeric = re.compile("\w")
+
 def info2str(method: str, info: Any) -> str:
     log = logger.error if method in ON_DISPLAY else logger.warning
     unexpected_type = True
     method_name = method.replace("_", " ")
 
     if isinstance(info, (int, float)):
         info = None if info == 0 else str(info)
@@ -228,14 +230,15 @@
         elif method == "instructions":
             if isinstance(info, str):
                 info = info.replace(linesep*2, linesep)
                 unexpected_type = False
             elif isinstance(info, list):
                 info = linesep.join(info)
                 unexpected_type = False
+    info = info if info and contains_alphanumeric.search(info) else None
     if not info or info.isspace() or info == "None":
         log("%s contains nothing", method_name.capitalize())
         return NA
     if unexpected_type:
         log("'%s' has the unhandled type %s", method, type(info))
     return str(info)
```

### Comparing `recipe2txt-0.1.1/recipe2txt/re2txt.py` & `recipe2txt-0.2.0/recipe2txt/re2txt.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.1/recipe2txt/sql.py` & `recipe2txt-0.2.0/recipe2txt/sql.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.1/recipe2txt/utils/ContextLogger.py` & `recipe2txt-0.2.0/recipe2txt/utils/ContextLogger.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,39 +252,40 @@
             self.logger.error(f"Leaving context '{self.msg % self.args}' because of exception {exc_type}: {exc_value}",
                               extra=END_CONTEXT)
         return False
 
 
 def disable_loggers() -> None:
     for logger in logger_list:
+        setattr(logger, "was_disabled", logger.disabled)
         logger.disabled = True
 
 
-def enable_loggers() -> None:
+def reset_disable_loggers() -> None:
     for logger in logger_list:
-        logger.disabled = False
+        logger.disabled = getattr(logger, "was_disabled", False)
 
 
 @contextlib.contextmanager
 def suppress_logging() -> Generator[None, None, None]:
     disable_loggers()
     yield
-    enable_loggers()
+    reset_disable_loggers()
 
 
 class EndContextFilter(logging.Filter):
 
     def filter(self, record: logging.LogRecord) -> bool:
         if record.msg == DO_NOT_LOG:
             return False
         return True
 
 
 def get_file_handler(file: str = LOGFILE, level: int = logging.DEBUG) -> logging.FileHandler:
-    file_handler = RotatingFileHandler(file, mode='w', maxBytes=100000, backupCount=4, encoding="utf-8")
+    file_handler = RotatingFileHandler(file, mode='w', maxBytes=10000000, backupCount=4, encoding="utf-8")
     file_handler.setLevel(level)
     f = EndContextFilter()
     file_handler.addFilter(f)
     file_handler.setFormatter(logging.Formatter(_LOG_FORMAT_FILE, datefmt=DATEFMT))
     file_handler.doRollover()
     return file_handler
```

### Comparing `recipe2txt-0.1.1/recipe2txt/utils/conditional_imports.py` & `recipe2txt-0.2.0/recipe2txt/utils/conditional_imports.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.1/recipe2txt/utils/markdown.py` & `recipe2txt-0.2.0/recipe2txt/utils/markdown.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.1/recipe2txt/utils/misc.py` & `recipe2txt-0.2.0/recipe2txt/utils/misc.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.1/recipe2txt/utils/timer.py` & `recipe2txt-0.2.0/recipe2txt/utils/timer.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.1/recipe2txt/utils/traceback_utils.py` & `recipe2txt-0.2.0/recipe2txt/utils/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.1/recipe2txt.egg-info/PKG-INFO` & `recipe2txt-0.2.0/recipe2txt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recipe2txt
-Version: 0.1.1
+Version: 0.2.0
 Summary: Scrapes recipes and converts them to txt or markdown
 Author-email: Jan Philipp Berg <git.7ksst@aleeas.com>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Homepage, https://github.com/jp-berg/recipe2txt
 Project-URL: Bug Tracker, https://github.com/jp-berg/recipe2txt/issues
 Keywords: recipes,cooking,scraping,website
 Classifier: Programming Language :: Python :: 3
@@ -37,16 +37,20 @@
 
 # WARNING
 
 THIS SOFTWARE IS AT AN EARLY DEVELOPEMENT STAGE.
 
 BE CAREFUL SETTING THE `--output`-FLAG, ANY EXISTING FILES WITH THE SAME NAME WILL BE OVERWRITTEN.
 
+TESTED ONLY ON KUBUNTU 23.04.
+
 # Usage
 
+Install with `pip install recipe2txt`. You can either use `recipe2txt` or `re2txt` to run the program.
+
 ```
 usage: recipes2txt [-h] [-u URL [URL ...]] [-f FILE [FILE ...]] [-o OUTPUT]
                    [-v {debug,info,warning,error,critical}] [-con CONNECTIONS] [-ia] [-c {only,new,default}] [-d]
                    [-t TIMEOUT] [-md] [-sa | -erase | -do DEFAULT_OUTPUT_FILE]
 
 Scrapes URLs of recipes into text files
```

### Comparing `recipe2txt-0.1.1/recipe2txt.egg-info/SOURCES.txt` & `recipe2txt-0.2.0/recipe2txt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.1/test/test_contextlogger.py` & `recipe2txt-0.2.0/test/test_contextlogger.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.1/test/test_fetcher.py` & `recipe2txt-0.2.0/test/test_fetcher.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.1/test/test_helpers.py` & `recipe2txt-0.2.0/test/test_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
 def assertAccessibleFile(testcase: unittest.TestCase, file: Path, not_empty: bool = False) -> None:
     if not file.is_file():
         testcase.fail(f"{file} is not a file")
     with file.open("r") as f:
         if not f.readable():
             testcase.fail(f"{file} is not readable")
-    with file.open("w") as f:
+    with file.open("a") as f:
         if not f.writable():
             testcase.fail(f"{file} is not writable")
     if not_empty and file.stat().st_size == 0:
         testcase.fail(f"{file} is empty")
 
 def assertFilesEqual(testcase: unittest.TestCase, test: Path, validation: Path) -> None:
     with test.open('r') as test_file:
```

### Comparing `recipe2txt-0.1.1/test/test_html2recipe.py` & `recipe2txt-0.2.0/test/test_html2recipe.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,23 @@
     def test__get_info(self):
         for html, url, recipe in zip(file_gen.html_list, file_gen.url_list, file_gen.recipe_list):
             p = recipe_scrapers.scrape_html(html=html, org_url=url)
             for method in h2r.METHODS:
                 with self.subTest(i=url + " | " + method):
                     self.assertEqual(h2r._get_info(method, p, url), getattr(recipe, method))
 
+        bad_info = [("total_time", 0), ("ingredients", None),
+                    ("ingredients", []), ("instructions", [None, None]),
+                    ("instructions", ["", "\t", "\n"]), ("ingredients", "{["),
+                    ("instructions", ["[", " ", "}"])]
+
+        for url, (method, info) in zip(file_gen.url_list, bad_info):
+            with self.subTest(i=f"{method=} {info=}"):
+                self.assertEqual(h2r._get_info(method, info), h2r.NA)
+
     def test_html2recipe(self):
         for url, html, validation in zip(file_gen.url_list, file_gen.html_list, file_gen.recipe_list):
             with self.subTest(i=url):
                 if not (p := h2r.html2parsed(url, html)):
                     self.fail("Failed to parse")
                 if not (recipe := h2r.parsed2recipe(url, p)):
                     self.fail("Failed to convert to recipe")
```

### Comparing `recipe2txt-0.1.1/test/test_misc.py` & `recipe2txt-0.2.0/test/test_misc.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.1/test/test_sql.py` & `recipe2txt-0.2.0/test/test_sql.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.1/test/test_timer.py` & `recipe2txt-0.2.0/test/test_timer.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.1/test/test_traceback_utils.py` & `recipe2txt-0.2.0/test/test_traceback_utils.py`

 * *Files identical despite different names*

