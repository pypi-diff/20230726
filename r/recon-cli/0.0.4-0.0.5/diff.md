# Comparing `tmp/recon_cli-0.0.4.tar.gz` & `tmp/recon_cli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recon_cli-0.0.4.tar", last modified: Fri May 19 15:27:15 2023, max compression
+gzip compressed data, was "recon_cli-0.0.5.tar", last modified: Wed Jul 26 19:11:28 2023, max compression
```

## Comparing `recon_cli-0.0.4.tar` & `recon_cli-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0       51 2023-05-19 15:27:15.000000 recon_cli-0.0.4/.flake8
--rw-r--r--   0        0        0      231 2023-05-19 15:27:15.000000 recon_cli-0.0.4/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0      655 2023-05-19 15:27:15.000000 recon_cli-0.0.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0      625 2023-05-19 15:27:15.000000 recon_cli-0.0.4/.github/workflows/tox.yml
--rw-r--r--   0        0        0      948 2023-05-19 15:27:15.000000 recon_cli-0.0.4/.gitignore
--rw-r--r--   0        0        0      563 2023-05-19 15:27:15.000000 recon_cli-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1069 2023-05-19 15:27:15.000000 recon_cli-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0     7231 2023-05-19 15:27:15.000000 recon_cli-0.0.4/README.md
--rw-r--r--   0        0        0      970 2023-05-19 15:27:15.000000 recon_cli-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       93 2023-05-19 15:27:15.000000 recon_cli-0.0.4/recon/__init__.py
--rw-r--r--   0        0        0       35 2023-05-19 15:27:15.000000 recon_cli-0.0.4/recon/__main__.py
--rw-r--r--   0        0        0     4283 2023-05-19 15:27:15.000000 recon_cli-0.0.4/recon/main.py
--rw-r--r--   0        0        0    10351 2023-05-19 15:27:15.000000 recon_cli-0.0.4/recon/reconcile.py
--rw-r--r--   0        0        0      364 2023-05-19 15:27:15.000000 recon_cli-0.0.4/recon/utils.py
--rw-r--r--   0        0        0     1058 2023-05-19 15:27:15.000000 recon_cli-0.0.4/requirements.txt
--rw-r--r--   0        0        0        0 2023-05-19 15:27:15.000000 recon_cli-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     3113 2023-05-19 15:27:15.000000 recon_cli-0.0.4/tests/test_main.py
--rw-r--r--   0        0        0      374 2023-05-19 15:27:15.000000 recon_cli-0.0.4/tox.ini
--rw-r--r--   0        0        0     8042 1970-01-01 00:00:00.000000 recon_cli-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       51 2023-07-26 19:11:28.000000 recon_cli-0.0.5/.flake8
+-rw-r--r--   0        0        0      834 2023-07-26 19:11:28.000000 recon_cli-0.0.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2023-07-26 19:11:28.000000 recon_cli-0.0.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      231 2023-07-26 19:11:28.000000 recon_cli-0.0.5/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0      655 2023-07-26 19:11:28.000000 recon_cli-0.0.5/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      625 2023-07-26 19:11:28.000000 recon_cli-0.0.5/.github/workflows/tox.yml
+-rw-r--r--   0        0        0      948 2023-07-26 19:11:28.000000 recon_cli-0.0.5/.gitignore
+-rw-r--r--   0        0        0      563 2023-07-26 19:11:28.000000 recon_cli-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1069 2023-07-26 19:11:28.000000 recon_cli-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     7141 2023-07-26 19:11:28.000000 recon_cli-0.0.5/README.md
+-rw-r--r--   0        0        0      970 2023-07-26 19:11:28.000000 recon_cli-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0       93 2023-07-26 19:11:28.000000 recon_cli-0.0.5/recon/__init__.py
+-rw-r--r--   0        0        0       35 2023-07-26 19:11:28.000000 recon_cli-0.0.5/recon/__main__.py
+-rw-r--r--   0        0        0     4283 2023-07-26 19:11:28.000000 recon_cli-0.0.5/recon/main.py
+-rw-r--r--   0        0        0    12305 2023-07-26 19:11:28.000000 recon_cli-0.0.5/recon/reconcile.py
+-rw-r--r--   0        0        0      364 2023-07-26 19:11:28.000000 recon_cli-0.0.5/recon/utils.py
+-rw-r--r--   0        0        0     1058 2023-07-26 19:11:28.000000 recon_cli-0.0.5/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-26 19:11:28.000000 recon_cli-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     5327 2023-07-26 19:11:28.000000 recon_cli-0.0.5/tests/test_reconcile.py
+-rw-r--r--   0        0        0      374 2023-07-26 19:11:28.000000 recon_cli-0.0.5/tox.ini
+-rw-r--r--   0        0        0     7952 1970-01-01 00:00:00.000000 recon_cli-0.0.5/PKG-INFO
```

### Comparing `recon_cli-0.0.4/.github/workflows/publish.yml` & `recon_cli-0.0.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `recon_cli-0.0.4/.github/workflows/tox.yml` & `recon_cli-0.0.5/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `recon_cli-0.0.4/.gitignore` & `recon_cli-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `recon_cli-0.0.4/.pre-commit-config.yaml` & `recon_cli-0.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `recon_cli-0.0.4/LICENSE.txt` & `recon_cli-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `recon_cli-0.0.4/README.md` & `recon_cli-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,34 +28,34 @@
 ## Usage
 
 ### CLI
 
 ```plaintext
  Usage: recon [OPTIONS] LEFT RIGHT LEFT_ON RIGHT_ON
 
