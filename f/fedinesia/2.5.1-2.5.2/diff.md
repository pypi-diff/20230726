# Comparing `tmp/fedinesia-2.5.1.tar.gz` & `tmp/fedinesia-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedinesia-2.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fedinesia-2.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fedinesia-2.5.1.tar` & `fedinesia-2.5.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3481 2023-05-16 02:01:42.571817 fedinesia-2.5.1/README.rst
--rw-r--r--   0        0        0     3716 2023-05-16 02:01:42.571817 fedinesia-2.5.1/pyproject.toml
--rw-r--r--   0        0        0      471 2023-05-16 02:01:42.571817 fedinesia-2.5.1/src/fedinesia/__init__.py
--rw-r--r--   0        0        0    13741 2023-05-16 02:01:42.571817 fedinesia-2.5.1/src/fedinesia/amnesia.py
--rw-r--r--   0        0        0    16703 2023-05-16 02:01:42.571817 fedinesia-2.5.1/src/fedinesia/config.py
--rw-r--r--   0        0        0     9042 2023-05-16 02:01:42.571817 fedinesia-2.5.1/src/fedinesia/util.py
--rw-r--r--   0        0        0     5303 1970-01-01 00:00:00.000000 fedinesia-2.5.1/PKG-INFO
+-rw-r--r--   0        0        0     3481 2023-07-26 10:08:09.924931 fedinesia-2.5.2/README.rst
+-rw-r--r--   0        0        0     3737 2023-07-26 10:08:09.928931 fedinesia-2.5.2/pyproject.toml
+-rw-r--r--   0        0        0      471 2023-07-26 10:08:09.928931 fedinesia-2.5.2/src/fedinesia/__init__.py
+-rw-r--r--   0        0        0    13754 2023-07-26 10:08:09.928931 fedinesia-2.5.2/src/fedinesia/amnesia.py
+-rw-r--r--   0        0        0    16710 2023-07-26 10:08:09.928931 fedinesia-2.5.2/src/fedinesia/config.py
+-rw-r--r--   0        0        0     8962 2023-07-26 10:08:09.928931 fedinesia-2.5.2/src/fedinesia/util.py
+-rw-r--r--   0        0        0     5407 1970-01-01 00:00:00.000000 fedinesia-2.5.2/PKG-INFO
```

### Comparing `fedinesia-2.5.1/README.rst` & `fedinesia-2.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `fedinesia-2.5.1/pyproject.toml` & `fedinesia-2.5.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "fedinesia"
-description = 'Deletes old posts from fediverse accounts. Confirmed working with Mastodon and Pleroma (and Forks)'
+description = 'Deletes old posts from fediverse accounts. Confirmed working with Mastodon, Pleroma (and Forks), and Takahe'
 readme = "README.rst"
 authors = [
   { name = "marvin8", email = "marvin8@tuta.io" },
 ]
 requires-python = ">=3.8"
 license = {text = "AGPL-3.0-or-later"}
 dynamic = ["version"]
@@ -18,39 +18,42 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 
 dependencies = [
-    "rich>=13.3.1",
+    "rich>=13.4.2",
     "outdated>=0.2.2",
-    "tqdm>=4.64.1",
+    "tqdm>=4.65.0",
     "aiofiles>=23.1.0",
-    "minimal-activitypub>=0.5.2",
-    "click>=8.1.3",
-    "aiocsv>=1.2.3",
-    "typing-extensions>=4.5.0",
+    "minimal-activitypub>=0.5.5",
+    "click>=8.1.6",
+    "aiocsv>=1.2.4",
+    "typing-extensions>=4.7.1",
+    "pygments>=2.15.1",
+    "aiohttp>=3.8.5",
+    "certifi>=2023.7.22",
 ]
 [project.optional-dependencies]
 doc = [
-    "Sphinx>=6.1.3",
-    "python-docs-theme>=2022.1",
-    "sphinx-rtd-theme>=1.2.0",
+    "Sphinx>=6.2.1",
+    "python-docs-theme>=2023.5",
+    "sphinx-rtd-theme>=1.2.2",
 ]
 dev = [
-    "pre-commit>=3.0.4",
-    "black>=23.1.0",
-    "mypy>=1.0.0",
+    "pre-commit>=3.3.3",
+    "black>=23.7.0",
+    "mypy>=1.4.1",
     "safety>=2.3.4",
-    "pip-audit>=2.4.14",
-    "types-aiofiles>=22.1.0.8",
+    "pip-audit>=2.6.1",
+    "types-aiofiles>=23.1.0.5",
     "interrogate>=1.5.0",
-    "ruff>=0.0.247",
-    "flit>=3.8.0",
+    "ruff>=0.0.280",
+    "flit>=3.9.0",
 ]
 
 [project.scripts]
 fedinesia = "fedinesia.amnesia:start"
 
 [project.urls]
 Documentation = "https://codeberg.org/MarvinsMastodonTools/fedinesia/src/branch/main/README.rst"
@@ -91,16 +94,14 @@
 strict_equality = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unreachable = true
 warn_unused_configs = true
 no_implicit_reexport = true
 
-[tool.pdm]
-
 [tool.ruff]
 select = ["ARG", "B", "C4", "C90", "D", "E", "ERA", "F", "I", "PL", "RUF", "S", "UP", "W"]
 ignore = ["D203", "D205", "D213"]
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
 fixable = ["A", "B", "C", "D", "E", "F", "I", "UP"]
 unfixable = []
@@ -123,15 +124,14 @@
     "_build",
     "buck-out",
     "build",
     "dist",
     "node_modules",
     "venv",
 ]
-per-file-ignores = {}
 
 # Same as Black.
 line-length = 120
 
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
@@ -141,13 +141,11 @@
 [tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
 
 [tool.ruff.isort]
 force-single-line = true
 
-[tool.ruff.pycodestyle]
-
 [tool.scriv]
 categories = "Breaking, Added, Changed, Deprecated, Removed, Fixed, Security"
 format = "rst"
 version = "literal: src/fedinesia/__init__.py: __version__"
```

