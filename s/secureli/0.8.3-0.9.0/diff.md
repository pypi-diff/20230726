# Comparing `tmp/secureli-0.8.3.tar.gz` & `tmp/secureli-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secureli-0.8.3.tar", max compression
+gzip compressed data, was "secureli-0.9.0.tar", max compression
```

## Comparing `secureli-0.8.3.tar` & `secureli-0.9.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0    11343 2023-07-26 16:00:57.022905 secureli-0.8.3/LICENSE
--rw-r--r--   0        0        0    12497 2023-07-26 16:00:57.022905 secureli-0.8.3/README.md
--rw-r--r--   0        0        0     2094 2023-07-26 16:00:57.022905 secureli-0.8.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-26 16:00:57.022905 secureli-0.8.3/secureli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 16:00:57.022905 secureli-0.8.3/secureli/abstractions/__init__.py
--rw-r--r--   0        0        0     3919 2023-07-26 16:00:57.022905 secureli-0.8.3/secureli/abstractions/echo.py
--rw-r--r--   0        0        0      550 2023-07-26 16:00:57.022905 secureli-0.8.3/secureli/abstractions/lexer_guesser.py
--rw-r--r--   0        0        0     6906 2023-07-26 16:00:57.022905 secureli-0.8.3/secureli/abstractions/pre_commit.py
--rw-r--r--   0        0        0        0 2023-07-26 16:00:57.022905 secureli-0.8.3/secureli/actions/__init__.py
--rw-r--r--   0        0        0    11784 2023-07-26 16:00:57.022905 secureli-0.8.3/secureli/actions/action.py
--rw-r--r--   0        0        0      761 2023-07-26 16:00:57.022905 secureli-0.8.3/secureli/actions/build.py
--rw-r--r--   0        0        0     1160 2023-07-26 16:00:57.022905 secureli-0.8.3/secureli/actions/initializer.py
--rw-r--r--   0        0        0    10628 2023-07-26 16:00:57.022905 secureli-0.8.3/secureli/actions/scan.py
--rw-r--r--   0        0        0      791 2023-07-26 16:00:57.022905 secureli-0.8.3/secureli/actions/setup.py
--rw-r--r--   0        0        0     2087 2023-07-26 16:00:57.022905 secureli-0.8.3/secureli/actions/update.py
--rw-r--r--   0        0        0     6450 2023-07-26 16:00:57.022905 secureli-0.8.3/secureli/container.py
--rw-r--r--   0        0        0     2807 2023-07-26 16:00:57.022905 secureli-0.8.3/secureli/main.py
--rw-r--r--   0        0        0        0 2023-07-26 16:00:57.022905 secureli-0.8.3/secureli/repositories/__init__.py
--rw-r--r--   0        0        0     3685 2023-07-26 16:00:57.022905 secureli-0.8.3/secureli/repositories/repo_files.py
--rw-r--r--   0        0        0     3632 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/repositories/secureli_config.py
--rw-r--r--   0        0        0     3926 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/repositories/settings.py
--rw-r--r--   0        0        0       59 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/resources/__init__.py
--rw-r--r--   0        0        0      791 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/resources/files/base-pre-commit.yaml
--rw-r--r--   0        0        0     4883 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/resources/files/build.txt
--rw-r--r--   0        0        0       93 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/resources/files/configs/javascript.config.yaml
--rw-r--r--   0        0        0      161 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/resources/files/configs/typescript.config.yaml
--rw-r--r--   0        0        0      659 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/resources/files/csharp-pre-commit.yaml
--rw-r--r--   0        0        0      461 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/resources/files/epilog.md
--rw-r--r--   0        0        0      115 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/resources/files/go-pre-commit.yaml
--rw-r--r--   0        0        0      130 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/resources/files/java-pre-commit.yaml
--rw-r--r--   0        0        0      618 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/resources/files/javascript-pre-commit.yaml
--rw-r--r--   0        0        0      367 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/resources/files/python-pre-commit.yaml
--rw-r--r--   0        0        0      356 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/resources/files/secrets_detecting_repos.yaml
--rw-r--r--   0        0        0      232 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/resources/files/swift-pre-commit.yaml
--rw-r--r--   0        0        0      228 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/resources/files/terraform-pre-commit.yaml
--rw-r--r--   0        0        0      714 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/resources/files/typescript-pre-commit.yaml
--rw-r--r--   0        0        0      817 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/resources/read_resource.py
--rw-r--r--   0        0        0     1325 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/resources/slugify.py
--rw-r--r--   0        0        0        0 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/services/__init__.py
--rw-r--r--   0        0        0     3646 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/services/git_ignore.py
--rw-r--r--   0        0        0     3505 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/services/language_analyzer.py
--rw-r--r--   0        0        0    12318 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/services/language_config.py
--rw-r--r--   0        0        0    18724 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/services/language_support.py
--rw-r--r--   0        0        0     4614 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/services/logging.py
--rw-r--r--   0        0        0     6374 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/services/scanner.py
--rw-r--r--   0        0        0     1180 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/services/secureli_ignore.py
--rw-r--r--   0        0        0     3048 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/services/updater.py
--rw-r--r--   0        0        0     1482 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/settings.py
--rw-r--r--   0        0        0        0 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/utilities/__init__.py
--rw-r--r--   0        0        0     1080 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/utilities/git_meta.py
--rw-r--r--   0        0        0      254 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/utilities/hash.py
--rw-r--r--   0        0        0     1372 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/utilities/patterns.py
--rw-r--r--   0        0        0      198 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/utilities/secureli_meta.py
--rw-r--r--   0        0        0     1028 2023-07-26 16:00:57.026905 secureli-0.8.3/secureli/utilities/usage_stats.py
--rw-r--r--   0        0        0    13409 1970-01-01 00:00:00.000000 secureli-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0    11343 2023-07-26 20:54:11.361195 secureli-0.9.0/LICENSE
+-rw-r--r--   0        0        0    12497 2023-07-26 20:54:11.361195 secureli-0.9.0/README.md
+-rw-r--r--   0        0        0     2094 2023-07-26 20:54:11.365195 secureli-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/abstractions/__init__.py
+-rw-r--r--   0        0        0     3919 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/abstractions/echo.py
+-rw-r--r--   0        0        0      550 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/abstractions/lexer_guesser.py
+-rw-r--r--   0        0        0     6906 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/abstractions/pre_commit.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/actions/__init__.py
+-rw-r--r--   0        0        0    11917 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/actions/action.py
+-rw-r--r--   0        0        0      761 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/actions/build.py
+-rw-r--r--   0        0        0     1753 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/actions/initializer.py
+-rw-r--r--   0        0        0    10656 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/actions/scan.py
+-rw-r--r--   0        0        0      791 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/actions/setup.py
+-rw-r--r--   0        0        0     2087 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/actions/update.py
+-rw-r--r--   0        0        0     6490 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/container.py
+-rw-r--r--   0        0        0     2807 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/main.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/repositories/__init__.py
+-rw-r--r--   0        0        0     3685 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/repositories/repo_files.py
+-rw-r--r--   0        0        0     3632 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/repositories/secureli_config.py
+-rw-r--r--   0        0        0     3931 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/repositories/settings.py
+-rw-r--r--   0        0        0       59 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/resources/__init__.py
+-rw-r--r--   0        0        0      791 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/resources/files/base-pre-commit.yaml
+-rw-r--r--   0        0        0     4883 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/resources/files/build.txt
+-rw-r--r--   0        0        0       93 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/resources/files/configs/javascript.config.yaml
+-rw-r--r--   0        0        0      161 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/resources/files/configs/typescript.config.yaml
+-rw-r--r--   0        0        0      659 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/resources/files/csharp-pre-commit.yaml
+-rw-r--r--   0        0        0      461 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/resources/files/epilog.md
+-rw-r--r--   0        0        0      115 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/resources/files/go-pre-commit.yaml
+-rw-r--r--   0        0        0      130 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/resources/files/java-pre-commit.yaml
+-rw-r--r--   0        0        0      618 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/resources/files/javascript-pre-commit.yaml
+-rw-r--r--   0        0        0      367 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/resources/files/python-pre-commit.yaml
+-rw-r--r--   0        0        0      356 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/resources/files/secrets_detecting_repos.yaml
+-rw-r--r--   0        0        0      232 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/resources/files/swift-pre-commit.yaml
+-rw-r--r--   0        0        0      228 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/resources/files/terraform-pre-commit.yaml
+-rw-r--r--   0        0        0      714 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/resources/files/typescript-pre-commit.yaml
+-rw-r--r--   0        0        0      817 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/resources/read_resource.py
+-rw-r--r--   0        0        0     1325 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/resources/slugify.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/services/__init__.py
+-rw-r--r--   0        0        0     3646 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/services/git_ignore.py
+-rw-r--r--   0        0        0     3505 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/services/language_analyzer.py
+-rw-r--r--   0        0        0    12318 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/services/language_config.py
+-rw-r--r--   0        0        0    18724 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/services/language_support.py
+-rw-r--r--   0        0        0     4614 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/services/logging.py
+-rw-r--r--   0        0        0     6374 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/services/scanner.py
+-rw-r--r--   0        0        0     1180 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/services/secureli_ignore.py
+-rw-r--r--   0        0        0     3048 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/services/updater.py
+-rw-r--r--   0        0        0     1482 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/settings.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/utilities/__init__.py
+-rw-r--r--   0        0        0     1080 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/utilities/git_meta.py
+-rw-r--r--   0        0        0      254 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/utilities/hash.py
+-rw-r--r--   0        0        0     1372 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/utilities/patterns.py
+-rw-r--r--   0        0        0      198 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/utilities/secureli_meta.py
+-rw-r--r--   0        0        0     1028 2023-07-26 20:54:11.365195 secureli-0.9.0/secureli/utilities/usage_stats.py
+-rw-r--r--   0        0        0    13409 1970-01-01 00:00:00.000000 secureli-0.9.0/PKG-INFO
```

### Comparing `secureli-0.8.3/LICENSE` & `secureli-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `secureli-0.8.3/README.md` & `secureli-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `secureli-0.8.3/pyproject.toml` & `secureli-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secureli"
-version = "0.8.3"
+version = "0.9.0"
 description = "Secure Project Manager"
 authors = ["Caleb Tonn <caleb.tonn@slalom.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 secureli = "secureli.main:app"
```

### Comparing `secureli-0.8.3/secureli/abstractions/echo.py` & `secureli-0.9.0/secureli/abstractions/echo.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.3/secureli/abstractions/lexer_guesser.py` & `secureli-0.9.0/secureli/abstractions/lexer_guesser.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.3/secureli/abstractions/pre_commit.py` & `secureli-0.9.0/secureli/abstractions/pre_commit.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.3/secureli/actions/action.py` & `secureli-0.9.0/secureli/actions/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     InstallFailedError,
 )
 from secureli.repositories.secureli_config import (
     SecureliConfig,
     SecureliConfigRepository,
     VerifyConfigOutcome,
 )
