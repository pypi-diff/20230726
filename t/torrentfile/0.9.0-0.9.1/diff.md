# Comparing `tmp/torrentfile-0.9.0.tar.gz` & `tmp/torrentfile-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torrentfile-0.9.0.tar", last modified: Fri Jun  2 12:42:24 2023, max compression
+gzip compressed data, was "torrentfile-0.9.1.tar", last modified: Wed Jul 26 19:55:37 2023, max compression
```

## Comparing `torrentfile-0.9.0.tar` & `torrentfile-0.9.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 12:42:24.695457 torrentfile-0.9.0/
--rw-rw-rw-   0        0        0     1879 2022-06-06 03:34:50.000000 torrentfile-0.9.0/.cbuild
--rw-rw-rw-   0        0        0    10935 2023-06-02 07:12:23.000000 torrentfile-0.9.0/CHANGELOG.md
--rw-rw-rw-   0        0        0    11560 2022-04-01 22:38:43.000000 torrentfile-0.9.0/LICENSE
--rw-rw-rw-   0        0        0      153 2023-01-14 00:36:54.000000 torrentfile-0.9.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2602 2023-06-02 07:16:26.000000 torrentfile-0.9.0/Makefile
--rw-rw-rw-   0        0        0     9234 2023-06-02 12:42:24.694484 torrentfile-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     7730 2023-06-02 07:11:55.000000 torrentfile-0.9.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 12:42:24.674872 torrentfile-0.9.0/assets/
--rw-rw-rw-   0        0        0   999094 2022-10-21 07:26:02.000000 torrentfile-0.9.0/assets/Torrentfile.gif
--rw-rw-rw-   0        0        0    67244 2022-05-08 04:09:13.000000 torrentfile-0.9.0/assets/torrentfile-icon.ico
--rw-rw-rw-   0        0        0    31493 2022-05-08 04:09:13.000000 torrentfile-0.9.0/assets/torrentfile-icon.png
--rw-rw-rw-   0        0        0    25857 2022-02-13 04:29:03.000000 torrentfile-0.9.0/assets/torrentfile.png
--rw-rw-rw-   0        0        0    28319 2023-03-23 06:06:04.000000 torrentfile-0.9.0/assets/torrentfile_square.png
-drwxrwxrwx   0        0        0        0 2023-06-02 12:42:24.676872 torrentfile-0.9.0/c/
--rw-rw-rw-   0        0        0    12601 2022-04-05 09:08:46.000000 torrentfile-0.9.0/c/hasher.c
--rw-rw-rw-   0        0        0     1396 2022-04-01 22:38:43.000000 torrentfile-0.9.0/c/hasher.h
--rw-rw-rw-   0        0        0    11387 2022-04-01 22:38:43.000000 torrentfile-0.9.0/c/sha.c
--rw-rw-rw-   0        0        0     1629 2022-04-01 22:38:43.000000 torrentfile-0.9.0/c/sha.h
--rw-rw-rw-   0        0        0     2658 2023-06-02 11:57:14.000000 torrentfile-0.9.0/pyproject.toml
--rw-rw-rw-   0        0        0       13 2022-06-05 02:35:20.000000 torrentfile-0.9.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 12:42:24.695457 torrentfile-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0      914 2022-08-07 23:54:01.000000 torrentfile-0.9.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 12:42:24.680890 torrentfile-0.9.0/tests/
--rw-rw-rw-   0        0        0    16240 2023-06-02 12:41:18.000000 torrentfile-0.9.0/tests/test_cli.py
--rw-rw-rw-   0        0        0    11034 2023-06-02 12:41:18.000000 torrentfile-0.9.0/tests/test_commands.py
--rw-rw-rw-   0        0        0     7349 2023-06-02 12:41:18.000000 torrentfile-0.9.0/tests/test_edit.py
--rw-rw-rw-   0        0        0     5378 2023-06-02 12:41:18.000000 torrentfile-0.9.0/tests/test_interactive.py
--rw-rw-rw-   0        0        0     5822 2023-06-02 12:41:18.000000 torrentfile-0.9.0/tests/test_rebuild.py
--rw-rw-rw-   0        0        0     8794 2023-06-02 12:41:18.000000 torrentfile-0.9.0/tests/test_recheck.py
--rw-rw-rw-   0        0        0     7015 2023-06-02 12:41:18.000000 torrentfile-0.9.0/tests/test_torrent.py
--rw-rw-rw-   0        0        0     6562 2023-06-02 12:41:18.000000 torrentfile-0.9.0/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-02 12:42:24.689867 torrentfile-0.9.0/torrentfile/
--rw-rw-rw-   0        0        0     1449 2023-06-02 07:12:23.000000 torrentfile-0.9.0/torrentfile/__init__.py
--rw-rw-rw-   0        0        0     1079 2023-03-26 13:35:42.000000 torrentfile-0.9.0/torrentfile/__main__.py
--rw-rw-rw-   0        0        0    17744 2023-06-02 12:41:18.000000 torrentfile-0.9.0/torrentfile/cli.py
--rw-rw-rw-   0        0        0    12699 2023-06-02 12:41:17.000000 torrentfile-0.9.0/torrentfile/commands.py
--rw-rw-rw-   0        0        0     3777 2023-05-03 00:46:54.000000 torrentfile-0.9.0/torrentfile/edit.py
--rw-rw-rw-   0        0        0    16772 2023-06-02 07:11:55.000000 torrentfile-0.9.0/torrentfile/hasher.py
--rw-rw-rw-   0        0        0    11740 2023-06-02 12:41:17.000000 torrentfile-0.9.0/torrentfile/interactive.py
--rw-rw-rw-   0        0        0     7972 2023-06-02 12:41:17.000000 torrentfile-0.9.0/torrentfile/mixins.py
--rw-rw-rw-   0        0        0    19284 2023-06-02 12:41:17.000000 torrentfile-0.9.0/torrentfile/rebuild.py
--rw-rw-rw-   0        0        0    20532 2023-06-02 12:41:17.000000 torrentfile-0.9.0/torrentfile/recheck.py
--rw-rw-rw-   0        0        0    24434 2023-06-02 12:41:18.000000 torrentfile-0.9.0/torrentfile/torrent.py
--rw-rw-rw-   0        0        0    10731 2023-06-02 12:41:18.000000 torrentfile-0.9.0/torrentfile/utils.py
--rw-rw-rw-   0        0        0      905 2023-06-02 07:12:23.000000 torrentfile-0.9.0/torrentfile/version.py
-drwxrwxrwx   0        0        0        0 2023-06-02 12:42:24.694484 torrentfile-0.9.0/torrentfile.egg-info/
--rw-rw-rw-   0        0        0     9234 2023-06-02 12:42:24.000000 torrentfile-0.9.0/torrentfile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      957 2023-06-02 12:42:24.000000 torrentfile-0.9.0/torrentfile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 12:42:24.000000 torrentfile-0.9.0/torrentfile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-06-02 12:42:24.000000 torrentfile-0.9.0/torrentfile.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-06-02 12:42:24.000000 torrentfile-0.9.0/torrentfile.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-02 12:42:24.000000 torrentfile-0.9.0/torrentfile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2018 2023-05-03 00:46:54.000000 torrentfile-0.9.0/tox.ini
+drwxrwxrwx   0        0        0        0 2023-07-26 19:55:37.481449 torrentfile-0.9.1/
+-rw-rw-rw-   0        0        0     1879 2022-06-06 03:34:50.000000 torrentfile-0.9.1/.cbuild
+-rw-rw-rw-   0        0        0    11208 2023-07-25 03:54:43.000000 torrentfile-0.9.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0    11560 2022-04-01 22:38:43.000000 torrentfile-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0      153 2023-01-14 00:36:54.000000 torrentfile-0.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2703 2023-06-04 07:00:23.000000 torrentfile-0.9.1/Makefile
+-rw-rw-rw-   0        0        0     9056 2023-07-26 19:55:37.481449 torrentfile-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7552 2023-07-25 03:26:01.000000 torrentfile-0.9.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 19:55:37.459450 torrentfile-0.9.1/assets/
+-rw-rw-rw-   0        0        0   439978 2023-06-04 07:00:23.000000 torrentfile-0.9.1/assets/Torrentfile.gif
+-rw-rw-rw-   0        0        0    67244 2022-05-08 04:09:13.000000 torrentfile-0.9.1/assets/torrentfile-icon.ico
+-rw-rw-rw-   0        0        0    31493 2022-05-08 04:09:13.000000 torrentfile-0.9.1/assets/torrentfile-icon.png
+-rw-rw-rw-   0        0        0    25857 2022-02-13 04:29:03.000000 torrentfile-0.9.1/assets/torrentfile.png
+-rw-rw-rw-   0        0        0    28319 2023-03-23 06:06:04.000000 torrentfile-0.9.1/assets/torrentfile_square.png
+drwxrwxrwx   0        0        0        0 2023-07-26 19:55:37.462449 torrentfile-0.9.1/c/
+-rw-rw-rw-   0        0        0    12601 2022-04-05 09:08:46.000000 torrentfile-0.9.1/c/hasher.c
+-rw-rw-rw-   0        0        0     1396 2022-04-01 22:38:43.000000 torrentfile-0.9.1/c/hasher.h
+-rw-rw-rw-   0        0        0    11387 2022-04-01 22:38:43.000000 torrentfile-0.9.1/c/sha.c
+-rw-rw-rw-   0        0        0     1629 2022-04-01 22:38:43.000000 torrentfile-0.9.1/c/sha.h
+-rw-rw-rw-   0        0        0     2767 2023-07-25 03:26:01.000000 torrentfile-0.9.1/pyproject.toml
+-rw-rw-rw-   0        0        0       13 2022-06-05 02:35:20.000000 torrentfile-0.9.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 19:55:37.482451 torrentfile-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      914 2022-08-07 23:54:01.000000 torrentfile-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 19:55:37.467449 torrentfile-0.9.1/tests/
+-rw-rw-rw-   0        0        0    16304 2023-07-26 19:54:23.000000 torrentfile-0.9.1/tests/test_cli.py
+-rw-rw-rw-   0        0        0    11034 2023-07-26 19:54:23.000000 torrentfile-0.9.1/tests/test_commands.py
+-rw-rw-rw-   0        0        0     7208 2023-07-26 19:54:23.000000 torrentfile-0.9.1/tests/test_edit.py
+-rw-rw-rw-   0        0        0     5378 2023-07-26 19:54:23.000000 torrentfile-0.9.1/tests/test_interactive.py
+-rw-rw-rw-   0        0        0     5822 2023-07-26 19:54:23.000000 torrentfile-0.9.1/tests/test_rebuild.py
+-rw-rw-rw-   0        0        0     8794 2023-07-26 19:54:23.000000 torrentfile-0.9.1/tests/test_recheck.py
+-rw-rw-rw-   0        0        0     7039 2023-07-26 19:54:23.000000 torrentfile-0.9.1/tests/test_torrent.py
+-rw-rw-rw-   0        0        0     6821 2023-07-26 19:54:23.000000 torrentfile-0.9.1/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-26 19:55:37.476450 torrentfile-0.9.1/torrentfile/
+-rw-rw-rw-   0        0        0     1449 2023-06-04 07:00:23.000000 torrentfile-0.9.1/torrentfile/__init__.py
+-rw-rw-rw-   0        0        0     1079 2023-03-26 13:35:42.000000 torrentfile-0.9.1/torrentfile/__main__.py
+-rw-rw-rw-   0        0        0    17989 2023-07-26 19:54:22.000000 torrentfile-0.9.1/torrentfile/cli.py
+-rw-rw-rw-   0        0        0    12699 2023-07-26 19:54:22.000000 torrentfile-0.9.1/torrentfile/commands.py
+-rw-rw-rw-   0        0        0     3708 2023-07-25 03:26:01.000000 torrentfile-0.9.1/torrentfile/edit.py
+-rw-rw-rw-   0        0        0    17061 2023-07-25 03:26:08.000000 torrentfile-0.9.1/torrentfile/hasher.py
+-rw-rw-rw-   0        0        0    11740 2023-07-26 19:54:22.000000 torrentfile-0.9.1/torrentfile/interactive.py
+-rw-rw-rw-   0        0        0     7972 2023-07-26 19:54:22.000000 torrentfile-0.9.1/torrentfile/mixins.py
+-rw-rw-rw-   0        0        0    19284 2023-07-26 19:54:22.000000 torrentfile-0.9.1/torrentfile/rebuild.py
+-rw-rw-rw-   0        0        0    20532 2023-07-26 19:54:22.000000 torrentfile-0.9.1/torrentfile/recheck.py
+-rw-rw-rw-   0        0        0    25304 2023-07-26 19:54:22.000000 torrentfile-0.9.1/torrentfile/torrent.py
+-rw-rw-rw-   0        0        0    11173 2023-07-26 19:54:22.000000 torrentfile-0.9.1/torrentfile/utils.py
+-rw-rw-rw-   0        0        0      905 2023-07-25 03:26:01.000000 torrentfile-0.9.1/torrentfile/version.py
+drwxrwxrwx   0        0        0        0 2023-07-26 19:55:37.480451 torrentfile-0.9.1/torrentfile.egg-info/
+-rw-rw-rw-   0        0        0     9056 2023-07-26 19:55:37.000000 torrentfile-0.9.1/torrentfile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      957 2023-07-26 19:55:37.000000 torrentfile-0.9.1/torrentfile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 19:55:37.000000 torrentfile-0.9.1/torrentfile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-07-26 19:55:37.000000 torrentfile-0.9.1/torrentfile.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-26 19:55:37.000000 torrentfile-0.9.1/torrentfile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-26 19:55:37.000000 torrentfile-0.9.1/torrentfile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2018 2023-05-03 00:46:54.000000 torrentfile-0.9.1/tox.ini
```

### Comparing `torrentfile-0.9.0/.cbuild` & `torrentfile-0.9.1/.cbuild`

 * *Files identical despite different names*

### Comparing `torrentfile-0.9.0/CHANGELOG.md` & `torrentfile-0.9.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # CHANGELOG
 
+## Version 0.9.1
+
+- Clean up and consolidate many cli help strings
+- Removed some of the less popularly used argument shortcuts
+- Edited module and class level docstrings
+- Removed old/useless code.
+- Added `--align` cli flag for piece aligning v1 torrents
+
+---
+
 ## Version 0.9.0
 
 - Updates to Documentation.
 - Updated the main Gif in the readme file
 - Improved unittesting
 - Added new tests for functions in utils module
