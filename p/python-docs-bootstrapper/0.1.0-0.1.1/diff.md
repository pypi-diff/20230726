# Comparing `tmp/python-docs-bootstrapper-0.1.0.tar.gz` & `tmp/python-docs-bootstrapper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-docs-bootstrapper-0.1.0.tar", last modified: Wed Jul 26 07:31:34 2023, max compression
+gzip compressed data, was "python-docs-bootstrapper-0.1.1.tar", last modified: Wed Jul 26 18:32:18 2023, max compression
```

## Comparing `python-docs-bootstrapper-0.1.0.tar` & `python-docs-bootstrapper-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 07:31:34.288237 python-docs-bootstrapper-0.1.0/
--rw-rw-rw-   0        0        0     1087 2023-07-26 07:30:50.000000 python-docs-bootstrapper-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1714 2023-07-26 07:31:34.288237 python-docs-bootstrapper-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      614 2023-07-26 07:30:50.000000 python-docs-bootstrapper-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 07:31:34.241338 python-docs-bootstrapper-0.1.0/bootstrapper/
--rw-rw-rw-   0        0        0       40 2023-07-26 07:30:50.000000 python-docs-bootstrapper-0.1.0/bootstrapper/__init__.py
--rw-rw-rw-   0        0        0     5667 2023-07-25 17:07:37.000000 python-docs-bootstrapper-0.1.0/bootstrapper/bootstrapper.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:31:34.256988 python-docs-bootstrapper-0.1.0/bootstrapper/data/
--rw-rw-rw-   0        0        0      117 2023-07-25 15:10:26.000000 python-docs-bootstrapper-0.1.0/bootstrapper/data/.gitignore
--rw-rw-rw-   0        0        0     4707 2023-07-25 17:02:29.000000 python-docs-bootstrapper-0.1.0/bootstrapper/data/Makefile
--rw-rw-rw-   0        0        0     1847 2023-07-26 07:30:50.000000 python-docs-bootstrapper-0.1.0/bootstrapper/data/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 07:31:34.288237 python-docs-bootstrapper-0.1.0/python_docs_bootstrapper.egg-info/
--rw-rw-rw-   0        0        0     1714 2023-07-26 07:31:34.000000 python-docs-bootstrapper-0.1.0/python_docs_bootstrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-07-26 07:31:34.000000 python-docs-bootstrapper-0.1.0/python_docs_bootstrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 07:31:34.000000 python-docs-bootstrapper-0.1.0/python_docs_bootstrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-07-26 07:31:34.000000 python-docs-bootstrapper-0.1.0/python_docs_bootstrapper.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-07-26 07:31:34.000000 python-docs-bootstrapper-0.1.0/python_docs_bootstrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-26 07:31:34.000000 python-docs-bootstrapper-0.1.0/python_docs_bootstrapper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 07:31:34.288237 python-docs-bootstrapper-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1807 2023-07-25 16:53:52.000000 python-docs-bootstrapper-0.1.0/setup.py
+drwxrwxr-x   0 egeakman  (1000) egeakman  (1000)        0 2023-07-26 18:32:18.300450 python-docs-bootstrapper-0.1.1/
+-rw-rw-r--   0 egeakman  (1000) egeakman  (1000)     1066 2023-07-25 20:16:28.000000 python-docs-bootstrapper-0.1.1/LICENSE
+-rw-rw-r--   0 egeakman  (1000) egeakman  (1000)     1631 2023-07-26 18:32:18.300450 python-docs-bootstrapper-0.1.1/PKG-INFO
+-rw-rw-r--   0 egeakman  (1000) egeakman  (1000)      584 2023-07-25 19:43:54.000000 python-docs-bootstrapper-0.1.1/README.md
+drwxrwxr-x   0 egeakman  (1000) egeakman  (1000)        0 2023-07-26 18:32:18.300450 python-docs-bootstrapper-0.1.1/bootstrapper/
+-rw-rw-r--   0 egeakman  (1000) egeakman  (1000)       39 2023-07-25 20:17:11.000000 python-docs-bootstrapper-0.1.1/bootstrapper/__init__.py
+-rw-rw-r--   0 egeakman  (1000) egeakman  (1000)     7647 2023-07-26 20:31:44.000000 python-docs-bootstrapper-0.1.1/bootstrapper/bootstrapper.py
+drwxrwxr-x   0 egeakman  (1000) egeakman  (1000)        0 2023-07-26 18:32:18.300450 python-docs-bootstrapper-0.1.1/bootstrapper/data/
+-rw-rw-r--   0 egeakman  (1000) egeakman  (1000)      105 2023-07-25 19:17:07.000000 python-docs-bootstrapper-0.1.1/bootstrapper/data/.gitignore
+-rw-rw-r--   0 egeakman  (1000) egeakman  (1000)     4564 2023-07-25 19:17:07.000000 python-docs-bootstrapper-0.1.1/bootstrapper/data/Makefile
+-rw-rw-r--   0 egeakman  (1000) egeakman  (1000)     1830 2023-07-25 19:34:03.000000 python-docs-bootstrapper-0.1.1/bootstrapper/data/README.md
+drwxrwxr-x   0 egeakman  (1000) egeakman  (1000)        0 2023-07-26 18:32:18.300450 python-docs-bootstrapper-0.1.1/python_docs_bootstrapper.egg-info/
+-rw-rw-r--   0 egeakman  (1000) egeakman  (1000)     1631 2023-07-26 18:32:18.000000 python-docs-bootstrapper-0.1.1/python_docs_bootstrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 egeakman  (1000) egeakman  (1000)      454 2023-07-26 18:32:18.000000 python-docs-bootstrapper-0.1.1/python_docs_bootstrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 egeakman  (1000) egeakman  (1000)        1 2023-07-26 18:32:18.000000 python-docs-bootstrapper-0.1.1/python_docs_bootstrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 egeakman  (1000) egeakman  (1000)       64 2023-07-26 18:32:18.000000 python-docs-bootstrapper-0.1.1/python_docs_bootstrapper.egg-info/entry_points.txt
+-rw-rw-r--   0 egeakman  (1000) egeakman  (1000)       14 2023-07-26 18:32:18.000000 python-docs-bootstrapper-0.1.1/python_docs_bootstrapper.egg-info/requires.txt
+-rw-rw-r--   0 egeakman  (1000) egeakman  (1000)       13 2023-07-26 18:32:18.000000 python-docs-bootstrapper-0.1.1/python_docs_bootstrapper.egg-info/top_level.txt
+-rw-rw-r--   0 egeakman  (1000) egeakman  (1000)       38 2023-07-26 18:32:18.300450 python-docs-bootstrapper-0.1.1/setup.cfg
+-rw-rw-r--   0 egeakman  (1000) egeakman  (1000)     1749 2023-07-26 16:57:18.000000 python-docs-bootstrapper-0.1.1/setup.py
```

### Comparing `python-docs-bootstrapper-0.1.0/LICENSE` & `python-docs-bootstrapper-0.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Ege Akman
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Ege Akman
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `python-docs-bootstrapper-0.1.0/PKG-INFO` & `python-docs-bootstrapper-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-Metadata-Version: 2.1
-Name: python-docs-bootstrapper
-Version: 0.1.0
-Summary: Bootstrapper for Python documentation translations
-Home-page: https://github.com/egeakman/python-docs-bootstrapper
-Download-URL: https://github.com/egeakman/python-docs-bootstrapper/archive/0.1.0.tar.gz
-Author: egeakman
-Author-email: me@egeakman.dev
-License: CC0-1.0
-Project-URL: Homepage, https://github.com/egeakman/python-docs-bootstrapper
-Project-URL: Issues, https://github.com/egeakman/python-docs-bootstrapper/issues
-Keywords: documentation,translation,sphinx,i18n,python-docs,CLI,automation,utilities
-Classifier: Topic :: Utilities
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# python-docs-bootstrapper
-
-This repository contains the scripts and data used to bootstrap a new translation of the Python documentation.
-
-## Installation
-
-```bash
-$ pip install python-docs-bootstrapper
-```
-
-## Usage
-
-```bash
-$ bootstrapper --help
-usage: bootstrapper [-h] [-b BRANCH] language
-
-positional arguments:
-  language              IETF language tag (e.g. tr, pt-br)
-
-options:
-  -h, --help            show this help message and exit
-  -b BRANCH, --branch BRANCH
-                        CPython branch (e.g. 3.12)
-```
-
-## Example
-
-```bash
-$ bootstrapper tr --branch 3.12
-```
+Metadata-Version: 2.1
+Name: python-docs-bootstrapper
+Version: 0.1.1
+Summary: Bootstrapper for Python documentation translations
+Home-page: https://github.com/egeakman/python-docs-bootstrapper
+Download-URL: https://github.com/egeakman/python-docs-bootstrapper/archive/0.1.1.tar.gz
+Author: egeakman
+Author-email: me@egeakman.dev
+License: MIT
+Project-URL: Homepage, https://github.com/egeakman/python-docs-bootstrapper
+Project-URL: Issues, https://github.com/egeakman/python-docs-bootstrapper/issues
+Keywords: documentation,translation,sphinx,i18n,python-docs,CLI,automation,utilities
+Classifier: Topic :: Utilities
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# python-docs-bootstrapper
+
+This repository contains the scripts and data used to bootstrap a new translation of the Python documentation.
+
+## Installation
+
+```bash
+$ pip install python-docs-bootstrapper
+```
+
+## Usage
+
+```bash
+$ bootstrapper --help
+usage: bootstrapper [-h] [-b BRANCH] language
+
+positional arguments:
+  language              IETF language tag (e.g. tr, pt-br)
+
+options:
+  -h, --help            show this help message and exit
+  -b BRANCH, --branch BRANCH
+                        CPython branch (e.g. 3.12)
+```
+
+## Example
+
+```bash
+$ bootstrapper tr --branch 3.12
+```
```