### Comparing `fedinesia-2.5.1/src/fedinesia/amnesia.py` & `fedinesia-2.5.2/src/fedinesia/amnesia.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 from .util import should_keep
 
 traceback.install(show_locals=True)
 logger = logging.getLogger(__display_name__)
 logger.setLevel(logging.DEBUG)
 
 
-async def main(  # noqa: max-complexity: 13
+async def main(  # noqa: C901, PLR0912, PLR0913, PLR0915
     config_file: str,
     is_dry_run: bool,
     debug_log_file: Optional[str],
     audit_log_file: Optional[str],
     audit_log_style: Optional[str],
     batch_size: Optional[int],
     limit: Optional[int],
```

### Comparing `fedinesia-2.5.1/src/fedinesia/config.py` & `fedinesia-2.5.2/src/fedinesia/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,17 +60,16 @@
     skip_deleting_poll: Optional[bool]
     skip_deleting_dm: Optional[bool]
     skip_deleting_media: Optional[bool]
     skip_deleting_faved_at_least: Optional[int]
     skip_deleting_boost_at_least: Optional[int]
     skip_deleting_reactions_at_least: Optional[int]
 
-    def __init__(  # noqa: max-complexity: 12
-        self: BC, config: Optional[Dict[str, Any]]
-    ) -> None:
+    def __init__(self: BC, config: Optional[Dict[str, Any]]) -> None:  # noqa: C901
+        """Initialise instance."""
         if not config:
             config = {}
 
         self.log_level = config.get("log_level", "WARN")
 
         std_out_formatter = logging.Formatter(
             "%(name)s[%(process)d] %(levelname)s %(message)s",
```

### Comparing `fedinesia-2.5.1/src/fedinesia/util.py` & `fedinesia-2.5.2/src/fedinesia/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,16 +118,14 @@
 
     async def add_entry(self: AL, status: Status) -> None:
         """Append an entry/status details to the audit log file."""
         if self.style == AuditLog.Style.PLAIN:
             await self._add_plain_entry(status)
         elif self.style == AuditLog.Style.CSV:
             await self._add_csv_entry(status)
-        else:
-            print(f"Unsupported log style passed: {self.style=}")
 
     async def _add_plain_entry(self: AL, status: Status) -> None:
         """Append a plain text entry/status details to the audit log file."""
         entry = (
             f"{arrow.now().format('YYYY-MM-DD hh:mm:ss')} -"
             f" Removed {'poll' if status.get('poll', False) else 'status'} {status.get('url')}"
             f" created @ {status.get('created_at')}"
```

### Comparing `fedinesia-2.5.1/PKG-INFO` & `fedinesia-2.5.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 Metadata-Version: 2.1
 Name: fedinesia
-Version: 2.5.1
-Summary: Deletes old posts from fediverse accounts. Confirmed working with Mastodon and Pleroma (and Forks)
+Version: 2.5.2
+Summary: Deletes old posts from fediverse accounts. Confirmed working with Mastodon, Pleroma (and Forks), and Takahe
 Author-email: marvin8 <marvin8@tuta.io>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: rich>=13.3.1
+Requires-Dist: rich>=13.4.2
 Requires-Dist: outdated>=0.2.2
-Requires-Dist: tqdm>=4.64.1
+Requires-Dist: tqdm>=4.65.0
 Requires-Dist: aiofiles>=23.1.0
-Requires-Dist: minimal-activitypub>=0.5.2
-Requires-Dist: click>=8.1.3
-Requires-Dist: aiocsv>=1.2.3
-Requires-Dist: typing-extensions>=4.5.0
-Requires-Dist: pre-commit>=3.0.4 ; extra == "dev"
-Requires-Dist: black>=23.1.0 ; extra == "dev"
-Requires-Dist: mypy>=1.0.0 ; extra == "dev"
+Requires-Dist: minimal-activitypub>=0.5.5
+Requires-Dist: click>=8.1.6
+Requires-Dist: aiocsv>=1.2.4
+Requires-Dist: typing-extensions>=4.7.1
+Requires-Dist: pygments>=2.15.1
+Requires-Dist: aiohttp>=3.8.5
+Requires-Dist: certifi>=2023.7.22
+Requires-Dist: pre-commit>=3.3.3 ; extra == "dev"
+Requires-Dist: black>=23.7.0 ; extra == "dev"
+Requires-Dist: mypy>=1.4.1 ; extra == "dev"
 Requires-Dist: safety>=2.3.4 ; extra == "dev"
-Requires-Dist: pip-audit>=2.4.14 ; extra == "dev"
-Requires-Dist: types-aiofiles>=22.1.0.8 ; extra == "dev"
+Requires-Dist: pip-audit>=2.6.1 ; extra == "dev"
+Requires-Dist: types-aiofiles>=23.1.0.5 ; extra == "dev"
 Requires-Dist: interrogate>=1.5.0 ; extra == "dev"
-Requires-Dist: ruff>=0.0.247 ; extra == "dev"
-Requires-Dist: flit>=3.8.0 ; extra == "dev"
-Requires-Dist: Sphinx>=6.1.3 ; extra == "doc"
-Requires-Dist: python-docs-theme>=2022.1 ; extra == "doc"
-Requires-Dist: sphinx-rtd-theme>=1.2.0 ; extra == "doc"
+Requires-Dist: ruff>=0.0.280 ; extra == "dev"
+Requires-Dist: flit>=3.9.0 ; extra == "dev"
+Requires-Dist: Sphinx>=6.2.1 ; extra == "doc"
+Requires-Dist: python-docs-theme>=2023.5 ; extra == "doc"
+Requires-Dist: sphinx-rtd-theme>=1.2.2 ; extra == "doc"
 Project-URL: Changelog, https://codeberg.org/MarvinsMastodonTools/fedinesia/src/branch/main/CHANGELOG.rst
 Project-URL: Documentation, https://codeberg.org/MarvinsMastodonTools/fedinesia/src/branch/main/README.rst
 Project-URL: Issues, https://codeberg.org/MarvinsMastodonTools/fedinesia/issues
 Project-URL: Source, https://codeberg.org/MarvinsMastodonTools/fedinesia
 Provides-Extra: dev
 Provides-Extra: doc
```