+from secureli.repositories.settings import SecureliRepository
 from secureli.services.language_analyzer import LanguageAnalyzerService, AnalyzeResult
 from secureli.services.language_support import LanguageSupportService
 from secureli.services.scanner import ScannerService, ScanMode
 from secureli.services.updater import UpdaterService
 from secureli.services.language_config import LanguageNotSupportedError
 
 
@@ -55,21 +56,23 @@
     def __init__(
         self,
         echo: EchoAbstraction,
         language_analyzer: LanguageAnalyzerService,
         language_support: LanguageSupportService,
         scanner: ScannerService,
         secureli_config: SecureliConfigRepository,
+        settings: SecureliRepository,
         updater: UpdaterService,
     ):
         self.echo = echo
         self.language_analyzer = language_analyzer
         self.language_support = language_support
         self.scanner = scanner
         self.secureli_config = secureli_config
+        self.settings = settings
         self.updater = updater
 
 
 class Action(ABC):
     """The base Action class for any action that can analyze, install and update SeCureLI's configuration."""
 
     def __init__(self, action_deps: ActionDependencies):
```

### Comparing `secureli-0.8.3/secureli/actions/build.py` & `secureli-0.9.0/secureli/actions/build.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.3/secureli/actions/initializer.py` & `secureli-0.9.0/secureli/actions/initializer.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,12 +19,23 @@
     def initialize_repo(self, folder_path: Path, reset: bool, always_yes: bool):
         """
         Initializes SeCureLI for the specified folder path
         :param folder_path: The folder path to initialize the repo for
         :param reset: If true, disregard existing configuration and start fresh
         :param always_yes: Assume "Yes" to all prompts
         """
