# Comparing `tmp/sync_pre_commit_lock-0.1.2.tar.gz` & `tmp/sync_pre_commit_lock-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sync_pre_commit_lock-0.1.2.tar", last modified: Mon Jul  3 19:56:02 2023, max compression
+gzip compressed data, was "sync_pre_commit_lock-0.2.0.tar", last modified: Wed Jul 26 20:02:31 2023, max compression
```

## Comparing `sync_pre_commit_lock-0.1.2.tar` & `sync_pre_commit_lock-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,33 @@
--rw-r--r--   0        0        0    35149 2023-07-03 19:55:47.710878 sync_pre_commit_lock-0.1.2/LICENSE
--rw-r--r--   0        0        0     4951 2023-07-03 19:55:47.710878 sync_pre_commit_lock-0.1.2/README.md
--rw-r--r--   0        0        0     2917 2023-07-03 19:56:02.874856 sync_pre_commit_lock-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      778 2023-07-03 19:55:47.710878 sync_pre_commit_lock-0.1.2/src/sync_pre_commit_lock/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 19:55:47.710878 sync_pre_commit_lock-0.1.2/src/sync_pre_commit_lock/actions/__init__.py
--rw-r--r--   0        0        0     3199 2023-07-03 19:55:47.710878 sync_pre_commit_lock-0.1.2/src/sync_pre_commit_lock/actions/install_hooks.py
--rw-r--r--   0        0        0     8336 2023-07-03 19:55:47.710878 sync_pre_commit_lock-0.1.2/src/sync_pre_commit_lock/actions/sync_hooks.py
--rw-r--r--   0        0        0     2039 2023-07-03 19:55:47.710878 sync_pre_commit_lock-0.1.2/src/sync_pre_commit_lock/config.py
--rw-r--r--   0        0        0     1694 2023-07-03 19:55:47.710878 sync_pre_commit_lock-0.1.2/src/sync_pre_commit_lock/db.py
--rw-r--r--   0        0        0     3933 2023-07-03 19:55:47.710878 sync_pre_commit_lock-0.1.2/src/sync_pre_commit_lock/pdm_plugin.py
--rw-r--r--   0        0        0     4310 2023-07-03 19:55:47.710878 sync_pre_commit_lock-0.1.2/src/sync_pre_commit_lock/poetry_plugin.py
--rw-r--r--   0        0        0       93 2023-07-03 19:55:47.710878 sync_pre_commit_lock-0.1.2/src/sync_pre_commit_lock/py.typed
--rw-r--r--   0        0        0     1172 2023-07-03 19:55:47.710878 sync_pre_commit_lock-0.1.2/src/sync_pre_commit_lock/utils.py
--rw-r--r--   0        0        0       39 2023-07-03 19:55:47.710878 sync_pre_commit_lock-0.1.2/tests/conftest.py
--rw-r--r--   0        0        0      405 2023-07-03 19:55:47.710878 sync_pre_commit_lock-0.1.2/tests/fixtures/poetry_project/.pre-commit-config.yaml
--rw-r--r--   0        0        0     8012 2023-07-03 19:55:47.710878 sync_pre_commit_lock-0.1.2/tests/fixtures/poetry_project/poetry.lock
--rw-r--r--   0        0        0      412 2023-07-03 19:55:47.710878 sync_pre_commit_lock-0.1.2/tests/fixtures/poetry_project/pyproject.toml
--rw-r--r--   0        0        0     6401 2023-07-03 19:55:47.710878 sync_pre_commit_lock-0.1.2/tests/test_actions/test_install_hooks.py
--rw-r--r--   0        0        0     5997 2023-07-03 19:55:47.710878 sync_pre_commit_lock-0.1.2/tests/test_actions/test_pre_commit_config_file.py
--rw-r--r--   0        0        0    13297 2023-07-03 19:55:47.710878 sync_pre_commit_lock-0.1.2/tests/test_actions/test_sync_hooks.py
--rw-r--r--   0        0        0     2736 2023-07-03 19:55:47.710878 sync_pre_commit_lock-0.1.2/tests/test_config.py
--rw-r--r--   0        0        0      273 2023-07-03 19:55:47.710878 sync_pre_commit_lock-0.1.2/tests/test_db.py
--rw-r--r--   0        0        0     3225 2023-07-03 19:55:47.710878 sync_pre_commit_lock-0.1.2/tests/test_pdm/test_pdm_plugin.py
--rw-r--r--   0        0        0     2093 2023-07-03 19:55:47.710878 sync_pre_commit_lock-0.1.2/tests/test_pdm/test_pdm_sync_pre_commit_hook.py
--rw-r--r--   0        0        0     3192 2023-07-03 19:55:47.710878 sync_pre_commit_lock-0.1.2/tests/test_poetry/test_poetry_plugin.py
--rw-r--r--   0        0        0     1323 2023-07-03 19:55:47.710878 sync_pre_commit_lock-0.1.2/tests/test_utils.py
--rw-r--r--   0        0        0    46792 1970-01-01 00:00:00.000000 sync_pre_commit_lock-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-26 20:02:16.730483 sync_pre_commit_lock-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5034 2023-07-26 20:02:16.730483 sync_pre_commit_lock-0.2.0/README.md
+-rw-r--r--   0        0        0     3020 2023-07-26 20:02:31.614621 sync_pre_commit_lock-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      778 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/actions/__init__.py
+-rw-r--r--   0        0        0     3232 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/actions/install_hooks.py
+-rw-r--r--   0        0        0     5427 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/actions/sync_hooks.py
+-rw-r--r--   0        0        0     2039 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/config.py
+-rw-r--r--   0        0        0     1694 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/db.py
+-rw-r--r--   0        0        0     3933 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/pdm_plugin.py
+-rw-r--r--   0        0        0     4310 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/poetry_plugin.py
+-rw-r--r--   0        0        0     4054 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/pre_commit_config.py
+-rw-r--r--   0        0        0       93 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/py.typed
+-rw-r--r--   0        0        0     1172 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/utils.py
+-rw-r--r--   0        0        0       39 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0      405 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/fixtures/poetry_project/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     8012 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/fixtures/poetry_project/poetry.lock
+-rw-r--r--   0        0        0      412 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/fixtures/poetry_project/pyproject.toml
+-rw-r--r--   0        0        0      687 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/fixtures/sample_pre_commit_config/pre-commit-config-document-separator.yaml
+-rw-r--r--   0        0        0      696 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/fixtures/sample_pre_commit_config/pre-commit-config-start-empty-lines.yaml
+-rw-r--r--   0        0        0      493 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/fixtures/sample_pre_commit_config/pre-commit-config-with-local.yaml
+-rw-r--r--   0        0        0      661 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/fixtures/sample_pre_commit_config/pre-commit-config.yaml
+-rw-r--r--   0        0        0     1116 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/fixtures/sample_pre_commit_config/sample-django-stubs.yaml
+-rw-r--r--   0        0        0     6401 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/test_actions/test_install_hooks.py
+-rw-r--r--   0        0        0    13332 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/test_actions/test_sync_hooks.py
+-rw-r--r--   0        0        0     2627 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/test_config.py
+-rw-r--r--   0        0        0      273 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/test_db.py
+-rw-r--r--   0        0        0     3225 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/test_pdm/test_pdm_plugin.py
+-rw-r--r--   0        0        0     2093 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/test_pdm/test_pdm_sync_pre_commit_hook.py
+-rw-r--r--   0        0        0     3192 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/test_poetry/test_poetry_plugin.py
+-rw-r--r--   0        0        0     3071 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/test_pre_commit_config_file.py
+-rw-r--r--   0        0        0     1323 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/test_utils.py
+-rw-r--r--   0        0        0    46881 1970-01-01 00:00:00.000000 sync_pre_commit_lock-0.2.0/PKG-INFO
```

### Comparing `sync_pre_commit_lock-0.1.2/LICENSE` & `sync_pre_commit_lock-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.1.2/README.md` & `sync_pre_commit_lock-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,16 @@
 - [ ] Add a dedicated CLI command to manage sync/install
 - [ ] Expose a pre-commit hook to sync the lockfile
 - [ ] Support nested params for some repos? Like mypy types
 - [ ] Support reading DB from a Python module?
 - [ ] Support reordering DB inputs (file/global config/python module/cli)?
 - [ ] Test using SSH/file dependencies?
 - [ ] Check ref existence before writing?