-╭─ Arguments ──────────────────────────────────────────────────────────────────────────────────────────╮
-│ *    left          FILE  Path to the left dataset. [required]                                        │
-│ *    right         FILE  Path to the right dataset. [required]                                       │
-│ *    left_on       TEXT  Reconcile using this field from the left dataset. [required]                │
-│ *    right_on      TEXT  Reconcile using this field from the right dataset. [required]               │
-╰──────────────────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────╮
-│ --help          Show this message and exit.                                                          │
-╰──────────────────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Input options ──────────────────────────────────────────────────────────────────────────────────────╮
-│ --left-suffix         TEXT  Suffix to append to the left dataset's column names. [default: _left]    │
-│ --right-suffix        TEXT  Suffix to append to the right dataset's column names. [default: _right]  │
-│ --left-sheet          TEXT  Sheet to read from left if left is a spreadsheet. [default: Sheet1]      │
-│ --right-sheet         TEXT  Sheet to read from left if left is a spreadsheet. [default: Sheet1]      │
-╰──────────────────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Output options ─────────────────────────────────────────────────────────────────────────────────────╮
-│ --output-file                      TEXT  Path to save results (in xlsx format) to.                   │
-│ --std-out        --no-std-out            Print results to stdout. [default: no-std-out]              │
-│ --info-only      --no-info-only          Print summary results only. [default: no-info-only]         │
-╰──────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Arguments ──────────────────────────────────────────────────────────────────────────────────────╮
+│ *    left          FILE  Path to the left dataset. [required]                                    │
+│ *    right         FILE  Path to the right dataset. [required]                                   │
+│ *    left_on       TEXT  Reconcile using this field from the left dataset. [required]            │
+│ *    right_on      TEXT  Reconcile using this field from the right dataset. [required]           │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
+│ --help          Show this message and exit.                                                      │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Input options ──────────────────────────────────────────────────────────────────────────────────╮
+│ --left-suffix     TEXT  Suffix to append to the left dataset's column names. [default: _left]    │
+│ --right-suffix    TEXT  Suffix to append to the right dataset's column names. [default: _right]  │
+│ --left-sheet      TEXT  Sheet to read from left if left is a spreadsheet. [default: Sheet1]      │
+│ --right-sheet     TEXT  Sheet to read from left if left is a spreadsheet. [default: Sheet1]      │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Output options ─────────────────────────────────────────────────────────────────────────────────╮
+│ --output-file                  TEXT  Path to save results (in xlsx format) to.                   │
+│ --std-out        --no-std-out          Print results to stdout. [default: no-std-out]            │
+│ --info-only      --no-info-only        Print summary results only. [default: no-info-only]       │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
 ### Python
 
 ```python
 # Recon import
 from recon import Reconcile
@@ -102,14 +102,15 @@
 
 # Output methods:
 # `recon_components` parameter is an ordered list of any of the DataFrame property names.
 # "all" is a shorthand for most properties.
 recon.info()  # Prints a summary of recon results
 recon.to_stdout(recon_components=["all"]) # Prints all recon results to console
 recon.to_xlsx(path="recon_results.xlsx", recon_components=["all"]) # Saves all recon results to xlsx
+recon.to_object() # returns a ReconciledReport object
 ```
 
 ## Dependencies
 
 - [pandas](https://pandas.pydata.org/pandas-docs/stable/getting_started/install.html#required-dependencies) with [performance](https://pandas.pydata.org/pandas-docs/stable/getting_started/install.html#performance-dependencies-recommended) and [excel](https://pandas.pydata.org/pandas-docs/stable/getting_started/install.html#excel-files) optional dependencies to perform the reconciliation.
 - [Typer](https://typer.tiangolo.com/) powers the command line interface.
```

### Comparing `recon_cli-0.0.4/pyproject.toml` & `recon_cli-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "recon-cli"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Mynhardt Burger", email="mynhardt+recon@gmail.com" },
 ]
 description = "Simple command line tool to reconcile datasets"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `recon_cli-0.0.4/recon/main.py` & `recon_cli-0.0.5/recon/main.py`

 * *Files identical despite different names*

### Comparing `recon_cli-0.0.4/recon/reconcile.py` & `recon_cli-0.0.5/recon/reconcile.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 import sys
+from dataclasses import dataclass
 from enum import Enum
 from functools import cached_property
 from os import PathLike
-from pathlib import PurePath
 from textwrap import dedent
-from typing import Any, Literal, Union
+from typing import Any, Literal, Optional, Union
 
 import pandas as pd
 
 from recon.utils import ensure_df
 
 FilePath = Union[str, "PathLike[str]"]
 Suffixes = Union[
@@ -33,20 +33,58 @@
 
 
 Relationship = Enum(
     "Relationship", ["ONE_TO_ONE", "ONE_TO_MANY", "MANY_TO_ONE", "MANY_TO_MANY", "NONE"]
 )
 
 
+@dataclass
+class ReconciledData:
+    both: pd.DataFrame
+    left_duplicate: pd.DataFrame
+    right_duplicate: pd.DataFrame
+    left_only: pd.DataFrame
+    right_only: pd.DataFrame
+
+
+@dataclass
+class ReconciledArgs:
+    left_on: str
+    right_on: str
+    left_suffix: Optional[str] = None
+    right_suffix: Optional[str] = None
+    left_sheet_name: Optional[str] = None
+    right_sheet_name: Optional[str] = None
+
+
+@dataclass
+class ReconciledStats:
+    rows: int = 0
+    both_rows: int = 0
+    unique_rows: int = 0
+    duplicated_rows: int = 0
+
+
+@dataclass
+class ReconciledReport:
+    data: ReconciledData
+    args: ReconciledArgs
+    relationship: Relationship
+    left_stats: ReconciledStats
+    right_stats: ReconciledStats
+
+
 class Reconcile:
     def __init__(self) -> None:
         self.left: pd.DataFrame
         self.right: pd.DataFrame
         self.left_on: str
         self.right_on: str
+        self.left_sheet_name: Optional[str] = None
+        self.right_sheet_name: Optional[str] = None
 
         self.suffixes: tuple[str, str]
 
         self._output_dispatch = [
             "left_only",
             "right_only",
             "left_duplicate",
@@ -214,14 +252,46 @@
         Left: {left_stats}
         Right: {right_stats}
         Relationship: {self.relationship} ({self.left_on}:{self.right_on})
         """
         )
         print(report)
 
+    def to_object(self) -> ReconciledReport:
+        return ReconciledReport(
+            data=ReconciledData(
+                both=self.both,
+                left_duplicate=self.left_duplicate,
+                right_duplicate=self.right_duplicate,
+                left_only=self.left_only,
+                right_only=self.right_only,
+            ),
+            args=ReconciledArgs(
+                left_on=self.left_on,
+                right_on=self.right_on,
+                left_suffix=self.suffixes[0],
+                right_suffix=self.suffixes[1],
+                left_sheet_name=self.left_sheet_name,
+                right_sheet_name=self.right_sheet_name,
+            ),
+            relationship=self.relationship,
+            left_stats=ReconciledStats(
+                rows=len(self.left),
+                both_rows=len(self.left_both),
+                unique_rows=len(self.left_only),
+                duplicated_rows=len(self.left_duplicate),
+            ),
+            right_stats=ReconciledStats(
+                rows=len(self.right),
+                both_rows=len(self.right_both),
+                unique_rows=len(self.right_only),
+                duplicated_rows=len(self.right_duplicate),
+            ),
+        )
+
     def to_xlsx(
         self,
         path: FilePath,
         recon_components: list[RECON_COMPONENTS] = ["all"],
         **kwargs,
     ) -> None:
         if recon_components == ["all"]:
@@ -246,26 +316,27 @@
         print("--------- START ----------")
         for component in write_list:
             print(f"--------- {component} ----------")
             getattr(self, component).to_csv(sys.stdout, index_label="index", **kwargs)
         print("--------- END ----------")
 
     @staticmethod
-    def _read_file(
-        data: FilePath,
+    def _read_obj(
+        data: Any,
         sheet_name: str = "Sheet1",
         **kwargs,
     ):
-        file_path = PurePath(data)
-        if file_path.suffix.lower() in {".xlsx", ".xls", ".xlsm", ".xlsb"}:
-            if not isinstance(sheet_name, (str, int)):
-                raise ValueError("Importing of multiple sheets is not supported")
-            return pd.read_excel(file_path, sheet_name, **kwargs)
+        try:
+            excel_file = pd.ExcelFile(data)
+        except Exception:
+            pass
         else:
-            return pd.read_csv(file_path, **kwargs)
+            return pd.read_excel(excel_file, sheet_name, **kwargs)
+
+        return pd.read_csv(data, **kwargs)
 
     @staticmethod
     def _load_df(
         recon_obj: "Reconcile",
         left_df: pd.DataFrame,
         right_df: pd.DataFrame,
         left_on: str,
@@ -301,23 +372,25 @@
         suffixes: tuple[str, str] = ("_left", "_right"),
         left_kwargs: dict[str, Any] = {},
         right_kwargs: dict[str, Any] = {},
     ):
         """
         Returns a :class:`Reconcile` object populated with data which can be queried.
 
-        Excel files are identified by their extension. All other extensions
-        are assumed to be csv. :param:`left_kwargs` and :param:`right_kwargs` are
+        :param:`left_kwargs` and :param:`right_kwargs` are
         passed onto the `pandas.read_excel()` and `pandas.read_csv()` methods.
         """
+        recon = Reconcile()
 
-        left_df = Reconcile._read_file(left_file, **left_kwargs)
-        right_df = Reconcile._read_file(right_file, **right_kwargs)
+        left_df = Reconcile._read_obj(left_file, **left_kwargs)
+        recon.left_sheet_name = left_kwargs.get("sheet_name", None)
+
+        right_df = Reconcile._read_obj(right_file, **right_kwargs)
+        recon.right_sheet_name = right_kwargs.get("sheet_name", None)
 
-        recon = Reconcile()
         recon = Reconcile._load_df(
             recon, left_df, right_df, left_on, right_on, suffixes
         )
 
         return recon
 
     @staticmethod
```

### Comparing `recon_cli-0.0.4/requirements.txt` & `recon_cli-0.0.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `recon_cli-0.0.4/PKG-INFO` & `recon_cli-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recon-cli
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple command line tool to reconcile datasets
 Author-email: Mynhardt Burger <mynhardt+recon@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -49,34 +49,34 @@
 ## Usage
 
 ### CLI
 
 ```plaintext
  Usage: recon [OPTIONS] LEFT RIGHT LEFT_ON RIGHT_ON
 
-╭─ Arguments ──────────────────────────────────────────────────────────────────────────────────────────╮
-│ *    left          FILE  Path to the left dataset. [required]                                        │
-│ *    right         FILE  Path to the right dataset. [required]                                       │
-│ *    left_on       TEXT  Reconcile using this field from the left dataset. [required]                │
-│ *    right_on      TEXT  Reconcile using this field from the right dataset. [required]               │
-╰──────────────────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────╮
-│ --help          Show this message and exit.                                                          │
-╰──────────────────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Input options ──────────────────────────────────────────────────────────────────────────────────────╮
-│ --left-suffix         TEXT  Suffix to append to the left dataset's column names. [default: _left]    │
-│ --right-suffix        TEXT  Suffix to append to the right dataset's column names. [default: _right]  │
-│ --left-sheet          TEXT  Sheet to read from left if left is a spreadsheet. [default: Sheet1]      │
-│ --right-sheet         TEXT  Sheet to read from left if left is a spreadsheet. [default: Sheet1]      │
-╰──────────────────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Output options ─────────────────────────────────────────────────────────────────────────────────────╮
-│ --output-file                      TEXT  Path to save results (in xlsx format) to.                   │
-│ --std-out        --no-std-out            Print results to stdout. [default: no-std-out]              │
-│ --info-only      --no-info-only          Print summary results only. [default: no-info-only]         │
-╰──────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Arguments ──────────────────────────────────────────────────────────────────────────────────────╮
+│ *    left          FILE  Path to the left dataset. [required]                                    │
+│ *    right         FILE  Path to the right dataset. [required]                                   │
+│ *    left_on       TEXT  Reconcile using this field from the left dataset. [required]            │
+│ *    right_on      TEXT  Reconcile using this field from the right dataset. [required]           │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
+│ --help          Show this message and exit.                                                      │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Input options ──────────────────────────────────────────────────────────────────────────────────╮
+│ --left-suffix     TEXT  Suffix to append to the left dataset's column names. [default: _left]    │
+│ --right-suffix    TEXT  Suffix to append to the right dataset's column names. [default: _right]  │
+│ --left-sheet      TEXT  Sheet to read from left if left is a spreadsheet. [default: Sheet1]      │
+│ --right-sheet     TEXT  Sheet to read from left if left is a spreadsheet. [default: Sheet1]      │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Output options ─────────────────────────────────────────────────────────────────────────────────╮
+│ --output-file                  TEXT  Path to save results (in xlsx format) to.                   │
+│ --std-out        --no-std-out          Print results to stdout. [default: no-std-out]            │
+│ --info-only      --no-info-only        Print summary results only. [default: no-info-only]       │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
 ### Python
 
 ```python
 # Recon import
 from recon import Reconcile
@@ -123,14 +123,15 @@
 
 # Output methods:
 # `recon_components` parameter is an ordered list of any of the DataFrame property names.
 # "all" is a shorthand for most properties.
 recon.info()  # Prints a summary of recon results
 recon.to_stdout(recon_components=["all"]) # Prints all recon results to console
 recon.to_xlsx(path="recon_results.xlsx", recon_components=["all"]) # Saves all recon results to xlsx
+recon.to_object() # returns a ReconciledReport object
 ```
 
 ## Dependencies
 
 - [pandas](https://pandas.pydata.org/pandas-docs/stable/getting_started/install.html#required-dependencies) with [performance](https://pandas.pydata.org/pandas-docs/stable/getting_started/install.html#performance-dependencies-recommended) and [excel](https://pandas.pydata.org/pandas-docs/stable/getting_started/install.html#excel-files) optional dependencies to perform the reconciliation.
 - [Typer](https://typer.tiangolo.com/) powers the command line interface.
```