+
+        # Will create a blank .secureli.yaml file if it does not exist
+        settings = self.action_deps.settings.load()
+
+        # Why are we saving settings? CLI should not be modifying them....just reading
+        # With a templated example .secureli.yaml file, we won't be able to save
+        # 1. Remove functionality that verifies pre-commit-config.yaml against generated template
+        # 1. Remove functionality to automatically add ignores files and ignore hooks to .secureli.yaml/pre_commit.
+        # 1. Remove settings.save()
+        self.action_deps.settings.save(settings)
+
         verify_result = self.verify_install(folder_path, reset, always_yes)
         if verify_result.outcome in ScanAction.halting_outcomes:
             self.logging.failure(LogAction.init, verify_result.outcome)
         else:
             self.logging.success(LogAction.init)
```

### Comparing `secureli-0.8.3/secureli/actions/scan.py` & `secureli-0.9.0/secureli/actions/scan.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,21 +32,21 @@
 
     def __init__(
         self,
         action_deps: ActionDependencies,
         echo: EchoAbstraction,
         logging: LoggingService,
         scanner: ScannerService,
-        settings_repository: SecureliRepository,
+        # settings_repository: SecureliRepository,
     ):
         super().__init__(action_deps)
         self.scanner = scanner
         self.echo = echo
         self.logging = logging