```

### Comparing `torrentfile-0.9.0/LICENSE` & `torrentfile-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torrentfile-0.9.0/Makefile` & `torrentfile-0.9.1/Makefile`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-.PHONY: clean help test docs release
-.DEFAULT_GOAL := help
-
-define PRINT_HELP_PYSCRIPT
-import re, sys
-for line in sys.stdin:
-	match = re.match(r'^([a-zA-Z_-]+):.*?## (.*)$$', line)
-	if match:
-		target, help = match.groups()
-		print("%-20s %s" % (target, help))
-endef
-export PRINT_HELP_PYSCRIPT
-
-define UPDATE_PACKAGE_VERSION
-import json
-from torrentfile.version import __version__
-data = json.load(open("package.json"))
-if data['version'] != __version__:
-	data['version'] = __version__
-	json.dump(data, open("package.json", "wt"), indent=2)
-endef
-export UPDATE_PACKAGE_VERSION
-
-define RENAME_FILE
-from torrentfile.version import __version__
-import os
-import sys
-if sys.platform == "win32":
-	inexe = "./torrentfile-windows-exec.zip"
-	exe = f"./dist/torrentfile-v{__version__}-win-exe.zip"
-	indir = "./torrentfile-windows-dir.zip"
-	dir = f"./dist/torrentfile-v{__version__}-win-dir.zip"
-	os.rename(inexe, exe)
-	os.rename(indir, dir)
-endef
-export RENAME_FILE
-
-BROWSER := python -c "$$BROWSER_PYSCRIPT"
-
-RENAME := python -c "$$RENAME_FILE"
-
-help:
-	@python -c "$$PRINT_HELP_PYSCRIPT" < $(MAKEFILE_LIST)
-
-clean: clean-build ## remove all build, test, coverage and Python artifacts
-
-clean-build: ## remove build artifacts
-	@echo Cleaning
-	rm -rvf build/
-	rm -fvr dist/
-	rm -fvr .eggs/
-	rm -fvr .tox/
-	rm -fv .coverage
-	rm -fv coverage.xml
-	rm -fvr htmlcov/
-	rm -fv corbertura.xml
-	rm -fvr .pytest_cache
-	rm -rvf Release
-	rm -rfv *.egg-info
-	rm -rfv .benchmarks
-	rm -rfv .codacy-coverage
-	rm -rfv node_modules
-	rm -fv torrentfile.log
-	rm -fvr -- *'/__pycache__'
-	rm -frv runner/build
-	rm -frv runner/dist
-	rm -rfv *.zip
-	rm -fv *.spec
-
-test: ## Get coverage report
-	pip install --pre --upgrade --force-reinstall --no-cache -rrequirements.txt
-	tox
-
-docs: ## Regenerate docs from changes
-	rm -rfv docs/*
-	rm -rfv site/index.md
-	cp -rfv README.md site/index.md
-	cp -rfv CHANGELOG.md site/changelog.md
-	rm -rfv site/htmlcov
-	mv -fv htmlcov site/
-	mkdocs build
-	touch docs/.nojekyll
-
-push: clean test docs ## Push to github
-	git add .
-	git commit -m "$m"
-	git push
-
-setup: clean test ## setup and build repo
-	python setup.py sdist bdist_wheel bdist_egg
-	pip install -e .
-	twine upload dist/*
-
-compile: clean test ## compile application for distribution
-	pip install pyinstaller
-	pip install -e .
-	pyinstaller -F --name torrentfile --icon ./assets/torrentfile-icon.ico ./bin/torrentfile
-	pyinstaller --name torrentfile --icon ./assets/torrentfile-icon.ico ./bin/torrentfile
-	7z a ./torrentfile-windows-exec.zip ./dist/torrentfile.exe
-	7z a ./torrentfile-windows-dir.zip ./dist/torrentfile
-	python -c "$$RENAME_FILE"
+.PHONY: clean help test docs release
+.DEFAULT_GOAL := help
+
+define PRINT_HELP_PYSCRIPT
+import re, sys
+for line in sys.stdin:
+	match = re.match(r'^([a-zA-Z_-]+):.*?## (.*)$$', line)
+	if match:
+		target, help = match.groups()
+		print("%-20s %s" % (target, help))
+endef
+export PRINT_HELP_PYSCRIPT
+
+define UPDATE_PACKAGE_VERSION
+import json
+from torrentfile.version import __version__
+data = json.load(open("package.json"))
+if data['version'] != __version__:
+	data['version'] = __version__
+	json.dump(data, open("package.json", "wt"), indent=2)
+endef
+export UPDATE_PACKAGE_VERSION
+
+define RENAME_FILE
+from torrentfile.version import __version__
+import os
+import sys
+if sys.platform == "win32":
+	inexe = "./torrentfile-windows-exec.zip"
+	exe = f"./dist/torrentfile-v{__version__}-win-exe.zip"
+	indir = "./torrentfile-windows-dir.zip"
+	dir = f"./dist/torrentfile-v{__version__}-win-dir.zip"
+	os.rename(inexe, exe)
+	os.rename(indir, dir)
+endef
+export RENAME_FILE
+
+BROWSER := python -c "$$BROWSER_PYSCRIPT"
+
+RENAME := python -c "$$RENAME_FILE"
+
+help:
+	@python -c "$$PRINT_HELP_PYSCRIPT" < $(MAKEFILE_LIST)
+
+clean: clean-build ## remove all build, test, coverage and Python artifacts
+
+clean-build: ## remove build artifacts
+	@echo Cleaning
+	rm -rvf build/
+	rm -fvr dist/
+	rm -fvr .eggs/
+	rm -fvr .tox/
+	rm -fv .coverage
+	rm -fv coverage.xml
+	rm -fvr htmlcov/
+	rm -fv corbertura.xml
+	rm -fvr .pytest_cache
+	rm -rvf Release
+	rm -rfv *.egg-info
+	rm -rfv .benchmarks
+	rm -rfv .codacy-coverage
+	rm -rfv node_modules
+	rm -fv torrentfile.log
+	rm -fvr -- *'/__pycache__'
+	rm -frv runner/build
+	rm -frv runner/dist
+	rm -rfv *.zip
+	rm -fv *.spec
+
+test: ## Get coverage report
+	pip install --pre --upgrade --force-reinstall --no-cache -rrequirements.txt
+	tox
+
+docs: ## Regenerate docs from changes
+	rm -rfv docs/*
+	rm -rfv site/index.md
+	cp -rfv README.md site/index.md
+	cp -rfv CHANGELOG.md site/changelog.md
+	rm -rfv site/htmlcov
+	mv -fv htmlcov site/
+	mkdocs build
+	touch docs/.nojekyll
+
+push: clean test docs ## Push to github
+	git add .
+	git commit -m "$m"
+	git push
+
+setup: clean test ## setup and build repo
+	python setup.py sdist bdist_wheel bdist_egg
+	pip install -e .
+	twine upload dist/*
+
+compile: clean test ## compile application for distribution
+	pip install pyinstaller
+	pip install -e .
+	pyinstaller -F --name torrentfile --icon ./assets/torrentfile-icon.ico ./bin/torrentfile
+	pyinstaller --name torrentfile --icon ./assets/torrentfile-icon.ico ./bin/torrentfile
+	7z a ./torrentfile-windows-exec.zip ./dist/torrentfile.exe
+	7z a ./torrentfile-windows-dir.zip ./dist/torrentfile
+	python -c "$$RENAME_FILE"
```

### Comparing `torrentfile-0.9.0/PKG-INFO` & `torrentfile-0.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torrentfile
-Version: 0.9.0
+Version: 0.9.1
 Summary: Terminal based command line tool for creating Bittorrent files.
 Author-email: alexpdev <alexpdev@pm.me>
 Project-URL: homepage, https://github.com/alexpdev/torrentfile
 Project-URL: repository, https://github.com
 Project-URL: documentation, https://alexpdev.github.io/torrentfile
 Project-URL: changelog, https://alexpdev.github.io/torrentfile/changelog/
 Project-URL: issues, https://github.com/alexpdev/torrentfile/issues