-- [ ] Support multiple hooks repos for the same dependency?
+- [ ] Support multiple hooks repos for the same dependency? E.g. ruff new and old repo
 - [ ] New feature to convert from pre-commit online to local?
+- [ ] Warning if pre-commit CI auto update is also set?
 
 ## Inspiration
 
 This project is inspired by @floatingpurr's [sync_with_pdm](https://github.com/floatingpurr/sync_with_pdm/) and [sync_with_poetry](https://github.com/floatingpurr/sync_with_poetry/).
 
 The code to install pre-commit hooks automatically is **adapted** from @vstrimaitis's [poetry-pre-commit-plugin](https://github.com/vstrimaitis/poetry-pre-commit-plugin/), licensed under GPL-3.
```

### Comparing `sync_pre_commit_lock-0.1.2/pyproject.toml` & `sync_pre_commit_lock-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "sync-pre-commit-lock"
-version = "0.1.2"
+version = "0.2.0"
 description = "PDM plugin to sync your pre-commit versions with your lockfile, and install them, all automatically."
 authors = [
     { name = "Gabriel Dugny", email = "sync-pre-commit-lock@dugny.me" },
 ]
 dependencies = [
-    "PyYAML>=6.0",
     "tomli>=2.0.0; python_version < \"3.11\"",
+    "strictyaml>=1.7.3",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -55,14 +55,15 @@
 [tool.pdm]
 plugins = [
     "-e .",
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
+    "PyYAML>=6.0",
     "black>=23.3.0",
     "mypy>=1.4.1",
     "ruff>=0.0.275",
     "types-PyYAML>=6.0.12.10",
     "pytest>=7.4.0",
     "pytest-mock>=3.11.1",
     "pytest-cov>=4.1.0",
@@ -84,14 +85,17 @@
 extend-ignore = [
     "S101",
 ]
 target-version = "py310"
 
 [tool.mypy]
 strict = true
+overrides = [
+    { module = "strictyaml", ignore_missing_imports = true },
+]
 
 [tool.black]
 line-length = 120
 target-version = [
     "py310",
 ]
```

### Comparing `sync_pre_commit_lock-0.1.2/src/sync_pre_commit_lock/__init__.py` & `sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/__init__.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.1.2/src/sync_pre_commit_lock/actions/install_hooks.py` & `sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/actions/install_hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     def _is_pre_commit_package_installed(self) -> bool:
         try:
             # Try is `pre-commit --version` works
             output = subprocess.check_output(
                 self.check_pre_commit_version_command,  # noqa: S603
             ).decode()
             return "pre-commit" in output
-        except FileNotFoundError:
+        except (subprocess.CalledProcessError, FileNotFoundError):
             return False
 
     @staticmethod
     def _are_pre_commit_hooks_installed(git_root: Path) -> bool:
         return (git_root / "hooks" / "pre-commit").exists()
 
     @staticmethod
```

### Comparing `sync_pre_commit_lock-0.1.2/src/sync_pre_commit_lock/config.py` & `sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/config.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.1.2/src/sync_pre_commit_lock/db.py` & `sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/db.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.1.2/src/sync_pre_commit_lock/pdm_plugin.py` & `sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/pdm_plugin.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.1.2/src/sync_pre_commit_lock/poetry_plugin.py` & `sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/poetry_plugin.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.1.2/src/sync_pre_commit_lock/utils.py` & `sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/utils.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.1.2/tests/fixtures/poetry_project/poetry.lock` & `sync_pre_commit_lock-0.2.0/tests/fixtures/poetry_project/poetry.lock`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.1.2/tests/test_actions/test_install_hooks.py` & `sync_pre_commit_lock-0.2.0/tests/test_actions/test_install_hooks.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.1.2/tests/test_actions/test_sync_hooks.py` & `sync_pre_commit_lock-0.2.0/tests/test_actions/test_sync_hooks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from pathlib import Path
 from unittest.mock import MagicMock, patch
 
 from sync_pre_commit_lock import Printer
 from sync_pre_commit_lock.actions.sync_hooks import (
     GenericLockedPackage,
-    PreCommitHookConfig,
-    PreCommitRepo,
     SyncPreCommitHooksVersion,
 )
 from sync_pre_commit_lock.config import SyncPreCommitLockConfig
 from sync_pre_commit_lock.db import PackageRepoMapping, RepoInfo
+from sync_pre_commit_lock.pre_commit_config import PreCommitHookConfig, PreCommitRepo
 
 
 def test_execute_returns_early_when_disabled() -> None:
     printer = MagicMock(spec=Printer)
     pre_commit_config_file_path = MagicMock(spec=Path)
     locked_packages: dict[str, GenericLockedPackage] = {}
     plugin_config: SyncPreCommitLockConfig = MagicMock(spec=SyncPreCommitLockConfig)
@@ -46,15 +45,15 @@
         plugin_config=plugin_config,
         dry_run=dry_run,
     )
     syncer.execute()
     printer.debug.assert_called_once_with("Dry run, skipping pre-commit hook check")
 
 
-@patch("sync_pre_commit_lock.actions.sync_hooks.PreCommitHookConfig.from_yaml_file", side_effect=FileNotFoundError())
+@patch("sync_pre_commit_lock.pre_commit_config.PreCommitHookConfig.from_yaml_file", side_effect=FileNotFoundError())
 def test_execute_handles_file_not_found(mock_from_yaml_file: MagicMock) -> None:
     printer = MagicMock(spec=Printer)
     pre_commit_config_file_path = MagicMock(spec=Path)
     locked_packages: dict[str, GenericLockedPackage] = {}
     plugin_config = MagicMock(spec=SyncPreCommitLockConfig)
     plugin_config.disable_sync_from_lock = False
     dry_run = False
@@ -68,15 +67,15 @@
     )
     syncer.execute()
     printer.info.assert_called_once_with(
         f"No pre-commit config file detected at {pre_commit_config_file_path}, skipping sync."
     )
 
 
-@patch("sync_pre_commit_lock.actions.sync_hooks.PreCommitHookConfig.from_yaml_file", side_effect=ValueError())
+@patch("sync_pre_commit_lock.pre_commit_config.PreCommitHookConfig.from_yaml_file", side_effect=ValueError())
 def test_execute_handles_file_invalid(mock_from_yaml_file: MagicMock) -> None:
     printer = MagicMock(spec=Printer)
     pre_commit_config_file_path = MagicMock(spec=Path)
     locked_packages: dict[str, GenericLockedPackage] = {}
     plugin_config = MagicMock(spec=SyncPreCommitLockConfig)
     plugin_config.disable_sync_from_lock = False
     dry_run = False
@@ -88,15 +87,15 @@
         plugin_config=plugin_config,
         dry_run=dry_run,
     )
     syncer.execute()
     printer.error.assert_called_once_with(f"Invalid pre-commit config file: {pre_commit_config_file_path}: ")
 
 
-@patch("sync_pre_commit_lock.actions.sync_hooks.PreCommitHookConfig.from_yaml_file")
+@patch("sync_pre_commit_lock.pre_commit_config.PreCommitHookConfig.from_yaml_file")
 @patch.object(SyncPreCommitHooksVersion, "build_mapping")
 @patch.object(SyncPreCommitHooksVersion, "analyze_repos")
 def test_execute_synchronizes_hooks(
     mock_analyze_repos: MagicMock, mock_build_mapping: MagicMock, mock_from_yaml_file: MagicMock
 ) -> None:
     printer = MagicMock(spec=Printer)
     pre_commit_config_file_path = MagicMock(spec=Path)
@@ -124,15 +123,15 @@
     # Assertions
     mock_build_mapping.assert_called_once()
     mock_analyze_repos.assert_called_once()
     pre_commit_config.update_pre_commit_repo_versions.assert_called_once_with({PreCommitRepo("repo1", "rev1"): "rev2"})
     printer.success.assert_called_with("Pre-commit hooks have been updated to match the lockfile!")
 
 
-@patch("sync_pre_commit_lock.actions.sync_hooks.PreCommitHookConfig.from_yaml_file")
+@patch("sync_pre_commit_lock.pre_commit_config.PreCommitHookConfig.from_yaml_file")
 @patch.object(SyncPreCommitHooksVersion, "build_mapping")
 @patch.object(SyncPreCommitHooksVersion, "analyze_repos")
 def test_execute_synchronizes_hooks_all_good(
     mock_analyze_repos: MagicMock, mock_build_mapping: MagicMock, mock_from_yaml_file: MagicMock
 ) -> None:
     printer = MagicMock(spec=Printer)
     pre_commit_config_file_path = MagicMock(spec=Path)
@@ -157,15 +156,15 @@
 
     syncer.execute()
 
     # Assertions
     mock_build_mapping.assert_called_once()
     mock_analyze_repos.assert_called_once()
     pre_commit_config.update_pre_commit_repo_versions.assert_not_called()
-    printer.success.assert_called_with("All matched pre-commit hooks already in sync with the lockfile!")
+    printer.info.assert_called_with("All matched pre-commit hooks already in sync with the lockfile!")
 
 
 def test_get_pre_commit_repo_new_version() -> None:
     printer = MagicMock(spec=Printer)
     pre_commit_config_file_path = MagicMock(spec=Path)
     locked_packages: dict[str, GenericLockedPackage] = {"lib_name": GenericLockedPackage("lib_name", "2.0.0")}
     plugin_config = MagicMock(spec=SyncPreCommitLockConfig)
```

### Comparing `sync_pre_commit_lock-0.1.2/tests/test_config.py` & `sync_pre_commit_lock-0.2.0/tests/test_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from unittest.mock import MagicMock, patch
 
 from sync_pre_commit_lock.config import SyncPreCommitLockConfig, from_toml, load_config
 from sync_pre_commit_lock.db import RepoInfo
 
 
-# @patch('sync_pre_commit_lock.config.SyncPreCommitLockConfig.__dataclass_fields__', new_callable=MagicMock)
 def test_from_toml() -> None:
     data = {
         "disable-sync-from-lock": True,
         "ignore": ["a", "b"],
         "pre-commit-config-file": ".test-config.yaml",
         "dependency-mapping": {"pytest": {"repo": "pytest", "rev": "${ver}"}},
     }
```

### Comparing `sync_pre_commit_lock-0.1.2/tests/test_pdm/test_pdm_plugin.py` & `sync_pre_commit_lock-0.2.0/tests/test_pdm/test_pdm_plugin.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.1.2/tests/test_pdm/test_pdm_sync_pre_commit_hook.py` & `sync_pre_commit_lock-0.2.0/tests/test_pdm/test_pdm_sync_pre_commit_hook.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.1.2/tests/test_poetry/test_poetry_plugin.py` & `sync_pre_commit_lock-0.2.0/tests/test_poetry/test_poetry_plugin.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.1.2/tests/test_utils.py` & `sync_pre_commit_lock-0.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.1.2/PKG-INFO` & `sync_pre_commit_lock-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sync-pre-commit-lock
-Version: 0.1.2
+Version: 0.2.0
 Summary: PDM plugin to sync your pre-commit versions with your lockfile, and install them, all automatically.
 Author-Email: Gabriel Dugny <sync-pre-commit-lock@dugny.me>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -690,16 +690,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Project-URL: Homepage, https://github.com/GabDug/sync-pre-commit-lock
 Project-URL: Changelog, https://github.com/GabDug/sync-pre-commit-lock/blob/main/CHANGELOG.md
 Project-URL: Bug tracker, https://github.com/GabDug/sync-pre-commit-lock/issues
 Requires-Python: >=3.10
-Requires-Dist: PyYAML>=6.0
 Requires-Dist: tomli>=2.0.0; python_version < "3.11"
+Requires-Dist: strictyaml>=1.7.3
 Requires-Dist: pdm>=2.7.4; extra == "pdm"
 Provides-Extra: pdm
 Description-Content-Type: text/markdown
 
 # sync-pre-commit-lock
 
 [![Tests](https://github.com/GabDug/sync-pre-commit-lock/actions/workflows/ci.yml/badge.svg)](https://github.com/GabDug/sync-pre-commit-lock/actions/workflows/ci.yml)
@@ -801,15 +801,16 @@
 - [ ] Add a dedicated CLI command to manage sync/install
 - [ ] Expose a pre-commit hook to sync the lockfile
 - [ ] Support nested params for some repos? Like mypy types
 - [ ] Support reading DB from a Python module?
 - [ ] Support reordering DB inputs (file/global config/python module/cli)?
 - [ ] Test using SSH/file dependencies?
 - [ ] Check ref existence before writing?
-- [ ] Support multiple hooks repos for the same dependency?
+- [ ] Support multiple hooks repos for the same dependency? E.g. ruff new and old repo
 - [ ] New feature to convert from pre-commit online to local?
+- [ ] Warning if pre-commit CI auto update is also set?
 
 ## Inspiration
 
 This project is inspired by @floatingpurr's [sync_with_pdm](https://github.com/floatingpurr/sync_with_pdm/) and [sync_with_poetry](https://github.com/floatingpurr/sync_with_poetry/).
 
 The code to install pre-commit hooks automatically is **adapted** from @vstrimaitis's [poetry-pre-commit-plugin](https://github.com/vstrimaitis/poetry-pre-commit-plugin/), licensed under GPL-3.
```