-        self.settings = settings_repository
+        # self.settings = settings_repository
 
     def scan_repo(
         self,
         folder_path: Path,
         scan_mode: ScanMode,
         always_yes: bool,
         specific_test: Optional[str] = None,
@@ -104,15 +104,15 @@
         always_yes: bool,
     ):
         """
         Processes any failures found during the scan.
         :param failures: List of Failure objects representing linter failures
         :param always_yes: Assume "Yes" to all prompts
         """
-        settings = self.settings.load()
+        settings = self.action_deps.settings.load()
 
         ignore_fail_prompt = "Failures detected during scan.\n"
         ignore_fail_prompt += "Add an ignore rule?"
 
         # Ask if the user wants to ignore a failure
         if always_yes:
             always_yes_warning = "Hook failures were detected but the scan was initiated with the 'yes' flag.\n"
@@ -135,15 +135,15 @@
                 if failure.repo == OutputParseErrors.REPO_NOT_FOUND:
                     self._handle_repo_not_found(failure)
                 elif always_yes or add_ignore_for_id:
                     settings = self._add_ignore_for_failure(
                         failure=failure, always_yes=always_yes, settings_file=settings
                     )
 
-            self.settings.save(settings=settings)
+            self.action_deps.settings.save(settings=settings)
 
     def _add_ignore_for_failure(
         self,
         failure: Failure,
         always_yes: bool,
         settings_file: SecureliFile,
     ):