### Comparing `python-docs-bootstrapper-0.1.0/bootstrapper/data/Makefile` & `python-docs-bootstrapper-0.1.1/bootstrapper/data/Makefile`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-# Makefile for {{translation.language}} Python Documentation
-#
-# Here is what you can do:
-#
-# - make  # Automatically build an HTML local version
-# - make todo  # To list remaining tasks and show current progression
-# - make verifs  # To check for correctness: wrapping, spelling
-# - make wrap  # To rewrap modified files
-# - make spell  # To check for spelling
-# - make clean # To remove build artifacts
-# - make fuzzy  # To find fuzzy strings
-#
-# Modes are: autobuild-stable, autobuild-dev, and autobuild-html,
-# documented in gen/src/3.6/Doc/Makefile as we're only delegating the
-# real work to the Python Doc Makefile.
-
-# Configuration
-
-# The CPYTHON_CURRENT_COMMIT is the commit, in the cpython repository,
-# from which we generated our po files.  We use it here so when we
-# test build, we're building with the .rst files that generated our
-# .po files.
-
-CPYTHON_CURRENT_COMMIT := {{translation.head}}
-LANGUAGE := {{translation.language}}
-BRANCH := {{translation.branch}}
-
-EXCLUDED := \
-	whatsnew/2.?.po \
-	whatsnew/3.[0-10].po
-
-# Internal variables
-
-UPSTREAM := https://github.com/python/cpython
-
-PYTHON := $(shell which python3)
-MODE := html
-POSPELL_TMP_DIR := .pospell/
-JOBS := auto
-ADDITIONAL_ARGS := --keep-going --color
-SPHINXERRORHANDLING = -W
-
-# Detect OS
-
-ifeq '$(findstring ;,$(PATH))' ';'
-    detected_OS := Windows
-else
-    detected_OS := $(shell uname 2>/dev/null || echo Unknown)
-    detected_OS := $(patsubst CYGWIN%,Cygwin,$(detected_OS))
-    detected_OS := $(patsubst MSYS%,MSYS,$(detected_OS))
-    detected_OS := $(patsubst MINGW%,MSYS,$(detected_OS))
-endif
-
-ifeq ($(detected_OS),Darwin)        # Mac OS X
-    CP_CMD := gcp                   # accessible with `brew install coreutils` or `brew upgrade coreutils`
-else
-    CP_CMD := cp
-endif
-
-.PHONY: all
-all: ensure_prerequisites
-	git -C venv/cpython checkout $(CPYTHON_CURRENT_COMMIT) || (git -C venv/cpython fetch && git -C venv/cpython checkout $(CPYTHON_CURRENT_COMMIT))
-	mkdir -p locales/$(LANGUAGE)/LC_MESSAGES/
-	$(CP_CMD) -u --parents *.po */*.po locales/$(LANGUAGE)/LC_MESSAGES/
-	$(MAKE) -C venv/cpython/Doc/ \
-	  JOBS='$(JOBS)'             \
-	  SPHINXOPTS='-D locale_dirs=$(abspath locales) \
-	  -D language=$(LANGUAGE)           \
-	  -D gettext_compact=0              \
-	  -D latex_engine=xelatex           \
-	  -D latex_elements.inputenc=       \
-	  -D latex_elements.fontenc=        \
-	  $(ADDITIONAL_ARGS)'               \
-	  SPHINXERRORHANDLING=$(SPHINXERRORHANDLING) \
-	  $(MODE)
-	@echo "Build success, open file://$(abspath venv/cpython/)/Doc/build/html/index.html or run 'make htmlview' to see them."
-
-
-# We clone cpython/ inside venv/ because venv/ is the only directory
-# excluded by cpython' Sphinx configuration.
-venv/cpython/.git/HEAD:
-	git clone https://github.com/python/cpython venv/cpython
-
-
-.PHONY: ensure_prerequisites
-ensure_prerequisites: venv/cpython/.git/HEAD
-	@if ! (blurb help >/dev/null 2>&1 && sphinx-build --version >/dev/null 2>&1); then \
-	    git -C venv/cpython/ checkout $(BRANCH); \
-	    echo "You're missing dependencies please install:"; \
-	    echo ""; \
-	    echo "  python -m pip install -r venv/cpython/Doc/requirements.txt"; \
-	    exit 1; \
-	fi
-
-.PHONY: htmlview
-htmlview: MODE=htmlview
-htmlview: all
-
-.PHONY: todo
-todo: ensure_prerequisites
-	potodo --exclude venv .venv $(EXCLUDED)
-
-.PHONY: wrap
-wrap: ensure_prerequisites
-	@echo "Re wrapping modified files"
-	powrap -m
-
-SRCS = $(shell git diff --name-only $(BRANCH) | grep '.po$$')
-# foo/bar.po => $(POSPELL_TMP_DIR)/foo/bar.po.out
-DESTS = $(addprefix $(POSPELL_TMP_DIR)/,$(addsuffix .out,$(SRCS)))
-
-.PHONY: spell
-spell: ensure_prerequisites $(DESTS)
-
-.PHONY: line-length
-line-length:
-	@echo "Searching for long lines..."
-	@awk '{if (length(gensub(/శ్రీనివాస్/, ".", "g", $$0)) > 80 && length(gensub(/[^ ]/, "", "g")) > 1) {print FILENAME ":" FNR, "line too long:", $$0; ERRORS+=1}} END {if (ERRORS>0) {exit 1}}' *.po */*.po
-
-.PHONY: sphinx-lint
-sphinx-lint:
-	@echo "Checking all files using sphinx-lint..."
-	@sphinx-lint --enable all --disable line-too-long *.po */*.po
-
-$(POSPELL_TMP_DIR)/%.po.out: %.po dict
-	@echo "Pospell checking $<..."
-	@mkdir -p $(@D)
-	pospell -p dict -l tr_TR $< && touch $@
-
-.PHONY: fuzzy
-fuzzy: ensure_prerequisites
-	potodo -f --exclude venv .venv $(EXCLUDED)
-
-.PHONY: verifs
-verifs: spell line-length sphinx-lint
-
-.PHONY: clean
-clean:
-	@echo "Cleaning *.mo and $(POSPELL_TMP_DIR)"
-	rm -rf $(POSPELL_TMP_DIR) locales/$(LANGUAGE)/LC_MESSAGES/
-	find -name '*.mo' -delete
-	@echo "Cleaning build directory"
-	$(MAKE) -C venv/cpython/Doc/ clean
+# Makefile for {{translation.language}} Python Documentation
+#
+# Here is what you can do:
+#
+# - make  # Automatically build an HTML local version
+# - make todo  # To list remaining tasks and show current progression
+# - make verifs  # To check for correctness: wrapping, spelling
+# - make wrap  # To rewrap modified files
+# - make spell  # To check for spelling
+# - make clean # To remove build artifacts
+# - make fuzzy  # To find fuzzy strings
+#
+# Modes are: autobuild-stable, autobuild-dev, and autobuild-html,
+# documented in gen/src/3.6/Doc/Makefile as we're only delegating the
+# real work to the Python Doc Makefile.
+
+# Configuration
+
+# The CPYTHON_CURRENT_COMMIT is the commit, in the cpython repository,
+# from which we generated our po files.  We use it here so when we
+# test build, we're building with the .rst files that generated our
+# .po files.
+
+CPYTHON_CURRENT_COMMIT := {{translation.head}}
+LANGUAGE := {{translation.language}}
+BRANCH := {{translation.branch}}
+
+EXCLUDED := \
+	whatsnew/2.?.po \
+	whatsnew/3.[0-10].po
+
+# Internal variables
+
+UPSTREAM := https://github.com/python/cpython
+
+PYTHON := $(shell which python3)
+MODE := html
+POSPELL_TMP_DIR := .pospell/
+JOBS := auto
+ADDITIONAL_ARGS := --keep-going --color
+SPHINXERRORHANDLING = -W
+
+# Detect OS
+
+ifeq '$(findstring ;,$(PATH))' ';'
+    detected_OS := Windows
+else
+    detected_OS := $(shell uname 2>/dev/null || echo Unknown)
+    detected_OS := $(patsubst CYGWIN%,Cygwin,$(detected_OS))
+    detected_OS := $(patsubst MSYS%,MSYS,$(detected_OS))
+    detected_OS := $(patsubst MINGW%,MSYS,$(detected_OS))
+endif
+
+ifeq ($(detected_OS),Darwin)        # Mac OS X
+    CP_CMD := gcp                   # accessible with `brew install coreutils` or `brew upgrade coreutils`
+else
+    CP_CMD := cp
+endif
+
+.PHONY: all
+all: ensure_prerequisites
+	git -C venv/cpython checkout $(CPYTHON_CURRENT_COMMIT) || (git -C venv/cpython fetch && git -C venv/cpython checkout $(CPYTHON_CURRENT_COMMIT))
+	mkdir -p locales/$(LANGUAGE)/LC_MESSAGES/
+	$(CP_CMD) -u --parents *.po */*.po locales/$(LANGUAGE)/LC_MESSAGES/
+	$(MAKE) -C venv/cpython/Doc/ \
+	  JOBS='$(JOBS)'             \
+	  SPHINXOPTS='-D locale_dirs=$(abspath locales) \
+	  -D language=$(LANGUAGE)           \
+	  -D gettext_compact=0              \
+	  -D latex_engine=xelatex           \
+	  -D latex_elements.inputenc=       \
+	  -D latex_elements.fontenc=        \
+	  $(ADDITIONAL_ARGS)'               \
+	  SPHINXERRORHANDLING=$(SPHINXERRORHANDLING) \
+	  $(MODE)
+	@echo "Build success, open file://$(abspath venv/cpython/)/Doc/build/html/index.html or run 'make htmlview' to see them."
+
+
+# We clone cpython/ inside venv/ because venv/ is the only directory
+# excluded by cpython' Sphinx configuration.
+venv/cpython/.git/HEAD:
+	git clone https://github.com/python/cpython venv/cpython
+
+
+.PHONY: ensure_prerequisites
+ensure_prerequisites: venv/cpython/.git/HEAD
+	@if ! (blurb help >/dev/null 2>&1 && sphinx-build --version >/dev/null 2>&1); then \
+	    git -C venv/cpython/ checkout $(BRANCH); \
+	    echo "You're missing dependencies please install:"; \
+	    echo ""; \
+	    echo "  python -m pip install -r venv/cpython/Doc/requirements.txt"; \
+	    exit 1; \
+	fi
+
+.PHONY: htmlview
+htmlview: MODE=htmlview
+htmlview: all
+
+.PHONY: todo
+todo: ensure_prerequisites
+	potodo --exclude venv .venv $(EXCLUDED)
+
+.PHONY: wrap
+wrap: ensure_prerequisites
+	@echo "Re wrapping modified files"
+	powrap -m
+
+SRCS = $(shell git diff --name-only $(BRANCH) | grep '.po$$')
+# foo/bar.po => $(POSPELL_TMP_DIR)/foo/bar.po.out
+DESTS = $(addprefix $(POSPELL_TMP_DIR)/,$(addsuffix .out,$(SRCS)))
+
+.PHONY: spell
+spell: ensure_prerequisites $(DESTS)
+
+.PHONY: line-length
+line-length:
+	@echo "Searching for long lines..."
+	@awk '{if (length(gensub(/శ్రీనివాస్/, ".", "g", $$0)) > 80 && length(gensub(/[^ ]/, "", "g")) > 1) {print FILENAME ":" FNR, "line too long:", $$0; ERRORS+=1}} END {if (ERRORS>0) {exit 1}}' *.po */*.po
+
+.PHONY: sphinx-lint
+sphinx-lint:
+	@echo "Checking all files using sphinx-lint..."
+	@sphinx-lint --enable all --disable line-too-long *.po */*.po
+
+$(POSPELL_TMP_DIR)/%.po.out: %.po dict
+	@echo "Pospell checking $<..."
+	@mkdir -p $(@D)
+	pospell -p dict -l tr_TR $< && touch $@
+
+.PHONY: fuzzy
+fuzzy: ensure_prerequisites
+	potodo -f --exclude venv .venv $(EXCLUDED)
+
+.PHONY: verifs
+verifs: spell line-length sphinx-lint
+
+.PHONY: clean
+clean:
+	@echo "Cleaning *.mo and $(POSPELL_TMP_DIR)"
+	rm -rf $(POSPELL_TMP_DIR) locales/$(LANGUAGE)/LC_MESSAGES/
+	find -name '*.mo' -delete
+	@echo "Cleaning build directory"
+	$(MAKE) -C venv/cpython/Doc/ clean
```

### Comparing `python-docs-bootstrapper-0.1.0/bootstrapper/data/README.md` & `python-docs-bootstrapper-0.1.1/bootstrapper/data/README.md`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# python-docs-{{translation.language}}
-
-Hello! This is the repository of the {{translation.language}} translation of the Python documentation.
-
-You can refer to the following resources throughout this journey:
-
-- [DevGuide Translating Section](https://devguide.python.org/documentation/translating/) (add your translation to the list!)
-- [PEP 545](https://www.python.org/dev/peps/pep-0545/) (the PEP that describes the translation process)
-- [Other Translations](https://github.com/orgs/python/repositories?q=python-docs) (see how other translations are doing it)
-- [Python Docs Discord Server](https://discord.com/invite/sMWqvzXvde) (especially the `#translations` channel)
-
-## Documentation Contribution Agreement
-Python's documentation is maintained using a global network of volunteers. By posting this project on Transifex, Github, and other public places, and inviting you to participate, we are proposing an agreement that you will provide your improvements to Python's documentation or the translation of Python's documentation for the PSF's use under the CC0 license (available at https://creativecommons.org/publicdomain/zero/1.0/legalcode). In return, you may publicly claim credit for the portion of the translation you contributed and if your translation is accepted by the PSF, you may (but are not required to) submit a patch including an appropriate annotation in the Misc/ACKS or TRANSLATORS file. Although nothing in this Documentation Contribution Agreement obligates the PSF to incorporate your textual contribution, your participation in the Python community is welcomed and appreciated.
-
-You signify acceptance of this agreement by submitting your work to the PSF for inclusion in the documentation.
-
-**Do not forget to replace this file with your own README that describes your translation and community!**
+# python-docs-{{translation.language}}
+
+Hello! This is the repository of the {{translation.language}} translation of the Python documentation.
+
+You can refer to the following resources throughout this journey:
+
+- [DevGuide Translating Section](https://devguide.python.org/documentation/translating/) (add your translation to the list!)
+- [PEP 545](https://www.python.org/dev/peps/pep-0545/) (the PEP that describes the translation process)
+- [Other Translations](https://github.com/orgs/python/repositories?q=python-docs) (see how other translations are doing it)
+- [Python Docs Discord Server](https://discord.com/invite/sMWqvzXvde) (especially the `#translations` channel)
+
+## Documentation Contribution Agreement
+Python's documentation is maintained using a global network of volunteers. By posting this project on Transifex, Github, and other public places, and inviting you to participate, we are proposing an agreement that you will provide your improvements to Python's documentation or the translation of Python's documentation for the PSF's use under the CC0 license (available at https://creativecommons.org/publicdomain/zero/1.0/legalcode). In return, you may publicly claim credit for the portion of the translation you contributed and if your translation is accepted by the PSF, you may (but are not required to) submit a patch including an appropriate annotation in the Misc/ACKS or TRANSLATORS file. Although nothing in this Documentation Contribution Agreement obligates the PSF to incorporate your textual contribution, your participation in the Python community is welcomed and appreciated.
+
+You signify acceptance of this agreement by submitting your work to the PSF for inclusion in the documentation.
+
+**Do not forget to replace this file with your own README that describes your translation and community!**
```

### Comparing `python-docs-bootstrapper-0.1.0/python_docs_bootstrapper.egg-info/PKG-INFO` & `python-docs-bootstrapper-0.1.1/python_docs_bootstrapper.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-Metadata-Version: 2.1
-Name: python-docs-bootstrapper
-Version: 0.1.0
-Summary: Bootstrapper for Python documentation translations
-Home-page: https://github.com/egeakman/python-docs-bootstrapper
-Download-URL: https://github.com/egeakman/python-docs-bootstrapper/archive/0.1.0.tar.gz
-Author: egeakman
-Author-email: me@egeakman.dev
-License: CC0-1.0
-Project-URL: Homepage, https://github.com/egeakman/python-docs-bootstrapper
-Project-URL: Issues, https://github.com/egeakman/python-docs-bootstrapper/issues
-Keywords: documentation,translation,sphinx,i18n,python-docs,CLI,automation,utilities
-Classifier: Topic :: Utilities
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# python-docs-bootstrapper
-
-This repository contains the scripts and data used to bootstrap a new translation of the Python documentation.
-
-## Installation
-
-```bash
-$ pip install python-docs-bootstrapper
-```
-
-## Usage
-
-```bash
-$ bootstrapper --help
-usage: bootstrapper [-h] [-b BRANCH] language
-
-positional arguments:
-  language              IETF language tag (e.g. tr, pt-br)
-
-options:
-  -h, --help            show this help message and exit
-  -b BRANCH, --branch BRANCH
-                        CPython branch (e.g. 3.12)
-```
-
-## Example
-
-```bash
-$ bootstrapper tr --branch 3.12
-```
+Metadata-Version: 2.1
+Name: python-docs-bootstrapper
+Version: 0.1.1
+Summary: Bootstrapper for Python documentation translations
+Home-page: https://github.com/egeakman/python-docs-bootstrapper
+Download-URL: https://github.com/egeakman/python-docs-bootstrapper/archive/0.1.1.tar.gz
+Author: egeakman
+Author-email: me@egeakman.dev
+License: MIT
+Project-URL: Homepage, https://github.com/egeakman/python-docs-bootstrapper
+Project-URL: Issues, https://github.com/egeakman/python-docs-bootstrapper/issues
+Keywords: documentation,translation,sphinx,i18n,python-docs,CLI,automation,utilities
+Classifier: Topic :: Utilities
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# python-docs-bootstrapper
+
+This repository contains the scripts and data used to bootstrap a new translation of the Python documentation.
+
+## Installation
+
+```bash
+$ pip install python-docs-bootstrapper
+```
+
+## Usage
+
+```bash
+$ bootstrapper --help
+usage: bootstrapper [-h] [-b BRANCH] language
+
+positional arguments:
+  language              IETF language tag (e.g. tr, pt-br)
+
+options:
+  -h, --help            show this help message and exit
+  -b BRANCH, --branch BRANCH
+                        CPython branch (e.g. 3.12)
+```
+
+## Example
+
+```bash
+$ bootstrapper tr --branch 3.12
+```
```