@@ -44,25 +44,25 @@
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/b67ff65b3d574025b65b6587266bbab7)](https://www.codacy.com/gh/alexpdev/torrentfile/dashboard?utm_source=github.com&utm_medium=referral&utm_content=alexpdev/torrentfile&utm_campaign=Badge_Coverage)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/b67ff65b3d574025b65b6587266bbab7)](https://www.codacy.com/gh/alexpdev/torrentfile/dashboard?utm_source=github.com&utm_medium=referral&utm_content=alexpdev/torrentfile&utm_campaign=Badge_Grade)
 [![DeepSource](https://deepsource.io/gh/alexpdev/TorrentFile.svg/?label=active+issues&token=16Sl_dF7nTU8YgPilcqhvHm8)](https://deepsource.io/gh/alexpdev/torrentfile/)
 [![codecov](https://codecov.io/gh/alexpdev/torrentfile/branch/master/graph/badge.svg?token=EWF7NIL9SQ)](https://codecov.io/gh/alexpdev/torrentfile?color=navy&logo=codecov)
 
 ## 🌐 Overview
 
-A command line interface for creating, reviewing, editing, or verifying bittorrent meta files (`.torrent` files). 
+A command line interface for creating, reviewing, editing, or verifying bittorrent meta files (`.torrent` files).
 _`torrentfile`_ is open source, and supports all versions of Bittorrent files, including hybrid meta files. The code base
 is also importable and can easily be used as a library for creating or manipulating torrent files in external projects.
 Documentation is available at [https://alexpdev.github.io/torrentfile](https://alexpdev.github.io/torrentfile).
 
 > A GUI frontend for this project can be found at <https://github.com/alexpdev/TorrentfileQt>
 
 ## 🔌 Requirements
 
--   Python 3.6+
--   Tested on Linux, Windows and Mac
+- Python 3.6+
+- Tested on Linux, Windows and Mac
 
 ## 💻 Install
 
 **PyPi:**
 
 ```bash
 pip install torrentfile
@@ -91,32 +91,29 @@
 ## 📝 License
 
 Apache Software License v2.0 - See [LICENSE]("https://github.com/alexpdev/torrentfile/blob/master/LICENSE")
 
 ## 💡 Issues & Requests & PRs
 
 If you encounter any bugs or would like to request a new feature please open a new issue.
-
-> PRs and other contributions are welcome
-
-<https://github.com/alexpdev/torrentfile/issues>
+PRs and other contributions that are meaningful and add value to the project are welcome.
 
 * * *
 
 ## Usage Examples
 
 ### Creating Bittorrent Files
 
 Creating a basic torrent file is as easy as using the create subcommand with the path to the torrent file.
 
 ```bash
 torrentfile create /path/to/content
 ```
 
-You can add one or more trackers by using any one of `-a`, `--announce` 
+You can add one or more trackers by using any one of `-a`, `--announce`
 flags and listing their URL as a space separated list.
 
 ```bash
 torrentfile create /path/to/content -a http://tracker1.com http://tracker2.net
 ```
 
 If you intend to distribute the file on a private tracker then you should use one  
@@ -128,18 +125,14 @@
 ```
 
 By default **`torrentfile`** displays a progress bar indicating how much of the content  
 has already been processed.  To turn off this display you can either use `--quiet` mode in  
 as a global flag or you can set the `--prog` flag to 0.
 
 ```bash
-torrentfile --quiet create /path/to/content
-```
-
-```bash
 torrentfile create /path/to/content --prog 0
 ```
 
 **`torrentfile`** extracts the name of the contents top level file or directory  
 and saves the torrent file to the current working directory with the extracted title.
 
 For example running the follwing command would create `./content.torrent`.
@@ -160,38 +153,37 @@
 
 For example the following command would create a torrent file at `/some/other/path/content.torrent`.
 
 ```bash
 torrentfile create /path/to/content -o /some/other/path/
 ```
 
-Bittorrent protocol V1 is still the most commonly used version, therefore _`torrentfile`_ creates
-Bittorrent version 1 torrent files by default. To specify creating a V2 file or hybrid (v1 and v2)
-use the `--meta-version` followed by the specific version number format to use.  The options include:
-`1`(v1 default), `2`(v2), or `3`(v1 & v2).
+_`torrentfile`_ creates Bittorrent v1 files by default. To create a V2 or hybrid (v1 and v2)
+torrent file, use the `--meta-version` option followed by the preferred version number option.
+The options include:  `1`(v1 default), `2`(v2), or `3`(v1 & v2).
 
 ```bash
 torrentfile create /path/to/content --meta-version 2
 ```
 
 ```bash
 torrentfile create /path/to/content --meta-version 3 
 ```
 
->`torrentfile` now includes the option to command line flags for the `create` sub-command from an `ini` style
+`torrentfile` includes the option to command line flags for the `create` sub-command from an `ini` style
 configuration file, by using the `--config` and optional `--config-path` options to specify the path
 to the configuration file.  If `--config-path` is ommited, then `torrentfile` will look by default in the current
-working directory for a file named `torrentfile.ini`. If the file is not discovered in the current working directory, 
-it will move on to look `~/.torrentfile/torrentfile.ini` followed by `~/.config/torrentfile.ini`.  Please see the 
+working directory for a file named `torrentfile.ini`. If the file is not discovered in the current working directory,
+it will move on to look `~/.torrentfile/torrentfile.ini` followed by `~/.config/torrentfile.ini`.  Please see the
 [documentation](https://alexpdev.github.io/torrentfile/overview/) for more details on how the configuration file should be
 formatted.
 
 ### Check/Recheck Torrent
 
-The `recheck` subcommand allows you to scan a Bittorrent file and compare it's contents, 
+The `recheck` subcommand allows you to scan a Bittorrent file and compare it's contents,
 against a file or directory containing the contents the torrent file was created from.
 The output provided by this process gives a detailed perspective if any files are missing
 or have been corrupted in any way.  Supports any version of Bittorrent file.
 
 ```bash
 torrentfile recheck /path/to/some.torrent /path/to/content
 ```
@@ -211,15 +203,15 @@
 ```bash
 torrentfile edit -h
 ```
 
 ### Create Magnet
 
 To create a magnet URI for a pre-existing torrent meta file, use the sub-command  
-`magnet` or `m` with the path to the torrent file.
+`magnet` with the path to the torrent file.
 
 ```bash
 torrentfile magnet /path/to/some.torrent
 ```
 
 ### GUI
```

### Comparing `torrentfile-0.9.0/README.md` & `torrentfile-0.9.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/b67ff65b3d574025b65b6587266bbab7)](https://www.codacy.com/gh/alexpdev/torrentfile/dashboard?utm_source=github.com&utm_medium=referral&utm_content=alexpdev/torrentfile&utm_campaign=Badge_Coverage)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/b67ff65b3d574025b65b6587266bbab7)](https://www.codacy.com/gh/alexpdev/torrentfile/dashboard?utm_source=github.com&utm_medium=referral&utm_content=alexpdev/torrentfile&utm_campaign=Badge_Grade)
 [![DeepSource](https://deepsource.io/gh/alexpdev/TorrentFile.svg/?label=active+issues&token=16Sl_dF7nTU8YgPilcqhvHm8)](https://deepsource.io/gh/alexpdev/torrentfile/)
 [![codecov](https://codecov.io/gh/alexpdev/torrentfile/branch/master/graph/badge.svg?token=EWF7NIL9SQ)](https://codecov.io/gh/alexpdev/torrentfile?color=navy&logo=codecov)
 
 ## 🌐 Overview
 
-A command line interface for creating, reviewing, editing, or verifying bittorrent meta files (`.torrent` files). 
+A command line interface for creating, reviewing, editing, or verifying bittorrent meta files (`.torrent` files).
 _`torrentfile`_ is open source, and supports all versions of Bittorrent files, including hybrid meta files. The code base
 is also importable and can easily be used as a library for creating or manipulating torrent files in external projects.
 Documentation is available at [https://alexpdev.github.io/torrentfile](https://alexpdev.github.io/torrentfile).
 
 > A GUI frontend for this project can be found at <https://github.com/alexpdev/TorrentfileQt>
 
 ## 🔌 Requirements
 
--   Python 3.6+
--   Tested on Linux, Windows and Mac
+- Python 3.6+
+- Tested on Linux, Windows and Mac
 
 ## 💻 Install
 
 **PyPi:**
 
 ```bash
 pip install torrentfile
@@ -59,32 +59,29 @@
 ## 📝 License
 
 Apache Software License v2.0 - See [LICENSE]("https://github.com/alexpdev/torrentfile/blob/master/LICENSE")
 
 ## 💡 Issues & Requests & PRs
 
 If you encounter any bugs or would like to request a new feature please open a new issue.
-
-> PRs and other contributions are welcome
-
-<https://github.com/alexpdev/torrentfile/issues>
+PRs and other contributions that are meaningful and add value to the project are welcome.
 
 * * *
 
 ## Usage Examples
 
 ### Creating Bittorrent Files
 
 Creating a basic torrent file is as easy as using the create subcommand with the path to the torrent file.
 
 ```bash
 torrentfile create /path/to/content
 ```
 
-You can add one or more trackers by using any one of `-a`, `--announce` 
+You can add one or more trackers by using any one of `-a`, `--announce`
 flags and listing their URL as a space separated list.
 
 ```bash
 torrentfile create /path/to/content -a http://tracker1.com http://tracker2.net
 ```
 
 If you intend to distribute the file on a private tracker then you should use one  
@@ -96,18 +93,14 @@
 ```
 
 By default **`torrentfile`** displays a progress bar indicating how much of the content  
 has already been processed.  To turn off this display you can either use `--quiet` mode in  
 as a global flag or you can set the `--prog` flag to 0.
 
 ```bash
-torrentfile --quiet create /path/to/content
-```
-
-```bash
 torrentfile create /path/to/content --prog 0
 ```
 
 **`torrentfile`** extracts the name of the contents top level file or directory  
 and saves the torrent file to the current working directory with the extracted title.
 
 For example running the follwing command would create `./content.torrent`.
@@ -128,38 +121,37 @@
 
 For example the following command would create a torrent file at `/some/other/path/content.torrent`.
 
 ```bash
 torrentfile create /path/to/content -o /some/other/path/
 ```
 
-Bittorrent protocol V1 is still the most commonly used version, therefore _`torrentfile`_ creates
-Bittorrent version 1 torrent files by default. To specify creating a V2 file or hybrid (v1 and v2)
-use the `--meta-version` followed by the specific version number format to use.  The options include:
-`1`(v1 default), `2`(v2), or `3`(v1 & v2).
+_`torrentfile`_ creates Bittorrent v1 files by default. To create a V2 or hybrid (v1 and v2)
+torrent file, use the `--meta-version` option followed by the preferred version number option.
+The options include:  `1`(v1 default), `2`(v2), or `3`(v1 & v2).
 
 ```bash
 torrentfile create /path/to/content --meta-version 2
 ```
 
 ```bash
 torrentfile create /path/to/content --meta-version 3 
 ```
 
->`torrentfile` now includes the option to command line flags for the `create` sub-command from an `ini` style
+`torrentfile` includes the option to command line flags for the `create` sub-command from an `ini` style
 configuration file, by using the `--config` and optional `--config-path` options to specify the path
 to the configuration file.  If `--config-path` is ommited, then `torrentfile` will look by default in the current
-working directory for a file named `torrentfile.ini`. If the file is not discovered in the current working directory, 
-it will move on to look `~/.torrentfile/torrentfile.ini` followed by `~/.config/torrentfile.ini`.  Please see the 
+working directory for a file named `torrentfile.ini`. If the file is not discovered in the current working directory,
+it will move on to look `~/.torrentfile/torrentfile.ini` followed by `~/.config/torrentfile.ini`.  Please see the
 [documentation](https://alexpdev.github.io/torrentfile/overview/) for more details on how the configuration file should be
 formatted.
 
 ### Check/Recheck Torrent
 
-The `recheck` subcommand allows you to scan a Bittorrent file and compare it's contents, 
+The `recheck` subcommand allows you to scan a Bittorrent file and compare it's contents,
 against a file or directory containing the contents the torrent file was created from.
 The output provided by this process gives a detailed perspective if any files are missing
 or have been corrupted in any way.  Supports any version of Bittorrent file.
 
 ```bash
 torrentfile recheck /path/to/some.torrent /path/to/content
 ```
@@ -179,15 +171,15 @@
 ```bash
 torrentfile edit -h
 ```
 
 ### Create Magnet
 
 To create a magnet URI for a pre-existing torrent meta file, use the sub-command  
-`magnet` or `m` with the path to the torrent file.
+`magnet` with the path to the torrent file.
 
 ```bash
 torrentfile magnet /path/to/some.torrent
 ```
 
 ### GUI
```

### Comparing `torrentfile-0.9.0/assets/torrentfile-icon.ico` & `torrentfile-0.9.1/assets/torrentfile-icon.ico`

 * *Files identical despite different names*

### Comparing `torrentfile-0.9.0/assets/torrentfile-icon.png` & `torrentfile-0.9.1/assets/torrentfile-icon.png`

 * *Files identical despite different names*

### Comparing `torrentfile-0.9.0/assets/torrentfile.png` & `torrentfile-0.9.1/assets/torrentfile.png`

 * *Files identical despite different names*

### Comparing `torrentfile-0.9.0/assets/torrentfile_square.png` & `torrentfile-0.9.1/assets/torrentfile_square.png`

 * *Files identical despite different names*

### Comparing `torrentfile-0.9.0/c/hasher.c` & `torrentfile-0.9.1/c/hasher.c`

 * *Files identical despite different names*

### Comparing `torrentfile-0.9.0/c/hasher.h` & `torrentfile-0.9.1/c/hasher.h`

 * *Files identical despite different names*

### Comparing `torrentfile-0.9.0/c/sha.c` & `torrentfile-0.9.1/c/sha.c`

 * *Files identical despite different names*

### Comparing `torrentfile-0.9.0/c/sha.h` & `torrentfile-0.9.1/c/sha.h`

 * *Files identical despite different names*

### Comparing `torrentfile-0.9.0/pyproject.toml` & `torrentfile-0.9.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-[build-system]
-requires = ["setuptools>=40.8.0", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "torrentfile"
-authors = [{name = "alexpdev", email = "alexpdev@pm.me"}]
-description = "Terminal based command line tool for creating Bittorrent files."
-version = "0.9.0"
-readme = "README.md"
-requires-python = ">=3.6"
-keywords = ["Bittorrent", "torrent", "bittorrent-metafiles", "CLI", "torrentfile"]
-classifiers = [
-    "Environment :: Console",
-    "Development Status :: 4 - Beta",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3 :: Only",
-    "Intended Audience :: End Users/Desktop",
-    "Intended Audience :: Developers",
-    "Topic :: Utilities",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "License :: OSI Approved :: Apache Software License",
-]
-dependencies = ["pyben"]
-
-[project.scripts]
-torrentfile = "torrentfile:main"
-tfile = "torrentfile:main"
-
-[project.urls]
-homepage = "https://github.com/alexpdev/torrentfile"
-repository = "https://github.com"
-documentation = "https://alexpdev.github.io/torrentfile"
-changelog = "https://alexpdev.github.io/torrentfile/changelog/"
-issues = "https://github.com/alexpdev/torrentfile/issues"
-
-[tool.setuptools]
-packages = ["torrentfile"]
-
-[tool.bandit]
-skips = ["B101"]
-
-[tool.black]
-line-length = 79
-
-[tool.autopep8]
-max_line_length = 80
-ignore = "E266"
-in-place = true
-recursive = true
-aggressive = 3
-
-[tool.pytest.ini_options]
-testpaths = [
-    "tests",
-    "torrentfile",
-]
-console_output_style = "progress"
-addopts = "--maxfail=3"
-
-
-[tool.pylint. 'MESSAGES CONTROL']
-disable = [
-    "R1729",
-    "W0108",
-    "W0106",
-    "redefined-outer-name",
-    "attribute-defined-outside-init",
-    "invalid-name",
-    "not-callable",
-    "consider-using-with",
-    "implicit-str-concat",
-    "no-member"
-]
-
-[tool.pylint. 'VARIABLES']
-callbacks = ["cb_", "_cb", "hook_"]
-
-[tool.pylint. 'FORMAT']
-max-line-length = 80
-single-line-if-stmt = true
-
-[tool.pylint.'SIMILARITIES']
-ignore-comments = true
-ignore-docstrings=true
-ignore-imports=true
-
-[tool.pylint. 'DESIGN']
-max-args=15
-min-public-methods=0
-max-attributes=20
-max-statements=75
-max-branches=20
-min-similarity-lines=4
-max-locals=25
-
-[tool.isort]
-multi_line_output = 4
-length_sort_straight = true
-line_length = 80
-wrap_length = 79
+[build-system]
+requires = ["setuptools>=40.8.0", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "torrentfile"
+authors = [{name = "alexpdev", email = "alexpdev@pm.me"}]
+description = "Terminal based command line tool for creating Bittorrent files."
+version = "0.9.1"
+readme = "README.md"
+requires-python = ">=3.6"
+keywords = ["Bittorrent", "torrent", "bittorrent-metafiles", "CLI", "torrentfile"]
+classifiers = [
+    "Environment :: Console",
+    "Development Status :: 4 - Beta",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.6",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3 :: Only",
+    "Intended Audience :: End Users/Desktop",
+    "Intended Audience :: Developers",
+    "Topic :: Utilities",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "License :: OSI Approved :: Apache Software License",
+]
+dependencies = ["pyben"]
+
+[project.scripts]
+torrentfile = "torrentfile:main"
+tfile = "torrentfile:main"
+
+[project.urls]
+homepage = "https://github.com/alexpdev/torrentfile"
+repository = "https://github.com"
+documentation = "https://alexpdev.github.io/torrentfile"
+changelog = "https://alexpdev.github.io/torrentfile/changelog/"
+issues = "https://github.com/alexpdev/torrentfile/issues"
+
+[tool.setuptools]
+packages = ["torrentfile"]
+
+[tool.bandit]
+skips = ["B101"]
+
+[tool.black]
+line-length = 79
+
+[tool.autopep8]
+max_line_length = 80
+ignore = "E266"
+in-place = true
+recursive = true
+aggressive = 3
+
+[tool.pytest.ini_options]
+testpaths = [
+    "tests",
+    "torrentfile",
+]
+console_output_style = "progress"
+addopts = "--maxfail=3"
+
+
+[tool.pylint. 'MESSAGES CONTROL']
+disable = [
+    "R1729",
+    "W0108",
+    "W0106",
+    "redefined-outer-name",
+    "attribute-defined-outside-init",
+    "invalid-name",
+    "not-callable",
+    "consider-using-with",
+    "implicit-str-concat",
+    "no-member"
+]
+
+[tool.pylint. 'VARIABLES']
+callbacks = ["cb_", "_cb", "hook_"]
+
+[tool.pylint. 'FORMAT']
+max-line-length = 80
+single-line-if-stmt = true
+
+[tool.pylint.'SIMILARITIES']
+ignore-comments = true
+ignore-docstrings=true
+ignore-imports=true
+
+[tool.pylint. 'DESIGN']
+max-args=15
+min-public-methods=0
+max-attributes=20
+max-statements=75
+max-branches=20
+min-similarity-lines=4
+max-locals=25
+
+[tool.isort]
+multi_line_output = 4
+length_sort_straight = true
+line_length = 80
+wrap_length = 79
```

### Comparing `torrentfile-0.9.0/setup.py` & `torrentfile-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `torrentfile-0.9.0/tests/test_cli.py` & `torrentfile-0.9.1/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,15 @@
         "torrentfile",
         "create",
         folder,
         "--piece-length",
         str(piece_length),
         "--meta-version",
         version,
-        "--tracker",
+        "--announce",
         "https://announce.org/tracker",
         "-o",
         torrent,
     ]
     sys.argv = args
     execute()
     meta = pyben.load(torrent)
@@ -180,15 +180,15 @@
         "torrentfile",
         "create",
         folder,
         "--meta-version",
         version,
         "-o",
         torrent,
-        "--tracker",
+        "--announce",
     ] + trackers
     sys.argv = args
     execute()
     meta = pyben.load(torrent)
     for url in trackers:
         assert url in [j for i in meta["announce-list"] for j in i]
 
@@ -291,23 +291,24 @@
         "-q",
         "create",
         folder,
         "--piece-length",
         str(piece_length),
         "--meta-version",
         version,
+        "--align",
         "--comment",
         "this is a comment",
         "-o",
         torrent,
     ]
     sys.argv = args
     execute()
     meta = pyben.load(torrent)
-    assert "TorrentFile" in meta["created by"]
+    assert "torrentfile" in meta["created by"]
 
 
 @pytest.mark.parametrize("piece_length", [2**exp for exp in range(14, 21)])
 @pytest.mark.parametrize("version", ["1", "2", "3"])
 def test_cli_web_seeds(folder, piece_length, version):
     """
     Test if created torrents recieve a web seeds field in meta info.
@@ -315,17 +316,18 @@
     folder, torrent = folder
     args = [
         "torrentfile",
         "create",
         folder,
         "--piece-length",
         str(piece_length),
+        "--align",
         "--meta-version",
         version,
-        "-w",
+        "--web-seed",
         "https://webseed.url/1",
         "https://webseed.url/2",
         "https://webseed.url/3",
         "-o",
         torrent,
     ]
     sys.argv = args
@@ -449,15 +451,15 @@
     if sys.platform != "win32" and ending == "\\":  # pragma: nocover
         ending = "/"
     args = [
         "torrentfile",
         "create",
         "-o",
         outfile,
-        "-t",
+        "-a",
         "https://announce1.org",
         "--private",
         str(dir1) + ending,
     ]
     sys.argv = args
     execute()
     assert os.path.exists(outfile)
@@ -471,30 +473,30 @@
     """
     if sys.platform != "win32":
         sep = "/"  # pragma: nocover
     parent = os.path.dirname(dir1) + sep
     args = [
         "torrentfile",
         "create",
-        "-t",
+        "-a",
         "https://announce1.org",
         "--private",
         "-o",
         parent,
         str(dir1),
     ]
     sys.argv = args
     execute()
     outfile = str(dir1) + ".torrent"
     assert os.path.exists(outfile)
     rmpath(outfile)
 
 
-@pytest.mark.parametrize(
-    "flag", ["-t", "-w", "--announce", "--web-seed", "--http-seed"])
+@pytest.mark.parametrize("flag",
+                         ["-a", "--announce", "--web-seed", "--http-seed"])
 def test_cli_announce_path(dir1, flag):
     """
     Test CLI when path is placed after the trackers flag.
     """
     outfile = str(dir1) + ".torrent"
     args = [
         "torrentfile",
```

### Comparing `torrentfile-0.9.0/tests/test_commands.py` & `torrentfile-0.9.1/tests/test_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
     """
     Test the info_command action from the Command Line Interface.
     """
     outfile = str(file1) + ".torrent"
     args = [
         "torrentfile",
         "create",
-        "-t",
+        "-a",
         "url1",
         "url2",
         "url3",
         "--web-seed",
         "url4",
         "url5",
         "--http-seed",
```

### Comparing `torrentfile-0.9.0/tests/test_edit.py` & `torrentfile-0.9.1/tests/test_edit.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,16 @@
 def test_fix():
     """
     Testing dir fixtures.
     """
     assert dir2 and metafile2 and dir1
 
 
-@pytest.mark.parametrize("announce",
-                         [["urla"], ["urlb", "urlc"], ["urla", "urlb", "urlc"]]
-                         )
+@pytest.mark.parametrize(
+    "announce", [["urla"], ["urlb", "urlc"], ["urla", "urlb", "urlc"]])
 def test_edit_torrent(metafile2, announce):
     """
     Test edit torrent with announce param.
     """
     edits = {"announce": announce}
     data = edit_torrent(metafile2, edits)
     meta = pyben.load(metafile2)
@@ -83,31 +82,29 @@
     edits = {"httpseeds": httpseeds}
     data = edit_torrent(metafile2, edits)
     meta = pyben.load(metafile2)
     assert data == meta
     assert data["httpseeds"] == httpseeds.split()
 
 
-@pytest.mark.parametrize("url_list",
-                         [["urla"], ["urlb", "urlc"], ["urla", "urlb", "urlc"]]
-                         )
+@pytest.mark.parametrize(
+    "url_list", [["urla"], ["urlb", "urlc"], ["urla", "urlb", "urlc"]])
 def test_edit_urllist(metafile2, url_list):
     """
     Test edit torrent with webseed param as string.
     """
     edits = {"url-list": url_list}
     data = edit_torrent(metafile2, edits)
     meta = pyben.load(metafile2)
     assert data == meta
     assert data["url-list"] == url_list
 
 
-@pytest.mark.parametrize("httpseed",
-                         [["urla"], ["urlb", "urlc"], ["urla", "urlb", "urlc"]]
-                         )
+@pytest.mark.parametrize(
+    "httpseed", [["urla"], ["urlb", "urlc"], ["urla", "urlb", "urlc"]])
 def test_edit_httpseeds(metafile2, httpseed):
     """
     Test edit torrent with webseed param as string.
     """
     edits = {"httpseeds": httpseed}
     data = edit_torrent(metafile2, edits)
     meta = pyben.load(metafile2)
```

### Comparing `torrentfile-0.9.0/tests/test_interactive.py` & `torrentfile-0.9.1/tests/test_interactive.py`

 * *Files identical despite different names*

### Comparing `torrentfile-0.9.0/tests/test_rebuild.py` & `torrentfile-0.9.1/tests/test_rebuild.py`

 * *Files identical despite different names*

### Comparing `torrentfile-0.9.0/tests/test_recheck.py` & `torrentfile-0.9.1/tests/test_recheck.py`

 * *Files identical despite different names*

### Comparing `torrentfile-0.9.0/tests/test_torrent.py` & `torrentfile-0.9.1/tests/test_torrent.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,14 +220,15 @@
     tfile = tempfile(exp=26)
     outfile = str(tfile) + ".torrent"
     args = {
         "path": tfile,
         "progress": progress,
         "piece_length": "14",
         "outfile": outfile,
+        "align": True,
     }
     torrent = version(**args)
     outfile, _ = torrent.write()
     assert os.path.exists(outfile)
     rmpath(tfile, outfile)
```

### Comparing `torrentfile-0.9.0/tests/test_utils.py` & `torrentfile-0.9.1/tests/test_utils.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,259 +1,259 @@
-#! /usr/bin/python3
-# -*- coding: utf-8 -*-
-
-##############################################################################
-#    Copyright (C) 2021-current alexpdev
-#
-#    Licensed under the Apache License, Version 2.0 (the "License");
-#    you may not use this file except in compliance with the License.
-#    You may obtain a copy of the License at
-#
-#        http://www.apache.org/licenses/LICENSE-2.0
-#
-#    Unless required by applicable law or agreed to in writing, software
-#    distributed under the License is distributed on an "AS IS" BASIS,
-#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#    See the License for the specific language governing permissions and
-#    limitations under the License.
-##############################################################################
-"""
-Unittest functions for testing torrentfile utils module.
-"""
-import math
-
-import pytest
-
-from tests import dir1, dir2, rmpath
-from torrentfile import utils
-from torrentfile.__main__ import main
-
-
-def test_main_exists():
-    """
-    Test if main exists
-    """
-    assert main
-
-
-@pytest.mark.parametrize("size", [156634528, 2**30, 67987, 16384, 8563945])
-def test_get_piece_length(size):
-    """
-    Test function for best piece length for given size.
-    """
-    value = utils.get_piece_length(size)
-    assert value % 1024 == 0
-
-
-@pytest.mark.parametrize("size", [156634528, 2**30, 67987, 16384, 8563945])
-def test_get_piece_length_max(size):
-    """
-    Test function for best piece length for given size maximum.
-    """
-    value = utils.get_piece_length(size)
-    assert value < 2**27
-
-
-@pytest.mark.parametrize("size", [156634528, 2**30, 67987, 16384, 8563945])
-def test_get_piece_length_min(size):
-    """
-    Test function for best piece length for given size minimum.
-    """
-    value = utils.get_piece_length(size)
-    assert value >= 2**14
-
-
-def test_get_path_length_mod(dir1):
-    """
-    Test function for the best piece length for provided path.
-    """
-    assert utils.path_piece_length(dir1) % (2**14) == 0
-
-
-def test_get_path_length_min(dir1):
-    """
-    Test function for getting piece length for folders min.
-    """
-    assert utils.path_piece_length(dir1) >= (2**14)
-
-
-def test_get_path_length_max(dir1):
-    """
-    Test function for getting piece length for folders max.
-    """
-    assert utils.path_piece_length(dir1) <= (2**27)
-
-
-def test_path_stat(dir1):
-    """
-    Test function for acquiring piece length information on folder.
-    """
-    _, _, piece_length = utils.path_stat(dir1)
-    assert piece_length % (2**14) == 0
-
-
-def test_path_stat_size(dir1):
-    """
-    Test function for acquiring total size information on folder.
-    """
-    _, totalsize, _ = utils.path_stat(dir1)
-    assert totalsize == (2**18) * 8
-
-
-def test_path_stat_filelist_size(dir1):
-    """
-    Test function for acquiring file list information on folder.
-    """
-    filelist, _, _ = utils.path_stat(dir1)
-    assert len(filelist) == 8
-
-
-def test_get_filelist(dir1):
-    """
-    Test function for get a list of files in a directory.
-    """
-    filelist = utils.get_file_list(dir1)
-    assert len(filelist) == 8
-
-
-def test_get_path_size(dir1):
-    """
-    Test function for getting total size of directory.
-    """
-    pathsize = utils.path_size(dir1)
-    assert pathsize == (2**18) * 8
-
-
-def test_filelist_total(dir1):
-    """
-    Test function for acquiring a filelist for directory.
-    """
-    total, _ = utils.filelist_total(dir1)
-    assert total == (2**18) * 8
-
-
-def test_piecelength_error_fixtures():
-    """
-    Test exception for uninterpretable piece length value.
-    """
-    try:
-        raise utils.PieceLengthValueError("message")
-    except utils.PieceLengthValueError:
-        assert True
-        assert dir1
-
-
-def test_missing_path_error():
-    """
-    Test exception for missing path parameter.
-    """
-    try:
-        raise utils.MissingPathError("message")
-    except utils.MissingPathError:
-        assert True
-        assert dir2
-
-
-@pytest.mark.parametrize("value", [5, 32, 18, 225, 16384, 256000])
-def test_next_power_2(value):
-    """
-    Test next power of 2 function in utils module.
-    """
-    result = utils.next_power_2(value)
-    log = math.log2(result)
-    assert log == int(log)
-    assert result % 2 == 0
-    assert result >= value
-
-
-@pytest.mark.parametrize(
-    "amount, result",
-    [
-        (1, f"{float(1)} Byte"),
-        (100, "100.0 Bytes"),
-        (1100, "1.1 KiB"),
-        (1_100_000, "1.0 MiB"),
-        (1_100_000_000, "1.0 GiB"),
-        (4_400_120_000, "4.1 GiB"),
-        (4_000_120_000, "3.7 GiB"),
-    ],
-)
-def test_humanize_bytes(amount, result):
-    """
-    Test humanize bytes function.
-    """
-    assert utils.humanize_bytes(amount) == result
-
-
-@pytest.mark.parametrize("amount, result", [(i, 2**i) for i in range(14, 25)])
-def test_normalize_piece_length_int(amount, result):
-    """Test normalize piece length function.
-
-    Parameters
-    ----------
-    amount : `str` or `int`
-        piece length or representation
-    result : int
-        expected output.
-    """
-    assert utils.normalize_piece_length(amount) == result
-
-
-@pytest.mark.parametrize("amount, result",
-                         [(str(i), 2**i) for i in range(14, 21)])
-def test_normalize_piece_length_str(amount, result):
-    """Test normalize piece length function.
-
-    Parameters
-    ----------
-    amount : `str` or `int`
-        piece length or representation
-    result : int
-        expected output.
-    """
-    assert utils.normalize_piece_length(amount) == result
-
-
-@pytest.mark.parametrize("amount",
-                         ["hello", 11, 0, 100000, 28, "zero", "fifteen"])
-def test_norm_plength_errors(amount):
-    """Test function to normalize piece length errors.
-
-    Parameters
-    ----------
-    amount : any
-        arguments intended to raise an exception.
-    """
-    try:
-        assert utils.normalize_piece_length(amount)
-    except utils.PieceLengthValueError:
-        assert True
-
-
-def test_filelisttotal_missing(dir2):
-    """Test function filelist total with missing path.
-
-    Parameters
-    ----------
-    dir2 : pytest.fixture
-        fixture containing a temporary directory
-    """
-    rmpath(dir2)
-    try:
-        utils.filelist_total(dir2)
-    except utils.MissingPathError:
-        assert True
-
-
-def test_argument_error():
-    """
-    Test Argument Error.
-
-    Raises
-    ------
-    utils.ArgumentError
-        Arg error
-    """
-    try:
-        raise utils.ArgumentError("This message raised by argument error")
-    except utils.ArgumentError:
-        assert True
+#! /usr/bin/python3
+# -*- coding: utf-8 -*-
+
+##############################################################################
+#    Copyright (C) 2021-current alexpdev
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+##############################################################################
+"""
+Unittest functions for testing torrentfile utils module.
+"""
+import math
+
+import pytest
+
+from tests import dir1, dir2, rmpath
+from torrentfile import utils
+from torrentfile.__main__ import main
+
+
+def test_main_exists():
+    """
+    Test if main exists
+    """
+    assert main
+
+
+@pytest.mark.parametrize("size", [156634528, 2**30, 67987, 16384, 8563945])
+def test_get_piece_length(size):
+    """
+    Test function for best piece length for given size.
+    """
+    value = utils.get_piece_length(size)
+    assert value % 1024 == 0
+
+
+@pytest.mark.parametrize("size", [156634528, 2**30, 67987, 16384, 8563945])
+def test_get_piece_length_max(size):
+    """
+    Test function for best piece length for given size maximum.
+    """
+    value = utils.get_piece_length(size)
+    assert value < 2**27
+
+
+@pytest.mark.parametrize("size", [156634528, 2**30, 67987, 16384, 8563945])
+def test_get_piece_length_min(size):
+    """
+    Test function for best piece length for given size minimum.
+    """
+    value = utils.get_piece_length(size)
+    assert value >= 2**14
+
+
+def test_get_path_length_mod(dir1):
+    """
+    Test function for the best piece length for provided path.
+    """
+    assert utils.path_piece_length(dir1) % (2**14) == 0
+
+
+def test_get_path_length_min(dir1):
+    """
+    Test function for getting piece length for folders min.
+    """
+    assert utils.path_piece_length(dir1) >= (2**14)
+
+
+def test_get_path_length_max(dir1):
+    """
+    Test function for getting piece length for folders max.
+    """
+    assert utils.path_piece_length(dir1) <= (2**27)
+
+
+def test_path_stat(dir1):
+    """
+    Test function for acquiring piece length information on folder.
+    """
+    _, _, piece_length = utils.path_stat(dir1)
+    assert piece_length % (2**14) == 0
+
+
+def test_path_stat_size(dir1):
+    """
+    Test function for acquiring total size information on folder.
+    """
+    _, totalsize, _ = utils.path_stat(dir1)
+    assert totalsize == (2**18) * 8
+
+
+def test_path_stat_filelist_size(dir1):
+    """
+    Test function for acquiring file list information on folder.
+    """
+    filelist, _, _ = utils.path_stat(dir1)
+    assert len(filelist) == 8
+
+
+def test_get_filelist(dir1):
+    """
+    Test function for get a list of files in a directory.
+    """
+    filelist = utils.get_file_list(dir1)
+    assert len(filelist) == 8
+
+
+def test_get_path_size(dir1):
+    """
+    Test function for getting total size of directory.
+    """
+    pathsize = utils.path_size(dir1)
+    assert pathsize == (2**18) * 8
+
+
+def test_filelist_total(dir1):
+    """
+    Test function for acquiring a filelist for directory.
+    """
+    total, _ = utils.filelist_total(dir1)
+    assert total == (2**18) * 8
+
+
+def test_piecelength_error_fixtures():
+    """
+    Test exception for uninterpretable piece length value.
+    """
+    try:
+        raise utils.PieceLengthValueError("message")
+    except utils.PieceLengthValueError:
+        assert True
+        assert dir1
+
+
+def test_missing_path_error():
+    """
+    Test exception for missing path parameter.
+    """
+    try:
+        raise utils.MissingPathError("message")
+    except utils.MissingPathError:
+        assert True
+        assert dir2
+
+
+@pytest.mark.parametrize("value", [5, 32, 18, 225, 16384, 256000])
+def test_next_power_2(value):
+    """
+    Test next power of 2 function in utils module.
+    """
+    result = utils.next_power_2(value)
+    log = math.log2(result)
+    assert log == int(log)
+    assert result % 2 == 0
+    assert result >= value
+
+
+@pytest.mark.parametrize(
+    "amount, result",
+    [
+        (1, f"{float(1)} Byte"),
+        (100, "100.0 Bytes"),
+        (1100, "1.1 KiB"),
+        (1_100_000, "1.0 MiB"),
+        (1_100_000_000, "1.0 GiB"),
+        (4_400_120_000, "4.1 GiB"),
+        (4_000_120_000, "3.7 GiB"),
+    ],
+)
+def test_humanize_bytes(amount, result):
+    """
+    Test humanize bytes function.
+    """
+    assert utils.humanize_bytes(amount) == result
+
+
+@pytest.mark.parametrize("amount, result", [(i, 2**i) for i in range(14, 25)])
+def test_normalize_piece_length_int(amount, result):
+    """Test normalize piece length function.
+
+    Parameters
+    ----------
+    amount : `str` or `int`
+        piece length or representation
+    result : int
+        expected output.
+    """
+    assert utils.normalize_piece_length(amount) == result
+
+
+@pytest.mark.parametrize("amount, result",
+                         [(str(i), 2**i) for i in range(14, 21)])
+def test_normalize_piece_length_str(amount, result):
+    """Test normalize piece length function.
+
+    Parameters
+    ----------
+    amount : `str` or `int`
+        piece length or representation
+    result : int
+        expected output.
+    """
+    assert utils.normalize_piece_length(amount) == result
+
+
+@pytest.mark.parametrize("amount",
+                         ["hello", 11, 0, 100000, 28, "zero", "fifteen"])
+def test_norm_plength_errors(amount):
+    """Test function to normalize piece length errors.
+
+    Parameters
+    ----------
+    amount : any
+        arguments intended to raise an exception.
+    """
+    try:
+        assert utils.normalize_piece_length(amount)
+    except utils.PieceLengthValueError:
+        assert True
+
+
+def test_filelisttotal_missing(dir2):
+    """Test function filelist total with missing path.
+
+    Parameters
+    ----------
+    dir2 : pytest.fixture
+        fixture containing a temporary directory
+    """
+    rmpath(dir2)
+    try:
+        utils.filelist_total(dir2)
+    except utils.MissingPathError:
+        assert True
+
+
+def test_argument_error():
+    """
+    Test Argument Error.
+
+    Raises
+    ------
+    utils.ArgumentError
+        Arg error
+    """
+    try:
+        raise utils.ArgumentError("This message raised by argument error")
+    except utils.ArgumentError:
+        assert True
```

### Comparing `torrentfile-0.9.0/torrentfile/__init__.py` & `torrentfile-0.9.1/torrentfile/__init__.py`

 * *Files identical despite different names*

### Comparing `torrentfile-0.9.0/torrentfile/__main__.py` & `torrentfile-0.9.1/torrentfile/__main__.py`

 * *Files identical despite different names*

### Comparing `torrentfile-0.9.0/torrentfile/cli.py` & `torrentfile-0.9.1/torrentfile/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,675 +1,664 @@
-#! /usr/bin/python3
-# -*- coding: utf-8 -*-
-
-##############################################################################
-#    Copyright (C) 2021-current alexpdev
-#
-#    Licensed under the Apache License, Version 2.0 (the "License");
-#    you may not use this file except in compliance with the License.
-#    You may obtain a copy of the License at
-#
-#        http://www.apache.org/licenses/LICENSE-2.0
-#
-#    Unless required by applicable law or agreed to in writing, software
-#    distributed under the License is distributed on an "AS IS" BASIS,
-#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#    See the License for the specific language governing permissions and
-#    limitations under the License.
-##############################################################################
-"""
-Command Line Interface for TorrentFile project.
-
-This module provides the primary command line argument parser for
-the torrentfile package. The main_script function is automatically
-invoked when called from command line, and parses accompanying arguments.
-
-Functions
----------
-main_script :
-    process command line arguments and run program.
-activate_logger :
-    turns on debug mode and logging facility.
-
-Classes
--------
-Config : class
-    controls logging configuration
-TorrentFileHelpFormatter : HelpFormatter
-    the command line help message formatter
-"""
-
-import io
-import sys
-import logging
-from argparse import ArgumentParser, HelpFormatter
-
-from torrentfile.commands import (
-    create, edit, get_magnet, info, rebuild, recheck, rename)
-from torrentfile.utils import toggle_debug_mode
-from torrentfile.version import __version__ as version
-
-
-class Config:
-    """
-    Class the controls the logging configuration and output settings.
-
-    Controls the logging level, or whether to app should operate in quiet mode.
-    """
-
-    @staticmethod
-    def activate_quiet():
-        """
-        Activate quiet mode for the duration of the programs life.
-
-        When quiet mode is enabled, no logging, progress or state information
-        is output to the terminal
-        """
-        if sys.stdout or sys.stderr:
-            sys.stdout = io.StringIO()
-            sys.stderr = io.StringIO()
-
-    @staticmethod
-    def activate_logger():
-        """
-        Activate the builtin logging mechanism when passed debug flag from CLI.
-        """
-        logging.basicConfig(level=logging.WARNING)
-        logger = logging.getLogger()
-        console_handler = logging.StreamHandler(stream=sys.stderr)
-        stream_formatter = logging.Formatter(
-            "[%(asctime)s] [%(levelno)s] %(message)s",
-            datefmt="%H:%M:%S",
-            style="%",
-        )
-        console_handler.setFormatter(stream_formatter)
-        console_handler.setLevel(logging.DEBUG)
-        logger.setLevel(logging.DEBUG)
-        logger.addHandler(console_handler)
-        logger.debug("Debug: ON")
-        toggle_debug_mode(True)
-
-
-class TorrentFileHelpFormatter(HelpFormatter):
-    """
-    Formatting class for help tips provided by the CLI.
-
-    Subclasses Argparse.HelpFormatter.
-    """
-
-    def __init__(self,
-                 prog: str,
-                 width: int = 45,
-                 max_help_positions: int = 45):
-        """
-        Construct HelpFormat class for usage output.
-
-        Parameters
-        ----------
-        prog : str
-            Name of the program.
-        width : int
-            Max width of help message output.
-        max_help_positions : int
-            max length until line wrap.
-        """
-        super().__init__(prog,
-                         width=width,
-                         max_help_position=max_help_positions)
-
-    def _split_lines(self, text: str, _: int) -> list:
-        """
-        Split multiline help messages and remove indentation.
-
-        Parameters
-        ----------
-        text : str
-            text that needs to be split
-        _ : int
-            max width for line.
-
-        Returns
-        -------
-        list :
-            split into multiline text list
-        """
-        lines = text.split("\n")
-        return [line.strip() for line in lines if line]
-
-    def _format_text(self, text: str) -> str:
-        """
-        Format text for cli usage messages.
-
-        Parameters
-        ----------
-        text : str
-            Pre-formatted text.
-
-        Returns
-        -------
-        str
-            Formatted text from input.
-        """
-        text = text % {"prog": self._prog} if "%(prog)" in text else text
-        text = self._whitespace_matcher.sub(" ", text).strip()
-        return text + "\n\n"
-
-    def _join_parts(self, part_strings: list) -> str:
-        """
-        Combine different sections of the help message.
-
-        Parameters
-        ----------
-        part_strings : list
-            List of argument help messages and headers.
-
-        Returns
-        -------
-        str
-            Fully formatted help message for CLI.
-        """
-        parts = self._format_headers(part_strings)
-        return super()._join_parts(parts)
-
-    @staticmethod
-    def _format_headers(parts: list) -> list:
-        """
-        Format help message section headers.
-
-        Parameters
-        ----------
-        parts : list
-            List of individual lines for help message.
-
-        Returns
-        -------
-        list
-            Input list with formatted section headers.
-        """
-        if parts and parts[0].startswith("usage:"):
-            parts[0] = "Usage\n=====\n  " + parts[0][6:]
-        headings = [i for i in range(len(parts)) if parts[i].endswith(":\n")]
-        for i in headings[::-1]:
-            parts[i] = parts[i][:-2].title()
-            underline = "".join(["\n", "-" * len(parts[i]), "\n"])
-            parts.insert(i + 1, underline)
-        return parts
-
-
-def execute(args: list = None) -> list:
-    """
-    Execute program with provided list of arguments.
-
-    If no arguments are given then it defaults to using
-    sys.argv.  This is the main entrypoint for the program
-    and command line interface.
-
-    Parameters
-    ----------
-    args : list
-        Commandline arguments. default=None
-
-    Returns
-    -------
-    list
-        Depends on what the command line args were.
-    """
-    toggle_debug_mode(False)
-    if not args:
-        if sys.argv[1:]:
-            args = sys.argv[1:]
-        else:
-            args = ["-h"]
-
-    parser = ArgumentParser(
-        "torrentfile",
-        usage="torrentfile <options>",
-        description=(
-            "Command line tools for creating, editing, checking, building "
-            "and interacting with Bittorrent meta files"),
-        prefix_chars="-",
-        formatter_class=TorrentFileHelpFormatter,
-        conflict_handler="resolve",
-    )
-
-    parser.add_argument(
-        "-q",
-        "--quiet",
-        help="Turn off all text output.",
-        dest="quiet",
-        action="store_true",
-    )
-
-    parser.add_argument(
-        "-V",
-        "--version",
-        action="version",
-        version=f"torrentfile v{version}",
-        help="show program version and exit",
-    )
-
-    parser.add_argument(
-        "-v",
-        "--verbose",
-        action="store_true",
-        dest="debug",
-        help="output debug information",
-    )
-
-    parser.set_defaults(func=parser.print_help)
-
-    subparsers = parser.add_subparsers(
-        title="Commands",
-        dest="command",
-        metavar="create, edit, info, magnet, recheck, rebuild, rename\n",
-    )
-
-    create_parser = subparsers.add_parser(
-        "create",
-        help="Create a new Bittorrent file.",
-        prefix_chars="-",
-        aliases=["c", "new"],
-        formatter_class=TorrentFileHelpFormatter,
-    )
-
-    create_parser.add_argument(
-        "-a",
-        "-t",
-        "--announce",
-        "--tracker",
-        action="store",
-        dest="announce",
-        metavar="<url>",
-        nargs="+",
-        default=[],
-        help="One or more space-seperated torrent tracker url(s).",
-    )
-
-    create_parser.add_argument(
-        "-p",
-        "--private",
-        action="store_true",
-        dest="private",
-        help="Creates private torrent with multi-tracker and DHT turned off.",
-    )
-
-    create_parser.add_argument(
-        "-s",
-        "--source",
-        action="store",
-        dest="source",
-        metavar="<source>",
-        help="Add a source string. Useful for cross-seeding.",
-    )
-
-    create_parser.add_argument(
-        "--config",
-        action="store_true",
-        dest="config",
-        help="""
-        Parse torrent information from a config file. Looks in the current
-        working directory, or the directory named .torrentfile in the users
-        home directory for a torrentfile.ini file. See --config-path option.
-        """,
-    )
-
-    create_parser.add_argument(
-        "--config-path",
-        action="store",
-        metavar="<path>",
-        dest="config_path",
-        help="""
-        Use this option in combination with -f or --config
-        options to specify location of config file.
-        """,
-    )
-
-    create_parser.add_argument(
-        "-m",
-        "--magnet",
-        action="store_true",
-        dest="magnet",
-    )
-
-    create_parser.add_argument(
-        "-c",
-        "--comment",
-        action="store",
-        dest="comment",
-        metavar="<comment>",
-        help="Include a comment in file metadata",
-    )
-
-    create_parser.add_argument(
-        "-o",
-        "--out",
-        action="store",
-        dest="outfile",
-        metavar="<path>",
-        help="Explicitly specify the path to write the file .torrent file",
-    )
-
-    create_parser.add_argument(
-        "--prog",
-        "--progress",
-        default="1",
-        action="store",
-        dest="progress",
-        metavar="<int>",
-        help="""
-        Set the progress bar level.
-        Options = 0, 1
-        (0) = Do not display progress bar.
-        (1) = Display progress bar.(default)
-        """,
-    )
-
-    create_parser.add_argument(
-        "--meta-version",
-        default="1",
-        choices=["1", "2", "3"],
-        action="store",
-        dest="meta_version",
-        metavar="<int>",
-        help="""
-        Bittorrent metafile version.
-        Options = 1, 2, 3
-        (1) = Bittorrent v1 (Default)
-        (2) = Bittorrent v2
-        (3) = Bittorrent v1 & v2 hybrid
-        """,
-    )
-
-    create_parser.add_argument(
-        "--piece-length",
-        action="store",
-        dest="piece_length",
-        metavar="<int>",
-        help="""
-        (Default: auto calculated based on total size of content) Number of
-        bytes for per chunk of data transmitted by Bittorrent client.
-        Acceptable values include integers 14-26 which will be interpreted
-        as exponent for power of 2.  e.g. 14 = 16KiB pieces.
-        Examples:: [--piece-length 14] [--piece-length 20]
-        """,
-    )
-
-    create_parser.add_argument(
-        "-w",
-        "--web-seed",
-        action="store",
-        dest="url_list",
-        metavar="<url>",
-        nargs="+",
-        help="list of web addresses where torrent data exists (GetRight).",
-    )
-
-    create_parser.add_argument(
-        "--http-seed",
-        action="store",
-        dest="httpseeds",
-        metavar="<url>",
-        nargs="+",
-        help="list of URLs, addresses where content can be found (Hoffman).",
-    )
-
-    create_parser.add_argument(
-        "content",
-        action="store",
-        metavar="<content>",
-        nargs="?",
-        help="Path to content file or directory",
-    )
-
-    create_parser.set_defaults(func=create)
-
-    edit_parser = subparsers.add_parser(
-        "edit",
-        help="""Edit existing torrent meta file.""",
-        aliases=["e"],
-        prefix_chars="-",
-        formatter_class=TorrentFileHelpFormatter,
-    )
-
-    edit_parser.add_argument(
-        "metafile",
-        action="store",
-        help="path to *.torrent file",
-        metavar="<*.torrent>",
-    )
-
-    edit_parser.add_argument(
-        "--tracker",
-        action="store",
-        dest="announce",
-        metavar="<url>",
-        nargs="+",
-        help="""
-        Replace current list of tracker/announce urls with one or more space
-        seperated Bittorrent tracker announce url(s).
-        """,
-    )
-
-    edit_parser.add_argument(
-        "--web-seed",
-        action="store",
-        dest="url_list",
-        metavar="<url>",
-        nargs="+",
-        help="Replace current list of web-seed urls with one or more url(s)",
-    )
-
-    edit_parser.add_argument(
-        "--http-seed",
-        action="store",
-        dest="httpseeds",
-        metavar="<url>",
-        nargs="+",
-        help="replace all currently listed addresses with new list (Hoffman).",
-    )
-
-    edit_parser.add_argument(
-        "--private",
-        action="store_true",
-        help="Make torrent private.",
-        dest="private",
-    )
-
-    edit_parser.add_argument(
-        "--comment",
-        help="Replaces any existing comment with <comment>",
-        metavar="<comment>",
-        dest="comment",
-        action="store",
-    )
-
-    edit_parser.add_argument(
-        "--source",
-        action="store",
-        dest="source",
-        metavar="<source>",
-        help="Replaces current source with <source>",
-    )
-
-    edit_parser.set_defaults(func=edit)
-
-    info_parser = subparsers.add_parser(
-        "info",
-        help="Show detailed information about a torrent file.",
-        aliases=["i"],
-        prefix_chars="-",
-        formatter_class=TorrentFileHelpFormatter,
-    )
-
-    info_parser.add_argument(
-        "metafile",
-        action="store",
-        metavar="<*.torrent>",
-        help="path to pre-existing torrent file.",
-    )
-
-    info_parser.set_defaults(func=info)
-
-    magnet_parser = subparsers.add_parser(
-        "magnet",
-        help="Generate magnet url from an existing Bittorrent meta file.",
-        aliases=["m"],
-        prefix_chars="-",
-        formatter_class=TorrentFileHelpFormatter,
-    )
-
-    magnet_parser.add_argument(
-        "metafile",
-        action="store",
-        help="Path to Bittorrent meta file.",
-        metavar="<*.torrent>",
-    )
-
-    magnet_parser.add_argument(
-        "--meta-version",
-        action="store",
-        choices=["0", "1", "2", "3"],
-        default="0",
-        help="""
-        This option is only relevant for hybrid torrent files.
-        Options = 0, 1, 2, 3
-        (0) = [default] version is determined automatically
-        (1) = create V1 magnet link only
-        (2) = create V2 magnet link only
-        (3) = create a hybrid magnet link
-        """,
-        dest="meta_version",
-        metavar="<int>",
-    )
-
-    magnet_parser.set_defaults(func=get_magnet)
-
-    check_parser = subparsers.add_parser(
-        "recheck",
-        help="Gives a detailed look at how much of the torrent is available.",
-        aliases=["check", "r"],
-        prefix_chars="-",
-        formatter_class=TorrentFileHelpFormatter,
-    )
-
-    check_parser.add_argument(
-        "metafile",
-        action="store",
-        metavar="<*.torrent>",
-        help="path to .torrent file.",
-    )
-
-    check_parser.add_argument(
-        "content",
-        action="store",
-        metavar="<content>",
-        help="path to content file or directory",
-    )
-
-    check_parser.set_defaults(func=recheck)
-
-    rebuild_parser = subparsers.add_parser(
-        "rebuild",
-        help="""
-        Re-assemble files obtained from a bittorrent file into the
-        appropriate file structure for re-seeding.  Read documentation
-        for more information, or use cases.
-        """,
-        formatter_class=TorrentFileHelpFormatter,
-    )
-
-    rebuild_parser.add_argument(
-        "-m",
-        "--metafiles",
-        action="store",
-        metavar="<*.torrent>",
-        nargs="+",
-        dest="metafiles",
-        required=True,
-        help="path(s) to .torrent file(s)/folder(s) containing .torrent files",
-    )
-
-    rebuild_parser.add_argument(
-        "-c"
-        "--contents",
-        action="store",
-        dest="contents",
-        nargs="+",
-        required=True,
-        metavar="<contents>",
-        help="folders that might contain the source contents needed to rebuld",
-    )
-
-    rebuild_parser.add_argument(
-        "-d",
-        "--destination",
-        action="store",
-        dest="destination",
-        required=True,
-        metavar="<destination>",
-        help="path to where torrents will be re-assembled",
-    )
-
-    rebuild_parser.set_defaults(func=rebuild)
-
-    rename_parser = subparsers.add_parser(
-        "rename",
-        help="""Rename a torrent file to it's original name provided in the
-                metadata/the same name you see in your torrent client.""",
-        formatter_class=TorrentFileHelpFormatter,
-    )
-
-    rename_parser.add_argument(
-        "target",
-        action="store",
-        metavar="<target>",
-        help="path to file that needs renaming.",
-    )
-
-    rename_parser.set_defaults(func=rename)
-
-    all_commands = [
-        "c",
-        "e",
-        "i",
-        "m",
-        "r",
-        "-i",
-        "-h",
-        "-V",
-        "new",
-        "edit",
-        "info",
-        "check",
-        "create",
-        "magnet",
-        "rename",
-        "rebuild",
-        "recheck",
-    ]
-    if not any(i for i in all_commands if i in args):
-        start = 0
-        while args[start] in ["-v", "-q"]:
-            start += 1
-        args.insert(start, "create")
-
-    args = parser.parse_args(args)
-
-    if args.quiet:
-        Config.activate_quiet()
-
-    elif args.debug:
-        Config.activate_logger()
-
-    if hasattr(args, "func"):
-        return args.func(args)
-    return args  # pragma: nocover
-
-
-main_script = execute
-
-
-def main() -> None:
-    """
-    Initiate main function for CLI script.
-    """
-    execute()
+#! /usr/bin/python3
+# -*- coding: utf-8 -*-
+
+##############################################################################
+#    Copyright (C) 2021-current alexpdev
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+##############################################################################
+"""
+Command Line Interface for TorrentFile project.
+
+This module provides the primary command line argument parser for
+the torrentfile package. The main_script function is automatically
+invoked when called from command line, and parses accompanying arguments.
+
+Functions
+---------
+main_script :
+    process command line arguments and run program.
+activate_logger :
+    turns on debug mode and logging facility.
+
+Classes
+-------
+Config : class
+    controls logging configuration
+TorrentFileHelpFormatter : HelpFormatter
+    the command line help message formatter
+"""
+
+import io
+import sys
+import logging
+from argparse import ArgumentParser, HelpFormatter
+
+from torrentfile import commands
+from torrentfile.utils import toggle_debug_mode
+from torrentfile.version import __version__ as version
+
+
+class Config:
+    """
+    Class the controls the logging configuration and output settings.
+
+    Controls the logging level, or whether to app should operate in quiet mode.
+    """
+
+    @staticmethod
+    def activate_quiet():
+        """
+        Activate quiet mode for the duration of the programs life.
+
+        When quiet mode is enabled, no logging, progress or state information
+        is output to the terminal
+        """
+        if sys.stdout or sys.stderr:
+            sys.stdout = io.StringIO()
+            sys.stderr = io.StringIO()
+
+    @staticmethod
+    def activate_logger():
+        """
+        Activate the builtin logging mechanism when passed debug flag from CLI.
+        """
+        logging.basicConfig(level=logging.WARNING)
+        logger = logging.getLogger()
+        console_handler = logging.StreamHandler(stream=sys.stderr)
+        stream_formatter = logging.Formatter(
+            "[%(asctime)s] [%(levelno)s] %(message)s",
+            datefmt="%H:%M:%S",
+            style="%",
+        )
+        console_handler.setFormatter(stream_formatter)
+        console_handler.setLevel(logging.DEBUG)
+        logger.setLevel(logging.DEBUG)
+        logger.addHandler(console_handler)
+        logger.debug("Debug: ON")
+        toggle_debug_mode(True)
+
+
+class TorrentFileHelpFormatter(HelpFormatter):
+    """
+    Formatting class for help tips provided by the CLI.
+
+    Subclasses Argparse.HelpFormatter.
+    """
+
+    def __init__(self,
+                 prog: str,
+                 width: int = 45,
+                 max_help_positions: int = 45):
+        """
+        Construct HelpFormat class for usage output.
+
+        Parameters
+        ----------
+        prog : str
+            Name of the program.
+        width : int
+            Max width of help message output.
+        max_help_positions : int
+            max length until line wrap.
+        """
+        super().__init__(prog,
+                         width=width,
+                         max_help_position=max_help_positions)
+
+    def _split_lines(self, text: str, _: int) -> list:
+        """
+        Split multiline help messages and remove indentation.
+
+        Parameters
+        ----------
+        text : str
+            text that needs to be split
+        _ : int
+            max width for line.
+
+        Returns
+        -------
+        list :
+            split into multiline text list
+        """
+        lines = text.split("\n")
+        return [line.strip() for line in lines if line]
+
+    def _format_text(self, text: str) -> str:
+        """
+        Format text for cli usage messages.
+
+        Parameters
+        ----------
+        text : str
+            Pre-formatted text.
+
+        Returns
+        -------
+        str
+            Formatted text from input.
+        """
+        text = text % {"prog": self._prog} if "%(prog)" in text else text
+        text = self._whitespace_matcher.sub(" ", text).strip()
+        return text + "\n\n"
+
+    def _join_parts(self, part_strings: list) -> str:
+        """
+        Combine different sections of the help message.
+
+        Parameters
+        ----------
+        part_strings : list
+            List of argument help messages and headers.
+
+        Returns
+        -------
+        str
+            Fully formatted help message for CLI.
+        """
+        parts = self._format_headers(part_strings)
+        return super()._join_parts(parts)
+
+    @staticmethod
+    def _format_headers(parts: list) -> list:
+        """
+        Format help message section headers.
+
+        Parameters
+        ----------
+        parts : list
+            List of individual lines for help message.
+
+        Returns
+        -------
+        list
+            Input list with formatted section headers.
+        """
+        if parts and parts[0].startswith("usage:"):
+            parts[0] = "Usage\n=====\n  " + parts[0][6:]
+        headings = [i for i in range(len(parts)) if parts[i].endswith(":\n")]
+        for i in headings[::-1]:
+            parts[i] = parts[i][:-2].title()
+            underline = "".join(["\n", "-" * len(parts[i]), "\n"])
+            parts.insert(i + 1, underline)
+        return parts
+
+
+def execute(args: list = None) -> list:
+    """
+    Execute program with provided list of arguments.
+
+    If no arguments are given then it defaults to using
+    sys.argv.  This is the main entrypoint for the program
+    and command line interface.
+
+    Parameters
+    ----------
+    args : list
+        Commandline arguments. default=None
+
+    Returns
+    -------
+    list
+        Depends on what the command line args were.
+    """
+    toggle_debug_mode(False)
+    if not args:
+        if sys.argv[1:]:
+            args = sys.argv[1:]
+        else:
+            args = ["-h"]
+
+    parser = ArgumentParser(
+        "torrentfile",
+        usage="torrentfile <options>",
+        description=(
+            "Command line tool for creating, editing, validating, building "
+            "and interacting with all versions of Bittorrent files"),
+        prefix_chars="-",
+        formatter_class=TorrentFileHelpFormatter,
+        conflict_handler="resolve",
+    )
+
+    parser.add_argument(
+        "-q",
+        "--quiet",
+        help="Turn off all text output.",
+        dest="quiet",
+        action="store_true",
+    )
+
+    parser.add_argument(
+        "-V",
+        "--version",
+        action="version",
+        version=f"torrentfile v{version}",
+        help="show program version and exit",
+    )
+
+    parser.add_argument(
+        "-v",
+        "--verbose",
+        action="store_true",
+        dest="debug",
+        help="output debug information",
+    )
+
+    parser.set_defaults(func=parser.print_help)
+
+    subparsers = parser.add_subparsers(
+        title="Commands",
+        dest="command",
+        metavar="create, edit, info, magnet, recheck, rebuild, rename\n",
+    )
+
+    create_parser = subparsers.add_parser(
+        "create",
+        help="Create a new Bittorrent file.",
+        prefix_chars="-",
+        aliases=["new"],
+        formatter_class=TorrentFileHelpFormatter,
+    )
+
+    create_parser.add_argument(
+        "-a",
+        "--announce",
+        "--tracker",
+        action="store",
+        dest="announce",
+        metavar="<url>",
+        nargs="+",
+        default=[],
+        help="one or more space-seperated tracker url(s)",
+    )
+
+    create_parser.add_argument(
+        "-p",
+        "--private",
+        action="store_true",
+        dest="private",
+        help="create private torrent",
+    )
+
+    create_parser.add_argument(
+        "-s",
+        "--source",
+        action="store",
+        dest="source",
+        metavar="<source>",
+        help="add source field to the metadata",
+    )
+
+    create_parser.add_argument(
+        "--config",
+        action="store_true",
+        dest="config",
+        help="""
+        Parse torrent information from a config file. Looks in the current
+        working directory, or the directory named .torrentfile in the users
+        home directory for a torrentfile.ini file. See --config-path option.
+        """,
+    )
+
+    create_parser.add_argument(
+        "--config-path",
+        action="store",
+        metavar="<path>",
+        dest="config_path",
+        help="use in combination with --config to provide config file path",
+    )
+
+    create_parser.add_argument(
+        "-m",
+        "--magnet",
+        action="store_true",
+        dest="magnet",
+    )
+
+    create_parser.add_argument(
+        "-c",
+        "--comment",
+        action="store",
+        dest="comment",
+        metavar="<comment>",
+        help="include a comment in the torrent file metadata",
+    )
+
+    create_parser.add_argument(
+        "-o",
+        "--out",
+        action="store",
+        dest="outfile",
+        metavar="<path>",
+        help="path to write torrent file",
+    )
+
+    create_parser.add_argument(
+        "--prog",
+        "--progress",
+        default="1",
+        action="store",
+        dest="progress",
+        metavar="<int>",
+        help="""
+        set the progress bar level
+        Options = 0, 1
+        (0) = Do not display progress bar.
+        (1) = Display progress bar.(default)
+        """,
+    )
+
+    create_parser.add_argument(
+        "--meta-version",
+        default="1",
+        choices=["1", "2", "3"],
+        action="store",
+        dest="meta_version",
+        metavar="<int>",
+        help="""
+        bittorrent metafile version
+        options = 1, 2, 3
+        (1) = Bittorrent v1 (Default)
+        (2) = Bittorrent v2
+        (3) = Bittorrent v1 & v2 hybrid
+        """,
+    )
+
+    create_parser.add_argument(
+        "--piece-length",
+        action="store",
+        dest="piece_length",
+        metavar="<int>",
+        help="""
+        (Default: auto calculated based on total size of content)
+        acceptable values include numbers 14-26
+        14 = 16KiB, 20 = 1MiB, 21 = 2MiB etc.  Examples:[--piece-length 14]
+        """,
+    )
+
+    create_parser.add_argument(
+        "--web-seed",
+        action="store",
+        dest="url_list",
+        metavar="<url>",
+        nargs="+",
+        help="list of web addresses where torrent data exists (GetRight)",
+    )
+
+    create_parser.add_argument(
+        "--http-seed",
+        action="store",
+        dest="httpseeds",
+        metavar="<url>",
+        nargs="+",
+        help="list of URLs, addresses where content can be found (Hoffman)",
+    )
+
+    create_parser.add_argument(
+        "--align",
+        action="store_true",
+        help=("Align pieces to file boundaries. "
+              "This option is ignored when not used with V1 torrents."),
+    )
+
+    create_parser.add_argument(
+        "content",
+        action="store",
+        metavar="<content>",
+        nargs="?",
+        help="path to content file or directory",
+    )
+
+    create_parser.set_defaults(func=commands.create)
+
+    edit_parser = subparsers.add_parser(
+        "edit",
+        help="edit torrent file",
+        prefix_chars="-",
+        formatter_class=TorrentFileHelpFormatter,
+    )
+
+    edit_parser.add_argument(
+        "metafile",
+        action="store",
+        help="path to *.torrent file",
+        metavar="<*.torrent>",
+    )
+
+    edit_parser.add_argument(
+        "--tracker",
+        action="store",
+        dest="announce",
+        metavar="<url>",
+        nargs="+",
+        help="replace current trackers with one or more urls",
+    )
+
+    edit_parser.add_argument(
+        "--web-seed",
+        action="store",
+        dest="url_list",
+        metavar="<url>",
+        nargs="+",
+        help="replace current web-seed with one or more url(s)",
+    )
+
+    edit_parser.add_argument(
+        "--http-seed",
+        action="store",
+        dest="httpseeds",
+        metavar="<url>",
+        nargs="+",
+        help="replace current http-seed urls with new ones (Hoffman)",
+    )
+
+    edit_parser.add_argument(
+        "--private",
+        action="store_true",
+        help="make torrent private",
+        dest="private",
+    )
+
+    edit_parser.add_argument(
+        "--comment",
+        help="replaces any existing comment with <comment>",
+        metavar="<comment>",
+        dest="comment",
+        action="store",
+    )
+
+    edit_parser.add_argument(
+        "--source",
+        action="store",
+        dest="source",
+        metavar="<source>",
+        help="replaces current source with <source>",
+    )
+
+    edit_parser.set_defaults(func=commands.edit)
+
+    info_parser = subparsers.add_parser(
+        "info",
+        help="show detailed information about a torrent file",
+        prefix_chars="-",
+        formatter_class=TorrentFileHelpFormatter,
+    )
+
+    info_parser.add_argument(
+        "metafile",
+        action="store",
+        metavar="<*.torrent>",
+        help="path to torrent file",
+    )
+
+    info_parser.set_defaults(func=commands.info)
+
+    magnet_parser = subparsers.add_parser(
+        "magnet",
+        help="generate magnet url from an existing torrent file",
+        aliases=["m"],
+        prefix_chars="-",
+        formatter_class=TorrentFileHelpFormatter,
+    )
+
+    magnet_parser.add_argument(
+        "metafile",
+        action="store",
+        help="path to torrent file",
+        metavar="<*.torrent>",
+    )
+
+    magnet_parser.add_argument(
+        "--meta-version",
+        action="store",
+        choices=["0", "1", "2", "3"],
+        default="0",
+        help="""
+        This option is only relevant for hybrid torrent files.
+        Options = 0, 1, 2, 3
+        (0) = [default] version is determined automatically
+        (1) = create V1 magnet link only
+        (2) = create V2 magnet link only
+        (3) = create a hybrid magnet link
+        """,
+        dest="meta_version",
+        metavar="<int>",
+    )
+
+    magnet_parser.set_defaults(func=commands.get_magnet)
+
+    check_parser = subparsers.add_parser(
+        "recheck",
+        help="gives a detailed look at how much of the torrent is available",
+        aliases=["check"],
+        prefix_chars="-",
+        formatter_class=TorrentFileHelpFormatter,
+    )
+
+    check_parser.add_argument(
+        "metafile",
+        action="store",
+        metavar="<*.torrent>",
+        help="path to .torrent file.",
+    )
+
+    check_parser.add_argument(
+        "content",
+        action="store",
+        metavar="<content>",
+        help="path to content file or directory",
+    )
+
+    check_parser.set_defaults(func=commands.recheck)
+
+    rebuild_parser = subparsers.add_parser(
+        "rebuild",
+        help="""
+        Re-assemble files obtained from a bittorrent file into the
+        appropriate file structure for re-seeding.  Read documentation
+        for more information, or use cases.
+        """,
+        formatter_class=TorrentFileHelpFormatter,
+    )
+
+    rebuild_parser.add_argument(
+        "-m",
+        "--metafiles",
+        action="store",
+        metavar="<*.torrent>",
+        nargs="+",
+        dest="metafiles",
+        required=True,
+        help="path(s) to .torrent file(s)/folder(s) containing .torrent files",
+    )
+
+    rebuild_parser.add_argument(
+        "-c"
+        "--contents",
+        action="store",
+        dest="contents",
+        nargs="+",
+        required=True,
+        metavar="<contents>",
+        help="folders that might contain the source contents needed to rebuld",
+    )
+
+    rebuild_parser.add_argument(
+        "-d",
+        "--destination",
+        action="store",
+        dest="destination",
+        required=True,
+        metavar="<destination>",
+        help="path to where torrents will be re-assembled",
+    )
+
+    rebuild_parser.set_defaults(func=commands.rebuild)
+
+    rename_parser = subparsers.add_parser(
+        "rename",
+        help="""Rename a torrent file to it's original name provided in the
+                metadata/the same name you see in your torrent client.""",
+        formatter_class=TorrentFileHelpFormatter,
+    )
+
+    rename_parser.add_argument(
+        "target",
+        action="store",
+        metavar="<target>",
+        help="path to torrent file",
+    )
+
+    rename_parser.set_defaults(func=commands.rename)
+
+    all_commands = [
+        "m",
+        "-h",
+        "-V",
+        "new",
+        "edit",
+        "info",
+        "check",
+        "create",
+        "magnet",
+        "rename",
+        "rebuild",
+        "recheck",
+    ]
+    if not any(i for i in all_commands if i in args):
+        start = 0
+        while args[start] in ["-v", "-q"]:
+            start += 1
+        args.insert(start, "create")
+
+    args = parser.parse_args(args)
+
+    if args.quiet:
+        Config.activate_quiet()
+
+    elif args.debug:
+        Config.activate_logger()
+
+    if hasattr(args, "func"):
+        return args.func(args)
+    return args  # pragma: nocover
+
+
+main_script = execute
+
+
+def main() -> None:
+    """
+    Initiate main function for CLI script.
+    """
+    execute()
```

### Comparing `torrentfile-0.9.0/torrentfile/commands.py` & `torrentfile-0.9.1/torrentfile/commands.py`

 * *Files identical despite different names*

### Comparing `torrentfile-0.9.0/torrentfile/edit.py` & `torrentfile-0.9.1/torrentfile/edit.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,22 +21,14 @@
 
 Provides a facility by which certain properties of a torrent meta file can be
 edited by the user. The various command line arguments indicate which fields
 should be edited, and what the new value should be.  Depending on what fields
 are chosen to edit, this command can trigger a new info hash which means the
 torrent will no longer be able to participate in the same swarm as the original
 unedited torrent.
-
-Keywords
---------
-private
-comment
-source
-trackers
-web-seeds
 """
 
 import os
 import logging
 
 import pyben
```

### Comparing `torrentfile-0.9.0/torrentfile/hasher.py` & `torrentfile-0.9.1/torrentfile/hasher.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,18 +47,25 @@
         List of files.
     piece_length : int
         Size of chuncks to split the data into.
     progress : int
         default = None
     """
 
-    def __init__(self, paths: list, piece_length: int, progress: bool = True):
+    def __init__(
+        self,
+        paths: list,
+        piece_length: int,
+        progress: bool = True,
+        align: bool = False,
+    ):
         """Generate hashes of piece length data from filelist contents."""
         self.piece_length = piece_length
         self.paths = paths
+        self.align = align
         self.progress = progress
         self.total = sum(os.path.getsize(i) for i in self.paths)
         self.index = 0
         self.current = open(self.paths[0], "rb")
         if self.progress:
             total = os.path.getsize(self.paths[0])
             self.prog_start(total, self.paths[0])
@@ -85,14 +92,20 @@
             Incomplete piece containing partial data
 
         Returns
         -------
         digest : bytearray
             SHA1 digest of the complete piece.
         """
+        if self.align:
+            target = self.piece_length - len(arr)
+            temp = bytearray(target)
+            arr.extend(temp)
+            return sha1(arr).digest()  # nosec
+
         while len(arr) < self.piece_length and self.next_file():
             target = self.piece_length - len(arr)
             temp = bytearray(target)
             size = self.current.readinto(temp)
             arr.extend(temp[:size])
             self.prog_update(size)
             if size == target:
@@ -202,15 +215,15 @@
 
     def process_file(self, fd: str):
         """
         Calculate hashes over 16KiB chuncks of file content.
 
         Parameters
         ----------
-        fd : TextIOWrapper
+        fd : BytesIO
             Opened file in read mode.
         """
         while True:
             blocks = []
             leaf = bytearray(BLOCK_SIZE)
             # generate leaves of merkle tree
```

### Comparing `torrentfile-0.9.0/torrentfile/interactive.py` & `torrentfile-0.9.1/torrentfile/interactive.py`

 * *Files identical despite different names*

### Comparing `torrentfile-0.9.0/torrentfile/mixins.py` & `torrentfile-0.9.1/torrentfile/mixins.py`

 * *Files identical despite different names*

### Comparing `torrentfile-0.9.0/torrentfile/rebuild.py` & `torrentfile-0.9.1/torrentfile/rebuild.py`

 * *Files identical despite different names*

### Comparing `torrentfile-0.9.0/torrentfile/recheck.py` & `torrentfile-0.9.1/torrentfile/recheck.py`

 * *Files identical despite different names*

### Comparing `torrentfile-0.9.0/torrentfile/torrent.py` & `torrentfile-0.9.1/torrentfile/torrent.py`

 * *Files 3% similar despite different names*

```diff
@@ -251,14 +251,15 @@
             cls.hasher.set_callback(func)
 
     def __init__(
         self,
         path=None,
         announce=None,
         comment=None,
+        align=False,
         piece_length=None,
         private=False,
         outfile=None,
         source=None,
         progress=1,
         cwd=False,
         httpseeds=None,
@@ -295,15 +296,15 @@
 
         # base path to torrent content.
         self.path = path
 
         logger.debug("path parameter found %s", path)
 
         self.meta = {
-            "created by": f"TorrentFile_v{version}",
+            "created by": f"torrentfile_v{version}",
             "creation date": int(datetime.timestamp(datetime.now())),
             "info": {},
         }
 
         # Format piece_length attribute.
         if piece_length:
             self.piece_length = utils.normalize_piece_length(piece_length)
@@ -319,14 +320,16 @@
         # Most torrent clients have editting trackers as a feature.
         elif isinstance(announce, str):
             self.announce, self.announce_list = announce, [[announce]]
 
         elif isinstance(announce, Sequence):
             self.announce, self.announce_list = announce[0], [announce]
 
+        self.align = align
+
         if self.announce:
             self.meta["announce"] = self.announce
             self.meta["announce-list"] = self.announce_list
         if comment:
             self.meta["info"]["comment"] = comment
             logger.debug("comment parameter found %s", comment)
         if private:
@@ -441,24 +444,44 @@
         dict
             metadata dictionary for torrent file
         """
         info = self.meta["info"]
         size, filelist = utils.filelist_total(self.path)
         if os.path.isfile(self.path):
             info["length"] = size
-        else:
+        elif not self.align:
             info["files"] = [{
                 "length":
                 os.path.getsize(path),
                 "path":
                 os.path.relpath(path, self.path).split(os.sep),
             } for path in filelist]
+        else:
+            info["files"] = []
+            for path in filelist:
+                filesize = os.path.getsize(path)
+                info["files"].append({
+                    "length":
+                    filesize,
+                    "path":
+                    os.path.relpath(path, self.path).split(os.sep),
+                })
+                if filesize < self.piece_length:
+                    remainder = self.piece_length - filesize
+                else:
+                    remainder = filesize % self.piece_length
+                if remainder:
+                    info["files"].append({
+                        "attr": "p",
+                        "length": remainder,
+                        "path": [".pad", str(remainder)],
+                    })
         pieces = bytearray()
 
-        feeder = Hasher(filelist, self.piece_length, self.progress)
+        feeder = Hasher(filelist, self.piece_length, self.progress, self.align)
         for piece in feeder:
             pieces.extend(piece)
 
         info["pieces"] = pieces
 
 
 class TorrentFileV2(MetaFile, ProgMixin):
```

### Comparing `torrentfile-0.9.0/torrentfile/utils.py` & `torrentfile-0.9.1/torrentfile/utils.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,442 +1,442 @@
-#! /usr/bin/python3
-# -*- coding: utf-8 -*-
-
-##############################################################################
-#    Copyright (C) 2021-current alexpdev
-#
-#    Licensed under the Apache License, Version 2.0 (the "License");
-#    you may not use this file except in compliance with the License.
-#    You may obtain a copy of the License at
-#
-#        http://www.apache.org/licenses/LICENSE-2.0
-#
-#    Unless required by applicable law or agreed to in writing, software
-#    distributed under the License is distributed on an "AS IS" BASIS,
-#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#    See the License for the specific language governing permissions and
-#    limitations under the License.
-##############################################################################
-"""
-Utility functions and classes used throughout package.
-"""
-
-import os
-import math
-import shutil
-from pathlib import Path
-
-
-class Memo:
-    """
-    Memoize cache.
-
-    Parameters
-    ----------
-    func : Callable
-        The results of this callable will be cached.
-    """
-
-    def __init__(self, func):
-        """
-        Construcor for cache.
-        """
-        self.func = func
-        self.counter = 0
-        self.cache = {}
-
-    def __call__(self, path: str):
-        """
-        Invoke each time memo function is called.
-
-        Parameters
-        ----------
-        path : str
-            The relative or absolute path being used as key in cache dict.
-
-        Returns
-        -------
-        Any :
-            The results of calling the function with path.
-        """
-        if path in self.cache and os.path.exists(path):
-            self.counter += 1
-            return self.cache[path]
-        result = self.func(path)
-        self.cache[path] = result
-        return result
-
-
-class MissingPathError(Exception):
-    """
-    Path parameter is required to specify target content.
-
-    Creating a .torrent file with no contents seems rather silly.
-
-    Parameters
-    ----------
-    message : str
-        Message for user (optional).
-    """
-
-    def __init__(self, message: str = None):
-        """
-        Raise when creating a meta file without specifying target content.
-
-        The `message` argument is a message to pass to Exception base class.
-        """
-        self.message = f"Path arguement is missing and required {str(message)}"
-        super().__init__(message)
-
-
-class PieceLengthValueError(Exception):
-    """
-    Piece Length parameter must equal a perfect power of 2.
-
-    Parameters
-    ----------
-    message : str
-        Message for user (optional).
-    """
-
-    def __init__(self, message: str = None):
-        """
-        Raise when creating a meta file with incorrect piece length value.
-
-        The `message` argument is a message to pass to Exception base class.
-        """
-        self.message = f"Incorrect value for piece length: {str(message)}"
-        super().__init__(message)
-
-
-class ArgumentError(Exception):
-    """
-    Exception for mismatched or mistyped CLI arguments.
-    """
-
-
-SUFFIXES = ["KiB", "MiB", "GiB", "TiB", "PiB", "EiB", "ZiB", "YiB"]
-
-
-def humanize_bytes(amount: int) -> str:
-    """
-    Convert integer into human readable memory sized denomination.
-
-    Parameters
-    ----------
-    amount : int
-        total number of bytes.
-
-    Returns
-    -------
-    str
-        human readable representation of the given amount of bytes.
-    """
-    base = 1024
-    amount = float(amount)
-    value = abs(amount)
-    if value == 1:
-        return f"{amount} Byte"
-    if value < base:
-        return f"{amount} Bytes"
-    for i, s in enumerate(SUFFIXES):
-        unit = base**(i + 2)
-        if value < unit:
-            break
-    value = base * amount / unit
-    return f"{value:.1f} {s}"
-
-
-def normalize_piece_length(piece_length: int) -> int:
-    """
-    Verify input piece_length is valid and convert accordingly.
-
-    Parameters
-    ----------
-    piece_length : int | str
-        The piece length provided by user.
-
-    Returns
-    -------
-    int
-        normalized piece length.
-
-    Raises
-    ------
-    PieceLengthValueError :
-        Piece length is improper value.
-    """
-    if isinstance(piece_length, str):
-        if piece_length.isnumeric():
-            piece_length = int(piece_length)
-        else:
-            raise PieceLengthValueError(piece_length)
-
-    if piece_length > (1 << 14):
-        if 2**math.log2(piece_length) == piece_length:
-            return piece_length
-        raise PieceLengthValueError(piece_length)
-
-    if 13 < piece_length < 26:
-        return 2**piece_length
-    if piece_length <= 13:
-        raise PieceLengthValueError(piece_length)
-
-    log = int(math.log2(piece_length))
-    if 2**log == piece_length:
-        return piece_length
-    raise PieceLengthValueError
-
-
-def get_piece_length(size: int) -> int:
-    """
-    Calculate the ideal piece length for bittorrent data.
-
-    Parameters
-    ----------
-    size : int
-        Total bits of all files incluided in .torrent file.
-
-    Returns
-    -------
-    int
-        Ideal piece length.
-    """
-    exp = 14
-    while size / (2**exp) > 1000 and exp < 24:
-        exp += 1
-    return 2**exp
-
-
-@Memo
-def filelist_total(pathstring: str) -> os.PathLike:
-    """
-    Perform error checking and format conversion to os.PathLike.
-
-    Parameters
-    ----------
-    pathstring : str
-        An existing filesystem path.
-
-    Returns
-    -------
-    os.PathLike
-        Input path converted to bytes format.
-
-    Raises
-    ------
-    MissingPathError
-        File could not be found.
-    """
-    if os.path.exists(pathstring):
-        path = Path(pathstring)
-        return _filelist_total(path)
-    raise MissingPathError
-
-
-def _filelist_total(path: os.PathLike) -> tuple:
-    """
-    Recursively search directory tree for files.
-
-    Parameters
-    ----------
-    path : str
-        Path to file or directory base
-
-    Returns
-    -------
-    Tuple[int, List] :
-        int - sum of sizes for all files collected
-        list - all file paths within directory tree
-    """
-    if path.is_file():
-        file_size = os.path.getsize(path)
-        return file_size, [str(path)]
-    total = 0
-    filelist = []
-    if path.is_dir():
-        for item in path.iterdir():
-            size, paths = filelist_total(item)
-            total += size
-            filelist.extend(paths)
-    return total, sorted(filelist)
-
-
-def path_size(path: str) -> int:
-    """
-    Return the total size of all files in path recursively.
-
-    Parameters
-    ----------
-    path : str
-        path to target file or directory.
-
-    Returns
-    -------
-    int
-        total size of files.
-    """
-    total_size, _ = filelist_total(path)
-    return total_size
-
-
-def get_file_list(path: str) -> list:
-    """
-    Return a sorted list of file paths contained in directory.
-
-    Parameters
-    ----------
-    path : str
-        target file or directory.
-
-    Returns
-    -------
-    list :
-        sorted list of file paths.
-    """
-    _, filelist = filelist_total(path)
-    return filelist
-
-
-def path_stat(path: str) -> tuple:
-    """
-    Calculate directory statistics.
-
-    Parameters
-    ----------
-    path : str
-        The path to start calculating from.
-
-    Returns
-    -------
-    Tuple[list, int, int] :
-        list - List of all files contained in Directory
-        int - Total sum of bytes from all contents of dir
-        int - The size of pieces of the torrent contents.
-    """
-    total_size, filelist = filelist_total(path)
-    piece_length = get_piece_length(total_size)
-    return (filelist, total_size, piece_length)
-
-
-def path_piece_length(path: str) -> int:
-    """
-    Calculate piece length for input path and contents.
-
-    Parameters
-    ----------
-    path : str
-        The absolute path to directory and contents.
-
-    Returns
-    -------
-    int
-        The size of pieces of torrent content.
-    """
-    psize = path_size(path)
-    return get_piece_length(psize)
-
-
-def next_power_2(value: int) -> int:
-    """
-    Calculate the next perfect power of 2 equal to or greater than value.
-
-    Parameters
-    ----------
-    value : int
-        integer value that is less than some perfect power of 2.
-
-    Returns
-    -------
-    int
-        The next power of 2 greater than value, or value if already power of 2.
-    """
-    if not value & (value - 1) and value:
-        return value
-    start = 1
-    while start < value:
-        start <<= 1
-    return start
-
-
-def copypath(source: str, dest: str) -> None:
-    """
-    Copy the file located at source to dest.
-
-    If one or more directory paths don't exist in dest, they will be created.
-    If dest already exists and dest and source are the same size, it will be
-    ignored, however if dest is smaller than source, dest will be overwritten.
-
-    Parameters
-    ----------
-    source : str
-        path to source file
-    dest : str
-        path to target destination
-    """
-    if not os.path.exists(source) or (os.path.exists(dest)
-                                      and os.path.getsize(source)
-                                      <= os.path.getsize(dest)):
-        return
-    path_parts = Path(dest).parts
-    if len(path_parts) > 1:
-        root = path_parts[0]
-        path_parts = path_parts[1:-1]
-        if not os.path.exists(root):
-            os.mkdir(root)  # pragma: nocover
-        for part in path_parts:
-            path = os.path.join(root, part)
-            if not os.path.exists(path):
-                os.mkdir(path)
-            root = path
-        shutil.copy(source, dest)
-
-
-def toggle_debug_mode(switch_on: bool):
-    """
-    Switch the environment variable debug indicator on or off.
-
-    Parameters
-    ----------
-    switch_on : bool
-        if true turn debug mode on otherwise off
-    """
-    os.environ["TORRENTFILE_DEBUG"] = "ON" if switch_on else "OFF"
-
-
-def debug_is_on() -> bool:
-    """
-    Return True if debug mode is on in environment variables.
-
-    Returns
-    -------
-    bool
-        is debug mode on
-    """
-    return os.environ["TORRENTFILE_DEBUG"] == "ON"
-
-
-def check_path_writable(path: str) -> bool:
-    """
-    Test if output path is writable.
-
-    Parameters
-    ----------
-    path : str
-        file system path string
-
-    Returns
-    -------
-    bool
-        True if writeable, otherwise raises PermissionError
-    """
-    try:
-        if path.endswith("\\") or path.endswith("/"):
-            path = os.path.join(path, ".torrent")
-        with open(path, "ab") as _:
-            pass
-        os.remove(path)
-    except PermissionError as err:  # pragma: nocover
-        directory = os.path.dirname(path)
-        message = f"Target directory is not writeable {directory}"
-        raise PermissionError(message) from err
-    return True
+#! /usr/bin/python3
+# -*- coding: utf-8 -*-
+
+##############################################################################
+#    Copyright (C) 2021-current alexpdev
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+##############################################################################
+"""
+Utility functions and classes used throughout package.
+"""
+
+import os
+import math
+import shutil
+from pathlib import Path
+
+
+class Memo:
+    """
+    Memoize cache.
+
+    Parameters
+    ----------
+    func : Callable
+        The results of this callable will be cached.
+    """
+
+    def __init__(self, func):
+        """
+        Construcor for cache.
+        """
+        self.func = func
+        self.counter = 0
+        self.cache = {}
+
+    def __call__(self, path: str):
+        """
+        Invoke each time memo function is called.
+
+        Parameters
+        ----------
+        path : str
+            The relative or absolute path being used as key in cache dict.
+
+        Returns
+        -------
+        Any :
+            The results of calling the function with path.
+        """
+        if path in self.cache and os.path.exists(path):
+            self.counter += 1
+            return self.cache[path]
+        result = self.func(path)
+        self.cache[path] = result
+        return result
+
+
+class MissingPathError(Exception):
+    """
+    Path parameter is required to specify target content.
+
+    Creating a .torrent file with no contents seems rather silly.
+
+    Parameters
+    ----------
+    message : str
+        Message for user (optional).
+    """
+
+    def __init__(self, message: str = None):
+        """
+        Raise when creating a meta file without specifying target content.
+
+        The `message` argument is a message to pass to Exception base class.
+        """
+        self.message = f"Path arguement is missing and required {str(message)}"
+        super().__init__(message)
+
+
+class PieceLengthValueError(Exception):
+    """
+    Piece Length parameter must equal a perfect power of 2.
+
+    Parameters
+    ----------
+    message : str
+        Message for user (optional).
+    """
+
+    def __init__(self, message: str = None):
+        """
+        Raise when creating a meta file with incorrect piece length value.
+
+        The `message` argument is a message to pass to Exception base class.
+        """
+        self.message = f"Incorrect value for piece length: {str(message)}"
+        super().__init__(message)
+
+
+class ArgumentError(Exception):
+    """
+    Exception for mismatched or mistyped CLI arguments.
+    """
+
+
+SUFFIXES = ["KiB", "MiB", "GiB", "TiB", "PiB", "EiB", "ZiB", "YiB"]
+
+
+def humanize_bytes(amount: int) -> str:
+    """
+    Convert integer into human readable memory sized denomination.
+
+    Parameters
+    ----------
+    amount : int
+        total number of bytes.
+
+    Returns
+    -------
+    str
+        human readable representation of the given amount of bytes.
+    """
+    base = 1024
+    amount = float(amount)
+    value = abs(amount)
+    if value == 1:
+        return f"{amount} Byte"
+    if value < base:
+        return f"{amount} Bytes"
+    for i, s in enumerate(SUFFIXES):
+        unit = base**(i + 2)
+        if value < unit:
+            break
+    value = base * amount / unit
+    return f"{value:.1f} {s}"
+
+
+def normalize_piece_length(piece_length: int) -> int:
+    """
+    Verify input piece_length is valid and convert accordingly.
+
+    Parameters
+    ----------
+    piece_length : int | str
+        The piece length provided by user.
+
+    Returns
+    -------
+    int
+        normalized piece length.
+
+    Raises
+    ------
+    PieceLengthValueError :
+        Piece length is improper value.
+    """
+    if isinstance(piece_length, str):
+        if piece_length.isnumeric():
+            piece_length = int(piece_length)
+        else:
+            raise PieceLengthValueError(piece_length)
+
+    if piece_length > (1 << 14):
+        if 2**math.log2(piece_length) == piece_length:
+            return piece_length
+        raise PieceLengthValueError(piece_length)
+
+    if 13 < piece_length < 26:
+        return 2**piece_length
+    if piece_length <= 13:
+        raise PieceLengthValueError(piece_length)
+
+    log = int(math.log2(piece_length))
+    if 2**log == piece_length:
+        return piece_length
+    raise PieceLengthValueError
+
+
+def get_piece_length(size: int) -> int:
+    """
+    Calculate the ideal piece length for bittorrent data.
+
+    Parameters
+    ----------
+    size : int
+        Total bits of all files incluided in .torrent file.
+
+    Returns
+    -------
+    int
+        Ideal piece length.
+    """
+    exp = 14
+    while size / (2**exp) > 1000 and exp < 24:
+        exp += 1
+    return 2**exp
+
+
+@Memo
+def filelist_total(pathstring: str) -> os.PathLike:
+    """
+    Perform error checking and format conversion to os.PathLike.
+
+    Parameters
+    ----------
+    pathstring : str
+        An existing filesystem path.
+
+    Returns
+    -------
+    os.PathLike
+        Input path converted to bytes format.
+
+    Raises
+    ------
+    MissingPathError
+        File could not be found.
+    """
+    if os.path.exists(pathstring):
+        path = Path(pathstring)
+        return _filelist_total(path)
+    raise MissingPathError
+
+
+def _filelist_total(path: os.PathLike) -> tuple:
+    """
+    Recursively search directory tree for files.
+
+    Parameters
+    ----------
+    path : str
+        Path to file or directory base
+
+    Returns
+    -------
+    Tuple[int, List] :
+        int - sum of sizes for all files collected
+        list - all file paths within directory tree
+    """
+    if path.is_file():
+        file_size = os.path.getsize(path)
+        return file_size, [str(path)]
+    total = 0
+    filelist = []
+    if path.is_dir():
+        for item in path.iterdir():
+            size, paths = filelist_total(item)
+            total += size
+            filelist.extend(paths)
+    return total, sorted(filelist)
+
+
+def path_size(path: str) -> int:
+    """
+    Return the total size of all files in path recursively.
+
+    Parameters
+    ----------
+    path : str
+        path to target file or directory.
+
+    Returns
+    -------
+    int
+        total size of files.
+    """
+    total_size, _ = filelist_total(path)
+    return total_size
+
+
+def get_file_list(path: str) -> list:
+    """
+    Return a sorted list of file paths contained in directory.
+
+    Parameters
+    ----------
+    path : str
+        target file or directory.
+
+    Returns
+    -------
+    list :
+        sorted list of file paths.
+    """
+    _, filelist = filelist_total(path)
+    return filelist
+
+
+def path_stat(path: str) -> tuple:
+    """
+    Calculate directory statistics.
+
+    Parameters
+    ----------
+    path : str
+        The path to start calculating from.
+
+    Returns
+    -------
+    Tuple[list, int, int] :
+        list - List of all files contained in Directory
+        int - Total sum of bytes from all contents of dir
+        int - The size of pieces of the torrent contents.
+    """
+    total_size, filelist = filelist_total(path)
+    piece_length = get_piece_length(total_size)
+    return (filelist, total_size, piece_length)
+
+
+def path_piece_length(path: str) -> int:
+    """
+    Calculate piece length for input path and contents.
+
+    Parameters
+    ----------
+    path : str
+        The absolute path to directory and contents.
+
+    Returns
+    -------
+    int
+        The size of pieces of torrent content.
+    """
+    psize = path_size(path)
+    return get_piece_length(psize)
+
+
+def next_power_2(value: int) -> int:
+    """
+    Calculate the next perfect power of 2 equal to or greater than value.
+
+    Parameters
+    ----------
+    value : int
+        integer value that is less than some perfect power of 2.
+
+    Returns
+    -------
+    int
+        The next power of 2 greater than value, or value if already power of 2.
+    """
+    if not value & (value - 1) and value:
+        return value
+    start = 1
+    while start < value:
+        start <<= 1
+    return start
+
+
+def copypath(source: str, dest: str) -> None:
+    """
+    Copy the file located at source to dest.
+
+    If one or more directory paths don't exist in dest, they will be created.
+    If dest already exists and dest and source are the same size, it will be
+    ignored, however if dest is smaller than source, dest will be overwritten.
+
+    Parameters
+    ----------
+    source : str
+        path to source file
+    dest : str
+        path to target destination
+    """
+    if not os.path.exists(source) or (os.path.exists(dest)
+                                      and os.path.getsize(source)
+                                      <= os.path.getsize(dest)):
+        return
+    path_parts = Path(dest).parts
+    if len(path_parts) > 1:
+        root = path_parts[0]
+        path_parts = path_parts[1:-1]
+        if not os.path.exists(root):
+            os.mkdir(root)  # pragma: nocover
+        for part in path_parts:
+            path = os.path.join(root, part)
+            if not os.path.exists(path):
+                os.mkdir(path)
+            root = path
+        shutil.copy(source, dest)
+
+
+def toggle_debug_mode(switch_on: bool):
+    """
+    Switch the environment variable debug indicator on or off.
+
+    Parameters
+    ----------
+    switch_on : bool
+        if true turn debug mode on otherwise off
+    """
+    os.environ["TORRENTFILE_DEBUG"] = "ON" if switch_on else "OFF"
+
+
+def debug_is_on() -> bool:
+    """
+    Return True if debug mode is on in environment variables.
+
+    Returns
+    -------
+    bool
+        is debug mode on
+    """
+    return os.environ["TORRENTFILE_DEBUG"] == "ON"
+
+
+def check_path_writable(path: str) -> bool:
+    """
+    Test if output path is writable.
+
+    Parameters
+    ----------
+    path : str
+        file system path string
+
+    Returns
+    -------
+    bool
+        True if writeable, otherwise raises PermissionError
+    """
+    try:
+        if path.endswith("\\") or path.endswith("/"):
+            path = os.path.join(path, ".torrent")
+        with open(path, "ab") as _:
+            pass
+        os.remove(path)
+    except PermissionError as err:  # pragma: nocover
+        directory = os.path.dirname(path)
+        message = f"Target directory is not writeable {directory}"
+        raise PermissionError(message) from err
+    return True
```

### Comparing `torrentfile-0.9.0/torrentfile/version.py` & `torrentfile-0.9.1/torrentfile/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 ##############################################################################
 """
 Holds the release version number.
 """
 
-__version__ = "0.9.0"
+__version__ = "0.9.1"
```

### Comparing `torrentfile-0.9.0/torrentfile.egg-info/PKG-INFO` & `torrentfile-0.9.1/torrentfile.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torrentfile
-Version: 0.9.0
+Version: 0.9.1
 Summary: Terminal based command line tool for creating Bittorrent files.
 Author-email: alexpdev <alexpdev@pm.me>
 Project-URL: homepage, https://github.com/alexpdev/torrentfile
 Project-URL: repository, https://github.com
 Project-URL: documentation, https://alexpdev.github.io/torrentfile
 Project-URL: changelog, https://alexpdev.github.io/torrentfile/changelog/
 Project-URL: issues, https://github.com/alexpdev/torrentfile/issues
@@ -44,25 +44,25 @@
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/b67ff65b3d574025b65b6587266bbab7)](https://www.codacy.com/gh/alexpdev/torrentfile/dashboard?utm_source=github.com&utm_medium=referral&utm_content=alexpdev/torrentfile&utm_campaign=Badge_Coverage)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/b67ff65b3d574025b65b6587266bbab7)](https://www.codacy.com/gh/alexpdev/torrentfile/dashboard?utm_source=github.com&utm_medium=referral&utm_content=alexpdev/torrentfile&utm_campaign=Badge_Grade)
 [![DeepSource](https://deepsource.io/gh/alexpdev/TorrentFile.svg/?label=active+issues&token=16Sl_dF7nTU8YgPilcqhvHm8)](https://deepsource.io/gh/alexpdev/torrentfile/)
 [![codecov](https://codecov.io/gh/alexpdev/torrentfile/branch/master/graph/badge.svg?token=EWF7NIL9SQ)](https://codecov.io/gh/alexpdev/torrentfile?color=navy&logo=codecov)
 
 ## 🌐 Overview
 
-A command line interface for creating, reviewing, editing, or verifying bittorrent meta files (`.torrent` files). 
+A command line interface for creating, reviewing, editing, or verifying bittorrent meta files (`.torrent` files).
 _`torrentfile`_ is open source, and supports all versions of Bittorrent files, including hybrid meta files. The code base
 is also importable and can easily be used as a library for creating or manipulating torrent files in external projects.
 Documentation is available at [https://alexpdev.github.io/torrentfile](https://alexpdev.github.io/torrentfile).
 
 > A GUI frontend for this project can be found at <https://github.com/alexpdev/TorrentfileQt>
 
 ## 🔌 Requirements
 
--   Python 3.6+
--   Tested on Linux, Windows and Mac
+- Python 3.6+
+- Tested on Linux, Windows and Mac
 
 ## 💻 Install
 
 **PyPi:**
 
 ```bash
 pip install torrentfile
@@ -91,32 +91,29 @@
 ## 📝 License
 
 Apache Software License v2.0 - See [LICENSE]("https://github.com/alexpdev/torrentfile/blob/master/LICENSE")
 
 ## 💡 Issues & Requests & PRs
 
 If you encounter any bugs or would like to request a new feature please open a new issue.
-
-> PRs and other contributions are welcome
-
-<https://github.com/alexpdev/torrentfile/issues>
+PRs and other contributions that are meaningful and add value to the project are welcome.
 
 * * *
 
 ## Usage Examples
 
 ### Creating Bittorrent Files
 
 Creating a basic torrent file is as easy as using the create subcommand with the path to the torrent file.
 
 ```bash
 torrentfile create /path/to/content
 ```
 
-You can add one or more trackers by using any one of `-a`, `--announce` 
+You can add one or more trackers by using any one of `-a`, `--announce`
 flags and listing their URL as a space separated list.
 
 ```bash
 torrentfile create /path/to/content -a http://tracker1.com http://tracker2.net
 ```
 
 If you intend to distribute the file on a private tracker then you should use one  
@@ -128,18 +125,14 @@
 ```
 
 By default **`torrentfile`** displays a progress bar indicating how much of the content  
 has already been processed.  To turn off this display you can either use `--quiet` mode in  
 as a global flag or you can set the `--prog` flag to 0.
 
 ```bash
-torrentfile --quiet create /path/to/content
-```
-
-```bash
 torrentfile create /path/to/content --prog 0
 ```
 
 **`torrentfile`** extracts the name of the contents top level file or directory  
 and saves the torrent file to the current working directory with the extracted title.
 
 For example running the follwing command would create `./content.torrent`.
@@ -160,38 +153,37 @@
 
 For example the following command would create a torrent file at `/some/other/path/content.torrent`.
 
 ```bash
 torrentfile create /path/to/content -o /some/other/path/
 ```
 
-Bittorrent protocol V1 is still the most commonly used version, therefore _`torrentfile`_ creates
-Bittorrent version 1 torrent files by default. To specify creating a V2 file or hybrid (v1 and v2)
-use the `--meta-version` followed by the specific version number format to use.  The options include:
-`1`(v1 default), `2`(v2), or `3`(v1 & v2).
+_`torrentfile`_ creates Bittorrent v1 files by default. To create a V2 or hybrid (v1 and v2)
+torrent file, use the `--meta-version` option followed by the preferred version number option.
+The options include:  `1`(v1 default), `2`(v2), or `3`(v1 & v2).
 
 ```bash
 torrentfile create /path/to/content --meta-version 2
 ```
 
 ```bash
 torrentfile create /path/to/content --meta-version 3 
 ```
 
->`torrentfile` now includes the option to command line flags for the `create` sub-command from an `ini` style
+`torrentfile` includes the option to command line flags for the `create` sub-command from an `ini` style
 configuration file, by using the `--config` and optional `--config-path` options to specify the path
 to the configuration file.  If `--config-path` is ommited, then `torrentfile` will look by default in the current
-working directory for a file named `torrentfile.ini`. If the file is not discovered in the current working directory, 
-it will move on to look `~/.torrentfile/torrentfile.ini` followed by `~/.config/torrentfile.ini`.  Please see the 
+working directory for a file named `torrentfile.ini`. If the file is not discovered in the current working directory,
+it will move on to look `~/.torrentfile/torrentfile.ini` followed by `~/.config/torrentfile.ini`.  Please see the
 [documentation](https://alexpdev.github.io/torrentfile/overview/) for more details on how the configuration file should be
 formatted.
 
 ### Check/Recheck Torrent
 
-The `recheck` subcommand allows you to scan a Bittorrent file and compare it's contents, 
+The `recheck` subcommand allows you to scan a Bittorrent file and compare it's contents,
 against a file or directory containing the contents the torrent file was created from.
 The output provided by this process gives a detailed perspective if any files are missing
 or have been corrupted in any way.  Supports any version of Bittorrent file.
 
 ```bash
 torrentfile recheck /path/to/some.torrent /path/to/content
 ```
@@ -211,15 +203,15 @@
 ```bash
 torrentfile edit -h
 ```
 
 ### Create Magnet
 
 To create a magnet URI for a pre-existing torrent meta file, use the sub-command  
-`magnet` or `m` with the path to the torrent file.
+`magnet` with the path to the torrent file.
 
 ```bash
 torrentfile magnet /path/to/some.torrent
 ```
 
 ### GUI
```

### Comparing `torrentfile-0.9.0/torrentfile.egg-info/SOURCES.txt` & `torrentfile-0.9.1/torrentfile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torrentfile-0.9.0/tox.ini` & `torrentfile-0.9.1/tox.ini`

 * *Files identical despite different names*