```

### Comparing `secureli-0.8.3/secureli/actions/setup.py` & `secureli-0.9.0/secureli/actions/setup.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.3/secureli/actions/update.py` & `secureli-0.9.0/secureli/actions/update.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.3/secureli/container.py` & `secureli-0.9.0/secureli/container.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,14 +142,15 @@
     action_deps = providers.Factory(
         ActionDependencies,
         echo=echo,
         language_analyzer=language_analyzer_service,
         language_support=language_support_service,
         scanner=scanner_service,
         secureli_config=secureli_config_repository,
+        settings=settings_repository,
         updater=updater_service,
     )
 
     """The Build Action, used to render the build_data using the echo"""
     build_action = providers.Factory(
         BuildAction,
         build_data=build_data,
@@ -167,15 +168,15 @@
     """Scan Action, representing what happens when the scan command is invoked"""
     scan_action = providers.Factory(
         ScanAction,
         action_deps=action_deps,
         echo=echo,
         logging=logging_service,
         scanner=scanner_service,
-        settings_repository=settings_repository,
+        # settings_repository=settings_repository,
     )
 
     """Update Action, representing what happens when the update command is invoked"""
     update_action = providers.Factory(
         UpdateAction,
         action_deps=action_deps,
         echo=echo,
```

### Comparing `secureli-0.8.3/secureli/main.py` & `secureli-0.9.0/secureli/main.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.3/secureli/repositories/repo_files.py` & `secureli-0.9.0/secureli/repositories/repo_files.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.3/secureli/repositories/secureli_config.py` & `secureli-0.9.0/secureli/repositories/secureli_config.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.3/secureli/repositories/settings.py` & `secureli-0.9.0/secureli/repositories/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 
     repos: list[PreCommitRepo] = Field(default=[])
     suppressed_repos: list[str] = Field(default=[])
 
 
 class SecureliFile(BaseModel):
     """
-    Represents the contents of the .secureli file
+    Represents the contents of the .secureli.yaml file
     """
 
     repo_files: Optional[RepoFilesSettings]
     echo: Optional[EchoSettings]
     language_support: Optional[LanguageSupportSettings] = Field(default=None)
     pre_commit: Optional[PreCommitSettings] = Field(default=None)
```

### Comparing `secureli-0.8.3/secureli/resources/files/base-pre-commit.yaml` & `secureli-0.9.0/secureli/resources/files/base-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.8.3/secureli/resources/files/build.txt` & `secureli-0.9.0/secureli/resources/files/build.txt`

 * *Files identical despite different names*

### Comparing `secureli-0.8.3/secureli/resources/files/csharp-pre-commit.yaml` & `secureli-0.9.0/secureli/resources/files/csharp-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.8.3/secureli/resources/files/javascript-pre-commit.yaml` & `secureli-0.9.0/secureli/resources/files/javascript-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.8.3/secureli/resources/files/typescript-pre-commit.yaml` & `secureli-0.9.0/secureli/resources/files/typescript-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.8.3/secureli/resources/read_resource.py` & `secureli-0.9.0/secureli/resources/read_resource.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.3/secureli/resources/slugify.py` & `secureli-0.9.0/secureli/resources/slugify.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.3/secureli/services/git_ignore.py` & `secureli-0.9.0/secureli/services/git_ignore.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.3/secureli/services/language_analyzer.py` & `secureli-0.9.0/secureli/services/language_analyzer.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.3/secureli/services/language_config.py` & `secureli-0.9.0/secureli/services/language_config.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.3/secureli/services/language_support.py` & `secureli-0.9.0/secureli/services/language_support.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.3/secureli/services/logging.py` & `secureli-0.9.0/secureli/services/logging.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.3/secureli/services/scanner.py` & `secureli-0.9.0/secureli/services/scanner.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.3/secureli/services/secureli_ignore.py` & `secureli-0.9.0/secureli/services/secureli_ignore.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.3/secureli/services/updater.py` & `secureli-0.9.0/secureli/services/updater.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.3/secureli/settings.py` & `secureli-0.9.0/secureli/settings.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.3/secureli/utilities/git_meta.py` & `secureli-0.9.0/secureli/utilities/git_meta.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.3/secureli/utilities/patterns.py` & `secureli-0.9.0/secureli/utilities/patterns.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.3/secureli/utilities/usage_stats.py` & `secureli-0.9.0/secureli/utilities/usage_stats.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.3/PKG-INFO` & `secureli-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secureli
-Version: 0.8.3
+Version: 0.9.0
 Summary: Secure Project Manager
 License: Apache-2.0
 Author: Caleb Tonn
 Author-email: caleb.tonn@slalom.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

